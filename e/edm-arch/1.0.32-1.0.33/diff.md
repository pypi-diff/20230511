# Comparing `tmp/edm-arch-1.0.32.tar.gz` & `tmp/edm-arch-1.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edm-arch-1.0.32.tar", last modified: Wed May 10 12:38:48 2023, max compression
+gzip compressed data, was "edm-arch-1.0.33.tar", last modified: Thu May 11 11:27:41 2023, max compression
```

## Comparing `edm-arch-1.0.32.tar` & `edm-arch-1.0.33.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:38:48.137064 edm-arch-1.0.32/
--rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 edm-arch-1.0.32/LICENSE
--rw-rw-rw-   0        0        0    16069 2023-05-10 12:38:48.138031 edm-arch-1.0.32/PKG-INFO
--rw-rw-rw-   0        0        0    15175 2023-05-08 09:53:16.000000 edm-arch-1.0.32/README.md
--rw-rw-rw-   0        0        0      522 2022-06-10 11:27:08.000000 edm-arch-1.0.32/pyproject.toml
--rw-rw-rw-   0        0        0     1255 2023-05-10 12:38:48.140033 edm-arch-1.0.32/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 edm-arch-1.0.32/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:38:48.087197 edm-arch-1.0.32/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 12:38:48.108031 edm-arch-1.0.32/src/edm_arch.egg-info/
--rw-rw-rw-   0        0        0    16069 2023-05-10 12:38:48.000000 edm-arch-1.0.32/src/edm_arch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      658 2023-05-10 12:38:48.000000 edm-arch-1.0.32/src/edm_arch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:38:48.000000 edm-arch-1.0.32/src/edm_arch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-22 11:44:30.000000 edm-arch-1.0.32/src/edm_arch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      162 2023-05-10 12:38:48.000000 edm-arch-1.0.32/src/edm_arch.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 12:38:48.000000 edm-arch-1.0.32/src/edm_arch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 12:38:48.125026 edm-arch-1.0.32/src/edmpy/
--rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.32/src/edmpy/__init__.py
--rw-rw-rw-   0        0        0       79 2022-06-21 13:54:13.000000 edm-arch-1.0.32/src/edmpy/__main__.py
--rw-rw-rw-   0        0        0    28026 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/cfg.py
--rw-rw-rw-   0        0        0       18 2023-03-08 09:12:03.000000 edm-arch-1.0.32/src/edmpy/constants.py
--rw-rw-rw-   0        0        0     5289 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/db.py
--rw-rw-rw-   0        0        0    13461 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/edm.kv
--rw-rw-rw-   0        0        0   122722 2023-05-10 12:35:53.000000 edm-arch-1.0.32/src/edmpy/edm.py
--rw-rw-rw-   0        0        0     5691 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/geo.py
--rw-rw-rw-   0        0        0     2496 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/ini.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:38:48.135030 edm-arch-1.0.32/src/edmpy/lib/
--rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.32/src/edmpy/lib/__init__.py
--rw-rw-rw-   0        0        0     4214 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/lib/blockdata.py
--rw-rw-rw-   0        0        0     4332 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/lib/colorscheme.py
--rw-rw-rw-   0        0        0     2334 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/lib/constants.py
--rw-rw-rw-   0        0        0     4035 2023-03-08 08:56:31.000000 edm-arch-1.0.32/src/edmpy/lib/dbs.py
--rw-rw-rw-   0        0        0   175935 2023-05-10 12:05:08.000000 edm-arch-1.0.32/src/edmpy/lib/e5_widgets.py
--rw-rw-rw-   0        0        0     1792 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/lib/misc.py
--rw-rw-rw-   0        0        0        0 2022-06-07 20:43:53.000000 edm-arch-1.0.32/src/edmpy/py.typed
--rw-rw-rw-   0        0        0    44643 2023-05-10 12:13:46.000000 edm-arch-1.0.32/src/edmpy/totalstation.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:27:41.188964 edm-arch-1.0.33/
+-rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 edm-arch-1.0.33/LICENSE
+-rw-rw-rw-   0        0        0    16069 2023-05-11 11:27:41.189971 edm-arch-1.0.33/PKG-INFO
+-rw-rw-rw-   0        0        0    15175 2023-05-08 09:53:16.000000 edm-arch-1.0.33/README.md
+-rw-rw-rw-   0        0        0      523 2023-05-11 08:29:35.000000 edm-arch-1.0.33/pyproject.toml
+-rw-rw-rw-   0        0        0     1255 2023-05-11 11:27:41.191968 edm-arch-1.0.33/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 edm-arch-1.0.33/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:27:41.132289 edm-arch-1.0.33/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 11:27:41.155282 edm-arch-1.0.33/src/edm_arch.egg-info/
+-rw-rw-rw-   0        0        0    16069 2023-05-11 11:27:41.000000 edm-arch-1.0.33/src/edm_arch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-05-11 11:27:41.000000 edm-arch-1.0.33/src/edm_arch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 11:27:41.000000 edm-arch-1.0.33/src/edm_arch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-06-22 11:44:30.000000 edm-arch-1.0.33/src/edm_arch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      162 2023-05-11 11:27:41.000000 edm-arch-1.0.33/src/edm_arch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-11 11:27:41.000000 edm-arch-1.0.33/src/edm_arch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 11:27:41.175962 edm-arch-1.0.33/src/edmpy/
+-rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.33/src/edmpy/__init__.py
+-rw-rw-rw-   0        0        0       79 2022-06-21 13:54:13.000000 edm-arch-1.0.33/src/edmpy/__main__.py
+-rw-rw-rw-   0        0        0    28032 2023-05-11 11:24:27.000000 edm-arch-1.0.33/src/edmpy/cfg.py
+-rw-rw-rw-   0        0        0       18 2023-03-08 09:12:03.000000 edm-arch-1.0.33/src/edmpy/constants.py
+-rw-rw-rw-   0        0        0     5301 2023-05-11 11:23:24.000000 edm-arch-1.0.33/src/edmpy/db.py
+-rw-rw-rw-   0        0        0    13461 2023-05-08 09:53:16.000000 edm-arch-1.0.33/src/edmpy/edm.kv
+-rw-rw-rw-   0        0        0   122859 2023-05-11 11:27:16.000000 edm-arch-1.0.33/src/edmpy/edm.py
+-rw-rw-rw-   0        0        0     5691 2023-05-08 09:53:16.000000 edm-arch-1.0.33/src/edmpy/geo.py
+-rw-rw-rw-   0        0        0     2508 2023-05-11 11:24:10.000000 edm-arch-1.0.33/src/edmpy/ini.py
+drwxrwxrwx   0        0        0        0 2023-05-11 11:27:41.187956 edm-arch-1.0.33/src/edmpy/lib/
+-rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.33/src/edmpy/lib/__init__.py
+-rw-rw-rw-   0        0        0     4220 2023-05-11 11:23:24.000000 edm-arch-1.0.33/src/edmpy/lib/blockdata.py
+-rw-rw-rw-   0        0        0     4338 2023-05-11 11:23:24.000000 edm-arch-1.0.33/src/edmpy/lib/colorscheme.py
+-rw-rw-rw-   0        0        0     2334 2023-05-08 09:53:16.000000 edm-arch-1.0.33/src/edmpy/lib/constants.py
+-rw-rw-rw-   0        0        0     4035 2023-03-08 08:56:31.000000 edm-arch-1.0.33/src/edmpy/lib/dbs.py
+-rw-rw-rw-   0        0        0   175959 2023-05-11 11:21:32.000000 edm-arch-1.0.33/src/edmpy/lib/e5_widgets.py
+-rw-rw-rw-   0        0        0     1792 2023-05-08 09:53:16.000000 edm-arch-1.0.33/src/edmpy/lib/misc.py
+-rw-rw-rw-   0        0        0        0 2022-06-07 20:43:53.000000 edm-arch-1.0.33/src/edmpy/py.typed
+-rw-rw-rw-   0        0        0    44655 2023-05-11 11:23:24.000000 edm-arch-1.0.33/src/edmpy/totalstation.py
```

### Comparing `edm-arch-1.0.32/LICENSE` & `edm-arch-1.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.32/PKG-INFO` & `edm-arch-1.0.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edm-arch
-Version: 1.0.32
+Version: 1.0.33
 Summary: Total stations for archaeologists
 Home-page: https://github.com/surf3s/EDM
 Author: Shannon P. McPherron
 Author-email: mcpherron@eva.mpg.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/surf3s/EDM/issues
 Platform: unix
