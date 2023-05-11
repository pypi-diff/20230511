# Comparing `tmp/scandal-0.1.1.tar.gz` & `tmp/scandal-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scandal-0.1.1.tar", max compression
+gzip compressed data, was "scandal-0.1.4.tar", max compression
```

## Comparing `scandal-0.1.1.tar` & `scandal-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       10 2023-05-11 10:48:24.685323 scandal-0.1.1/README.md
--rw-r--r--   0        0        0      693 2023-05-11 10:48:24.685323 scandal-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2467 2023-05-11 10:48:24.685323 scandal-0.1.1/scandal/__init__.py
--rw-r--r--   0        0        0      168 2023-05-11 10:48:24.685323 scandal-0.1.1/scandal/__main__.py
--rw-r--r--   0        0        0     3056 2023-05-11 10:48:24.685323 scandal-0.1.1/scandal/_auth.py
--rw-r--r--   0        0        0      114 2023-05-11 10:48:24.685323 scandal-0.1.1/scandal/_connection.py
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 scandal-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-05-11 15:09:29.169522 scandal-0.1.4/README.md
+-rw-r--r--   0        0        0      693 2023-05-11 15:09:29.169522 scandal-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2467 2023-05-11 15:09:29.169522 scandal-0.1.4/scandal/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-11 15:09:29.169522 scandal-0.1.4/scandal/__main__.py
+-rw-r--r--   0        0        0     3056 2023-05-11 15:09:29.169522 scandal-0.1.4/scandal/_auth.py
+-rw-r--r--   0        0        0      114 2023-05-11 15:09:29.169522 scandal-0.1.4/scandal/_connection.py
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 scandal-0.1.4/PKG-INFO
```

### Comparing `scandal-0.1.1/pyproject.toml` & `scandal-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scandal-0.1.1/scandal/__init__.py` & `scandal-0.1.4/scandal/__init__.py`

 * *Files identical despite different names*

### Comparing `scandal-0.1.1/scandal/_auth.py` & `scandal-0.1.4/scandal/_auth.py`

 * *Files identical despite different names*

### Comparing `scandal-0.1.1/PKG-INFO` & `scandal-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scandal
-Version: 0.1.1
+Version: 0.1.4
 Summary: 
 Author: Nicholas Gates
 Author-email: nick@nickgates.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

