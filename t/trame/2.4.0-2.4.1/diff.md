# Comparing `tmp/trame-2.4.0.tar.gz` & `tmp/trame-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-2.4.0.tar", last modified: Tue Apr 25 15:55:15 2023, max compression
+gzip compressed data, was "trame-2.4.1.tar", last modified: Thu May 11 01:48:09 2023, max compression
```

## Comparing `trame-2.4.0.tar` & `trame-2.4.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:55:15.697538 trame-2.4.0/
--rw-r--r--   0 root         (0) root         (0)      552 2023-04-25 15:55:10.000000 trame-2.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-25 15:55:10.000000 trame-2.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6855 2023-04-25 15:55:15.697538 trame-2.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6117 2023-04-25 15:55:10.000000 trame-2.4.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     1151 2023-04-25 15:55:15.697538 trame-2.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 15:55:11.000000 trame-2.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:55:15.689538 trame-2.4.0/trame/
--rw-r--r--   0 root         (0) root         (0)      552 2023-04-25 15:55:10.000000 trame-2.4.0/trame/LICENSE
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-25 15:55:11.000000 trame-2.4.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:55:15.693538 trame-2.4.0/trame/app/
--rw-r--r--   0 root         (0) root         (0)     2388 2023-04-25 15:55:11.000000 trame-2.4.0/trame/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      271 2023-04-25 15:55:11.000000 trame-2.4.0/trame/app/asynchronous.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-04-25 15:55:11.000000 trame-2.4.0/trame/app/dev.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-04-25 15:55:11.000000 trame-2.4.0/trame/app/file_upload.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-04-25 15:55:11.000000 trame-2.4.0/trame/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-04-25 15:55:11.000000 trame-2.4.0/trame/app/mimetypes.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-04-25 15:55:11.000000 trame-2.4.0/trame/app/singleton.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-04-25 15:55:11.000000 trame-2.4.0/trame/app/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:55:15.693538 trame-2.4.0/trame/assets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 15:55:11.000000 trame-2.4.0/trame/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4337 2023-04-25 15:55:11.000000 trame-2.4.0/trame/assets/local.py
--rw-r--r--   0 root         (0) root         (0)     4362 2023-04-25 15:55:11.000000 trame-2.4.0/trame/assets/remote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:55:15.693538 trame-2.4.0/trame/env/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 15:55:11.000000 trame-2.4.0/trame/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-04-25 15:55:11.000000 trame-2.4.0/trame/env/paraview.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-04-25 15:55:11.000000 trame-2.4.0/trame/env/utils.py
--rw-r--r--   0 root         (0) root         (0)     1311 2023-04-25 15:55:11.000000 trame-2.4.0/trame/env/venv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:55:15.697538 trame-2.4.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 15:55:11.000000 trame-2.4.0/trame/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:55:15.697538 trame-2.4.0/trame/tools/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 15:55:11.000000 trame-2.4.0/trame/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-04-25 15:55:11.000000 trame-2.4.0/trame/tools/app.py
--rw-r--r--   0 root         (0) root         (0)     2926 2023-04-25 15:55:11.000000 trame-2.4.0/trame/tools/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:55:15.697538 trame-2.4.0/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-25 15:55:11.000000 trame-2.4.0/trame/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:55:15.697538 trame-2.4.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 15:55:11.000000 trame-2.4.0/trame/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:55:15.689538 trame-2.4.0/trame.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6855 2023-04-25 15:55:15.000000 trame-2.4.0/trame.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      689 2023-04-25 15:55:15.000000 trame-2.4.0/trame.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 15:55:15.000000 trame-2.4.0/trame.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      260 2023-04-25 15:55:15.000000 trame-2.4.0/trame.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-25 15:55:15.000000 trame-2.4.0/trame.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:48:09.079681 trame-2.4.1/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-11 01:48:05.000000 trame-2.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-11 01:48:05.000000 trame-2.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6855 2023-05-11 01:48:09.079681 trame-2.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6117 2023-05-11 01:48:05.000000 trame-2.4.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-05-11 01:48:09.079681 trame-2.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 01:48:05.000000 trame-2.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:48:09.067680 trame-2.4.1/trame/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-11 01:48:05.000000 trame-2.4.1/trame/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-11 01:48:05.000000 trame-2.4.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:48:09.075681 trame-2.4.1/trame/app/
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-05-11 01:48:05.000000 trame-2.4.1/trame/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-05-11 01:48:05.000000 trame-2.4.1/trame/app/asynchronous.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-05-11 01:48:05.000000 trame-2.4.1/trame/app/cone.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-05-11 01:48:05.000000 trame-2.4.1/trame/app/dev.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-11 01:48:05.000000 trame-2.4.1/trame/app/file_upload.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-05-11 01:48:05.000000 trame-2.4.1/trame/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-05-11 01:48:05.000000 trame-2.4.1/trame/app/mimetypes.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-05-11 01:48:05.000000 trame-2.4.1/trame/app/singleton.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-05-11 01:48:05.000000 trame-2.4.1/trame/app/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:48:09.075681 trame-2.4.1/trame/assets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 01:48:05.000000 trame-2.4.1/trame/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4337 2023-05-11 01:48:05.000000 trame-2.4.1/trame/assets/local.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2023-05-11 01:48:05.000000 trame-2.4.1/trame/assets/remote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:48:09.079681 trame-2.4.1/trame/env/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 01:48:05.000000 trame-2.4.1/trame/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-05-11 01:48:05.000000 trame-2.4.1/trame/env/paraview.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-05-11 01:48:05.000000 trame-2.4.1/trame/env/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-05-11 01:48:05.000000 trame-2.4.1/trame/env/venv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:48:09.079681 trame-2.4.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 01:48:05.000000 trame-2.4.1/trame/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:48:09.079681 trame-2.4.1/trame/tools/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 01:48:05.000000 trame-2.4.1/trame/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-05-11 01:48:05.000000 trame-2.4.1/trame/tools/app.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-05-11 01:48:05.000000 trame-2.4.1/trame/tools/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:48:09.079681 trame-2.4.1/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-11 01:48:05.000000 trame-2.4.1/trame/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:48:09.079681 trame-2.4.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 01:48:05.000000 trame-2.4.1/trame/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 01:48:09.071680 trame-2.4.1/trame.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6855 2023-05-11 01:48:09.000000 trame-2.4.1/trame.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      707 2023-05-11 01:48:09.000000 trame-2.4.1/trame.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 01:48:09.000000 trame-2.4.1/trame.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      260 2023-05-11 01:48:09.000000 trame-2.4.1/trame.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-11 01:48:09.000000 trame-2.4.1/trame.egg-info/top_level.txt
```

### Comparing `trame-2.4.0/LICENSE` & `trame-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/PKG-INFO` & `trame-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 2.4.0
+Version: 2.4.1
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-2.4.0/README.rst` & `trame-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/setup.cfg` & `trame-2.4.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame
-version = 2.4.0
+version = 2.4.1
 description = Trame, a framework to build applications in plain Python
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache License 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-2.4.0/trame/LICENSE` & `trame-2.4.1/trame/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/app/__init__.py` & `trame-2.4.1/trame/app/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/app/dev.py` & `trame-2.4.1/trame/app/dev.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/app/file_upload.py` & `trame-2.4.1/trame/app/file_upload.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/app/jupyter.py` & `trame-2.4.1/trame/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/app/mimetypes.py` & `trame-2.4.1/trame/app/mimetypes.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/app/singleton.py` & `trame-2.4.1/trame/app/singleton.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/app/testing.py` & `trame-2.4.1/trame/app/testing.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/assets/local.py` & `trame-2.4.1/trame/assets/local.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/assets/remote.py` & `trame-2.4.1/trame/assets/remote.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/env/paraview.py` & `trame-2.4.1/trame/env/paraview.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/env/utils.py` & `trame-2.4.1/trame/env/utils.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/env/venv.py` & `trame-2.4.1/trame/env/venv.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/tools/app.py` & `trame-2.4.1/trame/tools/app.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame/tools/www.py` & `trame-2.4.1/trame/tools/www.py`

 * *Files identical despite different names*

### Comparing `trame-2.4.0/trame.egg-info/PKG-INFO` & `trame-2.4.1/trame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 2.4.0
+Version: 2.4.1
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-2.4.0/trame.egg-info/SOURCES.txt` & `trame-2.4.1/trame.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 trame.egg-info/PKG-INFO
 trame.egg-info/SOURCES.txt
 trame.egg-info/dependency_links.txt
 trame.egg-info/requires.txt
 trame.egg-info/top_level.txt
 trame/app/__init__.py
 trame/app/asynchronous.py
+trame/app/cone.py
 trame/app/dev.py
 trame/app/file_upload.py
 trame/app/jupyter.py
 trame/app/mimetypes.py
 trame/app/singleton.py
 trame/app/testing.py
 trame/assets/__init__.py
```

