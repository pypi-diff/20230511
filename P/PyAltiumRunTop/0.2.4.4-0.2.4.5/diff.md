# Comparing `tmp/PyAltiumRunTop-0.2.4.4.tar.gz` & `tmp/PyAltiumRunTop-0.2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAltiumRunTop-0.2.4.4.tar", last modified: Mon Mar  6 02:14:23 2023, max compression
+gzip compressed data, was "PyAltiumRunTop-0.2.4.5.tar", last modified: Thu May 11 09:28:37 2023, max compression
```

## Comparing `PyAltiumRunTop-0.2.4.4.tar` & `PyAltiumRunTop-0.2.4.5.tar`

### file list

```diff
@@ -1,35 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.707089 PyAltiumRunTop-0.2.4.4/
--rw-rw-rw-   0        0        0     1051 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/LICENSE
--rw-rw-rw-   0        0        0       33 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2735 2023-03-06 02:14:23.707089 PyAltiumRunTop-0.2.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     1879 2023-03-02 09:07:41.000000 PyAltiumRunTop-0.2.4.4/README.md
--rw-rw-rw-   0        0        0      819 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/pyproject.toml
--rw-rw-rw-   0        0        0     1228 2023-03-06 02:14:23.708086 PyAltiumRunTop-0.2.4.4/setup.cfg
--rw-rw-rw-   0        0        0       69 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.687668 PyAltiumRunTop-0.2.4.4/src/
-drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.697113 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/
--rw-rw-rw-   0        0        0     2672 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      575 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 09:14:50.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       73 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.698113 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/
--rw-rw-rw-   0        0        0    14566 2023-03-03 06:17:54.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/AltiumRun.py
--rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.704097 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/helpers/
--rw-rw-rw-   0        0        0     1987 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/helpers/AltiumHelper.py
--rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/helpers/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/py.typed
-drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.706091 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/
--rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/__init__.py
--rw-rw-rw-   0        0        0      525 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/logger.pas
--rw-rw-rw-   0        0        0      478 2023-02-27 09:06:28.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/main.pas
--rw-rw-rw-   0        0        0     7285 2023-03-06 02:14:13.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/updateSitNum0302.pas
-drwxrwxrwx   0        0        0        0 2023-03-06 02:14:23.702102 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/
--rw-rw-rw-   0        0        0     2735 2023-03-06 02:14:23.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      903 2023-03-06 02:14:23.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 02:14:23.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 09:40:41.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       73 2023-03-06 02:14:23.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-06 02:14:23.000000 PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.789040 PyAltiumRunTop-0.2.4.5/
+-rw-rw-rw-   0        0        0     1051 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2801 2023-05-11 09:28:37.789040 PyAltiumRunTop-0.2.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1943 2023-03-08 01:12:55.000000 PyAltiumRunTop-0.2.4.5/README.md
+-rw-rw-rw-   0        0        0      819 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1228 2023-05-11 09:28:37.790036 PyAltiumRunTop-0.2.4.5/setup.cfg
+-rw-rw-rw-   0        0        0       69 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.756127 PyAltiumRunTop-0.2.4.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.760117 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/
+-rw-rw-rw-   0        0        0     2672 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      575 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 09:14:50.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       73 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.768095 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/
+-rw-rw-rw-   0        0        0    20034 2023-04-16 12:00:32.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRun.py
+-rw-rw-rw-   0        0        0    20094 2023-04-26 07:44:50.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRun15.py
+-rw-rw-rw-   0        0        0    20041 2023-04-16 11:56:03.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunAd.py
+-rw-rw-rw-   0        0        0    20149 2023-04-26 07:44:50.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunAd15.py
+-rw-rw-rw-   0        0        0    23181 2023-05-11 09:28:11.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunEnv.py
+-rw-rw-rw-   0        0        0    23191 2023-05-11 09:28:11.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunEnv15.py
+-rw-rw-rw-   0        0        0    20045 2023-04-16 12:05:11.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunexe.py
+-rw-rw-rw-   0        0        0    20105 2023-04-26 07:44:50.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunexe15.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.774079 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/helpers/
+-rw-rw-rw-   0        0        0     2415 2023-04-26 07:29:08.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/helpers/AltiumHelper.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/helpers/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.788147 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/__init__.py
+-rw-rw-rw-   0        0        0      525 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/logger.pas
+-rw-rw-rw-   0        0        0      478 2023-02-27 09:06:28.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/main.pas
+-rw-rw-rw-   0        0        0     7285 2023-03-06 02:14:13.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/updateSitNum0302.pas
+drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.773082 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/
+-rw-rw-rw-   0        0        0     2801 2023-05-11 09:28:37.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-05-11 09:28:37.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 09:28:37.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 09:40:41.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       73 2023-05-11 09:28:37.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-11 09:28:37.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-16 11:51:19.000000 PyAltiumRunTop-0.2.4.5/src/__init__.py
```

### Comparing `PyAltiumRunTop-0.2.4.4/LICENSE` & `PyAltiumRunTop-0.2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.4/PKG-INFO` & `PyAltiumRunTop-0.2.4.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAltiumRunTop
-Version: 0.2.4.4
+Version: 0.2.4.5
 Summary: A library that can run scripts in altium designer
 Home-page: https://github.com/wqh0109663/PyAltiumRun
 Author: Dylan Gybels,wqh0109663
 Author-email: dylangybels@gmail.com,wqh0109663@gmail.com
 License: MIT
 Keywords: Altium,Scripting,Runner
 Platform: win32
