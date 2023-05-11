# Comparing `tmp/xguard-1.0.2.tar.gz` & `tmp/xguard-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xguard-1.0.2.tar", last modified: Thu May 11 13:12:48 2023, max compression
+gzip compressed data, was "xguard-1.0.3.tar", last modified: Thu May 11 12:58:58 2023, max compression
```

## Comparing `xguard-1.0.2.tar` & `xguard-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gus       (1000) gus       (1000)        0 2023-05-11 13:12:48.974598 xguard-1.0.2/
--rw-r--r--   0 gus       (1000) gus       (1000)     3562 2023-05-11 13:12:48.971265 xguard-1.0.2/PKG-INFO
--rw-r--r--   0 gus       (1000) gus       (1000)     3122 2023-05-11 13:11:41.000000 xguard-1.0.2/README.txt
-drwxr-xr-x   0 gus       (1000) gus       (1000)        0 2023-05-11 13:12:48.971265 xguard-1.0.2/core/
--rw-r--r--   0 gus       (1000) gus       (1000)     1005 2023-05-11 12:22:04.000000 xguard-1.0.2/core/__init__.py
--rw-r--r--   0 gus       (1000) gus       (1000)       38 2023-05-11 13:12:48.974598 xguard-1.0.2/setup.cfg
--rw-r--r--   0 gus       (1000) gus       (1000)      696 2023-05-11 13:12:13.000000 xguard-1.0.2/setup.py
-drwxr-xr-x   0 gus       (1000) gus       (1000)        0 2023-05-11 13:12:48.971265 xguard-1.0.2/tests/
--rw-r--r--   0 gus       (1000) gus       (1000)       90 2023-05-11 12:57:45.000000 xguard-1.0.2/tests/test_is_gt.py
-drwxr-xr-x   0 gus       (1000) gus       (1000)        0 2023-05-11 13:12:48.971265 xguard-1.0.2/xguard.egg-info/
--rw-r--r--   0 gus       (1000) gus       (1000)     3562 2023-05-11 13:12:48.000000 xguard-1.0.2/xguard.egg-info/PKG-INFO
--rw-r--r--   0 gus       (1000) gus       (1000)      176 2023-05-11 13:12:48.000000 xguard-1.0.2/xguard.egg-info/SOURCES.txt
--rw-r--r--   0 gus       (1000) gus       (1000)        1 2023-05-11 13:12:48.000000 xguard-1.0.2/xguard.egg-info/dependency_links.txt
--rw-r--r--   0 gus       (1000) gus       (1000)        5 2023-05-11 13:12:48.000000 xguard-1.0.2/xguard.egg-info/top_level.txt
+drwxr-xr-x   0 gus       (1000) gus       (1000)        0 2023-05-11 12:58:58.991208 xguard-1.0.3/
+-rw-r--r--   0 gus       (1000) gus       (1000)     3582 2023-05-11 12:58:58.991208 xguard-1.0.3/PKG-INFO
+-rw-r--r--   0 gus       (1000) gus       (1000)     3142 2023-05-11 12:54:33.000000 xguard-1.0.3/README.txt
+drwxr-xr-x   0 gus       (1000) gus       (1000)        0 2023-05-11 12:58:58.987874 xguard-1.0.3/core/
+-rw-r--r--   0 gus       (1000) gus       (1000)     1005 2023-05-11 12:22:04.000000 xguard-1.0.3/core/__init__.py
+-rw-r--r--   0 gus       (1000) gus       (1000)       38 2023-05-11 12:58:58.991208 xguard-1.0.3/setup.cfg
+-rw-r--r--   0 gus       (1000) gus       (1000)      696 2023-05-11 12:58:23.000000 xguard-1.0.3/setup.py
+drwxr-xr-x   0 gus       (1000) gus       (1000)        0 2023-05-11 12:58:58.991208 xguard-1.0.3/tests/
+-rw-r--r--   0 gus       (1000) gus       (1000)       90 2023-05-11 12:57:45.000000 xguard-1.0.3/tests/test_is_gt.py
+drwxr-xr-x   0 gus       (1000) gus       (1000)        0 2023-05-11 12:58:58.991208 xguard-1.0.3/xguard.egg-info/
+-rw-r--r--   0 gus       (1000) gus       (1000)     3582 2023-05-11 12:58:58.000000 xguard-1.0.3/xguard.egg-info/PKG-INFO
+-rw-r--r--   0 gus       (1000) gus       (1000)      176 2023-05-11 12:58:58.000000 xguard-1.0.3/xguard.egg-info/SOURCES.txt
+-rw-r--r--   0 gus       (1000) gus       (1000)        1 2023-05-11 12:58:58.000000 xguard-1.0.3/xguard.egg-info/dependency_links.txt
+-rw-r--r--   0 gus       (1000) gus       (1000)        5 2023-05-11 12:58:58.000000 xguard-1.0.3/xguard.egg-info/top_level.txt
```

### Comparing `xguard-1.0.2/PKG-INFO` & `xguard-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: xguard
-Version: 1.0.2
+Version: 1.0.3
 Summary: yet another guard clauses libary
 Home-page: https://github.com/johngitahi/xguard
 Author: John Gitahi
 Author-email: gitahi109@gmail.com
 License: MIT
 Keywords: guard clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # xguard
 