```

### Comparing `edm-arch-1.0.32/README.md` & `edm-arch-1.0.33/README.md`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.32/pyproject.toml` & `edm-arch-1.0.33/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "src/tests",
 ]
 
 [tool.mypy]
 mypy_path = "src"
 check_untyped_defs = true
 disallow_any_generics = true
-ignore_missing_imports = true
+ignore_missing_imports = false
 no_implicit_optional = true
 show_error_codes = true
 strict_equality = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
```

### Comparing `edm-arch-1.0.32/setup.cfg` & `edm-arch-1.0.33/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 646d 2d61 7263 680d 0a64 6573   = edm-arch..des
 00000020: 6372 6970 7469 6f6e 203d 2054 6f74 616c  cription = Total
 00000030: 2073 7461 7469 6f6e 7320 666f 7220 6172   stations for ar
 00000040: 6368 6165 6f6c 6f67 6973 7473 0d0a 7665  chaeologists..ve
-00000050: 7273 696f 6e20 3d20 312e 302e 3332 0d0a  rsion = 1.0.32..
+00000050: 7273 696f 6e20 3d20 312e 302e 3333 0d0a  rsion = 1.0.33..
 00000060: 6175 7468 6f72 203d 2053 6861 6e6e 6f6e  author = Shannon
 00000070: 2050 2e20 4d63 5068 6572 726f 6e0d 0a61   P. McPherron..a
 00000080: 7574 686f 725f 656d 6169 6c20 3d20 6d63  uthor_email = mc
 00000090: 7068 6572 726f 6e40 6576 612e 6d70 672e  pherron@eva.mpg.
 000000a0: 6465 0d0a 6c6f 6e67 5f64 6573 6372 6970  de..long_descrip
 000000b0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 000000c0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
