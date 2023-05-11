# Comparing `tmp/UEVaultManager-1.1.1.2.tar.gz` & `tmp/UEVaultManager-1.1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.1.1.2.tar", last modified: Thu May 11 15:57:48 2023, max compression
+gzip compressed data, was "UEVaultManager-1.1.1.3.tar", last modified: Thu May 11 16:15:42 2023, max compression
```

## Comparing `UEVaultManager-1.1.1.2.tar` & `UEVaultManager-1.1.1.3.tar`

### file list

```diff
@@ -1,60 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.833494 UEVaultManager-1.1.1.2/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.1.1.2/LICENSE
--rw-rw-rw-   0        0        0     5698 2023-05-11 15:57:48.832394 UEVaultManager-1.1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4926 2023-05-11 15:56:47.000000 UEVaultManager-1.1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.748560 UEVaultManager-1.1.1.2/UEVaultManager/
--rw-rw-rw-   0        0        0      719 2023-05-11 15:57:03.000000 UEVaultManager-1.1.1.2/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.778662 UEVaultManager-1.1.1.2/UEVaultManager/api/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    20251 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0      884 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/api/lgd.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.781665 UEVaultManager-1.1.1.2/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0    61539 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    42168 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.782661 UEVaultManager-1.1.1.2/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.785522 UEVaultManager-1.1.1.2/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38025 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.793524 UEVaultManager-1.1.1.2/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6686 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    22112 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/lfs/lgndry.py
--rw-rw-rw-   0        0        0     5528 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3040 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.809700 UEVaultManager-1.1.1.2/UEVaultManager/models/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     1351 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5078 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0       72 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     1334 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/gql.py
--rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30499 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.811702 UEVaultManager-1.1.1.2/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0      933 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.831393 UEVaultManager-1.1.1.2/UEVaultManager/utils/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3455 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5577 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1075 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10270 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      309 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      562 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.2/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:57:48.769660 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     5698 2023-05-11 15:57:48.000000 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1479 2023-05-11 15:57:48.000000 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:57:48.000000 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-11 15:57:48.000000 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-05-11 15:57:48.000000 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-11 15:57:48.000000 UEVaultManager-1.1.1.2/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 15:57:48.833494 UEVaultManager-1.1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2051 2023-05-11 15:20:44.000000 UEVaultManager-1.1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:15:42.752555 UEVaultManager-1.1.1.3/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5698 2023-05-11 16:15:42.752555 UEVaultManager-1.1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4926 2023-05-11 15:56:47.000000 UEVaultManager-1.1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 16:15:42.642709 UEVaultManager-1.1.1.3/UEVaultManager/
+-rw-rw-rw-   0        0        0      719 2023-05-11 16:15:00.000000 UEVaultManager-1.1.1.3/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:15:42.672436 UEVaultManager-1.1.1.3/UEVaultManager/api/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    20251 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0      884 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/api/lgd.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:15:42.675437 UEVaultManager-1.1.1.3/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0    61539 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    42168 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:15:42.677436 UEVaultManager-1.1.1.3/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:15:42.680436 UEVaultManager-1.1.1.3/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38025 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:15:42.687895 UEVaultManager-1.1.1.3/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6686 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    22112 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/lfs/lgndry.py
+-rw-rw-rw-   0        0        0     5528 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3040 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:15:42.706330 UEVaultManager-1.1.1.3/UEVaultManager/models/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     1351 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5078 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0       72 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     1334 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/models/gql.py
+-rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30499 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:15:42.709335 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0      933 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:15:42.724722 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     4112 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6419 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    23010 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0     7778 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0     1124 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    10585 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+-rw-rw-rw-   0        0        0     2104 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     4910 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    24626 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0     2102 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0     9293 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0     1471 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:15:42.750554 UEVaultManager-1.1.1.3/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.3/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3455 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.3/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5577 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.3/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1075 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.3/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10270 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.3/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      309 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.3/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      562 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.3/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.3/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:15:42.665136 UEVaultManager-1.1.1.3/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     5698 2023-05-11 16:15:42.000000 UEVaultManager-1.1.1.3/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2104 2023-05-11 16:15:42.000000 UEVaultManager-1.1.1.3/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 16:15:42.000000 UEVaultManager-1.1.1.3/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-11 16:15:42.000000 UEVaultManager-1.1.1.3/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-05-11 16:15:42.000000 UEVaultManager-1.1.1.3/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-11 16:15:42.000000 UEVaultManager-1.1.1.3/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 16:15:42.753559 UEVaultManager-1.1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2174 2023-05-11 16:14:47.000000 UEVaultManager-1.1.1.3/setup.py
```

### Comparing `UEVaultManager-1.1.1.2/LICENSE` & `UEVaultManager-1.1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/PKG-INFO` & `UEVaultManager-1.1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.1.1.2
+Version: 1.1.1.3
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `UEVaultManager-1.1.1.2/README.md` & `UEVaultManager-1.1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/__init__.py` & `UEVaultManager-1.1.1.3/UEVaultManager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """UEVaultManager"""
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.1.1.2'
+__version__ = '1.1.1.3'
 # Pegasus Seiya
 # Dragon Shiryu
 # Cygnus Hyoga
 __codename__ = 'Cygnus'
 # Andromeda Shun
 # Phoenix Ikki
 # Leo Aiolia
```

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/api/egs.py` & `UEVaultManager-1.1.1.3/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/api/lgd.py` & `UEVaultManager-1.1.1.3/UEVaultManager/api/lgd.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.1.1.3/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/assets/main.ico` & `UEVaultManager-1.1.1.3/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/cli.py` & `UEVaultManager-1.1.1.3/UEVaultManager/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/core.py` & `UEVaultManager-1.1.1.3/UEVaultManager/core.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.1.1.3/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.1.1.3/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.1.1.3/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.1.1.3/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/lfs/lgndry.py` & `UEVaultManager-1.1.1.3/UEVaultManager/lfs/lgndry.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.1.1.3/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.1.1.3/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/models/app.py` & `UEVaultManager-1.1.1.3/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/models/chunk.py` & `UEVaultManager-1.1.1.3/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/models/config.py` & `UEVaultManager-1.1.1.3/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/models/downloading.py` & `UEVaultManager-1.1.1.3/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/models/egl.py` & `UEVaultManager-1.1.1.3/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/models/gql.py` & `UEVaultManager-1.1.1.3/UEVaultManager/models/gql.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.1.1.3/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/models/manifest.py` & `UEVaultManager-1.1.1.3/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.1.1.3/UEVaultManager/tkgui/main.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.1.1.3/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/utils/cli.py` & `UEVaultManager-1.1.1.3/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.1.1.3/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.1.1.3/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.1.1.3/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.1.1.3/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.1.1.3/UEVaultManager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.1.1.2
+Version: 1.1.1.3
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `UEVaultManager-1.1.1.2/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.1.1.3/UEVaultManager.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -33,14 +33,27 @@
 UEVaultManager/models/egl.py
 UEVaultManager/models/exceptions.py
 UEVaultManager/models/gql.py
 UEVaultManager/models/json_manifest.py
 UEVaultManager/models/manifest.py
 UEVaultManager/tkgui/__init__.py
 UEVaultManager/tkgui/main.py
+UEVaultManager/tkgui/modules/EditCellWindowClass.py
+UEVaultManager/tkgui/modules/EditRowWindowClass.py
+UEVaultManager/tkgui/modules/EditableTableClass.py
+UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+UEVaultManager/tkgui/modules/GUISettingsClass.py
+UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+UEVaultManager/tkgui/modules/SaferDictClass.py
+UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+UEVaultManager/tkgui/modules/UEVMGuiClass.py
+UEVaultManager/tkgui/modules/WebImageClass.py
+UEVaultManager/tkgui/modules/__init__.py
+UEVaultManager/tkgui/modules/functions.py
+UEVaultManager/tkgui/modules/globals.py
 UEVaultManager/utils/__init__.py
 UEVaultManager/utils/aliasing.py
 UEVaultManager/utils/cli.py
 UEVaultManager/utils/custom_parser.py
 UEVaultManager/utils/egl_crypt.py
 UEVaultManager/utils/env.py
 UEVaultManager/utils/rolling_hash.py
```

