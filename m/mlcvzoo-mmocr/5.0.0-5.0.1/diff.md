# Comparing `tmp/mlcvzoo_mmocr-5.0.0.tar.gz` & `tmp/mlcvzoo_mmocr-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_mmocr-5.0.0.tar", max compression
+gzip compressed data, was "mlcvzoo_mmocr-5.0.1.tar", max compression
```

## Comparing `mlcvzoo_mmocr-5.0.0.tar` & `mlcvzoo_mmocr-5.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      393 2023-02-22 09:03:18.476272 mlcvzoo_mmocr-5.0.0/README.md
--rw-r--r--   0        0        0      177 2023-02-24 16:41:01.275508 mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/__init__.py
--rw-r--r--   0        0        0     3449 2023-02-24 16:41:01.275508 mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/configuration.py
--rw-r--r--   0        0        0     3228 2023-02-22 09:03:18.476272 mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/mlcvzoo_mmocr_dataset.py
--rw-r--r--   0        0        0     4675 2023-02-24 16:41:01.275508 mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/model.py
--rw-r--r--   0        0        0      154 2023-02-22 09:03:18.476272 mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/py.typed
--rw-r--r--   0        0        0      379 2023-02-22 09:03:18.476272 mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/structs.py
--rw-r--r--   0        0        0     4832 2023-02-24 16:41:01.279508 mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/text_detection_model.py
--rw-r--r--   0        0        0     3951 2023-02-24 16:41:01.279508 mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/text_recognition_model.py
--rw-r--r--   0        0        0    11416 2023-02-22 09:03:18.484272 mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/third_party/LICENSE
--rw-r--r--   0        0        0      103 2023-02-22 09:03:18.484272 mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/third_party/README.md
--rw-r--r--   0        0        0      154 2023-02-22 09:03:18.484272 mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/third_party/__init__.py
--rw-r--r--   0        0        0     1183 2023-02-22 09:03:18.484272 mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/third_party/mmocr.py
--rw-r--r--   0        0        0     4033 2023-02-24 16:41:01.283508 mlcvzoo_mmocr-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     1571 1970-01-01 00:00:00.000000 mlcvzoo_mmocr-5.0.0/setup.py
--rw-r--r--   0        0        0     2103 1970-01-01 00:00:00.000000 mlcvzoo_mmocr-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0      393 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/README.md
+-rw-r--r--   0        0        0      177 2023-05-11 11:10:51.233392 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/__init__.py
+-rw-r--r--   0        0        0     3449 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/configuration.py
+-rw-r--r--   0        0        0     3228 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/mlcvzoo_mmocr_dataset.py
+-rw-r--r--   0        0        0     4719 2023-05-11 08:05:29.657505 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/model.py
+-rw-r--r--   0        0        0      154 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/py.typed
+-rw-r--r--   0        0        0      379 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/structs.py
+-rw-r--r--   0        0        0     4828 2023-05-11 08:05:29.657505 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/text_detection_model.py
+-rw-r--r--   0        0        0     3947 2023-05-11 08:05:29.657505 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/text_recognition_model.py
+-rw-r--r--   0        0        0    11416 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/third_party/LICENSE
+-rw-r--r--   0        0        0      103 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/third_party/README.md
+-rw-r--r--   0        0        0      154 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/third_party/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/third_party/mmocr.py
+-rw-r--r--   0        0        0     3988 2023-05-11 14:03:20.820970 mlcvzoo_mmocr-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 mlcvzoo_mmocr-5.0.1/setup.py
+-rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 mlcvzoo_mmocr-5.0.1/PKG-INFO
```

### Comparing `mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/configuration.py` & `mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/mlcvzoo_mmocr_dataset.py` & `mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/mlcvzoo_mmocr_dataset.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/model.py` & `mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,22 +121,24 @@
             end,
             results,
         )
 
         return results
 
     @staticmethod
