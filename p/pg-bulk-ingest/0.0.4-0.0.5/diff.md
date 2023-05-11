# Comparing `tmp/pg_bulk_ingest-0.0.4.tar.gz` & `tmp/pg_bulk_ingest-0.0.5.tar.gz`

## Comparing `pg_bulk_ingest-0.0.4.tar` & `pg_bulk_ingest-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.4/pg_bulk_ingest.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.4/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.4/LICENSE
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.4/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.5/pg_bulk_ingest.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.5/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.5/PKG-INFO
```

### Comparing `pg_bulk_ingest-0.0.4/pg_bulk_ingest.py` & `pg_bulk_ingest-0.0.5/pg_bulk_ingest.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,30 +82,32 @@
             .replace('\r', '\\r')
             .replace('\t', '\\t')
         )
 
     null = '\\N'
 
     first_table = next(iter(metadata.tables.values()))
+    intermediate_metadata_obj = sa.MetaData()
     intermediate_tables = tuple(sa.Table(
         uuid.uuid4().hex,
-        metadata,
+        intermediate_metadata_obj,
         *(
             sa.Column(column.name, column.type, primary_key=column.primary_key)
             for column in table.columns
         ),
         schema=table.schema
     ) for table in tuple(metadata.tables.values()))
 
     # Create the table and intermediate tables
     for intermediate_table in intermediate_tables:
         conn.execute(bind_identifiers('''
             CREATE SCHEMA IF NOT EXISTS {}
         ''', intermediate_table.schema))
     metadata.create_all(conn)
+    intermediate_metadata_obj.create_all(conn)
 
     # Insert rows into just the first intermediate table
     first_intermediate_table = intermediate_tables[0]
     converters = tuple(get_converter(column.type) for column in first_intermediate_table.columns)
     def db_rows():
         for row, table in rows:
             if table is not first_table:
@@ -130,8 +132,8 @@
         intermediate_table=sql.Identifier(first_intermediate_table.name),      
         primary_keys=sql.SQL(',').join((sql.Identifier(column.name) for column in first_table.columns if column.primary_key)),
         updates=sql.SQL(',').join(sql.SQL('{} = EXCLUDED.{}').format(sql.Identifier(column.name), sql.Identifier(column.name)) for column in first_table.columns),
     )
     conn.execute(sa.text(insert_query.as_string(conn.connection.driver_connection)))
 
     # Drop the intermediate table
-    metadata.drop_all(conn, tables=intermediate_tables)
+    intermediate_metadata_obj.drop_all(conn)
```

### Comparing `pg_bulk_ingest-0.0.4/.gitignore` & `pg_bulk_ingest-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.4/LICENSE` & `pg_bulk_ingest-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.4/README.md` & `pg_bulk_ingest-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.4/pyproject.toml` & `pg_bulk_ingest-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-bulk-ingest"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pg_bulk_ingest-0.0.4/PKG-INFO` & `pg_bulk_ingest-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-bulk-ingest
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking
 Project-URL: Source, https://github.com/uktrade/pg-bulk-ingest
 Author-email: Department for International Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