### Comparing `UEVaultManager-1.1.1.2/setup.py` & `UEVaultManager-1.1.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # !/usr/bin/env python
 # coding: utf-8
 
 import sys
 from pathlib import Path
 
+import setuptools
 from setuptools import setup
 
 from UEVaultManager import __name__, __version__, __license__, __author__, __author_email__, __copyright__, __description__, __url__
 
 if sys.version_info < (3, 9):
     sys.exit('python 3.9 or higher is required for UEVaultManager')
 
@@ -22,26 +23,28 @@
     author=__author__,
     author_email=__author_email__,
     copyright=__copyright__,
     description=__description__,
     long_description=__long_description__,
     long_description_content_type='text/markdown',
     url=__url__,
-    packages=[
-        'UEVaultManager',  #
-        'UEVaultManager.api',  #
-        'UEVaultManager.assets',  #
-        'UEVaultManager.downloader',  #
-        'UEVaultManager.downloader.mp',  #
-        'UEVaultManager.lfs',  #
-        'UEVaultManager.models',  #
-        'UEVaultManager.tkgui',  #
-        'UEVaultManager.utils',  #
-    ],
-    data_files=[('', ['UEVaultManager/assets/UEVM_200x200.png','UEVaultManager/assets/main.ico'])],
+    packages=setuptools.find_packages(),
+    # packages=[
+    #     'UEVaultManager',  #
+    #     'UEVaultManager.api',  #
+    #     'UEVaultManager.assets',  #
+    #     'UEVaultManager.downloader',  #
+    #     'UEVaultManager.downloader.mp',  #
+    #     'UEVaultManager.lfs',  #
+    #     'UEVaultManager.models',  #
+    #     'UEVaultManager.tkgui',  #
+    #     'UEVaultManager.utils',  #
+    # ],
+    # data_files=[('', ['UEVaultManager/assets/UEVM_200x200.png','UEVaultManager/assets/main.ico'])],
+    package_data={'': ['assets/*']},
     entry_points=dict(console_scripts=['UEVaultManager = UEVaultManager.cli:main']),
     install_requires=[
         'requests<3.0',  #
         'setuptools',  #
         'wheel'
     ],
     extras_require=dict(webview=['pywebview>=3.4'], webview_gtk=[
```

