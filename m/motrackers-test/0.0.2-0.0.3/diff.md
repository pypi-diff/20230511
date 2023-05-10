# Comparing `tmp/motrackers_test-0.0.2.tar.gz` & `tmp/motrackers_test-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motrackers_test-0.0.2.tar", last modified: Wed May 10 22:02:42 2023, max compression
+gzip compressed data, was "motrackers_test-0.0.3.tar", last modified: Wed May 10 22:21:40 2023, max compression
```

## Comparing `motrackers_test-0.0.2.tar` & `motrackers_test-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:02:42.426979 motrackers_test-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-10 22:02:42.426979 motrackers_test-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:02:42.418979 motrackers_test-0.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:02:42.418979 motrackers_test-0.0.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:02:42.418979 motrackers_test-0.0.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:02:42.418979 motrackers_test-0.0.2/examples/example_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/examples/example_scripts/detector_Caffe_SSDMobileNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/examples/example_scripts/detector_TF_SSDMobileNetV2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/examples/example_scripts/detector_YOLOv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/examples/example_scripts/mot_Caffe_SSDMobileNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/examples/example_scripts/mot_TF_SSDMobileNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/examples/example_scripts/mot_YOLOv3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:02:42.422979 motrackers_test-0.0.2/examples/motmetrics_eval/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/examples/motmetrics_eval/motmeterics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:02:42.422979 motrackers_test-0.0.2/motrackers/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/centroid_kf_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:02:42.422979 motrackers_test-0.0.2/motrackers/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/detectors/caffe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/detectors/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/detectors/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/detectors/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/iou_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/kalman_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/sort_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/tracker_img.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:02:42.422979 motrackers_test-0.0.2/motrackers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/utils/filechooser_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/motrackers/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:02:42.426979 motrackers_test-0.0.2/motrackers_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-10 22:02:42.000000 motrackers_test-0.0.2/motrackers_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-10 22:02:42.000000 motrackers_test-0.0.2/motrackers_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:02:42.000000 motrackers_test-0.0.2/motrackers_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-10 22:02:42.000000 motrackers_test-0.0.2/motrackers_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 22:02:42.000000 motrackers_test-0.0.2/motrackers_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-10 22:02:09.000000 motrackers_test-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 22:02:42.426979 motrackers_test-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:21:40.291017 motrackers_test-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-10 22:21:40.291017 motrackers_test-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:21:40.287017 motrackers_test-0.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:21:40.291017 motrackers_test-0.0.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:21:40.287017 motrackers_test-0.0.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:21:40.291017 motrackers_test-0.0.3/examples/example_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/examples/example_scripts/detector_Caffe_SSDMobileNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/examples/example_scripts/detector_TF_SSDMobileNetV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/examples/example_scripts/detector_YOLOv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/examples/example_scripts/mot_Caffe_SSDMobileNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/examples/example_scripts/mot_TF_SSDMobileNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/examples/example_scripts/mot_YOLOv3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:21:40.291017 motrackers_test-0.0.3/examples/motmetrics_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/examples/motmetrics_eval/motmeterics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:21:40.291017 motrackers_test-0.0.3/motrackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/centroid_kf_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:21:40.291017 motrackers_test-0.0.3/motrackers/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/detectors/caffe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/detectors/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/detectors/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/detectors/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/iou_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/kalman_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/sort_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/tracker_img.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:21:40.291017 motrackers_test-0.0.3/motrackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/utils/filechooser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/motrackers/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:21:40.291017 motrackers_test-0.0.3/motrackers_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-10 22:21:40.000000 motrackers_test-0.0.3/motrackers_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-10 22:21:40.000000 motrackers_test-0.0.3/motrackers_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:21:40.000000 motrackers_test-0.0.3/motrackers_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-10 22:21:40.000000 motrackers_test-0.0.3/motrackers_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 22:21:40.000000 motrackers_test-0.0.3/motrackers_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-10 22:21:15.000000 motrackers_test-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 22:21:40.291017 motrackers_test-0.0.3/setup.cfg
```

### Comparing `motrackers_test-0.0.2/LICENSE` & `motrackers_test-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/PKG-INFO` & `motrackers_test-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motrackers_test
-Version: 0.0.2
+Version: 0.0.3
 Summary: Multi-object trackers in Python
 Author-email: "Aditya M. Deshpande" <adityadeshpande2010@gmail.com>
 Project-URL: homepath, https://adipandas.github.io/multi-object-tracker
 Project-URL: repository, https://github.com/adipandas/multi-object-tracker
 Keywords: tracking,object,multi-object,python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >3.6
