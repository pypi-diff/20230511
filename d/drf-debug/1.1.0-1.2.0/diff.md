# Comparing `tmp/drf-debug-1.1.0.tar.gz` & `tmp/drf-debug-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-debug-1.1.0.tar", last modified: Thu May 11 18:14:50 2023, max compression
+gzip compressed data, was "drf-debug-1.2.0.tar", last modified: Thu May 11 18:22:46 2023, max compression
```

## Comparing `drf-debug-1.1.0.tar` & `drf-debug-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 dori      (1000) dori      (1001)        0 2023-05-11 18:14:50.473057 drf-debug-1.1.0/
--rw-r--r--   0 dori      (1000) dori      (1001)     2732 2023-05-11 18:14:50.473057 drf-debug-1.1.0/PKG-INFO
--rw-r--r--   0 dori      (1000) dori      (1001)     2318 2023-05-11 18:11:17.000000 drf-debug-1.1.0/README.md
-drwxr-xr-x   0 dori      (1000) dori      (1001)        0 2023-05-11 18:14:50.469724 drf-debug-1.1.0/drf_debug.egg-info/
--rw-r--r--   0 dori      (1000) dori      (1001)     2732 2023-05-11 18:14:50.000000 drf-debug-1.1.0/drf_debug.egg-info/PKG-INFO
--rw-r--r--   0 dori      (1000) dori      (1001)      561 2023-05-11 18:14:50.000000 drf-debug-1.1.0/drf_debug.egg-info/SOURCES.txt
--rw-r--r--   0 dori      (1000) dori      (1001)        1 2023-05-11 18:14:50.000000 drf-debug-1.1.0/drf_debug.egg-info/dependency_links.txt
--rw-r--r--   0 dori      (1000) dori      (1001)       38 2023-05-11 18:14:50.000000 drf-debug-1.1.0/drf_debug.egg-info/requires.txt
--rw-r--r--   0 dori      (1000) dori      (1001)        9 2023-05-11 18:14:50.000000 drf-debug-1.1.0/drf_debug.egg-info/top_level.txt
--rw-r--r--   0 dori      (1000) dori      (1001)      936 2023-05-11 18:14:50.473057 drf-debug-1.1.0/setup.cfg
--rw-r--r--   0 dori      (1000) dori      (1001)      747 2023-05-11 18:13:32.000000 drf-debug-1.1.0/setup.py
-drwxr-xr-x   0 dori      (1000) dori      (1001)        0 2023-05-11 18:14:50.473057 drf-debug-1.1.0/tracking/
--rw-r--r--   0 dori      (1000) dori      (1001)        0 2023-05-10 08:14:40.000000 drf-debug-1.1.0/tracking/__init__.py
--rw-r--r--   0 dori      (1000) dori      (1001)      604 2023-05-10 09:15:37.000000 drf-debug-1.1.0/tracking/admin.py
--rw-r--r--   0 dori      (1000) dori      (1001)      450 2023-05-10 16:12:59.000000 drf-debug-1.1.0/tracking/app_settings.py
--rw-r--r--   0 dori      (1000) dori      (1001)      148 2023-05-10 08:14:40.000000 drf-debug-1.1.0/tracking/apps.py
--rw-r--r--   0 dori      (1000) dori      (1001)     3839 2023-05-11 14:18:36.000000 drf-debug-1.1.0/tracking/base_mixins.py
--rw-r--r--   0 dori      (1000) dori      (1001)     1947 2023-05-10 09:21:55.000000 drf-debug-1.1.0/tracking/base_models.py
-drwxr-xr-x   0 dori      (1000) dori      (1001)        0 2023-05-11 18:14:50.473057 drf-debug-1.1.0/tracking/migrations/
--rw-r--r--   0 dori      (1000) dori      (1001)     2087 2023-05-10 09:22:32.000000 drf-debug-1.1.0/tracking/migrations/0001_initial.py
--rw-r--r--   0 dori      (1000) dori      (1001)        0 2023-05-10 09:22:32.000000 drf-debug-1.1.0/tracking/migrations/__init__.py
--rw-r--r--   0 dori      (1000) dori      (1001)      270 2023-05-10 18:19:32.000000 drf-debug-1.1.0/tracking/mixins.py
--rw-r--r--   0 dori      (1000) dori      (1001)      102 2023-05-10 09:08:13.000000 drf-debug-1.1.0/tracking/models.py
-drwxr-xr-x   0 dori      (1000) dori      (1001)        0 2023-05-11 18:14:50.473057 drf-debug-1.1.0/tracking/tests/
--rw-r--r--   0 dori      (1000) dori      (1001)        0 2023-05-10 19:05:58.000000 drf-debug-1.1.0/tracking/tests/__init__.py
--rw-r--r--   0 dori      (1000) dori      (1001)     5933 2023-05-11 14:26:01.000000 drf-debug-1.1.0/tracking/tests/test_mixins.py
--rw-r--r--   0 dori      (1000) dori      (1001)     4793 2023-05-11 17:23:37.000000 drf-debug-1.1.0/tracking/tests/test_models.py
--rw-r--r--   0 dori      (1000) dori      (1001)      545 2023-05-11 07:05:46.000000 drf-debug-1.1.0/tracking/tests/urls.py
--rw-r--r--   0 dori      (1000) dori      (1001)     1610 2023-05-11 07:05:40.000000 drf-debug-1.1.0/tracking/tests/views.py
+drwxr-xr-x   0 dori      (1000) dori      (1001)        0 2023-05-11 18:22:46.569337 drf-debug-1.2.0/
+-rw-r--r--   0 dori      (1000) dori      (1001)     2732 2023-05-11 18:22:46.569337 drf-debug-1.2.0/PKG-INFO
+-rw-r--r--   0 dori      (1000) dori      (1001)     2318 2023-05-11 18:11:17.000000 drf-debug-1.2.0/README.md
+drwxr-xr-x   0 dori      (1000) dori      (1001)        0 2023-05-11 18:22:46.556004 drf-debug-1.2.0/drf_debug.egg-info/
+-rw-r--r--   0 dori      (1000) dori      (1001)     2732 2023-05-11 18:22:46.000000 drf-debug-1.2.0/drf_debug.egg-info/PKG-INFO
+-rw-r--r--   0 dori      (1000) dori      (1001)      561 2023-05-11 18:22:46.000000 drf-debug-1.2.0/drf_debug.egg-info/SOURCES.txt
+-rw-r--r--   0 dori      (1000) dori      (1001)        1 2023-05-11 18:22:46.000000 drf-debug-1.2.0/drf_debug.egg-info/dependency_links.txt
+-rw-r--r--   0 dori      (1000) dori      (1001)       38 2023-05-11 18:22:46.000000 drf-debug-1.2.0/drf_debug.egg-info/requires.txt
+-rw-r--r--   0 dori      (1000) dori      (1001)        9 2023-05-11 18:22:46.000000 drf-debug-1.2.0/drf_debug.egg-info/top_level.txt
+-rw-r--r--   0 dori      (1000) dori      (1001)      936 2023-05-11 18:22:46.569337 drf-debug-1.2.0/setup.cfg
+-rw-r--r--   0 dori      (1000) dori      (1001)      747 2023-05-11 18:22:30.000000 drf-debug-1.2.0/setup.py
+drwxr-xr-x   0 dori      (1000) dori      (1001)        0 2023-05-11 18:22:46.556004 drf-debug-1.2.0/tracking/
+-rw-r--r--   0 dori      (1000) dori      (1001)        0 2023-05-10 08:14:40.000000 drf-debug-1.2.0/tracking/__init__.py
+-rw-r--r--   0 dori      (1000) dori      (1001)      604 2023-05-10 09:15:37.000000 drf-debug-1.2.0/tracking/admin.py
+-rw-r--r--   0 dori      (1000) dori      (1001)      450 2023-05-10 16:12:59.000000 drf-debug-1.2.0/tracking/app_settings.py
+-rw-r--r--   0 dori      (1000) dori      (1001)      148 2023-05-10 08:14:40.000000 drf-debug-1.2.0/tracking/apps.py
+-rw-r--r--   0 dori      (1000) dori      (1001)     3839 2023-05-11 14:18:36.000000 drf-debug-1.2.0/tracking/base_mixins.py
+-rw-r--r--   0 dori      (1000) dori      (1001)     1947 2023-05-10 09:21:55.000000 drf-debug-1.2.0/tracking/base_models.py
+drwxr-xr-x   0 dori      (1000) dori      (1001)        0 2023-05-11 18:22:46.559337 drf-debug-1.2.0/tracking/migrations/
+-rw-r--r--   0 dori      (1000) dori      (1001)     2087 2023-05-10 09:22:32.000000 drf-debug-1.2.0/tracking/migrations/0001_initial.py
+-rw-r--r--   0 dori      (1000) dori      (1001)        0 2023-05-10 09:22:32.000000 drf-debug-1.2.0/tracking/migrations/__init__.py
+-rw-r--r--   0 dori      (1000) dori      (1001)      270 2023-05-10 18:19:32.000000 drf-debug-1.2.0/tracking/mixins.py
+-rw-r--r--   0 dori      (1000) dori      (1001)      102 2023-05-10 09:08:13.000000 drf-debug-1.2.0/tracking/models.py
+drwxr-xr-x   0 dori      (1000) dori      (1001)        0 2023-05-11 18:22:46.569337 drf-debug-1.2.0/tracking/tests/
+-rw-r--r--   0 dori      (1000) dori      (1001)        0 2023-05-10 19:05:58.000000 drf-debug-1.2.0/tracking/tests/__init__.py
+-rw-r--r--   0 dori      (1000) dori      (1001)     5933 2023-05-11 14:26:01.000000 drf-debug-1.2.0/tracking/tests/test_mixins.py
+-rw-r--r--   0 dori      (1000) dori      (1001)     4793 2023-05-11 17:23:37.000000 drf-debug-1.2.0/tracking/tests/test_models.py
+-rw-r--r--   0 dori      (1000) dori      (1001)      545 2023-05-11 07:05:46.000000 drf-debug-1.2.0/tracking/tests/urls.py
+-rw-r--r--   0 dori      (1000) dori      (1001)     1610 2023-05-11 07:05:40.000000 drf-debug-1.2.0/tracking/tests/views.py
```

### Comparing `drf-debug-1.1.0/PKG-INFO` & `drf-debug-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-debug
-Version: 1.1.0
+Version: 1.2.0
 Summary: API tracking package.
 Home-page: https://github.com/dori-dev/drf-debug
 Author: Mohammad Dori
 Author-email: mr.dori.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `drf-debug-1.1.0/README.md` & `drf-debug-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drf-debug-1.1.0/drf_debug.egg-info/PKG-INFO` & `drf-debug-1.2.0/drf_debug.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-debug
-Version: 1.1.0
+Version: 1.2.0
 Summary: API tracking package.
 Home-page: https://github.com/dori-dev/drf-debug
 Author: Mohammad Dori
 Author-email: mr.dori.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `drf-debug-1.1.0/drf_debug.egg-info/SOURCES.txt` & `drf-debug-1.2.0/drf_debug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-debug-1.1.0/setup.cfg` & `drf-debug-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-debug
