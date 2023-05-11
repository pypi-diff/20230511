# Comparing `tmp/sunpy-soar-1.7.tar.gz` & `tmp/sunpy-soar-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunpy-soar-1.7.tar", last modified: Fri Apr 14 15:22:37 2023, max compression
+gzip compressed data, was "sunpy-soar-1.8.tar", last modified: Thu May 11 11:28:01 2023, max compression
```

## Comparing `sunpy-soar-1.7.tar` & `sunpy-soar-1.8.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.397114 sunpy-soar-1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-14 15:22:16.000000 sunpy-soar-1.7/.github/workflows/python-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-14 15:22:16.000000 sunpy-soar-1.7/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-14 15:22:16.000000 sunpy-soar-1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-14 15:22:16.000000 sunpy-soar-1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-14 15:22:16.000000 sunpy-soar-1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-14 15:22:37.401114 sunpy-soar-1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-14 15:22:16.000000 sunpy-soar-1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-14 15:22:16.000000 sunpy-soar-1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-14 15:22:37.405114 sunpy-soar-1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/sunpy_soar/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/sunpy_soar/data/
--rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/data/attrs.json
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/data/instrument_attrs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/sunpy_soar/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-14 15:22:16.000000 sunpy-soar-1.7/sunpy_soar/tests/test_sunpy_soar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/sunpy_soar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-14 15:22:37.000000 sunpy-soar-1.7/sunpy_soar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-14 15:22:37.000000 sunpy-soar-1.7/sunpy_soar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:22:37.000000 sunpy-soar-1.7/sunpy_soar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:22:37.000000 sunpy-soar-1.7/sunpy_soar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 15:22:37.000000 sunpy-soar-1.7/sunpy_soar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 15:22:37.000000 sunpy-soar-1.7/sunpy_soar.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:22:37.401114 sunpy-soar-1.7/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-14 15:22:16.000000 sunpy-soar-1.7/tools/update_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:28:01.488172 sunpy-soar-1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:28:01.476172 sunpy-soar-1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:28:01.484172 sunpy-soar-1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-11 11:27:38.000000 sunpy-soar-1.8/.github/workflows/python-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-11 11:27:38.000000 sunpy-soar-1.8/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-11 11:27:38.000000 sunpy-soar-1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-11 11:27:38.000000 sunpy-soar-1.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-11 11:27:38.000000 sunpy-soar-1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-11 11:28:01.488172 sunpy-soar-1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-11 11:27:38.000000 sunpy-soar-1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-11 11:27:38.000000 sunpy-soar-1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-11 11:28:01.488172 sunpy-soar-1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:28:01.484172 sunpy-soar-1.8/sunpy_soar/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-11 11:27:38.000000 sunpy-soar-1.8/sunpy_soar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-11 11:27:38.000000 sunpy-soar-1.8/sunpy_soar/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-11 11:27:38.000000 sunpy-soar-1.8/sunpy_soar/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:28:01.488172 sunpy-soar-1.8/sunpy_soar/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-05-11 11:27:38.000000 sunpy-soar-1.8/sunpy_soar/data/attrs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-11 11:27:38.000000 sunpy-soar-1.8/sunpy_soar/data/instrument_attrs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-11 11:27:38.000000 sunpy-soar-1.8/sunpy_soar/data/soop_attrs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:28:01.488172 sunpy-soar-1.8/sunpy_soar/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:27:38.000000 sunpy-soar-1.8/sunpy_soar/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-11 11:27:38.000000 sunpy-soar-1.8/sunpy_soar/tests/test_sunpy_soar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:28:01.484172 sunpy-soar-1.8/sunpy_soar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-11 11:28:01.000000 sunpy-soar-1.8/sunpy_soar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-11 11:28:01.000000 sunpy-soar-1.8/sunpy_soar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:28:01.000000 sunpy-soar-1.8/sunpy_soar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:28:01.000000 sunpy-soar-1.8/sunpy_soar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 11:28:01.000000 sunpy-soar-1.8/sunpy_soar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 11:28:01.000000 sunpy-soar-1.8/sunpy_soar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:28:01.488172 sunpy-soar-1.8/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-11 11:27:38.000000 sunpy-soar-1.8/tools/update_data.py
```

### Comparing `sunpy-soar-1.7/.github/workflows/python-release.yml` & `sunpy-soar-1.8/.github/workflows/python-release.yml`

 * *Files identical despite different names*

### Comparing `sunpy-soar-1.7/.github/workflows/python-test.yml` & `sunpy-soar-1.8/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `sunpy-soar-1.7/.pre-commit-config.yaml` & `sunpy-soar-1.8/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
           [
             "--count",
             "--select",
             "E901,E902,F822,F823",
           ]
         exclude: ".*(.fits|.fts|.fit|.header|.txt|tca.*|extern.*|.rst|.md|cm/__init__.py|sunpy/extern|sunpy/visualization/colormaps/color_tables.py)$"
   - repo: https://github.com/PyCQA/autoflake
-    rev: v2.0.2
+    rev: v2.1.1
     hooks:
       - id: autoflake
         args:
           [
             "--in-place",
             "--remove-all-unused-imports",
             "--remove-unused-variable",
```

