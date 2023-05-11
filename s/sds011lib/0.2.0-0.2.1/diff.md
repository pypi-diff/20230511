# Comparing `tmp/sds011lib-0.2.0.tar.gz` & `tmp/sds011lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sds011lib-0.2.0.tar", max compression
+gzip compressed data, was "sds011lib-0.2.1.tar", max compression
```

## Comparing `sds011lib-0.2.0.tar` & `sds011lib-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-11 03:31:51.862807 sds011lib-0.2.0/LICENSE
--rw-r--r--   0        0        0      710 2023-05-11 03:31:51.862807 sds011lib-0.2.0/README.md
--rw-r--r--   0        0        0      955 2023-05-11 03:31:51.866807 sds011lib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    19852 2023-05-11 03:31:51.866807 sds011lib-0.2.0/sds011lib/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-11 03:31:51.866807 sds011lib-0.2.0/sds011lib/constants.py
--rw-r--r--   0        0        0     2332 2023-05-11 03:31:51.866807 sds011lib-0.2.0/sds011lib/exceptions.py
--rw-r--r--   0        0        0     5797 2023-05-11 03:31:51.866807 sds011lib-0.2.0/sds011lib/responses.py
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 sds011lib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-11 04:19:13.201784 sds011lib-0.2.1/LICENSE
+-rw-r--r--   0        0        0      710 2023-05-11 04:19:13.201784 sds011lib-0.2.1/README.md
+-rw-r--r--   0        0        0      955 2023-05-11 04:19:13.201784 sds011lib-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    19852 2023-05-11 04:19:13.201784 sds011lib-0.2.1/sds011lib/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-11 04:19:13.201784 sds011lib-0.2.1/sds011lib/constants.py
+-rw-r--r--   0        0        0     2332 2023-05-11 04:19:13.201784 sds011lib-0.2.1/sds011lib/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-11 04:19:13.201784 sds011lib-0.2.1/sds011lib/py.typed
+-rw-r--r--   0        0        0     5797 2023-05-11 04:19:13.201784 sds011lib-0.2.1/sds011lib/responses.py
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 sds011lib-0.2.1/PKG-INFO
```

### Comparing `sds011lib-0.2.0/LICENSE` & `sds011lib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sds011lib-0.2.0/README.md` & `sds011lib-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sds011lib-0.2.0/pyproject.toml` & `sds011lib-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sds011lib"
-version = "0.2.0"
+version = "0.2.1"
 description = "SDS011 Library"
 authors = ["Tim Orme <TimothyOrme@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyserial = "^3.5"
```

### Comparing `sds011lib-0.2.0/sds011lib/__init__.py` & `sds011lib-0.2.1/sds011lib/__init__.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.2.0/sds011lib/constants.py` & `sds011lib-0.2.1/sds011lib/constants.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.2.0/sds011lib/exceptions.py` & `sds011lib-0.2.1/sds011lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.2.0/sds011lib/responses.py` & `sds011lib-0.2.1/sds011lib/responses.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.2.0/PKG-INFO` & `sds011lib-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sds011lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: SDS011 Library
 Author: Tim Orme
 Author-email: TimothyOrme@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

