# Comparing `tmp/batdetect2-1.0.4.tar.gz` & `tmp/batdetect2-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batdetect2-1.0.4.tar", last modified: Mon May  1 17:07:09 2023, max compression
+gzip compressed data, was "batdetect2-1.0.5.tar", last modified: Thu May 11 13:13:14 2023, max compression
```

## Comparing `batdetect2-1.0.4.tar` & `batdetect2-1.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    17694 2023-05-01 17:06:53.465622 batdetect2-1.0.4/LICENSE.md
--rw-r--r--   0        0        0     5584 2023-05-01 17:06:53.465622 batdetect2-1.0.4/README.md
--rw-r--r--   0        0        0       22 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/__init__.py
--rw-r--r--   0        0        0    12537 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/api.py
--rw-r--r--   0        0        0     4117 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/cli.py
--rw-r--r--   0        0        0        0 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/detector/__init__.py
--rw-r--r--   0        0        0     4225 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/detector/compute_features.py
--rw-r--r--   0        0        0     4970 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/detector/model_helpers.py
--rw-r--r--   0        0        0    10568 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/detector/models.py
--rw-r--r--   0        0        0     7481 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/detector/parameters.py
--rw-r--r--   0        0        0     5873 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/detector/post_process.py
--rw-r--r--   0        0        0        0 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/evaluate/__init__.py
--rw-r--r--   0        0        0    25540 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/evaluate/evaluate_models.py
--rw-r--r--   0        0        0     2244 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/evaluate/readme.md
--rw-r--r--   0        0        0        0 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/finetune/__init__.py
--rw-r--r--   0        0        0     9902 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/finetune/finetune_model.py
--rw-r--r--   0        0        0     6324 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/finetune/prep_data_finetune.py
--rw-r--r--   0        0        0     3158 2023-05-01 17:06:53.465622 batdetect2-1.0.4/batdetect2/finetune/readme.md
--rw-r--r--   0        0        0  7600690 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/models/Net2DFast_UK_same.pth.tar
--rw-r--r--   0        0        0       25 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/models/readme.md
--rw-r--r--   0        0        0     9832 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/plot.py
--rw-r--r--   0        0        0        0 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/train/__init__.py
--rw-r--r--   0        0        0    20543 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/train/audio_dataloader.py
--rwxr-xr-x   0        0        0    13217 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/train/evaluate.py
--rw-r--r--   0        0        0     1580 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/train/losses.py
--rw-r--r--   0        0        0     1186 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/train/readme.md
--rw-r--r--   0        0        0    17515 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/train/train_model.py
--rw-r--r--   0        0        0    12533 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/train/train_split.py
--rw-r--r--   0        0        0     5961 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/train/train_utils.py
--rw-r--r--   0        0        0    11150 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/types.py
--rw-r--r--   0        0        0        0 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/utils/__init__.py
--rw-r--r--   0        0        0     8455 2023-05-01 17:06:53.521624 batdetect2-1.0.4/batdetect2/utils/audio_utils.py
--rw-r--r--   0        0        0    23243 2023-05-01 17:06:53.525624 batdetect2-1.0.4/batdetect2/utils/detector_utils.py
--rw-r--r--   0        0        0    16322 2023-05-01 17:06:53.525624 batdetect2-1.0.4/batdetect2/utils/plot_utils.py
--rw-r--r--   0        0        0     7940 2023-05-01 17:06:53.525624 batdetect2-1.0.4/batdetect2/utils/visualize.py
--rw-r--r--   0        0        0     8059 2023-05-01 17:06:53.525624 batdetect2-1.0.4/batdetect2/utils/wavfile.py
--rw-r--r--   0        0        0     1749 2023-05-01 17:06:53.541625 batdetect2-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 17:06:53.541625 batdetect2-1.0.4/tests/__init__.py
--rw-r--r--   0        0        0     8805 2023-05-01 17:06:53.541625 batdetect2-1.0.4/tests/test_api.py
--rw-r--r--   0        0        0     1853 2023-05-01 17:06:53.541625 batdetect2-1.0.4/tests/test_cli.py
--rw-r--r--   0        0        0     6537 1970-01-01 00:00:00.000000 batdetect2-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    17694 2023-05-11 13:13:04.611105 batdetect2-1.0.5/LICENSE.md
+-rw-r--r--   0        0        0     5584 2023-05-11 13:13:04.611105 batdetect2-1.0.5/README.md
+-rw-r--r--   0        0        0       22 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/__init__.py
+-rw-r--r--   0        0        0    12537 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/api.py
+-rw-r--r--   0        0        0     4117 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/cli.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/detector/__init__.py
+-rw-r--r--   0        0        0     4225 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/detector/compute_features.py
+-rw-r--r--   0        0        0     4970 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/detector/model_helpers.py
+-rw-r--r--   0        0        0    10568 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/detector/models.py
+-rw-r--r--   0        0        0     7481 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/detector/parameters.py
+-rw-r--r--   0        0        0     5873 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/detector/post_process.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/evaluate/__init__.py
+-rw-r--r--   0        0        0    25540 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/evaluate/evaluate_models.py
+-rw-r--r--   0        0        0     2244 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/evaluate/readme.md
+-rw-r--r--   0        0        0        0 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/finetune/__init__.py
+-rw-r--r--   0        0        0     9902 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/finetune/finetune_model.py
+-rw-r--r--   0        0        0     6324 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/finetune/prep_data_finetune.py
+-rw-r--r--   0        0        0     3158 2023-05-11 13:13:04.611105 batdetect2-1.0.5/batdetect2/finetune/readme.md
+-rw-r--r--   0        0        0  7600690 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/models/Net2DFast_UK_same.pth.tar
+-rw-r--r--   0        0        0       25 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/models/readme.md
+-rw-r--r--   0        0        0     9832 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/plot.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/__init__.py
+-rw-r--r--   0        0        0    20543 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/audio_dataloader.py
+-rwxr-xr-x   0        0        0    13217 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/evaluate.py
+-rw-r--r--   0        0        0     1580 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/losses.py
+-rw-r--r--   0        0        0     1186 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/readme.md
+-rw-r--r--   0        0        0    17515 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/train_model.py
+-rw-r--r--   0        0        0    12533 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/train_split.py
+-rw-r--r--   0        0        0     5961 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/train/train_utils.py
+-rw-r--r--   0        0        0    11150 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/types.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/utils/__init__.py
+-rw-r--r--   0        0        0     8455 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/utils/audio_utils.py
+-rw-r--r--   0        0        0    23712 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/utils/detector_utils.py
+-rw-r--r--   0        0        0    16322 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/utils/plot_utils.py
+-rw-r--r--   0        0        0     7940 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/utils/visualize.py
+-rw-r--r--   0        0        0     8059 2023-05-11 13:13:04.659105 batdetect2-1.0.5/batdetect2/utils/wavfile.py
+-rw-r--r--   0        0        0     1749 2023-05-11 13:13:04.675105 batdetect2-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 13:13:04.675105 batdetect2-1.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     9321 2023-05-11 13:13:04.675105 batdetect2-1.0.5/tests/test_api.py
+-rw-r--r--   0        0        0     1853 2023-05-11 13:13:04.675105 batdetect2-1.0.5/tests/test_cli.py
+-rw-r--r--   0        0        0     6537 1970-01-01 00:00:00.000000 batdetect2-1.0.5/PKG-INFO
```

### Comparing `batdetect2-1.0.4/LICENSE.md` & `batdetect2-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/README.md` & `batdetect2-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/api.py` & `batdetect2-1.0.5/batdetect2/api.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/cli.py` & `batdetect2-1.0.5/batdetect2/cli.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/detector/compute_features.py` & `batdetect2-1.0.5/batdetect2/detector/compute_features.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/detector/model_helpers.py` & `batdetect2-1.0.5/batdetect2/detector/model_helpers.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/detector/models.py` & `batdetect2-1.0.5/batdetect2/detector/models.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/detector/parameters.py` & `batdetect2-1.0.5/batdetect2/detector/parameters.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/detector/post_process.py` & `batdetect2-1.0.5/batdetect2/detector/post_process.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/evaluate/evaluate_models.py` & `batdetect2-1.0.5/batdetect2/evaluate/evaluate_models.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/evaluate/readme.md` & `batdetect2-1.0.5/batdetect2/evaluate/readme.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/finetune/finetune_model.py` & `batdetect2-1.0.5/batdetect2/finetune/finetune_model.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/finetune/prep_data_finetune.py` & `batdetect2-1.0.5/batdetect2/finetune/prep_data_finetune.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/finetune/readme.md` & `batdetect2-1.0.5/batdetect2/finetune/readme.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/models/Net2DFast_UK_same.pth.tar` & `batdetect2-1.0.5/batdetect2/models/Net2DFast_UK_same.pth.tar`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/plot.py` & `batdetect2-1.0.5/batdetect2/plot.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/train/audio_dataloader.py` & `batdetect2-1.0.5/batdetect2/train/audio_dataloader.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/train/evaluate.py` & `batdetect2-1.0.5/batdetect2/train/evaluate.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/train/losses.py` & `batdetect2-1.0.5/batdetect2/train/losses.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/train/readme.md` & `batdetect2-1.0.5/batdetect2/train/readme.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/train/train_model.py` & `batdetect2-1.0.5/batdetect2/train/train_model.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/train/train_split.py` & `batdetect2-1.0.5/batdetect2/train/train_split.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/train/train_utils.py` & `batdetect2-1.0.5/batdetect2/train/train_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/types.py` & `batdetect2-1.0.5/batdetect2/types.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/utils/audio_utils.py` & `batdetect2-1.0.5/batdetect2/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/utils/detector_utils.py` & `batdetect2-1.0.5/batdetect2/utils/detector_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,26 +139,34 @@
     model = model.to(device)
     model.eval()
 
     return model, params
 
 
 def _merge_results(predictions, spec_feats, cnn_feats, spec_slices):
-    predictions_m = {}
+    predictions_m = {
+        "det_probs": np.array([]),
+        "x_pos": np.array([]),
+        "y_pos": np.array([]),
+        "bb_widths": np.array([]),
+        "bb_heights": np.array([]),
+        "start_times": np.array([]),
+        "end_times": np.array([]),
+        "low_freqs": np.array([]),
+        "high_freqs": np.array([]),
+        "class_probs": np.array([]),
+    }
+
     num_preds = np.sum([len(pp["det_probs"]) for pp in predictions])
 
     if num_preds > 0:
         for key in predictions[0].keys():
             predictions_m[key] = np.hstack(
                 [pp[key] for pp in predictions if pp["det_probs"].shape[0] > 0]
             )
-    else:
-        # hack in case where no detected calls as we need some of the key
-        # names in dict
-        predictions_m = predictions[0]
 
     if len(spec_feats) > 0:
         spec_feats = np.vstack(spec_feats)
 
     if len(cnn_feats) > 0:
         cnn_feats = np.vstack(cnn_feats)
 
@@ -222,29 +230,37 @@
         time_exp (float): Time expansion factor.
         duration (float): Duration of audio file.
         predictions (dict): Predictions.
 
     Returns:
         dict: Results in the format expected by the annotation tool.
     """
-    # Get a single class prediction for the file
-    class_overall = pp.overall_class_pred(
-        predictions["det_probs"],
-        predictions["class_probs"],
-    )
+    try:
+        # Get a single class prediction for the file
+        class_overall = pp.overall_class_pred(
+            predictions["det_probs"],
+            predictions["class_probs"],
+        )
+        class_name = class_names[np.argmax(class_overall)]
+        annotations = get_annotations_from_preds(predictions, class_names)
+    except (np.AxisError, ValueError):
+        # No detections
+        class_overall = np.zeros(len(class_names))
+        class_name = "None"
+        annotations = []
 
     return {
         "id": file_id,
         "annotated": False,
         "issues": False,
         "notes": "Automatically generated.",
         "time_exp": time_exp,
         "duration": round(float(duration), 4),
-        "annotation": get_annotations_from_preds(predictions, class_names),
-        "class_name": class_names[np.argmax(class_overall)],
+        "annotation": annotations,
+        "class_name": class_name,
     }
 
 
 def convert_results(
     file_id: str,
     time_exp: float,
     duration: float,
```

