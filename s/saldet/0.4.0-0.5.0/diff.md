# Comparing `tmp/saldet-0.4.0.tar.gz` & `tmp/saldet-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saldet-0.4.0.tar", max compression
+gzip compressed data, was "saldet-0.5.0.tar", max compression
```

## Comparing `saldet-0.4.0.tar` & `saldet-0.5.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.4.0/LICENSE
--rw-r--r--   0        0        0       71 2023-05-09 18:23:52.446725 saldet-0.4.0/README.md
--rw-r--r--   0        0        0      786 2023-05-10 20:49:29.941429 saldet-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       87 2023-05-10 20:49:29.941501 saldet-0.4.0/saldet/__init__.py
--rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.4.0/saldet/dataset/__init__.py
--rw-r--r--   0        0        0     2581 2023-05-10 17:49:03.356850 saldet-0.4.0/saldet/dataset/inference.py
--rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.4.0/saldet/dataset/saliency.py
--rw-r--r--   0        0        0       25 2023-05-10 20:46:44.439113 saldet-0.4.0/saldet/experiment/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 19:22:28.111423 saldet-0.4.0/saldet/experiment/inference.py
--rw-r--r--   0        0        0     2312 2023-05-10 20:46:44.791975 saldet-0.4.0/saldet/experiment/train.py
--rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.4.0/saldet/io/__init__.py
--rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.4.0/saldet/io/config.py
--rw-r--r--   0        0        0     1845 2023-05-10 19:54:12.367968 saldet-0.4.0/saldet/io/image.py
--rw-r--r--   0        0        0       98 2023-05-10 20:45:02.484536 saldet-0.4.0/saldet/loss/__init__.py
--rw-r--r--   0        0        0      310 2023-05-10 20:45:02.489998 saldet-0.4.0/saldet/loss/_factory.py
--rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.4.0/saldet/loss/attn_guided.py
--rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.4.0/saldet/loss/bce_iou_loss.py
--rw-r--r--   0        0        0     1130 2023-05-10 20:15:48.390884 saldet-0.4.0/saldet/loss/multi_bce.py
--rw-r--r--   0        0        0      858 2023-05-10 18:06:50.913204 saldet-0.4.0/saldet/loss/pg.py
--rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.4.0/saldet/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.4.0/saldet/lr_scheduler/lr_scheduler.py
--rw-r--r--   0        0        0       52 2023-05-10 17:15:58.921970 saldet-0.4.0/saldet/model/__init__.py
--rw-r--r--   0        0        0     2282 2023-05-10 19:34:30.563217 saldet-0.4.0/saldet/model/_factory.py
--rw-r--r--   0        0        0       67 2023-05-10 17:15:59.631830 saldet-0.4.0/saldet/model/models/__init__.py
--rw-r--r--   0        0        0    10194 2023-05-10 17:15:59.633279 saldet-0.4.0/saldet/model/models/pgnet.py
--rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.4.0/saldet/model/models/resnet.py
--rw-r--r--   0        0        0    25344 2023-05-10 17:15:59.521603 saldet-0.4.0/saldet/model/models/swin.py
--rw-r--r--   0        0        0     6809 2023-05-10 17:15:59.637029 saldet-0.4.0/saldet/model/models/u2net.py
--rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.4.0/saldet/ops/__init__.py
--rw-r--r--   0        0        0      930 2023-05-10 20:47:50.389781 saldet-0.4.0/saldet/ops/tensor.py
--rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.4.0/saldet/optimizer/__init__.py
--rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.4.0/saldet/optimizer/optimizer.py
--rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.4.0/saldet/pl/__init__.py
--rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.4.0/saldet/pl/data.py
--rw-r--r--   0        0        0     2370 2023-05-10 17:15:59.638743 saldet-0.4.0/saldet/pl/model.py
--rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.4.0/saldet/trainer/__init__.py
--rw-r--r--   0        0        0     1681 2023-05-10 20:46:44.795184 saldet-0.4.0/saldet/trainer/callbacks.py
--rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.4.0/saldet/transform/__init__.py
--rw-r--r--   0        0        0     3420 2023-05-10 18:05:44.622461 saldet-0.4.0/saldet/transform/transform.py
--rw-r--r--   0        0        0       49 2023-05-10 20:48:29.232128 saldet-0.4.0/saldet/utils/__init__.py
--rw-r--r--   0        0        0      225 2023-05-10 17:16:58.601910 saldet-0.4.0/saldet/utils/device.py
--rw-r--r--   0        0        0      330 2023-05-10 20:48:12.118076 saldet-0.4.0/saldet/utils/time.py
--rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 saldet-0.4.0/setup.py
--rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 saldet-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3446 2023-05-11 09:06:14.060537 saldet-0.5.0/README.md
+-rw-r--r--   0        0        0      917 2023-05-11 09:07:28.509787 saldet-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-05-11 09:06:14.060928 saldet-0.5.0/saldet/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.5.0/saldet/dataset/__init__.py
+-rw-r--r--   0        0        0     2564 2023-05-11 09:06:14.061164 saldet-0.5.0/saldet/dataset/inference.py
+-rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.5.0/saldet/dataset/saliency.py
+-rw-r--r--   0        0        0       58 2023-05-11 09:06:14.061366 saldet-0.5.0/saldet/experiment/__init__.py
+-rw-r--r--   0        0        0     2915 2023-05-11 09:06:14.061549 saldet-0.5.0/saldet/experiment/inference.py
+-rw-r--r--   0        0        0     2312 2023-05-10 20:46:44.791975 saldet-0.5.0/saldet/experiment/train.py
+-rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.5.0/saldet/io/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.5.0/saldet/io/config.py
+-rw-r--r--   0        0        0     1873 2023-05-11 09:06:14.061761 saldet-0.5.0/saldet/io/image.py
+-rw-r--r--   0        0        0       98 2023-05-10 20:45:02.484536 saldet-0.5.0/saldet/loss/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-10 20:45:02.489998 saldet-0.5.0/saldet/loss/_factory.py
+-rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.5.0/saldet/loss/attn_guided.py
+-rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.5.0/saldet/loss/bce_iou_loss.py
+-rw-r--r--   0        0        0     1130 2023-05-10 20:15:48.390884 saldet-0.5.0/saldet/loss/multi_bce.py
+-rw-r--r--   0        0        0      858 2023-05-10 18:06:50.913204 saldet-0.5.0/saldet/loss/pg.py
+-rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.5.0/saldet/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.5.0/saldet/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0        0        0       52 2023-05-10 17:15:58.921970 saldet-0.5.0/saldet/model/__init__.py
+-rw-r--r--   0        0        0     2282 2023-05-11 07:54:40.355900 saldet-0.5.0/saldet/model/_factory.py
+-rw-r--r--   0        0        0       67 2023-05-10 17:15:59.631830 saldet-0.5.0/saldet/model/models/__init__.py
+-rw-r--r--   0        0        0    10194 2023-05-10 17:15:59.633279 saldet-0.5.0/saldet/model/models/pgnet.py
+-rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.5.0/saldet/model/models/resnet.py
+-rw-r--r--   0        0        0    25344 2023-05-10 17:15:59.521603 saldet-0.5.0/saldet/model/models/swin.py
+-rw-r--r--   0        0        0     6809 2023-05-10 17:15:59.637029 saldet-0.5.0/saldet/model/models/u2net.py
+-rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.5.0/saldet/ops/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-10 20:47:50.389781 saldet-0.5.0/saldet/ops/tensor.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.5.0/saldet/optimizer/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.5.0/saldet/optimizer/optimizer.py
+-rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.5.0/saldet/pl/__init__.py
+-rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.5.0/saldet/pl/data.py
+-rw-r--r--   0        0        0     2370 2023-05-10 21:13:19.786920 saldet-0.5.0/saldet/pl/model.py
+-rw-r--r--   0        0        0       43 2023-05-11 09:06:14.061938 saldet-0.5.0/saldet/plot/__init__.py
+-rw-r--r--   0        0        0     2525 2023-05-11 09:06:14.062100 saldet-0.5.0/saldet/plot/plot.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.5.0/saldet/trainer/__init__.py
+-rw-r--r--   0        0        0     1681 2023-05-10 20:46:44.795184 saldet-0.5.0/saldet/trainer/callbacks.py
+-rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.5.0/saldet/transform/__init__.py
+-rw-r--r--   0        0        0     3420 2023-05-10 18:05:44.622461 saldet-0.5.0/saldet/transform/transform.py
+-rw-r--r--   0        0        0       49 2023-05-11 07:54:47.520753 saldet-0.5.0/saldet/utils/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-10 17:16:58.601910 saldet-0.5.0/saldet/utils/device.py
+-rw-r--r--   0        0        0      330 2023-05-10 20:48:12.118076 saldet-0.5.0/saldet/utils/time.py
+-rw-r--r--   0        0        0     4726 1970-01-01 00:00:00.000000 saldet-0.5.0/setup.py
+-rw-r--r--   0        0        0     4524 1970-01-01 00:00:00.000000 saldet-0.5.0/PKG-INFO
```

### Comparing `saldet-0.4.0/LICENSE` & `saldet-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/pyproject.toml` & `saldet-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 [tool.poetry]
 name = "saldet"
