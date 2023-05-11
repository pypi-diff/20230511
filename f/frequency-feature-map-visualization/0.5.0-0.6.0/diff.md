# Comparing `tmp/frequency_feature_map_visualization-0.5.0.tar.gz` & `tmp/frequency_feature_map_visualization-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequency_feature_map_visualization-0.5.0.tar", last modified: Thu May 11 13:33:42 2023, max compression
+gzip compressed data, was "frequency_feature_map_visualization-0.6.0.tar", last modified: Thu May 11 14:05:28 2023, max compression
```

## Comparing `frequency_feature_map_visualization-0.5.0.tar` & `frequency_feature_map_visualization-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-11 13:33:42.201212 frequency_feature_map_visualization-0.5.0/
--rw-r--r--   0 fuguanghui   (501) staff       (20)      530 2023-05-11 13:33:42.201086 frequency_feature_map_visualization-0.5.0/PKG-INFO
-drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-11 13:33:42.200103 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization/
--rw-rw-r--   0 fuguanghui   (501) staff       (20)      196 2023-05-10 15:35:39.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization/__init__.py
--rw-r--r--   0 fuguanghui   (501) staff       (20)     7548 2023-05-11 13:30:29.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization/feature_map_visualization.py
-drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-11 13:33:42.200884 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/
--rw-r--r--   0 fuguanghui   (501) staff       (20)      530 2023-05-11 13:33:42.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/PKG-INFO
--rw-r--r--   0 fuguanghui   (501) staff       (20)      415 2023-05-11 13:33:42.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/SOURCES.txt
--rw-r--r--   0 fuguanghui   (501) staff       (20)        1 2023-05-11 13:33:42.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/dependency_links.txt
--rw-r--r--   0 fuguanghui   (501) staff       (20)       23 2023-05-11 13:33:42.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/requires.txt
--rw-r--r--   0 fuguanghui   (501) staff       (20)       36 2023-05-11 13:33:42.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/top_level.txt
--rw-r--r--   0 fuguanghui   (501) staff       (20)       38 2023-05-11 13:33:42.201256 frequency_feature_map_visualization-0.5.0/setup.cfg
--rw-rw-r--   0 fuguanghui   (501) staff       (20)      689 2023-05-11 13:33:28.000000 frequency_feature_map_visualization-0.5.0/setup.py
+drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-11 14:05:28.493232 frequency_feature_map_visualization-0.6.0/
+-rw-r--r--   0 fuguanghui   (501) staff       (20)      530 2023-05-11 14:05:28.493113 frequency_feature_map_visualization-0.6.0/PKG-INFO
+drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-11 14:05:28.492095 frequency_feature_map_visualization-0.6.0/frequency_feature_map_visualization/
+-rw-rw-r--   0 fuguanghui   (501) staff       (20)      196 2023-05-10 15:35:39.000000 frequency_feature_map_visualization-0.6.0/frequency_feature_map_visualization/__init__.py
+-rw-r--r--   0 fuguanghui   (501) staff       (20)     7548 2023-05-11 14:04:31.000000 frequency_feature_map_visualization-0.6.0/frequency_feature_map_visualization/feature_map_visualization.py
+drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-11 14:05:28.492918 frequency_feature_map_visualization-0.6.0/frequency_feature_map_visualization.egg-info/
+-rw-r--r--   0 fuguanghui   (501) staff       (20)      530 2023-05-11 14:05:28.000000 frequency_feature_map_visualization-0.6.0/frequency_feature_map_visualization.egg-info/PKG-INFO
+-rw-r--r--   0 fuguanghui   (501) staff       (20)      415 2023-05-11 14:05:28.000000 frequency_feature_map_visualization-0.6.0/frequency_feature_map_visualization.egg-info/SOURCES.txt
+-rw-r--r--   0 fuguanghui   (501) staff       (20)        1 2023-05-11 14:05:28.000000 frequency_feature_map_visualization-0.6.0/frequency_feature_map_visualization.egg-info/dependency_links.txt
+-rw-r--r--   0 fuguanghui   (501) staff       (20)       23 2023-05-11 14:05:28.000000 frequency_feature_map_visualization-0.6.0/frequency_feature_map_visualization.egg-info/requires.txt
+-rw-r--r--   0 fuguanghui   (501) staff       (20)       36 2023-05-11 14:05:28.000000 frequency_feature_map_visualization-0.6.0/frequency_feature_map_visualization.egg-info/top_level.txt
+-rw-r--r--   0 fuguanghui   (501) staff       (20)       38 2023-05-11 14:05:28.493274 frequency_feature_map_visualization-0.6.0/setup.cfg
+-rw-rw-r--   0 fuguanghui   (501) staff       (20)      689 2023-05-11 14:05:17.000000 frequency_feature_map_visualization-0.6.0/setup.py
```

### Comparing `frequency_feature_map_visualization-0.5.0/PKG-INFO` & `frequency_feature_map_visualization-0.6.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequency_feature_map_visualization
-Version: 0.5.0
+Version: 0.6.0
 Summary: This code is designed to visualize and save the feature maps of 3D and 2D models. The feature maps can be viewed in the image domain and frequency domain, and saved as .npy files.
 Home-page: UNKNOWN
 Author: Guanghui FU
 Author-email: aslanfu123@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization/feature_map_visualization.py` & `frequency_feature_map_visualization-0.6.0/frequency_feature_map_visualization/feature_map_visualization.py`

 * *Files identical despite different names*

### Comparing `frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/PKG-INFO` & `frequency_feature_map_visualization-0.6.0/frequency_feature_map_visualization.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequency-feature-map-visualization
-Version: 0.5.0
+Version: 0.6.0
 Summary: This code is designed to visualize and save the feature maps of 3D and 2D models. The feature maps can be viewed in the image domain and frequency domain, and saved as .npy files.
 Home-page: UNKNOWN
 Author: Guanghui FU
 Author-email: aslanfu123@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `frequency_feature_map_visualization-0.5.0/setup.py` & `frequency_feature_map_visualization-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="frequency_feature_map_visualization",
-    version="0.5.0",
+    version="0.6.0",
     description="This code is designed to visualize and save the feature maps of 3D and 2D models. The feature maps can be viewed in the image domain and frequency domain, and saved as .npy files.",
     author="Guanghui FU",
     author_email="aslanfu123@gmail.com",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "torch",
```

