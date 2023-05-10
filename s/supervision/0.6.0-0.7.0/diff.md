# Comparing `tmp/supervision-0.6.0.tar.gz` & `tmp/supervision-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supervision-0.6.0.tar", last modified: Wed Apr 19 21:02:56 2023, max compression
+gzip compressed data, was "supervision-0.7.0.tar", last modified: Wed May 10 22:44:27 2023, max compression
```

## Comparing `supervision-0.6.0.tar` & `supervision-0.7.0.tar`

### file list

```diff
@@ -1,54 +1,62 @@
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.969612 supervision-0.6.0/
--rw-r--r--   0 skalskip   (501) staff       (20)     1065 2022-12-02 12:52:46.000000 supervision-0.6.0/LICENSE.md
--rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-19 21:02:56.969431 supervision-0.6.0/PKG-INFO
--rw-r--r--   0 skalskip   (501) staff       (20)     4450 2023-03-21 12:38:19.000000 supervision-0.6.0/README.md
--rw-r--r--   0 skalskip   (501) staff       (20)       38 2023-04-19 21:02:56.969689 supervision-0.6.0/setup.cfg
--rw-r--r--   0 skalskip   (501) staff       (20)     2220 2023-02-12 22:07:08.000000 supervision-0.6.0/setup.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.959638 supervision-0.6.0/supervision/
--rw-r--r--   0 skalskip   (501) staff       (20)     1044 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.961377 supervision-0.6.0/supervision/dataset/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/dataset/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5189 2023-04-19 21:02:26.000000 supervision-0.6.0/supervision/dataset/core.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.961966 supervision-0.6.0/supervision/dataset/formats/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/dataset/formats/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5912 2023-04-19 21:02:26.000000 supervision-0.6.0/supervision/dataset/formats/pascal_voc.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.963585 supervision-0.6.0/supervision/detection/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.6.0/supervision/detection/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     6171 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/detection/annotate.py
--rw-r--r--   0 skalskip   (501) staff       (20)    14736 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/detection/core.py
--rw-r--r--   0 skalskip   (501) staff       (20)     7162 2023-04-13 08:46:01.000000 supervision-0.6.0/supervision/detection/line_counter.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.963997 supervision-0.6.0/supervision/detection/tools/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-10 21:52:53.000000 supervision-0.6.0/supervision/detection/tools/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5056 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/detection/tools/polygon_zone.py
--rw-r--r--   0 skalskip   (501) staff       (20)     9634 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/detection/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.965674 supervision-0.6.0/supervision/draw/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.6.0/supervision/draw/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3675 2023-02-07 18:30:08.000000 supervision-0.6.0/supervision/draw/color.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5147 2023-03-13 13:53:19.000000 supervision-0.6.0/supervision/draw/utils.py
--rw-r--r--   0 skalskip   (501) staff       (20)      621 2023-04-19 14:17:19.000000 supervision-0.6.0/supervision/file.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.966660 supervision-0.6.0/supervision/geometry/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.6.0/supervision/geometry/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1397 2023-02-07 18:30:08.000000 supervision-0.6.0/supervision/geometry/core.py
--rw-r--r--   0 skalskip   (501) staff       (20)      993 2023-02-07 18:30:08.000000 supervision-0.6.0/supervision/geometry/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.967008 supervision-0.6.0/supervision/notebook/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.6.0/supervision/notebook/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     2831 2023-04-10 21:52:53.000000 supervision-0.6.0/supervision/notebook/utils.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5049 2023-02-07 18:30:08.000000 supervision-0.6.0/supervision/video.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.960948 supervision-0.6.0/supervision.egg-info/
--rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-19 21:02:56.000000 supervision-0.6.0/supervision.egg-info/PKG-INFO
--rw-r--r--   0 skalskip   (501) staff       (20)     1104 2023-04-19 21:02:56.000000 supervision-0.6.0/supervision.egg-info/SOURCES.txt
--rw-r--r--   0 skalskip   (501) staff       (20)        1 2023-04-19 21:02:56.000000 supervision-0.6.0/supervision.egg-info/dependency_links.txt
--rw-r--r--   0 skalskip   (501) staff       (20)      138 2023-04-19 21:02:56.000000 supervision-0.6.0/supervision.egg-info/requires.txt
--rw-r--r--   0 skalskip   (501) staff       (20)       17 2023-04-19 21:02:56.000000 supervision-0.6.0/supervision.egg-info/top_level.txt
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.967269 supervision-0.6.0/test/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.6.0/test/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.967812 supervision-0.6.0/test/detection/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.6.0/test/detection/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3742 2023-02-12 22:07:08.000000 supervision-0.6.0/test/detection/test_core.py
--rw-r--r--   0 skalskip   (501) staff       (20)     8054 2023-04-19 14:17:19.000000 supervision-0.6.0/test/detection/test_utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.968124 supervision-0.6.0/test/draw/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.6.0/test/draw/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1097 2023-02-02 10:53:06.000000 supervision-0.6.0/test/draw/test_color.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-19 21:02:56.969039 supervision-0.6.0/test/geometry/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.6.0/test/geometry/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1854 2023-02-07 18:30:08.000000 supervision-0.6.0/test/geometry/test_dataclasses.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.936566 supervision-0.7.0/
+-rw-r--r--   0 skalskip   (501) staff       (20)     1065 2022-12-02 12:52:46.000000 supervision-0.7.0/LICENSE.md
+-rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-05-10 22:44:27.936430 supervision-0.7.0/PKG-INFO
+-rw-r--r--   0 skalskip   (501) staff       (20)     4450 2023-03-21 12:38:19.000000 supervision-0.7.0/README.md
+-rw-r--r--   0 skalskip   (501) staff       (20)       38 2023-05-10 22:44:27.936620 supervision-0.7.0/setup.cfg
+-rw-r--r--   0 skalskip   (501) staff       (20)     2220 2023-02-12 22:07:08.000000 supervision-0.7.0/setup.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.929311 supervision-0.7.0/supervision/
+-rw-r--r--   0 skalskip   (501) staff       (20)     1044 2023-05-10 13:02:27.000000 supervision-0.7.0/supervision/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.930746 supervision-0.7.0/supervision/dataset/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.7.0/supervision/dataset/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     8641 2023-05-10 12:01:26.000000 supervision-0.7.0/supervision/dataset/core.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.931360 supervision-0.7.0/supervision/dataset/formats/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-19 14:17:19.000000 supervision-0.7.0/supervision/dataset/formats/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5564 2023-05-10 12:01:26.000000 supervision-0.7.0/supervision/dataset/formats/pascal_voc.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5633 2023-05-10 12:01:26.000000 supervision-0.7.0/supervision/dataset/formats/yolo.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1094 2023-05-10 12:01:26.000000 supervision-0.7.0/supervision/dataset/ultils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.932461 supervision-0.7.0/supervision/detection/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.7.0/supervision/detection/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     6799 2023-05-09 10:13:33.000000 supervision-0.7.0/supervision/detection/annotate.py
+-rw-r--r--   0 skalskip   (501) staff       (20)    20838 2023-05-10 12:01:26.000000 supervision-0.7.0/supervision/detection/core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     7589 2023-05-10 16:45:50.000000 supervision-0.7.0/supervision/detection/line_counter.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.932884 supervision-0.7.0/supervision/detection/tools/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-10 21:52:53.000000 supervision-0.7.0/supervision/detection/tools/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5056 2023-04-19 14:17:19.000000 supervision-0.7.0/supervision/detection/tools/polygon_zone.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     9634 2023-04-19 14:17:19.000000 supervision-0.7.0/supervision/detection/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.933487 supervision-0.7.0/supervision/draw/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.7.0/supervision/draw/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     3675 2023-02-07 18:30:08.000000 supervision-0.7.0/supervision/draw/color.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5147 2023-03-13 13:53:19.000000 supervision-0.7.0/supervision/draw/utils.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1734 2023-05-10 12:01:26.000000 supervision-0.7.0/supervision/file.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.934052 supervision-0.7.0/supervision/geometry/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.7.0/supervision/geometry/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1397 2023-02-07 18:30:08.000000 supervision-0.7.0/supervision/geometry/core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)      993 2023-02-07 18:30:08.000000 supervision-0.7.0/supervision/geometry/utils.py
+-rw-r--r--   0 skalskip   (501) staff       (20)      421 2023-05-03 22:43:10.000000 supervision-0.7.0/supervision/internal.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.934382 supervision-0.7.0/supervision/notebook/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.7.0/supervision/notebook/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     2839 2023-05-03 22:43:10.000000 supervision-0.7.0/supervision/notebook/utils.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5049 2023-02-07 18:30:08.000000 supervision-0.7.0/supervision/video.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.930175 supervision-0.7.0/supervision.egg-info/
+-rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-05-10 22:44:27.000000 supervision-0.7.0/supervision.egg-info/PKG-INFO
+-rw-r--r--   0 skalskip   (501) staff       (20)     1286 2023-05-10 22:44:27.000000 supervision-0.7.0/supervision.egg-info/SOURCES.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)        1 2023-05-10 22:44:27.000000 supervision-0.7.0/supervision.egg-info/dependency_links.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)      138 2023-05-10 22:44:27.000000 supervision-0.7.0/supervision.egg-info/requires.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)       17 2023-05-10 22:44:27.000000 supervision-0.7.0/supervision.egg-info/top_level.txt
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.934625 supervision-0.7.0/test/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.7.0/test/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.934749 supervision-0.7.0/test/dataset/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-05-10 12:01:26.000000 supervision-0.7.0/test/dataset/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.934973 supervision-0.7.0/test/dataset/formats/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-05-10 12:01:26.000000 supervision-0.7.0/test/dataset/formats/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     6532 2023-05-10 12:01:26.000000 supervision-0.7.0/test/dataset/formats/test_yolo.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.935524 supervision-0.7.0/test/detection/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.7.0/test/detection/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     6749 2023-05-04 15:46:53.000000 supervision-0.7.0/test/detection/test_core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     8054 2023-04-19 14:17:19.000000 supervision-0.7.0/test/detection/test_utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.935791 supervision-0.7.0/test/draw/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.7.0/test/draw/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1097 2023-02-02 10:53:06.000000 supervision-0.7.0/test/draw/test_color.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-05-10 22:44:27.936169 supervision-0.7.0/test/geometry/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.7.0/test/geometry/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1854 2023-02-07 18:30:08.000000 supervision-0.7.0/test/geometry/test_dataclasses.py
```

### Comparing `supervision-0.6.0/LICENSE.md` & `supervision-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `supervision-0.6.0/PKG-INFO` & `supervision-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervision
-Version: 0.6.0
+Version: 0.7.0
 Summary: A set of easy-to-use utils that will come in handy in any Computer Vision project
 Home-page: https://github.com/roboflow/supervision
 Author: Piotr Skalski
 Author-email: piotr.skalski92@gmail.com
 License: MIT
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: supervision Version: 0.6.0 Summary: A set of easy-
+Metadata-Version: 2.1 Name: supervision Version: 0.7.0 Summary: A set of easy-
 to-use utils that will come in handy in any Computer Vision project Home-page:
 https://github.com/roboflow/supervision Author: Piotr Skalski Author-email:
 piotr.skalski92@gmail.com License: MIT Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `supervision-0.6.0/README.md` & `supervision-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `supervision-0.6.0/setup.py` & `supervision-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `supervision-0.6.0/supervision/__init__.py` & `supervision-0.7.0/supervision/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 from supervision.dataset.core import Dataset
 from supervision.detection.annotate import BoxAnnotator, MaskAnnotator
 from supervision.detection.core import Detections
 from supervision.detection.line_counter import LineZone, LineZoneAnnotator
 from supervision.detection.tools.polygon_zone import PolygonZone, PolygonZoneAnnotator
 from supervision.detection.utils import (
```

### Comparing `supervision-0.6.0/supervision/dataset/formats/pascal_voc.py` & `supervision-0.7.0/supervision/dataset/formats/pascal_voc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from typing import List, Optional, Tuple
 from xml.dom.minidom import parseString
 from xml.etree.ElementTree import Element, SubElement, parse, tostring
 
 import numpy as np
 
+from supervision.dataset.ultils import approximate_mask_with_polygons
 from supervision.detection.core import Detections
-from supervision.detection.utils import (
-    approximate_polygon,
-    filter_polygons_by_area,
-    mask_to_polygons,
-    polygon_to_xyxy,
-)
+from supervision.detection.utils import polygon_to_xyxy
 
 
 def object_to_pascal_voc(
     xyxy: np.ndarray, name: str, polygon: Optional[np.ndarray] = None
 ) -> Element:
     root = Element("object")
 
@@ -100,32 +96,24 @@
     segmented = SubElement(annotation, "segmented")
     segmented.text = "0"
 
     # Add object elements
     for xyxy, mask, _, class_id, _ in detections:
         name = classes[class_id]
         if mask is not None:
-            polygons = mask_to_polygons(mask=mask)
-            if len(polygons) == 1:
-                polygons = filter_polygons_by_area(
-                    polygons=polygons, min_area=None, max_area=maximum_detection_area
-                )
-            else:
-                polygons = filter_polygons_by_area(
-                    polygons=polygons,
-                    min_area=minimum_detection_area,
-                    max_area=maximum_detection_area,
-                )
+            polygons = approximate_mask_with_polygons(
+                mask=mask,
+                min_image_area_percentage=min_image_area_percentage,
+                max_image_area_percentage=max_image_area_percentage,
+                approximation_percentage=approximation_percentage,
+            )
             for polygon in polygons:
-                approx_polygon = approximate_polygon(
-                    polygon=polygon, percentage=approximation_percentage
-                )
-                xyxy = polygon_to_xyxy(polygon=approx_polygon)
+                xyxy = polygon_to_xyxy(polygon=polygon)
                 next_object = object_to_pascal_voc(
-                    xyxy=xyxy, name=name, polygon=approx_polygon
+                    xyxy=xyxy, name=name, polygon=polygon
                 )
                 annotation.append(next_object)
         else:
             next_object = object_to_pascal_voc(xyxy=xyxy, name=name)
             annotation.append(next_object)
 
     # Generate XML string
```

### Comparing `supervision-0.6.0/supervision/detection/annotate.py` & `supervision-0.7.0/supervision/detection/annotate.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,21 +43,42 @@
         detections: Detections,
         labels: Optional[List[str]] = None,
         skip_label: bool = False,
     ) -> np.ndarray:
         """
         Draws bounding boxes on the frame using the detections provided.
 
-        Parameters:
+        Args:
             scene (np.ndarray): The image on which the bounding boxes will be drawn
             detections (Detections): The detections for which the bounding boxes will be drawn
-            labels (Optional[List[str]]): An optional list of labels corresponding to each detection. If labels is provided, the confidence score of the detection will be replaced with the label.
-            skip_label (bool): Is set to True, skips bounding box label annotation.
+            labels (Optional[List[str]]): An optional list of labels corresponding to each detection. If `labels` are not provided, corresponding `class_id` will be used as label.
+            skip_label (bool): Is set to `True`, skips bounding box label annotation.
         Returns:
             np.ndarray: The image with the bounding boxes drawn on it
+
+        Example:
+            ```python
+            >>> import supervision as sv
+
+            >>> classes = ['person', ...]
+            >>> image = ...
+            >>> detections = sv.Detections(...)
+
+            >>> box_annotator = sv.BoxAnnotator()
+            >>> labels = [
+            ...     f"{classes[class_id]} {confidence:0.2f}"
+            ...     for _, _, confidence, class_id, _
+            ...     in detections
+            ... ]
+            >>> annotated_frame = box_annotator.annotate(
+            ...     scene=image.copy(),
+            ...     detections=detections,
+            ...     labels=labels
+            ... )
+            ```
         """
         font = cv2.FONT_HERSHEY_SIMPLEX
         for i in range(len(detections)):
             x1, y1, x2, y2 = detections.xyxy[i].astype(int)
             class_id = (
                 detections.class_id[i] if detections.class_id is not None else None
             )
