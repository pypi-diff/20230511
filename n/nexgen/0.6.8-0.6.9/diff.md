# Comparing `tmp/nexgen-0.6.8.tar.gz` & `tmp/nexgen-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexgen-0.6.8.tar", last modified: Sun May 22 16:13:29 2022, max compression
+gzip compressed data, was "nexgen-0.6.9.tar", last modified: Mon Jul 18 13:42:29 2022, max compression
```

## Comparing `nexgen-0.6.8.tar` & `nexgen-0.6.9.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-22 16:13:29.030538 nexgen-0.6.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     1528 2022-05-22 16:13:18.000000 nexgen-0.6.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)       71 2022-05-22 16:13:18.000000 nexgen-0.6.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     2117 2022-05-22 16:13:29.030538 nexgen-0.6.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1186 2022-05-22 16:13:18.000000 nexgen-0.6.8/README.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      100 2022-05-22 16:13:18.000000 nexgen-0.6.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)     1387 2022-05-22 16:13:29.030538 nexgen-0.6.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)       92 2022-05-22 16:13:18.000000 nexgen-0.6.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-22 16:13:29.018538 nexgen-0.6.8/src/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-22 16:13:29.026538 nexgen-0.6.8/src/nexgen/
--rw-r--r--   0 vsts      (1001) docker     (121)     7224 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-22 16:13:29.026538 nexgen-0.6.8/src/nexgen/beamlines/
--rw-r--r--   0 vsts      (1001) docker     (121)     1370 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/beamlines/I03_Eiger.phil
--rw-r--r--   0 vsts      (1001) docker     (121)     1412 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/beamlines/I19-2_Eiger.phil
--rw-r--r--   0 vsts      (1001) docker     (121)     1518 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/beamlines/I19-2_Tristan.phil
--rw-r--r--   0 vsts      (1001) docker     (121)    15071 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/beamlines/I19_2_nxs.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3227 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/beamlines/I19_2_params.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1266 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/beamlines/I24_Eiger.phil
--rw-r--r--   0 vsts      (1001) docker     (121)    12416 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/beamlines/I24_Eiger_nxs.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1937 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/beamlines/I24_Eiger_params.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7682 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/beamlines/SSX_Tristan_nxs.py
--rw-r--r--   0 vsts      (1001) docker     (121)       79 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/beamlines/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-22 16:13:29.026538 nexgen-0.6.8/src/nexgen/command_line/
--rw-r--r--   0 vsts      (1001) docker     (121)     3083 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/command_line/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7749 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/command_line/copy_nexus.py
--rw-r--r--   0 vsts      (1001) docker     (121)    33628 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/command_line/nexus_generator.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7538 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/command_line/nxs_phil.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3812 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/command_line/phil_files_cli.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-22 16:13:29.026538 nexgen-0.6.8/src/nexgen/nxs_copy/
--rw-r--r--   0 vsts      (1001) docker     (121)     4727 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/nxs_copy/CopyNexus.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6793 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/nxs_copy/CopyTristanNexus.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3744 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/nxs_copy/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-22 16:13:29.030538 nexgen-0.6.8/src/nexgen/nxs_write/
--rw-r--r--   0 vsts      (1001) docker     (121)    31994 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/nxs_write/NXclassWriters.py
--rw-r--r--   0 vsts      (1001) docker     (121)    21352 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/nxs_write/NexusWriter.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11290 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/nxs_write/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-22 16:13:29.030538 nexgen-0.6.8/src/nexgen/tools/
--rw-r--r--   0 vsts      (1001) docker     (121)    10383 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/tools/DataWriter.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1983 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/tools/ExtendedRequest.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4938 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/tools/GDAjson2params.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6572 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/tools/MetaReader.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6504 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/tools/Metafile.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3542 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/tools/VDS_tools.py
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-22 16:13:18.000000 nexgen-0.6.8/src/nexgen/tools/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-22 16:13:29.026538 nexgen-0.6.8/src/nexgen.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     2117 2022-05-22 16:13:28.000000 nexgen-0.6.8/src/nexgen.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1328 2022-05-22 16:13:28.000000 nexgen-0.6.8/src/nexgen.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-05-22 16:13:28.000000 nexgen-0.6.8/src/nexgen.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      260 2022-05-22 16:13:28.000000 nexgen-0.6.8/src/nexgen.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-05-22 16:13:28.000000 nexgen-0.6.8/src/nexgen.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       70 2022-05-22 16:13:28.000000 nexgen-0.6.8/src/nexgen.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        7 2022-05-22 16:13:28.000000 nexgen-0.6.8/src/nexgen.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-18 13:42:29.945882 nexgen-0.6.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1528 2022-07-18 13:42:24.000000 nexgen-0.6.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)       71 2022-07-18 13:42:24.000000 nexgen-0.6.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     2117 2022-07-18 13:42:29.945882 nexgen-0.6.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     1186 2022-07-18 13:42:24.000000 nexgen-0.6.9/README.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)      100 2022-07-18 13:42:24.000000 nexgen-0.6.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1387 2022-07-18 13:42:29.945882 nexgen-0.6.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)       92 2022-07-18 13:42:24.000000 nexgen-0.6.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-18 13:42:29.937882 nexgen-0.6.9/src/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-18 13:42:29.941882 nexgen-0.6.9/src/nexgen/
+-rw-r--r--   0 vsts      (1001) docker     (121)     7319 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-18 13:42:29.941882 nexgen-0.6.9/src/nexgen/beamlines/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1370 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/beamlines/I03_Eiger.phil
+-rw-r--r--   0 vsts      (1001) docker     (121)     1412 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/beamlines/I19-2_Eiger.phil
+-rw-r--r--   0 vsts      (1001) docker     (121)     1518 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/beamlines/I19-2_Tristan.phil
+-rw-r--r--   0 vsts      (1001) docker     (121)    15478 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/beamlines/I19_2_nxs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3227 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/beamlines/I19_2_params.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1266 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/beamlines/I24_Eiger.phil
+-rw-r--r--   0 vsts      (1001) docker     (121)    15621 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/beamlines/I24_Eiger_nxs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1937 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/beamlines/I24_Eiger_params.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7565 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/beamlines/SSX_Tristan_nxs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4745 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/beamlines/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-18 13:42:29.941882 nexgen-0.6.9/src/nexgen/command_line/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3083 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/command_line/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7579 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/command_line/copy_nexus.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    33098 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/command_line/nexus_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7500 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/command_line/nxs_phil.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4464 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/command_line/phil_files_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2177 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/log.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-18 13:42:29.941882 nexgen-0.6.9/src/nexgen/nxs_copy/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4729 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/nxs_copy/CopyNexus.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7276 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/nxs_copy/CopyTristanNexus.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4115 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/nxs_copy/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-18 13:42:29.945882 nexgen-0.6.9/src/nexgen/nxs_write/
+-rw-r--r--   0 vsts      (1001) docker     (121)    32080 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/nxs_write/NXclassWriters.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22547 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/nxs_write/NexusWriter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12619 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/nxs_write/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-18 13:42:29.945882 nexgen-0.6.9/src/nexgen/tools/
+-rw-r--r--   0 vsts      (1001) docker     (121)    10374 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/tools/DataWriter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1983 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/tools/ExtendedRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4938 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/tools/GDAjson2params.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6559 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/tools/MetaReader.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6504 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/tools/Metafile.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6416 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/tools/VDS_tools.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-18 13:42:24.000000 nexgen-0.6.9/src/nexgen/tools/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-18 13:42:29.941882 nexgen-0.6.9/src/nexgen.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2117 2022-07-18 13:42:29.000000 nexgen-0.6.9/src/nexgen.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     1346 2022-07-18 13:42:29.000000 nexgen-0.6.9/src/nexgen.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-18 13:42:29.000000 nexgen-0.6.9/src/nexgen.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      260 2022-07-18 13:42:29.000000 nexgen-0.6.9/src/nexgen.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-18 13:42:29.000000 nexgen-0.6.9/src/nexgen.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)       70 2022-07-18 13:42:29.000000 nexgen-0.6.9/src/nexgen.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        7 2022-07-18 13:42:29.000000 nexgen-0.6.9/src/nexgen.egg-info/top_level.txt
```

### Comparing `nexgen-0.6.8/LICENSE` & `nexgen-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nexgen-0.6.8/PKG-INFO` & `nexgen-0.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexgen
-Version: 0.6.8
+Version: 0.6.9
 Summary: Next Generation Nexus Generator
 Home-page: UNKNOWN
 Author: Diamond Light Source - Scientific Software
 Author-email: scientificsoftware@diamond.ac.uk
 License: BSD 3-Clause License
 Project-URL: Documentation, https://nexgen.readthedocs.io/
 Project-URL: GitHub, https://github.com/dials/nexgen
```

### Comparing `nexgen-0.6.8/README.rst` & `nexgen-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `nexgen-0.6.8/setup.cfg` & `nexgen-0.6.9/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nexgen
-version = 0.6.8
+version = 0.6.9
 description = Next Generation Nexus Generator
 long_description = file: README.rst
 author = Diamond Light Source - Scientific Software
 author_email = scientificsoftware@diamond.ac.uk
 license = BSD 3-Clause License
 license_file = LICENSE
 classifiers =
```

