# Comparing `tmp/pikendus_backend-0.2.2.tar.gz` & `tmp/pikendus_backend-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikendus_backend-0.2.2.tar", last modified: Thu May 11 11:11:03 2023, max compression
+gzip compressed data, was "pikendus_backend-0.2.3.tar", last modified: Thu May 11 11:20:21 2023, max compression
```

## Comparing `pikendus_backend-0.2.2.tar` & `pikendus_backend-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-05-11 11:10:35.652582 pikendus_backend-0.2.2/LICENSE
--rw-r--r--   0        0        0     3105 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/PikendusWheelBuilder.py
--rw-r--r--   0        0        0     1702 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/__init__.py
--rw-r--r--   0        0        0      823 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/main.py
--rwxr-xr-x   0        0        0     3459 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/scripts/calc_dep_f90.py
--rw-r--r--   0        0        0     4213 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/scripts/compile.py
--rwxr-xr-x   0        0        0     1728 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/scripts/gene_py_src.py
--rwxr-xr-x   0        0        0     2117 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/scripts/ligne_debug.py
--rw-r--r--   0        0        0    13199 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/structure.py
--rw-r--r--   0        0        0     2652 2023-05-11 11:11:03.232354 pikendus_backend-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 pikendus_backend-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 11:19:52.671451 pikendus_backend-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3105 2023-05-11 11:19:52.671451 pikendus_backend-0.2.3/pikendus_backend/PikendusWheelBuilder.py
+-rw-r--r--   0        0        0     1702 2023-05-11 11:19:52.671451 pikendus_backend-0.2.3/pikendus_backend/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-11 11:19:52.671451 pikendus_backend-0.2.3/pikendus_backend/main.py
+-rwxr-xr-x   0        0        0     3459 2023-05-11 11:19:52.672451 pikendus_backend-0.2.3/pikendus_backend/scripts/calc_dep_f90.py
+-rw-r--r--   0        0        0     4213 2023-05-11 11:19:52.672451 pikendus_backend-0.2.3/pikendus_backend/scripts/compile.py
+-rwxr-xr-x   0        0        0     1728 2023-05-11 11:19:52.672451 pikendus_backend-0.2.3/pikendus_backend/scripts/gene_py_src.py
+-rwxr-xr-x   0        0        0     2117 2023-05-11 11:19:52.672451 pikendus_backend-0.2.3/pikendus_backend/scripts/ligne_debug.py
+-rw-r--r--   0        0        0    13199 2023-05-11 11:19:52.672451 pikendus_backend-0.2.3/pikendus_backend/structure.py
+-rw-r--r--   0        0        0     2780 2023-05-11 11:20:21.922962 pikendus_backend-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 pikendus_backend-0.2.3/PKG-INFO
```

### Comparing `pikendus_backend-0.2.2/LICENSE` & `pikendus_backend-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.2/pikendus_backend/PikendusWheelBuilder.py` & `pikendus_backend-0.2.3/pikendus_backend/PikendusWheelBuilder.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.2/pikendus_backend/__init__.py` & `pikendus_backend-0.2.3/pikendus_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.2/pikendus_backend/main.py` & `pikendus_backend-0.2.3/pikendus_backend/main.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.2/pikendus_backend/scripts/calc_dep_f90.py` & `pikendus_backend-0.2.3/pikendus_backend/scripts/calc_dep_f90.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.2/pikendus_backend/scripts/compile.py` & `pikendus_backend-0.2.3/pikendus_backend/scripts/compile.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.2/pikendus_backend/scripts/gene_py_src.py` & `pikendus_backend-0.2.3/pikendus_backend/scripts/gene_py_src.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.2/pikendus_backend/scripts/ligne_debug.py` & `pikendus_backend-0.2.3/pikendus_backend/scripts/ligne_debug.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.2/pikendus_backend/structure.py` & `pikendus_backend-0.2.3/pikendus_backend/structure.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.2/pyproject.toml` & `pikendus_backend-0.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,24 @@
     "rich>=13.3",
     "setuptools-scm>=7.1",
     "pdm-backend>=2.0.6",
     "wheel>=0.40.0",
     "numpy>=1.24.3",
     "toml>=0.10.2",
     "networkx>=3.1",
+    "PyYAML>=6.0",
 ]
 requires-python = ">3.8"
-version = "0.2.2"
+version = "0.2.3"
 
 [project.urls]
 "Bug Tracker" = "https://gitlab.com/ydethe/pikendus-backend/issues"
 Homepage = "https://gitlab.com/ydethe/pikendus-backend"
 Source = "https://gitlab.com/ydethe/pikendus-backend"
+Documentation = "https://ydethe.gitlab.io/-/pikendus-backend/-/jobs/4267041254/artifacts/htmldoc/index.html"
 
 [tool.pylint.main]
 ignore-patterns = [
     "kt_*.py",
 ]
 
 [tool.pylint.format]
```

### Comparing `pikendus_backend-0.2.2/PKG-INFO` & `pikendus_backend-0.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: pikendus-backend
-Version: 0.2.2
+Version: 0.2.3
 Summary: A PEP517 compliant build backend, able to compile C and fortran source files
 Author-Email: Yann de Thé <yann@johncloud.fr>
 Project-URL: Bug tracker, https://gitlab.com/ydethe/pikendus-backend/issues
 Project-URL: Homepage, https://gitlab.com/ydethe/pikendus-backend
 Project-URL: Source, https://gitlab.com/ydethe/pikendus-backend
+Project-URL: Documentation, https://ydethe.gitlab.io/-/pikendus-backend/-/jobs/4267041254/artifacts/htmldoc/index.html
 Requires-Python: >3.8
 Requires-Dist: rich>=13.3
 Requires-Dist: setuptools-scm>=7.1
 Requires-Dist: pdm-backend>=2.0.6
 Requires-Dist: wheel>=0.40.0
 Requires-Dist: numpy>=1.24.3
 Requires-Dist: toml>=0.10.2
 Requires-Dist: networkx>=3.1
+Requires-Dist: PyYAML>=6.0
```