### Comparing `sunpy-soar-1.7/LICENSE` & `sunpy-soar-1.8/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021 David Stansby All rights reserved.
+Copyright (c) 2021-2023 David Stansby All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
     Redistributions of source code must retain the above copyright notice,
     this list of conditions and the following disclaimer.
```

### Comparing `sunpy-soar-1.7/PKG-INFO` & `sunpy-soar-1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpy-soar
-Version: 1.7
+Version: 1.8
 Summary: A sunpy plugin for accessing data in the Solar Orbiter Archive (SOAR).
 Home-page: 
 Author: David Stansby
 Author-email: d.stansby@ucl.ac.uk
 License: BSD-2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Provides-Extra: tests
 License-File: LICENSE
 
 sunpy-soar
 ==========
@@ -104,14 +105,18 @@
 ===========
 The SunPy developers maintain this package.
 Contributions for new features and bug fixes are welcome.
 
 Changelog
 =========
 
+1.8
+---
+- Added ability to query with SOOP name.
+
 1.7
 ---
 - Added STIX data products to the list of valid data product identifiers.
 
 1.6
 ---
 - Registered a list of instruments available from the SOAR, with the ``a.Instrument`` attribute.
```

### Comparing `sunpy-soar-1.7/README.rst` & `sunpy-soar-1.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,18 @@
 ===========
 The SunPy developers maintain this package.
 Contributions for new features and bug fixes are welcome.
 
 Changelog
 =========
 
+1.8
+---
+- Added ability to query with SOOP name.
+
 1.7
 ---
 - Added STIX data products to the list of valid data product identifiers.
 
 1.6
 ---
 - Registered a list of instruments available from the SOAR, with the ``a.Instrument`` attribute.
```

### Comparing `sunpy-soar-1.7/setup.cfg` & `sunpy-soar-1.8/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 zip_safe = False
 packages = find:
 python_requires = >= 3.7
 install_requires =
```

### Comparing `sunpy-soar-1.7/sunpy_soar/attrs.py` & `sunpy-soar-1.8/sunpy_soar/attrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,20 @@
     def __init__(self, *args, **kwargs):
         warnings.warn(
             "'a.soar.Identifier' is deprecated; use 'a.soar.Product' instead.",
             SunpyDeprecationWarning)
         super().__init__(*args, **kwargs)
 
 
+class SOOP(SimpleAttr):
+    """
+    The SOOP name to search for.
+    """
+
+
 walker = AttrWalker()
 
 
 @walker.add_creator(AttrOr)
 def create_or(wlk, tree):
     """
     Creator for OR. Loops through the next level down in the tree and appends
@@ -119,7 +125,12 @@
 def _(wlk, attr, params):
     params.append(f"descriptor='{attr.value}'")
 
 
 @walker.add_applier(a.Provider)
 def _(wlk, attr, params):
     params.append(f"provider='{attr.value}'")
+
+
+@walker.add_applier(SOOP)
+def _(wlk, attr, params):
+    params.append(f"soop_name='{attr.value}'")
```

### Comparing `sunpy-soar-1.7/sunpy_soar/client.py` & `sunpy-soar-1.8/sunpy_soar/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import requests
 import sunpy.net.attrs as a
 from sunpy import log
 from sunpy.net.attr import and_
 from sunpy.net.base_client import BaseClient, QueryResponseTable
 from sunpy.time import parse_time
 
-from sunpy_soar.attrs import Identifier, Product, walker
+from sunpy_soar.attrs import SOOP, Identifier, Product, walker
 
 __all__ = ['SOARClient']
 
 
 class SOARClient(BaseClient):
     """
     Client to access the Solar Orbiter Archive (SOAR).
