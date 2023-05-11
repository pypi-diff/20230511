# Comparing `tmp/enstools-compression-2023.4.1.tar.gz` & `tmp/enstools-compression-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstools-compression-2023.4.1.tar", last modified: Mon Apr 17 16:08:59 2023, max compression
+gzip compressed data, was "enstools-compression-2023.5.tar", last modified: Thu May 11 15:11:19 2023, max compression
```

## Comparing `enstools-compression-2023.4.1.tar` & `enstools-compression-2023.5.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.975639 enstools-compression-2023.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    10898 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1662 2023-04-17 16:08:59.975639 enstools-compression-2023.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-17 15:51:33.000000 enstools-compression-2023.4.1/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.971639 enstools-compression-2023.4.1/enstools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.973639 enstools-compression-2023.4.1/enstools/compression/
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.973639 enstools-compression-2023.4.1/enstools/compression/analyzer/
--rw-rw-rw-   0 root         (0) root         (0)     3099 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/analyzer/AnalysisOptions.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/analyzer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6293 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/analyzer/analyze_data_array.py
--rwxrwxrwx   0 root         (0) root         (0)    10373 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/analyzer/analyzer.py
--rw-rw-rw-   0 root         (0) root         (0)     8194 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/analyzer/analyzer_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/api.py
--rw-rw-rw-   0 root         (0) root         (0)    16861 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/cli.py
--rwxrwxrwx   0 root         (0) root         (0)    11172 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/compressor.py
--rwxrwxrwx   0 root         (0) root         (0)     3354 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/emulation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.974639 enstools-compression-2023.4.1/enstools/compression/emulators/
--rw-rw-rw-   0 root         (0) root         (0)     1188 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/emulators/EmulatorClass.py
--rw-rw-rw-   0 root         (0) root         (0)     2565 2023-02-10 12:30:33.000000 enstools-compression-2023.4.1/enstools/compression/emulators/FiltersEmulator.py
--rwxrwxrwx   0 root         (0) root         (0)     2885 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/emulators/LibpressioEmulator.py
--rwxrwxrwx   0 root         (0) root         (0)     2036 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/emulators/ZFPEmulator.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/emulators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2715 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/evaluator.py
--rw-rw-rw-   0 root         (0) root         (0)     3736 2023-02-10 12:30:33.000000 enstools-compression-2023.4.1/enstools/compression/h5netcdf_compressor.py
--rw-rw-rw-   0 root         (0) root         (0)    11156 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     4557 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/pruner.py
--rw-rw-rw-   0 root         (0) root         (0)    10801 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/significant_bits.py
--rw-rw-rw-   0 root         (0) root         (0)      910 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/size_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     7903 2023-02-10 12:30:33.000000 enstools-compression-2023.4.1/enstools/compression/slicing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.974639 enstools-compression-2023.4.1/enstools/compression/xr_accessor/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/xr_accessor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5314 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/enstools/compression/xr_accessor/accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:08:59.975639 enstools-compression-2023.4.1/enstools_compression.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1662 2023-04-17 16:08:59.000000 enstools-compression-2023.4.1/enstools_compression.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1284 2023-04-17 16:08:59.000000 enstools-compression-2023.4.1/enstools_compression.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 16:08:59.000000 enstools-compression-2023.4.1/enstools_compression.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-17 16:08:59.000000 enstools-compression-2023.4.1/enstools_compression.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-04-17 16:08:59.000000 enstools-compression-2023.4.1/enstools_compression.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-17 16:08:59.000000 enstools-compression-2023.4.1/enstools_compression.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 16:08:59.975639 enstools-compression-2023.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-01-18 16:33:07.000000 enstools-compression-2023.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:11:19.355095 enstools-compression-2023.5/
+-rw-rw-rw-   0 root         (0) root         (0)    10898 2023-01-18 16:33:07.000000 enstools-compression-2023.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-01-18 16:33:07.000000 enstools-compression-2023.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-11 15:11:19.354095 enstools-compression-2023.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-01-18 16:33:07.000000 enstools-compression-2023.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-11 13:20:17.000000 enstools-compression-2023.5/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:11:19.350095 enstools-compression-2023.5/enstools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:11:19.352095 enstools-compression-2023.5/enstools/compression/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:11:19.353095 enstools-compression-2023.5/enstools/compression/analyzer/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-01-18 16:33:07.000000 enstools-compression-2023.5/enstools/compression/analyzer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4050 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/analyzer/analysis_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     6932 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/analyzer/analyze_data_array.py
+-rwxrwxrwx   0 root         (0) root         (0)    10707 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/analyzer/analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)    12948 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/analyzer/analyzer_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    19012 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)    11108 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/compressor.py
+-rwxrwxrwx   0 root         (0) root         (0)     5492 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/emulation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:11:19.353095 enstools-compression-2023.5/enstools/compression/emulators/
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/emulators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/emulators/emulator_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/emulators/filters_emulator.py
+-rwxrwxrwx   0 root         (0) root         (0)     4847 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/emulators/libpressio_emulator.py
+-rwxrwxrwx   0 root         (0) root         (0)     2959 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/emulators/zfp_emulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2908 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/evaluator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5369 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/h5netcdf_compressor.py
+-rw-rw-rw-   0 root         (0) root         (0)    12646 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     4660 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/pruner.py
+-rw-rw-rw-   0 root         (0) root         (0)    19657 2023-05-11 13:20:17.000000 enstools-compression-2023.5/enstools/compression/significant_bits.py
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/size_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8244 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/slicing.py
+-rw-rw-rw-   0 root         (0) root         (0)     6731 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/xr_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:11:19.354095 enstools-compression-2023.5/enstools_compression.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-11 15:11:19.000000 enstools-compression-2023.5/enstools_compression.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-05-11 15:11:19.000000 enstools-compression-2023.5/enstools_compression.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 15:11:19.000000 enstools-compression-2023.5/enstools_compression.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-11 15:11:19.000000 enstools-compression-2023.5/enstools_compression.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-05-11 15:11:19.000000 enstools-compression-2023.5/enstools_compression.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-11 15:11:19.000000 enstools-compression-2023.5/enstools_compression.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 15:11:19.355095 enstools-compression-2023.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-01-18 16:33:07.000000 enstools-compression-2023.5/setup.py
```

### Comparing `enstools-compression-2023.4.1/LICENSE` & `enstools-compression-2023.5/LICENSE`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.4.1/PKG-INFO` & `enstools-compression-2023.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstools-compression
-Version: 2023.4.1
+Version: 2023.5
 Home-page: https://github.com/wavestoweather/enstools-compression
 Author: Oriol Tintó
 Author-email: oriol.tinto@lmu.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enstools-compression [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-compression.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `enstools-compression-2023.4.1/README.md` & `enstools-compression-2023.5/README.md`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.4.1/enstools/compression/analyzer/AnalysisOptions.py` & `enstools-compression-2023.5/enstools/compression/analyzer/analysis_options.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,23 @@
+"""
+Module containing AnalysisOptions and AnalysisParameters classes.
+"""
 from dataclasses import dataclass
 from typing import Union
 
 from enstools.core.errors import EnstoolsError
 from enstools.encoding.api import lossy_compressors_and_modes
 
 
 @dataclass
 class AnalysisOptions:
+    """
+    A class representing analysis options, including compressor, mode,
+    constraints, and thresholds.
+    """
     compressor: str
     mode: str
     constrains: str
     thresholds: dict
 
     def __init__(self,
                  compressor: Union[str, None],
@@ -30,61 +37,79 @@
             self.thresholds = thresholds
         else:
             raise AssertionError("Only one of the two arguments should be provided.")
 
 
 @dataclass
 class AnalysisParameters:
+    """
+    A class representing analysis parameters, including the AnalysisOptions instance.
+    """
     options: AnalysisOptions
 
     def __post_init__(self):
         # If mode is not None, compressor also shouldn't be None
         if self.options.mode is not None and self.options.compressor is None:
             raise EnstoolsError(f"Compression mode is assigned to {self.options.mode} but no compressor is specified.")
         self.multi_mode = self.options.mode in [None, "None", "all"]
 
     @property
     def compressors(self):
+        """
+        Get the list of compressors to be used based on the AnalysisOptions instance.
+
+        :return: A list of compressor names. If the option is "None" or "all",
+                 it returns all available compressors from the `lossy_compressors_and_modes` dictionary.
+                 Otherwise, it returns a list containing a single compressor specified in the options.
+        """
         if self.options.compressor in ["None", "all"]:
-            return [compressor for compressor in lossy_compressors_and_modes]
-        else:
-            return [self.options.compressor]
+            return list(lossy_compressors_and_modes)
+
+        return [self.options.compressor]
 
     def get_compressor_mode_combinations(self):
         """
-        Get a list of compressors and modes that will be evaluated.
-        :return:
+        Get a list of compressor and mode combinations that will be evaluated.
+
+        :return: A dictionary with keys in the format "compressor:mode" and
+                 values as tuples (compressor, mode).
         """
 
         combinations_dictionary = {}
         # In case both the compressor and the mode are defined, just return these
         if not self.multi_mode:
             combinations_dictionary[f"{self.options.compressor}:{self.options.mode}"] = (
                 self.options.compressor, self.options.mode)
             return combinations_dictionary
-        else:
-            # Otherwise, loop over the possible combinations
-            for compressor in self.compressors:
-                for mode in lossy_compressors_and_modes[compressor]:
-                    # FIXME: For now we are skipping the norm2 and psnr modes for sz3 because seem to be buggy
-                    if mode in ["norm2", "psnr"]:
-                        continue
-                    combinations_dictionary[f"{compressor}:{mode}"] = (compressor, mode)
-            return combinations_dictionary
+
+        # Otherwise, loop over the possible combinations
+        for compressor in self.compressors:
+            for mode in lossy_compressors_and_modes[compressor]:
+                # FIXME: For now we are skipping the norm2 and psnr modes for sz3 because seem to be buggy
+                if mode in ["norm2", "psnr"]:
+                    continue
+                combinations_dictionary[f"{compressor}:{mode}"] = (compressor, mode)
+        return combinations_dictionary
 
 
 def from_dict_to_csv(dictionary: dict) -> str:
     """
-    Convert a dictionary to a csv string.
+    Convert a dictionary to a CSV string.
+
+    :param dictionary: The dictionary to convert.
+    :return: The CSV string representation of the dictionary.
     """
     return ",".join([f"{key}:{value}" for key, value in dictionary.items()])
 
 
 def from_csv_to_dict(csv: str) -> dict:
     """
-    Convert a csv string to a dictionary.
+    Convert a CSV string to a dictionary.
+
+    :param csv: The CSV string to convert.
+    :return: The dictionary representation of the CSV string.
     """
     to_return = {}
     for entry in csv.split(","):
         key, value = entry.split(":")
         to_return[key] = float(value)
     return to_return
```

### Comparing `enstools-compression-2023.4.1/enstools/compression/analyzer/analyze_data_array.py` & `enstools-compression-2023.5/enstools/compression/analyzer/analyze_data_array.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,65 @@
+"""
+This module provides functions to find the compression specification that corresponds
+to a given data array and a set of compression options.
+
+The main function, `analyze_data_array`, takes a `data_array` and an `options` object
+and returns the compression specification and metrics computed with the compressed data.
+
+The functions use a bisection method to find the optimal compression parameter that meets
+quality requirements.
+"""
+# pylint: disable=W0603
 import copy
 import logging