### Comparing `nexgen-0.6.8/src/nexgen/__init__.py` & `nexgen-0.6.9/src/nexgen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """
 General tools useful to create NeXus format files.
 """
 
 __author__ = "Diamond Light Source - Scientific Software"
 __email__ = "scientificsoftware@diamond.ac.uk"
-__version__ = "0.6.8"
+__version__ = "0.6.9"
 __version_tuple__ = tuple(int(x) for x in __version__.split("."))
 
+import logging
 import re
 from datetime import datetime
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
 import h5py
 import numpy as np
 import pint
 
+# Logging set up
+logging.getLogger("nexgen").addHandler(logging.NullHandler())
+
 # Initialize registry and a Quantity constructor
 ureg = pint.UnitRegistry()
 Q_ = ureg.Quantity
 
 # Define scope extract type
 # Scope = freephil.common.scope_extract
```

### Comparing `nexgen-0.6.8/src/nexgen/beamlines/I03_Eiger.phil` & `nexgen-0.6.9/src/nexgen/beamlines/I03_Eiger.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.6.8/src/nexgen/beamlines/I19-2_Eiger.phil` & `nexgen-0.6.9/src/nexgen/beamlines/I19-2_Eiger.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.6.8/src/nexgen/beamlines/I19-2_Tristan.phil` & `nexgen-0.6.9/src/nexgen/beamlines/I19-2_Tristan.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.6.8/src/nexgen/beamlines/I19_2_nxs.py` & `nexgen-0.6.9/src/nexgen/beamlines/I19_2_nxs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,41 @@
 """
 Create a NeXus file for time-resolved collections on I19-2.
 Available detectors: Tristan 10M, Eiger 2X 4M.
 """
 
 import glob
 import logging
-import sys
 from collections import namedtuple
 from datetime import datetime
 from pathlib import Path
 from typing import Tuple, Union
 
 import h5py
 
-from .. import get_iso_timestamp, get_nexus_filename
-from ..nxs_write import calculate_rotation_scan_range
+from .. import get_iso_timestamp, get_nexus_filename, log
+from ..nxs_write import calculate_scan_range
 from ..nxs_write.NexusWriter import call_writers
 from ..nxs_write.NXclassWriters import write_NXdatetime, write_NXentry
 from ..tools.ExtendedRequest import ExtendedRequestIO
 from ..tools.GDAjson2params import (
     read_detector_params_from_json,
     read_geometry_from_json,
 )
+from ..tools.VDS_tools import image_vds_writer
 from .I19_2_params import (
     dset_links,
     eiger4M_params,
     goniometer_axes,
     source,
     tristan10M_params,
 )
 
 # Define a logger object and a formatter
-logger = logging.getLogger("NeXusGenerator.I19-2")
-logger.setLevel(logging.DEBUG)
-formatter = logging.Formatter("%(name)s %(levelname)s %(message)s")  # %(asctime)s
-# Define a stream handler
-CH = logging.StreamHandler(sys.stdout)
-CH.setLevel(logging.DEBUG)
-CH.setFormatter(formatter)
-logger.addHandler(CH)
+logger = logging.getLogger("nexgen.I19-2_NeXus")
 
 # Tristan mask and flatfield files
 maskfile = "Tristan10M_mask_with_spec.h5"
 flatfieldfile = "Tristan10M_flat_field_coeff_with_Mo_17.479keV.h5"
 
 tr_collect = namedtuple(
     "tr_collect",
@@ -67,14 +60,26 @@
 detector = {}  # tristan10M_params
 module = {}
 beam = {"flux": None}
 attenuator = {}
 
 
 def read_from_xml(xmlfile: Union[Path, str], detector_name: str):
+    """
+    Extract information about the collection and the beamline contained in the xml file.
+
+    Args:
+        xmlfile (Union[Path, str]): Path to xml file.
+        detector_name (str): Detector in use for the current collection
+
+    Returns:
+        scan_axis (str): Name of the rotation scan axis
+        pos (Dict): Dictionary containing the (start,end,increment) values for each goniometer axis.
+        num (int): Number of images written.
+    """
     ecr = ExtendedRequestIO(xmlfile)
 
     # Attenuator
     attenuator["transmission"] = ecr.getTransmission()
 
     # Detector [2theta, det_z]
     if "tristan" in detector_name.lower():
@@ -164,15 +169,15 @@
                 OSC,
             )
 
             # write_NXdatetime(nxsfile, (None, timestamps[1]))
             if timestamps[1]:
                 write_NXdatetime(nxsfile, (None, timestamps[1]))
             #    nxentry.create_dataset("end_time", data=np.string_(timestamps[1]))
-            logger.info(f"{master_file} correctly written.")
+            logger.info(f"The file {master_file} was written correctly.")
     except Exception as err:
         logger.exception(err)
         logger.info(
             f"An error occurred and {master_file} couldn't be written correctly."
         )
 
 
@@ -202,23 +207,24 @@
         Path(f).expanduser().resolve() for f in sorted(glob.glob(filename_template))
     ]
     logger.info(f"Found {len(filenames)} files in directory.")
 
     # Get scan range array
     logger.info("Calculating scan range...")
     scan_idx = goniometer["axes"].index(scan_axis)
-    scan_range = calculate_rotation_scan_range(
-        goniometer["starts"][scan_idx],
-        goniometer["ends"][scan_idx],
-        goniometer["increments"][scan_idx],
-        n_images=n_frames,
-    )
 
     # Define OSC scans dictionary
-    OSC = {scan_axis: scan_range}
+    OSC = calculate_scan_range(
+        [goniometer["axes"][scan_idx]],
+        [goniometer["starts"][scan_idx]],
+        [goniometer["ends"][scan_idx]],
+        axes_increments=[goniometer["increments"][scan_idx]],
+        # n_images=n_frames,
+        rotation=True,
+    )
 
     # Get on with the writing now...
     try:
         with h5py.File(master_file, "x") as nxsfile:
             write_NXentry(nxsfile)
 
             if timestamps[0]:
@@ -239,15 +245,18 @@
                 transl_scan=None,
                 metafile=TR.meta_file,
                 link_list=dset_links,
             )
 
             if timestamps[1]:
                 write_NXdatetime(nxsfile, (None, timestamps[1]))
-            logger.info(f"{master_file} correctly written.")
+
+            # Write VDS
+            image_vds_writer(nxsfile, (int(n_frames), *detector["image_size"]))
+            logger.info(f"The file {master_file} was written correctly.")
     except Exception as err:
         logger.exception(err)
         logger.info(
             f"An error occurred and {master_file} couldn't be written correctly."
         )
 
 
@@ -277,20 +286,19 @@
         detector_json=tr_params["detector_json"]
         if tr_params["detector_json"]
         else None,
     )
 
     # Define a file handler
     logfile = TR.meta_file.parent / "nexus_writer.log"
-    FH = logging.FileHandler(logfile, mode="a")
-    FH.setLevel(logging.DEBUG)
-    FH.setFormatter(formatter)
-    logger.addHandler(FH)
+    # Configure logging
+    log.config(logfile.as_posix())
 
-    logger.info(f"{TR.detector_name} NeXus file writer.")
+    logger.info("NeXus file writer for beamline I19-2 at DLS.")
+    logger.info(f"Detector in use for this experiment: {TR.detector_name}.")
     logger.info(f"Current collection directory: {TR.meta_file.parent}")
     # Add some information to logger
     logger.info("Creating a NeXus file for %s ..." % TR.meta_file.name)
     # Get NeXus filename
     master_file = get_nexus_filename(TR.meta_file)
     logger.info("NeXus file will be saved as %s" % master_file)
```

### Comparing `nexgen-0.6.8/src/nexgen/beamlines/I19_2_params.py` & `nexgen-0.6.9/src/nexgen/beamlines/I19_2_params.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.6.8/src/nexgen/beamlines/I24_Eiger.phil` & `nexgen-0.6.9/src/nexgen/beamlines/I24_Eiger.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.6.8/src/nexgen/beamlines/I24_Eiger_nxs.py` & `nexgen-0.6.9/src/nexgen/beamlines/I24_Eiger_nxs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 """
 Create a NeXus file for serial crystallography datasets collected on I24 Eiger 2X 9M detector.
 """
 import glob
 import logging
-import sys
 from collections import namedtuple
 from pathlib import Path
 from typing import List
 
 import h5py
+import numpy as np
 
-from .. import get_iso_timestamp, get_nexus_filename
+from .. import get_iso_timestamp, get_nexus_filename, log
 from ..nxs_write.NexusWriter import ScanReader, call_writers
 from ..nxs_write.NXclassWriters import write_NXdatetime, write_NXentry, write_NXnote
 from ..tools.VDS_tools import image_vds_writer
+from . import compute_goniometer, read_chip_map
 from .I24_Eiger_params import dset_links, eiger9M_params, goniometer_axes, source
 
-# import numpy as np
-
-
 # Define a logger object and a formatter
-logger = logging.getLogger("NeXusGenerator.I24")
-logger.setLevel(logging.DEBUG)
-formatter = logging.Formatter("%(asctime)s %(name)s %(levelname)s %(message)s")
-# Define a stream handler
-CH = logging.StreamHandler(sys.stdout)
-CH.setLevel(logging.DEBUG)
-CH.setFormatter(formatter)
-logger.addHandler(CH)
+logger = logging.getLogger("nexgen.I24")
 
 ssx_collect = namedtuple(
     "ssx_collect",
     [
         "visitpath",
         "filename",
         "exp_type",
@@ -43,27 +34,29 @@
         "exposure_time",
         "transmission",
         "wavelength",
         "flux",
         "pump_status",
         "pump_exp",
         "pump_delay",
+        "chip_info",
+        "chipmap",
     ],
 )
 
 coordinate_frame = "mcstas"
 
 # Initialize dictionaries
 goniometer = goniometer_axes
 detector = eiger9M_params
 module = {}
 beam = {}
 attenuator = {}
 
-
+#
 def extruder(
     master_file: Path,
     filename: List[Path],
     SSX: namedtuple,
     metafile: Path = None,  # Just in case meta is not generated for some reason
 ):
     """
@@ -145,19 +138,19 @@
                     logger.warning(
                         "Pump delay has not been recorded and won't be written to file."
                     )
                 loc = "/entry/source/notes"
                 write_NXnote(nxsfile, loc, pump_info)
 
             # Write VDS
-            image_vds_writer(nxsfile, (SSX.num_imgs, *detector["image_size"]))
+            image_vds_writer(nxsfile, (int(SSX.num_imgs), *detector["image_size"]))
 
             if timestamps[1]:
                 write_NXdatetime(nxsfile, (None, timestamps[1]))
-            logger.info(f"{master_file} correctly written.")
+            logger.info(f"The file {master_file} was written correctly.")
     except Exception as err:
         logger.exception(err)
         logger.info(
             f"An error occurred and {master_file} couldn't be written correctly."
         )
 
 
