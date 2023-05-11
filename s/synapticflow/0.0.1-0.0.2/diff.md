# Comparing `tmp/synapticflow-0.0.1.tar.gz` & `tmp/synapticflow-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapticflow-0.0.1.tar", max compression
+gzip compressed data, was "synapticflow-0.0.2.tar", max compression
```

## Comparing `synapticflow-0.0.1.tar` & `synapticflow-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    35149 2023-03-27 09:01:56.624062 synapticflow-0.0.1/LICENSE
--rw-r--r--   0        0        0     3224 2023-04-10 04:18:10.075412 synapticflow-0.0.1/README.md
--rw-r--r--   0        0        0     1202 2023-04-10 07:13:40.787549 synapticflow-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-07 12:54:46.443837 synapticflow-0.0.1/synapticflow/.DS_Store
--rw-r--r--   0        0        0      894 2023-04-10 07:13:15.224098 synapticflow-0.0.1/synapticflow/__init__.py
--rw-r--r--   0        0        0      888 2023-04-09 16:26:03.907966 synapticflow-0.0.1/synapticflow/network/__init__.py
--rw-r--r--   0        0        0      651 2023-04-09 16:31:19.669191 synapticflow-0.0.1/synapticflow/network/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    60989 2023-04-10 04:13:39.844147 synapticflow-0.0.1/synapticflow/network/__pycache__/neural_populations.cpython-39.pyc
--rw-r--r--   0        0        0    87884 2023-04-10 03:54:27.580176 synapticflow-0.0.1/synapticflow/network/neural_populations.py
--rw-r--r--   0        0        0      776 2023-04-07 14:45:50.487754 synapticflow-0.0.1/synapticflow/plotting/__init__.py
--rw-r--r--   0        0        0      649 2023-04-09 16:34:08.316076 synapticflow-0.0.1/synapticflow/plotting/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    16708 2023-04-10 04:13:42.214184 synapticflow-0.0.1/synapticflow/plotting/__pycache__/visualization.cpython-39.pyc
--rw-r--r--   0        0        0    16715 2023-04-10 03:52:43.853966 synapticflow-0.0.1/synapticflow/plotting/visualization.py
--rw-r--r--   0        0        0     4377 1970-01-01 00:00:00.000000 synapticflow-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-27 09:01:56.624062 synapticflow-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3224 2023-04-10 04:18:10.075412 synapticflow-0.0.2/README.md
+-rw-r--r--   0        0        0     1202 2023-05-11 01:31:07.115029 synapticflow-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-11 01:13:36.467467 synapticflow-0.0.2/synapticflow/.DS_Store
+-rw-r--r--   0        0        0      967 2023-05-11 01:31:13.044893 synapticflow-0.0.2/synapticflow/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-11 01:16:12.645161 synapticflow-0.0.2/synapticflow/network/__init__.py
+-rw-r--r--   0        0        0      651 2023-04-09 16:31:19.669191 synapticflow-0.0.2/synapticflow/network/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    60989 2023-04-10 04:13:39.844147 synapticflow-0.0.2/synapticflow/network/__pycache__/neural_populations.cpython-39.pyc
+-rw-r--r--   0        0        0     8041 2023-05-11 01:16:31.982145 synapticflow-0.0.2/synapticflow/network/connections.py
+-rw-r--r--   0        0        0    87884 2023-04-10 03:54:27.580176 synapticflow-0.0.2/synapticflow/network/neural_populations.py
+-rw-r--r--   0        0        0      776 2023-04-07 14:45:50.487754 synapticflow-0.0.2/synapticflow/plotting/__init__.py
+-rw-r--r--   0        0        0      649 2023-04-09 16:34:08.316076 synapticflow-0.0.2/synapticflow/plotting/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    16708 2023-04-10 04:13:42.214184 synapticflow-0.0.2/synapticflow/plotting/__pycache__/visualization.cpython-39.pyc
+-rw-r--r--   0        0        0    16715 2023-04-10 03:52:43.853966 synapticflow-0.0.2/synapticflow/plotting/visualization.py
+-rw-r--r--   0        0        0     4377 1970-01-01 00:00:00.000000 synapticflow-0.0.2/PKG-INFO
```

### Comparing `synapticflow-0.0.1/LICENSE` & `synapticflow-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.1/README.md` & `synapticflow-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.1/pyproject.toml` & `synapticflow-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "synapticflow"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     "Arsham Gholamzadeh Khoee <arsham.gh97@gmail.com>",
     "Mobin Nesari <mobinnesari81@gmail.com>",
     "Mohammad Mehdi Begmaz <mohammadmehdi.begmaz@gmail.com>",
     "Negar Sourati <negarsourati@gmail.com>"
 ]
 maintainers =[
```

### Comparing `synapticflow-0.0.1/synapticflow/__init__.py` & `synapticflow-0.0.2/synapticflow/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,8 +20,11 @@
 from .plotting import raster_plot
 from .plotting import plot_weights
 from .plotting import plot_potential
 from .plotting import plot_refractory_count
 from .plotting import plot_neuron
 from .plotting import plot_periodic
 
-__version__ = 'V0.0.1'
+from .network import AbstractConnection
+from .network import Connection
+
+__version__ = 'V0.0.2'
```

### Comparing `synapticflow-0.0.1/synapticflow/network/__init__.py` & `synapticflow-0.0.2/synapticflow/network/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,8 +20,11 @@
 from .neural_populations import BLIFPopulation
 from .neural_populations import ALIFPopulation
 from .neural_populations import ELIFPopulation
 from .neural_populations import QLIFPopulation
 from .neural_populations import AELIFPopulation
 from .neural_populations import AQLIFPopulation
 from .neural_populations import CLIFPopulation
-from .neural_populations import SRM0Node
+from .neural_populations import SRM0Node
+
+from .connections import AbstractConnection
+from .connections import Connection
```

### Comparing `synapticflow-0.0.1/synapticflow/network/__pycache__/__init__.cpython-39.pyc` & `synapticflow-0.0.2/synapticflow/network/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.1/synapticflow/network/__pycache__/neural_populations.cpython-39.pyc` & `synapticflow-0.0.2/synapticflow/network/__pycache__/neural_populations.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.1/synapticflow/network/neural_populations.py` & `synapticflow-0.0.2/synapticflow/network/neural_populations.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.1/synapticflow/plotting/__init__.py` & `synapticflow-0.0.2/synapticflow/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.1/synapticflow/plotting/__pycache__/__init__.cpython-39.pyc` & `synapticflow-0.0.2/synapticflow/plotting/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.1/synapticflow/plotting/__pycache__/visualization.cpython-39.pyc` & `synapticflow-0.0.2/synapticflow/plotting/__pycache__/visualization.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.1/synapticflow/plotting/visualization.py` & `synapticflow-0.0.2/synapticflow/plotting/visualization.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.1/PKG-INFO` & `synapticflow-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapticflow
-Version: 0.0.1
+Version: 0.0.2
 Summary: A powerful Python package for simulating spiking neural networks (SNNs) using PyTorch with GPU acceleration.
 Keywords: Delay Learning,RSTDP,STDP,Spiking Neural Network (SNN)
 Author: Arsham Gholamzadeh Khoee
 Author-email: arsham.gh97@gmail.com
 Maintainer: Arsham Gholamzadeh Khoee
 Maintainer-email: arsham.gh97@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: synapticflow Version: 0.0.1 Summary: A powerful
+Metadata-Version: 2.1 Name: synapticflow Version: 0.0.2 Summary: A powerful
 Python package for simulating spiking neural networks (SNNs) using PyTorch with
 GPU acceleration. Keywords: Delay Learning,RSTDP,STDP,Spiking Neural Network
 (SNN) Author: Arsham Gholamzadeh Khoee Author-email: arsham.gh97@gmail.com
 Maintainer: Arsham Gholamzadeh Khoee Maintainer-email: arsham.gh97@gmail.com
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 2 Classifier:
 Programming Language :: Python :: 2.7 Classifier: Programming Language ::
```

