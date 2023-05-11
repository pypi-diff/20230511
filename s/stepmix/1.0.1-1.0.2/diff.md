# Comparing `tmp/stepmix-1.0.1.tar.gz` & `tmp/stepmix-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepmix-1.0.1.tar", last modified: Sun Apr 30 21:21:57 2023, max compression
+gzip compressed data, was "stepmix-1.0.2.tar", last modified: Thu May 11 14:01:51 2023, max compression
```

## Comparing `stepmix-1.0.1.tar` & `stepmix-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      954 2023-01-11 22:01:14.079040 stepmix-1.0.1/.github/workflows/pytest.yaml
--rw-r--r--   0        0        0       54 2023-01-11 22:01:14.079040 stepmix-1.0.1/.gitignore
--rw-r--r--   0        0        0      309 2023-01-11 22:01:14.079040 stepmix-1.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1068 2023-01-11 22:01:14.079040 stepmix-1.0.1/LICENSE
--rw-r--r--   0        0        0     2428 2023-04-25 21:29:34.007800 stepmix-1.0.1/README-dev.md
--rw-r--r--   0        0        0     5261 2023-04-30 21:21:22.007846 stepmix-1.0.1/README.md
--rw-r--r--   0        0        0      638 2023-01-11 22:01:14.079040 stepmix-1.0.1/docs/Makefile
--rw-r--r--   0        0        0      764 2023-01-11 22:01:14.079040 stepmix-1.0.1/docs/make.bat
--rw-r--r--   0        0        0      929 2023-01-11 22:01:14.079040 stepmix-1.0.1/docs/source/api.rst
--rw-r--r--   0        0        0     1016 2023-04-30 21:21:22.007846 stepmix-1.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      955 2023-01-11 22:01:14.083040 stepmix-1.0.1/docs/source/index.rst
--rw-r--r--   0        0        0      283 2023-04-25 21:29:34.007800 stepmix-1.0.1/docs/source/installation.rst
--rw-r--r--   0        0        0     2814 2023-01-11 22:01:14.083040 stepmix-1.0.1/docs/source/tutorials.rst
--rw-r--r--   0        0        0     1872 2023-04-30 21:21:22.007846 stepmix-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      579 2023-04-25 21:29:34.007800 stepmix-1.0.1/scripts/README.md
--rwxr-xr-x   0        0        0     5603 2023-03-09 18:24:49.769774 stepmix-1.0.1/scripts/run_bakk_simulation.py
--rwxr-xr-x   0        0        0     4996 2023-03-09 22:19:26.676204 stepmix-1.0.1/scripts/run_bakk_simulation_complete.py
--rw-r--r--   0        0        0      174 2023-04-30 21:21:22.007846 stepmix-1.0.1/stepmix/__init__.py
--rw-r--r--   0        0        0     8113 2023-01-11 22:01:14.083040 stepmix-1.0.1/stepmix/bootstrap.py
--rw-r--r--   0        0        0     2033 2023-01-11 22:01:14.083040 stepmix-1.0.1/stepmix/corrections.py
--rw-r--r--   0        0        0    11630 2023-03-09 22:19:26.676204 stepmix-1.0.1/stepmix/datasets.py
--rw-r--r--   0        0        0        0 2023-01-11 22:01:14.083040 stepmix-1.0.1/stepmix/emission/__init__.py
--rw-r--r--   0        0        0     1660 2023-01-11 22:01:14.083040 stepmix-1.0.1/stepmix/emission/build_emission.py
--rw-r--r--   0        0        0     6283 2023-03-09 22:19:26.676204 stepmix-1.0.1/stepmix/emission/categorical.py
--rw-r--r--   0        0        0     4831 2023-03-09 21:04:30.147441 stepmix-1.0.1/stepmix/emission/covariate.py
--rw-r--r--   0        0        0     6031 2023-01-11 22:01:14.083040 stepmix-1.0.1/stepmix/emission/emission.py
--rw-r--r--   0        0        0    15489 2023-01-12 20:57:50.331048 stepmix-1.0.1/stepmix/emission/gaussian.py
--rw-r--r--   0        0        0     4681 2023-03-09 22:19:26.676204 stepmix-1.0.1/stepmix/emission/nested.py
--rw-r--r--   0        0        0    52639 2023-03-09 18:24:49.769774 stepmix-1.0.1/stepmix/stepmix.py
--rw-r--r--   0        0        0    18189 2023-04-30 21:21:22.007846 stepmix-1.0.1/stepmix/utils.py
--rw-r--r--   0        0        0     4074 2023-03-09 22:19:26.676204 stepmix-1.0.1/test/conftest.py
--rw-r--r--   0        0        0     3608 2023-03-09 22:19:26.676204 stepmix-1.0.1/test/test_benchmarks.py
--rw-r--r--   0        0        0     4499 2023-01-11 22:01:14.083040 stepmix-1.0.1/test/test_bootstrap.py
--rw-r--r--   0        0        0     8818 2023-04-30 21:21:22.007846 stepmix-1.0.1/test/test_emission.py
--rw-r--r--   0        0        0     1479 2023-01-11 22:01:14.083040 stepmix-1.0.1/test/test_fiml.py
--rw-r--r--   0        0        0     1781 2023-04-30 21:21:22.007846 stepmix-1.0.1/test/test_inputs.py
--rw-r--r--   0        0        0     4284 2023-03-09 18:24:49.769774 stepmix-1.0.1/test/test_random_state.py
--rw-r--r--   0        0        0      795 2023-01-11 22:01:14.083040 stepmix-1.0.1/test/test_sklearn.py
--rw-r--r--   0        0        0     4570 2023-01-11 22:01:14.083040 stepmix-1.0.1/test/test_steps.py
--rw-r--r--   0        0        0     6525 1970-01-01 00:00:00.000000 stepmix-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      954 2023-01-11 22:01:14.079040 stepmix-1.0.2/.github/workflows/pytest.yaml
+-rw-r--r--   0        0        0       54 2023-01-11 22:01:14.079040 stepmix-1.0.2/.gitignore
+-rw-r--r--   0        0        0      309 2023-01-11 22:01:14.079040 stepmix-1.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1068 2023-01-11 22:01:14.079040 stepmix-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2428 2023-04-25 21:29:34.007800 stepmix-1.0.2/README-dev.md
+-rw-r--r--   0        0        0     5261 2023-04-30 21:21:22.007846 stepmix-1.0.2/README.md
+-rw-r--r--   0        0        0      638 2023-01-11 22:01:14.079040 stepmix-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0      764 2023-01-11 22:01:14.079040 stepmix-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0      929 2023-01-11 22:01:14.079040 stepmix-1.0.2/docs/source/api.rst
+-rw-r--r--   0        0        0     1016 2023-05-11 13:57:34.709443 stepmix-1.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0      955 2023-01-11 22:01:14.083040 stepmix-1.0.2/docs/source/index.rst
+-rw-r--r--   0        0        0      283 2023-04-25 21:29:34.007800 stepmix-1.0.2/docs/source/installation.rst
+-rw-r--r--   0        0        0     2814 2023-01-11 22:01:14.083040 stepmix-1.0.2/docs/source/tutorials.rst
+-rw-r--r--   0        0        0     1872 2023-05-11 13:57:34.709443 stepmix-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      579 2023-04-25 21:29:34.007800 stepmix-1.0.2/scripts/README.md
+-rwxr-xr-x   0        0        0     5603 2023-03-09 18:24:49.769774 stepmix-1.0.2/scripts/run_bakk_simulation.py
+-rwxr-xr-x   0        0        0     4996 2023-03-09 22:19:26.676204 stepmix-1.0.2/scripts/run_bakk_simulation_complete.py
+-rw-r--r--   0        0        0      174 2023-05-11 13:57:34.709443 stepmix-1.0.2/stepmix/__init__.py
+-rw-r--r--   0        0        0     8359 2023-05-11 13:57:34.709443 stepmix-1.0.2/stepmix/bootstrap.py
+-rw-r--r--   0        0        0     2033 2023-01-11 22:01:14.083040 stepmix-1.0.2/stepmix/corrections.py
+-rw-r--r--   0        0        0    11630 2023-03-09 22:19:26.676204 stepmix-1.0.2/stepmix/datasets.py
+-rw-r--r--   0        0        0        0 2023-01-11 22:01:14.083040 stepmix-1.0.2/stepmix/emission/__init__.py
+-rw-r--r--   0        0        0     1660 2023-01-11 22:01:14.083040 stepmix-1.0.2/stepmix/emission/build_emission.py
+-rw-r--r--   0        0        0     6283 2023-03-09 22:19:26.676204 stepmix-1.0.2/stepmix/emission/categorical.py
+-rw-r--r--   0        0        0     4831 2023-03-09 21:04:30.147441 stepmix-1.0.2/stepmix/emission/covariate.py
+-rw-r--r--   0        0        0     6031 2023-01-11 22:01:14.083040 stepmix-1.0.2/stepmix/emission/emission.py
+-rw-r--r--   0        0        0    15489 2023-01-12 20:57:50.331048 stepmix-1.0.2/stepmix/emission/gaussian.py
+-rw-r--r--   0        0        0     4681 2023-03-09 22:19:26.676204 stepmix-1.0.2/stepmix/emission/nested.py
+-rw-r--r--   0        0        0    52639 2023-03-09 18:24:49.769774 stepmix-1.0.2/stepmix/stepmix.py
+-rw-r--r--   0        0        0    18189 2023-04-30 21:21:22.007846 stepmix-1.0.2/stepmix/utils.py
+-rw-r--r--   0        0        0     4074 2023-03-09 22:19:26.676204 stepmix-1.0.2/test/conftest.py
+-rw-r--r--   0        0        0     3608 2023-03-09 22:19:26.676204 stepmix-1.0.2/test/test_benchmarks.py
+-rw-r--r--   0        0        0     4788 2023-05-11 13:57:34.709443 stepmix-1.0.2/test/test_bootstrap.py
+-rw-r--r--   0        0        0     8818 2023-04-30 21:21:22.007846 stepmix-1.0.2/test/test_emission.py
+-rw-r--r--   0        0        0     1479 2023-01-11 22:01:14.083040 stepmix-1.0.2/test/test_fiml.py
+-rw-r--r--   0        0        0     1781 2023-04-30 21:21:22.007846 stepmix-1.0.2/test/test_inputs.py
+-rw-r--r--   0        0        0     4284 2023-03-09 18:24:49.769774 stepmix-1.0.2/test/test_random_state.py
+-rw-r--r--   0        0        0      795 2023-01-11 22:01:14.083040 stepmix-1.0.2/test/test_sklearn.py
+-rw-r--r--   0        0        0     4570 2023-01-11 22:01:14.083040 stepmix-1.0.2/test/test_steps.py
+-rw-r--r--   0        0        0     6525 1970-01-01 00:00:00.000000 stepmix-1.0.2/PKG-INFO
```

### Comparing `stepmix-1.0.1/.github/workflows/pytest.yaml` & `stepmix-1.0.2/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/LICENSE` & `stepmix-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/README-dev.md` & `stepmix-1.0.2/README-dev.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/README.md` & `stepmix-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/docs/Makefile` & `stepmix-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/docs/make.bat` & `stepmix-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/docs/source/api.rst` & `stepmix-1.0.2/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/docs/source/conf.py` & `stepmix-1.0.2/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 sys.path.insert(0, os.path.abspath("../.."))
 
 project = "StepMix"
 copyright = "2022, Labo-Lacourse"
 author = "Sacha Morin, Robin Legault"
 
 release = "0.0"
