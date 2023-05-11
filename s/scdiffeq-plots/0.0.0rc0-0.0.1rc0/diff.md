# Comparing `tmp/scdiffeq_plots-0.0.0rc0.tar.gz` & `tmp/scdiffeq_plots-0.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdiffeq_plots-0.0.0rc0.tar", last modified: Sat May  6 21:13:37 2023, max compression
+gzip compressed data, was "scdiffeq_plots-0.0.1rc0.tar", last modified: Thu May 11 20:21:37 2023, max compression
```

## Comparing `scdiffeq_plots-0.0.0rc0.tar` & `scdiffeq_plots-0.0.1rc0.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:13:37.394811 scdiffeq_plots-0.0.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-06 21:13:18.000000 scdiffeq_plots-0.0.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-06 21:13:37.394811 scdiffeq_plots-0.0.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-06 21:13:18.000000 scdiffeq_plots-0.0.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:13:37.390811 scdiffeq_plots-0.0.0rc0/scdiffeq_plots/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 21:13:18.000000 scdiffeq_plots-0.0.0rc0/scdiffeq_plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:13:37.394811 scdiffeq_plots-0.0.0rc0/scdiffeq_plots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-06 21:13:37.000000 scdiffeq_plots-0.0.0rc0/scdiffeq_plots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-06 21:13:37.000000 scdiffeq_plots-0.0.0rc0/scdiffeq_plots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 21:13:37.000000 scdiffeq_plots-0.0.0rc0/scdiffeq_plots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 21:13:37.000000 scdiffeq_plots-0.0.0rc0/scdiffeq_plots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 21:13:37.000000 scdiffeq_plots-0.0.0rc0/scdiffeq_plots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 21:13:37.394811 scdiffeq_plots-0.0.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-06 21:13:18.000000 scdiffeq_plots-0.0.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:21:37.795623 scdiffeq_plots-0.0.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-11 20:21:37.795623 scdiffeq_plots-0.0.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:21:37.791622 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/_loss_viz_ax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:21:37.795623 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/_plot_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/_style_spines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:21:37.795623 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/utils/_abc_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:21:37.795623 scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-11 20:21:37.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 20:21:37.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:21:37.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 20:21:37.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 20:21:37.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:21:37.795623 scdiffeq_plots-0.0.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/setup.py
```

### Comparing `scdiffeq_plots-0.0.0rc0/LICENSE` & `scdiffeq_plots-0.0.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `scdiffeq_plots-0.0.0rc0/PKG-INFO` & `scdiffeq_plots-0.0.1rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdiffeq_plots
-Version: 0.0.0rc0
+Version: 0.0.1rc0
 Summary: Plotting functions associated wtih analyses from scDiffEq
 Home-page: https://github.com/mvinyard/sc-neural-diffeqs
 Author: Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `scdiffeq_plots-0.0.0rc0/scdiffeq_plots.egg-info/PKG-INFO` & `scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdiffeq-plots
-Version: 0.0.0rc0
+Version: 0.0.1rc0
 Summary: Plotting functions associated wtih analyses from scDiffEq
 Home-page: https://github.com/mvinyard/sc-neural-diffeqs
 Author: Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `scdiffeq_plots-0.0.0rc0/setup.py` & `scdiffeq_plots-0.0.1rc0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import re
 import os
 import sys
 
 setuptools.setup(
     name="scdiffeq_plots",
-    version="0.0.0rc0",
+    version="0.0.1rc0",
     python_requires=">3.9.0",
     author="Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard",
     author_email="mvinyard@broadinstitute.org",
     url="https://github.com/mvinyard/sc-neural-diffeqs",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="Plotting functions associated wtih analyses from scDiffEq",
```

