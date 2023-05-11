# Comparing `tmp/CxAdmin-1.0.8.tar.gz` & `tmp/CxAdmin-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CxAdmin-1.0.8.tar", last modified: Mon Jan  9 13:23:38 2023, max compression
+gzip compressed data, was "CxAdmin-1.0.9.tar", last modified: Tue Jan 10 12:57:26 2023, max compression
```

## Comparing `CxAdmin-1.0.8.tar` & `CxAdmin-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 felixweber   (501) staff       (20)        0 2023-01-09 13:23:38.769035 CxAdmin-1.0.8/
--rw-r--r--   0 felixweber   (501) staff       (20)     2303 2023-01-09 13:23:38.769143 CxAdmin-1.0.8/PKG-INFO
--rw-r--r--   0 felixweber   (501) staff       (20)      103 2023-01-03 14:29:32.000000 CxAdmin-1.0.8/pyproject.toml
--rw-r--r--   0 felixweber   (501) staff       (20)      574 2023-01-09 13:23:38.769457 CxAdmin-1.0.8/setup.cfg
-drwxr-xr-x   0 felixweber   (501) staff       (20)        0 2023-01-09 13:23:38.763996 CxAdmin-1.0.8/src/
-drwxr-xr-x   0 felixweber   (501) staff       (20)        0 2023-01-09 13:23:38.764186 CxAdmin-1.0.8/src/CxAdmin/
-drwxr-xr-x   0 felixweber   (501) staff       (20)        0 2023-01-09 13:23:38.765288 CxAdmin-1.0.8/src/CxAdmin/CxAdmin.egg-info/
--rw-r--r--   0 felixweber   (501) staff       (20)     2303 2023-01-09 13:23:38.000000 CxAdmin-1.0.8/src/CxAdmin/CxAdmin.egg-info/PKG-INFO
--rw-r--r--   0 felixweber   (501) staff       (20)      505 2023-01-09 13:23:38.000000 CxAdmin-1.0.8/src/CxAdmin/CxAdmin.egg-info/SOURCES.txt
--rw-r--r--   0 felixweber   (501) staff       (20)        1 2023-01-09 13:23:38.000000 CxAdmin-1.0.8/src/CxAdmin/CxAdmin.egg-info/dependency_links.txt
--rw-r--r--   0 felixweber   (501) staff       (20)        4 2023-01-09 13:23:38.000000 CxAdmin-1.0.8/src/CxAdmin/CxAdmin.egg-info/top_level.txt
-drwxr-xr-x   0 felixweber   (501) staff       (20)        0 2023-01-09 13:23:38.767678 CxAdmin-1.0.8/src/CxAdmin/api/
--rw-r--r--   0 felixweber   (501) staff       (20)        0 2022-10-14 15:05:56.000000 CxAdmin-1.0.8/src/CxAdmin/api/__init__.py
--rw-r--r--   0 felixweber   (501) staff       (20)      230 2023-01-09 13:14:54.000000 CxAdmin-1.0.8/src/CxAdmin/api/cxEnvironment.py
--rw-r--r--   0 felixweber   (501) staff       (20)      236 2023-01-09 13:14:54.000000 CxAdmin-1.0.8/src/CxAdmin/api/cxFlows.py
--rw-r--r--   0 felixweber   (501) staff       (20)      259 2023-01-09 13:14:54.000000 CxAdmin-1.0.8/src/CxAdmin/api/cxItem.py
--rw-r--r--   0 felixweber   (501) staff       (20)     2469 2023-01-09 13:14:36.000000 CxAdmin-1.0.8/src/CxAdmin/api/cxLists.py
--rw-r--r--   0 felixweber   (501) staff       (20)      339 2023-01-09 13:14:54.000000 CxAdmin-1.0.8/src/CxAdmin/api/cxQueues.py
--rw-r--r--   0 felixweber   (501) staff       (20)      171 2023-01-09 13:14:54.000000 CxAdmin-1.0.8/src/CxAdmin/api/cxStatistics.py
-drwxr-xr-x   0 felixweber   (501) staff       (20)        0 2023-01-09 13:23:38.768683 CxAdmin-1.0.8/src/CxAdmin/api/http/
--rw-r--r--   0 felixweber   (501) staff       (20)        0 2023-01-09 12:12:25.000000 CxAdmin-1.0.8/src/CxAdmin/api/http/__init__.py
--rw-r--r--   0 felixweber   (501) staff       (20)      551 2022-10-18 14:29:57.000000 CxAdmin-1.0.8/src/CxAdmin/api/http/httpClientModel.py
--rw-r--r--   0 felixweber   (501) staff       (20)     2348 2023-01-09 13:14:54.000000 CxAdmin-1.0.8/src/CxAdmin/api/http/httpclient.py
+drwxr-xr-x   0 felixweber   (501) staff       (20)        0 2023-01-10 12:57:26.079278 CxAdmin-1.0.9/
+-rw-r--r--   0 felixweber   (501) staff       (20)     2303 2023-01-10 12:57:26.079359 CxAdmin-1.0.9/PKG-INFO
+-rw-r--r--   0 felixweber   (501) staff       (20)      103 2023-01-03 14:29:32.000000 CxAdmin-1.0.9/pyproject.toml
+-rw-r--r--   0 felixweber   (501) staff       (20)      574 2023-01-10 12:57:26.079650 CxAdmin-1.0.9/setup.cfg
+drwxr-xr-x   0 felixweber   (501) staff       (20)        0 2023-01-10 12:57:26.076324 CxAdmin-1.0.9/src/
+drwxr-xr-x   0 felixweber   (501) staff       (20)        0 2023-01-10 12:57:26.076488 CxAdmin-1.0.9/src/CxAdmin/
+drwxr-xr-x   0 felixweber   (501) staff       (20)        0 2023-01-10 12:57:26.077673 CxAdmin-1.0.9/src/CxAdmin/CxAdmin.egg-info/
+-rw-r--r--   0 felixweber   (501) staff       (20)     2303 2023-01-10 12:57:26.000000 CxAdmin-1.0.9/src/CxAdmin/CxAdmin.egg-info/PKG-INFO
+-rw-r--r--   0 felixweber   (501) staff       (20)      505 2023-01-10 12:57:26.000000 CxAdmin-1.0.9/src/CxAdmin/CxAdmin.egg-info/SOURCES.txt
+-rw-r--r--   0 felixweber   (501) staff       (20)        1 2023-01-10 12:57:26.000000 CxAdmin-1.0.9/src/CxAdmin/CxAdmin.egg-info/dependency_links.txt
+-rw-r--r--   0 felixweber   (501) staff       (20)        4 2023-01-10 12:57:26.000000 CxAdmin-1.0.9/src/CxAdmin/CxAdmin.egg-info/top_level.txt
+drwxr-xr-x   0 felixweber   (501) staff       (20)        0 2023-01-10 12:57:26.078724 CxAdmin-1.0.9/src/CxAdmin/api/
+-rw-r--r--   0 felixweber   (501) staff       (20)        0 2022-10-14 15:05:56.000000 CxAdmin-1.0.9/src/CxAdmin/api/__init__.py
+-rw-r--r--   0 felixweber   (501) staff       (20)      230 2023-01-09 13:14:54.000000 CxAdmin-1.0.9/src/CxAdmin/api/cxEnvironment.py
+-rw-r--r--   0 felixweber   (501) staff       (20)      236 2023-01-09 13:14:54.000000 CxAdmin-1.0.9/src/CxAdmin/api/cxFlows.py
+-rw-r--r--   0 felixweber   (501) staff       (20)      259 2023-01-09 13:14:54.000000 CxAdmin-1.0.9/src/CxAdmin/api/cxItem.py
+-rw-r--r--   0 felixweber   (501) staff       (20)     2469 2023-01-09 13:14:36.000000 CxAdmin-1.0.9/src/CxAdmin/api/cxLists.py
+-rw-r--r--   0 felixweber   (501) staff       (20)      339 2023-01-09 13:14:54.000000 CxAdmin-1.0.9/src/CxAdmin/api/cxQueues.py
+-rw-r--r--   0 felixweber   (501) staff       (20)      171 2023-01-09 13:14:54.000000 CxAdmin-1.0.9/src/CxAdmin/api/cxStatistics.py
+drwxr-xr-x   0 felixweber   (501) staff       (20)        0 2023-01-10 12:57:26.079143 CxAdmin-1.0.9/src/CxAdmin/api/http/
+-rw-r--r--   0 felixweber   (501) staff       (20)        0 2023-01-09 12:12:25.000000 CxAdmin-1.0.9/src/CxAdmin/api/http/__init__.py
+-rw-r--r--   0 felixweber   (501) staff       (20)      551 2022-10-18 14:29:57.000000 CxAdmin-1.0.9/src/CxAdmin/api/http/httpClientModel.py
+-rw-r--r--   0 felixweber   (501) staff       (20)     2348 2023-01-09 13:14:54.000000 CxAdmin-1.0.9/src/CxAdmin/api/http/httpclient.py
```

### Comparing `CxAdmin-1.0.8/PKG-INFO` & `CxAdmin-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CxAdmin
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python SDK for interacting with the CxEngage API
 Home-page: https://github.com/ntflix/cxadmin
 Author: Felix Weber
 Author-email: felix@iron59.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `CxAdmin-1.0.8/setup.cfg` & `CxAdmin-1.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CxAdmin
-version = 1.0.8
+version = 1.0.9
 author = Felix Weber
 author_email = felix@iron59.co.uk
 description = Python SDK for interacting with the CxEngage API
 long_description = file: readme.md
 long_description_content_type = text/markdown
 readme = file: readme.md
 url = https://github.com/ntflix/cxadmin
```

### Comparing `CxAdmin-1.0.8/src/CxAdmin/CxAdmin.egg-info/PKG-INFO` & `CxAdmin-1.0.9/src/CxAdmin/CxAdmin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CxAdmin
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python SDK for interacting with the CxEngage API
 Home-page: https://github.com/ntflix/cxadmin
 Author: Felix Weber
 Author-email: felix@iron59.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `CxAdmin-1.0.8/src/CxAdmin/api/cxLists.py` & `CxAdmin-1.0.9/src/CxAdmin/api/cxLists.py`

 * *Files identical despite different names*

### Comparing `CxAdmin-1.0.8/src/CxAdmin/api/http/httpClientModel.py` & `CxAdmin-1.0.9/src/CxAdmin/api/http/httpClientModel.py`

 * *Files identical despite different names*

### Comparing `CxAdmin-1.0.8/src/CxAdmin/api/http/httpclient.py` & `CxAdmin-1.0.9/src/CxAdmin/api/http/httpclient.py`

 * *Files identical despite different names*

