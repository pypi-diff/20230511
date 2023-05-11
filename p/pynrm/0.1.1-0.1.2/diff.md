# Comparing `tmp/pynrm-0.1.1.tar.gz` & `tmp/pynrm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynrm-0.1.1.tar", last modified: Fri May  5 17:57:57 2023, max compression
+gzip compressed data, was "pynrm-0.1.2.tar", last modified: Thu May 11 06:51:05 2023, max compression
```

## Comparing `pynrm-0.1.1.tar` & `pynrm-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-05 17:57:57.214803 pynrm-0.1.1/
--rw-r--r--   0 katejeon   (501) staff       (20)      294 2023-05-05 17:28:09.000000 pynrm-0.1.1/.bumpversion.cfg
--rw-r--r--   0 katejeon   (501) staff       (20)      694 2023-05-02 19:16:19.000000 pynrm-0.1.1/.readthedocs.yaml
--rw-r--r--   0 katejeon   (501) staff       (20)     1488 2023-04-07 15:59:33.000000 pynrm-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 katejeon   (501) staff       (20)    11357 2023-04-07 15:59:33.000000 pynrm-0.1.1/LICENSE
--rw-r--r--   0 katejeon   (501) staff       (20)      540 2023-05-05 17:03:35.000000 pynrm-0.1.1/MANIFEST.in
--rw-r--r--   0 katejeon   (501) staff       (20)     2251 2023-04-07 15:59:33.000000 pynrm-0.1.1/Makefile
--rw-r--r--   0 katejeon   (501) staff       (20)    15730 2023-05-05 17:57:57.214312 pynrm-0.1.1/PKG-INFO
--rw-r--r--   0 katejeon   (501) staff       (20)     1938 2023-05-05 17:03:35.000000 pynrm-0.1.1/README.md
-drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-05 17:57:57.207034 pynrm-0.1.1/docs/
--rw-r--r--   0 katejeon   (501) staff       (20)      634 2023-04-06 22:27:41.000000 pynrm-0.1.1/docs/Makefile
--rw-r--r--   0 katejeon   (501) staff       (20)     2002 2023-04-08 20:20:03.000000 pynrm-0.1.1/docs/conf.py
--rw-r--r--   0 katejeon   (501) staff       (20)     1595 2023-04-08 20:20:03.000000 pynrm-0.1.1/docs/index.rst
--rw-r--r--   0 katejeon   (501) staff       (20)      760 2023-04-06 22:27:41.000000 pynrm-0.1.1/docs/make.bat
--rw-r--r--   0 katejeon   (501) staff       (20)      542 2023-04-08 20:20:03.000000 pynrm-0.1.1/docs/pynrm.rst
-drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-05 17:57:57.209322 pynrm-0.1.1/pynrm/
--rw-r--r--   0 katejeon   (501) staff       (20)     2930 2023-05-05 17:03:35.000000 pynrm-0.1.1/pynrm/Pedigree.py
--rw-r--r--   0 katejeon   (501) staff       (20)     7676 2023-05-05 17:03:35.000000 pynrm-0.1.1/pynrm/Simulator.py
--rw-r--r--   0 katejeon   (501) staff       (20)       22 2023-05-05 17:28:09.000000 pynrm-0.1.1/pynrm/__init__.py
--rw-r--r--   0 katejeon   (501) staff       (20)       36 2023-05-05 00:54:10.000000 pynrm-0.1.1/pynrm/__main__.py
--rw-r--r--   0 katejeon   (501) staff       (20)     2852 2023-05-05 17:03:35.000000 pynrm-0.1.1/pynrm/nrm.py
-drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-05 17:57:57.213545 pynrm-0.1.1/pynrm/tests/
--rw-r--r--   0 katejeon   (501) staff       (20)     1278 2023-05-05 17:03:35.000000 pynrm-0.1.1/pynrm/tests/test_nrm.py
--rw-r--r--   0 katejeon   (501) staff       (20)     1150 2023-05-05 17:03:35.000000 pynrm-0.1.1/pynrm/tests/test_pedigree.py
--rw-r--r--   0 katejeon   (501) staff       (20)     2433 2023-05-05 17:03:35.000000 pynrm-0.1.1/pynrm/tests/test_simulator.py
-drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-05 17:57:57.211333 pynrm-0.1.1/pynrm.egg-info/
--rw-r--r--   0 katejeon   (501) staff       (20)    15730 2023-05-05 17:57:57.000000 pynrm-0.1.1/pynrm.egg-info/PKG-INFO
--rw-r--r--   0 katejeon   (501) staff       (20)      497 2023-05-05 17:57:57.000000 pynrm-0.1.1/pynrm.egg-info/SOURCES.txt
--rw-r--r--   0 katejeon   (501) staff       (20)        1 2023-05-05 17:57:57.000000 pynrm-0.1.1/pynrm.egg-info/dependency_links.txt
--rw-r--r--   0 katejeon   (501) staff       (20)      169 2023-05-05 17:57:57.000000 pynrm-0.1.1/pynrm.egg-info/requires.txt
--rw-r--r--   0 katejeon   (501) staff       (20)        6 2023-05-05 17:57:57.000000 pynrm-0.1.1/pynrm.egg-info/top_level.txt
--rw-r--r--   0 katejeon   (501) staff       (20)     2169 2023-05-05 17:28:09.000000 pynrm-0.1.1/pyproject.toml
--rw-r--r--   0 katejeon   (501) staff       (20)       38 2023-05-05 17:57:57.214927 pynrm-0.1.1/setup.cfg
--rw-r--r--   0 katejeon   (501) staff       (20)      144 2023-04-06 22:24:45.000000 pynrm-0.1.1/setup.py
+drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-11 06:51:05.133685 pynrm-0.1.2/
+-rw-r--r--   0 katejeon   (501) staff       (20)      294 2023-05-11 06:40:10.000000 pynrm-0.1.2/.bumpversion.cfg
+-rw-r--r--   0 katejeon   (501) staff       (20)      694 2023-05-02 19:16:19.000000 pynrm-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 katejeon   (501) staff       (20)     1488 2023-04-07 15:59:33.000000 pynrm-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 katejeon   (501) staff       (20)    11357 2023-04-07 15:59:33.000000 pynrm-0.1.2/LICENSE
+-rw-r--r--   0 katejeon   (501) staff       (20)      561 2023-05-11 06:29:35.000000 pynrm-0.1.2/MANIFEST.in
+-rw-r--r--   0 katejeon   (501) staff       (20)     2251 2023-04-07 15:59:33.000000 pynrm-0.1.2/Makefile
+-rw-r--r--   0 katejeon   (501) staff       (20)    16111 2023-05-11 06:51:05.133036 pynrm-0.1.2/PKG-INFO
+-rw-r--r--   0 katejeon   (501) staff       (20)     2319 2023-05-11 06:29:35.000000 pynrm-0.1.2/README.md
+drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-11 06:51:05.125944 pynrm-0.1.2/docs/
+-rw-r--r--   0 katejeon   (501) staff       (20)      634 2023-04-06 22:27:41.000000 pynrm-0.1.2/docs/Makefile
+-rw-r--r--   0 katejeon   (501) staff       (20)     2002 2023-05-11 06:29:35.000000 pynrm-0.1.2/docs/conf.py
+-rw-r--r--   0 katejeon   (501) staff       (20)     2019 2023-05-11 06:29:35.000000 pynrm-0.1.2/docs/index.rst
+-rw-r--r--   0 katejeon   (501) staff       (20)      760 2023-04-06 22:27:41.000000 pynrm-0.1.2/docs/make.bat
+-rw-r--r--   0 katejeon   (501) staff       (20)      542 2023-04-08 20:20:03.000000 pynrm-0.1.2/docs/pynrm.rst
+drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-11 06:51:05.127970 pynrm-0.1.2/pynrm/
+-rw-r--r--   0 katejeon   (501) staff       (20)     2930 2023-05-11 04:34:26.000000 pynrm-0.1.2/pynrm/Pedigree.py
+-rw-r--r--   0 katejeon   (501) staff       (20)     9683 2023-05-11 06:00:07.000000 pynrm-0.1.2/pynrm/Simulator.py
+-rw-r--r--   0 katejeon   (501) staff       (20)       22 2023-05-11 06:40:10.000000 pynrm-0.1.2/pynrm/__init__.py
+-rw-r--r--   0 katejeon   (501) staff       (20)       36 2023-05-11 05:45:19.000000 pynrm-0.1.2/pynrm/__main__.py
+-rw-r--r--   0 katejeon   (501) staff       (20)     2852 2023-05-11 05:45:33.000000 pynrm-0.1.2/pynrm/nrm.py
+drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-11 06:51:05.132259 pynrm-0.1.2/pynrm/tests/
+-rw-r--r--   0 katejeon   (501) staff       (20)     1285 2023-05-11 06:00:07.000000 pynrm-0.1.2/pynrm/tests/test_nrm.py
+-rw-r--r--   0 katejeon   (501) staff       (20)     1166 2023-05-11 06:00:07.000000 pynrm-0.1.2/pynrm/tests/test_pedigree.py
+-rw-r--r--   0 katejeon   (501) staff       (20)     3348 2023-05-11 06:00:07.000000 pynrm-0.1.2/pynrm/tests/test_simulator.py
+drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-11 06:51:05.130496 pynrm-0.1.2/pynrm.egg-info/
+-rw-r--r--   0 katejeon   (501) staff       (20)    16111 2023-05-11 06:51:05.000000 pynrm-0.1.2/pynrm.egg-info/PKG-INFO
+-rw-r--r--   0 katejeon   (501) staff       (20)      497 2023-05-11 06:51:05.000000 pynrm-0.1.2/pynrm.egg-info/SOURCES.txt
+-rw-r--r--   0 katejeon   (501) staff       (20)        1 2023-05-11 06:51:05.000000 pynrm-0.1.2/pynrm.egg-info/dependency_links.txt
+-rw-r--r--   0 katejeon   (501) staff       (20)      180 2023-05-11 06:51:05.000000 pynrm-0.1.2/pynrm.egg-info/requires.txt
+-rw-r--r--   0 katejeon   (501) staff       (20)        6 2023-05-11 06:51:05.000000 pynrm-0.1.2/pynrm.egg-info/top_level.txt
+-rw-r--r--   0 katejeon   (501) staff       (20)     2183 2023-05-11 06:40:10.000000 pynrm-0.1.2/pyproject.toml
+-rw-r--r--   0 katejeon   (501) staff       (20)       38 2023-05-11 06:51:05.133839 pynrm-0.1.2/setup.cfg
+-rw-r--r--   0 katejeon   (501) staff       (20)      166 2023-05-11 06:47:42.000000 pynrm-0.1.2/setup.py
```

### Comparing `pynrm-0.1.1/.readthedocs.yaml` & `pynrm-0.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pynrm-0.1.1/CONTRIBUTING.md` & `pynrm-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pynrm-0.1.1/LICENSE` & `pynrm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynrm-0.1.1/MANIFEST.in` & `pynrm-0.1.2/MANIFEST.in`

 * *Files 12% similar despite different names*

```diff
@@ -20,10 +20,11 @@
 recursive-include docs *.py
 recursive-include docs Makefile
 
 # Patterns to exclude from any directory
 global-exclude *~
 global-exclude *.pyc
 global-exclude *.pyo
