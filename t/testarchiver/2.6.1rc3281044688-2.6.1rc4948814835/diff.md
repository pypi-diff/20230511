# Comparing `tmp/testarchiver-2.6.1rc3281044688.tar.gz` & `tmp/testarchiver-2.6.1rc4948814835.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testarchiver-2.6.1rc3281044688.tar", last modified: Wed Oct 19 11:10:32 2022, max compression
+gzip compressed data, was "testarchiver-2.6.1rc4948814835.tar", last modified: Thu May 11 14:10:42 2023, max compression
```

## Comparing `testarchiver-2.6.1rc3281044688.tar` & `testarchiver-2.6.1rc4948814835.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 11:10:32.753706 testarchiver-2.6.1rc3281044688/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    22041 2022-10-19 11:10:32.753706 testarchiver-2.6.1rc3281044688/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18920 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 11:10:32.749706 testarchiver-2.6.1rc3281044688/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/helpers/diff2change_context_list.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-19 11:10:32.753706 testarchiver-2.6.1rc3281044688/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 11:10:32.749706 testarchiver-2.6.1rc3281044688/test_archiver/
--rw-r--r--   0 runner    (1001) docker     (121)     3193 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/ArchiverRobotListener.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30819 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/archiver.py
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/archiver_listeners.py
--rw-r--r--   0 runner    (1001) docker     (121)    12364 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/configs.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16682 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/database.py
--rw-r--r--   0 runner    (1001) docker     (121)    39573 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/output_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 11:10:32.753706 testarchiver-2.6.1rc3281044688/test_archiver/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     9036 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/schemas/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 11:10:32.749706 testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 11:10:32.753706 testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/postgres/
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/postgres/0001-schema_update_table_and_log_message_index.sql
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/postgres/0002-execution_paths.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 11:10:32.753706 testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/sqlite/
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/sqlite/0001-schema_update_table_and_log_message_index.sql
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/sqlite/0002-execution_paths.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 11:10:32.753706 testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/sqlite/testing/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/sqlite/testing/10001-minor_test_update1.sql
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/sqlite/testing/10002-minor_test_update2.sql
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/sqlite/testing/10003-major_test_update.sql
--rw-r--r--   0 runner    (1001) docker     (121)     4392 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/schemas/schema_postgres.sql
--rw-r--r--   0 runner    (1001) docker     (121)     4435 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/schemas/schema_sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-10-19 11:10:15.000000 testarchiver-2.6.1rc3281044688/test_archiver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 11:10:32.753706 testarchiver-2.6.1rc3281044688/testarchiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22041 2022-10-19 11:10:32.000000 testarchiver-2.6.1rc3281044688/testarchiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-10-19 11:10:32.000000 testarchiver-2.6.1rc3281044688/testarchiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 11:10:32.000000 testarchiver-2.6.1rc3281044688/testarchiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-19 11:10:32.000000 testarchiver-2.6.1rc3281044688/testarchiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 11:10:32.000000 testarchiver-2.6.1rc3281044688/testarchiver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-19 11:10:32.000000 testarchiver-2.6.1rc3281044688/testarchiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-19 11:10:32.000000 testarchiver-2.6.1rc3281044688/testarchiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:10:42.189477 testarchiver-2.6.1rc4948814835/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-05-11 14:10:42.189477 testarchiver-2.6.1rc4948814835/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19018 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:10:42.185477 testarchiver-2.6.1rc4948814835/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/helpers/diff2change_context_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:10:42.189477 testarchiver-2.6.1rc4948814835/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:10:42.185477 testarchiver-2.6.1rc4948814835/test_archiver/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/ArchiverRobotListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/archiver_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/configs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16691 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39573 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/output_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:10:42.189477 testarchiver-2.6.1rc4948814835/test_archiver/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/schemas/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:10:42.185477 testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:10:42.189477 testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/postgres/0001-schema_update_table_and_log_message_index.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/postgres/0002-execution_paths.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:10:42.189477 testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/sqlite/0001-schema_update_table_and_log_message_index.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/sqlite/0002-execution_paths.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:10:42.189477 testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/sqlite/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/sqlite/testing/10001-minor_test_update1.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/sqlite/testing/10002-minor_test_update2.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/sqlite/testing/10003-major_test_update.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/schemas/schema_postgres.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/schemas/schema_sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-11 14:10:22.000000 testarchiver-2.6.1rc4948814835/test_archiver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:10:42.189477 testarchiver-2.6.1rc4948814835/testarchiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-05-11 14:10:41.000000 testarchiver-2.6.1rc4948814835/testarchiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-11 14:10:42.000000 testarchiver-2.6.1rc4948814835/testarchiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:10:41.000000 testarchiver-2.6.1rc4948814835/testarchiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 14:10:41.000000 testarchiver-2.6.1rc4948814835/testarchiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:10:41.000000 testarchiver-2.6.1rc4948814835/testarchiver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 14:10:41.000000 testarchiver-2.6.1rc4948814835/testarchiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 14:10:41.000000 testarchiver-2.6.1rc4948814835/testarchiver.egg-info/top_level.txt
```

### Comparing `testarchiver-2.6.1rc3281044688/LICENSE` & `testarchiver-2.6.1rc4948814835/LICENSE`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/PKG-INFO` & `testarchiver-2.6.1rc4948814835/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testarchiver
-Version: 2.6.1rc3281044688
+Version: 2.6.1rc4948814835
 Summary: Tools for serialising test results to SQL database 
 Home-page: https://github.com/salabs/TestArchiver
 Author: Tommi Oinonen
 Author-email: salabs-mail@siili.com
 License: Apache License 2.0
 Description: # TestArchiver
         
@@ -239,14 +239,17 @@
         
         This example is mimicking adding daylight savings (1hr = 3600 secs) onto
         a system offset secs of 7200 (GMT+2). i.e. if the computer being used had the 'daylight savings' setting
         of and you want to manually add it during archiving.
         
         
         # Release notes
+        - 2.6.2 (2023-05-11)
+          * Fixes error message when newer schema used in archive than for archiver
+        
         - 2.6.1 (2022-10-19)
           * Fixes a bug/regression that caused data of log messages not to be archived.
         
         - 2.6.0 (2022-09-15)
           * `--max_log_message_length` option to control the length of log messages archived.
             Defaults to 2000 chars. Negative values will archive log messages from the end.
           * Ignores return statements without warnigns from Robot Framework 5.x inputs
```

