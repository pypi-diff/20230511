# Comparing `tmp/bimcvcovid19i-0.0.6.tar.gz` & `tmp/bimcvcovid19i-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimcvcovid19i-0.0.6.tar", last modified: Wed May 10 21:10:21 2023, max compression
+gzip compressed data, was "bimcvcovid19i-0.0.7.tar", last modified: Wed May 10 22:27:43 2023, max compression
```

## Comparing `bimcvcovid19i-0.0.6.tar` & `bimcvcovid19i-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,35 @@
-drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 21:10:21.748313 bimcvcovid19i-0.0.6/
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1088 2022-10-18 07:33:34.000000 bimcvcovid19i-0.0.6/LICENSE
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      169 2022-10-18 07:33:57.000000 bimcvcovid19i-0.0.6/MANIFEST.in
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1108 2023-05-10 21:10:21.748313 bimcvcovid19i-0.0.6/PKG-INFO
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      576 2022-10-27 06:18:30.000000 bimcvcovid19i-0.0.6/README.md
-drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 21:10:21.748313 bimcvcovid19i-0.0.6/bimcvcovid19i/
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2022-10-24 11:36:01.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/__init__.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       22 2022-10-24 13:46:59.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/__version__.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      884 2022-12-02 18:20:47.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/assets.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)    16778 2023-05-08 09:30:42.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/data.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2022-10-18 16:36:33.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/interface.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     4886 2022-12-03 14:07:39.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/postprocessing.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      225 2022-10-18 07:10:47.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/py.typed
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     5648 2022-10-21 12:40:09.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/tools.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6988 2022-10-25 16:48:30.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/typing.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     3802 2023-05-08 09:47:17.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/webdav.py
-drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 21:10:21.748313 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1108 2023-05-10 21:10:21.000000 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/PKG-INFO
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      529 2023-05-10 21:10:21.000000 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/SOURCES.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2023-05-10 21:10:21.000000 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/dependency_links.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2022-10-18 07:36:29.000000 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/not-zip-safe
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2023-05-10 21:10:21.000000 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/requires.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       14 2023-05-10 21:10:21.000000 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/top_level.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2022-12-02 14:19:33.000000 bimcvcovid19i-0.0.6/requirements.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       38 2023-05-10 21:10:21.748313 bimcvcovid19i-0.0.6/setup.cfg
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1325 2022-10-18 09:08:11.000000 bimcvcovid19i-0.0.6/setup.py
+drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 22:27:43.767092 bimcvcovid19i-0.0.7/
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1088 2022-10-18 07:33:34.000000 bimcvcovid19i-0.0.7/LICENSE
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      169 2022-10-18 07:33:57.000000 bimcvcovid19i-0.0.7/MANIFEST.in
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1207 2023-05-10 22:27:43.767092 bimcvcovid19i-0.0.7/PKG-INFO
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      675 2023-05-10 22:10:21.000000 bimcvcovid19i-0.0.7/README.md
+drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 22:27:43.767092 bimcvcovid19i-0.0.7/bimcvcovid19i/
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2022-10-24 11:36:01.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/__init__.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/__init__.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       22 2023-05-10 22:26:40.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/__version__.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/__version__.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      884 2023-05-10 21:16:06.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/assets.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      285 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/assets.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)    17304 2023-05-10 21:41:37.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/data.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     2058 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/data.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2022-10-18 16:36:33.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/interface.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/interface.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     4886 2022-12-03 14:07:39.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/postprocessing.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1333 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/postprocessing.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      225 2022-10-18 07:10:47.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/py.typed
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6745 2023-05-10 22:04:37.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/tools.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1261 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/tools.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6995 2023-05-10 22:05:50.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/typing.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     2438 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/typing.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     3802 2023-05-08 09:47:17.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/webdav.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      501 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/webdav.pyi
+drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 22:27:43.767092 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1207 2023-05-10 22:27:43.000000 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/PKG-INFO
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      769 2023-05-10 22:27:43.000000 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/SOURCES.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2023-05-10 22:27:43.000000 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/dependency_links.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2022-10-18 07:36:29.000000 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/not-zip-safe
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2023-05-10 22:27:43.000000 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/requires.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       14 2023-05-10 22:27:43.000000 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/top_level.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2022-12-02 14:19:33.000000 bimcvcovid19i-0.0.7/requirements.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       38 2023-05-10 22:27:43.767092 bimcvcovid19i-0.0.7/setup.cfg
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1325 2022-10-18 09:08:11.000000 bimcvcovid19i-0.0.7/setup.py
```

### Comparing `bimcvcovid19i-0.0.6/LICENSE` & `bimcvcovid19i-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.6/PKG-INFO` & `bimcvcovid19i-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimcvcovid19i
-Version: 0.0.6
+Version: 0.0.7
 Summary: Interface for working with BIMCV COVID 19 dataset
 Home-page: https://github.com/rilshok/BIMCV-COVID-19-interface
 Author: Vladislav A. Proskurov
 Author-email: rilshok@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -24,11 +24,12 @@
 
 ```bash
 pip install bimcvcovid19i
 ```
 
 ## System requirements
 
