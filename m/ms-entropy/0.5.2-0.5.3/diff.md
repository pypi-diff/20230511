# Comparing `tmp/ms_entropy-0.5.2.tar.gz` & `tmp/ms_entropy-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_entropy-0.5.2.tar", last modified: Wed May 10 08:00:11 2023, max compression
+gzip compressed data, was "ms_entropy-0.5.3.tar", last modified: Thu May 11 18:19:14 2023, max compression
```

## Comparing `ms_entropy-0.5.2.tar` & `ms_entropy-0.5.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 08:00:11.122063 ms_entropy-0.5.2/
--rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.5.2/LICENSE
--rw-rw-r--   0 yli       (1000) yli       (1000)       68 2023-05-10 07:52:05.000000 ms_entropy-0.5.2/MANIFEST.in
--rw-rw-r--   0 yli       (1000) yli       (1000)      422 2023-05-10 08:00:11.122063 ms_entropy-0.5.2/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     3264 2023-03-29 23:15:55.000000 ms_entropy-0.5.2/README.md
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 08:00:11.118063 ms_entropy-0.5.2/ms_entropy/
--rw-rw-r--   0 yli       (1000) yli       (1000)      155 2023-05-10 07:39:51.000000 ms_entropy-0.5.2/ms_entropy/__init__.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 08:00:11.118063 ms_entropy-0.5.2/ms_entropy/entropy_search/
--rw-rw-r--   0 yli       (1000) yli       (1000)       52 2023-05-10 07:39:35.000000 ms_entropy-0.5.2/ms_entropy/entropy_search/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    20245 2023-05-10 07:39:35.000000 ms_entropy-0.5.2/ms_entropy/entropy_search/flash_entropy_search.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    27891 2023-05-10 07:39:35.000000 ms_entropy-0.5.2/ms_entropy/entropy_search/flash_entropy_search_core.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     5661 2023-05-10 07:39:35.000000 ms_entropy-0.5.2/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 08:00:11.118063 ms_entropy-0.5.2/ms_entropy/file_io/
--rw-rw-r--   0 yli       (1000) yli       (1000)       40 2023-05-10 07:39:40.000000 ms_entropy-0.5.2/ms_entropy/file_io/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     2047 2023-05-10 07:39:40.000000 ms_entropy-0.5.2/ms_entropy/file_io/lbm2_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     1690 2023-05-10 07:39:40.000000 ms_entropy-0.5.2/ms_entropy/file_io/mgf_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     1930 2023-05-10 07:39:40.000000 ms_entropy-0.5.2/ms_entropy/file_io/msp_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     1974 2023-05-10 07:39:40.000000 ms_entropy-0.5.2/ms_entropy/file_io/mzml_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)      920 2023-05-10 07:39:40.000000 ms_entropy-0.5.2/ms_entropy/file_io/shared.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     4249 2023-05-10 07:39:40.000000 ms_entropy-0.5.2/ms_entropy/file_io/spec_file.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 08:00:11.122063 ms_entropy-0.5.2/ms_entropy/tools/
--rw-rw-r--   0 yli       (1000) yli       (1000)      118 2023-05-10 07:39:45.000000 ms_entropy-0.5.2/ms_entropy/tools/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-10 07:43:19.000000 ms_entropy-0.5.2/ms_entropy/tools/fast_entropy.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-10 07:39:45.000000 ms_entropy-0.5.2/ms_entropy/tools/fast_entropy.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-10 07:43:20.000000 ms_entropy-0.5.2/ms_entropy/tools/fast_spectrum.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-10 07:39:45.000000 ms_entropy-0.5.2/ms_entropy/tools/fast_spectrum.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)     4318 2023-05-10 07:39:45.000000 ms_entropy-0.5.2/ms_entropy/tools/tools.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 08:00:11.118063 ms_entropy-0.5.2/ms_entropy.egg-info/
--rw-rw-r--   0 yli       (1000) yli       (1000)      422 2023-05-10 08:00:11.000000 ms_entropy-0.5.2/ms_entropy.egg-info/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     1404 2023-05-10 08:00:11.000000 ms_entropy-0.5.2/ms_entropy.egg-info/SOURCES.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-05-10 08:00:11.000000 ms_entropy-0.5.2/ms_entropy.egg-info/dependency_links.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)      103 2023-05-10 08:00:11.000000 ms_entropy-0.5.2/ms_entropy.egg-info/requires.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-05-10 08:00:11.000000 ms_entropy-0.5.2/ms_entropy.egg-info/top_level.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.5.2/pyproject.toml
--rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-05-10 08:00:11.122063 ms_entropy-0.5.2/setup.cfg
--rw-rw-r--   0 yli       (1000) yli       (1000)     1658 2023-05-10 08:00:04.000000 ms_entropy-0.5.2/setup.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/
+-rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.5.3/LICENSE
+-rw-rw-r--   0 yli       (1000) yli       (1000)       68 2023-05-10 07:52:05.000000 ms_entropy-0.5.3/MANIFEST.in
+-rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3264 2023-03-29 23:15:55.000000 ms_entropy-0.5.3/README.md
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/ms_entropy/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      155 2023-05-10 07:39:51.000000 ms_entropy-0.5.3/ms_entropy/__init__.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/ms_entropy/entropy_search/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      196 2023-05-10 21:32:05.000000 ms_entropy-0.5.3/ms_entropy/entropy_search/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    20245 2023-05-10 07:39:35.000000 ms_entropy-0.5.3/ms_entropy/entropy_search/flash_entropy_search.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    27891 2023-05-10 07:39:35.000000 ms_entropy-0.5.3/ms_entropy/entropy_search/flash_entropy_search_core.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5661 2023-05-10 07:39:35.000000 ms_entropy-0.5.3/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/ms_entropy/file_io/
+-rw-rw-r--   0 yli       (1000) yli       (1000)       62 2023-05-10 23:13:55.000000 ms_entropy-0.5.3/ms_entropy/file_io/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     2047 2023-05-10 07:39:40.000000 ms_entropy-0.5.3/ms_entropy/file_io/lbm2_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1690 2023-05-10 07:39:40.000000 ms_entropy-0.5.3/ms_entropy/file_io/mgf_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1930 2023-05-10 07:39:40.000000 ms_entropy-0.5.3/ms_entropy/file_io/msp_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1974 2023-05-10 07:39:40.000000 ms_entropy-0.5.3/ms_entropy/file_io/mzml_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)      920 2023-05-10 07:39:40.000000 ms_entropy-0.5.3/ms_entropy/file_io/shared.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5718 2023-05-10 23:12:41.000000 ms_entropy-0.5.3/ms_entropy/file_io/spec_file.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/ms_entropy/tools/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      118 2023-05-10 07:39:45.000000 ms_entropy-0.5.3/ms_entropy/tools/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-10 07:43:19.000000 ms_entropy-0.5.3/ms_entropy/tools/fast_entropy.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-10 07:39:45.000000 ms_entropy-0.5.3/ms_entropy/tools/fast_entropy.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-10 07:43:20.000000 ms_entropy-0.5.3/ms_entropy/tools/fast_spectrum.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-10 07:39:45.000000 ms_entropy-0.5.3/ms_entropy/tools/fast_spectrum.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4318 2023-05-10 07:39:45.000000 ms_entropy-0.5.3/ms_entropy/tools/tools.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/ms_entropy.egg-info/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-11 18:19:14.000000 ms_entropy-0.5.3/ms_entropy.egg-info/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1404 2023-05-11 18:19:14.000000 ms_entropy-0.5.3/ms_entropy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-05-11 18:19:14.000000 ms_entropy-0.5.3/ms_entropy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       84 2023-05-11 18:19:14.000000 ms_entropy-0.5.3/ms_entropy.egg-info/requires.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-05-11 18:19:14.000000 ms_entropy-0.5.3/ms_entropy.egg-info/top_level.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.5.3/pyproject.toml
+-rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/setup.cfg
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1648 2023-05-11 18:17:51.000000 ms_entropy-0.5.3/setup.py
```

### Comparing `ms_entropy-0.5.2/LICENSE` & `ms_entropy-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/README.md` & `ms_entropy-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/entropy_search/flash_entropy_search.py` & `ms_entropy-0.5.3/ms_entropy/entropy_search/flash_entropy_search.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/entropy_search/flash_entropy_search_core.py` & `ms_entropy-0.5.3/ms_entropy/entropy_search/flash_entropy_search_core.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py` & `ms_entropy-0.5.3/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/file_io/lbm2_file.py` & `ms_entropy-0.5.3/ms_entropy/file_io/lbm2_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/file_io/mgf_file.py` & `ms_entropy-0.5.3/ms_entropy/file_io/mgf_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/file_io/msp_file.py` & `ms_entropy-0.5.3/ms_entropy/file_io/msp_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/file_io/mzml_file.py` & `ms_entropy-0.5.3/ms_entropy/file_io/mzml_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/file_io/shared.py` & `ms_entropy-0.5.3/ms_entropy/file_io/shared.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/tools/fast_entropy.c` & `ms_entropy-0.5.3/ms_entropy/tools/fast_entropy.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/tools/fast_entropy.pyx` & `ms_entropy-0.5.3/ms_entropy/tools/fast_entropy.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/tools/fast_spectrum.c` & `ms_entropy-0.5.3/ms_entropy/tools/fast_spectrum.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/tools/fast_spectrum.pyx` & `ms_entropy-0.5.3/ms_entropy/tools/fast_spectrum.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy/tools/tools.py` & `ms_entropy-0.5.3/ms_entropy/tools/tools.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/ms_entropy.egg-info/SOURCES.txt` & `ms_entropy-0.5.3/ms_entropy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.2/setup.py` & `ms_entropy-0.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 import os
 
 
 os.environ['CFLAGS'] = '-O3 -Wno-cpp -Wno-unused-function'
 
 setup(
     name='ms_entropy',
-    version='0.5.2',
+    version='0.5.3',
     license='Apache License 2.0',
     author='Yuanyue Li',
     url='https://github.com/YuanyueLi/SpectralEntropy',
     packages=find_packages(where='.', exclude=['tests', 'docs', 'examples', 'manuscript', 'dist', 'build']),
     python_requires='>=3.8',
     install_requires=[
         "numpy >= 1.18",
-        "cython >= 0.29"
+        "cython >= 0.29",
+        "lz4>=4.3.2",
+        "msgpack>=1.0.5",
+        "pymzml>=2.5.2"
     ],
     extras_require={
-        "gpu": ["cupy >= 8.3.0"],
-        "all": ["cupy >= 8.3.0", "lz4>=4.3.2", "msgpack>=1.0.5", "pymzml>=2.5.2"]
+        "gpu": ["cupy >= 8.3.0"]
     },
     keywords=[
         "ms entropy",
         "ms spectral entropy",
         "spectral entropy",
         "spectral similarity",
         "entropy similarity",
```

