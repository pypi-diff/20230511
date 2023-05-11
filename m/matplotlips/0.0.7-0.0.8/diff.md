# Comparing `tmp/matplotlips-0.0.7.tar.gz` & `tmp/matplotlips-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlips-0.0.7.tar", last modified: Wed May 10 17:26:51 2023, max compression
+gzip compressed data, was "matplotlips-0.0.8.tar", last modified: Thu May 11 01:37:31 2023, max compression
```

## Comparing `matplotlips-0.0.7.tar` & `matplotlips-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 17:26:51.693237 matplotlips-0.0.7/
--rw-rw-rw-   0        0        0      592 2023-05-10 17:26:51.693237 matplotlips-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 17:26:51.693237 matplotlips-0.0.7/matplotlips/
--rw-rw-rw-   0        0        0       30 2023-05-10 17:25:29.000000 matplotlips-0.0.7/matplotlips/__init__.py
--rw-rw-rw-   0        0        0    11525 2023-05-10 17:16:31.000000 matplotlips-0.0.7/matplotlips/charts.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:26:51.693237 matplotlips-0.0.7/matplotlips.egg-info/
--rw-rw-rw-   0        0        0      592 2023-05-10 17:26:51.000000 matplotlips-0.0.7/matplotlips.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-05-10 17:26:51.000000 matplotlips-0.0.7/matplotlips.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 17:26:51.000000 matplotlips-0.0.7/matplotlips.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 17:26:51.000000 matplotlips-0.0.7/matplotlips.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 17:26:51.693237 matplotlips-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-05-10 17:26:28.000000 matplotlips-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:37:31.565476 matplotlips-0.0.8/
+-rw-rw-rw-   0        0        0      592 2023-05-11 01:37:31.562859 matplotlips-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 01:37:31.534207 matplotlips-0.0.8/matplotlips/
+-rw-rw-rw-   0        0        0      815 2023-05-10 19:24:03.000000 matplotlips-0.0.8/matplotlips/__init__.py
+-rw-rw-rw-   0        0        0    68144 2023-05-11 01:35:43.000000 matplotlips-0.0.8/matplotlips/charts.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:37:31.547217 matplotlips-0.0.8/matplotlips.egg-info/
+-rw-rw-rw-   0        0        0      592 2023-05-11 01:37:31.000000 matplotlips-0.0.8/matplotlips.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-05-11 01:37:31.000000 matplotlips-0.0.8/matplotlips.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 01:37:31.000000 matplotlips-0.0.8/matplotlips.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 01:37:31.000000 matplotlips-0.0.8/matplotlips.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 01:37:31.565476 matplotlips-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-05-11 01:37:27.000000 matplotlips-0.0.8/setup.py
```

### Comparing `matplotlips-0.0.7/PKG-INFO` & `matplotlips-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlips
-Version: 0.0.7
+Version: 0.0.8
 Summary: TopG
 Home-page: UNKNOWN
 Author: andrew tate
 Author-email: <mail@neuralnine.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `matplotlips-0.0.7/matplotlips.egg-info/PKG-INFO` & `matplotlips-0.0.8/matplotlips.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlips
-Version: 0.0.7
+Version: 0.0.8
 Summary: TopG
 Home-page: UNKNOWN
 Author: andrew tate
 Author-email: <mail@neuralnine.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `matplotlips-0.0.7/setup.py` & `matplotlips-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'TopG'
 
 # Setting up
 setup(
 name="matplotlips",
     version=VERSION,
     author="andrew tate",
```