-from typing import Tuple, Type, Callable, Union
 import warnings
+from typing import Tuple, Callable
 
 import numpy as np
 import xarray
 
+from enstools.compression.emulators import DefaultEmulator
 from enstools.encoding.api import VariableEncoding
 from enstools.encoding.rules import COMPRESSION_SPECIFICATION_SEPARATOR
-
-from .AnalysisOptions import AnalysisOptions
-from enstools.compression.emulators import default_emulator
+from .analysis_options import AnalysisOptions
 from .analyzer_utils import get_metrics, get_parameter_range, bisection_method
 
 # These metrics will be used to select within the different encodings when aiming at a certain compression ratio.
 ANALYSIS_DIAGNOSTIC_METRICS = ["correlation_I", "ssim_I"]
 COMPRESSION_RATIO_LABEL = "compression_ratio"
-counter = 0
+
+COUNTER = 0
 
 
 def find_direct_relation(parameter_range, function_to_nullify):
-    MIN, MAX = parameter_range
-    firstQ = MIN + (MAX - MIN) / 10
-    thirdQ = MIN + 9*(MAX - MIN) / 10
-
-    eval_firstQ = function_to_nullify(firstQ)
-    eval_thirdQ = function_to_nullify(thirdQ)
-    return eval_thirdQ > eval_firstQ
+    """Return whether the nullified function has a direct relation between the parameter and the nullified value."""
+    min_val, max_val = parameter_range
+    first_q = min_val + (max_val - min_val) / 10
+    third_q = min_val + 9 * (max_val - min_val) / 10
+
+    eval_first_q = function_to_nullify(first_q)
+    eval_third_q = function_to_nullify(third_q)
+    return eval_third_q > eval_first_q
 
 
 def analyze_data_array(data_array: xarray.DataArray, options: AnalysisOptions) -> Tuple[str, dict]:
     """
     Find the compression specification corresponding to a certain data array and a given set of compression options.
     """
     # In case there is a time dimension, select the last element.
     # There are accumulative variables (like total precipitation) which have mostly 0 on the first time step.
     # Using the last time-step can represent an advantage somehow.
     if "time" in data_array.dims:
         data_array = data_array.isel(time=-1)
     # Check if the array contains any nan
     contains_nan = np.isnan(data_array.values).any()
     if contains_nan:
-        logging.warning(f"The variable {data_array.name!r} contains NaN. Falling to 'lossless'.\n"
-                        "It is possible to prevent that replacing the NaN values using the parameter --fill-na")
+        logging.warning("The variable %scontains NaN. Falling to 'lossless'.\n"
+                        "It is possible to prevent that replacing the NaN values using the parameter --fill-na",
+                        data_array.name)
         return "lossless", {**{COMPRESSION_RATIO_LABEL: 1.0}, **{met: 0. for met in ANALYSIS_DIAGNOSTIC_METRICS}}
 
     # Define the functions that will be used to find optimal parameters
     get_metric_from_parameter, function_to_nullify, constrain = define_functions_to_optimize(data_array, options)
 
     # Define parameter range
     parameter_range = get_parameter_range(data_array, options)
@@ -69,59 +82,59 @@
 
         # Compute metrics
         # When aiming for a compression ratio some other metrics need to be provided too.
         if COMPRESSION_RATIO_LABEL not in options.thresholds:
             metrics = get_metric_from_parameter(parameter)
         else:
             new_options = copy.deepcopy(options)
-            for m in ANALYSIS_DIAGNOSTIC_METRICS:
-                new_options.thresholds[m] = 1
+            for metric in ANALYSIS_DIAGNOSTIC_METRICS:
+                new_options.thresholds[metric] = 1
             get_metric_from_parameter, _, _ = define_functions_to_optimize(data_array, new_options)
             metrics = get_metric_from_parameter(parameter)
 
     # Define compression specification
     separator = COMPRESSION_SPECIFICATION_SEPARATOR
     compression_spec = f"{separator}".join(["lossy",
                                             options.compressor,
                                             options.mode,
                                             f"{parameter:.3g}",
                                             ])
 
-    logging.debug(f"Evaluated the function {counter} times.")
+    logging.debug("Evaluated the function %d times.", COUNTER)
     return compression_spec, metrics
 
 
 def define_functions_to_optimize(data_array: xarray.DataArray, options: AnalysisOptions) -> \
         Tuple[Callable, Callable, Callable]:
     """
     Function to get methods that will be used to perform a bisection method and find proper compression parameters.
     """
     thresholds = options.thresholds
-    global counter
-    counter = 0
+    global COUNTER
+    COUNTER = 0
 
     # Using a cache allows us to avoid recomputing when using the same parameters.
     # @functools.lru_cache
     def get_metrics_from_parameter(parameter: float) -> dict:
         """
         This function will return a dictionary with different metrics computed with data that has been compressed
         with a specific parameter.
         """
-        global counter
-        counter += 1
+        global COUNTER
+        COUNTER += 1
 
         target = data_array.copy(deep=True)
 
         # Set buffers
         uncompressed_data = data_array.values
 
         # Get encoding from options:
         encoding = VariableEncoding(compressor=options.compressor, mode=options.mode, parameter=parameter)
         # Create compressor for case
-        analysis_compressor = default_emulator(encoding, uncompressed_data)
+        analysis_compressor = DefaultEmulator(encoding, uncompressed_data)
         # Compress and decompress data
         decompressed = analysis_compressor.compress_and_decompress(uncompressed_data)
         # Assign values to target data_array (need to use enstools metrics)
         target.values = decompressed
 
         # Get compression ratio
         compression_ratio = analysis_compressor.compression_ratio()
@@ -132,15 +145,15 @@
     def function_to_nullify(parameter):
         """
         Our parameter will be optimal when the value of this function is 0.
         Which would be the less strict value that fulfills the quality requirements.
 
         """
         metrics = get_metrics_from_parameter(parameter)
-        return min([metrics[metric] - options.thresholds[metric] for metric in thresholds.keys()])
+        return min(metrics[metric] - options.thresholds[metric] for metric in thresholds.keys())
 
     def constrain(parameter):
         """
         If the value of the function_to_nullify is positive it means that the thresholds are fulfilled.
         """
         return function_to_nullify(parameter) >= 0.
```

### Comparing `enstools-compression-2023.4.1/enstools/compression/analyzer/analyzer.py` & `enstools-compression-2023.5/enstools/compression/analyzer/analyzer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """
-    #
-    # Routines to find optimal compression parameters to satisfy certain quality thresholds
-    #
+
+    Routines to find optimal compression parameters that maximise
+    compression ratios while satisfying certain quality thresholds.
 
 """
+
+import json
 import logging
 from pathlib import Path
 from typing import Union, List, Tuple, Dict
 
 import numpy as np
 import xarray
+import yaml
 
-from .AnalysisOptions import AnalysisOptions, AnalysisParameters
-from .analyze_data_array import analyze_data_array, ANALYSIS_DIAGNOSTIC_METRICS, COMPRESSION_RATIO_LABEL
 from enstools.compression.compressor import drop_variables
+from enstools.io import read
+from .analysis_options import AnalysisOptions, AnalysisParameters
+from .analyze_data_array import analyze_data_array, ANALYSIS_DIAGNOSTIC_METRICS, COMPRESSION_RATIO_LABEL
 
 logger = logging.getLogger("enstools.compression.analysis")
 
 
 def find_optimal_encoding(dataset: xarray.Dataset, options: AnalysisOptions):
     """
     Given a dataset, find the optimal compression parameters.
@@ -43,16 +47,16 @@
     If we are aiming for quality instead of compression ratio the same reasoning applies:
     all the provided encodings should satisfy the quality requirements, so the best one will be the one
     with the highest compression ratio.
     """
 
     if COMPRESSION_RATIO_LABEL in options.thresholds:
         return select_optimal_encoding_based_on_quality_metrics(encodings, metrics)
-    else:
-        return select_optimal_encoding_based_on_compression_ratio(encodings, metrics)
+
+    return select_optimal_encoding_based_on_compression_ratio(encodings, metrics)
 
 
 def select_optimal_encoding_based_on_compression_ratio(encodings: dict, metrics: dict) -> Tuple[Dict, Dict]:
     """
     Within the encodings provided, the one with higher compression ratio is selected.
     """
     # Unpack keys
@@ -104,22 +108,20 @@
     """
     Given a dataset and certain analysis options, find the compression parameters that fulfill the requirements for each
     combination of compressor and mode..
     :param dataset:
     :param options:
     :return:
     """
-    # Get list of variables and coordinates
-    variables = [v for v in dataset.data_vars]
-    coordinates = [v for v in dataset.coords]
-
-    compression_parameters = AnalysisParameters(options)
+    # Get lists of variables and coordinates
+    variables = list(dataset.data_vars)
+    coordinates = list(dataset.coords)
 
     # Get all possible combinations to analyze
-    combinations = compression_parameters.get_compressor_mode_combinations()
+    combinations = AnalysisParameters(options).get_compressor_mode_combinations()
 
     # Initialize dictionaries to save the results
     encodings = {}
     metrics = {}
     for combination in combinations:
         compressor, mode = combinations[combination]
         # Find optimal encoding
@@ -134,28 +136,31 @@
             # Small arrays will be losslessly compressed.
             # This number is arbitrary, a better based quantity is welcome.
             if dataset[var].size < 10000:
                 combination_encoding[var] = "lossless"
                 combination_metrics[var] = {COMPRESSION_RATIO_LABEL: 1.0}
                 continue
             if not np.issubdtype(dataset[var].dtype, np.floating):
-                logger.debug(
-                    f"Variable {var} is not a float, it is {dataset[var].dtype}. Going with lossless.")
+                logger.debug("Variable %s is not a float, it is %s. Going with lossless.", var, dataset[var].dtype)
                 combination_encoding[var] = "lossless"
                 combination_metrics[var] = {COMPRESSION_RATIO_LABEL: 1.0}
                 continue
 
             variable_encoding, variable_metrics = analyze_data_array(
                 data_array=dataset[var],
                 options=AnalysisOptions(compressor, mode, thresholds=options.thresholds)
             )
             combination_encoding[var] = variable_encoding
             combination_metrics[var] = variable_metrics
             # (dataset, variable_name, thresholds, compressor_name, mode)
