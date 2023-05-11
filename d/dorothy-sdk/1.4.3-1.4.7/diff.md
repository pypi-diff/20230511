# Comparing `tmp/dorothy-sdk-1.4.3.tar.gz` & `tmp/dorothy-sdk-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorothy-sdk-1.4.3.tar", last modified: Wed May  3 01:47:35 2023, max compression
+gzip compressed data, was "dorothy-sdk-1.4.7.tar", last modified: Thu May 11 13:08:17 2023, max compression
```

## Comparing `dorothy-sdk-1.4.3.tar` & `dorothy-sdk-1.4.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6058 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/bin/model_run
--rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/bin/model_train
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/dorothy_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/dorothy_sdk/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/resources/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/resources/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/resources/folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/resources/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/resources/quality_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/dorothy_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-03 01:47:35.000000 dorothy-sdk-1.4.3/dorothy_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-03 01:47:35.000000 dorothy-sdk-1.4.3/dorothy_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 01:47:35.000000 dorothy-sdk-1.4.3/dorothy_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 01:47:35.000000 dorothy-sdk-1.4.3/dorothy_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 01:47:35.000000 dorothy-sdk-1.4.3/dorothy_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:08:17.251549 dorothy-sdk-1.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-11 13:08:17.251549 dorothy-sdk-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:08:17.251549 dorothy-sdk-1.4.7/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6021 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/bin/model_run
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/bin/model_train
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:08:17.247549 dorothy-sdk-1.4.7/dorothy_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:08:17.247549 dorothy-sdk-1.4.7/dorothy_sdk/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/resources/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/resources/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/resources/folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/resources/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/resources/quality_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:08:17.247549 dorothy-sdk-1.4.7/dorothy_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-11 13:08:17.000000 dorothy-sdk-1.4.7/dorothy_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-11 13:08:17.000000 dorothy-sdk-1.4.7/dorothy_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:08:17.000000 dorothy-sdk-1.4.7/dorothy_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-11 13:08:17.000000 dorothy-sdk-1.4.7/dorothy_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 13:08:17.000000 dorothy-sdk-1.4.7/dorothy_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 13:08:17.251549 dorothy-sdk-1.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/setup.py
```

### Comparing `dorothy-sdk-1.4.3/PKG-INFO` & `dorothy-sdk-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorothy-sdk
-Version: 1.4.3
+Version: 1.4.7
 Summary: UNKNOWN
 Home-page: https://github.com/tb-brics/dorothy-sdk
 Author: Patrick Braz
 Author-email: patrickfbraz@poli.ufrj.br
 Maintainer: Patrick Braz
 Maintainer-email: patrickfbraz@poli.ufrj.br
 License: UNKNOWN
```

### Comparing `dorothy-sdk-1.4.3/README.rst` & `dorothy-sdk-1.4.7/README.rst`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.3/bin/model_run` & `dorothy-sdk-1.4.7/bin/model_run`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,15 @@
     log.info('  Carregando dataset do DOROTHY "%s"', dataset)
     return operate.get_dataset_images(dataset)
 
 
 def get_model(run_id, operate):
     if os.path.exists(run_id):
         log.info('  Carregando modelo local em  "%s"', run_id)
