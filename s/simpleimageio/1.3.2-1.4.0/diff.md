# Comparing `tmp/simpleimageio-1.3.2.tar.gz` & `tmp/simpleimageio-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleimageio-1.3.2.tar", last modified: Fri Apr 14 12:04:17 2023, max compression
+gzip compressed data, was "simpleimageio-1.4.0.tar", last modified: Thu May 11 10:57:38 2023, max compression
```

## Comparing `simpleimageio-1.3.2.tar` & `simpleimageio-1.4.0.tar`

### file list

```diff
@@ -1,47 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:17.109553 simpleimageio-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:17.105553 simpleimageio-1.3.2/Core/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:17.109553 simpleimageio-1.3.2/Core/External/
--rw-r--r--   0 runner    (1001) docker     (123)   114725 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/fpng.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/fpng.h
--rw-r--r--   0 runner    (1001) docker     (123)   319839 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/miniz.c
--rw-r--r--   0 runner    (1001) docker     (123)    69441 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/miniz.h
--rw-r--r--   0 runner    (1001) docker     (123)   273149 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/stb_image.h
--rw-r--r--   0 runner    (1001) docker     (123)    69564 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/stb_image_write.h
--rw-r--r--   0 runner    (1001) docker     (123)   163059 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/tiny_dng_loader.h
--rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/tiny_dng_writer.h
--rw-r--r--   0 runner    (1001) docker     (123)   269883 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/tinyexr.h
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/error_metrics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/filter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/image.h
--rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/imageio.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/manipulation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/tonemapping.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/vec3.h
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-14 12:04:17.109553 simpleimageio-1.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:17.101553 simpleimageio-1.3.2/PyWrapper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:17.109553 simpleimageio-1.3.2/PyWrapper/simpleimageio/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/corelib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/error_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    37535 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/imageViewer.js
--rw-r--r--   0 runner    (1001) docker     (123)    89794 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/jquery-3.6.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/manip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/tev.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/tonemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:04:17.109553 simpleimageio-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:17.109553 simpleimageio-1.3.2/simpleimageio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-14 12:04:17.000000 simpleimageio-1.3.2/simpleimageio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-14 12:04:17.000000 simpleimageio-1.3.2/simpleimageio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:04:17.000000 simpleimageio-1.3.2/simpleimageio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 12:04:17.000000 simpleimageio-1.3.2/simpleimageio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-14 12:04:17.000000 simpleimageio-1.3.2/simpleimageio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:57:38.078467 simpleimageio-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:57:38.074467 simpleimageio-1.4.0/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:57:38.074467 simpleimageio-1.4.0/Core/External/
+-rw-r--r--   0 runner    (1001) docker     (123)   114725 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/fpng.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/fpng.h
+-rw-r--r--   0 runner    (1001) docker     (123)   319839 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/miniz.c
+-rw-r--r--   0 runner    (1001) docker     (123)    69441 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/miniz.h
+-rw-r--r--   0 runner    (1001) docker     (123)   273149 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/stb_image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69564 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/stb_image_write.h
+-rw-r--r--   0 runner    (1001) docker     (123)   163059 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/tiny_dng_loader.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/tiny_dng_writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)   269883 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/tinyexr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/error_metrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/imageio.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/manipulation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/tonemapping.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/vec3.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-05-11 10:57:38.078467 simpleimageio-1.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:57:38.070467 simpleimageio-1.4.0/PyWrapper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:57:38.074467 simpleimageio-1.4.0/PyWrapper/simpleimageio/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/corelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/error_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/manip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/tev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/tonemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 10:57:38.078467 simpleimageio-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:57:38.078467 simpleimageio-1.4.0/simpleimageio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-05-11 10:57:38.000000 simpleimageio-1.4.0/simpleimageio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-11 10:57:38.000000 simpleimageio-1.4.0/simpleimageio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:57:38.000000 simpleimageio-1.4.0/simpleimageio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 10:57:38.000000 simpleimageio-1.4.0/simpleimageio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 10:57:38.000000 simpleimageio-1.4.0/simpleimageio.egg-info/top_level.txt
```

### Comparing `simpleimageio-1.3.2/Core/CMakeLists.txt` & `simpleimageio-1.4.0/Core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/External/fpng.cpp` & `simpleimageio-1.4.0/Core/External/fpng.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/External/fpng.h` & `simpleimageio-1.4.0/Core/External/fpng.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/External/miniz.c` & `simpleimageio-1.4.0/Core/External/miniz.c`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/External/miniz.h` & `simpleimageio-1.4.0/Core/External/miniz.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/External/stb_image.h` & `simpleimageio-1.4.0/Core/External/stb_image.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/External/stb_image_write.h` & `simpleimageio-1.4.0/Core/External/stb_image_write.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/External/tiny_dng_loader.h` & `simpleimageio-1.4.0/Core/External/tiny_dng_loader.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/External/tiny_dng_writer.h` & `simpleimageio-1.4.0/Core/External/tiny_dng_writer.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/External/tinyexr.h` & `simpleimageio-1.4.0/Core/External/tinyexr.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/error_metrics.cpp` & `simpleimageio-1.4.0/Core/error_metrics.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/filter.cpp` & `simpleimageio-1.4.0/Core/filter.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/image.h` & `simpleimageio-1.4.0/Core/image.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/imageio.cpp` & `simpleimageio-1.4.0/Core/imageio.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/manipulation.cpp` & `simpleimageio-1.4.0/Core/manipulation.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/tonemapping.cpp` & `simpleimageio-1.4.0/Core/tonemapping.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/Core/vec3.h` & `simpleimageio-1.4.0/Core/vec3.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/LICENSE` & `simpleimageio-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/PKG-INFO` & `simpleimageio-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleimageio
-Version: 1.3.2
+Version: 1.4.0
 Summary: A very simple Python wrapper to read and write various HDR and LDR image file formats.
 Home-page: https://github.com/pgrit/SimpleImageIO
 Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simpleimageio Version: 1.3.2 Summary: A very simple
+Metadata-Version: 2.1 Name: simpleimageio Version: 1.4.0 Summary: A very simple
 Python wrapper to read and write various HDR and LDR image file formats. Home-
 page: https://github.com/pgrit/SimpleImageIO Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE ![Build](https://github.com/pgrit/SimpleImageIO/workflows/Build/
 badge.svg) [https://buildstats.info/nuget/SimpleImageIO] # Simple Image IO A
```

