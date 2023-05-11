# Comparing `tmp/jaxutils-nightly-0.0.8.dev20230509.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20230510.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230509.tar", last modified: Tue May  9 00:06:37 2023, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230510.tar", last modified: Wed May 10 00:06:27 2023, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20230509.tar` & `jaxutils-nightly-0.0.8.dev20230510.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-09 00:06:37.092058 jaxutils-nightly-0.0.8.dev20230509/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-05-09 00:06:37.092058 jaxutils-nightly-0.0.8.dev20230509/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2894 2023-05-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230509/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-09 00:06:37.092058 jaxutils-nightly-0.0.8.dev20230509/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-05-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230509/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-05-09 00:06:37.092058 jaxutils-nightly-0.0.8.dev20230509/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-05-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230509/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-05-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230509/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-05-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230509/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-05-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230509/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-05-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230509/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-09 00:06:37.092058 jaxutils-nightly-0.0.8.dev20230509/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-05-09 00:06:37.000000 jaxutils-nightly-0.0.8.dev20230509/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-05-09 00:06:37.000000 jaxutils-nightly-0.0.8.dev20230509/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-09 00:06:37.000000 jaxutils-nightly-0.0.8.dev20230509/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-05-09 00:06:37.000000 jaxutils-nightly-0.0.8.dev20230509/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-05-09 00:06:37.000000 jaxutils-nightly-0.0.8.dev20230509/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-05-09 00:06:37.092058 jaxutils-nightly-0.0.8.dev20230509/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-05-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230509/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-05-09 00:06:30.000000 jaxutils-nightly-0.0.8.dev20230509/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 00:06:27.768787 jaxutils-nightly-0.0.8.dev20230510/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-05-10 00:06:27.768787 jaxutils-nightly-0.0.8.dev20230510/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2894 2023-05-10 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230510/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 00:06:27.768787 jaxutils-nightly-0.0.8.dev20230510/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-05-10 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230510/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-05-10 00:06:27.768787 jaxutils-nightly-0.0.8.dev20230510/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-05-10 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230510/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-05-10 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230510/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-05-10 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230510/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-05-10 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230510/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-05-10 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230510/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 00:06:27.768787 jaxutils-nightly-0.0.8.dev20230510/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-05-10 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230510/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-05-10 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230510/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-10 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230510/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-05-10 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230510/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-05-10 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230510/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-05-10 00:06:27.768787 jaxutils-nightly-0.0.8.dev20230510/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-05-10 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230510/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-05-10 00:06:22.000000 jaxutils-nightly-0.0.8.dev20230510/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20230509/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230510/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230509
+Version: 0.0.8.dev20230510
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230509/README.md` & `jaxutils-nightly-0.0.8.dev20230510/README.md`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230509/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20230510/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230509/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20230510/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230509/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20230510/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230509/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20230510/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230509/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20230510/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230509/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20230510/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230509/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230510/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230509
+Version: 0.0.8.dev20230510
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230509/setup.py` & `jaxutils-nightly-0.0.8.dev20230510/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230509/versioneer.py` & `jaxutils-nightly-0.0.8.dev20230510/versioneer.py`

 * *Files identical despite different names*