-version = "1.0.1"
+version = "1.0.2"
 
 
 # -- General configuration
 
 extensions = [
     "sphinx.ext.napoleon",
     # 'numpydoc',
```

### Comparing `stepmix-1.0.1/docs/source/index.rst` & `stepmix-1.0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/docs/source/tutorials.rst` & `stepmix-1.0.2/docs/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/pyproject.toml` & `stepmix-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "flit", "pytest", "sphinx", "sphinx-rtd-theme"]
 
 [project.urls]
 Homepage = "https://stepmix.readthedocs.io/en/latest/"
 
 [tool.bumpver]
-current_version = "1.0.1"
+current_version = "1.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `stepmix-1.0.1/scripts/README.md` & `stepmix-1.0.2/scripts/README.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/scripts/run_bakk_simulation.py` & `stepmix-1.0.2/scripts/run_bakk_simulation.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/scripts/run_bakk_simulation_complete.py` & `stepmix-1.0.2/scripts/run_bakk_simulation_complete.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/stepmix/bootstrap.py` & `stepmix-1.0.2/stepmix/bootstrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,14 +92,19 @@
         Fitted instance of the estimator.
     parameters: ndarray
         StepMix parameter dictionary. Follows the same convention as the parameters of the StepMix
         object. An additional axis of size (n_repetitions,) is added at position 0 of each parameter array.
     """
     n_samples = X.shape[0]
 
+    # Use the estimator built-in method to check the input
+    # This will ensure that X and Y are numpy arrays for the rest of the bootstrap procedure
+    estimator._check_initial_parameters(X)
+    X, Y = estimator._check_x_y(X, Y, reset=True)
+
     # First fit the base estimator and get class probabilities
     estimator.fit(X, Y)
     ref_class_probabilities = estimator.predict_proba(X, Y)
 
     # Not fit n_repetitions estimator with resampling and save parameters
     rng = check_random_state(estimator.random_state)
     parameters = list()
```

### Comparing `stepmix-1.0.1/stepmix/corrections.py` & `stepmix-1.0.2/stepmix/corrections.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/stepmix/datasets.py` & `stepmix-1.0.2/stepmix/datasets.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/stepmix/emission/build_emission.py` & `stepmix-1.0.2/stepmix/emission/build_emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/stepmix/emission/categorical.py` & `stepmix-1.0.2/stepmix/emission/categorical.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/stepmix/emission/covariate.py` & `stepmix-1.0.2/stepmix/emission/covariate.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/stepmix/emission/emission.py` & `stepmix-1.0.2/stepmix/emission/emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/stepmix/emission/gaussian.py` & `stepmix-1.0.2/stepmix/emission/gaussian.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/stepmix/emission/nested.py` & `stepmix-1.0.2/stepmix/emission/nested.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/stepmix/stepmix.py` & `stepmix-1.0.2/stepmix/stepmix.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/stepmix/utils.py` & `stepmix-1.0.2/stepmix/utils.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/test/conftest.py` & `stepmix-1.0.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/test/test_benchmarks.py` & `stepmix-1.0.2/test/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/test/test_bootstrap.py` & `stepmix-1.0.2/test/test_bootstrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import pandas as pd
 import pytest
 import matplotlib.pyplot as plt
 
 from stepmix import StepMix
 from stepmix.emission.build_emission import EMISSION_DICT
 from stepmix.bootstrap import find_best_permutation, bootstrap, plot_all_parameters_CI
 
@@ -114,7 +115,14 @@
     model, params = bootstrap(model_1, data_nested, data_nested, n_repetitions=3)
     assert isinstance(params["measurement"]["model_1"]["pis"][0], np.ndarray)
 
     # Also test plots
     figures = plot_all_parameters_CI(model.get_parameters(), params)
     for f in figures:
         plt.close(f)
+
+
+def test_bootstrap_df(data_nested, kwargs_nested):
+    """Call bootstrap procedure on a DataFrame."""
+    data_nested = pd.DataFrame(data_nested)
+    model_1 = StepMix(**kwargs_nested)
+    model, params = bootstrap(model_1, data_nested, data_nested, n_repetitions=3)
```

### Comparing `stepmix-1.0.1/test/test_emission.py` & `stepmix-1.0.2/test/test_emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/test/test_fiml.py` & `stepmix-1.0.2/test/test_fiml.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/test/test_inputs.py` & `stepmix-1.0.2/test/test_inputs.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/test/test_random_state.py` & `stepmix-1.0.2/test/test_random_state.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/test/test_sklearn.py` & `stepmix-1.0.2/test/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/test/test_steps.py` & `stepmix-1.0.2/test/test_steps.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.1/PKG-INFO` & `stepmix-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepmix
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for stepwise estimation of latent class models with measurement and structural components. The package can also be used to fit mixture models with various observed random variables.
 Keywords: clustering,mixtures,lca,em,latent-class-analysis,expectation–maximization
 Author-email: Sacha Morin <sacha.morin@mila.quebec>, Robin Legault <robin.legault@umontreal.ca>, Charles-Édouard Giguère <ce.giguere@gmail.com>, Éric Lacourse <eric.lacourse@umontreal.ca>, Roxane de la Sablonnière <roxane.de.la.sablonniere@umontreal.ca>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stepmix Version: 1.0.1 Summary: A Python package
+Metadata-Version: 2.1 Name: stepmix Version: 1.0.2 Summary: A Python package
 for stepwise estimation of latent class models with measurement and structural
 components. The package can also be used to fit mixture models with various
 observed random variables. Keywords: clustering,mixtures,lca,em,latent-class-
 analysis,expectationâmaximization Author-email: Sacha Morin
 morin@mila.quebec>, Robin Legault
 legault@umontreal.ca>, Charles-Ãdouard GiguÃ¨re
 giguere@gmail.com>, Ãric Lacourse
```

