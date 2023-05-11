# Comparing `tmp/pyBLACK-0.1.2.tar.gz` & `tmp/pyBLACK-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyBLACK-0.1.2.tar", last modified: Fri Jun 17 14:38:07 2022, max compression
+gzip compressed data, was "pyBLACK-0.1.3.tar", last modified: Thu Jul 28 09:35:18 2022, max compression
```

## Comparing `pyBLACK-0.1.2.tar` & `pyBLACK-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 iogiul     (501) staff       (20)        0 2022-06-17 14:38:07.696685 pyBLACK-0.1.2/
--rw-r--r--   0 iogiul     (501) staff       (20)       44 2022-06-16 16:52:42.000000 pyBLACK-0.1.2/MANIFEST.in
--rw-r--r--   0 iogiul     (501) staff       (20)      574 2022-06-17 14:38:07.696399 pyBLACK-0.1.2/PKG-INFO
--rw-r--r--   0 iogiul     (501) staff       (20)      327 2022-06-17 14:37:27.000000 pyBLACK-0.1.2/README.rst
-drwxr-xr-x   0 iogiul     (501) staff       (20)        0 2022-06-17 14:38:07.691118 pyBLACK-0.1.2/pyBLACK.egg-info/
--rw-r--r--   0 iogiul     (501) staff       (20)      574 2022-06-17 14:38:07.000000 pyBLACK-0.1.2/pyBLACK.egg-info/PKG-INFO
--rw-r--r--   0 iogiul     (501) staff       (20)      319 2022-06-17 14:38:07.000000 pyBLACK-0.1.2/pyBLACK.egg-info/SOURCES.txt
--rw-r--r--   0 iogiul     (501) staff       (20)        1 2022-06-17 14:38:07.000000 pyBLACK-0.1.2/pyBLACK.egg-info/dependency_links.txt
--rw-r--r--   0 iogiul     (501) staff       (20)       16 2022-06-17 14:38:07.000000 pyBLACK-0.1.2/pyBLACK.egg-info/requires.txt
--rw-r--r--   0 iogiul     (501) staff       (20)       19 2022-06-17 14:38:07.000000 pyBLACK-0.1.2/pyBLACK.egg-info/top_level.txt
-drwxr-xr-x   0 iogiul     (501) staff       (20)        0 2022-06-17 14:38:07.692206 pyBLACK-0.1.2/pyblack/
--rw-r--r--   0 iogiul     (501) staff       (20)       59 2022-06-17 13:59:12.000000 pyBLACK-0.1.2/pyblack/__init__.py
--rw-r--r--   0 iogiul     (501) staff       (20)      433 2022-06-16 16:52:42.000000 pyBLACK-0.1.2/pyblack/constants.py
-drwxr-xr-x   0 iogiul     (501) staff       (20)        0 2022-06-17 14:38:07.693649 pyBLACK-0.1.2/pyblack/gw/
--rw-r--r--   0 iogiul     (501) staff       (20)       33 2022-06-16 16:52:42.000000 pyBLACK-0.1.2/pyblack/gw/__init__.py
-drwxr-xr-x   0 iogiul     (501) staff       (20)        0 2022-06-17 14:38:07.694225 pyBLACK-0.1.2/pyblack/gw/ext_data/
--rw-r--r--   0 iogiul     (501) staff       (20)   150373 2022-06-16 16:52:42.000000 pyBLACK-0.1.2/pyblack/gw/ext_data/cured_gw_time.interpolation
--rw-r--r--   0 iogiul     (501) staff       (20)    13318 2022-06-17 14:10:17.000000 pyBLACK-0.1.2/pyblack/gw/gw_time.py
--rw-r--r--   0 iogiul     (501) staff       (20)       38 2022-06-17 14:38:07.696799 pyBLACK-0.1.2/setup.cfg
--rw-r--r--   0 iogiul     (501) staff       (20)      841 2022-06-16 16:52:42.000000 pyBLACK-0.1.2/setup.py
+drwxr-xr-x   0 iogiul     (501) staff       (20)        0 2022-07-28 09:35:18.699537 pyBLACK-0.1.3/
+-rwxr-xr-x   0 iogiul     (501) staff       (20)      890 2022-06-16 16:52:42.000000 pyBLACK-0.1.3/.gitignore
+-rw-r--r--   0 iogiul     (501) staff       (20)       44 2022-06-16 16:52:42.000000 pyBLACK-0.1.3/MANIFEST.in
+-rw-r--r--   0 iogiul     (501) staff       (20)      574 2022-07-28 09:35:18.699167 pyBLACK-0.1.3/PKG-INFO
+-rw-r--r--   0 iogiul     (501) staff       (20)      327 2022-06-17 14:37:27.000000 pyBLACK-0.1.3/README.rst
+drwxr-xr-x   0 iogiul     (501) staff       (20)        0 2022-07-28 09:35:18.690558 pyBLACK-0.1.3/pyBLACK.egg-info/
+-rw-r--r--   0 iogiul     (501) staff       (20)      574 2022-07-28 09:35:18.000000 pyBLACK-0.1.3/pyBLACK.egg-info/PKG-INFO
+-rw-r--r--   0 iogiul     (501) staff       (20)      571 2022-07-28 09:35:18.000000 pyBLACK-0.1.3/pyBLACK.egg-info/SOURCES.txt
+-rw-r--r--   0 iogiul     (501) staff       (20)        1 2022-07-28 09:35:18.000000 pyBLACK-0.1.3/pyBLACK.egg-info/dependency_links.txt
+-rw-r--r--   0 iogiul     (501) staff       (20)       16 2022-07-28 09:35:18.000000 pyBLACK-0.1.3/pyBLACK.egg-info/requires.txt
+-rw-r--r--   0 iogiul     (501) staff       (20)       19 2022-07-28 09:35:18.000000 pyBLACK-0.1.3/pyBLACK.egg-info/top_level.txt
+drwxr-xr-x   0 iogiul     (501) staff       (20)        0 2022-07-28 09:35:18.691519 pyBLACK-0.1.3/pyblack/
+-rw-r--r--   0 iogiul     (501) staff       (20)       59 2022-07-27 11:56:49.000000 pyBLACK-0.1.3/pyblack/__init__.py
+drwxr-xr-x   0 iogiul     (501) staff       (20)        0 2022-07-28 09:35:18.693382 pyBLACK-0.1.3/pyblack/__pycache__/
+-rw-r--r--   0 iogiul     (501) staff       (20)      156 2022-06-16 16:52:42.000000 pyBLACK-0.1.3/pyblack/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 iogiul     (501) staff       (20)      245 2022-07-27 12:06:19.000000 pyBLACK-0.1.3/pyblack/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 iogiul     (501) staff       (20)      444 2022-07-27 12:06:20.000000 pyBLACK-0.1.3/pyblack/__pycache__/constants.cpython-38.pyc
+-rw-r--r--   0 iogiul     (501) staff       (20)      705 2022-07-27 12:05:23.000000 pyBLACK-0.1.3/pyblack/constants.py
+drwxr-xr-x   0 iogiul     (501) staff       (20)        0 2022-07-28 09:35:18.694294 pyBLACK-0.1.3/pyblack/gw/
+-rw-r--r--   0 iogiul     (501) staff       (20)       33 2022-06-16 16:52:42.000000 pyBLACK-0.1.3/pyblack/gw/__init__.py
+drwxr-xr-x   0 iogiul     (501) staff       (20)        0 2022-07-28 09:35:18.697288 pyBLACK-0.1.3/pyblack/gw/__pycache__/
+-rw-r--r--   0 iogiul     (501) staff       (20)      219 2022-06-16 17:24:29.000000 pyBLACK-0.1.3/pyblack/gw/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 iogiul     (501) staff       (20)    11970 2022-07-27 12:06:19.000000 pyBLACK-0.1.3/pyblack/gw/__pycache__/gw_time.cpython-38.pyc
+drwxr-xr-x   0 iogiul     (501) staff       (20)        0 2022-07-28 09:35:18.697595 pyBLACK-0.1.3/pyblack/gw/ext_data/
+-rw-r--r--   0 iogiul     (501) staff       (20)   150373 2022-06-16 16:52:42.000000 pyBLACK-0.1.3/pyblack/gw/ext_data/cured_gw_time.interpolation
+-rw-r--r--   0 iogiul     (501) staff       (20)    13318 2022-07-12 12:31:13.000000 pyBLACK-0.1.3/pyblack/gw/gw_time.py
+-rwxr-xr-x   0 iogiul     (501) staff       (20)       76 2022-06-16 16:52:42.000000 pyBLACK-0.1.3/pypi_upload.sh
+-rw-r--r--   0 iogiul     (501) staff       (20)       38 2022-07-28 09:35:18.699660 pyBLACK-0.1.3/setup.cfg
+-rw-r--r--   0 iogiul     (501) staff       (20)      841 2022-06-16 16:52:42.000000 pyBLACK-0.1.3/setup.py
```

### Comparing `pyBLACK-0.1.2/PKG-INFO` & `pyBLACK-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBLACK
-Version: 0.1.2
+Version: 0.1.3
 Summary: suit of utilities for the DEMOBLACK group
 Home-page: https://gitlab.com/iogiul/pyblack
 Author: G. Iorio
 Author-email: giuliano.iorio.astro@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pyBLACK-0.1.2/pyBLACK.egg-info/PKG-INFO` & `pyBLACK-0.1.3/pyBLACK.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBLACK
-Version: 0.1.2
+Version: 0.1.3
 Summary: suit of utilities for the DEMOBLACK group
 Home-page: https://gitlab.com/iogiul/pyblack
 Author: G. Iorio
 Author-email: giuliano.iorio.astro@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pyBLACK-0.1.2/pyblack/gw/ext_data/cured_gw_time.interpolation` & `pyBLACK-0.1.3/pyblack/gw/ext_data/cured_gw_time.interpolation`

 * *Files identical despite different names*

### Comparing `pyBLACK-0.1.2/pyblack/gw/gw_time.py` & `pyBLACK-0.1.3/pyblack/gw/gw_time.py`

 * *Files identical despite different names*

### Comparing `pyBLACK-0.1.2/setup.py` & `pyBLACK-0.1.3/setup.py`

 * *Files identical despite different names*