-    def _get_framework_imports() -> Tuple[
-        Callable[[Any], Any],
-        Callable[[Any], Any],
-        Callable[[Any], Any],
-        Callable[[Any], Any],
-        Callable[[Any], Any],
-        Callable[[Any], Any],
-    ]:
+    def _get_framework_imports() -> (
+        Tuple[
+            Callable[[Any], Any],
+            Callable[[Any], Any],
+            Callable[[Any], Any],
+            Callable[[Any], Any],
+            Callable[[Any], Any],
+            Callable[[Any], Any],
+        ]
+    ):
         from mmocr.apis import init_detector, init_random_seed, train_detector
         from mmocr.datasets import build_dataset
         from mmocr.models import build_detector
         from mmocr.utils import collect_env
 
         return (
             init_detector,
```

### Comparing `mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/text_detection_model.py` & `mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/text_detection_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 
         # we skip last entry because this is a confidence value
         return list(zip(text_detection_result[:-1:2], text_detection_result[1:-1:2]))
 
     def __process_text_detection_result(
         self, result: Dict[str, Any]
     ) -> List[Segmentation]:
-
         segmentations: List[Segmentation] = list()
 
         for text_detection_result in result["boundary_result"]:
             score: float = text_detection_result[-1]
 
             polygon: PolygonType = (
                 MMOCRTextDetectionModel.__decode_mmocr_result_to_list_of_points(
@@ -108,33 +107,30 @@
                         segmentation.to_rect_polygon()
 
         return segmentations
 
     def predict(
         self, data_item: Union[str, ImageType]
     ) -> Tuple[Union[str, ImageType], List[Segmentation]]:
-
         assert self.net is not None
 
         return data_item, self.__process_text_detection_result(
             result=self._predict(data_item=data_item)
         )
 
     def predict_many(
         self, data_items: List[Union[str, ImageType]]
     ) -> List[Tuple[Union[str, ImageType], List[Segmentation]]]:
-
         assert self.net is not None
 
         prediction_list: List[Tuple[Union[str, ImageType], List[Segmentation]]] = []
 
         results = self._predict(data_item=data_items)
 
         for data_item, result in zip(data_items, results):
-
             segmentations = self.__process_text_detection_result(result=result)
 
             prediction_list.append(
                 (
                     data_item,
                     segmentations,
                 )
```

### Comparing `mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/text_recognition_model.py` & `mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/text_recognition_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,14 @@
             score = result["score"]
 
         return score if score >= score_threshold else None
 
     def predict(
         self, data_item: Union[str, ImageType]
     ) -> Tuple[Union[str, ImageType], List[OCRPerception]]:
-
         assert self.net is not None
 
         ocr_texts: List[OCRPerception] = []
 
         result = self._predict(data_item=data_item)
 
         score = self.__filter_result_score_by_mean(
@@ -94,30 +93,27 @@
             ocr_texts.append(OCRPerception(content=result["text"], score=score))
 
         return data_item, ocr_texts
 
     def predict_many(
         self, data_items: List[Union[str, ImageType]]
     ) -> List[Tuple[Union[str, ImageType], List[OCRPerception]]]:
-
         assert self.net is not None
 
         prediction_list: List[Tuple[Union[str, ImageType], List[OCRPerception]]] = []
 
         results = self._predict(data_item=data_items)
 
         for data_item, result in zip(data_items, results):
-
             score = self.__filter_result_score_by_mean(
                 result=result,
                 score_threshold=self.configuration.inference_config.score_threshold,
             )
 
             if score is not None:
-
                 prediction_list.append(
                     (
                         data_item,
                         [OCRPerception(content=result["text"], score=score)],
                     )
                 )
             else:
```

### Comparing `mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/third_party/LICENSE` & `mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/third_party/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmocr-5.0.0/mlcvzoo_mmocr/third_party/mmocr.py` & `mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/third_party/mmocr.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmocr-5.0.0/pyproject.toml` & `mlcvzoo_mmocr-5.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlcvzoo_mmocr"
-version = "5.0.0"
+version = "5.0.1"
 license = "Open Logistics License Version 1.0"
 description = "MLCVZoo MMOCR Package"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc"
 classifiers = [
@@ -33,39 +33,38 @@
 python = "^3.8"
 
 yaml-config-builder = { version = "^8" }
 related-mltoolbox = { version = "^1" }
 mlcvzoo_base = { version = "^5" }
 mlcvzoo_mmdetection = { version = "^5" }
 
+attrs = { version = ">=20" }
 # 4.6.0.66 leads to errors when building mmcv-full
 opencv-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66" }
 opencv-contrib-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66" }
 mmocr = { version=">=0.3,<=0.6.3" }
 mmdet = { version="^2.11.0" }
 # mmocr 0.6 has <= 1.6.0
 mmcv-full = { version=">=1.3.4,!=1.3.18" }
-pycocotools = { version="^2.0.2" }
+pycocotools = { version=">=2.0.2", markers = "platform_machine == 'x86_64'" }
 # 1.19.2 is oldest available on aarch64 but 1.19.5 leads to unbuildable pytorch there, all is well on amd64
 numpy = { version = ">=1.19.2,!=1.19.5" }
-nptyping = { version = "^2.0" }
-torch = { version = "^1.9" }
-torchvision = { version = "^0.10" }
-# TODO: remove when fixed by tensorboard: https://github.com/tensorflow/tensorboard/issues/5703
-protobuf =  {version="<=3.20"}
+nptyping = { version = ">=2.0" }
+torch = { version = ">=1.9" }
+torchvision = { version = ">=0.10" }
 
 [tool.poetry.dev-dependencies]
-mock = { version = "^4.0" }
-pytest = { version = "^7.0" }
-pytest-cov = { version = "^3.0.0" }
-black = { version = "^22" }
+mock = { version = ">=4.0" }
+pytest = { version = ">=7.0" }
+pytest-cov = { version = ">=3.0.0" }
+black = { version = ">=22" }
 mypy = { version = ">=0.961" }
-pylint = { version = "^2.9.6" }
-isort = { version = "^5.9" }
-pytest-mock = "^3.7"
+pylint = { version = ">=2.9.6" }
+isort = { version = ">=5.9" }
+pytest-mock = ">=3.7"
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
 requires = ["setuptools", "poetry_core>=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `mlcvzoo_mmocr-5.0.0/setup.py` & `mlcvzoo_mmocr-5.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,41 +4,44 @@
 packages = \
 ['mlcvzoo_mmocr', 'mlcvzoo_mmocr.third_party']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['mlcvzoo_base>=5,<6',
+['attrs>=20',
+ 'mlcvzoo_base>=5,<6',
  'mlcvzoo_mmdetection>=5,<6',
  'mmcv-full>=1.3.4,!=1.3.18',
  'mmdet>=2.11.0,<3.0.0',
  'mmocr>=0.3,<=0.6.3',
- 'nptyping>=2.0,<3.0',
+ 'nptyping>=2.0',
  'numpy>=1.19.2,!=1.19.5',
  'opencv-contrib-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66',
  'opencv-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66',
- 'protobuf<=3.20',
- 'pycocotools>=2.0.2,<3.0.0',
  'related-mltoolbox>=1,<2',
- 'torch>=1.9,<2.0',
- 'torchvision>=0.10,<0.11',
+ 'torch>=1.9',
+ 'torchvision>=0.10',
  'yaml-config-builder>=8,<9']
 
+extras_require = \
+{':platform_machine == "x86_64"': ['pycocotools>=2.0.2']}
+
 setup_kwargs = {
     'name': 'mlcvzoo-mmocr',
-    'version': '5.0.0',
+    'version': '5.0.1',
     'description': 'MLCVZoo MMOCR Package',
     'long_description': '# MLCVZoo MMOCR\n\nThe MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)\ncomputer vision algorithms. The package **mlcvzoo_mmocr** is the wrapper module for\nthe [mmocr framework](https://github.com/open-mmlab/mmocr).\n\nFurther information about the MLCVZoo can be found [here](../README.md).\n\n## Install\n`\npip install mlcvzoo-mmocr\n`\n\n## Technology stack\n\n- Python\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mlcvzoo_mmocr-5.0.0/PKG-INFO` & `mlcvzoo_mmocr-5.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-mmocr
-Version: 5.0.0
+Version: 5.0.1
 Summary: MLCVZoo MMOCR Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 License: Open Logistics License Version 1.0
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,28 +12,28 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: attrs (>=20)
 Requires-Dist: mlcvzoo_base (>=5,<6)
 Requires-Dist: mlcvzoo_mmdetection (>=5,<6)
 Requires-Dist: mmcv-full (>=1.3.4,!=1.3.18)
 Requires-Dist: mmdet (>=2.11.0,<3.0.0)
 Requires-Dist: mmocr (>=0.3,<=0.6.3)
-Requires-Dist: nptyping (>=2.0,<3.0)
+Requires-Dist: nptyping (>=2.0)
 Requires-Dist: numpy (>=1.19.2,!=1.19.5)
 Requires-Dist: opencv-contrib-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66)
 Requires-Dist: opencv-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66)
-Requires-Dist: protobuf (<=3.20)
-Requires-Dist: pycocotools (>=2.0.2,<3.0.0)
+Requires-Dist: pycocotools (>=2.0.2) ; platform_machine == "x86_64"
 Requires-Dist: related-mltoolbox (>=1,<2)
-Requires-Dist: torch (>=1.9,<2.0)
-Requires-Dist: torchvision (>=0.10,<0.11)
+Requires-Dist: torch (>=1.9)
+Requires-Dist: torchvision (>=0.10)
 Requires-Dist: yaml-config-builder (>=8,<9)
 Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc
 Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 Description-Content-Type: text/markdown
 
 # MLCVZoo MMOCR
```

