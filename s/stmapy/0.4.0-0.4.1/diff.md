# Comparing `tmp/stmapy-0.4.0.tar.gz` & `tmp/stmapy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stmapy-0.4.0.tar", last modified: Wed May 10 21:59:22 2023, max compression
+gzip compressed data, was "stmapy-0.4.1.tar", last modified: Wed May 10 23:29:05 2023, max compression
```

## Comparing `stmapy-0.4.0.tar` & `stmapy-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 florie    (1000) florie    (1000)        0 2023-05-10 21:59:22.818124 stmapy-0.4.0/
--rwxrwxr-x   0 florie    (1000) florie    (1000)     1068 2023-05-09 15:53:34.000000 stmapy-0.4.0/LICENSE
--rw-rw-r--   0 florie    (1000) florie    (1000)    11514 2023-05-10 21:59:22.818124 stmapy-0.4.0/PKG-INFO
--rwxrwxr-x   0 florie    (1000) florie    (1000)    10854 2023-05-10 18:55:57.000000 stmapy-0.4.0/README.md
--rw-rw-r--   0 florie    (1000) florie    (1000)       38 2023-05-10 21:59:22.818124 stmapy-0.4.0/setup.cfg
--rwxrwxr-x   0 florie    (1000) florie    (1000)     1189 2023-05-10 18:19:25.000000 stmapy-0.4.0/setup.py
-drwxrwxr-x   0 florie    (1000) florie    (1000)        0 2023-05-10 21:59:22.818124 stmapy-0.4.0/stmapy/
--rwxrwxr-x   0 florie    (1000) florie    (1000)      135 2023-05-10 18:46:50.000000 stmapy-0.4.0/stmapy/__init__.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)       22 2023-05-10 18:48:23.000000 stmapy-0.4.0/stmapy/_version.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)    61077 2023-05-10 18:51:17.000000 stmapy-0.4.0/stmapy/citswidget.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)      398 2023-05-10 18:46:15.000000 stmapy-0.4.0/stmapy/main.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)      312 2023-05-10 18:44:29.000000 stmapy-0.4.0/stmapy/matplotlibwidget.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)     3468 2023-05-10 18:44:29.000000 stmapy-0.4.0/stmapy/plotting.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)     9883 2023-05-10 18:44:29.000000 stmapy-0.4.0/stmapy/processing.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)    32334 2023-05-10 18:47:33.000000 stmapy-0.4.0/stmapy/reads.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)     5877 2023-05-10 18:44:29.000000 stmapy-0.4.0/stmapy/shape.py
-drwxrwxr-x   0 florie    (1000) florie    (1000)        0 2023-05-10 21:59:22.818124 stmapy-0.4.0/stmapy.egg-info/
--rw-rw-r--   0 florie    (1000) florie    (1000)    11514 2023-05-10 21:59:22.000000 stmapy-0.4.0/stmapy.egg-info/PKG-INFO
--rw-rw-r--   0 florie    (1000) florie    (1000)      381 2023-05-10 21:59:22.000000 stmapy-0.4.0/stmapy.egg-info/SOURCES.txt
--rw-rw-r--   0 florie    (1000) florie    (1000)        1 2023-05-10 21:59:22.000000 stmapy-0.4.0/stmapy.egg-info/dependency_links.txt
--rw-rw-r--   0 florie    (1000) florie    (1000)       44 2023-05-10 21:59:22.000000 stmapy-0.4.0/stmapy.egg-info/entry_points.txt
--rw-rw-r--   0 florie    (1000) florie    (1000)       40 2023-05-10 21:59:22.000000 stmapy-0.4.0/stmapy.egg-info/requires.txt
--rw-rw-r--   0 florie    (1000) florie    (1000)        7 2023-05-10 21:59:22.000000 stmapy-0.4.0/stmapy.egg-info/top_level.txt
+drwxrwxr-x   0 florie    (1000) florie    (1000)        0 2023-05-10 23:29:05.781658 stmapy-0.4.1/
+-rwxrwxr-x   0 florie    (1000) florie    (1000)     1068 2023-05-10 22:09:35.000000 stmapy-0.4.1/LICENSE
+-rw-rw-r--   0 florie    (1000) florie    (1000)    11514 2023-05-10 23:29:05.781658 stmapy-0.4.1/PKG-INFO
+-rwxrwxr-x   0 florie    (1000) florie    (1000)    10854 2023-05-10 22:09:35.000000 stmapy-0.4.1/README.md
+-rw-rw-r--   0 florie    (1000) florie    (1000)       38 2023-05-10 23:29:05.781658 stmapy-0.4.1/setup.cfg
+-rwxrwxr-x   0 florie    (1000) florie    (1000)     1515 2023-05-10 23:26:39.000000 stmapy-0.4.1/setup.py
+drwxrwxr-x   0 florie    (1000) florie    (1000)        0 2023-05-10 23:29:05.777658 stmapy-0.4.1/stmapy/
+-rwxrwxr-x   0 florie    (1000) florie    (1000)      135 2023-05-10 22:09:35.000000 stmapy-0.4.1/stmapy/__init__.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)       22 2023-05-10 23:26:54.000000 stmapy-0.4.1/stmapy/_version.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)    61077 2023-05-10 22:09:35.000000 stmapy-0.4.1/stmapy/citswidget.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)      398 2023-05-10 22:09:35.000000 stmapy-0.4.1/stmapy/main.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)      312 2023-05-10 22:09:35.000000 stmapy-0.4.1/stmapy/matplotlibwidget.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)     3468 2023-05-10 22:09:35.000000 stmapy-0.4.1/stmapy/plotting.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)     9883 2023-05-10 22:09:35.000000 stmapy-0.4.1/stmapy/processing.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)    32334 2023-05-10 22:09:35.000000 stmapy-0.4.1/stmapy/reads.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)     5877 2023-05-10 22:09:35.000000 stmapy-0.4.1/stmapy/shape.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)    38217 2023-05-10 22:09:35.000000 stmapy-0.4.1/stmapy/ui_citswidget.ui
+drwxrwxr-x   0 florie    (1000) florie    (1000)        0 2023-05-10 23:29:05.781658 stmapy-0.4.1/stmapy.egg-info/
+-rw-rw-r--   0 florie    (1000) florie    (1000)    11514 2023-05-10 23:29:05.000000 stmapy-0.4.1/stmapy.egg-info/PKG-INFO
+-rw-rw-r--   0 florie    (1000) florie    (1000)      405 2023-05-10 23:29:05.000000 stmapy-0.4.1/stmapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 florie    (1000) florie    (1000)        1 2023-05-10 23:29:05.000000 stmapy-0.4.1/stmapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 florie    (1000) florie    (1000)       89 2023-05-10 23:29:05.000000 stmapy-0.4.1/stmapy.egg-info/entry_points.txt
+-rw-rw-r--   0 florie    (1000) florie    (1000)       40 2023-05-10 23:29:05.000000 stmapy-0.4.1/stmapy.egg-info/requires.txt
+-rw-rw-r--   0 florie    (1000) florie    (1000)        7 2023-05-10 23:29:05.000000 stmapy-0.4.1/stmapy.egg-info/top_level.txt
```

### Comparing `stmapy-0.4.0/LICENSE` & `stmapy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.0/PKG-INFO` & `stmapy-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stmapy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Scanning tunneling microscopy analysis in Python
 Home-page: https://gitlab.com/lateqs/stmapy
 Author-email: loic.huder@gmail.com, florie.mesple@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `stmapy-0.4.0/README.md` & `stmapy-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.0/stmapy/citswidget.py` & `stmapy-0.4.1/stmapy/citswidget.py`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.0/stmapy/plotting.py` & `stmapy-0.4.1/stmapy/plotting.py`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.0/stmapy/processing.py` & `stmapy-0.4.1/stmapy/processing.py`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.0/stmapy/reads.py` & `stmapy-0.4.1/stmapy/reads.py`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.0/stmapy/shape.py` & `stmapy-0.4.1/stmapy/shape.py`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.0/stmapy.egg-info/PKG-INFO` & `stmapy-0.4.1/stmapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stmapy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Scanning tunneling microscopy analysis in Python
 Home-page: https://gitlab.com/lateqs/stmapy
 Author-email: loic.huder@gmail.com, florie.mesple@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

