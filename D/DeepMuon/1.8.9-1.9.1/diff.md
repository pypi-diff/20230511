# Comparing `tmp/DeepMuon-1.8.9.tar.gz` & `tmp/DeepMuon-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepMuon-1.8.9.tar", last modified: Sun Nov 20 13:41:42 2022, max compression
+gzip compressed data, was "DeepMuon-1.9.1.tar", last modified: Sat Dec  3 15:50:13 2022, max compression
```

## Comparing `DeepMuon-1.8.9.tar` & `DeepMuon-1.9.1.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.916375 DeepMuon-1.8.9/
--rw-rw-rw-   0        0        0       67 2022-09-21 15:38:32.000000 DeepMuon-1.8.9/.gitignore
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.826260 DeepMuon-1.8.9/DeepMuon/
--rw-rw-rw-   0        0        0      501 2022-10-07 14:38:30.000000 DeepMuon-1.8.9/DeepMuon/__init__.py
--rw-rw-rw-   0        0        0      228 2022-11-20 13:08:41.000000 DeepMuon-1.8.9/DeepMuon/__version__.py
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.796131 DeepMuon-1.8.9/DeepMuon/config/
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.842797 DeepMuon-1.8.9/DeepMuon/config/Hailing/
--rw-rw-rw-   0        0        0     1804 2022-11-19 13:27:44.000000 DeepMuon-1.8.9/DeepMuon/config/Hailing/CSPP.py
--rw-rw-rw-   0        0        0     1972 2022-11-19 16:15:35.000000 DeepMuon-1.8.9/DeepMuon/config/Hailing/CSPPV2.py
--rw-rw-rw-   0        0        0     1964 2022-11-20 13:24:38.000000 DeepMuon-1.8.9/DeepMuon/config/Hailing/RESMAX.py
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.844809 DeepMuon-1.8.9/DeepMuon/config/Pandax4T/
--rw-rw-rw-   0        0        0     1608 2022-11-19 13:27:47.000000 DeepMuon-1.8.9/DeepMuon/config/Pandax4T/MLP3.py
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.850806 DeepMuon-1.8.9/DeepMuon/dataset/
--rw-rw-rw-   0        0        0     9676 2022-11-20 13:22:55.000000 DeepMuon-1.8.9/DeepMuon/dataset/HailingData.py
--rw-rw-rw-   0        0        0     3221 2022-11-19 13:27:37.000000 DeepMuon-1.8.9/DeepMuon/dataset/Pandax4TData.py
--rw-rw-rw-   0        0        0      403 2022-11-20 12:30:08.000000 DeepMuon-1.8.9/DeepMuon/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.862496 DeepMuon-1.8.9/DeepMuon/models/
--rw-rw-rw-   0        0        0     1058 2022-11-19 13:27:29.000000 DeepMuon-1.8.9/DeepMuon/models/Airloss.py
--rw-rw-rw-   0        0        0    10243 2022-11-19 13:37:33.000000 DeepMuon-1.8.9/DeepMuon/models/CSPP.py
--rw-rw-rw-   0        0        0     2279 2022-11-19 13:27:27.000000 DeepMuon-1.8.9/DeepMuon/models/Pandax4T.py
--rw-rw-rw-   0        0        0     1861 2022-11-19 13:27:32.000000 DeepMuon-1.8.9/DeepMuon/models/SPP.py
--rw-rw-rw-   0        0        0     5306 2022-11-19 13:27:27.000000 DeepMuon-1.8.9/DeepMuon/models/ViT.py
--rw-rw-rw-   0        0        0      498 2022-11-20 12:32:29.000000 DeepMuon-1.8.9/DeepMuon/models/__init__.py
--rw-rw-rw-   0        0        0     8993 2022-11-20 13:30:53.000000 DeepMuon-1.8.9/DeepMuon/randtest.py
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.879168 DeepMuon-1.8.9/DeepMuon/test/
--rw-rw-rw-   0        0        0      289 2022-11-19 17:09:22.000000 DeepMuon-1.8.9/DeepMuon/test/__init__.py
--rw-rw-rw-   0        0        0      136 2022-11-19 13:27:51.000000 DeepMuon-1.8.9/DeepMuon/test/ana.sh
--rw-rw-rw-   0        0        0     5126 2022-11-19 13:27:50.000000 DeepMuon-1.8.9/DeepMuon/test/analysis.py
--rw-rw-rw-   0        0        0      112 2022-11-19 13:27:53.000000 DeepMuon-1.8.9/DeepMuon/test/com.sh
--rw-rw-rw-   0        0        0     2858 2022-11-19 13:27:52.000000 DeepMuon-1.8.9/DeepMuon/test/compare.py
--rw-rw-rw-   0        0        0    13196 2022-11-20 13:40:13.000000 DeepMuon-1.8.9/DeepMuon/test/inference.py
--rw-rw-rw-   0        0        0      128 2022-11-20 10:19:19.000000 DeepMuon-1.8.9/DeepMuon/test/inference.sh
--rw-rw-rw-   0        0        0     1211 2022-11-19 13:27:51.000000 DeepMuon-1.8.9/DeepMuon/test/model_info.py
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.887193 DeepMuon-1.8.9/DeepMuon/tools/
--rw-rw-rw-   0        0        0     6956 2022-11-19 16:01:26.000000 DeepMuon-1.8.9/DeepMuon/tools/AirConfig.py
--rw-rw-rw-   0        0        0     7598 2022-11-19 16:33:40.000000 DeepMuon-1.8.9/DeepMuon/tools/AirFunc.py
--rw-rw-rw-   0        0        0     1445 2022-11-19 17:04:48.000000 DeepMuon-1.8.9/DeepMuon/tools/AirLogger.py
--rw-rw-rw-   0        0        0      265 2022-11-20 10:59:36.000000 DeepMuon-1.8.9/DeepMuon/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.898719 DeepMuon-1.8.9/DeepMuon/train/
--rw-rw-rw-   0        0        0      207 2022-11-19 13:28:04.000000 DeepMuon-1.8.9/DeepMuon/train/__init__.py
--rw-rw-rw-   0        0        0    11150 2022-11-19 16:13:46.000000 DeepMuon-1.8.9/DeepMuon/train/dist_train.py
--rw-rw-rw-   0        0        0      215 2022-11-19 13:51:12.000000 DeepMuon-1.8.9/DeepMuon/train/dist_train.sh
--rw-rw-rw-   0        0        0     1547 2022-11-19 13:28:01.000000 DeepMuon-1.8.9/DeepMuon/train/run.py
--rw-rw-rw-   0        0        0    10440 2022-11-20 01:45:59.000000 DeepMuon-1.8.9/DeepMuon/train/train.py
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.836726 DeepMuon-1.8.9/DeepMuon.egg-info/
--rw-rw-rw-   0        0        0     2509 2022-11-20 13:41:42.000000 DeepMuon-1.8.9/DeepMuon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1310 2022-11-20 13:41:42.000000 DeepMuon-1.8.9/DeepMuon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-20 13:41:42.000000 DeepMuon-1.8.9/DeepMuon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2022-11-20 13:41:42.000000 DeepMuon-1.8.9/DeepMuon.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       61 2022-11-20 13:41:42.000000 DeepMuon-1.8.9/DeepMuon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-20 13:41:42.000000 DeepMuon-1.8.9/DeepMuon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      410 2022-10-10 08:54:56.000000 DeepMuon-1.8.9/LICENSE.txt
--rw-rw-rw-   0        0        0       31 2022-10-07 16:00:14.000000 DeepMuon-1.8.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2509 2022-11-20 13:41:42.915304 DeepMuon-1.8.9/PKG-INFO
--rw-rw-rw-   0        0        0     1507 2022-10-10 11:46:16.000000 DeepMuon-1.8.9/README.md
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.900755 DeepMuon-1.8.9/Resources/
--rw-rw-rw-   0        0        0   181364 2022-10-10 09:02:14.000000 DeepMuon-1.8.9/Resources/DeepMuon.png
-drwxrwxrwx   0        0        0        0 2022-11-20 13:41:42.913305 DeepMuon-1.8.9/Tutorial/
--rw-rw-rw-   0        0        0     1007 2022-10-30 06:34:26.000000 DeepMuon-1.8.9/Tutorial/1.Regulations.md
--rw-rw-rw-   0        0        0     2967 2022-10-30 06:36:34.000000 DeepMuon-1.8.9/Tutorial/2.Customize Dataset.md
--rw-rw-rw-   0        0        0     4229 2022-10-30 06:39:04.000000 DeepMuon-1.8.9/Tutorial/3.Customize Model.md
--rw-rw-rw-   0        0        0     6127 2022-10-30 06:48:27.000000 DeepMuon-1.8.9/Tutorial/4.Configuration.md
--rw-rw-rw-   0        0        0     1941 2022-10-10 08:38:56.000000 DeepMuon-1.8.9/Tutorial/5.Training and Inference.md
--rw-rw-rw-   0        0        0       42 2022-11-20 13:41:42.916375 DeepMuon-1.8.9/setup.cfg
--rw-rw-rw-   0        0        0     5807 2022-11-20 01:34:47.000000 DeepMuon-1.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.504363 DeepMuon-1.9.1/
+-rw-rw-rw-   0        0        0      100 2022-11-25 10:57:26.000000 DeepMuon-1.9.1/.gitignore
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.413718 DeepMuon-1.9.1/DeepMuon/
+-rw-rw-rw-   0        0        0      501 2022-10-07 14:38:30.000000 DeepMuon-1.9.1/DeepMuon/__init__.py
+-rw-rw-rw-   0        0        0      228 2022-12-03 15:48:31.000000 DeepMuon-1.9.1/DeepMuon/__version__.py
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.392131 DeepMuon-1.9.1/DeepMuon/config/
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.431447 DeepMuon-1.9.1/DeepMuon/config/Hailing/
+-rw-rw-rw-   0        0        0     1804 2022-11-19 13:27:44.000000 DeepMuon-1.9.1/DeepMuon/config/Hailing/CSPP.py
+-rw-rw-rw-   0        0        0     1972 2022-11-19 16:15:35.000000 DeepMuon-1.9.1/DeepMuon/config/Hailing/CSPPV2.py
+-rw-rw-rw-   0        0        0     1964 2022-11-20 13:24:38.000000 DeepMuon-1.9.1/DeepMuon/config/Hailing/RESMAX.py
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.433446 DeepMuon-1.9.1/DeepMuon/config/Pandax4T/
+-rw-rw-rw-   0        0        0     1608 2022-11-19 13:27:47.000000 DeepMuon-1.9.1/DeepMuon/config/Pandax4T/MLP3.py
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.439448 DeepMuon-1.9.1/DeepMuon/dataset/
+-rw-rw-rw-   0        0        0    10941 2022-12-03 15:40:04.000000 DeepMuon-1.9.1/DeepMuon/dataset/HailingData.py
+-rw-rw-rw-   0        0        0     3221 2022-11-19 13:27:37.000000 DeepMuon-1.9.1/DeepMuon/dataset/Pandax4TData.py
+-rw-rw-rw-   0        0        0      403 2022-11-20 12:30:08.000000 DeepMuon-1.9.1/DeepMuon/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.451220 DeepMuon-1.9.1/DeepMuon/models/
+-rw-rw-rw-   0        0        0     1058 2022-11-19 13:27:29.000000 DeepMuon-1.9.1/DeepMuon/models/Airloss.py
+-rw-rw-rw-   0        0        0    11361 2022-12-03 15:41:01.000000 DeepMuon-1.9.1/DeepMuon/models/CSPP.py
+-rw-rw-rw-   0        0        0     2279 2022-11-19 13:27:27.000000 DeepMuon-1.9.1/DeepMuon/models/Pandax4T.py
+-rw-rw-rw-   0        0        0     1861 2022-11-19 13:27:32.000000 DeepMuon-1.9.1/DeepMuon/models/SPP.py
+-rw-rw-rw-   0        0        0     5306 2022-11-19 13:27:27.000000 DeepMuon-1.9.1/DeepMuon/models/ViT.py
+-rw-rw-rw-   0        0        0      508 2022-12-03 15:36:43.000000 DeepMuon-1.9.1/DeepMuon/models/__init__.py
+-rw-rw-rw-   0        0        0     8940 2022-12-03 15:11:02.000000 DeepMuon-1.9.1/DeepMuon/randtest.py
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.463863 DeepMuon-1.9.1/DeepMuon/test/
+-rw-rw-rw-   0        0        0      262 2022-12-03 15:33:07.000000 DeepMuon-1.9.1/DeepMuon/test/__init__.py
+-rw-rw-rw-   0        0        0      136 2022-11-19 13:27:51.000000 DeepMuon-1.9.1/DeepMuon/test/ana.sh
+-rw-rw-rw-   0        0        0     5739 2022-11-26 04:27:31.000000 DeepMuon-1.9.1/DeepMuon/test/analysis.py
+-rw-rw-rw-   0        0        0      112 2022-11-19 13:27:53.000000 DeepMuon-1.9.1/DeepMuon/test/com.sh
+-rw-rw-rw-   0        0        0     3574 2022-11-26 04:20:22.000000 DeepMuon-1.9.1/DeepMuon/test/compare.py
+-rw-rw-rw-   0        0        0    13239 2022-12-03 15:33:37.000000 DeepMuon-1.9.1/DeepMuon/test/inference.py
+-rw-rw-rw-   0        0        0      128 2022-11-20 10:19:19.000000 DeepMuon-1.9.1/DeepMuon/test/inference.sh
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.476932 DeepMuon-1.9.1/DeepMuon/tools/
+-rw-rw-rw-   0        0        0     6956 2022-11-19 16:01:26.000000 DeepMuon-1.9.1/DeepMuon/tools/AirConfig.py
+-rw-rw-rw-   0        0        0     9362 2022-12-03 15:35:55.000000 DeepMuon-1.9.1/DeepMuon/tools/AirFunc.py
+-rw-rw-rw-   0        0        0     1445 2022-11-19 17:04:48.000000 DeepMuon-1.9.1/DeepMuon/tools/AirLogger.py
+-rw-rw-rw-   0        0        0      317 2022-12-03 15:33:21.000000 DeepMuon-1.9.1/DeepMuon/tools/__init__.py
+-rw-rw-rw-   0        0        0     2676 2022-12-03 15:33:57.000000 DeepMuon-1.9.1/DeepMuon/tools/mem_info.py
+-rw-rw-rw-   0        0        0     1689 2022-12-03 15:34:24.000000 DeepMuon-1.9.1/DeepMuon/tools/model_info.py
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.487298 DeepMuon-1.9.1/DeepMuon/train/
+-rw-rw-rw-   0        0        0      207 2022-11-19 13:28:04.000000 DeepMuon-1.9.1/DeepMuon/train/__init__.py
+-rw-rw-rw-   0        0        0    11150 2022-11-26 13:02:38.000000 DeepMuon-1.9.1/DeepMuon/train/dist_train.py
+-rw-rw-rw-   0        0        0      215 2022-11-19 13:51:12.000000 DeepMuon-1.9.1/DeepMuon/train/dist_train.sh
+-rw-rw-rw-   0        0        0     1547 2022-11-26 04:30:01.000000 DeepMuon-1.9.1/DeepMuon/train/run.py
+-rw-rw-rw-   0        0        0    10440 2022-11-20 01:45:59.000000 DeepMuon-1.9.1/DeepMuon/train/train.py
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.426070 DeepMuon-1.9.1/DeepMuon.egg-info/
+-rw-rw-rw-   0        0        0     2509 2022-12-03 15:50:13.000000 DeepMuon-1.9.1/DeepMuon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2022-12-03 15:50:13.000000 DeepMuon-1.9.1/DeepMuon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-03 15:50:13.000000 DeepMuon-1.9.1/DeepMuon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2022-12-03 15:50:13.000000 DeepMuon-1.9.1/DeepMuon.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       82 2022-12-03 15:50:13.000000 DeepMuon-1.9.1/DeepMuon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-12-03 15:50:13.000000 DeepMuon-1.9.1/DeepMuon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      415 2022-11-25 09:59:20.000000 DeepMuon-1.9.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       31 2022-10-07 16:00:14.000000 DeepMuon-1.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2509 2022-12-03 15:50:13.504363 DeepMuon-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1507 2022-10-10 11:46:16.000000 DeepMuon-1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.490319 DeepMuon-1.9.1/Resources/
+-rw-rw-rw-   0        0        0   181364 2022-10-10 09:02:14.000000 DeepMuon-1.9.1/Resources/DeepMuon.png
+drwxrwxrwx   0        0        0        0 2022-12-03 15:50:13.501865 DeepMuon-1.9.1/Tutorial/
+-rw-rw-rw-   0        0        0     1007 2022-10-30 06:34:26.000000 DeepMuon-1.9.1/Tutorial/1.Regulations.md
+-rw-rw-rw-   0        0        0     2967 2022-10-30 06:36:34.000000 DeepMuon-1.9.1/Tutorial/2.Customize Dataset.md
+-rw-rw-rw-   0        0        0     4229 2022-10-30 06:39:04.000000 DeepMuon-1.9.1/Tutorial/3.Customize Model.md
+-rw-rw-rw-   0        0        0     6127 2022-10-30 06:48:27.000000 DeepMuon-1.9.1/Tutorial/4.Configuration.md
+-rw-rw-rw-   0        0        0     1941 2022-10-10 08:38:56.000000 DeepMuon-1.9.1/Tutorial/5.Training and Inference.md
+-rw-rw-rw-   0        0        0       42 2022-12-03 15:50:13.504363 DeepMuon-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     5906 2022-12-03 15:47:20.000000 DeepMuon-1.9.1/setup.py
```

### Comparing `DeepMuon-1.8.9/DeepMuon/config/Hailing/CSPP.py` & `DeepMuon-1.9.1/DeepMuon/config/Hailing/CSPP.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon/config/Hailing/CSPPV2.py` & `DeepMuon-1.9.1/DeepMuon/config/Hailing/CSPPV2.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon/config/Hailing/RESMAX.py` & `DeepMuon-1.9.1/DeepMuon/config/Hailing/RESMAX.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon/config/Pandax4T/MLP3.py` & `DeepMuon-1.9.1/DeepMuon/config/Pandax4T/MLP3.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon/dataset/HailingData.py` & `DeepMuon-1.9.1/DeepMuon/dataset/HailingData.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: airscker
 Date: 2022-09-17 18:11:14
 LastEditors: airscker
