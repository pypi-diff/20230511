# Comparing `tmp/lazi-1.1.0.post13.tar.gz` & `tmp/lazi-1.2.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.1.0.post13.tar", max compression
+gzip compressed data, was "lazi-1.2.0.15.tar", max compression
```

## Comparing `lazi-1.1.0.post13.tar` & `lazi-1.2.0.15.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.1.0.post13/LICENSE
--rw-r--r--   0        0        0      980 2023-05-10 07:53:22.639513 lazi-1.1.0.post13/README.md
--rw-r--r--   0        0        0      104 2023-05-11 08:57:20.841058 lazi-1.1.0.post13/lazi/auto.py
--rw-r--r--   0        0        0       37 2023-05-11 10:10:32.878224 lazi-1.1.0.post13/lazi/conf/all.py
--rw-r--r--   0        0        0      863 2023-05-11 10:10:32.874224 lazi-1.1.0.post13/lazi/conf/base.py
--rw-r--r--   0        0        0      720 2023-05-11 10:24:25.485088 lazi-1.1.0.post13/lazi/conf/conf.py
--rw-r--r--   0        0        0      453 2023-05-11 09:12:13.132626 lazi-1.1.0.post13/lazi/core/__init__.py
--rw-r--r--   0        0        0     3173 2023-05-11 10:24:25.477088 lazi-1.1.0.post13/lazi/core/finder.py
--rw-r--r--   0        0        0     2609 2023-05-11 09:48:59.517349 lazi-1.1.0.post13/lazi/core/loader.py
--rw-r--r--   0        0        0     4953 2023-05-11 10:24:25.461088 lazi-1.1.0.post13/lazi/core/record.py
--rw-r--r--   0        0        0      815 2023-05-11 10:00:09.202100 lazi-1.1.0.post13/lazi/core/util.py
--rw-r--r--   0        0        0       32 2023-05-11 08:56:50.716672 lazi-1.1.0.post13/lazi/lazi.py
--rw-r--r--   0        0        0     1166 2023-05-11 10:39:13.272620 lazi-1.1.0.post13/pyproject.toml
--rw-r--r--   0        0        0     2130 1970-01-01 00:00:00.000000 lazi-1.1.0.post13/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.2.0.15/LICENSE
+-rw-r--r--   0        0        0     1386 2023-05-11 11:12:42.598828 lazi-1.2.0.15/README.md
+-rw-r--r--   0        0        0      104 2023-05-11 08:57:20.841058 lazi-1.2.0.15/lazi/auto.py
+-rw-r--r--   0        0        0       37 2023-05-11 10:10:32.878224 lazi-1.2.0.15/lazi/conf/all.py
+-rw-r--r--   0        0        0      863 2023-05-11 10:10:32.874224 lazi-1.2.0.15/lazi/conf/base.py
+-rw-r--r--   0        0        0      720 2023-05-11 10:24:25.485088 lazi-1.2.0.15/lazi/conf/conf.py
+-rw-r--r--   0        0        0      593 2023-05-11 11:10:16.320921 lazi-1.2.0.15/lazi/core/__init__.py
+-rw-r--r--   0        0        0     3173 2023-05-11 10:24:25.477088 lazi-1.2.0.15/lazi/core/finder.py
+-rw-r--r--   0        0        0     2609 2023-05-11 09:48:59.517349 lazi-1.2.0.15/lazi/core/loader.py
+-rw-r--r--   0        0        0     4953 2023-05-11 10:24:25.461088 lazi-1.2.0.15/lazi/core/record.py
+-rw-r--r--   0        0        0      815 2023-05-11 10:00:09.202100 lazi-1.2.0.15/lazi/core/util.py
+-rw-r--r--   0        0        0     1166 2023-05-11 11:16:15.941606 lazi-1.2.0.15/pyproject.toml
+-rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 lazi-1.2.0.15/PKG-INFO
```

### Comparing `lazi-1.1.0.post13/LICENSE` & `lazi-1.2.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `lazi-1.1.0.post13/README.md` & `lazi-1.2.0.15/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -5,33 +5,48 @@
 ## Usage:
 
 ```shell
 poetry add lazi
 ```
 
 ```python
-"""example.py
+"""Automatic lazy loading example.
 