### Comparing `testarchiver-2.6.1rc3281044688/README.md` & `testarchiver-2.6.1rc4948814835/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,17 @@
 
 This example is mimicking adding daylight savings (1hr = 3600 secs) onto
 a system offset secs of 7200 (GMT+2). i.e. if the computer being used had the 'daylight savings' setting
 of and you want to manually add it during archiving.
 
 
 # Release notes
+- 2.6.2 (2023-05-11)
+  * Fixes error message when newer schema used in archive than for archiver
+
 - 2.6.1 (2022-10-19)
   * Fixes a bug/regression that caused data of log messages not to be archived.
 
 - 2.6.0 (2022-09-15)
   * `--max_log_message_length` option to control the length of log messages archived.
     Defaults to 2000 chars. Negative values will archive log messages from the end.
   * Ignores return statements without warnigns from Robot Framework 5.x inputs
```

### Comparing `testarchiver-2.6.1rc3281044688/helpers/diff2change_context_list.py` & `testarchiver-2.6.1rc4948814835/helpers/diff2change_context_list.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/setup.py` & `testarchiver-2.6.1rc4948814835/setup.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/test_archiver/ArchiverRobotListener.py` & `testarchiver-2.6.1rc4948814835/test_archiver/ArchiverRobotListener.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/test_archiver/archiver.py` & `testarchiver-2.6.1rc4948814835/test_archiver/archiver.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/test_archiver/archiver_listeners.py` & `testarchiver-2.6.1rc4948814835/test_archiver/archiver_listeners.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/test_archiver/configs.py` & `testarchiver-2.6.1rc4948814835/test_archiver/configs.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/test_archiver/database.py` & `testarchiver-2.6.1rc4948814835/test_archiver/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     def check_and_update_schema(self):
         latest_update_applied = self._latest_update_applied()
         if latest_update_applied is None:
             if self._initialize_schema():
                 print('Test archive schema initialized')
                 return
             latest_update_applied = 0
