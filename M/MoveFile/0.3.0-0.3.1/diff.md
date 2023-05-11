# Comparing `tmp/moveFile-0.3.0.tar.gz` & `tmp/MoveFile-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveFile-0.3.0.tar", last modified: Fri May  5 12:11:06 2023, max compression
+gzip compressed data, was "MoveFile-0.3.1.tar", last modified: Thu May 11 09:52:23 2023, max compression
```

## Comparing `moveFile-0.3.0.tar` & `MoveFile-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 12:11:06.802070 moveFile-0.3.0/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 moveFile-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 moveFile-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      344 2023-05-05 12:11:06.802070 moveFile-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-22 07:19:14.000000 moveFile-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 12:11:06.791069 moveFile-0.3.0/moveFile/
-drwxrwxrwx   0        0        0        0 2023-05-05 12:11:06.800071 moveFile-0.3.0/moveFile/Ui/
--rw-rw-rw-   0        0        0        0 2023-02-22 02:56:19.000000 moveFile-0.3.0/moveFile/Ui/__init__.py
--rw-rw-rw-   0        0        0    71168 2023-04-28 06:15:40.000000 moveFile-0.3.0/moveFile/Ui/moveFileUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-22 08:31:58.000000 moveFile-0.3.0/moveFile/__init__.py
--rw-rw-rw-   0        0        0    35840 2023-04-28 06:14:13.000000 moveFile-0.3.0/moveFile/find_file_return_path_m1.pyd
--rw-rw-rw-   0        0        0   221696 2023-05-05 06:58:51.000000 moveFile-0.3.0/moveFile/moveFile.pyd
--rw-rw-rw-   0        0        0    68608 2023-04-28 06:14:21.000000 moveFile-0.3.0/moveFile/moveFileUi.pyd
--rw-rw-rw-   0        0        0    69632 2023-04-28 06:14:45.000000 moveFile-0.3.0/moveFile/optionDb.pyd
-drwxrwxrwx   0        0        0        0 2023-05-05 12:11:06.797073 moveFile-0.3.0/moveFile.egg-info/
--rw-rw-rw-   0        0        0      344 2023-05-05 12:11:06.000000 moveFile-0.3.0/moveFile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-05-05 12:11:06.000000 moveFile-0.3.0/moveFile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 12:11:06.000000 moveFile-0.3.0/moveFile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 12:11:06.000000 moveFile-0.3.0/moveFile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      135 2023-05-05 12:11:06.803069 moveFile-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      989 2023-05-05 12:10:57.000000 moveFile-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:52:23.311608 MoveFile-0.3.1/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 MoveFile-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 MoveFile-0.3.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-11 09:52:23.294606 MoveFile-0.3.1/MoveFile.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-05-11 09:52:23.000000 MoveFile-0.3.1/MoveFile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-05-11 09:52:23.000000 MoveFile-0.3.1/MoveFile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 09:52:23.000000 MoveFile-0.3.1/MoveFile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-11 09:52:23.000000 MoveFile-0.3.1/MoveFile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      409 2023-05-11 09:52:23.311608 MoveFile-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-22 07:19:14.000000 MoveFile-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 09:52:23.305603 MoveFile-0.3.1/moveFile/
+drwxrwxrwx   0        0        0        0 2023-05-11 09:52:23.309604 MoveFile-0.3.1/moveFile/Ui/
+-rw-rw-rw-   0        0        0        0 2023-02-22 02:56:19.000000 MoveFile-0.3.1/moveFile/Ui/__init__.py
+-rw-rw-rw-   0        0        0    71168 2023-04-28 06:15:40.000000 MoveFile-0.3.1/moveFile/Ui/moveFileUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-22 08:31:58.000000 MoveFile-0.3.1/moveFile/__init__.py
+-rw-rw-rw-   0        0        0    35840 2023-04-28 06:14:13.000000 MoveFile-0.3.1/moveFile/find_file_return_path_m1.pyd
+-rw-rw-rw-   0        0        0   228352 2023-05-11 09:48:11.000000 MoveFile-0.3.1/moveFile/moveFile.pyd
+-rw-rw-rw-   0        0        0    68608 2023-04-28 06:14:21.000000 MoveFile-0.3.1/moveFile/moveFileUi.pyd
+-rw-rw-rw-   0        0        0    69632 2023-04-28 06:14:45.000000 MoveFile-0.3.1/moveFile/optionDb.pyd
+-rw-rw-rw-   0        0        0      135 2023-05-11 09:52:23.312605 MoveFile-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2023-05-11 09:51:12.000000 MoveFile-0.3.1/setup.py
```

### Comparing `moveFile-0.3.0/LICENSE.txt` & `MoveFile-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `moveFile-0.3.0/setup.py` & `MoveFile-0.3.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 0
+PATCH = 1
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
-	name = "moveFile",
+	name = "MoveFile",
 	version = VERSION,
     author ="wangweidong",
     author_email = "17891967090@163.com",
     description='Due Diligence Toolkit Python project',
     long_description_content_type="text/markdown",
-	url = '',
+	url = 'https://alidocs.dingtalk.com/i/p/4oJRz0VRJyvmLZMydy0mV7WvjQn7MG89',
 	long_description = open('README.md',encoding="utf-8").read(),
     python_requires=">=3.8",
     install_requires=get_install_requires(),
     # package_dir = {"":"aaa"},
     # packages = find_packages(where="aaa"),
 	packages = find_packages(),
  	# license = 'Apache',
```

