# Comparing `tmp/pikendus_backend-0.2.0.tar.gz` & `tmp/pikendus_backend-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikendus_backend-0.2.0.tar", last modified: Thu May 11 09:44:26 2023, max compression
+gzip compressed data, was "pikendus_backend-0.2.2.tar", last modified: Thu May 11 11:11:03 2023, max compression
```

## Comparing `pikendus_backend-0.2.0.tar` & `pikendus_backend-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-05-08 19:50:05.311483 pikendus_backend-0.2.0/LICENSE
--rw-r--r--   0        0        0     3105 2023-05-11 09:41:52.877435 pikendus_backend-0.2.0/pikendus_backend/PikendusWheelBuilder.py
--rw-r--r--   0        0        0     1702 2023-05-11 09:41:52.877435 pikendus_backend-0.2.0/pikendus_backend/__init__.py
--rw-r--r--   0        0        0      823 2023-05-10 20:08:04.215486 pikendus_backend-0.2.0/pikendus_backend/main.py
--rwxr-xr-x   0        0        0     3459 2023-05-08 19:50:05.311483 pikendus_backend-0.2.0/pikendus_backend/scripts/calc_dep_f90.py
--rw-r--r--   0        0        0     4213 2023-05-10 19:50:28.916944 pikendus_backend-0.2.0/pikendus_backend/scripts/compile.py
--rwxr-xr-x   0        0        0     1728 2023-05-10 19:50:28.916944 pikendus_backend-0.2.0/pikendus_backend/scripts/gene_py_src.py
--rwxr-xr-x   0        0        0     2117 2023-05-08 19:50:05.311483 pikendus_backend-0.2.0/pikendus_backend/scripts/ligne_debug.py
--rw-r--r--   0        0        0    13199 2023-05-11 09:41:52.877435 pikendus_backend-0.2.0/pikendus_backend/structure.py
--rw-r--r--   0        0        0     2652 2023-05-11 09:44:26.904044 pikendus_backend-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 pikendus_backend-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 11:10:35.652582 pikendus_backend-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3105 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/PikendusWheelBuilder.py
+-rw-r--r--   0        0        0     1702 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/main.py
+-rwxr-xr-x   0        0        0     3459 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/scripts/calc_dep_f90.py
+-rw-r--r--   0        0        0     4213 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/scripts/compile.py
+-rwxr-xr-x   0        0        0     1728 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/scripts/gene_py_src.py
+-rwxr-xr-x   0        0        0     2117 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/scripts/ligne_debug.py
+-rw-r--r--   0        0        0    13199 2023-05-11 11:10:35.653582 pikendus_backend-0.2.2/pikendus_backend/structure.py
+-rw-r--r--   0        0        0     2652 2023-05-11 11:11:03.232354 pikendus_backend-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 pikendus_backend-0.2.2/PKG-INFO
```

### Comparing `pikendus_backend-0.2.0/LICENSE` & `pikendus_backend-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.0/pikendus_backend/PikendusWheelBuilder.py` & `pikendus_backend-0.2.2/pikendus_backend/PikendusWheelBuilder.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.0/pikendus_backend/__init__.py` & `pikendus_backend-0.2.2/pikendus_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.0/pikendus_backend/main.py` & `pikendus_backend-0.2.2/pikendus_backend/main.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.0/pikendus_backend/scripts/calc_dep_f90.py` & `pikendus_backend-0.2.2/pikendus_backend/scripts/calc_dep_f90.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.0/pikendus_backend/scripts/compile.py` & `pikendus_backend-0.2.2/pikendus_backend/scripts/compile.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.0/pikendus_backend/scripts/gene_py_src.py` & `pikendus_backend-0.2.2/pikendus_backend/scripts/gene_py_src.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.0/pikendus_backend/scripts/ligne_debug.py` & `pikendus_backend-0.2.2/pikendus_backend/scripts/ligne_debug.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.0/pikendus_backend/structure.py` & `pikendus_backend-0.2.2/pikendus_backend/structure.py`

 * *Files identical despite different names*

### Comparing `pikendus_backend-0.2.0/pyproject.toml` & `pikendus_backend-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "pdm-backend>=2.0.6",
     "wheel>=0.40.0",
     "numpy>=1.24.3",
     "toml>=0.10.2",
     "networkx>=3.1",
 ]
 requires-python = ">3.8"
-version = "0.2.0"
+version = "0.2.2"
 
 [project.urls]
 "Bug Tracker" = "https://gitlab.com/ydethe/pikendus-backend/issues"
 Homepage = "https://gitlab.com/ydethe/pikendus-backend"
 Source = "https://gitlab.com/ydethe/pikendus-backend"
 
 [tool.pylint.main]
```

### Comparing `pikendus_backend-0.2.0/PKG-INFO` & `pikendus_backend-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikendus-backend
-Version: 0.2.0
+Version: 0.2.2
 Summary: A PEP517 compliant build backend, able to compile C and fortran source files
 Author-Email: Yann de Thé <yann@johncloud.fr>
 Project-URL: Bug tracker, https://gitlab.com/ydethe/pikendus-backend/issues
 Project-URL: Homepage, https://gitlab.com/ydethe/pikendus-backend
 Project-URL: Source, https://gitlab.com/ydethe/pikendus-backend
 Requires-Python: >3.8
 Requires-Dist: rich>=13.3
```