```

### Comparing `motrackers_test-0.0.2/README.md` & `motrackers_test-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/docs/source/conf.py` & `motrackers_test-0.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/examples/example_scripts/detector_Caffe_SSDMobileNet.py` & `motrackers_test-0.0.3/examples/example_scripts/detector_Caffe_SSDMobileNet.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/examples/example_scripts/detector_TF_SSDMobileNetV2.py` & `motrackers_test-0.0.3/examples/example_scripts/detector_TF_SSDMobileNetV2.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/examples/example_scripts/detector_YOLOv3.py` & `motrackers_test-0.0.3/examples/example_scripts/detector_YOLOv3.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/examples/example_scripts/mot_Caffe_SSDMobileNet.py` & `motrackers_test-0.0.3/examples/example_scripts/mot_Caffe_SSDMobileNet.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/examples/example_scripts/mot_TF_SSDMobileNet.py` & `motrackers_test-0.0.3/examples/example_scripts/mot_TF_SSDMobileNet.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/examples/example_scripts/mot_YOLOv3.py` & `motrackers_test-0.0.3/examples/example_scripts/mot_YOLOv3.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/examples/motmetrics_eval/motmeterics.py` & `motrackers_test-0.0.3/examples/motmetrics_eval/motmeterics.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/centroid_kf_tracker.py` & `motrackers_test-0.0.3/motrackers/centroid_kf_tracker.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/detectors/caffe.py` & `motrackers_test-0.0.3/motrackers/detectors/caffe.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/detectors/detector.py` & `motrackers_test-0.0.3/motrackers/detectors/detector.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/detectors/tf.py` & `motrackers_test-0.0.3/motrackers/detectors/tf.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/detectors/yolo.py` & `motrackers_test-0.0.3/motrackers/detectors/yolo.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/iou_tracker.py` & `motrackers_test-0.0.3/motrackers/iou_tracker.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/kalman_tracker.py` & `motrackers_test-0.0.3/motrackers/kalman_tracker.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/sort_tracker.py` & `motrackers_test-0.0.3/motrackers/sort_tracker.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/track.py` & `motrackers_test-0.0.3/motrackers/track.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/tracker.py` & `motrackers_test-0.0.3/motrackers/tracker.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/tracker_img.py` & `motrackers_test-0.0.3/motrackers/tracker_img.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/utils/filechooser_utils.py` & `motrackers_test-0.0.3/motrackers/utils/filechooser_utils.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers/utils/misc.py` & `motrackers_test-0.0.3/motrackers/utils/misc.py`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/motrackers_test.egg-info/PKG-INFO` & `motrackers_test-0.0.3/motrackers_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motrackers-test
-Version: 0.0.2
+Version: 0.0.3
 Summary: Multi-object trackers in Python
 Author-email: "Aditya M. Deshpande" <adityadeshpande2010@gmail.com>
 Project-URL: homepath, https://adipandas.github.io/multi-object-tracker
 Project-URL: repository, https://github.com/adipandas/multi-object-tracker
 Keywords: tracking,object,multi-object,python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >3.6
```

### Comparing `motrackers_test-0.0.2/motrackers_test.egg-info/SOURCES.txt` & `motrackers_test-0.0.3/motrackers_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `motrackers_test-0.0.2/pyproject.toml` & `motrackers_test-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "motrackers_test"
-version = "0.0.2"
+version = "0.0.3"
 description = "Multi-object trackers in Python"
 authors = [
     {name = "Aditya M. Deshpande", email = "adityadeshpande2010@gmail.com"}
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 requires-python = ">3.6"
```