@@ -174,114 +167,176 @@
         master_file (Path):         Path to the NeXus file to be written.
         filename (List[Path]):      List of paths to file.
         SSX (namedtuple):           Parameters passed from the beamline.
         metafile (Path, optional):  Path to the _meta.h5 file. Defaults to None.
     """
     logger.info(f"Write NeXus file for {SSX.exp_type}")
 
+    # Check that the chip dict has been passed, raise error is not
+    if SSX.chip_info is None:
+        logger.error("No chip_dict found.")
+        raise ValueError(
+            "No information about the FT chip has been passed. \
+            Impossible to determine scan parameters. NeXus file won't be written."
+        )
+
     # Get timestamps in the correct format
     timestamps = (
         get_iso_timestamp(SSX.start_time),
         get_iso_timestamp(SSX.stop_time),
     )
     logger.info(f"Timestamps recorded: {timestamps}")
 
-    # Goniometer
-    # Set start and end values from input
-    # omega sam_z sam_y sam_x
-    goniometer["starts"] = []
-    goniometer["ends"] = []
-    goniometer["increments"] = []
-
-    # Identify rotation and grid scan axes, calculate ranges
-    OSC, TRANSL = ScanReader(goniometer, n_images=SSX.num_imgs)
-
-    # Log data
-    logger.info("Goniometer information")
-    for j in range(len(goniometer["axes"])):
-        logger.info(
-            f"Goniometer axis: {goniometer['axes'][j]} => {goniometer['starts'][j]}, {goniometer['types'][j]} on {goniometer['depends'][j]}"
+    # Is it a time resolved SSX experiment?
+    if int(SSX.chip_info["N_EXPOSURES"][1]) == 1:
+        goniometer["increments"] = [0.0, 0.0, 0.0, 0.0]
+        # Read chip map
+        blocks = read_chip_map(
+            SSX.chipmap,
+            SSX.chip_info["X_NUM_BLOCKS"][1],
+            SSX.chip_info["Y_NUM_BLOCKS"][1],
         )
-    logger.info(f"Oscillation axis: {OSC.keys()[0]}.")
-    logger.info(f"Fixed target axes: {list(TRANSL.keys())}.")
-
-    try:
-        with h5py.File(master_file, "x") as nxsfile:
-            write_NXentry(nxsfile)
 
-            if timestamps[0]:
-                write_NXdatetime(nxsfile, (timestamps[0], None))
-
-            call_writers(
-                nxsfile,
-                filename,
-                coordinate_frame,
-                (detector["mode"], SSX.num_imgs),
+        # Calculate scan start/end positions on chip
+        if type(blocks) is dict:
+            logger.info(f"Scanning blocks: {list(blocks.keys())}.")
+            start_pos, end_pos = compute_goniometer(SSX.chip_info, blocks=blocks)
+        else:
+            logger.info("Full chip: all the blocks will be scanned.")
+            start_pos, end_pos = compute_goniometer(SSX.chip_info, full=True)
+
+        # Iterate over blocks to calculate scan points
+        OSC = {"omega": np.array([])}
+        TRANSL = {"sam_y": np.array([]), "sam_x": np.array([])}
+        for s, e in zip(start_pos.values(), end_pos.values()):
+            goniometer["starts"] = s
+            goniometer["ends"] = e
+            osc, transl = ScanReader(
                 goniometer,
-                detector,
-                module,
-                source,
-                beam,
-                attenuator,
-                OSC,
-                transl_scan=TRANSL,
-                metafile=metafile,
-                link_list=dset_links,
+                n_images=(
+                    SSX.chip_info["Y_NUM_STEPS"][1],
+                    SSX.chip_info["X_NUM_STEPS"][1],
+                ),
+            )
+            OSC["omega"] = np.append(OSC["omega"], osc["omega"])
+            TRANSL["sam_y"] = np.append(TRANSL["sam_y"], transl["sam_y"])
+            TRANSL["sam_x"] = np.append(TRANSL["sam_x"], transl["sam_x"])
+
+        # Log data
+        logger.info("Goniometer information")
+        for j in range(len(goniometer["axes"])):
+            logger.info(
+                f"Goniometer axis: {goniometer['axes'][j]} => {goniometer['types'][j]} on {goniometer['depends'][j]}"
             )
+        logger.info(f"Oscillation axis: {list(OSC.keys())[0]}.")
+        logger.info(f"Grid scan axes: {list(TRANSL.keys())}.")
 
-            # Write pump-probe information if requested
-            if SSX.pump_status == "true":
-                logger.info("Pump status is True, write pump information to file.")
-                pump_info = {}
-                if SSX.pump_exp:
-                    pump_info["pump_exposure_time"] = SSX.pump_exp
-                    logger.info(f"Recorded pump exposure time: {SSX.pump_exp}")
-                else:
-                    pump_info["pump_exposure_time"] = None
-                    logger.warning(
-                        "Pump exposure time has not been recorded and won't be written to file."
-                    )
-                if SSX.pump_delay:
-                    pump_info["pump_delay"] = SSX.pump_delay
-                    logger.info(f"Recorded pump delay time: {SSX.pump_delay}")
-                else:
-                    pump_info["pump_delay"] = None
-                    logger.warning(
-                        "Pump delay has not been recorded and won't be written to file."
-                    )
-                loc = "/entry/source/notes"
-                write_NXnote(nxsfile, loc, pump_info)
+        # Check that things make sense
+        if SSX.num_imgs != len(OSC["omega"]):
+            logger.warning(
+                f"The total number of scan points is {len(OSC['omega'])}, which does not match the total nu mber of images passed as input {SSX.num_imgs}."
+            )
+            logger.warning(
+                "Reset SSX.num_imgs to number of scan points for vds creation"
+            )
+            tot_imgs = len(OSC["omega"])
+        else:
+            tot_imgs = SSX.num_imgs
+
+        # Write NeXus and VDS
+        try:
+            with h5py.File(master_file, "x") as nxsfile:
+                write_NXentry(nxsfile)
+
+                if timestamps[0]:
+                    write_NXdatetime(nxsfile, (timestamps[0], None))
+
+                call_writers(
+                    nxsfile,
+                    filename,
+                    coordinate_frame,
+                    (detector["mode"], tot_imgs),
+                    goniometer,
+                    detector,
+                    module,
+                    source,
+                    beam,
+                    attenuator,
+                    OSC,
+                    transl_scan=TRANSL,
+                    metafile=metafile,
+                    link_list=dset_links,
+                )
+
+                # Write pump-probe information if requested
+                if SSX.pump_status == "true":
+                    logger.info("Pump status is True, write pump information to file.")
+                    pump_info = {}
+                    if SSX.pump_exp:
+                        pump_info["pump_exposure_time"] = SSX.pump_exp
+                        logger.info(f"Recorded pump exposure time: {SSX.pump_exp}")
+                    else:
+                        pump_info["pump_exposure_time"] = None
+                        logger.warning(
+                            "Pump exposure time has not been recorded and won't be written to file."
+                        )
+                    if SSX.pump_delay:
+                        pump_info["pump_delay"] = SSX.pump_delay
+                        logger.info(f"Recorded pump delay time: {SSX.pump_delay}")
+                    else:
+                        pump_info["pump_delay"] = None
+                        logger.warning(
+                            "Pump delay has not been recorded and won't be written to file."
+                        )
+                    loc = "/entry/source/notes"
+                    write_NXnote(nxsfile, loc, pump_info)
+
+                # Write VDS
+                image_vds_writer(nxsfile, (int(tot_imgs), *detector["image_size"]))
+
+                if timestamps[1]:
+                    write_NXdatetime(nxsfile, (None, timestamps[1]))
+                logger.info(f"The file {master_file} was written correctly.")
+        except Exception as err:
+            logger.exception(err)
+            logger.info(
+                f"An error occurred and {master_file} couldn't be written correctly."
+            )
 
-            # Write VDS
-            image_vds_writer(nxsfile, (SSX.num_imgs, *detector["image_size"]))
+    else:
+        print("TimeResolved goes here")
+        # same as before but with the repeat added headache
 
-            if timestamps[1]:
-                write_NXdatetime(nxsfile, (None, timestamps[1]))
-            logger.info(f"{master_file} correctly written.")
-    except Exception as err:
-        logger.exception(err)
-        logger.info(
-            f"An error occurred and {master_file} couldn't be written correctly."
-        )
 
+def grid_scan_3D(
+    master_file: Path,
+    filename: List[Path],
+    SSX: namedtuple,
+    metafile: Path = None,
+):
+    logger.info(f"Write NeXus file for {SSX.exp_type}")
 
-def grid_scan_3D():
-    pass
+    # Get timestamps in the correct format
+    timestamps = (
+        get_iso_timestamp(SSX.start_time),
+        get_iso_timestamp(SSX.stop_time),
+    )
+    logger.info(f"Timestamps recorded: {timestamps}")
 
 
 def write_nxs(**ssx_params):
     """
     Gather all parameters from the beamline and call appropriate writer function for serial crystallography.
     """
     # Get info from the beamline
     SSX = ssx_collect(
         visitpath=Path(ssx_params["visitpath"]).expanduser().resolve(),
         filename=ssx_params["filename"],  # Template: test_##
         exp_type=ssx_params["exp_type"],
-        num_imgs=ssx_params["num_imgs"],
+        num_imgs=float(ssx_params["num_imgs"]),
         beam_center=ssx_params["beam_center"],
         detector_distance=ssx_params["det_dist"],
         start_time=ssx_params["start_time"].strftime("%Y-%m-%dT%H:%M:%S")
         if ssx_params["start_time"]
         else None,  # This should be datetiem type
         stop_time=ssx_params["stop_time"].strftime("%Y-%m-%dT%H:%M:%S")
         if ssx_params["stop_time"]
@@ -289,16 +344,28 @@
         exposure_time=ssx_params["exp_time"],
         transmission=ssx_params["transmission"],
         wavelength=ssx_params["wavelength"],
         flux=ssx_params["flux"],
         pump_status=ssx_params["pump_status"],
         pump_exp=ssx_params["pump_exp"],
         pump_delay=ssx_params["pump_delay"],
+        chip_info=None
+        if ssx_params["exp_type"] == "extruder"
+        else ssx_params[
+            "chip_info"
+        ],  # ssx_params["chip_info"] if ssx_params["chip_info"] else None,
+        chipmap=None
+        if ssx_params["exp_type"] == "extruder"
+        else Path(ssx_params["chipmap"]).expanduser().resolve(),
     )
 
+    logfile = SSX.visitpath / "nexus_writer.log"
+    # Configure logging
+    log.config(logfile.as_posix())
+
     # Add to dictionaries
     detector["starts"] = [SSX.detector_distance]
     detector["exposure_time"] = SSX.exposure_time
     detector["beam_center"] = SSX.beam_center
 
     attenuator["transmission"] = SSX.transmission
 
@@ -326,14 +393,15 @@
     # Set value for module_offset calculation.
     module["module_offset"] = "1"
 
     # Find datafiles
     filename_template = (
         metafile.parent / metafile.name.replace("meta", f"{6*'[0-9]'}")
     ).as_posix()
+    # if meta else (SSX.visitpath / SSX.filename).as_posix() + f"_{6*'[0-9]'}.h5"
     filename = [
         Path(f).expanduser().resolve() for f in sorted(glob.glob(filename_template))
     ]
 
     # Add some information to logger
     logger.info("Creating a NeXus file for %s ..." % metafile.name)
     # Get NeXus filename
@@ -342,19 +410,22 @@
 
     # Call correct function for the current experiment
     if SSX.exp_type == "extruder":
         extruder(master_file, filename, SSX, metafile)
     elif SSX.exp_type == "fixed_target":
         fixed_target(master_file, filename, SSX, metafile)
     elif SSX.exp_type == "3Dgridscan":
-        grid_scan_3D()
+        grid_scan_3D(master_file, filename, SSX, metafile)
+
+    logger.info("*EOF*\n")
 
 
 # # Example usage
 # if __name__ == "__main__":
+#     import sys
 #     from datetime import datetime
 
 #     write_nxs(
 #         visitpath=sys.argv[1],
 #         filename=sys.argv[2],
 #         exp_type="extruder",
 #         num_imgs=2450,
@@ -367,8 +438,10 @@
 #         exp_time=0.002,
 #         transmission=1.0,
 #         wavelength=0.649,
 #         flux=None,
 #         pump_status="true",  # this is a string on the beamline
 #         pump_exp=None,
 #         pump_delay=None,
+#         chip_info=None,
+#         chipmap=None,
 #     )
```

### Comparing `nexgen-0.6.8/src/nexgen/beamlines/I24_Eiger_params.py` & `nexgen-0.6.9/src/nexgen/beamlines/I24_Eiger_params.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.6.8/src/nexgen/beamlines/SSX_Tristan_nxs.py` & `nexgen-0.6.9/src/nexgen/beamlines/SSX_Tristan_nxs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 """
 Create a NeXus file for serial crystallography datasets collected on I19-2 Tristan10M detector.
 """
 
 import logging
-import sys
 from collections import namedtuple
 from pathlib import Path
 
 import h5py
 
-from .. import get_iso_timestamp, get_nexus_filename
+from .. import get_iso_timestamp, get_nexus_filename, log
 from ..nxs_write.NexusWriter import call_writers
 from ..nxs_write.NXclassWriters import write_NXdatetime, write_NXentry, write_NXnote
 from .I19_2_params import goniometer_axes, source, tristan10M_params
 
 # Define a logger object and a formatter
-logger = logging.getLogger("NeXusGenerator.I19-2_ssx")
-logger.setLevel(logging.DEBUG)
-formatter = logging.Formatter("%(asctime)s %(name)s %(levelname)s %(message)s")
-# Define a stream handler
-CH = logging.StreamHandler(sys.stdout)
-CH.setLevel(logging.DEBUG)
-CH.setFormatter(formatter)
-logger.addHandler(CH)
+logger = logging.getLogger("nexgen.I19-2_ssx")
 
 ssx_tr_collect = namedtuple(
     "ssx_collect",
     [
         "visitpath",
         "filename",
         "tot_num_X",
@@ -57,15 +49,15 @@
     """
     Gather all parameters from the beamline and call the NeXus writers.
     """
     # Get info from the beamline
     SSX_TR = ssx_tr_collect(
         visitpath=Path(ssx_params["visitpath"]).expanduser().resolve(),
         filename=ssx_params["filename"],
-        tot_num_X=ssx_params["tot_num_X"],
+        tot_num_X=float(ssx_params["tot_num_X"]),
         beam_center=ssx_params["beam_center"],
         detector_distance=ssx_params["det_dist"],
         start_time=ssx_params["start_time"].strftime("%Y-%m-%dT%H:%M:%S")
         if ssx_params["start_time"]
         else None,  # This should be datetiem type
         stop_time=ssx_params["stop_time"].strftime("%Y-%m-%dT%H:%M:%S")
         if ssx_params["stop_time"]
@@ -73,16 +65,21 @@
         exposure_time=ssx_params["exp_time"],
         transmission=ssx_params["transmission"],
         wavelength=ssx_params["wavelength"],
         pump_status=True,
         pump_exp=ssx_params["pump_exp"],
         pump_delay=ssx_params["pump_delay"],
     )
+
+    logfile = SSX_TR.visitpath / "nexus_writer.log"
+    # Configure logging
+    log.config(logfile.as_posix())
+
     logger.info(
-        f"Start NeXus File Writer for time-resolved SSX on {source['beamline_name']}."
+        f"Start NeXus File Writer for time-resolved SSX on beamline {source['beamline_name']} at DLS."
     )
 
     # Add to dictionaries
     # Detector
     detector["starts"] = [0.0, SSX_TR.detector_distance]
     detector["exposure_time"] = SSX_TR.exposure_time
     detector["beam_center"] = SSX_TR.beam_center
@@ -208,15 +205,15 @@
                 logger.warning(
                     "Pump delay has not been recorded and won't be written to file."
                 )
             write_NXnote(nxsfile, "/entry/source/notes", pump_info)
 
             if timestamps[1]:
                 write_NXdatetime(nxsfile, (None, timestamps[1]))
-            logger.info(f"{master_file} correctly written.")
+            logger.info(f"The file {master_file} was written correctly.")
     except Exception as err:
         logger.exception(err)
         logger.info(
             f"An error occurred and {master_file} couldn't be written correctly."
         )
```

### Comparing `nexgen-0.6.8/src/nexgen/command_line/__init__.py` & `nexgen-0.6.9/src/nexgen/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.6.8/src/nexgen/command_line/copy_nexus.py` & `nexgen-0.6.9/src/nexgen/command_line/copy_nexus.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 import argparse
 import logging
 import sys
 from pathlib import Path
 
 import freephil
 
+from .. import log
 from ..nxs_copy import CopyNexus, CopyTristanNexus
 from . import full_copy_parser, tristan_copy_parser, version_parser
 
 # Define a logger object and a formatter
-logger = logging.getLogger("CopyNeXus")
-logger.setLevel(logging.DEBUG)
-formatter = logging.Formatter("%(levelname)s %(message)s")
+logger = logging.getLogger("nexgen.CopyNeXus")
 
 # Phil scopes
 general_scope = freephil.parse(
     """
     input{
       original_nexus = None
         .type = path
@@ -96,14 +95,17 @@
     params = working_phil.extract()
     working_phil.show()
 
     if args.show_config:
         working_phil.show(attributes_level=args.attributes_level)
         sys.exit()
 
+    # Configure logging
+    log.config()
+
     logger.info("Copy metadata from one NeXus file to another.")
 
     # Path to data file and original nexus file
     data_file = [Path(d).expanduser().resolve() for d in params.input.data_filename]
     nexus_file = Path(params.input.original_nexus).expanduser().resolve()
     logger.info(f"NeXus file to be copied: {nexus_file}")
     logger.info(f"Input data to be saved in NeXus file: {data_file}")
@@ -140,14 +142,17 @@
     params = working_phil.extract()
     working_phil.show()
 
     if args.show_config:
         working_phil.show(attributes_level=args.attributes_level)
         sys.exit()
 
+    # Configure logging
+    log.config()
+
     logger.info("Copy metadata from Tristan NeXus file.")
 
     # Path to data and original nexus file
     data_file = [Path(d).expanduser().resolve() for d in params.input.data_filename]
     nexus_file = Path(params.input.tristan_nexus).expanduser().resolve()
     logger.info(f"Working directory: {data_file[0].parent}")
     logger.info(f"NeXus file to be copied: {nexus_file}")
@@ -223,19 +228,12 @@
     ),
     parents=[tristan_copy_parser],
 )
 parser_tristan.set_defaults(func=copy_tristan_nexus)
 
 
 def main():
