# Comparing `tmp/isa-ssl-0.2.0.tar.gz` & `tmp/isa-ssl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isa-ssl-0.2.0.tar", last modified: Fri Apr 21 16:28:10 2023, max compression
+gzip compressed data, was "isa-ssl-0.2.1.tar", last modified: Thu May 11 21:26:52 2023, max compression
```

## Comparing `isa-ssl-0.2.0.tar` & `isa-ssl-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-04-21 16:28:10.853470 isa-ssl-0.2.0/
--rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-02-13 21:31:07.000000 isa-ssl-0.2.0/LICENSE
--rw-rw-r--   0 magland   (1000) magland   (1000)      522 2023-04-21 16:28:10.853470 isa-ssl-0.2.0/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)     1836 2023-04-21 12:01:45.000000 isa-ssl-0.2.0/README.md
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-04-21 16:28:10.853470 isa-ssl-0.2.0/isa/
--rw-rw-r--   0 magland   (1000) magland   (1000)      104 2023-04-21 12:02:34.000000 isa-ssl-0.2.0/isa/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      630 2023-04-21 11:17:31.000000 isa-ssl-0.2.0/isa/_find_singular_file_in_dir.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1913 2023-04-21 11:50:18.000000 isa-ssl-0.2.0/isa/_project_config.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1089 2023-04-21 16:24:09.000000 isa-ssl-0.2.0/isa/add.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2913 2023-04-21 16:24:09.000000 isa-ssl-0.2.0/isa/auto_detect_vocalizations.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2003 2023-04-21 16:24:09.000000 isa-ssl-0.2.0/isa/cli.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     5842 2023-04-21 16:24:09.000000 isa-ssl-0.2.0/isa/create_spectrograms.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     4438 2023-04-21 16:24:09.000000 isa-ssl-0.2.0/isa/init.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2711 2023-04-21 12:48:51.000000 isa-ssl-0.2.0/isa/update.py
--rw-rw-r--   0 magland   (1000) magland   (1000)       97 2023-04-21 11:59:05.000000 isa-ssl-0.2.0/isa/version.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-04-21 16:28:10.853470 isa-ssl-0.2.0/isa_ssl.egg-info/
--rw-rw-r--   0 magland   (1000) magland   (1000)      522 2023-04-21 16:28:10.000000 isa-ssl-0.2.0/isa_ssl.egg-info/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)      420 2023-04-21 16:28:10.000000 isa-ssl-0.2.0/isa_ssl.egg-info/SOURCES.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        1 2023-04-21 16:28:10.000000 isa-ssl-0.2.0/isa_ssl.egg-info/dependency_links.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       36 2023-04-21 16:28:10.000000 isa-ssl-0.2.0/isa_ssl.egg-info/entry_points.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       27 2023-04-21 16:28:10.000000 isa-ssl-0.2.0/isa_ssl.egg-info/requires.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        4 2023-04-21 16:28:10.000000 isa-ssl-0.2.0/isa_ssl.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)      547 2023-04-21 16:28:10.853470 isa-ssl-0.2.0/setup.cfg
--rw-rw-r--   0 magland   (1000) magland   (1000)      327 2023-04-21 12:01:54.000000 isa-ssl-0.2.0/setup.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-05-11 21:26:52.960310 isa-ssl-0.2.1/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-02-13 21:31:07.000000 isa-ssl-0.2.1/LICENSE
+-rw-rw-r--   0 magland   (1000) magland   (1000)      522 2023-05-11 21:26:52.960310 isa-ssl-0.2.1/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1778 2023-04-21 18:25:46.000000 isa-ssl-0.2.1/README.md
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-05-11 21:26:52.960310 isa-ssl-0.2.1/isa/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1165 2023-04-26 12:02:24.000000 isa-ssl-0.2.1/isa/RtcsharePlugin.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      148 2023-04-21 18:04:05.000000 isa-ssl-0.2.1/isa/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      690 2023-05-10 16:00:58.000000 isa-ssl-0.2.1/isa/_find_singular_file_in_dir.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1913 2023-04-21 11:50:18.000000 isa-ssl-0.2.1/isa/_project_config.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1089 2023-04-21 16:24:09.000000 isa-ssl-0.2.1/isa/add.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     4044 2023-05-10 20:42:52.000000 isa-ssl-0.2.1/isa/auto_detect_vocalizations.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2003 2023-04-21 16:24:09.000000 isa-ssl-0.2.1/isa/cli.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     5842 2023-05-10 19:11:58.000000 isa-ssl-0.2.1/isa/create_spectrograms.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     4438 2023-04-21 16:24:09.000000 isa-ssl-0.2.1/isa/init.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2773 2023-05-10 20:40:36.000000 isa-ssl-0.2.1/isa/update.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)       97 2023-05-11 21:26:37.000000 isa-ssl-0.2.1/isa/version.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-05-11 21:26:52.960310 isa-ssl-0.2.1/isa_ssl.egg-info/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      522 2023-05-11 21:26:52.000000 isa-ssl-0.2.1/isa_ssl.egg-info/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)      442 2023-05-11 21:26:52.000000 isa-ssl-0.2.1/isa_ssl.egg-info/SOURCES.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        1 2023-05-11 21:26:52.000000 isa-ssl-0.2.1/isa_ssl.egg-info/dependency_links.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       36 2023-05-11 21:26:52.000000 isa-ssl-0.2.1/isa_ssl.egg-info/entry_points.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       41 2023-05-11 21:26:52.000000 isa-ssl-0.2.1/isa_ssl.egg-info/requires.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        4 2023-05-11 21:26:52.000000 isa-ssl-0.2.1/isa_ssl.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)      547 2023-05-11 21:26:52.960310 isa-ssl-0.2.1/setup.cfg
+-rw-rw-r--   0 magland   (1000) magland   (1000)      352 2023-05-11 21:26:10.000000 isa-ssl-0.2.1/setup.py
```

### Comparing `isa-ssl-0.2.0/LICENSE` & `isa-ssl-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.0/PKG-INFO` & `isa-ssl-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isa-ssl
-Version: 0.2.0
+Version: 0.2.1
 Summary: Isa (Ee-suh) is a visualization and annotation tool for sound source location.
 Home-page: https://github.com/scratchrealm/isa
 Author: Jeremy Magland and Ralph Peterson
 Author-email: jmagland@flatironinstitute.org
 Project-URL: Bug Tracker, https://github.com/scratchrealm/isa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `isa-ssl-0.2.0/README.md` & `isa-ssl-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # isa
 
