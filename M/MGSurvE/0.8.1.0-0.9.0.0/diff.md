# Comparing `tmp/MGSurvE-0.8.1.0.tar.gz` & `tmp/MGSurvE-0.9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MGSurvE-0.8.1.0.tar", last modified: Mon Apr 24 22:28:35 2023, max compression
+gzip compressed data, was "MGSurvE-0.9.0.0.tar", last modified: Fri Apr 28 00:58:27 2023, max compression
```

## Comparing `MGSurvE-0.8.1.0.tar` & `MGSurvE-0.9.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-04-24 22:28:35.963356 MGSurvE-0.8.1.0/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    35149 2022-04-07 16:28:31.000000 MGSurvE-0.8.1.0/LICENSE
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-04-24 22:28:35.963356 MGSurvE-0.8.1.0/MGSurvE/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      275 2022-04-21 22:03:09.000000 MGSurvE-0.8.1.0/MGSurvE/__init__.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       23 2023-04-24 22:28:35.000000 MGSurvE-0.8.1.0/MGSurvE/_version.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6881 2022-04-13 19:47:11.000000 MGSurvE-0.8.1.0/MGSurvE/auxiliary.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      604 2022-02-18 19:18:22.000000 MGSurvE-0.8.1.0/MGSurvE/colors.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1665 2022-04-07 16:28:31.000000 MGSurvE-0.8.1.0/MGSurvE/constants.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6409 2023-04-14 19:41:05.000000 MGSurvE-0.8.1.0/MGSurvE/kernels.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    21356 2022-08-10 16:42:54.000000 MGSurvE-0.8.1.0/MGSurvE/landscape.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4924 2022-03-21 16:18:35.000000 MGSurvE-0.8.1.0/MGSurvE/matrices.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1358 2022-02-18 19:21:24.000000 MGSurvE-0.8.1.0/MGSurvE/network.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    45037 2023-02-23 20:20:29.000000 MGSurvE-0.8.1.0/MGSurvE/optimization.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     9200 2022-05-13 21:20:28.000000 MGSurvE-0.8.1.0/MGSurvE/optimizationPSO.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    18224 2023-04-17 15:16:06.000000 MGSurvE-0.8.1.0/MGSurvE/plots.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6849 2023-03-02 20:49:07.000000 MGSurvE-0.8.1.0/MGSurvE/pointProcess.py
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-04-24 22:28:35.963356 MGSurvE-0.8.1.0/MGSurvE.egg-info/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4596 2023-04-24 22:28:35.000000 MGSurvE-0.8.1.0/MGSurvE.egg-info/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      451 2023-04-24 22:28:35.000000 MGSurvE-0.8.1.0/MGSurvE.egg-info/SOURCES.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        1 2023-04-24 22:28:35.000000 MGSurvE-0.8.1.0/MGSurvE.egg-info/dependency_links.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      214 2023-04-24 22:28:35.000000 MGSurvE-0.8.1.0/MGSurvE.egg-info/requires.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        8 2023-04-24 22:28:35.000000 MGSurvE-0.8.1.0/MGSurvE.egg-info/top_level.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4596 2023-04-24 22:28:35.963356 MGSurvE-0.8.1.0/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4162 2023-04-04 16:41:41.000000 MGSurvE-0.8.1.0/README.md
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       38 2023-04-24 22:28:35.963356 MGSurvE-0.8.1.0/setup.cfg
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1414 2023-03-29 20:42:31.000000 MGSurvE-0.8.1.0/setup.py
+drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-04-28 00:58:27.732098 MGSurvE-0.9.0.0/
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    35149 2022-04-07 16:28:31.000000 MGSurvE-0.9.0.0/LICENSE
+drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-04-28 00:58:27.732098 MGSurvE-0.9.0.0/MGSurvE/
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      275 2022-04-21 22:03:09.000000 MGSurvE-0.9.0.0/MGSurvE/__init__.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       23 2023-04-28 00:58:27.000000 MGSurvE-0.9.0.0/MGSurvE/_version.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6881 2022-04-13 19:47:11.000000 MGSurvE-0.9.0.0/MGSurvE/auxiliary.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      604 2022-02-18 19:18:22.000000 MGSurvE-0.9.0.0/MGSurvE/colors.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1665 2022-04-07 16:28:31.000000 MGSurvE-0.9.0.0/MGSurvE/constants.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6409 2023-04-14 19:41:05.000000 MGSurvE-0.9.0.0/MGSurvE/kernels.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    21356 2022-08-10 16:42:54.000000 MGSurvE-0.9.0.0/MGSurvE/landscape.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4924 2022-03-21 16:18:35.000000 MGSurvE-0.9.0.0/MGSurvE/matrices.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1358 2022-02-18 19:21:24.000000 MGSurvE-0.9.0.0/MGSurvE/network.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    45037 2023-02-23 20:20:29.000000 MGSurvE-0.9.0.0/MGSurvE/optimization.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     9200 2022-05-13 21:20:28.000000 MGSurvE-0.9.0.0/MGSurvE/optimizationPSO.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    18224 2023-04-17 15:16:06.000000 MGSurvE-0.9.0.0/MGSurvE/plots.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6849 2023-03-02 20:49:07.000000 MGSurvE-0.9.0.0/MGSurvE/pointProcess.py
+drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-04-28 00:58:27.732098 MGSurvE-0.9.0.0/MGSurvE.egg-info/
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4596 2023-04-28 00:58:27.000000 MGSurvE-0.9.0.0/MGSurvE.egg-info/PKG-INFO
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      451 2023-04-28 00:58:27.000000 MGSurvE-0.9.0.0/MGSurvE.egg-info/SOURCES.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        1 2023-04-28 00:58:27.000000 MGSurvE-0.9.0.0/MGSurvE.egg-info/dependency_links.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      214 2023-04-28 00:58:27.000000 MGSurvE-0.9.0.0/MGSurvE.egg-info/requires.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        8 2023-04-28 00:58:27.000000 MGSurvE-0.9.0.0/MGSurvE.egg-info/top_level.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4596 2023-04-28 00:58:27.732098 MGSurvE-0.9.0.0/PKG-INFO
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4162 2023-04-04 16:41:41.000000 MGSurvE-0.9.0.0/README.md
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       38 2023-04-28 00:58:27.732098 MGSurvE-0.9.0.0/setup.cfg
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1414 2023-03-29 20:42:31.000000 MGSurvE-0.9.0.0/setup.py
```

### Comparing `MGSurvE-0.8.1.0/LICENSE` & `MGSurvE-0.9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/MGSurvE/auxiliary.py` & `MGSurvE-0.9.0.0/MGSurvE/auxiliary.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/MGSurvE/colors.py` & `MGSurvE-0.9.0.0/MGSurvE/colors.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/MGSurvE/constants.py` & `MGSurvE-0.9.0.0/MGSurvE/constants.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/MGSurvE/kernels.py` & `MGSurvE-0.9.0.0/MGSurvE/kernels.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/MGSurvE/landscape.py` & `MGSurvE-0.9.0.0/MGSurvE/landscape.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/MGSurvE/matrices.py` & `MGSurvE-0.9.0.0/MGSurvE/matrices.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/MGSurvE/network.py` & `MGSurvE-0.9.0.0/MGSurvE/network.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/MGSurvE/optimization.py` & `MGSurvE-0.9.0.0/MGSurvE/optimization.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/MGSurvE/optimizationPSO.py` & `MGSurvE-0.9.0.0/MGSurvE/optimizationPSO.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/MGSurvE/plots.py` & `MGSurvE-0.9.0.0/MGSurvE/plots.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/MGSurvE/pointProcess.py` & `MGSurvE-0.9.0.0/MGSurvE/pointProcess.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/MGSurvE.egg-info/PKG-INFO` & `MGSurvE-0.9.0.0/MGSurvE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 0.8.1.0
+Version: 0.9.0.0
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-0.8.1.0/PKG-INFO` & `MGSurvE-0.9.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 0.8.1.0
+Version: 0.9.0.0
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-0.8.1.0/README.md` & `MGSurvE-0.9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.1.0/setup.py` & `MGSurvE-0.9.0.0/setup.py`

 * *Files identical despite different names*