@@ -135,15 +156,15 @@
 
     def annotate(
         self, scene: np.ndarray, detections: Detections, opacity: float = 0.5
     ) -> np.ndarray:
         """
         Overlays the masks on the given image based on the provided detections, with a specified opacity.
 
-        Parameters:
+        Args:
             scene (np.ndarray): The image on which the masks will be overlaid
             detections (Detections): The detections for which the masks will be overlaid
             opacity (float): The opacity of the masks, between 0 and 1, default is 0.5
 
         Returns:
             np.ndarray: The image with the masks overlaid
         """
```

### Comparing `supervision-0.6.0/supervision/detection/core.py` & `supervision-0.7.0/supervision/detection/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
+from dataclasses import astuple, dataclass
 from typing import Any, Iterator, List, Optional, Tuple
 
 import numpy as np
 
 from supervision.detection.utils import non_max_suppression, xywh_to_xyxy
 from supervision.geometry.core import Position
+from supervision.internal import deprecated
 
 
 def _validate_xyxy(xyxy: Any, n: int) -> None:
     is_valid = isinstance(xyxy, np.ndarray) and xyxy.shape == (n, 4)
     if not is_valid:
         raise ValueError("xyxy must be 2d np.ndarray with (n, 4) shape")
 
@@ -132,93 +133,184 @@
                 ),
             ]
         )
 
     @classmethod
     def from_yolov5(cls, yolov5_results) -> Detections:
         """
-        Creates a Detections instance from a YOLOv5 output Detections
+        Creates a Detections instance from a [YOLOv5](https://github.com/ultralytics/yolov5) inference result.
 
         Args:
             yolov5_results (yolov5.models.common.Detections): The output Detections instance from YOLOv5
 
         Returns:
             Detections: A new Detections object.
 
         Example:
             ```python
+            >>> import cv2
             >>> import torch
-            >>> from supervision import Detections
+            >>> import supervision as sv
 
+            >>> image = cv2.imread(SOURCE_IMAGE_PATH)
             >>> model = torch.hub.load('ultralytics/yolov5', 'yolov5s')
-            >>> results = model(IMAGE)
-            >>> detections = Detections.from_yolov5(results)
+            >>> result = model(image)
+            >>> detections = sv.Detections.from_yolov5(result)
             ```
         """
         yolov5_detections_predictions = yolov5_results.pred[0].cpu().cpu().numpy()
         return cls(
             xyxy=yolov5_detections_predictions[:, :4],
             confidence=yolov5_detections_predictions[:, 4],
             class_id=yolov5_detections_predictions[:, 5].astype(int),
         )
 
     @classmethod
     def from_yolov8(cls, yolov8_results) -> Detections:
         """
-        Creates a Detections instance from a YOLOv8 output Results
+        Creates a Detections instance from a [YOLOv8](https://github.com/ultralytics/ultralytics) inference result.
 
         Args:
             yolov8_results (ultralytics.yolo.engine.results.Results): The output Results instance from YOLOv8
 
         Returns:
             Detections: A new Detections object.
 
         Example:
             ```python
+            >>> import cv2
             >>> from ultralytics import YOLO
-            >>> from supervision import Detections
+            >>> import supervision as sv
 
+            >>> image = cv2.imread(SOURCE_IMAGE_PATH)
             >>> model = YOLO('yolov8s.pt')
-            >>> yolov8_results = model(IMAGE)[0]
-            >>> detections = Detections.from_yolov8(yolov8_results)
+            >>> result = model(image)[0]
+            >>> detections = sv.Detections.from_yolov8(result)
             ```
         """
         return cls(
             xyxy=yolov8_results.boxes.xyxy.cpu().numpy(),
             confidence=yolov8_results.boxes.conf.cpu().numpy(),
             class_id=yolov8_results.boxes.cls.cpu().numpy().astype(int),
         )
 
     @classmethod
