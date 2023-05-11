# Comparing `tmp/tally-counter-0.0.1.tar.gz` & `tmp/tally-counter-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tally-counter-0.0.1.tar", last modified: Fri Apr 14 22:16:37 2023, max compression
+gzip compressed data, was "tally-counter-1.0.0a0.tar", last modified: Thu May 11 21:12:54 2023, max compression
```

## Comparing `tally-counter-0.0.1.tar` & `tally-counter-1.0.0a0.tar`

### file list

```diff
@@ -1,22 +1,38 @@
-drwxr-xr-x   0 scott.houseman   (502) staff       (20)        0 2023-04-14 22:16:37.821805 tally-counter-0.0.1/
--rw-r--r--   0 scott.houseman   (502) staff       (20)     1071 2023-04-04 14:36:45.000000 tally-counter-0.0.1/LICENSE
--rw-r--r--   0 scott.houseman   (502) staff       (20)     4036 2023-04-14 22:16:37.821913 tally-counter-0.0.1/PKG-INFO
--rw-r--r--   0 scott.houseman   (502) staff       (20)     3537 2023-04-14 21:58:46.000000 tally-counter-0.0.1/README.md
--rw-r--r--   0 scott.houseman   (502) staff       (20)     1427 2023-04-14 07:47:26.000000 tally-counter-0.0.1/pyproject.toml
--rw-r--r--   0 scott.houseman   (502) staff       (20)       69 2023-04-14 22:16:37.822293 tally-counter-0.0.1/setup.cfg
-drwxr-xr-x   0 scott.houseman   (502) staff       (20)        0 2023-04-14 22:16:37.812730 tally-counter-0.0.1/src/
-drwxr-xr-x   0 scott.houseman   (502) staff       (20)        0 2023-04-14 22:16:37.817984 tally-counter-0.0.1/src/tally_counter/
--rw-r--r--   0 scott.houseman   (502) staff       (20)       52 2023-04-04 15:51:06.000000 tally-counter-0.0.1/src/tally_counter/__init__.py
--rw-r--r--   0 scott.houseman   (502) staff       (20)     1340 2023-04-14 16:35:28.000000 tally-counter-0.0.1/src/tally_counter/counter.py
--rw-r--r--   0 scott.houseman   (502) staff       (20)      762 2023-04-14 16:32:21.000000 tally-counter-0.0.1/src/tally_counter/data_point.py
--rw-r--r--   0 scott.houseman   (502) staff       (20)     3577 2023-04-14 22:08:18.000000 tally-counter-0.0.1/src/tally_counter/data_series.py
-drwxr-xr-x   0 scott.houseman   (502) staff       (20)        0 2023-04-14 22:16:37.819836 tally-counter-0.0.1/src/tally_counter.egg-info/
--rw-r--r--   0 scott.houseman   (502) staff       (20)     4036 2023-04-14 22:16:37.000000 tally-counter-0.0.1/src/tally_counter.egg-info/PKG-INFO
--rw-r--r--   0 scott.houseman   (502) staff       (20)      443 2023-04-14 22:16:37.000000 tally-counter-0.0.1/src/tally_counter.egg-info/SOURCES.txt
--rw-r--r--   0 scott.houseman   (502) staff       (20)        1 2023-04-14 22:16:37.000000 tally-counter-0.0.1/src/tally_counter.egg-info/dependency_links.txt
--rw-r--r--   0 scott.houseman   (502) staff       (20)       87 2023-04-14 22:16:37.000000 tally-counter-0.0.1/src/tally_counter.egg-info/requires.txt
--rw-r--r--   0 scott.houseman   (502) staff       (20)       14 2023-04-14 22:16:37.000000 tally-counter-0.0.1/src/tally_counter.egg-info/top_level.txt
-drwxr-xr-x   0 scott.houseman   (502) staff       (20)        0 2023-04-14 22:16:37.821383 tally-counter-0.0.1/tests/
--rw-r--r--   0 scott.houseman   (502) staff       (20)     2356 2023-04-14 16:48:37.000000 tally-counter-0.0.1/tests/test_counter.py
--rw-r--r--   0 scott.houseman   (502) staff       (20)      318 2023-04-14 16:36:46.000000 tally-counter-0.0.1/tests/test_data_point.py
--rw-r--r--   0 scott.houseman   (502) staff       (20)     3951 2023-04-14 22:08:18.000000 tally-counter-0.0.1/tests/test_data_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:12:54.911880 tally-counter-1.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:12:54.899880 tally-counter-1.0.0a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:12:54.903880 tally-counter-1.0.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-11 21:12:54.911880 tally-counter-1.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:12:54.907880 tally-counter-1.0.0a0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/docs/DEV.md
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 21:12:54.911880 tally-counter-1.0.0a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:12:54.899880 tally-counter-1.0.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:12:54.907880 tally-counter-1.0.0a0/src/tally_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/src/tally_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-11 21:12:54.000000 tally-counter-1.0.0a0/src/tally_counter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/src/tally_counter/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/src/tally_counter/data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/src/tally_counter/data_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/src/tally_counter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:12:54.907880 tally-counter-1.0.0a0/src/tally_counter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-11 21:12:54.000000 tally-counter-1.0.0a0/src/tally_counter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-11 21:12:54.000000 tally-counter-1.0.0a0/src/tally_counter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:12:54.000000 tally-counter-1.0.0a0/src/tally_counter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 21:12:54.000000 tally-counter-1.0.0a0/src/tally_counter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 21:12:54.000000 tally-counter-1.0.0a0/src/tally_counter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:12:54.911880 tally-counter-1.0.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/tests/test_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/tests/test_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-11 21:12:39.000000 tally-counter-1.0.0a0/tests/test_data_series.py
```

### Comparing `tally-counter-0.0.1/LICENSE` & `tally-counter-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `tally-counter-0.0.1/PKG-INFO` & `tally-counter-1.0.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tally-counter
-Version: 0.0.1
+Version: 1.0.0a0
 Summary: A Python tally counter class
 Author-email: Scott Houseman <scott.houseman@gmail.com>
 Project-URL: repository, https://github.com/houseman/tally-counter
 Keywords: statistics,counter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tally-counter-0.0.1/README.md` & `tally-counter-1.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `tally-counter-0.0.1/pyproject.toml` & `tally-counter-1.0.0a0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [project]
 name = "tally-counter"
