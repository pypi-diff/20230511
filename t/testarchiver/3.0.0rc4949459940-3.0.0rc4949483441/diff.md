# Comparing `tmp/testarchiver-3.0.0rc4949459940.tar.gz` & `tmp/testarchiver-3.0.0rc4949483441.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testarchiver-3.0.0rc4949459940.tar", last modified: Thu May 11 15:09:47 2023, max compression
+gzip compressed data, was "testarchiver-3.0.0rc4949483441.tar", last modified: Thu May 11 15:11:56 2023, max compression
```

## Comparing `testarchiver-3.0.0rc4949459940.tar` & `testarchiver-3.0.0rc4949483441.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:47.518339 testarchiver-3.0.0rc4949459940/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    27375 2023-05-11 15:09:47.518339 testarchiver-3.0.0rc4949459940/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23646 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:47.514339 testarchiver-3.0.0rc4949459940/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/helpers/diff2change_context_list.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:09:47.518339 testarchiver-3.0.0rc4949459940/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:47.518339 testarchiver-3.0.0rc4949459940/test_archiver/
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/ArchiverRobotListener.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/archiver_listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/configs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24082 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    39638 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/output_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:47.518339 testarchiver-3.0.0rc4949459940/test_archiver/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/schemas/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:47.514339 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:47.518339 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/postgres/0001-schema_update_table_and_log_message_index.sql
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/postgres/0002-execution_paths.sql
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/postgres/0003-test_run_mapping_cascade.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:47.518339 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/sqlite/0001-schema_update_table_and_log_message_index.sql
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/sqlite/0002-execution_paths.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/sqlite/0003-test_run_mapping_cascade.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:47.518339 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/sqlite/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/sqlite/testing/10001-minor_test_update1.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/sqlite/testing/10002-minor_test_update2.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/sqlite/testing/10003-major_test_update.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/schemas/schema_postgres.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/schemas/schema_sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-11 15:09:33.000000 testarchiver-3.0.0rc4949459940/test_archiver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:09:47.518339 testarchiver-3.0.0rc4949459940/testarchiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27375 2023-05-11 15:09:47.000000 testarchiver-3.0.0rc4949459940/testarchiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-11 15:09:47.000000 testarchiver-3.0.0rc4949459940/testarchiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:09:47.000000 testarchiver-3.0.0rc4949459940/testarchiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 15:09:47.000000 testarchiver-3.0.0rc4949459940/testarchiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:09:47.000000 testarchiver-3.0.0rc4949459940/testarchiver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 15:09:47.000000 testarchiver-3.0.0rc4949459940/testarchiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 15:09:47.000000 testarchiver-3.0.0rc4949459940/testarchiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:11:56.336659 testarchiver-3.0.0rc4949483441/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    27375 2023-05-11 15:11:56.336659 testarchiver-3.0.0rc4949483441/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23646 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:11:56.332658 testarchiver-3.0.0rc4949483441/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/helpers/diff2change_context_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:11:56.336659 testarchiver-3.0.0rc4949483441/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:11:56.332658 testarchiver-3.0.0rc4949483441/test_archiver/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/ArchiverRobotListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/archiver_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/configs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24082 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39638 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/output_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:11:56.332658 testarchiver-3.0.0rc4949483441/test_archiver/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/schemas/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:11:56.332658 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:11:56.332658 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/postgres/0001-schema_update_table_and_log_message_index.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/postgres/0002-execution_paths.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/postgres/0003-test_run_mapping_cascade.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:11:56.332658 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/sqlite/0001-schema_update_table_and_log_message_index.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/sqlite/0002-execution_paths.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/sqlite/0003-test_run_mapping_cascade.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:11:56.332658 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/sqlite/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/sqlite/testing/10001-minor_test_update1.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/sqlite/testing/10002-minor_test_update2.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/sqlite/testing/10003-major_test_update.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/schemas/schema_postgres.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/schemas/schema_sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-11 15:11:42.000000 testarchiver-3.0.0rc4949483441/test_archiver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:11:56.332658 testarchiver-3.0.0rc4949483441/testarchiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27375 2023-05-11 15:11:56.000000 testarchiver-3.0.0rc4949483441/testarchiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-11 15:11:56.000000 testarchiver-3.0.0rc4949483441/testarchiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:11:56.000000 testarchiver-3.0.0rc4949483441/testarchiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 15:11:56.000000 testarchiver-3.0.0rc4949483441/testarchiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:11:56.000000 testarchiver-3.0.0rc4949483441/testarchiver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 15:11:56.000000 testarchiver-3.0.0rc4949483441/testarchiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 15:11:56.000000 testarchiver-3.0.0rc4949483441/testarchiver.egg-info/top_level.txt
```

### Comparing `testarchiver-3.0.0rc4949459940/LICENSE` & `testarchiver-3.0.0rc4949483441/LICENSE`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/PKG-INFO` & `testarchiver-3.0.0rc4949483441/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testarchiver
-Version: 3.0.0rc4949459940
+Version: 3.0.0rc4949483441
 Summary: Tools for serialising test results to SQL database 
 Home-page: https://github.com/salabs/TestArchiver
 Author: Tommi Oinonen
 Author-email: salabs-mail@siili.com
 License: Apache License 2.0
 Description: # TestArchiver
```