-LastEditTime: 2022-11-20 21:22:20
+LastEditTime: 2022-12-03 23:40:04
 Description: NULL
 
 Copyright (c) 2022 by airscker, All Rights Reserved. 
 '''
 
 import numpy as np
 from tqdm import tqdm
@@ -63,16 +63,14 @@
     @returns the flipped image and label
     """
     image=np.array(image)
     image=image[:,:,::-1,:]
     label=np.array([label[0],label[1],-label[2]])
     return image,label
 
-
-
 class HailingDataset_Direct(Dataset):
     def __init__(self,datapath='./Hailing-Muon/data/1TeV/Hailing_1TeV_train_data.pkl',min_z=9):
         '''
         ## Dataset Built for Loading the Preprocessed Hailing 1TeV/10TeV Data
         - Args: 
             - datapath: The datapth of the preprocessed Hailing data, default to be './Hailing-Muon/data/1TeV/Hailing_1TeV_train_data.pkl'
         - Output:
@@ -115,15 +113,15 @@
         self.datapath=datapath
         self.origin_data=None
         self.pattern_imgs=[]
         self.pos_direction=[]
         self.__Init()
         self.__sort()
     def __len__(self):
-        return len(self.origin_data)
+        return len(self.origin_data)*8
     def __getitem__(self, index):
         # image=np.array(self.origin_data[index][0])
         # array=np.nonzero(np.count_nonzero(image,axis=(0,1,3)))
         # image=image[:,:,array[0][0]:(array[0][-1]+1),:]
         # image=np.append(image,np.zeros((10,10,max(9-image.shape[2],0),3)),axis=2)
         image=torch.from_numpy(self.sortedata[index][0])
         image=torch.permute(image,(3,0,1,2))