-Isa (Ee-suh) is a visualization and annotation tool for sound source location.
+Isa (Ee-suh) is a visualization and annotation tool for sound source localization.
 
 ## Installation and setup
 It is recommended that you use a Conda environment.
 
 Requirements
 * Linux or Mac
 * Conda (recommended)
 * Python >= 3.8
 * pyqt and opencv-python - todo: why is pyqt required?
 
-For now, during development, you must install isa from source. Clone this repo, then
+Install isa-ssl from PyPI:
 
 ```bash
-cd isa
-pip install -e .
+pip install isa-ssl
 ```
 
 Install rtcshare
 
 Todo: provide instructions for rtcshare
 
 ## Create a project
```

### Comparing `isa-ssl-0.2.0/isa/_find_singular_file_in_dir.py` & `isa-ssl-0.2.1/isa/_find_singular_file_in_dir.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,9 +11,10 @@
         for extension in extensions:
             if fname.endswith(extension):
                 matching_fnames.append(fname)
                 break
     if len(matching_fnames) == 0:
         return None
     if len(matching_fnames) > 1:
-        raise Exception(f'More than one {extension} file found in directory: {dirname}')
+        extensions_string = ', '.join(extensions)
+        raise Exception(f'More than one ({extensions_string}) file found in directory: {dirname}')
     return matching_fnames[0]
```

### Comparing `isa-ssl-0.2.0/isa/_project_config.py` & `isa-ssl-0.2.1/isa/_project_config.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.0/isa/add.py` & `isa-ssl-0.2.1/isa/add.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.0/isa/auto_detect_vocalizations.py` & `isa-ssl-0.2.1/isa/auto_detect_vocalizations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 from typing import Union, List
 import yaml
 import pickle
 import json
 import numpy as np
+import pandas as pd
+from ._find_singular_file_in_dir import _find_singular_file_in_dir
 
 
 def auto_detect_vocalizations(session: str, output_json_fname: str):
     dirname = f'./{session}'
     with open(f'{dirname}/isa-session.yaml', 'r') as f:
         config = yaml.safe_load(f)
