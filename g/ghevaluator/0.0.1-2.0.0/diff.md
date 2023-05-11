# Comparing `tmp/ghevaluator-0.0.1.tar.gz` & `tmp/ghevaluator-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghevaluator-0.0.1.tar", last modified: Thu May 11 11:22:16 2023, max compression
+gzip compressed data, was "ghevaluator-2.0.0.tar", last modified: Thu May 11 14:39:26 2023, max compression
```

## Comparing `ghevaluator-0.0.1.tar` & `ghevaluator-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 11:22:16.507475 ghevaluator-0.0.1/
--rw-r--r--   0 bebatut    (502) staff       (20)     1066 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/LICENSE
--rw-r--r--   0 bebatut    (502) staff       (20)       52 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/MANIFEST.in
--rw-r--r--   0 bebatut    (502) staff       (20)     4210 2023-05-11 11:22:16.507057 ghevaluator-0.0.1/PKG-INFO
--rw-r--r--   0 bebatut    (502) staff       (20)     2250 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/README.md
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 11:22:16.448888 ghevaluator-0.0.1/docs/
--rw-r--r--   0 bebatut    (502) staff       (20)      230 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/docs/.buildinfo
--rw-r--r--   0 bebatut    (502) staff       (20)     3602 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/docs/api_documentation.html
--rw-r--r--   0 bebatut    (502) staff       (20)     9842 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/docs/contributing.html
--rw-r--r--   0 bebatut    (502) staff       (20)     3557 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/docs/genindex.html
--rw-r--r--   0 bebatut    (502) staff       (20)     5726 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/docs/index.html
--rw-r--r--   0 bebatut    (502) staff       (20)     4306 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/docs/installation.html
--rw-r--r--   0 bebatut    (502) staff       (20)      371 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/docs/objects.inv
--rw-r--r--   0 bebatut    (502) staff       (20)     3433 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/docs/py-modindex.html
--rw-r--r--   0 bebatut    (502) staff       (20)     3170 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/docs/search.html
--rw-r--r--   0 bebatut    (502) staff       (20)     5577 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/docs/searchindex.js
--rw-r--r--   0 bebatut    (502) staff       (20)     8054 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/docs/usage.html
--rw-r--r--   0 bebatut    (502) staff       (20)      927 2023-05-11 11:11:05.000000 ghevaluator-0.0.1/pyproject.toml
--rw-r--r--   0 bebatut    (502) staff       (20)       38 2023-05-11 11:22:16.511042 ghevaluator-0.0.1/setup.cfg
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 11:22:16.414236 ghevaluator-0.0.1/src/
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 11:22:16.457124 ghevaluator-0.0.1/src/docs/
--rw-r--r--   0 bebatut    (502) staff       (20)     1133 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/src/docs/conf.py
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 11:22:16.502094 ghevaluator-0.0.1/src/ghevaluator.egg-info/
--rw-r--r--   0 bebatut    (502) staff       (20)     4210 2023-05-11 11:22:16.000000 ghevaluator-0.0.1/src/ghevaluator.egg-info/PKG-INFO
--rw-r--r--   0 bebatut    (502) staff       (20)      498 2023-05-11 11:22:16.000000 ghevaluator-0.0.1/src/ghevaluator.egg-info/SOURCES.txt
--rw-r--r--   0 bebatut    (502) staff       (20)        1 2023-05-11 11:22:16.000000 ghevaluator-0.0.1/src/ghevaluator.egg-info/dependency_links.txt
--rw-r--r--   0 bebatut    (502) staff       (20)       64 2023-05-11 11:22:16.000000 ghevaluator-0.0.1/src/ghevaluator.egg-info/requires.txt
--rw-r--r--   0 bebatut    (502) staff       (20)        5 2023-05-11 11:22:16.000000 ghevaluator-0.0.1/src/ghevaluator.egg-info/top_level.txt
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 11:22:16.505803 ghevaluator-0.0.1/tests/
--rw-r--r--   0 bebatut    (502) staff       (20)     9636 2023-05-11 09:08:31.000000 ghevaluator-0.0.1/tests/test_ghevaluator.py
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.661398 ghevaluator-2.0.0/
+-rw-r--r--   0 bebatut    (502) staff       (20)     1066 2023-05-11 09:08:31.000000 ghevaluator-2.0.0/LICENSE
+-rw-r--r--   0 bebatut    (502) staff       (20)       52 2023-05-11 09:08:31.000000 ghevaluator-2.0.0/MANIFEST.in
+-rw-r--r--   0 bebatut    (502) staff       (20)     4197 2023-05-11 14:39:26.660374 ghevaluator-2.0.0/PKG-INFO
+-rw-r--r--   0 bebatut    (502) staff       (20)     2237 2023-05-11 14:38:57.000000 ghevaluator-2.0.0/README.md
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.634285 ghevaluator-2.0.0/docs/
+-rw-r--r--   0 bebatut    (502) staff       (20)      230 2023-05-11 14:26:46.000000 ghevaluator-2.0.0/docs/.buildinfo
+-rw-r--r--   0 bebatut    (502) staff       (20)        0 2023-05-11 14:35:03.000000 ghevaluator-2.0.0/docs/.nojekyll
+-rw-r--r--   0 bebatut    (502) staff       (20)     3678 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/api_documentation.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     9913 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/contributing.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     3624 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/genindex.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     5790 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/index.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     4377 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/installation.html
+-rw-r--r--   0 bebatut    (502) staff       (20)      371 2023-05-11 14:26:46.000000 ghevaluator-2.0.0/docs/objects.inv
+-rw-r--r--   0 bebatut    (502) staff       (20)     3503 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/py-modindex.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     3235 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/search.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     5577 2023-05-11 14:26:46.000000 ghevaluator-2.0.0/docs/searchindex.js
+-rw-r--r--   0 bebatut    (502) staff       (20)     8118 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/usage.html
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.645951 ghevaluator-2.0.0/ghevaluator/
+-rw-r--r--   0 bebatut    (502) staff       (20)    11385 2023-05-11 09:08:31.000000 ghevaluator-2.0.0/ghevaluator/__init__.py
+-rw-r--r--   0 bebatut    (502) staff       (20)     1241 2023-05-11 09:08:31.000000 ghevaluator-2.0.0/ghevaluator/__main__.py
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.656834 ghevaluator-2.0.0/ghevaluator.egg-info/
+-rw-r--r--   0 bebatut    (502) staff       (20)     4197 2023-05-11 14:39:26.000000 ghevaluator-2.0.0/ghevaluator.egg-info/PKG-INFO
+-rw-r--r--   0 bebatut    (502) staff       (20)      579 2023-05-11 14:39:26.000000 ghevaluator-2.0.0/ghevaluator.egg-info/SOURCES.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)        1 2023-05-11 14:39:26.000000 ghevaluator-2.0.0/ghevaluator.egg-info/dependency_links.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)       58 2023-05-11 14:39:26.000000 ghevaluator-2.0.0/ghevaluator.egg-info/entry_points.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)       18 2023-05-11 14:39:26.000000 ghevaluator-2.0.0/ghevaluator.egg-info/requires.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)       42 2023-05-11 14:39:26.000000 ghevaluator-2.0.0/ghevaluator.egg-info/top_level.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)      981 2023-05-11 14:07:39.000000 ghevaluator-2.0.0/pyproject.toml
+-rw-r--r--   0 bebatut    (502) staff       (20)       38 2023-05-11 14:39:26.661579 ghevaluator-2.0.0/setup.cfg
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.394776 ghevaluator-2.0.0/src/
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.657613 ghevaluator-2.0.0/src/docs/
+-rw-r--r--   0 bebatut    (502) staff       (20)     1115 2023-05-11 14:25:17.000000 ghevaluator-2.0.0/src/docs/conf.py
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.659678 ghevaluator-2.0.0/tests/
+-rw-r--r--   0 bebatut    (502) staff       (20)     9636 2023-05-11 09:08:31.000000 ghevaluator-2.0.0/tests/test_ghevaluator.py
```

### Comparing `ghevaluator-0.0.1/LICENSE` & `ghevaluator-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghevaluator-0.0.1/PKG-INFO` & `ghevaluator-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghevaluator
-Version: 0.0.1
+Version: 2.0.0
 Summary: A command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON report file.
 Author: Teresa Müller
 Author-email: Siyu Chen <chensy96@gmail.com>, Bérénice Batut <berenice.batut@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Siyu Chen
         