+    def from_yolo_nas(cls, yolo_nas_results) -> Detections:
+        """
+        Creates a Detections instance from a [YOLO-NAS](https://github.com/Deci-AI/super-gradients/blob/master/YOLONAS.md) inference result.
+
+        Args:
+            yolo_nas_results (super_gradients.training.models.prediction_results.ImageDetectionPrediction): The output Results instance from YOLO-NAS
+
+        Returns:
+            Detections: A new Detections object.
+
+        Example:
+            ```python
+            >>> import cv2
+            >>> from super_gradients.training import models
+            >>> import supervision as sv
+
+            >>> image = cv2.imread(SOURCE_IMAGE_PATH)
+            >>> model = models.get('yolo_nas_l', pretrained_weights="coco")
+            >>> result = list(model.predict(image, conf=0.35))[0]
+            >>> detections = sv.Detections.from_yolo_nas(result)
+            ```
+        """
+        return cls(
+            xyxy=yolo_nas_results.prediction.bboxes_xyxy,
+            confidence=yolo_nas_results.prediction.confidence,
+            class_id=yolo_nas_results.prediction.labels.astype(int),
+        )
+
+    @classmethod
     def from_transformers(cls, transformers_results: dict) -> Detections:
         """
-        Creates a Detections instance from Object Detection Transformer output Results
+        Creates a Detections instance from object detection [transformer](https://github.com/huggingface/transformers) inference result.
 
         Returns:
             Detections: A new Detections object.
         """
         return cls(
             xyxy=transformers_results["boxes"].cpu().numpy(),
             confidence=transformers_results["scores"].cpu().numpy(),
             class_id=transformers_results["labels"].cpu().numpy().astype(int),
         )
 
     @classmethod
     def from_detectron2(cls, detectron2_results) -> Detections:
+        """
+        Create a Detections object from the [Detectron2](https://github.com/facebookresearch/detectron2) inference result.
+
+        Args:
+            detectron2_results: The output of a Detectron2 model containing instances with prediction data.
+
+        Returns:
+            (Detections): A Detections object containing the bounding boxes, class IDs, and confidences of the predictions.
+
+        Example:
+            ```python
+            >>> import cv2
+            >>> from detectron2.engine import DefaultPredictor
+            >>> from detectron2.config import get_cfg
+            >>> import supervision as sv
+
+            >>> image = cv2.imread(SOURCE_IMAGE_PATH)
+            >>> cfg = get_cfg()
+            >>> cfg.merge_from_file("path/to/config.yaml")
+            >>> cfg.MODEL.WEIGHTS = "path/to/model_weights.pth"
+            >>> predictor = DefaultPredictor(cfg)
+            >>> result = predictor(image)
+
+            >>> detections = sv.Detections.from_detectron2(result)
+            ```
+        """
         return cls(
             xyxy=detectron2_results["instances"].pred_boxes.tensor.cpu().numpy(),
             confidence=detectron2_results["instances"].scores.cpu().numpy(),
             class_id=detectron2_results["instances"]
             .pred_classes.cpu()
             .numpy()
             .astype(int),
         )
 
     @classmethod
     def from_roboflow(cls, roboflow_result: dict, class_list: List[str]) -> Detections:
+        """
+        Create a Detections object from the [Roboflow](https://roboflow.com/) API inference result.
+
+        Args:
+            roboflow_result (dict): The result from the Roboflow API containing predictions.
+            class_list (List[str]): A list of class names corresponding to the class IDs in the API result.
+
+        Returns:
+            (Detections): A Detections object containing the bounding boxes, class IDs, and confidences of the predictions.
+
+        Example:
+            ```python
+            >>> import supervision as sv
+
+            >>> roboflow_result = {
+            ...     "predictions": [
+            ...         {
+            ...             "x": 0.5,
+            ...             "y": 0.5,
+            ...             "width": 0.2,
+            ...             "height": 0.3,
+            ...             "class": "person",
+            ...             "confidence": 0.9
+            ...         },
+            ...         # ... more predictions ...
+            ...     ]
+            ... }
+            >>> class_list = ["person", "car", "dog"]
+
+            >>> detections = sv.Detections.from_roboflow(roboflow_result, class_list)
+            ```
+        """
         xyxy = []
         confidence = []
         class_id = []
 
         for prediction in roboflow_result["predictions"]:
             x = prediction["x"]
             y = prediction["y"]
@@ -237,26 +329,26 @@
             confidence=np.array(confidence),
             class_id=np.array(class_id).astype(int),
         )
 
     @classmethod
     def from_sam(cls, sam_result: List[dict]) -> Detections:
         """
-        Creates a Detections instance from Segment Anything Model (SAM) by Meta AI.
+        Creates a Detections instance from [Segment Anything Model](https://github.com/facebookresearch/segment-anything) inference result.
 
         Args:
             sam_result (List[dict]): The output Results instance from SAM
 
         Returns:
             Detections: A new Detections object.
 
         Example:
             ```python
-            >>> from segment_anything import sam_model_registry, SamAutomaticMaskGenerator
             >>> import supervision as sv
+            >>> from segment_anything import sam_model_registry, SamAutomaticMaskGenerator
 
             >>> sam = sam_model_registry[MODEL_TYPE](checkpoint=CHECKPOINT_PATH).to(device=DEVICE)
             >>> mask_generator = SamAutomaticMaskGenerator(sam)
             >>> sam_result = mask_generator.generate(IMAGE)
             >>> detections = sv.Detections.from_sam(sam_result=sam_result)
             ```
         """
