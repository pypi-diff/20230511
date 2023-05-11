# Comparing `tmp/graph-ensembles-0.2.1.tar.gz` & `tmp/graph-ensembles-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph-ensembles-0.2.1.tar", last modified: Tue Aug  3 15:31:30 2021, max compression
+gzip compressed data, was "graph-ensembles-0.2.2.tar", last modified: Thu May 11 21:27:50 2023, max compression
```

## Comparing `graph-ensembles-0.2.1.tar` & `graph-ensembles-0.2.2.tar`

### file list

```diff
@@ -1,46 +1,51 @@
-drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2021-08-03 15:31:30.001260 graph-ensembles-0.2.1/
--rw-r--r--   0 Leonardo   (501) staff       (20)     1854 2021-08-03 15:30:25.000000 graph-ensembles-0.2.1/HISTORY.rst
--rw-r--r--   0 Leonardo   (501) staff       (20)     1667 2020-11-16 10:28:50.000000 graph-ensembles-0.2.1/LICENSE.txt
--rw-r--r--   0 Leonardo   (501) staff       (20)      377 2021-07-12 08:00:10.000000 graph-ensembles-0.2.1/MANIFEST.in
--rw-r--r--   0 Leonardo   (501) staff       (20)     6816 2021-08-03 15:31:30.000935 graph-ensembles-0.2.1/PKG-INFO
--rw-r--r--   0 Leonardo   (501) staff       (20)     2827 2021-03-14 14:51:32.000000 graph-ensembles-0.2.1/README.rst
--rw-r--r--   0 Leonardo   (501) staff       (20)       65 2021-06-14 18:58:35.000000 graph-ensembles-0.2.1/cov_test.sh
-drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2021-08-03 15:31:29.989675 graph-ensembles-0.2.1/examples/
--rw-r--r--   0 Leonardo   (501) staff       (20)   129984 2021-03-29 15:02:35.000000 graph-ensembles-0.2.1/examples/block_graph.ipynb
--rw-r--r--   0 Leonardo   (501) staff       (20)    89087 2021-03-14 14:51:32.000000 graph-ensembles-0.2.1/examples/stripe_graph.ipynb
-drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2021-08-03 15:31:29.992818 graph-ensembles-0.2.1/performance/
--rw-r--r--   0 Leonardo   (501) staff       (20)     2174 2021-04-07 09:12:42.000000 graph-ensembles-0.2.1/performance/block_model.py
--rw-r--r--   0 Leonardo   (501) staff       (20)     4696 2021-07-12 08:00:10.000000 graph-ensembles-0.2.1/performance/fitness_model.py
--rw-r--r--   0 Leonardo   (501) staff       (20)     4002 2021-07-12 08:00:10.000000 graph-ensembles-0.2.1/performance/graph_gen.py
--rw-r--r--   0 Leonardo   (501) staff       (20)     5615 2021-07-12 08:00:10.000000 graph-ensembles-0.2.1/performance/label_graph_gen.py
--rw-r--r--   0 Leonardo   (501) staff       (20)     1256 2021-07-12 08:00:10.000000 graph-ensembles-0.2.1/performance/perf_all.sh
--rw-r--r--   0 Leonardo   (501) staff       (20)     5106 2021-07-12 08:00:10.000000 graph-ensembles-0.2.1/performance/stripe_model_inv.py
--rw-r--r--   0 Leonardo   (501) staff       (20)     5646 2021-07-12 08:00:10.000000 graph-ensembles-0.2.1/performance/stripe_model_multi.py
--rw-r--r--   0 Leonardo   (501) staff       (20)     5036 2021-07-12 08:00:10.000000 graph-ensembles-0.2.1/performance/stripe_model_single.py
--rw-r--r--   0 Leonardo   (501) staff       (20)       53 2020-11-16 10:28:50.000000 graph-ensembles-0.2.1/publish.sh
--rw-r--r--   0 Leonardo   (501) staff       (20)      161 2021-03-14 14:51:32.000000 graph-ensembles-0.2.1/pytest.ini
--rw-r--r--   0 Leonardo   (501) staff       (20)       38 2021-08-03 15:31:30.001376 graph-ensembles-0.2.1/setup.cfg
--rw-r--r--   0 Leonardo   (501) staff       (20)     1887 2021-08-03 15:30:49.000000 graph-ensembles-0.2.1/setup.py
-drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2021-08-03 15:31:29.985029 graph-ensembles-0.2.1/src/
-drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2021-08-03 15:31:29.994727 graph-ensembles-0.2.1/src/graph_ensembles/
--rw-r--r--   0 Leonardo   (501) staff       (20)       84 2021-04-07 09:09:39.000000 graph-ensembles-0.2.1/src/graph_ensembles/__init__.py
--rw-r--r--   0 Leonardo   (501) staff       (20)    41106 2021-08-02 15:01:51.000000 graph-ensembles-0.2.1/src/graph_ensembles/graphs.py
--rw-r--r--   0 Leonardo   (501) staff       (20)     5811 2021-04-07 09:09:39.000000 graph-ensembles-0.2.1/src/graph_ensembles/lib.py
-drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2021-08-03 15:31:29.998468 graph-ensembles-0.2.1/src/graph_ensembles/methods/
--rw-r--r--   0 Leonardo   (501) staff       (20)       67 2021-03-14 14:51:32.000000 graph-ensembles-0.2.1/src/graph_ensembles/methods/__init__.py
--rw-r--r--   0 Leonardo   (501) staff       (20)    46081 2021-08-03 12:43:10.000000 graph-ensembles-0.2.1/src/graph_ensembles/methods/ensemble.py
--rw-r--r--   0 Leonardo   (501) staff       (20)    11256 2021-04-07 09:09:39.000000 graph-ensembles-0.2.1/src/graph_ensembles/methods/graph.py
--rw-r--r--   0 Leonardo   (501) staff       (20)     8934 2021-07-12 08:00:10.000000 graph-ensembles-0.2.1/src/graph_ensembles/methods/solver.py
--rw-r--r--   0 Leonardo   (501) staff       (20)    94356 2021-08-03 12:47:54.000000 graph-ensembles-0.2.1/src/graph_ensembles/models.py
-drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2021-08-03 15:31:29.996857 graph-ensembles-0.2.1/src/graph_ensembles.egg-info/
--rw-r--r--   0 Leonardo   (501) staff       (20)     6816 2021-08-03 15:31:29.000000 graph-ensembles-0.2.1/src/graph_ensembles.egg-info/PKG-INFO
--rw-r--r--   0 Leonardo   (501) staff       (20)      985 2021-08-03 15:31:29.000000 graph-ensembles-0.2.1/src/graph_ensembles.egg-info/SOURCES.txt
--rw-r--r--   0 Leonardo   (501) staff       (20)        1 2021-08-03 15:31:29.000000 graph-ensembles-0.2.1/src/graph_ensembles.egg-info/dependency_links.txt
--rw-r--r--   0 Leonardo   (501) staff       (20)      228 2021-08-03 15:31:29.000000 graph-ensembles-0.2.1/src/graph_ensembles.egg-info/requires.txt
--rw-r--r--   0 Leonardo   (501) staff       (20)       16 2021-08-03 15:31:29.000000 graph-ensembles-0.2.1/src/graph_ensembles.egg-info/top_level.txt
-drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2021-08-03 15:31:30.000289 graph-ensembles-0.2.1/tests/
--rw-r--r--   0 Leonardo   (501) staff       (20)    28134 2021-07-12 08:00:10.000000 graph-ensembles-0.2.1/tests/test_block_model.py
--rw-r--r--   0 Leonardo   (501) staff       (20)    27023 2021-07-12 08:00:10.000000 graph-ensembles-0.2.1/tests/test_fitness_model.py
--rw-r--r--   0 Leonardo   (501) staff       (20)    45888 2021-04-07 09:09:39.000000 graph-ensembles-0.2.1/tests/test_graph_object.py
--rw-r--r--   0 Leonardo   (501) staff       (20)    75390 2021-08-03 15:14:43.000000 graph-ensembles-0.2.1/tests/test_stripe_model.py
--rw-r--r--   0 Leonardo   (501) staff       (20)      111 2021-03-14 14:51:32.000000 graph-ensembles-0.2.1/tox.ini
+drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2023-05-11 21:27:50.259766 graph-ensembles-0.2.2/
+-rw-r--r--   0 Leonardo   (501) staff       (20)     1987 2023-05-11 21:09:11.000000 graph-ensembles-0.2.2/HISTORY.rst
+-rw-r--r--   0 Leonardo   (501) staff       (20)     1667 2020-11-16 10:28:50.000000 graph-ensembles-0.2.2/LICENSE.txt
+-rw-r--r--   0 Leonardo   (501) staff       (20)      377 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/MANIFEST.in
+-rw-r--r--   0 Leonardo   (501) staff       (20)     5696 2023-05-11 21:27:50.259101 graph-ensembles-0.2.2/PKG-INFO
+-rw-r--r--   0 Leonardo   (501) staff       (20)     2827 2021-03-14 14:51:32.000000 graph-ensembles-0.2.2/README.rst
+-rw-r--r--   0 Leonardo   (501) staff       (20)       65 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/cov_test.sh
+drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2023-05-11 21:27:50.233084 graph-ensembles-0.2.2/examples/
+-rw-r--r--   0 Leonardo   (501) staff       (20)   129984 2021-03-29 15:02:35.000000 graph-ensembles-0.2.2/examples/block_graph.ipynb
+-rw-r--r--   0 Leonardo   (501) staff       (20)    89087 2021-03-14 14:51:32.000000 graph-ensembles-0.2.2/examples/stripe_graph.ipynb
+drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2023-05-11 21:27:50.239434 graph-ensembles-0.2.2/performance/
+-rw-r--r--   0 Leonardo   (501) staff       (20)     2174 2021-04-07 09:12:42.000000 graph-ensembles-0.2.2/performance/block_model.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)     4696 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/performance/fitness_model.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)     4002 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/performance/graph_gen.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)     5615 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/performance/label_graph_gen.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)     1256 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/performance/perf_all.sh
+-rw-r--r--   0 Leonardo   (501) staff       (20)     5106 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/performance/stripe_model_inv.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)     5646 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/performance/stripe_model_multi.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)     5036 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/performance/stripe_model_single.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)       53 2020-11-16 10:28:50.000000 graph-ensembles-0.2.2/publish.sh
+-rw-r--r--   0 Leonardo   (501) staff       (20)      161 2021-03-14 14:51:32.000000 graph-ensembles-0.2.2/pytest.ini
+-rw-r--r--   0 Leonardo   (501) staff       (20)       38 2023-05-11 21:27:50.259971 graph-ensembles-0.2.2/setup.cfg
+-rw-r--r--   0 Leonardo   (501) staff       (20)     1887 2023-05-11 21:26:47.000000 graph-ensembles-0.2.2/setup.py
+drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2023-05-11 21:27:50.224064 graph-ensembles-0.2.2/src/
+drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2023-05-11 21:27:50.243046 graph-ensembles-0.2.2/src/graph_ensembles/
+-rw-r--r--   0 Leonardo   (501) staff       (20)      104 2023-05-11 21:05:22.000000 graph-ensembles-0.2.2/src/graph_ensembles/__init__.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)    41106 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/src/graph_ensembles/graphs.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)     5811 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/src/graph_ensembles/lib.py
+drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2023-05-11 21:27:50.250129 graph-ensembles-0.2.2/src/graph_ensembles/methods/
+-rw-r--r--   0 Leonardo   (501) staff       (20)       67 2023-05-11 20:44:36.000000 graph-ensembles-0.2.2/src/graph_ensembles/methods/__init__.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)    50885 2023-05-11 20:41:01.000000 graph-ensembles-0.2.2/src/graph_ensembles/methods/ensemble.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)    11256 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/src/graph_ensembles/methods/graph.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)    21715 2023-05-11 20:54:24.000000 graph-ensembles-0.2.2/src/graph_ensembles/methods/solver.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)   116618 2023-05-11 20:41:01.000000 graph-ensembles-0.2.2/src/graph_ensembles/models.py
+drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2023-05-11 21:27:50.251801 graph-ensembles-0.2.2/src/graph_ensembles/spark/
+-rw-r--r--   0 Leonardo   (501) staff       (20)       22 2023-05-11 20:44:45.000000 graph-ensembles-0.2.2/src/graph_ensembles/spark/__init__.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)    34509 2023-05-11 21:04:52.000000 graph-ensembles-0.2.2/src/graph_ensembles/spark/models.py
+drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2023-05-11 21:27:50.246790 graph-ensembles-0.2.2/src/graph_ensembles.egg-info/
+-rw-r--r--   0 Leonardo   (501) staff       (20)     5696 2023-05-11 21:27:50.000000 graph-ensembles-0.2.2/src/graph_ensembles.egg-info/PKG-INFO
+-rw-r--r--   0 Leonardo   (501) staff       (20)     1114 2023-05-11 21:27:50.000000 graph-ensembles-0.2.2/src/graph_ensembles.egg-info/SOURCES.txt
+-rw-r--r--   0 Leonardo   (501) staff       (20)        1 2023-05-11 21:27:50.000000 graph-ensembles-0.2.2/src/graph_ensembles.egg-info/dependency_links.txt
+-rw-r--r--   0 Leonardo   (501) staff       (20)      228 2023-05-11 21:27:50.000000 graph-ensembles-0.2.2/src/graph_ensembles.egg-info/requires.txt
+-rw-r--r--   0 Leonardo   (501) staff       (20)       16 2023-05-11 21:27:50.000000 graph-ensembles-0.2.2/src/graph_ensembles.egg-info/top_level.txt
+drwxr-xr-x   0 Leonardo   (501) staff       (20)        0 2023-05-11 21:27:50.257712 graph-ensembles-0.2.2/tests/
+-rw-r--r--   0 Leonardo   (501) staff       (20)      575 2023-05-11 20:41:01.000000 graph-ensembles-0.2.2/tests/plot_tests.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)    28134 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/tests/test_block_model.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)    27023 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/tests/test_fitness_model.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)     1009 2023-05-11 20:41:01.000000 graph-ensembles-0.2.2/tests/test_fitness_model_multip.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)    45888 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/tests/test_graph_object.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)    75390 2023-03-24 09:59:51.000000 graph-ensembles-0.2.2/tests/test_stripe_model.py
+-rw-r--r--   0 Leonardo   (501) staff       (20)      111 2021-03-14 14:51:32.000000 graph-ensembles-0.2.2/tox.ini
```

### Comparing `graph-ensembles-0.2.1/HISTORY.rst` & `graph-ensembles-0.2.2/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 =======
 History
 =======
 