@@ -96,15 +96,15 @@
   $ make tests
   ```
 
 
 ## Documentation
 
 
-Documentation could be found at https://streetscience.community/Galaxy-History-Evaluator/
+Documentation could be found at https://streetscience.community/ghevaluator/
 
 To update it:
 
 1. Make the changes in `src/docs`
 2. Generate the doc with
 
     ```bash
```

### Comparing `ghevaluator-0.0.1/README.md` & `ghevaluator-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -58,15 +58,15 @@
   $ make tests
   ```
 
 
 ## Documentation
 
 
-Documentation could be found at https://streetscience.community/Galaxy-History-Evaluator/
+Documentation could be found at https://streetscience.community/ghevaluator/
 
 To update it:
 
 1. Make the changes in `src/docs`
 2. Generate the doc with
 
     ```bash
```

### Comparing `ghevaluator-0.0.1/docs/api_documentation.html` & `ghevaluator-2.0.0/docs/api_documentation.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>API documentation &#8212; Galaxy History Evaluator  documentation</title>
+    <title>API documentation &#8212; Galaxy History Evaluator 2.0.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
+    <link rel="canonical" href="/ghevaluator/api_documentation.html" />
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Contributing" href="contributing.html" />
     <link rel="prev" title="Installation" href="installation.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
