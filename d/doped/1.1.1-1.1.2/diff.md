# Comparing `tmp/doped-1.1.1.tar.gz` & `tmp/doped-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doped-1.1.1.tar", last modified: Tue May  9 23:32:05 2023, max compression
+gzip compressed data, was "doped-1.1.2.tar", last modified: Thu May 11 12:53:33 2023, max compression
```

## Comparing `doped-1.1.1.tar` & `doped-1.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.483678 doped-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 22:47:19.000000 doped-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-05-09 23:32:05.483678 doped-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-05-09 22:47:19.000000 doped-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.471678 doped-1.1.1/doped/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-09 22:47:19.000000 doped-1.1.1/doped/DefectSet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-09 22:47:19.000000 doped-1.1.1/doped/HSE06_RelaxSet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-09 22:47:19.000000 doped-1.1.1/doped/PBEsol_ConvergenceSet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-09 22:47:19.000000 doped-1.1.1/doped/PotcarSet.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2476 2023-05-09 22:47:19.000000 doped-1.1.1/doped/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    41977 2023-05-09 22:47:19.000000 doped-1.1.1/doped/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    71417 2023-05-09 22:47:19.000000 doped-1.1.1/doped/chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-05-09 22:47:19.000000 doped-1.1.1/doped/corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    35271 2023-05-09 22:47:19.000000 doped-1.1.1/doped/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.471678 doped-1.1.1/doped/pycdt/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.475678 doped-1.1.1/doped/pycdt/core/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47141 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/core/_chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    43829 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/core/defectsmaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.475678 doped-1.1.1/doped/pycdt/core/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/core/tests/test_chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/core/tests/test_defectsmaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.479678 doped-1.1.1/doped/pycdt/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53328 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/parse_calculations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.479678 doped-1.1.1/doped/pycdt/utils/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/tests/test_parse_calculations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/tests/test_vasp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/vasp.py
--rw-r--r--   0 runner    (1001) docker     (123)    40542 2023-05-09 22:47:19.000000 doped-1.1.1/doped/vasp_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.471678 doped-1.1.1/doped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-05-09 23:32:05.000000 doped-1.1.1/doped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-09 23:32:05.000000 doped-1.1.1/doped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:32:05.000000 doped-1.1.1/doped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 23:32:05.000000 doped-1.1.1/doped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 23:32:05.000000 doped-1.1.1/doped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-09 22:47:21.000000 doped-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 23:32:05.483678 doped-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.483678 doped-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    39969 2023-05-09 22:47:21.000000 doped-1.1.1/tests/test_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25523 2023-05-09 22:47:21.000000 doped-1.1.1/tests/test_chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-09 22:47:21.000000 doped-1.1.1/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-05-09 22:47:21.000000 doped-1.1.1/tests/test_vasp_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:53:33.087875 doped-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 12:13:52.000000 doped-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-11 12:53:33.083875 doped-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-11 12:13:52.000000 doped-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:53:33.075875 doped-1.1.2/doped/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-11 12:13:52.000000 doped-1.1.2/doped/DefectSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-11 12:13:52.000000 doped-1.1.2/doped/HSE06_RelaxSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-11 12:13:52.000000 doped-1.1.2/doped/PBEsol_ConvergenceSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-11 12:13:52.000000 doped-1.1.2/doped/PotcarSet.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2476 2023-05-11 12:13:52.000000 doped-1.1.2/doped/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41977 2023-05-11 12:13:52.000000 doped-1.1.2/doped/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71417 2023-05-11 12:13:52.000000 doped-1.1.2/doped/chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-05-11 12:13:52.000000 doped-1.1.2/doped/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35271 2023-05-11 12:13:52.000000 doped-1.1.2/doped/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:53:33.079875 doped-1.1.2/doped/pycdt/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:53:33.079875 doped-1.1.2/doped/pycdt/core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47141 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/core/_chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43829 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/core/defectsmaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:53:33.079875 doped-1.1.2/doped/pycdt/core/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/core/tests/test_chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/core/tests/test_defectsmaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:53:33.083875 doped-1.1.2/doped/pycdt/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53328 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/utils/parse_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/utils/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:53:33.083875 doped-1.1.2/doped/pycdt/utils/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/utils/tests/test_parse_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/utils/tests/test_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-05-11 12:13:52.000000 doped-1.1.2/doped/pycdt/utils/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40542 2023-05-11 12:13:52.000000 doped-1.1.2/doped/vasp_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:53:33.079875 doped-1.1.2/doped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-11 12:53:33.000000 doped-1.1.2/doped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-11 12:53:33.000000 doped-1.1.2/doped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:53:33.000000 doped-1.1.2/doped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-11 12:53:33.000000 doped-1.1.2/doped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 12:53:33.000000 doped-1.1.2/doped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-11 12:13:54.000000 doped-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:53:33.087875 doped-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:53:33.083875 doped-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    39969 2023-05-11 12:13:54.000000 doped-1.1.2/tests/test_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25523 2023-05-11 12:13:54.000000 doped-1.1.2/tests/test_chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-11 12:13:54.000000 doped-1.1.2/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-05-11 12:13:54.000000 doped-1.1.2/tests/test_vasp_input.py
```

### Comparing `doped-1.1.1/LICENSE` & `doped-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/PKG-INFO` & `doped-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doped
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python package to setup, process and analyse solid-state defect calculations with VASP
 Author-email: Seán Kavanagh <sean.kavanagh.19@ucl.ac.uk>
 License: MIT License
         
         Copyright (c) 2021 Seán Kavanagh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -72,15 +72,15 @@
 As such, it is recommended to install `doped` in a virtual python environment as follows:
 
 1. Create virtual environment and install: 
 ```bash
 conda create -n doped python=3.10  # create conda environment named doped
 conda activate doped  # activate doped conda environment
 pip install doped  # install doped and dependencies, can also  
-pip install numpy --upgrade # upgrade numpy to avoid binary incompatibility
+pip install --force --no-cache-dir numpy==1.23 # install numpy after doped to avoid binary incompatibility
 ```
 And then use this environment whenever using `doped`.
 Alternatively if desired, `doped` can also be installed from `conda` with:
 
 ```bash
   conda install -c conda-forge doped
 ```