+0.2.2 (2023-05-11)
+------------------
+* Created submodule spark for allowing some models to be parallelize computations using spark
+
 0.2.1 (2021-08-03)
 ------------------
 * Added option for faster computation of average nearest neighbour properties by allowing for multiple links between the same nodes.
 * Added compression option in to_networkx function.
 
 0.2.0 (2021-07-12)
 ------------------
```

### Comparing `graph-ensembles-0.2.1/LICENSE.txt` & `graph-ensembles-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/README.rst` & `graph-ensembles-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/examples/block_graph.ipynb` & `graph-ensembles-0.2.2/examples/block_graph.ipynb`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/examples/stripe_graph.ipynb` & `graph-ensembles-0.2.2/examples/stripe_graph.ipynb`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/performance/block_model.py` & `graph-ensembles-0.2.2/performance/block_model.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/performance/fitness_model.py` & `graph-ensembles-0.2.2/performance/fitness_model.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/performance/graph_gen.py` & `graph-ensembles-0.2.2/performance/graph_gen.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/performance/label_graph_gen.py` & `graph-ensembles-0.2.2/performance/label_graph_gen.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/performance/perf_all.sh` & `graph-ensembles-0.2.2/performance/perf_all.sh`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/performance/stripe_model_inv.py` & `graph-ensembles-0.2.2/performance/stripe_model_inv.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/performance/stripe_model_multi.py` & `graph-ensembles-0.2.2/performance/stripe_model_multi.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/performance/stripe_model_single.py` & `graph-ensembles-0.2.2/performance/stripe_model_single.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/setup.py` & `graph-ensembles-0.2.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     history = history_file.read()
 
 setup(
     name='graph-ensembles',
     author="Leonardo Niccolò Ialongo",
     author_email='leonardo.ialongo@gmail.com',
     python_requires='>=3.0',
-    version='0.2.1',
+    version='0.2.2',
     url='https://github.com/LeonardoIalongo/graph-ensembles',
     description=("The graph ensemble package contains a set of methods to"
                  " build fitness based graph ensembles from marginal"
                  " information."),
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/x-rst',
     license="GNU General Public License v3",
@@ -27,26 +27,26 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Operating System :: OS Independent',
     ],
     packages=['graph_ensembles', 'graph_ensembles.methods'],
     package_dir={'': 'src'},
-    install_requires=["numpy>=1.15",
-                      "numba>=0.53",
+    install_requires=["numpy>=1.22",
+                      "numba>=0.56.4",
                       "scipy>=1.0",
                       "pandas>=1.1",
                       "networkx>=1.0"
                       ],
     extras_require={
-        "dev": ["pytest==6.0.1",
-                "coverage==5.2.1",
-                "pytest-cov==2.10.1",
-                "flake8==3.8.3",
-                "wheel==0.35.1",
-                "matplotlib==3.3.2",
-                "check-manifest==0.44",
-                "setuptools==47.1.0",
-                "twine==3.2.0",
-                "tox==3.20.1"],
+        "dev": ["pytest==7.3.1",
+                "coverage==7.2.5",
+                "pytest-cov==4.0.0",
+                "flake8==6.0.0",
+                "wheel==0.40.0",
+                "matplotlib==3.7.1",
+                "check-manifest==0.49",
+                "setuptools==67.7.2",
+                "twine==4.0.2",
+                "tox==4.5.1"],
         },
     )
```

### Comparing `graph-ensembles-0.2.1/src/graph_ensembles/graphs.py` & `graph-ensembles-0.2.2/src/graph_ensembles/graphs.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/src/graph_ensembles/lib.py` & `graph-ensembles-0.2.2/src/graph_ensembles/lib.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/src/graph_ensembles/methods/ensemble.py` & `graph-ensembles-0.2.2/src/graph_ensembles/methods/ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import numpy.random as rng
 from numba import jit
 from math import ceil, sqrt, isinf, exp, log
+from multiprocess import Process
 
 
 # --------------- PROBABILITY FUNCTIONALS ---------------
 @jit(nopython=True)
 def p_fitness(param, x_i, x_j):
     tmp = param[0]*x_i*x_j
     if isinf(tmp):
@@ -22,25 +23,25 @@
         return 0
     else:
         return tmp / (1 + tmp1)**2
 
 
 @jit(nopython=True)
 def p_invariant(param, x_i, x_j):
-    tmp = param[0]*x_i*x_j
+    tmp = param*x_i*x_j
     if isinf(tmp):
         return 1
     else:
         return 1 - exp(-tmp)
 
 
 @jit(nopython=True)
 def jac_invariant(param, x_i, x_j):
     tmp = x_i*x_j
-    tmp1 = param[0]*tmp
+    tmp1 = param*tmp
     if isinf(tmp1):
         return 0
     else:
         return tmp * exp(-tmp1)
 
 
 @jit(nopython=True)
@@ -156,14 +157,26 @@
     for j in np.arange(len(fit_j)):
         val = fit_j[j]
         if j != i:
             d += p_f(param, fit_i, val)
 
     return d
 
+@jit(nopython=True)
+def fit_exp_degree_vertex_selfloops(p_f, param, i, fit_i, fit_j):
+    """ Compute the expected degree of the i-th vertex.
+    """
+    d = 0
+    for j in np.arange(len(fit_j)):
+        val = fit_j[j]
+        d += p_f(param, fit_i, val)
+
+    return d
+
+
 
 @jit(nopython=True)
 def fit_exp_edges(p_f, param, fit_out, fit_in):
     """ Compute the expected number of edges.
     """
     exp_edges = 0
     for i in np.arange(len(fit_out)):
@@ -173,28 +186,56 @@
             if i != j:
                 exp_edges += p_f(param, v_out, v_in)
 
     return exp_edges
 
 
 @jit(nopython=True)
+def fit_exp_edges_selfloops(p_f, param, fit_out, fit_in):
+    """ Compute the expected number of edges.
+    """
+    exp_edges = 0
+    for i in np.arange(len(fit_out)):
+        v_out = fit_out[i]
+        for j in np.arange(len(fit_in)):
+            v_in = fit_in[j]
+            exp_edges += p_f(param, v_out, v_in)
+
+    return exp_edges
+
+
+@jit(nopython=True)
 def fit_exp_edges_jac(jac_f, param, fit_out, fit_in):
     """ Compute the Jacobian of the objective function of the newton solver and its
     derivative for a single label of the stripe model.
     """
     jac = 0
     for i in np.arange(len(fit_out)):
         s_out = fit_out[i]
         for j in np.arange(len(fit_in)):
             s_in = fit_in[j]
             if i != j:
                 jac = jac_f(param, s_out, s_in)
 
     return jac
 
