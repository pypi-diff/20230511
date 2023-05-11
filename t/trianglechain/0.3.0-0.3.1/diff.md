# Comparing `tmp/trianglechain-0.3.0.tar.gz` & `tmp/trianglechain-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trianglechain-0.3.0.tar", last modified: Wed Apr 26 13:37:04 2023, max compression
+gzip compressed data, was "trianglechain-0.3.1.tar", last modified: Thu May 11 08:30:40 2023, max compression
```

## Comparing `trianglechain-0.3.0.tar` & `trianglechain-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 13:37:04.356767 trianglechain-0.3.0/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-04-26 13:23:10.000000 trianglechain-0.3.0/AUTHORS.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-04-26 13:23:10.000000 trianglechain-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1017 2023-04-26 13:36:31.000000 trianglechain-0.3.0/HISTORY.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-04-26 13:23:10.000000 trianglechain-0.3.0/LICENSE
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-04-26 13:23:10.000000 trianglechain-0.3.0/MANIFEST.in
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-04-26 13:37:04.356829 trianglechain-0.3.0/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-04-26 13:23:10.000000 trianglechain-0.3.0/README.md
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-04-26 13:23:11.000000 trianglechain-0.3.0/pyproject.toml
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1385 2023-04-26 13:37:04.357221 trianglechain-0.3.0/setup.cfg
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 13:37:04.352516 trianglechain-0.3.0/src/
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 13:37:04.355096 trianglechain-0.3.0/src/trianglechain/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8714 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/BaseChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13478 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/LineChain.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    27750 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/TriangleChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-04-26 13:36:45.000000 trianglechain-0.3.0/src/trianglechain/__init__.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13417 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    10416 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/density_estimation.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7853 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16438 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/make_subplots.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4349 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/params.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/utils_pj_hpd.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    18937 2023-04-26 13:23:11.000000 trianglechain-0.3.0/src/trianglechain/utils_plots.py
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 13:37:04.356043 trianglechain-0.3.0/src/trianglechain.egg-info/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-04-26 13:37:04.000000 trianglechain-0.3.0/src/trianglechain.egg-info/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      809 2023-04-26 13:37:04.000000 trianglechain-0.3.0/src/trianglechain.egg-info/SOURCES.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-04-26 13:37:04.000000 trianglechain-0.3.0/src/trianglechain.egg-info/dependency_links.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-04-26 13:23:29.000000 trianglechain-0.3.0/src/trianglechain.egg-info/not-zip-safe
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      308 2023-04-26 13:37:04.000000 trianglechain-0.3.0/src/trianglechain.egg-info/requires.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-04-26 13:37:04.000000 trianglechain-0.3.0/src/trianglechain.egg-info/top_level.txt
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 13:37:04.356659 trianglechain-0.3.0/tests/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      674 2023-04-26 13:23:11.000000 trianglechain-0.3.0/tests/test_bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2013 2023-04-26 13:23:11.000000 trianglechain-0.3.0/tests/test_limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      748 2023-04-26 13:23:11.000000 trianglechain-0.3.0/tests/test_linechain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2897 2023-04-26 13:23:11.000000 trianglechain-0.3.0/tests/test_params.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     4006 2023-04-26 13:23:11.000000 trianglechain-0.3.0/tests/test_trianglechain.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-11 08:30:40.306219 trianglechain-0.3.1/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-05-04 11:29:54.000000 trianglechain-0.3.1/AUTHORS.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-05-04 11:29:54.000000 trianglechain-0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1302 2023-05-11 08:30:03.000000 trianglechain-0.3.1/HISTORY.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-05-04 11:29:54.000000 trianglechain-0.3.1/LICENSE
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-05-04 11:29:54.000000 trianglechain-0.3.1/MANIFEST.in
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-05-11 08:30:40.306289 trianglechain-0.3.1/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-05-04 11:29:54.000000 trianglechain-0.3.1/README.md
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-05-04 11:29:54.000000 trianglechain-0.3.1/pyproject.toml
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1385 2023-05-11 08:30:40.306632 trianglechain-0.3.1/setup.cfg
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-11 08:30:40.301468 trianglechain-0.3.1/src/
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-11 08:30:40.304486 trianglechain-0.3.1/src/trianglechain/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8714 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/BaseChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13478 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/LineChain.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    27750 2023-05-11 08:01:21.000000 trianglechain-0.3.1/src/trianglechain/TriangleChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-05-11 08:29:44.000000 trianglechain-0.3.1/src/trianglechain/__init__.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13417 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    10416 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/density_estimation.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7853 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16438 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/make_subplots.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4349 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/params.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/utils_pj_hpd.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    18937 2023-05-04 11:29:54.000000 trianglechain-0.3.1/src/trianglechain/utils_plots.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-11 08:30:40.305330 trianglechain-0.3.1/src/trianglechain.egg-info/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-05-11 08:30:40.000000 trianglechain-0.3.1/src/trianglechain.egg-info/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      809 2023-05-11 08:30:40.000000 trianglechain-0.3.1/src/trianglechain.egg-info/SOURCES.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-05-11 08:30:40.000000 trianglechain-0.3.1/src/trianglechain.egg-info/dependency_links.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-05-11 08:24:36.000000 trianglechain-0.3.1/src/trianglechain.egg-info/not-zip-safe
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      308 2023-05-11 08:30:40.000000 trianglechain-0.3.1/src/trianglechain.egg-info/requires.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-05-11 08:30:40.000000 trianglechain-0.3.1/src/trianglechain.egg-info/top_level.txt
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-05-11 08:30:40.306046 trianglechain-0.3.1/tests/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      674 2023-05-04 11:29:54.000000 trianglechain-0.3.1/tests/test_bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2013 2023-05-04 11:29:54.000000 trianglechain-0.3.1/tests/test_limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      748 2023-05-04 11:29:54.000000 trianglechain-0.3.1/tests/test_linechain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2897 2023-05-04 11:29:54.000000 trianglechain-0.3.1/tests/test_params.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     4006 2023-05-04 11:29:54.000000 trianglechain-0.3.1/tests/test_trianglechain.py
```

### Comparing `trianglechain-0.3.0/CONTRIBUTING.rst` & `trianglechain-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/HISTORY.rst` & `trianglechain-0.3.1/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 .. :changelog:
 
 History
 -------
