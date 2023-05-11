# Comparing `tmp/crosscompute-printers-pdf-0.4.0.tar.gz` & `tmp/crosscompute-printers-pdf-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosscompute-printers-pdf-0.4.0.tar", last modified: Tue Apr 25 23:01:19 2023, max compression
+gzip compressed data, was "crosscompute-printers-pdf-0.4.1.tar", last modified: Thu May 11 14:13:10 2023, max compression
```

## Comparing `crosscompute-printers-pdf-0.4.0.tar` & `crosscompute-printers-pdf-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 23:01:19.337780 crosscompute-printers-pdf-0.4.0/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2022-08-29 00:24:28.000000 crosscompute-printers-pdf-0.4.0/LICENSE.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1931 2023-04-25 23:01:19.337780 crosscompute-printers-pdf-0.4.0/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)      921 2023-04-07 11:14:54.000000 crosscompute-printers-pdf-0.4.0/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 23:01:19.335780 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf/
--rw-r--r--   0 rhh       (1000) rhh       (1000)      848 2023-04-05 16:25:37.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf/__init__.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 23:01:19.336780 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf/scripts/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4460 2023-04-25 16:46:40.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf/scripts/print.js
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 23:01:19.336780 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1931 2023-04-25 23:01:19.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)      460 2023-04-25 23:01:19.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-04-25 23:01:19.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       67 2023-04-25 23:01:19.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/entry_points.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       42 2023-04-25 23:01:19.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/requires.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       26 2023-04-25 23:01:19.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/top_level.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-04-01 21:07:32.000000 crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1334 2023-04-25 23:01:19.337780 crosscompute-printers-pdf-0.4.0/setup.cfg
--rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2022-08-29 00:24:28.000000 crosscompute-printers-pdf-0.4.0/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-11 14:13:10.280563 crosscompute-printers-pdf-0.4.1/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2022-08-29 00:24:28.000000 crosscompute-printers-pdf-0.4.1/LICENSE.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1932 2023-05-11 14:13:10.280563 crosscompute-printers-pdf-0.4.1/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      921 2023-04-07 11:14:54.000000 crosscompute-printers-pdf-0.4.1/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-11 14:13:10.279563 crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      848 2023-04-05 16:25:37.000000 crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf/__init__.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-11 14:13:10.280563 crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf/scripts/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4593 2023-05-11 14:08:30.000000 crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf/scripts/print.js
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-11 14:13:10.280563 crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1932 2023-05-11 14:13:10.000000 crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      460 2023-05-11 14:13:10.000000 crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-11 14:13:10.000000 crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       67 2023-05-11 14:13:10.000000 crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf.egg-info/entry_points.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2023-05-11 14:13:10.000000 crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       26 2023-05-11 14:13:10.000000 crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-04-01 21:07:32.000000 crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1332 2023-05-11 14:13:10.281563 crosscompute-printers-pdf-0.4.1/setup.cfg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2022-08-29 00:24:28.000000 crosscompute-printers-pdf-0.4.1/setup.py
```

### Comparing `crosscompute-printers-pdf-0.4.0/LICENSE.md` & `crosscompute-printers-pdf-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crosscompute-printers-pdf-0.4.0/PKG-INFO` & `crosscompute-printers-pdf-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute-printers-pdf
-Version: 0.4.0
+Version: 0.4.1
 Summary: Print your automations in PDF format.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute-printers-pdf/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-printers-pdf
@@ -14,15 +14,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
 # PDF Printers for CrossCompute
 
 ## Installation
```

### Comparing `crosscompute-printers-pdf-0.4.0/README.md` & `crosscompute-printers-pdf-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf/__init__.py` & `crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf/scripts/print.js` & `crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf/scripts/print.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,11 @@
 'use strict';
 
+const CHROMIUM_PATH = process.env.CHROMIUM_PATH || 'chromium-browser';
+
 const fs = require('fs');
 const os = require('os');
 const path = require('path');
 
 const PDFMerger = require('pdf-merger-js');
 const express = require('express');
 const puppeteer = require('puppeteer');
@@ -35,15 +37,18 @@
         } else {
             batchDictionaries.push(batchDictionary);
         }
     }
     await browser.close();
 }
 const initialize = async () => {
-    browser = await puppeteer.launch();
+    browser = await puppeteer.launch({
+        headless: 'new',
+        executablePath: CHROMIUM_PATH,
+    });
     page = await browser.newPage();
 }
 const isReady = async (batchUri) => {
     const response = await fetch(batchUri + '/d/return_code');
     const responseText = await response.text();
     const returnCode = parseInt(responseText);
     return returnCode == 0;
```

### Comparing `crosscompute-printers-pdf-0.4.0/crosscompute_printers_pdf.egg-info/PKG-INFO` & `crosscompute-printers-pdf-0.4.1/crosscompute_printers_pdf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute-printers-pdf
-Version: 0.4.0
+Version: 0.4.1
 Summary: Print your automations in PDF format.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute-printers-pdf/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-printers-pdf
@@ -14,15 +14,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
 # PDF Printers for CrossCompute
 
 ## Installation
```

### Comparing `crosscompute-printers-pdf-0.4.0/setup.cfg` & `crosscompute-printers-pdf-0.4.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosscompute-printers-pdf
-version = 0.4.0
+version = 0.4.1
 description = Print your automations in PDF format.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://crosscompute.com
 author = CrossCompute Inc.
 author_email = support@crosscompute.com
 license = MIT
@@ -22,17 +22,17 @@
 project_urls = 
 	Bug Tracker = https://github.com/crosscompute/crosscompute-printers-pdf/issues
 	Documentation = https://github.com/crosscompute/crosscompute-printers-pdf
 	Source Code = https://github.com/crosscompute/crosscompute-printers-pdf
 
 [options]
 packages = find:
-python_requires = >=3.9
+python_requires = >=3.10
 install_requires = 
-	crosscompute>=0.9.2.10
+	crosscompute>=0.9.4
 zip_safe = True
 
 [options.package_data]
 crosscompute_printers_pdf = 
 	scripts/*.js
 
 [options.entry_points]
```

