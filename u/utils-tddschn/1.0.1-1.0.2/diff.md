# Comparing `tmp/utils-tddschn-1.0.1.tar.gz` & `tmp/utils_tddschn-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils-tddschn-1.0.1.tar", max compression
+gzip compressed data, was "utils_tddschn-1.0.2.tar", max compression
```

## Comparing `utils-tddschn-1.0.1.tar` & `utils_tddschn-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1113 2022-04-30 16:08:03.912675 utils-tddschn-1.0.1/LICENSE
--rw-r--r--   0        0        0        0 2022-04-24 13:06:34.906985 utils-tddschn-1.0.1/README.md
--rw-r--r--   0        0        0      739 2022-06-06 01:54:44.538723 utils-tddschn-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2022-06-06 01:54:44.539845 utils-tddschn-1.0.1/utils_tddschn/__init__.py
--rw-r--r--   0        0        0      857 2022-05-23 02:11:37.321922 utils-tddschn-1.0.1/utils_tddschn/git.py
--rw-r--r--   0        0        0     1265 2022-05-23 05:16:47.095172 utils-tddschn-1.0.1/utils_tddschn/sync/git.py
--rw-r--r--   0        0        0      619 2022-04-24 13:08:59.448577 utils-tddschn-1.0.1/utils_tddschn/sync/numpy.py
--rw-r--r--   0        0        0       24 2022-05-10 05:23:22.751711 utils-tddschn-1.0.1/utils_tddschn/sync/text.py
--rw-r--r--   0        0        0      646 2022-05-01 08:05:16.431802 utils-tddschn-1.0.1/utils_tddschn/sync/utils.py
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 utils-tddschn-1.0.1/setup.py
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 utils-tddschn-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1113 2023-05-11 04:08:08.457345 utils_tddschn-1.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-11 04:08:08.457728 utils_tddschn-1.0.2/README.md
+-rw-r--r--   0        0        0      739 2023-05-11 04:16:58.670821 utils_tddschn-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-11 04:16:58.671436 utils_tddschn-1.0.2/utils_tddschn/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-11 04:16:42.627974 utils_tddschn-1.0.2/utils_tddschn/fs/__init__.py
+-rw-r--r--   0        0        0     1056 2023-05-11 04:15:18.224890 utils_tddschn-1.0.2/utils_tddschn/fs/fs.py
+-rw-r--r--   0        0        0      857 2023-05-11 04:08:08.459665 utils_tddschn-1.0.2/utils_tddschn/git.py
+-rw-r--r--   0        0        0     1265 2023-05-11 04:08:08.459905 utils_tddschn-1.0.2/utils_tddschn/sync/git.py
+-rw-r--r--   0        0        0      619 2023-05-11 04:08:08.460072 utils_tddschn-1.0.2/utils_tddschn/sync/numpy.py
+-rw-r--r--   0        0        0       24 2023-05-11 04:08:08.460230 utils_tddschn-1.0.2/utils_tddschn/sync/text.py
+-rw-r--r--   0        0        0      646 2023-05-11 04:08:08.460404 utils_tddschn-1.0.2/utils_tddschn/sync/utils.py
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 utils_tddschn-1.0.2/PKG-INFO
```

### Comparing `utils-tddschn-1.0.1/LICENSE` & `utils_tddschn-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utils-tddschn-1.0.1/pyproject.toml` & `utils_tddschn-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utils-tddschn"
-version = "1.0.1"
+version = "1.0.2"
 description = ""
 authors = ["Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tddschn/utils-tddschn"
 repository = "https://github.com/tddschn/utils-tddschn"
 keywords = ["numpy", "utility"]
```

### Comparing `utils-tddschn-1.0.1/utils_tddschn/git.py` & `utils_tddschn-1.0.2/utils_tddschn/git.py`

 * *Files identical despite different names*

### Comparing `utils-tddschn-1.0.1/utils_tddschn/sync/git.py` & `utils_tddschn-1.0.2/utils_tddschn/sync/git.py`

 * *Files identical despite different names*

### Comparing `utils-tddschn-1.0.1/utils_tddschn/sync/numpy.py` & `utils_tddschn-1.0.2/utils_tddschn/sync/numpy.py`

 * *Files identical despite different names*

### Comparing `utils-tddschn-1.0.1/utils_tddschn/sync/utils.py` & `utils_tddschn-1.0.2/utils_tddschn/sync/utils.py`

 * *Files identical despite different names*

### Comparing `utils-tddschn-1.0.1/PKG-INFO` & `utils_tddschn-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: utils-tddschn
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Home-page: https://github.com/tddschn/utils-tddschn
 License: MIT
 Keywords: numpy,utility
 Author: Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Bug Tracker, https://github.com/tddschn/utils-tddschn/issues
 Project-URL: Repository, https://github.com/tddschn/utils-tddschn
 Description-Content-Type: text/markdown
```

