# Comparing `tmp/bfgdealer-0.0.4.tar.gz` & `tmp/bfgdealer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgdealer-0.0.4.tar", last modified: Fri May  5 16:15:21 2023, max compression
+gzip compressed data, was "bfgdealer-0.0.5.tar", last modified: Thu May 11 08:39:16 2023, max compression
```

## Comparing `bfgdealer-0.0.4.tar` & `bfgdealer-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-05 16:15:21.921491 bfgdealer-0.0.4/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgdealer-0.0.4/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)      898 2023-05-05 16:15:21.921491 bfgdealer-0.0.4/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      141 2023-02-01 12:53:56.000000 bfgdealer-0.0.4/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-05 16:15:21.918158 bfgdealer-0.0.4/bfgdealer/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      395 2023-02-01 12:53:06.000000 bfgdealer-0.0.4/bfgdealer/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       31 2023-05-05 16:12:36.000000 bfgdealer-0.0.4/bfgdealer/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-05 16:15:21.921491 bfgdealer-0.0.4/bfgdealer/source/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-01-30 17:36:30.000000 bfgdealer-0.0.4/bfgdealer/source/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    20266 2023-05-05 16:12:36.000000 bfgdealer-0.0.4/bfgdealer/source/board.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    10586 2023-05-05 16:12:36.000000 bfgdealer-0.0.4/bfgdealer/source/dealer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    27456 2023-05-05 16:12:36.000000 bfgdealer-0.0.4/bfgdealer/source/dealer_duo.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17454 2023-02-01 13:02:59.000000 bfgdealer-0.0.4/bfgdealer/source/dealer_engine.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    14324 2023-05-05 16:12:36.000000 bfgdealer-0.0.4/bfgdealer/source/dealer_solo.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-05 16:15:21.918158 bfgdealer-0.0.4/bfgdealer.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      898 2023-05-05 16:15:21.000000 bfgdealer-0.0.4/bfgdealer.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      395 2023-05-05 16:15:21.000000 bfgdealer-0.0.4/bfgdealer.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-05 16:15:21.000000 bfgdealer-0.0.4/bfgdealer.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-05-05 16:15:21.000000 bfgdealer-0.0.4/bfgdealer.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-05 16:15:21.921491 bfgdealer-0.0.4/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1186 2023-02-01 12:55:15.000000 bfgdealer-0.0.4/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:39:16.063919 bfgdealer-0.0.5/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgdealer-0.0.5/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      980 2023-05-11 08:39:16.063919 bfgdealer-0.0.5/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      141 2023-02-01 12:53:56.000000 bfgdealer-0.0.5/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:39:16.057252 bfgdealer-0.0.5/bfgdealer/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      548 2023-05-11 08:35:00.000000 bfgdealer-0.0.5/bfgdealer/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-11 08:37:22.000000 bfgdealer-0.0.5/bfgdealer/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:39:16.060586 bfgdealer-0.0.5/bfgdealer/source/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-01-30 17:36:30.000000 bfgdealer-0.0.5/bfgdealer/source/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    20266 2023-05-05 16:12:36.000000 bfgdealer-0.0.5/bfgdealer/source/board.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    10586 2023-05-05 16:12:36.000000 bfgdealer-0.0.5/bfgdealer/source/dealer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    27456 2023-05-05 16:12:36.000000 bfgdealer-0.0.5/bfgdealer/source/dealer_duo.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17454 2023-02-01 13:02:59.000000 bfgdealer-0.0.5/bfgdealer/source/dealer_engine.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    14324 2023-05-05 16:12:36.000000 bfgdealer-0.0.5/bfgdealer/source/dealer_solo.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:39:16.060586 bfgdealer-0.0.5/bfgdealer.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      980 2023-05-11 08:39:15.000000 bfgdealer-0.0.5/bfgdealer.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      395 2023-05-11 08:39:15.000000 bfgdealer-0.0.5/bfgdealer.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-11 08:39:15.000000 bfgdealer-0.0.5/bfgdealer.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-05-11 08:39:15.000000 bfgdealer-0.0.5/bfgdealer.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-11 08:39:16.063919 bfgdealer-0.0.5/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1186 2023-02-01 12:55:15.000000 bfgdealer-0.0.5/setup.py
```

### Comparing `bfgdealer-0.0.4/LICENSE.txt` & `bfgdealer-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.4/PKG-INFO` & `bfgdealer-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgdealer
-Version: 0.0.4
+Version: 0.0.5
 Summary: """A collection of modules that supports dealing Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, dealing
@@ -20,14 +20,20 @@
 ```bash
 pip install bfgdealer
 ```
 
 
 # Version History
 
+
+Version 0.0.5 11 May 2023
+
+1. Change __init__ to reflect set hand defn__
+
+------
 Version 0.0.4 05 May 2023
 
 1. Change set hands defn
 
 ------
 
 Version 0.0.3 14 Mar 2023
```

### Comparing `bfgdealer-0.0.4/bfgdealer/source/board.py` & `bfgdealer-0.0.5/bfgdealer/source/board.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.4/bfgdealer/source/dealer.py` & `bfgdealer-0.0.5/bfgdealer/source/dealer.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.4/bfgdealer/source/dealer_duo.py` & `bfgdealer-0.0.5/bfgdealer/source/dealer_duo.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.4/bfgdealer/source/dealer_engine.py` & `bfgdealer-0.0.5/bfgdealer/source/dealer_engine.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.4/bfgdealer/source/dealer_solo.py` & `bfgdealer-0.0.5/bfgdealer/source/dealer_solo.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.4/bfgdealer.egg-info/PKG-INFO` & `bfgdealer-0.0.5/bfgdealer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgdealer
-Version: 0.0.4
+Version: 0.0.5
 Summary: """A collection of modules that supports dealing Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, dealing
@@ -20,14 +20,20 @@
 ```bash
 pip install bfgdealer
 ```
 
 
 # Version History
 
+
+Version 0.0.5 11 May 2023
+
+1. Change __init__ to reflect set hand defn__
+
+------
 Version 0.0.4 05 May 2023
 
 1. Change set hands defn
 
 ------
 
 Version 0.0.3 14 Mar 2023
```

### Comparing `bfgdealer-0.0.4/setup.py` & `bfgdealer-0.0.5/setup.py`

 * *Files identical despite different names*

