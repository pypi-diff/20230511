# Comparing `tmp/autora-theorist-bms-1.0.0a0.tar.gz` & `tmp/autora-theorist-bms-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-bms-1.0.0a0.tar", last modified: Fri May  5 12:59:08 2023, max compression
+gzip compressed data, was "autora-theorist-bms-1.0.0b0.tar", last modified: Thu May 11 15:54:07 2023, max compression
```

## Comparing `autora-theorist-bms-1.0.0a0.tar` & `autora-theorist-bms-1.0.0b0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.375718 autora-theorist-bms-1.0.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.363718 autora-theorist-bms-1.0.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.367718 autora-theorist-bms-1.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-05 12:59:08.375718 autora-theorist-bms-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.367718 autora-theorist-bms-1.0.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/docs/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/docs/how_it_works.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.371718 autora-theorist-bms-1.0.0a0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   191653 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/docs/img/BMSEquationTreeOps.png
--rw-r--r--   0 runner    (1001) docker     (123)   503083 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/docs/img/BMSTempering.png
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/docs/introduction.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.371718 autora-theorist-bms-1.0.0a0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/docs/meta_parameters.md
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/docs/search_space.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1572980 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/docs/weber.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.371718 autora-theorist-bms-1.0.0a0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:59:08.375718 autora-theorist-bms-1.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.363718 autora-theorist-bms-1.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.363718 autora-theorist-bms-1.0.0a0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.363718 autora-theorist-bms-1.0.0a0/src/autora/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.371718 autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/fit_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)    60372 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/regressor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2860 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.371718 autora-theorist-bms-1.0.0a0/src/autora_theorist_bms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-05 12:59:08.000000 autora-theorist-bms-1.0.0a0/src/autora_theorist_bms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-05 12:59:08.000000 autora-theorist-bms-1.0.0a0/src/autora_theorist_bms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:59:08.000000 autora-theorist-bms-1.0.0a0/src/autora_theorist_bms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 12:59:08.000000 autora-theorist-bms-1.0.0a0/src/autora_theorist_bms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 12:59:08.000000 autora-theorist-bms-1.0.0a0/src/autora_theorist_bms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:08.375718 autora-theorist-bms-1.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-05-05 12:58:56.000000 autora-theorist-bms-1.0.0a0/tests/test_sklearn_bms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.404622 autora-theorist-bms-1.0.0b0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.396622 autora-theorist-bms-1.0.0b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.396622 autora-theorist-bms-1.0.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-11 15:54:07.404622 autora-theorist-bms-1.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.400622 autora-theorist-bms-1.0.0b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    34238 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/basic-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/how-it-works.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.400622 autora-theorist-bms-1.0.0b0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   191653 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/img/BMSEquationTreeOps.png
+-rw-r--r--   0 runner    (1001) docker     (123)   503083 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/img/BMSTempering.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.400622 autora-theorist-bms-1.0.0b0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/meta-parameters.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/search-space.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.400622 autora-theorist-bms-1.0.0b0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:54:07.404622 autora-theorist-bms-1.0.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.396622 autora-theorist-bms-1.0.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.396622 autora-theorist-bms-1.0.0b0/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.396622 autora-theorist-bms-1.0.0b0/src/autora/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.400622 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/fit_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60423 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/regressor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2860 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.404622 autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-11 15:54:07.000000 autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-11 15:54:07.000000 autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:54:07.000000 autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 15:54:07.000000 autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 15:54:07.000000 autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.404622 autora-theorist-bms-1.0.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/tests/test_sklearn_bms.py
```

### Comparing `autora-theorist-bms-1.0.0a0/.github/workflows/python-publish.yml` & `autora-theorist-bms-1.0.0b0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/.gitignore` & `autora-theorist-bms-1.0.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/.pre-commit-config.yaml` & `autora-theorist-bms-1.0.0b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/PKG-INFO` & `autora-theorist-bms-1.0.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: autora-theorist-bms
-Version: 1.0.0a0
+Version: 1.0.0b0
 Summary: Bayesian Machine Scientist theorist for AutoRA