@@ -104,15 +104,15 @@
                                      'Data product': info['descriptor'],
                                      'Level': info['level'],
                                      'Start time': info['begin_time'],
                                      'End time': info['end_time'],
                                      'Data item ID': info['data_item_id'],
                                      'Filename': info['filename'],
                                      'Filesize': info['filesize'],
-                                     })
+                                     'SOOP Name': info["soop_name"]})
 
     def fetch(self, query_results, *, path, downloader, **kwargs):
         """
         Queue a set of results to be downloaded. `BaseClient` does the actual
         downloading, so we just have to queue up the ``downloader``.
 
         Parameters
@@ -150,15 +150,15 @@
 
         Returns
         -------
         bool
             True if this client can handle the given query.
         """
         required = {a.Time}
-        optional = {a.Instrument, a.Level, a.Provider, Product, Identifier}
+        optional = {a.Instrument, a.Level, a.Provider, Product, Identifier, SOOP}
         if not cls.check_attr_types_in_query(query, required, optional):
             return False
         # check to make sure the instrument attr passed is one provided by the SOAR.
         # also check to make sure that the provider passed is the SOAR for which this client can handle.
         instr = [i[0].lower() for i in cls.register_values()[a.Instrument]]
         for x in query:
             if isinstance(x, a.Instrument) and str(x.value).lower() not in instr:
@@ -174,21 +174,28 @@
 
     @classmethod
     def register_values(cls):
         return cls.load_dataset_values()
 
     @staticmethod
     def load_dataset_values():
+        # Instrument attrs
         attrs_path = pathlib.Path(__file__).parent / 'data' / 'attrs.json'
         with open(attrs_path, 'r') as attrs_file:
             all_datasets = json.load(attrs_file)
-
         # Convert from dict to list of tuples
         all_datasets = [(id, desc) for id, desc in all_datasets.items()]
 
+        # Instrument attrs
         instr_path = pathlib.Path(__file__).parent / 'data' / 'instrument_attrs.json'
         with open(instr_path, 'r') as instr_attrs_file:
             all_instr = json.load(instr_attrs_file)
-
         all_instr = [(id, desc) for id, desc in all_instr.items()]
 