-    print('USING CONFIG')
-    print(config)
+    
+    try:
+        csv_fname = _find_singular_file_in_dir(dirname, ['.csv'])
+    except:
+        csv_fname = None
+
+    if csv_fname is not None:
+        print(f'Generating annotations.json from {csv_fname}')
+        csv_path = f'{dirname}/{csv_fname}'
+        annotations = _generate_annotations_from_csv(csv_path, sampling_frequency=config['audio_sr_hz'])
+        with open(output_json_fname, 'w') as f:
+            json.dump(annotations, f, indent=4)
+        return
 
     auto_detect_freq_range = config['auto_detect_freq_range']
     spectrogram_df = config['spectrogram_df']
     freq_range=[int(auto_detect_freq_range[0] / spectrogram_df), int(auto_detect_freq_range[1] / spectrogram_df)]
 
     spectrograms_fname = f'{dirname}/spectrograms.pkl'
     print(f'Loading {spectrograms_fname}')
@@ -67,8 +80,29 @@
                         # the vocalization was long enough
                         vocalizations.append(
                             {'vocalizationId': f'auto-{voc_ind}', 'startFrame': vocalization_start_frame, 'endFrame': vocalization_last_active_frame + 1, 'labels': ['auto']}
                         )
                         voc_ind = voc_ind + 1
                     vocalization_start_frame = None
                     vocalization_last_active_frame = None
-    return vocalizations
+    return vocalizations
+
+def _generate_annotations_from_csv(csv_fname: str, *, sampling_frequency: float):
+    # read in the csv file
+    x = pd.read_csv(csv_fname, header=None)
+
+    vocalizations = []
+    for r in range(len(x[0])):
+        vocalization = {
+            "vocalizationId": f"{r}",
+            "startFrame": int(x[0][r] * sampling_frequency),
+            "endFrame": int(x[1][r] * sampling_frequency),
+            "labels": []
+        }
+        vocalizations.append(vocalization)
+    
+    annotations = {
+        "samplingFrequency": sampling_frequency,
+        "vocalizations": vocalizations
+    }
+    
+    return annotations
```

### Comparing `isa-ssl-0.2.0/isa/cli.py` & `isa-ssl-0.2.1/isa/cli.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.0/isa/create_spectrograms.py` & `isa-ssl-0.2.1/isa/create_spectrograms.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.0/isa/init.py` & `isa-ssl-0.2.1/isa/init.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.0/isa/update.py` & `isa-ssl-0.2.1/isa/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from typing import Union
 from dataclasses import dataclass
 import yaml
+import pandas as pd
 from .create_spectrograms import create_spectrograms
 from .auto_detect_vocalizations import auto_detect_vocalizations
 from ._project_config import _get_project_config_value
 from .init import _initialize_or_update_session_dir
 
 @dataclass
 class IsaUpdateOpts:
@@ -14,14 +15,15 @@
     redo_vocalization_detection: bool=False
 
 def update(
     session: Union[str, None]=None,
     all: bool=False,
     opts: IsaUpdateOpts=IsaUpdateOpts()
 ):
+    print(f'Updating session: {session}')
     if opts.redo_spectrograms:
         if opts.no_vocalization_detection and opts.redo_vocalization_detection:
             raise Exception('You cannot specify both redo_vocalization_detection and no_vocalization_detection')
     if all:
         if session:
             raise Exception('Cannot specify session with all')
         session_names = _get_project_config_value('sessions')
```

### Comparing `isa-ssl-0.2.0/isa_ssl.egg-info/PKG-INFO` & `isa-ssl-0.2.1/isa_ssl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isa-ssl
-Version: 0.2.0
+Version: 0.2.1
 Summary: Isa (Ee-suh) is a visualization and annotation tool for sound source location.
 Home-page: https://github.com/scratchrealm/isa
 Author: Jeremy Magland and Ralph Peterson
 Author-email: jmagland@flatironinstitute.org
 Project-URL: Bug Tracker, https://github.com/scratchrealm/isa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `isa-ssl-0.2.0/setup.cfg` & `isa-ssl-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = isa-ssl
-version = 0.2.0
+version = 0.2.1
 author = Jeremy Magland and Ralph Peterson
 author_email = jmagland@flatironinstitute.org
 description = Isa (Ee-suh) is a visualization and annotation tool for sound source location.
 url = https://github.com/scratchrealm/isa
 include_package_data = True
 project_urls = 
 	Bug Tracker = https://github.com/scratchrealm/isa/issues
```

