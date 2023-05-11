# Comparing `tmp/tedana-0.0.9a0.tar.gz` & `tmp/tedana-0.0.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tedana-0.0.9a0.tar", last modified: Tue May  5 15:01:42 2020, max compression
+gzip compressed data, was "dist/tedana-0.0.9a1.tar", last modified: Sun May 10 18:55:58 2020, max compression
```

## Comparing `tedana-0.0.9a0.tar` & `tedana-0.0.9a1.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-05 15:01:42.000000 tedana-0.0.9a0/
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)       49 2019-09-25 00:22:11.000000 tedana-0.0.9a0/MANIFEST.in
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      983 2020-05-05 15:01:42.000000 tedana-0.0.9a0/PKG-INFO
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)    13666 2020-05-05 15:00:10.000000 tedana-0.0.9a0/README.md
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      303 2020-05-05 15:01:42.000000 tedana-0.0.9a0/setup.cfg
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2088 2019-11-06 14:13:06.000000 tedana-0.0.9a0/setup.py
-drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana/
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1096 2019-09-25 00:22:11.000000 tedana-0.0.9a0/tedana/__init__.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      498 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana/_version.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     7738 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/combine.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)    12754 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/decay.py
-drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana/decomposition/
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      269 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/decomposition/__init__.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1373 2019-11-12 03:58:07.000000 tedana-0.0.9a0/tedana/decomposition/_utils.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2847 2019-11-12 03:58:07.000000 tedana-0.0.9a0/tedana/decomposition/ica.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)    18935 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/decomposition/ma_pca.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)    11199 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/decomposition/pca.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2080 2019-09-25 00:22:11.000000 tedana-0.0.9a0/tedana/due.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     8577 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/gscontrol.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2140 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/info.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)    19107 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/io.py
-drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana/metrics/
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      246 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/metrics/__init__.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)    18003 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/metrics/kundu_fit.py
-drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana/selection/
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      284 2019-09-25 00:22:11.000000 tedana-0.0.9a0/tedana/selection/__init__.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2823 2019-11-12 03:58:07.000000 tedana-0.0.9a0/tedana/selection/_utils.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)    16126 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/selection/tedica.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     5238 2019-11-12 03:58:07.000000 tedana-0.0.9a0/tedana/selection/tedpca.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     5495 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/stats.py
-drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana/tests/
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      123 2019-09-25 00:22:11.000000 tedana-0.0.9a0/tedana/tests/__init__.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      523 2019-11-12 03:58:07.000000 tedana-0.0.9a0/tedana/tests/conftest.py
-drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana/tests/data/
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1825 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/data/cornell_three_echo_outputs.txt
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)   534936 2019-09-25 00:22:11.000000 tedana-0.0.9a0/tedana/tests/data/echo1.nii.gz
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)   504830 2019-09-25 00:22:11.000000 tedana-0.0.9a0/tedana/tests/data/echo2.nii.gz
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)   475338 2019-09-25 00:22:11.000000 tedana-0.0.9a0/tedana/tests/data/echo3.nii.gz
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1328 2019-09-25 00:22:11.000000 tedana-0.0.9a0/tedana/tests/data/fdist.npy
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1309 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/data/fiu_four_echo_outputs.txt
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     4481 2019-09-25 00:22:11.000000 tedana-0.0.9a0/tedana/tests/data/mask.nii.gz
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2398 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/data/nih_five_echo_outputs_verbose.txt
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2048 2019-09-25 00:22:11.000000 tedana-0.0.9a0/tedana/tests/test_combine.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     5274 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/test_decay.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1666 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/test_gscontrol.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     6096 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/test_integration.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     5325 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/test_io.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     4773 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/test_mapca.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2314 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/test_model_fit_dependence_metrics.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1576 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/test_model_kundu_metrics.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1246 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/test_selection.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     4759 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/test_stats.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     5894 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/test_t2smap.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     7255 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/test_utils.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      330 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/tests/test_viz.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      400 2019-09-25 00:22:11.000000 tedana-0.0.9a0/tedana/tests/utils.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)    11354 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/utils.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)    13541 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/viz.py
-drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana/workflows/
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      292 2019-09-25 00:22:11.000000 tedana-0.0.9a0/tedana/workflows/__init__.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      705 2019-11-12 03:58:07.000000 tedana-0.0.9a0/tedana/workflows/parser_utils.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)    10953 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/workflows/t2smap.py
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)    32055 2020-05-05 15:00:10.000000 tedana-0.0.9a0/tedana/workflows/tedana.py
-drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana.egg-info/
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      983 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana.egg-info/PKG-INFO
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1645 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana.egg-info/SOURCES.txt
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)        1 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana.egg-info/dependency_links.txt
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)       97 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana.egg-info/entry_points.txt
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)        1 2019-04-23 18:32:26.000000 tedana-0.0.9a0/tedana.egg-info/not-zip-safe
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)      335 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana.egg-info/requires.txt
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)        7 2020-05-05 15:01:42.000000 tedana-0.0.9a0/tedana.egg-info/top_level.txt
--rw-r--r--   0 emdupre   (1000) emdupre   (1000)    68611 2019-09-25 00:22:11.000000 tedana-0.0.9a0/versioneer.py
+drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-10 18:55:58.000000 tedana-0.0.9a1/
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)       49 2019-09-25 00:22:11.000000 tedana-0.0.9a1/MANIFEST.in
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      984 2020-05-10 18:55:58.000000 tedana-0.0.9a1/PKG-INFO
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)    13666 2020-05-05 15:00:10.000000 tedana-0.0.9a1/README.md
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      303 2020-05-10 18:55:58.000000 tedana-0.0.9a1/setup.cfg
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2088 2019-11-06 14:13:06.000000 tedana-0.0.9a1/setup.py
+drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana/
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1096 2019-09-25 00:22:11.000000 tedana-0.0.9a1/tedana/__init__.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      499 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana/_version.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     7738 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/combine.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)    12754 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/decay.py
+drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana/decomposition/
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      269 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/decomposition/__init__.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1373 2019-11-12 03:58:07.000000 tedana-0.0.9a1/tedana/decomposition/_utils.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2847 2019-11-12 03:58:07.000000 tedana-0.0.9a1/tedana/decomposition/ica.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)    18935 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/decomposition/ma_pca.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)    11199 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/decomposition/pca.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2080 2019-09-25 00:22:11.000000 tedana-0.0.9a1/tedana/due.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     8577 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/gscontrol.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2140 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/info.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)    19107 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/io.py
+drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana/metrics/
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      246 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/metrics/__init__.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)    18003 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/metrics/kundu_fit.py
+drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana/selection/
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      284 2019-09-25 00:22:11.000000 tedana-0.0.9a1/tedana/selection/__init__.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2823 2019-11-12 03:58:07.000000 tedana-0.0.9a1/tedana/selection/_utils.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)    16126 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/selection/tedica.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     5238 2019-11-12 03:58:07.000000 tedana-0.0.9a1/tedana/selection/tedpca.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     5495 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/stats.py
+drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana/tests/
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      123 2019-09-25 00:22:11.000000 tedana-0.0.9a1/tedana/tests/__init__.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      523 2019-11-12 03:58:07.000000 tedana-0.0.9a1/tedana/tests/conftest.py
+drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana/tests/data/
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1825 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/data/cornell_three_echo_outputs.txt
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)   534936 2019-09-25 00:22:11.000000 tedana-0.0.9a1/tedana/tests/data/echo1.nii.gz
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)   504830 2019-09-25 00:22:11.000000 tedana-0.0.9a1/tedana/tests/data/echo2.nii.gz
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)   475338 2019-09-25 00:22:11.000000 tedana-0.0.9a1/tedana/tests/data/echo3.nii.gz
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1328 2019-09-25 00:22:11.000000 tedana-0.0.9a1/tedana/tests/data/fdist.npy
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1309 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/data/fiu_four_echo_outputs.txt
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     4481 2019-09-25 00:22:11.000000 tedana-0.0.9a1/tedana/tests/data/mask.nii.gz
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      104 2020-05-10 18:54:37.000000 tedana-0.0.9a1/tedana/tests/data/nih_five_echo_outputs_t2smap.txt
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2398 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/data/nih_five_echo_outputs_verbose.txt
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2048 2019-09-25 00:22:11.000000 tedana-0.0.9a1/tedana/tests/test_combine.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     5274 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/test_decay.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1666 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/test_gscontrol.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     7491 2020-05-10 18:54:37.000000 tedana-0.0.9a1/tedana/tests/test_integration.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     5325 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/test_io.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     4773 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/test_mapca.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     2314 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/test_model_fit_dependence_metrics.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1576 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/test_model_kundu_metrics.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1246 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/test_selection.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     4759 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/test_stats.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     5894 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/test_t2smap.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     7255 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/test_utils.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      330 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/tests/test_viz.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      400 2019-09-25 00:22:11.000000 tedana-0.0.9a1/tedana/tests/utils.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)    11354 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/utils.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)    13541 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/viz.py
+drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana/workflows/
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      292 2019-09-25 00:22:11.000000 tedana-0.0.9a1/tedana/workflows/__init__.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      705 2019-11-12 03:58:07.000000 tedana-0.0.9a1/tedana/workflows/parser_utils.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)    10956 2020-05-10 18:54:37.000000 tedana-0.0.9a1/tedana/workflows/t2smap.py
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)    32055 2020-05-05 15:00:10.000000 tedana-0.0.9a1/tedana/workflows/tedana.py
+drwxr-xr-x   0 emdupre   (1000) emdupre   (1000)        0 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana.egg-info/
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      984 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana.egg-info/PKG-INFO
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)     1696 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana.egg-info/SOURCES.txt
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)        1 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana.egg-info/dependency_links.txt
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)       97 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana.egg-info/entry_points.txt
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)        1 2019-04-23 18:32:26.000000 tedana-0.0.9a1/tedana.egg-info/not-zip-safe
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)      335 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana.egg-info/requires.txt
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)        7 2020-05-10 18:55:58.000000 tedana-0.0.9a1/tedana.egg-info/top_level.txt
+-rw-r--r--   0 emdupre   (1000) emdupre   (1000)    68611 2019-09-25 00:22:11.000000 tedana-0.0.9a1/versioneer.py
```

### Comparing `tedana-0.0.9a0/PKG-INFO` & `tedana-0.0.9a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tedana
-Version: 0.0.9a0
+Version: 0.0.9a1
 Summary: TE-Dependent Analysis (tedana) of multi-echo functional magnetic resonance imaging (fMRI) data.
 Home-page: https://github.com/me-ica/tedana
 Author: tedana developers
 Author-email: emd222@cornell.edu
 Maintainer: Elizabeth DuPre
 Maintainer-email: emd222@cornell.edu
 License: LGPL 2.1