-![PyPI version](https://badge.fury.io/py/xguard.svg)](https://badge.fury.io/py/xguard)
-![License: GPLv3](https://img.shields.io/github/license/johngitahi/xguard?style=plastic)
+[![PyPI version](https://badge.fury.io/py/xguard.svg)](https://badge.fury.io/py/xguard)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 Xguard is yet another guard clause library.
 
 ## What are Guard Clauses
 A guard clause is simply a check that immediately exits the function, either with a return statement or an exception. If you're used to writing functions that check to ensure everything is valid for the function to run, then you write the main function code, and then you write else statements to deal with error cases, this involves inverting your current workflow. The benefit is that your code will tend to be shorter and simpler, and less deeply indented. [Credit](https://deviq.com/design-patterns/guard-clause)
 
 ## How to use this library
```

### Comparing `xguard-1.0.2/README.txt` & `xguard-1.0.3/README.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # xguard
 
-![PyPI version](https://badge.fury.io/py/xguard.svg)](https://badge.fury.io/py/xguard)
-![License: GPLv3](https://img.shields.io/github/license/johngitahi/xguard?style=plastic)
+[![PyPI version](https://badge.fury.io/py/xguard.svg)](https://badge.fury.io/py/xguard)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 Xguard is yet another guard clause library.
 
 ## What are Guard Clauses
 A guard clause is simply a check that immediately exits the function, either with a return statement or an exception. If you're used to writing functions that check to ensure everything is valid for the function to run, then you write the main function code, and then you write else statements to deal with error cases, this involves inverting your current workflow. The benefit is that your code will tend to be shorter and simpler, and less deeply indented. [Credit](https://deviq.com/design-patterns/guard-clause)
 
 ## How to use this library
```

### Comparing `xguard-1.0.2/core/__init__.py` & `xguard-1.0.3/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xguard-1.0.2/setup.py` & `xguard-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.txt", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="xguard",
-    version="1.0.2",
+    version="1.0.3",
     author="John Gitahi",
     author_email="gitahi109@gmail.com",
     description="yet another guard clauses libary",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     url="https://github.com/johngitahi/xguard",
```

### Comparing `xguard-1.0.2/xguard.egg-info/PKG-INFO` & `xguard-1.0.3/xguard.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: xguard
-Version: 1.0.2
+Version: 1.0.3
 Summary: yet another guard clauses libary
 Home-page: https://github.com/johngitahi/xguard
 Author: John Gitahi
 Author-email: gitahi109@gmail.com
 License: MIT
 Keywords: guard clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # xguard
 
-![PyPI version](https://badge.fury.io/py/xguard.svg)](https://badge.fury.io/py/xguard)
-![License: GPLv3](https://img.shields.io/github/license/johngitahi/xguard?style=plastic)
+[![PyPI version](https://badge.fury.io/py/xguard.svg)](https://badge.fury.io/py/xguard)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 Xguard is yet another guard clause library.
 
 ## What are Guard Clauses
 A guard clause is simply a check that immediately exits the function, either with a return statement or an exception. If you're used to writing functions that check to ensure everything is valid for the function to run, then you write the main function code, and then you write else statements to deal with error cases, this involves inverting your current workflow. The benefit is that your code will tend to be shorter and simpler, and less deeply indented. [Credit](https://deviq.com/design-patterns/guard-clause)
 
 ## How to use this library
```