+global-exclude *.png
 global-exclude .git
 global-exclude .ipynb_checkpoints
 global-exclude .DS_Store
```

### Comparing `pynrm-0.1.1/Makefile` & `pynrm-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `pynrm-0.1.1/PKG-INFO` & `pynrm-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrm
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python library for animal breeding simulation
 Author-email: Kate Jeon <hj2589@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,46 +221,58 @@
 License-File: LICENSE
 
 # pynrm
 
 `pynrm` is a lightweight and extensible Python library for livestock breeding simulation.
 
 ![Build Status](https://github.com/katehyerinjeon/pynrm/actions/workflows/build.yml/badge.svg)
-![PyPI](https://img.shields.io/pypi/v/pynrm)
+[![PyPI](https://img.shields.io/pypi/v/pynrm)](https://pypi.org/project/pynrm/)
 [![codecov](https://codecov.io/gh/katehyerinjeon/pynrm/branch/main/graph/badge.svg)](https://codecov.io/gh/katehyerinjeon/pynrm)
 ![GitHub](https://img.shields.io/github/license/katehyerinjeon/pynrm)
-![GitHub issues](https://img.shields.io/github/issues/katehyerinjeon/pynrm)
+[![GitHub issues](https://img.shields.io/github/issues/katehyerinjeon/pynrm)](https://github.com/katehyerinjeon/pynrm/issues)
 [![Docs](https://img.shields.io/readthedocs/pynrm.svg)](https://pynrm.readthedocs.io/)
 
 ## Overview
 The numerator relationship matrix describes additive genetic relationships within a population.
 Numerous evaluation-selection systems have been devised to produce populations with favorable genetic responses while maintaining moderate to low rates of inbreeding.
 `pynrm` provides a simple yet powerful simulation tool to forecast the stochastic impacts of these systems.
 One major bottleneck to running these simulations is that as the number of animals bred increases, the size of the matrix grows exponentially.
 `pynrm` efficiently solves for the numerator relationship matrix values by tracing up the pedigree for only the relevant ancestors, thereby minimizing computational overhead.
 
 ## Basic Usage
 ### Installation
 `pynrm` is available on PyPI:
 
 ```shell