-        ret = operate.load_model(run_id)
-        return ret[0].module_, ret[1]
+        return operate.load_model(run_id)
     log.info('  Carregando modelo do MLFlow com run ID "%s"', run_id)
     return operate.get_operation_model(run_id)
 
 
 def main():
   """
   Função principal do script. Ela organiza o workflow necessário para a operação do modelo.
```

### Comparing `dorothy-sdk-1.4.3/bin/model_train` & `dorothy-sdk-1.4.7/bin/model_train`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk/core.py` & `dorothy-sdk-1.4.7/dorothy_sdk/core.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk/dataset_wrapper.py` & `dorothy-sdk-1.4.7/dorothy_sdk/dataset_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     
     def _assemble_dataset(self):
         """Download and create a local version of the dataset"""
         ds = self.client.dataset(self.dataset)
         metadata_list = []
         for img in ds.list_images():
-            img = img.download_image(width=self.image_width, height=self.image_height, gray_scale=self.image_grayscale)
+            img.download_image(width=self.image_width, height=self.image_height, gray_scale=self.image_grayscale)
             image_local_path = os.path.join(self.cache_location, img._cached_image_name) if img._cache_enabled else None
             metadata_list.append({'image_url' : img.image_url, 'metadata' : img.metadata, 'image_local_path' : image_local_path})
 
         #Creating the metadata dataframe and saving it.
         df = self._assemble_metadata(metadata_list)
         df['y_true'] = 1
         df.loc[df.has_tb == False, 'y_true'] = 0
@@ -93,16 +93,16 @@
 
         #Saving metadata
         df.gender.replace(to_replace={'F' : 'female', 'M' : 'male'}, inplace=True)
         return df
 
 
     def _assemble_cv_splits(self):
-        cluster = self.client.cluster(f"cluster_{self.dataset}")
-        file = cluster.download_file()
+        ds = self.client.dataset(self.dataset)
+        file = ds.get_cross_validation_file()
         partition = pickle.loads(file)
 
         cols = ['partition', 'inner_split', 'set_type', 'image']
         df = pd.DataFrame(columns=cols)
 
         for i1, d1 in enumerate(partition):
             for i2, d2 in enumerate(d1):
```

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk/git_repo.py` & `dorothy-sdk-1.4.7/dorothy_sdk/git_repo.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk/mlflow.py` & `dorothy-sdk-1.4.7/dorothy_sdk/mlflow.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk/operation.py` & `dorothy-sdk-1.4.7/dorothy_sdk/operation.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk/resources/dataset.py` & `dorothy-sdk-1.4.7/dorothy_sdk/resources/dataset.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk/resources/folders.py` & `dorothy-sdk-1.4.7/dorothy_sdk/resources/folders.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk/resources/folds.py` & `dorothy-sdk-1.4.7/dorothy_sdk/resources/folds.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+import os
+import pickle
+from csv import DictWriter
 from dataclasses import dataclass, field
 from io import BytesIO
+from os import mkdir
 from os.path import exists, isdir
-from os import mknod, mkdir
-from typing import Dict, Any, Optional, Iterable, List
+from typing import Dict, Any, Iterable, List
 
+import pandas as pd
 from PIL import Image as PILImage
 from requests import Session
 
 from dorothy_sdk.utils import url_join
 
 
 class ImageFoldInstance:
@@ -60,14 +64,15 @@
     dataset: str = None
     cluster_id: str = None
     file_url: str = None
 
     def __init__(self, session: Session, host: str, **kwargs):
         self._session: Session = session
         self._service_host = host
+        self._images_folds_object = None
         if kwargs.get("datasets"):
             self.datasets = kwargs.get("datasets")
             if isinstance(self.datasets, str):
                 self.datasets = [self.datasets]
             if not isinstance(self.datasets, list):
                 raise ValueError("'datasets' must bu a list-like object")
 
@@ -85,35 +90,101 @@
                 response = request.json()
             if response.get("next", None) is None and len(response.get("results", [])) > 0:
                 for data in response.get("results"):
                     results.append(data)
         return results
 
     def _generate_fold_aggregation(self):
-        agg = {f"fold_{x}_{y}": Fold(name=f"fold_{x}_{y}") for x in range(10) for y in range(9)}
-        for dataset in self.datasets:
-            results = self._fetch_api_data(dataset)
-            for element in results:
-                image_instance = ImageFoldInstance(self._session,
-                                                   dataset_name=dataset,
-                                                   image_url=element.get("image_url"),
-                                                   project_id=element.get("image_project_id"),
-                                                   image_path=element.get("image_path"),
-                                                   has_tb=element.get("has_tb")
-                                                   )
-                fold = agg[element.get("fold_name")]
-                role = element.get("role")
-                if role.upper() == "TRAIN":
-                    fold.train.append(image_instance)
-                elif role.upper() == "TEST":
-                    fold.test.append(image_instance)
-                else:
-                    fold.validation.append(image_instance)
-        return agg
+        if not self._images_folds_object:
+            agg = {f"fold_{x}_{y}": Fold(name=f"fold_{x}_{y}") for x in range(10) for y in range(9)}
+            for dataset in self.datasets:
+                results = self._fetch_api_data(dataset)
+                for element in results:
+                    image_instance = ImageFoldInstance(self._session,
+                                                       dataset_name=dataset,
+                                                       image_url=element.get("image_url"),
+                                                       project_id=element.get("image_project_id"),
+                                                       image_path=element.get("image_path"),
+                                                       has_tb=element.get("has_tb")
+                                                       )
+                    fold = agg[element.get("fold_name")]
+                    role = element.get("role")
+                    if role.upper() == "TRAIN":
+                        fold.train.append(image_instance)
+                    elif role.upper() == "TEST":
+                        fold.test.append(image_instance)
+                    else:
+                        fold.validation.append(image_instance)
+            self._images_folds_object = agg
+            return agg
+        else:
+            return self._images_folds_object
 
     def get_folds(self, fold_name: str = None) -> Iterable[Fold]:
         fold_images: Dict[str, Any] = self._generate_fold_aggregation()
         if fold_name:
             yield fold_images[fold_name]
         else:
             for _, value in sorted(fold_images.items()):
                 yield value
+
+    def _get_folds_as_json(self) -> Iterable[Dict[str, Any]]:
+        results = list(self.get_folds())
+        for result in results:
+            row = {
+                "fold_name": result.name,
+                "test": result.name.replace("fold_", "").split("_")[0],
+                "sort": result.name.replace("fold_", "").split("_")[1],
+                "project_id": None,
+                "target": None,
+                "dataset_name": None,
+                "role": None
+            }
+            for image in result.train:
+                row["project_id"] = image.project_id
+                row["target"] = image.has_tb
+                row["role"] = "TRAIN"
+                row["dataset_name"] = image.dataset_name
+                yield row
+            for image in result.test:
+                row["project_id"] = image.project_id
+                row["target"] = image.has_tb
+                row["role"] = "TEST"
+                row["dataset_name"] = image.dataset_name
+                yield row
+            for image in result.validation:
+                row["project_id"] = image.project_id
+                row["target"] = image.has_tb
+                row["role"] = "VAL"
+                row["dataset_name"] = image.dataset_name
+                yield row
+
+    def get_pandas_dataframe(self):
+        return pd.DataFrame(list(self._get_folds_as_json()))
+
+    def download_picke(self, path: str = None) -> str:
+        results = list(self.get_folds())
+        matrix = [[[] for x in range(9)] for i in range(10)]
+        for result in results:
+            test = int(result.name.replace("fold_", "").split("_")[0])
+            sort = int(result.name.replace("fold_", "").split("_")[1])
+            matrix[test][sort] = [
+                [train_image.project_id for train_image in result.train],
+                [test_image.project_id for test_image in result.test],
+                [val_image.project_id for val_image in result.validation]
+            ]
+        if path is None:
+            path = os.path.join(os.getcwd(), "folds.pkl")
+        with open(path, mode="wb") as file:
+            pickle.dump(matrix, file)
+        return path
+
+    def download_csv(self, path: str = None) -> str:
+        if path is None:
+            path = os.path.join(os.getcwd(), "folds.csv")
+        with open(path, mode="w") as file:
+            fieldnames = ["fold_name", "test", "sort", "project_id", "target", "dataset_name", "role"]
+            writer = DictWriter(file, fieldnames=fieldnames)
+            writer.writeheader()
+            for row in self._get_folds_as_json():
+                writer.writerow(row)
+        return path
```

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk/resources/image.py` & `dorothy-sdk-1.4.7/dorothy_sdk/resources/image.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk/resources/quality_annotation.py` & `dorothy-sdk-1.4.7/dorothy_sdk/resources/quality_annotation.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk/session.py` & `dorothy-sdk-1.4.7/dorothy_sdk/session.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk.egg-info/PKG-INFO` & `dorothy-sdk-1.4.7/dorothy_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorothy-sdk
-Version: 1.4.3
+Version: 1.4.7
 Summary: UNKNOWN
 Home-page: https://github.com/tb-brics/dorothy-sdk
 Author: Patrick Braz
 Author-email: patrickfbraz@poli.ufrj.br
 Maintainer: Patrick Braz
 Maintainer-email: patrickfbraz@poli.ufrj.br
 License: UNKNOWN
```

### Comparing `dorothy-sdk-1.4.3/dorothy_sdk.egg-info/SOURCES.txt` & `dorothy-sdk-1.4.7/dorothy_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.3/setup.py` & `dorothy-sdk-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 INSTALL_REQUIRES = {
     "requests-cache==1.0.1",
     "GitPython==3.1.29",
     "py-cpuinfo==9.0.0",
     "nvsmi==0.4.2",
     "psutil==5.9.5",
     "Pillow==9.5.0",
+    "pandas==1.5.3"
 }
 
 setup(
     name=PACKAGE_NAME,
     url="https://github.com/tb-brics/dorothy-sdk",
     description=PACKAGE_DESCRIPTION,
     long_description=long_description,
```

