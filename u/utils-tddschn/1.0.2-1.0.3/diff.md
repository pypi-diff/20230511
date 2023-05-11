# Comparing `tmp/utils_tddschn-1.0.2.tar.gz` & `tmp/utils_tddschn-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_tddschn-1.0.2.tar", max compression
+gzip compressed data, was "utils_tddschn-1.0.3.tar", max compression
```

## Comparing `utils_tddschn-1.0.2.tar` & `utils_tddschn-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1113 2023-05-11 04:08:08.457345 utils_tddschn-1.0.2/LICENSE
--rw-r--r--   0        0        0        0 2023-05-11 04:08:08.457728 utils_tddschn-1.0.2/README.md
--rw-r--r--   0        0        0      739 2023-05-11 04:16:58.670821 utils_tddschn-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-11 04:16:58.671436 utils_tddschn-1.0.2/utils_tddschn/__init__.py
--rw-r--r--   0        0        0      102 2023-05-11 04:16:42.627974 utils_tddschn-1.0.2/utils_tddschn/fs/__init__.py
--rw-r--r--   0        0        0     1056 2023-05-11 04:15:18.224890 utils_tddschn-1.0.2/utils_tddschn/fs/fs.py
--rw-r--r--   0        0        0      857 2023-05-11 04:08:08.459665 utils_tddschn-1.0.2/utils_tddschn/git.py
--rw-r--r--   0        0        0     1265 2023-05-11 04:08:08.459905 utils_tddschn-1.0.2/utils_tddschn/sync/git.py
--rw-r--r--   0        0        0      619 2023-05-11 04:08:08.460072 utils_tddschn-1.0.2/utils_tddschn/sync/numpy.py
--rw-r--r--   0        0        0       24 2023-05-11 04:08:08.460230 utils_tddschn-1.0.2/utils_tddschn/sync/text.py
--rw-r--r--   0        0        0      646 2023-05-11 04:08:08.460404 utils_tddschn-1.0.2/utils_tddschn/sync/utils.py
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 utils_tddschn-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1113 2023-05-11 04:08:08.457345 utils_tddschn-1.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-11 04:08:08.457728 utils_tddschn-1.0.3/README.md
+-rw-r--r--   0        0        0      739 2023-05-11 04:28:44.940513 utils_tddschn-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-11 04:28:44.941146 utils_tddschn-1.0.3/utils_tddschn/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-11 04:16:42.627974 utils_tddschn-1.0.3/utils_tddschn/fs/__init__.py
+-rw-r--r--   0        0        0     1217 2023-05-11 04:28:39.557712 utils_tddschn-1.0.3/utils_tddschn/fs/fs.py
+-rw-r--r--   0        0        0      857 2023-05-11 04:08:08.459665 utils_tddschn-1.0.3/utils_tddschn/git.py
+-rw-r--r--   0        0        0     1265 2023-05-11 04:08:08.459905 utils_tddschn-1.0.3/utils_tddschn/sync/git.py
+-rw-r--r--   0        0        0      619 2023-05-11 04:08:08.460072 utils_tddschn-1.0.3/utils_tddschn/sync/numpy.py
+-rw-r--r--   0        0        0       24 2023-05-11 04:08:08.460230 utils_tddschn-1.0.3/utils_tddschn/sync/text.py
+-rw-r--r--   0        0        0      646 2023-05-11 04:08:08.460404 utils_tddschn-1.0.3/utils_tddschn/sync/utils.py
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 utils_tddschn-1.0.3/PKG-INFO
```

### Comparing `utils_tddschn-1.0.2/LICENSE` & `utils_tddschn-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `utils_tddschn-1.0.2/pyproject.toml` & `utils_tddschn-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utils-tddschn"
-version = "1.0.2"
+version = "1.0.3"
 description = ""
 authors = ["Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tddschn/utils-tddschn"
 repository = "https://github.com/tddschn/utils-tddschn"
 keywords = ["numpy", "utility"]
```

### Comparing `utils_tddschn-1.0.2/utils_tddschn/fs/fs.py` & `utils_tddschn-1.0.3/utils_tddschn/fs/fs.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,9 +30,14 @@
         files = dir_path.iterdir()
     else:
         if recursive:
             files = dir_path.rglob(glob_pattern)
         else:
             files = dir_path.glob(glob_pattern)
 
-    last_added_file = max(files, key=get_creation_time)
-    return last_added_file
+    try:
+        last_added_file = max(files, key=get_creation_time)
+        return last_added_file
+    except:
+        raise ValueError(
+            f"No files found in {dir_path} with pattern {glob_pattern} (recursive={recursive})"
+        )
```

### Comparing `utils_tddschn-1.0.2/utils_tddschn/git.py` & `utils_tddschn-1.0.3/utils_tddschn/git.py`

 * *Files identical despite different names*

### Comparing `utils_tddschn-1.0.2/utils_tddschn/sync/git.py` & `utils_tddschn-1.0.3/utils_tddschn/sync/git.py`

 * *Files identical despite different names*

### Comparing `utils_tddschn-1.0.2/utils_tddschn/sync/numpy.py` & `utils_tddschn-1.0.3/utils_tddschn/sync/numpy.py`

 * *Files identical despite different names*

### Comparing `utils_tddschn-1.0.2/utils_tddschn/sync/utils.py` & `utils_tddschn-1.0.3/utils_tddschn/sync/utils.py`

 * *Files identical despite different names*

### Comparing `utils_tddschn-1.0.2/PKG-INFO` & `utils_tddschn-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-tddschn
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Home-page: https://github.com/tddschn/utils-tddschn
 License: MIT
 Keywords: numpy,utility
 Author: Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

