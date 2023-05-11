# Comparing `tmp/vdk-gdp-execution-id-0.0.848464550.tar.gz` & `tmp/vdk-gdp-execution-id-0.0.863985686.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-gdp-execution-id-0.0.848464550.tar", last modified: Tue Apr 25 14:42:02 2023, max compression
+gzip compressed data, was "vdk-gdp-execution-id-0.0.863985686.tar", last modified: Thu May 11 07:40:01 2023, max compression
```

## Comparing `vdk-gdp-execution-id-0.0.848464550.tar` & `vdk-gdp-execution-id-0.0.863985686.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/
--rw-r--r--   0 root         (0) root         (0)     3622 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2937 2023-04-25 14:41:49.000000 vdk-gdp-execution-id-0.0.848464550/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-04-25 14:41:53.000000 vdk-gdp-execution-id-0.0.848464550/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/gdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/gdp/execution_id/
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-04-25 14:41:49.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/gdp/execution_id/gdp_execution_id_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     2322 2023-04-25 14:41:49.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/gdp/execution_id/gdp_execution_id_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:42:02.588134 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3622 2023-04-25 14:42:02.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-25 14:42:02.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 14:42:02.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-04-25 14:42:02.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-25 14:42:02.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-25 14:42:02.000000 vdk-gdp-execution-id-0.0.848464550/src/vdk_gdp_execution_id.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2023-05-11 07:39:48.000000 vdk-gdp-execution-id-0.0.863985686/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-05-11 07:39:52.000000 vdk-gdp-execution-id-0.0.863985686/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/gdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/gdp/execution_id/
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-05-11 07:39:48.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/gdp/execution_id/gdp_execution_id_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2322 2023-05-11 07:39:48.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/gdp/execution_id/gdp_execution_id_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-05-11 07:40:01.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-11 07:40:01.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 07:40:01.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-05-11 07:40:01.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-11 07:40:01.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-11 07:40:01.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/top_level.txt
```

### Comparing `vdk-gdp-execution-id-0.0.848464550/PKG-INFO` & `vdk-gdp-execution-id-0.0.863985686/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-gdp-execution-id
-Version: 0.0.848464550
+Version: 0.0.863985686
 Summary: This Versatile Data Kit SDK plugin is a Generative Data Pack, that expands each ingested dataset with the execution ID detected during data job run.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -100,7 +100,11 @@
 vdk-plugins/vdk-gdp-execution-id/requirements.txt
 
 Run
 
 ```bash
 pip install -r requirements.txt
 ```
+
+# Example
+
+Find an example data job using `vdk-gdp-execution-id` plugin in [examples/gdp-execution-id-example/](../../../examples/gdp-execution-id-example).
```

### Comparing `vdk-gdp-execution-id-0.0.848464550/README.md` & `vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: vdk-gdp-execution-id
+Version: 0.0.863985686
+Summary: This Versatile Data Kit SDK plugin is a Generative Data Pack, that expands each ingested dataset with the execution ID detected during data job run.
+Home-page: https://github.com/vmware/versatile-data-kit
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
 An installed Generative Data Pack plugin automatically expands the data sent for ingestion.
 
 This GDP plugin detects the execution ID of a Data Job running, and decorates your data product with it. So that,
 it is now possible to correlate a data record with a particular ingestion Data Job execution ID.
 
 **Each ingested dataset gets automatically expanded with a Data Job execution ID micro-dimension.**
 For example:
@@ -86,7 +100,11 @@
 vdk-plugins/vdk-gdp-execution-id/requirements.txt
 
 Run
 
 ```bash
 pip install -r requirements.txt
 ```
+
+# Example
+
+Find an example data job using `vdk-gdp-execution-id` plugin in [examples/gdp-execution-id-example/](../../../examples/gdp-execution-id-example).
```

### Comparing `vdk-gdp-execution-id-0.0.848464550/setup.py` & `vdk-gdp-execution-id-0.0.863985686/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
-__version__ = "0.0.848464550"
+__version__ = "0.0.863985686"
 
 setuptools.setup(
     name="vdk-gdp-execution-id",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="This Versatile Data Kit SDK plugin is a Generative Data Pack, that expands each ingested dataset "
     "with the execution ID detected during data job run.",
```

### Comparing `vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/gdp/execution_id/gdp_execution_id_configuration.py` & `vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/gdp/execution_id/gdp_execution_id_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-gdp-execution-id-0.0.848464550/src/vdk/plugin/gdp/execution_id/gdp_execution_id_plugin.py` & `vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/gdp/execution_id/gdp_execution_id_plugin.py`

 * *Files identical despite different names*