@@ -176,28 +174,59 @@
     def __len__(self):
         return len(self.origin_data)
     def __getitem__(self, index):
         image=np.array(self.origin_data[index][0])
         label=self.origin_data[index][1][3:]
         '''Data augmentation'''
         if self.augment:
-            oper=np.random.randint(-1,3)
-            if oper>=0:
-                image,label=self.augmentation[oper](image,label)
-        
+            oper=np.unique(np.random.randint(0,1,np.random.randint(0,2)))#[-1,0]range,[0,1]random length
+            for oper_i in range(len(oper)):
+                image,label=self.augmentation[oper[oper_i]](image,label)
         image=torch.from_numpy(image.copy())
         image=torch.permute(image,(3,0,1,2))
         image[1:,:,:,:]=0.0001*image[1:,:,:,:]
         label=torch.from_numpy(label)
         return image,label
     def __Init(self):
+        print(f'Loading dataset {self.datapath}')
+        with open(self.datapath,'rb')as f:
+            self.origin_data=pkl.load(f)
+        f.close()
+        print(f'Dataset {self.datapath} loaded')
+
+class HailingDataset_Plane_Z(Dataset):
+    def __init__(self,datapath='./Hailing-Muon/data/1TeV/Hailing_1TeV_train_data.pkl',min_z=9):
+        self.datapath=datapath
+        self.origin_data=None
+        self.pattern_imgs=[]
+        self.pos_direction=[]
+        self.min_z=min_z
+        self.__Init()
+    def __len__(self):
+        return len(self.origin_data)
+    def __getitem__(self, index):
+        image=np.array(self.origin_data[index][0])
+        image=torch.from_numpy(image)
+        image=torch.permute(image,(3,0,1,2))
+        image[1:,:,:,:]=0.0001*image[1:,:,:,:]
+        label=self.origin_data[index][1]
+        label1=[]
+        for i in range(40):
+            t=np.float((i-label[2])/label[5])
+            label1.append([np.array((label[3]*t+label[0]),(label[4]*t+label[1]),i)])
+        label1.append(np.array(self.origin_data[index][1][3:]))
+        label1=torch.from_numpy(label1)
+        return image,label1
+    def __Init(self):
         with open(self.datapath,'rb')as f:
             self.origin_data=pkl.load(f)
         f.close()
 