### Comparing `simpleimageio-1.3.2/PyWrapper/simpleimageio/corelib.py` & `simpleimageio-1.4.0/PyWrapper/simpleimageio/corelib.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/PyWrapper/simpleimageio/error_metrics.py` & `simpleimageio-1.4.0/PyWrapper/simpleimageio/error_metrics.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/PyWrapper/simpleimageio/flip.py` & `simpleimageio-1.4.0/PyWrapper/simpleimageio/flip.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 import pkgutil
 import numpy as np
 import uuid
 import base64
 from . import corelib
 
 def make_header():
-    js = pkgutil.get_data(__package__, 'jquery-3.6.4.min.js').decode('utf-8')
-    html = "<script>" + js + "</script>"
-
-    js = pkgutil.get_data(__package__, 'imageViewer.js').decode('utf-8')
-    html += "<script>" + js + "</script>"
-
-    css = pkgutil.get_data(__package__, 'style.css').decode('utf-8')
-    html += "<style>" + css + "</style>"
-    return html
+    js = pkgutil.get_data(__package__, 'flipbook.js').decode('utf-8')
+    return "<script>" + js + "</script>"
 
 def _rgb_to_rgbe(rgb):
     rgb = np.array(rgb, dtype=np.float32)
     maxcomp = np.max(rgb, axis=2)
 
     rgbe = np.zeros((rgb.shape[0], rgb.shape[1], 4), dtype=np.uint8)
     mask = maxcomp > 1e-32
@@ -35,42 +28,47 @@
     rgb[:,:,0] = np.ldexp(rgbe[:,:,0], exponent)
     rgb[:,:,1] = np.ldexp(rgbe[:,:,1], exponent)
     rgb[:,:,2] = np.ldexp(rgbe[:,:,2], exponent)
     return rgb
 
 def make_flip_book(images, html_width=900, html_height=800):
     id = "flipbook-" + str(uuid.uuid4())
-    html = f"<div id={id} style='width:{html_width}px;height:{html_height}px;'></div>"
-    html += "<div id='magnifier'><table class='magnifier'></table></div>"
 
     _, (_, width, height, _) = corelib.get_numpy_data(images[0][1])
     encoded_images = []
     names = []
+    types = []
     for name, img in images:
         img, (_, _, _, num_channels) = corelib.get_numpy_data(img)
         if num_channels == 1:
             img = np.tile(img, (1, 1, 3))
         rgbe = _rgb_to_rgbe(img)
