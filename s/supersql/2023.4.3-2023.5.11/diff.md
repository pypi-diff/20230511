# Comparing `tmp/supersql-2023.4.3.tar.gz` & `tmp/supersql-2023.5.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supersql-2023.4.3.tar", max compression
+gzip compressed data, was "supersql-2023.5.11.tar", max compression
```

## Comparing `supersql-2023.4.3.tar` & `supersql-2023.5.11.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0     1048 2023-01-20 23:27:04.000000 supersql-2023.4.3/LICENSE.md
--rwxr-xr-x   0        0        0     3014 2023-01-20 23:22:54.000000 supersql-2023.4.3/README.md
--rwxr-xr-x   0        0        0      861 2023-04-23 11:06:22.920837 supersql-2023.4.3/pyproject.toml
--rwxr-xr-x   0        0        0      269 2023-04-22 21:33:45.498403 supersql-2023.4.3/supersql/__init__.py
--rwxr-xr-x   0        0        0        0 2023-01-21 17:07:28.000000 supersql-2023.4.3/supersql/alternate.py
--rwxr-xr-x   0        0        0     3823 2023-04-22 19:22:20.869838 supersql-2023.4.3/supersql/column.py
--rwxr-xr-x   0        0        0      357 2023-04-22 21:47:06.761429 supersql-2023.4.3/supersql/constants.py
--rwxr-xr-x   0        0        0     1178 2023-01-23 01:14:26.000000 supersql-2023.4.3/supersql/core.py
--rwxr-xr-x   0        0        0     8626 2023-04-22 19:04:57.992610 supersql-2023.4.3/supersql/dquery.py
--rwxr-xr-x   0        0        0      518 2023-01-24 18:41:24.000000 supersql-2023.4.3/supersql/helpers.py
--rwxr-xr-x   0        0        0     8593 2023-04-22 19:50:07.215779 supersql-2023.4.3/supersql/query.py
--rwxr-xr-x   0        0        0     1133 2023-04-22 21:31:41.349988 supersql-2023.4.3/supersql/results.py
--rwxr-xr-x   0        0        0     1894 2023-04-22 11:20:09.187343 supersql-2023.4.3/supersql/table.py
--rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 supersql-2023.4.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1048 2023-01-20 23:27:04.000000 supersql-2023.5.11/LICENSE.md
+-rwxr-xr-x   0        0        0     3009 2023-05-11 20:09:51.228205 supersql-2023.5.11/README.md
+-rwxr-xr-x   0        0        0      862 2023-05-11 20:14:14.210680 supersql-2023.5.11/pyproject.toml
+-rwxr-xr-x   0        0        0      269 2023-04-22 21:33:45.498403 supersql-2023.5.11/supersql/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-01-21 17:07:28.000000 supersql-2023.5.11/supersql/alternate.py
+-rwxr-xr-x   0        0        0     3823 2023-04-22 19:22:20.869838 supersql-2023.5.11/supersql/column.py
+-rwxr-xr-x   0        0        0      357 2023-04-22 21:47:06.761429 supersql-2023.5.11/supersql/constants.py
+-rwxr-xr-x   0        0        0     1178 2023-01-23 01:14:26.000000 supersql-2023.5.11/supersql/core.py
+-rwxr-xr-x   0        0        0     8626 2023-04-22 19:04:57.992610 supersql-2023.5.11/supersql/dquery.py
+-rwxr-xr-x   0        0        0      518 2023-01-24 18:41:24.000000 supersql-2023.5.11/supersql/helpers.py
+-rwxr-xr-x   0        0        0     9297 2023-05-11 20:12:40.228866 supersql-2023.5.11/supersql/query.py
+-rwxr-xr-x   0        0        0     1133 2023-04-22 21:31:41.349988 supersql-2023.5.11/supersql/results.py
+-rwxr-xr-x   0        0        0     1894 2023-04-22 11:20:09.187343 supersql-2023.5.11/supersql/table.py
+-rw-r--r--   0        0        0     3710 1970-01-01 00:00:00.000000 supersql-2023.5.11/PKG-INFO
```

### Comparing `supersql-2023.4.3/LICENSE.md` & `supersql-2023.5.11/LICENSE.md`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.3/README.md` & `supersql-2023.5.11/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 
 &nbsp;
 
 
 ### NOTE: Still Very Much In Development
 
 ```sql