+
+
 class HailingData_Init:
     def __init__(self,datapath='./Hailing-Muon/data/1TeV/validate_norm.pkl',output='Hailing_1TeV_val_data.pkl',shape=(10,10,40,3)):
         """## Convert the Original Hailing Data into a list of Pattern Images(dtype: nparray -> torch.tensor) as well as Position-Direction(dtype: nparray -> torch.tensor)
         - Args:
             - datapath: The data path of the original Hailing data. Defaults to './Hailing-Muon/data/1TeV/validate_norm.pkl'.
             - output: The output path of the converted Hailing pattern image data: [description]. Defaults to 'Hailing_1TeV_val_data.pkl'.
             - shape: The shape of the Hailing pattern image data. Defaults to (10,10,40,3) for 1TeV data and (10,10,50,3) for 10TeV data available.
```

### Comparing `DeepMuon-1.8.9/DeepMuon/dataset/Pandax4TData.py` & `DeepMuon-1.9.1/DeepMuon/dataset/Pandax4TData.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon/models/Airloss.py` & `DeepMuon-1.9.1/DeepMuon/models/Airloss.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon/models/CSPP.py` & `DeepMuon-1.9.1/DeepMuon/models/CSPP.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,56 @@
 '''
 Author: airscker
 Date: 2022-10-13 07:51:47
 LastEditors: airscker
-LastEditTime: 2022-11-19 21:37:32
+LastEditTime: 2022-12-03 23:41:01
 Description: NULL
 
 Copyright (c) 2022 by airscker, All Rights Reserved. 
 '''
 import torch
 import torch.nn as nn
-from torch.nn import init
-import functools
-from torch.autograd import Variable
-import numpy as np
 import torch.nn.functional as F
-import math
 from monai.networks.blocks.convolutions import ResidualUnit
+torch.set_default_tensor_type(torch.DoubleTensor)
+
+class Plane(nn.Module):
+    def __init__(self):
+        super().__init__()
+        self.flatten = nn.Flatten()
+        self.linear_relu_stack = nn.Sequential(
+            nn.Linear(10*10, 52),
+            nn.BatchNorm1d(52),
+            nn.LeakyReLU(),
+            nn.Linear(52, 2)
+        )
+        self.linear_relu_stack2= nn.Sequential(
+            nn.Linear(3*40, 52),
+            nn.BatchNorm1d(52),
+            nn.LeakyReLU(),
+            nn.Linear(52, 3),
+            HailingDirectNorm()
+        )
+    def forward(self, x):
+        for i in range(40):
+            x_plane=x[:,:,:,:,i].to()
+            if torch.equal(x_plane,torch.zeros(x_plane.shape)):
+                x_plane=torch.zero(3)
+            else:
+                x_plane=self.flatten(x_plane) 
+                x_plane=self.linear_relu_stack(x_plane)
+                x_plane=torch.cat((x_plane,i),0)
+            if i==0:
+                logits=x_plane
+            else:
+                logits=torch.cat((logits,x_plane),dim=0)
+        track=self.flatten(logits)
+        track=self.linear_relu_stack2(logits)
+        logits=torch.cat((logits,track),dim=0)
+        return logits
 
 
 class UCSPP(nn.Module):
     def __init__(self):
         super().__init__()
         self.encode1=nn.Sequential(
             nn.AdaptiveMaxPool3d((10,10,20)),
```

### Comparing `DeepMuon-1.8.9/DeepMuon/models/Pandax4T.py` & `DeepMuon-1.9.1/DeepMuon/models/Pandax4T.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon/models/SPP.py` & `DeepMuon-1.9.1/DeepMuon/models/SPP.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon/models/ViT.py` & `DeepMuon-1.9.1/DeepMuon/models/ViT.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon/randtest.py` & `DeepMuon-1.9.1/DeepMuon/randtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: Airscker
 Date: 2022-08-25 22:02:01
 LastEditors: airscker
-LastEditTime: 2022-11-20 21:30:52
+LastEditTime: 2022-12-03 22:53:14
 Description: NULL
 
 Copyright (c) 2022 by Airscker, All Rights Reserved. 
 '''
 import shutil
 import time
 import os
@@ -212,23 +212,22 @@
 # model_para(SwinUNETR(img_size=[128,128,32],in_channels=3,out_channels=1,depths=(2,2,2,2),num_heads=(3,6,12,24),feature_size=24,spatial_dims=3),datasize=[1,3,128,128,32])
 # spmodel_para(spconv.SparseConv3d(3,3,3),datasize=(1,3,10,10,40))
 # a=torch.randn(10,10,10,40,3).cuda(0)
 # a=spconv.SparseConvTensor.from_dense(a)
 # conv=spconv.SubMConv3d(3,3,3)
 # print(conv(a))
 # model_para(SABlock(10,10),datasize=(1,10,10))
-# model_para(Vit_MLP(),datasize=[2,3,10,10,40])
 # model_para(unet.UNet(spatial_dims=3,in_channels=3,out_channels=1,channels=(6,12,24),strides=(1,1,1),num_res_units=3),datasize=[2,3,10,10,40],depth=5)
 # model_para(MLP3_3D_Direc(),datasize=[3,10,10,40,3])
 # model_para(MLP3(),datasize=[3,1,17,17])
 # model_optim()
 # model=MLP3()
 # print(model._get_name())
 # print(f'Total Time used: {time.time()-start}s')
 # model_para(SparseCSPP(),datasize=(2,10,10,40,3))
-# model_para(ResMax(),datasize=[2,3,10,10,40])
+model_para(STRM(),datasize=[2,3,10,10,40])
 del_pycache()
 
 # model_para(model=MLP3v2(),datasize=[3,1,17,17])
 # logger=AirLogger.LOGT()
 # logger.log(f'yes{1e4}')
 # logger.log(f'{time.ctime()}')
```

### Comparing `DeepMuon-1.8.9/DeepMuon/test/analysis.py` & `DeepMuon-1.9.1/DeepMuon/test/analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: airscker
 Date: 2022-10-05 15:08:10
 LastEditors: airscker
-LastEditTime: 2022-11-05 21:22:39
+LastEditTime: 2022-11-26 12:27:31
 Description: NULL
 
 Copyright (c) 2022 by airscker, All Rights Reserved. 
 '''
 from email.policy import default
 import numpy as np
 import pickle as pkl
@@ -48,14 +48,25 @@
             if epoch>len(train_info):
                 train_info.append(train_data)
             else:
                 train_info[epoch-1]=train_data
     return np.array(train_info)
 
 def data_analysis(thres,sigma,config,fold=0.8):
+    """
+    The data_analysis function is used to analyze the distribution of loss value and plot the loss/lr curve.
+    The function will also log key information of loss, including mean, std, sigma range and threshold value sigma range.
+    
+    
+    :param thres: Determine the threshold value of loss
+    :param sigma: Set the threshold of loss value
+    :param config: Specify the configuration file of the training process
+    :param fold=0.8: Set the threshold of loss value
+    :return: The result of the loss value distribution and threshold distribution, as well as the loss/lr curve
+    """
     # Load configuration
     assert os.path.exists(config),f'Config file {config} can not be found'
     train_config=Config(configpath=config)
     work_dir=train_config.paras['work_config']['work_dir']
     res_path=os.path.join(work_dir,'infer','inference_res.pkl')
     assert os.path.exists(res_path),f'Result file {res_path} can not be found'
     # Load inferenced results
```

### Comparing `DeepMuon-1.8.9/DeepMuon/test/compare.py` & `DeepMuon-1.9.1/DeepMuon/test/compare.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,38 @@
 '''
 Author: airscker
 Date: 2022-10-05 21:51:59
 LastEditors: airscker
-LastEditTime: 2022-11-14 12:33:32
+LastEditTime: 2022-11-26 12:20:17
 Description: NULL
 
 Copyright (c) 2022 by airscker, All Rights Reserved. 
 '''
 import pandas as pd
 import numpy as np
 import pickle as pkl
 import matplotlib.pyplot as plt
 
 from DeepMuon.tools.AirFunc import *
 from DeepMuon.test.analysis import *
 
 def loss_com(work_dirs,output='',max=0.2,num=0):
+    """
+    The loss_com function is used to compare the loss of several models.
+    It will plot two curves, one for training and another for testing.
+    The input is a list of work_dirs which contains the log file in each directory. 
+    The output will be saved as a jpg image under root path specified by output argument.
+    
+    :param work_dirs: Specify the path of a list of models
+    :param output='': Specify the root path of output, rather then a specific file
+    :param max=0.2: Set the maximum value of the loss curve, and if it is greater than 0
+    :param num=0: Specify the number of epochs to plot
+    :return: Three variables: loss_train,loss_test,loss_max
+    
+    """
     tsl=[]
     trl=[]
     name=[]
     # max=np.arcsin(max)*180/np.pi
     assert os.path.isdir(output),f'Please specify the root path of output,rather then {output}'
     for i in range(len(work_dirs)):
         logfile=os.path.join(work_dirs[i],'log.log')
@@ -50,15 +63,15 @@
 @click.command()
 @click.option('--root',default='/home/dachuang2022/Yufeng/Hailing-Muon/work_dir/1TeV')
 @click.option('--max',default=0.2)
 @click.option('--num',default=0)
 def run(root,max,num):
     # work_dirs=os.listdir(root)
     # work_dirs=['CSPP_4','CSPP_5','DResMax_1','ResMax_4']
-    work_dirs=['CSPP_5','ResMax_5','DResMax_1','DResMax_2']
+    work_dirs=['CSPP_5','ResMax_5','DResMax_1','DResMax_3','DResMax_5']
     
     # work_dirs=['MLP3_3D','MLP3_3D2','MLP3_3D3','MLP3_3D4','UNET_MLP','UNET_MLP_2','UNET_MLP_D','CNN1','CNN2','CNN3','CNN4']
     for i in range(len(work_dirs)):
         work_dirs[i]=os.path.join(root,work_dirs[i])
         loss_com(work_dirs,root,max,num=num)
         # info=load_log(os.path.join(root,work_dirs[i],'log.log'))
         # info=np.sqrt(3*info)*180/np.pi
```

### Comparing `DeepMuon-1.8.9/DeepMuon/test/inference.py` & `DeepMuon-1.9.1/DeepMuon/test/inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: Airscker
 Date: 2022-07-19 13:01:17
 LastEditors: airscker
-LastEditTime: 2022-11-20 21:36:12
+LastEditTime: 2022-12-03 23:33:36
 Description: NULL
 
 Copyright (c) 2022 by Airscker, All Rights Reserved. 
 '''
 import time
 import os
 from tqdm import tqdm
@@ -15,15 +15,15 @@
 import numpy as np
 import pickle as pkl
 from captum.attr import IntegratedGradients
 
 from DeepMuon.tools.AirConfig import Config
 from DeepMuon.tools.AirFunc import load_model, format_time, plot_hist_2nd
 from DeepMuon.tools.AirLogger import LOGT
-from DeepMuon.test.model_info import model_para
+from DeepMuon.tools.model_info import model_para
 from DeepMuon.test.analysis import loss_dist, data_analysis
 
 import torch
 from torch import nn
 from torch.utils.data import DataLoader
 import torchvision.models as models
 from torchvision.models.feature_extraction import get_graph_node_names, create_feature_extractor
@@ -31,15 +31,15 @@
 from torchinfo import summary
 from torch.utils.tensorboard import SummaryWriter
 torch.set_default_tensor_type(torch.DoubleTensor)
 torch.backends.cudnn.benchmark = True
 torch.set_printoptions(profile='full')
 
 
-def main(configs, ana, thres,neuron):
+def main(configs, ana, thres, neuron):
     # Initialize the basic training configuration
     loss_fn = configs['loss_fn']['backbone'](configs['loss_fn']['params'])
     batch_size = 1
     test_data = configs['test_dataset']['params']
     work_dir = configs['work_config']['work_dir']
     assert os.path.exists(
         work_dir), f'The work_dir specified in the config file can not be found: {work_dir}'
@@ -94,16 +94,17 @@
     logger.log(f'{sumres}', show=False)
     logger.log(f'GFLOPs: {flops}, Number of Parameters: {params}')
     logger.log(f'Loss Function: {loss_fn}')
 
     # save model architecture
     # writer=SummaryWriter(os.path.join(work_dir,'LOG'))
     # writer.add_graph(model,torch.rand(configs['hyperpara']['inputshape']).to(device))
-    if neuron>=0:
-        neuron_infer(device=device,dataloader=test_dataloader,model=model,loss_fn=loss_fn,work_dir=work_dir,index=neuron)
+    if neuron >= 0:
+        neuron_infer(device=device, dataloader=test_dataloader,
+                     model=model, loss_fn=loss_fn, work_dir=work_dir, index=neuron)
     # start inferencing
     loss, pred, real, loss_map = infer(
         device, test_dataloader, model, loss_fn, logger, thres=thres, ana=ana)
     # Save results
     with open(res, 'wb')as f:
         pkl.dump({'loss': loss, 'pred': pred, 'real': real}, f)
     f.close()
@@ -131,15 +132,15 @@
 
 def infer(device, dataloader, model, loss_fn, logger: LOGT, thres, ana=True):
     """
     The infer function is used to test the model on a dataset. It takes in a dataloader, 
     a model, and an optional loss function. The loss function is only needed if you want to 
     see the accuracy of your predictions (for example, if you are training). This will return 
     the average loss over all of the batches as well as two lists: one with predicted values for each batch and one with real values for each batch.
