# Comparing `tmp/carate-0.3.8.tar.gz` & `tmp/carate-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carate-0.3.8.tar", last modified: Mon Apr 17 16:40:20 2023, max compression
+gzip compressed data, was "carate-0.3.9.tar", last modified: Thu May 11 08:57:14 2023, max compression
```

## Comparing `carate-0.3.8.tar` & `carate-0.3.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.799767 carate-0.3.8/
--rw-r--r--   0 developer  (1001) developer  (1001)    33670 2023-03-27 16:07:17.000000 carate-0.3.8/LICENSE
--rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-04-17 16:40:20.799767 carate-0.3.8/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     6636 2023-04-05 20:48:54.000000 carate-0.3.8/README.md
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.796434 carate-0.3.8/carate/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.8/carate/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)      949 2023-04-15 18:59:22.000000 carate-0.3.8/carate/automate.py
--rw-r--r--   0 developer  (1001) developer  (1001)     7619 2023-04-15 18:59:22.000000 carate-0.3.8/carate/config.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1968 2023-04-17 16:22:52.000000 carate-0.3.8/carate/default_interface.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.796434 carate-0.3.8/carate/evaluation/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.8/carate/evaluation/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)    19159 2023-04-15 18:59:22.000000 carate-0.3.8/carate/evaluation/base.py
--rw-r--r--   0 developer  (1001) developer  (1001)      299 2023-04-15 18:59:22.000000 carate-0.3.8/carate/evaluation/classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)    11467 2023-04-17 16:22:52.000000 carate-0.3.8/carate/evaluation/regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)     7059 2023-04-15 18:59:22.000000 carate-0.3.8/carate/load_data.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.796434 carate-0.3.8/carate/models/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.8/carate/models/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)      483 2023-04-15 18:59:22.000000 carate-0.3.8/carate/models/base_model.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2048 2023-04-15 18:59:22.000000 carate-0.3.8/carate/models/cgc_classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1723 2023-04-15 18:59:22.000000 carate-0.3.8/carate/models/cgc_regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)      905 2023-04-15 18:59:22.000000 carate-0.3.8/carate/optimizer.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.799767 carate-0.3.8/carate/plotting/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.8/carate/plotting/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)    12892 2023-04-17 16:22:52.000000 carate-0.3.8/carate/plotting/base_plots.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1369 2023-04-17 16:21:54.000000 carate-0.3.8/carate/plotting/plot_classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)     5375 2023-04-15 18:59:22.000000 carate-0.3.8/carate/run.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.799767 carate-0.3.8/carate/utils/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.8/carate/utils/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2559 2023-04-15 18:59:22.000000 carate-0.3.8/carate/utils/convert_to_json.py
--rw-r--r--   0 developer  (1001) developer  (1001)     6362 2023-04-15 18:59:22.000000 carate-0.3.8/carate/utils/model_files.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1650 2023-04-15 18:59:22.000000 carate-0.3.8/carate/utils/training_result_parser.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.796434 carate-0.3.8/carate.egg-info/
--rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-04-17 16:40:20.000000 carate-0.3.8/carate.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     1030 2023-04-17 16:40:20.000000 carate-0.3.8/carate.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-17 16:40:20.000000 carate-0.3.8/carate.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       59 2023-04-17 16:40:20.000000 carate-0.3.8/carate.egg-info/entry_points.txt
--rw-r--r--   0 developer  (1001) developer  (1001)      154 2023-04-17 16:40:20.000000 carate-0.3.8/carate.egg-info/requires.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        7 2023-04-17 16:40:20.000000 carate-0.3.8/carate.egg-info/top_level.txt
--rw-r--r--   0 developer  (1001) developer  (1001)     1022 2023-04-17 16:40:12.000000 carate-0.3.8/pyproject.toml
--rw-r--r--   0 developer  (1001) developer  (1001)      459 2023-04-17 16:40:20.803100 carate-0.3.8/setup.cfg
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-17 16:40:20.799767 carate-0.3.8/tests/
--rw-r--r--   0 developer  (1001) developer  (1001)     4661 2023-03-29 18:42:59.000000 carate-0.3.8/tests/test_classification.py
--rw-r--r--   0 developer  (1001) developer  (1001)      732 2023-04-12 18:04:08.000000 carate-0.3.8/tests/test_cli.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2217 2023-03-29 18:42:59.000000 carate-0.3.8/tests/test_config.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2642 2023-04-12 18:04:08.000000 carate-0.3.8/tests/test_data_loader.py
--rw-r--r--   0 developer  (1001) developer  (1001)      978 2023-04-17 16:23:39.000000 carate-0.3.8/tests/test_plotting.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2827 2023-04-17 16:22:52.000000 carate-0.3.8/tests/test_regression.py
--rw-r--r--   0 developer  (1001) developer  (1001)      546 2023-03-27 16:07:17.000000 carate-0.3.8/tests/test_runner.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1522 2023-03-29 18:42:59.000000 carate-0.3.8/tests/test_utils_convert_py_to_json.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-05-11 08:57:14.966202 carate-0.3.9/
+-rw-r--r--   0 developer  (1001) developer  (1001)    33670 2023-03-27 16:07:17.000000 carate-0.3.9/LICENSE
+-rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-05-11 08:57:14.966202 carate-0.3.9/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     6636 2023-04-05 20:48:54.000000 carate-0.3.9/README.md
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-05-11 08:57:14.959536 carate-0.3.9/carate/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.9/carate/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      949 2023-04-15 18:59:22.000000 carate-0.3.9/carate/automate.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     7619 2023-04-15 18:59:22.000000 carate-0.3.9/carate/config.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1968 2023-04-17 16:22:52.000000 carate-0.3.9/carate/default_interface.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-05-11 08:57:14.962869 carate-0.3.9/carate/evaluation/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.9/carate/evaluation/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    19159 2023-04-15 18:59:22.000000 carate-0.3.9/carate/evaluation/base.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      299 2023-04-15 18:59:22.000000 carate-0.3.9/carate/evaluation/classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    11476 2023-05-11 08:49:18.000000 carate-0.3.9/carate/evaluation/regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     7059 2023-04-15 18:59:22.000000 carate-0.3.9/carate/load_data.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-05-11 08:57:14.962869 carate-0.3.9/carate/models/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.9/carate/models/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      483 2023-04-15 18:59:22.000000 carate-0.3.9/carate/models/base_model.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2048 2023-04-15 18:59:22.000000 carate-0.3.9/carate/models/cgc_classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1723 2023-04-15 18:59:22.000000 carate-0.3.9/carate/models/cgc_regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      905 2023-04-15 18:59:22.000000 carate-0.3.9/carate/optimizer.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-05-11 08:57:14.962869 carate-0.3.9/carate/plotting/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.9/carate/plotting/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     8457 2023-05-09 10:38:00.000000 carate-0.3.9/carate/plotting/base_plots.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1369 2023-05-06 19:21:09.000000 carate-0.3.9/carate/plotting/plot_classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     5375 2023-04-15 18:59:22.000000 carate-0.3.9/carate/run.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-05-11 08:57:14.962869 carate-0.3.9/carate/utils/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-15 18:59:22.000000 carate-0.3.9/carate/utils/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2559 2023-04-15 18:59:22.000000 carate-0.3.9/carate/utils/convert_to_json.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     6362 2023-04-15 18:59:22.000000 carate-0.3.9/carate/utils/model_files.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1650 2023-04-15 18:59:22.000000 carate-0.3.9/carate/utils/training_result_parser.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-05-11 08:57:14.962869 carate-0.3.9/carate.egg-info/
+-rw-r--r--   0 developer  (1001) developer  (1001)     7206 2023-05-11 08:57:14.000000 carate-0.3.9/carate.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     1030 2023-05-11 08:57:14.000000 carate-0.3.9/carate.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-05-11 08:57:14.000000 carate-0.3.9/carate.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       59 2023-05-11 08:57:14.000000 carate-0.3.9/carate.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)      154 2023-05-11 08:57:14.000000 carate-0.3.9/carate.egg-info/requires.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        7 2023-05-11 08:57:14.000000 carate-0.3.9/carate.egg-info/top_level.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)     1027 2023-05-11 08:57:09.000000 carate-0.3.9/pyproject.toml
+-rw-r--r--   0 developer  (1001) developer  (1001)      459 2023-05-11 08:57:14.966202 carate-0.3.9/setup.cfg
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-05-11 08:57:14.966202 carate-0.3.9/tests/
+-rw-r--r--   0 developer  (1001) developer  (1001)     4661 2023-03-29 18:42:59.000000 carate-0.3.9/tests/test_classification.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      732 2023-04-12 18:04:08.000000 carate-0.3.9/tests/test_cli.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2217 2023-03-29 18:42:59.000000 carate-0.3.9/tests/test_config.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2642 2023-04-12 18:04:08.000000 carate-0.3.9/tests/test_data_loader.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1021 2023-05-06 19:19:16.000000 carate-0.3.9/tests/test_plotting.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2827 2023-04-17 16:22:52.000000 carate-0.3.9/tests/test_regression.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      546 2023-03-27 16:07:17.000000 carate-0.3.9/tests/test_runner.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1522 2023-03-29 18:42:59.000000 carate-0.3.9/tests/test_utils_convert_py_to_json.py
```

### Comparing `carate-0.3.8/LICENSE` & `carate-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/PKG-INFO` & `carate-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carate
-Version: 0.3.8
+Version: 0.3.9
 Summary: Providing reproducible modeling
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/sail.black/carate.git
 Project-URL: Bug Tracker, https://www.codeberg.org/sail.black/carate.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `carate-0.3.8/README.md` & `carate-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/automate.py` & `carate-0.3.9/carate/automate.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/config.py` & `carate-0.3.9/carate/config.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/default_interface.py` & `carate-0.3.9/carate/default_interface.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/evaluation/base.py` & `carate-0.3.9/carate/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/evaluation/regression.py` & `carate-0.3.9/carate/evaluation/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,14 +178,15 @@
 
             del train_dataset, test_dataset
 
             if normalize:
                 norm_factor = self.__normalization_factor(
                     data_set=loaded_dataset, num_classes=num_classes
                 )
