# Comparing `tmp/phase-o-matic-0.0.6.tar.gz` & `tmp/phase-o-matic-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phase-o-matic-0.0.6.tar", last modified: Thu May 11 20:15:26 2023, max compression
+gzip compressed data, was "phase-o-matic-0.0.7.tar", last modified: Thu May 11 20:19:49 2023, max compression
```

## Comparing `phase-o-matic-0.0.6.tar` & `phase-o-matic-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:15:26.600233 phase-o-matic-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-11 20:15:26.600233 phase-o-matic-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:15:26.600233 phase-o-matic-0.0.6/phase_o_matic/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/phase_o_matic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/phase_o_matic/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/phase_o_matic/phase_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/phase_o_matic/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/phase_o_matic/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/phase_o_matic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:15:26.600233 phase-o-matic-0.0.6/phase_o_matic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-11 20:15:26.000000 phase-o-matic-0.0.6/phase_o_matic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-11 20:15:26.000000 phase-o-matic-0.0.6/phase_o_matic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:15:26.000000 phase-o-matic-0.0.6/phase_o_matic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 20:15:26.000000 phase-o-matic-0.0.6/phase_o_matic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 20:15:26.000000 phase-o-matic-0.0.6/phase_o_matic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:15:26.600233 phase-o-matic-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-11 20:15:10.000000 phase-o-matic-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:15:26.600233 phase-o-matic-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-11 20:15:09.000000 phase-o-matic-0.0.6/tests/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:19:49.179319 phase-o-matic-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-11 20:19:49.179319 phase-o-matic-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:19:49.179319 phase-o-matic-0.0.7/phase_o_matic/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/phase_o_matic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/phase_o_matic/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/phase_o_matic/phase_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/phase_o_matic/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/phase_o_matic/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/phase_o_matic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:19:49.179319 phase-o-matic-0.0.7/phase_o_matic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-11 20:19:49.000000 phase-o-matic-0.0.7/phase_o_matic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-11 20:19:49.000000 phase-o-matic-0.0.7/phase_o_matic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:19:49.000000 phase-o-matic-0.0.7/phase_o_matic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 20:19:49.000000 phase-o-matic-0.0.7/phase_o_matic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 20:19:49.000000 phase-o-matic-0.0.7/phase_o_matic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:19:49.179319 phase-o-matic-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:19:49.179319 phase-o-matic-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/tests/test_preprocess.py
```

### Comparing `phase-o-matic-0.0.6/LICENSE` & `phase-o-matic-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.6/PKG-INFO` & `phase-o-matic-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phase-o-matic
-Version: 0.0.6
+Version: 0.0.7
 Summary: InSAR Atmospheric Delay Corrections with ERA5.
 Home-page: https://github.com/ZachKeskinen/phase-o-matic
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `phase-o-matic-0.0.6/README.md` & `phase-o-matic-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.6/phase_o_matic/download.py` & `phase-o-matic-0.0.7/phase_o_matic/download.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.6/phase_o_matic/phase_delay.py` & `phase-o-matic-0.0.7/phase_o_matic/phase_delay.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.6/phase_o_matic/preprocess.py` & `phase-o-matic-0.0.7/phase_o_matic/preprocess.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.6/phase_o_matic/presto.py` & `phase-o-matic-0.0.7/phase_o_matic/presto.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.6/phase_o_matic/utils.py` & `phase-o-matic-0.0.7/phase_o_matic/utils.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.6/phase_o_matic.egg-info/PKG-INFO` & `phase-o-matic-0.0.7/phase_o_matic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phase-o-matic
-Version: 0.0.6
+Version: 0.0.7
 Summary: InSAR Atmospheric Delay Corrections with ERA5.
 Home-page: https://github.com/ZachKeskinen/phase-o-matic
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `phase-o-matic-0.0.6/setup.py` & `phase-o-matic-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version='0.0.6',
+    version='0.0.7',
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
```

### Comparing `phase-o-matic-0.0.6/tests/test_download.py` & `phase-o-matic-0.0.7/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.6/tests/test_preprocess.py` & `phase-o-matic-0.0.7/tests/test_preprocess.py`

 * *Files identical despite different names*