+
+0.3.1 (2023-05-11)
+++++++++++++++++++
+
+* FIX: showing labels in most upper left corner when using only the upper triangle
+* improved documenation
+
 0.3.0 (2023-04-26)
 ++++++++++++++++++
 
 * FEATURE: LineChain class to handle line chains
 * FEATURE: params_from to select params from one specific input
 * FEATURE: add_derived_params to add derived params to the input array
 * FEATURE: new possible input type: pandas DataFrame
 * FEATURE: colors are varied automatically according the matplotlib color cycle
+* FEATURE: when computing bestfits and uncertainties, it automatically detects if to show bestfit +/- uncertainty or a lower/upper limit.
 * FIX: ylimits in 1D plots
 * FIX: tick values when choosing many ticks
 * improved documenation
 * dependency cleanup
 
-
 0.2.1 (2023-03-20)
 ++++++++++++++++++
 
 * FIX: bug in 1D histograms when using prob
 
 0.2.0 (2023-02-09)
 ++++++++++++++++++
```

### Comparing `trianglechain-0.3.0/LICENSE` & `trianglechain-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/PKG-INFO` & `trianglechain-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.3.0
+Version: 0.3.1
 Summary: Code to plot multidimensional distributions
 Author: Silvan Fischbacher, Tomasz Kacprzak
 Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `trianglechain-0.3.0/README.md` & `trianglechain-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/pyproject.toml` & `trianglechain-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/setup.cfg` & `trianglechain-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/src/trianglechain/BaseChain.py` & `trianglechain-0.3.1/src/trianglechain/BaseChain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/src/trianglechain/LineChain.py` & `trianglechain-0.3.1/src/trianglechain/LineChain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/src/trianglechain/TriangleChain.py` & `trianglechain-0.3.1/src/trianglechain/TriangleChain.py`

 * *Files 0% similar despite different names*

```diff
@@ -661,15 +661,15 @@
         local_tri = "upper"
         # y tick labels
         for i in range(0, n_dim - 1):
             if columns[i] != "EMPTY":
                 axc = get_current_ax(ax, local_tri, i, n_dim - 1)
                 plot_tick_labels(axc, "y", i, tri, grid_kwargs)
         # x tick labels
-        for i in range(1, n_dim):
+        for i in range(0, n_dim):
             if columns[i] != "EMPTY":
                 axc = get_current_ax(ax, local_tri, 0, i)
                 plot_tick_labels(axc, "x", i, tri, grid_kwargs)
 
     ########
     # grid #
     ########
```

### Comparing `trianglechain-0.3.0/src/trianglechain/bestfit.py` & `trianglechain-0.3.1/src/trianglechain/bestfit.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/src/trianglechain/density_estimation.py` & `trianglechain-0.3.1/src/trianglechain/density_estimation.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/src/trianglechain/limits.py` & `trianglechain-0.3.1/src/trianglechain/limits.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/src/trianglechain/make_subplots.py` & `trianglechain-0.3.1/src/trianglechain/make_subplots.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/src/trianglechain/params.py` & `trianglechain-0.3.1/src/trianglechain/params.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/src/trianglechain/utils_pj_hpd.py` & `trianglechain-0.3.1/src/trianglechain/utils_pj_hpd.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/src/trianglechain/utils_plots.py` & `trianglechain-0.3.1/src/trianglechain/utils_plots.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/src/trianglechain.egg-info/PKG-INFO` & `trianglechain-0.3.1/src/trianglechain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.3.0
+Version: 0.3.1
 Summary: Code to plot multidimensional distributions
 Author: Silvan Fischbacher, Tomasz Kacprzak
 Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `trianglechain-0.3.0/src/trianglechain.egg-info/SOURCES.txt` & `trianglechain-0.3.1/src/trianglechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/tests/test_bestfit.py` & `trianglechain-0.3.1/tests/test_bestfit.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/tests/test_limits.py` & `trianglechain-0.3.1/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/tests/test_linechain.py` & `trianglechain-0.3.1/tests/test_linechain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/tests/test_params.py` & `trianglechain-0.3.1/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.3.0/tests/test_trianglechain.py` & `trianglechain-0.3.1/tests/test_trianglechain.py`

 * *Files identical despite different names*

