# Comparing `tmp/dagster-snowflake-pyspark-0.19.3.tar.gz` & `tmp/dagster-snowflake-pyspark-0.19.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-snowflake-pyspark-0.19.3.tar", last modified: Thu May  4 17:55:32 2023, max compression
+gzip compressed data, was "dagster-snowflake-pyspark-0.19.4.tar", last modified: Thu May 11 17:07:52 2023, max compression
```

## Comparing `dagster-snowflake-pyspark-0.19.3.tar` & `dagster-snowflake-pyspark-0.19.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:32.981826 dagster-snowflake-pyspark-0.19.3/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-04 17:42:14.000000 dagster-snowflake-pyspark-0.19.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-04 17:42:14.000000 dagster-snowflake-pyspark-0.19.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-04 17:55:32.981826 dagster-snowflake-pyspark-0.19.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      161 2023-05-04 17:42:14.000000 dagster-snowflake-pyspark-0.19.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:32.981826 dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark/
--rw-r--r--   0 root         (0) root         (0)      421 2023-05-04 17:42:14.000000 dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-04 17:42:14.000000 dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)     9162 2023-05-04 17:42:14.000000 dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-04 17:42:14.000000 dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:32.981826 dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-04 17:55:32.000000 dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      510 2023-05-04 17:55:32.000000 dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:55:32.000000 dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:55:32.000000 dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-04 17:55:32.000000 dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-04 17:55:32.000000 dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-04 17:55:32.981826 dagster-snowflake-pyspark-0.19.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1510 2023-05-04 17:42:14.000000 dagster-snowflake-pyspark-0.19.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:07:52.239761 dagster-snowflake-pyspark-0.19.4/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-11 16:58:41.000000 dagster-snowflake-pyspark-0.19.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-11 16:58:41.000000 dagster-snowflake-pyspark-0.19.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-11 17:07:52.239761 dagster-snowflake-pyspark-0.19.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      161 2023-05-11 16:58:41.000000 dagster-snowflake-pyspark-0.19.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:07:52.239761 dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-05-11 16:58:41.000000 dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-11 16:58:41.000000 dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9162 2023-05-11 16:58:41.000000 dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-11 16:58:41.000000 dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:07:52.239761 dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-11 17:07:52.000000 dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      510 2023-05-11 17:07:52.000000 dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 17:07:52.000000 dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 17:07:52.000000 dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-11 17:07:52.000000 dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-11 17:07:52.000000 dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-11 17:07:52.243761 dagster-snowflake-pyspark-0.19.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-05-11 16:58:41.000000 dagster-snowflake-pyspark-0.19.4/setup.py
```

### Comparing `dagster-snowflake-pyspark-0.19.3/LICENSE` & `dagster-snowflake-pyspark-0.19.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pyspark-0.19.3/PKG-INFO` & `dagster-snowflake-pyspark-0.19.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pyspark
-Version: 0.19.3
+Version: 0.19.4
 Summary: Package for integrating Snowflake and PySpark with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py` & `dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pyspark-0.19.3/dagster_snowflake_pyspark.egg-info/PKG-INFO` & `dagster-snowflake-pyspark-0.19.4/dagster_snowflake_pyspark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pyspark
-Version: 0.19.3
+Version: 0.19.4
 Summary: Package for integrating Snowflake and PySpark with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-snowflake-pyspark-0.19.3/setup.py` & `dagster-snowflake-pyspark-0.19.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_snowflake_pyspark_tests*"]),
     install_requires=[
-        "dagster==1.3.3",
-        "dagster-snowflake==0.19.3",
+        "dagster==1.3.4",
+        "dagster-snowflake==0.19.4",
         "pyspark",
         "requests",
         "sqlalchemy!=1.4.42",  # workaround for https://github.com/snowflakedb/snowflake-sqlalchemy/issues/350
         "snowflake-sqlalchemy>=1.2",
     ],
     zip_safe=False,
 )
```

