# Comparing `tmp/TEDEouS-0.1.0.tar.gz` & `tmp/TEDEouS-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEDEouS-0.1.0.tar", last modified: Wed May 10 20:21:07 2023, max compression
+gzip compressed data, was "TEDEouS-0.1.1.tar", last modified: Wed May 10 21:13:22 2023, max compression
```

## Comparing `TEDEouS-0.1.0.tar` & `TEDEouS-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:21:07.966845 TEDEouS-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-10 20:21:02.000000 TEDEouS-0.1.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-10 20:21:07.966845 TEDEouS-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-10 20:21:02.000000 TEDEouS-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:21:07.966845 TEDEouS-0.1.0/TEDEouS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-10 20:21:07.000000 TEDEouS-0.1.0/TEDEouS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 20:21:07.000000 TEDEouS-0.1.0/TEDEouS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:21:07.000000 TEDEouS-0.1.0/TEDEouS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:21:07.000000 TEDEouS-0.1.0/TEDEouS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 20:21:07.966845 TEDEouS-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-10 20:21:03.000000 TEDEouS-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:22.275539 TEDEouS-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-10 21:13:22.275539 TEDEouS-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:22.271538 TEDEouS-0.1.1/TEDEouS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-10 21:13:22.000000 TEDEouS-0.1.1/TEDEouS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-10 21:13:22.000000 TEDEouS-0.1.1/TEDEouS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:13:22.000000 TEDEouS-0.1.1/TEDEouS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 21:13:22.000000 TEDEouS-0.1.1/TEDEouS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 21:13:22.275539 TEDEouS-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:22.275539 TEDEouS-0.1.1/tedeous/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/tedeous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/tedeous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/tedeous/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/tedeous/derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/tedeous/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/tedeous/finite_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/tedeous/input_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/tedeous/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/tedeous/points_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-05-10 21:13:17.000000 TEDEouS-0.1.1/tedeous/solver.py
```

### Comparing `TEDEouS-0.1.0/LICENCE` & `TEDEouS-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `TEDEouS-0.1.0/PKG-INFO` & `TEDEouS-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TEDEouS
-Version: 0.1.0
+Version: 0.1.1
 Summary: TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library
 Author: Alexander Hvatov
 Author-email: itmo.nss.team@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `TEDEouS-0.1.0/README.rst` & `TEDEouS-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `TEDEouS-0.1.0/TEDEouS.egg-info/PKG-INFO` & `TEDEouS-0.1.1/TEDEouS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TEDEouS
-Version: 0.1.0
+Version: 0.1.1
 Summary: TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library
 Author: Alexander Hvatov
 Author-email: itmo.nss.team@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `TEDEouS-0.1.0/setup.py` & `TEDEouS-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def get_requirements():
     requirements = extract_requirements('requirements.txt')
     return requirements
 
 setup(
     name = 'TEDEouS',
-    version= '0.1.0' ,
+    version= '0.1.1' ,
     description = 'TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library',
     long_description = 'Combine power of pytorch, numerical methods and math overall to conquer and solve ALL {O,P}DEs. There are some examples to provide a little insight to an operator form',
     author = 'Alexander Hvatov',
     author_email = 'itmo.nss.team@gmail.com', # add email
     classifiers = [      
               'Development Status :: 3 - Alpha',
               'Programming Language :: Python :: 3',
```

