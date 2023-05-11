# Comparing `tmp/fastfft-0.1.0.tar.gz` & `tmp/fastfft-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfft-0.1.0.tar", last modified: Thu May 11 19:37:18 2023, max compression
+gzip compressed data, was "fastfft-0.1.1.tar", last modified: Thu May 11 19:54:19 2023, max compression
```

## Comparing `fastfft-0.1.0.tar` & `fastfft-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 19:37:18.607914 fastfft-0.1.0/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      360 2023-05-11 19:37:18.607785 fastfft-0.1.0/PKG-INFO
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       80 2023-05-11 18:18:49.000000 fastfft-0.1.0/README.md
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 19:37:18.607369 fastfft-0.1.0/fastfft.egg-info/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      360 2023-05-11 19:37:18.000000 fastfft-0.1.0/fastfft.egg-info/PKG-INFO
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      200 2023-05-11 19:37:18.000000 fastfft-0.1.0/fastfft.egg-info/SOURCES.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-11 19:37:18.000000 fastfft-0.1.0/fastfft.egg-info/dependency_links.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       13 2023-05-11 19:37:18.000000 fastfft-0.1.0/fastfft.egg-info/requires.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       10 2023-05-11 19:37:18.000000 fastfft-0.1.0/fastfft.egg-info/top_level.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      124 2023-05-11 19:31:57.000000 fastfft-0.1.0/pyproject.toml
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       38 2023-05-11 19:37:18.607950 fastfft-0.1.0/setup.cfg
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1177 2023-05-11 19:35:52.000000 fastfft-0.1.0/setup.py
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 19:37:18.607477 fastfft-0.1.0/src/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)   222574 2023-05-11 19:37:18.000000 fastfft-0.1.0/src/main.cpp
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 19:54:19.036476 fastfft-0.1.1/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      360 2023-05-11 19:54:19.036345 fastfft-0.1.1/PKG-INFO
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       80 2023-05-11 18:18:49.000000 fastfft-0.1.1/README.md
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 19:54:19.035989 fastfft-0.1.1/fastfft.egg-info/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      360 2023-05-11 19:54:19.000000 fastfft-0.1.1/fastfft.egg-info/PKG-INFO
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      202 2023-05-11 19:54:19.000000 fastfft-0.1.1/fastfft.egg-info/SOURCES.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-11 19:54:19.000000 fastfft-0.1.1/fastfft.egg-info/dependency_links.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       13 2023-05-11 19:54:19.000000 fastfft-0.1.1/fastfft.egg-info/requires.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       10 2023-05-11 19:54:19.000000 fastfft-0.1.1/fastfft.egg-info/top_level.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      124 2023-05-11 19:31:57.000000 fastfft-0.1.1/pyproject.toml
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       38 2023-05-11 19:54:19.036510 fastfft-0.1.1/setup.cfg
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1181 2023-05-11 19:53:39.000000 fastfft-0.1.1/setup.py
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 19:54:19.036102 fastfft-0.1.1/src/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)   111931 2023-05-11 19:54:18.000000 fastfft-0.1.1/src/__init__.c
```

### Comparing `fastfft-0.1.0/setup.py` & `fastfft-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,22 @@
     with open(filepath) as lockfile:
         lockjson = json.load(lockfile)
         return [dependency for dependency in lockjson.get('default')]
 
 
 ext_modules = [
     Extension("maxim_fft",
-              sources=["src/main.pyx"],
+              sources=["src/__init__.pyx"],
               )
 ]
 
 setup(
     name="fastfft",
     setup_requires=["cython", "numpy"],
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     python_requires='>=3.8',
     author="Maxim Movshin",
     description="Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/BSaaber/fastfft",
```