-    
+
     :param device: Specify which device to use
     :param dataloader: Generate the data
     :param model: Specify the model to be used
     :param loss_fn: Calculate the loss of our model
     :param logger:LOGT: Log the training process
     :param thres: Filter out the abnormal data
     :param ana=True: Determine whether to analyze the data
@@ -168,41 +169,44 @@
                                    real_value[num-1], loss_value]
             now_time = time.time()
             logger.log(
                 f'{num}/{num_batches} Loss: {loss_value}, Predicted: {pred_value[num-1]}, Real: {real_value[num-1]}, Time: {now_time-start_time}s, ETA: {format_time((num_batches-num)*(now_time-start_time))}')
             num += 1
     return test_loss, pred_value, real_value, loss_map
 
-def Integ_Grad(model: nn.Module, device: torch.device, data:torch.Tensor,target_num:int,logger:LOGT):
+
+def Integ_Grad(model: nn.Module, device: torch.device, data: torch.Tensor, target_num: int, logger: LOGT):
     '''
     The algorithm outputs an attribution score for each input element and a convergence delta. \
         The lower the absolute value of the convergence delta the better is the approximation.
 
     Positive attribution score means that the input in that particular position positively contributed to the final prediction and negative means the opposite. \
         The magnitude of the attribution score signifies the strength of the contribution. \
             Zero attribution score means no contribution from that particular feature.
     '''
     model.to(device)
     model.eval()
     ig = IntegratedGradients(model)
     # ig=DeepLift(model)
     for i in range(target_num):
