# Comparing `tmp/bp-data-visualization-1.0.4.tar.gz` & `tmp/bp-data-visualization-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp-data-visualization-1.0.4.tar", last modified: Wed May 10 10:44:53 2023, max compression
+gzip compressed data, was "bp-data-visualization-1.0.5.tar", last modified: Thu May 11 07:02:24 2023, max compression
```

## Comparing `bp-data-visualization-1.0.4.tar` & `bp-data-visualization-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:44:53.338640 bp-data-visualization-1.0.4/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-19 06:01:44.000000 bp-data-visualization-1.0.4/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       53 2023-04-19 06:01:44.000000 bp-data-visualization-1.0.4/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3029 2023-05-10 10:44:53.338349 bp-data-visualization-1.0.4/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2162 2023-05-09 08:38:21.000000 bp-data-visualization-1.0.4/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:44:53.330175 bp-data-visualization-1.0.4/bp_data_visualization.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3029 2023-05-10 10:44:53.000000 bp-data-visualization-1.0.4/bp_data_visualization.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      527 2023-05-10 10:44:53.000000 bp-data-visualization-1.0.4/bp_data_visualization.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-10 10:44:53.000000 bp-data-visualization-1.0.4/bp_data_visualization.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-05-10 10:44:53.000000 bp-data-visualization-1.0.4/bp_data_visualization.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       19 2023-05-10 10:44:53.000000 bp-data-visualization-1.0.4/bp_data_visualization.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:44:53.331257 bp-data-visualization-1.0.4/data_visualization/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2091 2023-04-24 10:01:27.000000 bp-data-visualization-1.0.4/data_visualization/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:44:53.325118 bp-data-visualization-1.0.4/data_visualization/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:44:53.332592 bp-data-visualization-1.0.4/data_visualization/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:44:53.334353 bp-data-visualization-1.0.4/data_visualization/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-10 10:39:33.000000 bp-data-visualization-1.0.4/data_visualization/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  2457735 2023-05-10 10:39:33.000000 bp-data-visualization-1.0.4/data_visualization/frontend/dist/assets/index-fc1e11f7.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      457 2023-05-10 10:41:53.000000 bp-data-visualization-1.0.4/data_visualization/frontend/dist/index.html
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-05-10 10:39:32.000000 bp-data-visualization-1.0.4/data_visualization/frontend/dist/vite.svg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-19 06:01:44.000000 bp-data-visualization-1.0.4/data_visualization/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-10 10:44:53.338745 bp-data-visualization-1.0.4/setup.cfg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      772 2023-05-10 10:44:51.000000 bp-data-visualization-1.0.4/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-11 07:02:24.612955 bp-data-visualization-1.0.5/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-19 06:01:44.000000 bp-data-visualization-1.0.5/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       53 2023-04-19 06:01:44.000000 bp-data-visualization-1.0.5/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3029 2023-05-11 07:02:24.612665 bp-data-visualization-1.0.5/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2162 2023-05-09 08:38:21.000000 bp-data-visualization-1.0.5/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-11 07:02:24.604395 bp-data-visualization-1.0.5/bp_data_visualization.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3029 2023-05-11 07:02:24.000000 bp-data-visualization-1.0.5/bp_data_visualization.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      527 2023-05-11 07:02:24.000000 bp-data-visualization-1.0.5/bp_data_visualization.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-11 07:02:24.000000 bp-data-visualization-1.0.5/bp_data_visualization.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-05-11 07:02:24.000000 bp-data-visualization-1.0.5/bp_data_visualization.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       19 2023-05-11 07:02:24.000000 bp-data-visualization-1.0.5/bp_data_visualization.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-11 07:02:24.605709 bp-data-visualization-1.0.5/data_visualization/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2091 2023-04-24 10:01:27.000000 bp-data-visualization-1.0.5/data_visualization/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-11 07:02:24.600682 bp-data-visualization-1.0.5/data_visualization/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-11 07:02:24.606930 bp-data-visualization-1.0.5/data_visualization/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-11 07:02:24.608032 bp-data-visualization-1.0.5/data_visualization/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-11 06:58:21.000000 bp-data-visualization-1.0.5/data_visualization/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  2457735 2023-05-11 06:58:21.000000 bp-data-visualization-1.0.5/data_visualization/frontend/dist/assets/index-fc1e11f7.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      457 2023-05-11 07:02:10.000000 bp-data-visualization-1.0.5/data_visualization/frontend/dist/index.html
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-05-11 06:58:20.000000 bp-data-visualization-1.0.5/data_visualization/frontend/dist/vite.svg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-19 06:01:44.000000 bp-data-visualization-1.0.5/data_visualization/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-11 07:02:24.613067 bp-data-visualization-1.0.5/setup.cfg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      772 2023-05-11 06:57:49.000000 bp-data-visualization-1.0.5/setup.py
```

### Comparing `bp-data-visualization-1.0.4/LICENSE` & `bp-data-visualization-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.4/PKG-INFO` & `bp-data-visualization-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bp-data-visualization
-Version: 1.0.4
+Version: 1.0.5
 Summary: Show data in charts
 Home-page: UNKNOWN
 Author: Bluepinapple
 Author-email: viveksthul@bluepinapple.com
 License: UNKNOWN
 Description: # Data Visualization
```

### Comparing `bp-data-visualization-1.0.4/README.md` & `bp-data-visualization-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.4/bp_data_visualization.egg-info/PKG-INFO` & `bp-data-visualization-1.0.5/bp_data_visualization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bp-data-visualization
-Version: 1.0.4
+Version: 1.0.5
 Summary: Show data in charts
 Home-page: UNKNOWN
 Author: Bluepinapple
 Author-email: viveksthul@bluepinapple.com
 License: UNKNOWN
 Description: # Data Visualization
```

### Comparing `bp-data-visualization-1.0.4/bp_data_visualization.egg-info/SOURCES.txt` & `bp-data-visualization-1.0.5/bp_data_visualization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.4/data_visualization/__init__.py` & `bp-data-visualization-1.0.5/data_visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.4/data_visualization/frontend/dist/assets/index-fc1e11f7.js` & `bp-data-visualization-1.0.5/data_visualization/frontend/dist/assets/index-fc1e11f7.js`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.4/data_visualization/frontend/dist/vite.svg` & `bp-data-visualization-1.0.5/data_visualization/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.4/data_visualization/register.py` & `bp-data-visualization-1.0.5/data_visualization/register.py`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.4/setup.py` & `bp-data-visualization-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="bp-data-visualization",
-    version="1.0.4",
+    version="1.0.5",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="Show data in charts",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

