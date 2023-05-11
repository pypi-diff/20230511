# Comparing `tmp/efemarai-0.3.4.tar.gz` & `tmp/efemarai-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efemarai-0.3.4.tar", last modified: Tue Apr 18 19:18:36 2023, max compression
+gzip compressed data, was "efemarai-0.3.5.tar", last modified: Thu May 11 12:22:38 2023, max compression
```

## Comparing `efemarai-0.3.4.tar` & `efemarai-0.3.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:18:36.086872 efemarai-0.3.4/
--rw-r--r--   0 root         (0) root         (0)     2763 2023-04-18 19:18:36.086872 efemarai-0.3.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2459 2023-04-18 12:01:21.000000 efemarai-0.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:18:36.086872 efemarai-0.3.4/efemarai/
--rw-rw-r--   0 root         (0) root         (0)      363 2023-04-18 19:17:37.000000 efemarai-0.3.4/efemarai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      931 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/base_checker.py
--rw-rw-r--   0 root         (0) root         (0)     4484 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/baseline.py
--rw-rw-r--   0 root         (0) root         (0)    34699 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/cli.py
--rw-rw-r--   0 root         (0) root         (0)       54 2022-08-08 14:41:49.000000 efemarai-0.3.4/efemarai/console.py
--rw-rw-r--   0 root         (0) root         (0)    17571 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/dataset.py
--rw-rw-r--   0 root         (0) root         (0)    12675 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/definition_checker.py
--rw-rw-r--   0 root         (0) root         (0)     3204 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:18:36.086872 efemarai-0.3.4/efemarai/fields/
--rw-rw-r--   0 root         (0) root         (0)     2037 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/fields/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    22788 2023-04-18 16:53:02.000000 efemarai-0.3.4/efemarai/fields/annotation_fields.py
--rw-rw-r--   0 root         (0) root         (0)     3605 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/fields/base_fields.py
--rw-rw-r--   0 root         (0) root         (0)    16180 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/fields/data_fields.py
--rw-rw-r--   0 root         (0) root         (0)     9485 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/fields/datapoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:18:36.086872 efemarai-0.3.4/efemarai/formats/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/formats/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      757 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/formats/config.py
--rw-rw-r--   0 root         (0) root         (0)     6690 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/formats/dataset_coco.py
--rw-rw-r--   0 root         (0) root         (0)     2023 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/formats/dataset_imagenet.py
--rw-rw-r--   0 root         (0) root         (0)      505 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/job_state.py
--rw-rw-r--   0 root         (0) root         (0)    13695 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/model.py
--rw-rw-r--   0 root         (0) root         (0)      547 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/problem_type.py
--rw-rw-r--   0 root         (0) root         (0)    25413 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/project.py
--rw-rw-r--   0 root         (0) root         (0)    13777 2023-03-20 16:49:10.000000 efemarai-0.3.4/efemarai/runtime_checker.py
--rw-rw-r--   0 root         (0) root         (0)    13047 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/session.py
--rw-rw-r--   0 root         (0) root         (0)     8960 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/stress_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:18:36.086872 efemarai-0.3.4/efemarai.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     2763 2023-04-18 19:18:36.000000 efemarai-0.3.4/efemarai.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      855 2023-04-18 19:18:36.000000 efemarai-0.3.4/efemarai.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-18 19:18:36.000000 efemarai-0.3.4/efemarai.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       70 2023-04-18 19:18:36.000000 efemarai-0.3.4/efemarai.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2022-07-25 12:08:08.000000 efemarai-0.3.4/efemarai.egg-info/not-zip-safe
--rw-rw-r--   0 root         (0) root         (0)      348 2023-04-18 19:18:36.000000 efemarai-0.3.4/efemarai.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2023-04-18 19:18:36.000000 efemarai-0.3.4/efemarai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 19:18:36.086872 efemarai-0.3.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1421 2023-04-18 12:01:21.000000 efemarai-0.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:22:38.479072 efemarai-0.3.5/
+-rw-r--r--   0 root         (0) root         (0)     9772 2023-05-11 12:22:38.479072 efemarai-0.3.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     9468 2023-05-11 12:21:44.000000 efemarai-0.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:22:38.475076 efemarai-0.3.5/efemarai/
+-rw-rw-r--   0 root         (0) root         (0)      363 2023-05-11 12:22:06.000000 efemarai-0.3.5/efemarai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      931 2023-04-14 14:40:33.000000 efemarai-0.3.5/efemarai/base_checker.py
+-rw-rw-r--   0 root         (0) root         (0)     4530 2023-05-02 14:22:12.000000 efemarai-0.3.5/efemarai/baseline.py
+-rw-rw-r--   0 root         (0) root         (0)    34647 2023-05-11 12:21:44.000000 efemarai-0.3.5/efemarai/cli.py
+-rw-rw-r--   0 root         (0) root         (0)       54 2022-07-27 12:37:35.000000 efemarai-0.3.5/efemarai/console.py
+-rw-rw-r--   0 root         (0) root         (0)    17560 2023-05-11 12:21:44.000000 efemarai-0.3.5/efemarai/dataset.py
+-rw-rw-r--   0 root         (0) root         (0)    12675 2023-04-14 14:40:33.000000 efemarai-0.3.5/efemarai/definition_checker.py
+-rw-rw-r--   0 root         (0) root         (0)     3204 2023-04-14 14:40:33.000000 efemarai-0.3.5/efemarai/domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:22:38.479072 efemarai-0.3.5/efemarai/fields/
+-rw-rw-r--   0 root         (0) root         (0)     2037 2023-04-14 14:40:33.000000 efemarai-0.3.5/efemarai/fields/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22788 2023-04-21 16:11:57.000000 efemarai-0.3.5/efemarai/fields/annotation_fields.py
+-rw-rw-r--   0 root         (0) root         (0)     3605 2023-04-18 12:44:31.000000 efemarai-0.3.5/efemarai/fields/base_fields.py
+-rw-rw-r--   0 root         (0) root         (0)    16220 2023-05-11 12:21:44.000000 efemarai-0.3.5/efemarai/fields/data_fields.py
+-rw-rw-r--   0 root         (0) root         (0)     9509 2023-05-11 12:21:44.000000 efemarai-0.3.5/efemarai/fields/datapoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:22:38.479072 efemarai-0.3.5/efemarai/formats/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-14 14:40:33.000000 efemarai-0.3.5/efemarai/formats/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      757 2023-04-14 14:40:33.000000 efemarai-0.3.5/efemarai/formats/config.py
+-rw-rw-r--   0 root         (0) root         (0)     6690 2023-04-14 14:40:33.000000 efemarai-0.3.5/efemarai/formats/dataset_coco.py
+-rw-rw-r--   0 root         (0) root         (0)     2031 2023-05-02 14:22:12.000000 efemarai-0.3.5/efemarai/formats/dataset_imagenet.py
+-rw-rw-r--   0 root         (0) root         (0)      505 2023-04-14 14:40:33.000000 efemarai-0.3.5/efemarai/job_state.py
+-rw-rw-r--   0 root         (0) root         (0)    13695 2023-04-14 14:40:33.000000 efemarai-0.3.5/efemarai/model.py
+-rw-rw-r--   0 root         (0) root         (0)      547 2023-04-14 14:40:33.000000 efemarai-0.3.5/efemarai/problem_type.py
+-rw-rw-r--   0 root         (0) root         (0)    25413 2023-04-14 14:40:33.000000 efemarai-0.3.5/efemarai/project.py
+-rw-rw-r--   0 root         (0) root         (0)    13743 2023-05-11 12:21:44.000000 efemarai-0.3.5/efemarai/runtime_checker.py
+-rw-rw-r--   0 root         (0) root         (0)    13047 2023-04-14 14:40:33.000000 efemarai-0.3.5/efemarai/session.py
+-rw-rw-r--   0 root         (0) root         (0)     9014 2023-05-02 14:22:12.000000 efemarai-0.3.5/efemarai/stress_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:22:38.475076 efemarai-0.3.5/efemarai.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     9772 2023-05-11 12:22:38.000000 efemarai-0.3.5/efemarai.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      855 2023-05-11 12:22:38.000000 efemarai-0.3.5/efemarai.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-11 12:22:38.000000 efemarai-0.3.5/efemarai.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       70 2023-05-11 12:22:38.000000 efemarai-0.3.5/efemarai.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2022-03-31 08:40:32.000000 efemarai-0.3.5/efemarai.egg-info/not-zip-safe
+-rw-rw-r--   0 root         (0) root         (0)      348 2023-05-11 12:22:38.000000 efemarai-0.3.5/efemarai.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-05-11 12:22:38.000000 efemarai-0.3.5/efemarai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 12:22:38.479072 efemarai-0.3.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1421 2023-04-14 14:40:33.000000 efemarai-0.3.5/setup.py
```

### Comparing `efemarai-0.3.4/efemarai/base_checker.py` & `efemarai-0.3.5/efemarai/base_checker.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.4/efemarai/baseline.py` & `efemarai-0.3.5/efemarai/baseline.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,23 +90,25 @@
         res += "\n)"
         return res
 
     @property
     def model(self):
         """Returns the model associated with the baseline."""
         if self._model is None:
