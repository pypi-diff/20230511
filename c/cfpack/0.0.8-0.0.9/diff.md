# Comparing `tmp/cfpack-0.0.8.tar.gz` & `tmp/cfpack-0.0.9.tar.gz`

## Comparing `cfpack-0.0.8.tar` & `cfpack-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.0.8/pyproject.toml.old
--rw-r--r--   0        0        0    39426 2020-02-02 00:00:00.000000 cfpack-0.0.8/cfpack/__init__.py
--rwxr-xr-x   0        0        0     5243 2020-02-02 00:00:00.000000 cfpack-0.0.8/cfpack/browser_control.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 cfpack-0.0.8/cfpack/constants.py
--rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 cfpack-0.0.8/cfpack/hdfio.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 cfpack-0.0.8/cfpack/matplotlibrc.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cfpack-0.0.8/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cfpack-0.0.8/LICENSE
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cfpack-0.0.8/README.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 cfpack-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 cfpack-0.0.9/.DS_Store
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack.browser_control.html
+-rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack.html
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.0.9/pyproject.toml.new
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.0.9/pyproject.toml.old
+-rw-r--r--   0        0        0    39571 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack/__init__.py
+-rwxr-xr-x   0        0        0     5243 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack/browser_control.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack/constants.py
+-rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack/hdfio.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack/matplotlibrc.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cfpack-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cfpack-0.0.9/LICENSE
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cfpack-0.0.9/README.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 cfpack-0.0.9/PKG-INFO
```

### Comparing `cfpack-0.0.8/pyproject.toml.old` & `cfpack-0.0.9/pyproject.toml.new`

 * *Files identical despite different names*

### Comparing `cfpack-0.0.8/cfpack/__init__.py` & `cfpack-0.0.9/cfpack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# written by Christoph Federrath, 2019-2022
+# written by Christoph Federrath, 2019-2023
 
 import numpy as np
 np.set_printoptions(linewidth=200) # increase the numpy printing linewidth a bit
 
 from . import constants as const # physical constants
 from . import matplotlibrc # set default plotting style
 
@@ -252,14 +252,21 @@
         pnames = model.param_names # parameter names (list)
         popt = ret_popt # parameter best-fit values (list)
         perr = ret_perr # parameter errors (list)
     return ret
 
 # === END fit ===
 
+# === START get_hostname ===
+def get_hostname():
+    import socket
+    hostname = socket.gethostname()
+    return hostname
+# === END get_hostname ===
+
 # === Decorator to print the runtime of the decorated function ===
 def timer_decorator(func):
     from functools import wraps
     @wraps(func)
     def timer_decorator_wrapper(*args, **kwargs):
         from time import perf_counter
         start_time = perf_counter() # start time
@@ -694,18 +701,18 @@
     return shock_jump_p(Mach,gamma) / shock_jump_rho(Mach,gamma)
 
 # return cell-centered coordinates | . | . |
 #                               xmin       xmax
 # or face-centred if keyword cell_centred=False
 def get_1d_coords(cmin=0, cmax=1, ndim=10, cell_centred=True):
     if cell_centred:
-        d = (cmax-cmin) / np.float(ndim)
+        d = (cmax-cmin) / float(ndim)
         offset = d/2
     else:
-        d = (cmax-cmin) / np.float(ndim-1)
+        d = (cmax-cmin) / float(ndim-1)
         offset = 0.0
     return np.linspace(cmin+offset, cmax-offset, num=ndim)
 
 def get_2d_coords(cmin=[0,0], cmax=[1,1], ndim=[10,10], cell_centred=True):
     cmin = np.array(cmin)
     cmax = np.array(cmax)
     ndim = np.array(ndim)
```

### Comparing `cfpack-0.0.8/cfpack/browser_control.py` & `cfpack-0.0.9/cfpack/browser_control.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.0.8/cfpack/constants.py` & `cfpack-0.0.9/cfpack/constants.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.0.8/cfpack/hdfio.py` & `cfpack-0.0.9/cfpack/hdfio.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.0.8/cfpack/matplotlibrc.py` & `cfpack-0.0.9/cfpack/matplotlibrc.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.0.8/LICENSE` & `cfpack-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cfpack-0.0.8/pyproject.toml` & `cfpack-0.0.9/pyproject.toml.old`

 * *Files identical despite different names*

### Comparing `cfpack-0.0.8/PKG-INFO` & `cfpack-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfpack
-Version: 0.0.8
+Version: 0.0.9
 Summary: Christoph Federrath (CF) python package (cfpack)
 Project-URL: Homepage, https://www.mso.anu.edu.au/~chfeder/codes/cfpack/cfpack.html
 Author-email: Christoph Federrath <christoph.federrath@anu.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Christoph Federrath
```