-        encoded_images.append("readRGBE('data:;base64," + base64.b64encode(rgbe).decode() + "')")
-        names.append(f"'{name}'")
+        encoded_images.append("data:;base64," + base64.b64encode(rgbe).decode())
+        names.append(name)
+        types.append("rgbe")
+
+    data = {
+        "dataUrls": encoded_images,
+        "types": types,
+        "names": names,
+        "width": width,
+        "height": height,
+        "initialZoom": 1.0,
+        "initialTMO": {
+            "activeTMO:": "exposure",
+            "exposure:": 0.0
+        },
+        "containerId": id,
+    }
 
-    initial_zoom_str = "'fit'"
-    initial_tmo_str = "null"
+    import json
+    json = json.dumps(data)
 
-    html += f"""
-    <script>
-    {{
-        let images = Promise.all([{",".join(encoded_images)}]);
-        images.then(values =>
-            AddFlipBook($("#{id}"), [{",".join(names)}], values, {width}, {height},
-                        {initial_zoom_str}, {initial_tmo_str})
-        );
-    }}
-    </script>
-    """
+    html = f"<div id={id} style='width:{html_width}px;height:{html_height}px;'></div>"
+    html += f"<script> {{ flipbook.MakeFlipBook({json}); }} </script>"
     return html
 
 def flip_header():
     """ Use this with Jupyter: Displays the HTML header in the current IPython kernel.
     """
     from IPython.display import display, HTML
     display(HTML(make_header()))
```

### Comparing `simpleimageio-1.3.2/PyWrapper/simpleimageio/image.py` & `simpleimageio-1.4.0/PyWrapper/simpleimageio/image.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/PyWrapper/simpleimageio/manip.py` & `simpleimageio-1.4.0/PyWrapper/simpleimageio/manip.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/PyWrapper/simpleimageio/tev.py` & `simpleimageio-1.4.0/PyWrapper/simpleimageio/tev.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/PyWrapper/simpleimageio/tonemap.py` & `simpleimageio-1.4.0/PyWrapper/simpleimageio/tonemap.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/README.md` & `simpleimageio-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.2/setup.py` & `simpleimageio-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         os.chdir(str(cwd))
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='simpleimageio',
-    version='1.3.2',
+    version='1.4.0',
     author='Pascal Grittmann',
     url='https://github.com/pgrit/SimpleImageIO',
 
     description='A very simple Python wrapper to read and write various HDR and LDR image file formats.',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `simpleimageio-1.3.2/simpleimageio.egg-info/PKG-INFO` & `simpleimageio-1.4.0/simpleimageio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleimageio
-Version: 1.3.2
+Version: 1.4.0
 Summary: A very simple Python wrapper to read and write various HDR and LDR image file formats.
 Home-page: https://github.com/pgrit/SimpleImageIO
 Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simpleimageio Version: 1.3.2 Summary: A very simple
+Metadata-Version: 2.1 Name: simpleimageio Version: 1.4.0 Summary: A very simple
 Python wrapper to read and write various HDR and LDR image file formats. Home-
 page: https://github.com/pgrit/SimpleImageIO Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE ![Build](https://github.com/pgrit/SimpleImageIO/workflows/Build/
 badge.svg) [https://buildstats.info/nuget/SimpleImageIO] # Simple Image IO A
```

### Comparing `simpleimageio-1.3.2/simpleimageio.egg-info/SOURCES.txt` & `simpleimageio-1.4.0/simpleimageio.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -22,18 +22,15 @@
 Core/External/tiny_dng_writer.h
 Core/External/tinyexr.h
 PyWrapper/simpleimageio/__init__.py
 PyWrapper/simpleimageio/corelib.py
 PyWrapper/simpleimageio/error_metrics.py
 PyWrapper/simpleimageio/flip.py
 PyWrapper/simpleimageio/image.py
-PyWrapper/simpleimageio/imageViewer.js
-PyWrapper/simpleimageio/jquery-3.6.4.min.js
 PyWrapper/simpleimageio/manip.py
-PyWrapper/simpleimageio/style.css
 PyWrapper/simpleimageio/tev.py
 PyWrapper/simpleimageio/tonemap.py
 simpleimageio.egg-info/PKG-INFO
 simpleimageio.egg-info/SOURCES.txt
 simpleimageio.egg-info/dependency_links.txt
 simpleimageio.egg-info/requires.txt
 simpleimageio.egg-info/top_level.txt
```