-            self._model = next(m for m in self.project.models if m.id == self._model_id)
+            self._model = next(
+                (m for m in self.project.models if m.id == self._model_id), None
+            )
         return self._model
 
     @property
     def dataset(self):
         """Returns the dataset associated with the baseline."""
         if self._dataset is None:
             self._dataset = next(
-                d for d in self.project.datasets if d.id == self._dataset_id
+                (d for d in self.project.datasets if d.id == self._dataset_id), None
             )
         return self._dataset
 
     @property
     def finished(self):
         """Returns if the baseline has successfully finished.
```

### Comparing `efemarai-0.3.4/efemarai/cli.py` & `efemarai-0.3.5/efemarai/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 from rich.prompt import Confirm
 from rich.table import Table
 
 import efemarai as ef
 from efemarai.console import console
 from efemarai.definition_checker import DefinitionChecker
 
-# import click_completion
-# click_completion.init()
 checker = DefinitionChecker()
 
 default_yaml = "efemarai.yaml"
 
 
 @click.group()
 @click.version_option(ef.__version__)
```

### Comparing `efemarai-0.3.4/efemarai/dataset.py` & `efemarai-0.3.5/efemarai/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,15 +370,15 @@
                 style="red",
             )
             return None
 
         return annotations[0]
 
     def finalize(self, min_asset_area=15, mask_generation=None):
-        response = self.project._put(
+        self.project._put(
             f"api/dataset/{self.id}/finalize",
             json={
                 "classes": [_cls._serialize() for _cls in self.classes],
                 "asset": {
                     "min_asset_area": min_asset_area,
                     "mask_generation": mask_generation,
                 },
```

### Comparing `efemarai-0.3.4/efemarai/definition_checker.py` & `efemarai-0.3.5/efemarai/definition_checker.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.4/efemarai/domain.py` & `efemarai-0.3.5/efemarai/domain.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.4/efemarai/fields/__init__.py` & `efemarai-0.3.5/efemarai/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.4/efemarai/fields/annotation_fields.py` & `efemarai-0.3.5/efemarai/fields/annotation_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,16 +511,16 @@
             confidence=confidence,
             id=id,
             description=description,
             ref_field=ref_field,
             key_name=key_name,
             user_attributes=user_attributes,
         )
-        self.x = x if not isinstance(i, (np.int64, np.int32)) else i.item()
-        self.y = y if not isinstance(i, (np.int64, np.int32)) else i.item()
+        self.x = x if not isinstance(x, (np.int64, np.int32)) else x.item()
+        self.y = y if not isinstance(y, (np.int64, np.int32)) else y.item()
         self.name = name
         self.index = index
         self.annotated = annotated
         self.occluded = occluded
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
```

### Comparing `efemarai-0.3.4/efemarai/fields/base_fields.py` & `efemarai-0.3.5/efemarai/fields/base_fields.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.4/efemarai/fields/data_fields.py` & `efemarai-0.3.5/efemarai/fields/data_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,16 @@
 
 from efemarai.fields.annotation_fields import AnnotationClass, InstanceField, Polygon
 from efemarai.fields.base_fields import BaseField, sdk_serialize
 
 
 def create_polygons_from_mask(mask_img, threshold_value=127):
     # Get contours as polygons and the area of the polygons
-    ret, thresh = cv2.threshold(mask_img, threshold_value, 255, 0)
-    (
-        contours,
-        hierarchy,
-    ) = cv2.findContours(  # Format: [[[[x1, y1]], [[x2, y2]]...], ...]
+    _, thresh = cv2.threshold(mask_img, threshold_value, 255, 0)
+    (contours, _,) = cv2.findContours(  # Format: [[[[x1, y1]], [[x2, y2]]...], ...]
         thresh, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
     )
     if not contours:
         return ([], 0)
 
     polygons_area = 0
     polygons = []  # Format: [[x1, y1, x2, y2...], []]
@@ -143,14 +140,18 @@
         if self._raw.dtype != np.uint8:
             raise AssertionError(f"Expected format {np.uint8}. Received {data.dtype}.")
 
         self._raw = data
         self.height = self._raw.shape[0]
         self.width = self._raw.shape[1]
 
+    @data.setter
+    def data(self, data):
+        self.set_data(data)
+
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  id={self.id}"
         res += f"\n  file_path={self.file_path}"
         res += "\n  data=" + (
             f"{self._raw.shape}, {self._raw.dtype}, min({np.min(self._raw)}), max({np.max(self._raw)})"
             if self._raw is not None
```

### Comparing `efemarai-0.3.4/efemarai/fields/datapoint.py` & `efemarai-0.3.5/efemarai/fields/datapoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,19 +92,19 @@
         Returns:
             inputs: list[BaseField]
 
         """
         self.inputs.append(_input)
         return self.inputs
 