```

### Comparing `edm-arch-1.0.32/src/edm_arch.egg-info/PKG-INFO` & `edm-arch-1.0.33/src/edm_arch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edm-arch
-Version: 1.0.32
+Version: 1.0.33
 Summary: Total stations for archaeologists
 Home-page: https://github.com/surf3s/EDM
 Author: Shannon P. McPherron
 Author-email: mcpherron@eva.mpg.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/surf3s/EDM/issues
 Platform: unix
```

### Comparing `edm-arch-1.0.32/src/edm_arch.egg-info/SOURCES.txt` & `edm-arch-1.0.33/src/edm_arch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.32/src/edmpy/cfg.py` & `edm-arch-1.0.33/src/edmpy/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 from tinydb import where
 import logging
 import os
 
-from lib.blockdata import blockdata
+from edmpy.lib.blockdata import blockdata
 
 __BUTTONS__ = 13
 __DEFAULT_FIELDS__ = ['X', 'Y', 'Z', 'SLOPED', 'VANGLE', 'HANGLE', 'STATIONX', 'STATIONY', 'STATIONZ', 'LOCALX', 'LOCALY', 'LOCALZ', 'DATE', 'PRISM', 'ID']
 __DEFAULT_FIELDS_NUMERIC__ = ['X', 'Y', 'Z', 'SLOPED', 'STATIONX', 'STATIONY', 'STATIONZ', 'LOCALX', 'LOCALY', 'LOCALZ', 'PRISM']
 
 
 class CFG(blockdata):