```

### Comparing `doped-1.1.1/README.md` & `doped-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 As such, it is recommended to install `doped` in a virtual python environment as follows:
 
 1. Create virtual environment and install: 
 ```bash
 conda create -n doped python=3.10  # create conda environment named doped
 conda activate doped  # activate doped conda environment
 pip install doped  # install doped and dependencies, can also  
-pip install numpy --upgrade # upgrade numpy to avoid binary incompatibility
+pip install --force --no-cache-dir numpy==1.23 # install numpy after doped to avoid binary incompatibility
 ```
 And then use this environment whenever using `doped`.
 Alternatively if desired, `doped` can also be installed from `conda` with:
 
 ```bash
   conda install -c conda-forge doped
 ```
```

### Comparing `doped-1.1.1/doped/DefectSet.yaml` & `doped-1.1.2/doped/DefectSet.yaml`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/PotcarSet.yaml` & `doped-1.1.2/doped/PotcarSet.yaml`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/__init__.py` & `doped-1.1.2/doped/__init__.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/analysis.py` & `doped-1.1.2/doped/analysis.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/chemical_potentials.py` & `doped-1.1.2/doped/chemical_potentials.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/corrections.py` & `doped-1.1.2/doped/corrections.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/plotting.py` & `doped-1.1.2/doped/plotting.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/pycdt/core/_chemical_potentials.py` & `doped-1.1.2/doped/pycdt/core/_chemical_potentials.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/pycdt/core/defectsmaker.py` & `doped-1.1.2/doped/pycdt/core/defectsmaker.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/pycdt/core/tests/test_chemical_potentials.py` & `doped-1.1.2/doped/pycdt/core/tests/test_chemical_potentials.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/pycdt/core/tests/test_defectsmaker.py` & `doped-1.1.2/doped/pycdt/core/tests/test_defectsmaker.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/pycdt/utils/parse_calculations.py` & `doped-1.1.2/doped/pycdt/utils/parse_calculations.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/pycdt/utils/plotter.py` & `doped-1.1.2/doped/pycdt/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/pycdt/utils/tests/test_parse_calculations.py` & `doped-1.1.2/doped/pycdt/utils/tests/test_parse_calculations.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/pycdt/utils/tests/test_vasp.py` & `doped-1.1.2/doped/pycdt/utils/tests/test_vasp.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/pycdt/utils/vasp.py` & `doped-1.1.2/doped/pycdt/utils/vasp.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped/vasp_input.py` & `doped-1.1.2/doped/vasp_input.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/doped.egg-info/PKG-INFO` & `doped-1.1.2/doped.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doped
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python package to setup, process and analyse solid-state defect calculations with VASP
 Author-email: Seán Kavanagh <sean.kavanagh.19@ucl.ac.uk>
 License: MIT License
         
         Copyright (c) 2021 Seán Kavanagh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -72,15 +72,15 @@
 As such, it is recommended to install `doped` in a virtual python environment as follows:
 
 1. Create virtual environment and install: 
 ```bash
 conda create -n doped python=3.10  # create conda environment named doped
 conda activate doped  # activate doped conda environment
 pip install doped  # install doped and dependencies, can also  
-pip install numpy --upgrade # upgrade numpy to avoid binary incompatibility
+pip install --force --no-cache-dir numpy==1.23 # install numpy after doped to avoid binary incompatibility
 ```
 And then use this environment whenever using `doped`.
 Alternatively if desired, `doped` can also be installed from `conda` with:
 
 ```bash
   conda install -c conda-forge doped
 ```
```

### Comparing `doped-1.1.1/doped.egg-info/SOURCES.txt` & `doped-1.1.2/doped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/pyproject.toml` & `doped-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "doped"
-version = "1.1.1"
+version = "1.1.2"
 description = "Python package to setup, process and analyse solid-state defect calculations with VASP"
 authors = [{name = "Seán Kavanagh", email = "sean.kavanagh.19@ucl.ac.uk"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -17,15 +17,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     ]
 requires-python = ">=3.7, <3.11"  # current pymatgen version <2022.8.23 incompatible with python 3.11
 dependencies = [
     "ase",
     "tabulate",
     "matplotlib",
-    "numpy>=1.21.0",
+    "numpy>=1.21.0,<1.24.0",
     "pymatgen<2022.8.23",
     "shakenbreak==22.11.1",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/SMTG-UCL/doped"
```

### Comparing `doped-1.1.1/tests/test_analysis.py` & `doped-1.1.2/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/tests/test_chemical_potentials.py` & `doped-1.1.2/tests/test_chemical_potentials.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/tests/test_corrections.py` & `doped-1.1.2/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.1/tests/test_vasp_input.py` & `doped-1.1.2/tests/test_vasp_input.py`

 * *Files identical despite different names*

