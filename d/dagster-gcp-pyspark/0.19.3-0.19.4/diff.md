# Comparing `tmp/dagster_gcp_pyspark-0.19.3.tar.gz` & `tmp/dagster_gcp_pyspark-0.19.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_gcp_pyspark-0.19.3.tar", last modified: Thu May  4 17:52:33 2023, max compression
+gzip compressed data, was "dagster_gcp_pyspark-0.19.4.tar", last modified: Thu May 11 17:09:08 2023, max compression
```

## Comparing `dagster_gcp_pyspark-0.19.3.tar` & `dagster_gcp_pyspark-0.19.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:52:33.116577 dagster_gcp_pyspark-0.19.3/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      649 2023-05-04 17:52:33.116577 dagster_gcp_pyspark-0.19.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      143 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:52:33.112577 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/
--rw-r--r--   0 root         (0) root         (0)      402 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:52:33.112577 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9900 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:52:33.112577 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      649 2023-05-04 17:52:33.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-04 17:52:33.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:52:33.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:52:33.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-04 17:52:33.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-04 17:52:33.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-05-04 17:52:33.116577 dagster_gcp_pyspark-0.19.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1366 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:09:08.143638 dagster_gcp_pyspark-0.19.4/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-05-11 16:58:41.000000 dagster_gcp_pyspark-0.19.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-11 16:58:41.000000 dagster_gcp_pyspark-0.19.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      649 2023-05-11 17:09:08.143638 dagster_gcp_pyspark-0.19.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      143 2023-05-11 16:58:41.000000 dagster_gcp_pyspark-0.19.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:09:08.139638 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-05-11 16:58:41.000000 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:09:08.143638 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9900 2023-05-11 16:58:41.000000 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-11 16:58:41.000000 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-11 16:58:41.000000 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:09:08.143638 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-05-11 17:09:08.000000 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-11 17:09:08.000000 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 17:09:08.000000 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 17:09:08.000000 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-11 17:09:08.000000 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-11 17:09:08.000000 dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-05-11 17:09:08.147638 dagster_gcp_pyspark-0.19.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-05-11 16:58:41.000000 dagster_gcp_pyspark-0.19.4/setup.py
```

### Comparing `dagster_gcp_pyspark-0.19.3/LICENSE` & `dagster_gcp_pyspark-0.19.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_gcp_pyspark-0.19.3/PKG-INFO` & `dagster_gcp_pyspark-0.19.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_gcp_pyspark
-Version: 0.19.3
+Version: 0.19.4
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py` & `dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/PKG-INFO` & `dagster_gcp_pyspark-0.19.4/dagster_gcp_pyspark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pyspark
-Version: 0.19.3
+Version: 0.19.4
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster_gcp_pyspark-0.19.3/setup.py` & `dagster_gcp_pyspark-0.19.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pyspark_tests*"]),
     install_requires=[
-        "dagster==1.3.3",
-        "dagster-gcp==0.19.3",
+        "dagster==1.3.4",
+        "dagster-gcp==0.19.4",
         "pyspark",
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