+        
             else:
                 norm_factor = 1.0
             for epoch in range(1, num_epoch + 1):
                 train_mae_loss = self.train(
                     model_net=model_net,
                     epoch=epoch,
                     optimizer=optimizer,
```

### Comparing `carate-0.3.8/carate/load_data.py` & `carate-0.3.9/carate/load_data.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/models/cgc_classification.py` & `carate-0.3.9/carate/models/cgc_classification.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/models/cgc_regression.py` & `carate-0.3.9/carate/models/cgc_regression.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/optimizer.py` & `carate-0.3.9/carate/optimizer.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/plotting/base_plots.py` & `carate-0.3.9/carate/plotting/base_plots.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 """
 from typing import Type, Optional, Dict, Any, List, Tuple
 import logging
 import numpy as np
 import matplotlib.pyplot as plt
 from amarium.utils import load_json_from_file, prepare_file_name_saving, append_slash
 
-
-logging.basicConfig(
-    filename="train.log",
-    encoding="utf-8",
-    level=logging.DEBUG,
-    format="%(asctime)s %(message)s",
+from carate.statistics.analysis import (
+    get_avg,
+    get_min,
+    get_max,
+    unpack_run,
+    get_stacked_list,
+    load_result_json,
+    get_min_max_avg_cv_run,
 )
 
 
 def plot_range_band_multi(
     result: List[Dict[str, float]],
     key_vals: List[str],
     file_name: str,
@@ -49,15 +51,15 @@
     axis.set_xlabel("Training step")
 
     for i in range(len(key_vals)):
         max_val: List[float]
         min_val: List[float]
         avg_val: List[float]
 
-        max_val, min_val, avg_val = unpack_cross_validation(
+        max_val, min_val, avg_val = get_min_max_avg_cv_run(
             result=result, key_val=key_vals[i]
         )
         logging.info(f"Max values are: {max_val}")
         logging.info(f"Min values are: {min_val}")
         logging.info(f"Avg values are: {avg_val}")
 
         axis.plot(avg_val, label=key_vals[i])
@@ -92,15 +94,15 @@
 
     :doc-author: Julian M. Kleber
     """
     max_val: List[float]
     min_val: List[float]
     avg_val: List[float]
 
-    max_val, min_val, avg_val = unpack_cross_validation(result=result, key_val=key_val)
+    max_val, min_val, avg_val = get_min_max_avg_cv_run(result=result, key_val=key_val)
 
     fig, axis = plt.subplots()
     if legend_text is not None:
         axis.plot(avg_val, "-", label=legend_text)
     else:
         axis.plot(avg_val, "-", label=legend_text)
     plot_range_fill(max_val, min_val, alpha, axis)
@@ -132,49 +134,14 @@
     :doc-author: Julian M. Kleber
     """
 
     training_steps = np.arange(0, len(max_val), 1)
     axis.fill_between(training_steps, min_val, max_val, alpha=alpha)
 
 
-def unpack_cross_validation(
-    result: List[Dict[str, List[float]]], key_val: str
-) -> Tuple[List[float]]:
-    """
-    The unpack_cross_validation function takes in a list of dictionaries, and a key value.
-    It then unpacks the values associated with that key into three lists: max_val, min_val, avg_val.
-    These lists are returned as a tuple.
-
-    :param result:List[Dict[str: Used to Store the result of each iteration.
-    :param float]]: Used to Store the results of the cross validation.
-    :param key_val:str: Used to Specify which key in the dictionary to use for the unpacking.
-    :return: The max, min and average value of the key_val parameter.
-
-    :doc-author: Julian M. Kleber
-    """
-
-    max_val = []
-    min_val = []
-    avg_val = []
-
-    arr_res = np.zeros((len(result), len(result[0][key_val])))
-
-    for i, res in enumerate(result):
-        assert len(res[key_val]) == arr_res.shape[1], str(len(res[key_val])) + str(
-            arr_res.shape[1]
-        )
-        arr_res[i, :] = res[key_val]
-
-    for i in range(arr_res.shape[1]):
-        max_val.append(get_max(arr_res[:, i].tolist()))
-        min_val.append(get_min(arr_res[:, i].tolist()))
-        avg_val.append(get_avg(arr_res[:, i].tolist()))
-
-    return (max_val, min_val, avg_val)
-
 
 def save_publication_graphic(
     fig_object: Type[plt.figure], file_name: str, prefix: Optional[str] = None
 ) -> None:
     """
     The save_publication_graphic function saves the current figure to a file.
 
@@ -192,89 +159,36 @@
     file_name = prepare_file_name_saving(
         file_name=file_name, prefix=prefix, suffix=".png"
     )
     plt.tight_layout()
     plt.savefig(file_name, dpi=300)
 
 
-def get_stacked_list(
-    path_to_directory: str, num_cv: int, json_name: str
-) -> List[Dict[str, float]]:
-    """
-    The get_stacked_list function takes in a path to a directory, the name of the column
-    that we want to stack, and the number of cross-validation folds. It then returns a list
-    of dictionaries that contain all of our stacked results.
-
-    :param path_to_directory:str: Used to Specify the directory where the json files are stored.
-    :param column_name:str: Used to Specify the column name of the dataframe in which we
-    want to get.
-    :param num_cv:int: Used to Specify the number of cross validation runs.
-    :param json_name:str: Used to Specify the name of the json file that will be parsed.
-    :return: A list of dictionaries, where each dictionary is the accuracy for a single cv.
-
-    :doc-author: Julian M. Kleber
-    """
-
-    results = []
-
-    path_to_directory = append_slash(path_to_directory)
-
-    for i in range(num_cv):
-        logging.info(f"Attempting cv {i}")
-
-        result = parse_acc_list_json(
-            path_to_json=path_to_directory + f"CV_{i}/" + json_name
-        )
-        results.append(result)
-        logging.info(f"parsed results for CV {i}")
-
-    return results
-
-
 def parse_old_file_format_for_plot(
     path_to_json: str,
 ) -> List[List[float]]:  # pragma no-cover
     """
     The parse_old_file_format_for_plot function takes in a path to a json file and returns the
     following:
 
     :param path_to_json:str: Used to Specify the path to the json file that we want to parse.
     :return: A list of dictionaries.
 
     :doc-author: Julian M. Kleber
     """
 
-    result_acc = parse_acc_list_json(path_to_json=path_to_json)
+    result_acc = load_result_json(path_to_json=path_to_json)
     train_frames_acc = parse_min_max_avg(result_acc["Train_acc"])
     test_frames_acc = parse_min_max_avg(result_acc["Test_acc"])
     return train_frames_acc, test_frames_acc
 
 
-def parse_acc_list_json(path_to_json: str) -> Dict[str, Any]:
-    """
-    The parse_acc_list_json function takes in a path to a json file and returns the contents of
-    that json file as a dictionary.The function also parses the "Acc" key in the dictionary,
-    which contains lists of tuples containing train and test accuracy values.
-    The function then separates these tuples into two separate lists, one for train accuracy values
-    and one for test accuracy values. These new lists are added to the original dictionary under
-    keys "Acc_train" and "Acc_val", respectively.
-
-    :param path_to_json:str: Used to Specify the path to the json file.
-    :return: A dictionary with the following keys:.
-
-    :doc-author: Julian M. Kleber
-    """
-
-    result = load_json_from_file(path_to_json)
-    return result
-
-
-def parse_acc_list_json_old_format(path_to_json: str) -> Dict[str, Any]:
+def load_result_json_old_format(path_to_json: str) -> Dict[str, Any]:
     """
-    The parse_acc_list_json function takes in a path to a json file and returns the contents of
+    The load_result_json function takes in a path to a json file and returns the contents of
     that json file as a dictionary.The function also parses the "Acc" key in the dictionary, which
     contains lists of tuples containing train and test accuracy values.
     The function then separates these tuples into two separate lists, one for train accuracy values
     and one for test accuracy values.These new lists are added to the original dictionary under
     keys "Acc_train" and "Acc_val", respectively.
 
     :param path_to_json:str: Used to Specify the path to the json file.
@@ -318,50 +232,7 @@
         minimum = get_min(step_list=step_list)
         maximum = get_max(step_list=step_list)
         average = get_avg(step_list=step_list)
         minima.append(minimum)
         maxima.append(maximum)
         averages.append(average)
     return [minima, maxima, averages]
-
-
-def get_avg(step_list: List[float]) -> float:
-    """
-    The get_avg function takes a list of floats and returns the average value.
-
-
-    :param step_list:List[float]: Used to Tell the function that it will be taking a list of
-    floats as an argument.
-    :return: The mean of the step_list.
-
-    :doc-author: Julian M. Kleber
-    """
-
-    return float(np.mean(step_list))
-
-
-def get_max(step_list: List[float]) -> float:
-    """
-    The get_max function takes a list of floats and returns the maximum value in that list.
-
-
-    :param step_list:List[float]: Used to Tell the function that step_list is a list of floats.
-    :return: The maximum value in the list.
-
-    :doc-author: Julian M. Kleber
-    """
-
-    return float(np.max(step_list))
-
-
-def get_min(step_list: List[float]) -> float:
-    """
-    The get_min function takes a list of floats and returns the minimum value in that list.
-
-    :param step_list:List[float]: Used to Specify the type of parameter that is being passed
-    into the function.
-    :return: The minimum value in the step_list.
-
-    :doc-author: Julian M. Kleber
-    """
-
-    return float(np.min(step_list))
```

### Comparing `carate-0.3.8/carate/plotting/plot_classification.py` & `carate-0.3.9/carate/plotting/plot_classification.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/run.py` & `carate-0.3.9/carate/run.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/utils/convert_to_json.py` & `carate-0.3.9/carate/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/utils/model_files.py` & `carate-0.3.9/carate/utils/model_files.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate/utils/training_result_parser.py` & `carate-0.3.9/carate/utils/training_result_parser.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/carate.egg-info/PKG-INFO` & `carate-0.3.9/carate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carate
-Version: 0.3.8
+Version: 0.3.9
 Summary: Providing reproducible modeling
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/sail.black/carate.git
 Project-URL: Bug Tracker, https://www.codeberg.org/sail.black/carate.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `carate-0.3.8/carate.egg-info/SOURCES.txt` & `carate-0.3.9/carate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/pyproject.toml` & `carate-0.3.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "carate"
-version = "0.3.8"
+version = "0.3.9"
 authors = [
   { name="Julian M. Kleber", email="julian.m.kleber@gmail.com" },
 ]
 description = "Providing reproducible modeling"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -24,15 +24,16 @@
     "torchaudio",
     "torch-geometric",
     "rdkit-pypi",
     "networkx[default]",
     "matplotlib",  
     "Click", 
     "amarium", 
-    "black"]
+    "black"
+    ]
 
 [project.urls]
 "Homepage" = "https://www.codeberg.org/sail.black/carate.git"
 "Bug Tracker" = "https://www.codeberg.org/sail.black/carate.git/issues"
 [tool.setuptools]
 
 packages = ["carate", "carate.evaluation", "carate.models", "carate.plotting", "carate.utils"]
```

### Comparing `carate-0.3.8/tests/test_classification.py` & `carate-0.3.9/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/tests/test_cli.py` & `carate-0.3.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/tests/test_config.py` & `carate-0.3.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/tests/test_data_loader.py` & `carate-0.3.9/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/tests/test_plotting.py` & `carate-0.3.9/tests/test_plotting.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 from carate.plotting.plot_classification import plot_classification_algorithm
 
 from tests.utils import check_plotting_dir
 
 
 def test_classification_plot_run():
     check_plotting_dir()
-    path_to_directory = "./notebooks/data/ENZYMES"
+    path_to_directory = "./notebooks/data/Classification/ENZYMES/"
     parameter = "Acc_test"
 
     plot_classification_algorithm(
         path_to_directory=path_to_directory, parameter=parameter
     )
     assert os.path.isdir("./plots")
     assert os.path.isfile(f"./plots/ENZYMES_{parameter}.png")
 
 
 def test_regression_plot_run():
     check_plotting_dir()
-    path_to_directory = "./notebooks/data/ALCHEMY_20_test_training_length_no_norm/"
+    path_to_directory = (
+        "./notebooks/data/Regression/ALCHEMY_20_test_training_length_no_norm/"
+    )
     parameter = "MAE Train"
     data_name = "alchemy_full.json"
 
     plot_classification_algorithm(
         path_to_directory=path_to_directory, parameter=parameter, data_name=data_name
     )
     assert os.path.isdir("./plots")
```

### Comparing `carate-0.3.8/tests/test_regression.py` & `carate-0.3.9/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/tests/test_runner.py` & `carate-0.3.9/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `carate-0.3.8/tests/test_utils_convert_py_to_json.py` & `carate-0.3.9/tests/test_utils_convert_py_to_json.py`

 * *Files identical despite different names*