-version = "0.0.1"
+# version = "0.0.0" # setuptools_scm extracts the version number from the project’s git tags during the build process
+dynamic = ["version"]
 authors = [
   { name="Scott Houseman", email="scott.houseman@gmail.com" },
 ]
 description = "A Python tally counter class"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -29,35 +30,42 @@
   "mypy",
   "pyupgrade",
   "pre-commit",
 
   # Test dependencies
   "pytest",
   "pytest-cov[all]",
-  "pytest-mock"
+  "pytest-mock",
+
+  # PyPI
+  "twine"
 ]
 
 [project.urls]
 repository = "https://github.com/houseman/tally-counter"
 
 [build-system]
 requires = [
-  "setuptools"
+  "setuptools>=45",
+  "setuptools_scm[toml]>=6.2"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = [
   "src"
 ]
 include = [
   "tally_counter*"
 ]
 namespaces = false
 
+[tool.setuptools_scm]
+write_to = "src/tally_counter/_version.py"
+
 [tool.isort]
 profile = "black"
 src_paths = [
     "src",
     "test"
 ]
 honor_noqa = true
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tally-counter-0.0.1/src/tally_counter/counter.py` & `tally-counter-1.0.0a0/src/tally_counter/counter.py`

 * *Files identical despite different names*

### Comparing `tally-counter-0.0.1/src/tally_counter/data_point.py` & `tally-counter-1.0.0a0/src/tally_counter/data_point.py`

 * *Files identical despite different names*

### Comparing `tally-counter-0.0.1/src/tally_counter/data_series.py` & `tally-counter-1.0.0a0/src/tally_counter/data_series.py`

 * *Files identical despite different names*

### Comparing `tally-counter-0.0.1/src/tally_counter.egg-info/PKG-INFO` & `tally-counter-1.0.0a0/src/tally_counter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tally-counter
-Version: 0.0.1
+Version: 1.0.0a0
 Summary: A Python tally counter class
 Author-email: Scott Houseman <scott.houseman@gmail.com>
 Project-URL: repository, https://github.com/houseman/tally-counter
 Keywords: statistics,counter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tally-counter-0.0.1/tests/test_counter.py` & `tally-counter-1.0.0a0/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `tally-counter-0.0.1/tests/test_data_series.py` & `tally-counter-1.0.0a0/tests/test_data_series.py`

 * *Files identical despite different names*