-    def _post(self, endpoint, json=None, params=None):
-        return self.dataset.project._session._post(endpoint, json, params)
+    def _post(self, endpoint, json_obj=None, params=None):
+        return self.dataset.project._session._post(endpoint, json_obj, params)
 
-    def _put(self, endpoint, json=None, params=None):
-        return self.dataset.project._put(endpoint, json, params)
+    def _put(self, endpoint, json_obj=None, params=None):
+        return self.dataset.project._put(endpoint, json_obj, params)
 
     def _handle_video(self, ef_video):
         with tempfile.TemporaryDirectory() as TMP_VIDEO_FRAME_DIR:
             video_info = ffmpeg.probe(ef_video.file_path)["streams"]
             width = [info["width"] for info in video_info if info.get("width")][0]
             height = [info["height"] for info in video_info if info.get("height")][0]
 
@@ -180,15 +180,15 @@
         serialized_targets = [
             json.loads(target._serialize()) for target in self.targets
         ]
         serialized_inputs = [json.loads(_input._serialize()) for _input in self.inputs]
 
         response = self._put(
             "api/datapoint/undefined",
-            json={
+            json_obj={
                 "access_token": self.dataset.project._session.token,
                 "datasetId": self.dataset.id,
                 "targets": serialized_targets,
                 "inputs": serialized_inputs,
             },
         )
 
@@ -232,15 +232,15 @@
 
             images = datapoints[0].get_inputs_with_type(ef.Image)
             # images is a list of all of the ef.Image elements in datapoints[0].
             # each of those images can be accessed by datapoints[0].get_input(images[0].key_name)
         """
         res = []
         for _input in self.inputs:
-            if ef_type is type(Video):
+            if isinstance(ef_type, Video):
                 res.append(_input)
                 continue
             if isinstance(_input, ef_type):
                 res.append(_input)
             if _input._cls == "Video":
                 # TODO: Use frame.index when indexes start from 0. Currently they start at 1.
                 for idx, frame in enumerate(_input.frames):
```

### Comparing `efemarai-0.3.4/efemarai/formats/config.py` & `efemarai-0.3.5/efemarai/formats/config.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.4/efemarai/formats/dataset_coco.py` & `efemarai-0.3.5/efemarai/formats/dataset_coco.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.4/efemarai/formats/dataset_imagenet.py` & `efemarai-0.3.5/efemarai/formats/dataset_imagenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ):
     """Upload an ImageNet style dataset in the system."""
     dataset = project.create_dataset(
         name=name, stage=stage, format=DatasetFormat.Custom
     )
 
     # Creating classes based on folders
-    classes = sorted(next(os.walk(data_url.replace("file://", "", 1)))[1])
+    classes = sorted(next((os.walk(data_url.replace("file://", "", 1))), None)[1])
 
     for i, class_name in enumerate(classes):
         dataset.add_annotation_class(
             id=i,
             name=class_name,
             color=CLASS_COLORS[i % len(CLASS_COLORS)],
         )
```

### Comparing `efemarai-0.3.4/efemarai/model.py` & `efemarai-0.3.5/efemarai/model.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.4/efemarai/problem_type.py` & `efemarai-0.3.5/efemarai/problem_type.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.4/efemarai/project.py` & `efemarai-0.3.5/efemarai/project.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.4/efemarai/runtime_checker.py` & `efemarai-0.3.5/efemarai/runtime_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,18 +274,18 @@
 
         if len(images) != len(predictions):
             self._error(
                 f"Invalid number of predictions: expected {len(images)},"
                 f" but got {len(predictions)} (in '{self._parent}')"
             )
 
-        for image, prediction in zip(images, predictions):
-            self._check_prediction(image, prediction)
+        for prediction in predictions:
+            self._check_prediction(prediction)
 
-    def _check_prediction(self, image, prediction):
+    def _check_prediction(self, prediction):
         if not isinstance(prediction, dict):
             self._error(
                 f"Each prediction must be a dict,"
                 f" not {type(prediction)} (in '{self._parent})"
             )
         supported_keys = {
             "classes",
```

### Comparing `efemarai-0.3.4/efemarai/session.py` & `efemarai-0.3.5/efemarai/session.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.4/efemarai/stress_test.py` & `efemarai-0.3.5/efemarai/stress_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,32 +154,34 @@
 
         return self._reports
 
     @property
     def model(self):
         """Returns the model associated with the stress test."""
         if self._model is None:
-            self._model = next(m for m in self.project.models if m.id == self._model_id)
+            self._model = next(
+                (m for m in self.project.models if m.id == self._model_id), None
+            )
         return self._model
 
     @property
     def domain(self):
         """Returns the domain associated with the stress test."""
         if self._domain is None:
             self._domain = next(
-                d for d in self.project.domains if d.id == self._domain_id
+                (d for d in self.project.domains if d.id == self._domain_id), None
             )
         return self._domain
 
     @property
     def dataset(self):
         """Returns the dataset associated with the stress test."""
         if self._dataset is None:
             self._dataset = next(
-                d for d in self.project.datasets if d.id == self._dataset_id
+                (d for d in self.project.datasets if d.id == self._dataset_id), None
             )
         return self._dataset
 
     @property
     def finished(self):
         """Returns if the stress test has successfully finished.
```

### Comparing `efemarai-0.3.4/efemarai.egg-info/SOURCES.txt` & `efemarai-0.3.5/efemarai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.4/setup.py` & `efemarai-0.3.5/setup.py`

 * *Files identical despite different names*