-Download-URL: https://github.com/ME-ICA/tedana/archive/0.0.9a.tar.gz
+Download-URL: https://github.com/ME-ICA/tedana/archive/0.0.9a1.tar.gz
 Description: To do.
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `tedana-0.0.9a0/README.md` & `tedana-0.0.9a1/README.md`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/setup.py` & `tedana-0.0.9a1/setup.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/__init__.py` & `tedana-0.0.9a1/tedana/__init__.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/combine.py` & `tedana-0.0.9a1/tedana/combine.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/decay.py` & `tedana-0.0.9a1/tedana/decay.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/decomposition/_utils.py` & `tedana-0.0.9a1/tedana/decomposition/_utils.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/decomposition/ica.py` & `tedana-0.0.9a1/tedana/decomposition/ica.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/decomposition/ma_pca.py` & `tedana-0.0.9a1/tedana/decomposition/ma_pca.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/decomposition/pca.py` & `tedana-0.0.9a1/tedana/decomposition/pca.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/due.py` & `tedana-0.0.9a1/tedana/due.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/gscontrol.py` & `tedana-0.0.9a1/tedana/gscontrol.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/info.py` & `tedana-0.0.9a1/tedana/info.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/io.py` & `tedana-0.0.9a1/tedana/io.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/metrics/kundu_fit.py` & `tedana-0.0.9a1/tedana/metrics/kundu_fit.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/selection/_utils.py` & `tedana-0.0.9a1/tedana/selection/_utils.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/selection/tedica.py` & `tedana-0.0.9a1/tedana/selection/tedica.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/selection/tedpca.py` & `tedana-0.0.9a1/tedana/selection/tedpca.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/stats.py` & `tedana-0.0.9a1/tedana/stats.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/conftest.py` & `tedana-0.0.9a1/tedana/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/data/cornell_three_echo_outputs.txt` & `tedana-0.0.9a1/tedana/tests/data/cornell_three_echo_outputs.txt`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/data/echo1.nii.gz` & `tedana-0.0.9a1/tedana/tests/data/echo1.nii.gz`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/data/echo2.nii.gz` & `tedana-0.0.9a1/tedana/tests/data/echo2.nii.gz`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/data/echo3.nii.gz` & `tedana-0.0.9a1/tedana/tests/data/echo3.nii.gz`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/data/fdist.npy` & `tedana-0.0.9a1/tedana/tests/data/fdist.npy`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/data/fiu_four_echo_outputs.txt` & `tedana-0.0.9a1/tedana/tests/data/fiu_four_echo_outputs.txt`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/data/mask.nii.gz` & `tedana-0.0.9a1/tedana/tests/data/mask.nii.gz`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/data/nih_five_echo_outputs_verbose.txt` & `tedana-0.0.9a1/tedana/tests/data/nih_five_echo_outputs_verbose.txt`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/test_combine.py` & `tedana-0.0.9a1/tedana/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/test_decay.py` & `tedana-0.0.9a1/tedana/tests/test_decay.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/test_gscontrol.py` & `tedana-0.0.9a1/tedana/tests/test_gscontrol.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/test_integration.py` & `tedana-0.0.9a1/tedana/tests/test_integration.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from pkg_resources import resource_filename
 
 import pytest
 import requests
 import pandas as pd
 
 from tedana.workflows import tedana as tedana_cli
