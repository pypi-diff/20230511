# Comparing `tmp/phase-o-matic-0.0.3.tar.gz` & `tmp/phase-o-matic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phase-o-matic-0.0.3.tar", last modified: Thu May 11 19:33:52 2023, max compression
+gzip compressed data, was "phase-o-matic-0.0.4.tar", last modified: Thu May 11 19:41:40 2023, max compression
```

## Comparing `phase-o-matic-0.0.3.tar` & `phase-o-matic-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-11 19:33:52.510638 phase-o-matic-0.0.3/
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     1073 2023-05-04 18:10:22.000000 phase-o-matic-0.0.3/LICENSE
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     4550 2023-05-11 19:33:52.510318 phase-o-matic-0.0.3/PKG-INFO
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     4050 2023-05-11 19:09:14.000000 phase-o-matic-0.0.3/README.md
-drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-11 19:33:52.505175 phase-o-matic-0.0.3/phase_o_matic/
-drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-11 19:33:52.508983 phase-o-matic-0.0.3/phase_o_matic/phase_o_matic.egg-info/
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     4550 2023-05-11 19:33:52.000000 phase-o-matic-0.0.3/phase_o_matic/phase_o_matic.egg-info/PKG-INFO
--rw-r--r--   0 zachkeskinen   (501) staff       (20)      343 2023-05-11 19:33:52.000000 phase-o-matic-0.0.3/phase_o_matic/phase_o_matic.egg-info/SOURCES.txt
--rw-r--r--   0 zachkeskinen   (501) staff       (20)        1 2023-05-11 19:33:52.000000 phase-o-matic-0.0.3/phase_o_matic/phase_o_matic.egg-info/dependency_links.txt
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       51 2023-05-11 19:33:52.000000 phase-o-matic-0.0.3/phase_o_matic/phase_o_matic.egg-info/requires.txt
--rw-r--r--   0 zachkeskinen   (501) staff       (20)        1 2023-05-11 19:33:52.000000 phase-o-matic-0.0.3/phase_o_matic/phase_o_matic.egg-info/top_level.txt
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       84 2023-05-11 19:28:36.000000 phase-o-matic-0.0.3/pyproject.toml
--rw-r--r--   0 zachkeskinen   (501) staff       (20)       38 2023-05-11 19:33:52.510737 phase-o-matic-0.0.3/setup.cfg
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     1003 2023-05-11 19:33:36.000000 phase-o-matic-0.0.3/setup.py
-drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-11 19:33:52.509881 phase-o-matic-0.0.3/tests/
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     2273 2023-05-10 20:11:26.000000 phase-o-matic-0.0.3/tests/test_download.py
--rw-r--r--   0 zachkeskinen   (501) staff       (20)     5053 2023-05-10 20:26:07.000000 phase-o-matic-0.0.3/tests/test_preprocess.py
+drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-11 19:41:40.444001 phase-o-matic-0.0.4/
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)     1073 2023-05-04 18:10:22.000000 phase-o-matic-0.0.4/LICENSE
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)     4714 2023-05-11 19:41:40.443633 phase-o-matic-0.0.4/PKG-INFO
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)     4050 2023-05-11 19:09:14.000000 phase-o-matic-0.0.4/README.md
+drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-11 19:41:40.440167 phase-o-matic-0.0.4/phase_o_matic/
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)       38 2023-05-10 18:09:00.000000 phase-o-matic-0.0.4/phase_o_matic/__init__.py
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)     3014 2023-05-10 20:11:35.000000 phase-o-matic-0.0.4/phase_o_matic/download.py
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)     6390 2023-05-10 20:40:18.000000 phase-o-matic-0.0.4/phase_o_matic/phase_delay.py
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)     9263 2023-05-11 19:12:37.000000 phase-o-matic-0.0.4/phase_o_matic/preprocess.py
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)     1152 2023-05-10 18:08:17.000000 phase-o-matic-0.0.4/phase_o_matic/presto.py
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)     1387 2023-05-10 20:47:48.000000 phase-o-matic-0.0.4/phase_o_matic/utils.py
+drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-11 19:41:40.442153 phase-o-matic-0.0.4/phase_o_matic.egg-info/
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)     4714 2023-05-11 19:41:40.000000 phase-o-matic-0.0.4/phase_o_matic.egg-info/PKG-INFO
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)      429 2023-05-11 19:41:40.000000 phase-o-matic-0.0.4/phase_o_matic.egg-info/SOURCES.txt
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)        1 2023-05-11 19:41:40.000000 phase-o-matic-0.0.4/phase_o_matic.egg-info/dependency_links.txt
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)       51 2023-05-11 19:41:40.000000 phase-o-matic-0.0.4/phase_o_matic.egg-info/requires.txt
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)       14 2023-05-11 19:41:40.000000 phase-o-matic-0.0.4/phase_o_matic.egg-info/top_level.txt
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)       84 2023-05-11 19:28:36.000000 phase-o-matic-0.0.4/pyproject.toml
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)       38 2023-05-11 19:41:40.444156 phase-o-matic-0.0.4/setup.cfg
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)     3952 2023-05-11 19:41:16.000000 phase-o-matic-0.0.4/setup.py
+drwxr-xr-x   0 zachkeskinen   (501) staff       (20)        0 2023-05-11 19:41:40.443174 phase-o-matic-0.0.4/tests/
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)     2273 2023-05-10 20:11:26.000000 phase-o-matic-0.0.4/tests/test_download.py
+-rw-r--r--   0 zachkeskinen   (501) staff       (20)     5053 2023-05-10 20:26:07.000000 phase-o-matic-0.0.4/tests/test_preprocess.py
```

### Comparing `phase-o-matic-0.0.3/LICENSE` & `phase-o-matic-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.3/PKG-INFO` & `phase-o-matic-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: phase-o-matic
-Version: 0.0.3
-Summary: InSAR Atmospheric Delay Corrections with ERA5
+Version: 0.0.4
+Summary: InSAR Atmospheric Delay Corrections with ERA5.
 Home-page: https://github.com/ZachKeskinen/phase-o-matic
