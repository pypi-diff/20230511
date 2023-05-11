# Comparing `tmp/xarray-safe-s1-2023.5.4.tar.gz` & `tmp/xarray-safe-s1-2023.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray-safe-s1-2023.5.4.tar", last modified: Thu May  4 10:20:43 2023, max compression
+gzip compressed data, was "xarray-safe-s1-2023.5.5.tar", last modified: Fri May  5 07:19:07 2023, max compression
```

## Comparing `xarray-safe-s1-2023.5.4.tar` & `xarray-safe-s1-2023.5.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:20:43.396277 xarray-safe-s1-2023.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:20:43.392277 xarray-safe-s1-2023.5.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:20:43.392277 xarray-safe-s1-2023.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-04 10:20:43.396277 xarray-safe-s1-2023.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:20:43.392277 xarray-safe-s1-2023.5.4/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:20:43.392277 xarray-safe-s1-2023.5.4/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:20:43.392277 xarray-safe-s1-2023.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:20:43.392277 xarray-safe-s1-2023.5.4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:20:43.392277 xarray-safe-s1-2023.5.4/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/docs/_static/css/xsar.css
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:20:43.392277 xarray-safe-s1-2023.5.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/docs/examples/simple_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:20:43.396277 xarray-safe-s1-2023.5.4/safe_s1/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/safe_s1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/safe_s1/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    27623 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/safe_s1/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    41424 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/safe_s1/sentinel1_xml_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/safe_s1/xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 10:20:43.396277 xarray-safe-s1-2023.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:20:43.396277 xarray-safe-s1-2023.5.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-04 10:20:21.000000 xarray-safe-s1-2023.5.4/test/test_s1reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:20:43.396277 xarray-safe-s1-2023.5.4/xarray_safe_s1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-04 10:20:43.000000 xarray-safe-s1-2023.5.4/xarray_safe_s1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-04 10:20:43.000000 xarray-safe-s1-2023.5.4/xarray_safe_s1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:20:43.000000 xarray-safe-s1-2023.5.4/xarray_safe_s1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-04 10:20:43.000000 xarray-safe-s1-2023.5.4/xarray_safe_s1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 10:20:43.000000 xarray-safe-s1-2023.5.4/xarray_safe_s1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.604241 xarray-safe-s1-2023.5.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.604241 xarray-safe-s1-2023.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.604241 xarray-safe-s1-2023.5.5/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.604241 xarray-safe-s1-2023.5.5/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.604241 xarray-safe-s1-2023.5.5/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/_static/css/xsar.css
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/examples/simple_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/safe_s1/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/safe_s1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/safe_s1/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    27623 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/safe_s1/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41424 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/safe_s1/sentinel1_xml_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/safe_s1/xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/test/test_s1reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-05 07:19:07.000000 xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-05 07:19:07.000000 xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:19:07.000000 xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-05 07:19:07.000000 xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:19:07.000000 xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/top_level.txt
```

### Comparing `xarray-safe-s1-2023.5.4/.github/workflows/publish.yml` & `xarray-safe-s1-2023.5.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/.pre-commit-config.yaml` & `xarray-safe-s1-2023.5.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/LICENSE` & `xarray-safe-s1-2023.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/PKG-INFO` & `xarray-safe-s1-2023.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-safe-s1
-Version: 2023.5.4
+Version: 2023.5.5
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Install test](https://github.com/umr-lops/xsar/actions/workflows/install-test.yml/badge.svg)
 # xarray-safe-s1
```

### Comparing `xarray-safe-s1-2023.5.4/README.md` & `xarray-safe-s1-2023.5.5/README.md`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/ci/requirements/environment.yaml` & `xarray-safe-s1-2023.5.5/ci/requirements/environment.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/docs/Makefile` & `xarray-safe-s1-2023.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/docs/conf.py` & `xarray-safe-s1-2023.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/docs/examples/simple_tutorial.ipynb` & `xarray-safe-s1-2023.5.5/docs/examples/simple_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/docs/index.rst` & `xarray-safe-s1-2023.5.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/docs/installing.rst` & `xarray-safe-s1-2023.5.5/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/docs/make.bat` & `xarray-safe-s1-2023.5.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/pyproject.toml` & `xarray-safe-s1-2023.5.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "fsspec",
     "rasterio",
     "affine",
     "pandas",
     "shapely",
     "pyproj",
     "dask",
+    "aiohttp",
 ]
 readme = "README.md"
 dynamic = ["version"]
 
 [build-system]
 requires = ["setuptools>=64.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `xarray-safe-s1-2023.5.4/safe_s1/metadata.py` & `xarray-safe-s1-2023.5.5/safe_s1/metadata.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/safe_s1/sentinel1_xml_mappings.py` & `xarray-safe-s1-2023.5.5/safe_s1/sentinel1_xml_mappings.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/safe_s1/xml_parser.py` & `xarray-safe-s1-2023.5.5/safe_s1/xml_parser.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/test/test_s1reader.py` & `xarray-safe-s1-2023.5.5/test/test_s1reader.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.4/xarray_safe_s1.egg-info/PKG-INFO` & `xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-safe-s1
-Version: 2023.5.4
+Version: 2023.5.5
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Install test](https://github.com/umr-lops/xsar/actions/workflows/install-test.yml/badge.svg)
 # xarray-safe-s1
```

### Comparing `xarray-safe-s1-2023.5.4/xarray_safe_s1.egg-info/SOURCES.txt` & `xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

