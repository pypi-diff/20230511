# Comparing `tmp/fastfft-0.0.dev0.tar.gz` & `tmp/fastfft-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfft-0.0.dev0.tar", last modified: Thu May 11 18:39:19 2023, max compression
+gzip compressed data, was "fastfft-0.1.0.tar", last modified: Thu May 11 19:37:18 2023, max compression
```

## Comparing `fastfft-0.0.dev0.tar` & `fastfft-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 18:39:19.449171 fastfft-0.0.dev0/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      340 2023-05-11 18:39:19.449000 fastfft-0.0.dev0/PKG-INFO
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       80 2023-05-11 18:18:49.000000 fastfft-0.0.dev0/README.md
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      107 2023-05-11 18:18:49.000000 fastfft-0.0.dev0/pyproject.toml
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       38 2023-05-11 18:39:19.449216 fastfft-0.0.dev0/setup.cfg
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1110 2023-05-11 18:24:07.000000 fastfft-0.0.dev0/setup.py
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 18:39:19.445222 fastfft-0.0.dev0/src/
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 18:39:19.448792 fastfft-0.0.dev0/src/fastfft.egg-info/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      340 2023-05-11 18:39:19.000000 fastfft-0.0.dev0/src/fastfft.egg-info/PKG-INFO
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      220 2023-05-11 18:39:19.000000 fastfft-0.0.dev0/src/fastfft.egg-info/SOURCES.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-11 18:39:19.000000 fastfft-0.0.dev0/src/fastfft.egg-info/dependency_links.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        7 2023-05-11 18:39:19.000000 fastfft-0.0.dev0/src/fastfft.egg-info/requires.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       10 2023-05-11 18:39:19.000000 fastfft-0.0.dev0/src/fastfft.egg-info/top_level.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)   222574 2023-05-11 18:24:10.000000 fastfft-0.0.dev0/src/main.cpp
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 19:37:18.607914 fastfft-0.1.0/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      360 2023-05-11 19:37:18.607785 fastfft-0.1.0/PKG-INFO
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       80 2023-05-11 18:18:49.000000 fastfft-0.1.0/README.md
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 19:37:18.607369 fastfft-0.1.0/fastfft.egg-info/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      360 2023-05-11 19:37:18.000000 fastfft-0.1.0/fastfft.egg-info/PKG-INFO
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      200 2023-05-11 19:37:18.000000 fastfft-0.1.0/fastfft.egg-info/SOURCES.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-11 19:37:18.000000 fastfft-0.1.0/fastfft.egg-info/dependency_links.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       13 2023-05-11 19:37:18.000000 fastfft-0.1.0/fastfft.egg-info/requires.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       10 2023-05-11 19:37:18.000000 fastfft-0.1.0/fastfft.egg-info/top_level.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      124 2023-05-11 19:31:57.000000 fastfft-0.1.0/pyproject.toml
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       38 2023-05-11 19:37:18.607950 fastfft-0.1.0/setup.cfg
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1177 2023-05-11 19:35:52.000000 fastfft-0.1.0/setup.py
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 19:37:18.607477 fastfft-0.1.0/src/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)   222574 2023-05-11 19:37:18.000000 fastfft-0.1.0/src/main.cpp
```

### Comparing `fastfft-0.0.dev0/setup.py` & `fastfft-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup, Extension
 from Cython.Build import cythonize
-import numpy as np
 import os
 import json
+import numpy as np
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 
 def read_pipenv_dependencies(fname):
     """Get from Pipfile.lock default dependencies."""
@@ -20,20 +20,22 @@
     Extension("maxim_fft",
               sources=["src/main.pyx"],
               )
 ]
 
 setup(
     name="fastfft",
-    version="0.0.dev0",
-    package_dir={'': 'src'},
-    packages=find_packages('src'),
+    setup_requires=["cython", "numpy"],
+    version="0.1.0",
+    packages=find_packages(),
+    python_requires='>=3.8',
     author="Maxim Movshin",
     description="Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/BSaaber/fastfft",
     ext_modules=cythonize(ext_modules),
+    include_dirs=np.get_include(),
     install_requires=[
         *read_pipenv_dependencies('Pipfile.lock'),
     ]
 )
```

### Comparing `fastfft-0.0.dev0/src/main.cpp` & `fastfft-0.1.0/src/main.cpp`

 * *Files identical despite different names*