-version = "0.4.0"
+version = "0.5.0"
 description = "Saliency Detection library (models, loss, utils) with PyTorch"
 authors = ["Riccardo Musmeci"]
+repository = "https://github.com/riccardomusmeci/saldet"
 license = "MIT"
 readme = "README.md"
+keywords = ["computer vision", "saliency detection"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 torch = "^2.0.1"
 tqdm = "^4.65.0"
 pyyaml = "^6.0"
 timm = "^0.6.13"
 albumentations = "^1.3.0"
 pytorch-lightning = "^2.0.0"
 torchvision = "^0.15.2"
 lightning-bolts = "^0.5.0"
-scriv = "^1.3.1"
-urllib3 = "^1.26.15"
+matplotlib= "^3.7.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 tox = "^4.5.1"
+scriv = "^1.3.1"
+urllib3 = "^1.26.15"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
 scriv = {extras = ["toml"], version = "^1.3.1"}
 
 [tool.scriv]
 format = "md"
```

### Comparing `saldet-0.4.0/saldet/dataset/inference.py` & `saldet-0.5.0/saldet/dataset/inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,27 +75,27 @@
         ]
         if len(images) == 0:
             raise FileExistsError(f"Folder {root_dir} does not have images.")
 
         print(f"> Inference dataset sanity check OK")
 
     def __getitem__(self, index) -> Tuple[torch.Tensor, str]:
-        """Return a tuple (image, filename)
+        """Return a tuple (image, image path)
 
         Args:
             index (int): index of dataset
 
         Returns:
-            Tuple[torch.Tensor, str]: image, filename
+            Tuple[torch.Tensor, str]: image, image path
         """
 
         image_path = self.images[index]
         image_name = image_path.split(os.sep)[-1]
         image = read_rgb(image_path)
 
         if self.transform is not None:
             image, _ = self.transform(image, None)
 
-        return image, os.path.splitext(image_name)[0]
+        return image, image_path
 
     def __len__(self):
         return len(self.images)
```

### Comparing `saldet-0.4.0/saldet/dataset/saliency.py` & `saldet-0.5.0/saldet/dataset/saliency.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/experiment/train.py` & `saldet-0.5.0/saldet/experiment/train.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/io/image.py` & `saldet-0.5.0/saldet/io/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,27 +43,27 @@
     img = cv2.imread(str(file_path), cv2.IMREAD_GRAYSCALE)
     if img is None:
         raise ValueError(f"Unable to read {file_path}.")
 
     img = img.astype("float64")
     if img.max() == 255:
         img /= 255
-
     return img
 
 
 def save_image(image: np.array, output_path: str):
     """Save an image at given path making sure the folder exists
 
     Args:
         image (np.array): image to save
         output_path (str): output path
     """
     output_dir = output_path.replace(os.path.basename(output_path), "")
-    os.makedirs(output_dir, exist_ok=True)
+    if output_dir != "":
+        os.makedirs(output_dir, exist_ok=True)
 
     if len(image.shape) > 2:
         image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
     try:
         cv2.imwrite(output_path, image)
     except Exception as excp:
         print(
```

### Comparing `saldet-0.4.0/saldet/loss/attn_guided.py` & `saldet-0.5.0/saldet/loss/attn_guided.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/loss/bce_iou_loss.py` & `saldet-0.5.0/saldet/loss/bce_iou_loss.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/loss/multi_bce.py` & `saldet-0.5.0/saldet/loss/multi_bce.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/loss/pg.py` & `saldet-0.5.0/saldet/loss/pg.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/lr_scheduler/lr_scheduler.py` & `saldet-0.5.0/saldet/lr_scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/model/_factory.py` & `saldet-0.5.0/saldet/model/_factory.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/model/models/pgnet.py` & `saldet-0.5.0/saldet/model/models/pgnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/model/models/resnet.py` & `saldet-0.5.0/saldet/model/models/resnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/model/models/swin.py` & `saldet-0.5.0/saldet/model/models/swin.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/model/models/u2net.py` & `saldet-0.5.0/saldet/model/models/u2net.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/ops/tensor.py` & `saldet-0.5.0/saldet/ops/tensor.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/optimizer/optimizer.py` & `saldet-0.5.0/saldet/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/pl/data.py` & `saldet-0.5.0/saldet/pl/data.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/pl/model.py` & `saldet-0.5.0/saldet/pl/model.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/trainer/callbacks.py` & `saldet-0.5.0/saldet/trainer/callbacks.py`

 * *Files identical despite different names*

### Comparing `saldet-0.4.0/saldet/transform/transform.py` & `saldet-0.5.0/saldet/transform/transform.py`

 * *Files identical despite different names*