+from tedana.workflows import t2smap as t2smap_cli
 from tedana import io
 
 
 def check_integration_outputs(fname, outpath):
     """
     Checks outputs of integration tests
 
@@ -179,7 +180,40 @@
              '--mix', os.path.join(out_dir, 'ica_mixing.tsv')])
     tedana_cli._main(args)
 
     # compare the generated output files
     fn = resource_filename('tedana',
                            'tests/data/cornell_three_echo_outputs.txt')
     check_integration_outputs(fn, out_dir)
+
+
+def test_integration_t2smap(skip_integration):
+    """Integration test of the full t2smap workflow using five-echo test data
+    """
+    if skip_integration:
+        pytest.skip('Skipping t2smap integration test')
+    out_dir = '/tmp/data/five-echo/t2smap_five-echo'
+    if os.path.exists(out_dir):
+        shutil.rmtree(out_dir)
+
+    # download data and run the test
+    download_test_data('https://osf.io/9c42e/download',
+                       os.path.dirname(out_dir))
+    prepend = '/tmp/data/five-echo/p06.SBJ01_S09_Task11_e'
+    suffix = '.sm.nii.gz'
+    datalist = [prepend + str(i + 1) + suffix for i in range(5)]
+    echo_times = [15.4, 29.7, 44.0, 58.3, 72.6]
+    args = (['-d'] + datalist + ['-e'] + [str(te) for te in echo_times] +
+            ['--out-dir', out_dir, '--fittype', 'curvefit'])
+    t2smap_cli._main(args)
+
+    # compare the generated output files
+    fname = resource_filename('tedana',
+                              'tests/data/nih_five_echo_outputs_t2smap.txt')
+    # Gets filepaths generated by integration test
+    existing = [os.path.relpath(f, out_dir) for f in
+                glob.glob(os.path.join(out_dir, '**'), recursive=True)[1:]]
+
+    # Compares remaining files with those expected
+    with open(fname, 'r') as f:
+        tocheck = f.read().splitlines()
+    assert sorted(tocheck) == sorted(existing)
```

### Comparing `tedana-0.0.9a0/tedana/tests/test_io.py` & `tedana-0.0.9a1/tedana/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/test_mapca.py` & `tedana-0.0.9a1/tedana/tests/test_mapca.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/test_model_fit_dependence_metrics.py` & `tedana-0.0.9a1/tedana/tests/test_model_fit_dependence_metrics.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/test_model_kundu_metrics.py` & `tedana-0.0.9a1/tedana/tests/test_model_kundu_metrics.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/test_selection.py` & `tedana-0.0.9a1/tedana/tests/test_selection.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/test_stats.py` & `tedana-0.0.9a1/tedana/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/test_t2smap.py` & `tedana-0.0.9a1/tedana/tests/test_t2smap.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/tests/test_utils.py` & `tedana-0.0.9a1/tedana/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/utils.py` & `tedana-0.0.9a1/tedana/utils.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/viz.py` & `tedana-0.0.9a1/tedana/viz.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/workflows/parser_utils.py` & `tedana-0.0.9a1/tedana/workflows/parser_utils.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana/workflows/t2smap.py` & `tedana-0.0.9a1/tedana/workflows/t2smap.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
                                       interpolation_method='lower')
     cap_t2s_sec = utils.millisec2sec(cap_t2s * 10.)
     LGR.debug('Setting cap on T2* map at {:.5f}s'.format(cap_t2s_sec))
     t2s_limited[t2s_limited > cap_t2s * 10] = cap_t2s
 
     LGR.info('Computing optimal combination')
     # optimally combine data
-    OCcatd = combine.make_optcom(catd, tes, mask, t2s=t2s_full,
+    OCcatd = combine.make_optcom(catd, tes, masksum, t2s=t2s_full,
                                  combmode=combmode)
 
     # clean up numerical errors
     for arr in (OCcatd, s0_limited, t2s_limited):
         np.nan_to_num(arr, copy=False)
 
     s0_limited[s0_limited < 0] = 0
```

### Comparing `tedana-0.0.9a0/tedana/workflows/tedana.py` & `tedana-0.0.9a1/tedana/workflows/tedana.py`

 * *Files identical despite different names*

### Comparing `tedana-0.0.9a0/tedana.egg-info/PKG-INFO` & `tedana-0.0.9a1/tedana.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tedana
-Version: 0.0.9a0
+Version: 0.0.9a1
 Summary: TE-Dependent Analysis (tedana) of multi-echo functional magnetic resonance imaging (fMRI) data.
 Home-page: https://github.com/me-ica/tedana
 Author: tedana developers
 Author-email: emd222@cornell.edu
 Maintainer: Elizabeth DuPre
 Maintainer-email: emd222@cornell.edu
 License: LGPL 2.1
-Download-URL: https://github.com/ME-ICA/tedana/archive/0.0.9a.tar.gz
+Download-URL: https://github.com/ME-ICA/tedana/archive/0.0.9a1.tar.gz
 Description: To do.
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `tedana-0.0.9a0/tedana.egg-info/SOURCES.txt` & `tedana-0.0.9a1/tedana.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,12 +51,13 @@
 tedana/tests/data/cornell_three_echo_outputs.txt
 tedana/tests/data/echo1.nii.gz
 tedana/tests/data/echo2.nii.gz
 tedana/tests/data/echo3.nii.gz
 tedana/tests/data/fdist.npy
 tedana/tests/data/fiu_four_echo_outputs.txt
 tedana/tests/data/mask.nii.gz
+tedana/tests/data/nih_five_echo_outputs_t2smap.txt
 tedana/tests/data/nih_five_echo_outputs_verbose.txt
 tedana/workflows/__init__.py
 tedana/workflows/parser_utils.py
 tedana/workflows/t2smap.py
 tedana/workflows/tedana.py
```

### Comparing `tedana-0.0.9a0/versioneer.py` & `tedana-0.0.9a1/versioneer.py`

 * *Files identical despite different names*