### Comparing `batdetect2-1.0.4/batdetect2/utils/plot_utils.py` & `batdetect2-1.0.5/batdetect2/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/utils/visualize.py` & `batdetect2-1.0.5/batdetect2/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/batdetect2/utils/wavfile.py` & `batdetect2-1.0.5/batdetect2/utils/wavfile.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/pyproject.toml` & `batdetect2-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "tests",
 ]
 venvPath = "."
 venv = ".venv"
 
 [project]
 name = "batdetect2"
-version = "1.0.4"
+version = "1.0.5"
 description = "Deep learning model for detecting and classifying bat echolocation calls in high frequency audio recordings."
 authors = [
     { name = "Oisin Mac Aodha", email = "oisin.macaodha@ed.ac.uk" },
     { name = "Santiago Martinez Balvanera", email = "santiago.balvanera.20@ucl.ac.uk" },
 ]
 dependencies = [
     "librosa",
```

### Comparing `batdetect2-1.0.4/tests/test_api.py` & `batdetect2-1.0.5/tests/test_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Test bat detect module API."""
 
+from pathlib import Path
+
 import os
 from glob import glob
 
 import numpy as np
 import torch
 from torch import nn
+import soundfile as sf
 
 from batdetect2 import api
 
 PKG_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 TEST_DATA_DIR = os.path.join(PKG_DIR, "example_data", "audio")
 TEST_DATA = glob(os.path.join(TEST_DATA_DIR, "*.wav"))
 
@@ -258,7 +261,24 @@
     config = api.get_config(spec_slices=True)
     results = api.process_file(TEST_DATA[0], config=config)
     detections = results["pred_dict"]["annotation"]
 
     assert "spec_slices" in results
     assert isinstance(results["spec_slices"], list)
     assert len(results["spec_slices"]) == len(detections)
+
+
+
+def test_process_file_with_empty_predictions_does_not_fail(
+    tmp_path: Path,
+):
+    """Test process file with empty predictions does not fail."""
+    # Create empty file
+    empty_file = tmp_path / "empty.wav"
+    empty_wav = np.zeros((0, 1), dtype=np.float32)
+    sf.write(empty_file, empty_wav, 256000)
+
+    # Process file
+    results = api.process_file(str(empty_file))
+
+    assert results is not None
+    assert len(results["pred_dict"]["annotation"]) == 0
```

### Comparing `batdetect2-1.0.4/tests/test_cli.py` & `batdetect2-1.0.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.4/PKG-INFO` & `batdetect2-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batdetect2
-Version: 1.0.4
+Version: 1.0.5
 Summary: Deep learning model for detecting and classifying bat echolocation calls in high frequency audio recordings.
 License: CC-by-nc-4
 Keywords: bat,echolocation,deep learning,audio,machine learning,classification,detection
 Author-email: Oisin Mac Aodha <oisin.macaodha@ed.ac.uk>,Santiago Martinez Balvanera <santiago.balvanera.20@ucl.ac.uk>
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

