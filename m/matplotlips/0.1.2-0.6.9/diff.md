# Comparing `tmp/matplotlips-0.1.2.tar.gz` & `tmp/matplotlips-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlips-0.1.2.tar", last modified: Thu May 11 01:46:53 2023, max compression
+gzip compressed data, was "matplotlips-0.6.9.tar", last modified: Thu May 11 21:44:52 2023, max compression
```

## Comparing `matplotlips-0.1.2.tar` & `matplotlips-0.6.9.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 01:46:53.862070 matplotlips-0.1.2/
--rw-rw-rw-   0        0        0      592 2023-05-11 01:46:53.852960 matplotlips-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 01:46:53.821299 matplotlips-0.1.2/matplotlips/
--rw-rw-rw-   0        0        0       30 2023-05-11 01:42:44.000000 matplotlips-0.1.2/matplotlips/__init__.py
--rw-rw-rw-   0        0        0    32471 2023-05-11 01:46:48.000000 matplotlips-0.1.2/matplotlips/charts.py
-drwxrwxrwx   0        0        0        0 2023-05-11 01:46:53.852960 matplotlips-0.1.2/matplotlips.egg-info/
--rw-rw-rw-   0        0        0      592 2023-05-11 01:46:53.000000 matplotlips-0.1.2/matplotlips.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-05-11 01:46:53.000000 matplotlips-0.1.2/matplotlips.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 01:46:53.000000 matplotlips-0.1.2/matplotlips.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-11 01:46:53.000000 matplotlips-0.1.2/matplotlips.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 01:46:53.862070 matplotlips-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-05-11 01:45:44.000000 matplotlips-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:44:52.356461 matplotlips-0.6.9/
+-rw-rw-rw-   0        0        0      592 2023-05-11 21:44:52.356461 matplotlips-0.6.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 21:44:52.341500 matplotlips-0.6.9/matplotlips/
+-rw-rw-rw-   0        0        0       62 2023-05-11 21:42:25.000000 matplotlips-0.6.9/matplotlips/__init__.py
+-rw-rw-rw-   0        0        0    24803 2023-05-11 21:41:21.000000 matplotlips-0.6.9/matplotlips/arrays.py
+-rw-rw-rw-   0        0        0    32471 2023-05-11 01:46:48.000000 matplotlips-0.6.9/matplotlips/charts.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:44:52.354456 matplotlips-0.6.9/matplotlips.egg-info/
+-rw-rw-rw-   0        0        0      592 2023-05-11 21:44:52.000000 matplotlips-0.6.9/matplotlips.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-05-11 21:44:52.000000 matplotlips-0.6.9/matplotlips.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 21:44:52.000000 matplotlips-0.6.9/matplotlips.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 21:44:52.000000 matplotlips-0.6.9/matplotlips.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 21:44:52.356461 matplotlips-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-05-11 21:43:41.000000 matplotlips-0.6.9/setup.py
```

### Comparing `matplotlips-0.1.2/PKG-INFO` & `matplotlips-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlips
-Version: 0.1.2
+Version: 0.6.9
 Summary: TopG
 Home-page: UNKNOWN
 Author: andrew tate
 Author-email: <mail@neuralnine.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `matplotlips-0.1.2/matplotlips/charts.py` & `matplotlips-0.6.9/matplotlips/charts.py`

 * *Files identical despite different names*

### Comparing `matplotlips-0.1.2/matplotlips.egg-info/PKG-INFO` & `matplotlips-0.6.9/matplotlips.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlips
-Version: 0.1.2
+Version: 0.6.9
 Summary: TopG
 Home-page: UNKNOWN
 Author: andrew tate
 Author-email: <mail@neuralnine.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `matplotlips-0.1.2/setup.py` & `matplotlips-0.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.2'
+VERSION = '0.6.9'
 DESCRIPTION = 'TopG'
 
 # Setting up
 setup(
 name="matplotlips",
     version=VERSION,
     author="andrew tate",
```

