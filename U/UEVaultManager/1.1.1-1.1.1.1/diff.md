# Comparing `tmp/UEVaultManager-1.1.1.tar.gz` & `tmp/UEVaultManager-1.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.1.1.tar", last modified: Thu May 11 14:59:17 2023, max compression
+gzip compressed data, was "UEVaultManager-1.1.1.1.tar", last modified: Thu May 11 15:50:42 2023, max compression
```

## Comparing `UEVaultManager-1.1.1.tar` & `UEVaultManager-1.1.1.1.tar`

### file list

```diff
@@ -1,57 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 14:59:17.507041 UEVaultManager-1.1.1/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     5700 2023-05-11 14:59:17.506041 UEVaultManager-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4930 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 14:59:17.424895 UEVaultManager-1.1.1/UEVaultManager/
--rw-rw-rw-   0        0        0      717 2023-05-11 14:58:41.000000 UEVaultManager-1.1.1/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 14:59:17.454370 UEVaultManager-1.1.1/UEVaultManager/api/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    20251 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0      884 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/api/lgd.py
--rw-rw-rw-   0        0        0    61539 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    42168 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-05-11 14:59:17.455370 UEVaultManager-1.1.1/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 14:59:17.458370 UEVaultManager-1.1.1/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38025 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-05-11 14:59:17.465589 UEVaultManager-1.1.1/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6686 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    22112 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/lfs/lgndry.py
--rw-rw-rw-   0        0        0     5528 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3040 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-11 14:59:17.483325 UEVaultManager-1.1.1/UEVaultManager/models/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     1351 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5078 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0       72 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     1334 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/models/gql.py
--rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30499 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-05-11 14:59:17.486322 UEVaultManager-1.1.1/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0      933 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-05-11 14:59:17.505041 UEVaultManager-1.1.1/UEVaultManager/utils/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3455 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5577 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1075 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10270 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      309 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      562 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-05-11 14:59:17.446370 UEVaultManager-1.1.1/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     5700 2023-05-11 14:59:17.000000 UEVaultManager-1.1.1/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1409 2023-05-11 14:59:17.000000 UEVaultManager-1.1.1/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 14:59:17.000000 UEVaultManager-1.1.1/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-11 14:59:17.000000 UEVaultManager-1.1.1/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-05-11 14:59:17.000000 UEVaultManager-1.1.1/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-11 14:59:17.000000 UEVaultManager-1.1.1/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 14:59:17.507041 UEVaultManager-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1938 2023-05-11 14:59:12.000000 UEVaultManager-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.203236 UEVaultManager-1.1.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5702 2023-05-11 15:50:42.202239 UEVaultManager-1.1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4930 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.118961 UEVaultManager-1.1.1.1/UEVaultManager/
+-rw-rw-rw-   0        0        0      719 2023-05-11 15:34:46.000000 UEVaultManager-1.1.1.1/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.149247 UEVaultManager-1.1.1.1/UEVaultManager/api/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    20251 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0      884 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/api/lgd.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.151242 UEVaultManager-1.1.1.1/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0    61539 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    42168 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.152241 UEVaultManager-1.1.1.1/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.155242 UEVaultManager-1.1.1.1/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38025 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.162242 UEVaultManager-1.1.1.1/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6686 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    22112 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/lfs/lgndry.py
+-rw-rw-rw-   0        0        0     5528 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3040 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.178681 UEVaultManager-1.1.1.1/UEVaultManager/models/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     1351 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5078 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0       72 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     1334 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/gql.py
+-rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30499 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.181681 UEVaultManager-1.1.1.1/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0      933 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.201239 UEVaultManager-1.1.1.1/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3455 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5577 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1075 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10270 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      309 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      562 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.140826 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     5702 2023-05-11 15:50:42.000000 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1479 2023-05-11 15:50:42.000000 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:50:42.000000 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-11 15:50:42.000000 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-05-11 15:50:42.000000 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-11 15:50:42.000000 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 15:50:42.203236 UEVaultManager-1.1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2051 2023-05-11 15:20:44.000000 UEVaultManager-1.1.1.1/setup.py
```

### Comparing `UEVaultManager-1.1.1/LICENSE` & `UEVaultManager-1.1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/PKG-INFO` & `UEVaultManager-1.1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.1.1
+Version: 1.1.1.1
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `UEVaultManager-1.1.1/README.md` & `UEVaultManager-1.1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/__init__.py` & `UEVaultManager-1.1.1.1/UEVaultManager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """UEVaultManager"""
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.1.1'
+__version__ = '1.1.1.1'
 # Pegasus Seiya
 # Dragon Shiryu
 # Cygnus Hyoga
 __codename__ = 'Cygnus'
 # Andromeda Shun
 # Phoenix Ikki
 # Leo Aiolia
```