@@ -93,15 +93,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2022, Siyu Chen, Teresa Müller, Bérénice Batut.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 6.1.3</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/api_documentation.rst.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -18,9 +18,9 @@
     * Contributing
 **** Related Topics ****
     * Documentation_overview
           o Previous: Installation
           o Next: Contributing
 **** Quick search ****
 [q                   ] [Go]
-©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_6.1.3 &
+©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_7.0.0 &
 Alabaster_0.7.13 | Page_source
```

### Comparing `ghevaluator-0.0.1/docs/contributing.html` & `ghevaluator-2.0.0/docs/contributing.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Contributing &#8212; Galaxy History Evaluator  documentation</title>
+    <title>Contributing &#8212; Galaxy History Evaluator 2.0.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
+    <link rel="canonical" href="/ghevaluator/contributing.html" />
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="prev" title="API documentation" href="api_documentation.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
   
@@ -171,15 +171,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2022, Siyu Chen, Teresa Müller, Bérénice Batut.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 6.1.3</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/contributing.rst.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -92,9 +92,9 @@
           o Tests
           o Documentation
 **** Related Topics ****
     * Documentation_overview
           o Previous: API_documentation
 **** Quick search ****
 [q                   ] [Go]
-©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_6.1.3 &
+©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_7.0.0 &
 Alabaster_0.7.13 | Page_source
```

### Comparing `ghevaluator-0.0.1/docs/genindex.html` & `ghevaluator-2.0.0/docs/genindex.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; Galaxy History Evaluator  documentation</title>
+    <title>Index &#8212; Galaxy History Evaluator 2.0.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
+    <link rel="canonical" href="/ghevaluator/genindex.html" />
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
   
   <meta name="viewport" content="width=device-width, initial-scale=0.9, maximum-scale=0.9" />
@@ -118,15 +118,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2022, Siyu Chen, Teresa Müller, Bérénice Batut.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 6.1.3</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
     </div>
```

#### html2text {}

```diff
@@ -20,9 +20,9 @@
     * Installation
     * API_documentation
     * Contributing
 **** Related Topics ****
     * Documentation_overview
 **** Quick search ****
 [q                   ] [Go]
-©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_6.1.3 &
+©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_7.0.0 &
 Alabaster_0.7.13
```

### Comparing `ghevaluator-0.0.1/docs/index.html` & `ghevaluator-2.0.0/docs/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Welcome to Galaxy History Evaluator’s documentation! &#8212; Galaxy History Evaluator  documentation</title>
+    <title>Welcome to Galaxy History Evaluator’s documentation! &#8212; Galaxy History Evaluator 2.0.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
+    <link rel="canonical" href="/ghevaluator/index.html" />
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Usage" href="usage.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
   
@@ -122,15 +122,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2022, Siyu Chen, Teresa Müller, Bérénice Batut.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 6.1.3</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/index.rst.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -36,9 +36,9 @@
     * API_documentation
     * Contributing
 **** Related Topics ****
     * Documentation_overview
           o Next: Usage
 **** Quick search ****
 [q                   ] [Go]
