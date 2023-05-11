# Comparing `tmp/pawflim-1.0.1.tar.gz` & `tmp/pawflim-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pawflim-1.0.1.tar", last modified: Tue May  9 19:18:00 2023, max compression
+gzip compressed data, was "pawflim-1.0.2.tar", last modified: Thu May 11 00:05:23 2023, max compression
```

## Comparing `pawflim-1.0.1.tar` & `pawflim-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:00.273449 pawflim-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:00.265449 pawflim-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:00.269449 pawflim-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-09 19:17:47.000000 pawflim-1.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-09 19:17:47.000000 pawflim-1.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 19:17:47.000000 pawflim-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-09 19:18:00.273449 pawflim-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-09 19:17:47.000000 pawflim-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:00.269449 pawflim-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   153455 2023-05-09 19:17:47.000000 pawflim-1.0.1/examples/simulated_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-09 19:17:47.000000 pawflim-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 19:17:47.000000 pawflim-1.0.1/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 19:17:47.000000 pawflim-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:18:00.273449 pawflim-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:00.273449 pawflim-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:00.273449 pawflim-1.0.1/src/pawflim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-09 19:18:00.000000 pawflim-1.0.1/src/pawflim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-09 19:18:00.000000 pawflim-1.0.1/src/pawflim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:18:00.000000 pawflim-1.0.1/src/pawflim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 19:18:00.000000 pawflim-1.0.1/src/pawflim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:18:00.000000 pawflim-1.0.1/src/pawflim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-09 19:17:47.000000 pawflim-1.0.1/src/pawflim.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-09 19:17:47.000000 pawflim-1.0.1/src/test_pawflim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:05:23.246965 pawflim-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:05:23.242965 pawflim-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:05:23.242965 pawflim-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-11 00:05:07.000000 pawflim-1.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-11 00:05:07.000000 pawflim-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-11 00:05:07.000000 pawflim-1.0.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 00:05:07.000000 pawflim-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-11 00:05:23.246965 pawflim-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-11 00:05:07.000000 pawflim-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:05:23.242965 pawflim-1.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   153455 2023-05-11 00:05:07.000000 pawflim-1.0.2/examples/simulated_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-11 00:05:07.000000 pawflim-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 00:05:07.000000 pawflim-1.0.2/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 00:05:07.000000 pawflim-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 00:05:23.246965 pawflim-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:05:23.242965 pawflim-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:05:23.246965 pawflim-1.0.2/src/pawflim/
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-11 00:05:07.000000 pawflim-1.0.2/src/pawflim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:05:23.246965 pawflim-1.0.2/src/pawflim/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-11 00:05:07.000000 pawflim-1.0.2/src/pawflim/tests/test_pawflim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:05:23.246965 pawflim-1.0.2/src/pawflim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-11 00:05:23.000000 pawflim-1.0.2/src/pawflim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-11 00:05:23.000000 pawflim-1.0.2/src/pawflim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:05:23.000000 pawflim-1.0.2/src/pawflim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 00:05:23.000000 pawflim-1.0.2/src/pawflim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 00:05:23.000000 pawflim-1.0.2/src/pawflim.egg-info/top_level.txt
```

### Comparing `pawflim-1.0.1/.github/workflows/test.yml` & `pawflim-1.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pawflim-1.0.1/LICENSE` & `pawflim-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pawflim-1.0.1/PKG-INFO` & `pawflim-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawflim
-Version: 1.0.1
+Version: 1.0.2
 Summary: Denoising via adaptive binning for FLIM datasets.
 Author-email: Mauro Silberberg <maurosilber@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mauro Silberberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pawflim-1.0.1/README.md` & `pawflim-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pawflim-1.0.1/examples/simulated_data.ipynb` & `pawflim-1.0.2/examples/simulated_data.ipynb`

 * *Files identical despite different names*

### Comparing `pawflim-1.0.1/pyproject.toml` & `pawflim-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pawflim-1.0.1/src/pawflim.egg-info/PKG-INFO` & `pawflim-1.0.2/src/pawflim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawflim
-Version: 1.0.1
+Version: 1.0.2
 Summary: Denoising via adaptive binning for FLIM datasets.
 Author-email: Mauro Silberberg <maurosilber@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mauro Silberberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pawflim-1.0.1/src/pawflim.py` & `pawflim-1.0.2/src/pawflim/__init__.py`

 * *Files identical despite different names*

### Comparing `pawflim-1.0.1/src/test_pawflim.py` & `pawflim-1.0.2/src/pawflim/tests/test_pawflim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import hypothesis
 import hypothesis.extra.numpy as st_np
 import hypothesis.strategies as st
 import numpy as np
 
-from .pawflim import _inverse
+from .. import _inverse
 
 
 def invertible(x: np.ndarray) -> bool:
     det = np.linalg.det(x)
     if np.isclose(det, 0) or not np.isfinite(det):
         return False
     else:
```