-|Dataset               |Original|Prepered|Total|
-|----------------------|:------:|:------:|:---:|
-|BIMCV COVID19 positive|    390G|    408G| 797G|
-|BIMCV COVID19 negative|    469G|    480G| 948G|
+|Dataset                         |Original|Prepered|Total|
+|--------------------------------|:------:|:------:|:---:|
+|BIMCV COVID19 positive cIter 12 |    390G|    408G| 797G|
+|BIMCV COVID19 negative cIter 12 |    469G|    480G| 948G|
+|BIMCV COVID19 positive cIter 123|    2.8T|      ?T|   ?T|
```

### Comparing `bimcvcovid19i-0.0.6/README.md` & `bimcvcovid19i-0.0.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 
 ```bash
 pip install bimcvcovid19i
 ```
 
 ## System requirements
 
-|Dataset               |Original|Prepered|Total|
-|----------------------|:------:|:------:|:---:|
-|BIMCV COVID19 positive|    390G|    408G| 797G|
-|BIMCV COVID19 negative|    469G|    480G| 948G|
+|Dataset                         |Original|Prepered|Total|
+|--------------------------------|:------:|:------:|:---:|
+|BIMCV COVID19 positive cIter 12 |    390G|    408G| 797G|
+|BIMCV COVID19 negative cIter 12 |    469G|    480G| 948G|
+|BIMCV COVID19 positive cIter 123|    2.8T|      ?T|   ?T|
```

### Comparing `bimcvcovid19i-0.0.6/bimcvcovid19i/assets.py` & `bimcvcovid19i-0.0.7/bimcvcovid19i/assets.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.6/bimcvcovid19i/data.py` & `bimcvcovid19i-0.0.7/bimcvcovid19i/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,16 +393,26 @@
     labels_tarfile_subpath = "covid19_posi/derivatives/labels/labels_covid_posi.tsv"
 
 
 class BIMCVCOVID19positiveData_123(BIMCVCOVID19Data):
     webdav_hostname = "https://b2drop.bsc.es/public.php/webdav"
     webdav_login = "BIMCV-COVID19-cIter_1_2_3"
     webdav_password = "maybeempty"
-    # TODO: maybe bug
 
+    subjects_tarfile_name = "covid19_posi_metadata.tar.gz"
+    subjects_tarfile_subpath = "covid19_posi/participants.tsv"
+
+    sessions_tarfile_name = "covid19_posi_sessions_tsv.tar.gz"
+
+    tests_tarfile_name = "covid19_posi_derivative.tar.gz"
+    tests_tarfile_subpath = "covid19_posi/derivatives/EHR/SIL_REG_COVID_POSI_iter123.txt"
+    # TODO: covid19_posi/derivatives/EHR/ contains other *.csv files
+
+    labels_tarfile_name = "covid19_posi_derivative.tar.gz"
+    labels_tarfile_subpath = "covid19_posi/derivatives/labels/Labels_covid_123.tsv"
 
 class BIMCVCOVID19negativeData_12(BIMCVCOVID19Data):
     webdav_hostname = "https://b2drop.bsc.es/public.php/webdav"
     webdav_login = "BIMCV-COVID19-cIter_1_2-Negative"
     webdav_password = "maybeempty"
 
     subjects_tarfile_name = "covid19_neg_metadata.tar.gz"
```

### Comparing `bimcvcovid19i-0.0.6/bimcvcovid19i/postprocessing.py` & `bimcvcovid19i-0.0.7/bimcvcovid19i/postprocessing.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.6/bimcvcovid19i/tools.py` & `bimcvcovid19i-0.0.7/bimcvcovid19i/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,23 +14,27 @@
     "png2numpy",
     "spacing_from_nifty",
     "down_type",
     "spacing_from_tags",
     "parse_dicom_tags",
     "derepr_strings_list",
     "open_from_tar",
+    "save_numpy",
+    "load_numpy",
 ]
 
 import contextlib
 import gzip
 import itertools as it
 import json
 import tarfile
 import typing as tp
+from gzip import GzipFile
 from pathlib import Path
+from typing import Optional
 
 import nibabel as nib  # type: ignore
 import numpy as np
 import pydicom
 import SimpleITK as sitk
 
 from .typing import LikePath, Spacing
@@ -196,7 +200,42 @@
 @contextlib.contextmanager
 def open_from_tar(path: LikePath, subpath: LikePath):
     path = str(Path(path).absolute())
     with tarfile.open(path) as file:
         member = file.extractfile(str(subpath))
         assert member is not None
         yield member
