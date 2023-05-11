# Comparing `tmp/soxspipe-0.7.2.tar.gz` & `tmp/soxspipe-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soxspipe-0.7.2.tar", last modified: Fri Mar  3 13:57:58 2023, max compression
+gzip compressed data, was "soxspipe-0.8.0.tar", last modified: Thu May 11 19:20:31 2023, max compression
```

## Comparing `soxspipe-0.7.2.tar` & `soxspipe-0.8.0.tar`

### file list

```diff
@@ -1,94 +1,98 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-03-03 13:57:58.682355 soxspipe-0.7.2/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      437 2023-03-03 13:31:11.000000 soxspipe-0.7.2/.readthedocs.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11001 2023-03-03 13:31:11.000000 soxspipe-0.7.2/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-03-03 13:31:11.000000 soxspipe-0.7.2/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      361 2023-03-03 13:31:11.000000 soxspipe-0.7.2/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2532 2023-03-03 13:57:58.682355 soxspipe-0.7.2/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1889 2023-03-03 13:31:11.000000 soxspipe-0.7.2/README.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-03-03 13:57:58.682355 soxspipe-0.7.2/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2060 2023-03-03 13:31:12.000000 soxspipe-0.7.2/setup.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-03-03 13:57:58.094334 soxspipe-0.7.2/soxspipe/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      141 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      474 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/advanced_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7864 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-03-03 13:57:58.102334 soxspipe-0.7.2/soxspipe/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      665 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1151 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/combiner.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    61170 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/create_dispersion_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    41751 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/detect_continuum.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    32171 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/detect_order_edges.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2932 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/detector_lookup.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3534 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/dispersion_map_to_pixel_arrays.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6484 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/filenamer.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/getpackagepath.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4422 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/keyword_lookup.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8665 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/polynomials.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    17809 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/set_of_files.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11869 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/subtract_background.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    68318 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/subtract_sky.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    29218 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/commonutils/toolkit.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4817 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/default_settings.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-03-03 13:57:58.106334 soxspipe-0.7.2/soxspipe/recipes/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      457 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/recipes/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    45875 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/recipes/_base_recipe_.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9153 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/recipes/soxs_disp_solution.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13354 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/recipes/soxs_mbias.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7748 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/recipes/soxs_mdark.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    34858 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/recipes/soxs_mflat.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6260 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/recipes/soxs_nod_mode.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10809 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/recipes/soxs_order_centres.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11616 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/recipes/soxs_spatial_solution.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11821 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/recipes/soxs_stare.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5777 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/recipes/soxs_straighten.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-03-03 13:57:58.106334 soxspipe-0.7.2/soxspipe/resources/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2732 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/soxs_detector_parameters.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      760 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/soxs_keywords.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-03-03 13:57:58.086333 soxspipe-0.7.2/soxspipe/resources/static_calibrations/
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-03-03 13:57:58.266340 soxspipe-0.7.2/soxspipe/resources/static_calibrations/soxs/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004) 33557761 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/soxs/BP_MAP_RP_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   155520 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/soxs/SOXS_PINHOLE_TAB_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   155520 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/soxs/SOXS_PINHOLE_TAB_NIR_OLD.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8640 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/soxs/SOXS_SPECTRAL_FORMAT_TAB_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    46080 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/soxs/skylines.fits
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-03-03 13:57:58.682355 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)  8674560 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004) 24629760 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x1.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004) 12340800 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)  6197760 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_2x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004) 32820480 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x1.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004) 16436160 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)  8245440 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_2x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    17280 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14400 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_UVB.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14400 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_VIS.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   169920 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   132480 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x1.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   132480 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   132480 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_2x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   167040 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x1.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   167040 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   167040 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_2x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    60480 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23040 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x1.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23040 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23040 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_2x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    28800 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x1.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    28800 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    28800 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_2x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    46080 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/skylines.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2713 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/xsh_detector_parameters.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9625 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/resources/xsh_keywords.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9670 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3272 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/test_settings_soxs.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3386 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/test_settings_soxs_sim.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8515 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/test_settings_xsh.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3389 2023-03-03 13:31:12.000000 soxspipe-0.7.2/soxspipe/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-03-03 13:57:58.094334 soxspipe-0.7.2/soxspipe.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2532 2023-03-03 13:57:57.000000 soxspipe-0.7.2/soxspipe.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3744 2023-03-03 13:57:57.000000 soxspipe-0.7.2/soxspipe.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-03-03 13:57:57.000000 soxspipe-0.7.2/soxspipe.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       52 2023-03-03 13:57:57.000000 soxspipe-0.7.2/soxspipe.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-03-03 13:35:32.000000 soxspipe-0.7.2/soxspipe.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      150 2023-03-03 13:57:57.000000 soxspipe-0.7.2/soxspipe.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        9 2023-03-03 13:57:57.000000 soxspipe-0.7.2/soxspipe.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-11 19:20:31.039819 soxspipe-0.8.0/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      437 2023-05-11 18:42:34.000000 soxspipe-0.8.0/.readthedocs.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12276 2023-05-11 18:42:34.000000 soxspipe-0.8.0/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-05-11 18:42:34.000000 soxspipe-0.8.0/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      361 2023-05-11 18:42:34.000000 soxspipe-0.8.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2516 2023-05-11 19:20:31.039819 soxspipe-0.8.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1873 2023-05-11 18:42:34.000000 soxspipe-0.8.0/README.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-05-11 19:20:31.039819 soxspipe-0.8.0/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1775 2023-05-11 18:42:34.000000 soxspipe-0.8.0/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-11 19:20:30.431797 soxspipe-0.8.0/soxspipe/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      141 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      498 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/advanced_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8991 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-11 19:20:30.435798 soxspipe-0.8.0/soxspipe/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      743 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1151 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/combiner.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    62950 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/create_dispersion_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      135 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/data_organiser.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    51220 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/data_organiser.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    42382 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/detect_continuum.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    32317 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/detect_order_edges.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2932 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/detector_lookup.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3534 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/dispersion_map_to_pixel_arrays.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6484 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/filenamer.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/getpackagepath.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4422 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/keyword_lookup.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8665 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/polynomials.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    17809 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/set_of_files.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11869 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/subtract_background.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    68756 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/subtract_sky.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    29416 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/toolkit.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1421 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/commonutils/uncompress.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4829 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/default_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   110592 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/pandas_export.db
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-11 19:20:30.443798 soxspipe-0.8.0/soxspipe/recipes/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      416 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/recipes/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    46549 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/recipes/_base_recipe_.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10383 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/recipes/soxs_disp_solution.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13613 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/recipes/soxs_mbias.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7937 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/recipes/soxs_mdark.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    36475 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/recipes/soxs_mflat.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11649 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/recipes/soxs_order_centres.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12701 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/recipes/soxs_spatial_solution.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12377 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/recipes/soxs_stare.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6025 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/recipes/soxs_straighten.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-11 19:20:30.447798 soxspipe-0.8.0/soxspipe/resources/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2732 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/resources/soxs_detector_parameters.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      760 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/resources/soxs_keywords.yaml
+-rwxr-xr-x   0 jenkins   (1003) jenkins   (1004)    45056 2023-05-11 18:42:34.000000 soxspipe-0.8.0/soxspipe/resources/soxspipe.db
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-11 19:20:30.419797 soxspipe-0.8.0/soxspipe/resources/static_calibrations/
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-11 19:20:30.631805 soxspipe-0.8.0/soxspipe/resources/static_calibrations/soxs/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004) 33557761 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/soxs/BP_MAP_RP_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   155520 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/soxs/SOXS_PINHOLE_TAB_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   155520 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/soxs/SOXS_PINHOLE_TAB_NIR_OLD.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8640 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/soxs/SOXS_SPECTRAL_FORMAT_TAB_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    46080 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/soxs/skylines.fits
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-11 19:20:31.039819 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)  8674560 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004) 24629760 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x1.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004) 12340800 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)  6197760 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_2x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004) 32820480 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x1.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004) 16436160 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)  8245440 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_2x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    17280 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14400 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_UVB.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14400 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_VIS.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   169920 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   132480 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x1.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   132480 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   132480 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_2x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   167040 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x1.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   167040 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   167040 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_2x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    60480 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23040 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x1.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23040 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23040 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_2x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    28800 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x1.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    28800 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    28800 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_2x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    46080 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/skylines.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2713 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/xsh_detector_parameters.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9625 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/resources/xsh_keywords.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9670 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3268 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/test_settings_soxs.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3382 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/test_settings_soxs_sim.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8511 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/test_settings_xsh.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3389 2023-05-11 18:42:35.000000 soxspipe-0.8.0/soxspipe/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-11 19:20:30.431797 soxspipe-0.8.0/soxspipe.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2516 2023-05-11 19:20:30.000000 soxspipe-0.8.0/soxspipe.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3880 2023-05-11 19:20:30.000000 soxspipe-0.8.0/soxspipe.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-11 19:20:30.000000 soxspipe-0.8.0/soxspipe.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       52 2023-05-11 19:20:30.000000 soxspipe-0.8.0/soxspipe.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-11 18:45:58.000000 soxspipe-0.8.0/soxspipe.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      144 2023-05-11 19:20:30.000000 soxspipe-0.8.0/soxspipe.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        9 2023-05-11 19:20:30.000000 soxspipe-0.8.0/soxspipe.egg-info/top_level.txt
```

### Comparing `soxspipe-0.7.2/CHANGES.md` & `soxspipe-0.8.0/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 
 # Release Notes  
 
+## v0.8.0 - March 3, 2023
+
+* **FEATURE:** we now have a data-organiser to sort data, prepare the required SOF files and generate reduction scripts.
+* **ENHANCEMENT:** '.db', '.yaml', '.sh' and '.log' extensions skipped when moving items to the misc folder
+* **ENHANCEMENT:** move information printed to STDOUT when preparing a workspace to inform the user of how the data is organised
+* **ENHANCEMENT:** code can automatically adjust polynomial fitting parameters to find a dispersion solution if those provided in the settings file fail.
+* **ENHANCEMENT:** uncompression of fits.Z files (if any) occurs before data-organising
+* **REFACTOR:** speed & robustness improvements to dispersion solution to 2D image map conversion.
+* **REFACTOR:** much fast check for product existence so recipes are quickly skipped if they have already run.
+* **REFACTOR:** removed the `intermediate-data-root` setting renamed to a more accurate `workspace-root-dir`
+* **REFACTOR:** removed the `reduced-data-root` setting.
+* **REFACTOR:** updating all depreciated pandas commands so pipeline is now compatible with 1.X and 2.X versions of pandas 
+* **FIXED** pandas 1.X and pandas 2.X were doing different things when renaming columns in data-frames. Both 1.X and 2.X now work in the pipeline.
+
 ## v0.7.2 - March 3, 2023
 
 * **REFACTOR:** Big improvements on sky-subtraction  
 * **REFACTOR:** UV order-edge detection more robust  
 * **REFACTOR:** changed quickstart guide compress to gzipped tar  
 * **REFACTOR:** updated default settings to be more robust
```

### Comparing `soxspipe-0.7.2/LICENSE` & `soxspipe-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/PKG-INFO` & `soxspipe-0.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: soxspipe
-Version: 0.7.2
+Version: 0.8.0
 Summary: A python package and command-line tools to The data-reduction pipeline for the SOXS instrument
 Home-page: https://github.com/thespacedoctor/soxspipe
-Download-URL: https://github.com/thespacedoctor/soxspipe/archive/v0.7.2.zip
+Download-URL: https://github.com/thespacedoctor/soxspipe/archive/v0.8.0.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: MIT
 Keywords: soxs, eso, data, pipeline, spectra
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # soxspipe
 
 <!-- INFO BADGES -->  