-        attr, delta = ig.attribute(data.to(device), target=i, return_convergence_delta=True)
+        attr, delta = ig.attribute(
+            data.to(device), target=i, return_convergence_delta=True)
         logger.log(f'Integrated Gradient Distribution for label_{i}')
         logger.log('IG Attributions:', attr)
         logger.log('Convergence Delta:', delta)
 
+
 def neuron_infer(device, dataloader, model: nn.Module, loss_fn, work_dir: str, index=0):
     """
     The neuron_infer function is used to infer the neuron values of a given model.
     It takes in the following parameters:
         - device: The torch device on which the computations will be run. This is typically set to cuda if you have a GPU available, otherwise it should be set to cpu. 
         - dataloader: A DataLoader object that can load your test dataset batch by batch (for example, ImageFolder from torchvision). It should return pairs of images and labels for each iteration. 
         - model: The PyTorch neural network model that we want to infer neurons for (in this case
-    
+
     :param device: Specify the device to use
     :param dataloader: Load the data
     :param model:nn.Module: Specify the model to be profiled
     :param loss_fn: Calculate the loss of the model
     :param work_dir:str: Specify the directory where the log file and neuron
     :param index=0: Specify the index of the data in the dataset
     :return: The loss value, the predicted value and the real value of a data point
@@ -257,25 +261,25 @@
 def run(config, neuron, ana, thres):
     """
     The run function is the main function that runs the training and testing of a model.
     It takes in a config file path, an analysis type (either 'train' or 'test'), 
     a threshold value for determining whether to classify as positive or negative, and 
     the neuron number you want to analyze. It then runs the training/testing process using 
     the parameters specified in that config file.
