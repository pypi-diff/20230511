# Comparing `tmp/smoloki-0.0.6.tar.gz` & `tmp/smoloki-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smoloki-0.0.6.tar", last modified: Tue Jan 31 06:29:32 2023, max compression
+gzip compressed data, was "smoloki-0.0.7.tar", last modified: Thu May 11 16:57:20 2023, max compression
```

## Comparing `smoloki-0.0.6.tar` & `smoloki-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 06:29:32.784160 smoloki-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-01-31 06:29:32.784160 smoloki-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-01-31 06:29:15.000000 smoloki-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 06:29:32.784160 smoloki-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-31 06:29:15.000000 smoloki-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 06:29:32.780160 smoloki-0.0.6/smoloki/
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-01-31 06:29:15.000000 smoloki-0.0.6/smoloki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-01-31 06:29:15.000000 smoloki-0.0.6/smoloki/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 06:29:32.784160 smoloki-0.0.6/smoloki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-01-31 06:29:32.000000 smoloki-0.0.6/smoloki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-31 06:29:32.000000 smoloki-0.0.6/smoloki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 06:29:32.000000 smoloki-0.0.6/smoloki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-31 06:29:32.000000 smoloki-0.0.6/smoloki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-31 06:29:32.000000 smoloki-0.0.6/smoloki.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:57:20.823409 smoloki-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-11 16:57:20.823409 smoloki-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-11 16:57:05.000000 smoloki-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:57:20.823409 smoloki-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-11 16:57:05.000000 smoloki-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:57:20.819409 smoloki-0.0.7/smoloki/
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-11 16:57:05.000000 smoloki-0.0.7/smoloki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-11 16:57:05.000000 smoloki-0.0.7/smoloki/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:57:20.823409 smoloki-0.0.7/smoloki/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-11 16:57:05.000000 smoloki-0.0.7/smoloki/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-11 16:57:05.000000 smoloki-0.0.7/smoloki/wrappers/nodejs.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:57:20.819409 smoloki-0.0.7/smoloki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-11 16:57:20.000000 smoloki-0.0.7/smoloki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-11 16:57:20.000000 smoloki-0.0.7/smoloki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:57:20.000000 smoloki-0.0.7/smoloki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 16:57:20.000000 smoloki-0.0.7/smoloki.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 16:57:20.000000 smoloki-0.0.7/smoloki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 16:57:20.000000 smoloki-0.0.7/smoloki.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:57:20.823409 smoloki-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-11 16:57:05.000000 smoloki-0.0.7/tests/test_logfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-11 16:57:05.000000 smoloki-0.0.7/tests/test_requests.py
```

### Comparing `smoloki-0.0.6/PKG-INFO` & `smoloki-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smoloki
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tiny library to push logs to `Grafana Loki` in `logfmt` format.
 Home-page: https://github.com/michaelkryukov/smoloki
 Author: Michael Krukov
 Author-email: krukov.michael@ya.ru
 Keywords: library,loki
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -50,14 +50,33 @@
   information       json-encoded string with information
 
 options:
   -h, --help        show this help message and exit
   -b BASE_ENDPOINT  base address of loki server
 ```
 
+## Usage in NodeJS
+
+Install simple wrapper for installed python module:
+
+```bash
+# In your project's folder
+smoloki-wrappers --install-wrapper-for-nodejs 'node_modules/'
+```
+
+Usage is along this lines:
+
+```js
+const smoloki = require('smoloki');
+
+// This is an async function executing CLI from previous
+// chapter under the hood.
+smoloki.push({ service: 'web' }, { level: 'info', event: 'request_completed' });
+```
+
 ## Implementation details
 
 - Calls to `push` method will never throw. Any exception will just be
     logged using `logging`.
 - Keys in labels and information must be strings.
 - Values in labels and information must be string, integers or floats.
 - If no `base_endpoint` provided (using parameter or env), nothing
```

### Comparing `smoloki-0.0.6/README.md` & `smoloki-0.0.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -34,14 +34,33 @@
   information       json-encoded string with information
 
 options:
   -h, --help        show this help message and exit
   -b BASE_ENDPOINT  base address of loki server
 ```
 
+## Usage in NodeJS
+
+Install simple wrapper for installed python module:
+
+```bash
+# In your project's folder
+smoloki-wrappers --install-wrapper-for-nodejs 'node_modules/'
+```
+
+Usage is along this lines:
+
+```js
+const smoloki = require('smoloki');
+
+// This is an async function executing CLI from previous
+// chapter under the hood.
+smoloki.push({ service: 'web' }, { level: 'info', event: 'request_completed' });
+```
+
 ## Implementation details
 
 - Calls to `push` method will never throw. Any exception will just be
     logged using `logging`.
 - Keys in labels and information must be strings.
 - Values in labels and information must be string, integers or floats.
 - If no `base_endpoint` provided (using parameter or env), nothing
```

### Comparing `smoloki-0.0.6/setup.py` & `smoloki-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,18 +19,25 @@
     author="Michael Krukov",
     author_email="krukov.michael@ya.ru",
     keywords=["library", "loki"],
     description="Tiny library to push logs to `Grafana Loki` in `logfmt` format.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/michaelkryukov/smoloki",
-    packages=setuptools.find_packages(include=("smoloki",)),
+    packages=setuptools.find_packages(),
     install_requires=[
         "aiohttp~=3.8.3",
     ],
+    entry_points={
+        "console_scripts": [
+            "smoloki = smoloki.__main__:main",
+            "smoloki-wrappers = smoloki.wrappers:main",
+        ],
+    },
+    package_data={"smoloki": ["wrappers/*.js"]},
     python_requires=">=3.8",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
```

### Comparing `smoloki-0.0.6/smoloki/__init__.py` & `smoloki-0.0.7/smoloki/__init__.py`

 * *Files identical despite different names*

### Comparing `smoloki-0.0.6/smoloki/__main__.py` & `smoloki-0.0.7/smoloki/__main__.py`

 * *Files identical despite different names*

### Comparing `smoloki-0.0.6/smoloki.egg-info/PKG-INFO` & `smoloki-0.0.7/smoloki.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smoloki
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tiny library to push logs to `Grafana Loki` in `logfmt` format.
 Home-page: https://github.com/michaelkryukov/smoloki
 Author: Michael Krukov
 Author-email: krukov.michael@ya.ru
 Keywords: library,loki
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -50,14 +50,33 @@
   information       json-encoded string with information
 
 options:
   -h, --help        show this help message and exit
   -b BASE_ENDPOINT  base address of loki server
 ```
 
+## Usage in NodeJS
+
+Install simple wrapper for installed python module:
+
+```bash
+# In your project's folder
+smoloki-wrappers --install-wrapper-for-nodejs 'node_modules/'
+```
+
+Usage is along this lines:
+
+```js
+const smoloki = require('smoloki');
+
+// This is an async function executing CLI from previous
+// chapter under the hood.
+smoloki.push({ service: 'web' }, { level: 'info', event: 'request_completed' });
+```
+
 ## Implementation details
 
 - Calls to `push` method will never throw. Any exception will just be
     logged using `logging`.
 - Keys in labels and information must be strings.
 - Values in labels and information must be string, integers or floats.
 - If no `base_endpoint` provided (using parameter or env), nothing
```

