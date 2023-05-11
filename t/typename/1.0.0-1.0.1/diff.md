# Comparing `tmp/typename-1.0.0.tar.gz` & `tmp/typename-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typename-1.0.0.tar", last modified: Thu May 11 08:11:57 2023, max compression
+gzip compressed data, was "typename-1.0.1.tar", last modified: Thu May 11 08:20:33 2023, max compression
```

## Comparing `typename-1.0.0.tar` & `typename-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rjs        (501) staff       (20)        0 2023-05-11 08:11:57.887616 typename-1.0.0/
--rw-r--r--   0 rjs        (501) staff       (20)     1063 2023-05-10 19:06:01.000000 typename-1.0.0/LICENSE.txt
--rw-r--r--   0 rjs        (501) staff       (20)     1712 2023-05-11 08:11:57.887664 typename-1.0.0/PKG-INFO
--rw-r--r--   0 rjs        (501) staff       (20)      310 2023-05-10 19:26:13.000000 typename-1.0.0/README.md
--rw-r--r--   0 rjs        (501) staff       (20)      375 2023-05-10 16:12:40.000000 typename-1.0.0/pyproject.toml
--rw-r--r--   0 rjs        (501) staff       (20)      840 2023-05-11 08:11:57.887926 typename-1.0.0/setup.cfg
-drwxr-xr-x   0 rjs        (501) staff       (20)        0 2023-05-11 08:11:57.886183 typename-1.0.0/src/
-drwxr-xr-x   0 rjs        (501) staff       (20)        0 2023-05-11 08:11:57.886801 typename-1.0.0/src/typename/
--rw-r--r--   0 rjs        (501) staff       (20)      405 2023-05-11 08:06:23.000000 typename-1.0.0/src/typename/__init__.py
-drwxr-xr-x   0 rjs        (501) staff       (20)        0 2023-05-11 08:11:57.887419 typename-1.0.0/src/typename.egg-info/
--rw-r--r--   0 rjs        (501) staff       (20)     1712 2023-05-11 08:11:57.000000 typename-1.0.0/src/typename.egg-info/PKG-INFO
--rw-r--r--   0 rjs        (501) staff       (20)      304 2023-05-11 08:11:57.000000 typename-1.0.0/src/typename.egg-info/SOURCES.txt
--rw-r--r--   0 rjs        (501) staff       (20)        1 2023-05-11 08:11:57.000000 typename-1.0.0/src/typename.egg-info/dependency_links.txt
--rw-r--r--   0 rjs        (501) staff       (20)       34 2023-05-11 08:11:57.000000 typename-1.0.0/src/typename.egg-info/requires.txt
--rw-r--r--   0 rjs        (501) staff       (20)        9 2023-05-11 08:11:57.000000 typename-1.0.0/src/typename.egg-info/top_level.txt
--rw-r--r--   0 rjs        (501) staff       (20)        1 2023-05-11 08:11:57.000000 typename-1.0.0/src/typename.egg-info/zip-safe
-drwxr-xr-x   0 rjs        (501) staff       (20)        0 2023-05-11 08:11:57.887524 typename-1.0.0/tests/
--rw-r--r--   0 rjs        (501) staff       (20)      155 2023-05-11 07:59:13.000000 typename-1.0.0/tests/test_typename.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:20:33.977342 typename-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 08:20:19.000000 typename-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-11 08:20:33.977342 typename-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-11 08:20:19.000000 typename-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-11 08:20:19.000000 typename-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-11 08:20:33.977342 typename-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:20:33.977342 typename-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:20:33.977342 typename-1.0.1/src/typename/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-11 08:20:19.000000 typename-1.0.1/src/typename/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:20:33.977342 typename-1.0.1/src/typename.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-11 08:20:33.000000 typename-1.0.1/src/typename.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-11 08:20:33.000000 typename-1.0.1/src/typename.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:20:33.000000 typename-1.0.1/src/typename.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 08:20:33.000000 typename-1.0.1/src/typename.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 08:20:33.000000 typename-1.0.1/src/typename.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:20:33.000000 typename-1.0.1/src/typename.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:20:33.977342 typename-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 08:20:19.000000 typename-1.0.1/tests/test_typename.py
```

### Comparing `typename-1.0.0/LICENSE.txt` & `typename-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `typename-1.0.0/PKG-INFO` & `typename-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typename
-Version: 1.0.0
+Version: 1.0.1
 Summary: Obtain the name of the type of an object
 Home-page: https://github.com/sixty-north/typename
 Author: Sixty North
 Author-email: systems+typename@sixty-north.com
 License: MIT License
 Keywords: Python types typename
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `typename-1.0.0/setup.cfg` & `typename-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `typename-1.0.0/src/typename.egg-info/PKG-INFO` & `typename-1.0.1/src/typename.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typename
-Version: 1.0.0
+Version: 1.0.1
 Summary: Obtain the name of the type of an object
 Home-page: https://github.com/sixty-north/typename
 Author: Sixty North
 Author-email: systems+typename@sixty-north.com
 License: MIT License
 Keywords: Python types typename
 Classifier: Development Status :: 3 - Alpha
```

