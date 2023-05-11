# Comparing `tmp/saldet-0.2.0.tar.gz` & `tmp/saldet-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saldet-0.2.0.tar", max compression
+gzip compressed data, was "saldet-0.4.0.tar", max compression
```

## Comparing `saldet-0.2.0.tar` & `saldet-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,44 @@
--rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.2.0/LICENSE
--rw-r--r--   0        0        0       71 2023-05-09 18:23:52.446725 saldet-0.2.0/README.md
--rw-r--r--   0        0        0      786 2023-05-10 17:23:56.060261 saldet-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       87 2023-05-10 17:18:00.823705 saldet-0.2.0/saldet/__init__.py
--rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.2.0/saldet/dataset/__init__.py
--rw-r--r--   0        0        0     2581 2023-05-10 17:14:45.339989 saldet-0.2.0/saldet/dataset/inference.py
--rw-r--r--   0        0        0     3796 2023-05-10 17:14:45.340877 saldet-0.2.0/saldet/dataset/saliency.py
--rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.2.0/saldet/io/__init__.py
--rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.2.0/saldet/io/config.py
--rw-r--r--   0        0        0     1768 2023-05-10 07:56:47.527866 saldet-0.2.0/saldet/io/image.py
--rw-r--r--   0        0        0       52 2023-05-10 17:15:58.921970 saldet-0.2.0/saldet/model/__init__.py
--rw-r--r--   0        0        0     2282 2023-05-10 17:15:59.631385 saldet-0.2.0/saldet/model/_factory.py
--rw-r--r--   0        0        0       67 2023-05-10 17:15:59.631830 saldet-0.2.0/saldet/model/models/__init__.py
--rw-r--r--   0        0        0    10194 2023-05-10 17:15:59.633279 saldet-0.2.0/saldet/model/models/pgnet.py
--rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.2.0/saldet/model/models/resnet.py
--rw-r--r--   0        0        0    25344 2023-05-10 17:15:59.521603 saldet-0.2.0/saldet/model/models/swin.py
--rw-r--r--   0        0        0     6809 2023-05-10 17:15:59.637029 saldet-0.2.0/saldet/model/models/u2net.py
--rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.2.0/saldet/ops/__init__.py
--rw-r--r--   0        0        0      849 2023-05-10 17:17:21.447837 saldet-0.2.0/saldet/ops/tensor.py
--rw-r--r--   0        0        0       35 2023-05-10 07:15:26.158434 saldet-0.2.0/saldet/pl/__init__.py
--rw-r--r--   0        0        0     2370 2023-05-10 17:15:59.638743 saldet-0.2.0/saldet/pl/model.py
--rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.2.0/saldet/transform/__init__.py
--rw-r--r--   0        0        0     3419 2023-05-10 17:15:13.926083 saldet-0.2.0/saldet/transform/transform.py
--rw-r--r--   0        0        0       27 2023-05-10 07:12:42.566274 saldet-0.2.0/saldet/utils/__init__.py
--rw-r--r--   0        0        0      225 2023-05-10 17:16:58.601910 saldet-0.2.0/saldet/utils/device.py
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 saldet-0.2.0/setup.py
--rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 saldet-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 17:45:56.566413 saldet-0.4.0/LICENSE
+-rw-r--r--   0        0        0       71 2023-05-09 18:23:52.446725 saldet-0.4.0/README.md
+-rw-r--r--   0        0        0      786 2023-05-10 20:49:29.941429 saldet-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-05-10 20:49:29.941501 saldet-0.4.0/saldet/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-10 17:14:45.334936 saldet-0.4.0/saldet/dataset/__init__.py
+-rw-r--r--   0        0        0     2581 2023-05-10 17:49:03.356850 saldet-0.4.0/saldet/dataset/inference.py
+-rw-r--r--   0        0        0     3797 2023-05-10 18:05:44.626516 saldet-0.4.0/saldet/dataset/saliency.py
+-rw-r--r--   0        0        0       25 2023-05-10 20:46:44.439113 saldet-0.4.0/saldet/experiment/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 19:22:28.111423 saldet-0.4.0/saldet/experiment/inference.py
+-rw-r--r--   0        0        0     2312 2023-05-10 20:46:44.791975 saldet-0.4.0/saldet/experiment/train.py
+-rw-r--r--   0        0        0       83 2023-05-10 17:11:55.596841 saldet-0.4.0/saldet/io/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-10 17:11:55.596887 saldet-0.4.0/saldet/io/config.py
+-rw-r--r--   0        0        0     1845 2023-05-10 19:54:12.367968 saldet-0.4.0/saldet/io/image.py
+-rw-r--r--   0        0        0       98 2023-05-10 20:45:02.484536 saldet-0.4.0/saldet/loss/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-10 20:45:02.489998 saldet-0.4.0/saldet/loss/_factory.py
+-rw-r--r--   0        0        0      719 2023-05-10 18:06:50.911291 saldet-0.4.0/saldet/loss/attn_guided.py
+-rw-r--r--   0        0        0      623 2023-05-10 20:38:17.791672 saldet-0.4.0/saldet/loss/bce_iou_loss.py
+-rw-r--r--   0        0        0     1130 2023-05-10 20:15:48.390884 saldet-0.4.0/saldet/loss/multi_bce.py
+-rw-r--r--   0        0        0      858 2023-05-10 18:06:50.913204 saldet-0.4.0/saldet/loss/pg.py
+-rw-r--r--   0        0        0       43 2023-05-10 20:46:44.439357 saldet-0.4.0/saldet/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-10 20:46:44.793210 saldet-0.4.0/saldet/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0        0        0       52 2023-05-10 17:15:58.921970 saldet-0.4.0/saldet/model/__init__.py
+-rw-r--r--   0        0        0     2282 2023-05-10 19:34:30.563217 saldet-0.4.0/saldet/model/_factory.py
+-rw-r--r--   0        0        0       67 2023-05-10 17:15:59.631830 saldet-0.4.0/saldet/model/models/__init__.py
+-rw-r--r--   0        0        0    10194 2023-05-10 17:15:59.633279 saldet-0.4.0/saldet/model/models/pgnet.py
+-rw-r--r--   0        0        0      670 2023-05-10 17:15:59.150356 saldet-0.4.0/saldet/model/models/resnet.py
+-rw-r--r--   0        0        0    25344 2023-05-10 17:15:59.521603 saldet-0.4.0/saldet/model/models/swin.py
+-rw-r--r--   0        0        0     6809 2023-05-10 17:15:59.637029 saldet-0.4.0/saldet/model/models/u2net.py
+-rw-r--r--   0        0        0       36 2023-05-10 17:17:21.240440 saldet-0.4.0/saldet/ops/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-10 20:47:50.389781 saldet-0.4.0/saldet/ops/tensor.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.439156 saldet-0.4.0/saldet/optimizer/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-10 20:46:44.794092 saldet-0.4.0/saldet/optimizer/optimizer.py
+-rw-r--r--   0        0        0       74 2023-05-10 20:45:43.432425 saldet-0.4.0/saldet/pl/__init__.py
+-rw-r--r--   0        0        0     3683 2023-05-10 20:45:43.437429 saldet-0.4.0/saldet/pl/data.py
+-rw-r--r--   0        0        0     2370 2023-05-10 17:15:59.638743 saldet-0.4.0/saldet/pl/model.py
+-rw-r--r--   0        0        0       40 2023-05-10 20:46:44.437376 saldet-0.4.0/saldet/trainer/__init__.py
+-rw-r--r--   0        0        0     1681 2023-05-10 20:46:44.795184 saldet-0.4.0/saldet/trainer/callbacks.py
+-rw-r--r--   0        0        0       41 2023-05-10 08:04:37.110954 saldet-0.4.0/saldet/transform/__init__.py
+-rw-r--r--   0        0        0     3420 2023-05-10 18:05:44.622461 saldet-0.4.0/saldet/transform/transform.py
+-rw-r--r--   0        0        0       49 2023-05-10 20:48:29.232128 saldet-0.4.0/saldet/utils/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-10 17:16:58.601910 saldet-0.4.0/saldet/utils/device.py
+-rw-r--r--   0        0        0      330 2023-05-10 20:48:12.118076 saldet-0.4.0/saldet/utils/time.py
+-rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 saldet-0.4.0/setup.py
+-rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 saldet-0.4.0/PKG-INFO
```

### Comparing `saldet-0.2.0/LICENSE` & `saldet-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saldet-0.2.0/pyproject.toml` & `saldet-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saldet"
-version = "0.2.0"
+version = "0.4.0"
 description = "Saliency Detection library (models, loss, utils) with PyTorch"
 authors = ["Riccardo Musmeci"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `saldet-0.2.0/saldet/dataset/inference.py` & `saldet-0.4.0/saldet/dataset/inference.py`

 * *Files identical despite different names*

### Comparing `saldet-0.2.0/saldet/dataset/saliency.py` & `saldet-0.4.0/saldet/dataset/saliency.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
             image = read_rgb(self.images[index])
         except Exception as e:
             print(f"Found error while loading image: {self.images[index]}")
             print(f"Exception {e}")
             sys.exit(0)
         try:
             mask = read_mask(self.masks[index])
+
         except Exception as e:
             print(f"Found error while loading mask: {self.masks[index]}")
             print(f"Exception {e}")
             sys.exit(0)
 
         if self.transform:
             image, mask = self.transform(image=image, mask=mask)
```

### Comparing `saldet-0.2.0/saldet/io/image.py` & `saldet-0.4.0/saldet/io/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,18 @@
     """
     if not os.path.exists(file_path):
         raise FileNotFoundError(f"The path {file_path} does not exist")
     img = cv2.imread(str(file_path), cv2.IMREAD_GRAYSCALE)
     if img is None:
         raise ValueError(f"Unable to read {file_path}.")
 
+    img = img.astype("float64")
+    if img.max() == 255:
+        img /= 255
+
     return img
 
 
 def save_image(image: np.array, output_path: str):
     """Save an image at given path making sure the folder exists
 
     Args:
```

### Comparing `saldet-0.2.0/saldet/model/_factory.py` & `saldet-0.4.0/saldet/model/_factory.py`

 * *Files identical despite different names*

### Comparing `saldet-0.2.0/saldet/model/models/pgnet.py` & `saldet-0.4.0/saldet/model/models/pgnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.2.0/saldet/model/models/resnet.py` & `saldet-0.4.0/saldet/model/models/resnet.py`

 * *Files identical despite different names*

### Comparing `saldet-0.2.0/saldet/model/models/swin.py` & `saldet-0.4.0/saldet/model/models/swin.py`

 * *Files identical despite different names*

### Comparing `saldet-0.2.0/saldet/model/models/u2net.py` & `saldet-0.4.0/saldet/model/models/u2net.py`

 * *Files identical despite different names*

### Comparing `saldet-0.2.0/saldet/ops/tensor.py` & `saldet-0.4.0/saldet/ops/tensor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import torch
 import torch.nn.functional as F
 
+from saldet.utils import device
+
 
 def flat(mask: torch.Tensor) -> torch.tensor:
     """Flat a mask
 
     Args:
         mask (torch.Tensor): input mask
 
@@ -12,14 +14,16 @@
         torch.tensor: flattened mask
     """
     batch_size = mask.shape[0]
     h = 28
     mask = F.interpolate(mask, size=(int(h), int(h)), mode="bilinear")
     x = mask.view(batch_size, 1, -1).permute(0, 2, 1)
     # print(x.shape)  b 28*28 1
+    if device() == "mps":
+        x = x.float()
     g = x @ x.transpose(-2, -1)  # b 28*28 28*28
     g = g.unsqueeze(1)  # b 1 28*28 28*28
     return g
 
 
 def normalize(x: torch.Tensor) -> torch.Tensor:
     """Normalize a tensor based on max and min of tensor
```

### Comparing `saldet-0.2.0/saldet/pl/model.py` & `saldet-0.4.0/saldet/pl/model.py`

 * *Files identical despite different names*

### Comparing `saldet-0.2.0/saldet/transform/transform.py` & `saldet-0.4.0/saldet/transform/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 
         if isinstance(mask, Image.Image):
             image = np.array(image)
 
         if mask is not None:
             sample = self.transform(image=image, mask=mask)
             image, mask = sample["image"], sample["mask"]
+
         else:
             image = self.transform(image=image)["image"]
             mask = None
 
         image = torch.from_numpy(image.transpose(2, 0, 1))
         if mask is not None:
             mask = torch.from_numpy(mask).long()
```

### Comparing `saldet-0.2.0/setup.py` & `saldet-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['saldet',
  'saldet.dataset',
+ 'saldet.experiment',
  'saldet.io',
+ 'saldet.loss',
+ 'saldet.lr_scheduler',
  'saldet.model',
  'saldet.model.models',
  'saldet.ops',
+ 'saldet.optimizer',
  'saldet.pl',
+ 'saldet.trainer',
  'saldet.transform',
  'saldet.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
@@ -25,15 +30,15 @@
  'torch>=2.0.1,<3.0.0',
  'torchvision>=0.15.2,<0.16.0',
  'tqdm>=4.65.0,<5.0.0',
  'urllib3>=1.26.15,<2.0.0']
 
 setup_kwargs = {
     'name': 'saldet',
-    'version': '0.2.0',
+    'version': '0.4.0',
     'description': 'Saliency Detection library (models, loss, utils) with PyTorch',
     'long_description': '# saldet\nSaliency Detection library (models, loss, utils) with PyTorch\n',
     'author': 'Riccardo Musmeci',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `saldet-0.2.0/PKG-INFO` & `saldet-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saldet
-Version: 0.2.0
+Version: 0.4.0
 Summary: Saliency Detection library (models, loss, utils) with PyTorch
 License: MIT
 Author: Riccardo Musmeci
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