-Author: Zachary Keskinen
+Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
-Keywords: phase-o-matic
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
 # phase-o-matic
 
 [![DOI](https://zenodo.org/badge/636333382.svg)](https://zenodo.org/badge/latestdoi/636333382)
 
 Python package for calculating Interferometric Synthetic Aperture Radar phase delays from ERA5 atmospheric models. Utilizes xarray to easily download, processes, and add phase delays to netcdfs of InSAR Phase. 
 
 Useful publications for this repo:
```

### Comparing `phase-o-matic-0.0.3/README.md` & `phase-o-matic-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.3/phase_o_matic/phase_o_matic.egg-info/PKG-INFO` & `phase-o-matic-0.0.4/phase_o_matic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: phase-o-matic
-Version: 0.0.3
-Summary: InSAR Atmospheric Delay Corrections with ERA5
+Version: 0.0.4
+Summary: InSAR Atmospheric Delay Corrections with ERA5.
 Home-page: https://github.com/ZachKeskinen/phase-o-matic
-Author: Zachary Keskinen
+Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
-Keywords: phase-o-matic
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
 # phase-o-matic
 
 [![DOI](https://zenodo.org/badge/636333382.svg)](https://zenodo.org/badge/latestdoi/636333382)
 
 Python package for calculating Interferometric Synthetic Aperture Radar phase delays from ERA5 atmospheric models. Utilizes xarray to easily download, processes, and add phase delays to netcdfs of InSAR Phase. 
 
 Useful publications for this repo:
```

### Comparing `phase-o-matic-0.0.3/tests/test_download.py` & `phase-o-matic-0.0.4/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.3/tests/test_preprocess.py` & `phase-o-matic-0.0.4/tests/test_preprocess.py`

 * *Files identical despite different names*