-©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_6.1.3 &
+©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_7.0.0 &
 Alabaster_0.7.13 | Page_source
```

### Comparing `ghevaluator-0.0.1/docs/installation.html` & `ghevaluator-2.0.0/docs/installation.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Installation &#8212; Galaxy History Evaluator  documentation</title>
+    <title>Installation &#8212; Galaxy History Evaluator 2.0.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
+    <link rel="canonical" href="/ghevaluator/installation.html" />
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="API documentation" href="api_documentation.html" />
     <link rel="prev" title="Usage" href="usage.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
@@ -109,15 +109,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2022, Siyu Chen, Teresa Müller, Bérénice Batut.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 6.1.3</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/installation.rst.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -26,9 +26,9 @@
     * Contributing
 **** Related Topics ****
     * Documentation_overview
           o Previous: Usage
           o Next: API_documentation
 **** Quick search ****
 [q                   ] [Go]
-©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_6.1.3 &
+©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_7.0.0 &
 Alabaster_0.7.13 | Page_source
```

### Comparing `ghevaluator-0.0.1/docs/py-modindex.html` & `ghevaluator-2.0.0/docs/py-modindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; Galaxy History Evaluator  documentation</title>
+    <title>Python Module Index &#8212; Galaxy History Evaluator 2.0.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
+    <link rel="canonical" href="/ghevaluator/py-modindex.html" />
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
 
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
   
@@ -108,15 +108,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2022, Siyu Chen, Teresa Müller, Bérénice Batut.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 6.1.3</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
     </div>
```

#### html2text {}

```diff
@@ -17,9 +17,9 @@
     * Installation
     * API_documentation
     * Contributing
 **** Related Topics ****
     * Documentation_overview
 **** Quick search ****
 [q                   ] [Go]
-©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_6.1.3 &
+©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_7.0.0 &
 Alabaster_0.7.13
```

### Comparing `ghevaluator-0.0.1/docs/search.html` & `ghevaluator-2.0.0/docs/search.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; Galaxy History Evaluator  documentation</title>
+    <title>Search &#8212; Galaxy History Evaluator 2.0.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
+    <link rel="canonical" href="/ghevaluator/search.html" />
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
   <script src="searchindex.js" defer></script>
   
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
@@ -109,15 +109,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2022, Siyu Chen, Teresa Müller, Bérénice Batut.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 6.1.3</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
     </div>
```

#### html2text {}

```diff
@@ -14,9 +14,9 @@
 Contents:
     * Usage
     * Installation
     * API_documentation
     * Contributing
 **** Related Topics ****
     * Documentation_overview
-©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_6.1.3 &
+©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_7.0.0 &
 Alabaster_0.7.13