-        if latest_update_applied < self._schema_updates[-1][0]:
+        if latest_update_applied < self.current_schema_version():
             for update_id, is_minor, file in self._schema_updates:
                 if update_id > latest_update_applied:
                     base_dir = Path(os.path.dirname(__file__))
                     script_file = base_dir / 'schemas/migrations' / self._db_engine_identifier() / file
                     if self.allow_major_schema_updates or (is_minor and self.allow_minor_schema_updates):
                         print('Running schema update {} from: {}'.format(update_id, script_file))
                         self._run_script(script_file)
@@ -97,18 +97,18 @@
                                                       'Run with --allow-minor-schema-updates option to '
                                                       'update the schema to match the archiver version.')
                     else:
                         raise ArchiverSchemaException('ERROR: pending major schema update is needed.'
                                                       'Run with --allow-major-schema-updates option to '
                                                       'update the schema to match the archiver version.')
 
-        elif latest_update_applied > self._schema_updates[-1][0]:
+        elif latest_update_applied > self.current_schema_version():
             # The schema is newer than the Archiver
             minimum_version = self.fetch_one_value('schema_updates', 'applied_by',
-                                                   {'update_id': latest_update_applied})
+                                                   {'schema_version': latest_update_applied})
             raise ArchiverSchemaException("ERROR: The version of TestArchiver is older than the schema. "
                                           "Please update to version '{}' or higher".format(minimum_version))
 
     def _latest_update_applied(self):
         try:
             return self.max_value('schema_updates', 'schema_version')
         except self.UndefinedTableError:
```

### Comparing `testarchiver-2.6.1rc3281044688/test_archiver/output_parser.py` & `testarchiver-2.6.1rc4948814835/test_archiver/output_parser.py`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/test_archiver/schemas/README.md` & `testarchiver-2.6.1rc4948814835/test_archiver/schemas/README.md`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/postgres/0001-schema_update_table_and_log_message_index.sql` & `testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/postgres/0001-schema_update_table_and_log_message_index.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/test_archiver/schemas/migrations/sqlite/0001-schema_update_table_and_log_message_index.sql` & `testarchiver-2.6.1rc4948814835/test_archiver/schemas/migrations/sqlite/0001-schema_update_table_and_log_message_index.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/test_archiver/schemas/schema_postgres.sql` & `testarchiver-2.6.1rc4948814835/test_archiver/schemas/schema_postgres.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/test_archiver/schemas/schema_sqlite.sql` & `testarchiver-2.6.1rc4948814835/test_archiver/schemas/schema_sqlite.sql`

 * *Files identical despite different names*

### Comparing `testarchiver-2.6.1rc3281044688/testarchiver.egg-info/PKG-INFO` & `testarchiver-2.6.1rc4948814835/testarchiver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testarchiver
-Version: 2.6.1rc3281044688
+Version: 2.6.1rc4948814835
 Summary: Tools for serialising test results to SQL database 
 Home-page: https://github.com/salabs/TestArchiver
 Author: Tommi Oinonen
 Author-email: salabs-mail@siili.com
 License: Apache License 2.0
 Description: # TestArchiver
         
@@ -239,14 +239,17 @@
         
         This example is mimicking adding daylight savings (1hr = 3600 secs) onto
         a system offset secs of 7200 (GMT+2). i.e. if the computer being used had the 'daylight savings' setting
         of and you want to manually add it during archiving.
         
         
         # Release notes
+        - 2.6.2 (2023-05-11)
+          * Fixes error message when newer schema used in archive than for archiver
+        
         - 2.6.1 (2022-10-19)
           * Fixes a bug/regression that caused data of log messages not to be archived.
         
         - 2.6.0 (2022-09-15)
           * `--max_log_message_length` option to control the length of log messages archived.
             Defaults to 2000 chars. Negative values will archive log messages from the end.
           * Ignores return statements without warnigns from Robot Framework 5.x inputs
```

### Comparing `testarchiver-2.6.1rc3281044688/testarchiver.egg-info/SOURCES.txt` & `testarchiver-2.6.1rc4948814835/testarchiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

