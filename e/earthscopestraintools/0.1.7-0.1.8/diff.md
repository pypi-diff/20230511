# Comparing `tmp/earthscopestraintools-0.1.7.tar.gz` & `tmp/earthscopestraintools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthscopestraintools-0.1.7.tar", last modified: Thu May 11 14:03:18 2023, max compression
+gzip compressed data, was "earthscopestraintools-0.1.8.tar", last modified: Thu May 11 16:46:59 2023, max compression
```

## Comparing `earthscopestraintools-0.1.7.tar` & `earthscopestraintools-0.1.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 14:03:18.290856 earthscopestraintools-0.1.7/
--rw-r--r--   0 gottlieb   (501) staff       (20)     1042 2023-02-21 23:33:21.000000 earthscopestraintools-0.1.7/LICENSE
--rw-r--r--   0 gottlieb   (501) staff       (20)     3217 2023-05-11 14:03:18.290442 earthscopestraintools-0.1.7/PKG-INFO
--rw-r--r--   0 gottlieb   (501) staff       (20)     1505 2023-03-07 14:24:27.000000 earthscopestraintools-0.1.7/README.md
--rw-r--r--   0 gottlieb   (501) staff       (20)      955 2023-05-01 19:26:39.000000 earthscopestraintools-0.1.7/pyproject.toml
--rw-r--r--   0 gottlieb   (501) staff       (20)       38 2023-05-11 14:03:18.290957 earthscopestraintools-0.1.7/setup.cfg
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 14:03:18.171108 earthscopestraintools-0.1.7/src/
--rw-r--r--   0 gottlieb   (501) staff       (20)        0 2023-02-13 22:17:58.000000 earthscopestraintools-0.1.7/src/__init__.py
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 14:03:18.179001 earthscopestraintools-0.1.7/src/earthscopestraintools/
--rw-r--r--   0 gottlieb   (501) staff       (20)        0 2023-02-13 22:17:58.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/__init__.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     7265 2023-05-04 18:11:43.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/ascii2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)    10688 2023-02-08 22:58:57.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/bottle.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1563 2023-03-07 13:59:16.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/bottle2mseed.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     6288 2023-05-11 14:00:15.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/bottle2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     6350 2023-03-07 14:19:55.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/bottletar.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     7409 2023-03-27 17:52:37.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/edid.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1591 2023-03-27 17:31:01.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/event.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     8507 2023-03-27 17:34:50.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/event_processing.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     4929 2021-03-10 22:31:02.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/event_site_terms.txt
--rw-r--r--   0 gottlieb   (501) staff       (20)    18330 2023-05-01 20:18:57.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/gtsm_metadata.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     4373 2023-05-02 17:31:35.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/mseed_tools.py
--rw-r--r--   0 gottlieb   (501) staff       (20)    10076 2023-05-01 20:13:12.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/processing.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     4346 2023-03-07 12:51:32.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/tdb2ascii.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     2725 2023-05-04 20:36:52.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/tdb2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)    32284 2023-05-04 19:05:01.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/tiledbtools.py
--rw-r--r--   0 gottlieb   (501) staff       (20)    25945 2023-05-02 17:52:53.000000 earthscopestraintools-0.1.7/src/earthscopestraintools/timeseries.py
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 14:03:18.193256 earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/
--rw-r--r--   0 gottlieb   (501) staff       (20)     3217 2023-05-11 14:03:18.000000 earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/PKG-INFO
--rw-r--r--   0 gottlieb   (501) staff       (20)     1174 2023-05-11 14:03:18.000000 earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/SOURCES.txt
--rw-r--r--   0 gottlieb   (501) staff       (20)        1 2023-05-11 14:03:18.000000 earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/dependency_links.txt
--rw-r--r--   0 gottlieb   (501) staff       (20)      120 2023-05-11 14:03:18.000000 earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/requires.txt
--rw-r--r--   0 gottlieb   (501) staff       (20)       22 2023-05-11 14:03:18.000000 earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/top_level.txt
-drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 14:03:18.289809 earthscopestraintools-0.1.7/test/
--rw-r--r--   0 gottlieb   (501) staff       (20)      240 2023-03-29 13:58:10.000000 earthscopestraintools-0.1.7/test/test_ascii2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1295 2023-03-07 13:56:58.000000 earthscopestraintools-0.1.7/test/test_bottle2mseed.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     2497 2023-05-04 17:47:25.000000 earthscopestraintools-0.1.7/test/test_bottle2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1336 2023-03-07 14:11:58.000000 earthscopestraintools-0.1.7/test/test_bottletar.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1044 2023-03-27 18:40:20.000000 earthscopestraintools-0.1.7/test/test_edid.py
--rw-r--r--   0 gottlieb   (501) staff       (20)      373 2023-05-01 20:05:48.000000 earthscopestraintools-0.1.7/test/test_gtsm_metadata.py
--rw-r--r--   0 gottlieb   (501) staff       (20)      470 2023-03-06 23:40:58.000000 earthscopestraintools-0.1.7/test/test_tdb2ascii.py
--rw-r--r--   0 gottlieb   (501) staff       (20)      351 2023-05-04 18:34:51.000000 earthscopestraintools-0.1.7/test/test_tdb2tdb.py
--rw-r--r--   0 gottlieb   (501) staff       (20)     1818 2023-03-27 22:45:21.000000 earthscopestraintools-0.1.7/test/test_ts2tdb.py
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 16:46:59.269739 earthscopestraintools-0.1.8/
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1042 2023-02-21 23:33:21.000000 earthscopestraintools-0.1.8/LICENSE
+-rw-r--r--   0 gottlieb   (501) staff       (20)     3217 2023-05-11 16:46:59.269265 earthscopestraintools-0.1.8/PKG-INFO
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1505 2023-03-07 14:24:27.000000 earthscopestraintools-0.1.8/README.md
+-rw-r--r--   0 gottlieb   (501) staff       (20)      976 2023-05-11 16:46:39.000000 earthscopestraintools-0.1.8/pyproject.toml
+-rw-r--r--   0 gottlieb   (501) staff       (20)       38 2023-05-11 16:46:59.269864 earthscopestraintools-0.1.8/setup.cfg
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 16:46:59.183649 earthscopestraintools-0.1.8/src/
+-rw-r--r--   0 gottlieb   (501) staff       (20)        0 2023-02-13 22:17:58.000000 earthscopestraintools-0.1.8/src/__init__.py
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 16:46:59.225444 earthscopestraintools-0.1.8/src/earthscopestraintools/
+-rw-r--r--   0 gottlieb   (501) staff       (20)        0 2023-02-13 22:17:58.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/__init__.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     7265 2023-05-04 18:11:43.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/ascii2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)    10688 2023-02-08 22:58:57.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/bottle.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1563 2023-03-07 13:59:16.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/bottle2mseed.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     6288 2023-05-11 14:00:15.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/bottle2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     6350 2023-03-07 14:19:55.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/bottletar.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     7409 2023-03-27 17:52:37.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/edid.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1591 2023-03-27 17:31:01.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/event.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     8507 2023-03-27 17:34:50.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/event_processing.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     4929 2021-03-10 22:31:02.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/event_site_terms.txt
+-rw-r--r--   0 gottlieb   (501) staff       (20)    18330 2023-05-01 20:18:57.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/gtsm_metadata.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     4373 2023-05-02 17:31:35.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/mseed_tools.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)    10076 2023-05-01 20:13:12.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/processing.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     4346 2023-03-07 12:51:32.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/tdb2ascii.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     2725 2023-05-04 20:36:52.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/tdb2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)    32284 2023-05-04 19:05:01.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/tiledbtools.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)    25945 2023-05-02 17:52:53.000000 earthscopestraintools-0.1.8/src/earthscopestraintools/timeseries.py
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 16:46:59.229605 earthscopestraintools-0.1.8/src/earthscopestraintools.egg-info/
+-rw-r--r--   0 gottlieb   (501) staff       (20)     3217 2023-05-11 16:46:59.000000 earthscopestraintools-0.1.8/src/earthscopestraintools.egg-info/PKG-INFO
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1174 2023-05-11 16:46:59.000000 earthscopestraintools-0.1.8/src/earthscopestraintools.egg-info/SOURCES.txt
+-rw-r--r--   0 gottlieb   (501) staff       (20)        1 2023-05-11 16:46:59.000000 earthscopestraintools-0.1.8/src/earthscopestraintools.egg-info/dependency_links.txt
+-rw-r--r--   0 gottlieb   (501) staff       (20)      134 2023-05-11 16:46:59.000000 earthscopestraintools-0.1.8/src/earthscopestraintools.egg-info/requires.txt
+-rw-r--r--   0 gottlieb   (501) staff       (20)       22 2023-05-11 16:46:59.000000 earthscopestraintools-0.1.8/src/earthscopestraintools.egg-info/top_level.txt
+drwxr-xr-x   0 gottlieb   (501) staff       (20)        0 2023-05-11 16:46:59.268592 earthscopestraintools-0.1.8/test/
+-rw-r--r--   0 gottlieb   (501) staff       (20)      240 2023-03-29 13:58:10.000000 earthscopestraintools-0.1.8/test/test_ascii2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1295 2023-03-07 13:56:58.000000 earthscopestraintools-0.1.8/test/test_bottle2mseed.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     2497 2023-05-04 17:47:25.000000 earthscopestraintools-0.1.8/test/test_bottle2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1336 2023-03-07 14:11:58.000000 earthscopestraintools-0.1.8/test/test_bottletar.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1044 2023-03-27 18:40:20.000000 earthscopestraintools-0.1.8/test/test_edid.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)      373 2023-05-01 20:05:48.000000 earthscopestraintools-0.1.8/test/test_gtsm_metadata.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)      470 2023-03-06 23:40:58.000000 earthscopestraintools-0.1.8/test/test_tdb2ascii.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)      351 2023-05-04 18:34:51.000000 earthscopestraintools-0.1.8/test/test_tdb2tdb.py
+-rw-r--r--   0 gottlieb   (501) staff       (20)     1818 2023-03-27 22:45:21.000000 earthscopestraintools-0.1.8/test/test_ts2tdb.py
```

### Comparing `earthscopestraintools-0.1.7/LICENSE` & `earthscopestraintools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/PKG-INFO` & `earthscopestraintools-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthscopestraintools
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of utilities for working with EarthScope strainmeter data
 Author-email: Mike Gottlieb <mike.gottlieb@eartscope.org>
 License: Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `earthscopestraintools-0.1.7/README.md` & `earthscopestraintools-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/pyproject.toml` & `earthscopestraintools-0.1.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "earthscopestraintools"
-version ="0.1.7"
+version ="0.1.8"
 authors = [
   { name="Mike Gottlieb", email="mike.gottlieb@eartscope.org" },
 ]
 description = "A collection of utilities for working with EarthScope strainmeter data"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+    "scipy>=1.10.1",
     "numpy>=1.24.1",
     "pandas>=1.5.3",
     "requests>=2.28.2",
     #"xmltodict>=0.13.0",
     "geopy>=2.3.0"
 ]
```

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/ascii2tdb.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/ascii2tdb.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/bottle.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/bottle.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/bottle2mseed.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/bottle2mseed.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/bottle2tdb.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/bottle2tdb.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/bottletar.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/bottletar.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/edid.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/edid.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/event.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/event.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/event_processing.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/event_processing.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/event_site_terms.txt` & `earthscopestraintools-0.1.8/src/earthscopestraintools/event_site_terms.txt`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/gtsm_metadata.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/gtsm_metadata.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/mseed_tools.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/mseed_tools.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/processing.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/processing.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/tdb2ascii.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/tdb2ascii.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/tdb2tdb.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/tdb2tdb.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/tiledbtools.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/tiledbtools.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools/timeseries.py` & `earthscopestraintools-0.1.8/src/earthscopestraintools/timeseries.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/PKG-INFO` & `earthscopestraintools-0.1.8/src/earthscopestraintools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthscopestraintools
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of utilities for working with EarthScope strainmeter data
 Author-email: Mike Gottlieb <mike.gottlieb@eartscope.org>
 License: Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `earthscopestraintools-0.1.7/src/earthscopestraintools.egg-info/SOURCES.txt` & `earthscopestraintools-0.1.8/src/earthscopestraintools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/test/test_bottle2mseed.py` & `earthscopestraintools-0.1.8/test/test_bottle2mseed.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/test/test_bottle2tdb.py` & `earthscopestraintools-0.1.8/test/test_bottle2tdb.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/test/test_bottletar.py` & `earthscopestraintools-0.1.8/test/test_bottletar.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/test/test_edid.py` & `earthscopestraintools-0.1.8/test/test_edid.py`

 * *Files identical despite different names*

### Comparing `earthscopestraintools-0.1.7/test/test_ts2tdb.py` & `earthscopestraintools-0.1.8/test/test_ts2tdb.py`

 * *Files identical despite different names*