@@ -266,32 +358,97 @@
 
         xywh = np.array([mask["bbox"] for mask in sorted_generated_masks])
         mask = np.array([mask["segmentation"] for mask in sorted_generated_masks])
 
         return Detections(xyxy=xywh_to_xyxy(boxes_xywh=xywh), mask=mask)
 
     @classmethod
+    @deprecated(
+        "Dataset loading and saving is going to be executed by supervision.dataset.core.Dataset"
+    )
     def from_coco_annotations(cls, coco_annotation: dict) -> Detections:
         xyxy, class_id = [], []
 
         for annotation in coco_annotation:
             x_min, y_min, width, height = annotation["bbox"]
             xyxy.append([x_min, y_min, x_min + width, y_min + height])
             class_id.append(annotation["category_id"])
 
         return cls(xyxy=np.array(xyxy), class_id=np.array(class_id))
 
     @classmethod
     def empty(cls) -> Detections:
+        """
+        Create an empty Detections object with no bounding boxes, confidences, or class IDs.
+
+        Returns:
+            (Detections): An empty Detections object.
+
+        Example:
+            ```python
+            >>> from supervision import Detections
+
+            >>> empty_detections = Detections.empty()
+            ```
+        """
         return cls(
             xyxy=np.empty((0, 4), dtype=np.float32),
             confidence=np.array([], dtype=np.float32),
             class_id=np.array([], dtype=int),
         )
 