-        return {Product: all_datasets, a.Instrument: all_instr, a.Provider:  [('SOAR', 'Solar Orbiter Archive.')]}
+        soop_path = pathlib.Path(__file__).parent / 'data' / 'soop_attrs.json'
+        with open(soop_path, 'r') as soop_path_file:
+            all_soops = json.load(soop_path_file)
+
+        all_soops = [(id, desc) for id, desc in all_soops.items()]
+
+        return {Product: all_datasets, a.Instrument: all_instr,
+                SOOP: all_soops, a.Provider:  [('SOAR', 'Solar Orbiter Archive.')]}
```

### Comparing `sunpy-soar-1.7/sunpy_soar/data/attrs.json` & `sunpy-soar-1.8/sunpy_soar/data/attrs.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9827586206896551%*

 * *Differences: {"'RPW-BIA-DENSITY'": "'Solar Orbiter Radio/Plasma Wave, LFR L3 plasma density derived from the "*

 * *                      "spacecraft potential'",*

 * * "'RPW-BIA-DENSITY-10-SECONDS'": "'Solar Orbiter Radio/Plasma Wave, LFR L3 plasma density derived "*

 * *                                 "from the spacecraft potential, downsampled'",*

 * * "'RPW-BIA-SCPOT'": "'Solar Orbiter Radio/Plasma Wave, LFR L3 spacecraft potential'",*

 * * "'RPW-BIA-SCPOT-10-SECONDS'": "'Solar Orbiter Radio/Plasma Wave, LFR L3 spacecraft potential, "*

 * *     […]*

```diff
@@ -111,20 +111,24 @@
     "PHI-HRT-BAZI": "",
     "PHI-HRT-BINC": "",
     "PHI-HRT-BLOS": "",
     "PHI-HRT-BMAG": "",
     "PHI-HRT-ICNT": "",
     "PHI-HRT-STOKES": "",
     "PHI-HRT-VLOS": "",
+    "RPW-BIA-DENSITY": "Solar Orbiter Radio/Plasma Wave, LFR L3 plasma density derived from the spacecraft potential",
+    "RPW-BIA-DENSITY-10-SECONDS": "Solar Orbiter Radio/Plasma Wave, LFR L3 plasma density derived from the spacecraft potential, downsampled",
     "RPW-BIA-DENSITY-10-SECONDS-CDAG": "Solar Orbiter Radio/Plasma Wave, LFR L3 plasma density derived from the spacecraft potential, downsampled",
     "RPW-BIA-DENSITY-CDAG": "Solar Orbiter Radio/Plasma Wave, LFR L3 plasma density derived from the spacecraft potential",
     "RPW-BIA-EFIELD": "Solar Orbiter Radio/Plasma Wave, LFR L3 electric field vector",
     "RPW-BIA-EFIELD-10-SECONDS": "Solar Orbiter Radio/Plasma Wave, LFR L3 electric field vector, downsampled",
     "RPW-BIA-EFIELD-10-SECONDS-CDAG": "Solar Orbiter Radio/Plasma Wave, LFR L3 electric field vector, downsampled",
     "RPW-BIA-EFIELD-CDAG": "Solar Orbiter Radio/Plasma Wave, LFR L3 electric field vector",
+    "RPW-BIA-SCPOT": "Solar Orbiter Radio/Plasma Wave, LFR L3 spacecraft potential",
+    "RPW-BIA-SCPOT-10-SECONDS": "Solar Orbiter Radio/Plasma Wave, LFR L3 spacecraft potential, downsampled",
     "RPW-BIA-SCPOT-10-SECONDS-CDAG": "Solar Orbiter Radio/Plasma Wave, LFR L3 spacecraft potential, downsampled",
     "RPW-BIA-SCPOT-CDAG": "Solar Orbiter Radio/Plasma Wave, LFR L3 spacecraft potential",
     "RPW-HFR-SURV": "Solar Orbiter Radio/Plasma Wave, HFR L2 parameters",
     "RPW-LFR-SURV-ASM": "Solar Orbiter Radio/Plasma Wave, LFR L2 parameters",
     "RPW-LFR-SURV-BP1": "Solar Orbiter Radio/Plasma Wave, LFR L2 parameters",
     "RPW-LFR-SURV-BP2": "Solar Orbiter Radio/Plasma Wave, LFR L2 parameters",
     "RPW-LFR-SURV-CWF": "Solar Orbiter Radio/Plasma Wave, LFR L1 parameters",
```

### Comparing `sunpy-soar-1.7/sunpy_soar/tests/test_sunpy_soar.py` & `sunpy-soar-1.8/sunpy_soar/tests/test_sunpy_soar.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,33 @@
 def test_registered_instr_attrs():
     # Check if the Solo instruments are registered in a.Instrument
     instr_attr = a.Instrument
     assert "SOAR" in instr_attr._attr_registry[instr_attr].client
     assert "stix" in instr_attr._attr_registry[instr_attr].name
 
 
+def test_registered_soop_names():
+    # Check if the soop names are registered in a.soar.SOOP
+    soop_attr = str(a.soar.SOOP)
+    assert "\nr_small_mres_mcad_ar_long_term" in soop_attr
+
+
+def test_search_soop():
+    instr = a.Instrument("EUI")
+    time = a.Time("2022-04-01 01:00", "2022-04-01 02:00")
+    soop_attr = a.soar.SOOP.r_small_mres_mcad_ar_long_term
+    res = Fido.search(time, instr, soop_attr)
+    assert "SOOP Name" in res[0].columns
+    assert res.file_num == 16
+
+    # test non valid soop name passed
+    res = Fido.search(time, instr, a.soar.SOOP("hello"))
+    assert res.file_num == 0
+
+
 def test_when_soar_provider_passed():
     # Tests when a.Provider.soar is passed that only SOARClient results are returned
     id = a.Instrument('EUI')
     time = a.Time('2022-04-01 00:00', '2022-04-01 01:00')
     provider = a.Provider.soar
     res = Fido.search(time & id & provider)
     assert len(res) == 1
```

### Comparing `sunpy-soar-1.7/sunpy_soar.egg-info/PKG-INFO` & `sunpy-soar-1.8/sunpy_soar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpy-soar
-Version: 1.7
+Version: 1.8
 Summary: A sunpy plugin for accessing data in the Solar Orbiter Archive (SOAR).
 Home-page: 
 Author: David Stansby
 Author-email: d.stansby@ucl.ac.uk
 License: BSD-2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Provides-Extra: tests
 License-File: LICENSE
 
 sunpy-soar
 ==========
@@ -104,14 +105,18 @@
 ===========
 The SunPy developers maintain this package.
 Contributions for new features and bug fixes are welcome.
 
 Changelog
 =========
 
+1.8
+---
+- Added ability to query with SOOP name.
+
 1.7
 ---
 - Added STIX data products to the list of valid data product identifiers.
 
 1.6
 ---
 - Registered a list of instruments available from the SOAR, with the ``a.Instrument`` attribute.
```

### Comparing `sunpy-soar-1.7/sunpy_soar.egg-info/SOURCES.txt` & `sunpy-soar-1.8/sunpy_soar.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 sunpy_soar.egg-info/SOURCES.txt
 sunpy_soar.egg-info/dependency_links.txt
 sunpy_soar.egg-info/not-zip-safe
 sunpy_soar.egg-info/requires.txt
 sunpy_soar.egg-info/top_level.txt
 sunpy_soar/data/attrs.json
 sunpy_soar/data/instrument_attrs.json
+sunpy_soar/data/soop_attrs.json
 sunpy_soar/tests/__init__.py
 sunpy_soar/tests/test_sunpy_soar.py
 tools/update_data.py
```

### Comparing `sunpy-soar-1.7/tools/update_data.py` & `sunpy-soar-1.8/tools/update_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,17 +51,36 @@
         if r["name"] not in instruments:
             pass
         else:
             instr_desc[r["name"]] = r["long_name"]
     return instr_desc
 
 
+def get_all_soops():
+    # Get the unique soop names
+    print("Updating SOOP descriptors...")
+    SOAR = TapPlus(url="http://soar.esac.esa.int/soar-sl-tap/tap")
+    job = SOAR.launch_job('select * from soar.soop')
+    res = job.get_results()
+
+    soop_names = {}
+    for row in res:
+        soop_names[row["soop_name"]] = ''
+
+    return soop_names
+
+
 if __name__ == '__main__':
     attr_file = pathlib.Path(__file__).parent.parent / 'sunpy_soar' / 'data' / 'attrs.json'
     descriptors = get_all_descriptors()
     with open(attr_file, 'w') as attrs_file:
         json.dump(dict(sorted(descriptors.items())), attrs_file, indent=2)
 
     instr_file = pathlib.Path(__file__).parent.parent / 'sunpy_soar' / 'data' / 'instrument_attrs.json'
     instr_descriptors = get_all_instruments()
     with open(instr_file, 'w') as instrs_file:
         json.dump(dict(sorted(instr_descriptors.items())), instrs_file, indent=2)
+
+    soop_file = pathlib.Path(__file__).parent.parent / 'sunpy_soar' / 'data' / 'soop_attrs.json'
+    soop_descriptors = get_all_soops()
+    with open(soop_file, 'w') as soops_file:
+        json.dump(dict(sorted(soop_descriptors.items())), soops_file, indent=2)
```

