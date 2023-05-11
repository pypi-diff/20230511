# Comparing `tmp/UEVaultManager-1.0.4.tar.gz` & `tmp/UEVaultManager-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.0.4.tar", last modified: Thu Mar 30 07:03:20 2023, max compression
+gzip compressed data, was "UEVaultManager-1.0.5.tar", last modified: Thu Mar 30 07:06:09 2023, max compression
```

## Comparing `UEVaultManager-1.0.4.tar` & `UEVaultManager-1.0.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 07:03:20.348359 UEVaultManager-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     5683 2023-03-30 07:03:20.347859 UEVaultManager-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4911 2023-03-29 17:33:20.000000 UEVaultManager-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 07:03:20.324794 UEVaultManager-1.0.4/UEVaultManager/
--rw-rw-rw-   0        0        0      498 2023-03-30 07:02:38.000000 UEVaultManager-1.0.4/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:03:20.330799 UEVaultManager-1.0.4/UEVaultManager/api/
--rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.4/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    20251 2023-02-22 20:15:44.000000 UEVaultManager-1.0.4/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0      884 2023-02-09 18:32:33.000000 UEVaultManager-1.0.4/UEVaultManager/api/lgd.py
--rw-rw-rw-   0        0        0    52857 2023-02-23 18:25:27.000000 UEVaultManager-1.0.4/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    39556 2023-02-23 15:17:05.000000 UEVaultManager-1.0.4/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:03:20.331300 UEVaultManager-1.0.4/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.4/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:03:20.332800 UEVaultManager-1.0.4/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.4/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38025 2023-02-20 12:25:16.000000 UEVaultManager-1.0.4/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-02-21 07:29:33.000000 UEVaultManager-1.0.4/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:03:20.336339 UEVaultManager-1.0.4/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.4/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-02-09 18:32:33.000000 UEVaultManager-1.0.4/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6686 2023-02-09 18:32:33.000000 UEVaultManager-1.0.4/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    21692 2023-02-22 20:03:37.000000 UEVaultManager-1.0.4/UEVaultManager/lfs/lgndry.py
--rw-rw-rw-   0        0        0     5528 2023-02-20 12:25:16.000000 UEVaultManager-1.0.4/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3040 2023-02-20 12:31:14.000000 UEVaultManager-1.0.4/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:03:20.341849 UEVaultManager-1.0.4/UEVaultManager/models/
--rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.4/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-02-20 10:54:01.000000 UEVaultManager-1.0.4/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-02-09 18:32:33.000000 UEVaultManager-1.0.4/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     1351 2023-02-21 07:23:44.000000 UEVaultManager-1.0.4/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     3627 2023-02-09 18:32:33.000000 UEVaultManager-1.0.4/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5074 2023-02-09 15:53:35.000000 UEVaultManager-1.0.4/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0       72 2023-01-05 18:12:15.000000 UEVaultManager-1.0.4/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     1334 2023-02-09 15:53:35.000000 UEVaultManager-1.0.4/UEVaultManager/models/gql.py
--rw-rw-rw-   0        0        0     5891 2023-02-09 18:32:33.000000 UEVaultManager-1.0.4/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30499 2023-02-16 16:54:16.000000 UEVaultManager-1.0.4/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:03:20.347358 UEVaultManager-1.0.4/UEVaultManager/utils/
--rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.4/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3455 2023-02-16 17:11:16.000000 UEVaultManager-1.0.4/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     2243 2023-02-20 18:25:41.000000 UEVaultManager-1.0.4/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1075 2023-02-21 07:29:33.000000 UEVaultManager-1.0.4/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10270 2023-02-21 07:23:45.000000 UEVaultManager-1.0.4/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      309 2023-01-05 18:12:15.000000 UEVaultManager-1.0.4/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      562 2023-02-09 17:53:24.000000 UEVaultManager-1.0.4/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     5891 2023-02-20 12:31:14.000000 UEVaultManager-1.0.4/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-03-30 07:03:20.329303 UEVaultManager-1.0.4/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     5683 2023-03-30 07:03:20.000000 UEVaultManager-1.0.4/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2023-03-30 07:03:20.000000 UEVaultManager-1.0.4/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 07:03:20.000000 UEVaultManager-1.0.4/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-03-30 07:03:20.000000 UEVaultManager-1.0.4/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-03-30 07:03:20.000000 UEVaultManager-1.0.4/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-30 07:03:20.000000 UEVaultManager-1.0.4/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 07:03:20.348359 UEVaultManager-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1849 2023-03-30 07:02:19.000000 UEVaultManager-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.591313 UEVaultManager-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5635 2023-03-30 07:06:09.590814 UEVaultManager-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4865 2023-03-30 07:04:58.000000 UEVaultManager-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.568641 UEVaultManager-1.0.5/UEVaultManager/
+-rw-rw-rw-   0        0        0      498 2023-03-30 07:05:18.000000 UEVaultManager-1.0.5/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.573747 UEVaultManager-1.0.5/UEVaultManager/api/
+-rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    20251 2023-02-22 20:15:44.000000 UEVaultManager-1.0.5/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0      884 2023-02-09 18:32:33.000000 UEVaultManager-1.0.5/UEVaultManager/api/lgd.py
+-rw-rw-rw-   0        0        0    52857 2023-02-23 18:25:27.000000 UEVaultManager-1.0.5/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    39556 2023-02-23 15:17:05.000000 UEVaultManager-1.0.5/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.574246 UEVaultManager-1.0.5/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.575747 UEVaultManager-1.0.5/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38025 2023-02-20 12:25:16.000000 UEVaultManager-1.0.5/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-02-21 07:29:33.000000 UEVaultManager-1.0.5/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.579313 UEVaultManager-1.0.5/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-02-09 18:32:33.000000 UEVaultManager-1.0.5/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6686 2023-02-09 18:32:33.000000 UEVaultManager-1.0.5/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    21692 2023-02-22 20:03:37.000000 UEVaultManager-1.0.5/UEVaultManager/lfs/lgndry.py
+-rw-rw-rw-   0        0        0     5528 2023-02-20 12:25:16.000000 UEVaultManager-1.0.5/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3040 2023-02-20 12:31:14.000000 UEVaultManager-1.0.5/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.585314 UEVaultManager-1.0.5/UEVaultManager/models/
+-rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-02-20 10:54:01.000000 UEVaultManager-1.0.5/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4478 2023-02-09 18:32:33.000000 UEVaultManager-1.0.5/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     1351 2023-02-21 07:23:44.000000 UEVaultManager-1.0.5/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     3627 2023-02-09 18:32:33.000000 UEVaultManager-1.0.5/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5074 2023-02-09 15:53:35.000000 UEVaultManager-1.0.5/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0       72 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     1334 2023-02-09 15:53:35.000000 UEVaultManager-1.0.5/UEVaultManager/models/gql.py
+-rw-rw-rw-   0        0        0     5891 2023-02-09 18:32:33.000000 UEVaultManager-1.0.5/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30499 2023-02-16 16:54:16.000000 UEVaultManager-1.0.5/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.590314 UEVaultManager-1.0.5/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0        0 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3455 2023-02-16 17:11:16.000000 UEVaultManager-1.0.5/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     2243 2023-02-20 18:25:41.000000 UEVaultManager-1.0.5/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1075 2023-02-21 07:29:33.000000 UEVaultManager-1.0.5/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10270 2023-02-21 07:23:45.000000 UEVaultManager-1.0.5/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      309 2023-01-05 18:12:15.000000 UEVaultManager-1.0.5/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      562 2023-02-09 17:53:24.000000 UEVaultManager-1.0.5/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     5891 2023-02-20 12:31:14.000000 UEVaultManager-1.0.5/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-03-30 07:06:09.572236 UEVaultManager-1.0.5/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     5635 2023-03-30 07:06:09.000000 UEVaultManager-1.0.5/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1347 2023-03-30 07:06:09.000000 UEVaultManager-1.0.5/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-30 07:06:09.000000 UEVaultManager-1.0.5/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-03-30 07:06:09.000000 UEVaultManager-1.0.5/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-03-30 07:06:09.000000 UEVaultManager-1.0.5/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-03-30 07:06:09.000000 UEVaultManager-1.0.5/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-30 07:06:09.591313 UEVaultManager-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1849 2023-03-30 07:02:19.000000 UEVaultManager-1.0.5/setup.py
```

### Comparing `UEVaultManager-1.0.4/LICENSE` & `UEVaultManager-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/PKG-INFO` & `UEVaultManager-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.0.4
+Version: 1.0.5
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -61,11 +61,7 @@
   * [Log files and debug](https://uevaultmanager.readthedocs.io/en/latest/output.html#log-files-and-debug)
   * [The output file](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-output-file)
   * [The individual json files](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-individual-json-files)
   * [how to fix invalid search result during the grabbing process](https://uevaultmanager.readthedocs.io/en/latest/output.html#how-to-fix-invalid-search-result-during-the-grabbing-process)
   * [possible values in the error Field](https://uevaultmanager.readthedocs.io/en/latest/output.html#possible-values-in-the-error-field)
 
 [Next](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
-
-* * *
-
-Â© Copyright 2023 Laurent Ongaro.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `UEVaultManager-1.0.4/README.md` & `UEVaultManager-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,11 +41,7 @@
   * [Log files and debug](https://uevaultmanager.readthedocs.io/en/latest/output.html#log-files-and-debug)
   * [The output file](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-output-file)
   * [The individual json files](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-individual-json-files)
   * [how to fix invalid search result during the grabbing process](https://uevaultmanager.readthedocs.io/en/latest/output.html#how-to-fix-invalid-search-result-during-the-grabbing-process)
   * [possible values in the error Field](https://uevaultmanager.readthedocs.io/en/latest/output.html#possible-values-in-the-error-field)
 
 [Next](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
-
-* * *
-
-© Copyright 2023 Laurent Ongaro.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `UEVaultManager-1.0.4/UEVaultManager/api/egs.py` & `UEVaultManager-1.0.5/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/api/lgd.py` & `UEVaultManager-1.0.5/UEVaultManager/api/lgd.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/cli.py` & `UEVaultManager-1.0.5/UEVaultManager/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/core.py` & `UEVaultManager-1.0.5/UEVaultManager/core.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.0.5/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.0.5/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.0.5/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.0.5/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/lfs/lgndry.py` & `UEVaultManager-1.0.5/UEVaultManager/lfs/lgndry.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.0.5/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.0.5/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/models/app.py` & `UEVaultManager-1.0.5/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/models/chunk.py` & `UEVaultManager-1.0.5/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/models/config.py` & `UEVaultManager-1.0.5/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/models/downloading.py` & `UEVaultManager-1.0.5/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/models/egl.py` & `UEVaultManager-1.0.5/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/models/gql.py` & `UEVaultManager-1.0.5/UEVaultManager/models/gql.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.0.5/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/models/manifest.py` & `UEVaultManager-1.0.5/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.0.5/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/utils/cli.py` & `UEVaultManager-1.0.5/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.0.5/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.0.5/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.0.5/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.0.5/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.0.5/UEVaultManager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.0.4
+Version: 1.0.5
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -61,11 +61,7 @@
   * [Log files and debug](https://uevaultmanager.readthedocs.io/en/latest/output.html#log-files-and-debug)
   * [The output file](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-output-file)
   * [The individual json files](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-individual-json-files)
   * [how to fix invalid search result during the grabbing process](https://uevaultmanager.readthedocs.io/en/latest/output.html#how-to-fix-invalid-search-result-during-the-grabbing-process)
   * [possible values in the error Field](https://uevaultmanager.readthedocs.io/en/latest/output.html#possible-values-in-the-error-field)
 
 [Next](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
-
-* * *
-
-Â© Copyright 2023 Laurent Ongaro.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `UEVaultManager-1.0.4/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.0.5/UEVaultManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.0.4/setup.py` & `UEVaultManager-1.0.5/setup.py`

 * *Files identical despite different names*

