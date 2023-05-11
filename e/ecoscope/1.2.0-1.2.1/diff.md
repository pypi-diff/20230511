# Comparing `tmp/ecoscope-1.2.0.tar.gz` & `tmp/ecoscope-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoscope-1.2.0.tar", last modified: Tue May  9 13:40:43 2023, max compression
+gzip compressed data, was "ecoscope-1.2.1.tar", last modified: Thu May 11 03:37:25 2023, max compression
```

## Comparing `ecoscope-1.2.0.tar` & `ecoscope-1.2.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.949401 ecoscope-1.2.0/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2023-05-09 13:36:07.000000 ecoscope-1.2.0/LICENSE
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-05-09 13:40:43.949401 ecoscope-1.2.0/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2935 2023-05-09 13:36:07.000000 ecoscope-1.2.0/README.rst
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.941401 ecoscope-1.2.0/ecoscope/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3744 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/__init__.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.945401 ecoscope-1.2.0/ecoscope/analysis/
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.945401 ecoscope-1.2.0/ecoscope/analysis/UD/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/UD/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/UD/etd_range.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/astronomy.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3881 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/percentile.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/proximity.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3505 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2735 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/analysis/speed.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.945401 ecoscope-1.2.0/ecoscope/base/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/base/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/base/_dataclasses.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25180 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/base/base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6650 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/base/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.945401 ecoscope-1.2.0/ecoscope/contrib/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       60 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/contrib/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/contrib/basemaps.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   112572 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/contrib/foliumap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2197 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/contrib/legend.txt
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.945401 ecoscope-1.2.0/ecoscope/io/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/io/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    32507 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/io/earthranger.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    12171 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/io/eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6620 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/io/raster.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2225 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/io/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.949401 ecoscope-1.2.0/ecoscope/mapping/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      141 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/mapping/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    17821 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/mapping/map.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.949401 ecoscope-1.2.0/ecoscope/plotting/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      376 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/plotting/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    14348 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/plotting/plot.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2023-05-09 13:36:07.000000 ecoscope-1.2.0/ecoscope/version.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.945401 ecoscope-1.2.0/ecoscope.egg-info/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-05-09 13:40:43.000000 ecoscope-1.2.0/ecoscope.egg-info/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1322 2023-05-09 13:40:43.000000 ecoscope-1.2.0/ecoscope.egg-info/SOURCES.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-09 13:40:43.000000 ecoscope-1.2.0/ecoscope.egg-info/dependency_links.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-09 13:40:43.000000 ecoscope-1.2.0/ecoscope.egg-info/not-zip-safe
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      284 2023-05-09 13:40:43.000000 ecoscope-1.2.0/ecoscope.egg-info/requires.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2023-05-09 13:40:43.000000 ecoscope-1.2.0/ecoscope.egg-info/top_level.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2023-05-09 13:36:07.000000 ecoscope-1.2.0/pyproject.toml
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2023-05-09 13:40:43.949401 ecoscope-1.2.0/setup.cfg
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1940 2023-05-09 13:36:07.000000 ecoscope-1.2.0/setup.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-09 13:40:43.949401 ecoscope-1.2.0/tests/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6080 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6908 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_earthranger_io.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_ecodataframe.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5098 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_ecomap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2907 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      862 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_speed.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1877 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_ud.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      329 2023-05-09 13:36:07.000000 ecoscope-1.2.0/tests/test_utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.649143 ecoscope-1.2.1/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2023-05-10 19:33:30.000000 ecoscope-1.2.1/LICENSE
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-05-11 03:37:25.649143 ecoscope-1.2.1/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2935 2023-05-10 19:33:30.000000 ecoscope-1.2.1/README.rst
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.641143 ecoscope-1.2.1/ecoscope/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3744 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/__init__.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.641143 ecoscope-1.2.1/ecoscope/analysis/
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.645143 ecoscope-1.2.1/ecoscope/analysis/UD/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/UD/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/UD/etd_range.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/astronomy.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3881 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/percentile.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/proximity.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3505 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2735 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/analysis/speed.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.645143 ecoscope-1.2.1/ecoscope/base/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/base/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/base/_dataclasses.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25180 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/base/base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6650 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/base/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.645143 ecoscope-1.2.1/ecoscope/contrib/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       60 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/contrib/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/contrib/basemaps.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   112572 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/contrib/foliumap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2197 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/contrib/legend.txt
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.645143 ecoscope-1.2.1/ecoscope/io/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/io/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    32515 2023-05-11 03:31:13.000000 ecoscope-1.2.1/ecoscope/io/earthranger.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    12171 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/io/eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6620 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/io/raster.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2225 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/io/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.645143 ecoscope-1.2.1/ecoscope/mapping/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      141 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/mapping/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    17821 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/mapping/map.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.645143 ecoscope-1.2.1/ecoscope/plotting/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      376 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/plotting/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    14348 2023-05-10 19:33:30.000000 ecoscope-1.2.1/ecoscope/plotting/plot.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2023-05-10 19:34:04.000000 ecoscope-1.2.1/ecoscope/version.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.641143 ecoscope-1.2.1/ecoscope.egg-info/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-05-11 03:37:25.000000 ecoscope-1.2.1/ecoscope.egg-info/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1322 2023-05-11 03:37:25.000000 ecoscope-1.2.1/ecoscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-11 03:37:25.000000 ecoscope-1.2.1/ecoscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-11 03:37:25.000000 ecoscope-1.2.1/ecoscope.egg-info/not-zip-safe
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      284 2023-05-11 03:37:25.000000 ecoscope-1.2.1/ecoscope.egg-info/requires.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2023-05-11 03:37:25.000000 ecoscope-1.2.1/ecoscope.egg-info/top_level.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2023-05-10 19:33:30.000000 ecoscope-1.2.1/pyproject.toml
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2023-05-11 03:37:25.649143 ecoscope-1.2.1/setup.cfg
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1940 2023-05-10 19:33:30.000000 ecoscope-1.2.1/setup.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-11 03:37:25.649143 ecoscope-1.2.1/tests/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6554 2023-05-11 03:34:07.000000 ecoscope-1.2.1/tests/test_base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6922 2023-05-10 19:42:08.000000 ecoscope-1.2.1/tests/test_earthranger_io.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_ecodataframe.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5098 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_ecomap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2907 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      862 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_speed.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1877 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_ud.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      329 2023-05-10 19:33:31.000000 ecoscope-1.2.1/tests/test_utils.py
```

### Comparing `ecoscope-1.2.0/LICENSE` & `ecoscope-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/PKG-INFO` & `ecoscope-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.2.0
+Version: 1.2.1
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.2.0/README.rst` & `ecoscope-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/__init__.py` & `ecoscope-1.2.1/ecoscope/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/analysis/UD/etd_range.py` & `ecoscope-1.2.1/ecoscope/analysis/UD/etd_range.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/analysis/astronomy.py` & `ecoscope-1.2.1/ecoscope/analysis/astronomy.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/analysis/ecograph.py` & `ecoscope-1.2.1/ecoscope/analysis/ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/analysis/geofence.py` & `ecoscope-1.2.1/ecoscope/analysis/geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/analysis/immobility.py` & `ecoscope-1.2.1/ecoscope/analysis/immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/analysis/percentile.py` & `ecoscope-1.2.1/ecoscope/analysis/percentile.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/analysis/proximity.py` & `ecoscope-1.2.1/ecoscope/analysis/proximity.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/analysis/seasons.py` & `ecoscope-1.2.1/ecoscope/analysis/seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/analysis/speed.py` & `ecoscope-1.2.1/ecoscope/analysis/speed.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/base/__init__.py` & `ecoscope-1.2.1/ecoscope/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/base/_dataclasses.py` & `ecoscope-1.2.1/ecoscope/base/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/base/base.py` & `ecoscope-1.2.1/ecoscope/base/base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/base/utils.py` & `ecoscope-1.2.1/ecoscope/base/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/contrib/basemaps.py` & `ecoscope-1.2.1/ecoscope/contrib/basemaps.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/contrib/foliumap.py` & `ecoscope-1.2.1/ecoscope/contrib/foliumap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/contrib/legend.txt` & `ecoscope-1.2.1/ecoscope/contrib/legend.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/io/earthranger.py` & `ecoscope-1.2.1/ecoscope/io/earthranger.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
                 left_on=["id", "source"],
                 right_on=["subjectsource__subject", "subjectsource__source"],
             )
 
         if relocations:
             return ecoscope.base.Relocations.from_gdf(
                 observations,
-                groupby_col="id",
+                groupby_col="subject_id",
                 uuid_col="id",
                 time_col="recorded_at",
             )
         else:
             return observations
 
     def get_subjectsource_observations(
```

### Comparing `ecoscope-1.2.0/ecoscope/io/eetools.py` & `ecoscope-1.2.1/ecoscope/io/eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/io/raster.py` & `ecoscope-1.2.1/ecoscope/io/raster.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/io/utils.py` & `ecoscope-1.2.1/ecoscope/io/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/mapping/map.py` & `ecoscope-1.2.1/ecoscope/mapping/map.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope/plotting/plot.py` & `ecoscope-1.2.1/ecoscope/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/ecoscope.egg-info/PKG-INFO` & `ecoscope-1.2.1/ecoscope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.2.0
+Version: 1.2.1
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.2.0/ecoscope.egg-info/SOURCES.txt` & `ecoscope-1.2.1/ecoscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/pyproject.toml` & `ecoscope-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/setup.py` & `ecoscope-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/tests/test_base.py` & `ecoscope-1.2.1/tests/test_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,38 +4,49 @@
 import pandas as pd
 import pandas.testing
 import pytest
 
 import ecoscope
 
 
-def test_redundant_columns_in_trajectory(movbank_relocations):
+def test_trajectory_is_not_empty(er_io):
+    # test there is actually data in trajectory
+    relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
+    trajectory = ecoscope.base.Trajectory.from_relocations(relocations)
+    assert not trajectory.empty
+
+
+def test_redundant_columns_in_trajectory(er_io):
     # test there is no redundant column in trajectory
-    trajectory = ecoscope.base.Trajectory.from_relocations(movbank_relocations)
+    relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
+    trajectory = ecoscope.base.Trajectory.from_relocations(relocations)
     assert "extra__fixtime" not in trajectory
     assert "extra___fixtime" not in trajectory
     assert "extra___geometry" not in trajectory
 
 
-def test_relocs_speedfilter(movbank_relocations):
+def test_relocs_speedfilter(er_io):
+    relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
     relocs_speed_filter = ecoscope.base.RelocsSpeedFilter(max_speed_kmhr=8)
-    relocs_after_filter = movbank_relocations.apply_reloc_filter(relocs_speed_filter)
+    relocs_after_filter = relocations.apply_reloc_filter(relocs_speed_filter)
     relocs_after_filter.remove_filtered(inplace=True)
-    assert movbank_relocations.shape[0] != relocs_after_filter.shape[0]
+    assert relocations.shape[0] != relocs_after_filter.shape[0]
 
 
-def test_relocs_distancefilter(movbank_relocations):
+def test_relocs_distancefilter(er_io):
+    relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
     relocs_speed_filter = ecoscope.base.RelocsDistFilter(min_dist_km=1.0, max_dist_km=6.0)
-    relocs_after_filter = movbank_relocations.apply_reloc_filter(relocs_speed_filter)
+    relocs_after_filter = relocations.apply_reloc_filter(relocs_speed_filter)
     relocs_after_filter.remove_filtered(inplace=True)
-    assert movbank_relocations.shape[0] != relocs_after_filter.shape[0]
+    assert relocations.shape[0] != relocs_after_filter.shape[0]
 
 
-def test_relocations_from_gdf_preserve_fields(movbank_relocations):
-    gpd.testing.assert_geodataframe_equal(movbank_relocations, ecoscope.base.Relocations.from_gdf(movbank_relocations))
+def test_relocations_from_gdf_preserve_fields(er_io):
+    relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
+    gpd.testing.assert_geodataframe_equal(relocations, ecoscope.base.Relocations.from_gdf(relocations))
 
 
 def test_displacement_property(movbank_relocations):
     trajectory = ecoscope.base.Trajectory.from_relocations(movbank_relocations)
     expected = pd.Series(
         [2633.760505, 147749.545621],
         index=pd.Index(["Habiba", "Salif Keita"], name="groupby_col"),
@@ -111,17 +122,17 @@
         max_x=1,
         min_y=12,
         max_y=18,
         filter_point_coords=[[180, 90], [0, 0]],
     )
     movbank_relocations.apply_reloc_filter(pnts_filter, inplace=True)
     movbank_relocations.remove_filtered(inplace=True)
-    movbank_trajectory = ecoscope.base.Trajectory.from_relocations(movbank_relocations)
-    downsampled_relocs_noint = movbank_trajectory.downsample("10800S", tolerance="900S")
-    downsampled_relocs_int = movbank_trajectory.downsample("10800S", interpolation=True)
+    trajectory = ecoscope.base.Trajectory.from_relocations(movbank_relocations)
+    downsampled_relocs_noint = trajectory.downsample("10800S", tolerance="900S")
+    downsampled_relocs_int = trajectory.downsample("10800S", interpolation=True)
 
     expected_noncontiguous_1 = gpd.read_feather("tests/test_output/upsampled_noncontiguous_1.feather")
     expected_noncontiguous_2 = gpd.read_feather("tests/test_output/upsampled_noncontiguous_2.feather")
     expected_downsample_noint = gpd.read_feather("tests/test_output/downsampled_relocs_noint.feather")
     expected_downsample_int = gpd.read_feather("tests/test_output/downsampled_relocs.feather")
 
     gpd.testing.assert_geodataframe_equal(upsampled_noncontiguous_1, expected_noncontiguous_1, check_less_precise=True)
```

### Comparing `ecoscope-1.2.0/tests/test_earthranger_io.py` & `ecoscope-1.2.1/tests/test_earthranger_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,16 +67,16 @@
 
 
 def test_get_subjectgroup_observations(er_io):
     relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
     assert "groupby_col" in relocations
 
 
-def test_get_events(er_io):
-    events = er_io.get_events()
+def test_get_events(er_events_io):
+    events = er_events_io.get_events()
     assert not events.empty
 
 
 @pytest.mark.filterwarnings("ignore:All-NaN slice encountered:RuntimeWarning")
 @pytest.mark.filterwarnings("ignore:Mean of empty slice:RuntimeWarning")
 def test_collar_voltage(er_io):
     start_time = pytz.utc.localize(datetime.datetime.now() - datetime.timedelta(days=31))
```

### Comparing `ecoscope-1.2.0/tests/test_ecodataframe.py` & `ecoscope-1.2.1/tests/test_ecodataframe.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/tests/test_ecograph.py` & `ecoscope-1.2.1/tests/test_ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/tests/test_eetools.py` & `ecoscope-1.2.1/tests/test_eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/tests/test_geofence.py` & `ecoscope-1.2.1/tests/test_geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/tests/test_immobility.py` & `ecoscope-1.2.1/tests/test_immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/tests/test_seasons.py` & `ecoscope-1.2.1/tests/test_seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.2.0/tests/test_ud.py` & `ecoscope-1.2.1/tests/test_ud.py`

 * *Files identical despite different names*

