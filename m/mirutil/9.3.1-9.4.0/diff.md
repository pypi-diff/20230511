# Comparing `tmp/mirutil-9.3.1.tar.gz` & `tmp/mirutil-9.4.0.tar.gz`

## Comparing `mirutil-9.3.1.tar` & `mirutil-9.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mirutil-9.3.1/.gitattributes
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 mirutil-9.3.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/__init__.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/async_requests.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/codal.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/const.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/datalore.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/df_utils.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/jdate.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/latex.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/ns.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/pathes.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/string_funcs.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/tsetmc.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mirutil-9.3.1/src/mirutil/utils.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 mirutil-9.3.1/test/t_async_requests.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 mirutil-9.3.1/test/t_download.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mirutil-9.3.1/test/test.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 mirutil-9.3.1/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 mirutil-9.3.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mirutil-9.3.1/README.md
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 mirutil-9.3.1/pyproject.toml
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 mirutil-9.3.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mirutil-9.4.0/.gitattributes
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 mirutil-9.4.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/__init__.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/async_requests.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/codal.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/const.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/datalore.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/df_utils.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/jdate.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/latex.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/ns.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/pathes.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/string_funcs.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/tsetmc.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mirutil-9.4.0/src/mirutil/utils.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 mirutil-9.4.0/test/t_async_requests.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 mirutil-9.4.0/test/t_download.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mirutil-9.4.0/test/test.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 mirutil-9.4.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 mirutil-9.4.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mirutil-9.4.0/README.md
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 mirutil-9.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 mirutil-9.4.0/PKG-INFO
```

### Comparing `mirutil-9.3.1/src/mirutil/async_requests.py` & `mirutil-9.4.0/src/mirutil/async_requests.py`

 * *Files identical despite different names*

### Comparing `mirutil-9.3.1/src/mirutil/datalore.py` & `mirutil-9.4.0/src/mirutil/datalore.py`

 * *Files identical despite different names*

### Comparing `mirutil-9.3.1/src/mirutil/df_utils.py` & `mirutil-9.4.0/src/mirutil/df_utils.py`

 * *Files identical despite different names*

### Comparing `mirutil-9.3.1/src/mirutil/jdate.py` & `mirutil-9.4.0/src/mirutil/jdate.py`

 * *Files identical despite different names*

### Comparing `mirutil-9.3.1/src/mirutil/latex.py` & `mirutil-9.4.0/src/mirutil/latex.py`

 * *Files identical despite different names*

### Comparing `mirutil-9.3.1/src/mirutil/ns.py` & `mirutil-9.4.0/src/mirutil/ns.py`

 * *Files identical despite different names*

### Comparing `mirutil-9.3.1/src/mirutil/pathes.py` & `mirutil-9.4.0/src/mirutil/pathes.py`

 * *Files identical despite different names*

### Comparing `mirutil-9.3.1/src/mirutil/string_funcs.py` & `mirutil-9.4.0/src/mirutil/string_funcs.py`

 * *Files identical despite different names*

### Comparing `mirutil-9.3.1/src/mirutil/tsetmc.py` & `mirutil-9.4.0/src/mirutil/tsetmc.py`

 * *Files identical despite different names*

### Comparing `mirutil-9.3.1/src/mirutil/utils.py` & `mirutil-9.4.0/src/mirutil/utils.py`

 * *Files identical despite different names*

### Comparing `mirutil-9.3.1/.gitignore` & `mirutil-9.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mirutil-9.3.1/LICENSE` & `mirutil-9.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mirutil-9.3.1/pyproject.toml` & `mirutil-9.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mirutil"
-version = "9.3.1"
+version = "9.4.0"
 authors = [{ name = "Mahdi Mir", email = "imahdimir@gmail.com" }]
 description = "Tools for getting and cleaning TSE data"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
     "persiantools",
     "pandas",
```

### Comparing `mirutil-9.3.1/PKG-INFO` & `mirutil-9.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirutil
-Version: 9.3.1
+Version: 9.4.0
 Summary: Tools for getting and cleaning TSE data
 Project-URL: Homepage, https://github.com/imahdimir/mirutil
 Project-URL: Bug Tracker, https://github.com/imahdimir/mirutil/issues
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
```

