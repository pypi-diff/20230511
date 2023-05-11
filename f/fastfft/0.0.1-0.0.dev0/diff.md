# Comparing `tmp/fastfft-0.0.1.tar.gz` & `tmp/fastfft-0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfft-0.0.1.tar", last modified: Thu May 11 19:09:46 2023, max compression
+gzip compressed data, was "fastfft-0.0.dev0.tar", last modified: Thu May 11 18:39:19 2023, max compression
```

## Comparing `fastfft-0.0.1.tar` & `fastfft-0.0.dev0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 19:09:46.034455 fastfft-0.0.1/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      360 2023-05-11 19:09:46.034334 fastfft-0.0.1/PKG-INFO
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       80 2023-05-11 18:18:49.000000 fastfft-0.0.1/README.md
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      107 2023-05-11 18:18:49.000000 fastfft-0.0.1/pyproject.toml
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       38 2023-05-11 19:09:46.034485 fastfft-0.0.1/setup.cfg
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1117 2023-05-11 19:09:29.000000 fastfft-0.0.1/setup.py
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 19:09:46.033044 fastfft-0.0.1/src/
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 19:09:46.034174 fastfft-0.0.1/src/fastfft.egg-info/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      360 2023-05-11 19:09:46.000000 fastfft-0.0.1/src/fastfft.egg-info/PKG-INFO
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      220 2023-05-11 19:09:46.000000 fastfft-0.0.1/src/fastfft.egg-info/SOURCES.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-11 19:09:46.000000 fastfft-0.0.1/src/fastfft.egg-info/dependency_links.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        7 2023-05-11 19:09:46.000000 fastfft-0.0.1/src/fastfft.egg-info/requires.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       10 2023-05-11 19:09:46.000000 fastfft-0.0.1/src/fastfft.egg-info/top_level.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)   222574 2023-05-11 18:24:10.000000 fastfft-0.0.1/src/main.cpp
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 18:39:19.449171 fastfft-0.0.dev0/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      340 2023-05-11 18:39:19.449000 fastfft-0.0.dev0/PKG-INFO
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       80 2023-05-11 18:18:49.000000 fastfft-0.0.dev0/README.md
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      107 2023-05-11 18:18:49.000000 fastfft-0.0.dev0/pyproject.toml
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       38 2023-05-11 18:39:19.449216 fastfft-0.0.dev0/setup.cfg
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1110 2023-05-11 18:24:07.000000 fastfft-0.0.dev0/setup.py
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 18:39:19.445222 fastfft-0.0.dev0/src/
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 18:39:19.448792 fastfft-0.0.dev0/src/fastfft.egg-info/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      340 2023-05-11 18:39:19.000000 fastfft-0.0.dev0/src/fastfft.egg-info/PKG-INFO
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      220 2023-05-11 18:39:19.000000 fastfft-0.0.dev0/src/fastfft.egg-info/SOURCES.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-11 18:39:19.000000 fastfft-0.0.dev0/src/fastfft.egg-info/dependency_links.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        7 2023-05-11 18:39:19.000000 fastfft-0.0.dev0/src/fastfft.egg-info/requires.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       10 2023-05-11 18:39:19.000000 fastfft-0.0.dev0/src/fastfft.egg-info/top_level.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)   222574 2023-05-11 18:24:10.000000 fastfft-0.0.dev0/src/main.cpp
```

### Comparing `fastfft-0.0.1/setup.py` & `fastfft-0.0.dev0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from setuptools import find_packages, setup, Extension
 from Cython.Build import cythonize
+import numpy as np
 import os
 import json
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 
@@ -19,18 +20,17 @@
     Extension("maxim_fft",
               sources=["src/main.pyx"],
               )
 ]
 
 setup(
     name="fastfft",
-    version="0.0.1",
+    version="0.0.dev0",
     package_dir={'': 'src'},
     packages=find_packages('src'),
-    python_requires='>=3.8',
     author="Maxim Movshin",
     description="Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/BSaaber/fastfft",
     ext_modules=cythonize(ext_modules),
     install_requires=[
```

### Comparing `fastfft-0.0.1/src/main.cpp` & `fastfft-0.0.dev0/src/main.cpp`

 * *Files identical despite different names*

