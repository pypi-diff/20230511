# Comparing `tmp/QuickReaderPDF-0.1.1.tar.gz` & `tmp/QuickReaderPDF-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuickReaderPDF-0.1.1.tar", last modified: Tue Apr 18 19:48:34 2023, max compression
+gzip compressed data, was "QuickReaderPDF-0.1.2.tar", last modified: Thu May 11 00:53:07 2023, max compression
```

## Comparing `QuickReaderPDF-0.1.1.tar` & `QuickReaderPDF-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-04-18 19:48:34.899984 QuickReaderPDF-0.1.1/
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1069 2023-03-26 20:58:41.000000 QuickReaderPDF-0.1.1/LICENSE
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     3653 2023-04-18 19:48:34.899984 QuickReaderPDF-0.1.1/PKG-INFO
-drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-04-18 19:48:34.859984 QuickReaderPDF-0.1.1/QuickReaderPDF/
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)      125 2023-04-18 19:32:18.000000 QuickReaderPDF-0.1.1/QuickReaderPDF/__init__.py
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       99 2023-04-14 06:16:22.000000 QuickReaderPDF-0.1.1/QuickReaderPDF/__main__.py
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1993 2023-04-14 06:09:42.000000 QuickReaderPDF-0.1.1/QuickReaderPDF/pdfeditor.py
-drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-04-18 19:48:34.899984 QuickReaderPDF-0.1.1/QuickReaderPDF/tests/
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)        0 2023-04-14 06:09:42.000000 QuickReaderPDF-0.1.1/QuickReaderPDF/tests/__init__.py
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     2226 2023-04-14 06:09:42.000000 QuickReaderPDF-0.1.1/QuickReaderPDF/tests/test_all.py
-drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-04-18 19:48:34.899984 QuickReaderPDF-0.1.1/QuickReaderPDF.egg-info/
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     3653 2023-04-18 19:48:34.000000 QuickReaderPDF-0.1.1/QuickReaderPDF.egg-info/PKG-INFO
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)      378 2023-04-18 19:48:34.000000 QuickReaderPDF-0.1.1/QuickReaderPDF.egg-info/SOURCES.txt
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)        1 2023-04-18 19:48:34.000000 QuickReaderPDF-0.1.1/QuickReaderPDF.egg-info/dependency_links.txt
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)      156 2023-04-18 19:48:34.000000 QuickReaderPDF-0.1.1/QuickReaderPDF.egg-info/requires.txt
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       15 2023-04-18 19:48:34.000000 QuickReaderPDF-0.1.1/QuickReaderPDF.egg-info/top_level.txt
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1376 2023-04-18 19:02:03.000000 QuickReaderPDF-0.1.1/README.md
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     2397 2023-04-18 19:43:20.000000 QuickReaderPDF-0.1.1/pyproject.toml
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       38 2023-04-18 19:48:34.899984 QuickReaderPDF-0.1.1/setup.cfg
--rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       38 2023-04-14 06:09:42.000000 QuickReaderPDF-0.1.1/setup.py
+drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-05-11 00:53:07.428175 QuickReaderPDF-0.1.2/
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1069 2023-03-26 20:58:41.000000 QuickReaderPDF-0.1.2/LICENSE
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     3756 2023-05-11 00:53:07.428175 QuickReaderPDF-0.1.2/PKG-INFO
+drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-05-11 00:53:07.428175 QuickReaderPDF-0.1.2/QuickReaderPDF/
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)      160 2023-05-11 00:47:54.000000 QuickReaderPDF-0.1.2/QuickReaderPDF/__init__.py
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       99 2023-05-11 00:39:38.000000 QuickReaderPDF-0.1.2/QuickReaderPDF/__main__.py
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     4676 2023-05-11 00:39:38.000000 QuickReaderPDF-0.1.2/QuickReaderPDF/pdfeditor.py
+drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-05-11 00:53:07.428175 QuickReaderPDF-0.1.2/QuickReaderPDF/tests/
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)        0 2023-04-14 06:09:42.000000 QuickReaderPDF-0.1.2/QuickReaderPDF/tests/__init__.py
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     3458 2023-05-05 23:06:46.000000 QuickReaderPDF-0.1.2/QuickReaderPDF/tests/test_all.py
+drwxrwxr-x   0 shreyas   (1000) shreyas   (1000)        0 2023-05-11 00:53:07.428175 QuickReaderPDF-0.1.2/QuickReaderPDF.egg-info/
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     3756 2023-05-11 00:53:07.000000 QuickReaderPDF-0.1.2/QuickReaderPDF.egg-info/PKG-INFO
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)      378 2023-05-11 00:53:07.000000 QuickReaderPDF-0.1.2/QuickReaderPDF.egg-info/SOURCES.txt
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)        1 2023-05-11 00:53:07.000000 QuickReaderPDF-0.1.2/QuickReaderPDF.egg-info/dependency_links.txt
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)      156 2023-05-11 00:53:07.000000 QuickReaderPDF-0.1.2/QuickReaderPDF.egg-info/requires.txt
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       15 2023-05-11 00:53:07.000000 QuickReaderPDF-0.1.2/QuickReaderPDF.egg-info/top_level.txt
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     1480 2023-05-11 00:39:38.000000 QuickReaderPDF-0.1.2/README.md
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)     2397 2023-05-05 23:06:46.000000 QuickReaderPDF-0.1.2/pyproject.toml
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       38 2023-05-11 00:53:07.428175 QuickReaderPDF-0.1.2/setup.cfg
+-rw-rw-r--   0 shreyas   (1000) shreyas   (1000)       38 2023-04-14 06:09:42.000000 QuickReaderPDF-0.1.2/setup.py
```

### Comparing `QuickReaderPDF-0.1.1/LICENSE` & `QuickReaderPDF-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `QuickReaderPDF-0.1.1/PKG-INFO` & `QuickReaderPDF-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickReaderPDF
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package converts a pdf or a html file that the user wants to read to an new pdf file, which can be read faster! The idea is bionic reading, where we bold the first three letters of every word. We hope you enjoy reading your files faster!
 Author-email: Shreyas Bhat <shreyasbhat92@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Shreyas Bhat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,14 +44,16 @@
 
 License:
 ![license](https://img.shields.io/badge/license-MIT-blue)
 
 Issues:
 ![issues](https://img.shields.io/github/issues/Sbhat92/QuickReaderPDF)
 
+Pypi
+[![PyPI](https://img.shields.io/pypi/v/QuickReaderPDF)](https://pypi.org/project/QuickReaderPDF/)
 # overview
 
 Build:
 [![Linting, Testing Status](https://github.com/Sbhat92/QuickReaderPDF/actions/workflows/setup.yaml/badge.svg)](https://github.com/Sbhat92/QuickReaderPDF/actions/workflows/setup.yaml)
 
 COde coverage:
 [![Codecov](https://codecov.io/gh/Sbhat92/QuickReaderPDF/branch/main/graph/badge.svg)](https://codecov.io/gh/Sbhat92/QuickReaderPDF)
```

