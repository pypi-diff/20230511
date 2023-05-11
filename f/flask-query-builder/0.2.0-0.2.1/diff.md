# Comparing `tmp/flask-query-builder-0.2.0.tar.gz` & `tmp/flask_query_builder-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-query-builder-0.2.0.tar", max compression
+gzip compressed data, was "flask_query_builder-0.2.1.tar", max compression
```

## Comparing `flask-query-builder-0.2.0.tar` & `flask_query_builder-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2022-08-09 07:16:17.478057 flask-query-builder-0.2.0/flask_query_builder/__init__.py
--rw-r--r--   0        0        0      316 2022-08-09 07:16:16.650033 flask-query-builder-0.2.0/flask_query_builder/exceptions.py
--rw-r--r--   0        0        0      921 2022-08-09 07:16:16.650033 flask-query-builder-0.2.0/flask_query_builder/filters.py
--rw-r--r--   0        0        0     6115 2022-08-09 07:16:16.650033 flask-query-builder-0.2.0/flask_query_builder/querying.py
--rw-r--r--   0        0        0      442 2022-08-09 07:16:16.650033 flask-query-builder-0.2.0/flask_query_builder/sorts.py
--rw-r--r--   0        0        0      642 2022-08-09 07:16:17.478057 flask-query-builder-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      693 2022-08-09 07:16:27.240033 flask-query-builder-0.2.0/setup.py
--rw-r--r--   0        0        0      622 2022-08-09 07:16:27.240288 flask-query-builder-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 08:57:01.617879 flask_query_builder-0.2.1/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-11 08:57:02.501922 flask_query_builder-0.2.1/flask_query_builder/__init__.py
+-rw-r--r--   0        0        0      316 2023-05-11 08:57:01.617879 flask_query_builder-0.2.1/flask_query_builder/exceptions.py
+-rw-r--r--   0        0        0      921 2023-05-11 08:57:01.617879 flask_query_builder-0.2.1/flask_query_builder/filters.py
+-rw-r--r--   0        0        0     6115 2023-05-11 08:57:01.617879 flask_query_builder-0.2.1/flask_query_builder/querying.py
+-rw-r--r--   0        0        0      442 2023-05-11 08:57:01.617879 flask_query_builder-0.2.1/flask_query_builder/sorts.py
+-rw-r--r--   0        0        0      645 2023-05-11 08:57:02.501922 flask_query_builder-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 flask_query_builder-0.2.1/PKG-INFO
```

### Comparing `flask-query-builder-0.2.0/flask_query_builder/filters.py` & `flask_query_builder-0.2.1/flask_query_builder/filters.py`

 * *Files identical despite different names*

### Comparing `flask-query-builder-0.2.0/flask_query_builder/querying.py` & `flask_query_builder-0.2.1/flask_query_builder/querying.py`

 * *Files identical despite different names*

### Comparing `flask-query-builder-0.2.0/pyproject.toml` & `flask_query_builder-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "flask-query-builder"
-version = "0.2.0"
+version = "0.2.1"
 description = "A request query builder for flask and sqlalchemy"
 authors = ["Demos Petsas"]
 
 [tool.poetry.dependencies]
 python = ">=2.7,<2.8 || >=3.6.0, <3.10.0"
-SQLAlchemy = "1.4.0"
+SQLAlchemy = ">=1.4.0"
 Flask = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=3.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.8"]
@@ -20,8 +20,8 @@
 version_variable = [
     "flask_query_builder/__init__.py:__version__",
     "pyproject.toml:version"
 ]
 branch = "master"
 upload_to_pypi = true
 upload_to_release = true
-build_command = "pip install poetry && poetry build"
+build_command = "pip install poetry && poetry build"
```

### Comparing `flask-query-builder-0.2.0/PKG-INFO` & `flask_query_builder-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: flask-query-builder
-Version: 0.2.0
+Version: 0.2.1
 Summary: A request query builder for flask and sqlalchemy
 Author: Demos Petsas
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.10.*, !=3.11.*
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask
-Requires-Dist: SQLAlchemy (==1.4.0)
+Requires-Dist: SQLAlchemy (>=1.4.0)
```