### Comparing `testarchiver-3.0.0rc4949459940/README.md` & `testarchiver-3.0.0rc4949483441/README.md`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/helpers/diff2change_context_list.py` & `testarchiver-3.0.0rc4949483441/helpers/diff2change_context_list.py`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/setup.py` & `testarchiver-3.0.0rc4949483441/setup.py`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/ArchiverRobotListener.py` & `testarchiver-3.0.0rc4949483441/test_archiver/ArchiverRobotListener.py`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/archiver.py` & `testarchiver-3.0.0rc4949483441/test_archiver/archiver.py`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/archiver_listeners.py` & `testarchiver-3.0.0rc4949483441/test_archiver/archiver_listeners.py`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/configs.py` & `testarchiver-3.0.0rc4949483441/test_archiver/configs.py`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/database.py` & `testarchiver-3.0.0rc4949483441/test_archiver/database.py`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/output_parser.py` & `testarchiver-3.0.0rc4949483441/test_archiver/output_parser.py`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/schemas/README.md` & `testarchiver-3.0.0rc4949483441/test_archiver/schemas/README.md`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/postgres/0001-schema_update_table_and_log_message_index.sql` & `testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/postgres/0001-schema_update_table_and_log_message_index.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/postgres/0003-test_run_mapping_cascade.sql` & `testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/postgres/0003-test_run_mapping_cascade.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/sqlite/0001-schema_update_table_and_log_message_index.sql` & `testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/sqlite/0001-schema_update_table_and_log_message_index.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/schemas/migrations/sqlite/0003-test_run_mapping_cascade.sql` & `testarchiver-3.0.0rc4949483441/test_archiver/schemas/migrations/sqlite/0003-test_run_mapping_cascade.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/schemas/schema_postgres.sql` & `testarchiver-3.0.0rc4949483441/test_archiver/schemas/schema_postgres.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/test_archiver/schemas/schema_sqlite.sql` & `testarchiver-3.0.0rc4949483441/test_archiver/schemas/schema_sqlite.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-3.0.0rc4949459940/testarchiver.egg-info/PKG-INFO` & `testarchiver-3.0.0rc4949483441/testarchiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testarchiver
-Version: 3.0.0rc4949459940
+Version: 3.0.0rc4949483441
 Summary: Tools for serialising test results to SQL database 
 Home-page: https://github.com/salabs/TestArchiver
 Author: Tommi Oinonen
 Author-email: salabs-mail@siili.com
 License: Apache License 2.0
 Description: # TestArchiver
```

### Comparing `testarchiver-3.0.0rc4949459940/testarchiver.egg-info/SOURCES.txt` & `testarchiver-3.0.0rc4949483441/testarchiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