```

### Comparing `edm-arch-1.0.32/src/edmpy/db.py` & `edm-arch-1.0.33/src/edmpy/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from tinydb import TinyDB, Query, where
 import re
 from typing import Dict
 from math import sqrt
 import logging
 
-from geo import datum, unit, prism
-from lib.dbs import dbs
+from edmpy.geo import datum, unit, prism
+from edmpy.lib.dbs import dbs
 
 
 class DB(dbs):
     MAX_FIELDS = 30
     db = None
     filename = None
     db_name = 'points'
```

### Comparing `edm-arch-1.0.32/src/edmpy/edm.kv` & `edm-arch-1.0.33/src/edmpy/edm.kv`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.32/src/edmpy/edm.py` & `edm-arch-1.0.33/src/edmpy/edm.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 
 Changes for Version 1.0.31
   Fixed issue with numeric values saved as text in JSON after initial save
   Added Help JSON to view raw data in JSON file
 
 Changes for Version 1.0.32
   Fixing issues with GeoCom and station setup
+
+Changes for Version 1.0.33
+  Fixed installation issues
   
 Bugs/To Do
   could make menus work better with keyboard (at least with tab)
   there is no error checking on duplicates in datagrid edits
   Do unitchecking after doing an offset shot on suffix 0 points
   On import, integers (like Suffix) are being converted to float values
   Good way to get random hash IDs
@@ -83,28 +86,28 @@
 from math import cos
 from math import sin
 from platform import python_version
 import logging
 from appdata import AppDataPaths
 
 # My libraries for this project
-from lib.e5_widgets import e5_label, e5_button, e5_MessageBox, e5_DatagridScreen, e5_RecordEditScreen, e5_side_by_side_buttons, e5_textinput
-from lib.e5_widgets import edm_manual, DataGridTextBox, e5_SaveDialog, e5_LoadDialog, e5_PopUpMenu, e5_MainScreen, e5_InfoScreen, e5_scrollview_label
-from lib.e5_widgets import e5_LogScreen, e5_CFGScreen, e5_INIScreen, e5_SettingsScreen, e5_scrollview_menu, DataGridMenuList, SpinnerOptions
-from lib.e5_widgets import e5_JSONScreen, DataGridLabelAndField
-from lib.colorscheme import ColorScheme
-from lib.misc import restore_window_size_position, filename_only, platform_name
-
-from geo import point, prism
-from db import DB
-from ini import INI
-from cfg import CFG
-from totalstation import totalstation
-from constants import APP_NAME
-from lib.constants import __SPLASH_HELP__
+from edmpy.lib.e5_widgets import e5_label, e5_button, e5_MessageBox, e5_DatagridScreen, e5_RecordEditScreen, e5_side_by_side_buttons, e5_textinput
+from edmpy.lib.e5_widgets import edm_manual, DataGridTextBox, e5_SaveDialog, e5_LoadDialog, e5_PopUpMenu, e5_MainScreen, e5_InfoScreen, e5_scrollview_label
+from edmpy.lib.e5_widgets import e5_LogScreen, e5_CFGScreen, e5_INIScreen, e5_SettingsScreen, e5_scrollview_menu, DataGridMenuList, SpinnerOptions
+from edmpy.lib.e5_widgets import e5_JSONScreen, DataGridLabelAndField
+from edmpy.lib.colorscheme import ColorScheme
+from edmpy.lib.misc import restore_window_size_position, filename_only, platform_name
+
+from edmpy.geo import point, prism
+from edmpy.db import DB
+from edmpy.ini import INI
+from edmpy.cfg import CFG
+from edmpy.totalstation import totalstation
+from edmpy.constants import APP_NAME
+from edmpy.lib.constants import __SPLASH_HELP__
 
 # The database - pure Python
 from tinydb import TinyDB
 from tinydb import __version__ as __tinydb_version__
 
 # from plyer import gps
 # from plyer import __version__ as __plyer_version__
@@ -126,15 +129,15 @@
 """
 try:
     import win32timezone
     win32timezone.TimeZoneInfo.local()
 except ModuleNotFoundError:
     pass
 
-VERSION = '1.0.32'
+VERSION = '1.0.33'
 PRODUCTION_DATE = 'May, 2023'
 __DEFAULT_FIELDS__ = ['X', 'Y', 'Z', 'SLOPED', 'VANGLE', 'HANGLE', 'STATIONX', 'STATIONY', 'STATIONZ', 'LOCALX', 'LOCALY', 'LOCALZ', 'DATE', 'PRISM', 'ID']
 __BUTTONS__ = 13
 __LASTCOMPORT__ = 16
 MAX_SCREEN_WIDTH = 400
```