### Comparing `UEVaultManager-1.1.1/UEVaultManager/api/egs.py` & `UEVaultManager-1.1.1.1/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/api/lgd.py` & `UEVaultManager-1.1.1.1/UEVaultManager/api/lgd.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/cli.py` & `UEVaultManager-1.1.1.1/UEVaultManager/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/core.py` & `UEVaultManager-1.1.1.1/UEVaultManager/core.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.1.1.1/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.1.1.1/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.1.1.1/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.1.1.1/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/lfs/lgndry.py` & `UEVaultManager-1.1.1.1/UEVaultManager/lfs/lgndry.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.1.1.1/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.1.1.1/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/models/app.py` & `UEVaultManager-1.1.1.1/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/models/chunk.py` & `UEVaultManager-1.1.1.1/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/models/config.py` & `UEVaultManager-1.1.1.1/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/models/downloading.py` & `UEVaultManager-1.1.1.1/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/models/egl.py` & `UEVaultManager-1.1.1.1/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/models/gql.py` & `UEVaultManager-1.1.1.1/UEVaultManager/models/gql.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.1.1.1/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/models/manifest.py` & `UEVaultManager-1.1.1.1/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.1.1.1/UEVaultManager/tkgui/main.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.1.1.1/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/utils/cli.py` & `UEVaultManager-1.1.1.1/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.1.1.1/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.1.1.1/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.1.1.1/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.1.1.1/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.1.1.1/UEVaultManager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.1.1
+Version: 1.1.1.1
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `UEVaultManager-1.1.1/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.1.1.1/UEVaultManager.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 UEVaultManager.egg-info/dependency_links.txt
 UEVaultManager.egg-info/entry_points.txt
 UEVaultManager.egg-info/requires.txt
 UEVaultManager.egg-info/top_level.txt
 UEVaultManager/api/__init__.py
 UEVaultManager/api/egs.py
 UEVaultManager/api/lgd.py
+UEVaultManager/assets/UEVM_200x200.png
+UEVaultManager/assets/main.ico
 UEVaultManager/downloader/__init__.py
 UEVaultManager/downloader/mp/__init__.py
 UEVaultManager/downloader/mp/manager.py
 UEVaultManager/downloader/mp/workers.py
 UEVaultManager/lfs/__init__.py
 UEVaultManager/lfs/egl.py
 UEVaultManager/lfs/eos.py
```

### Comparing `UEVaultManager-1.1.1/setup.py` & `UEVaultManager-1.1.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,49 +8,50 @@
 
 from UEVaultManager import __name__, __version__, __license__, __author__, __author_email__, __copyright__, __description__, __url__
 
 if sys.version_info < (3, 9):
     sys.exit('python 3.9 or higher is required for UEVaultManager')
 
 this_directory = Path(__file__).parent
-__long_description__ = (this_directory / "README.md").read_text()
+__long_description__ = Path.joinpath(this_directory, 'README.md').read_text()
 # __long_description__ = ''.join(__long_description__[8:16])  # keep only description text
 
 setup(
     name=__name__,
     version=__version__,
     license=__license__,
     author=__author__,
     author_email=__author_email__,
     copyright=__copyright__,
     description=__description__,
     long_description=__long_description__,
+    long_description_content_type='text/markdown',
     url=__url__,
     packages=[
         'UEVaultManager',  #
         'UEVaultManager.api',  #
         'UEVaultManager.assets',  #
         'UEVaultManager.downloader',  #
         'UEVaultManager.downloader.mp',  #
         'UEVaultManager.lfs',  #
         'UEVaultManager.models',  #
         'UEVaultManager.tkgui',  #
         'UEVaultManager.utils',  #
     ],
+    data_files=[('', ['UEVaultManager/assets/UEVM_200x200.png','UEVaultManager/assets/main.ico'])],
     entry_points=dict(console_scripts=['UEVaultManager = UEVaultManager.cli:main']),
     install_requires=[
         'requests<3.0',  #
         'setuptools',  #
         'wheel'
     ],
     extras_require=dict(webview=['pywebview>=3.4'], webview_gtk=[
         'pywebview>=3.4',  #
         'PyGObject'
     ]),
-    long_description_content_type='text/markdown',
     python_requires='>=3.9',
     classifiers=[
         'License :: OSI Approved :: BSD License',  #
         'Programming Language :: Python :: 3.9',  #
         'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11',  #
         'Operating System :: OS Independent',  #
         'Development Status :: 4 - Beta'
```