-Author-email: Joshua Hewson <joshua_hewson@brown.edu>, Ben Andrew <benwallaceandrew@gmail.com>
+Author-email: Joshua Hewson <joshua_hewson@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-bms
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `autora-theorist-bms-1.0.0a0/README.md` & `autora-theorist-bms-1.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/docs/how_it_works.md` & `autora-theorist-bms-1.0.0b0/docs/how-it-works.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/docs/img/BMSEquationTreeOps.png` & `autora-theorist-bms-1.0.0b0/docs/img/BMSEquationTreeOps.png`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/docs/img/BMSTempering.png` & `autora-theorist-bms-1.0.0b0/docs/img/BMSTempering.png`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/docs/introduction.md` & `autora-theorist-bms-1.0.0b0/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/docs/meta_parameters.md` & `autora-theorist-bms-1.0.0b0/docs/meta-parameters.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/docs/search_space.ipynb` & `autora-theorist-bms-1.0.0b0/docs/search-space.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/mkdocs/base.yml` & `autora-theorist-bms-1.0.0b0/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/pyproject.toml` & `autora-theorist-bms-1.0.0b0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [project]
 name = "autora-theorist-bms"
 description = "Bayesian Machine Scientist theorist for AutoRA"
 authors = [
     { name = "Joshua Hewson", email = "joshua_hewson@brown.edu" },
-    { name = "Ben Andrew", email = "benwallaceandrew@gmail.com" }
 ]
 dynamic = ["version"]
 
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.8,<4"
```

### Comparing `autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/fit_prior.py` & `autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/fit_prior.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/mcmc.py` & `autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/mcmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 import pandas as pd
 import scipy
 from scipy.optimize import curve_fit
 from sympy import lambdify, latex, log, sympify
 
 from .prior import get_priors, relu
 
+import warnings
+warnings.filterwarnings("ignore")
+
 _logger = logging.getLogger(__name__)
 
 
 class Node:
     """
     Object that holds algebraic term. This could be a function, variable, or parameter.
```

### Comparing `autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/parallel.py` & `autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/parallel.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/prior.py` & `autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/prior.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/regressor.py` & `autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/regressor.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/src/autora/theorist/bms/utils.py` & `autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/src/autora_theorist_bms.egg-info/PKG-INFO` & `autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: autora-theorist-bms
-Version: 1.0.0a0
+Version: 1.0.0b0
 Summary: Bayesian Machine Scientist theorist for AutoRA
-Author-email: Joshua Hewson <joshua_hewson@brown.edu>, Ben Andrew <benwallaceandrew@gmail.com>
+Author-email: Joshua Hewson <joshua_hewson@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-bms
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `autora-theorist-bms-1.0.0a0/src/autora_theorist_bms.egg-info/SOURCES.txt` & `autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .gitignore
 .pre-commit-config.yaml
 README.md
 mkdocs.yml
 pyproject.toml
 .github/workflows/python-publish.yml
-docs/example.ipynb
-docs/how_it_works.md
-docs/introduction.md
-docs/meta_parameters.md
-docs/search_space.ipynb
-docs/weber.ipynb
+docs/basic-usage.ipynb
+docs/how-it-works.md
+docs/index.md
+docs/meta-parameters.md
+docs/quickstart.md
+docs/search-space.ipynb
 docs/img/BMSEquationTreeOps.png
 docs/img/BMSTempering.png
 docs/javascripts/mathjax.js
 mkdocs/base.yml
 src/autora/theorist/bms/__init__.py
 src/autora/theorist/bms/fit_prior.py
 src/autora/theorist/bms/mcmc.py
```

### Comparing `autora-theorist-bms-1.0.0a0/tests/README.md` & `autora-theorist-bms-1.0.0b0/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0a0/tests/test_sklearn_bms.py` & `autora-theorist-bms-1.0.0b0/tests/test_sklearn_bms.py`

 * *Files identical despite different names*