-    
+
     :param config: Pass the path to the config file
     :param neuron: Specify which data in the dataset to evaluate, if -1 specified the operation will be canceled
     :param ana: Specify which analysis to run
     :param thres: Specify the threshold for the model to be used in inference
     :return: The accuracy of the model
     """
     train_config = Config(configpath=config)
     if train_config.paras['gpu_config']['distributed'] == True:
         warnings.warn(
             'Distributed Training is not supported during model inference')
     train_config.paras['config'] = {'path': config}
-    main(train_config.paras, ana, thres,neuron)
+    main(train_config.paras, ana, thres, neuron)
 
 
 if __name__ == '__main__':
     print('\n---Starting Neural Network...---')
     run()
```

### Comparing `DeepMuon-1.8.9/DeepMuon/tools/AirConfig.py` & `DeepMuon-1.9.1/DeepMuon/tools/AirConfig.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon/tools/AirFunc.py` & `DeepMuon-1.9.1/DeepMuon/tools/AirFunc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: Airscker
 Date: 2022-09-02 14:37:59
 LastEditors: airscker
-LastEditTime: 2022-11-20 00:33:40
+LastEditTime: 2022-12-03 23:31:18
 Description: NULL
 
 Copyright (c) 2022 by Airscker, All Rights Reserved. 
 '''
 import time
 import os
 import matplotlib.pyplot as plt
@@ -82,14 +82,31 @@
     n,bins,_=plt.hist(data,rwidth=0.9,bins=bins)
     for i in range(len(n)):
         plt.text(bins[i], n[i]*1.02, round(n[i],6), fontsize=12, horizontalalignment="left")
     plt.show()
     return 0
 
 def plot_hist_2nd(data,title='x',bins=15,sigma=3,save='',show=False):
+    """
+    The plot_hist_2nd function plots a histogram of the data provided. 
+    It also includes lines to represent the mean and +/- 3 standard deviations.
+    The function takes in 4 parameters: 
+        1) data - The list of numbers that will be plotted as a histogram
+        2) title - The title for the plot
+        3) bins - The number of bins to use for the histogram (default is 15).
+        4) sigma - How many standard deviations away from mean should be highlighted (default is 3).
+    
+    :param data: Plot the histogram
+    :param title='x': Set the title of the plot
+    :param bins=15: Set the number of bins in the histogram
+    :param sigma=3: Set the sigma range of the distribution
+    :param save='': Save the plot as a 
+    :param show=False: Save the plot without showing it
+    :return: The n, bins, patchs from the plt
+    """
     plt.figure(figsize=(20,8))
     plt.title(f'Distribution of {title} Total Number: {len(data)}\
         \nMIN/MAX: {np.min(data)}/{np.max(data)} MEAN/STD: {np.mean(data)}/{np.std(data)}\
         \n{sigma}Sigma: {np.mean(data)+sigma*np.std(data)} {np.mean(data)-sigma*np.std(data)}')
     # n,bins,patchs=plt.hist(data,bins=list(np.arange(np.min(data)-0.01,np.max(data)+0.01,0.01)),rwidth=0.9)
     n,bins,patchs=plt.hist(data,bins=bins,rwidth=0.9)
     for i in range(len(n)):
@@ -104,14 +121,29 @@
     plt.fill_betweenx(y=np.array(axis[-2:])/2,x1=sigma_rangex[1],x2=np.max(data),alpha=0.2)
     plt.axis(axis)
     if save!='':
         plt.savefig(save)
     if show==True:
         plt.show()
 def plot_curve(data,title='Curve',axis_label=['Epoch','Loss'],data_label=['Curve1'],save='',show=False):
+    """
+    The plot_curve function plots a single or multiple curves on the same plot.
+    The function takes in a list of data and labels for each curve to be plotted.
+    The axis labels are optional, but if provided they will be used as x-axis label and y-axis label respectively. 
+    If no axis labels are provided, then the default values &quot;Epoch&quot; and &quot;Loss&quot; will be used instead.
+    
+    :param data: Plot the data, it can be a list of numpy array or a single numpy array
+    :param title='Curve': Set the title of the plot
+    :param axis_label=['Epoch': Set the label of the x-axis
+    :param 'Loss']: Set the title of the graph
+    :param data_label=['Curve1']: Label the curve in the plot
+    :param save='': Save the plot to a file
+    :param show=False: Save the plot as an image file
+    :return: Nothing, it just plots the curve on the current figure
+    """
     # data=np.array(data)
     plt.figure(figsize=(20,10))
     plt.title(f'{title}')
     if isinstance(data[0],list) or isinstance(data[0],np.ndarray):
         for i in range(len(data)):
             data[i]=np.array(data[i])
             label=data_label[i] if len(data_label)>=i+1 else f'Curve{i+1}'
@@ -187,9 +219,8 @@
     cache=[]
     for root,dirs,files in os.walk(path):
         # print(root,dirs,files)
         if root.endswith('__pycache__'):
             shutil.rmtree(root)
             cache.append(root)
             print(f'{root} was deleted')
-    return cache
-# print(__file__)
+    return cache
```

### Comparing `DeepMuon-1.8.9/DeepMuon/tools/AirLogger.py` & `DeepMuon-1.9.1/DeepMuon/tools/AirLogger.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon/train/dist_train.py` & `DeepMuon-1.9.1/DeepMuon/train/dist_train.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon/train/run.py` & `DeepMuon-1.9.1/DeepMuon/train/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: airscker
 Date: 2022-10-07 21:35:54
 LastEditors: airscker
-LastEditTime: 2022-11-14 17:30:02
+LastEditTime: 2022-11-26 12:29:53
 Description: NULL
 
 Copyright (c) 2022 by airscker, All Rights Reserved. 
 '''
 
 import os
 import argparse
```

### Comparing `DeepMuon-1.8.9/DeepMuon/train/train.py` & `DeepMuon-1.9.1/DeepMuon/train/train.py`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/DeepMuon.egg-info/PKG-INFO` & `DeepMuon-1.9.1/DeepMuon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepMuon
-Version: 1.8.9
+Version: 1.9.1
 Summary: DeepMuon Project Built for Simple and Direct Deep Learning Researches on Dark Matter Searching
 Home-page: UNKNOWN
 Author: Airscker/Yufeng Wang
 Author-email: wangyufeng@mail.ustc.edu.cn
 License: UNKNOWN
 Keywords: Deep Learning,Searching Dark Matter,Direct and Simple
 Platform: UNKNOWN
```

### Comparing `DeepMuon-1.8.9/DeepMuon.egg-info/SOURCES.txt` & `DeepMuon-1.9.1/DeepMuon.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,19 +28,20 @@
 DeepMuon/test/__init__.py
 DeepMuon/test/ana.sh
 DeepMuon/test/analysis.py
 DeepMuon/test/com.sh
 DeepMuon/test/compare.py
 DeepMuon/test/inference.py
 DeepMuon/test/inference.sh
-DeepMuon/test/model_info.py
 DeepMuon/tools/AirConfig.py
 DeepMuon/tools/AirFunc.py
 DeepMuon/tools/AirLogger.py
 DeepMuon/tools/__init__.py
+DeepMuon/tools/mem_info.py
+DeepMuon/tools/model_info.py
 DeepMuon/train/__init__.py
 DeepMuon/train/dist_train.py
 DeepMuon/train/dist_train.sh
 DeepMuon/train/run.py
 DeepMuon/train/train.py
 Resources/DeepMuon.png
 Tutorial/1.Regulations.md
```

### Comparing `DeepMuon-1.8.9/PKG-INFO` & `DeepMuon-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepMuon
-Version: 1.8.9
+Version: 1.9.1
 Summary: DeepMuon Project Built for Simple and Direct Deep Learning Researches on Dark Matter Searching
 Home-page: UNKNOWN
 Author: Airscker/Yufeng Wang
 Author-email: wangyufeng@mail.ustc.edu.cn
 License: UNKNOWN
 Keywords: Deep Learning,Searching Dark Matter,Direct and Simple
 Platform: UNKNOWN
```

### Comparing `DeepMuon-1.8.9/README.md` & `DeepMuon-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/Resources/DeepMuon.png` & `DeepMuon-1.9.1/Resources/DeepMuon.png`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/Tutorial/1.Regulations.md` & `DeepMuon-1.9.1/Tutorial/1.Regulations.md`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/Tutorial/2.Customize Dataset.md` & `DeepMuon-1.9.1/Tutorial/2.Customize Dataset.md`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/Tutorial/3.Customize Model.md` & `DeepMuon-1.9.1/Tutorial/3.Customize Model.md`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/Tutorial/4.Configuration.md` & `DeepMuon-1.9.1/Tutorial/4.Configuration.md`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/Tutorial/5.Training and Inference.md` & `DeepMuon-1.9.1/Tutorial/5.Training and Inference.md`

 * *Files identical despite different names*

### Comparing `DeepMuon-1.8.9/setup.py` & `DeepMuon-1.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,18 @@
                       'tqdm',
                       'numpy',
                       'pandas',
                       'numba',
                       'ptflops',
                       'torchinfo',
                       'captum',
-                      'monai'],
+                      'monai',
+                      'pynvml',
+                      'psutil',
+                      'GPUtil'],
     # Similar to `install_requires` above, these must be valid existing
     # projects.
     # extras_require={  # Optional
     #     "dev": ["check-manifest"],
     #     "test": ["coverage"],
     # },
     # If there are data files included in your packages that need to be
```

