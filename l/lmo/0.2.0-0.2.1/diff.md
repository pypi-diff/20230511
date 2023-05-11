# Comparing `tmp/lmo-0.2.0.tar.gz` & `tmp/lmo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmo-0.2.0.tar", max compression
+gzip compressed data, was "lmo-0.2.1.tar", max compression
```

## Comparing `lmo-0.2.0.tar` & `lmo-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.2.0/LICENSE
--rw-r--r--   0        0        0      480 2023-05-04 08:52:01.271335 lmo-0.2.0/README.md
--rw-r--r--   0        0        0      199 2023-05-02 23:21:30.443482 lmo-0.2.0/lmo/__init__.py
--rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.2.0/lmo/_meta.py
--rw-r--r--   0        0        0      128 2023-04-30 12:42:37.998900 lmo-0.2.0/lmo/_typing.py
--rw-r--r--   0        0        0     7036 2023-05-04 02:29:29.090059 lmo-0.2.0/lmo/multivariate.py
--rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.2.0/lmo/py.typed
--rw-r--r--   0        0        0      987 2023-05-04 01:04:36.508186 lmo-0.2.0/lmo/stats.py
--rw-r--r--   0        0        0     5757 2023-05-04 08:31:49.091411 lmo-0.2.0/lmo/univariate.py
--rw-r--r--   0        0        0     1482 2023-05-03 23:50:48.397361 lmo-0.2.0/lmo/weights.py
--rw-r--r--   0        0        0     1916 2023-05-04 09:17:58.820370 lmo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 lmo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.2.1/LICENSE
+-rw-r--r--   0        0        0      754 2023-05-11 19:25:30.130399 lmo-0.2.1/README.md
+-rw-r--r--   0        0        0      199 2023-05-02 23:21:30.443482 lmo-0.2.1/lmo/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.2.1/lmo/_meta.py
+-rw-r--r--   0        0        0      128 2023-04-30 12:42:37.998900 lmo-0.2.1/lmo/_typing.py
+-rw-r--r--   0        0        0     7036 2023-05-04 02:29:29.090059 lmo-0.2.1/lmo/multivariate.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.2.1/lmo/py.typed
+-rw-r--r--   0        0        0      987 2023-05-04 01:04:36.508186 lmo-0.2.1/lmo/stats.py
+-rw-r--r--   0        0        0     5850 2023-05-11 18:57:22.207683 lmo-0.2.1/lmo/univariate.py
+-rw-r--r--   0        0        0     1482 2023-05-03 23:50:48.397361 lmo-0.2.1/lmo/weights.py
+-rw-r--r--   0        0        0     1916 2023-05-11 19:28:18.473947 lmo-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 lmo-0.2.1/PKG-INFO
```

### Comparing `lmo-0.2.0/LICENSE` & `lmo-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmo-0.2.0/lmo/multivariate.py` & `lmo-0.2.1/lmo/multivariate.py`

 * *Files identical despite different names*

### Comparing `lmo-0.2.0/lmo/stats.py` & `lmo-0.2.1/lmo/stats.py`

 * *Files identical despite different names*

### Comparing `lmo-0.2.0/lmo/univariate.py` & `lmo-0.2.1/lmo/univariate.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,22 +113,25 @@
     x = np.sort(a, axis=axis, kind=sort)
 
     l_r = tl_moment(x, r, s, t, axis=axis)
 
     if k == 0:
         return l_r
     if k == r:
-        return np.ones_like(l_r)
+        return np.ones_like(l_r)[()]
 
     l_k = l_r if k == r else tl_moment(x, k, s, t, axis=axis)
 
-    if not l_k:
-        # respect the bounds; use nan instead of inf
-        return np.nan * l_r if l_r else l_r
-    return l_r / l_k
+    # i.e. `x / 0 = 0 if x == 0 else np.nan`
+    return np.divide(
+        l_r,
+        l_k,
+        out=np.where(l_r == 0, 0.0, np.nan),
+        where=l_k != 0
+    )[()]  # [()] converts any 0-dimensional arrays to scalar
 
 
 def tl_loc(
     a: npt.ArrayLike,
     /,
     s: int = 1,
     t: int = 1,
```

### Comparing `lmo-0.2.0/lmo/weights.py` & `lmo-0.2.1/lmo/weights.py`

 * *Files identical despite different names*

### Comparing `lmo-0.2.0/pyproject.toml` & `lmo-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "oldest-supported-numpy"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "lmo"
-version = "0.2.0"
+version = "0.2.1"
 description = "L-Moments for robust statistics."
 authors = ["Joren Hammudoglu <jhammudoglu@gmail.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 homepage = "https://github.com/jorenham/lmo/"
 repository = "https://github.com/jorenham/lmo/"
 classifiers = [
```

### Comparing `lmo-0.2.0/PKG-INFO` & `lmo-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmo
-Version: 0.2.0
+Version: 0.2.1
 Summary: L-Moments for robust statistics.
 Home-page: https://github.com/jorenham/lmo/
 License: BSD-3-Clause
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
@@ -25,23 +25,31 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Dist: numpy (>=1.21)
 Project-URL: Bug Tracker, https://github.com/jorenham/lmo/issues
 Project-URL: Repository, https://github.com/jorenham/lmo/
 Description-Content-Type: text/markdown
 
+<img src="./docs/static/lmo.svg" alt="jorenham/lmo" width="128" align="right">
+
 # Lmo
 
 <!--badges-start-->
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jorenham/lmo/CI.yml?branch=master&style=flat-square)
 [![PyPI](https://img.shields.io/pypi/v/lmo?style=flat-square)](https://pypi.org/project/lmo/)
 [![versions](https://img.shields.io/pypi/pyversions/lmo?style=flat-square)](https://github.com/jorenham/lmo)
 [![license](https://img.shields.io/github/license/jorenham/lmo?style=flat-square)](https://github.com/jorenham/lmo/blob/master/LICENSE?)
 <!--badges-end-->
 
 
 Streamlined calculation of L-moments and TL-moments.
 
 ---
 
-*Docs and examples coming soon*.
+[Documentation](https://jorenham.github.io/lmo/)
+
+---
+
+*Examples coming soon*.
+
```