+@jit(nopython=True)
+def fit_exp_edges_jac_selfloops(jac_f, param, fit_out, fit_in):
+    """ Compute the Jacobian of the objective function of the newton solver and its
+    derivative for a single label of the stripe model.
+    """
+    jac = 0
+    for i in np.arange(len(fit_out)):
+        s_out = fit_out[i]
+        for j in np.arange(len(fit_in)):
+            s_in = fit_in[j]
+            jac = jac_f(param, s_out, s_in)
+
+    return jac
+
 
 @jit(nopython=True)
 def fit_exp_edges_jac_alpha(jac_f, param, fit_out, fit_in):
     """ Compute the Jacobian of the objective function of the newton solver and its
     derivative for a single label of the stripe model.
     """
     jac = np.zeros(2, dtype=np.float64)
@@ -207,14 +248,31 @@
                 jac[0] += res[0]
                 jac[1] += res[1]
 
     return jac
 
 
 @jit(nopython=True)
+def fit_exp_edges_jac_alpha_selfloops(jac_f, param, fit_out, fit_in):
+    """ Compute the Jacobian of the objective function of the newton solver and its
+    derivative for a single label of the stripe model.
+    """
+    jac = np.zeros(2, dtype=np.float64)
+    for i in np.arange(len(fit_out)):
+        s_out = fit_out[i]
+        for j in np.arange(len(fit_in)):
+            s_in = fit_in[j]
+            res = jac_f(param, s_out, s_in)
+            jac[0] += res[0]
+            jac[1] += res[1]
+
+    return jac
+
+
+@jit(nopython=True)
 def fit_exp_degree(p_f, param, fit_out, fit_in):
     """ Compute the expected in and out degree sequences.
     """
     exp_d = np.zeros(len(fit_out), dtype=np.float64)
     exp_d_out = np.zeros(len(fit_out), dtype=np.float64)
     exp_d_in = np.zeros(len(fit_in), dtype=np.float64)
     for i in np.arange(len(fit_out)):
@@ -249,14 +307,38 @@
             s_in = fit_in[j]
             if i != j:
                 f += p_f(param, s_out, s_in)
                 jac += jac_f(param, s_out, s_in)
 
     return f - n_edges, jac
 
+@jit(nopython=True)
+def fit_f_jac_selfloops(p_f, jac_f, param, fit_out, fit_in):
+    """ Compute the objective function of the newton solver and its
+    derivative for a single label of the stripe model.
+    """
+    jac = 0
+    f = 0
+    for i in np.arange(len(fit_out)):
+        s_out = fit_out[i]
+        for j in np.arange(len(fit_in)):
+            s_in = fit_in[j]
+            f += p_f(param, s_out, s_in)
+            jac += jac_f(param, s_out, s_in)
+
+    return f, jac
+
+@jit(nopython=True)
+def NLL(param, out_in_pairs, remainder):
+    """Negative log likelihood of the scale invariant probability function"""
+    func = -np.sum(np.log(1-exp(-param*out_in_pairs[i][0]*out_in_pairs[i][1])) for i in range(len(out_in_pairs))) 
+    + param*(remainder - np.sum(out_in_pairs[i][0]*out_in_pairs[i][1] for i in range(len(out_in_pairs))))
+
+    return func
+    
 
 @jit(nopython=True)
 def fit_iterative(param, out_strength, in_strength, n_edges):
     """ Compute the next iteration of the fixed point method for a single
     label of the stripe model.
     """
     aux = 0
@@ -266,14 +348,30 @@
             s_in = in_strength[j]
             if i != j:
                 tmp = s_out*s_in
                 aux += tmp / (1 + param[0]*tmp)
 
     return n_edges/aux
 
+@jit(nopython=True)
+def fit_iterative_selfloops(param, out_strength, in_strength, n_edges):
+    """ Compute the next iteration of the fixed point method for a single
+    label of the stripe model.
+    """
+    aux = 0
+    for i in np.arange(len(out_strength)):
+        s_out = out_strength[i]
+        for j in np.arange(in_strength.shape[0]):
+            s_in = in_strength[j]
+            tmp = s_out*s_in
+            aux += tmp / (1 + param[0]*tmp)
+
+    return n_edges/aux
+
+
 
 @jit(nopython=True)
 def fit_eq_constr_alpha(x, p_f, fit_out, fit_in, num_e):
     exp_e = fit_exp_edges(p_f, x, fit_out, fit_in)
     return np.array([exp_e - num_e], dtype=np.float64)
 
 
@@ -299,14 +397,26 @@
             jac[0] += res[0]
             jac[1] += res[1]
 
     return jac
 
 
 @jit(nopython=True)
+def fit_ineq_jac_alpha_selfloops(x, jac_f, i, fit_i, fit_j):
+    jac = np.zeros(2, dtype=np.float64)
+    for j in np.arange(len(fit_j)):
+        j_val = fit_j[j]
+        res = jac_f(x, fit_i, j_val)
+        jac[0] += res[0]
+        jac[1] += res[1]
+
+    return jac
+
+
+@jit(nopython=True)
 def fit_av_nn_prop(p_f, param, fit_out, fit_in, prop, ndir='out'):
     """ Compute the expected number of edges.
     """
     av_nn = np.zeros(prop.shape, dtype=np.float64)
     for i in np.arange(len(fit_out)):
         s_out_i = fit_out[i]
         s_in_i = fit_in[i]
@@ -364,14 +474,48 @@
                 else:
                     like *= 1 - p
     if lgs:
         return like
     else:
         return log(like)
 
+@jit(nopython=True)
+def fit_likelihood_selfloops(adj_i, adj_j, p_f, param, out_strength, in_strength, lgs):
+    """ Compute the binary log likelihood of a graph given the fitted model.
+    """
+    if lgs:
+        like = 0
+    else:
+        like = 1
+
+    for i in np.arange(len(out_strength)):
+        s_out = out_strength[i]
+        n = adj_i[i]
+        m = adj_i[i+1]
+        j_list = adj_j[n:m]
+        for j in np.arange(len(in_strength)):
+            s_in = in_strength[j]
+            p = p_f(param, s_out, s_in)
+
+            # Check if link exists
+            if j in j_list:
+                if lgs:
+                    like += log(p)
+                else:
+                    like *= p
+            else:
+                if lgs:
+                    like += log(1 - p)
+                else:
+                    like *= 1 - p
+    if lgs:
+        return like
+    else:
+        return log(like)
+
 
 @jit(nopython=True)
 def fit_sample(p_f, param, out_strength, in_strength):
     """ Sample from the fitness model ensemble.
     """
     s_tot = np.sum(out_strength)
     msg = 'Sum of in/out strengths not the same.'
@@ -385,14 +529,34 @@
                 p = p_f(param, s_out, s_in)
                 if rng.random() < p:
                     w = np.float64(rng.exponential(s_out*s_in/(s_tot*p)))
                     sample.append((i, j, w))
 
     return sample
 
+@jit(nopython=True)
+def fit_sample_selfloops(p_f, param, out_strength, in_strength):
+    """ Sample from the fitness model ensemble.
+    """
+    s_tot = np.sum(out_strength)
+    msg = 'Sum of in/out strengths not the same.'
+    assert np.abs(1 - np.sum(in_strength)/s_tot) < 1e-6, msg
+    sample = []
+    for i in np.arange(len(out_strength)):
+        s_out = out_strength[i]
+        for j in np.arange(len(in_strength)):
+            s_in = in_strength[j]
+            p = p_f(param, s_out, s_in)
+            if rng.random() < p:
+                w = np.float64(rng.exponential(s_out*s_in/(s_tot*p)))
+                sample.append((i, j, w))
+
+    return sample
+
+
 
 # --------------- LAYER FITNESS METHODS ---------------
 @jit(nopython=True)
 def layer_exp_edges(p_f, param, fit_out, fit_in):
     """ Compute the expected number of edges.
     """
     exp_edges = 0
```

### Comparing `graph-ensembles-0.2.1/src/graph_ensembles/methods/graph.py` & `graph-ensembles-0.2.2/src/graph_ensembles/methods/graph.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/src/graph_ensembles/models.py` & `graph-ensembles-0.2.2/src/graph_ensembles/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 from . import graphs
 from . import methods as mt
 from . import lib
 import numpy as np
 import scipy.sparse as sp
 import warnings
+from src.graph_ensembles import methods as mt
+from numba import jit
+import time
+import multiprocessing as mp
+import scipy.optimize as opt
+from itertools import product
+
 
 
 class GraphEnsemble():
     """ General class for graph ensembles.
 
     All ensembles can be defined in three ways:
 
@@ -336,31 +343,26 @@
         the total number of edges
     num_vertices: int
         the total number of nodes
     z: float
         the density parameter
     """
 
-    def __init__(self, *args, scale_invariant=False, min_degree=False,
-                 **kwargs):
+    def __init__(self, *args, **kwargs):
         """ Return a FitnessModel for the given graph data.
 
         The model accepts as arguments either: a WeightedGraph, the
         strength sequences (in and out) and the number of edges,
         or the strength sequences and the z parameter.
 
         The model accepts the strength sequences as numpy recarrays. The first
         column must contain the node index to which the strength refers and
         in the second column there must be the value of the strength.
         All missing node ids are assumed zero.
 
-        The model defaults to the classic fitness model functional but can be
-        set to use the scale invariant formulation by setting the
-        scale_invariant flag to True. This changes the functional used for
-        the computation of the link probability but nothing else.
         """
         # If an argument is passed then it must be a graph
         if len(args) > 0:
             if isinstance(args[0], graphs.WeightedGraph):
                 g = args[0]
                 self.num_vertices = g.num_vertices
                 self.num_edges = g.num_edges
@@ -373,17 +375,14 @@
 
             if len(args) > 1:
                 msg = ('Unnamed arguments other than the Graph have been '
                        'ignored.')
                 warnings.warn(msg, UserWarning)
 
         # Get options from keyword arguments
-        self.scale_invariant = scale_invariant
-        self.min_degree = min_degree
-
         allowed_arguments = ['num_vertices', 'num_edges', 'out_strength',
                              'in_strength', 'param', 'discrete_weights']
         for name in kwargs:
             if name not in allowed_arguments:
                 raise ValueError('Illegal argument passed: ' + name)
             else:
                 setattr(self, name, kwargs[name])
@@ -453,18 +452,14 @@
             if self.num_edges < 0:
                 raise ValueError(
                     'Number of edges must be a positive number.')
         else:
             if not isinstance(self.param, np.ndarray):
                 self.param = np.array([self.param])
 
-            if self.min_degree:
-                if not (len(self.param) == 2):
-                    raise ValueError('The FitnessModel with min degree '
-                                     'correction requires two parameters.')
             else:
                 if not (len(self.param) == 1):
                     raise ValueError(
                         'The FitnessModel requires one parameter.')
             
             if not np.issubdtype(self.param.dtype, np.number):
                 raise ValueError('Parameters must be numeric.')
