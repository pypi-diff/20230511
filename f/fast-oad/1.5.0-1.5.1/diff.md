# Comparing `tmp/fast_oad-1.5.0.tar.gz` & `tmp/fast_oad-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_oad-1.5.0.tar", max compression
+gzip compressed data, was "fast_oad-1.5.1.tar", max compression
```

## Comparing `fast_oad-1.5.0.tar` & `fast_oad-1.5.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3488 2023-04-27 14:57:39.585432 fast_oad-1.5.0/README.md
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.147289 fast_oad-1.5.0/_fastoad/__init__.py
--rw-r--r--   0        0        0     2400 2023-04-27 14:57:40.889530 fast_oad-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     4909 1970-01-01 00:00:00.000000 fast_oad-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3488 2023-05-11 14:35:39.051014 fast_oad-1.5.1/README.md
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.382809 fast_oad-1.5.1/_fastoad/__init__.py
+-rw-r--r--   0        0        0     2400 2023-05-11 14:35:40.535024 fast_oad-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4909 1970-01-01 00:00:00.000000 fast_oad-1.5.1/PKG-INFO
```

### Comparing `fast_oad-1.5.0/README.md` & `fast_oad-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fast_oad-1.5.0/_fastoad/__init__.py` & `fast_oad-1.5.1/_fastoad/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad-1.5.0/pyproject.toml` & `fast_oad-1.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "FAST-OAD"
-version = "1.5.0" # This version number is overwritten by GitHub packaging workflow but setting 1.3 here will allow installation of CS25 models in development mode
+version = "1.5.1" # This version number is overwritten by GitHub packaging workflow but setting 1.3 here will allow installation of CS25 models in development mode
 description = "FAST-OAD is a framework for performing rapid Overall Aircraft Design"
 readme = "README.md"
 authors = [
     "Christophe DAVID <christophe.david@onera.fr>",
     "Scott DELBECQ <Scott.DELBECQ@isae-supaero.fr>"
 ]
 packages = [{ include = "_fastoad"}]
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering :: Physics"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-fast-oad-core = "^1.5.0"
+fast-oad-core = "^1.5.1"
 fast-oad-cs25 = ">=0.1.4"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
```

### Comparing `fast_oad-1.5.0/PKG-INFO` & `fast_oad-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-oad
-Version: 1.5.0
+Version: 1.5.1
 Summary: FAST-OAD is a framework for performing rapid Overall Aircraft Design
 Home-page: https://github.com/fast-aircraft-design/FAST-OAD
 License: GPL-3.0-only
 Keywords: aircraft,design,multi-disciplinary
 Author: Christophe DAVID
 Author-email: christophe.david@onera.fr
 Requires-Python: >=3.7,<4.0
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: fast-oad-core (>=1.5.0,<2.0.0)
+Requires-Dist: fast-oad-core (>=1.5.1,<2.0.0)
 Requires-Dist: fast-oad-cs25 (>=0.1.4)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="docs/img/FAST_OAD_logo2.jpg" alt="FAST-OAD logo" width="600">
 </p>
```