+
+
+def save_numpy(
+    value,
+    path,
+    *,
+    allow_pickle: bool = True,
+    fix_imports: bool = True,
+    compression: Optional[int] = None,
+    timestamp: Optional[int] = None,
+) -> None:
+    """A wrapper around ``np.save`` from deep_pipe."""
+    if compression is not None:
+        gzfile = GzipFile(path, "wb", compresslevel=compression, mtime=timestamp)
+        with gzfile as file:
+            return save_numpy(
+                value, file, allow_pickle=allow_pickle, fix_imports=fix_imports
+            )
+
+    np.save(path, value, allow_pickle=allow_pickle, fix_imports=fix_imports)
+
+
+def load_numpy(
+    path,
+    *,
+    allow_pickle: bool = True,
+    fix_imports: bool = True,
+    decompress: bool = False,
+):
+    """A wrapper around ``np.load`` from deep_pipe."""
+    if decompress:
+        with GzipFile(path, "rb") as file:
+            return load_numpy(file, allow_pickle=allow_pickle, fix_imports=fix_imports)
+
+    return np.load(path, allow_pickle=allow_pickle, fix_imports=fix_imports)
```

### Comparing `bimcvcovid19i-0.0.6/bimcvcovid19i/typing.py` & `bimcvcovid19i-0.0.7/bimcvcovid19i/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     modality: str
 
     def save(self, root: LikePath):
         root = Path(root)
         root.mkdir(exist_ok=True, parents=False)
         deli.save(self.uid, root / "uid.json")
         if self.image is not None:
-            deli.save(self.image, root / "image.npy.gz", compression=3, timestamp=0)
+            tools.save_numpy(self.image, root / "image.npy.gz", compression=3, timestamp=0)
             deli.save(self.image.shape, root / "shape.json")
         if self.spacing is not None:
             deli.save(list(map(float, self.spacing)), root / "spacing.json")
         if self.tags is not None:
             tools.save_json_gz(self.tags, root / "tags.json.gz", compression=3)
         deli.save(self.subject_id, root / "subject_id.json")
         deli.save(self.session_id, root / "session_id.json")
```

### Comparing `bimcvcovid19i-0.0.6/bimcvcovid19i/webdav.py` & `bimcvcovid19i-0.0.7/bimcvcovid19i/webdav.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/PKG-INFO` & `bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimcvcovid19i
-Version: 0.0.6
+Version: 0.0.7
 Summary: Interface for working with BIMCV COVID 19 dataset
 Home-page: https://github.com/rilshok/BIMCV-COVID-19-interface
 Author: Vladislav A. Proskurov
 Author-email: rilshok@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -24,11 +24,12 @@
 
 ```bash
 pip install bimcvcovid19i
 ```
 
 ## System requirements
 
-|Dataset               |Original|Prepered|Total|
-|----------------------|:------:|:------:|:---:|
-|BIMCV COVID19 positive|    390G|    408G| 797G|
-|BIMCV COVID19 negative|    469G|    480G| 948G|
+|Dataset                         |Original|Prepered|Total|
+|--------------------------------|:------:|:------:|:---:|
+|BIMCV COVID19 positive cIter 12 |    390G|    408G| 797G|
+|BIMCV COVID19 negative cIter 12 |    469G|    480G| 948G|
+|BIMCV COVID19 positive cIter 123|    2.8T|      ?T|   ?T|
```

### Comparing `bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/SOURCES.txt` & `bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 bimcvcovid19i/__init__.py
+bimcvcovid19i/__init__.pyi
 bimcvcovid19i/__version__.py
+bimcvcovid19i/__version__.pyi
 bimcvcovid19i/assets.py
+bimcvcovid19i/assets.pyi
 bimcvcovid19i/data.py
+bimcvcovid19i/data.pyi
 bimcvcovid19i/interface.py
+bimcvcovid19i/interface.pyi
 bimcvcovid19i/postprocessing.py
+bimcvcovid19i/postprocessing.pyi
 bimcvcovid19i/py.typed
 bimcvcovid19i/tools.py
+bimcvcovid19i/tools.pyi
 bimcvcovid19i/typing.py
+bimcvcovid19i/typing.pyi
 bimcvcovid19i/webdav.py
+bimcvcovid19i/webdav.pyi
 bimcvcovid19i.egg-info/PKG-INFO
 bimcvcovid19i.egg-info/SOURCES.txt
 bimcvcovid19i.egg-info/dependency_links.txt
 bimcvcovid19i.egg-info/not-zip-safe
 bimcvcovid19i.egg-info/requires.txt
 bimcvcovid19i.egg-info/top_level.txt
```

### Comparing `bimcvcovid19i-0.0.6/setup.py` & `bimcvcovid19i-0.0.7/setup.py`

 * *Files identical despite different names*

