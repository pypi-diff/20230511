# Comparing `tmp/alibabacloud_imm20200930-2.1.7.tar.gz` & `tmp/alibabacloud_imm20200930-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_imm20200930-2.1.7.tar", last modified: Thu Mar  9 11:03:00 2023, max compression
+gzip compressed data, was "dist/alibabacloud_imm20200930-2.1.9.tar", last modified: Mon Mar 13 06:50:17 2023, max compression
```

## Comparing `alibabacloud_imm20200930-2.1.7.tar` & `alibabacloud_imm20200930-2.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 11:03:00.000000 alibabacloud_imm20200930-2.1.7/
--rw-r--r--   0 root         (0) root         (0)     2734 2023-03-09 11:02:59.000000 alibabacloud_imm20200930-2.1.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-09 11:02:59.000000 alibabacloud_imm20200930-2.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-09 11:02:59.000000 alibabacloud_imm20200930-2.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2353 2023-03-09 11:03:00.000000 alibabacloud_imm20200930-2.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-03-09 11:02:59.000000 alibabacloud_imm20200930-2.1.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-03-09 11:02:59.000000 alibabacloud_imm20200930-2.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 11:03:00.000000 alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-09 11:02:59.000000 alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930/__init__.py
--rw-r--r--   0 root         (0) root         (0)   389328 2023-03-09 11:02:59.000000 alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930/client.py
--rw-r--r--   0 root         (0) root         (0)   735794 2023-03-09 11:02:59.000000 alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 11:03:00.000000 alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2353 2023-03-09 11:03:00.000000 alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-03-09 11:03:00.000000 alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 11:03:00.000000 alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-09 11:03:00.000000 alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-09 11:03:00.000000 alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-09 11:03:00.000000 alibabacloud_imm20200930-2.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2023-03-09 11:02:59.000000 alibabacloud_imm20200930-2.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/
+-rw-r--r--   0 root         (0) root         (0)     2896 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   389328 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930/client.py
+-rw-r--r--   0 root         (0) root         (0)   735794 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-03-13 06:50:17.000000 alibabacloud_imm20200930-2.1.9/setup.py
```

### Comparing `alibabacloud_imm20200930-2.1.7/ChangeLog.md` & `alibabacloud_imm20200930-2.1.9/ChangeLog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+2023-03-09 Version: 2.1.7
+- Fix bug for MaxResults.
+- Add BatchGetFigureCluster API.
+- Add new structs.
+- Fix bug for pod.
+- Fix some bugs and support RocketMQ.
+
 2023-02-08 Version: 2.1.6
 - Support SimilarImageClustering.
 
 2023-02-08 Version: 2.1.5
 - Support more regions.
 
 2023-01-30 Version: 2.1.4
```

### Comparing `alibabacloud_imm20200930-2.1.7/LICENSE` & `alibabacloud_imm20200930-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_imm20200930-2.1.7/PKG-INFO` & `alibabacloud_imm20200930-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_imm20200930
-Version: 2.1.7
+Version: 2.1.9
 Summary: Alibaba Cloud Intelligent Media Management (20200930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_imm20200930-2.1.7/README-CN.md` & `alibabacloud_imm20200930-2.1.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_imm20200930-2.1.7/README.md` & `alibabacloud_imm20200930-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930/client.py` & `alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930/models.py` & `alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_imm20200930-2.1.7/alibabacloud_imm20200930.egg-info/PKG-INFO` & `alibabacloud_imm20200930-2.1.9/alibabacloud_imm20200930.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-imm20200930
-Version: 2.1.7
+Version: 2.1.9
 Summary: Alibaba Cloud Intelligent Media Management (20200930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_imm20200930-2.1.7/setup.py` & `alibabacloud_imm20200930-2.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_imm20200930.
 
-Created on 09/03/2023
+Created on 13/03/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_imm20200930"
 NAME = "alibabacloud_imm20200930" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Intelligent Media Management (20200930) SDK Library for Python"
```

