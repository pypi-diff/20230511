# Comparing `tmp/pygameHat-1.1.2.tar.gz` & `tmp/pygameHat-1.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygameHat-1.1.2.tar", last modified: Mon May  8 13:22:02 2023, max compression
+gzip compressed data, was "pygameHat-1.1.2.1.tar", last modified: Thu May 11 18:56:08 2023, max compression
```

## Comparing `pygameHat-1.1.2.tar` & `pygameHat-1.1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 13:22:02.564541 pygameHat-1.1.2/
--rw-rw-rw-   0        0        0       29 2023-04-17 15:20:38.000000 pygameHat-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      543 2023-05-08 13:22:02.565594 pygameHat-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 13:22:02.365582 pygameHat-1.1.2/pygameHat/
--rw-rw-rw-   0        0        0    43860 2023-05-08 13:19:12.000000 pygameHat-1.1.2/pygameHat/__init__.py
--rw-rw-rw-   0        0        0       11 2023-04-17 14:59:31.000000 pygameHat-1.1.2/pygameHat/pygameHat.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:22:02.545545 pygameHat-1.1.2/pygameHat.egg-info/
--rw-rw-rw-   0        0        0      543 2023-05-08 13:22:02.000000 pygameHat-1.1.2/pygameHat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-05-08 13:22:02.000000 pygameHat-1.1.2/pygameHat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 13:22:02.000000 pygameHat-1.1.2/pygameHat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-08 13:22:02.000000 pygameHat-1.1.2/pygameHat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-08 13:22:02.000000 pygameHat-1.1.2/pygameHat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 13:22:02.591503 pygameHat-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-05-08 13:21:54.000000 pygameHat-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:56:08.837662 pygameHat-1.1.2.1/
+-rw-rw-rw-   0        0        0       29 2023-04-17 15:20:38.000000 pygameHat-1.1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      545 2023-05-11 18:56:08.837662 pygameHat-1.1.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 18:56:08.677611 pygameHat-1.1.2.1/pygameHat/
+-rw-rw-rw-   0        0        0    43862 2023-05-11 18:55:01.000000 pygameHat-1.1.2.1/pygameHat/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-04-17 14:59:31.000000 pygameHat-1.1.2.1/pygameHat/pygameHat.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:56:08.787607 pygameHat-1.1.2.1/pygameHat.egg-info/
+-rw-rw-rw-   0        0        0      545 2023-05-11 18:56:07.000000 pygameHat-1.1.2.1/pygameHat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-05-11 18:56:07.000000 pygameHat-1.1.2.1/pygameHat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 18:56:07.000000 pygameHat-1.1.2.1/pygameHat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-11 18:56:07.000000 pygameHat-1.1.2.1/pygameHat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 18:56:07.000000 pygameHat-1.1.2.1/pygameHat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 18:56:08.844658 pygameHat-1.1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-05-11 18:54:47.000000 pygameHat-1.1.2.1/setup.py
```

### Comparing `pygameHat-1.1.2/PKG-INFO` & `pygameHat-1.1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.1.2
+Version: 1.1.2.1
 Summary: Pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,engine,pygame,game,maker
```

### Comparing `pygameHat-1.1.2/pygameHat/__init__.py` & `pygameHat-1.1.2.1/pygameHat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pygame, sys, time, base64, os, json
 
 #pygame initialization
-version = "Beta 1.1.2"
+version = "Beta 1.1.2.1"
 print(f"\nAdditional hello from pygameHat {version} :D")
 print("\nThis version may not be compatible with older versions")
 
 pygame.init()
 pygame.font.init()
 try:
     pygame.mixer.init()
```

### Comparing `pygameHat-1.1.2/pygameHat.egg-info/PKG-INFO` & `pygameHat-1.1.2.1/pygameHat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.1.2
+Version: 1.1.2.1
 Summary: Pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,engine,pygame,game,maker
```

### Comparing `pygameHat-1.1.2/setup.py` & `pygameHat-1.1.2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.1.2'
+VERSION = '1.1.2.1'
 DESCRIPTION = 'Pygame game-making engine'
 
 # Setting up
 setup(
     name="pygameHat",
     version=VERSION,
     author="Wojciech Błajda",
     #author_email="None",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=["pygame", "sys", "time", "base64", "os", "json"],
+    install_requires=["pygame", "pyinstaller"],
     keywords=['python', 'engine', 'pygame', 'game', 'maker'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

