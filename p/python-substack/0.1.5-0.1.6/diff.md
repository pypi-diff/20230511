# Comparing `tmp/python_substack-0.1.5.tar.gz` & `tmp/python_substack-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_substack-0.1.5.tar", max compression
+gzip compressed data, was "python_substack-0.1.6.tar", max compression
```

## Comparing `python_substack-0.1.5.tar` & `python_substack-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-02-23 16:02:10.560425 python_substack-0.1.5/LICENSE
--rw-r--r--   0        0        0      305 2023-02-23 16:02:10.560425 python_substack-0.1.5/README.md
--rw-r--r--   0        0        0      621 2023-02-23 16:02:10.560425 python_substack-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      388 2023-02-23 16:02:10.560425 python_substack-0.1.5/substack/__init__.py
--rw-r--r--   0        0        0     6488 2023-02-23 16:02:10.560425 python_substack-0.1.5/substack/api.py
--rw-r--r--   0        0        0      841 2023-02-23 16:02:10.560425 python_substack-0.1.5/substack/exceptions.py
--rw-r--r--   0        0        0     3746 2023-02-23 16:02:10.560425 python_substack-0.1.5/substack/post.py
--rw-r--r--   0        0        0     1051 1970-01-01 00:00:00.000000 python_substack-0.1.5/setup.py
--rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 python_substack-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-11 14:13:36.455150 python_substack-0.1.6/LICENSE
+-rw-r--r--   0        0        0      724 2023-05-11 14:13:36.455150 python_substack-0.1.6/README.md
+-rw-r--r--   0        0        0      619 2023-05-11 14:13:36.455150 python_substack-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-05-11 14:13:36.455150 python_substack-0.1.6/substack/__init__.py
+-rw-r--r--   0        0        0     8274 2023-05-11 14:13:36.455150 python_substack-0.1.6/substack/api.py
+-rw-r--r--   0        0        0      841 2023-05-11 14:13:36.455150 python_substack-0.1.6/substack/exceptions.py
+-rw-r--r--   0        0        0     5669 2023-05-11 14:13:36.455150 python_substack-0.1.6/substack/post.py
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 python_substack-0.1.6/PKG-INFO
```

### Comparing `python_substack-0.1.5/LICENSE` & `python_substack-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_substack-0.1.5/pyproject.toml` & `python_substack-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "python-substack"
-version = "0.1.5"
+version = "0.1.6"
 description = "A Python wrapper around the Substack API."
 authors = ["Paolo Mazza <mazzapaolo2019@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "substack" }
 ]
 
 readme = "README.md"
 
-repository = "https://github.com/mazza8/python-substack"
-homepage = "https://github.com/mazza8/python-substack"
+repository = "https://github.com/ma2za/python-substack"
+homepage = "https://github.com/ma2za/python-substack"
 
 keywords = ["substack"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 requests = "^2.28.1"
```

### Comparing `python_substack-0.1.5/substack/exceptions.py` & `python_substack-0.1.6/substack/exceptions.py`

 * *Files identical despite different names*

