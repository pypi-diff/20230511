# Comparing `tmp/testarchiver-2.6.1rc4948985236.tar.gz` & `tmp/testarchiver-2.6.1rc4949012430.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testarchiver-2.6.1rc4948985236.tar", last modified: Thu May 11 14:25:30 2023, max compression
+gzip compressed data, was "testarchiver-2.6.1rc4949012430.tar", last modified: Thu May 11 14:28:32 2023, max compression
```

## Comparing `testarchiver-2.6.1rc4948985236.tar` & `testarchiver-2.6.1rc4949012430.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:25:30.187892 testarchiver-2.6.1rc4948985236/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-05-11 14:25:30.187892 testarchiver-2.6.1rc4948985236/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19058 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:25:30.183892 testarchiver-2.6.1rc4948985236/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/helpers/diff2change_context_list.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:25:30.187892 testarchiver-2.6.1rc4948985236/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:25:30.183892 testarchiver-2.6.1rc4948985236/test_archiver/
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/ArchiverRobotListener.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/archiver_listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/configs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16691 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    39573 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/output_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:25:30.183892 testarchiver-2.6.1rc4948985236/test_archiver/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/schemas/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:25:30.183892 testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:25:30.187892 testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/postgres/0001-schema_update_table_and_log_message_index.sql
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/postgres/0002-execution_paths.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:25:30.187892 testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/sqlite/0001-schema_update_table_and_log_message_index.sql
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/sqlite/0002-execution_paths.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:25:30.187892 testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/sqlite/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/sqlite/testing/10001-minor_test_update1.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/sqlite/testing/10002-minor_test_update2.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/sqlite/testing/10003-major_test_update.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/schemas/schema_postgres.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/schemas/schema_sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-11 14:25:16.000000 testarchiver-2.6.1rc4948985236/test_archiver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:25:30.187892 testarchiver-2.6.1rc4948985236/testarchiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-05-11 14:25:29.000000 testarchiver-2.6.1rc4948985236/testarchiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-11 14:25:30.000000 testarchiver-2.6.1rc4948985236/testarchiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:25:29.000000 testarchiver-2.6.1rc4948985236/testarchiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 14:25:29.000000 testarchiver-2.6.1rc4948985236/testarchiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:25:29.000000 testarchiver-2.6.1rc4948985236/testarchiver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 14:25:29.000000 testarchiver-2.6.1rc4948985236/testarchiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 14:25:29.000000 testarchiver-2.6.1rc4948985236/testarchiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:28:32.602876 testarchiver-2.6.1rc4949012430/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-05-11 14:28:32.602876 testarchiver-2.6.1rc4949012430/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19058 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:28:32.598876 testarchiver-2.6.1rc4949012430/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/helpers/diff2change_context_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:28:32.602876 testarchiver-2.6.1rc4949012430/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:28:32.598876 testarchiver-2.6.1rc4949012430/test_archiver/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/ArchiverRobotListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/archiver_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/configs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16691 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39573 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/output_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:28:32.598876 testarchiver-2.6.1rc4949012430/test_archiver/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/schemas/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:28:32.598876 testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:28:32.598876 testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/postgres/0001-schema_update_table_and_log_message_index.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/postgres/0002-execution_paths.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:28:32.602876 testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/sqlite/0001-schema_update_table_and_log_message_index.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/sqlite/0002-execution_paths.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:28:32.602876 testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/sqlite/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/sqlite/testing/10001-minor_test_update1.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/sqlite/testing/10002-minor_test_update2.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/sqlite/testing/10003-major_test_update.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/schemas/schema_postgres.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/schemas/schema_sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-11 14:28:01.000000 testarchiver-2.6.1rc4949012430/test_archiver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:28:32.602876 testarchiver-2.6.1rc4949012430/testarchiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-05-11 14:28:30.000000 testarchiver-2.6.1rc4949012430/testarchiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-11 14:28:32.000000 testarchiver-2.6.1rc4949012430/testarchiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:28:30.000000 testarchiver-2.6.1rc4949012430/testarchiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 14:28:30.000000 testarchiver-2.6.1rc4949012430/testarchiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:28:30.000000 testarchiver-2.6.1rc4949012430/testarchiver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 14:28:30.000000 testarchiver-2.6.1rc4949012430/testarchiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 14:28:30.000000 testarchiver-2.6.1rc4949012430/testarchiver.egg-info/top_level.txt
```

### Comparing `testarchiver-2.6.1rc4948985236/LICENSE` & `testarchiver-2.6.1rc4949012430/LICENSE`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/PKG-INFO` & `testarchiver-2.6.1rc4949012430/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testarchiver
-Version: 2.6.1rc4948985236
+Version: 2.6.1rc4949012430
 Summary: Tools for serialising test results to SQL database 
 Home-page: https://github.com/salabs/TestArchiver
 Author: Tommi Oinonen
 Author-email: salabs-mail@siili.com
 License: Apache License 2.0
 Description: # TestArchiver
```

### Comparing `testarchiver-2.6.1rc4948985236/README.md` & `testarchiver-2.6.1rc4949012430/README.md`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/helpers/diff2change_context_list.py` & `testarchiver-2.6.1rc4949012430/helpers/diff2change_context_list.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/setup.py` & `testarchiver-2.6.1rc4949012430/setup.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/test_archiver/ArchiverRobotListener.py` & `testarchiver-2.6.1rc4949012430/test_archiver/ArchiverRobotListener.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/test_archiver/archiver.py` & `testarchiver-2.6.1rc4949012430/test_archiver/archiver.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/test_archiver/archiver_listeners.py` & `testarchiver-2.6.1rc4949012430/test_archiver/archiver_listeners.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/test_archiver/configs.py` & `testarchiver-2.6.1rc4949012430/test_archiver/configs.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/test_archiver/database.py` & `testarchiver-2.6.1rc4949012430/test_archiver/database.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/test_archiver/output_parser.py` & `testarchiver-2.6.1rc4949012430/test_archiver/output_parser.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/test_archiver/schemas/README.md` & `testarchiver-2.6.1rc4949012430/test_archiver/schemas/README.md`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/postgres/0001-schema_update_table_and_log_message_index.sql` & `testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/postgres/0001-schema_update_table_and_log_message_index.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/test_archiver/schemas/migrations/sqlite/0001-schema_update_table_and_log_message_index.sql` & `testarchiver-2.6.1rc4949012430/test_archiver/schemas/migrations/sqlite/0001-schema_update_table_and_log_message_index.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/test_archiver/schemas/schema_postgres.sql` & `testarchiver-2.6.1rc4949012430/test_archiver/schemas/schema_postgres.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/test_archiver/schemas/schema_sqlite.sql` & `testarchiver-2.6.1rc4949012430/test_archiver/schemas/schema_sqlite.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc4948985236/testarchiver.egg-info/PKG-INFO` & `testarchiver-2.6.1rc4949012430/testarchiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testarchiver
-Version: 2.6.1rc4948985236
+Version: 2.6.1rc4949012430
 Summary: Tools for serialising test results to SQL database 
 Home-page: https://github.com/salabs/TestArchiver
 Author: Tommi Oinonen
 Author-email: salabs-mail@siili.com
 License: Apache License 2.0
 Description: # TestArchiver
```

### Comparing `testarchiver-2.6.1rc4948985236/testarchiver.egg-info/SOURCES.txt` & `testarchiver-2.6.1rc4949012430/testarchiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

