# Comparing `tmp/terrace-0.0.82.tar.gz` & `tmp/terrace-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrace-0.0.82.tar", last modified: Thu May 11 16:54:53 2023, max compression
+gzip compressed data, was "terrace-0.0.90.tar", last modified: Thu May 11 20:47:17 2023, max compression
```

## Comparing `terrace-0.0.82.tar` & `terrace-0.0.90.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 16:54:53.310071 terrace-0.0.82/
--rw-r--r--   0 boris     (1000) boris     (1001)     1077 2023-05-11 15:23:16.000000 terrace-0.0.82/LICENSE.txt
--rw-r--r--   0 boris     (1000) boris     (1001)     6147 2023-05-11 16:54:53.310071 terrace-0.0.82/PKG-INFO
--rw-r--r--   0 boris     (1000) boris     (1001)     5785 2023-05-11 16:54:52.000000 terrace-0.0.82/README.md
--rw-r--r--   0 boris     (1000) boris     (1001)       38 2023-05-11 16:54:53.310071 terrace-0.0.82/setup.cfg
--rw-r--r--   0 boris     (1000) boris     (1001)      693 2023-05-11 16:54:41.000000 terrace-0.0.82/setup.py
-drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 16:54:53.306738 terrace-0.0.82/src/
-drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 16:54:53.306738 terrace-0.0.82/src/terrace/
--rw-r--r--   0 boris     (1000) boris     (1001)      249 2023-05-11 15:23:16.000000 terrace-0.0.82/src/terrace/__init__.py
--rw-r--r--   0 boris     (1000) boris     (1001)    13436 2023-05-11 15:23:16.000000 terrace-0.0.82/src/terrace/batch.py
--rw-r--r--   0 boris     (1000) boris     (1001)     5773 2023-05-11 16:54:00.000000 terrace-0.0.82/src/terrace/categorical_tensor.py
--rw-r--r--   0 boris     (1000) boris     (1001)     1000 2023-05-11 15:23:16.000000 terrace-0.0.82/src/terrace/dataframe.py
--rw-r--r--   0 boris     (1000) boris     (1001)     9337 2023-05-11 15:23:16.000000 terrace-0.0.82/src/terrace/graph.py
--rw-r--r--   0 boris     (1000) boris     (1001)     2592 2023-05-11 15:23:16.000000 terrace-0.0.82/src/terrace/meta_utils.py
--rw-r--r--   0 boris     (1000) boris     (1001)     5051 2023-05-11 15:23:16.000000 terrace-0.0.82/src/terrace/module.py
-drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 16:54:53.310071 terrace-0.0.82/src/terrace.egg-info/
--rw-r--r--   0 boris     (1000) boris     (1001)     6147 2023-05-11 16:54:53.000000 terrace-0.0.82/src/terrace.egg-info/PKG-INFO
--rw-r--r--   0 boris     (1000) boris     (1001)      377 2023-05-11 16:54:53.000000 terrace-0.0.82/src/terrace.egg-info/SOURCES.txt
--rw-r--r--   0 boris     (1000) boris     (1001)        1 2023-05-11 16:54:53.000000 terrace-0.0.82/src/terrace.egg-info/dependency_links.txt
--rw-r--r--   0 boris     (1000) boris     (1001)       11 2023-05-11 16:54:53.000000 terrace-0.0.82/src/terrace.egg-info/requires.txt
--rw-r--r--   0 boris     (1000) boris     (1001)        8 2023-05-11 16:54:53.000000 terrace-0.0.82/src/terrace.egg-info/top_level.txt
+drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 20:47:17.893788 terrace-0.0.90/
+-rw-r--r--   0 boris     (1000) boris     (1001)     1077 2023-05-11 15:23:16.000000 terrace-0.0.90/LICENSE.txt
+-rw-r--r--   0 boris     (1000) boris     (1001)     6147 2023-05-11 20:47:17.893788 terrace-0.0.90/PKG-INFO
+-rw-r--r--   0 boris     (1000) boris     (1001)     5785 2023-05-11 20:47:17.000000 terrace-0.0.90/README.md
+-rw-r--r--   0 boris     (1000) boris     (1001)       38 2023-05-11 20:47:17.893788 terrace-0.0.90/setup.cfg
+-rw-r--r--   0 boris     (1000) boris     (1001)      693 2023-05-11 20:46:30.000000 terrace-0.0.90/setup.py
+drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 20:47:17.893788 terrace-0.0.90/src/
+drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 20:47:17.893788 terrace-0.0.90/src/terrace/
+-rw-r--r--   0 boris     (1000) boris     (1001)      408 2023-05-11 20:46:06.000000 terrace-0.0.90/src/terrace/__init__.py
+-rw-r--r--   0 boris     (1000) boris     (1001)    13436 2023-05-11 15:23:16.000000 terrace-0.0.90/src/terrace/batch.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     5773 2023-05-11 16:54:00.000000 terrace-0.0.90/src/terrace/categorical_tensor.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     1000 2023-05-11 15:23:16.000000 terrace-0.0.90/src/terrace/dataframe.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     9337 2023-05-11 15:23:16.000000 terrace-0.0.90/src/terrace/graph.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     2592 2023-05-11 15:23:16.000000 terrace-0.0.90/src/terrace/meta_utils.py
+-rw-r--r--   0 boris     (1000) boris     (1001)     5051 2023-05-11 15:23:16.000000 terrace-0.0.90/src/terrace/module.py
+drwxr-xr-x   0 boris     (1000) boris     (1001)        0 2023-05-11 20:47:17.893788 terrace-0.0.90/src/terrace.egg-info/
+-rw-r--r--   0 boris     (1000) boris     (1001)     6147 2023-05-11 20:47:17.000000 terrace-0.0.90/src/terrace.egg-info/PKG-INFO
+-rw-r--r--   0 boris     (1000) boris     (1001)      377 2023-05-11 20:47:17.000000 terrace-0.0.90/src/terrace.egg-info/SOURCES.txt
+-rw-r--r--   0 boris     (1000) boris     (1001)        1 2023-05-11 20:47:17.000000 terrace-0.0.90/src/terrace.egg-info/dependency_links.txt
+-rw-r--r--   0 boris     (1000) boris     (1001)       11 2023-05-11 20:47:17.000000 terrace-0.0.90/src/terrace.egg-info/requires.txt
+-rw-r--r--   0 boris     (1000) boris     (1001)        8 2023-05-11 20:47:17.000000 terrace-0.0.90/src/terrace.egg-info/top_level.txt
```

### Comparing `terrace-0.0.82/LICENSE.txt` & `terrace-0.0.90/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `terrace-0.0.82/PKG-INFO` & `terrace-0.0.90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrace
-Version: 0.0.82
+Version: 0.0.90
 Summary: high level PyTorch utils
 Home-page: https://github.com/mixarcid/terrace
 Author: Michael Brocidiacono
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `terrace-0.0.82/README.md` & `terrace-0.0.90/README.md`

 * *Files identical despite different names*

### Comparing `terrace-0.0.82/setup.py` & `terrace-0.0.90/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name="terrace",
-    version="0.0.82",
+    version="0.0.90",
     author="Michael Brocidiacono",
     author_email="",
     description="high level PyTorch utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mixarcid/terrace",
     packages=setuptools.find_packages(
```

### Comparing `terrace-0.0.82/src/terrace/batch.py` & `terrace-0.0.90/src/terrace/batch.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.82/src/terrace/categorical_tensor.py` & `terrace-0.0.90/src/terrace/categorical_tensor.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.82/src/terrace/dataframe.py` & `terrace-0.0.90/src/terrace/dataframe.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.82/src/terrace/graph.py` & `terrace-0.0.90/src/terrace/graph.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.82/src/terrace/meta_utils.py` & `terrace-0.0.90/src/terrace/meta_utils.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.82/src/terrace/module.py` & `terrace-0.0.90/src/terrace/module.py`

 * *Files identical despite different names*

### Comparing `terrace-0.0.82/src/terrace.egg-info/PKG-INFO` & `terrace-0.0.90/src/terrace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrace
-Version: 0.0.82
+Version: 0.0.90
 Summary: high level PyTorch utils
 Home-page: https://github.com/mixarcid/terrace
 Author: Michael Brocidiacono
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