```

### Comparing `ghevaluator-0.0.1/docs/searchindex.js` & `ghevaluator-2.0.0/docs/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -318,41 +318,17 @@
         "sphinx.domains.math": 2,
         "sphinx.domains.python": 3,
         "sphinx.domains.rst": 2,
         "sphinx.domains.std": 2,
         "sphinx": 57
     },
     "alltitles": {
-        "Welcome to Galaxy History Evaluator\u2019s documentation!": [
-            [2, "welcome-to-galaxy-history-evaluator-s-documentation"]
-        ],
-        "Contents:": [
-            [2, null]
-        ],
-        "Indices and tables": [
-            [2, "indices-and-tables"]
-        ],
-        "Installation": [
-            [3, "installation"]
-        ],
-        "Requirements": [
-            [3, "requirements"]
-        ],
-        "Installation via pip": [
-            [3, "installation-via-pip"]
-        ],
         "API documentation": [
             [0, "module-__main__"]
         ],
-        "Usage": [
-            [4, "usage"]
-        ],
-        "Output": [
-            [4, "output"]
-        ],
         "Contributing": [
             [1, "contributing"]
         ],
         "What should I know before I get started?": [
             [1, "what-should-i-know-before-i-get-started"]
         ],
         "How can I contribute?": [
@@ -368,14 +344,38 @@
             [1, "development"]
         ],
         "Tests": [
             [1, "tests"]
         ],
         "Documentation": [
             [1, "documentation"]
+        ],
+        "Welcome to Galaxy History Evaluator\u2019s documentation!": [
+            [2, "welcome-to-galaxy-history-evaluator-s-documentation"]
+        ],
+        "Contents:": [
+            [2, null]
+        ],
+        "Indices and tables": [
+            [2, "indices-and-tables"]
+        ],
+        "Installation": [
+            [3, "installation"]
+        ],
+        "Requirements": [
+            [3, "requirements"]
+        ],
+        "Installation via pip": [
+            [3, "installation-via-pip"]
+        ],
+        "Usage": [
+            [4, "usage"]
+        ],
+        "Output": [
+            [4, "output"]
         ]
     },
     "indexentries": {
         "__main__": [
             [0, "module-__main__"]
         ],
         "module": [
```

### Comparing `ghevaluator-0.0.1/docs/usage.html` & `ghevaluator-2.0.0/docs/usage.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Usage &#8212; Galaxy History Evaluator  documentation</title>
+    <title>Usage &#8212; Galaxy History Evaluator 2.0.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
+    <link rel="canonical" href="/ghevaluator/usage.html" />
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Installation" href="installation.html" />
     <link rel="prev" title="Welcome to Galaxy History Evaluator’s documentation!" href="index.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
@@ -141,15 +141,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2022, Siyu Chen, Teresa Müller, Bérénice Batut.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 6.1.3</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/usage.rst.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -57,9 +57,9 @@
     * Contributing
 **** Related Topics ****
     * Documentation_overview
           o Previous: Welcome_to_Galaxy_History_Evaluatorâs_documentation!
           o Next: Installation
 **** Quick search ****
 [q                   ] [Go]
-©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_6.1.3 &
+©2022, Siyu Chen, Teresa MÃ¼ller, BÃ©rÃ©nice Batut. | Powered by Sphinx_7.0.0 &
 Alabaster_0.7.13 | Page_source
```

### Comparing `ghevaluator-0.0.1/pyproject.toml` & `ghevaluator-2.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghevaluator"
-version = "0.0.1"
+version = "2.0.0"
 authors = [
   { name="Siyu Chen", email="chensy96@gmail.com" },
   { name="Teresa Müller" },
   { name="Bérénice Batut", email="berenice.batut@gmail.com" },
 ]
 description = "A command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON report file."
 readme = "README.md"
@@ -16,17 +16,23 @@
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering"
 ]
 
 dependencies = [
     "bioblend",
     "requests",
-    'importlib-metadata; python_version<"3.8"',
 ]
 
+[project.scripts]
+ghevaluator = "ghevaluator.__main__:main"
+
 [project.urls]
 repository = "https://github.com/SteetScienceCommunity/ghevaluator"
 documentation = "https://streetscience.community/ghevaluator/"
 
 [build-system]
 requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages]
+find = {} 
+
```

### Comparing `ghevaluator-0.0.1/src/docs/conf.py` & `ghevaluator-2.0.0/src/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # Configuration file for the Sphinx documentation builder.
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
-import os
-import sys
-sys.path.insert(0, os.path.abspath('..'))
-
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Galaxy History Evaluator'
 copyright = '2022, Siyu Chen, Teresa Müller, Bérénice Batut'
 author = 'Siyu Chen, Teresa Müller, Bérénice Batut'
+release = '2.0.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc']
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'alabaster'
 html_static_path = ['_static']
+html_baseurl = '/ghevaluator'
```

### Comparing `ghevaluator-0.0.1/src/ghevaluator.egg-info/PKG-INFO` & `ghevaluator-2.0.0/ghevaluator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghevaluator
-Version: 0.0.1
+Version: 2.0.0
 Summary: A command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON report file.
 Author: Teresa Müller
 Author-email: Siyu Chen <chensy96@gmail.com>, Bérénice Batut <berenice.batut@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Siyu Chen
         
@@ -96,15 +96,15 @@
   $ make tests
   ```
 
 
 ## Documentation
 
 
-Documentation could be found at https://streetscience.community/Galaxy-History-Evaluator/
+Documentation could be found at https://streetscience.community/ghevaluator/
 
 To update it:
 
 1. Make the changes in `src/docs`
 2. Generate the doc with
 
     ```bash
```

### Comparing `ghevaluator-0.0.1/tests/test_ghevaluator.py` & `ghevaluator-2.0.0/tests/test_ghevaluator.py`

 * *Files identical despite different names*

