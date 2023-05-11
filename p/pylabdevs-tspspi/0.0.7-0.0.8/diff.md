# Comparing `tmp/pylabdevs-tspspi-0.0.7.tar.gz` & `tmp/pylabdevs-tspspi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylabdevs-tspspi-0.0.7.tar", last modified: Mon Feb 20 12:26:48 2023, max compression
+gzip compressed data, was "pylabdevs-tspspi-0.0.8.tar", last modified: Thu May 11 10:53:01 2023, max compression
```

## Comparing `pylabdevs-tspspi-0.0.7.tar` & `pylabdevs-tspspi-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2023-02-20 12:26:48.655453 pylabdevs-tspspi-0.0.7/
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     1410 2023-02-20 12:26:06.000000 pylabdevs-tspspi-0.0.7/LICENSE.md
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     1452 2023-02-20 12:26:48.655546 pylabdevs-tspspi-0.0.7/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     1014 2023-02-20 12:26:06.000000 pylabdevs-tspspi-0.0.7/README.md
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)      183 2023-02-20 12:26:06.000000 pylabdevs-tspspi-0.0.7/pyproject.toml
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)      592 2023-02-20 12:26:48.656046 pylabdevs-tspspi-0.0.7/setup.cfg
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2023-02-20 12:26:48.649921 pylabdevs-tspspi-0.0.7/src/
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2023-02-20 12:26:48.651976 pylabdevs-tspspi-0.0.7/src/labdevices/
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)      300 2023-02-20 12:26:06.000000 pylabdevs-tspspi-0.0.7/src/labdevices/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)      252 2023-02-20 12:26:06.000000 pylabdevs-tspspi-0.0.7/src/labdevices/exceptions.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)    19231 2023-02-20 12:26:06.000000 pylabdevs-tspspi-0.0.7/src/labdevices/functiongenerator.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     3262 2023-02-20 12:26:06.000000 pylabdevs-tspspi-0.0.7/src/labdevices/gcodedevice.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)    16464 2023-02-20 12:26:06.000000 pylabdevs-tspspi-0.0.7/src/labdevices/oscilloscope.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     6317 2023-02-20 12:26:06.000000 pylabdevs-tspspi-0.0.7/src/labdevices/powersupply.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     3884 2023-02-20 12:26:06.000000 pylabdevs-tspspi-0.0.7/src/labdevices/serialringbuffer.py
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2023-02-20 12:26:48.655313 pylabdevs-tspspi-0.0.7/src/pylabdevs_tspspi.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     1452 2023-02-20 12:26:48.000000 pylabdevs-tspspi-0.0.7/src/pylabdevs_tspspi.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)      482 2023-02-20 12:26:48.000000 pylabdevs-tspspi-0.0.7/src/pylabdevs_tspspi.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)        1 2023-02-20 12:26:48.000000 pylabdevs-tspspi-0.0.7/src/pylabdevs_tspspi.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)       14 2023-02-20 12:26:48.000000 pylabdevs-tspspi-0.0.7/src/pylabdevs_tspspi.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)       11 2023-02-20 12:26:48.000000 pylabdevs-tspspi-0.0.7/src/pylabdevs_tspspi.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2023-05-11 10:53:01.944770 pylabdevs-tspspi-0.0.8/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     1410 2023-05-11 10:52:27.000000 pylabdevs-tspspi-0.0.8/LICENSE.md
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     1452 2023-05-11 10:53:01.944853 pylabdevs-tspspi-0.0.8/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     1014 2023-05-11 10:52:27.000000 pylabdevs-tspspi-0.0.8/README.md
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)      183 2023-05-11 10:52:27.000000 pylabdevs-tspspi-0.0.8/pyproject.toml
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)      592 2023-05-11 10:53:01.945330 pylabdevs-tspspi-0.0.8/setup.cfg
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2023-05-11 10:53:01.941512 pylabdevs-tspspi-0.0.8/src/
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2023-05-11 10:53:01.943746 pylabdevs-tspspi-0.0.8/src/labdevices/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)      300 2023-05-11 10:52:27.000000 pylabdevs-tspspi-0.0.8/src/labdevices/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)      252 2023-05-11 10:52:27.000000 pylabdevs-tspspi-0.0.8/src/labdevices/exceptions.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)    19231 2023-05-11 10:52:27.000000 pylabdevs-tspspi-0.0.8/src/labdevices/functiongenerator.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     3262 2023-05-11 10:52:27.000000 pylabdevs-tspspi-0.0.8/src/labdevices/gcodedevice.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)    16464 2023-05-11 10:52:27.000000 pylabdevs-tspspi-0.0.8/src/labdevices/oscilloscope.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     6317 2023-05-11 10:52:27.000000 pylabdevs-tspspi-0.0.8/src/labdevices/powersupply.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     3670 2023-05-11 10:52:27.000000 pylabdevs-tspspi-0.0.8/src/labdevices/pressuregauge.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     3884 2023-05-11 10:52:27.000000 pylabdevs-tspspi-0.0.8/src/labdevices/serialringbuffer.py
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2023-05-11 10:53:01.944641 pylabdevs-tspspi-0.0.8/src/pylabdevs_tspspi.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     1452 2023-05-11 10:53:01.000000 pylabdevs-tspspi-0.0.8/src/pylabdevs_tspspi.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)      514 2023-05-11 10:53:01.000000 pylabdevs-tspspi-0.0.8/src/pylabdevs_tspspi.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)        1 2023-05-11 10:53:01.000000 pylabdevs-tspspi-0.0.8/src/pylabdevs_tspspi.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)       14 2023-05-11 10:53:01.000000 pylabdevs-tspspi-0.0.8/src/pylabdevs_tspspi.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)       11 2023-05-11 10:53:01.000000 pylabdevs-tspspi-0.0.8/src/pylabdevs_tspspi.egg-info/top_level.txt
```

### Comparing `pylabdevs-tspspi-0.0.7/LICENSE.md` & `pylabdevs-tspspi-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pylabdevs-tspspi-0.0.7/PKG-INFO` & `pylabdevs-tspspi-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylabdevs-tspspi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Lab devices base classes
 Home-page: https://github.com/tspspi/pylabdevs
 Author: Thomas Spielauer
 Author-email: pypipackages01@tspi.at
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pylabdevs-tspspi-0.0.7/README.md` & `pylabdevs-tspspi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pylabdevs-tspspi-0.0.7/setup.cfg` & `pylabdevs-tspspi-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylabdevs-tspspi-0.0.7/src/labdevices/functiongenerator.py` & `pylabdevs-tspspi-0.0.8/src/labdevices/functiongenerator.py`

 * *Files identical despite different names*

### Comparing `pylabdevs-tspspi-0.0.7/src/labdevices/gcodedevice.py` & `pylabdevs-tspspi-0.0.8/src/labdevices/gcodedevice.py`

 * *Files identical despite different names*

### Comparing `pylabdevs-tspspi-0.0.7/src/labdevices/oscilloscope.py` & `pylabdevs-tspspi-0.0.8/src/labdevices/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `pylabdevs-tspspi-0.0.7/src/labdevices/powersupply.py` & `pylabdevs-tspspi-0.0.8/src/labdevices/powersupply.py`

 * *Files identical despite different names*

### Comparing `pylabdevs-tspspi-0.0.7/src/labdevices/serialringbuffer.py` & `pylabdevs-tspspi-0.0.8/src/labdevices/serialringbuffer.py`

 * *Files identical despite different names*

### Comparing `pylabdevs-tspspi-0.0.7/src/pylabdevs_tspspi.egg-info/PKG-INFO` & `pylabdevs-tspspi-0.0.8/src/pylabdevs_tspspi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylabdevs-tspspi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Lab devices base classes
 Home-page: https://github.com/tspspi/pylabdevs
 Author: Thomas Spielauer
 Author-email: pypipackages01@tspi.at
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