### Comparing `edm-arch-1.0.32/src/edmpy/geo.py` & `edm-arch-1.0.33/src/edmpy/geo.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.32/src/edmpy/ini.py` & `edm-arch-1.0.33/src/edmpy/ini.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from lib.blockdata import blockdata
-from constants import APP_NAME
+from edmpy.lib.blockdata import blockdata
+from edmpy.constants import APP_NAME
 
 
 class INI(blockdata):
 
     def __init__(self, filename = ''):
         if filename == '':
             filename = APP_NAME + '.ini'
```

### Comparing `edm-arch-1.0.32/src/edmpy/lib/blockdata.py` & `edm-arch-1.0.33/src/edmpy/lib/blockdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # To Do
 #   Consider implications of not writing the block data after each update
 
 import logging
 import os
 
-from lib.constants import APP_NAME
+from edmpy.lib.constants import APP_NAME
 
 
 class blockdata:
 
     filename = ''
     blocks = []
```

### Comparing `edm-arch-1.0.32/src/edmpy/lib/colorscheme.py` & `edm-arch-1.0.33/src/edmpy/lib/colorscheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from kivy.core.window import Window
-from lib.misc import platform_name
+from edmpy.lib.misc import platform_name
 
 BLACK = 0x000000
 WHITE = 0xFFFFFF
 MIDDLE_GREY = (.5, .5, .5, 1)
 DARK_GREY = (.2, .2, .2, 1)
 
 # Color from Google material design
```

### Comparing `edm-arch-1.0.32/src/edmpy/lib/constants.py` & `edm-arch-1.0.33/src/edmpy/lib/constants.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.32/src/edmpy/lib/dbs.py` & `edm-arch-1.0.33/src/edmpy/lib/dbs.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.32/src/edmpy/lib/e5_widgets.py` & `edm-arch-1.0.33/src/edmpy/lib/e5_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 import re
 import requests
 import json
 import urllib
 from threading import Thread
 from appdata import AppDataPaths
 
-from lib.constants import __SPLASH_HELP__
-from lib.constants import APP_NAME
-from lib.colorscheme import ColorScheme, make_rgb, BLACK, WHITE, GOOGLE_COLORS, MIDDLE_GREY, DARK_GREY
-from lib.misc import platform_name, locate_file
+from edmpy.lib.constants import __SPLASH_HELP__
+from edmpy.lib.constants import APP_NAME
+from edmpy.lib.colorscheme import ColorScheme, make_rgb, BLACK, WHITE, GOOGLE_COLORS, MIDDLE_GREY, DARK_GREY
+from edmpy.lib.misc import platform_name, locate_file
 
 
 SCROLLBAR_WIDTH = 5
 TEXTBOX_HEIGHT = 30
 
 
 def width_calculator(fraction_size = .8, maximum_width = 800):
```

### Comparing `edm-arch-1.0.32/src/edmpy/lib/misc.py` & `edm-arch-1.0.33/src/edmpy/lib/misc.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.32/src/edmpy/totalstation.py` & `edm-arch-1.0.33/src/edmpy/totalstation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from kivy.properties import ObjectProperty
 import serial
 import os
-from geo import point, prism
-from constants import APP_NAME
+from edmpy.geo import point, prism
+from edmpy.constants import APP_NAME
 from math import sqrt
 from math import pi
 from math import cos
 from math import sin
 from math import acos
 from angles import r2d, deci2sexa, Angle
 import string
```