-SELECT * FROM customers ORDER BY last_name ASC LIMIT 5
+SELECT * FROM customers ORDER BY last_name DESC LIMIT 5
 ```
 
 
 ```py
 # query.SELECT('*') is the same as query.SELECT() or query.SELECT(customers)
-query.SELECT().FROM(customers).ORDER_BY(-customers.last_name).LIMIT(5)
+query.SELECT().FROM(customers).ORDER_BY(last_name = -1).LIMIT(5)
 ```
 
 &nbsp;
 
 ## Why?
 Let's be honest:
 
@@ -58,15 +58,15 @@
 
 
 # Without table schema discovery/reflection i.e. using strings -- NOT OPTIMAL
 results = query.SELECT(
         'first_name', 'last_name', 'email'
     ).FROM(
         'employees'
-    ).WHERE('email = someone@example.com').execute()
+    ).WHERE(email = 'someone@example.com').execute()
 
 for result in results:
     print(result)
 
 
 # reflect table schema and fields into a python object for easy querying
 emps = query.database.table('employees')
```

### Comparing `supersql-2023.4.3/pyproject.toml` & `supersql-2023.5.11/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supersql"
-version = "2023.4.3"
+version = "2023.5.11"
 description = "Thin wrapper on top of SQL that enables you write SQL code in python easily"
 authors = ["Tersoo Ortserga <codesage@live.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `supersql-2023.4.3/supersql/column.py` & `supersql-2023.5.11/supersql/column.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.3/supersql/core.py` & `supersql-2023.5.11/supersql/core.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.3/supersql/dquery.py` & `supersql-2023.5.11/supersql/dquery.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.3/supersql/helpers.py` & `supersql-2023.5.11/supersql/helpers.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.3/supersql/query.py` & `supersql-2023.5.11/supersql/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """
 """
+from enum import Enum
 from typing import Iterable, List, Tuple, TYPE_CHECKING, TypeVar
 
+from inflection import tableize
+
 from .constants import *
 from .column import Column
 from .results import Rows
 from .table import Table
 
 
 if TYPE_CHECKING: from supersql import Supersql  # pragma: no cover
@@ -24,38 +27,46 @@
 
     def __str__(self) -> str:
         sql = ' '.join(s() for s in self._sql)
         return sql
     
     def _clone(self):
         this = Query(self._engine)
-        this._sql = self._sql
+        this._sql = [s for s in self._sql]
+        this._args = [a for a in self._args]
         return this
 
     def _conditional(self, condition: Column, param: any, command: str):
         if(isinstance(condition, str)):
             if not param:
                 raise ValueError('''
                     To prevent SQL Injection please use parameterized query with string
                     or use Supersql <type, 'Column'> syntax.
                 ''')
         elif not isinstance(condition, Column):
             raise ValueError(f'''
                 Supersql {command} command only accepts <type, 'Column'> or a parameterized
                 string and param second argument.
             ''')
+
+        if isinstance(condition, str):
+            self._args.append(Column.QUOTE(param))
+        else:
+            self._args.append(condition._arg)
+
+        this = self._clone()
         def _():
             # NOTE: self inside here is self of original query i.e. complete closure every time it is called it appends again
             if isinstance(condition, str):
-                self._args.append(Column.QUOTE(param))
+                # this._args.append(Column.QUOTE(param))
                 sql = f'{command} {condition}'
             else:
-                self._args.append(condition._arg)
-                arguments = len(self._args)
-                vendor = self._engine._vendor
+                # this._args.append(condition._arg)
+                arguments = len(this._args)
+                vendor = this._engine._vendor
                 if vendor == POSTGRES: placeholder = f'${arguments}'
                 else: placeholder = '?'
                 column_sql = condition._sql.replace('--?--', placeholder)
                 sql = f'''{command} {column_sql}'''
             return sql
         self._sql.append(_)
         return self
@@ -110,14 +121,23 @@
         return self._conditional(condition, param, AND)
 
     def ASC(self):
         def _():
             return f'ASC'
         self._sql.append(_)
         return self
+    
+    def CREATE(self, artifact: Table | Enum):
+        if isinstance(artifact, Table):
+            table = artifact.__table__ or artifact.__class__.__name__
+            self._sql.append(lambda: f'CREATE TABLE {tableize(table)}')
+        if isinstance(artifact, Enum):
+            # create type snake_case(artifiact) as enum ()
+            pass
+        return self
 
     def DESC(self):
         def _():
             return f'DESC'
         self._sql.append(_)
         return self
 
@@ -154,29 +174,33 @@
     def INSERT_INTO(self, table: Table, columns: List[Column]):
         self._zero = self._zero or INSERT
         def _():
             return f'''INSERT INTO {table} ({', '.join(str(column) for column in columns)})'''
         self._sql.append(_)
         return self
 
+    def JOIN(self, *tables: Table):
+        for table in tables:...
+        return self
+
     def LIMIT(self, limit: int):
         return self._limit_offset(limit, LIMIT)
 
     def OFFSET(self, offset: int):
         return self._limit_offset(offset, OFFSET)
 
     def OR(self, condition: Column | str, param = None):
         return self._conditional(condition, param, OR)
 
     def ORDER_BY(self, column: Column):
         def _():
             return f'''ORDER BY {column._sql or column}'''
         self._sql.append(_)
         return self
-    
+
     def RAW(self, statement: str):
         self._sql.append(lambda: statement)
         return self
 
     def RETURNING(self, column: Column):
         def _():
             return f'RETURNING {column}'
@@ -195,24 +219,25 @@
         self._zero = self._zero or SELECT
         def _():
             _columns = [Column.COERCE(f) for f in columns]
             return f'''SELECT {', '.join(_columns)}''' if _columns else 'SELECT *'
         self._sql.append(_)
         return self
 
-    def SET(self, *columns: Column):
+    def SET(self, **kwargs):
+        statements = []
+        vendor = self._engine._vendor
+        for column in kwargs:
+            arg = Column.QUOTE(kwargs.get(column))
+            self._args.append(arg)
+            if vendor == POSTGRES: placeholder = f'${len(self._args)}'
+            else: placeholder = '?'
+            statements.append(f'{column} = {placeholder}')
+
         def _():
-            vendor = self._engine._vendor
-            statements = []
-            for column in columns:
-                self._args.append(column._arg)
-                if vendor == POSTGRES: placeholder = f'${len(self._args)}'
-                else: placeholder = '?'
-                column_sql = column._sql.replace('--?--', placeholder)
-                statements.append(column_sql)
             return f"SET {', '.join(statements)}"
         self._sql.append(_)
         return self
 
     def UPDATE(self, table: Table):
         self._zero = self._zero or UPDATE
         self._sql.append(lambda : f'''UPDATE {table}''')
```

### Comparing `supersql-2023.4.3/supersql/results.py` & `supersql-2023.5.11/supersql/results.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.3/supersql/table.py` & `supersql-2023.5.11/supersql/table.py`

 * *Files identical despite different names*

### Comparing `supersql-2023.4.3/PKG-INFO` & `supersql-2023.5.11/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supersql
-Version: 2023.4.3
+Version: 2023.5.11
 Summary: Thin wrapper on top of SQL that enables you write SQL code in python easily
 Author: Tersoo Ortserga
 Author-email: codesage@live.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -40,21 +40,21 @@
 
 &nbsp;
 
 
 ### NOTE: Still Very Much In Development
 
 ```sql
-SELECT * FROM customers ORDER BY last_name ASC LIMIT 5
+SELECT * FROM customers ORDER BY last_name DESC LIMIT 5
 ```
 
 
 ```py
 # query.SELECT('*') is the same as query.SELECT() or query.SELECT(customers)
-query.SELECT().FROM(customers).ORDER_BY(-customers.last_name).LIMIT(5)
+query.SELECT().FROM(customers).ORDER_BY(last_name = -1).LIMIT(5)
 ```
 
 &nbsp;
 
 ## Why?
 Let's be honest:
 
@@ -77,15 +77,15 @@
 
 
 # Without table schema discovery/reflection i.e. using strings -- NOT OPTIMAL
 results = query.SELECT(
         'first_name', 'last_name', 'email'
     ).FROM(
         'employees'
-    ).WHERE('email = someone@example.com').execute()
+    ).WHERE(email = 'someone@example.com').execute()
 
 for result in results:
     print(result)
 
 
 # reflect table schema and fields into a python object for easy querying
 emps = query.database.table('employees')
```

