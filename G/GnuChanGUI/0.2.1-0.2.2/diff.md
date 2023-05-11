# Comparing `tmp/GnuChanGUI-0.2.1.tar.gz` & `tmp/GnuChanGUI-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GnuChanGUI-0.2.1.tar", last modified: Thu May 11 17:59:20 2023, max compression
+gzip compressed data, was "GnuChanGUI-0.2.2.tar", last modified: Thu May 11 19:13:59 2023, max compression
```

## Comparing `GnuChanGUI-0.2.1.tar` & `GnuChanGUI-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 archkubi  (1000) archkubi  (1000)        0 2023-05-11 17:59:20.494239 GnuChanGUI-0.2.1/
-drwxr-xr-x   0 archkubi  (1000) archkubi  (1000)        0 2023-05-11 17:59:20.493239 GnuChanGUI-0.2.1/GnuChanGUI.egg-info/
--rw-r--r--   0 archkubi  (1000) archkubi  (1000)      787 2023-05-11 17:59:20.000000 GnuChanGUI-0.2.1/GnuChanGUI.egg-info/PKG-INFO
--rw-r--r--   0 archkubi  (1000) archkubi  (1000)      187 2023-05-11 17:59:20.000000 GnuChanGUI-0.2.1/GnuChanGUI.egg-info/SOURCES.txt
--rw-r--r--   0 archkubi  (1000) archkubi  (1000)        1 2023-05-11 17:59:20.000000 GnuChanGUI-0.2.1/GnuChanGUI.egg-info/dependency_links.txt
--rw-r--r--   0 archkubi  (1000) archkubi  (1000)       12 2023-05-11 17:59:20.000000 GnuChanGUI-0.2.1/GnuChanGUI.egg-info/requires.txt
--rw-r--r--   0 archkubi  (1000) archkubi  (1000)        1 2023-05-11 17:59:20.000000 GnuChanGUI-0.2.1/GnuChanGUI.egg-info/top_level.txt
--rw-r--r--   0 archkubi  (1000) archkubi  (1000)      787 2023-05-11 17:59:20.494239 GnuChanGUI-0.2.1/PKG-INFO
--rw-r--r--   0 archkubi  (1000) archkubi  (1000)      225 2023-05-09 21:22:21.000000 GnuChanGUI-0.2.1/README.md
--rw-r--r--   0 archkubi  (1000) archkubi  (1000)       38 2023-05-11 17:59:20.495240 GnuChanGUI-0.2.1/setup.cfg
--rw-r--r--   0 archkubi  (1000) archkubi  (1000)      840 2023-05-11 17:59:15.000000 GnuChanGUI-0.2.1/setup.py
+drwxr-xr-x   0 archkubi  (1000) archkubi  (1000)        0 2023-05-11 19:13:59.828253 GnuChanGUI-0.2.2/
+drwxr-xr-x   0 archkubi  (1000) archkubi  (1000)        0 2023-05-11 19:13:59.825253 GnuChanGUI-0.2.2/GnuChanGUI.egg-info/
+-rw-r--r--   0 archkubi  (1000) archkubi  (1000)      787 2023-05-11 19:13:58.000000 GnuChanGUI-0.2.2/GnuChanGUI.egg-info/PKG-INFO
+-rw-r--r--   0 archkubi  (1000) archkubi  (1000)      187 2023-05-11 19:13:58.000000 GnuChanGUI-0.2.2/GnuChanGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 archkubi  (1000) archkubi  (1000)        1 2023-05-11 19:13:58.000000 GnuChanGUI-0.2.2/GnuChanGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 archkubi  (1000) archkubi  (1000)       12 2023-05-11 19:13:58.000000 GnuChanGUI-0.2.2/GnuChanGUI.egg-info/requires.txt
+-rw-r--r--   0 archkubi  (1000) archkubi  (1000)        1 2023-05-11 19:13:58.000000 GnuChanGUI-0.2.2/GnuChanGUI.egg-info/top_level.txt
+-rw-r--r--   0 archkubi  (1000) archkubi  (1000)      787 2023-05-11 19:13:59.827253 GnuChanGUI-0.2.2/PKG-INFO
+-rw-r--r--   0 archkubi  (1000) archkubi  (1000)      225 2023-05-09 21:22:21.000000 GnuChanGUI-0.2.2/README.md
+-rw-r--r--   0 archkubi  (1000) archkubi  (1000)       38 2023-05-11 19:13:59.828253 GnuChanGUI-0.2.2/setup.cfg
+-rw-r--r--   0 archkubi  (1000) archkubi  (1000)      840 2023-05-11 19:13:31.000000 GnuChanGUI-0.2.2/setup.py
```

### Comparing `GnuChanGUI-0.2.1/GnuChanGUI.egg-info/PKG-INFO` & `GnuChanGUI-0.2.2/GnuChanGUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GnuChanGUI
-Version: 0.2.1
+Version: 0.2.2
 Summary: pysimplegui base gui for beginner
 Home-page: https://github.com/gnuchanos/GnuChanGUI
 Author: archkubi
 Author-email: gnuchanos@gmail.com
 Keywords: PySimpleGUI,GnuChanGUI,beginner gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `GnuChanGUI-0.2.1/PKG-INFO` & `GnuChanGUI-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GnuChanGUI
-Version: 0.2.1
+Version: 0.2.2
 Summary: pysimplegui base gui for beginner
 Home-page: https://github.com/gnuchanos/GnuChanGUI
 Author: archkubi
 Author-email: gnuchanos@gmail.com
 Keywords: PySimpleGUI,GnuChanGUI,beginner gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `GnuChanGUI-0.2.1/setup.py` & `GnuChanGUI-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name="GnuChanGUI",
-    version="0.2.1",
+    version="0.2.2",
     author="archkubi",
     author_email="gnuchanos@gmail.com",
     description="pysimplegui base gui for beginner",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/gnuchanos/GnuChanGUI",
     packages=find_packages(),
```