@@ -475,28 +470,16 @@
         # Check that sum of in and out strengths are equal
         msg = 'Sums of strengths do not match.'
         assert np.allclose(np.sum(self.out_strength),
                            np.sum(self.in_strength),
                            atol=1e-14, rtol=1e-9), msg
 
         # Get the correct probability functional
-        if scale_invariant:
-            if min_degree:
-                msg = 'Cannot constrain min degree in scale invariant model.'
-                raise ValueError(msg)
-            else:
-                self.prob_fun = mt.p_invariant
-                self.jac_fun = mt.jac_invariant
-        else:
-            if min_degree:
-                self.prob_fun = mt.p_fitness_alpha
-                self.jac_fun = mt.jac_fitness_alpha
-            else:
-                self.prob_fun = mt.p_fitness
-                self.jac_fun = mt.jac_fitness
+        self.prob_fun = mt.p_fitness
+        self.jac_fun = mt.jac_fitness
 
         # If param are set computed expected number of edges per label
         if hasattr(self, 'param'):
             self.num_edges = mt.fit_exp_edges(
                 self.prob_fun,
                 self.param,
                 self.out_strength,
@@ -520,103 +503,33 @@
         max_iter : int or float
             maximum number of iteration
         verbose: boolean
             if true print debug info while iterating
 
         """
         if method is None:
-            if not self.min_degree:
-                method = 'newton'
-        elif self.min_degree:
-            warnings.warn('Method not recognised for solver with min degree '
-                          'constraint, using default SLSQP.', UserWarning)
-
-        if (method == 'fixed-point') and self.scale_invariant:
-            raise Exception('Fixed point solver not supported for scale '
-                            'invariant functional.')
+            method = 'newton'
 
         if x0 is None:
-            if self.min_degree:
-                x0 = np.array([0, 1], dtype=np.float64)
-            else:
-                x0 = np.array([0], dtype=np.float64)
-        else:
-            if not isinstance(x0, np.ndarray):
-                try:
-                    x0 = np.array([x for x in x0])
-                except Exception:
-                    x0 = np.array([x0])
+            x0 = np.array([0], dtype=np.float64)
 
-            if self.min_degree:
-                if not (len(x0) == 2):
-                    raise ValueError('The FitnessModel with min degree '
-                                     'correction requires two parameters.')
-            else:
-                if not (len(x0) == 1):
-                    raise ValueError(
-                        'The FitnessModel requires one parameter.')
-
-            if not np.issubdtype(x0.dtype, np.number):
-                raise ValueError('x0 must be numeric.')
+        if not isinstance(x0, np.ndarray):
+            x0 = np.array([x0])
 
-            if np.any(x0 < 0):
-                raise ValueError('x0 must be positive.')
+        if not (len(x0) == 1):
+            raise ValueError(
+                'The FitnessModel requires one parameter.')
 
-        if self.min_degree:
-            # Find min degree node
-            if np.any(x0 == 0):
-                self.param = np.ones(x0.shape, dtype=np.float64)
-            else:
-                self.param = x0
-            self.expected_degrees()
-            d_out = self.exp_out_degree
-            d_in = self.exp_in_degree
-            min_out_i = np.argmin(d_out[d_out > 0])
-            min_in_i = np.argmin(d_in[d_in > 0])
-
-            def min_d(x):
-                return np.array([mt.fit_ineq_constr_alpha(
-                                    x, self.prob_fun, min_out_i,
-                                    self.out_strength[min_out_i],
-                                    self.in_strength),
-                                 mt.fit_ineq_constr_alpha(
-                                    x, self.prob_fun, min_in_i,
-                                    self.in_strength[min_in_i],
-                                    self.out_strength)
-                                 ], dtype=np.float64)
-
-            def jac_min_d(x):
-                return np.stack(
-                    (mt.fit_ineq_jac_alpha(
-                        x, self.jac_fun, min_out_i,
-                        self.out_strength[min_out_i],
-                        self.in_strength),
-                     mt.fit_ineq_jac_alpha(
-                        x, self.jac_fun, min_in_i,
-                        self.in_strength[min_in_i],
-                        self.out_strength)),
-                    axis=0)
+        if not np.issubdtype(x0.dtype, np.number):
+            raise ValueError('x0 must be numeric.')
 
-            # Solve
-            sol = mt.alpha_solver(
-                x0=x0,
-                fun=lambda x: mt.fit_eq_constr_alpha(
-                    x, self.prob_fun, self.out_strength,
-                    self.in_strength, self.num_edges),
-                jac=lambda x: mt.fit_eq_jac_alpha(
-                    x, self.jac_fun, self.out_strength,
-                    self.in_strength),
-                min_d=min_d,
-                jac_min_d=jac_min_d,
-                tol=tol,
-                max_iter=max_iter,
-                verbose=verbose,
-                full_return=True)
+        if np.any(x0 < 0):
+            raise ValueError('x0 must be positive.')
 
-        elif method == "newton":
+        if method == "newton":
             sol = mt.newton_solver(
                 x0=x0,
                 fun=lambda x: mt.fit_f_jac(
                     self.prob_fun, self.jac_fun, x,
                     self.out_strength, self.in_strength, self.num_edges),
                 tol=tol,
                 xtol=xtol,
@@ -876,33 +789,27 @@
         the total number of nodes
     num_labels: int
         the total number of labels by which the vector strengths are computed
     param: np.ndarray
         the parameters vector
     """
 
-    def __init__(self, *args, per_label=True, scale_invariant=False,
-                 min_degree=False, **kwargs):
+    def __init__(self, *args, per_label=True, **kwargs):
         """ Return a StripeFitnessModel for the given graph data.
 
         The model accepts as arguments either: a WeightedLabelGraph, the
         strength sequences (in and out) and the number of edges (per label),
         or the strength sequences and the z parameter (per label).
 
         The model accepts the strength sequences as numpy recarrays. The first
         column must contain the label index, the second column the node index
         to which the strength refers, and in the third column must have the
         value of the strength for the node label pair. All node label pairs
         not included are assumed zero.
 
-        The model defaults to the classic fitness model functional but can be
-        set to use the scale invariant formulation by setting the
-        scale_invariant flag to True. This changes the functional used for
-        the computation of the link probability but nothing else.
-
         Note that the number of edges given implicitly determines if the
         quantity preserved is the total number of edges or the number of edges
         per label. Pass only one integer for the first and a numpy array for
         the second. Note that if an array is passed then the index must be the
         same as the one in the strength sequence.
 
         """
@@ -927,17 +834,14 @@
 
             if len(args) > 1:
                 msg = ('Unnamed arguments other than the Graph have been '
                        'ignored.')
                 warnings.warn(msg, UserWarning)
 
         # Get options from keyword arguments
-        self.scale_invariant = scale_invariant
-        self.min_degree = min_degree
-
         allowed_arguments = ['num_vertices', 'num_edges', 'num_labels',
                              'out_strength', 'in_strength', 'param',
                              'discrete_weights']
         for name in kwargs:
             if name not in allowed_arguments:
                 raise ValueError('Illegal argument passed: ' + name)
             else:
@@ -1084,38 +988,26 @@
             if self.param.ndim < 2:
                 self.param = np.array([self.param])
             elif self.param.ndim > 2:
                 raise ValueError('StripeFitnessModel parameters must have '
                                  'two dimensions max.')
 
             p_shape = self.param.shape
-            if self.min_degree:
-                msg = ('StripeFitnessModel with min degree correction requires'
-                       ' two element or two rows with number of columns '
-                       'equal to the number of labels.')
-                if p_shape[0] != 2:
-                    raise ValueError(msg)
-                elif p_shape[1] == self.num_labels:
-                    self.per_label = True
-                elif p_shape[1] == 1:
-                    self.per_label = False
-                else:
-                    raise ValueError(msg)
+        
+            msg = ('StripeFitnessModel requires an array of parameters '
+                   'with number of elements equal to the number of labels '
+                   'or to one.')
+            if p_shape[0] != 1:
+                raise ValueError(msg)
+            elif p_shape[1] == self.num_labels:
+                self.per_label = True
+            elif p_shape[1] == 1:
+                self.per_label = False
             else:
-                msg = ('StripeFitnessModel requires an array of parameters '
-                       'with number of elements equal to the number of labels '
-                       'or to one.')
-                if p_shape[0] != 1:
-                    raise ValueError(msg)
-                elif p_shape[1] == self.num_labels:
-                    self.per_label = True
-                elif p_shape[1] == 1:
-                    self.per_label = False
-                else:
-                    raise ValueError(msg)
+                raise ValueError(msg)
 
             if not np.issubdtype(self.param.dtype, np.number):
                 raise ValueError('Parameters must be numeric.')
 
             if np.any(self.param < 0):
                 raise ValueError('Parameters must be positive.')
 
@@ -1130,28 +1022,16 @@
         for row in self.in_strength:
             tot_in[row.label] += row.value
 
         msg = 'Sums of strengths per label do not match.'
         assert np.allclose(tot_out, tot_in, atol=1e-14, rtol=1e-9), msg
 
         # Get the correct probability functional
-        if scale_invariant:
-            if min_degree:
-                msg = 'Cannot constrain min degree in scale invariant model.'
-                raise ValueError(msg)
-            else:
-                self.prob_fun = mt.p_invariant
-                self.jac_fun = mt.jac_invariant
-        else:
-            if min_degree:
-                self.prob_fun = mt.p_fitness_alpha
-                self.jac_fun = mt.jac_fitness_alpha
-            else:
-                self.prob_fun = mt.p_fitness
-                self.jac_fun = mt.jac_fitness
+        self.prob_fun = mt.p_fitness
+        self.jac_fun = mt.jac_fitness
 
         # If param are set computed expected number of edges per label
         if hasattr(self, 'param'):
             if self.per_label:
                 self.expected_num_edges_label()
                 self.num_edges = self.exp_num_edges_label
             else:
@@ -1176,155 +1056,68 @@
         max_iter : int or float
             maximum number of iteration
         verbose: boolean
             if true print debug info while iterating
 
         """
         if method is None:
-            if not self.min_degree:
-                method = 'newton'
-        elif self.min_degree:
-            warnings.warn('Method not recognised for solver with min degree '
-                          'constraint, using default SLSQP.', UserWarning)
-
-        if (method == 'fixed-point') and (self.scale_invariant or not
-                                          self.per_label):
-            raise Exception('Fixed point solver not supported for scale '
-                            'invariant functional or for fit not per label.')
+            method = 'newton'
+
+        if (method == 'fixed-point') and self.per_label:
+            raise Exception('Fixed point solver not supported for fit '
+                            'not per label.')
 
         # Ensure initial conditions x0 are of correct format
         if x0 is None:
             if self.per_label:
-                num_clm = self.num_labels
-            else:
-                num_clm = 1
-
-            if self.min_degree:
-                x0 = np.zeros((2, num_clm), dtype=np.float64)
-                x0[1, :] = 1
+                x0 = np.zeros((1, self.num_labels), dtype=np.float64)
             else:
-                x0 = np.zeros((1, num_clm), dtype=np.float64)
-        else:
-            if not isinstance(x0, np.ndarray):
-                try:
-                    x0 = np.array([x for x in x0])
-                except Exception:
-                    x0 = np.array([x0])
+                x0 = np.zeros((1, 1), dtype=np.float64)
+            
+        if not isinstance(x0, np.ndarray):
+            try:
+                x0 = np.array([x for x in x0])
+            except Exception:
+                x0 = np.array([x0])
 
         # Ensure that x0 has two dimensions (row 1: z, row 2: alpha,
         # each column is a layer, if single z then single column)
         if x0.ndim < 2:
             x0 = np.array([x0])
         elif x0.ndim > 2:
             raise ValueError('StripeFitnessModel x0 must have '
                              'two dimensions max.')
         p_shape = x0.shape
-        if self.min_degree:
-            msg = ('StripeFitnessModel with min degree correction requires'
-                   ' two element or two rows with number of columns '
-                   'equal to the number of labels.')
-            if p_shape[0] != 2:
-                raise ValueError(msg)
-            elif self.per_label:
-                assert p_shape[1] == self.num_labels, msg
-            else:
-                assert p_shape[1] == 1, msg
+        msg = ('StripeFitnessModel requires an array of parameters '
+               'with number of elements equal to the number of labels '
+               'or to one.')
+        if p_shape[0] != 1:
+            raise ValueError(msg)
+        elif self.per_label:
+            assert p_shape[1] == self.num_labels, msg
         else:
-            msg = ('StripeFitnessModel requires an array of parameters '
-                   'with number of elements equal to the number of labels '
-                   'or to one.')
-            if p_shape[0] != 1:
-                raise ValueError(msg)
-            elif self.per_label:
-                assert p_shape[1] == self.num_labels, msg
-            else:
-                assert p_shape[1] == 1, msg
+            assert p_shape[1] == 1, msg
 
         if not np.issubdtype(x0.dtype, np.number):
             raise ValueError('Parameters must be numeric.')
 
         if np.any(x0 < 0):
             raise ValueError('Parameters must be positive.')
 
-        if self.min_degree:
-            # Initialize param to compute min degree
-            if np.any(x0 == 0):
-                self.param = np.ones(x0.shape, dtype=np.float64)
-            else:
-                self.param = x0
-
-            if self.per_label:
-                self.expected_degrees_by_label()
-                d_out = self.exp_out_degree_label
-                d_in = self.exp_in_degree_label
-            else:
-                self.expected_degrees()
-                d_out = self.exp_out_degree
-                d_in = self.exp_in_degree
-
         # Fit by layer
         if self.per_label:
-            if self.min_degree:
-                self.param = np.empty((2, self.num_labels), dtype=np.float64)
-            else:
-                self.param = np.empty((1, self.num_labels), dtype=np.float64)
-            
+            self.param = np.empty((1, self.num_labels), dtype=np.float64)
             self.solver_output = [None]*self.num_labels
 
             for i in range(self.num_labels):
                 s_out = self.out_strength[self.out_strength.label == i]
                 s_in = self.in_strength[self.in_strength.label == i]
                 num_e = self.num_edges[i]
                 
-                if self.min_degree:
-                    # Find min degree node
-                    d_out_l = d_out[d_out.label == i]
-                    d_in_l = d_in[d_in.label == i]
-                    min_d_out = np.argmin(d_out_l.value[d_out_l.value > 0])
-                    min_d_in = np.argmin(d_in_l.value[d_in_l.value > 0])
-                    min_out_id = d_out_l[min_d_out].id
-                    min_in_id = d_in_l[min_d_in].id
-                    min_s_out = s_out[s_out.id == min_out_id].value[0]
-                    min_s_in = s_in[s_in.id == min_in_id].value[0]
-
-                    def min_d(x):
-                        return np.array([
-                            mt.layer_ineq_constr_alpha(
-                                x, self.prob_fun, min_out_id,
-                                min_s_out, s_in),
-                            mt.layer_ineq_constr_alpha(
-                                x, self.prob_fun, min_in_id,
-                                min_s_in, s_out)],
-                            dtype=np.float64)
-
-                    def jac_min_d(x):
-                        return np.stack([
-                            mt.layer_ineq_jac_alpha(
-                                x, self.jac_fun, min_out_id,
-                                min_s_out, s_in),
-                            mt.layer_ineq_jac_alpha(
-                                x, self.jac_fun, min_in_id,
-                                min_s_in, s_out)],
-                            axis=0)
-
-                    # Solve
-                    sol = mt.alpha_solver(
-                        x0=x0[:, i],
-                        fun=lambda x: mt.layer_eq_constr_alpha(
-                            x, self.prob_fun, s_out, s_in, num_e),
-                        jac=lambda x: mt.layer_eq_jac_alpha(
-                            x, self.jac_fun, s_out, s_in),
-                        min_d=min_d,
-                        jac_min_d=jac_min_d,
-                        tol=tol,
-                        max_iter=max_iter,
-                        verbose=verbose,
-                        full_return=True)
-
-                elif method == "newton":
+                if method == "newton":
                     sol = mt.newton_solver(
                         x0=x0[:, i],
                         fun=lambda x: mt.layer_f_jac(
                             self.prob_fun, self.jac_fun, x,
                             s_out, s_in, num_e),
                         tol=tol,
                         xtol=xtol,
@@ -1374,63 +1167,15 @@
             s_out_i = s_out.indptr
             s_out_j = s_out.indices
             s_out_w = s_out.data
             s_in_i = s_in.indptr
             s_in_j = s_in.indices
             s_in_w = s_in.data
                 
-            if self.min_degree:
-                # Find min degree node
-                min_out_id = np.argmin(d_out[d_out > 0])
-                min_in_id = np.argmin(d_in[d_in > 0])
-                min_out_label = s_out_j[min_out_id: min_out_id + 1]
-                min_in_label = s_in_j[min_in_id: min_in_id + 1]
-                min_out_vals = s_out_w[min_out_id: min_out_id + 1]
-                min_in_vals = s_in_w[min_in_id: min_in_id + 1]
-                
-                def min_d(x):
-                    return np.array([
-                        mt.stripe_ineq_constr_alpha(
-                            x, self.prob_fun, min_out_id, min_out_label,
-                            min_out_vals, s_in_i, s_in_j, s_in_w),
-                        mt.stripe_ineq_constr_alpha(
-                            x, self.prob_fun, min_in_id, min_in_label,
-                            min_in_vals, s_out_i, s_out_j, s_out_w)],
-                        dtype=np.float64)
-
-                def jac_min_d(x):
-                    return np.stack([
-                        mt.stripe_ineq_jac_alpha(
-                            x, self.prob_fun, self.jac_fun,
-                            min_out_id, min_out_label, min_out_vals,
-                            s_in_i, s_in_j, s_in_w),
-                        mt.stripe_ineq_jac_alpha(
-                            x, self.prob_fun, self.jac_fun,
-                            min_in_id, min_in_label, min_in_vals,
-                            s_out_i, s_out_j, s_out_w)],
-                        axis=0)
-
-                # Solve
-                sol = mt.alpha_solver(
-                    x0=x0[:, 0],
-                    fun=lambda x: mt.stripe_eq_constr_alpha(
-                        x, self.prob_fun, s_out_i, s_out_j, s_out_w,
-                        s_in_i, s_in_j, s_in_w, self.num_edges),
-                    jac=lambda x: mt.stripe_eq_jac_alpha(
-                        x, self.prob_fun, self.jac_fun,
-                        s_out_i, s_out_j, s_out_w,
-                        s_in_i, s_in_j, s_in_w),
-                    min_d=min_d,
-                    jac_min_d=jac_min_d,
-                    tol=tol,
-                    max_iter=max_iter,
-                    verbose=verbose,
-                    full_return=True)
-
-            elif method == "newton":
+            if method == "newton":
                 sol = mt.newton_solver(
                     x0=x0[:, 0],
                     fun=lambda x: mt.stripe_f_jac(
                         self.prob_fun, self.jac_fun, x,
                         s_out_i, s_out_j, s_out_w,
                         s_in_i, s_in_j, s_in_w, self.num_edges),
                     tol=tol,
@@ -1846,17 +1591,14 @@
 
     def sample(self):
         """ Return a Graph sampled from the ensemble.
         """
         if not hasattr(self, 'param'):
             raise Exception('Ensemble has to be fitted before sampling.')
 
-        if self.min_degree and not hasattr(self, 'alpha'):
-            raise Exception('Ensemble has to be fitted before sampling.')
-
         # Generate uninitialised graph object
         g = graphs.WeightedLabelGraph.__new__(graphs.WeightedLabelGraph)
         g.lv = graphs.LabelVertexList()
 
         # Initialise common object attributes
         g.num_vertices = self.num_vertices
         g.id_dtype = self.id_dtype
@@ -1890,14 +1632,928 @@
         g.total_weight = np.sum(e.weight)
         g.total_weight_label = mt.compute_tot_weight_by_label(
                 g.e, g.num_labels)
 
         return g
 
 
+class ScaleInvariantModel(GraphEnsemble):
+    """ The Scale Invariant model takes the strengths of each node in order to
+    construct a probability distribution over all possible graphs with the 
+    additional property that the parameters are consistent across all possible
+    node aggregations.
+
+    Attributes
+    ----------
+    out_strength: np.ndarray
+        the out strength sequence
+    in_strength: np.ndarray
+        the in strength sequence
+    num_edges: int
+        the total number of edges
+    num_vertices: int
+        the total number of nodes
+    z: float
+        the density parameter
+    """
+
+    def __init__(self, *args, **kwargs):
+        """ Return a FitnessModel for the given graph data.
+
+        The model accepts as arguments either: a WeightedGraph, the
+        strength sequences (in and out) and the number of edges,
+        or the strength sequences and the z parameter.
+
+        The model accepts the strength sequences as numpy recarrays. The first
+        column must contain the node index to which the strength refers and
+        in the second column there must be the value of the strength.
+        All missing node ids are assumed zero.
+
+        The model defaults to the classic fitness model functional but can be
+        set to use the scale invariant formulation by setting the
+        scale_invariant flag to True. This changes the functional used for
+        the computation of the link probability but nothing else.
+        """
+        # If an argument is passed then it must be a graph
+        if len(args) > 0:
+            if isinstance(args[0], graphs.WeightedGraph):
+                g = args[0]
+                self.num_vertices = g.num_vertices
+                self.num_edges = g.num_edges
+                self.id_dtype = g.id_dtype
+                self.out_strength = g.out_strength(get=True)
+                self.in_strength = g.in_strength(get=True)
+            else:
+                raise ValueError('First argument passed must be a '
+                                 'WeightedGraph.')
+
+            if len(args) > 1:
+                msg = ('Unnamed arguments other than the Graph have been '
+                       'ignored.')
+                warnings.warn(msg, UserWarning)
+
+        # Get options from keyword arguments
+        allowed_arguments = ['num_vertices', 'num_edges', 'out_strength',
+                             'in_strength', 'param', 'discrete_weights']
+        for name in kwargs:
+            if name not in allowed_arguments:
+                raise ValueError('Illegal argument passed: ' + name)
+            else:
+                setattr(self, name, kwargs[name])
+
+        # Ensure that all necessary fields have been set
+        if not hasattr(self, 'num_vertices'):
+            raise ValueError('Number of vertices not set.')
+        else:
+            try: 
+                assert self.num_vertices / int(self.num_vertices) == 1
+                self.num_vertices = int(self.num_vertices)
+            except Exception:
+                raise ValueError('Number of vertices must be an integer.')
+
+            if self.num_vertices <= 0:
+                raise ValueError(
+                    'Number of vertices must be a positive number.')
+
+        if not hasattr(self, 'out_strength'):
+            raise ValueError('out_strength not set.')
+
+        if not hasattr(self, 'in_strength'):
+            raise ValueError('in_strength not set.')
+
+        if not (hasattr(self, 'num_edges') or
+                hasattr(self, 'param')):
+            raise ValueError('Either num_edges or param must be set.')
+
+        if not hasattr(self, 'id_dtype'):
+            num_bytes = mt.get_num_bytes(self.num_vertices)
+            self.id_dtype = np.dtype('u' + str(num_bytes))
+
+        # Ensure that strengths passed adhere to format (ndarray)
+        msg = ("Out strength must be a numpy array of length " +
+               str(self.num_vertices))
+        assert isinstance(self.out_strength, np.ndarray), msg
+        assert self.out_strength.shape == (self.num_vertices,), msg
+
+        msg = ("In strength must be a numpy array of length " +
+               str(self.num_vertices))
+        assert isinstance(self.in_strength, np.ndarray), msg
+        assert self.in_strength.shape == (self.num_vertices,), msg
+
+        # Ensure that strengths have positive values only
+        msg = "Out strength must contain positive values only."
+        assert np.all(self.out_strength >= 0), msg
+
+        msg = "In strength must contain positive values only."
+        assert np.all(self.in_strength >= 0), msg
+
+        # Ensure that number of edges is a positive number
+        if hasattr(self, 'num_edges'):
+            try: 
+                tmp = len(self.num_edges)
+                if tmp == 1:
+                    self.num_edges = self.num_edges[0]
+                else:
+                    raise ValueError('Number of edges must be a number.')
+            except TypeError:
+                pass        
+                
+            try:
+                self.num_edges = self.num_edges * 1.0
+            except TypeError:
+                raise ValueError('Number of edges must be a number.')
+
+            if self.num_edges < 0:
+                raise ValueError(
+                    'Number of edges must be a positive number.')
+        else:
+            if not isinstance(self.param, np.ndarray):
+                self.param = np.array([self.param])
+
+            if not (len(self.param) == 1):
+                raise ValueError(
+                    'The ScaleInvariantModel requires one parameter.')
+            
+            if not np.issubdtype(self.param.dtype, np.number):
+                raise ValueError('Parameters must be numeric.')
+
+            if np.any(self.param < 0):
+                raise ValueError('Parameters must be positive.')
+
+        # Check that sum of in and out strengths are equal
+        msg = 'Sums of strengths do not match.'
+        assert np.allclose(np.sum(self.out_strength),
+                           np.sum(self.in_strength),
+                           atol=1e-14, rtol=1e-9), msg
+
+        # Get the correct probability functional
+        self.prob_fun = mt.p_invariant
+        self.jac_fun = mt.jac_invariant
+
+        # If param are set computed expected number of edges per label
+        if hasattr(self, 'param'):
+            self.num_edges = mt.fit_exp_edges(
+                self.prob_fun,
+                self.param,
+                self.out_strength,
+                self.in_strength)
+
+    def fit(self, x0=None, tol=1e-5, xtol=1e-12, max_iter=100, verbose=False):
+        """ Compute the optimal z to match the given number of edges.
+
+        Parameters
+        ----------
+        x0: float
+            optional initial conditions for parameters
+        method: 'newton' or 'fixed-point'
+            selects which method to use for the solver
+        tol : float
+            tolerance for the exit condition on the norm
+        eps : float
+            tolerance for the exit condition on difference between two
+            iterations
+        max_iter : int or float
+            maximum number of iteration
+        verbose: boolean
+            if true print debug info while iterating
+
+        """
+        
+        if x0 is None:
+            x0 = np.array([0], dtype=np.float64)
+        
+        if not isinstance(x0, np.ndarray):
+            try:
+                x0 = np.array([x for x in x0])
+            except Exception:
+                x0 = np.array([x0])
+
+        if not (len(x0) == 1):
+            raise ValueError(
+                'The ScaleInvariantModel requires one parameter.')
+
+            if not np.issubdtype(x0.dtype, np.number):
+                raise ValueError('x0 must be numeric.')
+
+            if np.any(x0 < 0):
+                raise ValueError('x0 must be positive.')
+
+        sol = mt.newton_solver(
+            x0=x0,
+            fun=lambda x: mt.fit_f_jac(
+                self.prob_fun, self.jac_fun, x,
+                self.out_strength, self.in_strength, self.num_edges),
+            tol=tol,
+            xtol=xtol,
+            max_iter=max_iter,
+            verbose=verbose,
+            full_return=True)
+
+        # Update results and check convergence
+        self.param = sol.x
+        self.solver_output = sol
+
+        if not sol.converged:
+            warnings.warn('Fit did not converge', UserWarning)
+
+    def expected_num_edges(self, get=False):
+        """ Compute the expected number of edges (per label).
+        """
+        if not hasattr(self, 'param'):
+            raise Exception('Model must be fitted before hand.')
+        
+        self.exp_num_edges = mt.fit_exp_edges(
+                self.prob_fun,
+                self.param,
+                self.out_strength,
+                self.in_strength)
+
+        if get:
+            return self.exp_num_edges
+
+    def expected_degrees(self, get=False):
+        """ Compute the expected out/in degree for a given z.
+        """
+        if not hasattr(self, 'param'):
+            raise Exception('Ensemble has to be fitted before sampling.')
+
+        self.exp_degree, self.exp_out_degree, self.exp_in_degree = \
+            mt.fit_exp_degree(self.prob_fun, self.param, self.out_strength,
+                              self.in_strength)
+
+        if get:
+            return self.exp_degree, self.exp_out_degree, self.exp_in_degree
+
+    def expected_degree(self, get=False):
+        """ Compute the expected undirected degree for a given z.
+        """
+        self.expected_degrees()
+
+        if get:
+            return self.exp_degree
+
+    def expected_out_degree(self, get=False):
+        """ Compute the expected out degree for a given z.
+        """
+        self.expected_degrees()
+
+        if get:
+            return self.exp_out_degree
+
+    def expected_in_degree(self, get=False):
+        """ Compute the expected in degree for a given z.
+        """
+        self.expected_degrees()
+        
+        if get:
+            return self.exp_in_degree
+
+    def expected_av_nn_property(self, prop, ndir='out', deg_recompute=False):
+        """ Computes the expected value of the nearest neighbour average of
+        the property array. The array must have the first dimension
+        corresponding to the vertex index.
+        """
+        # Check first dimension of property array is correct
+        if not prop.shape[0] == self.num_vertices:
+            msg = ('Property array must have first dimension size be equal to'
+                   ' the number of vertices.')
+            raise ValueError(msg)
+
+        # Compute correct expected degree
+        if deg_recompute or not hasattr(self, 'exp_out_degree'):
+            self.expected_degrees()
+
+        if ndir == 'out':
+            deg = self.exp_out_degree
+        elif ndir == 'in':
+            deg = self.exp_in_degree
+        elif ndir == 'out-in':
+            deg = self.exp_degree
+        else:
+            raise ValueError('Neighbourhood direction not recognised.')
+
+        av_nn = mt.fit_av_nn_prop(self.prob_fun, self.param, self.out_strength,
+                                  self.in_strength, prop, ndir=ndir)
+        
+        # Test that mask is the same
+        ind = deg != 0
+        msg = 'Got a av_nn for an empty neighbourhood.'
+        assert np.all(av_nn[~ind] == 0), msg
+        
+        # Average results
+        av_nn[ind] = av_nn[ind] / deg[ind]
+
+        return av_nn
+
+    def expected_av_nn_degree(self, ddir='out', ndir='out',
+                              deg_recompute=False, get=False):
+        """ Computes the expected value of the nearest neighbour average of
+        the degree.
+        """
+        # Compute correct expected degree
+        if deg_recompute or not hasattr(self, 'exp_out_degree'):
+            self.expected_degrees()
+
+        if ddir == 'out':
+            deg = self.exp_out_degree
+        elif ddir == 'in':
+            deg = self.exp_in_degree
+        elif ddir == 'out-in':
+            deg = self.exp_degree
+        else:
+            raise ValueError('Neighbourhood direction not recognised.')
+
+        # Compute property and set attribute
+        name = ('exp_av_' + ndir.replace('-', '_') + 
+                '_nn_d_' + ddir.replace('-', '_'))
+        res = self.expected_av_nn_property(deg, ndir=ndir, deg_recompute=False)
+        setattr(self, name, res)
+
+        if get:
+            return getattr(self, name)
+
+    def expected_av_nn_strength(self, sdir='out', ndir='out',
+                                deg_recompute=False, get=False):
+        """ Computes the expected value of the nearest neighbour average of
+        the strength.
+        """
+        # Select the correct strength
+        if sdir == 'out':
+            s = self.out_strength
+        elif sdir == 'in':
+            s = self.in_strength
+        elif sdir == 'out-in':
+            s = self.out_strength + self.in_strength
+        else:
+            raise ValueError('Neighbourhood direction not recognised.')
+
+        # Compute property and set attribute
+        name = ('exp_av_' + ndir.replace('-', '_') + 
+                '_nn_s_' + sdir.replace('-', '_'))
+        res = self.expected_av_nn_property(s, ndir=ndir,
+                                           deg_recompute=deg_recompute)
+        setattr(self, name, res)
+
+        if get:
+            return getattr(self, name)
+
+    def log_likelihood(self, g, log_space=True):
+        """ Compute the likelihood a graph given the fitted model.
+
+        Accepts as input either a graph or an adjacency matrix.
+        """
+        if not hasattr(self, 'param'):
+            raise Exception('Ensemble has to be fitted before.')
+
+        if isinstance(g, graphs.DirectedGraph):
+            # Extract binary adjacency matrix from graph
+            adj = g.adjacency_matrix(kind='csr')
+        elif isinstance(g, sp.spmatrix):
+            adj = g.asformat('csr')
+        elif isinstance(g, np.ndarray):
+            adj = sp.csr_matrix(g)
+        else:
+            raise ValueError('g input not a graph or adjacency matrix.')
+
+        # Ensure dimensions are correct
+        if adj.shape != (self.num_vertices, self.num_vertices):
+            msg = ('Passed graph adjacency matrix does not have the correct '
+                   'shape: {0} instead of {1}'.format(
+                    adj.shape, (self.num_vertices, self.num_vertices)))
+            raise ValueError(msg)
+
+        # Compute log likelihood of graph
+        like = mt.fit_likelihood(
+            adj.indptr, adj.indices, self.prob_fun, self.param,
+            self.out_strength, self.in_strength, log_space)
+
+        return like
+
+    def sample(self):
+        """ Return a Graph sampled from the ensemble.
+        """
+        if not hasattr(self, 'param'):
+            raise Exception('Ensemble has to be fitted before sampling.')
+
+        # Generate uninitialised graph object
+        g = graphs.WeightedGraph.__new__(graphs.WeightedGraph)
+
+        # Initialise common object attributes
+        g.num_vertices = self.num_vertices
+        g.id_dtype = self.id_dtype
+        g.v = np.arange(g.num_vertices, dtype=g.id_dtype).view(
+            type=np.recarray, dtype=[('id', g.id_dtype)])
+        g.id_dict = {}
+        for x in g.v.id:
+            g.id_dict[x] = x
+
+        # Sample edges and extract properties
+        e = mt.fit_sample(
+                self.prob_fun, self.param, self.out_strength, self.in_strength)
+
+        e = np.array(e,
+                     dtype=[('src', 'f8'),
+                            ('dst', 'f8'),
+                            ('weight', 'f8')]).view(type=np.recarray)
+
+        e = e.astype([('src', g.id_dtype),
+                      ('dst', g.id_dtype),
+                      ('weight', 'f8')])
+        g.sort_ind = np.argsort(e)
+        g.e = e[g.sort_ind]
+        g.num_edges = mt.compute_num_edges(g.e)
+        g.total_weight = np.sum(e.weight)
+
+        return g
+
+class ScaleInvariantModel_selfloops(GraphEnsemble):
+    """ The Scale Invariant model takes the strengths of each node in order to
+    construct a probability distribution over all possible graphs with the 
+    additional property that the parameters are consistent across all possible
+    node aggregations. This class includes possible self-loops.
+
+    Attributes
+    ----------
+    out_strength: np.ndarray
+        the out strength sequence
+    in_strength: np.ndarray
+        the in strength sequence
+    num_edges: int
+        the total number of edges
+    num_vertices: int
+        the total number of nodes
+    z: float
+        the density parameter
+    """
+
+    def __init__(self, *args, **kwargs):
+        """ Return a FitnessModel for the given graph data.
+
+        The model accepts as arguments either: a WeightedGraph, the
+        strength sequences (in and out) and the number of edges,
+        or the strength sequences and the z parameter.
+
+        The model accepts the strength sequences as numpy recarrays. The first
+        column must contain the node index to which the strength refers and
+        in the second column there must be the value of the strength.
+        All missing node ids are assumed zero.
+
+        The model defaults to the classic fitness model functional but can be
+        set to use the scale invariant formulation by setting the
+        scale_invariant flag to True. This changes the functional used for
+        the computation of the link probability but nothing else.
+        """
+        # If an argument is passed then it must be a graph
+        if len(args) > 0:
+            if isinstance(args[0], graphs.WeightedGraph):
+                g = args[0]
+                self.num_vertices = g.num_vertices
+                self.num_edges = g.num_edges
+                self.id_dtype = g.id_dtype
+                self.out_strength = g.out_strength(get=True)
+                self.in_strength = g.in_strength(get=True)
+            else:
+                raise ValueError('First argument passed must be a '
+                                 'WeightedGraph.')
+
+            if len(args) > 1:
+                msg = ('Unnamed arguments other than the Graph have been '
+                       'ignored.')
+                warnings.warn(msg, UserWarning)
+
+        # Get options from keyword arguments
+        allowed_arguments = ['num_vertices', 'num_edges', 'out_strength',
+                             'in_strength', 'param', 'discrete_weights']
+        for name in kwargs:
+            if name not in allowed_arguments:
+                raise ValueError('Illegal argument passed: ' + name)
+            else:
+                setattr(self, name, kwargs[name])
+
+        # Ensure that all necessary fields have been set
+        if not hasattr(self, 'num_vertices'):
+            raise ValueError('Number of vertices not set.')
+        else:
+            try: 
+                assert self.num_vertices / int(self.num_vertices) == 1
+                self.num_vertices = int(self.num_vertices)
+            except Exception:
+                raise ValueError('Number of vertices must be an integer.')
+
+            if self.num_vertices <= 0:
+                raise ValueError(
+                    'Number of vertices must be a positive number.')
+
+        if not hasattr(self, 'out_strength'):
+            raise ValueError('out_strength not set.')
+
+        if not hasattr(self, 'in_strength'):
+            raise ValueError('in_strength not set.')
+
+        if not (hasattr(self, 'num_edges') or
+                hasattr(self, 'param')):
+            raise ValueError('Either num_edges or param must be set.')
+
+        if not hasattr(self, 'id_dtype'):
+            num_bytes = mt.get_num_bytes(self.num_vertices)
+            self.id_dtype = np.dtype('u' + str(num_bytes))
+
+        # Ensure that strengths passed adhere to format (ndarray)
+        msg = ("Out strength must be a numpy array of length " +
+               str(self.num_vertices))
+        assert isinstance(self.out_strength, np.ndarray), msg
+        assert self.out_strength.shape == (self.num_vertices,), msg
+
+        msg = ("In strength must be a numpy array of length " +
+               str(self.num_vertices))
+        assert isinstance(self.in_strength, np.ndarray), msg
+        assert self.in_strength.shape == (self.num_vertices,), msg
+
+        # Ensure that strengths have positive values only
+        msg = "Out strength must contain positive values only."
+        assert np.all(self.out_strength >= 0), msg
+
+        msg = "In strength must contain positive values only."
+        assert np.all(self.in_strength >= 0), msg
+
+        # Ensure that number of edges is a positive number
+        if hasattr(self, 'num_edges'):
+            try: 
+                tmp = len(self.num_edges)
+                if tmp == 1:
+                    self.num_edges = self.num_edges[0]
+                else:
+                    raise ValueError('Number of edges must be a number.')
+            except TypeError:
+                pass        
+                
+            try:
+                self.num_edges = self.num_edges * 1.0
+            except TypeError:
+                raise ValueError('Number of edges must be a number.')
+
+            if self.num_edges < 0:
+                raise ValueError(
+                    'Number of edges must be a positive number.')
+        else:
+            if not isinstance(self.param, np.ndarray):
+                self.param = np.array([self.param])
+
+            if not (len(self.param) == 1):
+                raise ValueError(
+                    'The ScaleInvariantModel requires one parameter.')
+            
+            if not np.issubdtype(self.param.dtype, np.number):
+                raise ValueError('Parameters must be numeric.')
+
+            if np.any(self.param < 0):
+                raise ValueError('Parameters must be positive.')
+
+        # Check that sum of in and out strengths are equal
+        msg = 'Sums of strengths do not match.'
+        assert np.allclose(np.sum(self.out_strength),
+                           np.sum(self.in_strength),
+                           atol=1e-14, rtol=1e-9), msg
+
+        # Get the correct probability functional
+        self.prob_fun = mt.p_invariant
+        self.jac_fun = mt.jac_invariant
+
+        # If param are set computed expected number of edges per label
+        if hasattr(self, 'param'):
+            self.num_edges = mt.fit_exp_edges_selfloops(
+                self.prob_fun,
+                self.param,
+                self.out_strength,
+                self.in_strength)
+
+    def fit(self, x0=None, tol=1e-5, xtol=1e-12, max_iter=100, verbose=False):
+        """ Compute the optimal z to match the given number of edges.
+
+        Parameters
+        ----------
+        x0: float
+            optional initial conditions for parameters
+        method: 'newton' or 'fixed-point'
+            selects which method to use for the solver
+        tol : float
+            tolerance for the exit condition on the norm
+        eps : float
+            tolerance for the exit condition on difference between two
+            iterations
+        max_iter : int or float
+            maximum number of iteration
+        verbose: boolean
+            if true print debug info while iterating
+
+        """
+        
+        if x0 is None:
+            x0 = np.array([0], dtype=np.float64)
+        
+        if not isinstance(x0, np.ndarray):
+            try:
+                x0 = np.array([x for x in x0])
+            except Exception:
+                x0 = np.array([x0])
+
+        if not (len(x0) == 1):
+            raise ValueError(
+                'The ScaleInvariantModel requires one parameter.')
+
+            if not np.issubdtype(x0.dtype, np.number):
+                raise ValueError('x0 must be numeric.')
+
+            if np.any(x0 < 0):
+                raise ValueError('x0 must be positive.')
+            
+        #Classic newton solver
+        # sol = mt.newton_solver(
+        #     x0=x0,
+        #     fun=lambda x: mt.fit_f_jac_selfloops(
+        #         self.prob_fun, self.jac_fun, x,
+        #         self.out_strength, self.in_strength, self.num_edges),
+        #     tol=tol,
+        #     xtol=xtol,
+        #     max_iter=max_iter,
+        #     verbose=verbose,
+        #     full_return=True)
+
+        #Multiprocessing method
+        # n_nodes = self.num_vertices
+        # block_size = 10000
+        # density = 0.001
+        # target = density * n_nodes**2
+
+        # n_blocks = np.floor(n_nodes/block_size)
+        # n_blocks = n_blocks.astype(int)
+        # p_function = mt.p_invariant
+        # jac_function = mt.jac_invariant
+
+        # def jac_fit(delta, pool, n_blocks):
+        #     jobs = []
+
+        #     for i in range(n_blocks):
+        #         #Define blocks of block_size
+        #         begin_xout = i*block_size
+        #         end_xout = (i+1)*block_size
+        #         jobs.append(
+        #             pool.apply_async(mt.fit_f_jac_selfloops, 
+        #                             (p_function, jac_function, delta, self.out_strength[begin_xout:end_xout], self.in_strength))
+        #         )
+
+        #     #Add the last block with the remaining calculations to the pool
+        #     last_xout = n_blocks*block_size
+        #     jobs.append(
+        #         pool.apply_async(mt.fit_f_jac_selfloops, 
+        #                         (p_function, jac_function, delta, self.out_strength[last_xout:], self.in_strength))
+        #     )
+            
+        #     # Collect results from the workers through the pool result queue
+        #     tot_fval = -target
+        #     tot_fgrad = 0
+        #     for job in jobs:
+        #         tmp = job.get()
+        #         tot_fval += tmp[0]
+        #         tot_fgrad += tmp[1]
+            
+        #     return tot_fval, tot_fgrad
+        
+        # start=time.time()
+        # #Generate pool
+        # pool = mp.Pool(mp.cpu_count())
+        # sol = mt.newton_solver_pool(0, lambda x, y: jac_fit(x,y, n_blocks), pool, full_return=True, verbose=True)
+        # print(sol is None)
+        # pool.close()
+        # pool.join()
+
+        # Update results and check convergence
+
+        #Minimize log likelihood
+        #First calculate the constant remainder (to optimize the minimization)
+        in_out_combinations = list(product(self.out_strength, self.in_strength))
+        remainder = np.sum(in_out_combinations[i][0]*in_out_combinations[i][1] for i in range(len(in_out_combinations)))
+        sol = opt.minimize(fun = lambda x: mt.NLL(x, pairs, remainder), x0=0)
+        self.param = sol.x
+        self.solver_output = sol
+
+        if not sol.converged:
+            warnings.warn('Fit did not converge', UserWarning)
+
+    def expected_num_edges(self, get=False):
+        """ Compute the expected number of edges (per label).
+        """
+        if not hasattr(self, 'param'):
+            raise Exception('Model must be fitted before hand.')
+        
+        self.exp_num_edges = mt.fit_exp_edges_selfloops(
+                self.prob_fun,
+                self.param,
+                self.out_strength,
+                self.in_strength)
+
+        if get:
+            return self.exp_num_edges
+
+    def expected_degrees(self, get=False):
+        """ Compute the expected out/in degree for a given z.
+        """
+        if not hasattr(self, 'param'):
+            raise Exception('Ensemble has to be fitted before sampling.')
+
+        self.exp_degree, self.exp_out_degree, self.exp_in_degree = \
+            mt.fit_exp_degree(self.prob_fun, self.param, self.out_strength,
+                              self.in_strength)
+
+        if get:
+            return self.exp_degree, self.exp_out_degree, self.exp_in_degree
+
+    def expected_degree(self, get=False):
+        """ Compute the expected undirected degree for a given z.
+        """
+        self.expected_degrees()
+
+        if get:
+            return self.exp_degree
+
+    def expected_out_degree(self, get=False):
+        """ Compute the expected out degree for a given z.
+        """
+        self.expected_degrees()
+
+        if get:
+            return self.exp_out_degree
+
+    def expected_in_degree(self, get=False):
+        """ Compute the expected in degree for a given z.
+        """
+        self.expected_degrees()
+        
+        if get:
+            return self.exp_in_degree
+
+    def expected_av_nn_property(self, prop, ndir='out', deg_recompute=False):
+        """ Computes the expected value of the nearest neighbour average of
+        the property array. The array must have the first dimension
+        corresponding to the vertex index.
+        """
+        # Check first dimension of property array is correct
+        if not prop.shape[0] == self.num_vertices:
+            msg = ('Property array must have first dimension size be equal to'
+                   ' the number of vertices.')
+            raise ValueError(msg)
+
+        # Compute correct expected degree
+        if deg_recompute or not hasattr(self, 'exp_out_degree'):
+            self.expected_degrees()
+
+        if ndir == 'out':
+            deg = self.exp_out_degree
+        elif ndir == 'in':
+            deg = self.exp_in_degree
+        elif ndir == 'out-in':
+            deg = self.exp_degree
+        else:
+            raise ValueError('Neighbourhood direction not recognised.')
+
+        av_nn = mt.fit_av_nn_prop(self.prob_fun, self.param, self.out_strength,
+                                  self.in_strength, prop, ndir=ndir)
+        
+        # Test that mask is the same
+        ind = deg != 0
+        msg = 'Got a av_nn for an empty neighbourhood.'
+        assert np.all(av_nn[~ind] == 0), msg
+        
+        # Average results
+        av_nn[ind] = av_nn[ind] / deg[ind]
+
+        return av_nn
+
+    def expected_av_nn_degree(self, ddir='out', ndir='out',
+                              deg_recompute=False, get=False):
+        """ Computes the expected value of the nearest neighbour average of
+        the degree.
+        """
+        # Compute correct expected degree
+        if deg_recompute or not hasattr(self, 'exp_out_degree'):
+            self.expected_degrees()
+
+        if ddir == 'out':
+            deg = self.exp_out_degree
+        elif ddir == 'in':
+            deg = self.exp_in_degree
+        elif ddir == 'out-in':
+            deg = self.exp_degree
+        else:
+            raise ValueError('Neighbourhood direction not recognised.')
+
+        # Compute property and set attribute
+        name = ('exp_av_' + ndir.replace('-', '_') + 
+                '_nn_d_' + ddir.replace('-', '_'))
+        res = self.expected_av_nn_property(deg, ndir=ndir, deg_recompute=False)
+        setattr(self, name, res)
+
+        if get:
+            return getattr(self, name)
+
+    def expected_av_nn_strength(self, sdir='out', ndir='out',
+                                deg_recompute=False, get=False):
+        """ Computes the expected value of the nearest neighbour average of
+        the strength.
+        """
+        # Select the correct strength
+        if sdir == 'out':
+            s = self.out_strength
+        elif sdir == 'in':
+            s = self.in_strength
+        elif sdir == 'out-in':
+            s = self.out_strength + self.in_strength
+        else:
+            raise ValueError('Neighbourhood direction not recognised.')
+
+        # Compute property and set attribute
+        name = ('exp_av_' + ndir.replace('-', '_') + 
+                '_nn_s_' + sdir.replace('-', '_'))
+        res = self.expected_av_nn_property(s, ndir=ndir,
+                                           deg_recompute=deg_recompute)
+        setattr(self, name, res)
+
+        if get:
+            return getattr(self, name)
+
+    def log_likelihood(self, g, log_space=True):
+        """ Compute the likelihood a graph given the fitted model.
+
+        Accepts as input either a graph or an adjacency matrix.
+        """
+        if not hasattr(self, 'param'):
+            raise Exception('Ensemble has to be fitted before.')
+
+        if isinstance(g, graphs.DirectedGraph):
+            # Extract binary adjacency matrix from graph
+            adj = g.adjacency_matrix(kind='csr')
+        elif isinstance(g, sp.spmatrix):
+            adj = g.asformat('csr')
+        elif isinstance(g, np.ndarray):
+            adj = sp.csr_matrix(g)
+        else:
+            raise ValueError('g input not a graph or adjacency matrix.')
+
+        # Ensure dimensions are correct
+        if adj.shape != (self.num_vertices, self.num_vertices):
+            msg = ('Passed graph adjacency matrix does not have the correct '
+                   'shape: {0} instead of {1}'.format(
+                    adj.shape, (self.num_vertices, self.num_vertices)))
+            raise ValueError(msg)
+
+        # Compute log likelihood of graph
+        like = mt.fit_likelihood(
+            adj.indptr, adj.indices, self.prob_fun, self.param,
+            self.out_strength, self.in_strength, log_space)
+
+        return like
+
+    def sample(self):
+        """ Return a Graph sampled from the ensemble.
+        """
+        if not hasattr(self, 'param'):
+            raise Exception('Ensemble has to be fitted before sampling.')
+
+        # Generate uninitialised graph object
+        g = graphs.WeightedGraph.__new__(graphs.WeightedGraph)
+
+        # Initialise common object attributes
+        g.num_vertices = self.num_vertices
+        g.id_dtype = self.id_dtype
+        g.v = np.arange(g.num_vertices, dtype=g.id_dtype).view(
+            type=np.recarray, dtype=[('id', g.id_dtype)])
+        g.id_dict = {}
+        for x in g.v.id:
+            g.id_dict[x] = x
+
+        # Sample edges and extract properties
+        e = mt.fit_sample(
+                self.prob_fun, self.param, self.out_strength, self.in_strength)
+
+        e = np.array(e,
+                     dtype=[('src', 'f8'),
+                            ('dst', 'f8'),
+                            ('weight', 'f8')]).view(type=np.recarray)
+
+        e = e.astype([('src', g.id_dtype),
+                      ('dst', g.id_dtype),
+                      ('weight', 'f8')])
+        g.sort_ind = np.argsort(e)
+        g.e = e[g.sort_ind]
+        g.num_edges = mt.compute_num_edges(g.e)
+        g.total_weight = np.sum(e.weight)
+
+        return g
+
+
 class BlockFitnessModel(GraphEnsemble):
     """ A generalized fitness model that allows for grouped vertices.
 
     This model allows to take into account the group of each vertex and
     include this information as part of the model. The strength sequence is
     therefore now subdivided in strength from and to each group.
```

### Comparing `graph-ensembles-0.2.1/src/graph_ensembles.egg-info/SOURCES.txt` & `graph-ensembles-0.2.2/src/graph_ensembles.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -26,11 +26,15 @@
 src/graph_ensembles.egg-info/dependency_links.txt
 src/graph_ensembles.egg-info/requires.txt
 src/graph_ensembles.egg-info/top_level.txt
 src/graph_ensembles/methods/__init__.py
 src/graph_ensembles/methods/ensemble.py
 src/graph_ensembles/methods/graph.py
 src/graph_ensembles/methods/solver.py
+src/graph_ensembles/spark/__init__.py
+src/graph_ensembles/spark/models.py
+tests/plot_tests.py
 tests/test_block_model.py
 tests/test_fitness_model.py
+tests/test_fitness_model_multip.py
 tests/test_graph_object.py
 tests/test_stripe_model.py
```

### Comparing `graph-ensembles-0.2.1/tests/test_block_model.py` & `graph-ensembles-0.2.2/tests/test_block_model.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/tests/test_fitness_model.py` & `graph-ensembles-0.2.2/tests/test_fitness_model.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/tests/test_graph_object.py` & `graph-ensembles-0.2.2/tests/test_graph_object.py`

 * *Files identical despite different names*

### Comparing `graph-ensembles-0.2.1/tests/test_stripe_model.py` & `graph-ensembles-0.2.2/tests/test_stripe_model.py`

 * *Files identical despite different names*

