# Comparing `tmp/phase-o-matic-0.0.4.tar.gz` & `tmp/phase-o-matic-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phase-o-matic-0.0.4.tar", last modified: Thu May 11 19:41:40 2023, max compression
+gzip compressed data, was "phase-o-matic-0.0.6.tar", last modified: Thu May 11 20:15:26 2023, max compression
```

## Comparing `phase-o-matic-0.0.4.tar` & `phase-o-matic-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-11 19:41:40.444001 phase-o-matic-0.0.4/
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     1073 2023-05-04 18:10:22.000000 phase-o-matic-0.0.4/LICENSE
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     4714 2023-05-11 19:41:40.443633 phase-o-matic-0.0.4/PKG-INFO
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     4050 2023-05-11 19:09:14.000000 phase-o-matic-0.0.4/README.md
-drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-11 19:41:40.440167 phase-o-matic-0.0.4/phase_o_matic/
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       38 2023-05-10 18:09:00.000000 phase-o-matic-0.0.4/phase_o_matic/__init__.py
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     3014 2023-05-10 20:11:35.000000 phase-o-matic-0.0.4/phase_o_matic/download.py
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     6390 2023-05-10 20:40:18.000000 phase-o-matic-0.0.4/phase_o_matic/phase_delay.py
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     9263 2023-05-11 19:12:37.000000 phase-o-matic-0.0.4/phase_o_matic/preprocess.py
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     1152 2023-05-10 18:08:17.000000 phase-o-matic-0.0.4/phase_o_matic/presto.py
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     1387 2023-05-10 20:47:48.000000 phase-o-matic-0.0.4/phase_o_matic/utils.py
-drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-11 19:41:40.442153 phase-o-matic-0.0.4/phase_o_matic.egg-info/
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     4714 2023-05-11 19:41:40.000000 phase-o-matic-0.0.4/phase_o_matic.egg-info/PKG-INFO
--rw-r--r--   0 zachkeskinen   (501) staff       (20)      429 2023-05-11 19:41:40.000000 phase-o-matic-0.0.4/phase_o_matic.egg-info/SOURCES.txt
--rw-r--r--   0 zachkeskinen   (501) staff       (20)        1 2023-05-11 19:41:40.000000 phase-o-matic-0.0.4/phase_o_matic.egg-info/dependency_links.txt
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       51 2023-05-11 19:41:40.000000 phase-o-matic-0.0.4/phase_o_matic.egg-info/requires.txt
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       14 2023-05-11 19:41:40.000000 phase-o-matic-0.0.4/phase_o_matic.egg-info/top_level.txt
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       84 2023-05-11 19:28:36.000000 phase-o-matic-0.0.4/pyproject.toml
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       38 2023-05-11 19:41:40.444156 phase-o-matic-0.0.4/setup.cfg
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     3952 2023-05-11 19:41:16.000000 phase-o-matic-0.0.4/setup.py
-drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-11 19:41:40.443174 phase-o-matic-0.0.4/tests/
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     2273 2023-05-10 20:11:26.000000 phase-o-matic-0.0.4/tests/test_download.py
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     5053 2023-05-10 20:26:07.000000 phase-o-matic-0.0.4/tests/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:15:26.600233 phase-o-matic-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-11 20:15:26.600233 phase-o-matic-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:15:26.600233 phase-o-matic-0.0.6/phase_o_matic/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/phase_o_matic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/phase_o_matic/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/phase_o_matic/phase_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/phase_o_matic/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/phase_o_matic/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/phase_o_matic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:15:26.600233 phase-o-matic-0.0.6/phase_o_matic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-11 20:15:26.000000 phase-o-matic-0.0.6/phase_o_matic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-11 20:15:26.000000 phase-o-matic-0.0.6/phase_o_matic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:15:26.000000 phase-o-matic-0.0.6/phase_o_matic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 20:15:26.000000 phase-o-matic-0.0.6/phase_o_matic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 20:15:26.000000 phase-o-matic-0.0.6/phase_o_matic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:15:26.600233 phase-o-matic-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-11 20:15:10.000000 phase-o-matic-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:15:26.600233 phase-o-matic-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/tests/test_preprocess.py
```

### Comparing `phase-o-matic-0.0.4/LICENSE` & `phase-o-matic-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.4/PKG-INFO` & `phase-o-matic-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phase-o-matic
-Version: 0.0.4
+Version: 0.0.6
 Summary: InSAR Atmospheric Delay Corrections with ERA5.
 Home-page: https://github.com/ZachKeskinen/phase-o-matic
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `phase-o-matic-0.0.4/README.md` & `phase-o-matic-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.4/phase_o_matic/download.py` & `phase-o-matic-0.0.6/phase_o_matic/download.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.4/phase_o_matic/phase_delay.py` & `phase-o-matic-0.0.6/phase_o_matic/phase_delay.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.4/phase_o_matic/preprocess.py` & `phase-o-matic-0.0.6/phase_o_matic/preprocess.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.4/phase_o_matic/presto.py` & `phase-o-matic-0.0.6/phase_o_matic/presto.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.4/phase_o_matic/utils.py` & `phase-o-matic-0.0.6/phase_o_matic/utils.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.4/phase_o_matic.egg-info/PKG-INFO` & `phase-o-matic-0.0.6/phase_o_matic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phase-o-matic
-Version: 0.0.4
+Version: 0.0.6
 Summary: InSAR Atmospheric Delay Corrections with ERA5.
 Home-page: https://github.com/ZachKeskinen/phase-o-matic
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `phase-o-matic-0.0.4/setup.py` & `phase-o-matic-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Note: To use the 'upload' functionality of this file, you must:
 #   $ pipenv install twine --dev
 
+"""
+To upload run:
+
+python3 -m build
+twine upload dist/*
+
+in the home directory of this file.
+
+to have github auto-release:
+https://dev.to/iamtekson/publish-package-to-pypi-and-release-new-version-using-github-actions-108k
+
+git tag -a "v0.0.6" -m "new tag"
+git push --tags
+"""
+
 import io
 import os
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
@@ -98,15 +113,15 @@
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version=about['__version__'],
+    version='0.0.6',
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
```

### Comparing `phase-o-matic-0.0.4/tests/test_download.py` & `phase-o-matic-0.0.6/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.4/tests/test_preprocess.py` & `phase-o-matic-0.0.6/tests/test_preprocess.py`

 * *Files identical despite different names*