-            logger.debug(f"{var} {variable_encoding}  CR:{variable_metrics[COMPRESSION_RATIO_LABEL]:.1f}")
+            logger.debug("%s %s  CR:%.1f",
+                         var,
+                         variable_encoding,
+                         variable_metrics[COMPRESSION_RATIO_LABEL],
+                         )
         encodings[combination] = combination_encoding
         metrics[combination] = combination_metrics
 
     return encodings, metrics
 
 
 def analyze_files(file_paths: Union[Path, List[Path]],
@@ -186,15 +191,14 @@
 
     print(
         f"\nAnalyzing files to determine optimal compression options for compressor {compressor!r} "
         f"with mode {mode!r} to fulfill the following constrains:\n"
         f"{constrains}\n"
     )
     print()
-    from enstools.io import read
 
     # Load dataset, possibly using a grid file
     if grid:
         dataset = read(file_paths, constant=grid)
     else:
         dataset = read(file_paths)
 
@@ -214,14 +218,25 @@
 def analyze_dataset(dataset: xarray.Dataset,
                     constrains: str = "correlation_I:5,ssim_I:2",
                     compressor: str = None,
                     mode: str = None,
                     fill_na: Union[float, bool] = False,
                     variables: List = None,
                     ):
+    """
+    Finds optimal compression parameters for a dataset to fulfill certain thresholds.
+
+    :param dataset:
+    :param constrains:
+    :param compressor:
+    :param mode:
+    :param fill_na:
+    :param variables:
+    :return:
+    """
     if variables is not None:
         dataset = drop_variables(dataset, variables)
 
     if fill_na is not False:
         dataset = dataset.fillna(fill_na)
 
     options = AnalysisOptions(compressor=compressor, mode=mode, constrains=constrains)
@@ -233,27 +248,26 @@
     Output the encoding dictionary to a file or to the stdout.
     :param encoding:
     :param output_file:
     :param file_format:
     :return:
     """
     if file_format == "json":
-        import json
         if output_file:
-            print("Compression options saved in: %s " % output_file)
-            with open(output_file, "w") as outfile:
+            output_file = Path(output_file)
+            print(f"Compression options saved in: {output_file}")
+            with output_file.open("w", encoding="utf-8") as outfile:
                 json.dump(encoding, outfile, indent=4, sort_keys=True)
         else:
             print("Compression options:")
             print(json.dumps(encoding, indent=4, sort_keys=True))
     elif file_format == "yaml":
-        import yaml
         if output_file:
             output_file = Path(output_file)
-            print("Compression options saved in: %s " % output_file)
-            with open(output_file, "w") as outfile:
+            print(f"Compression options saved in: {output_file}")
+            with output_file.open("w", encoding="utf-8") as outfile:
                 yaml.dump(encoding, outfile, sort_keys=True)
         else:
             print("Compression options:")
             print(yaml.dump(encoding, indent=4, sort_keys=True))
 
     return encoding
```

### Comparing `enstools-compression-2023.4.1/enstools/compression/cli.py` & `enstools-compression-2023.5/enstools/compression/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """
 Command Line Interface for different enstools-compression utilities
 """
+import argparse
+import sys
+from typing import List
+import glob
+from os.path import realpath
 
 # Few help messages
-compressor_help_text = """
+COMPRESSOR_HELP = """
 compress: 
 
 Tool to apply HDF5 compression filters to netCDF files. Compression specifications must follow the Compression Specification Format, more details below.
 
 Examples
 --------
 
@@ -97,19 +102,20 @@
 
 # For each possible usage (compress, analyze, ...) we will define a function to add
 # the corresponding command line arguments to the parser and another one to manage the call
 
 ###############################
 # Compressor
 def add_subparser_compressor(subparsers):
-    import argparse
-
+    """
+    Function to add the compressor subparser
+    """
     subparser = subparsers.add_parser('compress', help='Compress help',
                                       formatter_class=argparse.RawDescriptionHelpFormatter,
-                                      description=compressor_help_text)
+                                      description=COMPRESSOR_HELP)
     subparser.add_argument("files", type=expand_paths, nargs='*',
                            help="Path to file/files that will be compressed."
                                 "Multiple files and regex patterns are allowed.")
     subparser.add_argument("-o", '--output', type=str, dest="output", default=None, required=True)
 
     subparser.add_argument('--compression', type=str, dest="compression", nargs="+", default="lossless",
                            help="""
@@ -127,15 +133,19 @@
     subparser.add_argument("--fill-na", dest="fill_na", default=False,
                            help="Fill the missing values with a float.")
 
     subparser.set_defaults(which='compressor')
 
 
 def call_compressor(args):
-    from os.path import realpath
+    """
+    Function to be called with the compressor subparser
+    """
+    # pylint: disable=import-outside-toplevel
+
     # Read the output folder from the command line and assert that it exists and has write permissions.
     output = realpath(args.output)
 
     file_paths = args.files
     file_paths = sum(file_paths, [])
 
     # Compression options
@@ -163,15 +173,15 @@
     from enstools.compression.api import compress
     compress(file_paths, output, compression, nodes, variables_to_keep=variables, emulate=emulate, fill_na=fill_na)
 
 
 ###############################
 # Analyzer
 
-analyzer_help_text = """
+ANALYZE_HELP = """
 analyze: 
 
 Tool to find which compression specifications maximise the compression ratio while maintaining certain quality metrics provided by the argument **constrains**.
 
 Examples
 --------
 
@@ -203,17 +213,19 @@
     >>> "metric1:value1,metric2:value2,metric3:value3"
 
 
 """
 
 
 def add_subparser_analyzer(subparsers):
-    import argparse
+    """
+    Function to add the analyzer subparser
+    """
 
-    subparser = subparsers.add_parser('analyze', help=analyzer_help_text,
+    subparser = subparsers.add_parser('analyze', help=ANALYZE_HELP,
                                       formatter_class=argparse.RawDescriptionHelpFormatter)
 
     subparser.add_argument("--constrains", dest="constrains",
                            default="correlation_I:5,ssim_I:2", type=str,
                            help="Quality constrains that need to be fulfilled.")
 
     subparser.add_argument("--output", "-o", dest="output", default=None, type=str,
@@ -247,14 +259,19 @@
                                 "Must be a list of comma separated values: i.e. vor,temp,qv"
                                 "Default=None")
 
     subparser.set_defaults(which='analyzer')
 
 
 def call_analyzer(args):
+    """
+    Function to be called with the analyzer subparser
+    """
+    # pylint: disable=import-outside-toplevel
+
     file_paths = args.files
     grid = args.grid
     # Compression options
     constrains = args.constrains
     compressor = args.compressor
     mode = args.mode
 
@@ -288,111 +305,165 @@
         variables=variables,
     )
 
 
 ###############################
 # Find significand bits
 
-significant_bits_help_text = """
+SIGNIFICANT_HELP = """
 significand:
 
 Tool to find the ammount of significand bits in a data file following the approach described in Klöwer et al 2021 _[1].
 
 .. [1] Klöwer, M., Razinger, M., Dominguez, J.J. et al. Compressing atmospheric data into its real information content.
 Nat Comput Sci 1, 713-724 (2021). https://doi.org/10.1038/s43588-021-00156-2
 
 """
 
 
 def add_subparser_significand(subparsers):
-    import argparse
+    """
+    Function to add the significand subparser
+    """
 
-    subparser = subparsers.add_parser('significand', help=significant_bits_help_text,
+    subparser = subparsers.add_parser('significand', help=SIGNIFICANT_HELP,
                                       formatter_class=argparse.RawDescriptionHelpFormatter)
     subparser.add_argument("--output", "-o", dest="output", default=None, type=str,
                            help="Path to the file where the configuration will be saved."
                                 "If not provided will be print in the stdout.")
     subparser.add_argument("--grid", "-g", dest="grid", default=None, type=str,
                            help="Path to the file containing grid information.")
     subparser.add_argument("files", type=str, nargs="+",
                            help='List of files to compress. Multiple files and regex patterns are allowed.')
     subparser.set_defaults(which='significand')
 
 
 def call_significand(args):
+    """
+    Function to be called with the significand subparser
+    """
+    # pylint: disable=import-outside-toplevel
+
     from enstools.compression.api import analyze_file_significant_bits
     file_paths = args.files
 
     for file_path in file_paths:
         analyze_file_significant_bits(file_path)
 
 
 ###############################
 # Evaluator
-evaluate_help_text = """
+EVALUATE_HELP = """
 evaluate:
 
 Tool to quickly compare two datasets, mainly though to compare a compressed dataset with its reference.
 
 """
 
 
-def add_subsubparser(subparsers):
-    import argparse
-    subparser = subparsers.add_parser('evaluate', help=evaluate_help_text,
+def add_subparser_evaluator(subparsers):
+    """
+    Function to add the evaluator subparser
+    """
+
+    subparser = subparsers.add_parser('evaluate', help=EVALUATE_HELP,
                                       formatter_class=argparse.RawDescriptionHelpFormatter)
     subparser.add_argument("--reference", "-r", dest="reference_file", default=None, type=str,
                            help="Path to reference file. Default=%(default)s", required=True)
     subparser.add_argument("--target", "-t", dest="target_file", default=None, type=str,
                            help="Path to target file", required=True)
     subparser.add_argument("--plot", dest="plot", default=False, action='store_true',
                            help="Produce evaluation plots. Default=%(default)s")
     subparser.add_argument("-g", "--gradients", dest="gradients", default=False, action='store_true',
                            help="Compute gradients. Default=%(default)s")
     subparser.set_defaults(which='evaluator')
 
 
 def call_evaluator(args):
+    """
+    Function to be called with the evaluator subparser
+    """
+    # pylint: disable=import-outside-toplevel
+
     reference_file_path = args.reference_file
     target_file_path = args.target_file
     plot = args.plot
     gradients = args.gradients
 
     from enstools.compression.api import evaluate
     evaluate(reference_file_path, target_file_path, plot=plot, create_gradients=gradients)
 
 
 ###############################
 # Pruner
-pruner_help_text = """
+PRUNER_HELP = """
 pruner:
 
 Tool to prune a file up to a certain number of significant bits.
 
 """
 
 
 def add_subparser_pruner(subparsers):
-    import argparse
-    subparser = subparsers.add_parser('prune', help=pruner_help_text,
+    """
+    Function to add the pruner subparser
+    """
+
+    subparser = subparsers.add_parser('prune', help=PRUNER_HELP,
                                       formatter_class=argparse.RawDescriptionHelpFormatter)
     subparser.add_argument("files", type=str, nargs="+",
                            help='List of files to compress. Multiple files and regex patterns are allowed.')
     subparser.add_argument("-o", '--output', type=str, dest="output", default=None, required=True)
     subparser.set_defaults(which='pruner')
 
 
 def call_pruner(args):
+    """
+    Function to be called with the pruner subparser
+    """
+    # pylint: disable=import-outside-toplevel
     from enstools.compression.pruner import pruner
     file_paths = args.files
     output = args.output
 
     pruner(file_paths, output)
 
 
+def add_subparser_load_plugins(subparsers):
+    """
+    Function to add the load_plugins subparser
+    """
+
+    load_subparser = subparsers.add_parser('load-plugins',
+                                           help="Add the HDF5PLUGINPATH path to the environment",
+                                           formatter_class=argparse.RawDescriptionHelpFormatter)
+    load_subparser.set_defaults(which='load-plugins')
+    unload_subparser = subparsers.add_parser('unload-plugins', help="Remove the HDF5PLUGINPATH from the environment",
+                                             formatter_class=argparse.RawDescriptionHelpFormatter)
+    unload_subparser.set_defaults(which='unload-plugins')
+
+
+def call_load_plugins():
+    """
+    Function to be called with the load_plugins subparser
+    """
+    # pylint: disable=import-outside-toplevel
+    from enstools.compression.plugins import load_plugins
+    load_plugins()
+
+
+def call_unload_plugins():
+    """
+    Function to be called with the unload_plugins subparser
+    """
+    # pylint: disable=import-outside-toplevel
+    from enstools.compression.plugins import unload_plugins
+    unload_plugins()
+
+
 ###############################
 
 def add_subparsers(parser):
     """
     Add the different subparsers.
     """
 
@@ -401,36 +472,39 @@
     # Create the parser for the "compressor" command
     add_subparser_compressor(subparsers)
     # Create the parser for the "analyzer" command
     add_subparser_analyzer(subparsers)
     # Create the parser for the "significand" command
     add_subparser_significand(subparsers)
     # Create the parser for the "evaluator" command
-    add_subsubparser(subparsers)
+    add_subparser_evaluator(subparsers)
     # Create the parser for the "pruner" command
     add_subparser_pruner(subparsers)
     # To add an additional subparser, just create a function like the ones above and add the call here.
+    add_subparser_load_plugins(subparsers)
 
 
-def expand_paths(string: str):
-    import glob
-    from os.path import realpath
+def expand_paths(string: str) -> List[str]:
     """
-    Small function to expand the file paths
+    Expand paths using glob.
     """
+
     files = glob.glob(string)
     return [realpath(f) for f in files]
 
 
 ###############################
 
-def get_parser():
-    # Create parser
-    import argparse
+def get_parser() -> argparse.ArgumentParser:
+    """
+    Create a parser object and return it
+    Returns
+    -------
 
+    """
     # Create the top-level parser
     parser = argparse.ArgumentParser()
     parser.set_defaults(which=None)
 
     # Add the different subparsers.
     # If willing to add new parser, this is the function where to look at.
     add_subparsers(parser)
@@ -448,20 +522,24 @@
 
     # Parse the command line arguments
     args = parser.parse_args()
 
     # Process options according to the selected option
     if args.which is None:
         parser.print_help()
-        exit(0)
+        sys.exit(1)
     elif args.which == "compressor":
         call_compressor(args)
     elif args.which == "analyzer":
         call_analyzer(args)
     elif args.which == "significand":
         call_significand(args)
     elif args.which == "evaluator":
         call_evaluator(args)
     elif args.which == "pruner":
         call_pruner(args)
+    elif args.which == "load-plugins":
+        call_load_plugins()
+    elif args.which == "unload-plugins":
+        call_unload_plugins()
     else:
         raise NotImplementedError
```

### Comparing `enstools-compression-2023.4.1/enstools/compression/compressor.py` & `enstools-compression-2023.5/enstools/compression/compressor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,66 @@
 """
 #
 # Functions to compress netcdf/grib files from the command line.
 #
 
 """
 import logging
-import time
-from functools import partial
 from os import rename, access, W_OK
-from os.path import isfile, isdir
+from os.path import isdir
+from os.path import splitext
+from pathlib import Path
+from pprint import pprint
 from typing import Union, List
+
 import xarray
-from pathlib import Path
-from enstools.io.paths import clean_paths
+from dask.distributed import performance_report
 
 from enstools.compression.emulation import emulate_compression_on_dataset
+from enstools.core import init_cluster
+from enstools.io import read, write
+from enstools.io.file_type import get_file_type
+from enstools.io.paths import clean_paths
+from .size_metrics import compression_ratio
 
 
 def drop_variables(dataset: xarray.Dataset, variables_to_keep: List[str]) -> xarray.Dataset:
     """
     Drop all the variables that are not in list variables_to_keep.
     Keeps the coordinates.
     """
     # Drop the undesired variables and keep the coordinates
-    coordinates = [v for v in dataset.coords]
+    coordinates = list(dataset.coords)
     variables = [v for v in dataset.variables if v not in coordinates]
     variables_to_drop = [v for v in variables if v not in variables_to_keep]
     return dataset.drop_vars(variables_to_drop)
 
 
 def fix_filename(file_name: str) -> str:
+    """
+    Replace grib2 or grb file specification with .nc
+    Parameters
+    ----------
+    file_name
+
+    Returns
+    -------
+    fixed_file_name
+
+    """
     cases = [".grib2", ".grb"]
     for case in cases:
         file_name = file_name.replace(case, ".nc")
     return file_name
 
 
 def transfer(file_paths: Union[List[str], str, Path, List[Path]],
              output: Path,
              compression: str = "lossless",
-             variables_to_keep: List[str] = [],
+             variables_to_keep: List[str] = None,
              emulate: bool = False,
              fill_na: Union[float, bool] = False,
              ) -> None:
     """
     This function loops through a list of files creating delayed dask tasks to copy each one of the files while
     optionally using compression.
     If there are dask workers available the tasks will be automatically distributed when using compute.
@@ -64,15 +81,16 @@
     # Just make sure that output is a Path object
     output = Path(output).resolve()
 
     # If we have a single file, we might accept a output filename instead of an output folder.
     # Some assertions first to prevent wrong usage.
     if len(file_paths) == 0:
         raise AssertionError("file_paths can't be an empty list")
-    elif len(file_paths) == 1:
+
+    if len(file_paths) == 1:
         file_path = file_paths[0]
         new_file_path = destination_path(file_path, output) if isdir(output) else output
         transfer_file(file_path, new_file_path, compression,
                       variables_to_keep, emulate=emulate, fill_na=fill_na)
     elif len(file_paths) > 1:
         # In case of having more than one file, check that output corresponds to a directory
         assert output.is_dir(), "For multiple files, the output parameter should be a directory"
@@ -93,14 +111,32 @@
         file_paths: List[Path],
         output: Path,
         compression: str = "lossless",
         variables_to_keep: List[str] = None,
         emulate: bool = False,
         fill_na: Union[float, bool] = False
 ) -> None:
+    """
+        This function will copy multiple files while optionally applying compression.
+
+    Parameters
+    ----------
+    file_paths
+    output
+    compression
+    variables_to_keep
+    emulate
+    fill_na
+
+    Returns
+    -------
+
+    """
+    # pylint: disable=import-outside-toplevel
+
     output = Path(output)
     file_paths = clean_paths(paths=file_paths)
 
     from dask import compute
     # Create and fill the list of tasks
     tasks = []
 
@@ -148,31 +184,31 @@
 
     destination: string
             path to the new file that will be created.
 
     compression: string
             compression specification or path to json configuration file
     """
-    from enstools.io import read, write
+
     dataset = read(origin, decode_times=False)
     if variables_to_keep is not None:
         dataset = drop_variables(dataset, variables_to_keep)
 
     if fill_na is not False:
         dataset = dataset.fillna(fill_na)
-        logging.info(f"Filling missing values with {fill_na!r}")
+        logging.info("Filling missing values with %s", fill_na)
 
     # In case we are using emulate, we compress and decompress the dataset using LibPressio and output
     # the file without compression only to measure the impact compression would have.
     if emulate:
         dataset, _ = emulate_compression_on_dataset(dataset, compression)
         return write(dataset, destination, file_format="NC", compute=compute, compression=None,
                      format="NETCDF4_CLASSIC", engine="netcdf4")
-    else:
-        return write(dataset, destination, file_format="NC", compression=compression, compute=compute)
+
+    return write(dataset, destination, file_format="NC", compression=compression, compute=compute)
 
 
 def destination_path(origin_path: Path, destination_folder: Path):
     """
     Function to obtain the destination file from the source file and the destination folder.
     If the source file has GRIB format (.grb) , it will be changed to netCDF (.nc).
 
@@ -182,16 +218,14 @@
             path to the original file
 
     destination_folder : string
             path to the destination folder
 
     Returns the path to the new file that will be placed in the destination folder.
     """
-    from os.path import splitext
-    from enstools.io.file_type import get_file_type
 
     file_name = origin_path.name
 
     file_format = get_file_type(file_name, only_extension=True)
     if file_format != "NC":
         bname, _ = splitext(file_name)
         file_name = bname + ".nc"
@@ -234,30 +268,16 @@
 
     Returns
     -------
 
     """
     file_paths = clean_paths(file_paths)
     output = Path(output)
-    # In case of using automatic compression option, call here get_compression_parameters()
-    if compression == "auto":
-        from .analyzer import analyze_files
-        if output.is_dir():
-            compression_parameters_path = output / "compression_parameters.yaml"
-        else:
-            compression_parameters_path = output.parent.resolve() / "compression_parameters.yaml"
-        # By using thresholds = None we will be using the default values.
-        analyze_files(file_paths=file_paths, output_file=compression_parameters_path)
-        # Now lets continue setting compression = compression_parameters_path
-        compression = compression_parameters_path
-
     # In case of wanting to use additional nodes
     if nodes > 0:
-        from enstools.core import init_cluster
-        from dask.distributed import performance_report
         with init_cluster(nodes, extend=True) as client:
             client.wait_for_workers(nodes)
             client.get_versions(check=True)
             with performance_report(filename="dask-report.html"):
                 # Transfer will copy the files from its origin path to the output folder,
                 # using read and write functions from enstools
                 transfer(file_paths,
@@ -274,25 +294,35 @@
         transfer(file_paths, output, compression,
                  variables_to_keep=variables_to_keep, emulate=emulate, fill_na=fill_na)
 
     if show_compression_ratios:
         check_compression_ratios(file_paths, output)
 
 
-def check_compression_ratios(file_paths: List[Path], output: Path):
+def check_compression_ratios(file_paths: List[Path], output: Path) -> None:
+    """
+    Utility to compute and print the compression ratios.
+    Parameters
+    ----------
+    file_paths
+    output
+
+    Returns
+    -------
+
+    """
     # Compute compression ratios
-    from .size_metrics import compression_ratio
-    from os.path import join, basename
-    from pprint import pprint
     compression_ratios = {}
 
     for file_path in file_paths:
         file_name = file_path.name
         file_name = fix_filename(file_name)
         if output.is_dir():
             new_file_path = output / file_name
         elif output.is_file():
             new_file_path = output
-        CR = compression_ratio(file_path.as_posix(), new_file_path.as_posix())
-        compression_ratios[file_name] = CR
+        else:
+            raise AssertionError(f"Output {output} is neither a file nor a folder!")
+        file_compression_ratio = compression_ratio(file_path.as_posix(), new_file_path.as_posix())
+        compression_ratios[file_name] = file_compression_ratio
     print("Compression ratios after compression:")
     pprint(compression_ratios)
```

### Comparing `enstools-compression-2023.4.1/enstools/compression/emulators/EmulatorClass.py` & `enstools-compression-2023.5/enstools/compression/emulators/emulator_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     and has a method to compress_and_decompress the data.
 
     Its is useful to evaluate the errors that are introduced by the compression.
     """
     @abstractmethod
     def __init__(self, specification: Encoding, uncompressed_data: np.ndarray):
         """Init method requires certain parameters"""
-        ...
 
     @abstractmethod
     def compress_and_decompress(self, uncompressed_data: np.array) -> np.array:
         """
         Gets a numpy array and returns the same array after compression and deflation .
         Parameters
         ----------
```

### Comparing `enstools-compression-2023.4.1/enstools/compression/emulators/FiltersEmulator.py` & `enstools-compression-2023.5/enstools/compression/emulators/filters_emulator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,117 @@
 """
 Definition of the class FilterEmulator: an Emulator that uses the hdf5 filters.
 """
 
 import io
-from typing import Union
 
 import numpy as np
+import h5py
 
-from .EmulatorClass import Emulator
-from enstools.io import write, read
 from enstools.core.tempdir import TempDir
-from pathlib import Path
-from enstools.encoding.api import VariableEncoding
 from enstools.encoding.variable_encoding import Encoding
-from enstools.compression.size_metrics import file_size
+from .emulator_class import Emulator
+
 
-import h5py
 
 # TODO: Patch to make Tempdir usable as a context manager. Shouldn't be necessary in future releases of enstools.
 
 
 if not hasattr(TempDir, "__enter__"):
+    # pylint: disable=unused-argument
     def __enter__(self, parentdir=None, check_free_space=False, cleanup=True):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.cleanup()
 
     TempDir.__enter__ = __enter__
     TempDir.__exit__ = __exit__
 
 
 class FilterEmulator(Emulator):
     """
-    Use the filters to compress the data
+    Emulator class that relies on the hdf5 filters to compress the data using a IO file object to do that in memory.
     """
 
     def __init__(self, specification: Encoding, uncompressed_data: np.ndarray):
+        """
+        Initialize the FilterEmulator.
+
+        Args:
+            specification (Encoding): The encoding specification.
+            uncompressed_data (np.ndarray): The uncompressed data.
+        """
+
         self.compression = specification
 
         self._compression_ratio = None
 
     def compress(self, uncompressed_data: np.ndarray) -> np.ndarray:
+        """
+        FilterEmulator doesn't have the compress method implemented.
+        Use directly compress_and_decompress.
+
+        """
+
         raise NotImplementedError
 
     def decompress(self, compressed_data: np.ndarray) -> np.ndarray:
+        """
+        FilterEmulator doesn't have the decompress method implemented.
+        Use directly compress_and_decompress.
+
+        """
+
         raise NotImplementedError
 
     def compress_and_decompress(self, uncompressed_data: np.ndarray) -> np.ndarray:
+        """
+        Compress and decompress the data.
+
+        Args:
+            uncompressed_data (np.ndarray): The uncompressed data.
+
+        Returns:
+            np.ndarray: The decompressed data.
+        """
+
         # Create a temporary directory in the system memory
-        
+
         dummy_var = "tmp"
 
         # Calculate uncompressed size
         uncompressed_size = uncompressed_data.dtype.itemsize * uncompressed_data.size
 
         # If the key "chunksizes" is inside the encoding, we need to rename it.
         encoding = dict(self.compression)
         if "chunksizes" in encoding:
             encoding["chunks"] = encoding.pop("chunksizes")
 
         # Initialize file object
         with io.BytesIO() as bio:
-        
+
             # Compress data
-            with h5py.File(bio, mode='w') as f:
-                f.create_dataset(dummy_var, data=uncompressed_data, **encoding)
-            
+            with h5py.File(bio, mode='w') as temporary_file:
+                temporary_file.create_dataset(dummy_var, data=uncompressed_data, **encoding)
+
             # Get compressed file
             compressed_size = bio.getbuffer().nbytes
 
             # Decompress data
-            with h5py.File(bio, mode="r") as f:
-                recovered_data = f[dummy_var][()]
+            with h5py.File(bio, mode="r") as temporary_file:
+                recovered_data = temporary_file[dummy_var][()]
 
             # Save compression ratio
             self._compression_ratio = uncompressed_size / compressed_size
 
             # Return the recovered data
             return recovered_data
 
     def compression_ratio(self):
+        """
+        Get the compression ratio.
+
+        Returns:
+            float: The compression ratio.
+        """
         return self._compression_ratio
```

### Comparing `enstools-compression-2023.4.1/enstools/compression/emulators/LibpressioEmulator.py` & `enstools-compression-2023.5/enstools/compression/emulators/zfp_emulator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,96 @@
 """
-Definition of the class LibpressioEmulator: an Emulator that uses Libpressio.
+Definition of the class ZFPEmulator: an Emulator that uses ZFP.
+Can only work with the ZFP compressor.
 """
-
+from sys import getsizeof
 
 import numpy as np
+import zfpy
 
-from enstools.compression.emulators.EmulatorClass import Emulator
+from enstools.compression.emulators.emulator_class import Emulator
 from enstools.core.errors import EnstoolsError
+
+
 from enstools.encoding.variable_encoding import Encoding, LossyEncoding
 
 
-def libpressio_is_available():
+class ZFPEmulator(Emulator):
     """
-    Check if libpressio is available.
+    Emulator class that relies on the zfpy library to compress the data.
+    Only usable for zfp compressor.
     """
-    try:
-        from libpressio import PressioCompressor
-        return True
-    except ModuleNotFoundError:
-        return False
-
-
-class LibpressioEmulator(Emulator):
-    def __init__(self, specification: Encoding, uncompressed_data: np.ndarray = None):
-        from libpressio import PressioCompressor
+    # pylint: disable=c-extension-no-member
+    def __init__(self, specification: Encoding, uncompressed_data: np.ndarray):
         if not isinstance(specification, LossyEncoding):
-            raise EnstoolsError("Our current implementation of Libpressio only covers lossy compressors.")
+            raise EnstoolsError("Our current implementation of ZFPEmulator only covers the lossy compressor ZFP.")
+
         compressor_name = specification.compressor
         mode = specification.mode
         parameter = specification.parameter
-        self._config = compressor_configuration(
-            compressor_name, mode, parameter, uncompressed_data)
-        self.compressor = PressioCompressor.from_config(self._config)
+
+        if compressor_name != "zfp":
+            raise EnstoolsError(f"Trying to use ZFP analysis compressor for compressor {compressor_name}")
+
+        if mode == "accuracy":
+            mode = "tolerance"
+        self.parameters = {mode: parameter}
+        self._compression_ratio = None
 
     def compress(self, uncompressed_data: np.ndarray) -> np.ndarray:
-        self._shape = uncompressed_data.shape
-        self._dtype = uncompressed_data.dtype
-        return self.compressor.encode(uncompressed_data)
+        """
+        Compress the uncompressed data.
+
+        Args:
+            uncompressed_data (np.ndarray): The uncompressed data.
+
+        Returns:
+            np.ndarray: The compressed data.
+        """
+
+        # Compress the data
+        compressed_data = zfpy.compress_numpy(uncompressed_data, **self.parameters)
+
+        # Get compression ratio
+        compressed_size = getsizeof(compressed_data)
+        original_size = uncompressed_data.size * uncompressed_data.itemsize
+        compression_ratio = original_size / compressed_size
+        # Store compression ratio
+        self._compression_ratio = compression_ratio
+        # Return compressed data
+        return compressed_data
 
     def decompress(self, compressed_data: np.ndarray) -> np.ndarray:
-        decompressed = np.zeros(shape=self._shape, dtype=self._dtype)
-        decompressed = self.compressor.decode(compressed_data, decompressed)
-        return decompressed
+        """
+        Decompress the compressed data.
+
+        Args:
+            compressed_data (np.ndarray): The compressed data.
+
+        Returns:
+            np.ndarray: The decompressed data.
+        """
+
+        return zfpy.decompress_numpy(compressed_data)
 
     def compress_and_decompress(self, uncompressed_data: np.ndarray) -> np.ndarray:
+        """
+        Compress and decompress the data.
+
+        Args:
+            uncompressed_data (np.ndarray): The uncompressed data.
+
+        Returns:
+            np.ndarray: The decompressed data.
+        """
+
         compressed_data = self.compress(uncompressed_data=uncompressed_data)
         return self.decompress(compressed_data=compressed_data)
 
     def compression_ratio(self):
-        metrics = self.compressor.get_metrics()
-        return metrics['size:compression_ratio']
-
+        """
+        Get the compression ratio.
 
-def compressor_configuration(compressor: str, mode: str, parameter: float,
-                             data: np.ndarray):
-    if compressor == "sz":
-        compressor_config = {
-            "sz:error_bound_mode_str": mode,
-            "sz:abs_err_bound": parameter,
-            "sz:rel_err_bound": parameter,
-            "sz:pw_rel_err_bound": parameter,
-            "sz:metric": "size",
-        }
-    elif compressor == "zfp":
-        compressor_config = {
-            f"zfp:{mode}": parameter,
-            "zfp:type": 3 if data.dtype == np.float32 else 4,
-            "zfp:dims": len(data.shape),
-            "zfp:wra": 0,
-            "zfp:execution_name": "serial",
-            "zfp:metric": "size",
-        }
-    else:
-        raise NotImplementedError(
-            f"{compressor} {mode}")
-    return {
-        "compressor_id": compressor,
-        "compressor_config": compressor_config,
-    }
+        Returns:
+            float: The compression ratio.
+        """
+        return self._compression_ratio
```

### Comparing `enstools-compression-2023.4.1/enstools/compression/evaluator.py` & `enstools-compression-2023.5/enstools/compression/evaluator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 """
 #
 # Functions to evaluate differences in netcdf/grib files that should represent the same data.
 #
 
 """
-from enstools.compression.metrics import DataArrayMetrics, DatasetMetrics
-
-
-class bcolors:
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKCYAN = '\033[96m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
+import warnings as _warnings
 
+from enstools.compression.metrics import DataArrayMetrics, DatasetMetrics
 
-v_char = u'\u2713'
+# Some hardcoded ASCII characters to format the output
+HEADER = '\033[95m'
+OKBLUE = '\033[94m'
+OKCYAN = '\033[96m'
+OKGREEN = '\033[92m'
+WARNING = '\033[93m'
+FAIL = '\033[91m'
+ENDC = '\033[0m'
+BOLD = '\033[1m'
+UNDERLINE = '\033[4m'
+V_CHAR = '\u2713'
 
 
 def print_green(text: str):
-    print(f"{bcolors.OKGREEN}{text}{bcolors.ENDC}")
+    """Prints the given text in green color.
+
+    Args:
+        text (str): The text to be printed in green color.
+    """
+    print(f"{OKGREEN}{text}{ENDC}")
 
 
 def print_red(text: str):
-    print(f"{bcolors.FAIL}{text}{bcolors.ENDC}")
+    """Prints the given text in red color.
+
+    Args:
+        text (str): The text to be printed in red color.
+    """
+    print(f"{FAIL}{text}{ENDC}")
 
 
-def evaluate(reference_path: str, target_path: str, plot: bool = False, create_gradients=False):
+def evaluate(reference_path: str, target_path: str, plot: bool = False, create_gradients: bool = False):
     """
     The purpose of this routine is to obtain some metrics and plots on how similar are two datasets.
     """
 
     file_comparison = DatasetMetrics(reference_path, target_path)
 
     if create_gradients:
@@ -49,43 +58,43 @@
     # As a tentative idea, we can rise some warnings in case some metrics are below certain thresholds:
     # These thresholds could be:
     #   ssim_I < 3
     #   correlation_I < 4
     #   nrmse_I < 2
 
     def checks(metrics: DataArrayMetrics):
-        import warnings as _warnings
+
         thresholds = {
             "ssim_I": 3,
             "correlation_I": 4,
             "nrmse_I": 2,
             # "max_rel_diff": 10000000,
             "ks_I": 2,
         }
         for key, value in thresholds.items():
             with _warnings.catch_warnings():
                 _warnings.simplefilter("ignore")
                 if any(metrics[key] < value):
-                    yield f"{bcolors.BOLD}{key}{bcolors.ENDC} index is low: {metrics[key].max().values:.1f}."
+                    yield f"{BOLD}{key}{ENDC} index is low: {metrics[key].max().values:.1f}."
 
     warnings = {}
     for variable in variables:
         warnings[variable] = list(checks(file_comparison[variable]))
 
     for variable in variables:
         if warnings[variable]:
             print_red(f"{variable} X")
             for warning in warnings[variable]:
                 print(f"\t{warning}")
         else:
-            print_green(f"{variable} {v_char}")
+            print_green(f"{variable} {V_CHAR}")
 
     print("\nSUMMARY:")
-    num_variables_with_warnings = sum([1 if len(warnings[v]) > 0 else 0 for v in variables])
+    num_variables_with_warnings = sum(1 if len(warnings[v]) > 0 else 0 for v in variables)
     if not num_variables_with_warnings:
-        print_green(f"Any variable has warnings!")
+        print_green("Any variable has warnings!")
     else:
         print(f"{num_variables_with_warnings}/{len(variables)}  variables have warnings.\n\n")
 
     # Produce visual reports
     if plot:
         file_comparison.make_plots()
```

### Comparing `enstools-compression-2023.4.1/enstools/compression/metrics.py` & `enstools-compression-2023.5/enstools/compression/metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,70 @@
+"""
+This module provides tools to compute metrics on two datasets, typically a reference dataset
+and a target dataset, where both datasets have the same variables and dimensions.
+"""
+
+from inspect import getmembers, isfunction, signature
+from os import makedirs
+from os.path import isdir, join
 from os.path import isfile
 from typing import Callable, Union
-from enstools.core.errors import EnstoolsError
 
 import numpy as np
 import xarray
 
+import enstools.scores
+from enstools.core.errors import EnstoolsError
 from enstools.io import read
 
 
 def get_matching_scores(arguments: list) -> dict:
     """
     Returns a dictionary of functions that match with the provided arguments.
+
+    Args:
+        arguments (list): A list of argument names to match against function signatures.
+
+    Returns:
+        dict: A dictionary with function names as keys and function objects as values.
     """
-    import enstools.scores
-    from inspect import getmembers, isfunction, signature
     functions_list = getmembers(enstools.scores, isfunction)
 
     def check_signature(function: Callable):
         sig = signature(function)
-        return all([arg in sig.parameters for arg in arguments])
+        return all(arg in sig.parameters for arg in arguments)
 
     # Keep only the functions that match the desired
     return {name: fun for name, fun in functions_list if check_signature(fun)}
 
 
 # Workaround to update the list of available metrics when the metrics are used,
 # not only when the module is imported.
-class AvailableMetrics:
-    @property
-    def get(self):
-        return get_matching_scores(arguments=["reference", "target"])
 
-available_metrics = AvailableMetrics()
+def get_available_metrics() -> dict:
+    """
+    A function to get the list of available metrics and update it when needed.
+    """
+    return get_matching_scores(arguments=["reference", "target"])
 
 
 class DataArrayMetrics:
     """
-    First object oriented approach to avoid redundant computation of metrics. (i.e. don't compute mse several times)
+    First object-oriented approach to avoid redundant computation of metrics
+    (i.e., don't compute MSE several times).
     """
+
     difference: np.ndarray
     available_metrics: list
 
     def __init__(self, reference: Union[xarray.DataArray, np.ndarray],
                  target: Union[xarray.DataArray, np.ndarray]) -> None:
+        """
+        Initialize a new DataArrayMetrics object.
+        """
         # Setting reference and reference_values  depending on the type of the input
         if isinstance(reference, np.ndarray):
             self.reference = xarray.DataArray(reference)
         else:
             self.reference = reference
 
         if isinstance(target, np.ndarray):
@@ -57,121 +75,131 @@
         # If the inputs have NaNs, replace them with a fill value
         self.fix_nan()
 
         # Initialize an empty dictionary for metrics
         self.metric_values = {}
 
         # Add the list of available metrics from metric_definitions
-        self.available_metrics = list(available_metrics.get.keys())
+        self.available_metrics = list(get_available_metrics().keys())
 
     def __getitem__(self, name: str) -> xarray.DataArray:
+        """
+        Return the metric value if already computed or compute and return the metric value.
+        """
         # Look if the metric has already been computed.
         # If its true, just return it, otherwise compute it and then return it.
         if name not in self.metric_values:
             self.metric_values[name] = self.compute_metric(name)
         return self.metric_values[name]
 
-    def fix_nan(self):
-        # FIXME: That looks a bit dangerous.
+    def fix_nan(self, fill_value: float = -1000):
+        """
+        Replace NaNs in the reference and target arrays with a fill value.
+        """
         # Replace NaNs with a fill value.
-        fill_value = -10000.
         if np.isnan(self.reference.values).any():
             self.reference.values[np.isnan(self.reference.values)] = fill_value
         if np.isnan(self.target.values).any():
             self.target.values[np.isnan(self.target.values)] = fill_value
 
     def compute_metric(self, method: str) -> xarray.DataArray:
+        """
+        Compute the specified metric for the reference and target arrays.
+        """
         if method not in self.available_metrics:
             raise EnstoolsError(f"Metric {method!r} not available.")
-        return available_metrics.get[method](self.reference, self.target)
+        return get_available_metrics()[method](self.reference, self.target)
 
     def plot_summary(self, output_folder: str = "report"):
-        # TODO: This is not the proper place to put this code. Move it somewhere else.
+        # pylint: disable=import-outside-toplevel
+        """
+        Generate a summary plot for the reference, target, and their differences.
+        """
         import matplotlib.pyplot as plt
         import matplotlib as mpl
 
-        from os.path import isdir, join
-        from os import makedirs
-
-        # Get dimensions  
+        # TODO: This is not the proper place to put this code. Move it somewhere else.
+        # Get dimensions
         shape = self.reference.shape
         # Get variable name from DataArray object
         variable_name = self.reference.name
 
         if len(shape) == 4:
-            y, z, x, y = shape
-            sl = (0, int(z / 2), slice(None), slice(None))
+            _, z_dim, _, _ = shape
+            slice_indices = (0, int(z_dim / 2), slice(None), slice(None))
         elif len(shape) == 3:
-            sl = 0, slice(None), slice(None)
+            slice_indices = 0, slice(None), slice(None)
         elif len(shape) == 2:
-            sl = slice(None), slice(None)
+            slice_indices = slice(None), slice(None)
         elif len(shape) == 1:
             return
         else:
             raise NotImplementedError
 
-        plot_num = 4
-        reference_data = self.reference[sl]
-        target_data = self.target[sl]
+        reference_data = self.reference[slice_indices]
+        target_data = self.target[slice_indices]
 
-        var_range = np.max(reference_data)-np.min(reference_data)
+        var_range = np.max(reference_data) - np.min(reference_data)
 
         # Prepare a plot of an intermediate level
         plt.figure(figsize=(9, 9))
 
         # Plot reference
-        plt.subplot(int(f"{plot_num}11"))
+        plt.subplot(int("411"))
         plt.imshow(reference_data)
         plt.colorbar()
         # Plot comparison target
-        plt.subplot(int(f"{plot_num}12"))
+        plt.subplot(int("412"))
         plt.imshow(target_data)
         plt.colorbar()
 
         # Plot differences
-        plt.subplot(int(f"{plot_num}13"))
+        plt.subplot(int("413"))
         color_levels = 7
         cmap = plt.cm.seismic  # define the colormap
         # extract all colors from the colormap
         cmaplist = [cmap(i) for i in range(cmap.N)]
         # Generate new colormap with only few levels
         cmap = mpl.colors.LinearSegmentedColormap.from_list('Custom cmap', cmaplist, color_levels)
-        difference = self.target[sl]-self.reference[sl]
-        _min = np.min(difference)
-        _max = np.max(difference)
-        __ = max(abs(_min), _max)
-        factor = var_range / __
-        vmin = -__
-        vmax = __
-        # vmin =-iqr/10
-        # vmax = iqr/10
+        difference = self.target[slice_indices] - self.reference[slice_indices]
+        max_abs_diff = max(abs(np.min(difference)), np.max(difference))
+        factor = var_range / max_abs_diff
+        vmin = -max_abs_diff
+        vmax = max_abs_diff
         plt.imshow(difference, vmin=vmin, vmax=vmax, cmap=cmap)
         plt.title(f"The difference range is {factor:.1f} smaller than the InterQuartileRange")
         cbar = plt.colorbar()
         cbar.set_ticks(np.linspace(vmin, vmax, color_levels + 1))
 
         # Put something related with the metrics
         fig = plt.gcf()
-        ax = fig.add_subplot(414, polar=True)
+        axis = fig.add_subplot(414, polar=True)
 
         selected_metrics = ["correlation_I", "ssim_I", "nrmse_I"]
         selected_values = np.array([self[m] for m in selected_metrics])
-        make_radar_chart(variable_name, selected_metrics, selected_values, ax)
+        make_radar_chart(variable_name, selected_metrics, selected_values, axis)
         if not isdir(output_folder):
             makedirs(output_folder)
         plt.tight_layout()
         plt.savefig(join(output_folder, f"report_{variable_name}.png"))
         plt.close("all")
 
     def __repr__(self):
         return f"DataArray Metrics (id:{id(self)}) Variable:{self.reference.name}"
 
 
 class DatasetMetrics:
+    """
+    A class for computing metrics and generating plots for given reference and target datasets.
+    """
+
     def __init__(self, reference: Union[str, xarray.Dataset], target: Union[str, xarray.Dataset]) -> None:
+        """
+        Initialize a new DatasetMetrics object.
+        """
         # Check that files exist and save them
 
         if not isinstance(reference, xarray.Dataset):
             assert isfile(reference), f"Path {reference} its not a valid file."
 
             self.reference_path = reference
 
@@ -188,63 +216,71 @@
 
             # Read files
             self.target = read(self.target_path)
         else:
             self.target = target
 
         # Get variables
-        self.coords = [v for v in self.reference.coords]
+        self.coords = list(self.reference.coords)
         self.variables = [v for v in self.reference.variables if v not in self.coords]
 
         # Consistency check
         self.check_consistency()
 
         # Initialize metrics
         self.metrics = {}
         self.initialize_metrics()
 
     def check_consistency(self) -> None:
+        """
+        Check if the reference and target datasets are consistent.
+        """
         # Check that files are meant to represent the same things
         assert set(self.reference.variables) == set(self.target.variables)
         assert set(self.reference.coords) == set(self.target.coords)
 
     def initialize_metrics(self) -> None:
+        """
+        Initialize DataArrayMetrics objects for each variable in the datasets.
+        """
         for variable in self.variables:
             self.metrics[variable] = DataArrayMetrics(self.reference[variable], self.target[variable])
-        pass
 
     def __getitem__(self, name: str) -> DataArrayMetrics:
         assert name in self.variables, f"The provided variable name {name} does not exist in this dataset."
         return self.metrics[name]
 
     def make_plots(self):
+        """
+        Generate plots for all variables in the datasets.
+        """
         print("Producing plots:")
         for index, variable in enumerate(self.variables):
             print(f"\r{index + 1}/{len(self.variables)} {variable:30} ", end="")
             self[variable].plot_summary()
         print("\rPlots done!" + 30 * " ")
 
     def create_gradients(self):
         """
-        Create first order gradients
+        Create first-order gradients for all variables in the datasets.
         """
         for variable in self.variables:
             ref_grad = array_gradient(self[variable].reference)
             target_grad = array_gradient(self[variable].target)
             if ref_grad is not None:
                 self.reference[ref_grad.name] = ref_grad
                 self.target[target_grad.name] = target_grad
 
         # Update list of variables to include the gradients
         self.variables = [v for v in self.reference.variables if v not in self.reference.coords]
         self.initialize_metrics()
 
     def create_second_order_gradients(self):
         """
-        Create first order gradients
+        Create second-order gradients for all gradient variables in the datasets.
         """
         for variable in [v for v in self.variables if v.count("_gradient")]:
             ref_grad = array_gradient(self[variable].reference)
             target_grad = array_gradient(self[variable].target)
             ref_grad.name = ref_grad.name.replace("_gradient" * 2, "_gradient_O2")  # type: ignore
             target_grad.name = target_grad.name.replace("_gradient" * 2, "_gradient_O2")  # type: ignore
             if ref_grad is not None:
@@ -256,41 +292,43 @@
         self.initialize_metrics()
 
     def __repr__(self):
         return f"Dataset Metrics (id:{id(self)}) Variables:" \
                f"{[v for v in self.reference.variables if v not in self.reference.coords]}"
 
 
-def make_radar_chart(name, attribute_labels, stats, ax):
+def make_radar_chart(name, attribute_labels, stats, axis):
+    # pylint: disable=import-outside-toplevel
+    """
+    Create a radar chart for the given attributes and their values.
+    """
     import matplotlib.pyplot as plt
+
     markers = [0, 3, 6, 9, 12]
     # str_markers = ["0", "3", "6", "9", "12"]
 
     labels = np.array(attribute_labels)
 
     angles = np.linspace(0, 2 * np.pi, len(labels), endpoint=False)
     stats = np.concatenate((stats, [stats[0]]))
     angles = np.concatenate((angles, [angles[0]]))
 
-    ax.plot(angles, stats, 'o-', linewidth=.5, alpha=1, markersize=5)
-    ax.fill(angles, stats, alpha=0.25)
-    ax.set_thetagrids(angles[:-1] * 180 / np.pi, labels)
+    axis.plot(angles, stats, 'o-', linewidth=.5, alpha=1, markersize=5)
+    axis.fill(angles, stats, alpha=0.25)
+    axis.set_thetagrids(angles[:-1] * 180 / np.pi, labels)
 
-    ax.plot(angles, [5, 3, 2, 5], ":", color="r", alpha=.5)
+    axis.plot(angles, [5, 3, 2, 5], ":", color="r", alpha=.5)
     plt.yticks(markers)
-    ax.set_title(name)
-    ax.grid(True)
+    axis.set_title(name)
+    axis.grid(True)
 
 
 def array_gradient(data_array: xarray.DataArray) -> Union[None, xarray.DataArray]:
     """
-    Takes one Data Array and returns the gradient.
-    In case of multidimensional data, it returns the magnitude of the gradient.
-
-    Maybe it shouldn't be in this file.
+    Calculate the gradient of a DataArray. For multidimensional data, return the magnitude of the gradient.
     """
     dimensions = len(data_array.shape)
     if dimensions == 1:
         return None
 
     gradient_axis = tuple(range(1, dimensions))
```

### Comparing `enstools-compression-2023.4.1/enstools/compression/pruner.py` & `enstools-compression-2023.5/enstools/compression/pruner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,25 @@
-import xarray
+"""
+Functions to prune numpy arrays to a certain number of significant bits.
+"""
+
+from os import access, W_OK
+from os.path import isdir
+from pathlib import Path
+from typing import Union, List
+
 import numpy as np
 import xarray
 
+from enstools.compression.compressor import destination_path
+from enstools.io import read, write
+from enstools.io.paths import clean_paths
 from .compressor import drop_variables
 from .significant_bits import get_uint_type_by_bit_length, single_bit_mask, apply_mask, \
     mask_generator
-from enstools.io.paths import clean_paths
-from typing import Union, List
-from pathlib import Path
 
 
 def prune_numpy_array(array: np.ndarray, significant_bits=0, round_to_nearest=True):
     """
     Create and apply a mask with number of ones given by the input variable significant_bits.
 
     Rounding is controlled by round_to_nearest input variable.
@@ -51,26 +59,24 @@
            significant_bit_info=None,
            variables_to_keep=None,
            ):
     """
     Apply bit prunning to a list of files.
 
     """
-    from enstools.compression.compressor import destination_path
-    from os.path import isdir
-    from os import access, W_OK
 
     file_paths = clean_paths(file_paths)
     output = Path(output).resolve()
 
     # If we have a single file, we might accept a output filename instead of an output folder.
     # Some assertions first to prevent wrong usage.
     if len(file_paths) == 0:
         raise AssertionError("file_paths can't be an empty list")
-    elif len(file_paths) == 1:
+
+    if len(file_paths) == 1:
         file_path = file_paths[0]
         new_file_path = destination_path(file_path, output) if output.is_dir() else output
         prune_file(file_path, new_file_path, significant_bit_info=significant_bit_info,
                    variables_to_keep=variables_to_keep)
     elif len(file_paths) > 1:
         # In case of having more than one file, check that output corresponds to a directory
         assert isdir(output), "For multiple files, the output parameter should be a directory"
@@ -81,22 +87,23 @@
                        variables_to_keep=variables_to_keep)
 
 
 def prune_file(file_path, destination, significant_bit_info=None, variables_to_keep=None):
     """
     Apply bit pruning to a file. 
     """
-    from enstools.io import read, write
+
     print(f"{file_path} -> {destination}")
     dataset = read(file_path)
 
     if variables_to_keep is not None:
         dataset = drop_variables(dataset, variables_to_keep)
 
     if significant_bit_info is None:
+        # pylint: disable=import-outside-toplevel
         from enstools.compression.significant_bits import analyze_file_significant_bits
         significant_bits_dictionary = analyze_file_significant_bits(file_path)
     else:
         significant_bits_dictionary = significant_bit_info
     print(significant_bits_dictionary)
     prune_dataset(dataset, significant_bits_dictionary)
```

### Comparing `enstools-compression-2023.4.1/enstools/compression/slicing.py` & `enstools-compression-2023.5/enstools/compression/slicing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 This file contains classes and methods to divide a multi dimensional slice in different parts, via selecting a
 chunk size or the number of desired parts.
 """
 
-
 import logging
 from typing import List, Tuple
 
 from itertools import product
 import numpy as np
 
 
 def split_array(array: np.ndarray, parts: int):
     """
-    Splits the given array into a specified number of parts. 
+    Splits the given array into a specified number of parts.
     The function returns a list of chunks, where each chunk is a numpy array.
 
     :param array: A numpy array to be split
     :param parts: An int, the number of parts to split the array into
     :return: A list of numpy arrays representing the chunks
     """
 
@@ -30,31 +29,37 @@
         # Check if the number of chunks generated by the current chunk size is equal to the desired number of parts
         if np.prod(
                 [shape[i] // chunk_size[i] + int(shape[i] % chunk_size[i] != 0) for i in range(len(shape))]) == parts:
             possible_chunk_sizes.append(chunk_size)
     # Sort the possible chunk sizes in ascending order of the sum of the squares of their dimensions
     possible_chunk_sizes.sort(key=lambda x: np.sum(np.array(x) ** 2))  # type: ignore
     if not possible_chunk_sizes:
-        logging.warning(f"Could not divide the domain in {parts} parts. Trying with parts={parts - 1}.")
+        logging.warning("Could not divide the domain in %d parts. Trying with parts=%d.", parts, parts - 1)
         return split_array(array=array, parts=parts - 1)
-    chunk_size = possible_chunk_sizes[0]
+    selected_chunk_size = possible_chunk_sizes[0]
 
     chunks = []
     # Get the number of chunks for the first possible chunk size
-    n_chunks = [shape[i] // chunk_size[i] + int(shape[i] % chunk_size[i] != 0) for i in range(len(shape))]
-    indexes = [range(n_chunks[i]) for i in range(len(shape))]
+    num_chunks = [shape[i] // selected_chunk_size[i] + int(shape[i] % selected_chunk_size[i] != 0) for i in
+                  range(len(shape))]
+    indexes = [range(num_chunks[i]) for i in range(len(shape))]
     # Iterate over the chunks and append the corresponding slice of the array to the chunks list
     for indx in product(*indexes):
-        sl = tuple(
-            slice(chunk_size[i] * indx[i], min(chunk_size[i] * (indx[i] + 1), shape[i])) for i in range(len(shape)))
-        chunks.append(array[sl])
+        current_slice = tuple(
+            slice(selected_chunk_size[i] * indx[i], min(selected_chunk_size[i] * (indx[i] + 1), shape[i])) for i in
+            range(len(shape)))
+        chunks.append(array[current_slice])
     return chunks
 
 
 class MultiDimensionalSlice:
+    """
+    A class representing a multi-dimensional slice.
+    """
+
     def __init__(self, indices: Tuple[int, ...], slices: Tuple[slice, ...] = (slice(0, 0, 0),)):
         """
         Initialize the MultiDimensionalSlice object with indices and slice
         :param indices: Tuple of indices
         :param slices: Tuple of slice objects representing the slice indices
         """
         self.indices = indices
@@ -68,20 +73,24 @@
 
     @property
     def size(self):
         """
         Return the size of the slice
         """
         size = 1
-        for s in self.slices:
-            size *= s.stop - s.start
+        for current_slice in self.slices:
+            size *= current_slice.stop - current_slice.start
         return size
 
 
 class MultiDimensionalSliceCollection:
+    """
+    A class representing a collection of multi-dimensional slices.
+    """
+
     def __init__(self, *, objects_array: np.ndarray = None, shape: Tuple[int, ...] = None,
                  chunk_sizes: Tuple[int, ...] = None):
         """
         Initializes the MultiDimensionalSliceCollection class.
 
         Args:
             objects_array (np.ndarray): an array of MultiDimensionalSlice objects
@@ -127,68 +136,79 @@
         chunk_size
 
         Returns
         -------
         MultiDimensionalSliceCollection
 
         """
-        cs = chunk_size
         collection_shape = tuple(
-            [shape[i] // cs[i] + int(shape[i] % cs[i] != 0) for i in range(len(shape))])
-        # Calculates the shape of the collection of chunks, by dividing the shape of the array by the size of the chunks 
-        # and adding 1 if there is a remainder 
+            shape[i] // chunk_size[i] + int(shape[i] % chunk_size[i] != 0) for i in range(len(shape)))
         objects = np.empty(collection_shape, dtype=MultiDimensionalSlice)
-        # Initializes an empty array of the same shape as the collection with the dtype of MyObject
-        n_chunks = [shape[i] // cs[i] + int(shape[i] % cs[i] != 0) for i in range(len(shape))]
-        # Calculates the number of chunks in each dimension
-        indexes = [range(n_chunks[i]) for i in range(len(shape))]
-        # Create the indexes to iterate over the collection
+        num_chunks = [shape[i] // chunk_size[i] + int(shape[i] % chunk_size[i] != 0) for i in range(len(shape))]
+        indexes = [range(num_chunks[i]) for i in range(len(shape))]
 
         for indx in product(*indexes):
-            sl = tuple(slice(cs[i] * indx[i], min(cs[i] * (indx[i] + 1), shape[i])) for i in range(len(shape)))
-            # for each index of the collection create a slice that corresponds
-            # to the portion of the array contained in the chunk
-            objects[indx] = MultiDimensionalSlice(indices=indx, slices=sl)
-            # assigns the created object to the corresponding position in the collection array
+            current_slice = tuple(
+                slice(chunk_size[i] * indx[i], min(chunk_size[i] * (indx[i] + 1), shape[i])) for i in range(len(shape)))
+            objects[indx] = MultiDimensionalSlice(indices=indx, slices=current_slice)
         self.__initialize_from_array(objects_array=objects)
 
     def __getitem__(self, args):
-        return self.objects[args]  # returns the object at the specified position of the collection array
+        return self.objects[args]
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self.collection_shape})"  # returns a string representation of the class
+        return f"{self.__class__.__name__}({self.collection_shape})"
 
     @property
     def slice(self) -> Tuple[slice, ...]:
+        """
+        Calculate the total slice that covers all the MultiDimensionalSlice objects in the collection.
+
+        Returns:
+            Tuple[slice, ...]: A tuple of slice objects representing the total slice.
+        """
+
         total_slice = tuple(slice(None) for _ in self.collection_shape)
         for obj in self.objects.flat:
-            for i, s in enumerate(obj.slices):
+            for i, current_slice in enumerate(obj.slices):
                 if total_slice[i].start is None:
-                    total_slice = total_slice[:i] + (s,) + total_slice[i + 1:]
+                    total_slice = total_slice[:i] + (current_slice,) + total_slice[i + 1:]
                 else:
-                    if s.start < total_slice[i].start:
+                    if current_slice.start < total_slice[i].start:
                         total_slice = total_slice[:i] + (
-                        slice(s.start, total_slice[i].stop, total_slice[i].step),) + total_slice[i + 1:]
-                    if s.stop > total_slice[i].stop:
+                            slice(current_slice.start, total_slice[i].stop, total_slice[i].step),) + total_slice[i + 1:]
+                    if current_slice.stop > total_slice[i].stop:
                         total_slice = total_slice[:i] + (
-                        slice(total_slice[i].start, s.stop, total_slice[i].step),) + total_slice[i + 1:]
+                            slice(total_slice[i].start, current_slice.stop, total_slice[i].step),) + total_slice[i + 1:]
         return total_slice
 
     def split(self, parts: int) -> List['MultiDimensionalSliceCollection']:
         """
-        Divide the MultiDimensionalSliceCollection into a different parts of similar size
+        Divide the MultiDimensionalSliceCollection into different parts of similar size.
 
         Args:
-            parts (int): Number of parts to divide the group
+            parts (int): Number of parts to divide the group.
 
         Returns:
-            _type_: _description_
+            list: A list of MultiDimensionalSliceCollection objects representing the divided parts.
         """
         array_parts = split_array(self.objects, parts)
         return [MultiDimensionalSliceCollection(objects_array=p) for p in array_parts]
 
     @property
     def size(self) -> int:
-        return sum([ob.size for ob in self.objects.ravel()])
+        """
+        Calculate the total size of the MultiDimensionalSliceCollection.
+
+        Returns:
+            int: The total size of the collection.
+        """
+        return sum(ob.size for ob in self.objects.ravel())
 
     def __len__(self) -> int:
+        """
+        Calculate the total number of objects in the MultiDimensionalSliceCollection.
+
+        Returns:
+            int: The total number of objects in the collection.
+        """
         return self.objects.size
```

### Comparing `enstools-compression-2023.4.1/enstools/compression/xr_accessor/accessor.py` & `enstools-compression-2023.5/enstools/compression/xr_accessor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,33 @@
+"""
+This module registers the xarray compression accessor for Datasets and DataArrays.
+After importing this module xarray datasets can use the compression methods in a convenient way, for example:
+    dataset.compression("lossy,sz,pw_rel,0.0001")
+or 
+    data_array.compression("lossy,sz,pw_rel,0.0001")
 
-from enstools.compression.emulation import emulate_compression_on_data_array, emulate_compression_on_dataset
-from enstools.encoding.api import VariableEncoding, DatasetEncoding
-from os import PathLike
-import xarray
+"""
 
-# Imports for typing
+from os import PathLike
 from typing import Union
+
 from dask import delayed
+import xarray
+
+from enstools.encoding.api import VariableEncoding, DatasetEncoding
+from enstools.compression.emulation import emulate_compression_on_data_array, emulate_compression_on_dataset
+from enstools.compression.analyzer.analysis_options import AnalysisOptions
+from enstools.compression.analyzer.analyzer import analyze_data_array, analyze_dataset
 
 
 @xarray.register_dataarray_accessor("compression")
 class EnstoolsCompressionDataArrayAccessor:
+    """
+    Enstools-compression DataArray accessor class.
+    """
     def __init__(self, xarray_obj: xarray.DataArray):
         """
         Initialize the accessor saving a reference of the data array.
 
         Parameters
         ----------
         xarray_obj: xarray.DataArray
@@ -49,36 +62,63 @@
         Parameters
         ----------
         compression: str
         in_place: bool
 
         Returns
         -------
+        xarray.DataArray
+
 
         """
         return self.emulate(compression=compression, in_place=in_place)
 
     def analyze(self,
                 constrains="correlation_I:5,ssim_I:2",
                 compressor="sz",
                 compression_mode="abs",
                 ):
-        from enstools.compression.analyzer.analyzer import analyze_data_array
-        from enstools.compression.analyzer.AnalysisOptions import AnalysisOptions
+        """
+        Apply the analysis method on the DataArray
+
+        Parameters
+        ----------
+        constrains: str
+        compressor: str
+        compression_mode: str
+
+        Returns
+        -------
+        dict
 
+        """
         options = AnalysisOptions(compressor, compression_mode, constrains=constrains)
         return analyze_data_array(self._obj, options=options)
 
     @staticmethod
     def encoding(compression: str):
+        """
+        Returns the VariableEncoding corresponding to this DataArray
+
+        Args:
+            compression (str): compression specification string
+
+        Returns:
+            VariableEncoding
+        """
         return VariableEncoding(specification=compression)
 
 
 @xarray.register_dataset_accessor("compression")
+# pylint: disable=too-few-public-methods
 class EnstoolsCompressionDatasetAccessor:
+    """
+    Enstools-compression Dataset accessor class.
+    """
+
     def __init__(self, xarray_obj: xarray.Dataset):
         """
         Initialize the accessor saving a reference of the dataset.
 
         Parameters
         ----------
         xarray_obj: xarray.Dataset
@@ -106,18 +146,40 @@
             dataset[var].attrs["compression_ratio"] = f"{_metrics['compression_ratio']:.2f}"
         return dataset
 
     def analyze(self,
                 constrains="correlation_I:5,ssim_I:2",
                 **kwargs
                 ):
-        from enstools.compression.analyzer.analyzer import analyze_dataset
+        """
+        Apply the analysis method on the Dataset
+
+        Parameters
+        ----------
+        constrains: str
+        compressor: str
+        compression_mode: str
+
+        Returns
+        -------
+        dict
+
+        """
         return analyze_dataset(dataset=self._obj, constrains=constrains, **kwargs)
 
     def encoding(self, compression: str):
+        """
+        Returns the DatasetEncoding corresponding to this DataArray
+
+        Args:
+            compression (str): compression specification string
+
+        Returns:
+            DatasetEncoding
+        """
         return DatasetEncoding(self._obj, compression=compression)
 
     def __call__(self, compression: str, in_place=False) -> xarray.Dataset:
         """
         Calling the accessor directly uses emulate method.
 
         Parameters
@@ -130,14 +192,17 @@
 
         """
         return self.emulate(compression=compression, in_place=in_place)
 
 
 @xarray.register_dataset_accessor("to_compressed_netcdf")
 class EnstoolsCompressionToCompressedNetcdf:
+    """
+    Accessor to enable the method to_compressed_netcdf to xarray Datasets
+    """
     def __init__(self, xarray_obj: xarray.Dataset):
         """
         Initialize the accessor saving a reference of the dataset.
 
         Parameters
         ----------
         xarray_obj: xarray.Dataset
```

### Comparing `enstools-compression-2023.4.1/enstools_compression.egg-info/PKG-INFO` & `enstools-compression-2023.5/enstools_compression.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstools-compression
-Version: 2023.4.1
+Version: 2023.5
 Home-page: https://github.com/wavestoweather/enstools-compression
 Author: Oriol Tintó
 Author-email: oriol.tinto@lmu.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enstools-compression [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-compression.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `enstools-compression-2023.4.1/enstools_compression.egg-info/SOURCES.txt` & `enstools-compression-2023.5/enstools_compression.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 enstools/compression/api.py
 enstools/compression/cli.py
 enstools/compression/compressor.py
 enstools/compression/emulation.py
 enstools/compression/evaluator.py
 enstools/compression/h5netcdf_compressor.py
 enstools/compression/metrics.py
+enstools/compression/plugins.py
 enstools/compression/pruner.py
 enstools/compression/significant_bits.py
 enstools/compression/size_metrics.py
 enstools/compression/slicing.py
-enstools/compression/analyzer/AnalysisOptions.py
+enstools/compression/xr_accessor.py
 enstools/compression/analyzer/__init__.py
+enstools/compression/analyzer/analysis_options.py
 enstools/compression/analyzer/analyze_data_array.py
 enstools/compression/analyzer/analyzer.py
 enstools/compression/analyzer/analyzer_utils.py
-enstools/compression/emulators/EmulatorClass.py
-enstools/compression/emulators/FiltersEmulator.py
-enstools/compression/emulators/LibpressioEmulator.py
-enstools/compression/emulators/ZFPEmulator.py
 enstools/compression/emulators/__init__.py
-enstools/compression/xr_accessor/__init__.py
-enstools/compression/xr_accessor/accessor.py
+enstools/compression/emulators/emulator_class.py
+enstools/compression/emulators/filters_emulator.py
+enstools/compression/emulators/libpressio_emulator.py
+enstools/compression/emulators/zfp_emulator.py
 enstools_compression.egg-info/PKG-INFO
 enstools_compression.egg-info/SOURCES.txt
 enstools_compression.egg-info/dependency_links.txt
 enstools_compression.egg-info/entry_points.txt
 enstools_compression.egg-info/requires.txt
 enstools_compression.egg-info/top_level.txt
```

### Comparing `enstools-compression-2023.4.1/setup.py` & `enstools-compression-2023.5/setup.py`

 * *Files identical despite different names*

