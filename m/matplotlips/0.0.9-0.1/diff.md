# Comparing `tmp/matplotlips-0.0.9.tar.gz` & `tmp/matplotlips-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlips-0.0.9.tar", last modified: Thu May 11 01:42:56 2023, max compression
+gzip compressed data, was "matplotlips-0.1.tar", last modified: Thu May 11 01:44:17 2023, max compression
```

## Comparing `matplotlips-0.0.9.tar` & `matplotlips-0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 01:42:56.011190 matplotlips-0.0.9/
--rw-rw-rw-   0        0        0      592 2023-05-11 01:42:56.011190 matplotlips-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 01:42:55.979605 matplotlips-0.0.9/matplotlips/
--rw-rw-rw-   0        0        0       30 2023-05-11 01:42:44.000000 matplotlips-0.0.9/matplotlips/__init__.py
--rw-rw-rw-   0        0        0    68144 2023-05-11 01:35:43.000000 matplotlips-0.0.9/matplotlips/charts.py
-drwxrwxrwx   0        0        0        0 2023-05-11 01:42:56.011190 matplotlips-0.0.9/matplotlips.egg-info/
--rw-rw-rw-   0        0        0      592 2023-05-11 01:42:55.000000 matplotlips-0.0.9/matplotlips.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-05-11 01:42:55.000000 matplotlips-0.0.9/matplotlips.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 01:42:55.000000 matplotlips-0.0.9/matplotlips.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-11 01:42:55.000000 matplotlips-0.0.9/matplotlips.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 01:42:56.011190 matplotlips-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-05-11 01:42:51.000000 matplotlips-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:44:17.657253 matplotlips-0.1/
+-rw-rw-rw-   0        0        0      590 2023-05-11 01:44:17.651456 matplotlips-0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 01:44:17.633700 matplotlips-0.1/matplotlips/
+-rw-rw-rw-   0        0        0       30 2023-05-11 01:42:44.000000 matplotlips-0.1/matplotlips/__init__.py
+-rw-rw-rw-   0        0        0    68144 2023-05-11 01:35:43.000000 matplotlips-0.1/matplotlips/charts.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:44:17.651456 matplotlips-0.1/matplotlips.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-05-11 01:44:17.000000 matplotlips-0.1/matplotlips.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-05-11 01:44:17.000000 matplotlips-0.1/matplotlips.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 01:44:17.000000 matplotlips-0.1/matplotlips.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 01:44:17.000000 matplotlips-0.1/matplotlips.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 01:44:17.657253 matplotlips-0.1/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-05-11 01:44:05.000000 matplotlips-0.1/setup.py
```

### Comparing `matplotlips-0.0.9/PKG-INFO` & `matplotlips-0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlips
-Version: 0.0.9
+Version: 0.1
 Summary: TopG
 Home-page: UNKNOWN
 Author: andrew tate
 Author-email: <mail@neuralnine.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `matplotlips-0.0.9/matplotlips/charts.py` & `matplotlips-0.1/matplotlips/charts.py`

 * *Files identical despite different names*

### Comparing `matplotlips-0.0.9/matplotlips.egg-info/PKG-INFO` & `matplotlips-0.1/matplotlips.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlips
-Version: 0.0.9
+Version: 0.1
 Summary: TopG
 Home-page: UNKNOWN
 Author: andrew tate
 Author-email: <mail@neuralnine.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `matplotlips-0.0.9/setup.py` & `matplotlips-0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.9'
+VERSION = '0.1'
 DESCRIPTION = 'TopG'
 
 # Setting up
 setup(
 name="matplotlips",
     version=VERSION,
     author="andrew tate",
```

