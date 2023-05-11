# Comparing `tmp/typename-1.0.1.tar.gz` & `tmp/typename-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typename-1.0.1.tar", last modified: Thu May 11 08:20:33 2023, max compression
+gzip compressed data, was "typename-1.0.2.tar", last modified: Thu May 11 08:45:19 2023, max compression
```

## Comparing `typename-1.0.1.tar` & `typename-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:20:33.977342 typename-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 08:20:19.000000 typename-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-11 08:20:33.977342 typename-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-11 08:20:19.000000 typename-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-11 08:20:19.000000 typename-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-11 08:20:33.977342 typename-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:20:33.977342 typename-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:20:33.977342 typename-1.0.1/src/typename/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-11 08:20:19.000000 typename-1.0.1/src/typename/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:20:33.977342 typename-1.0.1/src/typename.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-11 08:20:33.000000 typename-1.0.1/src/typename.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-11 08:20:33.000000 typename-1.0.1/src/typename.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:20:33.000000 typename-1.0.1/src/typename.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 08:20:33.000000 typename-1.0.1/src/typename.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 08:20:33.000000 typename-1.0.1/src/typename.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:20:33.000000 typename-1.0.1/src/typename.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:20:33.977342 typename-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 08:20:19.000000 typename-1.0.1/tests/test_typename.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:45:19.368553 typename-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 08:45:00.000000 typename-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-11 08:45:19.368553 typename-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-11 08:45:00.000000 typename-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-11 08:45:00.000000 typename-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-11 08:45:19.368553 typename-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:45:19.364554 typename-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:45:19.364554 typename-1.0.2/src/typename/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-11 08:45:00.000000 typename-1.0.2/src/typename/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:45:19.368553 typename-1.0.2/src/typename.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-11 08:45:19.000000 typename-1.0.2/src/typename.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-11 08:45:19.000000 typename-1.0.2/src/typename.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:45:19.000000 typename-1.0.2/src/typename.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 08:45:19.000000 typename-1.0.2/src/typename.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 08:45:19.000000 typename-1.0.2/src/typename.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:45:19.000000 typename-1.0.2/src/typename.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:45:19.368553 typename-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 08:45:00.000000 typename-1.0.2/tests/test_typename.py
```

### Comparing `typename-1.0.1/LICENSE.txt` & `typename-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `typename-1.0.1/PKG-INFO` & `typename-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typename
-Version: 1.0.1
+Version: 1.0.2
 Summary: Obtain the name of the type of an object
 Home-page: https://github.com/sixty-north/typename
 Author: Sixty North
 Author-email: systems+typename@sixty-north.com
 License: MIT License
 Keywords: Python types typename
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `typename-1.0.1/setup.cfg` & `typename-1.0.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 zip_safe = True
 include_package_data = False
 package_dir = 
 	=src
 packages = find:
 
 [options.extras_require]
-dev = bumpversion
+dev = bumpversion; build; twine
 test = pytest
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `typename-1.0.1/src/typename.egg-info/PKG-INFO` & `typename-1.0.2/src/typename.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typename
-Version: 1.0.1
+Version: 1.0.2
 Summary: Obtain the name of the type of an object
 Home-page: https://github.com/sixty-north/typename
 Author: Sixty North
 Author-email: systems+typename@sixty-north.com
 License: MIT License
 Keywords: Python types typename
 Classifier: Development Status :: 3 - Alpha
```

