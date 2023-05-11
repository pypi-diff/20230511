# Comparing `tmp/pg_bulk_ingest-0.0.3.tar.gz` & `tmp/pg_bulk_ingest-0.0.4.tar.gz`

## Comparing `pg_bulk_ingest-0.0.3.tar` & `pg_bulk_ingest-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.3/pg_bulk_ingest.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.3/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.3/LICENSE
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.3/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.4/pg_bulk_ingest.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.4/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.4/PKG-INFO
```

### Comparing `pg_bulk_ingest-0.0.3/pg_bulk_ingest.py` & `pg_bulk_ingest-0.0.4/pg_bulk_ingest.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,86 @@
 def upsert(conn, metadata, rows):
 
     def bind_identifiers(query_str, *identifiers):
         return sa.text(sql.SQL(query_str).format(
             *(sql.Identifier(identifier) for identifier in identifiers)
         ).as_string(conn.connection.driver_connection))
 
+    def to_file_like_obj(iterable, base):
+        chunk = base()
+        offset = 0
+        it = iter(iterable)
+
+        def up_to_iter(size):
+            nonlocal chunk, offset
+
+            while size:
+                if offset == len(chunk):
+                    try:
+                        chunk = next(it)
+                    except StopIteration:
+                        break
+                    else:
+                        offset = 0
+                to_yield = min(size, len(chunk) - offset)
+                offset = offset + to_yield
+                size -= to_yield
+                yield chunk[offset - to_yield : offset]
+
+        class FileLikeObj(IOBase):
+            def readable(self):
+                return True
+
+            def read(self, size=-1):
+                return base().join(
+                    up_to_iter(float('inf') if size is None or size < 0 else size)
+                )
+
+        return FileLikeObj()
+
+    def get_converter(sa_type):
+        if isinstance(sa_type, sa.Integer):
+            return lambda v: (null if v is None else str(int(v)))
+        elif isinstance(sa_type, sa.JSON):
+            return lambda v: (null if v is None else escape_string(json.dumps(v)))
+        elif isinstance(sa_type, sa.ARRAY):
+            return lambda v: (
+                null
+                if v is None
+                else escape_string(
+                    '{'
+                    + (
+                        ','.join(
+                            (
+                                'NULL'
+                                if item is None
+                                else ('"' + escape_array_item(str(item)) + '"')
+                            )
+                            for item in v
+                        )
+                    )
+                    + '}',
+                )
+            )
+        else:
+            return lambda v: (null if v is None else escape_string(str(v)))
+
+    def escape_array_item(text):
+        return text.replace('\\', '\\\\').replace('"', '\\"')
+
+    def escape_string(text):
+        return (
+            text.replace('\\', '\\\\')
+            .replace('\n', '\\n')
+            .replace('\r', '\\r')
+            .replace('\t', '\\t')
+        )
+
+    null = '\\N'
+
     first_table = next(iter(metadata.tables.values()))
     intermediate_tables = tuple(sa.Table(
         uuid.uuid4().hex,
         metadata,
         *(
             sa.Column(column.name, column.type, primary_key=column.primary_key)
             for column in table.columns
@@ -29,20 +101,21 @@
         conn.execute(bind_identifiers('''
             CREATE SCHEMA IF NOT EXISTS {}
         ''', intermediate_table.schema))
     metadata.create_all(conn)
 
     # Insert rows into just the first intermediate table
     first_intermediate_table = intermediate_tables[0]
+    converters = tuple(get_converter(column.type) for column in first_intermediate_table.columns)
     def db_rows():
         for row, table in rows:
             if table is not first_table:
                 continue
-            yield '\t'.join(get_converter(column.type)(field) for (field,column) in zip(row, table.columns))+'\n'
-            
+            yield '\t'.join(converter(value) for (converter,value) in zip(converters, row)) + '\n'
+
     with conn.connection.driver_connection.cursor() as cursor:
         cursor.copy_expert(str(bind_identifiers("COPY {}.{} FROM STDIN", first_intermediate_table.schema, first_intermediate_table.name)), to_file_like_obj(db_rows(), str), size=65536)
 
 
     # Copy from that intermediate table into the main table, using
     # ON CONFLICT to update any existing rows
     insert_query = sql.SQL('''
@@ -58,80 +131,7 @@
         primary_keys=sql.SQL(',').join((sql.Identifier(column.name) for column in first_table.columns if column.primary_key)),
         updates=sql.SQL(',').join(sql.SQL('{} = EXCLUDED.{}').format(sql.Identifier(column.name), sql.Identifier(column.name)) for column in first_table.columns),
     )
     conn.execute(sa.text(insert_query.as_string(conn.connection.driver_connection)))
 
     # Drop the intermediate table
     metadata.drop_all(conn, tables=intermediate_tables)
-
-def to_file_like_obj(iterable, base):
-    chunk = base()
-    offset = 0
-    it = iter(iterable)
-
-    def up_to_iter(size):
-        nonlocal chunk, offset
-
-        while size:
-            if offset == len(chunk):
-                try:
-                    chunk = next(it)
-                except StopIteration:
-                    break
-                else:
-                    offset = 0
-            to_yield = min(size, len(chunk) - offset)
-            offset = offset + to_yield
-            size -= to_yield
-            yield chunk[offset - to_yield : offset]
-
-    class FileLikeObj(IOBase):
-        def readable(self):
-            return True
-
-        def read(self, size=-1):
-            return base().join(
-                up_to_iter(float('inf') if size is None or size < 0 else size)
-            )
-
-    return FileLikeObj()
-
-def get_converter(sa_type):
-    if isinstance(sa_type, sa.Integer):
-        return lambda v: (null if v is None else str(int(v)))
-    elif isinstance(sa_type, sa.JSON):
-        return lambda v: (null if v is None else escape_string(json.dumps(v)))
-    elif isinstance(sa_type, sa.ARRAY):
-        return lambda v: (
-            null
-            if v is None
-            else escape_string(
-                '{'
-                + (
-                    ','.join(
-                        (
-                            'NULL'
-                            if item is None
-                            else ('"' + escape_array_item(str(item)) + '"')
-                        )
-                        for item in v
-                    )
-                )
-                + '}',
-            )
-        )
-    else:
-        return lambda v: (null if v is None else escape_string(str(v)))
-    
-def escape_array_item(text):
-    return text.replace('\\', '\\\\').replace('"', '\\"')
-
-def escape_string(text):
-    return (
-        text.replace('\\', '\\\\')
-        .replace('\n', '\\n')
-        .replace('\r', '\\r')
-        .replace('\t', '\\t')
-    )
-
-null = '\\N'
-
```

### Comparing `pg_bulk_ingest-0.0.3/.gitignore` & `pg_bulk_ingest-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.3/LICENSE` & `pg_bulk_ingest-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.3/README.md` & `pg_bulk_ingest-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.3/pyproject.toml` & `pg_bulk_ingest-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-bulk-ingest"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pg_bulk_ingest-0.0.3/PKG-INFO` & `pg_bulk_ingest-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-bulk-ingest
-Version: 0.0.3
+Version: 0.0.4
 Summary: A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking
 Project-URL: Source, https://github.com/uktrade/pg-bulk-ingest
 Author-email: Department for International Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