-    # Define a stream handler
-    CH = logging.StreamHandler(sys.stdout)
-    CH.setLevel(logging.DEBUG)
-    CH.setFormatter(formatter)
-    # Add handler to logger
-    logger.addHandler(CH)
-
     args = parser.parse_args()
     args.func(args)
 
 
 # main()
```

### Comparing `nexgen-0.6.8/src/nexgen/command_line/nexus_generator.py` & `nexgen-0.6.9/src/nexgen/command_line/nexus_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import h5py
 import numpy as np
 
 from .. import (
     get_filename_template,
     get_iso_timestamp,
     get_nexus_filename,
+    log,
     units_of_time,
 )
 from ..nxs_write.NexusWriter import (  # write_nexus_demo, write_nexus
     ScanReader,
     call_writers,
 )
 from ..nxs_write.NXclassWriters import write_NXdatetime, write_NXentry, write_NXnote
@@ -32,19 +33,16 @@
     add_tristan_spec,
     demo_parser,
     detectormode_parser,
     nexus_parser,
     version_parser,
 )
 
-# Define a logger object and a formatter
-logger = logging.getLogger("NeXusGenerator")
-logger.setLevel(logging.DEBUG)
-# formatter = logging.Formatter("%(levelname)s %(message)s")
-formatter = logging.Formatter("%(asctime)s %(name)s %(levelname)s %(message)s")
+# Define a logger object
+logger = logging.getLogger("nexgen.NeXusGenerator")
 
 # Phil scopes
 master_phil = freephil.parse(
     """
     output {
       master_filename = None
         .type = path
@@ -190,20 +188,18 @@
     if params.output.master_filename:
         master_file = Path(params.output.master_filename).expanduser().resolve()
     else:
         master_file = get_nexus_filename(datafiles[0])
 
     # Start logger
     logfile = master_file.parent / "generate_nexus.log"
-    # Define a file handler for logging
-    FH = logging.FileHandler(logfile, mode="a")
-    FH.setLevel(logging.DEBUG)
-    FH.setFormatter(formatter)
-    # Add handlers to logger
-    logger.addHandler(FH)
+    # Configure logging
+    log.config(logfile.as_posix())
+
+    logger.info("NeXus file writer for existing dataset.")
 
     # Add some information to logger
     logger.info("Create a NeXus file for %s" % datafiles[0])
     logger.info(
         "Number of experiment data files in directory, linked to the Nexus file: %d"
         % len(datafiles)
     )
@@ -298,15 +294,15 @@
     if TRANSL:
         logger.info(f"Scan along the {list(TRANSL.keys())} axes.")
         for k, v in TRANSL.items():
             logger.info(f"{k} scan from {v[0]} to {v[-1]}.")
     logger.info("\n")
 
     logger.info(
-        f"Detector information:\n {detector.description}, {detector.detector_type}"
+        f"Detector information: {detector.description}, {detector.detector_type}"
     )
     logger.info(
         f"Sensor made of {detector.sensor_material} x {detector.sensor_thickness}"
     )
     logger.info(f"Trusted pixels > {detector.underload} and < {detector.overload}")
     logger.info(
         f"Image is a {detector.image_size} array of {detector.pixel_size} pixels"
@@ -393,23 +389,23 @@
                 )
             else:
                 logger.info("VDS won't be written.")
 
             # Write /entry/start_time and /entry/end_time
             write_NXdatetime(nxsfile, timestamps)
 
-        logger.info(f"{master_file} correctly written.")
+        logger.info(f"The file {master_file} was written correctly.")
     except Exception as err:
         logger.info(
             f"An error occurred and {master_file} couldn't be written correctly."
         )
         logger.exception(err)
         # logger.error(err)
 
-    logger.info("EOF")
+    logger.info("EOF\n")
 
 
 def write_demo_cli(args):
     cl = demo_phil.command_line_argument_interpreter()
     working_phil = demo_phil.fetch(cl.process_and_fetch(args.phil_args))
     params = working_phil.extract()
 
@@ -421,20 +417,18 @@
     master_file = Path(params.output.master_filename).expanduser().resolve()
     # Just in case ...
     if master_file.suffix == ".h5" and "master" not in master_file.stem:
         master_file = Path(master_file.as_posix().replace(".h5", "_master.h5"))
 
     # Start logger
     logfile = master_file.parent / "generate_demo.log"
-    # Define a file handler for logging
-    FH = logging.FileHandler(logfile, mode="w")
-    FH.setLevel(logging.DEBUG)
-    FH.setFormatter(formatter)
-    # Add handlers to logger
-    logger.addHandler(FH)
+    # Configure logging
+    log.config(logfile.as_posix())
+
+    logger.info("Demo NeXus file writer with blank data HDF5 files.")
 
     # Get data file name template
     data_file_template = get_filename_template(master_file)
 
     # Add some information to logger
     logger.info("NeXus file will be saved as %s" % params.output.master_filename)
     logger.info("Data file(s) template: %s" % data_file_template)
@@ -495,15 +489,15 @@
     # Define rotation and translation axes
     OSC, TRANSL = ScanReader(
         goniometer.__dict__,
         data_type[0],
         n_images=data_type[1],
         snaked=params.input.snaked,
     )
-    print(OSC)
+
     # Log scan information
     logger.info(f"Rotation scan axis: {list(OSC.keys())[0]}.")
     logger.info(
         f"Scan from {list(OSC.values())[0][0]} to {list(OSC.values())[0][-1]}.\n"
     )
     if TRANSL:
         logger.info(f"Scan along the {list(TRANSL.keys())} axes.")
@@ -513,15 +507,15 @@
 
     # Fix the number of images if not passed from command line.
     if data_type[0] == "images" and data_type[1] is None:
         data_type = ("images", len(list(OSC.values())[0]))
         logger.warning(f"Total number of images updated to: {data_type[1]}")
         logger.warning("\n")
 
-    logger.info("Detector information:\n%s" % detector.description)
+    logger.info("Detector information: %s" % detector.description)
     logger.info(
         f"Sensor made of {detector.sensor_material} x {detector.sensor_thickness}"
     )
     if data_type[0] == "images":
         logger.info(f"Trusted pixels > {detector.underload} and < {detector.overload}")
     logger.info(
         f"Image is a {detector.image_size} array of {detector.pixel_size} pixels"
@@ -649,22 +643,22 @@
 
             # Write /entry/start_time and /entry/end_time
             timestamps = (get_iso_timestamp(start_time), get_iso_timestamp(end_time))
             logger.info("Writing timestamps to NeXus.")
             logger.info(f"Start time: {timestamps[0]}")
             logger.info(f"End time: {timestamps[1]}")
             write_NXdatetime(nxsfile, timestamps)
-        logger.info(f"{master_file} correctly written.")
+        logger.info(f"The file {master_file} was written correctly.")
     except Exception as err:
         logger.info(
             f"An error occurred and {master_file} couldn't be written correctly."
         )
         logger.exception(err)
 
-    logger.info("EOF")
+    logger.info("EOF\n")
 
 
 def write_with_meta_cli(args):
     cl = meta_phil.command_line_argument_interpreter()
     working_phil = meta_phil.fetch(cl.process_and_fetch(args.phil_args))
     params = working_phil.extract()
 
@@ -695,20 +689,18 @@
         ).as_posix()
         datafiles = [
             Path(d).expanduser().resolve() for d in sorted(glob.glob(datafile_pattern))
         ]
 
     # Start logger
     logfile = master_file.parent / "generate_nexus_from_meta.log"
-    # Define a file handler for logging
-    FH = logging.FileHandler(logfile, mode="a")
-    FH.setLevel(logging.DEBUG)
-    FH.setFormatter(formatter)
-    # Add handlers to logger
-    logger.addHandler(FH)
+    # Configure logging
+    log.config(logfile.as_posix())
+
+    logger.info("NeXus file writer for existing dataset with meta file available.")
 
     # Add some information to logger
     logger.info("Create a NeXus file for %s" % datafiles[0])
     logger.info(
         "Number of experiment data files in directory, linked to the Nexus file: %d"
         % len(datafiles)
     )
@@ -807,15 +799,15 @@
     logger.info("\n")
 
     if detector.description is None:
         logger.warning("No detector description provided, exit.")
         sys.exit("Please provide a detector description for identification.")
 
     logger.info(
-        f"Detector information:\n {detector.description}, {detector.detector_type}"
+        f"Detector information: {detector.description}, {detector.detector_type}"
     )
     logger.info(
         f"Sensor made of {detector.sensor_material} x {detector.sensor_thickness}"
     )
     logger.info(f"Trusted pixels > {detector.underload} and < {detector.overload}")
     logger.info(
         f"Image is a {detector.image_size} array of {detector.pixel_size} pixels"
@@ -917,22 +909,22 @@
                 )
             else:
                 logger.info("VDS won't be written.")
 
             # Write /entry/start_time and /entry/end_time
             write_NXdatetime(nxsfile, timestamps)
 
-            logger.info(f"{master_file} correctly written.")
+            logger.info(f"The file {master_file} was written correctly.")
     except Exception as err:
         logger.info(
             f"An error occurred and {master_file} couldn't be written correctly."
         )
         logger.exception(err)
 
-    logger.info("EOF")
+    logger.info("EOF\n")
 
 
 # Define subparsers
 subparsers = parser.add_subparsers(
     help="Choose whether to write a NXmx NeXus file for a collection or a demo. \
         Run generate_nexus <command> --help to see the parameters for each sub-command.",
     required=True,
@@ -970,18 +962,12 @@
     help="List of datasets that should not be overwritten even if present in meta file",
     type=str,
 )
 parser_NXmx_meta.set_defaults(func=write_with_meta_cli)
 
 
 def main():
-    # Define a stream handler
-    CH = logging.StreamHandler(sys.stdout)
-    CH.setLevel(logging.DEBUG)
-    CH.setFormatter(formatter)
-    logger.addHandler(CH)
-
     args = parser.parse_args()
     args.func(args)
 
 
 # main()
```

### Comparing `nexgen-0.6.8/src/nexgen/command_line/nxs_phil.py` & `nexgen-0.6.9/src/nexgen/command_line/nxs_phil.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,21 +109,21 @@
         .type = strings
         .help = "Axis units, from mm or deg"
       software_version = None
         .type = str
         .help = "Detector software version"
     }
     tristanSpec {
-      detector_tick = None          # 1562.5ps
+      detector_tick = 1562.5ps
         .type = str
         .help = "Tristan specific - detector tick, in ps"
-      detector_frequency = None     # 6.4e+08Hz
+      detector_frequency = 6.4e+08Hz
         .type = str
         .help = "Tristan specific - detector frequency, in Hz"
-      timeslice_rollover = None     # 18
+      timeslice_rollover = 18
         .type = int
         .help = "Tristan specific - timeslice rollover bits"
     }
     """
 )
 
 goniometer_scope = freephil.parse(
```

### Comparing `nexgen-0.6.8/src/nexgen/command_line/phil_files_cli.py` & `nexgen-0.6.9/src/nexgen/command_line/phil_files_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """
 Command line tool to get an existing .phil file with goniometer/detector metadata or to create a new one.
 These files can be used as input for the NeXus generator CLI.
 """
 
 import argparse
+import logging
 import shutil
 import sys
 
 import freephil
 
 try:
     from importlib.resources import files
 except ImportError:
     # Python < 3.9 compatibility
     from importlib_resources import files
 
 from pathlib import Path
 
-from .. import beamlines
+from .. import beamlines, log
 from . import nexus_parser, version_parser
 
+# Define a logger object
+logger = logging.getLogger("nexgen.NeXusGenerator")
+
 scopes = freephil.parse(
     """
     include scope nexgen.command_line.nxs_phil.goniometer_scope
     include scope nexgen.command_line.nxs_phil.beamline_scope
     include scope nexgen.command_line.nxs_phil.detector_scope
     include scope nexgen.command_line.nxs_phil.module_scope
     """,
@@ -58,43 +62,53 @@
 
 def get_beamline_phil(args):
     # Determine where to save file
     if args.output:
         odir = Path(args.output).expanduser().resolve()
     else:
         odir = Path(".").expanduser().resolve()
-        print(
+        logger.warning(
             "No output directory was specified by user. A copy of the file will be saved in the current directory."
         )
 
     # Look for file
     filedir = files(beamlines)
     found = [f for f in sorted(filedir.glob("*.phil")) if args.phil_file == f.name]
     if len(found) == 0:
-        print(f"No {args.phil_file} found.")
+        logger.info(f"No {args.phil_file} found.")
     elif len(found) == 1:
-        print(f"{args.phil_file} found. Copying in {odir}.")
+        logger.info(f"{args.phil_file} found. Copying in {odir}.")
         shutil.copy(found[0], odir)
 
 
 def create_new_phil(args):
     cl = scopes.command_line_argument_interpreter()
     working_phil = scopes.fetch(cl.process_and_fetch(args.phil_args))
 
     if args.show_config:
         working_phil.show(attributes_level=args.attributes_level)
         sys.exit()
 
+    if args.skip is True:
+        logger.warning(
+            "The scope containing Tristan specs will be removed before writing."
+        )
+        tristanSpec = [
+            obj for obj in working_phil.objects if "tristanSpec" in obj.as_str()
+        ][0]
+        working_phil.objects.remove(tristanSpec)
+
     # Write to file
     if args.filename:
         filename = Path(args.filename).expanduser().resolve()
+        logger.info(f"Writing new .phil file to {filename.name} in {filename.parent}.")
         with open(filename, "w") as fout:
             fout.write(working_phil.as_str())
     else:
-        print(working_phil.as_str())
+        logger.info(working_phil.as_str())
 
 
 # Define subparsers
 subparser = parser.add_subparsers(
     help="Run nexgen_phil <command> --help to see the options for each command.",
     required=True,
     dest="command",
@@ -120,19 +134,27 @@
     "new",
     description=("Write a new .phil file."),
     parents=[nexus_parser],
 )
 parser_create.add_argument(
     "-f", "--filename", type=str, help="Filename for new .phil template."
 )
-# TODO Find a way to avoid writing Tristan spec if detector is Eiger!
+parser_create.add_argument(
+    "-s",
+    "--skip",
+    help="Pass to avoid writing tristanSpec scope for non-Tristan detectors.",
+    action="store_true",
+)
 parser_create.set_defaults(func=create_new_phil)
 
 
 def main():
+    # Configure logging
+    log.config()
+
     args = parser.parse_args()
     if args.command == "list":
         args.func()
     else:
         args.func(args)
```

### Comparing `nexgen-0.6.8/src/nexgen/nxs_copy/CopyNexus.py` & `nexgen-0.6.9/src/nexgen/nxs_copy/CopyNexus.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import h5py
 
 from .. import get_nexus_filename
 from ..nxs_write import create_attributes
 from . import get_nexus_tree
 
-copy_logger = logging.getLogger("CopyNeXus.copy")
+copy_logger = logging.getLogger("nexgen.CopyNeXus")
 
 
 def images_nexus(
     data_file: List[Union[Path, str]],
     original_nexus: Optional[Union[Path, str]],
     simple_copy: bool = True,
     skip_group: List[str] = ["NXdata"],
```

### Comparing `nexgen-0.6.8/src/nexgen/nxs_copy/CopyTristanNexus.py` & `nexgen-0.6.9/src/nexgen/nxs_copy/CopyTristanNexus.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import h5py
 import numpy as np
 
 from ..nxs_write import create_attributes
 from . import convert_scan_axis, get_nexus_tree, identify_tristan_scan_axis
 
-tristan_logger = logging.getLogger("CopyNeXus.tristan")
+tristan_logger = logging.getLogger("nexgen.CopyTristanNeXus")
 
 
 def single_image_nexus(
     data_file: Optional[Union[Path, str]],
     tristan_nexus: Optional[Union[Path, str]],
     write_mode: str = "x",
 ) -> str:
@@ -25,21 +25,21 @@
 
     Copy the nexus tree from the original NeXus file for a collection on Tristan
     detector. In the case of a single image, the input scan_axis is a (start, stop) tuple where start and
     stop have the same value, for a pump-probe experiment the values might differ for some older datasets.
     The scan_axis in the new file will therefore be one single number, equal to the "start".
 
     Args:
-        data_file:      String or Path pointing to the HDF5 file containing the newly binned images.
-        tristan_nexus:  String or Path pointing to the input NeXus file with experiment metadata to be copied.
-        write_mode:     String indicating writing mode for the output NeXus file.  Accepts any valid
-                        h5py file opening mode.
+        data_file (Optional[Union[Path, str]]): String or Path pointing to the HDF5 file containing the newly binned images.
+        tristan_nexus (Optional[Union[Path, str]]): String or Path pointing to the input NeXus file with experiment metadata to be copied.
+        write_mode (str, optional): String indicating writing mode for the output NeXus file.  Accepts any valid
+                        h5py file opening mode. Defaults to "x".
 
     Returns:
-        nxs_filename:   The name of the output NeXus file.
+        nxs_filename (str): The name of the output NeXus file.
     """
     data_file = Path(data_file).expanduser().resolve()
     tristan_nexus = Path(tristan_nexus).expanduser().resolve()
     nxs_filename = data_file.parent / f"{data_file.stem}.nxs"
     with h5py.File(tristan_nexus, "r") as nxs_in, h5py.File(
         nxs_filename, write_mode
     ) as nxs_out:
@@ -95,23 +95,27 @@
     Copy the nexus tree from the original NeXus file for a collection on Tristan
     detector. In this case multiple images from a rotation collection have been
     binned and the scan_axis to be found in the input file is a (start, stop) tuple.
     The scan_axis in the new file will therefore be a list of angles.
     Osc and num_bins are mutually exclusive arguments to work out the scan_axis list.
 
     Args:
-        data_file:      String or Path pointing to the HDF5 file containing the newly binned images.
-        tristan_nexus:  String or Path pointing to the input NeXus file with experiment metadata to be copied.
-        write_mode:     String indicating writing mode for the output NeXus file.  Accepts any valid
-                        h5py file opening mode.
-        osc:            Oscillation angle (degrees).
-        nbins:          Number of binned images.
+        data_file (Optional[Union[Path, str]]): String or Path pointing to the HDF5 file containing the newly binned images.
+        tristan_nexus (Optional[Union[Path, str]]): String or Path pointing to the input NeXus file with experiment metadata to be copied.
+        write_mode (str, optional): String indicating writing mode for the output NeXus file.  Accepts any valid
+                        h5py file opening mode. Defaults to "x".
+        osc (float, optional): Oscillation angle (degrees). Defaults to None.
+        nbins (int, optional): Number of binned images. Defaults to None.
+
+    Raises:
+        ValueError: When both osc and nbins have been passed. The two values are mutually exclusive.
+        ValueError: When neither osc nor nbins has been passed. It won't be possible to calculate the scan range without at least one of them.
 
     Returns:
-        nxs_filename:   The name of the output NeXus file.
+        nxs_filename (str): The name of the output NeXus file.
     """
     data_file = Path(data_file).expanduser().resolve()
     tristan_nexus = Path(tristan_nexus).expanduser().resolve()
     nxs_filename = data_file.parent / f"{data_file.stem}.nxs"
     with h5py.File(tristan_nexus, "r") as nxs_in, h5py.File(
         nxs_filename, write_mode
     ) as nxs_out:
```

### Comparing `nexgen-0.6.8/src/nexgen/nxs_copy/__init__.py` & `nexgen-0.6.9/src/nexgen/nxs_copy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,23 +16,36 @@
 def h5str(h5_value: str | np.string_ | bytes) -> str:
     """
     Convert a value returned an h5py attribute to str.
 
     h5py can return either a bytes-like (numpy.string_) or str object
     for attribute values depending on whether the value was written as
     fixed or variable length. This function collapses the two to str.
+
+    Args:
+        h5_value (str | np.string_ | bytes): Original attribute value.
+
+    Returns:
+        str: Attribute value collapsed to str.
     """
     if isinstance(h5_value, (np.string_, bytes)):
         return h5_value.decode("utf-8")
     return h5_value
 
 
 def get_skip_list(nxentry: h5py.Group, skip_obj: list[str]) -> list[str]:
     """
-    Get a list of all the objects that hould not be copied in the nex NeXus file.
+    Get a list of all the objects that should not be copied in the new NeXus file.
+
+    Args:
+        nxentry (h5py.Group): "/entry/" group of a NeXus file.
+        skip_obj (list[str]): List of objects that should not be copied.
+
+    Returns:
+        list[str]: List of "NXclass" objects to skip during copy.
     """
     obj_list = walk_nxs(nxentry)
     skip_list = []
     for obj in obj_list:
         try:
             if nxentry[obj].attrs["NX_class"] in np.string_(skip_obj):
                 skip_list.append(obj)
```

### Comparing `nexgen-0.6.8/src/nexgen/nxs_write/NXclassWriters.py` & `nexgen-0.6.9/src/nexgen/nxs_write/NXclassWriters.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     split_arrays,
     units_of_length,
     units_of_time,
     ureg,
 )
 from . import calculate_origin, create_attributes, set_dependency
 
-NXclass_logger = logging.getLogger("NeXusGenerator.writer.NXclass")
+NXclass_logger = logging.getLogger("nexgen.NXclass_writers")
 NXclass_logger.setLevel(logging.DEBUG)
 
 
 # NXentry writer
 def write_NXentry(nxsfile: h5py.File, definition: str = "NXmx") -> h5py.Group:
     """
     Write NXentry group at top level of the NeXus file.
@@ -251,15 +251,18 @@
                         vectors[osc_axis],
                     ),
                 )
                 nxtransformations[ax] = nxsfile[nxax.name]
             # Write {axisname}_increment_set and {axis_name}_end datasets
             if data_type[0] == "images":
                 increment_set = np.repeat(goniometer["increments"][idx], len(osc_range))
-                nxsample_ax.create_dataset(ax + "_increment_set", data=increment_set)
+                nxsample_ax.create_dataset(
+                    ax + "_increment_set",
+                    data=goniometer["increments"][idx],
+                )  # increment_set
                 nxsample_ax.create_dataset(ax + "_end", data=osc_range + increment_set)
         elif ax in scan_axes:
             # For translations
             if (
                 "data" in nxsfile["/entry"].keys()
                 and ax in nxsfile["/entry/data"].keys()
             ):
@@ -844,8 +847,8 @@
 
     # Write datasets
     for k, v in info.items():
         if v:  # Just in case one value is not recorded and set as None
             if type(v) is str:
                 v = np.string_(v)
             nxnote.create_dataset(k, data=v)
-            NXclass_logger.info(f"{k} dataset writte in {loc}.")
+            NXclass_logger.info(f"{k} dataset written in {loc}.")
```

### Comparing `nexgen-0.6.8/src/nexgen/nxs_write/NexusWriter.py` & `nexgen-0.6.9/src/nexgen/nxs_write/NexusWriter.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 import numpy as np
 
 from .. import units_of_time
 from ..tools.DataWriter import generate_event_files, generate_image_files
 from ..tools.MetaReader import overwrite_beam, overwrite_detector
 from ..tools.VDS_tools import image_vds_writer, vds_file_writer
 from . import (
-    calculate_grid_scan_range,
-    calculate_rotation_scan_range,
+    calculate_scan_range,
     find_grid_scan_axes,
     find_number_of_images,
     find_osc_axis,
 )
 from .NXclassWriters import (
     write_NXdata,
     write_NXdatetime,
@@ -86,41 +85,45 @@
     osc_axis = find_osc_axis(
         goniometer.axes, goniometer.starts, goniometer.ends, goniometer.types
     )
     idx = goniometer.axes.index(osc_axis)
 
     if detector.mode == "events":
         data_type = ("events", len(datafiles))
-        osc_range = (goniometer.starts[idx], goniometer.ends[idx])
+        OSC = {osc_axis: (goniometer.starts[idx], goniometer.ends[idx])}
     else:
         # Find total number of images that have been written across the files.
         if len(datafiles) == 1:
             with h5py.File(datafiles[0], "r") as f:
                 num_images = f["data"].shape[0]
         else:
             num_images = find_number_of_images(datafiles)
         data_type = ("images", num_images)
         writer_logger.info(f"Total number of images: {num_images}")
 
         # Compute rotation scan_range
         if goniometer.increments[idx] != 0.0:
-            osc_range = calculate_rotation_scan_range(
-                goniometer.starts[idx],
-                goniometer.ends[idx],
-                axis_increment=goniometer.increments[idx],
+            OSC = calculate_scan_range(
+                [osc_axis],
+                [goniometer.starts[idx]],
+                [goniometer.ends[idx]],
+                axes_increments=[goniometer.increments[idx]],
+                rotation=True,
             )
         else:
-            osc_range = calculate_rotation_scan_range(
-                goniometer.starts[idx], goniometer.ends[idx], n_images=num_images
+            OSC = calculate_scan_range(
+                [osc_axis],
+                [goniometer.starts[idx]],
+                [goniometer.ends[idx]],
+                n_images=num_images,
+                rotation=True,
             )
 
-    OSC = {osc_axis: osc_range}
-
     writer_logger.info(f"Rotatin scan axis: {osc_axis}")
-    writer_logger.info(f"Scan from {osc_range[0]} tp {osc_range[-1]}.")
+    writer_logger.info(f"Scan from {OSC[osc_axis][0]} tp {OSC[osc_axis][-1]}.")
 
     # Look for a translation scan (usually on xy)
     transl_axes = find_grid_scan_axes(
         goniometer.axes, goniometer.starts, goniometer.ends, goniometer.types
     )
     # If xy scan axes are identified, add to dictionary
     if len(transl_axes) > 0:
@@ -131,15 +134,15 @@
         transl_increments = [goniometer.increments[i] for i in tr_idx]
         for tr in range(len(transl_axes)):
             writer_logger.info(
                 f"{transl_axes[tr]} scan from {transl_starts[tr]} to {transl_ends[tr]}, with a step of {transl_increments[tr]}"
             )
         # TODO decide what to do for n_images=(nx,ny) in this case...
         # Tbh, it should work without it anyway
-        transl_range = calculate_grid_scan_range(
+        transl_range = calculate_scan_range(
             transl_axes,
             transl_starts,
             transl_ends,
             transl_increments,
         )  # NB. leaving snaked = False for demo. TODO change at some point.
         TRANSL = transl_range
 
@@ -250,61 +253,69 @@
         transl_starts = [goniometer.starts[i] for i in tr_idx]
         transl_ends = [goniometer.ends[i] for i in tr_idx]
         transl_increments = [goniometer.increments[i] for i in tr_idx]
         for tr in range(len(transl_axes)):
             writer_logger.info(
                 f"{transl_axes[tr]} scan from {transl_starts[tr]} to {transl_ends[tr]}, with a step of {transl_increments[tr]}"
             )
-        transl_range = calculate_grid_scan_range(
+        transl_range = calculate_scan_range(
             transl_axes,
             transl_starts,
             transl_ends,
             transl_increments,
         )  # NB. leaving snaked = False for demo. TODO change at some point.
         TRANSL = transl_range
     else:
         TRANSL = {}
 
     # TODO FIXME the number of images should come from CLI if it's a xy scan.
     # Compute scan_range for rotation axis
     idx = goniometer.axes.index(osc_axis)
     if data_type[0] == "images":
         if data_type[1] is None and len(transl_axes) == 0:
-            osc_range = calculate_rotation_scan_range(
-                goniometer.starts[idx],
-                goniometer.ends[idx],
-                axis_increment=goniometer.increments[idx],
+            OSC = calculate_scan_range(
+                [osc_axis],
+                [goniometer.starts[idx]],
+                [goniometer.ends[idx]],
+                axes_increments=[goniometer.increments[idx]],
+                rotation=True,
             )
-            data_type = ("images", len(osc_range))
+            data_type = ("images", len(OSC[osc_axis]))
         elif data_type[1] is None and len(transl_axes) > 0:
             ax1 = transl_axes[0]
             num_imgs = len(transl_range[ax1])
-            osc_range = calculate_rotation_scan_range(
-                goniometer.starts[idx], goniometer.ends[idx], n_images=num_imgs
+            OSC = calculate_scan_range(
+                [osc_axis],
+                [goniometer.starts[idx]],
+                [goniometer.ends[idx]],
+                n_images=num_imgs,
+                rotation=True,
             )
             data_type = ("images", num_imgs)
         else:
             ax1 = transl_axes[0]
             if data_type[1] != len(transl_range[ax1]):
                 raise ValueError(
                     "The total number of images doesn't match the number of scan points, please double check the input."
                 )
             # assert data_type[1] == len(
             #     transl_range[ax1]
             # ), "The total number of images doesn't match the number of scan points, please double check the input."
-            osc_range = calculate_rotation_scan_range(
-                goniometer.starts[idx], goniometer.ends[idx], n_images=data_type[1]
+            OSC = calculate_scan_range(
+                [osc_axis],
+                [goniometer.starts[idx]],
+                [goniometer.ends[idx]],
+                n_images=data_type[1],
+                rotation=True,
             )
     elif data_type[0] == "events":
-        osc_range = (goniometer.starts[idx], goniometer.ends[idx])
-
-    OSC = {osc_axis: osc_range}
+        OSC = {osc_axis: (goniometer.starts[idx], goniometer.ends[idx])}
 
     writer_logger.info(f"Rotation scan axis: {osc_axis}.")
-    writer_logger.info(f"Scan from {osc_range[0]} to {osc_range[-1]}.")
+    writer_logger.info(f"Scan from {OSC[osc_axis][0]} to {OSC[osc_axis][-1]}.")
 
     # Figure out how many files will need to be written
     writer_logger.info("Calculating number of files to write ...")
     if data_type[0] == "events":
         # Determine the number of files. Write one file per module.
         # FIXME Either a 10M or a 2M, no other possibilities at this moment.
         n_files = 10 if "10M" in detector.description.upper() else 2
@@ -366,34 +377,37 @@
     else:
         writer_logger.info("VDS won't be written.")
 
 
 def ScanReader(
     goniometer: Dict,
     data_type: str = "images",
-    n_images: int = None,
-    snaked: bool = False,
+    n_images: Union[int, Tuple] = None,
+    snaked: bool = True,
 ) -> Tuple[Dict, Dict]:
     """
     Read the information passed from the goniometer and return a definition of the scan.
 
     Args:
         goniometer (Dict): Goniometer geometry definition.
         data_type (str, optional): Type of data being written, can be images of events. Defaults to "images".
-        n_images (int, optional): Total number of images to write. If passed, \
-                                    the number of images will override the axis_increment value of the rotation scan. Defaults to None.
-        snaked (bool, optional): 2D scan parameter. If True, defines a snaked grid scan. Defaults to False.
+        n_images (Union[int, Tuple], optional): Total number of images to write. If passed, \
+                                    the number of images will override the axis_increment value of the rotation scan. \
+                                    Defaults to None.
+        snaked (bool, optional): 2D scan parameter. If True, defines a snaked grid scan. Defaults to True.
 
     Raises:
         ValueError: If the total number of images passed doesn't match the number of scan points when dealing with a 2D/3D scan.
 
     Returns:
-        Tuple[Dict,Dict]: Two separate dictionaries. The first defines the rotation scan, the second the linear/grid scan. \
+        Tuple[Dict, Dict]: Two separate dictionaries. The first defines the rotation scan, the second the linear/grid scan. \
                             When dealing with a set of stills or a simple rotation scan, the second value will return None.
     """
+    logger = logging.getLogger("nexgen.ScanReader")
+    logger.setLevel(logging.DEBUG)
     # First find which axes deifne a rotation/translation scan
     osc_axis = find_osc_axis(
         goniometer["axes"],
         goniometer["starts"],
         goniometer["ends"],
         goniometer["types"],
     )
@@ -407,66 +421,89 @@
 
     # If there's a linear/grid scan, get dictionary
     if len(transl_axes) > 0:
         transl_idx = [goniometer["axes"].index(j) for j in transl_axes]
         transl_start = [goniometer["starts"][i] for i in transl_idx]
         transl_end = [goniometer["ends"][i] for i in transl_idx]
         transl_increment = [goniometer["increments"][i] for i in transl_idx]
-        TRANSL = calculate_grid_scan_range(
-            transl_axes, transl_start, transl_end, transl_increment, snaked=snaked
-        )
+        if n_images and type(n_images) is int:
+            TRANSL = calculate_scan_range(
+                transl_axes,
+                transl_start,
+                transl_end,
+                transl_increment,
+                # (n_images,),
+                snaked=snaked,
+            )
+        elif n_images and type(n_images) is tuple:
+            TRANSL = calculate_scan_range(
+                transl_axes, transl_start, transl_end, n_images=n_images, snaked=snaked
+            )
+        else:
+            TRANSL = calculate_scan_range(
+                transl_axes, transl_start, transl_end, transl_increment, snaked=snaked
+            )
+        logger.info(f"{len(transl_axes)} scan axis/axes found (translation).")
     else:
         TRANSL = None
 
     # Once that's defined, go through the various cases
     # Return either 2 dictionaries or (Dict, None)
     if data_type == "events" and len(transl_axes) == 0:
-        osc_range = (goniometer["starts"][osc_idx], goniometer["ends"][osc_idx])
+        OSC = {osc_axis: (goniometer["starts"][osc_idx], goniometer["ends"][osc_idx])}
     elif data_type == "events" and len(transl_axes) > 0:
-        osc_range = (goniometer["starts"][osc_idx], goniometer["ends"][osc_idx])
+        OSC = {osc_axis: (goniometer["starts"][osc_idx], goniometer["ends"][osc_idx])}
         # Overwrite TRANSL
         for k, s, e in zip(transl_axes, transl_start, transl_end):
             TRANSL[k] = (s, e)
     else:
         if n_images is None and len(transl_axes) == 0:
-            osc_range = calculate_rotation_scan_range(
-                goniometer["starts"][osc_idx],
-                goniometer["ends"][osc_idx],
-                axis_increment=goniometer["increments"][osc_idx],
+            OSC = calculate_scan_range(
+                [osc_axis],
+                [goniometer["starts"][osc_idx]],
+                [goniometer["ends"][osc_idx]],
+                axes_increments=[goniometer["increments"][osc_idx]],
+                rotation=True,
             )
         elif n_images is None and len(transl_axes) > 0:
             ax = transl_axes[0]
             n_images = len(TRANSL[ax])
-            osc_range = calculate_rotation_scan_range(
-                goniometer["starts"][osc_idx],
-                goniometer["ends"][osc_idx],
+            OSC = calculate_scan_range(
+                [osc_axis],
+                [goniometer["starts"][osc_idx]],
+                [goniometer["ends"][osc_idx]],
                 n_images=n_images,
+                rotation=True,
             )
         elif n_images is not None and len(transl_axes) > 0:
             ax = transl_axes[0]
+            n_images = np.prod(n_images) if type(n_images) is tuple else n_images
             if n_images != len(TRANSL[ax]):
                 raise ValueError(
                     "The value passed as the total number of images doesn't match the number of scan points, please check the input."
                 )
-            # FIXME alternatively I could write a warning message and force it to
-            # obey one or the other directive. TBD
-            osc_range = calculate_rotation_scan_range(
-                goniometer["starts"][osc_idx],
-                goniometer["ends"][osc_idx],
+            #
+            OSC = calculate_scan_range(
+                [osc_axis],
+                [goniometer["starts"][osc_idx]],
+                [goniometer["ends"][osc_idx]],
                 n_images=n_images,
+                rotation=True,
             )
         else:
-            osc_range = calculate_rotation_scan_range(
-                goniometer["starts"][osc_idx],
-                goniometer["ends"][osc_idx],
-                axis_increment=goniometer["increments"][osc_idx],
+            n_images = np.prod(n_images) if type(n_images) is tuple else n_images
+            OSC = calculate_scan_range(
+                [osc_axis],
+                [goniometer["starts"][osc_idx]],
+                [goniometer["ends"][osc_idx]],
                 n_images=n_images,
+                rotation=True,
             )
 
-    OSC = {osc_axis: osc_range}
+    # logger.info(f"{osc_axis} set as rotation axis.")
     return OSC, TRANSL
 
 
 # def call_writers(*args,**kwargs):
 def call_writers(
     nxsfile: h5py.File,
     datafiles: List[Union[Path, str]],
@@ -498,15 +535,15 @@
         beam (Dict): Beam properties.
         attenuator (Dict): Attenuator properties.
         osc_scan (Dict): Axis defining the rotation scan. It should be passed even when still.
         transl_scan (Dict, optional): Axes defining a linear or 2D scan. Defaults to None.
         metafile (Union[Path, str], optional): File containing the metadata. Defaults to None.
         link_list (List, optional): List of datasets that can be copied from the metafile. Defaults to None.
     """
-    logger = logging.getLogger("NeXusGenerator.writer")
+    logger = logging.getLogger("nexgen.Call")
     logger.setLevel(logging.DEBUG)
     logger.info("Calling the writers ...")
 
     # Check that filenames are paths
     if all(isinstance(f, Path) for f in datafiles) is False:
         datafiles = [Path(f).expanduser().resolve() for f in datafiles]
```

### Comparing `nexgen-0.6.8/src/nexgen/nxs_write/__init__.py` & `nexgen-0.6.9/src/nexgen/nxs_write/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Utilities for writing new NeXus format files.
 """
 
+from __future__ import annotations
+
 import math
 from pathlib import Path
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Tuple
 
 import h5py
 import numpy as np
 from h5py import AttributeManager
 from scanspec.core import Path as ScanPath
 from scanspec.specs import Line
 
 
-def create_attributes(
-    nxs_obj: Union[h5py.Group, h5py.Dataset], names: Tuple, values: Tuple
-):
+def create_attributes(nxs_obj: h5py.Group | h5py.Dataset, names: Tuple, values: Tuple):
     """
     Create or overwrite attributes with additional metadata information.
 
     Args:
         nxs_obj:    NeXus object (Group or Dataset) to which the attributes should be attached
         names:      Tuple containing the names of the new attributes
         values:     Tuple containing the values relative to the names
@@ -33,16 +33,16 @@
 
 def set_dependency(dep_info: str, path: str = None):
     """
     Define value for "depends_on" attribute.
     If the attribute points to the head of the dependency chain, simply pass "." for dep_info.
 
     Args:
-        dep_info:   The name of the transformation upon which the current one depends on.
-        path:       Where the transformation is. Set to None, if passed it points to location in the NeXus tree.
+        dep_info (str): The name of the transformation upon which the current one depends on.
+        path (str): Where the transformation is. Set to None, if passed it points to location in the NeXus tree.
     Returns:
         The value to be passed to the attribute "depends_on"
     """
     if dep_info == ".":
         return np.string_(".")
     if path:
         if path.endswith("/") is False:
@@ -64,21 +64,21 @@
 
     This function identifies the scan axis from the list passed as argument.
     The scan axis is the one where start and end value are not the same.
     If there is only one rotation axis, that is the one returned.
     In the case scan axis cannot be identified, a default value is arbitrarily assigned.
 
     Args:
-        axes_names (list):      List of names associated to goniometer axes.
-        axes_starts (list):     List of start values.
-        axes_ends (list):       List of end values.
-        axes_types (list):      List of axes types, useful to identify only the rotation axes.
-        default (str):          String to deafult to in case scan axis is not found.
+        axes_names (list): List of names associated to goniometer axes.
+        axes_starts (list): List of start values.
+        axes_ends (list): List of end values.
+        axes_types (list): List of axes types, useful to identify only the rotation axes.
+        default (str): String to deafult to in case scan axis is not found.
     Returns:
-        scan_axis (str):        String identifying the rotation scan axis.
+        scan_axis (str): String identifying the rotation scan axis.
     """
     # This assumes that at least one rotation axis is always passed.
     # Assuming all list are of the same length ...
     if len(axes_names) == 0:
         raise ValueError(
             "Impossible to determine translation scan. No axes passed to find_osc_axis function. Please make sure at least one value is passed."
         )
@@ -99,43 +99,14 @@
         elif idx.count(True) == 1:
             scan_axis = axes_names[idx.index(True)]
         else:
             raise ValueError("Unable to correctly identify the rotation scan axis.")
     return scan_axis
 
 
-def calculate_rotation_scan_range(
-    axis_start: float,
-    axis_end: float,
-    axis_increment: float = None,
-    n_images: int = None,
-) -> np.ndarray:
-    """
-    Calculate the scan range for a rotation collection and return as a numpy array.
-    For this calculation axes_increments and n_images are mutually exclusive.
-    If there are multiple images but no rotation scan, return a numpy array of axis_start repeated n_images times.
-
-    Args:
-        axis_start (float):         Rotation axis position at the beginning of the scan, float.
-        axis_end (float):           Rotation axis position at the end of the scan, float.
-        axis_increment (float):     Range through which the axis moves each frame, float.
-        n_images (int):             Alternatively, number of images, int.
-    Returns:
-        scan_range (np.ndarray):    Numpy array of values for the rotation axis.
-    """
-    if n_images:
-        if axis_start == axis_end:
-            scan_range = np.repeat(axis_start, n_images)
-        else:
-            scan_range = np.linspace(axis_start, axis_end, n_images)
-    else:
-        scan_range = np.arange(axis_start, axis_end, axis_increment)
-    return scan_range
-
-
 def find_grid_scan_axes(
     axes_names: List,
     axes_starts: List,
     axes_ends: List,
     axes_types: List,
 ) -> List[str]:
     """
@@ -144,15 +115,15 @@
     Args:
         axes_names (List): List of names associated to goniometer axes.
         axes_starts (List): List of start values.
         axes_ends (List): List of end values.
         axes_types (List): List of axes types, useful to identify only the translation axes.
 
     Returns:
-        List[str]: List of strings identifying the linear/grid scan axes. If no axes are identified, it will return an empty list.
+        scan_axis (List[str]): List of strings identifying the linear/grid scan axes. If no axes are identified, it will return an empty list.
     """
     if len(axes_names) == 0:
         raise ValueError(
             "Impossible to determine translation scan. No axes passed to find_grid_scan_axes function. Please make sure at least one value is passed."
         )
 
     # Look only at translation axes
@@ -164,74 +135,125 @@
     scan_axis = []
     for n, ax in enumerate(axes_names):
         if axes_starts[n] != axes_ends[n]:
             scan_axis.append(ax)
     return scan_axis
 
 
-def calculate_grid_scan_range(
+def calculate_scan_range(
     axes_names: List,
     axes_starts: List,
     axes_ends: List,
-    axes_increments: List,
-    n_images: Union[Tuple, int] = None,
-    snaked: bool = False,
+    axes_increments: List = None,
+    n_images: Tuple | int = None,
+    snaked: bool = True,
+    rotation: bool = False,
 ) -> Dict[str, np.ndarray]:
     """
-    Calculate the scan range for a linear/grid scan from the number of images to be written.
-    If the number of images is not provided, it can be calculated from the increment value of the axis.
+    Calculate the scan range for a linear/grid scan or a rotation scan from the number of images to be written.
+    If the number of images is not provided, it can be calculated from the increment value of the axis (these values are mutually exclusive).
+    When dealing with a rotation axis, if there are multiple images but no rotation scan, return axis_start repeated n_images times.
 
     Args:
         axes_names (List): List of names for the axes involved in the scan.
         axes_starts (List): List of axis positions at the beginning of the scan.
         axes_ends (List): List of axis positions at the end of the scan.
-        axes_increments (List, optional): List of ranges through which the axes move each frame.
-        n_images (Tuple|int, optional): Number of images to be written. If writing a 2D scan, it should be a (nx, ny) tuple, \
+        axes_increments (List, optional): List of ranges through which the axes move each frame. Mostly used for rotation scans. Defaults to None.
+        n_images (Tuple | int, optional): Number of images to be written. If writing a 2D scan, it should be a (nx, ny) tuple, \
                                         where tot_n_img=nx*ny, any int value is at this time ignored. Defaults to None.
-        snaked (bool): If True, scanspec will "draw" a snaked grid. Defaults to False.
+        snaked (bool): If True, scanspec will "draw" a snaked grid. Defaults to True.
+        rotation (bool): Tell the function to calculate a rotation scan. Defaults to False.
+
+    Raises:
+        TypeError: If the input axes are not lists.
+        ValueError: When an empty axes names list has been passed.
+        ValueError: When both axes_increments and n_images have been passed. The two values are mutually exclusive.
+        ValueError: When neither axes_increments not n_images have been passed.
+        ValueError: For a grid scan, if axes_increments is None, n_images must be a tuple of len=2 to be sure to accurately calculate the scan points.
 
     Returns:
         Dict[str, np.ndarray]: A dictionary of ("axis_name": axis_range) key-value pairs.
     """
-    if len(axes_names) == 1:
+    if type(axes_names) != list or type(axes_starts) != list or type(axes_ends) != list:
+        raise TypeError("Input values for axes must be passed as lists.")
+
+    if len(axes_names) == 0:
+        raise ValueError("No axes have been passed, impossible to determine scan.")
+
+    if n_images and axes_increments:
+        raise ValueError(
+            "The axes_increments and n_images arguments are mutually exclusive. Please pass just one of those."
+            "For a 2D scan it is recommended that n_images is passed."
+        )
+    elif not n_images and not axes_increments:
+        raise ValueError(
+            "Impossible to calculate scan points, please pass either the axes increment values or the number of scan points (n_images) per axis."
+            "For a 2D scan it is recommended that n_images is passed."
+        )
+
+    if len(axes_names) == 1 and rotation is True:
         if not n_images:
-            n_images = int(abs(axes_starts[0] - axes_ends[0]) / axes_increments[0])
+            n_images = round(abs(axes_starts[0] - axes_ends[0]) / axes_increments[0])
+
+        if axes_starts[0] != axes_ends[0] and axes_increments:
+            axes_ends[0] = axes_ends[0] - axes_increments[0]
+        elif axes_starts[0] != axes_ends[0] and not axes_increments:
+            inc = (axes_ends[0] - axes_starts[0]) / n_images
+            axes_ends[0] = axes_ends[0] - inc
+
+        spec = Line(axes_names[0], axes_starts[0], axes_ends[0], n_images)
+        scan_path = ScanPath(spec.calculate())
+
+    elif len(axes_names) == 1 and rotation is False:
+        if not n_images:
+            # FIXME This calculation still gives the wrong increment between scan points.
+            n_images = (
+                round(abs(axes_starts[0] - axes_ends[0]) / axes_increments[0]) + 1
+            )
+        elif type(n_images) is tuple and len(n_images) == 1:
+            # This is mostly a double paranoid check
+            n_images = n_images[0]
+
         spec = Line(axes_names[0], axes_starts[0], axes_ends[0], n_images)
         scan_path = ScanPath(spec.calculate())
+
     else:
-        n_images0 = int(abs(axes_starts[0] - axes_ends[0]) / axes_increments[0])
-        n_images1 = int(abs(axes_starts[1] - axes_ends[1]) / axes_increments[1])
-        if n_images and type(n_images) is tuple:
-            # Overwrite
+        if not n_images:
+            # FIXME This calculation still gives the wrong increment between scan points.
+            n_images0 = (
+                round(abs(axes_starts[0] - axes_ends[0]) / axes_increments[0]) + 1
+            )
+            n_images1 = (
+                round(abs(axes_starts[1] - axes_ends[1]) / axes_increments[1]) + 1
+            )
+        elif len(n_images) == 1:
+            raise ValueError(
+                "Impossible to correctly calculate scan points from just the total number of images."
+                "Please either pass a tuple with the number of scan point per axis or the axes increments."
+            )
+        else:
             n_images0 = n_images[0]
             n_images1 = n_images[1]
-        # if not n_images:
-        #     n_images0 = int(abs(axes_starts[0] - axes_ends[0]) / axes_increments[0])
-        #     n_images1 = int(abs(axes_starts[1] - axes_ends[1]) / axes_increments[1])
-        # else:
-        #     # FIXME Need to be careful with n_images, it's not the total that should be passed here.
-        #     # Tot number of images (those passed in CLI or from beamline I guess) = n0*n1
-        #     n_images0 = n_images[0]
-        #     n_images1 = n_images[1]
+
         if snaked is True:
             spec = Line(axes_names[0], axes_starts[0], axes_ends[0], n_images0) * ~Line(
                 axes_names[1], axes_starts[1], axes_ends[1], n_images1
             )
         else:
             spec = Line(axes_names[0], axes_starts[0], axes_ends[0], n_images0) * Line(
                 axes_names[1], axes_starts[1], axes_ends[1], n_images1
             )
         scan_path = ScanPath(spec.calculate())
 
     return scan_path.consume().midpoints
 
 
 def calculate_origin(
-    beam_center_fs: Union[List, Tuple],
-    fs_pixel_size: Union[List, Tuple],
+    beam_center_fs: List | Tuple,
+    fs_pixel_size: List | Tuple,
     fast_axis_vector: Tuple,
     slow_axis_vector: Tuple,
     mode: str = "1",
 ):
     """
     Calculate the offset of the detector.
 
@@ -262,21 +284,22 @@
     if mode == "1":
         offset_val = 1.0
     else:
         offset_val = math.hypot(*det_origin[:-1])
     return det_origin, offset_val
 
 
-def find_number_of_images(datafile_list: List[Path]):
+def find_number_of_images(datafile_list: List[Path]) -> int:
     """
     Calculate total number of images when there's more than one input HDF5 file.
 
     Args:
-        datafiles:  List of paths to the input image files.
+        datafile_list (List[Path]): List of paths to the input image files.
+
     Returns:
-        num_images: Total number of images.
+        num_images (int): Total number of images._summary_
     """
     num_images = 0
     for filename in datafile_list:
         with h5py.File(filename, "r") as f:
             num_images += f["data"].shape[0]
-    return num_images
+    return int(num_images)
```

### Comparing `nexgen-0.6.8/src/nexgen/tools/DataWriter.py` & `nexgen-0.6.9/src/nexgen/tools/DataWriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from typing import List, Tuple, Union
 
 import h5py
 import numpy as np
 from hdf5plugin import Bitshuffle
 
-data_logger = logging.getLogger("NeXusGenerator.writer.data")
+data_logger = logging.getLogger("nexgen.DataWriter")
 
 # Random number generator
 rng = np.random.default_rng()
 
 # Eiger specific
 eiger_modules = {"1M": (1, 2), "4M": (2, 4), "9M": (3, 6), "16M": (4, 8)}
 eiger_mod_size = (512, 1028)
```

### Comparing `nexgen-0.6.8/src/nexgen/tools/ExtendedRequest.py` & `nexgen-0.6.9/src/nexgen/tools/ExtendedRequest.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.6.8/src/nexgen/tools/GDAjson2params.py` & `nexgen-0.6.9/src/nexgen/tools/GDAjson2params.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.6.8/src/nexgen/tools/MetaReader.py` & `nexgen-0.6.9/src/nexgen/tools/MetaReader.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import h5py
 
 from .. import units_of_length
 from .Metafile import DectrisMetafile, TristanMetafile
 
 # TODO actually define the type for scope extract and replace Any with Union
-overwrite_logger = logging.getLogger("NeXusGenerator.writer.from_meta")
+overwrite_logger = logging.getLogger("nexgen.MetaReader")
 overwrite_logger.setLevel(logging.DEBUG)
 
 
 def overwrite_beam(meta_file: h5py.File, name: str, beam: Any):
     """
     Looks for the wavelength value in the _meta.h5 file.
     If found, it overwrites the value that was parsed from the command line.
@@ -31,15 +31,15 @@
         if wl is None:
             overwrite_logger.info("No wavelength information found in meta file.")
             return
     else:
         raise ValueError("Unknown detector: please pass a valid detector description.")
     # If value exists, overwrite. Otherwise, create.
     overwrite_logger.warning("Wavelength will be overwritten.")
-    overwrite_logger.info(f"Value for wavelngth found in meta file: {wl}")
+    overwrite_logger.info(f"Value for wavelength found in meta file: {wl}")
     if type(beam) is dict:
         beam["wavelength"] = wl
     else:
         try:
             beam.__dict__["wavelength"] = wl
         except KeyError:
             beam.__inject__("wavelength", wl)
```

### Comparing `nexgen-0.6.8/src/nexgen/tools/Metafile.py` & `nexgen-0.6.9/src/nexgen/tools/Metafile.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.6.8/src/nexgen.egg-info/PKG-INFO` & `nexgen-0.6.9/src/nexgen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexgen
-Version: 0.6.8
+Version: 0.6.9
 Summary: Next Generation Nexus Generator
 Home-page: UNKNOWN
 Author: Diamond Light Source - Scientific Software
 Author-email: scientificsoftware@diamond.ac.uk
 License: BSD 3-Clause License
 Project-URL: Documentation, https://nexgen.readthedocs.io/
 Project-URL: GitHub, https://github.com/dials/nexgen
```

### Comparing `nexgen-0.6.8/src/nexgen.egg-info/SOURCES.txt` & `nexgen-0.6.9/src/nexgen.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 src/nexgen/__init__.py
+src/nexgen/log.py
 src/nexgen.egg-info/PKG-INFO
 src/nexgen.egg-info/SOURCES.txt
 src/nexgen.egg-info/dependency_links.txt
 src/nexgen.egg-info/entry_points.txt
 src/nexgen.egg-info/not-zip-safe
 src/nexgen.egg-info/requires.txt
 src/nexgen.egg-info/top_level.txt
```

