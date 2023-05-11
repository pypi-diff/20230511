# Comparing `tmp/smoloki-0.0.7.tar.gz` & `tmp/smoloki-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smoloki-0.0.7.tar", last modified: Thu May 11 16:57:20 2023, max compression
+gzip compressed data, was "smoloki-0.0.8.tar", last modified: Thu May 11 17:24:45 2023, max compression
```

## Comparing `smoloki-0.0.7.tar` & `smoloki-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:57:20.823409 smoloki-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-11 16:57:20.823409 smoloki-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-11 16:57:05.000000 smoloki-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:57:20.823409 smoloki-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-11 16:57:05.000000 smoloki-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:57:20.819409 smoloki-0.0.7/smoloki/
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-11 16:57:05.000000 smoloki-0.0.7/smoloki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-11 16:57:05.000000 smoloki-0.0.7/smoloki/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:57:20.823409 smoloki-0.0.7/smoloki/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-11 16:57:05.000000 smoloki-0.0.7/smoloki/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-11 16:57:05.000000 smoloki-0.0.7/smoloki/wrappers/nodejs.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:57:20.819409 smoloki-0.0.7/smoloki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-11 16:57:20.000000 smoloki-0.0.7/smoloki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-11 16:57:20.000000 smoloki-0.0.7/smoloki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:57:20.000000 smoloki-0.0.7/smoloki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 16:57:20.000000 smoloki-0.0.7/smoloki.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 16:57:20.000000 smoloki-0.0.7/smoloki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 16:57:20.000000 smoloki-0.0.7/smoloki.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:57:20.823409 smoloki-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-11 16:57:05.000000 smoloki-0.0.7/tests/test_logfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-11 16:57:05.000000 smoloki-0.0.7/tests/test_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:24:45.730966 smoloki-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-11 17:24:45.730966 smoloki-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-11 17:24:30.000000 smoloki-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 17:24:45.730966 smoloki-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-11 17:24:30.000000 smoloki-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:24:45.726966 smoloki-0.0.8/smoloki/
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-11 17:24:30.000000 smoloki-0.0.8/smoloki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-11 17:24:30.000000 smoloki-0.0.8/smoloki/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:24:45.730966 smoloki-0.0.8/smoloki/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-11 17:24:30.000000 smoloki-0.0.8/smoloki/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-11 17:24:30.000000 smoloki-0.0.8/smoloki/wrappers/nodejs.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:24:45.730966 smoloki-0.0.8/smoloki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-11 17:24:45.000000 smoloki-0.0.8/smoloki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-11 17:24:45.000000 smoloki-0.0.8/smoloki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 17:24:45.000000 smoloki-0.0.8/smoloki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 17:24:45.000000 smoloki-0.0.8/smoloki.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 17:24:45.000000 smoloki-0.0.8/smoloki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 17:24:45.000000 smoloki-0.0.8/smoloki.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:24:45.730966 smoloki-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-11 17:24:30.000000 smoloki-0.0.8/tests/test_logfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-11 17:24:30.000000 smoloki-0.0.8/tests/test_requests.py
```

### Comparing `smoloki-0.0.7/PKG-INFO` & `smoloki-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: smoloki
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tiny library to push logs to `Grafana Loki` in `logfmt` format.
 Home-page: https://github.com/michaelkryukov/smoloki
 Author: Michael Krukov
 Author-email: krukov.michael@ya.ru
 Keywords: library,loki
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # smoloki
 
 [![PyPI version](https://badge.fury.io/py/smoloki.svg)](https://badge.fury.io/py/smoloki)
 
 Tiny library to push logs to `Grafana Loki` in `logfmt` format.
```

### Comparing `smoloki-0.0.7/README.md` & `smoloki-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `smoloki-0.0.7/setup.py` & `smoloki-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     entry_points={
         "console_scripts": [
             "smoloki = smoloki.__main__:main",
             "smoloki-wrappers = smoloki.wrappers:main",
         ],
     },
     package_data={"smoloki": ["wrappers/*.js"]},
-    python_requires=">=3.8",
+    python_requires=">=3.7",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
     ],
```

### Comparing `smoloki-0.0.7/smoloki/__init__.py` & `smoloki-0.0.8/smoloki/__init__.py`

 * *Files identical despite different names*

### Comparing `smoloki-0.0.7/smoloki/__main__.py` & `smoloki-0.0.8/smoloki/__main__.py`

 * *Files identical despite different names*

### Comparing `smoloki-0.0.7/smoloki/wrappers/__init__.py` & `smoloki-0.0.8/smoloki/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `smoloki-0.0.7/smoloki/wrappers/nodejs.js` & `smoloki-0.0.8/smoloki/wrappers/nodejs.js`

 * *Files identical despite different names*

### Comparing `smoloki-0.0.7/smoloki.egg-info/PKG-INFO` & `smoloki-0.0.8/smoloki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: smoloki
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tiny library to push logs to `Grafana Loki` in `logfmt` format.
 Home-page: https://github.com/michaelkryukov/smoloki
 Author: Michael Krukov
 Author-email: krukov.michael@ya.ru
 Keywords: library,loki
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # smoloki
 
 [![PyPI version](https://badge.fury.io/py/smoloki.svg)](https://badge.fury.io/py/smoloki)
 
 Tiny library to push logs to `Grafana Loki` in `logfmt` format.
```

### Comparing `smoloki-0.0.7/tests/test_logfmt.py` & `smoloki-0.0.8/tests/test_logfmt.py`

 * *Files identical despite different names*

### Comparing `smoloki-0.0.7/tests/test_requests.py` & `smoloki-0.0.8/tests/test_requests.py`

 * *Files identical despite different names*

