# Comparing `tmp/pandus-2.0.0.tar.gz` & `tmp/pandus-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandus-2.0.0.tar", max compression
+gzip compressed data, was "pandus-2.0.1.tar", max compression
```

## Comparing `pandus-2.0.0.tar` & `pandus-2.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-02-14 09:23:55.719510 pandus-2.0.0/LICENSE
--rw-r--r--   0        0        0      702 2023-02-14 18:37:38.648319 pandus-2.0.0/README.md
--rw-r--r--   0        0        0       80 2023-02-14 09:35:19.822392 pandus-2.0.0/pandus/__init__.py
--rw-r--r--   0        0        0      210 2023-02-14 17:46:26.960126 pandus-2.0.0/pandus/pandus.py
--rw-r--r--   0        0        0      767 2023-04-03 15:02:57.383226 pandus-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1638 1970-01-01 00:00:00.000000 pandus-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-02-14 09:23:55.719510 pandus-2.0.1/LICENSE
+-rw-r--r--   0        0        0      705 2023-04-03 15:05:57.050972 pandus-2.0.1/README.md
+-rw-r--r--   0        0        0       80 2023-02-14 09:35:19.822392 pandus-2.0.1/pandus/__init__.py
+-rw-r--r--   0        0        0      210 2023-02-14 17:46:26.960126 pandus-2.0.1/pandus/pandus.py
+-rw-r--r--   0        0        0      774 2023-04-24 10:45:10.624039 pandus-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1641 1970-01-01 00:00:00.000000 pandus-2.0.1/PKG-INFO
```

### Comparing `pandus-2.0.0/LICENSE` & `pandus-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandus-2.0.0/README.md` & `pandus-2.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pandus
 [![PyPI version](https://badge.fury.io/py/pandus.svg)](https://badge.fury.io/py/pandus)
 
 ## What is it?
-**pandus** is a fork of the popular data analysis library [pandas](https://pandas.pydata.org/), with the sole purpose of providing a different name. It provides a drop-in replacement for pandas, with all the same functionality and API, but with the name changed to "pandus".
+**pandus** is a wrapper around popular data analysis library [pandas](https://pandas.pydata.org/), with the sole purpose of providing a different name. It provides a drop-in replacement for pandas, with all the same functionality and API, but with the name changed to "pandus".
 
 Note that while pandas is a serious library for data analysis, pandus is not intended to be taken seriously and is purely for fun. Use at your own risk!
 
 
 ## Why?
 Because of an inside joke.
```

### Comparing `pandus-2.0.0/pyproject.toml` & `pandus-2.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandus"
-version = "2.0.0"
+version = "2.0.1"
 description = "A simple wrapper around Pandas"
 authors = ["Egor Georgiev"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/egor-georgiev/pandus"
 repository = "https://github.com/egor-georgiev/pandus"
 keywords = ["pandus", "pandas", "data-science", "data-analysis"]
@@ -15,14 +15,14 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-pandas = "2.0.0"
+pandas = "2.0.1"
 
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pandus-2.0.0/PKG-INFO` & `pandus-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandus
-Version: 2.0.0
+Version: 2.0.1
 Summary: A simple wrapper around Pandas
 Home-page: https://github.com/egor-georgiev/pandus
 License: MIT
 Keywords: pandus,pandas,data-science,data-analysis
 Author: Egor Georgiev
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -14,23 +14,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: pandas (==2.0.0)
+Requires-Dist: pandas (==2.0.1)
 Project-URL: Repository, https://github.com/egor-georgiev/pandus
 Description-Content-Type: text/markdown
 
 # pandus
 [![PyPI version](https://badge.fury.io/py/pandus.svg)](https://badge.fury.io/py/pandus)
 
 ## What is it?
-**pandus** is a fork of the popular data analysis library [pandas](https://pandas.pydata.org/), with the sole purpose of providing a different name. It provides a drop-in replacement for pandas, with all the same functionality and API, but with the name changed to "pandus".
+**pandus** is a wrapper around popular data analysis library [pandas](https://pandas.pydata.org/), with the sole purpose of providing a different name. It provides a drop-in replacement for pandas, with all the same functionality and API, but with the name changed to "pandus".
 
 Note that while pandas is a serious library for data analysis, pandus is not intended to be taken seriously and is purely for fun. Use at your own risk!
 
 
 ## Why?
 Because of an inside joke.
```