-$ pip install pyrnm
+$ pip install pynrm
 ```
 
 ### Supported Features
 - Livestock reproduction simulations that provide fine-grained control
 ```python
 from pynrm import Pedigree, Simulator
 
-pedigree = Pedigree()
-simulator = Simulator(pedigree, 10, 100, 0.6, 1)
+# Create a simulator instance
+simulator = Simulator(Pedigree(50, 50), 5, 20, 0.6, 0.0)
 
-simulator.reproduce()
+# Reproduce 4 generations
+for i in range(4):
+    simulator.reproduce()
 ```
 
-- Data visualization and analysis of simulation results (COMING SOON)
+- Data visualization and analysis of simulation results
+```python
+# Plot average inbreeding coefficients by generation
+simulator.plot_inbreeding_by_gen()
+
+# Plot average EBV by generation
+simulator.plot_ebv_by_gen()
+
+# Export generated pedigree data as csv
+simulator.export_to_csv("pedigree.csv")
+```
 
 ## Documentation
 Official documentation is available [here](https://pynrm.readthedocs.io/).
 
 ## Contribution
 Contributions are welcome! There are many ways to contribute to this project. Get started [here](CONTRIBUTING.md).
```

### Comparing `pynrm-0.1.1/README.md` & `pynrm-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 # pynrm
 
 `pynrm` is a lightweight and extensible Python library for livestock breeding simulation.
 
 ![Build Status](https://github.com/katehyerinjeon/pynrm/actions/workflows/build.yml/badge.svg)
-![PyPI](https://img.shields.io/pypi/v/pynrm)
+[![PyPI](https://img.shields.io/pypi/v/pynrm)](https://pypi.org/project/pynrm/)
 [![codecov](https://codecov.io/gh/katehyerinjeon/pynrm/branch/main/graph/badge.svg)](https://codecov.io/gh/katehyerinjeon/pynrm)
 ![GitHub](https://img.shields.io/github/license/katehyerinjeon/pynrm)
-![GitHub issues](https://img.shields.io/github/issues/katehyerinjeon/pynrm)
+[![GitHub issues](https://img.shields.io/github/issues/katehyerinjeon/pynrm)](https://github.com/katehyerinjeon/pynrm/issues)
 [![Docs](https://img.shields.io/readthedocs/pynrm.svg)](https://pynrm.readthedocs.io/)
 
 ## Overview
 The numerator relationship matrix describes additive genetic relationships within a population.
 Numerous evaluation-selection systems have been devised to produce populations with favorable genetic responses while maintaining moderate to low rates of inbreeding.
 `pynrm` provides a simple yet powerful simulation tool to forecast the stochastic impacts of these systems.
 One major bottleneck to running these simulations is that as the number of animals bred increases, the size of the matrix grows exponentially.
 `pynrm` efficiently solves for the numerator relationship matrix values by tracing up the pedigree for only the relevant ancestors, thereby minimizing computational overhead.
 
 ## Basic Usage
 ### Installation
 `pynrm` is available on PyPI:
 
 ```shell
-$ pip install pyrnm
+$ pip install pynrm
 ```
 
 ### Supported Features
 - Livestock reproduction simulations that provide fine-grained control
 ```python
 from pynrm import Pedigree, Simulator
 
-pedigree = Pedigree()
-simulator = Simulator(pedigree, 10, 100, 0.6, 1)
+# Create a simulator instance
+simulator = Simulator(Pedigree(50, 50), 5, 20, 0.6, 0.0)
 
-simulator.reproduce()
+# Reproduce 4 generations
+for i in range(4):
+    simulator.reproduce()
 ```
 
-- Data visualization and analysis of simulation results (COMING SOON)
+- Data visualization and analysis of simulation results
+```python
+# Plot average inbreeding coefficients by generation
+simulator.plot_inbreeding_by_gen()
+
+# Plot average EBV by generation
+simulator.plot_ebv_by_gen()
+
+# Export generated pedigree data as csv
+simulator.export_to_csv("pedigree.csv")
+```
 
 ## Documentation
 Official documentation is available [here](https://pynrm.readthedocs.io/).
 
 ## Contribution
 Contributions are welcome! There are many ways to contribute to this project. Get started [here](CONTRIBUTING.md).
```

### Comparing `pynrm-0.1.1/docs/Makefile` & `pynrm-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynrm-0.1.1/docs/conf.py` & `pynrm-0.1.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'pynrm'
 copyright = '2023, Kate Jeon'
 author = 'Kate Jeon'
 
 # The full version, including alpha/beta/rc tags
-release = '0.1.0'
+release = '0.1.2'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `pynrm-0.1.1/docs/index.rst` & `pynrm-0.1.2/docs/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -35,21 +35,40 @@
 
 -  Livestock reproduction simulations that provide fine-grained control
 
 .. code:: python
 
    from pynrm import Pedigree, Simulator
 
-   pedigree = Pedigree()
-   simulator = Simulator(pedigree, 10, 100, 0.6, 1)
+   # Create a simulator instance
+   simulator = Simulator(Pedigree(50, 50), 5, 20, 0.6, 0.0)
 
-   simulator.reproduce()
+   # Reproduce 4 generations
+   for i in range(4):
+      simulator.reproduce()
 
 -  Data visualization and analysis of simulation results
 
+.. code:: python
+
+   # Plot average inbreeding coefficients by generation
+   simulator.plot_inbreeding_by_gen()
+
+   # Plot average EBV by generation
+   simulator.plot_ebv_by_gen()
+
+   # Export generated pedigree data as csv
+   simulator.export_to_csv("pedigree.csv")
+
+.. image:: images/fig1.png
+   :width: 600
+
+.. image:: images/fig2.png
+   :width: 600
+
 Reference
 ---------
 
 .. toctree::
    :maxdepth: 4
 
    pynrm
```

### Comparing `pynrm-0.1.1/docs/make.bat` & `pynrm-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynrm-0.1.1/docs/pynrm.rst` & `pynrm-0.1.2/docs/pynrm.rst`

 * *Files identical despite different names*

### Comparing `pynrm-0.1.1/pynrm/Pedigree.py` & `pynrm-0.1.2/pynrm/Pedigree.py`

 * *Files identical despite different names*

### Comparing `pynrm-0.1.1/pynrm/Simulator.py` & `pynrm-0.1.2/pynrm/Simulator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import matplotlib.pyplot as plt
 import numpy as np
 import random
-from .nrm import get_nrm
+from .nrm import get_nrm, get_avg_inbreeding
 from .Pedigree import Pedigree
 
 
 class Simulator:
     """Simulates reproductive cycles.
 
     Performs livestock breeding simulations that provide fine-grained control.
@@ -55,25 +56,25 @@
         self.h = h
         self.w = w
         self.gen = 0
 
     def get_ebv(self, sire, dam):
         """Randomly generates EBV of an individual animal.
 
-        EBV is computed using heritability, EBV values and inbreeding coefficients of sire and dam. It first solves the
+        EBV is computed using heritability, EBV and inbreeding coefficients of sire and dam. It first solves the
         square root of heritability and average of inbreeding coefficients of sire and dam derived from NRM. Then, it
-        calculates some values, multiplies by random normal deviates, and adds them to the average of EBV values of
+        calculates some values, multiplies by random normal deviates, and adds them to the average of EBV of
         sire and dam.
 
         Args:
             sire: An integer indicating the sire id.
             dam: An integer indicating the dam id.
 
         Returns:
-            A float that corresponds to the randomly generated ebv value.
+            A float that corresponds to the randomly generated EBV.
         """
 
         if sire < 0:
             raise ValueError("'sire' cannot be negative")
         if dam < 0:
             raise ValueError("'dam' cannot be negative")
 
@@ -83,26 +84,26 @@
         ebv = 0.5 * (self.pedigree.data.iloc[sire].ebv + self.pedigree.data.iloc[dam].ebv)
         +round(np.random.normal(0, 1), 3) * h_sqrt * np.sqrt((1 - f) / 2)
         +round(np.random.normal(0, 1), 3) * np.sqrt(1 - self.h)
 
         return round(ebv, 3)
 
     def get_adjusted_ebv(self, candidate, already_selected):
-        """Computes adjusted EBV value of the candidate.
+        """Computes adjusted EBV of the candidate.
 
-        EBV values are adjusted to alleviate high inbreeding when selecting top k animals. This is calculated by
-        solving the average relationship between the candidate and already selected animals. EBV value of the candidate
+        EBV is adjusted to alleviate high inbreeding when selecting top k animals. This is calculated by
+        solving the average relationship between the candidate and already selected animals. EBV of the candidate
         is then penalized for the average relationship with the user-defined weight of the simulator.
 
         Args:
             candidate: An integer indicating the candidate id.
             already_selected: A list of already selected animals.
 
         Returns:
-            A float that corresponds to the adjusted EBV value of the candidate.
+            A float that corresponds to the adjusted EBV of the candidate.
         """
 
         ebv = self.pedigree.data.iloc[candidate].ebv
 
         # if none selected as top k yet, then original EBV is used for scoring
         if len(already_selected) == 0:
             return round(ebv, 3)
@@ -136,18 +137,18 @@
         if len(top_k) > k:
             raise ValueError("Length of 'top_k' should not exceed k")
 
         # base case - top k animals selected
         if len(top_k) == k:
             return top_k
 
+        # print("Length of candidates:", len(candidates))
         # recursive case
         for i, candidate in enumerate(candidates):
             adjusted_ebv = self.get_adjusted_ebv(candidate, top_k)
-
             if i == 0:
                 selected = candidate
                 max_adjusted_ebv = adjusted_ebv
             else:
                 if adjusted_ebv > max_adjusted_ebv:
                     selected = candidate
                     max_adjusted_ebv = adjusted_ebv
@@ -170,15 +171,17 @@
         # fetch all males and females from the latest generation
         curr_gen = self.pedigree.data[self.pedigree.data["gen"] == self.gen]
         all_males = curr_gen[curr_gen["sex"] == "M"].index.tolist()
         all_females = curr_gen[curr_gen["sex"] == "F"].index.tolist()
 
         # select top males and females to reproduce
         top_males = self.get_top_k([], all_males, self.male_k)
+        # print("Get top {} males from {} done".format(self.male_k, len(all_males)))
         top_females = self.get_top_k([], all_females, self.female_k)
+        # print("Get top {} females {} done".format(self.female_k, len(all_females)))
 
         # copy current pedigree data before reproduction and increment generation number
         new_pedigree_data = self.pedigree.data
         self.gen += 1
 
         for i in range(len(top_males)):
             sire = top_males[i]
@@ -192,7 +195,55 @@
                     ebv,
                     random.choices(["M", "F"])[0],
                 ]
 
         self.pedigree = Pedigree(new_pedigree_data)
 
         return new_pedigree_data
+
+    def plot_inbreeding_by_gen(self):
+        """Plot average inbreeding coefficients by generation.
+
+        Average inbreeding coefficients by generation is calculated and displayed as a basic line graph. All
+        generations that have been generated in a Simulator instance is displayed.
+        """
+        gen = list(range(0, self.gen + 1))
+        avg_inbreeding = []
+
+        for i in range(self.gen + 1):
+            avg_inbreeding.append(get_avg_inbreeding(self.pedigree, i))
+
+        plt.plot(gen, avg_inbreeding)
+        plt.xticks(np.arange(0, self.gen + 1, 1))
+        plt.xlabel("Generation")
+        plt.ylabel("Inbreeding Coefficient")
+        plt.title("Average Inbreeding Coefficient by Generation")
+        plt.show()
+
+    def plot_ebv_by_gen(self):
+        """Plot average EBV by generation.
+
+        Average EBV by generation is calculated and displayed as a basic line graph. All generations that have been
+        generated in a Simulator instance is displayed.
+        """
+        gen = list(range(0, self.gen + 1))
+        avg_ebv = []
+
+        for i in range(self.gen + 1):
+            avg_ebv.append(self.pedigree.get_avg_ebv(i))
+
+        plt.plot(gen, avg_ebv)
+        plt.xticks(np.arange(0, self.gen + 1, 1))
+        plt.xlabel("Generation")
+        plt.ylabel("Estimated Breeding Value")
+        plt.title("Average Estimated Breeding Value by Generation")
+        plt.show()
+
+    def export_to_csv(self, filename):
+        """Exports generated pedigree data as csv.
+
+        Writes pedigree data that have been generated in a Simulator instance to a comma-separated values (csv) file.
+
+        Args:
+            filename: A name of the path object or file-like object to export to.
+        """
+        self.pedigree.data.to_csv(filename)
```

### Comparing `pynrm-0.1.1/pynrm/nrm.py` & `pynrm-0.1.2/pynrm/nrm.py`

 * *Files identical despite different names*

### Comparing `pynrm-0.1.1/pynrm/tests/test_nrm.py` & `pynrm-0.1.2/pynrm/tests/test_nrm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 from pynrm.nrm import get_nrm, get_avg_inbreeding
-from pynrm.Pedigree import Pedigree
+import pynrm.Pedigree as Pedigree
 
 
 class TestNrm(unittest.TestCase):
     def setUp(self):
-        self.pedigree = Pedigree()
+        self.pedigree = Pedigree.Pedigree()
 
     def tearDown(self):
         self.pedigree = None
 
     def test_get_nrm(self):
         with self.assertRaises(TypeError):
             get_nrm("not dataframe", 0, 0)
```

### Comparing `pynrm-0.1.1/pynrm/tests/test_pedigree.py` & `pynrm-0.1.2/pynrm/tests/test_pedigree.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import pandas as pd
 import unittest
-from pynrm.Pedigree import Pedigree
+import pynrm.Pedigree as Pedigree
 
 
 class TestSimulator(unittest.TestCase):
     def setUp(self):
-        self.pedigree = Pedigree()
+        self.pedigree = Pedigree.Pedigree()
 
     def tearDown(self):
         self.pedigree = None
 
     def test_pedigree(self):
         with self.assertRaises(TypeError):
-            Pedigree("not dataframe")
+            Pedigree.Pedigree("not dataframe")
 
         self.assertEqual(self.pedigree.data.shape[1], 5, "expected 5 columns")
         self.assertEqual(self.pedigree.data[self.pedigree.data["sex"] == "M"].shape[0], 500, "expected 500 males")
         self.assertEqual(self.pedigree.data[self.pedigree.data["sex"] == "F"].shape[0], 500, "expected 500 females")
         self.assertEqual(self.pedigree.data["gen"][0], 0, "expected generation 0")
         self.assertTrue(pd.isna(self.pedigree.data["sire"][0]), "expected sire NA")
         self.assertTrue(pd.isna(self.pedigree.data["dam"][0]), "expected dam NA")
```

### Comparing `pynrm-0.1.1/pynrm/tests/test_simulator.py` & `pynrm-0.1.2/pynrm/tests/test_simulator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import unittest
-from pynrm.Pedigree import Pedigree
-from pynrm.Simulator import Simulator
+from unittest import mock
+import pynrm.Simulator as Simulator
+import pynrm.Pedigree as Pedigree
 
 
 class TestSimulator(unittest.TestCase):
     def setUp(self):
-        self.simulator = Simulator(Pedigree(), 2, 4, 0.6, 0.2)
+        self.simulator = Simulator.Simulator(Pedigree.Pedigree(), 2, 4, 0.6, 0.2)
 
     def tearDown(self):
         self.simulator = None
 
     def test_simulator(self):
         with self.assertRaises(TypeError):
-            Simulator("not dataframe", 2, 4, 0.6, 0.2)
+            Simulator.Simulator("not dataframe", 2, 4, 0.6, 0.2)
         with self.assertRaises(TypeError):
-            Simulator(self.simulator.pedigree, "not int", 4, 0.6, 0.2)
+            Simulator.Simulator(self.simulator.pedigree, "not int", 4, 0.6, 0.2)
         with self.assertRaises(TypeError):
-            Simulator(self.simulator.pedigree, 2, "not int", 0.6, 0.2)
+            Simulator.Simulator(self.simulator.pedigree, 2, "not int", 0.6, 0.2)
         with self.assertRaises(TypeError):
-            Simulator(self.simulator.pedigree, 2, 4, "not float", 0.2)
+            Simulator.Simulator(self.simulator.pedigree, 2, 4, "not float", 0.2)
         with self.assertRaises(TypeError):
-            Simulator(self.simulator.pedigree, 2, 4, 0.6, "not float")
+            Simulator.Simulator(self.simulator.pedigree, 2, 4, 0.6, "not float")
         with self.assertRaises(ValueError):
-            Simulator(self.simulator.pedigree, -2, 4, 0.6, 0.2)
+            Simulator.Simulator(self.simulator.pedigree, -2, 4, 0.6, 0.2)
         with self.assertRaises(ValueError):
-            Simulator(self.simulator.pedigree, 2, -4, 0.6, 0.2)
+            Simulator.Simulator(self.simulator.pedigree, 2, -4, 0.6, 0.2)
         with self.assertRaises(ValueError):
-            Simulator(self.simulator.pedigree, 2, 4, -0.6, 0.2)
+            Simulator.Simulator(self.simulator.pedigree, 2, 4, -0.6, 0.2)
         with self.assertRaises(ValueError):
-            Simulator(self.simulator.pedigree, 2, 4, 0.6, -0.2)
+            Simulator.Simulator(self.simulator.pedigree, 2, 4, 0.6, -0.2)
 
     def test_get_ebv(self):
         with self.assertRaises(ValueError):
             self.simulator.get_ebv(-1, 0)
         with self.assertRaises(ValueError):
             self.simulator.get_ebv(0, -1)
 
@@ -56,10 +57,27 @@
             "not a list with the best ebv when k = 1",
         )
 
     def test_reproduce(self):
         self.simulator.reproduce()
         self.assertEqual(self.simulator.gen, 1, "generation not incremented")
 
+    @mock.patch("%s.Simulator.plt" % __name__)
+    def test_plot_inbreeding_by_gen(self, mock_plt):
+        self.simulator.reproduce()
+        self.simulator.plot_inbreeding_by_gen()
+        mock_plt.title.assert_called_once_with("Average Inbreeding Coefficient by Generation")
+
+    @mock.patch("%s.Simulator.plt" % __name__)
+    def test_plot_ebv_by_gen(self, mock_plt):
+        self.simulator.reproduce()
+        self.simulator.plot_ebv_by_gen()
+        mock_plt.title.assert_called_once_with("Average Estimated Breeding Value by Generation")
+
+    def test_export_to_csv(self):
+        with mock.patch.object(self.simulator.pedigree.data, "to_csv") as to_csv_mock:
+            self.simulator.export_to_csv("pedigree.csv")
+            to_csv_mock.assert_called_with("pedigree.csv")
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pynrm-0.1.1/pynrm.egg-info/PKG-INFO` & `pynrm-0.1.2/pynrm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrm
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python library for animal breeding simulation
 Author-email: Kate Jeon <hj2589@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,46 +221,58 @@
 License-File: LICENSE
 
 # pynrm
 
 `pynrm` is a lightweight and extensible Python library for livestock breeding simulation.
 
 ![Build Status](https://github.com/katehyerinjeon/pynrm/actions/workflows/build.yml/badge.svg)
-![PyPI](https://img.shields.io/pypi/v/pynrm)
+[![PyPI](https://img.shields.io/pypi/v/pynrm)](https://pypi.org/project/pynrm/)
 [![codecov](https://codecov.io/gh/katehyerinjeon/pynrm/branch/main/graph/badge.svg)](https://codecov.io/gh/katehyerinjeon/pynrm)
 ![GitHub](https://img.shields.io/github/license/katehyerinjeon/pynrm)
-![GitHub issues](https://img.shields.io/github/issues/katehyerinjeon/pynrm)
+[![GitHub issues](https://img.shields.io/github/issues/katehyerinjeon/pynrm)](https://github.com/katehyerinjeon/pynrm/issues)
 [![Docs](https://img.shields.io/readthedocs/pynrm.svg)](https://pynrm.readthedocs.io/)
 
 ## Overview
 The numerator relationship matrix describes additive genetic relationships within a population.
 Numerous evaluation-selection systems have been devised to produce populations with favorable genetic responses while maintaining moderate to low rates of inbreeding.
 `pynrm` provides a simple yet powerful simulation tool to forecast the stochastic impacts of these systems.
 One major bottleneck to running these simulations is that as the number of animals bred increases, the size of the matrix grows exponentially.
 `pynrm` efficiently solves for the numerator relationship matrix values by tracing up the pedigree for only the relevant ancestors, thereby minimizing computational overhead.
 
 ## Basic Usage
 ### Installation
 `pynrm` is available on PyPI:
 
 ```shell
-$ pip install pyrnm
+$ pip install pynrm
 ```
 
 ### Supported Features
 - Livestock reproduction simulations that provide fine-grained control
 ```python
 from pynrm import Pedigree, Simulator
 
-pedigree = Pedigree()
-simulator = Simulator(pedigree, 10, 100, 0.6, 1)
+# Create a simulator instance
+simulator = Simulator(Pedigree(50, 50), 5, 20, 0.6, 0.0)
 
-simulator.reproduce()
+# Reproduce 4 generations
+for i in range(4):
+    simulator.reproduce()
 ```
 
-- Data visualization and analysis of simulation results (COMING SOON)
+- Data visualization and analysis of simulation results
+```python
+# Plot average inbreeding coefficients by generation
+simulator.plot_inbreeding_by_gen()
+
+# Plot average EBV by generation
+simulator.plot_ebv_by_gen()
+
+# Export generated pedigree data as csv
+simulator.export_to_csv("pedigree.csv")
+```
 
 ## Documentation
 Official documentation is available [here](https://pynrm.readthedocs.io/).
 
 ## Contribution
 Contributions are welcome! There are many ways to contribute to this project. Get started [here](CONTRIBUTING.md).
```

### Comparing `pynrm-0.1.1/pyproject.toml` & `pynrm-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "pynrm"
 authors = [{name = "Kate Jeon", email = "hj2589@columbia.edu"}]
 description="A python library for animal breeding simulation"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.7"
 
-dependencies = ["numpy", "pandas"]
+dependencies = ["numpy", "pandas", "matplotlib"]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
```