-Automatic lazy loading example.
 Install django to run, or change the imports.
 """
 import lazi.auto                 # Install import tracking.
 import django.test               # Import stuff.
-print(len(lazi.auto.RECORD))     # Peek at the internals for demonstration.
+print(lazi.used_count())         # Count loaded modules.
 TestCase = django.test.TestCase  # Trigger lazy loading.
-print(len(lazi.auto.RECORD))     # More modules were lazy loaded.
+print(lazi.used_count())         # More modules were lazy loaded.
 ```
 
 ```shell
 python example.py
 ```
 
 ```python
-6
-198
+5
+211
+```
+
+```python
+"""Manual lazy loading example.
+"""
+import lazi.core                        # Import Lazi.
+django = lazi.lazy("django")            # Import stuff.
+django_test = lazi.lazy("django.test")  # Import more stuff.
+print(lazi.used_count())                # Count loaded modules.
+TestCase = django_test.TestCase         # Trigger lazy loading.
+print(lazi.used_count())                # Module was lazy loaded.
+```
+
+```python
+1
+2
 ```
 
 ## Metadata
 
 Reference for developers: The json dict below contains Python versioning parameters:
 - Soft `min` (ignore rev) & hard `max` compatible versions.
 - Recommended `use` & creator's environment `dev` versions.
```

### Comparing `lazi-1.1.0.post13/lazi/conf/base.py` & `lazi-1.2.0.15/lazi/conf/base.py`

 * *Files identical despite different names*

### Comparing `lazi-1.1.0.post13/lazi/conf/conf.py` & `lazi-1.2.0.15/lazi/conf/conf.py`

 * *Files identical despite different names*

### Comparing `lazi-1.1.0.post13/lazi/core/finder.py` & `lazi-1.2.0.15/lazi/core/finder.py`

 * *Files identical despite different names*

### Comparing `lazi-1.1.0.post13/lazi/core/loader.py` & `lazi-1.2.0.15/lazi/core/loader.py`

 * *Files identical despite different names*

### Comparing `lazi-1.1.0.post13/lazi/core/record.py` & `lazi-1.2.0.15/lazi/core/record.py`

 * *Files identical despite different names*

### Comparing `lazi-1.1.0.post13/lazi/core/util.py` & `lazi-1.2.0.15/lazi/core/util.py`

 * *Files identical despite different names*

### Comparing `lazi-1.1.0.post13/pyproject.toml` & `lazi-1.2.0.15/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.1.0-13"
+version = "1.2.0.15"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "README.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
```

### Comparing `lazi-1.1.0.post13/PKG-INFO` & `lazi-1.2.0.15/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazi
-Version: 1.1.0.post13
+Version: 1.2.0.15
 Summary: A lightweight and extensible way to implement lazy imports globally.
 Home-page: https://github.com/sitbon/lazi
 License: AGPLv3
 Author: Phillip Sitbon
 Author-email: phillip.sitbon@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: Environment :: Web Environment
@@ -32,33 +32,48 @@
 ## Usage:
 
 ```shell
 poetry add lazi
 ```
 
 ```python
-"""example.py
+"""Automatic lazy loading example.
 
-Automatic lazy loading example.
 Install django to run, or change the imports.
 """
 import lazi.auto                 # Install import tracking.
 import django.test               # Import stuff.
-print(len(lazi.auto.RECORD))     # Peek at the internals for demonstration.
+print(lazi.used_count())         # Count loaded modules.
 TestCase = django.test.TestCase  # Trigger lazy loading.
-print(len(lazi.auto.RECORD))     # More modules were lazy loaded.
+print(lazi.used_count())         # More modules were lazy loaded.
 ```
 
 ```shell
 python example.py
 ```
 
 ```python
-6
-198
+5
+211
+```
+
+```python
+"""Manual lazy loading example.
+"""
+import lazi.core                        # Import Lazi.
+django = lazi.lazy("django")            # Import stuff.
+django_test = lazi.lazy("django.test")  # Import more stuff.
+print(lazi.used_count())                # Count loaded modules.
+TestCase = django_test.TestCase         # Trigger lazy loading.
+print(lazi.used_count())                # Module was lazy loaded.
+```
+
+```python
+1
+2
 ```
 
 ## Metadata
 
 Reference for developers: The json dict below contains Python versioning parameters:
 - Soft `min` (ignore rev) & hard `max` compatible versions.
 - Recommended `use` & creator's environment `dev` versions.
```

