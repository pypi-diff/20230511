# Comparing `tmp/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1.tar.gz` & `tmp/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1.tar", last modified: Thu Feb  9 02:54:43 2023, max compression
+gzip compressed data, was "dist/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2.tar", last modified: Thu May 11 03:29:09 2023, max compression
```

## Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1.tar` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22810 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py
--rw-r--r--   0 root         (0) root         (0)    16218 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-02-09 02:54:43.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:09.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-11 03:29:08.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-11 03:29:08.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-11 03:29:09.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-11 03:29:08.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-11 03:29:08.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:09.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-11 03:29:09.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-11 03:29:09.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:29:09.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-11 03:29:09.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-11 03:29:09.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:29:09.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 03:29:08.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34424 2023-05-11 03:29:08.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py
+-rw-r--r--   0 root         (0) root         (0)    39027 2023-05-11 03:29:08.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-11 03:29:09.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-11 03:29:08.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/setup.py
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/LICENSE` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/PKG-INFO` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_68b3ee3230284cddaa19740dcaf251d8
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/README-CN.md` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/README.md` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-68b3ee3230284cddaa19740dcaf251d8
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.1/setup.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_68b3ee3230284cddaa19740dcaf251d8.
 
-Created on 09/02/2023
+Created on 11/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8"
 NAME = "antchain_ak_68b3ee3230284cddaa19740dcaf251d8" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python"
```

