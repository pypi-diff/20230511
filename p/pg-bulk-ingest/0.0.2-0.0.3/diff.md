# Comparing `tmp/pg_bulk_ingest-0.0.2.tar.gz` & `tmp/pg_bulk_ingest-0.0.3.tar.gz`

## Comparing `pg_bulk_ingest-0.0.2.tar` & `pg_bulk_ingest-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.2/pg_bulk_ingest.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.2/LICENSE
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.2/README.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.3/pg_bulk_ingest.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.3/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.3/PKG-INFO
```

### Comparing `pg_bulk_ingest-0.0.2/.gitignore` & `pg_bulk_ingest-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.2/LICENSE` & `pg_bulk_ingest-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.2/README.md` & `pg_bulk_ingest-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.2/pyproject.toml` & `pg_bulk_ingest-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-bulk-ingest"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "sqlalchemy>=2.0.12",
-    "psycopg[binary]>=3.1.9",
+    "sqlalchemy>=1.4.0,<2.0.0", 
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest>=7.2.1",
+    "psycopg2-binary>=2.8.6",
 ]
 
 [project.urls]
 "Source" = "https://github.com/uktrade/pg-bulk-ingest"
 
 [tool.hatch.build]
 include = [
```

### Comparing `pg_bulk_ingest-0.0.2/PKG-INFO` & `pg_bulk_ingest-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pg-bulk-ingest
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking
 Project-URL: Source, https://github.com/uktrade/pg-bulk-ingest
 Author-email: Department for International Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: psycopg[binary]>=3.1.9
-Requires-Dist: sqlalchemy>=2.0.12
+Requires-Dist: sqlalchemy<2.0.0,>=1.4.0
 Provides-Extra: dev
+Requires-Dist: psycopg2-binary>=2.8.6; extra == 'dev'
 Requires-Dist: pytest>=7.2.1; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # pg-bulk-ingest
 
 A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking
```

