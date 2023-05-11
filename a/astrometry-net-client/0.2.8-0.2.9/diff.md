# Comparing `tmp/astrometry_net_client-0.2.8.tar.gz` & `tmp/astrometry_net_client-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrometry_net_client-0.2.8.tar", last modified: Wed Nov  2 19:12:39 2022, max compression
+gzip compressed data, was "astrometry_net_client-0.2.9.tar", last modified: Thu Nov 17 08:24:29 2022, max compression
```

## Comparing `astrometry_net_client-0.2.8.tar` & `astrometry_net_client-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2022-11-02 19:12:39.189401 astrometry_net_client-0.2.8/
--rw-r--r--   0 sten      (1000) sten      (1000)     1067 2022-08-30 07:13:54.000000 astrometry_net_client-0.2.8/LICENSE
--rw-r--r--   0 sten      (1000) sten      (1000)     6277 2022-11-02 19:12:39.189401 astrometry_net_client-0.2.8/PKG-INFO
--rw-r--r--   0 sten      (1000) sten      (1000)     5396 2022-08-30 09:48:22.000000 astrometry_net_client-0.2.8/README.rst
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2022-11-02 19:12:39.189401 astrometry_net_client-0.2.8/astrometry_net_client/
--rw-r--r--   0 sten      (1000) sten      (1000)      345 2022-11-02 18:32:15.000000 astrometry_net_client-0.2.8/astrometry_net_client/__init__.py
--rw-r--r--   0 sten      (1000) sten      (1000)     8994 2022-11-02 18:34:56.000000 astrometry_net_client-0.2.8/astrometry_net_client/client.py
--rw-r--r--   0 sten      (1000) sten      (1000)      448 2022-11-02 18:32:11.000000 astrometry_net_client-0.2.8/astrometry_net_client/config.py
--rw-r--r--   0 sten      (1000) sten      (1000)      663 2022-11-02 18:32:13.000000 astrometry_net_client-0.2.8/astrometry_net_client/exceptions.py
--rw-r--r--   0 sten      (1000) sten      (1000)     6688 2022-11-02 19:09:33.000000 astrometry_net_client-0.2.8/astrometry_net_client/request.py
--rw-r--r--   0 sten      (1000) sten      (1000)     5036 2022-11-02 18:32:23.000000 astrometry_net_client-0.2.8/astrometry_net_client/session.py
--rw-r--r--   0 sten      (1000) sten      (1000)     7743 2022-11-02 18:34:56.000000 astrometry_net_client-0.2.8/astrometry_net_client/settings.py
--rw-r--r--   0 sten      (1000) sten      (1000)    16080 2022-11-02 18:34:56.000000 astrometry_net_client-0.2.8/astrometry_net_client/statusables.py
--rw-r--r--   0 sten      (1000) sten      (1000)     3774 2022-11-02 18:32:30.000000 astrometry_net_client-0.2.8/astrometry_net_client/uploads.py
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2022-11-02 19:12:39.189401 astrometry_net_client-0.2.8/astrometry_net_client.egg-info/
--rw-r--r--   0 sten      (1000) sten      (1000)     6277 2022-11-02 19:12:39.000000 astrometry_net_client-0.2.8/astrometry_net_client.egg-info/PKG-INFO
--rw-r--r--   0 sten      (1000) sten      (1000)      565 2022-11-02 19:12:39.000000 astrometry_net_client-0.2.8/astrometry_net_client.egg-info/SOURCES.txt
--rw-r--r--   0 sten      (1000) sten      (1000)        1 2022-11-02 19:12:39.000000 astrometry_net_client-0.2.8/astrometry_net_client.egg-info/dependency_links.txt
--rw-r--r--   0 sten      (1000) sten      (1000)       17 2022-11-02 19:12:39.000000 astrometry_net_client-0.2.8/astrometry_net_client.egg-info/requires.txt
--rw-r--r--   0 sten      (1000) sten      (1000)       22 2022-11-02 19:12:39.000000 astrometry_net_client-0.2.8/astrometry_net_client.egg-info/top_level.txt
--rw-r--r--   0 sten      (1000) sten      (1000)      128 2022-11-02 19:12:39.192734 astrometry_net_client-0.2.8/setup.cfg
--rw-r--r--   0 sten      (1000) sten      (1000)     1140 2022-11-02 19:12:03.000000 astrometry_net_client-0.2.8/setup.py
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2022-11-17 08:24:29.592383 astrometry_net_client-0.2.9/
+-rw-r--r--   0 sten      (1000) sten      (1000)     1067 2022-08-30 07:13:54.000000 astrometry_net_client-0.2.9/LICENSE
+-rw-r--r--   0 sten      (1000) sten      (1000)     6277 2022-11-17 08:24:29.592383 astrometry_net_client-0.2.9/PKG-INFO
+-rw-r--r--   0 sten      (1000) sten      (1000)     5396 2022-08-30 09:48:22.000000 astrometry_net_client-0.2.9/README.rst
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2022-11-17 08:24:29.592383 astrometry_net_client-0.2.9/astrometry_net_client/
+-rw-r--r--   0 sten      (1000) sten      (1000)      345 2022-11-02 18:32:15.000000 astrometry_net_client-0.2.9/astrometry_net_client/__init__.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     8994 2022-11-02 18:34:56.000000 astrometry_net_client-0.2.9/astrometry_net_client/client.py
+-rw-r--r--   0 sten      (1000) sten      (1000)      448 2022-11-02 18:32:11.000000 astrometry_net_client-0.2.9/astrometry_net_client/config.py
+-rw-r--r--   0 sten      (1000) sten      (1000)      663 2022-11-02 18:32:13.000000 astrometry_net_client-0.2.9/astrometry_net_client/exceptions.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     6688 2022-11-02 19:09:33.000000 astrometry_net_client-0.2.9/astrometry_net_client/request.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     5036 2022-11-02 18:32:23.000000 astrometry_net_client-0.2.9/astrometry_net_client/session.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     7743 2022-11-02 18:34:56.000000 astrometry_net_client-0.2.9/astrometry_net_client/settings.py
+-rw-r--r--   0 sten      (1000) sten      (1000)    16080 2022-11-02 18:34:56.000000 astrometry_net_client-0.2.9/astrometry_net_client/statusables.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     3774 2022-11-02 18:32:30.000000 astrometry_net_client-0.2.9/astrometry_net_client/uploads.py
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2022-11-17 08:24:29.592383 astrometry_net_client-0.2.9/astrometry_net_client.egg-info/
+-rw-r--r--   0 sten      (1000) sten      (1000)     6277 2022-11-17 08:24:29.000000 astrometry_net_client-0.2.9/astrometry_net_client.egg-info/PKG-INFO
+-rw-r--r--   0 sten      (1000) sten      (1000)      565 2022-11-17 08:24:29.000000 astrometry_net_client-0.2.9/astrometry_net_client.egg-info/SOURCES.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)        1 2022-11-17 08:24:29.000000 astrometry_net_client-0.2.9/astrometry_net_client.egg-info/dependency_links.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)       17 2022-11-17 08:24:29.000000 astrometry_net_client-0.2.9/astrometry_net_client.egg-info/requires.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)       22 2022-11-17 08:24:29.000000 astrometry_net_client-0.2.9/astrometry_net_client.egg-info/top_level.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)      128 2022-11-17 08:24:29.592383 astrometry_net_client-0.2.9/setup.cfg
+-rw-r--r--   0 sten      (1000) sten      (1000)     1140 2022-11-17 08:17:40.000000 astrometry_net_client-0.2.9/setup.py
```

### Comparing `astrometry_net_client-0.2.8/LICENSE` & `astrometry_net_client-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.8/PKG-INFO` & `astrometry_net_client-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrometry_net_client
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Python interface for the Astrometry.net API.
 Home-page: https://github.com/StenSipma/astrometry_net_client
 Author: Sten Sipma
 Author-email: sten.sipma@ziggo.nl
 Keywords: astronomy astrometry client coordinates wcs api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `astrometry_net_client-0.2.8/README.rst` & `astrometry_net_client-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.8/astrometry_net_client/client.py` & `astrometry_net_client-0.2.9/astrometry_net_client/client.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.8/astrometry_net_client/exceptions.py` & `astrometry_net_client-0.2.9/astrometry_net_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.8/astrometry_net_client/request.py` & `astrometry_net_client-0.2.9/astrometry_net_client/request.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.8/astrometry_net_client/session.py` & `astrometry_net_client-0.2.9/astrometry_net_client/session.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.8/astrometry_net_client/settings.py` & `astrometry_net_client-0.2.9/astrometry_net_client/settings.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.8/astrometry_net_client/statusables.py` & `astrometry_net_client-0.2.9/astrometry_net_client/statusables.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.8/astrometry_net_client/uploads.py` & `astrometry_net_client-0.2.9/astrometry_net_client/uploads.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.8/astrometry_net_client.egg-info/PKG-INFO` & `astrometry_net_client-0.2.9/astrometry_net_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrometry-net-client
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Python interface for the Astrometry.net API.
 Home-page: https://github.com/StenSipma/astrometry_net_client
 Author: Sten Sipma
 Author-email: sten.sipma@ziggo.nl
 Keywords: astronomy astrometry client coordinates wcs api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `astrometry_net_client-0.2.8/astrometry_net_client.egg-info/SOURCES.txt` & `astrometry_net_client-0.2.9/astrometry_net_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.8/setup.py` & `astrometry_net_client-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="astrometry_net_client",
-    version="0.2.8",
+    version="0.2.9",
     author="Sten Sipma",
     author_email="sten.sipma@ziggo.nl",
     description="A Python interface for the Astrometry.net API.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/StenSipma/astrometry_net_client",
     packages=["astrometry_net_client"],
```