-version = 1.1.0
+version = 1.2.0
 description = API tracking package.
 long_description = file:README.md
 url = https://github.com/dori-dev/def-debug
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

### Comparing `drf-debug-1.1.0/setup.py` & `drf-debug-1.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="drf-debug",
-    version="1.1.0",
+    version="1.2.0",
     author="Mohammad Dori",
     author_email="mr.dori.dev@gmail.com",
     description="API tracking package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dori-dev/drf-debug",
     classifiers=[
```

### Comparing `drf-debug-1.1.0/tracking/admin.py` & `drf-debug-1.2.0/tracking/admin.py`

 * *Files identical despite different names*

### Comparing `drf-debug-1.1.0/tracking/base_mixins.py` & `drf-debug-1.2.0/tracking/base_mixins.py`

 * *Files identical despite different names*

### Comparing `drf-debug-1.1.0/tracking/base_models.py` & `drf-debug-1.2.0/tracking/base_models.py`

 * *Files identical despite different names*

### Comparing `drf-debug-1.1.0/tracking/migrations/0001_initial.py` & `drf-debug-1.2.0/tracking/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-debug-1.1.0/tracking/tests/test_mixins.py` & `drf-debug-1.2.0/tracking/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `drf-debug-1.1.0/tracking/tests/test_models.py` & `drf-debug-1.2.0/tracking/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `drf-debug-1.1.0/tracking/tests/urls.py` & `drf-debug-1.2.0/tracking/tests/urls.py`

 * *Files identical despite different names*

### Comparing `drf-debug-1.1.0/tracking/tests/views.py` & `drf-debug-1.2.0/tracking/tests/views.py`

 * *Files identical despite different names*