+    @classmethod
+    def merge(cls, detections_list: List[Detections]) -> Detections:
+        """
+        Merge a list of Detections objects into a single Detections object.
+
+        This method takes a list of Detections objects and combines their respective fields (`xyxy`, `mask`,
+        `confidence`, `class_id`, and `tracker_id`) into a single Detections object. If all elements in a field are not
+        `None`, the corresponding field will be stacked. Otherwise, the field will be set to `None`.
+
+        Args:
+            detections_list (List[Detections]): A list of Detections objects to merge.
+
+        Returns:
+            (Detections): A single Detections object containing the merged data from the input list.
+
+        Example:
+            ```python
+            >>> from supervision import Detections
+
+            >>> detections_1 = Detections(...)
+            >>> detections_2 = Detections(...)
+
+            >>> merged_detections = Detections.merge([detections_1, detections_2])
+            ```
+        """
+        if len(detections_list) == 0:
+            return Detections.empty()
+
+        detections_tuples_list = [astuple(detection) for detection in detections_list]
+        xyxy, mask, confidence, class_id, tracker_id = [
+            list(field) for field in zip(*detections_tuples_list)
+        ]
+
+        all_not_none = lambda l: all(x is not None for x in l)
+
+        xyxy = np.vstack(xyxy)
+        mask = np.vstack(mask) if all_not_none(mask) else None
+        confidence = np.hstack(confidence) if all_not_none(confidence) else None
+        class_id = np.hstack(class_id) if all_not_none(class_id) else None
+        tracker_id = np.hstack(tracker_id) if all_not_none(tracker_id) else None
+
+        return cls(
+            xyxy=xyxy,
+            mask=mask,
+            confidence=confidence,
+            class_id=class_id,
+            tracker_id=tracker_id,
+        )
+
     def get_anchor_coordinates(self, anchor: Position) -> np.ndarray:
         """
         Returns the bounding box coordinates for a specific anchor.
 
         Args:
             anchor (Position): Position of bounding box anchor for which to return the coordinates.
```

### Comparing `supervision-0.6.0/supervision/detection/line_counter.py` & `supervision-0.7.0/supervision/detection/line_counter.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import cv2
 import numpy as np
 
 from supervision.detection.core import Detections
 from supervision.draw.color import Color
 from supervision.geometry.core import Point, Rect, Vector
+from typing import Optional
 
 
 class LineZone:
     """
     Count the number of objects that cross a line.
     """
 
@@ -66,25 +67,26 @@
 
             self.tracker_state[tracker_id] = tracker_state
             if tracker_state:
                 self.in_count += 1
             else:
                 self.out_count += 1
 
-
 class LineZoneAnnotator:
     def __init__(
         self,
         thickness: float = 2,
         color: Color = Color.white(),
         text_thickness: float = 2,
         text_color: Color = Color.black(),
         text_scale: float = 0.5,
         text_offset: float = 1.5,
         text_padding: int = 10,
+        custom_in_text: Optional[str] = None,
+        custom_out_text: Optional[str] = None,
     ):
         """
         Initialize the LineCounterAnnotator object with default values.
 
         Attributes:
             thickness (float): The thickness of the line that will be drawn.
             color (Color): The color of the line that will be drawn.
@@ -98,14 +100,16 @@
         self.thickness: float = thickness
         self.color: Color = color
         self.text_thickness: float = text_thickness
         self.text_color: Color = text_color
         self.text_scale: float = text_scale
         self.text_offset: float = text_offset
         self.text_padding: int = text_padding
+        self.custom_in_text: str = custom_in_text
+        self.custom_out_text: str = custom_out_text
 
     def annotate(self, frame: np.ndarray, line_counter: LineZone) -> np.ndarray:
         """
         Draws the line on the frame using the line_counter provided.
 
         Attributes:
             frame (np.ndarray): The image on which the line will be drawn.
@@ -137,16 +141,17 @@
             line_counter.vector.end.as_xy_int_tuple(),
             radius=5,
             color=self.text_color.as_bgr(),
             thickness=-1,
             lineType=cv2.LINE_AA,
         )
 
-        in_text = f"in: {line_counter.in_count}"
-        out_text = f"out: {line_counter.out_count}"
+        in_text = f"{self.custom_in_text}: {line_counter.in_count}" if self.custom_in_text is not None else f"in: {line_counter.in_count}"
+        out_text = f"{self.custom_out_text}: {line_counter.out_count}" if self.custom_out_text is not None else f"out: {line_counter.out_count}"
+
 
         (in_text_width, in_text_height), _ = cv2.getTextSize(
             in_text, cv2.FONT_HERSHEY_SIMPLEX, self.text_scale, self.text_thickness
         )
         (out_text_width, out_text_height), _ = cv2.getTextSize(
             out_text, cv2.FONT_HERSHEY_SIMPLEX, self.text_scale, self.text_thickness
         )
@@ -215,7 +220,8 @@
             (out_text_x, out_text_y),
             cv2.FONT_HERSHEY_SIMPLEX,
             self.text_scale,
             self.text_color.as_bgr(),
             self.text_thickness,
             cv2.LINE_AA,
         )
+        return frame
```

### Comparing `supervision-0.6.0/supervision/detection/tools/polygon_zone.py` & `supervision-0.7.0/supervision/detection/tools/polygon_zone.py`

 * *Files identical despite different names*

### Comparing `supervision-0.6.0/supervision/detection/utils.py` & `supervision-0.7.0/supervision/detection/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.6.0/supervision/draw/color.py` & `supervision-0.7.0/supervision/draw/color.py`

 * *Files identical despite different names*

### Comparing `supervision-0.6.0/supervision/draw/utils.py` & `supervision-0.7.0/supervision/draw/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.6.0/supervision/geometry/core.py` & `supervision-0.7.0/supervision/geometry/core.py`

 * *Files identical despite different names*

### Comparing `supervision-0.6.0/supervision/geometry/utils.py` & `supervision-0.7.0/supervision/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.6.0/supervision/notebook/utils.py` & `supervision-0.7.0/supervision/notebook/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         ```python
         >>> import cv2
         >>> import supervision as sv
 
         >>> image = cv2.imread("path/to/image.jpg")
 
         %matplotlib inline
-        >>> sv.plot_image(image, (16, 16))
+        >>> sv.plot_image(image=image, size=(16, 16))
         ```
     """
     plt.figure(figsize=size)
 
     if image.ndim == 2:
         plt.imshow(image, cmap=cmap)
     else:
@@ -67,15 +67,15 @@
         >>> image2 = cv2.imread("path/to/image2.jpg")
         >>> image3 = cv2.imread("path/to/image3.jpg")
 
         >>> images = [image1, image2, image3]
         >>> titles = ["Image 1", "Image 2", "Image 3"]
 
         %matplotlib inline
-        >>> plot_images_grid(images, grid_size=(2, 2), titles=titles, figsize=(16, 16))
+        >>> plot_images_grid(images, grid_size=(2, 2), titles=titles, size=(16, 16))
         ```
     """
     nrows, ncols = grid_size
 
     if len(images) > nrows * ncols:
         raise ValueError(
             "The number of images exceeds the grid size. Please increase the grid size or reduce the number of images."
```

### Comparing `supervision-0.6.0/supervision/video.py` & `supervision-0.7.0/supervision/video.py`

 * *Files identical despite different names*

### Comparing `supervision-0.6.0/supervision.egg-info/PKG-INFO` & `supervision-0.7.0/supervision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervision
-Version: 0.6.0
+Version: 0.7.0
 Summary: A set of easy-to-use utils that will come in handy in any Computer Vision project
 Home-page: https://github.com/roboflow/supervision
 Author: Piotr Skalski
 Author-email: piotr.skalski92@gmail.com
 License: MIT
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: supervision Version: 0.6.0 Summary: A set of easy-
+Metadata-Version: 2.1 Name: supervision Version: 0.7.0 Summary: A set of easy-
 to-use utils that will come in handy in any Computer Vision project Home-page:
 https://github.com/roboflow/supervision Author: Piotr Skalski Author-email:
 piotr.skalski92@gmail.com License: MIT Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `supervision-0.6.0/supervision.egg-info/SOURCES.txt` & `supervision-0.7.0/supervision.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 LICENSE.md
 README.md
 setup.py
 supervision/__init__.py
 supervision/file.py
+supervision/internal.py
 supervision/video.py
 supervision.egg-info/PKG-INFO
 supervision.egg-info/SOURCES.txt
 supervision.egg-info/dependency_links.txt
 supervision.egg-info/requires.txt
 supervision.egg-info/top_level.txt
 supervision/dataset/__init__.py
 supervision/dataset/core.py
+supervision/dataset/ultils.py
 supervision/dataset/formats/__init__.py
 supervision/dataset/formats/pascal_voc.py
+supervision/dataset/formats/yolo.py
 supervision/detection/__init__.py
 supervision/detection/annotate.py
 supervision/detection/core.py
 supervision/detection/line_counter.py
 supervision/detection/utils.py
 supervision/detection/tools/__init__.py
 supervision/detection/tools/polygon_zone.py
@@ -25,14 +28,17 @@
 supervision/draw/utils.py
 supervision/geometry/__init__.py
 supervision/geometry/core.py
 supervision/geometry/utils.py
 supervision/notebook/__init__.py
 supervision/notebook/utils.py
 test/__init__.py
+test/dataset/__init__.py
+test/dataset/formats/__init__.py
+test/dataset/formats/test_yolo.py
 test/detection/__init__.py
 test/detection/test_core.py
 test/detection/test_utils.py
 test/draw/__init__.py
 test/draw/test_color.py
 test/geometry/__init__.py
 test/geometry/test_dataclasses.py
```

### Comparing `supervision-0.6.0/test/detection/test_utils.py` & `supervision-0.7.0/test/detection/test_utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.6.0/test/draw/test_color.py` & `supervision-0.7.0/test/draw/test_color.py`

 * *Files identical despite different names*

### Comparing `supervision-0.6.0/test/geometry/test_dataclasses.py` & `supervision-0.7.0/test/geometry/test_dataclasses.py`

 * *Files identical despite different names*

