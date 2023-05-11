# Comparing `tmp/UEVaultManager-1.0.5.tar.gz` & `tmp/UEVaultManager-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.0.5.tar", last modified: Thu Mar 30 07:06:09 2023, max compression
+gzip compressed data, was "UEVaultManager-1.1.0.tar", last modified: Thu May 11 14:51:04 2023, max compression
```

## Comparing `UEVaultManager-1.0.5.tar` & `UEVaultManager-1.1.0.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.591313 UEVaultManager-1.0.5/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     5635 2023-03-30 07:06:09.590814 UEVaultManager-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4865 2023-03-30 07:04:58.000000 UEVaultManager-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.568641 UEVaultManager-1.0.5/UEVaultManager/
--rw-rw-rw-   0        0        0      498 2023-03-30 07:05:18.000000 UEVaultManager-1.0.5/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.573747 UEVaultManager-1.0.5/UEVaultManager/api/
--rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    20251 2023-02-22 20:15:44.000000 UEVaultManager-1.0.5/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0      884 2023-02-09 18:32:33.000000 UEVaultManager-1.0.5/UEVaultManager/api/lgd.py
--rw-rw-rw-   0        0        0    52857 2023-02-23 18:25:27.000000 UEVaultManager-1.0.5/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    39556 2023-02-23 15:17:05.000000 UEVaultManager-1.0.5/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.574246 UEVaultManager-1.0.5/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.575747 UEVaultManager-1.0.5/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38025 2023-02-20 12:25:16.000000 UEVaultManager-1.0.5/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-02-21 07:29:33.000000 UEVaultManager-1.0.5/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.579313 UEVaultManager-1.0.5/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-02-09 18:32:33.000000 UEVaultManager-1.0.5/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6686 2023-02-09 18:32:33.000000 UEVaultManager-1.0.5/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    21692 2023-02-22 20:03:37.000000 UEVaultManager-1.0.5/UEVaultManager/lfs/lgndry.py
--rw-rw-rw-   0        0        0     5528 2023-02-20 12:25:16.000000 UEVaultManager-1.0.5/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3040 2023-02-20 12:31:14.000000 UEVaultManager-1.0.5/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.585314 UEVaultManager-1.0.5/UEVaultManager/models/
--rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-02-20 10:54:01.000000 UEVaultManager-1.0.5/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-02-09 18:32:33.000000 UEVaultManager-1.0.5/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     1351 2023-02-21 07:23:44.000000 UEVaultManager-1.0.5/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     3627 2023-02-09 18:32:33.000000 UEVaultManager-1.0.5/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5074 2023-02-09 15:53:35.000000 UEVaultManager-1.0.5/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0       72 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     1334 2023-02-09 15:53:35.000000 UEVaultManager-1.0.5/UEVaultManager/models/gql.py
--rw-rw-rw-   0        0        0     5891 2023-02-09 18:32:33.000000 UEVaultManager-1.0.5/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30499 2023-02-16 16:54:16.000000 UEVaultManager-1.0.5/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.590314 UEVaultManager-1.0.5/UEVaultManager/utils/
--rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3455 2023-02-16 17:11:16.000000 UEVaultManager-1.0.5/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     2243 2023-02-20 18:25:41.000000 UEVaultManager-1.0.5/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1075 2023-02-21 07:29:33.000000 UEVaultManager-1.0.5/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10270 2023-02-21 07:23:45.000000 UEVaultManager-1.0.5/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      309 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      562 2023-02-09 17:53:24.000000 UEVaultManager-1.0.5/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     5891 2023-02-20 12:31:14.000000 UEVaultManager-1.0.5/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.572236 UEVaultManager-1.0.5/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     5635 2023-03-30 07:06:09.000000 UEVaultManager-1.0.5/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2023-03-30 07:06:09.000000 UEVaultManager-1.0.5/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 07:06:09.000000 UEVaultManager-1.0.5/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-03-30 07:06:09.000000 UEVaultManager-1.0.5/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-03-30 07:06:09.000000 UEVaultManager-1.0.5/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-30 07:06:09.000000 UEVaultManager-1.0.5/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 07:06:09.591313 UEVaultManager-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1849 2023-03-30 07:02:19.000000 UEVaultManager-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 14:51:04.669156 UEVaultManager-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5700 2023-05-11 14:51:04.668157 UEVaultManager-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4930 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 14:51:04.583196 UEVaultManager-1.1.0/UEVaultManager/
+-rw-rw-rw-   0        0        0      717 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 14:51:04.613197 UEVaultManager-1.1.0/UEVaultManager/api/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    20251 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0      884 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/api/lgd.py
+-rw-rw-rw-   0        0        0    61539 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    42168 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-05-11 14:51:04.614197 UEVaultManager-1.1.0/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 14:51:04.618198 UEVaultManager-1.1.0/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38025 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-11 14:51:04.628197 UEVaultManager-1.1.0/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6686 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    22112 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/lfs/lgndry.py
+-rw-rw-rw-   0        0        0     5528 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3040 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-11 14:51:04.644920 UEVaultManager-1.1.0/UEVaultManager/models/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     1351 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5078 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0       72 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     1334 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/models/gql.py
+-rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30499 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-05-11 14:51:04.647920 UEVaultManager-1.1.0/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0      933 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 14:51:04.667159 UEVaultManager-1.1.0/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.0/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3455 2023-05-11 14:38:29.000000 UEVaultManager-1.1.0/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5577 2023-05-11 14:38:29.000000 UEVaultManager-1.1.0/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1075 2023-05-11 14:38:29.000000 UEVaultManager-1.1.0/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10270 2023-05-11 14:38:29.000000 UEVaultManager-1.1.0/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      309 2023-05-11 14:38:29.000000 UEVaultManager-1.1.0/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      562 2023-05-11 14:38:29.000000 UEVaultManager-1.1.0/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:29.000000 UEVaultManager-1.1.0/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-05-11 14:51:04.605197 UEVaultManager-1.1.0/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     5700 2023-05-11 14:51:04.000000 UEVaultManager-1.1.0/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1409 2023-05-11 14:51:04.000000 UEVaultManager-1.1.0/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 14:51:04.000000 UEVaultManager-1.1.0/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-11 14:51:04.000000 UEVaultManager-1.1.0/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-05-11 14:51:04.000000 UEVaultManager-1.1.0/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-11 14:51:04.000000 UEVaultManager-1.1.0/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 14:51:04.669156 UEVaultManager-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1900 2023-05-11 14:38:29.000000 UEVaultManager-1.1.0/setup.py
```

### Comparing `UEVaultManager-1.0.5/LICENSE` & `UEVaultManager-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/PKG-INFO` & `UEVaultManager-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.0.5
+Version: 1.1.0
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: webview
 Provides-Extra: webview_gtk
 License-File: LICENSE
 
 Welcome to UEVaultManager
 ==========================================
