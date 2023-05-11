# Comparing `tmp/UEVaultManager-1.1.1.1.tar.gz` & `tmp/UEVaultManager-1.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.1.1.1.tar", last modified: Thu May 11 15:50:42 2023, max compression
+gzip compressed data, was "UEVaultManager-1.1.1.2.tar", last modified: Thu May 11 15:57:48 2023, max compression
```

## Comparing `UEVaultManager-1.1.1.1.tar` & `UEVaultManager-1.1.1.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.203236 UEVaultManager-1.1.1.1/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.1.1.1/LICENSE
--rw-rw-rw-   0        0        0     5702 2023-05-11 15:50:42.202239 UEVaultManager-1.1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4930 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.118961 UEVaultManager-1.1.1.1/UEVaultManager/
--rw-rw-rw-   0        0        0      719 2023-05-11 15:34:46.000000 UEVaultManager-1.1.1.1/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.149247 UEVaultManager-1.1.1.1/UEVaultManager/api/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    20251 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0      884 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/api/lgd.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.151242 UEVaultManager-1.1.1.1/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0    61539 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    42168 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.152241 UEVaultManager-1.1.1.1/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.155242 UEVaultManager-1.1.1.1/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38025 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.162242 UEVaultManager-1.1.1.1/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6686 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    22112 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/lfs/lgndry.py
--rw-rw-rw-   0        0        0     5528 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3040 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.178681 UEVaultManager-1.1.1.1/UEVaultManager/models/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     1351 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5078 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0       72 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     1334 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/gql.py
--rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30499 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.181681 UEVaultManager-1.1.1.1/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0      933 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.201239 UEVaultManager-1.1.1.1/UEVaultManager/utils/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3455 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5577 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1075 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10270 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      309 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      562 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.1/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:50:42.140826 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     5702 2023-05-11 15:50:42.000000 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1479 2023-05-11 15:50:42.000000 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:50:42.000000 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-11 15:50:42.000000 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-05-11 15:50:42.000000 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-11 15:50:42.000000 UEVaultManager-1.1.1.1/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 15:50:42.203236 UEVaultManager-1.1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2051 2023-05-11 15:20:44.000000 UEVaultManager-1.1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.833494 UEVaultManager-1.1.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5698 2023-05-11 15:57:48.832394 UEVaultManager-1.1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4926 2023-05-11 15:56:47.000000 UEVaultManager-1.1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.748560 UEVaultManager-1.1.1.2/UEVaultManager/
+-rw-rw-rw-   0        0        0      719 2023-05-11 15:57:03.000000 UEVaultManager-1.1.1.2/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.778662 UEVaultManager-1.1.1.2/UEVaultManager/api/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    20251 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0      884 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/api/lgd.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.781665 UEVaultManager-1.1.1.2/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0    61539 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    42168 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.782661 UEVaultManager-1.1.1.2/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.785522 UEVaultManager-1.1.1.2/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38025 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.793524 UEVaultManager-1.1.1.2/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6686 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    22112 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/lfs/lgndry.py
+-rw-rw-rw-   0        0        0     5528 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3040 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.809700 UEVaultManager-1.1.1.2/UEVaultManager/models/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     1351 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5078 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0       72 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     1334 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/gql.py
+-rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30499 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.811702 UEVaultManager-1.1.1.2/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0      933 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.831393 UEVaultManager-1.1.1.2/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3455 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5577 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1075 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10270 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      309 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      562 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.769660 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     5698 2023-05-11 15:57:48.000000 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1479 2023-05-11 15:57:48.000000 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:57:48.000000 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-11 15:57:48.000000 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-05-11 15:57:48.000000 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-11 15:57:48.000000 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 15:57:48.833494 UEVaultManager-1.1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2051 2023-05-11 15:20:44.000000 UEVaultManager-1.1.1.2/setup.py
```

### Comparing `UEVaultManager-1.1.1.1/LICENSE` & `UEVaultManager-1.1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/PKG-INFO` & `UEVaultManager-1.1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.1.1.1
+Version: 1.1.1.2
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: webview
 Provides-Extra: webview_gtk
 License-File: LICENSE
 
 Welcome to UEVaultManager
 ==========================================
