# Comparing `tmp/alacorder-80.3.6.tar.gz` & `tmp/alacorder-80.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.3.6.tar", max compression
+gzip compressed data, was "alacorder-80.3.7.tar", max compression
```

## Comparing `alacorder-80.3.6.tar` & `alacorder-80.3.7.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.6/LICENSE
--rw-r--r--   0        0        0     6538 2023-05-09 14:42:24.077836 alacorder-80.3.6/README.md
--rw-r--r--   0        0        0      697 2023-05-10 17:48:38.930662 alacorder-80.3.6/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-09 14:49:08.351375 alacorder-80.3.6/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.6/src/alacorder/__init__.py
--rw-r--r--   0        0        0   210898 2023-05-10 17:48:13.766329 alacorder-80.3.6/src/alacorder/__main__.py
--rw-r--r--   0        0        0   210898 2023-05-10 17:47:57.031458 alacorder-80.3.6/src/alacorder/alac.py
--rw-r--r--   0        0        0     7467 1970-01-01 00:00:00.000000 alacorder-80.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.7/LICENSE
+-rw-r--r--   0        0        0     6538 2023-05-09 14:42:24.077836 alacorder-80.3.7/README.md
+-rw-r--r--   0        0        0      697 2023-05-10 22:46:53.867967 alacorder-80.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.7/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   210898 2023-05-10 22:45:11.591026 alacorder-80.3.7/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   210898 2023-05-10 22:45:05.975144 alacorder-80.3.7/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7467 1970-01-01 00:00:00.000000 alacorder-80.3.7/PKG-INFO
```

### Comparing `alacorder-80.3.6/LICENSE` & `alacorder-80.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.6/README.md` & `alacorder-80.3.7/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.6/pyproject.toml` & `alacorder-80.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.3.6"
+version = "80.3.7"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.3.6/src/alacorder/__main__.py` & `alacorder-80.3.7/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.6"
+version = "80.3.7"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3240,15 +3240,15 @@
                 for x, url in enumerate(results):
                     window.write_event_value("PROGRESS-TEXT", x + 1)
                     downloadPDF(driver, url)
             else:
                 for x, url in enumerate(tqdm(results)):
                     downloadPDF(driver, url)
             query[i, "CASES_FOUND"] = len(results)
-            query[i, "RETRIEVED"] = datetime.now().strftime("%H:%M:%S %d-%m-%Y")
+            query[i, "RETRIEVED"] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
             query[i, "QUERY_COMPLETE"] = "Y"
             if not no_update:
                 qwrite = query.drop(
                     "TEMP_NAME",
                     "TEMP_PARTY_TYPE",
                     "TEMP_SSN",
                     "TEMP_DOB",
```

### Comparing `alacorder-80.3.6/src/alacorder/alac.py` & `alacorder-80.3.7/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.6"
+version = "80.3.7"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3240,15 +3240,15 @@
                 for x, url in enumerate(results):
                     window.write_event_value("PROGRESS-TEXT", x + 1)
                     downloadPDF(driver, url)
             else:
                 for x, url in enumerate(tqdm(results)):
                     downloadPDF(driver, url)
             query[i, "CASES_FOUND"] = len(results)
-            query[i, "RETRIEVED"] = datetime.now().strftime("%H:%M:%S %d-%m-%Y")
+            query[i, "RETRIEVED"] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
             query[i, "QUERY_COMPLETE"] = "Y"
             if not no_update:
                 qwrite = query.drop(
                     "TEMP_NAME",
                     "TEMP_PARTY_TYPE",
                     "TEMP_SSN",
                     "TEMP_DOB",
```

### Comparing `alacorder-80.3.6/PKG-INFO` & `alacorder-80.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.3.6
+Version: 80.3.7
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