@@ -18,15 +18,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 PyAltiumRun
 
-[![PyPI version](https://badgen.net/pypi/v/PyAltiumRun)](https://pypi.org/project/PyAltiumRun/)  [![PyPI version](https://badgen.net/pypi/license/PyAltiumRun)](https://github.com/krakdustten/PyAltiumRun/blob/master/LICENSE) [![PyPI version](https://badgen.net/pypi/python/PyAltiumRun)](https://pypi.org/project/PyAltiumRun/)
+[![PyPI version](https://badgen.net/pypi/v/PyAltiumRunTop)](https://pypi.org/project/PyAltiumRunTop/)  [![PyPI version](https://badgen.net/pypi/license/PyAltiumRunTop)](https://github.com/krakdustten/PyAltiumRun/blob/master/LICENSE) [![PyPI version](https://badgen.net/pypi/python/PyAltiumRunTop)](https://pypi.org/project/PyAltiumRunTop/)
 
 A Python interface that can run Delphiscript  in [Altium Designer](https://www.altium.com/).
 
 New features can be requested in the [Github Issues](https://github.com/krakdustten/PyAltiumRun/issues).
 
 ## Update 
 Fix bug log_str
@@ -34,17 +34,19 @@
 Add Parameter Pas File
 
 ## Installation requirements
 
 Altium designer must be installed before running this library.
 
 ## Quick start
-
+```shell script
+pip install PyAltiumRunTop
+```
 ~~~python
-from PyAltiumRun.AltiumRun import AltiumRun
+from PyAltiumRunTop.AltiumRun import AltiumRun
 
 run = AltiumRun(use_internal_logger=True)                       #Create runner object
 run.clear_log_file()                                            #Clear the logs of the previous run
 run.set_project_to_open(r"Altium_project/Arduino_uno.PrjPcb")   #Define an Altium project to open
 run.add_script(r"Altium_scripts/generate_docs.pas")             #Add a script to the runner
 run.set_function("gen_docs", "Arduino_uno")                     #Set the function to run
 run.run()                                                       #Run
```

### Comparing `PyAltiumRunTop-0.2.4.4/README.md` & `PyAltiumRunTop-0.2.4.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 PyAltiumRun
 
-[![PyPI version](https://badgen.net/pypi/v/PyAltiumRun)](https://pypi.org/project/PyAltiumRun/)  [![PyPI version](https://badgen.net/pypi/license/PyAltiumRun)](https://github.com/krakdustten/PyAltiumRun/blob/master/LICENSE) [![PyPI version](https://badgen.net/pypi/python/PyAltiumRun)](https://pypi.org/project/PyAltiumRun/)
+[![PyPI version](https://badgen.net/pypi/v/PyAltiumRunTop)](https://pypi.org/project/PyAltiumRunTop/)  [![PyPI version](https://badgen.net/pypi/license/PyAltiumRunTop)](https://github.com/krakdustten/PyAltiumRun/blob/master/LICENSE) [![PyPI version](https://badgen.net/pypi/python/PyAltiumRunTop)](https://pypi.org/project/PyAltiumRunTop/)
 
 A Python interface that can run Delphiscript  in [Altium Designer](https://www.altium.com/).
 
 New features can be requested in the [Github Issues](https://github.com/krakdustten/PyAltiumRun/issues).
 
 ## Update 
 Fix bug log_str
@@ -12,17 +12,19 @@
 Add Parameter Pas File
 
 ## Installation requirements
 
 Altium designer must be installed before running this library.
 
 ## Quick start
-
+```shell script
+pip install PyAltiumRunTop
+```
 ~~~python
-from PyAltiumRun.AltiumRun import AltiumRun
+from PyAltiumRunTop.AltiumRun import AltiumRun
 
 run = AltiumRun(use_internal_logger=True)                       #Create runner object
 run.clear_log_file()                                            #Clear the logs of the previous run
 run.set_project_to_open(r"Altium_project/Arduino_uno.PrjPcb")   #Define an Altium project to open
 run.add_script(r"Altium_scripts/generate_docs.pas")             #Add a script to the runner
 run.set_function("gen_docs", "Arduino_uno")                     #Set the function to run
 run.run()                                                       #Run
```

### Comparing `PyAltiumRunTop-0.2.4.4/pyproject.toml` & `PyAltiumRunTop-0.2.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.4/setup.cfg` & `PyAltiumRunTop-0.2.4.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 7941 6c74 6975 6d52 756e 546f   = PyAltiumRunTo
 00000020: 700d 0a76 6572 7369 6f6e 203d 2030 2e32  p..version = 0.2
-00000030: 2e34 2e34 0d0a 6465 7363 7269 7074 696f  .4.4..descriptio
+00000030: 2e34 2e35 0d0a 6465 7363 7269 7074 696f  .4.5..descriptio
 00000040: 6e20 3d20 4120 6c69 6272 6172 7920 7468  n = A library th
 00000050: 6174 2063 616e 2072 756e 2073 6372 6970  at can run scrip
 00000060: 7473 2069 6e20 616c 7469 756d 2064 6573  ts in altium des
 00000070: 6967 6e65 720d 0a6c 6f6e 675f 6465 7363  igner..long_desc
 00000080: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000090: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 000000a0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
```

### Comparing `PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/PKG-INFO` & `PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.4/src/PyAltiumRun.egg-info/SOURCES.txt` & `PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/AltiumRun.py` & `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRun.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import sys
 from time import sleep
 from typing import List, Optional, Dict, Any
 from PyAltiumRunTop.helpers import AltiumHelper
 import os
 import subprocess
-
+import pathlib
 
 class AltiumRun:
     """An Altium runner object
 
     This object holds the configuration parameters to create a Altium scripting project and run it accordingly.
     """
 
     def __init__(self, altium_version: Optional[str] = None, use_internal_logger: bool = True):
         self.set_used_altium_version()
         self._project_path = os.path.dirname(sys.argv[0]) + "/scripting_project"
 
+        pathlib.Path(self._project_path).mkdir(parents=True, exist_ok=True)
         self.external_scripts_path: List[str] = []
         r"""A list of all the paths to the needed scripts."""
 
         self._internal_scripts_path: List[str] = []
 
         self._use_internal_logger = use_internal_logger
         self._project_path_to_open: Optional[str] = None
@@ -163,14 +164,37 @@
         :param function_name: The name of the function to run in the Altium script as string.
         :param args: The arguments given to the Altium script function.
         """
         self._generate_script_from_base_top("updateSitNum0302.pas")
         self.add_script(self._project_path + "/updateSitNum0302.pas")
         self.set_function_name(function_name)
         self.set_function_parameters(*args)
+    # this one for me
+    def set_function_top2(self, function_name: str, *args: List[Any]) -> None:
+        r"""Set the function name and arguments of the Altium script function needed to be run.
+
+        :param function_name: The name of the function to run in the Altium script as string.
+        :param args: The arguments given to the Altium script function.
+        """
+        self._generate_script_from_base_top("exportAdBom2BasicBom.pas")
+        self.add_script(self._project_path + "/exportAdBom2BasicBom.pas")
+        self._generate_script_from_base_top("getproductCode.pas")
+        self.add_script(self._project_path + "/getproductCode.pas")
+        self.set_function_name(function_name)
+        self.set_function_parameters(*args)
+
+    def set_function_top3(self, function_name: str, *args: List[Any]) -> None:
+        r"""Set the function name and arguments of the Altium script function needed to be run.
+
+        :param function_name: The name of the function to run in the Altium script as string.
+        :param args: The arguments given to the Altium script function.
+        """
+        self.set_function_name(function_name)
+        self.set_function_parameters(*args)
+
     def runTop(self, wait_until_finished: bool = True, timeout: float = 10) -> bool:
         r"""Runs the script based on the settings defined.
 
         If Altium Designer is running it will run the script in that instance and leave it open.
         If Altium Desinger is not running it will start a new instance and close it when finished.
 
         This functions waits until the script is finished when the :param:`wait_until_finished` parameter is True.
@@ -207,14 +231,106 @@
         f_running.close()
 
         self._process = subprocess.Popen(command)
         if wait_until_finished:
             return self.wait_until_finished(timeout)
         return self.wait_until_finished(0.1)
 
+    def runTop2(self, wait_until_finished: bool = True, timeout: float = 10) -> bool:
+        r"""Runs the script based on the settings defined.
+
+        If Altium Designer is running it will run the script in that instance and leave it open.
+        If Altium Desinger is not running it will start a new instance and close it when finished.
+
+        This functions waits until the script is finished when the :param:`wait_until_finished` parameter is True.
+        A timeout can be set for this waiting on finish.
+
+        :param wait_until_finished: If the function should wait for the script to finish.
+        :param timeout: The timeout when waiting for the script to finish.
+        :return: True, if the script is finished.
+        """
+        # Generate the path for the scripting project
+        if not os.path.exists(self._project_path):
+            os.makedirs(self._project_path)
+        if not os.path.exists(self._project_path + "/data"):
+            os.makedirs(self._project_path + "/data")
+
+        self._internal_scripts_path.clear()
+        if self._use_internal_logger:
+            self._generate_logger_script()
+        self._generate_main_script()
+        self._internal_scripts_path.append(self._project_path + "/exportAdBom2BasicBom.pas")
+        self._generate_script_from_base_top("exportAdBom2BasicBom.pas")
+
+        self._internal_scripts_path.append(self._project_path + "/updateSitNum0302.pas")
+        self._generate_script_from_base_top("updateSitNum0302.pas")
+
+        self._generate_scripting_project()
+        self.get_log_file_path()
+
+
+
+        project = (self._project_path + "/script_project.PrjScr").replace("/", "\\")
+        script = "main.pas>SCRIPTING_SYSTEM_MAIN"
+        command = f"\"{self._altium_path}\" -RScriptingSystem:RunScript(ProjectName=\"{project}\"|ProcName=\"{script}\")"
+
+        f_running = open(self._project_path + "/data/running", 'w')
+        f_running.write("")
+        f_running.close()
+
+        self._process = subprocess.Popen(command)
+        if wait_until_finished:
+            return self.wait_until_finished(timeout)
+        return self.wait_until_finished(0.1)
+
+    def runTop3(self, wait_until_finished: bool = True, timeout: float = 10) -> bool:
+        r"""Runs the script based on the settings defined.
+
+        If Altium Designer is running it will run the script in that instance and leave it open.
+        If Altium Desinger is not running it will start a new instance and close it when finished.
+
+        This functions waits until the script is finished when the :param:`wait_until_finished` parameter is True.
+        A timeout can be set for this waiting on finish.
+
+        :param wait_until_finished: If the function should wait for the script to finish.
+        :param timeout: The timeout when waiting for the script to finish.
+        :return: True, if the script is finished.
+        """
+        # Generate the path for the scripting project
+        if not os.path.exists(self._project_path):
+            os.makedirs(self._project_path)
+        if not os.path.exists(self._project_path + "/data"):
+            os.makedirs(self._project_path + "/data")
+
+        self._internal_scripts_path.clear()
+        if self._use_internal_logger:
+            self._generate_logger_script()
+        self._generate_main_script()
+        self._internal_scripts_path.append(self._project_path + "/getproductCode.pas")
+        self._generate_script_from_base_top("getproductCode.pas")
+
+        self._internal_scripts_path.append(self._project_path + "/updateSitNum0302.pas")
+        self._generate_script_from_base_top("updateSitNum0302.pas")
+
+        self._generate_scripting_project()
+        self.get_log_file_path()
+
+        project = (self._project_path + "/script_project.PrjScr").replace("/", "\\")
+        script = "main.pas>SCRIPTING_SYSTEM_MAIN"
+        command = f"\"{self._altium_path}\" -RScriptingSystem:RunScript(ProjectName=\"{project}\"|ProcName=\"{script}\")"
+
+        f_running = open(self._project_path + "/data/running", 'w')
+        f_running.write("")
+        f_running.close()
+
+        self._process = subprocess.Popen(command)
+        if wait_until_finished:
+            return self.wait_until_finished(timeout)
+        return self.wait_until_finished(0.1)
+
     def run(self, wait_until_finished: bool = True, timeout: float = 10) -> bool:
         r"""Runs the script based on the settings defined.
 
         If Altium Designer is running it will run the script in that instance and leave it open.
         If Altium Desinger is not running it will start a new instance and close it when finished.
 
         This functions waits until the script is finished when the :param:`wait_until_finished` parameter is True.
@@ -322,21 +438,21 @@
             if len(text) > 1:
                 text = text[:-2]
             return text + "]"
         print(type(param))
         return None
 
     def _generate_script_from_base(self, name: str, variables: Dict[str, Any] = {}) -> None:
-        origin = os.path.dirname(os.path.abspath(__file__)) + '\\scriptingbase\\' + name
+        origin = 'D:\\adTemp\\scriptingbase\\' + name
         destination = self._project_path + '/' + name
         self._generate_script_from_source(origin, destination, variables)
 
 
     def _generate_script_from_base_top(self, name: str) -> None:
-        origin = os.path.dirname(os.path.abspath(__file__)) + '\\scriptingbase\\' + name
+        origin = 'D:\\adTemp\\scriptingbase\\' + name
         destination = self._project_path + '/' + name
         self._generate_script_from_source_top(origin, destination)
     def _generate_script_from_source_top(self, origin: str, destination: str) -> None:
         f_or = open(origin, 'r')
         f_de = open(destination, 'w')
         line = f_or.readline()
         while line:
```

### Comparing `PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/helpers/AltiumHelper.py` & `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/helpers/AltiumHelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,7 +45,19 @@
                     return var_str
             if type(build_str) is str:
                 if build_str == version:
                     return var_str
             i += 1
         except WindowsError:
             return None
+
+
+def get_system_env_variable(variable_name: str) -> Any:
+    with winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE,
+                        r'SYSTEM\CurrentControlSet\Control\Session Manager\Environment',
+                        0, winreg.KEY_READ) as key:
+
+        try:
+            variable_value, _ = winreg.QueryValueEx(key, variable_name)
+            return variable_value
+        except FileNotFoundError:
+            return None
```

### Comparing `PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/logger.pas` & `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/logger.pas`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop/scriptingbase/updateSitNum0302.pas` & `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/updateSitNum0302.pas`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/PKG-INFO` & `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAltiumRunTop
-Version: 0.2.4.4
+Version: 0.2.4.5
 Summary: A library that can run scripts in altium designer
 Home-page: https://github.com/wqh0109663/PyAltiumRun
 Author: Dylan Gybels,wqh0109663
 Author-email: dylangybels@gmail.com,wqh0109663@gmail.com
 License: MIT
 Keywords: Altium,Scripting,Runner
 Platform: win32
@@ -18,15 +18,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 PyAltiumRun
 
-[![PyPI version](https://badgen.net/pypi/v/PyAltiumRun)](https://pypi.org/project/PyAltiumRun/)  [![PyPI version](https://badgen.net/pypi/license/PyAltiumRun)](https://github.com/krakdustten/PyAltiumRun/blob/master/LICENSE) [![PyPI version](https://badgen.net/pypi/python/PyAltiumRun)](https://pypi.org/project/PyAltiumRun/)
+[![PyPI version](https://badgen.net/pypi/v/PyAltiumRunTop)](https://pypi.org/project/PyAltiumRunTop/)  [![PyPI version](https://badgen.net/pypi/license/PyAltiumRunTop)](https://github.com/krakdustten/PyAltiumRun/blob/master/LICENSE) [![PyPI version](https://badgen.net/pypi/python/PyAltiumRunTop)](https://pypi.org/project/PyAltiumRunTop/)
 
 A Python interface that can run Delphiscript  in [Altium Designer](https://www.altium.com/).
 
 New features can be requested in the [Github Issues](https://github.com/krakdustten/PyAltiumRun/issues).
 
 ## Update 
 Fix bug log_str
@@ -34,17 +34,19 @@
 Add Parameter Pas File
 
 ## Installation requirements
 
 Altium designer must be installed before running this library.
 
 ## Quick start
-
+```shell script
+pip install PyAltiumRunTop
+```
 ~~~python
-from PyAltiumRun.AltiumRun import AltiumRun
+from PyAltiumRunTop.AltiumRun import AltiumRun
 
 run = AltiumRun(use_internal_logger=True)                       #Create runner object
 run.clear_log_file()                                            #Clear the logs of the previous run
 run.set_project_to_open(r"Altium_project/Arduino_uno.PrjPcb")   #Define an Altium project to open
 run.add_script(r"Altium_scripts/generate_docs.pas")             #Add a script to the runner
 run.set_function("gen_docs", "Arduino_uno")                     #Set the function to run
 run.run()                                                       #Run
```

### Comparing `PyAltiumRunTop-0.2.4.4/src/PyAltiumRunTop.egg-info/SOURCES.txt` & `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+src/__init__.py
 src/PyAltiumRun.egg-info/PKG-INFO
 src/PyAltiumRun.egg-info/SOURCES.txt
 src/PyAltiumRun.egg-info/dependency_links.txt
 src/PyAltiumRun.egg-info/not-zip-safe
 src/PyAltiumRun.egg-info/requires.txt
 src/PyAltiumRun.egg-info/top_level.txt
 src/PyAltiumRunTop/AltiumRun.py
+src/PyAltiumRunTop/AltiumRun15.py
+src/PyAltiumRunTop/AltiumRunAd.py
+src/PyAltiumRunTop/AltiumRunAd15.py
+src/PyAltiumRunTop/AltiumRunEnv.py
+src/PyAltiumRunTop/AltiumRunEnv15.py
+src/PyAltiumRunTop/AltiumRunexe.py
+src/PyAltiumRunTop/AltiumRunexe15.py
 src/PyAltiumRunTop/__init__.py
 src/PyAltiumRunTop/py.typed
 src/PyAltiumRunTop.egg-info/PKG-INFO
 src/PyAltiumRunTop.egg-info/SOURCES.txt
 src/PyAltiumRunTop.egg-info/dependency_links.txt
 src/PyAltiumRunTop.egg-info/not-zip-safe
 src/PyAltiumRunTop.egg-info/requires.txt
```