-![UEVM_200x200.png](UEVaultManager%2Fassets%2FUEVM_200x200.png)
+![UEVM_200x200.png](UEVaultManager/assets/UEVM_200x200.png)
 
 | pypi                                                                                                                 | py_versions                                                                                                          | github                                                                                                                         | docs                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
 | [![Current PyPi Version](https://img.shields.io/pypi/v/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![py_versions](https://img.shields.io/pypi/pyversions/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![github](https://img.shields.io/github/v/tag/LaurentOngaro/uevaultmanager)](https://github.com/LaurentOngaro/UEVaultManager) | [![docs](https://img.shields.io/readthedocs/uevaultmanager/latest)](https://uevaultmanager.readthedocs.io/en/latest/?badge=latest) |
 
 **UEVaultManager** is an open-source assets manager that can list assets and
 their data from the Epic Games Marketplace. It is developed in Python, so
```

### Comparing `UEVaultManager-1.1.1.1/README.md` & `UEVaultManager-1.1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Welcome to UEVaultManager
 ==========================================
-![UEVM_200x200.png](UEVaultManager%2Fassets%2FUEVM_200x200.png)
+![UEVM_200x200.png](UEVaultManager/assets/UEVM_200x200.png)
 
 | pypi                                                                                                                 | py_versions                                                                                                          | github                                                                                                                         | docs                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
 | [![Current PyPi Version](https://img.shields.io/pypi/v/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![py_versions](https://img.shields.io/pypi/pyversions/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![github](https://img.shields.io/github/v/tag/LaurentOngaro/uevaultmanager)](https://github.com/LaurentOngaro/UEVaultManager) | [![docs](https://img.shields.io/readthedocs/uevaultmanager/latest)](https://uevaultmanager.readthedocs.io/en/latest/?badge=latest) |
 
 **UEVaultManager** is an open-source assets manager that can list assets and
 their data from the Epic Games Marketplace. It is developed in Python, so
```

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/__init__.py` & `UEVaultManager-1.1.1.2/UEVaultManager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """UEVaultManager"""
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.1.1.1'
+__version__ = '1.1.1.2'
 # Pegasus Seiya
 # Dragon Shiryu
 # Cygnus Hyoga
 __codename__ = 'Cygnus'
 # Andromeda Shun
 # Phoenix Ikki
 # Leo Aiolia
```

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/api/egs.py` & `UEVaultManager-1.1.1.2/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/api/lgd.py` & `UEVaultManager-1.1.1.2/UEVaultManager/api/lgd.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.1.1.2/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/assets/main.ico` & `UEVaultManager-1.1.1.2/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/cli.py` & `UEVaultManager-1.1.1.2/UEVaultManager/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/core.py` & `UEVaultManager-1.1.1.2/UEVaultManager/core.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.1.1.2/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.1.1.2/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.1.1.2/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.1.1.2/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/lfs/lgndry.py` & `UEVaultManager-1.1.1.2/UEVaultManager/lfs/lgndry.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.1.1.2/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.1.1.2/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/models/app.py` & `UEVaultManager-1.1.1.2/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/models/chunk.py` & `UEVaultManager-1.1.1.2/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/models/config.py` & `UEVaultManager-1.1.1.2/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/models/downloading.py` & `UEVaultManager-1.1.1.2/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/models/egl.py` & `UEVaultManager-1.1.1.2/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/models/gql.py` & `UEVaultManager-1.1.1.2/UEVaultManager/models/gql.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.1.1.2/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/models/manifest.py` & `UEVaultManager-1.1.1.2/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.1.1.2/UEVaultManager/tkgui/main.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.1.1.2/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/utils/cli.py` & `UEVaultManager-1.1.1.2/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.1.1.2/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.1.1.2/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.1.1.2/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.1.1.2/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.1.1.2/UEVaultManager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.1.1.1
+Version: 1.1.1.2
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: webview
 Provides-Extra: webview_gtk
 License-File: LICENSE
 
 Welcome to UEVaultManager
 ==========================================
-![UEVM_200x200.png](UEVaultManager%2Fassets%2FUEVM_200x200.png)
+![UEVM_200x200.png](UEVaultManager/assets/UEVM_200x200.png)
 
 | pypi                                                                                                                 | py_versions                                                                                                          | github                                                                                                                         | docs                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
 | [![Current PyPi Version](https://img.shields.io/pypi/v/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![py_versions](https://img.shields.io/pypi/pyversions/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![github](https://img.shields.io/github/v/tag/LaurentOngaro/uevaultmanager)](https://github.com/LaurentOngaro/UEVaultManager) | [![docs](https://img.shields.io/readthedocs/uevaultmanager/latest)](https://uevaultmanager.readthedocs.io/en/latest/?badge=latest) |
 
 **UEVaultManager** is an open-source assets manager that can list assets and
 their data from the Epic Games Marketplace. It is developed in Python, so
```

### Comparing `UEVaultManager-1.1.1.1/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.1.1.2/UEVaultManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.1/setup.py` & `UEVaultManager-1.1.1.2/setup.py`

 * *Files identical despite different names*

