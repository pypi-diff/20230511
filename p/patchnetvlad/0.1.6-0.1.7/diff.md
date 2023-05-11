# Comparing `tmp/patchnetvlad-0.1.6.tar.gz` & `tmp/patchnetvlad-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchnetvlad-0.1.6.tar", last modified: Thu Nov 11 03:32:09 2021, max compression
+gzip compressed data, was "patchnetvlad-0.1.7.tar", last modified: Thu May 11 01:40:01 2023, max compression
```

## Comparing `patchnetvlad-0.1.6.tar` & `patchnetvlad-0.1.7.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.276595 patchnetvlad-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12268 2021-11-11 03:32:09.276595 patchnetvlad-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11420 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)     2742 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/download_models.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8248 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/feature_extract.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9968 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/feature_match.py
--rw-r--r--   0 runner    (1001) docker     (121)     4711 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/match_realtime.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10600 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/match_two.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.248594 patchnetvlad-0.1.6/patchnetvlad/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.252594 patchnetvlad-0.1.6/patchnetvlad/configs/
--rw-r--r--   0 runner    (1001) docker     (121)      427 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/configs/performance.ini
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/configs/speed.ini
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/configs/storage.ini
--rw-r--r--   0 runner    (1001) docker     (121)      434 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/configs/train.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.252594 patchnetvlad-0.1.6/patchnetvlad/dataset_gt_files/
--rw-r--r--   0 runner    (1001) docker     (121)   883708 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_gt_files/nordland.npz
--rw-r--r--   0 runner    (1001) docker     (121)   269820 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_gt_files/pitts30k_test.npz
--rw-r--r--   0 runner    (1001) docker     (121)  1221548 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_gt_files/tokyo247.npz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.268595 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/example_imageNames_index.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/example_imageNames_query.txt
--rw-r--r--   0 runner    (1001) docker     (121)  1155152 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/mapillarycph_imageNames_index.txt
--rw-r--r--   0 runner    (1001) docker     (121)    44322 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/mapillarycph_imageNames_query.txt
--rw-r--r--   0 runner    (1001) docker     (121)   574665 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/mapillarysf_imageNames_index.txt
--rw-r--r--   0 runner    (1001) docker     (121)    21296 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/mapillarysf_imageNames_query.txt
--rw-r--r--   0 runner    (1001) docker     (121)   965720 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/nordland_imageNames_index.txt
--rw-r--r--   0 runner    (1001) docker     (121)   965720 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/nordland_imageNames_query.txt
--rw-r--r--   0 runner    (1001) docker     (121)   442499 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/pitts30k_imageNames_index.txt
--rw-r--r--   0 runner    (1001) docker     (121)   390216 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/pitts30k_imageNames_query.txt
--rw-r--r--   0 runner    (1001) docker     (121)  6990528 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/tokyo247_imageNames_index.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15750 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/tokyo247_imageNames_query.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.268595 patchnetvlad-0.1.6/patchnetvlad/example_images/
--rwxr-xr-x   0 runner    (1001) docker     (121)   576369 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/example_images/tokyo_db.png
--rwxr-xr-x   0 runner    (1001) docker     (121)  4397563 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/example_images/tokyo_query.jpg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.272595 patchnetvlad-0.1.6/patchnetvlad/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7411 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/models/local_matcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/models/models_generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     5437 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/models/netvlad.py
--rw-r--r--   0 runner    (1001) docker     (121)     8529 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/models/patchnetvlad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.272595 patchnetvlad-0.1.6/patchnetvlad/output_features/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/output_features/.hidden
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.272595 patchnetvlad-0.1.6/patchnetvlad/pretrained_models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/pretrained_models/.hidden
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.272595 patchnetvlad-0.1.6/patchnetvlad/results/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/results/.hidden
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.272595 patchnetvlad-0.1.6/patchnetvlad/tools/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4664 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/tools/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/tools/gen_image_file_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     6551 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/tools/patch_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.276595 patchnetvlad-0.1.6/patchnetvlad/training_tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/training_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      873 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/training_tools/convert_kapture_to_msls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4434 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/training_tools/get_clusters.py
--rw-r--r--   0 runner    (1001) docker     (121)    24104 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/training_tools/msls.py
--rw-r--r--   0 runner    (1001) docker     (121)     3947 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/training_tools/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     5579 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/training_tools/train_epoch.py
--rw-r--r--   0 runner    (1001) docker     (121)     5302 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/patchnetvlad/training_tools/val.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 03:32:09.252594 patchnetvlad-0.1.6/patchnetvlad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12268 2021-11-11 03:32:08.000000 patchnetvlad-0.1.6/patchnetvlad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2021-11-11 03:32:09.000000 patchnetvlad-0.1.6/patchnetvlad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-11 03:32:08.000000 patchnetvlad-0.1.6/patchnetvlad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-11-11 03:32:08.000000 patchnetvlad-0.1.6/patchnetvlad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-11-11 03:32:08.000000 patchnetvlad-0.1.6/patchnetvlad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-11-11 03:32:08.000000 patchnetvlad-0.1.6/patchnetvlad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-11 03:32:09.276595 patchnetvlad-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2959 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    11800 2021-11-11 03:32:00.000000 patchnetvlad-0.1.6/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.049310 patchnetvlad-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-11 01:39:41.000000 patchnetvlad-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-05-11 01:40:01.049310 patchnetvlad-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12009 2023-05-11 01:39:41.000000 patchnetvlad-0.1.7/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3087 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/download_models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8568 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/feature_extract.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10131 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/feature_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/match_realtime.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10600 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/match_two.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.021310 patchnetvlad-0.1.7/patchnetvlad/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.021310 patchnetvlad-0.1.7/patchnetvlad/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/configs/netvlad_extract.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/configs/performance.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/configs/speed.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/configs/storage.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/configs/train.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.025310 patchnetvlad-0.1.7/patchnetvlad/dataset_gt_files/
+-rw-r--r--   0 runner    (1001) docker     (123)   883708 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_gt_files/nordland.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   269820 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_gt_files/pitts30k_test.npz
+-rw-r--r--   0 runner    (1001) docker     (123)  1221548 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_gt_files/tokyo247.npz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.041310 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/example_imageNames_index.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/example_imageNames_query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1155152 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/mapillarycph_imageNames_index.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    44322 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/mapillarycph_imageNames_query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   574665 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/mapillarysf_imageNames_index.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21296 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/mapillarysf_imageNames_query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   965720 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/nordland_imageNames_index.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   965720 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/nordland_imageNames_query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   442499 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/pitts30k_imageNames_index.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   390216 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/pitts30k_imageNames_query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  6990528 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/tokyo247_imageNames_index.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/tokyo247_imageNames_query.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.041310 patchnetvlad-0.1.7/patchnetvlad/example_images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   576369 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/example_images/tokyo_db.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)  4397563 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/example_images/tokyo_query.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.045310 patchnetvlad-0.1.7/patchnetvlad/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/models/local_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/models/models_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/models/netvlad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/models/patchnetvlad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.045310 patchnetvlad-0.1.7/patchnetvlad/output_features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/output_features/.hidden
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.045310 patchnetvlad-0.1.7/patchnetvlad/pretrained_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/pretrained_models/.hidden
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.045310 patchnetvlad-0.1.7/patchnetvlad/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/results/.hidden
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.049310 patchnetvlad-0.1.7/patchnetvlad/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/tools/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/tools/gen_image_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/tools/patch_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.049310 patchnetvlad-0.1.7/patchnetvlad/training_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/training_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/training_tools/convert_kapture_to_msls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/training_tools/get_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/training_tools/msls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/training_tools/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/training_tools/train_epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/patchnetvlad/training_tools/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:40:01.021310 patchnetvlad-0.1.7/patchnetvlad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-05-11 01:40:00.000000 patchnetvlad-0.1.7/patchnetvlad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-11 01:40:00.000000 patchnetvlad-0.1.7/patchnetvlad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 01:40:00.000000 patchnetvlad-0.1.7/patchnetvlad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-11 01:40:00.000000 patchnetvlad-0.1.7/patchnetvlad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-11 01:40:00.000000 patchnetvlad-0.1.7/patchnetvlad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 01:40:00.000000 patchnetvlad-0.1.7/patchnetvlad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 01:40:01.049310 patchnetvlad-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-05-11 01:39:42.000000 patchnetvlad-0.1.7/train.py
```

### Comparing `patchnetvlad-0.1.6/LICENSE` & `patchnetvlad-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/PKG-INFO` & `patchnetvlad-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: patchnetvlad
-Version: 0.1.6
+Version: 0.1.7
 Summary: Patch-NetVLAD: An open-source Python implementation of the CVPR2021 paper
 Home-page: https://github.com/QVPR/Patch-NetVLAD
 Author: Stephen Hausler, Sourav Garg, Ming Xu, Michael Milford and Tobias Fischer
 Author-email: stephen.hausler@hdr.qut.edu.au
 License: MIT
 Keywords: python,place recognition,image retrieval,computer vision,robotics
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -57,15 +56,23 @@
 
 The code is licensed under the [MIT License](./LICENSE).
 
 ## Installation
 We recommend using conda (or better: mamba) to install all dependencies. If you have not yet installed conda/mamba, please download and install [`mambaforge`](https://github.com/conda-forge/miniforge).
 
 ```bash
-conda create -n patchnetvlad python=3.8 numpy pytorch-gpu torchvision natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge
+# On Linux:
+conda create -n patchnetvlad python numpy pytorch-gpu torchvision natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge
+# On MacOS (x86 Intel processor):
+conda create -n patchnetvlad python numpy pytorch torchvision natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge
+# On MacOS (ARM M1/M2 processor):
+conda create -n patchnetvlad python numpy pytorch torchvision natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge -c tobiasrobotics
+# On Windows:
+conda create -n patchnetvlad python numpy natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge
+conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
 
 conda activate patchnetvlad
 ```
 
 We provide several pre-trained models and configuration files. The pre-trained models will be downloaded automatically into the `pretrained_models` the first time feature extraction is performed.
 
 <details>
@@ -183,9 +190,7 @@
 `np.savez('dataset_gt_files/my_dataset.npz', utmQ=my_utmQ, utmDb=my_utmDb, posDistThr=my_posDistThr)`
 
 ## Acknowledgements
 We would like to thank Gustavo Carneiro, Niko Suenderhauf and Mark Zolotas for their valuable comments in preparing this paper. This work received funding from the Australian Government, via grant AUSMURIB000001 associated with ONR MURI grant N00014-19-1-2571. The authors acknowledge continued support from the Queensland University of Technology (QUT) through the Centre for Robotics.
 
 ## Related works
 Please check out [this collection](https://qcr.github.io/collection/vpr_overview/) of related works on place recognition.
-
-
```

### Comparing `patchnetvlad-0.1.6/README.md` & `patchnetvlad-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,23 @@
 
 The code is licensed under the [MIT License](./LICENSE).
 
 ## Installation
 We recommend using conda (or better: mamba) to install all dependencies. If you have not yet installed conda/mamba, please download and install [`mambaforge`](https://github.com/conda-forge/miniforge).
 
 ```bash
-conda create -n patchnetvlad python=3.8 numpy pytorch-gpu torchvision natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge
+# On Linux:
+conda create -n patchnetvlad python numpy pytorch-gpu torchvision natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge
+# On MacOS (x86 Intel processor):
+conda create -n patchnetvlad python numpy pytorch torchvision natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge
+# On MacOS (ARM M1/M2 processor):
+conda create -n patchnetvlad python numpy pytorch torchvision natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge -c tobiasrobotics
+# On Windows:
+conda create -n patchnetvlad python numpy natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge
+conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
 
 conda activate patchnetvlad
 ```
 
 We provide several pre-trained models and configuration files. The pre-trained models will be downloaded automatically into the `pretrained_models` the first time feature extraction is performed.
 
 <details>
```

### Comparing `patchnetvlad-0.1.6/download_models.py` & `patchnetvlad-0.1.7/download_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 
 import os
+import argparse
 import urllib.request
 from patchnetvlad.tools import PATCHNETVLAD_ROOT_DIR
 
 
 def ask_yesno(question):
     """
     Helper to get yes / no answer from user.
@@ -44,8 +45,13 @@
             urllib.request.urlretrieve("https://cloudstor.aarnet.edu.au/plus/s/WKl45MoboSyB4SH/download", os.path.join(dest_dir, "pittsburgh_WPCA512.pth.tar"))
         if not os.path.isfile(os.path.join(dest_dir, "pittsburgh_WPCA4096.pth.tar")):
             print('Downloading pittsburgh_WPCA4096.pth.tar')
             urllib.request.urlretrieve("https://cloudstor.aarnet.edu.au/plus/s/1aoTGbFjsekeKlB/download", os.path.join(dest_dir, "pittsburgh_WPCA4096.pth.tar"))
         print('Downloaded all pretrained models.')
 
 if __name__ == "__main__":
-    download_all_models()
+    parser = argparse.ArgumentParser(description='Download Pretrained Models for Patch-NetVLAD')
+    parser.add_argument('--ask_for_permission', action='store_true',
+                        help='Ask for permission before downloading pretrained models.')
+    args = parser.parse_args()
+
+    download_all_models(ask_for_permission=args.ask_for_permission)
```

### Comparing `patchnetvlad-0.1.6/feature_extract.py` & `patchnetvlad-0.1.7/feature_extract.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,37 +131,44 @@
 
     if not os.path.isfile(opt.dataset_file_path):
         opt.dataset_file_path = join(PATCHNETVLAD_ROOT_DIR, 'dataset_imagenames', opt.dataset_file_path)
 
     dataset = PlaceDataset(None, opt.dataset_file_path, opt.dataset_root_dir, None, config['feature_extract'])
 
     # must resume to do extraction
-    resume_ckpt = config['global_params']['resumePath'] + config['global_params']['num_pcs'] + '.pth.tar'
+    if config['global_params']['num_pcs'] != '0':
+        resume_ckpt = config['global_params']['resumePath'] + config['global_params']['num_pcs'] + '.pth.tar'
+    else:
+        resume_ckpt = config['global_params']['resumePath'] + '.pth.tar'
 
     # backup: try whether resume_ckpt is relative to PATCHNETVLAD_ROOT_DIR
     if not isfile(resume_ckpt):
         resume_ckpt = join(PATCHNETVLAD_ROOT_DIR, resume_ckpt)
         if not isfile(resume_ckpt):
             from download_models import download_all_models
             download_all_models(ask_for_permission=True)
 
     if isfile(resume_ckpt):
         print("=> loading checkpoint '{}'".format(resume_ckpt))
         checkpoint = torch.load(resume_ckpt, map_location=lambda storage, loc: storage)
-        assert checkpoint['state_dict']['WPCA.0.bias'].shape[0] == int(config['global_params']['num_pcs'])
+        if config['global_params']['num_pcs'] != '0':
+            assert checkpoint['state_dict']['WPCA.0.bias'].shape[0] == int(config['global_params']['num_pcs'])
         config['global_params']['num_clusters'] = str(checkpoint['state_dict']['pool.centroids'].shape[0])
 
-        model = get_model(encoder, encoder_dim, config['global_params'], append_pca_layer=True)
+        if config['global_params']['num_pcs'] != '0':
+            use_pca = True
+        else:
+            use_pca = False
+        model = get_model(encoder, encoder_dim, config['global_params'], append_pca_layer=use_pca)
         model.load_state_dict(checkpoint['state_dict'])
         
         if int(config['global_params']['nGPU']) > 1 and torch.cuda.device_count() > 1:
             model.encoder = nn.DataParallel(model.encoder)
             # if opt.mode.lower() != 'cluster':
             model.pool = nn.DataParallel(model.pool)
-
        
         model = model.to(device)
         print("=> loaded checkpoint '{}'".format(resume_ckpt, ))
     else:
         raise FileNotFoundError("=> no checkpoint found at '{}'".format(resume_ckpt))
 
     feature_extract(dataset, model, device, opt, config)
```

### Comparing `patchnetvlad-0.1.6/feature_match.py` & `patchnetvlad-0.1.7/feature_match.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                 _, idx = np.unique(np.floor(pred / 12).astype(np.int), return_index=True)
                 pred = pred[np.sort(idx)]
                 pred = pred[:max(n_values)]
                 predictions_new.append(pred)
             predictions = np.array(predictions_new)
         else:
             # noinspection PyArgumentList
-            _, predictions = faiss_index.search(qFeat, min(len(qFeat), max(n_values)))
+            _, predictions = faiss_index.search(qFeat, min(len(dbFeat), max(n_values)))
 
     reranked_predictions = local_matcher(predictions, eval_set, input_query_local_features_prefix,
                                          input_index_local_features_prefix, config, device)
 
     # save predictions to files - Kapture Output
     write_kapture_output(opt, eval_set, predictions, 'NetVLAD_predictions.txt')
     write_kapture_output(opt, eval_set, reranked_predictions, 'PatchNetVLAD_predictions.txt')
@@ -175,14 +175,15 @@
     parser.add_argument('--query_input_features_dir', type=str, required=True,
                         help='Path to load all query patch-netvlad features')
     parser.add_argument('--index_input_features_dir', type=str, required=True,
                         help='Path to load all database patch-netvlad features')
     parser.add_argument('--ground_truth_path', type=str, default=None,
                         help='Path (with extension) to a file that stores the ground-truth data')
     parser.add_argument('--result_save_folder', type=str, default='results')
+    parser.add_argument('--posDistThr', type=int, default=None, help='Manually set ground truth threshold')
     parser.add_argument('--nocuda', action='store_true', help='If true, use CPU only. Else use GPU.')
 
     opt = parser.parse_args()
     print(opt)
 
     configfile = opt.config_path
     assert os.path.isfile(configfile)
@@ -196,15 +197,16 @@
     device = torch.device("cuda" if cuda else "cpu")
 
     if not os.path.isfile(opt.query_file_path):
         opt.query_file_path = join(PATCHNETVLAD_ROOT_DIR, 'dataset_imagenames', opt.query_file_path)
     if not os.path.isfile(opt.index_file_path):
         opt.index_file_path = join(PATCHNETVLAD_ROOT_DIR, 'dataset_imagenames', opt.index_file_path)
 
-    dataset = PlaceDataset(opt.query_file_path, opt.index_file_path, opt.dataset_root_dir, opt.ground_truth_path, config['feature_extract'])
+    dataset = PlaceDataset(opt.query_file_path, opt.index_file_path, opt.dataset_root_dir, opt.ground_truth_path,
+                           config['feature_extract'], posDistThr=opt.posDistThr)
 
     feature_match(dataset, device, opt, config)
 
     torch.cuda.empty_cache()  # garbage clean GPU memory, a bug can occur when Pytorch doesn't automatically clear the
                               # memory after runs
     print('Done')
```

### Comparing `patchnetvlad-0.1.6/match_realtime.py` & `patchnetvlad-0.1.7/match_realtime.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/match_two.py` & `patchnetvlad-0.1.7/match_two.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_gt_files/nordland.npz` & `patchnetvlad-0.1.7/patchnetvlad/dataset_gt_files/nordland.npz`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_gt_files/pitts30k_test.npz` & `patchnetvlad-0.1.7/patchnetvlad/dataset_gt_files/pitts30k_test.npz`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_gt_files/tokyo247.npz` & `patchnetvlad-0.1.7/patchnetvlad/dataset_gt_files/tokyo247.npz`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/mapillarycph_imageNames_index.txt` & `patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/mapillarycph_imageNames_index.txt`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/mapillarycph_imageNames_query.txt` & `patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/mapillarycph_imageNames_query.txt`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/mapillarysf_imageNames_index.txt` & `patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/mapillarysf_imageNames_index.txt`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/mapillarysf_imageNames_query.txt` & `patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/mapillarysf_imageNames_query.txt`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/nordland_imageNames_index.txt` & `patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/nordland_imageNames_index.txt`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/nordland_imageNames_query.txt` & `patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/nordland_imageNames_query.txt`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/pitts30k_imageNames_index.txt` & `patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/pitts30k_imageNames_index.txt`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/pitts30k_imageNames_query.txt` & `patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/pitts30k_imageNames_query.txt`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/tokyo247_imageNames_index.txt` & `patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/tokyo247_imageNames_index.txt`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/dataset_imagenames/tokyo247_imageNames_query.txt` & `patchnetvlad-0.1.7/patchnetvlad/dataset_imagenames/tokyo247_imageNames_query.txt`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/example_images/tokyo_db.png` & `patchnetvlad-0.1.7/patchnetvlad/example_images/tokyo_db.png`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/example_images/tokyo_query.jpg` & `patchnetvlad-0.1.7/patchnetvlad/example_images/tokyo_query.jpg`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/models/local_matcher.py` & `patchnetvlad-0.1.7/patchnetvlad/models/local_matcher.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/models/models_generic.py` & `patchnetvlad-0.1.7/patchnetvlad/models/models_generic.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 '''
 
 
+from packaging.version import parse as parse_version
+import torchvision
 import torchvision.models as models
 import torch.nn as nn
 import torch.nn.functional as F
 from patchnetvlad.models.netvlad import NetVLAD
 from patchnetvlad.models.patchnetvlad import PatchNetVLAD
 
 
@@ -47,15 +49,19 @@
 def get_pca_encoding(model, vlad_encoding):
     pca_encoding = model.WPCA(vlad_encoding.unsqueeze(-1).unsqueeze(-1))
     return pca_encoding
 
 
 def get_backend():
     enc_dim = 512
-    enc = models.vgg16(pretrained=True)
+    if parse_version(torchvision.__version__) >= parse_version('0.13'):
+        enc = models.vgg16(weights='IMAGENET1K_V1')
+    else:
+        enc = models.vgg16(pretrained=True)
+
     layers = list(enc.features.children())[:-2]
     # only train conv5_1, conv5_2, and conv5_3 (leave rest same as Imagenet trained weights)
     for layer in layers[:-5]:
         for p in layer.parameters():
             p.requires_grad = False
     enc = nn.Sequential(*layers)
     return enc_dim, enc
@@ -74,15 +80,15 @@
         net_vlad = PatchNetVLAD(num_clusters=int(config['num_clusters']), dim=encoder_dim,
                                 vladv2=config.getboolean('vladv2'),
                                 patch_sizes=config['patch_sizes'], strides=config['strides'])
         nn_model.add_module('pool', net_vlad)
     elif config['pooling'].lower() == 'max':
         global_pool = nn.AdaptiveMaxPool2d((1, 1))
         nn_model.add_module('pool', nn.Sequential(*[global_pool, Flatten(), L2Norm()]))
-    elif config['pooling'].pooling.lower() == 'avg':
+    elif config['pooling'].lower() == 'avg':
         global_pool = nn.AdaptiveAvgPool2d((1, 1))
         nn_model.add_module('pool', nn.Sequential(*[global_pool, Flatten(), L2Norm()]))
     else:
         raise ValueError('Unknown pooling type: ' + config['pooling'].lower())
 
     if append_pca_layer:
         num_pcs = int(config['num_pcs'])
```

### Comparing `patchnetvlad-0.1.6/patchnetvlad/models/netvlad.py` & `patchnetvlad-0.1.7/patchnetvlad/models/netvlad.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/models/patchnetvlad.py` & `patchnetvlad-0.1.7/patchnetvlad/models/patchnetvlad.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/tools/datasets.py` & `patchnetvlad-0.1.7/patchnetvlad/tools/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,24 +49,26 @@
             transforms.ToTensor(),
             transforms.Normalize(mean=[0.485, 0.456, 0.406],
                                  std=[0.229, 0.224, 0.225]),
         ])
 
 
 class PlaceDataset(data.Dataset):
-    def __init__(self, query_file_path, index_file_path, dataset_root_dir, ground_truth_path, config):
+    def __init__(self, query_file_path, index_file_path, dataset_root_dir, ground_truth_path, config, posDistThr=None):
         super().__init__()
 
         self.queries, self.database, self.numQ, self.numDb, self.utmQ, self.utmDb, self.posDistThr = None, None, None, None, None, None, None
         if query_file_path is not None:
             self.queries, self.numQ = self.parse_text_file(query_file_path)
         if index_file_path is not None:
             self.database, self.numDb = self.parse_text_file(index_file_path)
         if ground_truth_path is not None:
             self.utmQ, self.utmDb, self.posDistThr = self.parse_gt_file(ground_truth_path)
+        if posDistThr is not None:
+            self.posDistThr = posDistThr
 
         if self.queries is not None:
             self.images = self.database + self.queries
         else:
             self.images = self.database
 
         self.images = [os.path.join(dataset_root_dir, image) for image in self.images]
```

### Comparing `patchnetvlad-0.1.6/patchnetvlad/tools/gen_image_file_list.py` & `patchnetvlad-0.1.7/patchnetvlad/tools/gen_image_file_list.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/tools/patch_matcher.py` & `patchnetvlad-0.1.7/patchnetvlad/tools/patch_matcher.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/training_tools/convert_kapture_to_msls.py` & `patchnetvlad-0.1.7/patchnetvlad/training_tools/convert_kapture_to_msls.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/training_tools/get_clusters.py` & `patchnetvlad-0.1.7/patchnetvlad/training_tools/get_clusters.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/training_tools/msls.py` & `patchnetvlad-0.1.7/patchnetvlad/training_tools/msls.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/training_tools/tools.py` & `patchnetvlad-0.1.7/patchnetvlad/training_tools/tools.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/training_tools/train_epoch.py` & `patchnetvlad-0.1.7/patchnetvlad/training_tools/train_epoch.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad/training_tools/val.py` & `patchnetvlad-0.1.7/patchnetvlad/training_tools/val.py`

 * *Files identical despite different names*

### Comparing `patchnetvlad-0.1.6/patchnetvlad.egg-info/PKG-INFO` & `patchnetvlad-0.1.7/patchnetvlad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: patchnetvlad
-Version: 0.1.6
+Version: 0.1.7
 Summary: Patch-NetVLAD: An open-source Python implementation of the CVPR2021 paper
 Home-page: https://github.com/QVPR/Patch-NetVLAD
 Author: Stephen Hausler, Sourav Garg, Ming Xu, Michael Milford and Tobias Fischer
 Author-email: stephen.hausler@hdr.qut.edu.au
 License: MIT
 Keywords: python,place recognition,image retrieval,computer vision,robotics
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -57,15 +56,23 @@
 
 The code is licensed under the [MIT License](./LICENSE).
 
 ## Installation
 We recommend using conda (or better: mamba) to install all dependencies. If you have not yet installed conda/mamba, please download and install [`mambaforge`](https://github.com/conda-forge/miniforge).
 
 ```bash
-conda create -n patchnetvlad python=3.8 numpy pytorch-gpu torchvision natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge
+# On Linux:
+conda create -n patchnetvlad python numpy pytorch-gpu torchvision natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge
+# On MacOS (x86 Intel processor):
+conda create -n patchnetvlad python numpy pytorch torchvision natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge
+# On MacOS (ARM M1/M2 processor):
+conda create -n patchnetvlad python numpy pytorch torchvision natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge -c tobiasrobotics
+# On Windows:
+conda create -n patchnetvlad python numpy natsort tqdm opencv pillow scikit-learn faiss matplotlib-base -c conda-forge
+conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
 
 conda activate patchnetvlad
 ```
 
 We provide several pre-trained models and configuration files. The pre-trained models will be downloaded automatically into the `pretrained_models` the first time feature extraction is performed.
 
 <details>
@@ -183,9 +190,7 @@
 `np.savez('dataset_gt_files/my_dataset.npz', utmQ=my_utmQ, utmDb=my_utmDb, posDistThr=my_posDistThr)`
 
 ## Acknowledgements
 We would like to thank Gustavo Carneiro, Niko Suenderhauf and Mark Zolotas for their valuable comments in preparing this paper. This work received funding from the Australian Government, via grant AUSMURIB000001 associated with ONR MURI grant N00014-19-1-2571. The authors acknowledge continued support from the Queensland University of Technology (QUT) through the Centre for Robotics.
 
 ## Related works
 Please check out [this collection](https://qcr.github.io/collection/vpr_overview/) of related works on place recognition.
-
-
```

### Comparing `patchnetvlad-0.1.6/patchnetvlad.egg-info/SOURCES.txt` & `patchnetvlad-0.1.7/patchnetvlad.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 patchnetvlad/__init__.py
 patchnetvlad.egg-info/PKG-INFO
 patchnetvlad.egg-info/SOURCES.txt
 patchnetvlad.egg-info/dependency_links.txt
 patchnetvlad.egg-info/entry_points.txt
 patchnetvlad.egg-info/requires.txt
 patchnetvlad.egg-info/top_level.txt
+patchnetvlad/configs/netvlad_extract.ini
 patchnetvlad/configs/performance.ini
 patchnetvlad/configs/speed.ini
 patchnetvlad/configs/storage.ini
 patchnetvlad/configs/train.ini
 patchnetvlad/dataset_gt_files/nordland.npz
 patchnetvlad/dataset_gt_files/pitts30k_test.npz
 patchnetvlad/dataset_gt_files/tokyo247.npz
```

### Comparing `patchnetvlad-0.1.6/setup.py` & `patchnetvlad-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # workaround as opencv-python does not show up in "pip list" within a conda environment
 # we do not care as conda recipe has py-opencv requirement anyhow
 is_conda = os.path.exists(os.path.join(sys.prefix, 'conda-meta'))
 if not is_conda:
     install_require_list.append('opencv-python')
 
 setup(name='patchnetvlad',
-      version='0.1.6',
+      version='0.1.7',
       description='Patch-NetVLAD: An open-source Python implementation of the CVPR2021 paper',
       long_description = long_description,
       long_description_content_type='text/markdown',
       author='Stephen Hausler, Sourav Garg, Ming Xu, Michael Milford and Tobias Fischer',
       author_email='stephen.hausler@hdr.qut.edu.au',
       url='https://github.com/QVPR/Patch-NetVLAD',
       license='MIT',
```

### Comparing `patchnetvlad-0.1.6/train.py` & `patchnetvlad-0.1.7/train.py`

 * *Files identical despite different names*

