# Comparing `tmp/pqinput-0.0.4.tar.gz` & `tmp/pqinput-0.0.400.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqinput-0.0.4.tar", last modified: Wed May 10 13:25:45 2023, max compression
+gzip compressed data, was "pqinput-0.0.400.tar", last modified: Wed May 10 13:35:19 2023, max compression
```

## Comparing `pqinput-0.0.4.tar` & `pqinput-0.0.400.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 13:25:45.898127 pqinput-0.0.4/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.4/LICENSE.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3885 2023-05-10 13:25:45.898127 pqinput-0.0.4/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3314 2023-05-09 09:41:50.000000 pqinput-0.0.4/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 13:25:45.898127 pqinput-0.0.4/pqinput/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      106 2023-05-09 11:00:00.000000 pqinput-0.0.4/pqinput/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8243 2023-05-10 13:13:23.000000 pqinput-0.0.4/pqinput/drawPES.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    14637 2023-05-10 13:19:55.000000 pqinput-0.0.4/pqinput/inpxml.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 13:25:45.898127 pqinput-0.0.4/pqinput.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3885 2023-05-10 13:25:45.000000 pqinput-0.0.4/pqinput.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      226 2023-05-10 13:25:45.000000 pqinput-0.0.4/pqinput.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-10 13:25:45.000000 pqinput-0.0.4/pqinput.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-10 13:25:45.000000 pqinput-0.0.4/pqinput.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      540 2023-05-10 13:25:01.000000 pqinput-0.0.4/pyproject.toml
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-10 13:25:45.898127 pqinput-0.0.4/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      651 2023-05-10 13:24:53.000000 pqinput-0.0.4/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 13:35:19.195708 pqinput-0.0.400/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.400/LICENSE.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3887 2023-05-10 13:35:19.195708 pqinput-0.0.400/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3314 2023-05-09 09:41:50.000000 pqinput-0.0.400/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 13:35:19.195708 pqinput-0.0.400/pqinput/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      106 2023-05-09 11:00:00.000000 pqinput-0.0.400/pqinput/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8243 2023-05-10 13:13:23.000000 pqinput-0.0.400/pqinput/drawPES.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    14637 2023-05-10 13:19:55.000000 pqinput-0.0.400/pqinput/inpxml.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 13:35:19.195708 pqinput-0.0.400/pqinput.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3887 2023-05-10 13:35:19.000000 pqinput-0.0.400/pqinput.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      226 2023-05-10 13:35:19.000000 pqinput-0.0.400/pqinput.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-10 13:35:19.000000 pqinput-0.0.400/pqinput.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-10 13:35:19.000000 pqinput-0.0.400/pqinput.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      542 2023-05-10 13:34:58.000000 pqinput-0.0.400/pyproject.toml
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-10 13:35:19.195708 pqinput-0.0.400/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      653 2023-05-10 13:35:06.000000 pqinput-0.0.400/setup.py
```

### Comparing `pqinput-0.0.4/LICENSE.txt` & `pqinput-0.0.400/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.4/PKG-INFO` & `pqinput-0.0.400/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.4
+Version: 0.0.400
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.4/README.md` & `pqinput-0.0.400/README.md`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.4/pqinput/drawPES.py` & `pqinput-0.0.400/pqinput/drawPES.py`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.4/pqinput/inpxml.py` & `pqinput-0.0.400/pqinput/inpxml.py`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.4/pqinput.egg-info/PKG-INFO` & `pqinput-0.0.400/pqinput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.4
+Version: 0.0.400
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.4/pyproject.toml` & `pqinput-0.0.400/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pqinput"
-version = "0.0.4"
+version = "0.0.400"
 authors = [
   { name="Lucas Borges", email="lucas.borges@fysik.su.se" },
 ]
 description = "Create input files for QDng calculations"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pqinput-0.0.4/setup.py` & `pqinput-0.0.400/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name = "pqinput",
-    version = "0.0.4",
+    version = "0.0.400",
     author = "Lucas Borges",
     author_email = "lucas.borges@fysik.su.se",
     description = ("additional functions for QDng calculations setups."),
     license = "MIT",
     keywords = "qdng",
     url = "https://gitlab.fysik.su.se/lucas.borges/inputxml",
     packages=setuptools.find_packages(),
```