+![UEVM_200x200.png](UEVaultManager%2Fassets%2FUEVM_200x200.png)
 
 | pypi                                                                                                                 | py_versions                                                                                                          | github                                                                                                                         | docs                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
 | [![Current PyPi Version](https://img.shields.io/pypi/v/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![py_versions](https://img.shields.io/pypi/pyversions/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![github](https://img.shields.io/github/v/tag/LaurentOngaro/uevaultmanager)](https://github.com/LaurentOngaro/UEVaultManager) | [![docs](https://img.shields.io/readthedocs/uevaultmanager/latest)](https://uevaultmanager.readthedocs.io/en/latest/?badge=latest) |
 
 **UEVaultManager** is an open-source assets manager that can list assets and
 their data from the Epic Games Marketplace. It is developed in Python, so
```

### Comparing `UEVaultManager-1.0.5/README.md` & `UEVaultManager-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Welcome to UEVaultManager
 ==========================================
+![UEVM_200x200.png](UEVaultManager%2Fassets%2FUEVM_200x200.png)
 
 | pypi                                                                                                                 | py_versions                                                                                                          | github                                                                                                                         | docs                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
 | [![Current PyPi Version](https://img.shields.io/pypi/v/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![py_versions](https://img.shields.io/pypi/pyversions/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![github](https://img.shields.io/github/v/tag/LaurentOngaro/uevaultmanager)](https://github.com/LaurentOngaro/UEVaultManager) | [![docs](https://img.shields.io/readthedocs/uevaultmanager/latest)](https://uevaultmanager.readthedocs.io/en/latest/?badge=latest) |
 
 **UEVaultManager** is an open-source assets manager that can list assets and
 their data from the Epic Games Marketplace. It is developed in Python, so
```

### Comparing `UEVaultManager-1.0.5/UEVaultManager/api/egs.py` & `UEVaultManager-1.1.0/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/api/lgd.py` & `UEVaultManager-1.1.0/UEVaultManager/api/lgd.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/cli.py` & `UEVaultManager-1.1.0/UEVaultManager/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,20 +11,25 @@
 import webbrowser
 from collections import namedtuple
 from datetime import datetime
 from logging.handlers import QueueListener
 from multiprocessing import freeze_support, Queue as MPQueue
 from platform import platform
 from sys import exit, stdout, platform as sys_platform
-
+import UEVaultManager.tkgui.modules.functions as gui_f  # using the shortest variable name for globals for convenience
+import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
+# noinspection PyPep8Naming
+import UEVaultManager.tkgui.modules.UEVMGuiClass as gui_w  # using the shortest variable name for globals for convenience
 from UEVaultManager import __version__, __codename__
 from UEVaultManager.api.egs import create_empty_assets_extras
 from UEVaultManager.core import AppCore, CSV_headings
 from UEVaultManager.models.exceptions import InvalidCredentialsError
-from UEVaultManager.utils.cli import strtobool, check_and_create_path
+from UEVaultManager.tkgui.modules.ProgressWindowsClass import ProgressWindow
+from UEVaultManager.tkgui.modules.SaferDictClass import SaferDict
+from UEVaultManager.utils.cli import str_to_bool, check_and_create_path, create_list_from_string
 from UEVaultManager.utils.custom_parser import HiddenAliasSubparsersAction
 
 # todo custom formatter for cli logger (clean info, highlighted error/warning)
 logging.basicConfig(format='[%(name)s] %(levelname)s: %(message)s', level=logging.INFO)
 
 
 class UEVaultManagerCLI:
@@ -74,56 +79,70 @@
             self.logger.info(f'File {file_src} has not been found')
 
     def create_log_file_backup(self):
         self.create_file_backup(self.core.ignored_assets_filename_log)
         self.create_file_backup(self.core.notfound_assets_filename_log)
         self.create_file_backup(self.core.bad_data_assets_filename_log)
 
-    def create_asset_from_data(self, item, asset_id, no_data_text, no_data_value):
+    def create_asset_from_data(self, item, asset_id, no_text_data, no_int_data, no_float_data, bool_true_data, bool_false_data):
         record = {}
         metadata = item.metadata
         uid = metadata['id']
         category = metadata['categories'][0]['path']
         separator = ','
         try:
             tmp_list = [separator.join(item.get('compatibleApps')) for item in metadata['releaseInfo']]
             compatible_versions = separator.join(tmp_list)
         except TypeError as error:
             self.logger.warning(f'Error getting compatibleApps {item.app_name} : {error!r}')
-            compatible_versions = no_data_text
+            compatible_versions = no_text_data
         thumbnail_url = ''
         try:
             thumbnail_url = metadata['keyImages'][2]['url']  # 'Image' with 488 height
         except IndexError:
             self.logger.debug(f'asset {item.app_name} has no image')
         date_added = datetime.now().strftime(self.core.default_datetime_format)
         extras_data = None
         try:
             extras_data = self.core.lgd.get_item_extras(item.app_name)
         except AttributeError as error:
             self.logger.warning(f'Error getting extra data for {item.app_name} : {error!r}')
         if extras_data is None:
             extras_data = create_empty_assets_extras(item.app_name)
-        asset_url = no_data_text
-        review = no_data_value
-        price = no_data_value
-        purchased = False
-        supported_versions = no_data_text
-        page_title = no_data_text
-        grab_result = no_data_value
+        asset_url = no_text_data
+        review = no_int_data
+        price = no_float_data
+        purchased = bool_false_data
+        supported_versions = no_text_data
+        page_title = no_text_data
+        grab_result = no_int_data
         try:
             asset_url = extras_data['asset_url']
             review = extras_data['review']
             price = extras_data['price']
             purchased = extras_data['purchased']
             supported_versions = extras_data['supported_versions']
             page_title = extras_data['page_title']
             grab_result = extras_data['grab_result']
         except (TypeError, KeyError) as error:
             self.logger.warning(f'Key not found in extra data for {item.app_name} : {error!r}')
+
+        if self.core.engine_version_for_obsolete_assets == '' or supported_versions == '' or supported_versions == no_text_data:
+            obsolete = bool_false_data
+        else:
+            supported_versions_list = supported_versions.lower().replace('UE_', '')
+            supported_versions_list = create_list_from_string(supported_versions_list)
+            obsolete = bool_true_data
+            for _, version in enumerate(supported_versions_list):
+                if version == '':
+                    continue
+                else:
+                    if float(self.core.engine_version_for_obsolete_assets) >= float(version):
+                        obsolete = bool_false_data
+                        break
         try:
             values = (
                 # dans les infos
                 asset_id  # 'asset_id'
                 , item.app_name  # 'App name'
                 , item.app_title  # 'App title'
                 , category  # 'Category'
@@ -137,29 +156,30 @@
                 , uid  # 'Uid'
                 , metadata['creationDate']  # 'Creation Date'
                 , metadata['lastModifiedDate']  # 'Update Date'
                 , metadata['status']  # 'status'
                 # Modified Fields when added into the file
                 , date_added  # 'Date Added'
                 , price  # 'Price'
-                , no_data_value  # 'Old Price'
-                , False  # 'On Sale'
+                , no_float_data  # 'Old Price'
+                , bool_false_data  # 'On Sale'
                 , purchased  # 'Purchased'
+                , obsolete  # 'obsolete'
                 # Extracted from page, can be compared with value in metadata. Coud be used to if check data grabbing if OK
                 , supported_versions  # 'supported versions'
                 , page_title  # 'page title'
                 , grab_result  # 'grab result'
                 # Modified Fields when added into the file
-                , no_data_text  # 'Comment'
-                , no_data_text  # 'Stars'
-                , no_data_text  # 'Asset Folder'
-                , no_data_value  # 'Must Buy'
-                , no_data_text  # 'Test result
-                , no_data_text  # 'Installed Folder'
-                , no_data_text  # 'Alternative'
+                , no_text_data  # 'Comment'
+                , no_float_data  # 'Stars'
+                , no_text_data  # 'Asset Folder'
+                , bool_false_data  # 'Must Buy'
+                , no_text_data  # 'Test result
+                , no_text_data  # 'Installed Folder'
+                , no_text_data  # 'Alternative'
             )
             record = dict(zip(CSV_headings.keys(), values))
         except TypeError:
             self.logger.error(f'Could not create record for {item.app_name}')
 
         return asset_id, record
 
@@ -246,66 +266,81 @@
 
     def list_assets(self, args):
 
         def update_and_merge_csv_record_data(_asset, _items_in_file, _no_data_value) -> []:
             _asset_id = _asset[0]
             _csv_record = list(_asset[1].values())  # we need a list for the CSV comparison, not a dict
             # merge data from the items in the file (if exists) and those get by the application
-            # items_in_file is a dict of dict
+            # items_in_file must be a dict of dicts
             if _items_in_file.get(_asset_id):
-                # loops through its columns
-                index = 0
-                price_index = 0
-                _price = float(_no_data_value)
-                old_price = float(_no_data_value)
-                on_sale = _no_data_value
-                for key, keep_value_in_file in CSV_headings.items():
-                    if keep_value_in_file:
-                        _csv_record[index] = _items_in_file[_asset_id][key]
-                    # Get the old price in the previous file
-                    if key == 'Price':
-                        price_index = index
-                        try:
-                            _price = float(_csv_record[price_index])
-                            old_price = float(
-                                _items_in_file[_asset_id][key]
-                            )  # NOTE: the 'old price' is the 'price' saved in the file, not the 'old_price' in the file
-                        except Exception as _error:
-                            self.logger.warning(f'Price values can not be converted for asset {_asset_id}\nError:{_error!r}')
-                    index += 1
+                item_in_file = _items_in_file.get(_asset_id)
+                if len(item_in_file.keys()) != len(CSV_headings.keys()):
+                    self.logger.error(
+                        f'In the existing file, asset {_asset_id} has not the same number of keys as the CSV headings. This asset is ignored and its values will be overwritten'
+                    )
+                    return _csv_record
+                else:
+                    # loops through its columns
+                    index = 0
+                    price_index = 0
+                    _price = float(_no_data_value)
+                    old_price = float(_no_data_value)
+                    on_sale = _no_data_value
+                    for key, keep_value_in_file in CSV_headings.items():
+                        if item_in_file[key] is None:
+                            self.logger.error(
+                                f'In the existing file, asset {_asset_id} has no column named {key}. This asset is ignored and its values will be overwritten'
+                            )
+                            # print(f' CHECK for asset {_asset_id}')
+                            return _csv_record
+                        else:
+                            if keep_value_in_file:
+                                _csv_record[index] = item_in_file[key]
+                            # Get the old price in the previous file
+                            if key == 'Price':
+                                price_index = index
+                                try:
+                                    _price = float(_csv_record[price_index])
+                                    old_price = float(
+                                        item_in_file[key]
+                                    )  # NOTE: the 'old price' is the 'price' saved in the file, not the 'old_price' in the file
+                                except Exception as _error:
+                                    self.logger.warning(f'Old Price value can not be converted for asset {_asset_id}\nError:{_error!r}')
+                        index += 1
+
                 # compute the price related fields
                 if price_index > 0 and (isinstance(old_price, int) or isinstance(old_price, float)):
                     on_sale = True if _price > old_price else False
                 _csv_record[price_index + 1] = old_price
                 _csv_record[price_index + 2] = on_sale
             return _csv_record
 
-        def update_and_merge_json_record_data(_asset, _items_in_file, _no_data_value) -> dict:
+        def update_and_merge_json_record_data(_asset, _items_in_file, _no_float_value, _no_bool_false_value) -> dict:
             _asset_id = _asset[0]
             _json_record = _asset[1]
 
             # merge data from the items in the file (if exists) and those get by the application
             # items_in_file is a dict of dict
             if _items_in_file.get(_asset_id):
                 # loops through its columns
-                _price = float(_no_data_value)
-                old_price = float(_no_data_value)
-                on_sale = _no_data_value
+                _price = float(_no_float_value)
+                old_price = float(_no_float_value)
+                on_sale = _no_bool_false_value
                 for key, keep_value_in_file in CSV_headings.items():
                     if keep_value_in_file and _items_in_file[_asset_id].get(key):
                         _json_record[key] = _items_in_file[_asset_id][key]
 
                 # Get the old price in the previous file
                 try:
                     _price = float(_json_record['Price'])
                     old_price = float(
                         _items_in_file[_asset_id]['Price']
                     )  # NOTE: the 'old price' is the 'price' saved in the file, not the 'old_price' in the file
                 except Exception as _error:
-                    self.logger.warning(f'Price values can not be converted for asset {_asset_id}\nError:{_error!r}')
+                    self.logger.warning(f'Old Price values can not be converted for asset {_asset_id}\nError:{_error!r}')
 
                 # compute the price related fields
                 if isinstance(old_price, int) or isinstance(old_price, float):
                     on_sale = True if _price > old_price else False
                 _json_record['Old Price'] = old_price
                 _json_record['On Sale'] = on_sale
             return _json_record
@@ -317,51 +352,101 @@
 
         if args.force_refresh:
             self.logger.info('Refreshing asset list, this may take a while...')
         else:
             self.logger.info('Getting asset list... (this may take a while)')
 
         if args.filter_category:
-            self.logger.info(f'The String "{args.filter_category}" will be search in Assets category')
+            gui_g.UEVM_filter_category = args.filter_category
+
+        if gui_g.UEVM_filter_category != '' and gui_g.UEVM_filter_category != gui_g.s.default_category_for_all:
+            self.logger.info(f'The String "{gui_g.UEVM_filter_category }" will be search in Assets category')
+
+        gui_g.progress_window_ref = None
+        progress_window = None
+        if args.gui:
+            # check if the GUI is already running
+            if gui_g.UEVM_gui_ref is None:
+                # create a fake root because ProgressWindow must always be a top level window
+                gui_g.UEVM_gui_ref = gui_w.UEVMGuiHiddenRoot()
+                uewm_gui_exists = False
+            else:
+                uewm_gui_exists = True
+            # create and use a progress window (as a top level window)
+            gui_g.UEVM_log_ref = self.logger
+            progress_window = ProgressWindow(
+                title="Updating Assets List",
+                quit_on_close=not uewm_gui_exists,
+                width=300,
+                height=150,
+                max_value=200,
+                show_start_button=False,
+                show_stop_button=True,
+                function=self.core.get_asset_list,
+                function_parameters={
+                    'filter_category': gui_g.UEVM_filter_category,
+                    'force_refresh': args.force_refresh
+                }
+            )
+            if uewm_gui_exists:
+                # if the main gui is running, we already have a tk.mainloop running
+                # we need to constantly update the progress bar
+                while not progress_window.must_end:
+                    progress_window.update()
+            else:
+                # if the main gui is not running, we need to start a tk.mainloop
+                progress_window.mainloop()
+
+            items = progress_window.get_result()
 
-        items = self.core.get_asset_list(platform='Windows', filter_category=args.filter_category, force_refresh=args.force_refresh)
+        else:
+            items = self.core.get_asset_list(platform='Windows', filter_category=args.filter_category, force_refresh=args.force_refresh)
 
         if args.include_non_asset:
             na_items = self.core.get_non_asset_library_items(skip_ue=False)
             items.extend(na_items)
 
-        no_data_value = 0
-        no_data_text = 'N.A.'
+        no_int_data = 0
+        no_float_value = 0.0
+        no_text_data = ''
+        no_bool_true_data = True
+        no_bool_false_data = False
 
         # sort assets by name in reverse (to have the latest version first
         items = sorted(items, key=lambda x: x.app_name.lower(), reverse=True)
 
         # use a dict to store records and avoid duplicates (asset with the same asset_id and a different asset_name)
         assets_to_output = {}
         # create a minimal and full dict of data from existing assets
         assets_in_file = {}
 
         cpt = 0
         cpt_max = len(items)
+        if gui_g.progress_window_ref is not None:
+            gui_g.progress_window_ref.reset(new_value=0, new_text="Checking assets data...", new_max_value=len(items))
         for item in items:
+            if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
+                return
             cpt += 1
             # notes:
             #   asset_id is not unique because somme assets can have the same asset_id but with several UE versions
             #   app_name is unique because it includes the unreal version
             #   we use asset_id as key because we don't want to have several entries for the same asset
             #   some asset won't have asset_infos (mainly when using the -T option), in that case we use the app_title as asset_id
             if item.asset_infos.get('Windows'):
                 asset_id = item.asset_infos['Windows'].asset_id
             else:
                 asset_id = item.app_title
 
             if assets_to_output.get(asset_id):
                 self.logger.debug(f'Asset {asset_id} already present in the list (usually with another ue version)')
             else:
-                asset_id, asset = self.create_asset_from_data(item, asset_id, no_data_text, no_data_value)  # asset is a dict
+                asset_id, asset = self.create_asset_from_data(
+                    item, asset_id, no_text_data, no_int_data, no_float_value, no_bool_true_data, no_bool_false_data
+                )  # asset is a dict
                 assets_to_output[asset_id] = asset
 
             if self.core.verbose_mode:
                 self.logger.info(f'Asset id={asset_id} has been created from data. Done {cpt}/{cpt_max} items')
 
         # output with extended info
         if args.output and (args.csv or args.tsv or args.json) and self.core.create_output_backup:
@@ -372,14 +457,15 @@
                 file_src = args.output
                 # If the output file exists, we read its content to keep some data
                 try:
                     with open(file_src, 'r', encoding='utf-8') as output:
                         csv_file_content = csv.DictReader(output)
                         # get the data (it's a dict)
                         for csv_record in csv_file_content:
+                            # noinspection PyTypeChecker
                             asset_id = csv_record['Asset_id']
                             assets_in_file[asset_id] = csv_record
                         output.close()
                 except (FileExistsError, OSError, UnicodeDecodeError, StopIteration):
                     self.logger.warning(f'Could not read CSV record from the file {args.output}')
 
                 # write the content of the file to keep some data
@@ -392,31 +478,39 @@
                 output = stdout
             # end if args.output:
 
             try:
                 writer = csv.writer(output, dialect='excel-tab' if args.tsv else 'excel', lineterminator='\n')
                 writer.writerow(CSV_headings.keys())
                 cpt = 0
+                if gui_g.progress_window_ref is not None:
+                    gui_g.progress_window_ref.reset(
+                        new_value=0, new_text="Writing assets into csv file...", new_max_value=len(assets_to_output.items())
+                    )
                 for asset in sorted(assets_to_output.items()):
+                    if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
+                        return
                     asset_id = asset[0]
                     try:
                         if len(assets_in_file) > 0:
-                            csv_record_merged = update_and_merge_csv_record_data(asset, assets_in_file, no_data_value)
+                            csv_record_merged = update_and_merge_csv_record_data(asset, assets_in_file, no_int_data)
                         else:
-                            csv_record_merged = asset
+                            csv_record_merged = list(asset[1].values())
                         cpt += 1
                         writer.writerow(csv_record_merged)
                     except (OSError, UnicodeEncodeError, TypeError) as error:
                         self.logger.error(f'Could not write CSV record for {asset_id} into {args.output}\nError:{error!r}')
             except OSError:
                 self.logger.error(f'Could not write list result to {args.output}')
             output.close()
             self.logger.info(
                 f'\n======\n{cpt} assets have been printed or saved (without duplicates due to different UE versions)\nOperation Finished\n======\n'
             )
+            if args.gui and progress_window is not None:
+                progress_window.close_window()
             return
         # end if args.csv or args.tsv:
 
         if args.json:
             if args.output:
                 file_src = args.output
                 # If the output file exists, we read its content to keep some data
@@ -436,46 +530,51 @@
             else:
                 output = stdout
             # end if args.output:
 
             try:
                 cpt = 0
                 json_content = {}
-                # output.write("{\n")
+                if gui_g.progress_window_ref is not None:
+                    gui_g.progress_window_ref.reset(
+                        new_value=0, new_text="Writing assets into json file...", new_max_value=len(assets_to_output.items())
+                    )
                 for asset in sorted(assets_to_output.items()):
+                    if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
+                        return
                     asset_id = asset[0]
                     if len(assets_in_file) > 0:
-                        json_record_merged = update_and_merge_json_record_data(asset, assets_in_file, no_data_value)
+                        json_record_merged = update_and_merge_json_record_data(asset, assets_in_file, no_float_value, no_bool_false_data)
                     else:
                         json_record_merged = asset[1]
-            #      output.write(",\n")
+                    #      output.write(",\n")
                     try:
                         asset_id = json_record_merged['Asset_id']
                         json_content[asset_id] = json_record_merged
                         cpt += 1
                     except (OSError, UnicodeEncodeError, TypeError) as error:
                         self.logger.error(f'Could not write Json record for {asset_id} into {args.output}\nError:{error!r}')
 
                 json.dump(json_content, output, indent=2)
             except OSError:
                 self.logger.error(f'Could not write list result to {args.output}')
-
             output.close()
             self.logger.info(
                 f'\n======\n{cpt} assets have been printed or saved (without duplicates due to different UE versions)\nOperation Finished\n======\n'
             )
+            if args.gui and progress_window is not None:
+                progress_window.close_window()
             return
         # end if args.json:
 
         # here, no other output has been done before, so we print the asset in a quick format to the console
         print('\nAvailable UE Assets:')
         for asset in items:
             version = asset.app_version('Windows')
             print(f' * {asset.app_title.strip()} (App name: {asset.app_name} | Version: {version})')
-
         print(f'\nTotal: {len(items)}')
 
     def list_files(self, args):
         if not args.override_manifest and not args.app_name:
             print('You must provide either a manifest url/path or app name!')
             return
         elif args.app_name:
@@ -799,14 +898,48 @@
             if args.pretty_json:
                 print(json.dumps(token, indent=2, sort_keys=True))
             else:
                 print(json.dumps(token))
             return
         self.logger.info(f'Exchange code: {token["code"]}')
 
+    def edit_assets(self, args):
+        if not args.input:
+            input_filename = gui_g.s.csv_filename
+            self.logger.warning('The file to read data from has not been precised by the --input command option. The default file name will be used.')
+        else:
+            input_filename = gui_f.path_from_relative_to_absolute(args.input)
+
+        app_icon_filename = gui_f.path_from_relative_to_absolute(gui_g.s.app_icon_filename)
+        gui_g.UEVM_log_ref = self.logger
+        gui_g.UEVM_cli_ref = self
+        # args can not be used as it because it's an object that mainly run as a dict (but it's not)
+        # so we need to convert it to a dict first
+        temp_dict = vars(args)
+        # set output file name from the input one. Used by the "rebuild file content" button (or rebuild_data method)
+        temp_dict['output'] = input_filename
+        temp_dict['csv'] = True  # force csv output
+        temp_dict['gui'] = True
+        # create a SaferDict object from the dict (it will avoid errors when trying to access non-existing keys)
+        gui_g.UEVM_cli_args = SaferDict({})
+        # copy the dict content to the SaferDict object
+        gui_g.UEVM_cli_args.copy_from(temp_dict)
+
+        gui_g.UEVM_gui_ref = gui_w.UEVMGui(
+            title=gui_g.s.app_title,
+            width=gui_g.s.app_width,
+            height=gui_g.s.app_height,
+            icon=app_icon_filename,
+            screen_index=0,
+            file=input_filename,
+            show_open_file_dialog=not os.path.isfile(input_filename),
+        )
+        gui_g.UEVM_gui_ref.mainloop()
+        # gui_g.UEVM_gui_ref.quit()
+
 
 def main():
     parser = argparse.ArgumentParser(description=f'UEVaultManager v{__version__} - "{__codename__}"')
     parser.register('action', 'parsers', HiddenAliasSubparsersAction)
 
     # general arguments
     parser.add_argument('-H', '--full-help', dest='full_help', action='store_true', help='Show full help (including individual command help)')
@@ -832,14 +965,15 @@
     subparsers = parser.add_subparsers(title='Commands', dest='subparser_name', metavar='<command>')
     auth_parser = subparsers.add_parser('auth', help='Authenticate with the Epic Games Store')
     clean_parser = subparsers.add_parser('cleanup', help='Remove old temporary, metadata, and manifest files')
     info_parser = subparsers.add_parser('info', help='Prints info about specified app name or manifest')
     list_parser = subparsers.add_parser('list', aliases=('list-assets',), hide_aliases=True, help='List available assets')
     list_files_parser = subparsers.add_parser('list-files', help='List files in manifest')
     status_parser = subparsers.add_parser('status', help='Show UEVaultManager status information')
+    edit_parser = subparsers.add_parser('edit', aliases=('edit-assets',), hide_aliases=True, help='Edit the assets list file')
 
     # hidden commands have no help text
     get_token_parser = subparsers.add_parser('get-token')
 
     # Positional arguments
     list_files_parser.add_argument('app_name', nargs='?', metavar='<App Name>', help='Name of the app (optional)')
     info_parser.add_argument('app_name_or_manifest', help='App name or manifest path/URI', metavar='<App Name/Manifest URI>')
@@ -872,14 +1006,21 @@
         '-T', '--third-party', dest='include_non_asset', action='store_true', default=False, help='Include assets that are not installable.'
     )
     list_parser.add_argument('--csv', dest='csv', action='store_true', help='Output in in CSV format')
     list_parser.add_argument('--tsv', dest='tsv', action='store_true', help='Output in in TSV format')
     list_parser.add_argument('--json', dest='json', action='store_true', help='Output in in JSON format')
     list_parser.add_argument('-f', '--force-refresh', dest='force_refresh', action='store_true', help='Force a refresh of all assets metadata')
     list_parser.add_argument(
+        '-g',
+        '--gui',
+        dest='gui',
+        action='store_true',
+        help='Display additional informations using gui elements like dialog boxes or progress window'
+    )
+    list_parser.add_argument(
         '-fc',
         '--filter-category',
         dest='filter_category',
         action='store',
         help='Filter assets by category. Search against the asset category in the marketplace. Search is case insensitive and can be partial'
     )
     list_parser.add_argument(
@@ -912,14 +1053,22 @@
     info_parser.add_argument('--offline', dest='offline', action='store_true', help='Only print info available offline')
     info_parser.add_argument('--json', dest='json', action='store_true', help='Output information in JSON format')
     info_parser.add_argument('-f', '--force-refresh', dest='force_refresh', action='store_true', help='Force a refresh of all assets metadata')
 
     get_token_parser.add_argument('--json', dest='json', action='store_true', help='Output information in JSON format')
     get_token_parser.add_argument('--bearer', dest='bearer', action='store_true', help='Return fresh bearer token rather than an exchange code')
 
+    edit_parser.add_argument(
+        '-i', '--input', dest='input', metavar='<path/name>', action='store', help='The file name (with path) where the list should be read from'
+    )
+    # not use for now
+    # edit_parser.add_argument('--csv', dest='csv', action='store_true', help='Input file is in CSV format')
+    # edit_parser.add_argument('--tsv', dest='tsv', action='store_true', help='Input file is in TSV format')
+    # edit_parser.add_argument('--json', dest='json', action='store_true', help='Input file is in JSON format')
+
     args, extra = parser.parse_known_args()
 
     if args.version:
         print(f'UEVaultManager version "{__version__}", codename "{__codename__}"')
         exit(0)
 
     if not args.subparser_name or args.full_help:
@@ -953,23 +1102,25 @@
     if conf_log_level == 'debug' or args.debug:
         cli.core.verbose_mode = True
         logging.getLogger().setLevel(level=logging.DEBUG)
         # keep requests quiet
         logging.getLogger('requests').setLevel(logging.WARNING)
         logging.getLogger('urllib3').setLevel(logging.WARNING)
 
-    cli.core.create_output_backup = strtobool(cli.core.lgd.config.get('UEVaultManager', 'create_output_backup', fallback=True))
-    cli.core.create_log_backup = strtobool(cli.core.lgd.config.get('UEVaultManager', 'create_log_backup', fallback=True))
-    cli.core.verbose_mode = strtobool(cli.core.lgd.config.get('UEVaultManager', 'verbose_mode', fallback=False))
+    cli.core.create_output_backup = str_to_bool(cli.core.lgd.config.get('UEVaultManager', 'create_output_backup', fallback=True))
+    cli.core.create_log_backup = str_to_bool(cli.core.lgd.config.get('UEVaultManager', 'create_log_backup', fallback=True))
+    cli.core.verbose_mode = str_to_bool(cli.core.lgd.config.get('UEVaultManager', 'verbose_mode', fallback=False))
     cli.ue_assets_max_cache_duration = int(cli.core.lgd.config.get('UEVaultManager', 'ue_assets_max_cache_duration', fallback=1296000))
 
     cli.core.ignored_assets_filename_log = cli.core.lgd.config.get('UEVaultManager', 'ignored_assets_filename_log', fallback='')
     cli.core.notfound_assets_filename_log = cli.core.lgd.config.get('UEVaultManager', 'notfound_assets_filename_log', fallback='')
     cli.core.bad_data_assets_filename_log = cli.core.lgd.config.get('UEVaultManager', 'bad_data_assets_filename_log', fallback='')
 
+    cli.core.engine_version_for_obsolete_assets = cli.core.lgd.config.get('UEVaultManager', 'engine_version_for_obsolete_assets', fallback='4.26')
+
     if cli.core.create_log_backup:
         cli.create_log_file_backup()
 
     # open log file for assets if necessary
     cli.core.setup_assets_logging()
     cli.core.egs.notfound_logger = cli.core.notfound_logger
     cli.core.egs.ignored_logger = cli.core.ignored_logger
@@ -991,14 +1142,16 @@
             cli.status(args)
         elif args.subparser_name == 'info':
             cli.info(args)
         elif args.subparser_name == 'cleanup':
             cli.cleanup(args)
         elif args.subparser_name == 'get-token':
             cli.get_token(args)
+        elif args.subparser_name in {'edit', 'edit-assets'}:
+            cli.edit_assets(args)
     except KeyboardInterrupt:
         cli.logger.info('Command was aborted via KeyboardInterrupt, cleaning up...')
 
     # Disable the update message if JSON/TSV/CSV outputs are used
     disable_update_message = False
     if hasattr(args, 'json'):
         disable_update_message = args.json
```

### Comparing `UEVaultManager-1.0.5/UEVaultManager/core.py` & `UEVaultManager-1.1.0/UEVaultManager/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # coding: utf-8
 
 import json
 import logging
 import os
 import time
+import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
 from base64 import b64decode
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timedelta
 from hashlib import sha1
 from locale import getlocale, LC_CTYPE
 from platform import system
 from threading import current_thread, enumerate as thread_enumerate
@@ -31,15 +32,15 @@
 # The heading dict contains the title of each column and a boolean value to know if its contents must be preserved if it already exists in the output file (To Avoid overwriting data changed by the user in the file)
 CSV_headings = {
     'Asset_id': False,  # ! important: Do not Rename => this field is used as main key for each asset
     'App name': False,
     'App title': False,
     'Category': False,
     'Image': False,
-    'Url': False,
+    'Url': True,  # could be kept if a better url that can be used to download the asset is found
     'UE Version': False,
     'Compatible Versions': False,
     'Review': False,
     'Developer': False,
     'Description': False,
     'Uid': False,
     'Creation Date': False,
@@ -47,14 +48,15 @@
     'Status': False,
     # Modified Fields when added into the file (mainly from extras data)
     'Date Added': True,
     'Price': False,  # ! important: Rename Wisely => this field is searched by text in the next lines
     'Old Price': False,  # ! important: always place it after the Price field in the list
     'On Sale': False,  # ! important: always place it after the Old Price field in the list
     'Purchased': False,
+    'Obsolete': True,
     # Extracted from page, can be compared with value in metadata. Coud be used to if check data grabbing if OK
     'Supported Versions': False,
     'Page title': False,
     'Grab result': False,
     # User Fields
     'Comment': True,
     'Stars': True,
@@ -133,14 +135,15 @@
         # new file loggers
         self.ignored_logger = None
         self.notfound_logger = None
         self.bad_data_logger = None
         # store time to process metadata and extras update
         self.process_time_average = {'time': 0.0, 'count': 0}
         self.use_threads = False
+        self.engine_version_for_obsolete_assets = '4.26'
 
     def setup_assets_logging(self):
         formatter = logging.Formatter('%(message)s')
         message = f"-----\n{datetime.now().strftime(self.default_datetime_format)} Log Started\n-----\n"
 
         if self.ignored_assets_filename_log != '':
             ignored_assets_filename_log = self.ignored_assets_filename_log.replace('~/.config', self.lgd.path)
@@ -479,39 +482,50 @@
 
         _ret = []
         meta_updated = False
 
         # fetch asset information for Windows, all installed platforms, and the specified one
         platforms = {'Windows'}
         platforms |= {platform}
-
+        if gui_g.progress_window_ref is not None:
+            gui_g.progress_window_ref.reset(new_value=0, new_text="Fetching platforms...", new_max_value=len(platforms))
         for _platform in platforms:
             self.get_assets(update_assets=update_assets, platform=_platform)
+            if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
+                return []
 
         if not self.lgd.assets:
             return _ret
 
         assets = {}
+        if gui_g.progress_window_ref is not None:
+            gui_g.progress_window_ref.reset(new_value=0, new_text="Fetching assets...", new_max_value=len(self.lgd.assets.items()))
         for _platform, _assets in self.lgd.assets.items():
             for _asset in _assets:
+                if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
+                    return []
                 if _asset.app_name in assets:
                     assets[_asset.app_name][_platform] = _asset
                 else:
                     assets[_asset.app_name] = {_platform: _asset}
 
         fetch_list = {}
         assets_bypassed = {}
         apps = {}
 
         # loop through assets items to check for if they are for ue or not
         valid_items = []
         bypass_count = 0
         self.log.info(f'======\nSTARTING phase 1: asset indexing (ue or not)\n')
+        if gui_g.progress_window_ref is not None:
+            gui_g.progress_window_ref.reset(new_value=0, new_text="Indexing assets...", new_max_value=len(assets.items()))
         # note: we sort by reverse, as it the most recent version of an asset will be listed first
         for app_name, app_assets in sorted(assets.items(), reverse=True):
+            if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
+                return []
             # notes:
             #   asset_id is not unique because somme assets can have the same asset_id but with several UE versions
             #   app_name is unique because it includes the unreal version
             # asset_id = app_assets['Windows'].asset_id
             assets_bypassed[app_name] = False
             if app_assets['Windows'].namespace != 'ue':
                 self.log.debug(f'{app_name} has been bypassed (namespace != "ue") in phase 1')
@@ -531,21 +545,24 @@
         force_refresh = self.cache_is_invalidate
         if force_refresh:
             self.log.info(f'!! Assets metadata will be updated !!\n')
         else:
             self.log.info(f"Asset metadata won't be updated\n")
 
         self.log.info(f'======\nSTARTING phase 2:asset filtering and metadata updating\n')
-
+        if gui_g.progress_window_ref is not None:
+            gui_g.progress_window_ref.reset(new_value=0, new_text="Updating metadata...", new_max_value=len(valid_items))
         # loop through valid items to check for update and filtering
         bypass_count = 0
         filtered_items = []
         currently_fetching = {}
         i = 0
         while i < len(valid_items):
+            if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
+                return []
             item = valid_items[i]
             app_name = item['name']
             app_assets = item['asset']
             if self.verbose_mode:
                 self.log.info(f'Checking {app_name}....')
 
             item_metadata = self.lgd.get_item_meta(app_name)
@@ -588,25 +605,36 @@
             filtered_items.append(item)
             # end while i < len(valid_items):
 
         # setup and teardown of thread pool takes some time, so only do it when it makes sense.
         self.use_threads = len(fetch_list) > 5
         # self.use_threads = False  # test only
         if fetch_list:
+            if gui_g.progress_window_ref is not None:
+                gui_g.progress_window_ref.reset(new_value=0, new_text="Fetching missing metadata...\nIt Could take a while !", new_max_value=0)
+                gui_g.progress_window_ref.hide_progress_bar()
+                gui_g.progress_window_ref.hide_stop_button()
+
             self.log.info(f'Fetching metadata for {len(fetch_list)} app(s).')
             if self.use_threads:
                 # note:  unreal engine API limits the number of connection to 16. So no more than 16 threads !
                 with ThreadPoolExecutor(max_workers=min(16, os.cpu_count() + 2), thread_name_prefix="Asset_Fetcher") as executor:
                     executor.map(fetch_asset_meta, fetch_list.keys(), timeout=30.0)
 
         self.log.info(f'A total of {bypass_count} on {len(valid_items)} assets have been bypassed in phase 2')
         self.log.info(f'======\nSTARTING phase 3: emptying the List of assets to be fetched \n')
+        if gui_g.progress_window_ref is not None:
+            gui_g.progress_window_ref.show_progress_bar()  # show progress bar, must be before reset
+            gui_g.progress_window_ref.show_stop_button()
+            gui_g.progress_window_ref.reset(new_value=0, new_text="Checking assets data...", new_max_value=len(filtered_items))
         # loop through valid and filtered items
         meta_updated = (bypass_count == 0) and meta_updated  # to avoid deleting metadata files or assets that have been filtered
         while len(filtered_items) > 0:
+            if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
+                return []
             item = filtered_items.pop()
             app_name = item['name']
             app_assets = item['asset']
             if self.verbose_mode:
                 self.log.info(f'Checking {app_name}. Still {len(filtered_items)} assets to check')
             try:
                 app_item = apps.get(app_name)
@@ -622,17 +650,20 @@
                     del currently_fetching[app_name]
                 fetch_asset_meta(app_name)
 
             try:
                 is_bypassed = (app_name in assets_bypassed) and (assets_bypassed[app_name])
                 is_a_mod = any(i['path'] == 'mods' for i in app_item.metadata.get('categories', []))
             except (KeyError, IndexError, AttributeError):
-                self.log.debug(f'{app_name} has no metadata. adding to fetch list (again)')
-                fetch_list[app_name] = (app_name, item.namespace, item.catalog_item_id, True, True)
-                _ret.append(app_item)
+                self.log.debug(f'{app_name} has no metadata. Adding to the fetch list (again)')
+                try:
+                    fetch_list[app_name] = (app_name, item.namespace, item.catalog_item_id, True, True)
+                    _ret.append(app_item)
+                except (KeyError, IndexError, AttributeError):
+                    self.log.debug(f'{app_name} has an invalid format. Could not been added to the fetch list')
                 continue
 
             has_valid_platform = platform in app_assets
             is_still_fetching = (app_name in fetch_list) or (app_name in currently_fetching)
 
             if is_still_fetching:
                 # put again the asset in the list waiting when it will be fetched
```

### Comparing `UEVaultManager-1.0.5/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.1.0/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.1.0/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.1.0/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.1.0/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/lfs/lgndry.py` & `UEVaultManager-1.1.0/UEVaultManager/lfs/lgndry.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,19 +136,24 @@
             has_changed = True
         if not self.config.has_option('UEVaultManager', 'ignored_assets_filename_log'):
             self.config.set(
                 'UEVaultManager', '; Set the file name (and path) for logging issues with assets when running the --list command' + "\n" +
                 '; use "~/" at the start of the filename to store it relatively to the user directory'
             )
             self.config.set('UEVaultManager', 'ignored_assets_filename_log', '~/.config/ignored_assets.log')
+            has_changed = True
         if not self.config.has_option('UEVaultManager', 'notfound_assets_filename_log'):
             self.config.set('UEVaultManager', 'notfound_assets_filename_log', '~/.config/notfound_assets.log')
+            has_changed = True
         if not self.config.has_option('UEVaultManager', 'bad_data_assets_filename_log'):
             self.config.set('UEVaultManager', 'bad_data_assets_filename_log', '~/.config/bad_data_assets.log')
-
+            has_changed = True
+        if not self.config.has_option('UEVaultManager', 'engine_version_for_obsolete_assets'):
+            self.config.set('UEVaultManager', '; Set the minimal unreal engine version to check for obsolete assets (default is 4.26)')
+            self.config.set('UEVaultManager', 'engine_version_for_obsolete_assets', '4.26')
             has_changed = True
 
         if has_changed:
             self.save_config()
 
         # load existing app metadata
         _meta = None
```

### Comparing `UEVaultManager-1.0.5/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.1.0/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.1.0/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/models/app.py` & `UEVaultManager-1.1.0/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/models/chunk.py` & `UEVaultManager-1.1.0/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/models/config.py` & `UEVaultManager-1.1.0/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/models/downloading.py` & `UEVaultManager-1.1.0/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/models/egl.py` & `UEVaultManager-1.1.0/UEVaultManager/models/egl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from copy import deepcopy
 
-from UEVaultManager.utils.cli import strtobool
+from UEVaultManager.utils.cli import str_to_bool
 
 _template = {
     'AppCategories'         : ['public', 'games', 'applications'],
     'AppName'               : '',
     'AppVersionString'      : '',
     'BaseURLs'              : [],
     'BuildLabel'            : '',
@@ -87,15 +87,15 @@
         tmp.install_tags = json.pop('InstallTags', [])
         tmp.installation_guid = json.pop('InstallationGuid', '')
         tmp.launch_command = json.pop('LaunchCommand', '')
         tmp.executable = json.pop('LaunchExecutable', '')
         tmp.main_game_appname = json.pop('MainGameAppName', '')
         tmp.app_folder_name = json.pop('MandatoryAppFolderName', '')
         tmp.manifest_location = json.pop('ManifestLocation', '')
-        tmp.ownership_token = strtobool(json.pop('OwnershipToken', 'False'))
+        tmp.ownership_token = str_to_bool(json.pop('OwnershipToken', 'False'))
         tmp.staging_location = json.pop('StagingLocation', '')
         tmp.can_run_offline = json.pop('bCanRunOffline', True)
         tmp.is_incomplete_install = json.pop('bIsIncompleteInstall', False)
         tmp.needs_validation = json.pop('bNeedsValidation', False)
         tmp.remainder = json.copy()
         return tmp
```

### Comparing `UEVaultManager-1.0.5/UEVaultManager/models/gql.py` & `UEVaultManager-1.1.0/UEVaultManager/models/gql.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.1.0/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/models/manifest.py` & `UEVaultManager-1.1.0/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.1.0/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.1.0/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.1.0/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.1.0/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.1.0/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.5/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.1.0/UEVaultManager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.0.5
+Version: 1.1.0
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: webview
 Provides-Extra: webview_gtk
 License-File: LICENSE
 
 Welcome to UEVaultManager
 ==========================================
+![UEVM_200x200.png](UEVaultManager%2Fassets%2FUEVM_200x200.png)
 
 | pypi                                                                                                                 | py_versions                                                                                                          | github                                                                                                                         | docs                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
 | [![Current PyPi Version](https://img.shields.io/pypi/v/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![py_versions](https://img.shields.io/pypi/pyversions/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![github](https://img.shields.io/github/v/tag/LaurentOngaro/uevaultmanager)](https://github.com/LaurentOngaro/UEVaultManager) | [![docs](https://img.shields.io/readthedocs/uevaultmanager/latest)](https://uevaultmanager.readthedocs.io/en/latest/?badge=latest) |
 
 **UEVaultManager** is an open-source assets manager that can list assets and
 their data from the Epic Games Marketplace. It is developed in Python, so
```

### Comparing `UEVaultManager-1.0.5/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.1.0/UEVaultManager.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 UEVaultManager/models/config.py
 UEVaultManager/models/downloading.py
 UEVaultManager/models/egl.py
 UEVaultManager/models/exceptions.py
 UEVaultManager/models/gql.py
 UEVaultManager/models/json_manifest.py
 UEVaultManager/models/manifest.py
+UEVaultManager/tkgui/__init__.py
+UEVaultManager/tkgui/main.py
 UEVaultManager/utils/__init__.py
 UEVaultManager/utils/aliasing.py
 UEVaultManager/utils/cli.py
 UEVaultManager/utils/custom_parser.py
 UEVaultManager/utils/egl_crypt.py
 UEVaultManager/utils/env.py
 UEVaultManager/utils/rolling_hash.py
```

### Comparing `UEVaultManager-1.0.5/setup.py` & `UEVaultManager-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,18 @@
     long_description=__long_description__,
     url=__url__,
     packages=[
         'UEVaultManager',  #
         'UEVaultManager.api',  #
         'UEVaultManager.downloader',  #
         'UEVaultManager.downloader.mp',  #
-        'UEVaultManager.lfs', 'UEVaultManager.models',  #
-        'UEVaultManager.utils'
+        'UEVaultManager.lfs',  #
+        'UEVaultManager.models',  #
+        'UEVaultManager.utils',  #
+        'UEVaultManager.tkgui'  #
     ],
     entry_points=dict(console_scripts=['UEVaultManager = UEVaultManager.cli:main']),
     install_requires=[
         'requests<3.0',  #
         'setuptools',  #
         'wheel'
     ],
```