### Comparing `QuickReaderPDF-0.1.1/QuickReaderPDF.egg-info/PKG-INFO` & `QuickReaderPDF-0.1.2/QuickReaderPDF.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickReaderPDF
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package converts a pdf or a html file that the user wants to read to an new pdf file, which can be read faster! The idea is bionic reading, where we bold the first three letters of every word. We hope you enjoy reading your files faster!
 Author-email: Shreyas Bhat <shreyasbhat92@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Shreyas Bhat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,14 +44,16 @@
 
 License:
 ![license](https://img.shields.io/badge/license-MIT-blue)
 
 Issues:
 ![issues](https://img.shields.io/github/issues/Sbhat92/QuickReaderPDF)
 
+Pypi
+[![PyPI](https://img.shields.io/pypi/v/QuickReaderPDF)](https://pypi.org/project/QuickReaderPDF/)
 # overview
 
 Build:
 [![Linting, Testing Status](https://github.com/Sbhat92/QuickReaderPDF/actions/workflows/setup.yaml/badge.svg)](https://github.com/Sbhat92/QuickReaderPDF/actions/workflows/setup.yaml)
 
 COde coverage:
 [![Codecov](https://codecov.io/gh/Sbhat92/QuickReaderPDF/branch/main/graph/badge.svg)](https://codecov.io/gh/Sbhat92/QuickReaderPDF)
```

### Comparing `QuickReaderPDF-0.1.1/README.md` & `QuickReaderPDF-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 License:
 ![license](https://img.shields.io/badge/license-MIT-blue)
 
 Issues:
 ![issues](https://img.shields.io/github/issues/Sbhat92/QuickReaderPDF)
 
+Pypi
+[![PyPI](https://img.shields.io/pypi/v/QuickReaderPDF)](https://pypi.org/project/QuickReaderPDF/)
 # overview
 
 Build:
 [![Linting, Testing Status](https://github.com/Sbhat92/QuickReaderPDF/actions/workflows/setup.yaml/badge.svg)](https://github.com/Sbhat92/QuickReaderPDF/actions/workflows/setup.yaml)
 
 COde coverage:
 [![Codecov](https://codecov.io/gh/Sbhat92/QuickReaderPDF/branch/main/graph/badge.svg)](https://codecov.io/gh/Sbhat92/QuickReaderPDF)
@@ -33,8 +35,8 @@
 You're ready to go!
 
 ## Usage
 
 1. Open a terminal in the location of the pdf file you want. 
 2. `python <path to directory with package/pdfeditor.py> <name of existing pdf> <name of new pdf>`
 
-A new pdf file will be created!
+A new pdf file will be created!
```

### Comparing `QuickReaderPDF-0.1.1/pyproject.toml` & `QuickReaderPDF-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "QuickReaderPDF"
 authors = [{name = "Shreyas Bhat", email = "shreyasbhat92@gmail.com"}]
 description="This package converts a pdf or a html file that the user wants to read to an new pdf file, which can be read faster! The idea is bionic reading, where we bold the first three letters of every word. We hope you enjoy reading your files faster!"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