@@ -34,11 +34,8 @@
 [![](https://img.shields.io/github/issues/thespacedoctor/soxspipe/type:%20bug?label=bug%20issues)](https://github.com/thespacedoctor/soxspipe/issues?q=is%3Aissue+is%3Aopen+label%3A%22type%3A+bug%22+)
 
 *The data-reduction pipeline for the SOXS instrument* (a python package with command-line tools).
 
 Documentation for soxspipe is hosted by [Read the Docs](https://soxspipe.readthedocs.io/en/master/) ([development version](https://soxspipe.readthedocs.io/en/develop/) and [master version](https://soxspipe.readthedocs.io/en/master/)). The code lives on [github](https://github.com/thespacedoctor/soxspipe). Please report any issues you find [here](https://github.com/thespacedoctor/soxspipe/issues).
 
 
-## Features
-
-*
```

### Comparing `soxspipe-0.7.2/README.md` & `soxspipe-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,11 +17,8 @@
 [![](https://img.shields.io/github/issues/thespacedoctor/soxspipe/type:%20bug?label=bug%20issues)](https://github.com/thespacedoctor/soxspipe/issues?q=is%3Aissue+is%3Aopen+label%3A%22type%3A+bug%22+)
 
 *The data-reduction pipeline for the SOXS instrument* (a python package with command-line tools).
 
 Documentation for soxspipe is hosted by [Read the Docs](https://soxspipe.readthedocs.io/en/master/) ([development version](https://soxspipe.readthedocs.io/en/develop/) and [master version](https://soxspipe.readthedocs.io/en/master/)). The code lives on [github](https://github.com/thespacedoctor/soxspipe). Please report any issues you find [here](https://github.com/thespacedoctor/soxspipe/issues).
 
 
-## Features
-
-*
```

### Comparing `soxspipe-0.7.2/setup.py` & `soxspipe-0.8.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,39 +21,31 @@
     'matplotlib',
     'numpy',
     'unicodecsv',
     'pandas',
     'tabulate',
     'bottleneck',
     'multiprocess',
-    'csaps',
     'jinja2'
 ]
 
 # READ THE DOCS SERVERS
 exists = os.path.exists("/home/docs/")
 if exists:
-    # install_requires = ['fundamentals']
-    c_exclude_list = ['healpy', 'astropy',
-                      'numpy', 'sherlock', 'wcsaxes', 'HMpTy', 'ligo-gracedb', 'reproject', 'ccdproc', 'scipy'],
-    for e in c_exclude_list:
-        try:
-            install_requires.remove(e)
-        except:
-            pass
+    install_requires = ['fundamentals']
 
 setup(name="soxspipe",
       version=__version__,
       description="A python package and command-line tools to The data-reduction pipeline for the SOXS instrument",
       long_description=readme(),
       long_description_content_type='text/markdown',
       classifiers=[
           'Development Status :: 4 - Beta',
           'License :: OSI Approved :: MIT License',
-          'Programming Language :: Python :: 3.7',
+          'Programming Language :: Python :: 3.9',
           'Topic :: Utilities',
       ],
       keywords=['soxs, eso, data, pipeline, spectra'],
       url='https://github.com/thespacedoctor/soxspipe',
       download_url='https://github.com/thespacedoctor/soxspipe/archive/v%(__version__)s.zip' % locals(
       ),
       author='David Young',
```

### Comparing `soxspipe-0.7.2/soxspipe/cl_utils.py` & `soxspipe-0.8.0/soxspipe/cl_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 #!/usr/bin/env python
 # encoding: utf-8
 """
 Documentation for soxspipe can be found here: http://soxspipe.readthedocs.org
 
 Usage:
     soxspipe init
+    soxspipe prep <workspaceDirectory>
     soxspipe [-Vx] mbias <inputFrames> [-o <outputDirectory> -s <pathToSettingsFile>] 
     soxspipe [-Vx] mdark <inputFrames> [-o <outputDirectory> -s <pathToSettingsFile>]
-    soxspipe [-Vx] mflat <inputFrames> [-o <outputDirectory> -s <pathToSettingsFile>]
     soxspipe [-Vx] disp_sol <inputFrames> [-o <outputDirectory> -s <pathToSettingsFile>]
     soxspipe [-Vx] order_centres <inputFrames> [-o <outputDirectory> -s <pathToSettingsFile>]
+    soxspipe [-Vx] mflat <inputFrames> [-o <outputDirectory> -s <pathToSettingsFile>]
     soxspipe [-Vx] spat_sol <inputFrames> [-o <outputDirectory> -s <pathToSettingsFile>]
     soxspipe [-Vx] stare <inputFrames> [-o <outputDirectory> -s <pathToSettingsFile>]
 
 Options:
     init                                   setup the soxspipe settings file for the first time
+    prep                                   prepare a folder of raw data (workspace) for data reduction
     mbias                                  the master bias recipe
     mdark                                  the master dark recipe
     mflat                                  the master flat recipe
     disp_sol                               the disp solution recipe
     order_centres                          the order centres recipe
     spat_sol                               the spatial solution recipe
     stare                                  reduce stare mode science frames
@@ -48,14 +50,27 @@
     return (glob.glob(text + '*') + [None])[state]
 
 
 def main(arguments=None):
     """
     *The main function used when `cl_utils.py` is run as a single script from the cl, or when installed as a cl command*
     """
+    # QUICKLY SKIP IF PRODUCT EXIST
+    if len(sys.argv[1:]) == 2:
+        if sys.argv[2].split(".")[-1].lower() == "sof":
+            sofName = os.path.basename(sys.argv[2]).replace(".sof", "")
+            if "_STARE_" in sofName:
+                sofName += "_SKYSUB"
+            productPath = "./product/soxs-" + sys.argv[1].replace("_", "-").replace("sol", "solution").replace("centres", "centre").replace("spat", "spatial") + "/" + sofName + ".fits"
+
+            productPath = productPath.replace("//", "/")
+            if os.path.exists(productPath):
+                print(f"The product of this recipe already exists at '{productPath}'. To overwrite this product, rerun the pipeline command with the overwrite flag (-x).")
+                sys.exit(0)
+
     # setup the command-line util settings
     su = tools(
         arguments=arguments,
         docString=__doc__,
         logLevel="ERROR",
         options_first=False,
         projectName="soxspipe",
@@ -123,15 +138,15 @@
             pickleMe[k] = theseLocals[k]
         pickle.dump(pickleMe, open(pathToPickleFile, "wb"))
 
     verbose = a['verboseFlag']
 
     # PACK UP SOME OF THE CL SWITCHES INTO SETTINGS DICTIONARY
     if a['outputDirectory']:
-        settings["intermediate-data-root"] = a['outputDirectory']
+        settings["workspace-root-dir"] = a['outputDirectory']
 
     if a["init"]:
         from os.path import expanduser
         home = expanduser("~")
         filepath = home + "/.config/soxspipe/soxspipe.yaml"
         try:
             cmd = """open %(filepath)s""" % locals()
@@ -216,14 +231,23 @@
             inputFrames=a["inputFrames"],
             verbose=verbose,
             overwrite=a["overwriteFlag"]
         )
 
         reducedStare = recipe.produce_product()
 
+    if a['prep']:
+        from soxspipe.commonutils import data_organiser
+        do = data_organiser(
+            log=log,
+            settings=settings,
+            rootDir=a["workspaceDirectory"]
+        )
+        do.prepare()
+
     # CALL FUNCTIONS/OBJECTS
 
     if "dbConn" in locals() and dbConn:
         dbConn.commit()
         dbConn.close()
     ## FINISH LOGGING ##
     endTime = times.get_now_sql_datetime()
@@ -231,8 +255,9 @@
     log.info('-- FINISHED ATTEMPT TO RUN THE cl_utils.py AT %s (RUNTIME: %s) --' %
              (endTime, runningTime, ))
 
     return
 
 
 if __name__ == '__main__':
+
     main()
```

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/__init__.py` & `soxspipe-0.8.0/soxspipe/commonutils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,7 +11,9 @@
 from . import polynomials
 from . import toolkit
 from .detect_order_edges import detect_order_edges
 from .filenamer import filenamer
 from .dispersion_map_to_pixel_arrays import dispersion_map_to_pixel_arrays
 from .subtract_background import subtract_background
 from .subtract_sky import subtract_sky
+from .data_organiser import data_organiser
+from .uncompress import uncompress
```

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/combiner.py` & `soxspipe-0.8.0/soxspipe/commonutils/combiner.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/create_dispersion_map.py` & `soxspipe-0.8.0/soxspipe/commonutils/create_dispersion_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,16 @@
         *generate the dispersion map*
 
         **Return:**
             - ``mapPath`` -- path to the file containing the coefficients of the x,y polynomials of the global dispersion map fit
         """
         self.log.debug('starting the ``get`` method')
 
+        import pandas as pd
+
         # WHICH RECIPE ARE WE WORKING WITH?
         if self.firstGuessMap:
             slitDeg = self.recipeSettings["slit-deg"]
         else:
             slitDeg = 0
 
         # READ PREDICTED LINE POSITIONS FROM FILE - RETURNED AS DATAFRAME
@@ -203,46 +205,61 @@
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
         if "DISP" in self.recipeName.upper():
             tag = "single"
         else:
             tag = "multi"
 
-        self.qc = self.qc.append({
+        self.qc = pd.concat([self.qc, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "qc_name": "NLINE",
             "qc_value": detectedLines,
             "qc_comment": f"[lines] Number of lines detected in {tag} pinhole frame",
             "qc_unit": "lines",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "to_header": True
-        }, ignore_index=True)
-        self.qc = self.qc.append({
+        }).to_frame().T], ignore_index=True)
+
+        self.qc = pd.concat([self.qc, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "qc_name": "PLINE",
             "qc_value": percentageDetectedLines,
             "qc_comment": f"Proportion of lines detected in {tag} pinhole frame",
             "qc_unit": None,
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "to_header": True
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         orderDeg = self.recipeSettings["order-deg"]
         wavelengthDeg = self.recipeSettings["wavelength-deg"]
 
         # ITERATIVELY FIT THE POLYNOMIAL SOLUTIONS TO THE DATA
-        popt_x, popt_y, res_plots = self.fit_polynomials(
-            orderPixelTable=orderPixelTable,
-            wavelengthDeg=wavelengthDeg,
-            orderDeg=orderDeg,
-            slitDeg=slitDeg,
-            missingLines=missingLines
-        )
+        fitFound = False
+        tryCount = 0
+        while not fitFound and tryCount < 5:
+            try:
+                popt_x, popt_y, res_plots = self.fit_polynomials(
+                    orderPixelTable=orderPixelTable,
+                    wavelengthDeg=wavelengthDeg,
+                    orderDeg=orderDeg,
+                    slitDeg=slitDeg,
+                    missingLines=missingLines
+                )
+                fitFound = True
+            except Exception as e:
+                degList = [wavelengthDeg, orderDeg, slitDeg]
+                degList[degList.index(max(degList))] -= 1
+                wavelengthDeg, orderDeg, slitDeg = degList
+                print(f"Wavelength, Order and Slit fitting orders reduced to {wavelengthDeg}, {orderDeg}, {slitDeg} to try and achieve a dispersion solution.")
+                tryCount += 1
+                if tryCount == 5:
+                    print(f"Could not converge on a good fit to the dispersion solution. Please check the quality of your data or adjust your fitting parameters.")
+                    raise e
 
         # WRITE THE MAP TO FILE
         mapPath = self.write_map_to_file(
             popt_x, popt_y, orderDeg, wavelengthDeg, slitDeg)
 
         if self.firstGuessMap and self.orderTable and self.create2DMap:
             mapImagePath = self.map_to_image(dispersionMapPath=mapPath)
@@ -504,15 +521,15 @@
             for j in range(0, wavelengthDeg + 1):
                 for k in range(0, slitDeg + 1):
                     coeff_dict_y[f'c{i}{j}{k}'] = ycoeff[n_coeff]
                     n_coeff += 1
 
         # DETERMINE WHERE TO WRITE THE FILE
         home = expanduser("~")
-        outDir = self.settings["intermediate-data-root"].replace("~", home)
+        outDir = self.settings["workspace-root-dir"].replace("~", home)
         outDir += f"product/{self.recipeName}/"
         outDir = outDir.replace("//", "/")
         # Recursively create missing directories
         if not os.path.exists(outDir):
             os.makedirs(outDir)
 
         if not self.sofName:
@@ -594,14 +611,15 @@
             - ``mean`` -- the mean of the combine residuals
             - ``std`` -- the stdev of the combine residuals
             - ``median`` -- the median of the combine residuals
         """
         self.log.debug('starting the ``calculate_residuals`` method')
 
         import numpy as np
+        import pandas as pd
 
         arm = self.arm
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
         # ADD EXPONENTS TO ORDERTABLE UP-FRONT
@@ -640,104 +658,104 @@
         combined_res_mean = np.mean(orderPixelTable["residuals_xy"])
         combined_res_std = np.std(orderPixelTable["residuals_xy"])
         combined_res_median = np.median(orderPixelTable["residuals_xy"])
 
         if writeQCs:
             absx = abs(orderPixelTable["residuals_x"])
             absy = abs(orderPixelTable["residuals_y"])
-            self.qc = self.qc.append({
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "XRESMIN",
                 "qc_value": absx.min(),
                 "qc_comment": "[px] Minimum residual in dispersion solution fit along x-axis",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "XRESMAX",
                 "qc_value": absx.max(),
                 "qc_comment": "[px] Maximum residual in dispersion solution fit along x-axis",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "XRESRMS",
                 "qc_value": absx.std(),
                 "qc_comment": "[px] Std-dev of residual in dispersion solution fit along x-axis",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "YRESMIN",
                 "qc_value": absy.min(),
                 "qc_comment": "[px] Minimum residual in dispersion solution fit along y-axis",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "YRESMAX",
                 "qc_value": absy.max(),
                 "qc_comment": "[px] Maximum residual in dispersion solution fit along y-axis",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "YRESRMS",
                 "qc_value": absy.std(),
                 "qc_comment": "[px] Std-dev of residual in dispersion solution fit along y-axis",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "XYRESMIN",
                 "qc_value": orderPixelTable["residuals_xy"].min(),
                 "qc_comment": "[px] Minimum residual in dispersion solution fit (XY combined)",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "XYRESMAX",
                 "qc_value": orderPixelTable["residuals_xy"].max(),
                 "qc_comment": "[px] Maximum residual in dispersion solution fit (XY combined)",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "XYRESRMS",
                 "qc_value": orderPixelTable["residuals_xy"].std(),
                 "qc_comment": "[px] Std-dev of residual in dispersion solution (XY combined)",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
+            }).to_frame().T], ignore_index=True)
 
         self.log.debug('completed the ``calculate_residuals`` method')
         return combined_res_mean, combined_res_std, combined_res_median, orderPixelTable
 
     def fit_polynomials(
             self,
             orderPixelTable,
@@ -1021,34 +1039,34 @@
             )
             res_plots = res_plots.replace(".fits", ".pdf")
         else:
             res_plots = self.sofName + "_RESIDUALS.pdf"
         # plt.show()
 
         home = expanduser("~")
-        outDir = self.settings["intermediate-data-root"].replace("~", home) + "/qc/pdf/"
+        outDir = self.settings["workspace-root-dir"].replace("~", home) + "/qc/pdf/"
         outDir = outDir.replace("//", "/")
         # RECURSIVELY CREATE MISSING DIRECTORIes
         if not os.path.exists(outDir):
             os.makedirs(outDir)
 
         if self.firstGuessMap:
             filePath = f"{outDir}/{res_plots}"
         else:
             filePath = f"{outDir}/{res_plots}"
-        self.products = self.products.append({
+        self.products = pd.concat([self.products, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "product_label": "DISP_MAP_RES",
             "file_name": res_plots,
             "file_type": "PDF",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "product_desc": f"{self.arm} dispersion solution QC plots",
             "file_path": filePath
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         plt.tight_layout()
         # plt.show()
         plt.savefig(filePath, dpi=720)
 
         self.log.debug('completed the ``fit_polynomials`` method')
         return xcoeff, ycoeff, res_plots
@@ -1198,16 +1216,25 @@
 
         combinedSlitImage = False
         combinedWlImage = False
 
         # DEFINE AN INPUT ARRAY
         inputArray = [(order, minWl, maxWl) for order, minWl,
                       maxWl in zip(orderNums, waveLengthMin, waveLengthMax)]
+
+        # NUMPY CAN BE TRICKY WITH MP
+        numThreads = '1'
+        os.environ['OPENBLAS_NUM_THREADS'] = numThreads
+        os.environ['OMP_NUM_THREADS'] = numThreads
+        os.environ['BLAS_NUM_THREADS'] = numThreads
         results = fmultiprocess(log=self.log, function=self.order_to_image,
-                                inputArray=inputArray, poolSize=False, timeout=3600, turnOffMP=False)
+                                inputArray=inputArray, poolSize=6, timeout=3600, turnOffMP=False)
+        del os.environ['OPENBLAS_NUM_THREADS']
+        del os.environ['OMP_NUM_THREADS']
+        del os.environ['BLAS_NUM_THREADS']
 
         slitImages = [r[0] for r in results]
         wlImages = [r[1] for r in results]
 
         slitMap, wlMap, orderMap = self.create_placeholder_images(reverse=True)
 
         combinedSlitImage = Combiner(slitImages)
@@ -1216,15 +1243,15 @@
         combinedWlImage = combinedWlImage.sum_combine()
 
         combinedWlImage.data += wlMap.data
         combinedSlitImage.data += wlMap.data
 
         # DETERMINE WHERE TO WRITE THE FILE
         home = expanduser("~")
-        outDir = self.settings["intermediate-data-root"].replace("~", home) + f"/product/{self.recipeName}"
+        outDir = self.settings["workspace-root-dir"].replace("~", home) + f"/product/{self.recipeName}"
         outDir = outDir.replace("//", "/")
         # Recursively create missing directories
         if not os.path.exists(outDir):
             os.makedirs(outDir)
 
         #
 
@@ -1306,23 +1333,23 @@
             # GENERATE THE ORDERPIXEL TABLE FROM WL AND SLIT-POSTION GRID .. IF WITHIN THRESHOLD OF CENTRE OF DETECTOR PIXEL THEN INJECT INTO MAPS
             orderPixelTable, remainingCount = self.convert_and_fit(
                 order=order, bigWlArray=bigWlArray, bigSlitArray=bigSlitArray, slitMap=slitMap, wlMap=wlMap, iteration=iteration, plots=False)
 
             if remainingCount < 3:
                 break
 
+            orderPixelTable = orderPixelTable.drop_duplicates(subset=['pixel_x', 'pixel_y', 'order'])
             train_wlx = orderPixelTable["fit_x"].values
             train_wly = orderPixelTable["fit_y"].values
             train_wl = orderPixelTable["wavelength"].values
             train_sp = orderPixelTable["slit_position"].values
-            g = orderPixelTable[['pixel_x', 'pixel_y', 'order']].drop_duplicates()
 
             # USE CUBIC SPLINE NEIGHEST NEIGHBOUR TO SEED RESULTS
-            bigWlArray = griddata((train_wlx, train_wly), train_wl, (g['pixel_x'].values, g['pixel_y'].values), method="cubic")
-            bigSlitArray = griddata((train_wlx, train_wly), train_sp, (g['pixel_x'].values, g['pixel_y'].values), method="cubic")
+            bigWlArray = griddata((train_wlx, train_wly), train_wl, (orderPixelTable['pixel_x'].values, orderPixelTable['pixel_y'].values), method="cubic")
+            bigSlitArray = griddata((train_wlx, train_wly), train_sp, (orderPixelTable['pixel_x'].values, orderPixelTable['pixel_y'].values), method="cubic")
 
         self.log.debug('completed the ``order_to_image`` method')
         return slitMap, wlMap
 
     def convert_and_fit(
             self,
             order,
@@ -1397,15 +1424,16 @@
         mask = (orderPixelTable['residual_xy'] <
                 self.map_to_image_displacement_threshold)
         # KEEP ONLY VALUES CLOSEST TO CENTRE OF PIXEL
         newPixelValue = orderPixelTable.loc[mask].drop_duplicates(
             subset=['pixel_x', 'pixel_y'], keep="first")
         # REMOVE PIXELS FOUND IN newPixelValue FROM orderPixelTable
         orderPixelTable = newPixelValue[['pixel_x', 'pixel_y']].merge(orderPixelTable, on=[
-            'pixel_x', 'pixel_y'], how='right', indicator=True).query('_merge == "right_only"').drop('_merge', 1)
+            'pixel_x', 'pixel_y'], how='right', indicator=True).query('_merge == "right_only"').drop(columns=['_merge'])
+
         remainingCount = orderPixelTable.drop_duplicates(
             subset=['pixel_x', 'pixel_y'], keep="first")
 
         # ADD FITTED PIXELS TO PLACE HOLDER IMAGES
         for xx, yy, wavelength, slit_position in zip(newPixelValue["pixel_x"].values.astype(int), newPixelValue["pixel_y"].values.astype(int), newPixelValue["wavelength"].values, newPixelValue["slit_position"].values):
             try:
                 wlMap.data[yy, xx] = np.where(
@@ -1414,15 +1442,16 @@
                     np.isnan(slitMap.data[yy, xx]), slit_position, slitMap.data[yy, xx])
             except (IndexError):
                 # PIXELS OUTSIDE OF DETECTOR EDGES - IGNORE
                 pass
 
         sys.stdout.write("\x1b[1A\x1b[2K")
         percentageFound = (1 - (np.count_nonzero(np.isnan(wlMap.data)) / np.count_nonzero(wlMap.data))) * 100
-        print(f"ORDER {order:02d}, iteration {iteration:02d}. {percentageFound:0.2f}% order pixels now fitted. Fit found for {len(newPixelValue.index)} new pixels, {len(remainingCount.index)} image pixel remain to be constrained ({np.count_nonzero(np.isnan(wlMap.data))} nans in place-holder image)")
+        print(f"ORDER {order:02d}, iteration {iteration:02d}. {percentageFound:0.2f}% order pixels now fitted.")
+        # print(f"ORDER {order:02d}, iteration {iteration:02d}. {percentageFound:0.2f}% order pixels now fitted. Fit found for {len(newPixelValue.index)} new pixels, {len(remainingCount.index)} image pixel remain to be constrained ({np.count_nonzero(np.isnan(wlMap.data))} nans in place-holder image)")
 
         if plots:
             from matplotlib import cm
             import matplotlib.pyplot as plt
             # PLOT CCDDATA OBJECT
             rotatedImg = slitMap.data
             if self.axisA == "x":
```

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/detect_continuum.py` & `soxspipe-0.8.0/soxspipe/commonutils/detect_continuum.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,14 +250,15 @@
             - ``std`` -- the stdev of the residuals
             - ``median`` -- the median of the residuals
             - ``xfit`` -- fitted x values
         """
         self.log.debug('starting the ``calculate_residuals`` method')
 
         import numpy as np
+        import pandas as pd
 
         arm = self.arm
 
         poly = chebyshev_order_xy_polynomials(
             log=self.log, axisBCol=axisBCol, orderCol=orderCol, orderDeg=self.orderDeg, axisBDeg=self.axisBDeg).poly
 
         # CALCULATE RESIDUALS BETWEEN GAUSSIAN PEAK LINE POSITIONS AND POLY
@@ -278,54 +279,54 @@
             utcnow = datetime.utcnow()
             utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
             tag = "continuum"
             if "order-centre" in self.recipeName.lower():
                 tag = "order centre"
 
-            self.qc = self.qc.append({
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "XRESMIN",
                 "qc_value": res.min(),
                 "qc_comment": f"[px] Minimum residual in {tag} fit along x-axis",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "XRESMAX",
                 "qc_value": res.max(),
                 "qc_comment": f"[px] Maximum residual in {tag} fit along x-axis",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "XRESRMS",
                 "qc_value": res_std,
                 "qc_comment": f"[px] Std-dev of residual {tag} fit along x-axis",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "NORDERS",
                 "qc_value": uniqueorders,
                 "qc_comment": f"Number of order centre traces found",
                 "qc_unit": None,
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
+            }).to_frame().T], ignore_index=True)
 
         self.log.debug('completed the ``calculate_residuals`` method')
         return res, res_mean, res_std, res_median, xfit
 
     def write_order_table_to_file(
             self,
             frame,
@@ -347,17 +348,17 @@
 
         arm = self.arm
         kw = self.kw
 
         # DETERMINE WHERE TO WRITE THE FILE
         home = expanduser("~")
         if self.binx > 1 or self.biny > 1:
-            outDir = self.settings["intermediate-data-root"] + "/tmp"
+            outDir = self.settings["workspace-root-dir"] + "/tmp"
         else:
-            outDir = self.settings["intermediate-data-root"].replace("~", home) + f"/product/{self.recipeName}"
+            outDir = self.settings["workspace-root-dir"].replace("~", home) + f"/product/{self.recipeName}"
             outDir = outDir.replace("//", "/")
         # Recursively create missing directories
         if not os.path.exists(outDir):
             os.makedirs(outDir)
 
         if not self.sofName:
             filename = filenamer(
@@ -613,24 +614,24 @@
 
         from datetime import datetime
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
         basename = os.path.basename(plotPath)
 
-        self.products = self.products.append({
+        self.products = pd.concat([self.products, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "product_label": "ORDER_CENTRES_RES",
             "file_name": basename,
             "file_type": "PDF",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "product_desc": f"Residuals of the order centre polynomial fit",
             "file_path": plotPath
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         mean_res = np.mean(np.abs(orderPixelTable[f'cont_{self.axisA}_fit_res'].values))
         std_res = np.std(np.abs(orderPixelTable[f'cont_{self.axisA}_fit_res'].values))
 
         # WRITE OUT THE FITS TO THE ORDER CENTRE TABLE
         order_table_path = self.write_order_table_to_file(
             frame=self.pinholeFlat, orderPolyTable=orderPolyTable, orderMetaTable=orderMetaTable)
@@ -972,39 +973,51 @@
 
         # PLOT THE FINAL RESULTS:
         plt.subplots_adjust(top=0.92)
         for o, c in zip(uniqueOrders, colors):
             mask = (orderPixelTable['order'] == o)
             bottomleft.scatter(orderPixelTable.loc[mask][f'cont_{self.axisA}'].values, orderPixelTable.loc[mask][
                 f'cont_{self.axisA}_fit_res'].values, alpha=0.2, s=1, c=c)
-            bottomleft.text(orderPixelTable.loc[mask][f'cont_{self.axisA}'].values[10], orderPixelTable.loc[mask][
-                f'cont_{self.axisA}_fit_res'].values[10], int(o), fontsize=8, c=c, verticalalignment='bottom')
+            if len(orderPixelTable.loc[mask].index) > 10:
+                labelIndex = 10
+            else:
+                labelIndex = 1
+            bottomleft.text(orderPixelTable.loc[mask][f'cont_{self.axisA}'].values[labelIndex], orderPixelTable.loc[mask][
+                f'cont_{self.axisA}_fit_res'].values[labelIndex], int(o), fontsize=8, c=c, verticalalignment='bottom')
         bottomleft.set_xlabel(f'{self.axisA} pixel position', fontsize=10)
         bottomleft.set_ylabel(f'{self.axisA} residual', fontsize=10)
         bottomleft.tick_params(axis='both', which='major', labelsize=9)
 
         # PLOT THE FINAL RESULTS:
         plt.subplots_adjust(top=0.92)
         for o, c in zip(uniqueOrders, colors):
             mask = (orderPixelTable['order'] == o)
             bottomright.scatter(orderPixelTable.loc[mask][f'cont_{self.axisB}'].values, orderPixelTable.loc[mask][
                 f'cont_{self.axisA}_fit_res'].values, alpha=0.2, s=1, c=c)
-            bottomright.text(orderPixelTable.loc[mask][f'cont_{self.axisB}'].values[10], orderPixelTable.loc[mask][
-                f'cont_{self.axisA}_fit_res'].values[10], int(o), fontsize=8, c=c, verticalalignment='bottom')
+            if len(orderPixelTable.loc[mask].index) > 10:
+                labelIndex = 10
+            else:
+                labelIndex = 1
+            bottomright.text(orderPixelTable.loc[mask][f'cont_{self.axisB}'].values[labelIndex], orderPixelTable.loc[mask][
+                f'cont_{self.axisA}_fit_res'].values[labelIndex], int(o), fontsize=8, c=c, verticalalignment='bottom')
 
         bottomright.set_xlabel(f'{self.axisB} pixel position', fontsize=10)
         bottomright.tick_params(axis='both', which='major', labelsize=9)
         # bottomright.set_ylabel('x residual')
         bottomright.set_yticklabels([])
 
         stdToFwhm = 2 * (2 * math.log(2))**0.5
         for o, c in zip(uniqueOrders, colors):
             mask = (orderPixelTable['order'] == o)
             fwhmaxis.scatter(orderPixelTable.loc[mask]['wavelength'].values, orderPixelTable.loc[mask]['stddev_fit'].values * stdToFwhm, alpha=0.2, s=1, c=c)
-            fwhmaxis.text(orderPixelTable.loc[mask]['wavelength'].values[10], orderPixelTable.loc[mask]['stddev_fit'].values[10] * stdToFwhm, int(o), fontsize=8, c=c, verticalalignment='bottom')
+            if len(orderPixelTable.loc[mask].index) > 10:
+                labelIndex = 10
+            else:
+                labelIndex = 1
+            fwhmaxis.text(orderPixelTable.loc[mask]['wavelength'].values[labelIndex], orderPixelTable.loc[mask]['stddev_fit'].values[labelIndex] * stdToFwhm, int(o), fontsize=8, c=c, verticalalignment='bottom')
         fwhmaxis.set_xlabel('wavelength (nm)', fontsize=10)
         fwhmaxis.set_ylabel('FWHM (pixels)', fontsize=10)
         fwhmaxis.set_ylim(0, orderPixelTable['stddev_fit'].max() * stdToFwhm)
 
         mean_res = np.mean(np.abs(orderPixelTable[f'cont_{self.axisA}_fit_res'].values))
         std_res = np.std(np.abs(orderPixelTable[f'cont_{self.axisA}_fit_res'].values))
 
@@ -1019,15 +1032,15 @@
                 settings=self.settings
             )
             filename = filename.split("FLAT")[0] + "ORDER_CENTRES_residuals.pdf"
         else:
             filename = self.sofName + "_residuals.pdf"
 
         home = expanduser("~")
-        outDir = self.settings["intermediate-data-root"].replace("~", home) + "/qc/pdf"
+        outDir = self.settings["workspace-root-dir"].replace("~", home) + "/qc/pdf"
         outDir = outDir.replace("//", "/")
         # Recursively create missing directories
         if not os.path.exists(outDir):
             os.makedirs(outDir)
 
         filePath = f"{outDir}/{filename}"
         plt.tight_layout()
```

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/detect_order_edges.py` & `soxspipe-0.8.0/soxspipe/commonutils/detect_order_edges.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,65 +307,65 @@
         plotName = os.path.basename(plotPath)
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
         # RECORD PRODUCTS AND QCs
         if not isinstance(self.products, bool):
-            self.products = self.products.append({
+            self.products = pd.concat([self.products, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "product_label": f"ORDER_LOC{self.tag}",
                 "product_desc": "table of coefficients from polynomial fits to order locations",
                 "file_name": orderTableName,
                 "file_type": "FITS",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "file_path": orderTablePath
-            }, ignore_index=True)
-            self.products = self.products.append({
+            }).to_frame().T], ignore_index=True)
+            self.products = pd.concat([self.products, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "product_label": f"ORDER_LOC_RES{self.tag}",
                 "product_desc": "visualisation of goodness of order edge fitting",
                 "file_name": plotName,
                 "file_type": "PDF",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "file_path": plotPath
-            }, ignore_index=True)
+            }).to_frame().T], ignore_index=True)
         if not isinstance(self.qc, bool):
-            self.qc = self.qc.append({
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "XRESMIN",
                 "qc_value": min_res,
                 "qc_comment": "[px] Minimum residual in order edge fit along x-axis",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "XRESMAX",
                 "qc_value": max_res,
                 "qc_comment": "[px] Maximum residual in order edge fit along x-axis",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
-            self.qc = self.qc.append({
+            }).to_frame().T], ignore_index=True)
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "XRESRMS",
                 "qc_value": std_res,
                 "qc_comment": "[px] Std-dev of residual order edge fit along x-axis",
                 "qc_unit": "pixels",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
+            }).to_frame().T], ignore_index=True)
 
         self.log.debug('completed the ``get`` method')
 
         return self.products, self.qc, orderDetectionCounts
 
     def plot_results(
             self,
@@ -572,15 +572,15 @@
         filename = filenamer(
             log=self.log,
             frame=self.flatFrame,
             settings=self.settings
         )
         filename = filename.split("SLIT")[0] + "ORDER_EDGES_residuals.pdf"
         home = expanduser("~")
-        outDir = self.settings["intermediate-data-root"].replace("~", home) + "/qc/pdf"
+        outDir = self.settings["workspace-root-dir"].replace("~", home) + "/qc/pdf"
         filePath = f"{outDir}/{filename}"
         plt.tight_layout()
         # plt.show()
         plt.savefig(filePath, dpi=720)
 
         self.log.debug('completed the ``plot_results`` method')
         return filePath
```

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/detector_lookup.py` & `soxspipe-0.8.0/soxspipe/commonutils/detector_lookup.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/dispersion_map_to_pixel_arrays.py` & `soxspipe-0.8.0/soxspipe/commonutils/dispersion_map_to_pixel_arrays.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/filenamer.py` & `soxspipe-0.8.0/soxspipe/commonutils/filenamer.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/keyword_lookup.py` & `soxspipe-0.8.0/soxspipe/commonutils/keyword_lookup.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/polynomials.py` & `soxspipe-0.8.0/soxspipe/commonutils/polynomials.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/set_of_files.py` & `soxspipe-0.8.0/soxspipe/commonutils/set_of_files.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/subtract_background.py` & `soxspipe-0.8.0/soxspipe/commonutils/subtract_background.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/subtract_sky.py` & `soxspipe-0.8.0/soxspipe/commonutils/subtract_sky.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
             imageMapOrders.append(self.mapDF[self.mapDF["order"] == o])
 
         # NOTE MULTIPROCESSING THIS BLOCK RESULTS IN SLOWER PERFORMANCE
         for o in uniqueOrders:
             # SELECT ONLY A DATAFRAME CONTAINING ONLY A SINGLE ORDER
             imageMapOrder = self.mapDF[self.mapDF["order"] == o]
             # MASK OUTLYING PIXELS (imageMapOrderWithObject) AND ALSO THEN THE OBJECT PIXELS (imageMapOrderSkyOnly)
-            imageMapOrderWithObject, imageMapOrderSkyOnly = self.get_over_sampled_sky_from_order(imageMapOrder, clipBPs=False, clipSlitEdge=self.settings["sky-subtraction"]["clip-slit-edge-fraction"])
+            imageMapOrderWithObject, imageMapOrderSkyOnly = self.get_over_sampled_sky_from_order(imageMapOrder, clipBPs=True, clipSlitEdge=self.settings["sky-subtraction"]["clip-slit-edge-fraction"])
             allimageMapOrder.append(imageMapOrderSkyOnly)
             allimageMapOrderWithObject.append(imageMapOrderWithObject)
 
         # MASK OUT OBJECT PIXELS
         allimageMapOrder = self.clip_object_slit_positions(allimageMapOrder, aggressive=self.settings["sky-subtraction"]["aggressive_object_masking"])
 
         print(f"\n  ## FITTING SKY-FLUX WITH A BSPLINE (WAVELENGTH) AND LOW-ORDER POLY (SLIT-ILLUMINATION PROFILE)\n")
@@ -211,87 +211,87 @@
         for o, imageMapOrderSkyOnly, imageMapOrderWithObject in zip(uniqueOrders, allimageMapOrder, allimageMapOrderWithObject):
             if isinstance(imageMapOrderSkyOnly, pd.core.frame.DataFrame):
                 # INJECT THE PIXEL VALUES BACK INTO THE PLACEHOLDER IMAGES
                 skymodelCCDData, skySubtractedCCDData = self.add_data_to_placeholder_images(imageMapOrderSkyOnly, skymodelCCDData, skySubtractedCCDData)
                 if o == qcPlotOrder:
                     qc_plot_path = self.plot_sky_sampling(order=o, imageMapOrderWithObjectDF=imageMapOrderWithObject, imageMapOrderDF=imageMapOrderSkyOnly, tck=qctck, knotLocations=qcknots)
                     basename = os.path.basename(qc_plot_path)
-                    self.products = self.products.append({
+                    self.products = pd.concat([self.products, pd.Series({
                         "soxspipe_recipe": "soxs-stare",
                         "product_label": "SKY_MODEL_QC_PLOTS",
                         "file_name": basename,
                         "file_type": "PDF",
                         "obs_date_utc": self.dateObs,
                         "reduction_date_utc": utcnow,
                         "product_desc": f"QC plots for the sky-background modelling",
                         "file_path": qc_plot_path
-                    }, ignore_index=True)
+                    }).to_frame().T], ignore_index=True)
 
         filename = self.filenameTemplate.replace(".fits", "_SKYMODEL.fits")
         home = expanduser("~")
-        outDir = self.settings["intermediate-data-root"].replace("~", home) + f"/product/{self.recipeName}"
+        outDir = self.settings["workspace-root-dir"].replace("~", home) + f"/product/{self.recipeName}"
         outDir = outDir.replace("//", "/")
         # RECURSIVELY CREATE MISSING DIRECTORIES
         if not os.path.exists(outDir):
             os.makedirs(outDir)
 
         filePath = f"{outDir}/{filename}"
-        self.products = self.products.append({
+        self.products = pd.concat([self.products, pd.Series({
             "soxspipe_recipe": "soxs-stare",
             "product_label": "SKY_MODEL",
             "file_name": filename,
             "file_type": "FITS",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "product_desc": f"The sky background model",
             "file_path": filePath
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         # WRITE CCDDATA OBJECT TO FILE
         HDUList = skymodelCCDData.to_hdu(
             hdu_mask='QUAL', hdu_uncertainty='ERRS', hdu_flags=None)
         HDUList[0].name = "FLUX"
         HDUList.writeto(filePath, output_verify='exception',
                         overwrite=True, checksum=True)
 
         filename = self.filenameTemplate.replace(".fits", "_SKYSUB.fits")
         home = expanduser("~")
-        outDir = self.settings["intermediate-data-root"].replace("~", home) + f"/product/{self.recipeName}"
+        outDir = self.settings["workspace-root-dir"].replace("~", home) + f"/product/{self.recipeName}"
         filePath = f"{outDir}/{filename}"
-        self.products = self.products.append({
+        self.products = pd.concat([self.products, pd.Series({
             "soxspipe_recipe": "soxs-stare",
             "product_label": "SKY_SUBTRACTED_OBJECT",
             "file_name": filename,
             "file_type": "FITS",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "product_desc": f"The sky-subtracted object",
             "file_path": filePath
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         # WRITE CCDDATA OBJECT TO FILE
         HDUList = skySubtractedCCDData.to_hdu(
             hdu_mask='QUAL', hdu_uncertainty='ERRS', hdu_flags=None)
         HDUList[0].name = "FLUX"
         HDUList.writeto(filePath, output_verify='exception',
                         overwrite=True, checksum=True)
 
         comparisonPdf = self.plot_image_comparison(self.objectFrame, skymodelCCDData, skySubtractedCCDData)
 
         filename = os.path.basename(comparisonPdf)
-        self.products = self.products.append({
+        self.products = pd.concat([self.products, pd.Series({
             "soxspipe_recipe": "soxs-stare",
             "product_label": "SKY SUBTRACTION QUICKLOOK",
             "file_name": filename,
             "file_type": "PDF",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "product_desc": f"Sky-subtraction quicklook",
             "file_path": comparisonPdf
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         self.log.debug('completed the ``get`` method')
         return skymodelCCDData, skySubtractedCCDData, self.qc, self.products
 
     def get_over_sampled_sky_from_order(
             self,
             imageMapOrder,
@@ -451,30 +451,30 @@
         vmax = mean + 2 * std
         vmin = mean - 1 * std
         im = onerow.imshow(rotatedImg, vmin=0, vmax=100, cmap='gray', alpha=1)
         medianValue = np.median(rotatedImg.data.ravel())
         color = im.cmap(im.norm(medianValue))
         patches = [mpatches.Patch(color=color, label="unprocessed frame")]
 
-        onerow.set_title("Object & Sky Frame")
+        onerow.set_title("Object & Sky Frame", fontsize=10)
         onerow.set_xlabel(
             "y-axis", fontsize=10)
         onerow.set_ylabel(
             "x-axis", fontsize=10)
         ylimMinImage = imageMapOrderWithObjectDF["y"].min() - 10
         ylimMaxImage = imageMapOrderWithObjectDF["y"].max() + 10
         onerow.set_ylim(imageMapOrderWithObjectDF["x"].min() - 10, imageMapOrderWithObjectDF["x"].max() + 10)
         onerow.set_xlim(ylimMinImage, ylimMaxImage)
         onerow.invert_xaxis()
 
         # ORIGINAL DATA AND PERCENTILE SMOOTHED WAVELENGTH VS FLUX
         tworow.plot(
             imageMapOrderWithObjectDF["wavelength"].values,
             imageMapOrderWithObjectDF["flux"].values, label='unprocessed', alpha=0.2, c=grey, zorder=0)
-        tworow.set_title("STEP 1. Identify and clip outlying pixels (CRHs etc) and pixels containing object flux.")
+        tworow.set_title("STEP 1. Identify and clip outlying pixels (CRHs etc) and pixels containing object flux.", fontsize=10)
         # RAW MARKERS
         tworow.scatter(
             imageMapOrderDF.loc[imageMapOrderDF["clipped"] == False, "wavelength"].values,
             imageMapOrderDF.loc[imageMapOrderDF["clipped"] == False, "flux"].values, label='unclipped', s=rawMS, c=black, alpha=1., zorder=unclippedZ)
         # ROBUSTLY CLIPPED
         tworow.scatter(
             imageMapOrderDF.loc[imageMapOrderDF["clipped"] == True, "wavelength"].values,
@@ -555,15 +555,15 @@
         fiverow.set_ylabel(
             "x-axis", fontsize=10)
         fiverow.set_ylim(imageMapOrderWithObjectDF["x"].min() - 10, imageMapOrderWithObjectDF["x"].max() + 10)
         fiverow.set_xlim(ylimMinImage, ylimMaxImage)
         fiverow.invert_xaxis()
 
         # PLOT WAVELENGTH VS FLUX SKY MODEL
-        sixrow.set_title("STEP 2. Fit a univariate bspline to sky-flux as a function of wavelength")
+        sixrow.set_title("STEP 2. Fit a univariate bspline to sky-flux as a function of wavelength", fontsize=10)
         sixrow.scatter(
             imageMapOrderDF.loc[imageMapOrderDF["clipped"] == False, "wavelength"].values,
             imageMapOrderDF.loc[imageMapOrderDF["clipped"] == False, "flux"].values, s=medianMS, c=black, alpha=0.5, zorder=unclippedZ)
 
         if tck:
             wl = np.linspace(imageMapOrderDF["wavelength"].min(), imageMapOrderDF["wavelength"].max(), 1000000)
             sky = ip.splev(wl, tck)
@@ -613,15 +613,15 @@
         skySubImage = np.ma.array(skySubImage, mask=skySubMask)
         cmap = copy(cm.gray)
         std = np.nanstd(skySubImage)
         mean = np.nanmedian(skySubImage)
         vmax = mean + 0.2 * std
         vmin = mean - 0.2 * std
         im = eightrow.imshow(np.flipud(np.rot90(skySubImage, 1)), vmin=0, vmax=50, cmap=cmap, alpha=1.)
-        eightrow.set_title("STEP 3. Subtract the sky-model from the original data.")
+        eightrow.set_title("STEP 3. Subtract the sky-model from the original data.", fontsize=10)
         eightrow.set_xlabel(
             "y-axis", fontsize=10)
         eightrow.set_ylabel(
             "x-axis", fontsize=10)
         eightrow.set_ylim(imageMapOrderWithObjectDF["x"].min() - 10, imageMapOrderWithObjectDF["x"].max() + 10)
         eightrow.set_xlim(ylimMinImage, ylimMaxImage)
         eightrow.invert_xaxis()
@@ -657,15 +657,15 @@
             "wavelength (nm)", fontsize=10)
         tenrow.set_ylabel("residual/noise", fontsize=10)
 
         fig.suptitle(f"{self.arm} sky model: order {order}", fontsize=12, y=0.97)
 
         filename = self.filenameTemplate.replace(".fits", f"_SKYMODEL_QC_PLOTS_ORDER_{int(order)}.pdf")
         home = expanduser("~")
-        outDir = self.settings["intermediate-data-root"].replace("~", home) + "/qc/pdf"
+        outDir = self.settings["workspace-root-dir"].replace("~", home) + "/qc/pdf"
         filePath = f"{outDir}/{filename}"
 
         # plt.show()
         plt.savefig(filePath, dpi='figure')
 
         self.log.debug('completed the ``plot_sky_sampling`` method')
         return filePath
@@ -843,14 +843,21 @@
                 extraKnots = np.ma.compressed(np.ma.masked_array(potentialNewKnots, mask))
                 meanResiduals = np.ma.compressed(np.ma.masked_array(meanResiduals, mask))
                 allKnots = np.sort(np.concatenate((extraKnots, allKnots)))
 
             tck, fp, ier, msg = ip.splrep(goodWl, goodFlux, t=allKnots, k=bspline_order, w=goodWeights, full_output=True)
             t, c, k = tck
 
+            if ier == 10:
+                print(f"\t\tpoor fit on iteration {iterationCount} for order {imageMapOrder['order'].values[0]}. Reverting to last iteration.\n")
+                tck = tck_previous
+                break
+            else:
+                tck_previous = tck
+
             # GENERATE SKY-MODEL FROM BSPLINE
             imageMapOrder["sky_model"] = ip.splev(imageMapOrder["wavelength"].values, tck)
             imageMapOrder["sky_subtracted_flux"] = imageMapOrder["flux"] - imageMapOrder["sky_model"] * imageMapOrder['flux_normaliser']
             imageMapOrder["sky_subtracted_flux_error_ratio"] = imageMapOrder["sky_subtracted_flux"] / imageMapOrder["error"]
             imageMapOrder["sky_subtracted_flux_error_ratio_abs"] = imageMapOrder["sky_subtracted_flux_error_ratio"].abs()
 
             if iterationCount <= residualFloorIterationLimit:
@@ -1022,15 +1029,15 @@
         # subtitle = f"mean res: {mean_res:2.2f} pix, res stdev: {std_res:2.2f}"
         # fig.suptitle(f"traces of order-centre locations - pinhole flat-frame\n{subtitle}", fontsize=12)
 
         # plt.show()
         filename = self.filenameTemplate.replace(".fits", "_skysub_quicklook.pdf")
 
         home = expanduser("~")
-        outDir = self.settings["intermediate-data-root"].replace("~", home) + "/qc/pdf"
+        outDir = self.settings["workspace-root-dir"].replace("~", home) + "/qc/pdf"
         filePath = f"{outDir}/{filename}"
         plt.savefig(filePath, dpi=720)
 
         self.log.debug('completed the ``plot_results`` method')
         return filePath
 
     def rectify_order(
```

### Comparing `soxspipe-0.7.2/soxspipe/commonutils/toolkit.py` & `soxspipe-0.8.0/soxspipe/commonutils/toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -534,14 +534,15 @@
     ```python
     usage code
     ```
     """
     log.debug('starting the ``functionName`` function')
 
     import numpy as np
+    import pandas as pd
 
     # KEYWORD LOOKUP OBJECT - LOOKUP KEYWORD FROM DICTIONARY IN RESOURCES
     # FOLDER
     kw = keyword_lookup(
         log=log,
         settings=settings
     ).get
@@ -550,52 +551,52 @@
     dateObs = frame.header[kw("DATE_OBS")]
 
     nanCount = np.count_nonzero(np.isnan(frame.data))
 
     utcnow = datetime.utcnow()
     utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
-    qcTable = qcTable.append({
+    qcTable = pd.concat([qcTable, pd.Series({
         "soxspipe_recipe": recipeName,
         "qc_name": "N NAN PIXELS",
         "qc_value": nanCount,
         "qc_comment": "Number of NaN pixels",
         "qc_unit": "",
         "obs_date_utc": dateObs,
         "reduction_date_utc": utcnow,
         "to_header": False
-    }, ignore_index=True)
+    }).to_frame().T], ignore_index=True)
 
     # COUNT BAD-PIXELS
     badCount = frame.mask.sum()
     totalPixels = np.size(frame.mask)
     percent = (float(badCount) / float(totalPixels))
     percent = float("{:.6f}".format(percent))
 
-    qcTable = qcTable.append({
+    qcTable = pd.concat([qcTable, pd.Series({
         "soxspipe_recipe": recipeName,
         "qc_name": "N BAD PIXELS",
         "qc_value": int(badCount),
         "qc_comment": "Number of bad pixels",
         "qc_unit": "",
         "obs_date_utc": dateObs,
         "reduction_date_utc": utcnow,
         "to_header": True
-    }, ignore_index=True)
+    }).to_frame().T], ignore_index=True)
 
-    qcTable = qcTable.append({
+    qcTable = pd.concat([qcTable, pd.Series({
         "soxspipe_recipe": recipeName,
         "qc_name": "FRAC BAD PIXELS",
         "qc_value": percent,
         "qc_comment": "Fraction of bad pixels",
         "qc_unit": "",
         "obs_date_utc": dateObs,
         "reduction_date_utc": utcnow,
         "to_header": True
-    }, ignore_index=True)
+    }).to_frame().T], ignore_index=True)
 
     log.debug('completed the ``functionName`` function')
     return qcTable
 
 
 def spectroscopic_image_quality_checks(
         log,
@@ -628,14 +629,15 @@
     usage code
     ```
     """
     log.debug('starting the ``functionName`` function')
 
     import numpy.ma as ma
     import numpy as np
+    import pandas as pd
 
     # KEYWORD LOOKUP OBJECT - LOOKUP KEYWORD FROM DICTIONARY IN RESOURCES
     # FOLDER
     kw = keyword_lookup(
         log=log,
         settings=settings
     ).get
@@ -685,35 +687,35 @@
 
     mean = np.ma.mean(maskedFrame)
     flux = np.ma.sum(maskedFrame)
 
     utcnow = datetime.utcnow()
     utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
-    qcTable = qcTable.append({
+    qcTable = pd.concat([qcTable, pd.Series({
         "soxspipe_recipe": recipeName,
         "qc_name": "INNER ORDER PIX MEAN",
         "qc_value": mean,
         "qc_comment": "[e-] Mean inner-order pixel value",
         "qc_unit": "electrons",
         "obs_date_utc": dateObs,
         "reduction_date_utc": utcnow,
         "to_header": True
-    }, ignore_index=True)
+    }).to_frame().T], ignore_index=True)
 
-    qcTable = qcTable.append({
+    qcTable = pd.concat([qcTable, pd.Series({
         "soxspipe_recipe": recipeName,
         "qc_name": "INNER ORDER PIX SUM",
         "qc_value": flux,
         "qc_comment": "[e-] Sum of all inner-order pixel values",
         "qc_unit": "electrons",
         "obs_date_utc": dateObs,
         "reduction_date_utc": utcnow,
         "to_header": True
-    }, ignore_index=True)
+    }).to_frame().T], ignore_index=True)
 
     log.debug('completed the ``functionName`` function')
     return qcTable
 
 
 def read_spectral_format(
         log,
```

### Comparing `soxspipe-0.7.2/soxspipe/default_settings.yaml` & `soxspipe-0.8.0/soxspipe/default_settings.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 version: 1
 
-
-intermediate-data-root: ~/Desktop/soxspipe/intermediate
-reduced-data-root: ~/Desktop/soxspipe/reduced
-
 # INTERMEDIATE DATA PRODUCTS CAN CONSUME A LOT OF STORAGE SPACE - BE WARNED
 save-intermediate-products: False
 
 # instrument the data belongs to; `xsh` or `soxs`
 instrument: xsh
 data-extension: 0
 
@@ -25,14 +21,15 @@
     clipping-upper-sigma: 3   
     clipping-iteration-count: 5
 
 soxs-disp-solution:
     pixel-window-size: 10
     order-deg: 3
     wavelength-deg: 3
+    # number of sigma-clipping iterations to perform before settings on a polynomial fit for the dispersion solution
     poly-clipping-iteration-limit: 10
     poly-fitting-residual-clipping-sigma: 5
 
 soxs-order-centre:
     # NUMBER OF CROSS-ORDER SLICES PER ORDER
     order-sample-count: 200
     # LENGTH OF EACH SLICE (PIXELS)
@@ -44,47 +41,41 @@
     # DEGREE OF ORDER-COMPONENT OF GLOBAL POLYNOMIAL FIT TO ORDER CENTRES
     order-deg: 5
     # CLIPPING LIMIT (MEDIAN AND MAD) WHEN FITTING GLOBAL POLYNOMIAL TO ORDER CENTRES
     poly-fitting-residual-clipping-sigma: 3
     # MAXIMUM NUMBER OF CLIPPING ITERATIONS WHEN FITTING GLOBAL POLYNOMIAL TO ORDER CENTRES
     poly-clipping-iteration-limit: 7
 
-soxs-spatial-solution:
-    pixel-window-size: 10
-    order-deg: 5
-    wavelength-deg: 4
-    slit-deg: 2
-    # number of sigma-clipping iterations to perform before settings on a polynomial fit for the dispersion solution
-    poly-clipping-iteration-limit: 9
-    poly-fitting-residual-clipping-sigma: 5
-    map_to_image_displacement_threshold: 0.01 # in pixels
-
 soxs-mflat:
     centre-order-window: 20
     stacked-clipping-sigma: 5
     stacked-clipping-iterations: 5
     clipping-lower-sigma: 50
     clipping-upper-sigma: 1000   
     clipping-iteration-count: 1
     slice-length-for-edge-detection: 90
     slice-width-for-edge-detection: 5
     min-percentage-threshold-for-edge-detection: 20
     max-percentage-threshold-for-edge-detection: 50
-    disp-axis-deg: 5
-    order-deg: 3
+    disp-axis-deg: 2
+    order-deg: 5
     poly-fitting-residual-clipping-sigma: 5
-    poly-clipping-iteration-limit: 3
+    poly-clipping-iteration-limit: 5
     low-sensitivity-clipping-sigma: 2
-    
-soxs-stare:
-    stacked-clipping-sigma: 5
-    stacked-clipping-iterations: 5
-    clipping-iteration-count: 1
-    clipping-lower-sigma: 50
-    clipping-upper-sigma: 1000 
+
+soxs-spatial-solution:
+    pixel-window-size: 10
+    order-deg: 5
+    wavelength-deg: 4
+    slit-deg: 2
+    # number of sigma-clipping iterations to perform before settings on a polynomial fit for the dispersion solution
+    poly-clipping-iteration-limit: 9
+    poly-fitting-residual-clipping-sigma: 5
+    map_to_image_displacement_threshold: 0.01 # in pixels
+
 
 sky-subtraction:
     # MEDIAN CLIPPING FIRST USED TO CLIP MOST DEVIANT PIXELS (BAD AND CRHs)
     median_clipping_sigma: 3
     median_clipping_iterations: 5
     # ROLLING WINDOW LENGTH IN DATA POINTS
     median_rolling_window_size: 31
@@ -94,19 +85,28 @@
     percential_rolling_window_size: 15
     # FRACTION OF SLIT RANGE TO MASK AT UPPER AND LOWER SLIT EDGES
     clip-slit-edge-fraction: 0.05
     aggressive_object_masking: True
     bspline_order: 3
     slit_illumination_order: 3
 
+soxs-stare:
+    stacked-clipping-sigma: 5
+    stacked-clipping-iterations: 5
+    clipping-iteration-count: 1
+    clipping-lower-sigma: 50
+    clipping-upper-sigma: 1000 
+
 # UTILS
 background-subtraction:
     bspline-deg: 3
     median-filter-pixels: 9
 
+
+
 logging settings:
     formatters:
         file_style:
             format: '* %(asctime)s - %(name)s - %(levelname)s (%(pathname)s > %(funcName)s > %(lineno)d) - %(message)s  '
             datefmt: '%Y/%m/%d %H:%M:%S'
         console_style:
             format: '* %(asctime)s - %(levelname)s: %(pathname)s:%(funcName)s:%(lineno)d > %(message)s'
```

### Comparing `soxspipe-0.7.2/soxspipe/recipes/_base_recipe_.py` & `soxspipe-0.8.0/soxspipe/recipes/_base_recipe_.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,23 +62,21 @@
         self.log = log
 
         import pandas as pd
 
         log.debug("instansiating a new '__init__' object")
         self.recipeName = recipeName
         self.settings = settings
-        self.intermediateRootPath = self._absolute_path(
-            settings["intermediate-data-root"])
-        self.reducedRootPath = self._absolute_path(
-            settings["reduced-data-root"])
+        self.workspaceRootPath = self._absolute_path(
+            settings["workspace-root-dir"])
 
         # CHECK IF PRODUCT ALREADY EXISTS
         if inputFrames and not isinstance(inputFrames, list) and inputFrames.split(".")[-1].lower() == "sof":
             self.sofName = os.path.basename(inputFrames).replace(".sof", "")
-            productPath = self.intermediateRootPath + "/product/" + self.recipeName + "/" + self.sofName + ".fits"
+            productPath = self.workspaceRootPath + "/product/" + self.recipeName + "/" + self.sofName + ".fits"
             self.productPath = productPath.replace("//", "/")
             if os.path.exists(self.productPath) and not overwrite:
                 print(f"The product of this recipe already exists at '{self.productPath}'. To overwrite this product, rerun the pipeline command with the overwrite flag (-x).")
                 sys.exit(0)
         else:
             self.sofName = False
             self.productPath = False
@@ -269,17 +267,17 @@
             arr = np.frombuffer(boolMask, dtype=np.uint8)
             arr.shape = (frame.data.shape)
             boolMask = arr
 
         frame.mask = boolMask
 
         if save:
-            outDir = self.intermediateRootPath
+            outDir = self.workspaceRootPath
         else:
-            outDir = self.intermediateRootPath + "/tmp"
+            outDir = self.workspaceRootPath + "/tmp"
 
         # INJECT THE PRE KEYWORD
         utcnow = datetime.utcnow()
         frame.header["SXSPRE"] = (utcnow.strftime(
             "%Y-%m-%dT%H:%M:%S.%f"), "UTC timestamp")
 
         # RECURSIVELY CREATE MISSING DIRECTORIES
@@ -400,14 +398,16 @@
 
         from astropy import units as u
 
         kw = self.kw
 
         # CHECK WE ACTUALLY HAVE IMAGES
         if not len(self.inputFrames.files_filtered(include_path=True)):
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             raise FileNotFoundError(
                 "No image frames where passed to the recipe")
 
         arm = self.inputFrames.values(
             keyword=kw("SEQ_ARM"), unique=True)
 
         inst = self.inputFrames.values(kw("INSTRUME"), unique=True)
@@ -422,14 +422,16 @@
         elif self.inst == "XSHOOTER":
             self.axisA = "x"
             self.axisB = "y"
 
         # MIXED INPUT ARMS ARE BAD
         if len(arm) > 1:
             arms = " and ".join(arm)
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             print(self.inputFrames.summary)
             raise TypeError(
                 "Input frames are a mix of %(imageTypes)s" % locals())
         else:
             self.arm = arm[0]
 
         # CREATE DETECTOR LOOKUP DICTIONARY - SOME VALUES CAN BE OVERWRITTEN
@@ -452,28 +454,32 @@
             try:
                 cdelt1.remove(None)
                 cdelt2.remove(None)
             except:
                 pass
 
         if len(cdelt1) > 1 or len(cdelt2) > 1:
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             raise TypeError(
                 "Input frames are a mix of binnings" % locals())
 
         if cdelt1[0] and cdelt2[0]:
             self.detectorParams["binning"] = [int(cdelt2[0]), int(cdelt1[0])]
 
         # MIXED READOUT SPEEDS IS BAD
         readSpeed = self.inputFrames.values(
             keyword=kw("DET_READ_SPEED"), unique=True)
 
         with suppress(ValueError):
             readSpeed.remove(None)
 
         if len(readSpeed) > 1:
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             print(self.inputFrames.summary)
             raise TypeError(
                 f"Input frames are a mix of readout speeds. {readSpeed}" % locals())
 
         # MIXED GAIN SPEEDS IS BAD
         # HIERARCH ESO DET OUT1 CONAD - Electrons/ADU
         # CONAD IS REALLY GAIN AND HAS UNIT OF Electrons/ADU
@@ -484,14 +490,16 @@
             gain = self.inputFrames.values(
                 keyword=kw("GAIN"), unique=True)
 
         with suppress(ValueError):
             gain.remove(None)
 
         if len(gain) > 1:
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             print(self.inputFrames.summary)
             raise TypeError(
                 "Input frames are a mix of gain" % locals())
         if len(gain) and gain[0]:
             # UVB & VIS
             self.detectorParams["gain"] = gain[0] * u.electron / u.adu
         else:
@@ -503,14 +511,16 @@
         ron = self.inputFrames.values(
             keyword=kw("RON"), unique=True)
         with suppress(ValueError):
             ron.remove(None)
 
         # MIXED NOISE
         if len(ron) > 1:
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             print(self.inputFrames.summary)
             raise TypeError(f"Input frames are a mix of readnoise. {ron}" % locals())
         if len(ron) and ron[0]:
             # UVB & VIS
             self.detectorParams["ron"] = ron[0] * u.electron
         else:
             # NIR
@@ -555,15 +565,15 @@
 
         ```python
         recipe.clean_up()
         ```
         """
         self.log.debug('starting the ``clean_up`` method')
 
-        outDir = self.intermediateRootPath + "/tmp"
+        outDir = self.workspaceRootPath + "/tmp"
 
         try:
             shutil.rmtree(outDir)
         except:
             pass
 
         self.log.debug('completed the ``clean_up`` method')
@@ -1047,14 +1057,15 @@
         )
         ```
         """
         self.log.debug('starting the ``qc_bias_ron`` method')
 
         from astropy.stats import sigma_clip
         import numpy as np
+        import pandas as pd
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
         if not rawRon:
             # LIST OF RAW CCDDATA OBJECTS
             ccds = [c for c in self.inputFrames.ccds(ccd_kwargs={
@@ -1080,47 +1091,47 @@
             rawRon = dstd / math.sqrt(2)
 
         if rawRon:
             singleFrameType = frameType
             if frameType[0] == "M":
                 singleFrameType = frameType[1:]
 
-            self.qc = self.qc.append({
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "RON DETECTOR",
                 "qc_value": rawRon,
                 "qc_comment": f"[e-] RON in single {singleFrameType}",
                 "qc_unit": "electrons",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
+            }).to_frame().T], ignore_index=True)
 
         if masterFrame and not masterRon:
 
             # PREDICTED MASTER NOISE
             # predictedMasterRon = rawRon / math.sqrt(len(ccds))
 
             # FORCE CONVERSION OF CCDData OBJECT TO NUMPY ARRAY
             tmp = np.ma.array(masterFrame.data, mask=combinedMask)
 
             dmin, dmax, dmean, dstd = imstats(tmp)
             masterRon = dstd
 
         elif masterRon:
-            self.qc = self.qc.append({
+            self.qc = pd.concat([self.qc, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "qc_name": "RON MASTER",
                 "qc_value": masterRon,
                 "qc_comment": f"[e-] Combined RON in {frameType}",
                 "qc_unit": "electrons",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "to_header": True
-            }, ignore_index=True)
+            }).to_frame().T], ignore_index=True)
         else:
             masterRon = None
 
         self.log.debug('completed the ``qc_bias_ron`` method')
         return rawRon, masterRon
 
     def qc_median_flux_level(
@@ -1148,34 +1159,35 @@
             frameType="MBIAS",
             frameName="master bias")
         ```
         """
         self.log.debug('starting the ``qc_median_flux_level`` method')
 
         import numpy as np
+        import pandas as pd
 
         if not medianFlux:
             # DETERMINE MEDIAN BIAS LEVEL
             maskedDataArray = np.ma.array(
                 frame.data, mask=frame.mask)
             medianFlux = np.ma.median(maskedDataArray)
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
-        self.qc = self.qc.append({
+        self.qc = pd.concat([self.qc, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "qc_name": f"{frameType} MEDIAN".upper(),
             "qc_value": medianFlux,
             "qc_comment": f"[e-] Median flux level of {frameName}",
             "qc_unit": "electrons",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "to_header": True
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         self.log.debug('completed the ``qc_median_flux_level`` method')
         return medianFlux
 
     def subtact_mean_flux_level(
             self,
             rawFrame):
```

### Comparing `soxspipe-0.7.2/soxspipe/recipes/soxs_disp_solution.py` & `soxspipe-0.8.0/soxspipe/recipes/soxs_disp_solution.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,38 +114,61 @@
         """
         self.log.debug('starting the ``verify_input_frames`` method')
 
         kw = self.kw
 
         # BASIC VERIFICATION COMMON TO ALL RECIPES
         imageTypes, imageTech, imageCat = self._verify_input_frames_basics()
+        error = False
 
         if self.arm == "NIR":
             # WANT ON AND OFF PINHOLE FRAMES
             # MIXED INPUT IMAGE TYPES ARE BAD
-            if len(imageTypes) > 1:
-                imageTypes = " and ".join(imageTypes)
-                print(self.inputFrames.summary)
-                raise TypeError(
-                    "Input frames are a mix of %(imageTypes)s" % locals())
-
-            if imageTypes[0] != "LAMP,FMTCHK":
-                raise TypeError(
-                    "Input frames for soxspipe disp_solution need to be single pinhole lamp on and lamp off frames for NIR" % locals())
-
-            for i in imageTech:
-                if i not in ['ECHELLE,PINHOLE', 'IMAGE']:
-                    raise TypeError(
-                        "Input frames for soxspipe disp_solution need to be single pinhole lamp on and lamp off frames for NIR" % locals())
+            if not error:
+                if len(imageTypes) > 1:
+                    imageTypes = " and ".join(imageTypes)
+                    imageTypes = " and ".join(imageTypes)
+                    error = "Input frames for soxspipe disp_solution need to be single pinhole lamp on and lamp off frames for NIR" % locals()
+
+            if not error:
+                if imageTypes[0] != "LAMP,FMTCHK":
+                    error = "Input frames for soxspipe disp_solution need to be single pinhole lamp on and lamp off frames for NIR" % locals()
+
+            if not error:
+                for i in imageTech:
+                    if i not in ['ECHELLE,PINHOLE', 'IMAGE']:
+                        error = "Input frames for soxspipe disp_solution need to be single pinhole lamp on and lamp off frames for NIR" % locals()
+
+            if not error:
+                for i in ['ECHELLE,PINHOLE', 'IMAGE']:
+                    if i not in imageTech:
+                        error = "Input frames for soxspipe disp_solution need to be single pinhole lamp on and lamp off frames for NIR" % locals()
 
         else:
-            for i in imageTypes:
-                if i not in ["LAMP,FMTCHK", "BIAS", "DARK"]:
-                    raise TypeError(
-                        "Input frames for soxspipe disp_solution need to be single pinhole lamp on and a master-bias and possibly a master dark for UVB/VIS" % locals())
+            if not error:
+                for i in imageTypes:
+                    if i not in ["LAMP,FMTCHK"]:
+                        error = "Input frames for soxspipe disp_solution need to be single pinhole lamp on and a master-bias and possibly a master dark for UVB/VIS" % locals()
+
+            if not error:
+                for i in ['ECHELLE,PINHOLE']:
+                    if i not in imageTech:
+                        error = "Input frames for soxspipe disp_solution need to be single pinhole lamp on and a master-bias and possibly a master dark for UVB/VIS"
+
+            if not error:
+                for i in [f"MASTER_BIAS_{self.arm}"]:
+                    if i not in imageCat:
+                        error = "Input frames for soxspipe disp_solution need to be single pinhole lamp on and a master-bias and possibly a master dark for UVB/VIS"
+
+        if error:
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
+            print(self.inputFrames.summary)
+            print()
+            raise TypeError(error)
 
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
             self):
@@ -154,14 +177,15 @@
         **Return:**
             - ``productPath`` -- the path to the first guess dispersion map
         """
         self.log.debug('starting the ``produce_product`` method')
 
         from astropy.nddata import CCDData
         from astropy import units as u
+        import pandas as pd
 
         arm = self.arm
         kw = self.kw
         dp = self.detectorParams
 
         # self.inputFrames.summary.pprint_all()
 
@@ -197,15 +221,15 @@
             pinhole_image = CCDData.read(i, hdu=0, unit=u.adu, hdu_uncertainty='ERRS',
                                          hdu_mask='QUAL', hdu_flags='FLAGS', key_uncertainty_type='UTYPE')
 
         self.pinholeFrame = self.detrend(
             inputFrame=pinhole_image, master_bias=master_bias, dark=dark)
 
         if self.settings["save-intermediate-products"]:
-            outDir = self.intermediateRootPath
+            outDir = self.workspaceRootPath
             filePath = self._write(
                 frame=self.pinholeFrame,
                 filedir=outDir,
                 filename=False,
                 overwrite=True,
                 product=False
             )
@@ -221,29 +245,29 @@
         ).get()
 
         filename = os.path.basename(productPath)
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
-        self.products = self.products.append(productsTable)
-        self.qc = self.qc.append(qcTable)
+        self.products = pd.concat([self.products, productsTable])
+        self.qc = pd.concat([self.qc, qcTable])
 
         self.dateObs = self.pinholeFrame.header[kw("DATE_OBS")]
 
-        self.products = self.products.append({
+        self.products = pd.concat([self.products, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "product_label": "DISP_MAP",
             "file_name": filename,
             "file_type": "FITS Table",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "product_desc": f"{self.arm} first pass dispersion solution",
             "file_path": productPath
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         self.report_output()
         self.clean_up()
 
         self.log.debug('completed the ``produce_product`` method')
         return productPath
```

### Comparing `soxspipe-0.7.2/soxspipe/recipes/soxs_mbias.py` & `soxspipe-0.8.0/soxspipe/recipes/soxs_mbias.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,25 +115,29 @@
         self.log.debug('starting the ``verify_input_frames`` method')
 
         kw = self.kw
 
         # BASIC VERIFICATION COMMON TO ALL RECIPES
         imageTypes, imageTech, imageCat = self._verify_input_frames_basics()
 
+        error = False
+
         # MIXED INPUT IMAGE TYPES ARE BAD
         if len(imageTypes) > 1:
-            imageTypes = " and ".join(imageTypes)
-            print(self.inputFrames.summary)
-            raise TypeError(
-                "Input frames are a mix of %(imageTypes)s" % locals())
+            error = "Input frames are a mix of %(imageTypes)s" % locals()
         # NON-BIAS INPUT IMAGE TYPES ARE BAD
         elif imageTypes[0] != 'BIAS':
+            error = "Input frames not BIAS frames" % locals()
+
+        if error:
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             print(self.inputFrames.summary)
-            raise TypeError(
-                "Input frames not BIAS frames" % locals())
+            print()
+            raise TypeError(error)
 
         self.imageType = imageTypes[0]
 
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
@@ -142,14 +146,15 @@
 
         **Return:**
             - ``productPath`` -- the path to the master bias frame
         """
         self.log.debug('starting the ``produce_product`` method')
 
         import numpy as np
+        import pandas as pd
 
         arm = self.arm
         kw = self.kw
         dp = self.detectorParams
 
         # LIST OF CCDDATA OBJECTS
         ccds = [c for c in self.inputFrames.ccds(ccd_kwargs={"hdu_uncertainty": 'ERRS', "hdu_mask": 'QUAL', "hdu_flags": 'FLAGS', "key_uncertainty_type": 'UTYPE'})]
@@ -202,35 +207,35 @@
         self.update_fits_keywords(
             frame=combined_bias_mean
         )
 
         # WRITE TO DISK
         productPath = self._write(
             frame=combined_bias_mean,
-            filedir=self.intermediateRootPath,
+            filedir=self.workspaceRootPath,
             filename=False,
             overwrite=True
         )
         filename = os.path.basename(productPath)
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
         self.dateObs = combined_bias_mean.header[self.kw("DATE_OBS")]
 
-        self.products = self.products.append({
+        self.products = pd.concat([self.products, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "product_label": "MBIAS",
             "file_name": filename,
             "file_type": "FITS",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "product_desc": f"{self.arm} Master bias frame",
             "file_path": productPath
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         self.report_output()
         self.clean_up()
 
         self.log.debug('completed the ``produce_product`` method')
         return productPath
 
@@ -251,14 +256,15 @@
         ```python
         structx, structy = self.qc_bias_structure(combined_bias_mean)
         ```
         """
         self.log.debug('starting the ``qc_bias_structure`` method')
 
         import numpy as np
+        import pandas as pd
         plot = False
 
         collaps_ax1 = np.nansum(combined_bias_mean, axis=0)
         collaps_ax2 = np.nansum(combined_bias_mean, axis=1)
 
         x_axis = np.linspace(0, len(collaps_ax1), len(collaps_ax1), dtype=int)
         y_axis = np.linspace(0, len(collaps_ax2), len(collaps_ax2), dtype=int)
@@ -280,35 +286,35 @@
             plt.xlabel('y-axis')
             plt.ylabel('Summed Pixel Values')
             plt.show()
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
-        self.qc = self.qc.append({
+        self.qc = pd.concat([self.qc, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "qc_name": "STRUCTX",
             "qc_value": coeff_ax1[0],
             "qc_comment": "Slope of BIAS in X direction",
             "qc_unit": None,
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "to_header": True
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
-        self.qc = self.qc.append({
+        self.qc = pd.concat([self.qc, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "qc_name": "STRUCTY",
             "qc_value": coeff_ax2[0],
             "qc_comment": "Slope of BIAS in Y direction",
             "qc_unit": None,
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "to_header": True
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         self.log.debug('completed the ``qc_bias_structure`` method')
         return coeff_ax1[0], coeff_ax2[0]
 
     def qc_periodic_pattern_noise(
             self,
             frames):
@@ -329,14 +335,15 @@
         ```
         """
         self.log.debug('starting the ``qc_periodic_pattern_noise`` method')
 
         from scipy.stats import median_abs_deviation
         from astropy.stats import sigma_clip
         import numpy as np
+        import pandas as pd
 
         # LIST OF CCDDATA OBJECTS
         ccds = [c for c in frames.ccds(ccd_kwargs={"hdu_uncertainty": 'ERRS', "hdu_mask": 'QUAL', "hdu_flags": 'FLAGS', "key_uncertainty_type": 'UTYPE'})]
 
         ratios = []
         for frame in ccds:
             # FORCE CONVERSION OF CCDData OBJECT TO NUMPY ARRAY
@@ -362,23 +369,23 @@
             ratios.append(frame_std / frame_mad)
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
         ppnmax = max(ratios)
 
-        self.qc = self.qc.append({
+        self.qc = pd.concat([self.qc, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "qc_name": "PPNMAX",
             "qc_value": ppnmax,
             "qc_comment": "Max periodic pattern noise ratio in raw bias frames",
             "qc_unit": None,
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "to_header": True
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         self.log.debug('completed the ``qc_periodic_pattern_noise`` method')
         return ppnmax
 
     # use the tab-trigger below for new method
     # xt-class-method
```

### Comparing `soxspipe-0.7.2/soxspipe/recipes/soxs_mdark.py` & `soxspipe-0.8.0/soxspipe/recipes/soxs_mdark.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,35 +116,40 @@
         self.log.debug('starting the ``verify_input_frames`` method')
 
         kw = self.kw
 
         # BASIC VERIFICATION COMMON TO ALL RECIPES
         imageTypes, imageTech, imageCat = self._verify_input_frames_basics()
 
-        # MIXED INPUT IMAGE TYPES ARE BAD
-        if len(imageTypes) > 1:
-            imageTypes = " and ".join(imageTypes)
-            print(self.inputFrames.summary)
-            raise TypeError(
-                "Input frames are a mix of %(imageTypes)s" % locals())
-        # NON-BIAS INPUT IMAGE TYPES ARE BAD
-        elif imageTypes[0] != 'DARK':
-            print(self.inputFrames.summary)
-            raise TypeError(
-                "Input frames not DARK frames" % locals())
+        error = False
 
-        exptimes = self.inputFrames.values(
-            keyword=kw("EXPTIME"), unique=True)
         # MIXED INPUT IMAGE TYPES ARE BAD
-        if len(exptimes) > 1:
-            exptimes = [str(e) for e in exptimes]
-            exptimes = " and ".join(exptimes)
+        if not error:
+            if len(imageTypes) > 1:
+                imageTypes = " and ".join(imageTypes)
+                error = "Input frames are a mix of %(imageTypes)s" % locals()
+            # NON-BIAS INPUT IMAGE TYPES ARE BAD
+            elif imageTypes[0] != 'DARK':
+                error = "Input frames not DARK frames" % locals()
+
+        if not error:
+            exptimes = self.inputFrames.values(
+                keyword=kw("EXPTIME"), unique=True)
+            # MIXED INPUT IMAGE TYPES ARE BAD
+            if len(exptimes) > 1:
+                exptimes = [str(e) for e in exptimes]
+                exptimes = " and ".join(exptimes)
+                error = "Input frames have differing exposure-times %(exptimes)s" % locals()
+
+        if error:
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             print(self.inputFrames.summary)
-            raise TypeError(
-                "Input frames have differing exposure-times %(exptimes)s" % locals())
+            print()
+            raise TypeError(error)
 
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
             self):
@@ -152,14 +157,15 @@
 
         **Return:**
             - ``productPath`` -- the path to master dark frame
         """
         self.log.debug('starting the ``produce_product`` method')
 
         import numpy as np
+        import pandas as pd
 
         arm = self.arm
         kw = self.kw
         dp = self.detectorParams
 
         # LIST OF CCDDATA OBJECTS
         ccds = [c for c in self.inputFrames.ccds(ccd_kwargs={"hdu_uncertainty": 'ERRS', "hdu_mask": 'QUAL', "hdu_flags": 'FLAGS', "key_uncertainty_type": 'UTYPE'})]
@@ -199,35 +205,35 @@
         self.update_fits_keywords(
             frame=combined_dark_mean
         )
 
         # WRITE TO DISK
         productPath = self._write(
             frame=combined_dark_mean,
-            filedir=self.intermediateRootPath,
+            filedir=self.workspaceRootPath,
             filename=False,
             overwrite=True
         )
         filename = os.path.basename(productPath)
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
         self.dateObs = combined_dark_mean.header[kw("DATE_OBS")]
 
-        self.products = self.products.append({
+        self.products = pd.concat([self.products, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "product_label": "MDARK",
             "file_name": filename,
             "file_type": "FITS",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "product_desc": f"{self.arm} Master dark frame",
             "file_path": productPath
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         self.report_output()
         self.clean_up()
 
         self.log.debug('completed the ``produce_product`` method')
         return productPath
```

### Comparing `soxspipe-0.7.2/soxspipe/recipes/soxs_mflat.py` & `soxspipe-0.8.0/soxspipe/recipes/soxs_mflat.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,71 +116,99 @@
 
         If the fits files conform to required input for the recipe everything will pass silently, otherwise an exception will be raised.
         """
         self.log.debug('starting the ``verify_input_frames`` method')
 
         kw = self.kw
 
+        error = False
+
         import warnings
         from astropy.utils.exceptions import AstropyWarning
         warnings.simplefilter('ignore', AstropyWarning)
 
         # BASIC VERIFICATION COMMON TO ALL RECIPES
         imageTypes, imageTech, imageCat = self._verify_input_frames_basics()
 
         if self.arm == "NIR":
             # WANT ON AND OFF PINHOLE FRAMES
             # MIXED INPUT IMAGE TYPES ARE BAD
-            if len(imageTypes) > 1:
-                imageTypes = " and ".join(imageTypes)
-                raise TypeError(
-                    "Input frames are a mix of %(imageTypes)s" % locals())
-
-            if imageTypes[0] != "LAMP,FLAT":
-                raise TypeError(
-                    "Input frames for soxspipe mflat need to be slit flat lamp on and lamp off frames for NIR" % locals())
-
-            for i in imageTech:
-                if i not in ['ECHELLE,SLIT', 'IMAGE']:
-                    raise TypeError(
-                        f"Input frames for soxspipe mflat need to be slit flat lamp on and lamp off frames for NIR. You have provided {imageTech}" % locals())
+            if not error:
+                if len(imageTypes) > 1:
+                    imageTypes = " and ".join(imageTypes)
+                    error = "Input frames are a mix of %(imageTypes)s" % locals()
+
+            if not error:
+                if imageTypes[0] != "LAMP,FLAT":
+                    error = "Input frames for soxspipe mflat need to be flat-lamp on and lamp off frames for NIR" % locals()
+
+            if not error:
+                for i in imageTech:
+                    if i not in ['ECHELLE,SLIT', 'IMAGE']:
+                        error = "Input frames for soxspipe mflat need to be flat-lamp on and lamp off frames for NIR. You have provided {imageTech}" % locals()
+
+            if not error:
+                for i in ['ECHELLE,SLIT', 'IMAGE']:
+                    if i not in imageTech:
+                        error = "Input frames for soxspipe mflat need to be flat-lamp on and lamp off frames for NIR. You have provided {imageTech}" % locals()
 
         else:
-            for i in imageTypes:
-                if i not in ["LAMP,FLAT", "LAMP,QFLAT", "LAMP,DFLAT", "BIAS", "DARK"]:
-                    raise TypeError(
-                        "Input frames for soxspipe mflat need to be slit flat lamp frames and a master-bias and possibly a master dark for UVB/VIS" % locals())
+            if not error:
+                for i in imageTypes:
+                    if i not in ["LAMP,FLAT", "LAMP,QFLAT", "LAMP,DFLAT"]:
+                        error = "Input frames for soxspipe mflat need to be flat-lamp frames,a master-bias frame, an order-locations tables and possibly a master dark for UVB/VIS" % locals()
+
+            if not error:
+                for i in [f"MASTER_BIAS_{self.arm}", f"ORDER_TAB_{self.arm}"]:
+                    if i not in imageCat:
+                        error = "Input frames for soxspipe mflat need to be flat-lamp frames,a master-bias frame, an order-locations tables and possibly a master dark for UVB/VIS" % locals()
+
+            if not error:
+                found = False
+                for i in ["LAMP,FLAT", "LAMP,QFLAT", "LAMP,DFLAT"]:
+                    if i in imageTypes:
+                        found = True
+                if not found:
+                    error = "Input frames for soxspipe mflat need to be flat-lamp frames,a master-bias frame, an order-locations tables and possibly a master dark for UVB/VIS" % locals()
 
         # UV-VIS NEEDS BOTH D AND Q-LAMPS
-        if "LAMP,QFLAT" in imageTypes or "LAMP,DFLAT" in imageTypes:
-            if "LAMP,QFLAT" in imageTypes and "LAMP,DFLAT" in imageTypes:
-                pass
-            else:
-                for i in imageTypes:
-                    if "LAMP" in i:
-                        self.log.warning(f'Only "{i}" image types found. Please include both D2 and QTH lamp flats')
+        if not error:
+            if "LAMP,QFLAT" in imageTypes or "LAMP,DFLAT" in imageTypes:
+                if "LAMP,QFLAT" in imageTypes and "LAMP,DFLAT" in imageTypes:
+                    pass
+                else:
+                    for i in imageTypes:
+                        if "LAMP" in i:
+                            error = f'Only "{i}" image types found. Please include both D2 and QTH lamp flats'
 
         # LOOK FOR ORDER TABLE
-        arm = self.arm
-        if f"ORDER_TAB_{arm}" not in imageCat:
-            raise TypeError(
-                "Need an order centre for %(arm)s - none found with the input files" % locals())
+        if not error:
+            arm = self.arm
+            if f"ORDER_TAB_{arm}" not in imageCat:
+                error = f"Need an order centre for {arm} - none found with the input files"
 
         # CHECK EXPTIME
-        lamps = ["LAMP,FLAT", "LAMP,DFLAT", "LAMP,QFLAT"]
-        for l in lamps:
-            filterDict = {kw("DPR_TYPE"): l,
-                          kw("DPR_TECH"): "ECHELLE,SLIT"}
-            flatCollection = self.inputFrames.filter(**filterDict)
-            if len(flatCollection.files):
-                exptime = flatCollection.values(
-                    keyword=kw("EXPTIME"), unique=True)
-                if len(exptime) > 1:
-                    raise TypeError(
-                        f"Input {l} frames for soxspipe mflat need to have a unique exptime" % locals())
+        if not error:
+            lamps = ["LAMP,FLAT", "LAMP,DFLAT", "LAMP,QFLAT"]
+            for l in lamps:
+                filterDict = {kw("DPR_TYPE"): l,
+                              kw("DPR_TECH"): "ECHELLE,SLIT"}
+                flatCollection = self.inputFrames.filter(**filterDict)
+                if len(flatCollection.files):
+                    exptime = flatCollection.values(
+                        keyword=kw("EXPTIME"), unique=True)
+                    if len(exptime) > 1:
+                        error = f"Input {l} frames for soxspipe mflat need to have a unique exptime"
+
+        if error:
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
+            print(self.inputFrames.summary)
+            print()
+            raise TypeError(error)
 
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
             self):
@@ -280,15 +308,17 @@
                 sofName=self.sofName,
                 binx=self.binx,
                 biny=self.biny
             )
             productTable, qcTable, orderDetectionCounts = edges.get()
 
             if tag:
+                # NEED TO TRY AND RENAME BOTH ORDER AND COUNT COLUMNS FOR PANDAS 1.X and 2.X
                 orderDetectionCounts.rename(columns={"order": tag}, inplace=True)
+                orderDetectionCounts.rename(columns={"count": tag}, inplace=True)
                 orderDetectionCounts.index.names = ['order']
 
             self.detectionCountSet.append(orderDetectionCounts)
 
             mask = (productTable['product_label'] == f"ORDER_LOC{tag}")
             orderTablePath = productTable.loc[mask]["file_path"].values[0]
             self.orderTableSet.append(orderTablePath)
@@ -332,58 +362,58 @@
         else:
             self.products = productTable
             self.qc = qcTable
 
         quicklook_image(log=self.log, CCDObject=mflat, show=False, ext=None, surfacePlot=True, title="Final master flat frame")
 
         home = expanduser("~")
-        outDir = self.settings["intermediate-data-root"].replace("~", home)
+        outDir = self.settings["workspace-root-dir"].replace("~", home)
         # filePath = f"{outDir}/first_iteration_{arm}_master_flat.fits"
 
         self.update_fits_keywords(
             frame=mflat
         )
 
         # WRITE MFLAT TO FILE
         productPath = self._write(
             mflat, outDir, overwrite=True)
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
         basename = os.path.basename(productPath)
-        self.products = self.products.append({
+        self.products = pd.concat([self.products, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "product_label": f"MFLAT",
             "file_name": basename,
             "file_type": "FITS",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "product_desc": f"{self.arm} master spectroscopic flat frame",
             "file_path": productPath
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         if 1 == 0:
             filename = filenamer(
                 log=self.log,
                 frame=mflat,
                 settings=self.settings
             )
             filename = filename.replace(".fits", "_background.fits")
             filepath = self._write(
                 backgroundFrame, outDir, filename=filename, overwrite=True)
             filepath = os.path.abspath(filepath)
-            self.products = self.products.append({
+            self.products = pd.concat([self.products, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "product_label": "",
                 "file_name": filename,
                 "file_type": "FITS",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "product_desc": f"modelled scatter background light image (removed from master flat)",
                 "file_path": backgroundFrame
-            }, ignore_index=True)
+            }).to_frame().T], ignore_index=True)
 
         # ADD QUALITY CHECKS
         self.qc = generic_quality_checks(
             log=self.log, frame=mflat, settings=self.settings, recipeName=self.recipeName, qcTable=self.qc)
         self.qc = spectroscopic_image_quality_checks(
             log=self.log, frame=mflat, settings=self.settings, recipeName=self.recipeName, qcTable=self.qc, orderTablePath=orderTablePath)
 
@@ -488,15 +518,15 @@
 
         for frame in calibratedFlats:
             quicklook_image(log=self.log, CCDObject=frame, show=False)
 
         if 1 == 0:
             from os.path import expanduser
             home = expanduser("~")
-            outDir = self.settings["intermediate-data-root"].replace("~", home)
+            outDir = self.settings["workspace-root-dir"].replace("~", home)
             index = 1
             for frame in calibratedFlats:
                 filePath = f"{outDir}/{index:02}_flat_{arm}_calibrated.fits"
                 index += 1
                 self._write(frame, filePath, overwrite=True)
 
         self.log.debug('completed the ``calibrate_frame_set`` method')
@@ -682,23 +712,23 @@
 
         lowSensitivityPixelMask = (frameClipped.mask == 1) & (beforeMask != 1)
         lowSensPixelCount = lowSensitivityPixelMask.sum()
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
-        self.qc = self.qc.append({
+        self.qc = pd.concat([self.qc, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "qc_name": "NLOWSENS",
             "qc_value": lowSensPixelCount,
             "qc_comment": "Number of low-sensitivity pixels found in master flat",
             "qc_unit": "pixels",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
         print(f"        {lowSensPixelCount} low-sensitivity pixels added to bad-pixel mask")
 
         frame.mask = (lowSensitivityPixelMask == 1) | (originalBPM == 1)
 
         # SET INTRA-ORDER TO 1
         frame.data[interOrderMask] = 1
 
@@ -739,15 +769,17 @@
 
         import pandas as pd
 
         kw = self.kw
 
         # MERGE DETECTION DATAFRAMES - LISTING ALL ORDER EGDE LOCATIONS FOUND FOR EACH ORDER IN D AND QTH LAMP FRAMES
         detectionCount = pd.merge(self.detectionCountSet[0], self.detectionCountSet[1], left_index=True, right_index=True)
+
         detectionCount["best_frame"] = detectionCount.idxmax(axis=1)
+
         mask = (detectionCount['best_frame'] == "_QLAMP")
         orderFlip = detectionCount.loc[mask]
         # THIS IS THE ORDER THAT WE USE TO RESCALE ONE FLAT TO ANOTHER
         orderFlip = orderFlip.index.max() - 1
         filteredDf = medianOrderFluxDF.loc[(medianOrderFluxDF["order"] == orderFlip)]
         filteredDf["scale"] = filteredDf["_DLAMP"] / filteredDf["_QLAMP"]
         DQscale = filteredDf["scale"].values[0]
```

### Comparing `soxspipe-0.7.2/soxspipe/recipes/soxs_nod_mode.py` & `soxspipe-0.8.0/soxspipe/recipes/soxs_straighten.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,51 @@
 #!/usr/bin/env python
 # encoding: utf-8
 """
-*Reduced science spectral frames taking in nodding mode*
+*transform spectral image from detector pixel space to wavelength and slit-position space*
 
 :Author:
     David Young & Marco Landoni
 
 :Date Created:
-    September 24, 2021
+    May 17, 2021
 """
 ################# GLOBAL IMPORTS ####################
 from datetime import datetime
 from soxspipe.commonutils import keyword_lookup
 from ._base_recipe_ import _base_recipe_
 from fundamentals import tools
 from builtins import object
 import sys
 import os
 os.environ['TERM'] = 'vt100'
 
 
-class soxs_nod_mode(_base_recipe_):
+class soxs_straighten(_base_recipe_):
     """
-    *The soxs_nod_mode recipe*
+    *The soxs_straighten recipe*
 
-    **Key Arguments**
 
-        - ``log`` -- logger
-        - ``settings`` -- the settings dictionary
-        - ``inputFrames`` -- input fits frames. Can be a directory, a set-of-files (SOF) file or a list of fits frame paths.
-        - ``verbose`` -- verbose. True or False. Default *False*
-        - ``overwrite`` -- overwrite the prodcut file if it already exists. Default *False*
-
-    See `produce_product` method for usage.
-
-    ```eval_rst
-    .. todo::
-
-        - add usage info
-        - create a sublime snippet for usage
-        - create cl-util for this class
-        - add a tutorial about ``soxs_nod_mode`` to documentation
-    ```
     """
     # Initialisation
 
     def __init__(
             self,
             log,
             settings=False,
             inputFrames=[],
             verbose=False,
             overwrite=False
 
     ):
         # INHERIT INITIALISATION FROM  _base_recipe_
-        super(soxs_nod_mode, self).__init__(
-            log=log, settings=settings, inputFrames=inputFrames, overwrite=overwrite, recipeName="soxs-nod-mode")
+        super(soxs_straighten, self).__init__(
+            log=log, settings=settings, inputFrames=inputFrames, overwrite=overwrite, recipeName="soxs-straighten")
         self.log = log
-        log.debug("instansiating a new 'soxs_nod_mode' object")
+        log.debug("instansiating a new 'soxs_straighten' object")
         self.settings = settings
         self.inputFrames = inputFrames
         self.verbose = verbose
         self.recipeSettings = settings[self.recipeName]
         # xt-self-arg-tmpx
 
         # INITIAL ACTIONS
@@ -73,15 +56,15 @@
             log=self.log,
             settings=self.settings,
             inputFrames=self.inputFrames,
             ext=self.settings['data-extension']
         )
         self.inputFrames, self.supplementaryInput = sof.get()
 
-        # VERIFY THE FRAMES ARE THE ONES EXPECTED BY SOXS_nod_mode - NO MORE, NO LESS.
+        # VERIFY THE FRAMES ARE THE ONES EXPECTED BY SOXS_straighten - NO MORE, NO LESS.
         # PRINT SUMMARY OF FILES.
         print("# VERIFYING INPUT FRAMES")
         self.verify_input_frames()
         sys.stdout.write("\x1b[1A\x1b[2K")
         print("# VERIFYING INPUT FRAMES - ALL GOOD")
 
         # SORT IMAGE COLLECTION
@@ -95,95 +78,107 @@
         self.inputFrames = self.prepare_frames(
             save=self.settings["save-intermediate-products"])
 
         return None
 
     def verify_input_frames(
             self):
-        """*verify the input frame match those required by the soxs_nod_mode recipe*
+        """*verify the input frame match those required by the soxs_straighten recipe*
 
         **Return:**
             - ``None``
 
         If the fits files conform to required input for the recipe everything will pass silently, otherwise an exception shall be raised.
         """
         self.log.debug('starting the ``verify_input_frames`` method')
 
         kw = self.kw
 
+        error = False
+
         # BASIC VERIFICATION COMMON TO ALL RECIPES
         imageTypes, imageTech, imageCat = self._verify_input_frames_basics()
 
-        if self.arm == "NIR":
-            # WANT ON AND OFF PINHOLE FRAMES
-            # MIXED INPUT IMAGE TYPES ARE BAD
-            if len(imageTypes) > 1:
-                imageTypes = " and ".join(imageTypes)
-                print(self.inputFrames.summary)
-                raise TypeError(
-                    "Input frames are a mix of %(imageTypes)s" % locals())
-
-            if imageTypes[0] != "LAMP,FMTCHK":
-                raise TypeError(
-                    "Input frames for soxspipe nod_mode need to be ********* lamp on and lamp off frames for NIR" % locals())
-
-            for i in imageTech:
-                if i not in ['ECHELLE,PINHOLE', 'IMAGE']:
-                    raise TypeError(
-                        "Input frames for soxspipe nod_mode need to be ********* lamp on and lamp off frames for NIR" % locals())
-
-        else:
-            for i in imageTypes:
-                if i not in ["LAMP,FMTCHK", "BIAS", "DARK"]:
-                    raise TypeError(
-                        "Input frames for soxspipe nod_mode need to be ********* and a master-bias and possibly a master dark for UVB/VIS" % locals())
+        # NEED TO READD FILTERING
+
+        # if self.arm == "NIR":
+        #     # WANT ON AND OFF PINHOLE FRAMES
+        #     # MIXED INPUT IMAGE TYPES ARE BAD
+        #     if len(imageTypes) > 1:
+        #         imageTypes = " and ".join(imageTypes)
+        #         print(self.inputFrames.summary)
+        #         raise TypeError(
+        #             "Input frames are a mix of %(imageTypes)s" % locals())
+
+        #     if imageTypes[0] != "LAMP,FMTCHK":
+        #         raise TypeError(
+        #             "Input frames for soxspipe straighten need to be ********* lamp on and lamp off frames for NIR" % locals())
+
+        #     for i in imageTech:
+        #         if i not in ['ECHELLE,PINHOLE', 'IMAGE']:
+        #             raise TypeError(
+        #                 "Input frames for soxspipe straighten need to be ********* lamp on and lamp off frames for NIR" % locals())
+
+        # else:
+        #     for i in imageTypes:
+        #         if i not in ["LAMP,FMTCHK", "BIAS", "DARK"]:
+        #             raise TypeError(
+        #                 "Input frames for soxspipe straighten need to be ********* and a master-bias and possibly a master dark for UVB/VIS" % locals())
 
         # LOOK FOR ****
         arm = self.arm
-        if arm not in self.supplementaryInput or "DISP_MAP" not in self.supplementaryInput[arm]:
+        if arm not in self.supplementaryInput or "2D_MAP" not in self.supplementaryInput[arm]:
             raise TypeError(
-                "Need a **** for %(arm)s - none found with the input files" % locals())
+                "Need a full dispersion/spatial solution for %(arm)s - none found with the input files" % locals())
+
+        if error:
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
+            print(self.inputFrames.summary)
+            print()
+            raise TypeError(error)
 
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
             self):
-        """*The code to generate the product of the soxs_nod_mode recipe*
+        """*The code to generate the product of the soxs_straighten recipe*
 
         **Return:**
             - ``productPath`` -- the path to the final product
 
         **Usage**
 
         ```python
-        from soxspipe.recipes import soxs_nod_mode
-        recipe = soxs_nod_mode(
+        from soxspipe.recipes import soxs_straighten
+        recipe = soxs_straighten(
             log=log,
             settings=settings,
             inputFrames=fileList
         )
-        nod_modeFrame = recipe.produce_product()
+        straightenFrame = recipe.produce_product()
         ```
         """
         self.log.debug('starting the ``produce_product`` method')
 
         arm = self.arm
         kw = self.kw
         dp = self.detectorParams
 
         productPath = None
 
-        filename = os.path.basename(productPath)
+        # filename = os.path.basename(productPath)
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
         # xsoxs-append-to-product-report-table
+
         self.report_output()
         self.clean_up()
 
         self.log.debug('completed the ``produce_product`` method')
         return productPath
 
     # use the tab-trigger below for new method
```

### Comparing `soxspipe-0.7.2/soxspipe/recipes/soxs_order_centres.py` & `soxspipe-0.8.0/soxspipe/recipes/soxs_order_centres.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,46 +115,58 @@
 
         If the fits files conform to required input for the recipe everything will pass silently, otherwise an exception shall be raised.
         """
         self.log.debug('starting the ``verify_input_frames`` method')
 
         kw = self.kw
 
+        error = False
+
         # BASIC VERIFICATION COMMON TO ALL RECIPES
         imageTypes, imageTech, imageCat = self._verify_input_frames_basics()
 
         if self.arm == "NIR":
             # WANT ON AND OFF PINHOLE FRAMES
             # MIXED INPUT IMAGE TYPES ARE BAD
-            if len(imageTypes) > 1:
-                imageTypes = " and ".join(imageTypes)
-                print(self.inputFrames.summary)
-                raise TypeError(
-                    "Input frames are a mix of %(imageTypes)s" % locals())
-
-            if imageTypes[0] != "LAMP,ORDERDEF":
-                raise TypeError(
-                    "Input frames for soxspipe order_centres need to be single pinhole flat-lamp on and lamp off frames for NIR" % locals())
-
-            for i in imageTech:
-                if i not in ['ECHELLE,PINHOLE', 'IMAGE']:
-                    raise TypeError(
-                        "Input frames for soxspipe order_centres need to be single pinhole flat-lamp on and lamp off frames for NIR" % locals())
+            if not error:
+                if len(imageTypes) > 1:
+                    imageTypes = " and ".join(imageTypes)
+                    erorr = "Input frames are a mix of %(imageTypes)s" % locals()
+
+            if not error:
+                if imageTypes[0] != "LAMP,ORDERDEF":
+                    error = "Input frames for soxspipe order_centres need to be single pinhole flat-lamp on and lamp off frames and a first-guess dispersion solution table for NIR" % locals()
+
+            if not error:
+                for i in imageTech:
+                    if i not in ['ECHELLE,PINHOLE', 'IMAGE']:
+                        error = "Input frames for soxspipe order_centres need to be single pinhole flat-lamp on and lamp off frames a first-guess dispersion solution table for NIR" % locals()
+
+            if not error:
+                for i in [f"DISP_TAB_{self.arm}"]:
+                    if i not in imageCat:
+                        error = "Input frames for soxspipe order_centres need to be single pinhole flat-lamp on and lamp off frames a first-guess dispersion solution table for NIR" % locals()
 
         else:
-            for i in imageTypes:
-                if i not in ["LAMP,ORDERDEF", "BIAS", "DARK", 'LAMP,DORDERDEF', 'LAMP,QORDERDEF']:
-                    raise TypeError(
-                        f"Input frames for soxspipe order_centres need to be single pinhole flat-lamp on and a master-bias and possibly a master dark for UVB/VIS. Found {i}" % locals())
-
-        # LOOK FOR DISP MAP
-        arm = self.arm
-        if f"DISP_TAB_{arm}" not in imageCat:
-            raise TypeError(
-                "Need a first guess dispersion map for %(arm)s - none found with the input files" % locals())
+            if not error:
+                for i in imageTypes:
+                    if i not in ["LAMP,ORDERDEF", 'LAMP,DORDERDEF', 'LAMP,QORDERDEF']:
+                        error = "Input frames for soxspipe order_centres need to be single pinhole flat-lamp, a master-bias frame, a first-guess dispersion solution table and possibly a master dark for UVB/VIS. Found {i}" % locals()
+
+            if not error:
+                for i in [f"MASTER_BIAS_{self.arm}", f"DISP_TAB_{self.arm}"]:
+                    if i not in imageCat:
+                        error = "Input frames for soxspipe order_centres need to be single pinhole flat-lamp, a master-bias frame, a first-guess dispersion solution table and possibly a master dark for UVB/VIS." % locals()
+
+        if error:
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
+            print(self.inputFrames.summary)
+            print()
+            raise TypeError(error)
 
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
             self):
@@ -163,14 +175,15 @@
         **Return:**
             - ``productPath`` -- the path to the order-table
         """
         self.log.debug('starting the ``produce_product`` method')
 
         from astropy.nddata import CCDData
         from astropy import units as u
+        import pandas as pd
 
         arm = self.arm
         kw = self.kw
         dp = self.detectorParams
 
         productPath = None
 
@@ -219,15 +232,15 @@
         for i in self.inputFrames.files_filtered(include_path=True, **add_filters):
             disp_map_table = i
 
         self.orderFrame = self.detrend(
             inputFrame=orderDef_image, master_bias=master_bias, dark=dark)
 
         if self.settings["save-intermediate-products"]:
-            fileDir = self.intermediateRootPath
+            fileDir = self.workspaceRootPath
             filepath = self._write(
                 self.orderFrame, fileDir, filename=False, overwrite=True, product=False)
             print(f"\nCalibrated single pinhole frame frame saved to {filepath}\n")
 
         # FIND THE APPROPRIATE PREDICTED LINE-LIST
         if arm != "NIR" and kw('WIN_BINX') in self.orderFrame.header:
             binx = int(self.orderFrame.header[kw('WIN_BINX')])
@@ -248,33 +261,33 @@
             productsTable=self.products,
             sofName=self.sofName,
             binx=binx,
             biny=biny
         )
         productPath, qcTable, productsTable = detector.get()
 
-        self.products = self.products.append(productsTable)
-        self.qc = self.qc.append(qcTable)
+        self.products = pd.concat([self.products, productsTable])
+        self.qc = pd.concat([self.qc, qcTable])
 
         filename = os.path.basename(productPath)
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
         self.dateObs = self.orderFrame.header[kw("DATE_OBS")]
 
-        self.products = self.products.append({
+        self.products = pd.concat([self.products, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "product_label": "ORDER_CENTRES",
             "file_name": filename,
             "file_type": "FITS",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "product_desc": f"{self.arm} order centre traces",
             "file_path": productPath
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         self.report_output()
         self.clean_up()
 
         self.log.debug('completed the ``produce_product`` method')
         return productPath
```

### Comparing `soxspipe-0.7.2/soxspipe/recipes/soxs_spatial_solution.py` & `soxspipe-0.8.0/soxspipe/recipes/soxs_spatial_solution.py`

 * *Files 10% similar despite different names*

```diff
@@ -104,54 +104,61 @@
 
         If the fits files conform to required input for the recipe everything will pass silently, otherwise an exception shall be raised.
         """
         self.log.debug('starting the ``verify_input_frames`` method')
 
         kw = self.kw
 
+        error = False
+
         # BASIC VERIFICATION COMMON TO ALL RECIPES
         imageTypes, imageTech, imageCat = self._verify_input_frames_basics()
 
         if self.arm == "NIR":
             # WANT ON AND OFF PINHOLE FRAMES
-            for i in imageTypes:
-                if i not in ["LAMP,WAVE", "LAMP,FLAT"]:
-                    raise TypeError(
-                        f"Found a {i} file. Input frames for soxspipe spatial_solution need to be LAMP,WAVE. Can optionally supply a master-flat for NIR.")
-
-            for i in imageTech:
-                if i not in ['ECHELLE,MULTI-PINHOLE', 'IMAGE', 'ECHELLE,SLIT', 'ECHELLE,PINHOLE']:
-                    raise TypeError(
-                        f"Found a {i} file. Input frames for soxspipe spatial_solution need to be LAMP,WAVE. Can optionally supply a master-flat for NIR.")
-
-            if "LAMP,WAVE" not in imageTypes:
-                raise TypeError(
-                    "Input frames for soxspipe spatial_solution need to be LAMP,WAVE lamp on and lamp off frames for NIR" % locals())
-
-            if "ECHELLE,MULTI-PINHOLE" not in imageTech:
-                raise TypeError(
-                    "Input frames for soxspipe spatial_solution need to be LAMP,WAVE lamp on and lamp off frames for NIR" % locals())
+            if not error:
+                for i in imageTypes:
+                    if i not in ["LAMP,WAVE", "LAMP,FLAT"]:
+                        error = f"Found a {i} file. Input frames for soxspipe spatial_solution need to be LAMP,WAVE. Can optionally supply a master-flat for NIR."
+
+            if not error:
+                for i in imageTech:
+                    if i not in ['ECHELLE,MULTI-PINHOLE', 'IMAGE', 'ECHELLE,SLIT', 'ECHELLE,PINHOLE']:
+                        error = f"Found a {i} file. Input frames for soxspipe spatial_solution need to be LAMP,WAVE lamp on and lamp off frames, a first-guess dispersion solution table and an order location table for NIR. Can optionally supply a master-flat for NIR."
+
+            if not error:
+                if "LAMP,WAVE" not in imageTypes:
+                    error = "Input frames for soxspipe spatial_solution need to be LAMP,WAVE lamp on and lamp off frames, a first-guess dispersion solution table and an order location table for NIR. Can optionally supply a master-flat for NIR."
+
+            if not error:
+                if "ECHELLE,MULTI-PINHOLE" not in imageTech:
+                    error = "Input frames for soxspipe spatial_solution need to be LAMP,WAVE lamp on and lamp off frames, a first-guess dispersion solution table and an order location table for NIR. Can optionally supply a master-flat for NIR."
+
+            if not error:
+                for i in [f"ORDER_TAB_{self.arm}", f"DISP_TAB_{self.arm}"]:
+                    if i not in imageCat:
+                        error = "Input frames for soxspipe spatial_solution need to be LAMP,WAVE lamp on and lamp off frames, a first-guess dispersion solution table and an order location table for NIR. Can optionally supply a master-flat for NIR."
 
         else:
-            for i in imageTypes:
-                if i not in ["LAMP,WAVE", "BIAS", "DARK", "LAMP,FLAT"]:
-                    raise TypeError(
-                        f"Found a {i} file. Input frames for soxspipe spatial_solution need to be LAMP,WAVE and a master-bias. Can optionally supply a master-flat and/or master-dark for UVB/VIS.")
-
-        # LOOK FOR DISP MAP
-        arm = self.arm
-        if f"DISP_TAB_{arm}" not in imageCat:
-            raise TypeError(
-                "Need a first guess dispersion map for %(arm)s - none found with the input files" % locals())
-
-        # LOOK FOR ORDER TABLE
-        arm = self.arm
-        if f"ORDER_TAB_{arm}" not in imageCat:
-            raise TypeError(
-                "Need an order centre for %(arm)s - none found with the input files" % locals())
+            if not error:
+                for i in imageTypes:
+                    if i not in ["LAMP,WAVE", "LAMP,FLAT"]:
+                        error = f"Found a {i} frame. Input frames for soxspipe spatial_solution need to be LAMP,WAVE and a master-bias, a first-guess dispersion solution table and an order location table. Can optionally supply a master-flat and/or master-dark for UVB/VIS."
+
+            if not error:
+                for i in [f"MASTER_BIAS_{self.arm}", f"ORDER_TAB_{self.arm}", f"DISP_TAB_{self.arm}"]:
+                    if i not in imageCat:
+                        error = f"Input frames for soxspipe spatial_solution need to be LAMP,WAVE, a master-bias, a first-guess dispersion solution table and an order location table. Can optionally supply a master-flat and/or master-dark for UVB/VIS."
+
+        if error:
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
+            print(self.inputFrames.summary)
+            print()
+            raise TypeError(error)
 
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
             self):
@@ -172,14 +179,15 @@
         disp_map = recipe.produce_product()
         ```
         """
         self.log.debug('starting the ``produce_product`` method')
 
         from astropy.nddata import CCDData
         from astropy import units as u
+        import pandas as pd
 
         arm = self.arm
         kw = self.kw
         dp = self.detectorParams
 
         productPath = None
 
@@ -230,15 +238,15 @@
         for i in self.inputFrames.files_filtered(include_path=True, **add_filters):
             disp_map_table = i
 
         self.multiPinholeFrame = self.detrend(
             inputFrame=multi_pinhole_image, master_bias=master_bias, dark=dark, master_flat=master_flat, order_table=order_table)
 
         if self.settings["save-intermediate-products"]:
-            fileDir = self.intermediateRootPath
+            fileDir = self.workspaceRootPath
             filepath = self._write(
                 self.multiPinholeFrame, fileDir, filename=False, overwrite=True, product=False)
             print(f"\nCalibrated multi pinhole frame frame saved to {filepath}\n")
 
         # GENERATE AN UPDATED DISPERSION MAP
         from soxspipe.commonutils import create_dispersion_map
         mapPath, mapImagePath, res_plots, qcTable, productsTable = create_dispersion_map(
@@ -255,40 +263,40 @@
 
         from datetime import datetime
         filename = os.path.basename(mapPath)
 
         utcnow = datetime.utcnow()
         utcnow = utcnow.strftime("%Y-%m-%dT%H:%M:%S")
 
-        self.products = self.products.append(productsTable)
-        self.qc = self.qc.append(qcTable)
+        self.products = pd.concat([self.products, productsTable])
+        self.qc = pd.concat([self.qc, qcTable])
 
-        self.products = self.products.append({
+        self.products = pd.concat([self.products, pd.Series({
             "soxspipe_recipe": self.recipeName,
             "product_label": "SPAT_SOL",
             "file_name": filename,
             "file_type": "FITS",
             "obs_date_utc": self.dateObs,
             "reduction_date_utc": utcnow,
             "product_desc": f"{self.arm} full dispersion-spatial solution",
             "file_path": productPath
-        }, ignore_index=True)
+        }).to_frame().T], ignore_index=True)
 
         if mapImagePath:
             filename = os.path.basename(mapImagePath)
-            self.products = self.products.append({
+            self.products = pd.concat([self.products, pd.Series({
                 "soxspipe_recipe": self.recipeName,
                 "product_label": "2D_MAP",
                 "file_name": filename,
                 "file_type": "FITS",
                 "obs_date_utc": self.dateObs,
                 "reduction_date_utc": utcnow,
                 "product_desc": f"{self.arm} 2D detector map of wavelength, slit position and order",
                 "file_path": productPath
-            }, ignore_index=True)
+            }).to_frame().T], ignore_index=True)
 
         self.report_output()
 
         self.clean_up()
 
         self.log.debug('completed the ``produce_product`` method')
         return mapPath, mapImagePath, res_plots
```

### Comparing `soxspipe-0.7.2/soxspipe/recipes/soxs_stare.py` & `soxspipe-0.8.0/soxspipe/recipes/soxs_stare.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,41 +108,54 @@
 
         If the fits files conform to required input for the recipe everything will pass silently, otherwise an exception shall be raised.
         """
         self.log.debug('starting the ``verify_input_frames`` method')
 
         kw = self.kw
 
+        error = False
+
         # BASIC VERIFICATION COMMON TO ALL RECIPES
         imageTypes, imageTech, imageCat = self._verify_input_frames_basics()
 
         if self.arm == "NIR":
-
-            for i in imageTypes:
-                if i not in ["OBJECT", "LAMP,FLAT", "DARK", "STD,FLUX"]:
-                    raise TypeError(
-                        f"Found a {i} file. Input frames for soxspipe stare need to be OBJECT, ***. Can optionally supply a master-flat for NIR.")
-
-            for i in imageTech:
-                if i not in ['ECHELLE,SLIT,STARE', "IMAGE", "ECHELLE,SLIT", "ECHELLE,MULTI-PINHOLE", "ECHELLE,SLIT,NODDING"]:
-                    raise TypeError(
-                        "Input frames for soxspipe stare need to be ********* lamp on and lamp off frames for NIR" % locals())
+            if not error:
+                for i in imageTypes:
+                    if i not in ["OBJECT", "LAMP,FLAT", "DARK", "STD,FLUX"]:
+                        error = "Found a {i} file. Input frames for soxspipe stare need to be OBJECT, ***. Can optionally supply a master-flat for NIR."
+
+            if not error:
+                for i in imageTech:
+                    if i not in ['ECHELLE,SLIT,STARE', "IMAGE", "ECHELLE,SLIT", "ECHELLE,MULTI-PINHOLE", "ECHELLE,SLIT,NODDING"]:
+                        error = "Input frames for soxspipe stare need to be ********* lamp on and lamp off frames for NIR" % locals()
 
         else:
-            for i in imageTypes:
-                if i not in ["OBJECT", "LAMP,FLAT", "BIAS", "DARK"]:
-                    raise TypeError(
-                        "Input frames for soxspipe stare need to be ********* and a master-bias and possibly a master dark for UVB/VIS" % locals())
+            if not error:
+                for i in imageTypes:
+                    if i not in ["OBJECT", "LAMP,FLAT", "BIAS", "DARK"]:
+                        error = "Input frames for soxspipe stare need to be ********* and a master-bias and possibly a master dark for UVB/VIS" % locals()
+
+            if not error:
+                for i in [f"MASTER_BIAS_{self.arm}", f"DISP_TAB_{self.arm}"]:
+                    if i not in imageCat:
+                        error = "Input frames for soxspipe stare need to be ********* and a master-bias and possibly a master dark for UVB/VIS" % locals()
 
         # LOOK FOR ****
         arm = self.arm
         # if arm not in self.supplementaryInput or "DISP_MAP" not in self.supplementaryInput[arm]:
         #     raise TypeError(
         #         "Need a **** for %(arm)s - none found with the input files" % locals())
 
+        if error:
+            sys.stdout.write("\x1b[1A\x1b[2K")
+            print("# VERIFYING INPUT FRAMES - **ERROR**\n")
+            print(self.inputFrames.summary)
+            print()
+            raise TypeError(error)
+
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
             self):
         """*The code to generate the product of the soxs_stare recipe*
@@ -267,15 +280,15 @@
             sofName=self.sofName,
             recipeName=self.recipeName
         )
         skymodelCCDData, skySubtractedCCDData, self.qc, self.products = skymodel.subtract()
 
         from os.path import expanduser
         home = expanduser("~")
-        fileDir = self.settings["intermediate-data-root"].replace("~", home)
+        fileDir = self.settings["workspace-root-dir"].replace("~", home)
         # filename = "/override/filename.fits"
         filepath = self._write(combined_object, fileDir, filename="combined_object_frame.fits", overwrite=True)
         # print(f"\nxxx frame saved to {filepath}\n")
 
         # ADD QUALITY CHECKS
         self.qc = generic_quality_checks(
             log=self.log, frame=skySubtractedCCDData, settings=self.settings, recipeName=self.recipeName, qcTable=self.qc)
```

### Comparing `soxspipe-0.7.2/soxspipe/resources/soxs_detector_parameters.yaml` & `soxspipe-0.8.0/soxspipe/resources/soxs_detector_parameters.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/soxs_keywords.yaml` & `soxspipe-0.8.0/soxspipe/resources/soxs_keywords.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/soxs/BP_MAP_RP_NIR.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/soxs/BP_MAP_RP_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/soxs/SOXS_PINHOLE_TAB_NIR.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/soxs/SOXS_PINHOLE_TAB_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/soxs/SOXS_PINHOLE_TAB_NIR_OLD.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/soxs/SOXS_PINHOLE_TAB_NIR_OLD.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/soxs/SOXS_SPECTRAL_FORMAT_TAB_NIR.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/soxs/SOXS_SPECTRAL_FORMAT_TAB_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/soxs/skylines.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/soxs/skylines.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_NIR.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x1.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x1.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x2.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_2x2.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_2x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x1.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x1.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x2.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_2x2.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_2x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_NIR.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_UVB.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_UVB.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_VIS.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_VIS.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_NIR.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x1.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x1.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x2.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_2x2.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_2x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x1.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x1.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x2.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_2x2.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_2x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_NIR.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x1.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x1.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x2.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_2x2.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_2x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x1.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x1.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x2.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_2x2.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_2x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/static_calibrations/xsh/skylines.fits` & `soxspipe-0.8.0/soxspipe/resources/static_calibrations/xsh/skylines.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/xsh_detector_parameters.yaml` & `soxspipe-0.8.0/soxspipe/resources/xsh_detector_parameters.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/resources/xsh_keywords.yaml` & `soxspipe-0.8.0/soxspipe/resources/xsh_keywords.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/setup.cfg` & `soxspipe-0.8.0/soxspipe/setup.cfg`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe/test_settings_soxs.yaml` & `soxspipe-0.8.0/soxspipe/test_settings_soxs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 # # UTILS
 # background-subtraction:
 #     bspline-deg: 3
 #     median-filter-pixels: 11
 
 # test-data-root: ~/xshooter-pipeline-data/unittest_data
-intermediate-data-root: ~/soxspipe-unittests/intermediate/soxs
+workspace-root-dir: ~/soxspipe-unittests/intermediate/soxs
 reduced-data-root: ~/soxspipe-unittests/reduced/soxs
 
 # INTERMEDIATE DATA PRODUCTS CAN CONSUME A LOT OF STORAGE SPACE - BE WARNED
 save-intermediate-products: True
 
 logging settings:
     formatters:
```

### Comparing `soxspipe-0.7.2/soxspipe/test_settings_soxs_sim.yaml` & `soxspipe-0.8.0/soxspipe/test_settings_soxs_sim.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     bspline-deg: 2
     median-filter-pixels: 9
 
 
 data-extension: 1
 
 # test-data-root: ~/xshooter-pipeline-data/unittest_data
-intermediate-data-root: ~/soxspipe-unittests/intermediate/soxs_sim
+workspace-root-dir: ~/soxspipe-unittests/intermediate/soxs_sim
 reduced-data-root: ~/soxspipe-unittests/reduced/soxs_sim
 
 # INTERMEDIATE DATA PRODUCTS CAN CONSUME A LOT OF STORAGE SPACE - BE WARNED
 save-intermediate-products: True
 
 logging settings:
     formatters:
```

### Comparing `soxspipe-0.7.2/soxspipe/test_settings_xsh.yaml` & `soxspipe-0.8.0/soxspipe/test_settings_xsh.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -78,37 +78,38 @@
     # number of σ deviations from the median *pixel* flux beyond which pixel is excluded from stack
     stacked-clipping-sigma: 5
     # number of σ-clipping iterations to perform before stacking
     stacked-clipping-iterations: 5
     # number of σ below the median *frame* flux beyond which pixel is added to the bad-pixel mask
     clipping-lower-sigma: 50
     # number of σ above the median *frame* flux beyond which pixel is added to the bad-pixel mask
-    clipping-upper-sigma: 100   
+    clipping-upper-sigma: 1000   
     # number of sigma-clipping iterations to perform when added pixels to the bad-pixel mask
-    clipping-iteration-count: 0
+    clipping-iteration-count: 1
     # width of the slice to cut along the centre of each order when determining mean exposure level
-    centre-order-window: 13
+    centre-order-window: 20
     # length of image slice to take across orders when detecting edges
     slice-length-for-edge-detection: 90
     # width of image slice to take across orders when detecting edges
     slice-width-for-edge-detection: 5
     # minimum value flux can drop to as percentage of central flux and be counted as an order edge
     min-percentage-threshold-for-edge-detection: 20
     # maximum value flux can claim to as percentage of central flux and be counted as an order edge
     max-percentage-threshold-for-edge-detection: 50
     # degree of dispersion axis component of polynomal fit to order edges
-    disp-axis-deg: 3
+    disp-axis-deg: 5
     # degree of order component of polynomal fit to order edges
     order-deg: 3
     # number of σ deviations from the median fit residual beyond which individual data points are removed when iterating towards a fit of order edges
-    poly-fitting-residual-clipping-sigma: 3.0
+    poly-fitting-residual-clipping-sigma: 5
     # number of sigma-clipping iterations to perform before settings on a polynomial fit for the order edges
-    poly-clipping-iteration-limit: 2
+    poly-clipping-iteration-limit: 3
     # number of σ deviations below the median flux of a master-flat frame beyond which a pixel is added to the bad-pixel mask
     low-sensitivity-clipping-sigma: 2
+
     
 soxs-stare:
     # number of σ deviations from the median *pixel* flux beyond which pixel is excluded from stack
     stacked-clipping-sigma: 5
     # number of σ-clipping iterations to perform before stacking
     stacked-clipping-iterations: 5
     # number of σ below the median *frame* flux beyond which pixel is added to the bad-pixel mask
@@ -153,15 +154,15 @@
 
 # UTILS
 background-subtraction:
     bspline-deg: 2
     median-filter-pixels: 9
 
 test-data-root: ~/xshooter-pipeline-data/unittest_data/xsh
-intermediate-data-root: ~/soxspipe-unittests/intermediate/xsh
+workspace-root-dir: ~/soxspipe-unittests/intermediate/xsh
 reduced-data-root: ~/soxspipe-unittests/reduced/xsh
 
 
 
 data-extension: 0
 
 # INTERMEDIATE DATA PRODUCTS CAN CONSUME A LOT OF STORAGE SPACE - BE WARNED
```

### Comparing `soxspipe-0.7.2/soxspipe/utKit.py` & `soxspipe-0.8.0/soxspipe/utKit.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.7.2/soxspipe.egg-info/PKG-INFO` & `soxspipe-0.8.0/soxspipe.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: soxspipe
-Version: 0.7.2
+Version: 0.8.0
 Summary: A python package and command-line tools to The data-reduction pipeline for the SOXS instrument
 Home-page: https://github.com/thespacedoctor/soxspipe
-Download-URL: https://github.com/thespacedoctor/soxspipe/archive/v0.7.2.zip
+Download-URL: https://github.com/thespacedoctor/soxspipe/archive/v0.8.0.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: MIT
 Keywords: soxs, eso, data, pipeline, spectra
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # soxspipe
 
 <!-- INFO BADGES -->  
@@ -34,11 +34,8 @@
 [![](https://img.shields.io/github/issues/thespacedoctor/soxspipe/type:%20bug?label=bug%20issues)](https://github.com/thespacedoctor/soxspipe/issues?q=is%3Aissue+is%3Aopen+label%3A%22type%3A+bug%22+)
 
 *The data-reduction pipeline for the SOXS instrument* (a python package with command-line tools).
 
 Documentation for soxspipe is hosted by [Read the Docs](https://soxspipe.readthedocs.io/en/master/) ([development version](https://soxspipe.readthedocs.io/en/develop/) and [master version](https://soxspipe.readthedocs.io/en/master/)). The code lives on [github](https://github.com/thespacedoctor/soxspipe). Please report any issues you find [here](https://github.com/thespacedoctor/soxspipe/issues).
 
 
-## Features
-
-*
```

### Comparing `soxspipe-0.7.2/soxspipe.egg-info/SOURCES.txt` & `soxspipe-0.8.0/soxspipe.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.md
 setup.py
 soxspipe/__init__.py
 soxspipe/__version__.py
 soxspipe/advanced_settings.yaml
 soxspipe/cl_utils.py
 soxspipe/default_settings.yaml
+soxspipe/pandas_export.db
 soxspipe/setup.cfg
 soxspipe/test_settings_soxs.yaml
 soxspipe/test_settings_soxs_sim.yaml
 soxspipe/test_settings_xsh.yaml
 soxspipe/utKit.py
 soxspipe.egg-info/PKG-INFO
 soxspipe.egg-info/SOURCES.txt
@@ -20,39 +21,42 @@
 soxspipe.egg-info/entry_points.txt
 soxspipe.egg-info/not-zip-safe
 soxspipe.egg-info/requires.txt
 soxspipe.egg-info/top_level.txt
 soxspipe/commonutils/__init__.py
 soxspipe/commonutils/combiner.py
 soxspipe/commonutils/create_dispersion_map.py
+soxspipe/commonutils/data_organiser.md
+soxspipe/commonutils/data_organiser.py
 soxspipe/commonutils/detect_continuum.py
 soxspipe/commonutils/detect_order_edges.py
 soxspipe/commonutils/detector_lookup.py
 soxspipe/commonutils/dispersion_map_to_pixel_arrays.py
 soxspipe/commonutils/filenamer.py
 soxspipe/commonutils/getpackagepath.py
 soxspipe/commonutils/keyword_lookup.py
 soxspipe/commonutils/polynomials.py
 soxspipe/commonutils/set_of_files.py
 soxspipe/commonutils/subtract_background.py
 soxspipe/commonutils/subtract_sky.py
 soxspipe/commonutils/toolkit.py
+soxspipe/commonutils/uncompress.py
 soxspipe/recipes/__init__.py
 soxspipe/recipes/_base_recipe_.py
 soxspipe/recipes/soxs_disp_solution.py
 soxspipe/recipes/soxs_mbias.py
 soxspipe/recipes/soxs_mdark.py
 soxspipe/recipes/soxs_mflat.py
-soxspipe/recipes/soxs_nod_mode.py
 soxspipe/recipes/soxs_order_centres.py
 soxspipe/recipes/soxs_spatial_solution.py
 soxspipe/recipes/soxs_stare.py
 soxspipe/recipes/soxs_straighten.py
 soxspipe/resources/soxs_detector_parameters.yaml
 soxspipe/resources/soxs_keywords.yaml
+soxspipe/resources/soxspipe.db
 soxspipe/resources/xsh_detector_parameters.yaml
 soxspipe/resources/xsh_keywords.yaml
 soxspipe/resources/static_calibrations/soxs/BP_MAP_RP_NIR.fits
 soxspipe/resources/static_calibrations/soxs/SOXS_PINHOLE_TAB_NIR.fits
 soxspipe/resources/static_calibrations/soxs/SOXS_PINHOLE_TAB_NIR_OLD.fits
 soxspipe/resources/static_calibrations/soxs/SOXS_SPECTRAL_FORMAT_TAB_NIR.fits
 soxspipe/resources/static_calibrations/soxs/skylines.fits
```

