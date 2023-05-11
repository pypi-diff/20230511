# Comparing `tmp/ctapipe-0.8.0.tar.gz` & `tmp/ctapipe-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ctapipe-0.8.0.tar", last modified: Mon Jun 15 14:18:23 2020, max compression
+gzip compressed data, was "dist/ctapipe-0.9.1.tar", last modified: Fri Oct 23 13:46:11 2020, max compression
```

## Comparing `ctapipe-0.8.0.tar` & `ctapipe-0.9.1.tar`

### file list

```diff
@@ -1,420 +1,425 @@
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.658720 ctapipe-0.8.0/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       96 2020-03-18 13:27:32.000000 ctapipe-0.8.0/.codacy.yml
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.468723 ctapipe-0.8.0/.github/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      100 2020-03-18 13:27:32.000000 ctapipe-0.8.0/.github/release-drafter.yml
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1075 2020-05-15 13:48:03.000000 ctapipe-0.8.0/.gitignore
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/.gitmodules
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      203 2020-03-18 13:27:32.000000 ctapipe-0.8.0/.landscape.yml
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3949 2020-05-22 10:09:37.000000 ctapipe-0.8.0/.mailmap
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2298 2020-05-20 09:58:30.000000 ctapipe-0.8.0/.travis.yml
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1835 2020-03-18 13:27:32.000000 ctapipe-0.8.0/AUTHORS
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      376 2020-05-12 16:04:51.000000 ctapipe-0.8.0/CODEOWNERS
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11223 2020-03-18 13:27:32.000000 ctapipe-0.8.0/History.md
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1556 2020-03-18 13:27:32.000000 ctapipe-0.8.0/LICENSE
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      275 2020-05-15 13:48:03.000000 ctapipe-0.8.0/MANIFEST.in
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1592 2020-03-18 13:27:32.000000 ctapipe-0.8.0/Makefile
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3764 2020-06-15 14:18:23.658720 ctapipe-0.8.0/PKG-INFO
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2465 2020-05-11 13:28:39.000000 ctapipe-0.8.0/README.rst
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.468723 ctapipe-0.8.0/ci/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1027 2020-05-19 15:15:37.000000 ctapipe-0.8.0/ci/install.sh
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.468723 ctapipe-0.8.0/ctapipe/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      195 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       16 2020-06-15 14:18:23.000000 ctapipe-0.8.0/ctapipe/_version_cache.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.468723 ctapipe-0.8.0/ctapipe/analysis/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      104 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/analysis/__init__.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.468723 ctapipe-0.8.0/ctapipe/analysis/camera/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      102 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/analysis/camera/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4497 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/analysis/camera/charge_resolution.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.468723 ctapipe-0.8.0/ctapipe/analysis/camera/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/analysis/camera/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3450 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/analysis/camera/tests/test_charge_resolution.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.468723 ctapipe-0.8.0/ctapipe/analysis/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/analysis/tests/__init__.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.468723 ctapipe-0.8.0/ctapipe/calib/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      106 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/calib/__init__.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.472056 ctapipe-0.8.0/ctapipe/calib/camera/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      229 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/calib/camera/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5843 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/calib/camera/calibrator.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13707 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/calib/camera/flatfield.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2888 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/calib/camera/gainselection.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13172 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/calib/camera/pedestals.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.472056 ctapipe-0.8.0/ctapipe/calib/camera/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/calib/camera/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5300 2020-05-20 17:26:03.000000 ctapipe-0.8.0/ctapipe/calib/camera/tests/test_calibrator.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3059 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/calib/camera/tests/test_flatfield.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1759 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/calib/camera/tests/test_gainselection.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2627 2020-05-11 13:28:39.000000 ctapipe-0.8.0/ctapipe/calib/camera/tests/test_pedestals.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.472056 ctapipe-0.8.0/ctapipe/calib/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/calib/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1311 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/conftest.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    31405 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/containers.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.472056 ctapipe-0.8.0/ctapipe/coordinates/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1890 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/coordinates/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7301 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/coordinates/camera_frame.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6285 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/coordinates/ground_frames.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3353 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/coordinates/nominal_frame.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2407 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/coordinates/representation.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3713 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/coordinates/telescope_frame.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.472056 ctapipe-0.8.0/ctapipe/coordinates/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/coordinates/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6294 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/coordinates/tests/test_coordinates.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      954 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/coordinates/tests/test_engineering_frame.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2515 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/coordinates/tests/test_nominal_frame.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1143 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/coordinates/tests/test_roundtrip.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2719 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/coordinates/tests/test_telescope_frame.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.475389 ctapipe-0.8.0/ctapipe/core/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      765 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/core/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7517 2020-05-07 07:38:00.000000 ctapipe-0.8.0/ctapipe/core/component.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13141 2020-05-20 09:58:30.000000 ctapipe-0.8.0/ctapipe/core/container.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1131 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/core/logging.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      438 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/core/plugins.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10392 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/core/provenance.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4651 2020-04-08 12:18:28.000000 ctapipe-0.8.0/ctapipe/core/qualityquery.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      240 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/core/support.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.475389 ctapipe-0.8.0/ctapipe/core/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       47 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/core/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     9990 2020-03-18 13:31:42.000000 ctapipe-0.8.0/ctapipe/core/tests/test_component.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6916 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/core/tests/test_container.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1221 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/core/tests/test_provenance.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3069 2020-04-08 12:18:28.000000 ctapipe-0.8.0/ctapipe/core/tests/test_qualityquery.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3858 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/core/tests/test_tool.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11425 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/core/tests/test_traits.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13575 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/core/tool.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    14320 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/core/traits.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.478722 ctapipe-0.8.0/ctapipe/image/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      554 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    15480 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/cleaning.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1396 2020-06-15 14:17:32.000000 ctapipe-0.8.0/ctapipe/image/concentration.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    37997 2020-06-04 10:33:53.000000 ctapipe-0.8.0/ctapipe/image/extractor.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      376 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/geometry_converter.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6544 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/geometry_converter_astri.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1416 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/image/geometry_converter_chec.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    19708 2020-05-11 13:28:39.000000 ctapipe-0.8.0/ctapipe/image/geometry_converter_hex.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5515 2020-06-04 10:33:53.000000 ctapipe-0.8.0/ctapipe/image/hillas.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1291 2020-05-11 13:28:39.000000 ctapipe-0.8.0/ctapipe/image/leakage.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3774 2020-06-15 14:17:32.000000 ctapipe-0.8.0/ctapipe/image/morphology.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.478722 ctapipe-0.8.0/ctapipe/image/muon/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      261 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/muon/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4273 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/muon/features.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3228 2020-05-11 13:28:39.000000 ctapipe-0.8.0/ctapipe/image/muon/fitting.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    16866 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/muon/intensity_fitter.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1649 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/muon/ring_fitter.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.478722 ctapipe-0.8.0/ctapipe/image/muon/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3128 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/muon/tests/test_intensity_fit.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1320 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/muon/tests/test_muon_features.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1278 2020-04-06 15:46:15.000000 ctapipe-0.8.0/ctapipe/image/muon/tests/test_muon_fitting.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1360 2020-05-11 13:28:39.000000 ctapipe-0.8.0/ctapipe/image/muon/tests/test_ring_fitter.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11461 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/pixel_likelihood.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5562 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/reducer.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2414 2020-06-04 10:33:53.000000 ctapipe-0.8.0/ctapipe/image/statistics.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.478722 ctapipe-0.8.0/ctapipe/image/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/image/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     8528 2020-05-19 15:15:37.000000 ctapipe-0.8.0/ctapipe/image/tests/test_cleaning.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      856 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/tests/test_concentration.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    12907 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/tests/test_extractor.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4164 2020-06-04 10:33:53.000000 ctapipe-0.8.0/ctapipe/image/tests/test_geometry_converter.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7184 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/tests/test_hillas.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1741 2020-04-08 12:18:28.000000 ctapipe-0.8.0/ctapipe/image/tests/test_image_cleaner_component.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      591 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/tests/test_leakage.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3725 2020-06-15 14:17:32.000000 ctapipe-0.8.0/ctapipe/image/tests/test_morphology.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1519 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/tests/test_pixel_likelihood.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3026 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/tests/test_reducer.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1980 2020-05-22 10:09:37.000000 ctapipe-0.8.0/ctapipe/image/tests/test_statistics.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3035 2020-06-04 10:33:53.000000 ctapipe-0.8.0/ctapipe/image/tests/test_timing_parameters.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6242 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/tests/test_toy.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2319 2020-06-04 10:33:53.000000 ctapipe-0.8.0/ctapipe/image/timing.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    12340 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/image/toymodel.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.482056 ctapipe-0.8.0/ctapipe/instrument/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      512 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1938 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/atmosphere.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.482056 ctapipe-0.8.0/ctapipe/instrument/camera/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      256 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/camera/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2329 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/camera/description.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    25577 2020-05-22 12:41:45.000000 ctapipe-0.8.0/ctapipe/instrument/camera/geometry.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6738 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/camera/readout.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.482056 ctapipe-0.8.0/ctapipe/instrument/camera/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-04-08 12:18:28.000000 ctapipe-0.8.0/ctapipe/instrument/camera/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      439 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/camera/tests/test_description.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10591 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/camera/tests/test_geometry.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5186 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/camera/tests/test_readout.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2341 2020-06-12 10:21:51.000000 ctapipe-0.8.0/ctapipe/instrument/guess.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4195 2020-06-09 14:54:12.000000 ctapipe-0.8.0/ctapipe/instrument/optics.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10645 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/subarray.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2947 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/telescope.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.482056 ctapipe-0.8.0/ctapipe/instrument/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       85 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      586 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/tests/test_guessing.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1375 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/instrument/tests/test_optics.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3795 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/tests/test_subarray.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1490 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/instrument/tests/test_telescope.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.482056 ctapipe-0.8.0/ctapipe/io/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      603 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      827 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/array.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      249 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/datalevels.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10240 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/eventseeker.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10089 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/eventsource.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      577 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/files.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    16736 2020-06-15 14:17:32.000000 ctapipe-0.8.0/ctapipe/io/hdf5tableio.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6005 2020-05-19 15:15:37.000000 ctapipe-0.8.0/ctapipe/io/metadata.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    20152 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/simteleventsource.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5936 2020-06-15 14:17:32.000000 ctapipe-0.8.0/ctapipe/io/tableio.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.482056 ctapipe-0.8.0/ctapipe/io/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/io/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      410 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/io/tests/test_available_sources.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4614 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/tests/test_event_source.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1646 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/tests/test_eventseeker.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      458 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/tests/test_files.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    15392 2020-06-15 14:17:32.000000 ctapipe-0.8.0/ctapipe/io/tests/test_hdf5.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2096 2020-05-11 13:28:39.000000 ctapipe-0.8.0/ctapipe/io/tests/test_metadata.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      466 2020-05-11 13:28:39.000000 ctapipe-0.8.0/ctapipe/io/tests/test_prod2.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11128 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/tests/test_simteleventsource.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1179 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/tests/test_toysource.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4323 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/io/toymodel.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.485389 ctapipe-0.8.0/ctapipe/plotting/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       38 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/plotting/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11933 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/plotting/bokeh_event_viewer.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11003 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/plotting/charge_resolution.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.485389 ctapipe-0.8.0/ctapipe/plotting/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/plotting/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4556 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/plotting/tests/test_bokeh_event_viewer.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3895 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/plotting/tests/test_charge_resolution.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.485389 ctapipe-0.8.0/ctapipe/reco/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    14605 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/HillasReconstructor.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    32665 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/ImPACT.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      401 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6380 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/energy_regressor.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3443 2020-03-18 13:31:42.000000 ctapipe-0.8.0/ctapipe/reco/event_classifier.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    17437 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/hillas_intersection.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      826 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/reco_algorithms.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    16064 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/regressor_classifier_base.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2373 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/shower_max.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.485389 ctapipe-0.8.0/ctapipe/reco/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/reco/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     8499 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/tests/test_HillasReconstructor.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5675 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/tests/test_ImPACT.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1453 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/tests/test_energy_regressor.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6515 2020-03-18 13:31:42.000000 ctapipe-0.8.0/ctapipe/reco/tests/test_event_classifier.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     9235 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/tests/test_hillas_intersection.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2730 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/tests/test_reconstruction_methods.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2448 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/tests/test_regressor_classifier_base.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      748 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/reco/tests/test_showermaxestimator.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.485389 ctapipe-0.8.0/ctapipe/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      768 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/tests/coveragerc
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       87 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tests/setup_package.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.485389 ctapipe-0.8.0/ctapipe/tools/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       99 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/__init__.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.488722 ctapipe-0.8.0/ctapipe/tools/bokeh/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/tools/bokeh/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    12511 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/bokeh/file_viewer.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.488722 ctapipe-0.8.0/ctapipe/tools/bokeh/templates/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      645 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/tools/bokeh/templates/index.html
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      482 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/tools/bokeh/theme.yaml
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6479 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/camdemo.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6795 2020-05-25 18:38:52.000000 ctapipe-0.8.0/ctapipe/tools/display_dl1.py
--rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     6022 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/display_events_single_tel.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10395 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/display_integrator.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3950 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/display_summed_images.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4183 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/dump_instrument.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4711 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/dump_triggers.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4012 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/extract_charge_resolution.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5447 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/info.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10672 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/muon_reconstruction.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1426 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/plot_charge_resolution.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    27734 2020-05-22 13:40:25.000000 ctapipe-0.8.0/ctapipe/tools/stage1.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.488722 ctapipe-0.8.0/ctapipe/tools/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        4 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/tools/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7609 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/tests/test_tools.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1861 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/tools/utils.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.488722 ctapipe-0.8.0/ctapipe/utils/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     8701 2020-04-08 12:18:28.000000 ctapipe-0.8.0/ctapipe/utils/CutFlow.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      707 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2394 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/astro.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6935 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/datasets.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    12920 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/fitshistogram.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1429 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/linalg.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      465 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/utils/quantities.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1797 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/rgbtohex.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5393 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/table_interpolator.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2964 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/template_network_interpolator.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.488722 ctapipe-0.8.0/ctapipe/utils/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/utils/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2054 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/tests/test_CutFlow.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      653 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/tests/test_astro.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2151 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/tests/test_datasets.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3210 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/tests/test_fitshistogram.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      579 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/tests/test_linalg.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      890 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/utils/tests/test_quantities.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      700 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/tests/test_rgbtohex.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6189 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/tests/test_unstructured_interpolator.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     8824 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/utils/unstructured_interpolator.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5656 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/version.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.488722 ctapipe-0.8.0/ctapipe/visualization/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      279 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/visualization/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11473 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/visualization/bokeh.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11185 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/visualization/mpl_array.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    15589 2020-06-04 10:33:53.000000 ctapipe-0.8.0/ctapipe/visualization/mpl_camera.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.488722 ctapipe-0.8.0/ctapipe/visualization/tests/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.8.0/ctapipe/visualization/tests/__init__.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4132 2020-05-20 13:57:20.000000 ctapipe-0.8.0/ctapipe/visualization/tests/test_bokeh.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3248 2020-05-19 15:15:37.000000 ctapipe-0.8.0/ctapipe/visualization/tests/test_mpl.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.468723 ctapipe-0.8.0/ctapipe.egg-info/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3764 2020-06-15 14:18:23.000000 ctapipe-0.8.0/ctapipe.egg-info/PKG-INFO
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11990 2020-06-15 14:18:23.000000 ctapipe-0.8.0/ctapipe.egg-info/SOURCES.txt
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        1 2020-06-15 14:18:23.000000 ctapipe-0.8.0/ctapipe.egg-info/dependency_links.txt
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      803 2020-06-15 14:18:23.000000 ctapipe-0.8.0/ctapipe.egg-info/entry_points.txt
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        1 2020-03-18 13:30:42.000000 ctapipe-0.8.0/ctapipe.egg-info/not-zip-safe
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      623 2020-06-15 14:18:23.000000 ctapipe-0.8.0/ctapipe.egg-info/requires.txt
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        8 2020-06-15 14:18:23.000000 ctapipe-0.8.0/ctapipe.egg-info/top_level.txt
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.495389 ctapipe-0.8.0/docs/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2033 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/FAQ.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      604 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/Makefile
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.495389 ctapipe-0.8.0/docs/_static/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      365 2020-05-19 15:15:37.000000 ctapipe-0.8.0/docs/_static/theme_overrides.css
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.462056 ctapipe-0.8.0/docs/_templates/
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.495389 ctapipe-0.8.0/docs/_templates/autosummary/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      250 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      251 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      252 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      767 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/bibliography.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   242690 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/cameras.png
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5378 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/changelog.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7367 2020-05-22 10:09:37.000000 ctapipe-0.8.0/docs/conf.py
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.498722 ctapipe-0.8.0/docs/ctapipe_api/
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.498722 ctapipe-0.8.0/docs/ctapipe_api/analysis/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      344 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/analysis/index.rst
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.498722 ctapipe-0.8.0/docs/ctapipe_api/calib/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      714 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/ctapipe_api/calib/index.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1096 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/ctapipe_api/calib/index_camera.rst
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.498722 ctapipe-0.8.0/docs/ctapipe_api/containers/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      384 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/ctapipe_api/containers/index.rst
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.498722 ctapipe-0.8.0/docs/ctapipe_api/coordinates/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1542 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/coordinates/index.rst
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.498722 ctapipe-0.8.0/docs/ctapipe_api/core/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      592 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/core/corediagram.dot
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1271 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/core/index.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   116209 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/core/tool-component.pdf
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    37376 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/core/tool-component.png
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.502056 ctapipe-0.8.0/docs/ctapipe_api/image/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      310 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/image/cleaning.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    93504 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/image/dilate.png
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3182 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/ctapipe_api/image/extractor.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      236 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/image/geometry_converter.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      131 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/image/hillas.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      820 2020-04-08 13:37:54.000000 ctapipe-0.8.0/docs/ctapipe_api/image/index.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      173 2020-04-08 13:37:54.000000 ctapipe-0.8.0/docs/ctapipe_api/image/muon.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      166 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/image/pixel_likelihood.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      237 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/image/reducers.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      194 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/image/toymodel.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       79 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/index.rst
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.505389 ctapipe-0.8.0/docs/ctapipe_api/instrument/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      314 2020-04-08 12:18:28.000000 ctapipe-0.8.0/docs/ctapipe_api/instrument/camera.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3682 2020-04-08 12:18:28.000000 ctapipe-0.8.0/docs/ctapipe_api/instrument/camera_geometry.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1727 2020-04-08 12:18:28.000000 ctapipe-0.8.0/docs/ctapipe_api/instrument/camera_readout.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      359 2020-05-22 10:09:37.000000 ctapipe-0.8.0/docs/ctapipe_api/instrument/camerageometry_example.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      965 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/instrument/config.dot
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1730 2020-04-08 12:18:28.000000 ctapipe-0.8.0/docs/ctapipe_api/instrument/index.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      226 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/instrument/optics.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      564 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/instrument/subarray.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      278 2020-04-08 12:18:28.000000 ctapipe-0.8.0/docs/ctapipe_api/instrument/telescope.rst
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.505389 ctapipe-0.8.0/docs/ctapipe_api/io/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5182 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/ctapipe_api/io/index.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    80153 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/io/shower.png
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.505389 ctapipe-0.8.0/docs/ctapipe_api/reco/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6628 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/reco/ImPACT.rst
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.515389 ctapipe-0.8.0/docs/ctapipe_api/reco/images/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)  2645964 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/reco/images/ImageTemplates.png
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    88217 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/reco/images/goodness.png
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   191243 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/reco/images/likelihood.png
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   217537 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/reco/images/predictions.png
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1229 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/reco/index.rst
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.518722 ctapipe-0.8.0/docs/ctapipe_api/tools/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3161 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/tools/index.rst
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.518722 ctapipe-0.8.0/docs/ctapipe_api/utils/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1823 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/utils/index.rst
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.518722 ctapipe-0.8.0/docs/ctapipe_api/visualization/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      733 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_api/visualization/index.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   129249 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/ctapipe_logo.png
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.522055 ctapipe-0.8.0/docs/data_models/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3487 2020-05-19 15:15:37.000000 ctapipe-0.8.0/docs/data_models/dl1.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       66 2020-05-19 15:15:37.000000 ctapipe-0.8.0/docs/data_models/index.rst
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.542055 ctapipe-0.8.0/docs/development/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11881 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/development/code-guidelines.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      185 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/development/index.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1181 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/development/maintainer-info.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3563 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/development/pullrequests.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   152916 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/development/py-pipe-dependencies.pdf
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   109988 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/development/py-pipe-dependencies.png
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6705 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/development/rootmigration.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1761 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/development/style-guide.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6927 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/development/support-libraries.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   365231 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/event.png
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.568721 ctapipe-0.8.0/docs/examples/
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.572055 ctapipe-0.8.0/docs/examples/.ipynb_checkpoints/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     9978 2020-04-27 09:20:59.000000 ctapipe-0.8.0/docs/examples/.ipynb_checkpoints/InstrumentDescription-checkpoint.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    14337 2020-05-08 11:22:19.000000 ctapipe-0.8.0/docs/examples/.ipynb_checkpoints/Tools-checkpoint.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3779 2020-04-27 09:20:18.000000 ctapipe-0.8.0/docs/examples/.ipynb_checkpoints/convert_hex_to_square-checkpoint.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     9978 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/examples/InstrumentDescription.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    14337 2020-05-12 16:04:51.000000 ctapipe-0.8.0/docs/examples/Tools.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      114 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/examples/Tools.json
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4000 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/examples/camera_display.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11894 2020-05-15 12:26:00.000000 ctapipe-0.8.0/docs/examples/container.h5
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6557 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/examples/containers.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4543 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/examples/containers_with_enums_and_table_writer.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3779 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/examples/convert_hex_to_square.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3157 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/examples/dilate_image.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      493 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/examples/index.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6595 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/examples/nd_interpolation.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5036 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/examples/provenance.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    17417 2020-05-15 12:25:30.000000 ctapipe-0.8.0/docs/examples/provenance.log
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    12672 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/examples/table_writer_reader.ipynb
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.572055 ctapipe-0.8.0/docs/getting_started/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10375 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/getting_started/index.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13386 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/index.html
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1657 2020-05-19 15:15:37.000000 ctapipe-0.8.0/docs/index.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      811 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/make.bat
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      122 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/references.txt
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.598721 ctapipe-0.8.0/docs/tutorials/
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.622054 ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10156 2020-04-27 09:19:23.000000 ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/calibrated_data_exploration-checkpoint.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    17544 2020-04-28 10:32:38.000000 ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/coordinates_example-checkpoint.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13470 2020-04-27 12:33:50.000000 ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/ctapipe_handson-checkpoint.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    32287 2020-04-27 12:56:57.000000 ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/lst_analysis_bootcamp_2018-checkpoint.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13891 2020-04-27 09:15:18.000000 ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/raw_data_exploration-checkpoint.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7273 2020-04-27 12:56:30.000000 ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/theta_square-checkpoint.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10159 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/tutorials/calibrated_data_exploration.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    17532 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/tutorials/coordinates_example.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13471 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/tutorials/ctapipe_handson.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   100340 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/tutorials/ground_frame.png
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    21393 2020-05-15 12:27:16.000000 ctapipe-0.8.0/docs/tutorials/hillas.h5
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      208 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/tutorials/index.rst
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    32210 2020-05-19 15:15:37.000000 ctapipe-0.8.0/docs/tutorials/lst_analysis_bootcamp_2018.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13903 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/tutorials/raw_data_exploration.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7261 2020-05-11 13:28:39.000000 ctapipe-0.8.0/docs/tutorials/theta_square.ipynb
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   129772 2020-03-18 13:27:32.000000 ctapipe-0.8.0/docs/tutorials/tilted_ground_frame.png
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      680 2020-05-22 10:09:37.000000 ctapipe-0.8.0/environment.yml
-drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-06-15 14:18:23.655387 ctapipe-0.8.0/examples/
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      255 2020-03-18 13:27:32.000000 ctapipe-0.8.0/examples/README.rst
--rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     1248 2020-05-18 16:19:35.000000 ctapipe-0.8.0/examples/array_display.py
--rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     2400 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/calc_pedestals.py
--rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     1450 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/camera_animation.py
--rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     1773 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/camera_display_multi.py
--rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     1092 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/camera_norms.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      578 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/camera_rotation.py
--rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     3299 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/coordinate_transformations.py
--rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)      764 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/highlight_pixel.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      765 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/instrument_info.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      578 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/load_one_event.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      845 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/plot_all_cameras.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4306 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/plot_array_hillas.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      916 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/plot_camera_frames.py
--rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     1222 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/plot_hillas_parameters.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2803 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/plot_showers_in_nominal.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3360 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/plot_theta_square.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      140 2020-03-18 13:27:32.000000 ctapipe-0.8.0/examples/simple_event_writer.json
--rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     3132 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/simple_event_writer.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3672 2020-05-20 13:57:20.000000 ctapipe-0.8.0/examples/stereo_reconstruction.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3401 2020-05-11 13:28:39.000000 ctapipe-0.8.0/examples/tool_example.py
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      319 2020-05-15 13:48:03.000000 ctapipe-0.8.0/pyproject.toml
--rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      918 2020-06-15 14:18:23.658720 ctapipe-0.8.0/setup.cfg
--rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     3305 2020-06-09 14:36:44.000000 ctapipe-0.8.0/setup.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       96 2020-03-18 13:27:32.000000 ctapipe-0.9.1/.codacy.yml
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/.github/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      100 2020-03-18 13:27:32.000000 ctapipe-0.9.1/.github/release-drafter.yml
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1075 2020-10-21 13:05:50.000000 ctapipe-0.9.1/.gitignore
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/.gitmodules
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      203 2020-03-18 13:27:32.000000 ctapipe-0.9.1/.landscape.yml
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3949 2020-10-20 17:53:44.000000 ctapipe-0.9.1/.mailmap
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2298 2020-10-23 13:44:54.000000 ctapipe-0.9.1/.travis.yml
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1835 2020-03-18 13:27:32.000000 ctapipe-0.9.1/AUTHORS
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      376 2020-09-18 08:11:50.000000 ctapipe-0.9.1/CODEOWNERS
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11223 2020-03-18 13:27:32.000000 ctapipe-0.9.1/History.md
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1556 2020-03-18 13:27:32.000000 ctapipe-0.9.1/LICENSE
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      275 2020-05-15 13:48:03.000000 ctapipe-0.9.1/MANIFEST.in
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1592 2020-03-18 13:27:32.000000 ctapipe-0.9.1/Makefile
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4241 2020-10-23 13:46:11.000000 ctapipe-0.9.1/PKG-INFO
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2910 2020-10-20 17:53:44.000000 ctapipe-0.9.1/README.rst
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ci/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1027 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ci/install.sh
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      195 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       16 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/_version_cache.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/analysis/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      104 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/analysis/__init__.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/analysis/camera/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      102 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/analysis/camera/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4497 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/analysis/camera/charge_resolution.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/analysis/camera/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/analysis/camera/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3450 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/analysis/camera/tests/test_charge_resolution.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/analysis/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/analysis/tests/__init__.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/calib/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      106 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/calib/__init__.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/calib/camera/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      229 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/calib/camera/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5794 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/calib/camera/calibrator.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13707 2020-10-21 13:05:50.000000 ctapipe-0.9.1/ctapipe/calib/camera/flatfield.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2888 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/calib/camera/gainselection.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13172 2020-10-21 13:05:50.000000 ctapipe-0.9.1/ctapipe/calib/camera/pedestals.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/calib/camera/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/calib/camera/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5300 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/calib/camera/tests/test_calibrator.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3107 2020-10-21 13:05:50.000000 ctapipe-0.9.1/ctapipe/calib/camera/tests/test_flatfield.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1759 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/calib/camera/tests/test_gainselection.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2627 2020-10-21 13:05:50.000000 ctapipe-0.9.1/ctapipe/calib/camera/tests/test_pedestals.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/calib/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/calib/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1311 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/conftest.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    31429 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/containers.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/coordinates/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1890 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/coordinates/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7301 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/coordinates/camera_frame.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6285 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/coordinates/ground_frames.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3353 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/coordinates/nominal_frame.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2407 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/coordinates/representation.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3713 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/coordinates/telescope_frame.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/coordinates/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/coordinates/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6294 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/coordinates/tests/test_coordinates.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      954 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/coordinates/tests/test_engineering_frame.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2515 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/coordinates/tests/test_nominal_frame.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1143 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/coordinates/tests/test_roundtrip.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2719 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/coordinates/tests/test_telescope_frame.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/core/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      765 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/core/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     8788 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/core/component.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13141 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/core/container.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1131 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/core/logging.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      438 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/core/plugins.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10392 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/core/provenance.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4651 2020-04-08 12:18:28.000000 ctapipe-0.9.1/ctapipe/core/qualityquery.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      240 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/core/support.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/core/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       47 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/core/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11171 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/core/tests/test_component.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6916 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/core/tests/test_container.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1221 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/core/tests/test_provenance.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3069 2020-04-08 12:18:28.000000 ctapipe-0.9.1/ctapipe/core/tests/test_qualityquery.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4188 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/core/tests/test_tool.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11425 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/core/tests/test_traits.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13824 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/core/tool.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    14320 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/core/traits.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4457 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/fitting.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/image/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      554 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    15480 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/cleaning.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1402 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/concentration.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    38722 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/extractor.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      376 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/geometry_converter.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6544 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/geometry_converter_astri.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1416 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/image/geometry_converter_chec.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    19708 2020-07-13 10:24:42.000000 ctapipe-0.9.1/ctapipe/image/geometry_converter_hex.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5515 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/image/hillas.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1291 2020-07-13 10:24:42.000000 ctapipe-0.9.1/ctapipe/image/leakage.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4788 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/morphology.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/image/muon/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      261 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/muon/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4273 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/muon/features.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3228 2020-07-13 10:24:42.000000 ctapipe-0.9.1/ctapipe/image/muon/fitting.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    16610 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/muon/intensity_fitter.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1649 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/muon/ring_fitter.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/image/muon/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3128 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/muon/tests/test_intensity_fit.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1320 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/muon/tests/test_muon_features.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1278 2020-04-06 15:46:15.000000 ctapipe-0.9.1/ctapipe/image/muon/tests/test_muon_fitting.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1360 2020-07-13 10:24:42.000000 ctapipe-0.9.1/ctapipe/image/muon/tests/test_ring_fitter.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11461 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/image/pixel_likelihood.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6382 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/image/reducer.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2414 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/statistics.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/image/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/image/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     8528 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/tests/test_cleaning.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      856 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/tests/test_concentration.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13781 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/tests/test_extractor.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4164 2020-06-04 10:33:53.000000 ctapipe-0.9.1/ctapipe/image/tests/test_geometry_converter.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7184 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/image/tests/test_hillas.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1741 2020-04-08 12:18:28.000000 ctapipe-0.9.1/ctapipe/image/tests/test_image_cleaner_component.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      591 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/tests/test_leakage.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3934 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/tests/test_morphology.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1519 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/image/tests/test_pixel_likelihood.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3091 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/tests/test_reducer.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1980 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/tests/test_statistics.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3035 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/tests/test_timing_parameters.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6242 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/tests/test_toy.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2592 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/timing.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    12340 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/image/toymodel.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/instrument/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      512 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1938 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/atmosphere.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/instrument/camera/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      256 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/camera/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2329 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/camera/description.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    26241 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/camera/geometry.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6738 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/camera/readout.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/instrument/camera/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-04-08 12:18:28.000000 ctapipe-0.9.1/ctapipe/instrument/camera/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      439 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/camera/tests/test_description.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11117 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/camera/tests/test_geometry.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5186 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/camera/tests/test_readout.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2436 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/guess.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4997 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/optics.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    15495 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/instrument/subarray.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2947 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/telescope.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/instrument/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       85 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      586 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/tests/test_guessing.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2380 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/tests/test_optics.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5021 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/instrument/tests/test_subarray.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1490 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/instrument/tests/test_telescope.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/io/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      603 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      827 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/array.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1879 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/astropy_helpers.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      249 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/datalevels.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     8866 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/eventseeker.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10089 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/eventsource.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      577 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/files.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    18772 2020-10-22 08:00:06.000000 ctapipe-0.9.1/ctapipe/io/hdf5tableio.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6344 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/metadata.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    20425 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/io/simteleventsource.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6089 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/tableio.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/io/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/io/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1160 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/tests/test_astropy_helpers.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      410 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/io/tests/test_available_sources.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4614 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/io/tests/test_event_source.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2324 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/tests/test_eventseeker.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      458 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/tests/test_files.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    21507 2020-10-22 08:00:06.000000 ctapipe-0.9.1/ctapipe/io/tests/test_hdf5.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2312 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/tests/test_metadata.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      466 2020-07-13 10:24:42.000000 ctapipe-0.9.1/ctapipe/io/tests/test_prod2.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11112 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/io/tests/test_simteleventsource.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1179 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/tests/test_toysource.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4323 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/io/toymodel.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/plotting/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       38 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/plotting/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11933 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/plotting/bokeh_event_viewer.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11003 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/plotting/charge_resolution.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/plotting/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/plotting/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4556 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/plotting/tests/test_bokeh_event_viewer.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3895 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/plotting/tests/test_charge_resolution.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/reco/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    14605 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/reco/HillasReconstructor.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    32665 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/reco/ImPACT.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      401 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/reco/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6380 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/reco/energy_regressor.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3443 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/reco/event_classifier.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    17437 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/reco/hillas_intersection.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      826 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/reco/reco_algorithms.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    16064 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/reco/regressor_classifier_base.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2373 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/reco/shower_max.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/reco/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/reco/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     8499 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/reco/tests/test_HillasReconstructor.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5675 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/reco/tests/test_ImPACT.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1453 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/reco/tests/test_energy_regressor.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6515 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/reco/tests/test_event_classifier.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     9235 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/reco/tests/test_hillas_intersection.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2730 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/reco/tests/test_reconstruction_methods.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2448 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/reco/tests/test_regressor_classifier_base.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      748 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/reco/tests/test_showermaxestimator.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      768 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/tests/coveragerc
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       87 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/tests/setup_package.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2512 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/tests/test_fitting.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/tools/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       99 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/tools/__init__.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/tools/bokeh/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/tools/bokeh/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    12535 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/tools/bokeh/file_viewer.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/tools/bokeh/templates/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      645 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/tools/bokeh/templates/index.html
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      482 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/tools/bokeh/theme.yaml
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6479 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/tools/camdemo.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6795 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/tools/display_dl1.py
+-rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     6042 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/tools/display_events_single_tel.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10428 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/tools/display_integrator.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3950 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/tools/display_summed_images.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4213 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/tools/dump_instrument.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4711 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/tools/dump_triggers.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4012 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/tools/extract_charge_resolution.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5447 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/tools/info.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10672 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/tools/muon_reconstruction.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1426 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/tools/plot_charge_resolution.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    26160 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/tools/stage1.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/tools/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        4 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/tools/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     9687 2020-10-23 13:44:54.000000 ctapipe-0.9.1/ctapipe/tools/tests/test_tools.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1861 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/tools/utils.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/utils/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     8701 2020-04-08 12:18:28.000000 ctapipe-0.9.1/ctapipe/utils/CutFlow.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      707 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2394 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/astro.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6935 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/datasets.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    12920 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/fitshistogram.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1364 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/linalg.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      465 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/utils/quantities.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1797 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/rgbtohex.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5393 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/table_interpolator.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2964 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/template_network_interpolator.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/utils/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/utils/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2054 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/tests/test_CutFlow.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      653 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/tests/test_astro.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2151 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/tests/test_datasets.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3210 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/tests/test_fitshistogram.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      579 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/tests/test_linalg.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      890 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/utils/tests/test_quantities.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      700 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/tests/test_rgbtohex.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6189 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/tests/test_unstructured_interpolator.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     8824 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/utils/unstructured_interpolator.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5656 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/version.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/visualization/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      279 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/visualization/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11473 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/visualization/bokeh.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11185 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/visualization/mpl_array.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    16571 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/visualization/mpl_camera.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe/visualization/tests/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        0 2020-03-18 13:27:32.000000 ctapipe-0.9.1/ctapipe/visualization/tests/__init__.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4132 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/visualization/tests/test_bokeh.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3248 2020-10-20 17:53:44.000000 ctapipe-0.9.1/ctapipe/visualization/tests/test_mpl.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe.egg-info/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4241 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe.egg-info/PKG-INFO
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    12171 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe.egg-info/SOURCES.txt
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        1 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe.egg-info/dependency_links.txt
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      803 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe.egg-info/entry_points.txt
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        1 2020-03-18 13:30:42.000000 ctapipe-0.9.1/ctapipe.egg-info/not-zip-safe
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      623 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe.egg-info/requires.txt
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)        8 2020-10-23 13:46:11.000000 ctapipe-0.9.1/ctapipe.egg-info/top_level.txt
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2033 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/FAQ.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      604 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/Makefile
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/_static/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      365 2020-10-20 17:53:44.000000 ctapipe-0.9.1/docs/_static/theme_overrides.css
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/_templates/
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/_templates/autosummary/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      250 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      251 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      252 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1146 2020-10-23 13:44:54.000000 ctapipe-0.9.1/docs/bibliography.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   242690 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/cameras.png
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5378 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/changelog.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7367 2020-10-20 17:53:44.000000 ctapipe-0.9.1/docs/conf.py
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/analysis/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      344 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/analysis/index.rst
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/calib/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      714 2020-07-13 10:24:42.000000 ctapipe-0.9.1/docs/ctapipe_api/calib/index.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1096 2020-07-13 10:24:42.000000 ctapipe-0.9.1/docs/ctapipe_api/calib/index_camera.rst
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/containers/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      384 2020-07-13 10:24:42.000000 ctapipe-0.9.1/docs/ctapipe_api/containers/index.rst
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/coordinates/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1542 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/coordinates/index.rst
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/core/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      592 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/core/corediagram.dot
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1271 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/core/index.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   116209 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/core/tool-component.pdf
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    37376 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/core/tool-component.png
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/image/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    68438 2020-10-20 17:53:44.000000 ctapipe-0.9.1/docs/ctapipe_api/image/TwoPassWindowSum_1st_pass_example.png
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      310 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/image/cleaning.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    93504 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/image/dilate.png
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3369 2020-10-20 17:53:44.000000 ctapipe-0.9.1/docs/ctapipe_api/image/extractor.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      236 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/image/geometry_converter.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      131 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/image/hillas.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      820 2020-04-08 13:37:54.000000 ctapipe-0.9.1/docs/ctapipe_api/image/index.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      173 2020-04-08 13:37:54.000000 ctapipe-0.9.1/docs/ctapipe_api/image/muon.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      166 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/image/pixel_likelihood.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      237 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/image/reducers.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      194 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/image/toymodel.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       79 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/index.rst
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/instrument/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      314 2020-04-08 12:18:28.000000 ctapipe-0.9.1/docs/ctapipe_api/instrument/camera.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3682 2020-04-08 12:18:28.000000 ctapipe-0.9.1/docs/ctapipe_api/instrument/camera_geometry.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1727 2020-04-08 12:18:28.000000 ctapipe-0.9.1/docs/ctapipe_api/instrument/camera_readout.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      358 2020-10-20 17:53:44.000000 ctapipe-0.9.1/docs/ctapipe_api/instrument/camerageometry_example.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      965 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/instrument/config.dot
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1730 2020-04-08 12:18:28.000000 ctapipe-0.9.1/docs/ctapipe_api/instrument/index.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      226 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/instrument/optics.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      564 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/instrument/subarray.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      278 2020-04-08 12:18:28.000000 ctapipe-0.9.1/docs/ctapipe_api/instrument/telescope.rst
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/io/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5182 2020-07-13 10:24:42.000000 ctapipe-0.9.1/docs/ctapipe_api/io/index.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    80153 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/io/shower.png
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/reco/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6628 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/reco/ImPACT.rst
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/reco/images/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)  2645964 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/reco/images/ImageTemplates.png
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    88217 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/reco/images/goodness.png
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   191243 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/reco/images/likelihood.png
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   217537 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/reco/images/predictions.png
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1229 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/reco/index.rst
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/tools/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3161 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/tools/index.rst
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/utils/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1823 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/utils/index.rst
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/ctapipe_api/visualization/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      733 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_api/visualization/index.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   129249 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/ctapipe_logo.png
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/data_models/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3487 2020-10-20 17:53:44.000000 ctapipe-0.9.1/docs/data_models/dl1.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)       66 2020-10-20 17:53:44.000000 ctapipe-0.9.1/docs/data_models/index.rst
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/development/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11881 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/development/code-guidelines.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      185 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/development/index.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1181 2020-10-23 13:44:54.000000 ctapipe-0.9.1/docs/development/maintainer-info.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3563 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/development/pullrequests.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   152916 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/development/py-pipe-dependencies.pdf
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   109988 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/development/py-pipe-dependencies.png
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6705 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/development/rootmigration.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1761 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/development/style-guide.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6927 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/development/support-libraries.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   365231 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/event.png
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/examples/
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/examples/.ipynb_checkpoints/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     9978 2020-04-27 09:20:59.000000 ctapipe-0.9.1/docs/examples/.ipynb_checkpoints/InstrumentDescription-checkpoint.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    14304 2020-10-07 10:20:36.000000 ctapipe-0.9.1/docs/examples/.ipynb_checkpoints/Tools-checkpoint.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3779 2020-04-27 09:20:18.000000 ctapipe-0.9.1/docs/examples/.ipynb_checkpoints/convert_hex_to_square-checkpoint.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     9978 2020-07-13 10:24:42.000000 ctapipe-0.9.1/docs/examples/InstrumentDescription.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    14337 2020-10-19 12:51:30.000000 ctapipe-0.9.1/docs/examples/Tools.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      114 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/examples/Tools.json
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4000 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/examples/camera_display.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    11894 2020-07-24 09:22:13.000000 ctapipe-0.9.1/docs/examples/container.h5
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6557 2020-07-13 10:24:42.000000 ctapipe-0.9.1/docs/examples/containers.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4543 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/examples/containers_with_enums_and_table_writer.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3779 2020-07-13 10:24:42.000000 ctapipe-0.9.1/docs/examples/convert_hex_to_square.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3157 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/examples/dilate_image.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      493 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/examples/index.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     6595 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/examples/nd_interpolation.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     5036 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/examples/provenance.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    18322 2020-07-24 09:21:43.000000 ctapipe-0.9.1/docs/examples/provenance.log
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    12672 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/examples/table_writer_reader.ipynb
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/getting_started/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10375 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/getting_started/index.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13386 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/index.html
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     1657 2020-10-23 13:44:54.000000 ctapipe-0.9.1/docs/index.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      811 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/make.bat
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      122 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/references.txt
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/tutorials/
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10156 2020-04-27 09:19:23.000000 ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/calibrated_data_exploration-checkpoint.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    17544 2020-04-28 10:32:38.000000 ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/coordinates_example-checkpoint.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13470 2020-04-27 12:33:50.000000 ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/ctapipe_handson-checkpoint.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    32287 2020-04-27 12:56:57.000000 ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/lst_analysis_bootcamp_2018-checkpoint.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13891 2020-04-27 09:15:18.000000 ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/raw_data_exploration-checkpoint.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7273 2020-04-27 12:56:30.000000 ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/theta_square-checkpoint.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    10159 2020-07-13 10:24:42.000000 ctapipe-0.9.1/docs/tutorials/calibrated_data_exploration.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    17532 2020-07-13 10:24:42.000000 ctapipe-0.9.1/docs/tutorials/coordinates_example.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13471 2020-07-13 10:24:42.000000 ctapipe-0.9.1/docs/tutorials/ctapipe_handson.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   100340 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/tutorials/ground_frame.png
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    20948 2020-07-24 09:23:28.000000 ctapipe-0.9.1/docs/tutorials/hillas.h5
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      208 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/tutorials/index.rst
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    32210 2020-10-20 17:53:44.000000 ctapipe-0.9.1/docs/tutorials/lst_analysis_bootcamp_2018.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)    13935 2020-10-20 17:53:44.000000 ctapipe-0.9.1/docs/tutorials/raw_data_exploration.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     7261 2020-07-13 10:24:42.000000 ctapipe-0.9.1/docs/tutorials/theta_square.ipynb
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)   129772 2020-03-18 13:27:32.000000 ctapipe-0.9.1/docs/tutorials/tilted_ground_frame.png
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      680 2020-10-23 13:33:21.000000 ctapipe-0.9.1/environment.yml
+drwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)        0 2020-10-23 13:46:11.000000 ctapipe-0.9.1/examples/
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      255 2020-03-18 13:27:32.000000 ctapipe-0.9.1/examples/README.rst
+-rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     1248 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/array_display.py
+-rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     2400 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/calc_pedestals.py
+-rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     1450 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/camera_animation.py
+-rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     1773 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/camera_display_multi.py
+-rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     1092 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/camera_norms.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      578 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/camera_rotation.py
+-rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     3299 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/coordinate_transformations.py
+-rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)      764 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/highlight_pixel.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      765 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/instrument_info.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      578 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/load_one_event.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      845 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/plot_all_cameras.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     4306 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/plot_array_hillas.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      916 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/plot_camera_frames.py
+-rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     1222 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/plot_hillas_parameters.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     2803 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/plot_showers_in_nominal.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3360 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/plot_theta_square.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      140 2020-03-18 13:27:32.000000 ctapipe-0.9.1/examples/simple_event_writer.json
+-rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     3132 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/simple_event_writer.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3672 2020-10-20 17:53:44.000000 ctapipe-0.9.1/examples/stereo_reconstruction.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)     3401 2020-10-19 12:51:30.000000 ctapipe-0.9.1/examples/tool_example.py
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      319 2020-05-15 13:48:03.000000 ctapipe-0.9.1/pyproject.toml
+-rw-r--r--   0 maxnoe    (1000) maxnoe    (1000)      918 2020-10-23 13:46:11.000000 ctapipe-0.9.1/setup.cfg
+-rwxr-xr-x   0 maxnoe    (1000) maxnoe    (1000)     3305 2020-10-23 13:44:54.000000 ctapipe-0.9.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ctapipe-0.8.0/.gitignore` & `ctapipe-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/.mailmap` & `ctapipe-0.9.1/.mailmap`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/.travis.yml` & `ctapipe-0.9.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/AUTHORS` & `ctapipe-0.9.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/History.md` & `ctapipe-0.9.1/History.md`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/LICENSE` & `ctapipe-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/Makefile` & `ctapipe-0.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/PKG-INFO` & `ctapipe-0.9.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,72 @@
 Metadata-Version: 2.1
 Name: ctapipe
-Version: 0.8.0
+Version: 0.9.1
 Summary: CTA Python pipeline experimental version
 Home-page: https://github.com/cta-observatory/ctapipe
 Author: ctapipe developers
 Author-email: karl.kosack@cea.fr
 License: BSD 3-Clause License
-Description: =========================================================
-        ctapipe |teststatus| |codacy| |coverage| |conda| |doiv07|
-        =========================================================
+Description: ============================================================
+        ctapipe |teststatus| |codacy| |coverage| |conda| |doilatest|
+        ============================================================
         
         .. |teststatus| image:: https://travis-ci.com/cta-observatory/ctapipe.svg?branch=master
             :target: https://travis-ci.com/cta-observatory/ctapipe
             :alt: Test Status
         .. |codacy|  image:: https://api.codacy.com/project/badge/Grade/6192b471956b4cc684130c80c8214115   
           :target: https://www.codacy.com/gh/cta-observatory/ctapipe?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cta-observatory/ctapipe&amp;utm_campaign=Badge_Grade
         .. |conda| image:: https://anaconda.org/cta-observatory/ctapipe/badges/installer/conda.svg
         .. |coverage| image:: https://codecov.io/gh/cta-observatory/ctapipe/branch/master/graph/badge.svg
           :target: https://codecov.io/gh/cta-observatory/ctapipe
-        .. |doiv07| image:: https://zenodo.org/badge/37927055.svg
+        .. |doilatest| image:: https://zenodo.org/badge/37927055.svg
           :target: https://zenodo.org/badge/latestdoi/37927055
+        .. |doiv07| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3372211.svg
+           :target: https://doi.org/10.5281/zenodo.3372211
+        .. |doiv08| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3837306.svg
+           :target: https://doi.org/10.5281/zenodo.3837306
         
         Low-level data processing pipeline software for
         `CTA <www.cta-observatory.org>`_ (the Cherenkov Telescope Array)
         
         This is code is a prototype data processing framework and is under rapid
         development. It is not recommended for production use unless you are an
         expert or developer!
         
         * Code: https://github.com/cta-observatory/ctapipe
         * Docs: https://cta-observatory.github.io/ctapipe/
         * Slack: Contact Karl Kosack for invite
         
         Citing this software
         --------------------
-        If you use this software for a publication, please cite using the following DOIs: 
+        If you use this software for a publication, please cite the proper version using the following DOIs:
         
         - v0.7.0 : |doiv07|
-        
+        - v0.8.0 : |doiv08|
         
         Installation for Users
         ----------------------
         
         *ctapipe* and its dependencies may be installed using the *Anaconda* or
         *Miniconda* package system. We recommend creating a conda virtual environment
         first, to isolate the installed version and dependencies from your master
         environment (this is optional).
         
         
         The following command will set up a conda virtual environment, add the
-        necessary package channels, and download ctapipe and its dependencies. The
-        file *environment.yml* can be found in this repo. 
-        Note this is *pre-alpha* software and is not yet stable enough for end-users (expect large API changes until the first stable 1.0 release).
-        
-        ::
+        necessary package channels, and install ctapipe specified version and its dependencies::
         
+          CTAPIPE_VER=0.8.0
+          wget https://raw.githubusercontent.com/cta-observatory/ctapipe/v$CTAPIPE_VER/environment.yml
           conda env create -n cta -f environment.yml
           conda activate cta
-          conda install -c cta-observatory ctapipe
+          conda install -c cta-observatory ctapipe=$CTAPIPE_VER
         
+        The file *environment.yml* can be found in this repo. 
+        Note this is *pre-alpha* software and is not yet stable enough for end-users (expect large API changes until the first stable 1.0 release).
         
         Developers should follow the development install instructions found in the
         `documentation <https://cta-observatory.github
         .io/ctapipe/getting_started>`_.
         
         
 Platform: UNKNOWN
```

### Comparing `ctapipe-0.8.0/README.rst` & `ctapipe-0.9.1/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,62 @@
-=========================================================
-ctapipe |teststatus| |codacy| |coverage| |conda| |doiv07|
-=========================================================
+============================================================
+ctapipe |teststatus| |codacy| |coverage| |conda| |doilatest|
+============================================================
 
 .. |teststatus| image:: https://travis-ci.com/cta-observatory/ctapipe.svg?branch=master
     :target: https://travis-ci.com/cta-observatory/ctapipe
     :alt: Test Status
 .. |codacy|  image:: https://api.codacy.com/project/badge/Grade/6192b471956b4cc684130c80c8214115   
   :target: https://www.codacy.com/gh/cta-observatory/ctapipe?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cta-observatory/ctapipe&amp;utm_campaign=Badge_Grade
 .. |conda| image:: https://anaconda.org/cta-observatory/ctapipe/badges/installer/conda.svg
 .. |coverage| image:: https://codecov.io/gh/cta-observatory/ctapipe/branch/master/graph/badge.svg
   :target: https://codecov.io/gh/cta-observatory/ctapipe
-.. |doiv07| image:: https://zenodo.org/badge/37927055.svg
+.. |doilatest| image:: https://zenodo.org/badge/37927055.svg
   :target: https://zenodo.org/badge/latestdoi/37927055
+.. |doiv07| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3372211.svg
+   :target: https://doi.org/10.5281/zenodo.3372211
+.. |doiv08| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3837306.svg
+   :target: https://doi.org/10.5281/zenodo.3837306
 
 Low-level data processing pipeline software for
 `CTA <www.cta-observatory.org>`_ (the Cherenkov Telescope Array)
 
 This is code is a prototype data processing framework and is under rapid
 development. It is not recommended for production use unless you are an
 expert or developer!
 
 * Code: https://github.com/cta-observatory/ctapipe
 * Docs: https://cta-observatory.github.io/ctapipe/
 * Slack: Contact Karl Kosack for invite
 
 Citing this software
 --------------------
-If you use this software for a publication, please cite using the following DOIs: 
+If you use this software for a publication, please cite the proper version using the following DOIs:
 
 - v0.7.0 : |doiv07|
-
+- v0.8.0 : |doiv08|
 
 Installation for Users
 ----------------------
 
 *ctapipe* and its dependencies may be installed using the *Anaconda* or
 *Miniconda* package system. We recommend creating a conda virtual environment
 first, to isolate the installed version and dependencies from your master
 environment (this is optional).
 
 
 The following command will set up a conda virtual environment, add the
-necessary package channels, and download ctapipe and its dependencies. The
-file *environment.yml* can be found in this repo. 
-Note this is *pre-alpha* software and is not yet stable enough for end-users (expect large API changes until the first stable 1.0 release).
-
-::
+necessary package channels, and install ctapipe specified version and its dependencies::
 
+  CTAPIPE_VER=0.8.0
+  wget https://raw.githubusercontent.com/cta-observatory/ctapipe/v$CTAPIPE_VER/environment.yml
   conda env create -n cta -f environment.yml
   conda activate cta
-  conda install -c cta-observatory ctapipe
+  conda install -c cta-observatory ctapipe=$CTAPIPE_VER
 
+The file *environment.yml* can be found in this repo. 
+Note this is *pre-alpha* software and is not yet stable enough for end-users (expect large API changes until the first stable 1.0 release).
 
 Developers should follow the development install instructions found in the
 `documentation <https://cta-observatory.github
 .io/ctapipe/getting_started>`_.
```

### Comparing `ctapipe-0.8.0/ci/install.sh` & `ctapipe-0.9.1/ci/install.sh`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/analysis/camera/charge_resolution.py` & `ctapipe-0.9.1/ctapipe/analysis/camera/charge_resolution.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/analysis/camera/tests/test_charge_resolution.py` & `ctapipe-0.9.1/ctapipe/analysis/camera/tests/test_charge_resolution.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/calib/camera/calibrator.py` & `ctapipe-0.9.1/ctapipe/calib/camera/calibrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,15 @@
         self._dl0_empty_warn = False
 
         if image_extractor is None:
             image_extractor = NeighborPeakWindowSum(parent=self, subarray=subarray)
         self.image_extractor = image_extractor
 
         if data_volume_reducer is None:
-            data_volume_reducer = NullDataVolumeReducer(
-                parent=self, image_extractor=self.image_extractor
-            )
+            data_volume_reducer = NullDataVolumeReducer(parent=self, subarray=subarray)
         self.data_volume_reducer = data_volume_reducer
 
     def _check_r1_empty(self, waveforms):
         if waveforms is None:
             if not self._r1_empty_warn:
                 warnings.warn(
                     "Encountered an event with no R1 data. "
```

### Comparing `ctapipe-0.8.0/ctapipe/calib/camera/flatfield.py` & `ctapipe-0.9.1/ctapipe/calib/camera/flatfield.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/calib/camera/gainselection.py` & `ctapipe-0.9.1/ctapipe/calib/camera/gainselection.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/calib/camera/pedestals.py` & `ctapipe-0.9.1/ctapipe/calib/camera/pedestals.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/calib/camera/tests/test_calibrator.py` & `ctapipe-0.9.1/ctapipe/calib/camera/tests/test_calibrator.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/calib/camera/tests/test_flatfield.py` & `ctapipe-0.9.1/ctapipe/calib/camera/tests/test_flatfield.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,19 @@
                 optics_name="SST-ASTRI", camera_name="CHEC"
             ),
         },
     )
     subarray.tel[0].camera.readout.reference_pulse_shape = np.ones((1, 2))
     subarray.tel[0].camera.readout.reference_pulse_sample_width = u.Quantity(1, u.ns)
 
-    config = Config({"FixedWindowSum": {"window_start": 15, "window_width": 10}})
+    config = Config({"FixedWindowSum": {
+        "peak_index": 15,
+        "window_shift": 0,
+        "window_width": 10,
+    }})
     ff_calculator = FlasherFlatFieldCalculator(
         subarray=subarray,
         charge_product="FixedWindowSum",
         sample_size=n_events,
         tel_id=tel_id,
         config=config,
     )
```

### Comparing `ctapipe-0.8.0/ctapipe/calib/camera/tests/test_gainselection.py` & `ctapipe-0.9.1/ctapipe/calib/camera/tests/test_gainselection.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/calib/camera/tests/test_pedestals.py` & `ctapipe-0.9.1/ctapipe/calib/camera/tests/test_pedestals.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/conftest.py` & `ctapipe-0.9.1/ctapipe/conftest.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/containers.py` & `ctapipe-0.9.1/ctapipe/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -714,18 +714,18 @@
     )
     center_distance = Field(
         nan * u.deg, "Distance of ring center from camera center", unit=u.deg
     )
 
 
 class MuonEfficiencyContainer(Container):
-    width = Field(nan, "width of the muon ring in degrees")
-    impact = Field(nan, "distance of muon impact position from center of mirror")
-    impact_x = Field(nan, "impact parameter x position")
-    impact_y = Field(nan, "impact parameter y position")
+    width = Field(nan * u.deg, "width of the muon ring in degrees")
+    impact = Field(nan * u.m, "distance of muon impact position from center of mirror")
+    impact_x = Field(nan * u.m, "impact parameter x position")
+    impact_y = Field(nan * u.m, "impact parameter y position")
     optical_efficiency = Field(nan, "optical efficiency muon")
 
 
 class MuonParametersContainer(Container):
     containment = Field(nan, "containment of the ring inside the camera")
     completeness = Field(
         nan,
@@ -850,18 +850,18 @@
 class WaveformCalibrationContainer(Container):
     """
     Container for the pixel calibration coefficients
     """
 
     time = Field(nan * u.s, "Time associated to the calibration event", unit=u.s)
     time_min = Field(
-        nan * u.s, "Earliest time of validity for the calibration event", unit=u.s,
+        nan * u.s, "Earliest time of validity for the calibration event", unit=u.s
     )
     time_max = Field(
-        nan * u.s, "Latest time of validity for the calibration event", unit=u.s,
+        nan * u.s, "Latest time of validity for the calibration event", unit=u.s
     )
 
     dc_to_pe = Field(
         None,
         "np array of (digital count) to (photon electron) coefficients (n_chan, n_pix)",
     )
```

### Comparing `ctapipe-0.8.0/ctapipe/coordinates/__init__.py` & `ctapipe-0.9.1/ctapipe/coordinates/__init__.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/coordinates/camera_frame.py` & `ctapipe-0.9.1/ctapipe/coordinates/camera_frame.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/coordinates/ground_frames.py` & `ctapipe-0.9.1/ctapipe/coordinates/ground_frames.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/coordinates/nominal_frame.py` & `ctapipe-0.9.1/ctapipe/coordinates/nominal_frame.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/coordinates/representation.py` & `ctapipe-0.9.1/ctapipe/coordinates/representation.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/coordinates/telescope_frame.py` & `ctapipe-0.9.1/ctapipe/coordinates/telescope_frame.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/coordinates/tests/test_coordinates.py` & `ctapipe-0.9.1/ctapipe/coordinates/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/coordinates/tests/test_engineering_frame.py` & `ctapipe-0.9.1/ctapipe/coordinates/tests/test_engineering_frame.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/coordinates/tests/test_nominal_frame.py` & `ctapipe-0.9.1/ctapipe/coordinates/tests/test_nominal_frame.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/coordinates/tests/test_roundtrip.py` & `ctapipe-0.9.1/ctapipe/coordinates/tests/test_roundtrip.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/coordinates/tests/test_telescope_frame.py` & `ctapipe-0.9.1/ctapipe/coordinates/tests/test_telescope_frame.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/core/__init__.py` & `ctapipe-0.9.1/ctapipe/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/core/component.py` & `ctapipe-0.9.1/ctapipe/core/component.py`

 * *Files 7% similar despite different names*

```diff
@@ -204,7 +204,40 @@
         self.subarray = subarray
         # configure all of the TelescopeParameters
         for trait in list(self.class_traits()):
             try:
                 getattr(self, trait).attach_subarray(subarray)
             except (AttributeError, TypeError):
                 pass
+
+    @classmethod
+    def from_name(cls, name, subarray, config=None, parent=None, **kwargs):
+        """
+        Obtain an instance of a subclass via its name
+
+        Parameters
+        ----------
+        name : str
+            Name of the subclass to obtain
+        subarray: ctapipe.instrument.SubarrayDescription
+            The current subarray for this TelescopeComponent.
+        config : traitlets.loader.Config
+            Configuration specified by config file or cmdline arguments.
+            Used to set traitlet values.
+            This argument is typically only specified when using this method
+            from within a Tool.
+        parent : ctapipe.core.Tool
+            Tool executable that is calling this component.
+            Passes the correct logger and configuration to the component.
+            This argument is typically only specified when using this method
+            from within a Tool (config need not be passed if parent is used).
+        kwargs
+
+        Returns
+        -------
+        instace
+            Instance of subclass to this class
+        """
+        requested_subclass = cls.non_abstract_subclasses()[name]
+        return requested_subclass(
+            subarray=subarray, config=config, parent=parent, **kwargs
+        )
```

### Comparing `ctapipe-0.8.0/ctapipe/core/container.py` & `ctapipe-0.9.1/ctapipe/core/container.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/core/logging.py` & `ctapipe-0.9.1/ctapipe/core/logging.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/core/provenance.py` & `ctapipe-0.9.1/ctapipe/core/provenance.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/core/qualityquery.py` & `ctapipe-0.9.1/ctapipe/core/qualityquery.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/core/tests/test_component.py` & `ctapipe-0.9.1/ctapipe/core/tests/test_component.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from abc import abstractmethod, ABC
 
 import pytest
 from traitlets import Float, TraitError
 from traitlets.config.loader import Config
+import astropy.units as u
+import warnings
 
 from ctapipe.core import Component
 
 
 def test_non_abstract_children():
     """ check that we can find all constructable children """
     from ctapipe.core import non_abstract_children
@@ -91,15 +93,20 @@
 
     # Invalid type
     with pytest.raises(TraitError):
         comp = ExampleComponent(param="badvalue")
 
     # Invalid traitlet
     with pytest.raises(TraitError):
-        comp = ExampleComponent(incorrect="wrong")
+        # the current traitlets version already warns about this
+        # will be raising an error in the future, but we want the error
+        # now, filter the warning here to not clutter the log
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", category=DeprecationWarning)
+            comp = ExampleComponent(incorrect="wrong")
 
 
 def test_help():
     """ check that component help strings are generated correctly """
     help_msg = ExampleComponent.class_get_help()
     assert "Default: 1.0" in help_msg
 
@@ -216,18 +223,24 @@
     config = Config()
     config["ExampleSubclass2"] = Config()
     config["ExampleSubclass2"]["extra"] = 229.0
     comp = ExampleSubclass2(config=config)
     assert comp.extra == 229.0
 
 
-def test_extra_missing():
+def test_unknown_traitlet_raises():
     """ check that setting an incorrect trait raises an exception """
     with pytest.raises(TraitError):
-        ExampleSubclass1(extra=229.0)
+        # the current traitlets version already warns about this
+        # will be raising an error in the future, but we want the error
+        # now, filter the warning here to not clutter the log
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", category=DeprecationWarning)
+
+            ExampleSubclass1(extra=229.0)
 
 
 def test_extra_config_missing():
     """
     check that setting an incorrect trait via config also raises
     an exception
     """
@@ -331,7 +344,26 @@
 
 
 def test_component_html_repr():
     """ check the HTML repr for Jupyter notebooks """
     comp = ExampleComponent()
     html = comp._repr_html_()
     assert len(html) > 10
+
+
+def test_telescope_component():
+    from ctapipe.core import TelescopeComponent
+    from ctapipe.instrument import SubarrayDescription, TelescopeDescription
+
+    subarray = SubarrayDescription(
+        "test",
+        tel_positions={1: [0, 0, 0] * u.m},
+        tel_descriptions={1: TelescopeDescription.from_name("LST", "LSTCam")},
+    )
+
+    class Base(TelescopeComponent):
+        pass
+
+    class Sub(Base):
+        pass
+
+    assert isinstance(Base.from_name("Sub", subarray=subarray), Sub)
```

### Comparing `ctapipe-0.8.0/ctapipe/core/tests/test_container.py` & `ctapipe-0.9.1/ctapipe/core/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/core/tests/test_provenance.py` & `ctapipe-0.9.1/ctapipe/core/tests/test_provenance.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/core/tests/test_qualityquery.py` & `ctapipe-0.9.1/ctapipe/core/tests/test_qualityquery.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/core/tests/test_tool.py` & `ctapipe-0.9.1/ctapipe/core/tests/test_tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import pytest
 from traitlets import Float, TraitError, List, Dict
 from traitlets.config import Config
 
 from .. import Tool, Component
 from ..tool import export_tool_config_to_commented_yaml
 
@@ -34,14 +35,25 @@
         description = "test"
         userparam = Float(5.0, help="parameter").tag(config=True)
 
     tool = MyTool()
     assert tool.version_string != ""
 
 
+def test_provenance_dir():
+    """ check that the tool gets the provenance dir"""
+
+    class MyTool(Tool):
+        description = "test"
+        userparam = Float(5.0, help="parameter").tag(config=True)
+
+    tool = MyTool()
+    assert str(tool.provenance_log) == os.path.join(os.getcwd(), "application.provenance.log")
+
+
 def test_export_config_to_yaml():
     """ test that we can export a Tool's config to YAML"""
     import yaml
     from ctapipe.tools.camdemo import CameraDemo
 
     tool = CameraDemo()
     tool.num_events = 2
```

### Comparing `ctapipe-0.8.0/ctapipe/core/tests/test_traits.py` & `ctapipe-0.9.1/ctapipe/core/tests/test_traits.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/core/tool.py` & `ctapipe-0.9.1/ctapipe/core/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Classes to handle configurable command-line user interfaces """
 import logging
 import textwrap
 from abc import abstractmethod
 
-from traitlets import Unicode
+from traitlets import default, Unicode
 from traitlets.config import Application, Configurable
 
 from .. import __version__ as version
 from .traits import Path
 from . import Provenance
 from .logging import ColoredFormatter
 
@@ -110,14 +110,20 @@
         ),
     ).tag(config=True)
     log_format = Unicode(
         "%(levelname)s [%(name)s] (%(module)s/%(funcName)s): %(message)s",
         help="The Logging format template",
     ).tag(config=True)
 
+    provenance_log = Path(directory_ok=False)
+
+    @default('provenance_log')
+    def _default_provenance_log(self):
+        return self.name + '.provenance.log'
+
     _log_formatter_cls = ColoredFormatter
 
     def __init__(self, **kwargs):
         # make sure there are some default aliases in all Tools:
         if self.aliases:
             self.aliases["log-level"] = "Application.log_level"
             self.aliases["config"] = "Tool.config_file"
@@ -233,15 +239,16 @@
             exit_status = 1  # any other error
         finally:
             for activity in Provenance().finished_activities:
                 output_str = " ".join([x["url"] for x in activity.output])
                 self.log.info("Output: %s", output_str)
 
             self.log.debug("PROVENANCE: '%s'", Provenance().as_json(indent=3))
-            with open("provenance.log", mode="w+") as provlog:
+            self.provenance_log.parent.mkdir(parents=True, exist_ok=True)
+            with open(self.provenance_log, mode="a+") as provlog:
                 provlog.write(Provenance().as_json(indent=3))
 
         self.exit(exit_status)
 
     @property
     def version_string(self):
         """ a formatted version string with version, release, and git hash"""
```

### Comparing `ctapipe-0.8.0/ctapipe/core/traits.py` & `ctapipe-0.9.1/ctapipe/core/traits.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/__init__.py` & `ctapipe-0.9.1/ctapipe/image/__init__.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/cleaning.py` & `ctapipe-0.9.1/ctapipe/image/cleaning.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/concentration.py` & `ctapipe-0.9.1/ctapipe/image/concentration.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     delta_x = pix_x - x
     delta_y = pix_y - y
 
     # sort pixels by distance to cog
     cog_pixels = np.argsort(delta_x ** 2 + delta_y ** 2)
     conc_cog = np.sum(image[cog_pixels[:3]]) / h.intensity
 
-    if hillas_parameters.width != 0:
+    if hillas_parameters.width.value != 0:
         # get all pixels inside the hillas ellipse
         longi, trans = camera_to_shower_coordinates(
             pix_x, pix_y, x, y, h.psi.to_value(u.rad)
         )
         mask_core = (longi ** 2 / length ** 2) + (trans ** 2 / width ** 2) <= 1.0
         conc_core = image[mask_core].sum() / h.intensity
     else:
```

### Comparing `ctapipe-0.8.0/ctapipe/image/extractor.py` & `ctapipe-0.9.1/ctapipe/image/extractor.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,24 @@
     "integration_correction",
 ]
 
 
 from abc import abstractmethod
 from functools import lru_cache
 import numpy as np
-from traitlets import Int
-from ctapipe.core.traits import IntTelescopeParameter, FloatTelescopeParameter
+from traitlets import Int, Bool
+from ctapipe.core.traits import (
+    IntTelescopeParameter,
+    FloatTelescopeParameter,
+    BoolTelescopeParameter,
+)
 from ctapipe.core import TelescopeComponent
 from numba import njit, prange, guvectorize, float64, float32, int64
+from scipy.ndimage.filters import convolve1d
+from typing import Tuple
 
 from . import number_of_islands, largest_island, tailcuts_clean
 from .timing import timing_parameters
 from .hillas import hillas_parameters, camera_to_shower_coordinates
 
 
 @guvectorize(
@@ -109,48 +115,60 @@
     peak_time[0] = time_num / time_den if time_den > 0 else peak_index
     # Convert to units of ns
     peak_time[0] /= sampling_rate_ghz
     sum_[0] = i_sum
 
 
 @njit(parallel=True)
-def neighbor_average_waveform(waveforms, neighbors, lwt):
+def neighbor_average_waveform(waveforms, neighbors_indices, neighbors_indptr, lwt):
     """
     Obtain the average waveform built from the neighbors of each pixel
 
     Parameters
     ----------
     waveforms : ndarray
         Waveforms stored in a numpy array.
         Shape: (n_pix, n_samples)
-    neighbors : ndarray
-        2D array where each row is [pixel index, one neighbor of that pixel].
-        Changes per telescope.
-        Can be obtained from
-        `ctapipe.instrument.CameraGeometry.neighbor_matrix_where`.
+    neighbors_indices : ndarray
+        indices of a scipy csr sparse matrix of neighbors, i.e.
+        `ctapipe.instrument.CameraGeometry.neighbor_matrix_sparse.indices`.
+    neighbors_indptr : ndarray
+        indptr of a scipy csr sparse matrix of neighbors, i.e.
+        `ctapipe.instrument.CameraGeometry.neighbor_matrix_sparse.indptr`.
     lwt: int
         Weight of the local pixel (0: peak from neighbors only,
         1: local pixel counts as much as any neighbor)
 
     Returns
     -------
     average_wf : ndarray
         Average of neighbor waveforms for each pixel.
         Shape: (n_pix, n_samples)
 
     """
-    n_neighbors = neighbors.shape[0]
-    sum_ = waveforms * lwt
-    n = np.full(waveforms.shape, lwt, dtype=np.int32)
-    for i in prange(n_neighbors):
-        pixel = neighbors[i, 0]
-        neighbor = neighbors[i, 1]
-        sum_[pixel] += waveforms[neighbor]
-        n[pixel] += 1
-    return sum_ / n
+
+    n_pixels = waveforms.shape[0]
+    indptr = neighbors_indptr
+    indices = neighbors_indices
+
+    # initialize to waveforms weighted with lwt
+    # so the value of the pixel itself is already taken into account
+    average = waveforms * lwt
+
+    for pixel in prange(n_pixels):
+        neighbors = indices[indptr[pixel] : indptr[pixel + 1]]
+
+        n = lwt
+        for neighbor in neighbors:
+            average[pixel] += waveforms[neighbor]
+            n += 1
+
+        average[pixel] /= n
+
+    return average
 
 
 def subtract_baseline(waveforms, baseline_start, baseline_end):
     """
     Subtracts the waveform baseline, estimated as the mean waveform value
     in the interval [baseline_start:baseline_end]
 
@@ -236,37 +254,14 @@
 
         integration = sampled_pulse[start:end] * sample_width_ns
         correction[ichannel] = 1.0 / np.sum(integration)
 
     return correction
 
 
-def slide_window(waveform, width):
-    """Smooth a pixel's waveform (or a slice of it) with a kernel of certain
-     size via convolution.
-
-    Parameters
-    ----------
-    waveform : array_like
-        DL0-level waveform (or slice of it) of one event.
-        Shape: max (n_samples)
-    width : int
-        Size of the smoothing kernel.
-
-    Returns
-    -------
-    sum : array_like
-        Array containing the sums for each of the kernel positions.
-        Shape: max (n_samples - (window_width - 1))
-
-    """
-    sums = np.convolve(waveform, np.ones(width, dtype=int), "valid")
-    return sums
-
-
 class ImageExtractor(TelescopeComponent):
     def __init__(self, subarray, config=None, parent=None, **kwargs):
         """
         Base component to handle the extraction of charge and pulse time
         from an image cube (waveforms), taking into account the sampling rate
         of the waveform.
 
@@ -340,29 +335,36 @@
 
 
 class FixedWindowSum(ImageExtractor):
     """
     Extractor that sums within a fixed window defined by the user.
     """
 
-    window_start = IntTelescopeParameter(
-        default_value=0, help="Define the start position for the integration window"
+    peak_index = IntTelescopeParameter(
+        default_value=0, help="Manually select index where the peak is located"
     ).tag(config=True)
     window_width = IntTelescopeParameter(
         default_value=7, help="Define the width of the integration window"
     ).tag(config=True)
+    window_shift = IntTelescopeParameter(
+        default_value=0,
+        help="Define the shift of the integration window from the peak_index "
+        "(peak_index - shift)",
+    ).tag(config=True)
+
+    apply_integration_correction = BoolTelescopeParameter(
+        default_value=True, help="Apply the integration window correction"
+    ).tag(config=True)
 
     @lru_cache(maxsize=128)
     def _calculate_correction(self, telid):
         """
         Calculate the correction for the extracted change such that the value
         returned would equal 1 for a noise-less unit pulse.
 
-        Assuming the pulse is centered in the manually defined integration
-        window, the integration_correction with a shift=0 is correct.
         This method is decorated with @lru_cache to ensure it is only
         calculated once per telescope.
 
         Parameters
         ----------
         telid : int
 
@@ -375,44 +377,50 @@
         """
         readout = self.subarray.tel[telid].camera.readout
         return integration_correction(
             readout.reference_pulse_shape,
             readout.reference_pulse_sample_width.to_value("ns"),
             (1 / readout.sampling_rate).to_value("ns"),
             self.window_width.tel[telid],
-            0,
+            self.window_shift.tel[telid],
         )
 
     def __call__(self, waveforms, telid, selected_gain_channel):
         charge, peak_time = extract_around_peak(
             waveforms,
-            self.window_start.tel[telid],
+            self.peak_index.tel[telid],
             self.window_width.tel[telid],
-            0,
+            self.window_shift.tel[telid],
             self.sampling_rate[telid],
         )
-        charge *= self._calculate_correction(telid=telid)[selected_gain_channel]
+        if self.apply_integration_correction.tel[telid]:
+            charge *= self._calculate_correction(telid=telid)[selected_gain_channel]
         return charge, peak_time
 
 
 class GlobalPeakWindowSum(ImageExtractor):
     """
     Extractor which sums in a window about the
     peak from the global average waveform.
     """
 
     window_width = IntTelescopeParameter(
         default_value=7, help="Define the width of the integration window"
     ).tag(config=True)
+
     window_shift = IntTelescopeParameter(
         default_value=3,
         help="Define the shift of the integration window from the peak_index "
         "(peak_index - shift)",
     ).tag(config=True)
 
+    apply_integration_correction = BoolTelescopeParameter(
+        default_value=True, help="Apply the integration window correction"
+    ).tag(config=True)
+
     @lru_cache(maxsize=128)
     def _calculate_correction(self, telid):
         """
         Calculate the correction for the extracted change such that the value
         returned would equal 1 for a noise-less unit pulse.
 
         This method is decorated with @lru_cache to ensure it is only
@@ -443,33 +451,39 @@
         charge, peak_time = extract_around_peak(
             waveforms,
             peak_index,
             self.window_width.tel[telid],
             self.window_shift.tel[telid],
             self.sampling_rate[telid],
         )
-        charge *= self._calculate_correction(telid=telid)[selected_gain_channel]
+        if self.apply_integration_correction.tel[telid]:
+            charge *= self._calculate_correction(telid=telid)[selected_gain_channel]
         return charge, peak_time
 
 
 class LocalPeakWindowSum(ImageExtractor):
     """
     Extractor which sums in a window about the
     peak in each pixel's waveform.
     """
 
     window_width = IntTelescopeParameter(
         default_value=7, help="Define the width of the integration window"
     ).tag(config=True)
+
     window_shift = IntTelescopeParameter(
         default_value=3,
         help="Define the shift of the integration window"
         "from the peak_index (peak_index - shift)",
     ).tag(config=True)
 
+    apply_integration_correction = BoolTelescopeParameter(
+        default_value=True, help="Apply the integration window correction"
+    ).tag(config=True)
+
     @lru_cache(maxsize=128)
     def _calculate_correction(self, telid):
         """
         Calculate the correction for the extracted change such that the value
         returned would equal 1 for a noise-less unit pulse.
 
         This method is decorated with @lru_cache to ensure it is only
@@ -500,38 +514,45 @@
         charge, peak_time = extract_around_peak(
             waveforms,
             peak_index,
             self.window_width.tel[telid],
             self.window_shift.tel[telid],
             self.sampling_rate[telid],
         )
-        charge *= self._calculate_correction(telid=telid)[selected_gain_channel]
+        if self.apply_integration_correction.tel[telid]:
+            charge *= self._calculate_correction(telid=telid)[selected_gain_channel]
         return charge, peak_time
 
 
 class NeighborPeakWindowSum(ImageExtractor):
     """
     Extractor which sums in a window about the
     peak defined by the wavefroms in neighboring pixels.
     """
 
     window_width = IntTelescopeParameter(
         default_value=7, help="Define the width of the integration window"
     ).tag(config=True)
+
     window_shift = IntTelescopeParameter(
         default_value=3,
         help="Define the shift of the integration window "
         "from the peak_index (peak_index - shift)",
     ).tag(config=True)
+
     lwt = IntTelescopeParameter(
         default_value=0,
         help="Weight of the local pixel (0: peak from neighbors only, "
         "1: local pixel counts as much as any neighbor)",
     ).tag(config=True)
 
+    apply_integration_correction = BoolTelescopeParameter(
+        default_value=True, help="Apply the integration window correction"
+    ).tag(config=True)
+
     @lru_cache(maxsize=128)
     def _calculate_correction(self, telid):
         """
         Calculate the correction for the extracted change such that the value
         returned would equal 1 for a noise-less unit pulse.
 
         This method is decorated with @lru_cache to ensure it is only
@@ -554,27 +575,31 @@
             readout.reference_pulse_sample_width.to_value("ns"),
             (1 / readout.sampling_rate).to_value("ns"),
             self.window_width.tel[telid],
             self.window_shift.tel[telid],
         )
 
     def __call__(self, waveforms, telid, selected_gain_channel):
-        neighbors = self.subarray.tel[telid].camera.geometry.neighbor_matrix_where
+        neighbors = self.subarray.tel[telid].camera.geometry.neighbor_matrix_sparse
         average_wfs = neighbor_average_waveform(
-            waveforms, neighbors, self.lwt.tel[telid]
+            waveforms,
+            neighbors_indices=neighbors.indices,
+            neighbors_indptr=neighbors.indptr,
+            lwt=self.lwt.tel[telid],
         )
         peak_index = average_wfs.argmax(axis=-1)
         charge, peak_time = extract_around_peak(
             waveforms,
             peak_index,
             self.window_width.tel[telid],
             self.window_shift.tel[telid],
             self.sampling_rate[telid],
         )
-        charge *= self._calculate_correction(telid=telid)[selected_gain_channel]
+        if self.apply_integration_correction.tel[telid]:
+            charge *= self._calculate_correction(telid=telid)[selected_gain_channel]
         return charge, peak_time
 
 
 class BaselineSubtractedNeighborPeakWindowSum(NeighborPeakWindowSum):
     """
     Extractor that first subtracts the baseline before summing in a
     window about the peak defined by the wavefroms in neighboring pixels.
@@ -637,87 +662,71 @@
             ("type", "LST*", 6.0),
             ("type", "MST*", 8.0),
             ("type", "SST*", 4.0),
         ],
         help="Picture threshold for internal tail-cuts pass",
     ).tag(config=True)
 
-    # Boolean that is used to disable the 2np pass and return the 1st pass
-    disable_second_pass = False
+    disable_second_pass = Bool(
+        default_value=False,
+        help="only run the first pass of the extractor, for debugging purposes",
+    ).tag(config=True)
 
-    def _calculate_correction(self, telid, widths, shifts, selected_gain_channel):
+    apply_integration_correction = BoolTelescopeParameter(
+        default_value=True, help="Apply the integration window correction"
+    ).tag(config=True)
+
+    @lru_cache(maxsize=4096)
+    def _calculate_correction(self, telid, width, shift):
         """Obtain the correction for the integration window specified for each
         pixel.
 
         The TwoPassWindowSum image extractor applies potentially different
         parameters for the integration window to each pixel, depending on the
         position of the peak. It has been decided to apply gain selection
         directly here. For basic definitions look at the documentation of
         `integration_correction`.
 
         Parameters
         ----------
         telid : int
             Index of the telescope in use.
-        widths : array of shape N_pixels
-            Width of the integration window (in units of n_samples)
-        shifts : array of shape N_pixels
-            Values of the window shifts per pixel.
+        width : int
+            Width of the integration window in samples
+        shift : int
+            Window shift to the left of the pulse peak in samples
 
         Returns
         -------
         correction : ndarray
             Value of the pixel-wise gain-selected integration correction.
 
         """
         readout = self.subarray.tel[telid].camera.readout
         # Calculate correction of first pixel for both channels
-        correction = integration_correction(
+        return integration_correction(
             readout.reference_pulse_shape,
             readout.reference_pulse_sample_width.to_value("ns"),
             (1 / readout.sampling_rate).to_value("ns"),
-            widths[0],
-            shifts[0],
-        )
-        # then do the same for each remaining pixel and attach the result as
-        # a column containing information from both channels
-        for pixel in range(len(selected_gain_channel)):
-            new_pixel_both_channels = integration_correction(
-                readout.reference_pulse_shape,
-                readout.reference_pulse_sample_width.to_value("ns"),
-                (1 / readout.sampling_rate).to_value("ns"),
-                widths[pixel],
-                shifts[pixel],
-            )
-            # stack the columns (i.e pixels) so the final correction array
-            # is N_channels X N_pixels
-            correction = np.column_stack((correction, new_pixel_both_channels))
-
-        # select the right channel per pixel
-        correction = np.asarray(
-            [
-                correction[:, pix_id][selected_gain_channel[pix_id]]
-                for pix_id in range(len(selected_gain_channel))
-            ]
+            width,
+            shift,
         )
-        return correction
 
-    def _apply_first_pass(self, waveforms, telid, selected_gain_channel):
+    def _apply_first_pass(
+        self, waveforms, telid
+    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
         Execute step 1.
 
         Parameters
         ----------
         waveforms : array of size (N_pixels, N_samples)
             DL0-level waveforms of one event.
         telid : int
             Index of the telescope.
-        selected_gain_channel: array of size (N_channels, N_pixels)
-            Array containing the index of the selected gain channel for each
-            pixel (0 for low gain, 1 for high gain).
 
         Returns
         -------
         charge : array_like
             Integrated charge per pixel.
             Shape: (n_pix)
         pulse_time : array_like
@@ -726,80 +735,77 @@
         """
         # STEP 1
 
         # Starting from DL0, the channel is already selected (if more than one)
         # event.dl0.tel[tel_id].waveform object has shape (N_pixels, N_samples)
 
         # For each pixel, we slide a 3-samples window through the
-        # waveform without touching the extremes (so later we can increase it
-        # to 5), summing each time the ADC counts contained within it.
+        # waveform summing each time the ADC counts contained within it.
+
+        peak_search_window_width = 3
+        sums = convolve1d(
+            waveforms, np.ones(peak_search_window_width), axis=1, mode="nearest"
+        )
+        # 'sums' has now still shape of (N_pixels, N_samples)
+        # each element is the center-sample of each 3-samples sliding window
+
+        # For each pixel, we check where the peak search window encountered
+        # the maximum number of ADC counts.
+        # We want to stop before the edge of the readout window in order to
+        # later extend the search window to a 1+3+1 integration window.
+        # Since in 'sums' the peak index corresponds to the center of the
+        # search window, we shift it on the right by 2 samples so to get the
+        # correspondent sample index in each waveform.
+        peak_index = np.argmax(sums[:, 2:-2], axis=1) + 2
+        # Now peak_index has the shape of (N_pixels).
+
+        # The final 5-samples window will be 1+3+1, centered on the 3-samples
+        # window in which the highest amount of ADC counts has been found
+        window_width = peak_search_window_width + 2
+        window_shift = 2
 
-        # 'width' could be configurable in a generalized version
-        # Right now this image extractor is optimized for LSTCam and NectarCam
-        width = 3
-        sums = np.apply_along_axis(slide_window, 1, waveforms[:, 1:-1], width)
-        # Note that the input waveforms are clipped at the extremes because
-        # we want to extend this 3-samples window to 5 samples
-        # 'sums' has now the shape of (N_pixels, N_samples-4)
-
-        # For each pixel, in each of the (N_samples - 4) positions, we check
-        # where the window encountered the maximum number of ADC counts
-        startWindows = np.apply_along_axis(np.argmax, 1, sums)
-        # Now startWindows has the shape of (N_pixels).
-        # Note that the index values stored in startWindows come from 'sums'
-        # of which the first index (0) corresponds of index 1 of each waveform
-        # since we clipped them before.
-
-        # Since we have to add 1 sample on each side, window_shift will always
-        # be (-)1, while window_width will always be window1_width + 1
-        # so we the final 5-samples window will be 1+3+1
-        window_widths = np.full_like(startWindows, width + 1)
-        window_shifts = np.full_like(startWindows, 1)
-
-        # the 'peak_index' argument of 'extract_around_peak' has a different
-        # meaning here: it's the start of the 3-samples window.
-        # Since since the "sums" arrays started from index 1 of each waveform,
-        # then each peak index has to be increased by one
+        # this function is applied to all pixels together
         charge_1stpass, pulse_time_1stpass = extract_around_peak(
             waveforms,
-            startWindows + 1,
-            window_widths,
-            window_shifts,
+            peak_index,
+            window_width,
+            window_shift,
             self.sampling_rate[telid],
         )
 
         # Get integration correction factors
-        correction = self._calculate_correction(
-            telid, window_widths, window_shifts, selected_gain_channel
-        )
+        if self.apply_integration_correction.tel[telid]:
+            correction = self._calculate_correction(telid, window_width, window_shift)
+        else:
+            correction = np.ones(waveforms.shape[0])
 
         return charge_1stpass, pulse_time_1stpass, correction
 
     def _apply_second_pass(
         self,
         waveforms,
         telid,
         selected_gain_channel,
-        charge_1stpass,
+        charge_1stpass_uncorrected,
         pulse_time_1stpass,
         correction,
-    ):
+    ) -> Tuple[np.ndarray, np.ndarray]:
         """
         Follow steps from 2 to 7.
 
         Parameters
         ----------
         waveforms : array of shape (N_pixels, N_samples)
             DL0-level waveforms of one event.
         telid : int
             Index of the telescope.
         selected_gain_channel: array of shape (N_channels, N_pixels)
             Array containing the index of the selected gain channel for each
             pixel (0 for low gain, 1 for high gain).
-        charge_1stpass : array of shape N_pixels
+        charge_1stpass_uncorrected : array of shape N_pixels
             Pixel charges reconstructed with the 1st pass, but not corrected.
         pulse_time_1stpass : array of shape N_pixels
             Pixel-wise pulse times reconstructed with the 1st pass.
         correction: array of shape N_pixels
             Charge correction from 1st pass.
 
         Returns
@@ -816,15 +822,15 @@
             Samples in which the waveform peak has been recognized.
             Same specifications as above.
             Shape: (n_pix)
         """
         # STEP 2
 
         # Apply correction to 1st pass charges
-        charge_1stpass = charge_1stpass * correction
+        charge_1stpass = charge_1stpass_uncorrected * correction[selected_gain_channel]
 
         # Set thresholds for core-pixels depending on telescope
         core_th = self.core_threshold.tel[telid]
         # Boundary thresholds will be half of core thresholds.
 
         # Preliminary image cleaning with simple two-level tail-cut
         camera_geometry = self.subarray.tel[telid].camera.geometry
@@ -848,28 +854,28 @@
         else:
             # ...find the biggest one
             mask_biggest = largest_island(labels)
             image_2 = image_1.copy()
             image_2[~mask_biggest] = 0
 
         # Indexes of pixels that will need the 2nd pass
-        nonCore_pixels_ids = np.where(image_2 < core_th)[0]
-        nonCore_pixels_mask = image_2 < core_th
+        non_core_pixels_ids = np.where(image_2 < core_th)[0]
+        non_core_pixels_mask = image_2 < core_th
 
         # STEP 4
 
         # if the resulting image has less then 3 pixels
         # or there are more than 3 pixels but all contain a number of
         # photoelectrons above the core threshold
         if np.count_nonzero(image_2) < 3:
             # we return the 1st pass information
             # NOTE: In this case, the image was not bright enough!
             # We should label it as "bad and NOT use it"
             return charge_1stpass, pulse_time_1stpass
-        elif len(nonCore_pixels_ids) == 0:
+        elif len(non_core_pixels_ids) == 0:
             # Since all reconstructed charges are above the core threshold,
             # there is no need to perform the 2nd pass.
             # We return the 1st pass information.
             # NOTE: In this case, even if this is 1st pass information,
             # the image is actually very bright! We should label it as "good"!
             return charge_1stpass, pulse_time_1stpass
 
@@ -877,30 +883,28 @@
         hillas = hillas_parameters(camera_geometry, image_2)
 
         # STEP 5
 
         # linear fit of pulse time vs. distance along major image axis
         # using only the main island surviving the preliminary
         # image cleaning
-        # WARNING: in case of outliers, the fit can perform better if
-        # it is a robust algorithm.
         timing = timing_parameters(camera_geometry, image_2, pulse_time_1stpass, hillas)
 
+        # If the fit returns nan
+        if np.isnan(timing.slope):
+            return charge_1stpass, pulse_time_1stpass
+
         # get projected distances along main image axis
         long, _ = camera_to_shower_coordinates(
-            camera_geometry.pix_x,
-            camera_geometry.pix_y,
-            hillas.x,
-            hillas.y,
-            hillas.psi,
+            camera_geometry.pix_x, camera_geometry.pix_y, hillas.x, hillas.y, hillas.psi
         )
 
         # get the predicted times as a linear relation
         predicted_pulse_times = (
-            timing.slope * long[nonCore_pixels_ids] + timing.intercept
+            timing.slope * long[non_core_pixels_ids] + timing.intercept
         )
 
         predicted_peaks = np.zeros(len(predicted_pulse_times))
 
         # Convert time in ns to sample index using the sampling rate from
         # the readout.
         # Approximate the value obtained to nearest integer, then cast to
@@ -912,83 +916,108 @@
         # Due to the fit these peak indexes can now be also outside of the
         # readout window, so later we check for this.
 
         # STEP 6
 
         # select only the waveforms correspondent to the non-core pixels
         # of the main island survived from the 1st pass image cleaning
-        nonCore_waveforms = waveforms[nonCore_pixels_ids]
+        non_core_waveforms = waveforms[non_core_pixels_ids]
 
         # Build 'width' and 'shift' arrays that adapt on the position of the
         # window along each waveform
 
-        # Now the definition of peak_index is really the peak.
-        # We have to add 2 samples each side, so the shist will always
-        # be (-)2, while width will always end 4 samples to the right.
-        # This "always" refers to a 5-samples window of course
-        window_widths = np.full_like(predicted_peaks, 4, dtype=np.int64)
-        window_shifts = np.full_like(predicted_peaks, 2, dtype=np.int64)
+        # As before we will integrate the charge in a 5-sample window centered
+        # on the peak
+        window_width_default = 5
+        window_shift_default = 2
+
+        # now let's deal with some edge cases: the predicted peak falls before
+        # or after the readout window:
+        peak_before_window = predicted_peaks < 0
+        peak_after_window = predicted_peaks > (non_core_waveforms.shape[1] - 1)
 
         # BUT, if the resulting 5-samples window falls outside of the readout
         # window then we take the first (or last) 5 samples
-        window_widths[predicted_peaks < 0] = 4
-        window_shifts[predicted_peaks < 0] = 0
-        window_widths[predicted_peaks > (waveforms.shape[1] - 1)] = 4
-        window_shifts[predicted_peaks > (waveforms.shape[1] - 1)] = 4
+        window_width_before = 5
+        window_shift_before = 0
+
+        # in the case where the window is after, shift backward
+        window_width_after = 5
+        window_shift_after = 5
+
+        # and put them together:
+        window_widths = np.full(non_core_waveforms.shape[0], window_width_default)
+        window_widths[peak_before_window] = window_width_before
+        window_widths[peak_after_window] = window_width_after
+        window_shifts = np.full(non_core_waveforms.shape[0], window_shift_default)
+        window_shifts[peak_before_window] = window_shift_before
+        window_shifts[peak_after_window] = window_shift_after
 
         # Now we can also (re)define the patological predicted times
         # because (we needed them to define the corrispective widths
         # and shifts)
-
         # set sample to 0 (beginning of the waveform) if predicted time
         # falls before
         predicted_peaks[predicted_peaks < 0] = 0
         # set sample to max-1 (first sample has index 0)
         # if predicted time falls after
         predicted_peaks[predicted_peaks > (waveforms.shape[1] - 1)] = (
             waveforms.shape[1] - 1
         )
 
         # re-calibrate non-core pixels using the fixed 5-samples window
-        charge_noCore, pulse_times_noCore = extract_around_peak(
-            nonCore_waveforms,
+        charge_no_core, pulse_times_no_core = extract_around_peak(
+            non_core_waveforms,
             predicted_peaks,
             window_widths,
             window_shifts,
             self.sampling_rate[telid],
         )
 
-        # Modify integration correction factors only for non-core pixels
-        correction_2ndPass = self._calculate_correction(
-            telid,
-            window_widths,
-            window_shifts,
-            selected_gain_channel[nonCore_pixels_ids],
-        )
-        np.put(correction, [nonCore_pixels_ids], correction_2ndPass)
+        if self.apply_integration_correction.tel[telid]:
+            # Modify integration correction factors only for non-core pixels
+            # now we compute 3 corrections for the default, before, and after cases:
+            correction = self._calculate_correction(
+                telid, window_width_default, window_shift_default
+            )[selected_gain_channel][non_core_pixels_mask]
+
+            correction_before = self._calculate_correction(
+                telid, window_width_before, window_shift_before
+            )[selected_gain_channel][non_core_pixels_mask]
+
+            correction_after = self._calculate_correction(
+                telid, window_width_after, window_shift_after
+            )[selected_gain_channel][non_core_pixels_mask]
+
+            correction[peak_before_window] = correction_before[peak_before_window]
+            correction[peak_after_window] = correction_after[peak_after_window]
+
+            charge_no_core *= correction
 
         # STEP 7
 
         # Combine core and non-core pixels in the final output
 
         # this is the biggest cluster from the cleaned image
         # it contains the core pixels (which we leave untouched)
         # plus possibly some non-core pixels
         charge_2ndpass = image_2.copy()
         # Now we overwrite the charges of all non-core pixels in the camera
         # plus all those pixels which didn't survive the preliminary
         # cleaning.
         # We apply also their corrections.
-        charge_2ndpass[nonCore_pixels_mask] = charge_noCore * correction_2ndPass
+        charge_2ndpass[non_core_pixels_mask] = charge_no_core
 
         # Same approach for the pulse times
-        pulse_time_2npass = pulse_time_1stpass  # core + non-core pixels
-        pulse_time_2npass[nonCore_pixels_mask] = pulse_times_noCore  # non-core pixels
+        pulse_time_2ndpass = pulse_time_1stpass  # core + non-core pixels
+        pulse_time_2ndpass[
+            non_core_pixels_mask
+        ] = pulse_times_no_core  # non-core pixels
 
-        return charge_2ndpass, pulse_time_2npass
+        return charge_2ndpass, pulse_time_2ndpass
 
     def __call__(self, waveforms, telid, selected_gain_channel):
         """
         Call this ImageExtractor.
 
         Parameters
         ----------
@@ -1006,23 +1035,21 @@
             Integrated charge per pixel.
             Shape: (n_pix)
         pulse_time : array_like
             Samples in which the waveform peak has been recognized.
             Shape: (n_pix)
         """
 
-        charge1, pulse_time1, correction1 = self._apply_first_pass(
-            waveforms, telid, selected_gain_channel
-        )
+        charge1, pulse_time1, correction1 = self._apply_first_pass(waveforms, telid)
 
         # FIXME: properly make sure that output is 32Bit instead of downcasting here
         if self.disable_second_pass:
             return (
-                (charge1 * correction1).astype("float32"),
+                (charge1 * correction1[selected_gain_channel]).astype("float32"),
                 pulse_time1.astype("float32"),
             )
 
         charge2, pulse_time2 = self._apply_second_pass(
-            waveforms, telid, selected_gain_channel, charge1, pulse_time1, correction1,
+            waveforms, telid, selected_gain_channel, charge1, pulse_time1, correction1
         )
         # FIXME: properly make sure that output is 32Bit instead of downcasting here
         return charge2.astype("float32"), pulse_time2.astype("float32")
```

### Comparing `ctapipe-0.8.0/ctapipe/image/geometry_converter_astri.py` & `ctapipe-0.9.1/ctapipe/image/geometry_converter_astri.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/geometry_converter_chec.py` & `ctapipe-0.9.1/ctapipe/image/geometry_converter_chec.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/geometry_converter_hex.py` & `ctapipe-0.9.1/ctapipe/image/geometry_converter_hex.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/hillas.py` & `ctapipe-0.9.1/ctapipe/image/hillas.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/leakage.py` & `ctapipe-0.9.1/ctapipe/image/leakage.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/muon/features.py` & `ctapipe-0.9.1/ctapipe/image/muon/features.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/muon/fitting.py` & `ctapipe-0.9.1/ctapipe/image/muon/fitting.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/muon/intensity_fitter.py` & `ctapipe-0.9.1/ctapipe/image/muon/intensity_fitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -210,14 +210,16 @@
     oversampling=3,
     min_lambda_m=300e-9,
     max_lambda_m=600e-9,
 ):
     """Function for producing the expected image for a given set of trial
     muon parameters without using astropy units but expecting the input to
     be in the correct ones.
+
+    See [chalmecalvet2013]_
     """
 
     # First produce angular position of each pixel w.r.t muon center
     dx = pixel_x_rad - center_x_rad
     dy = pixel_y_rad - center_y_rad
     ang = np.arctan2(dy, dx)
     # Add muon rotation angle
@@ -251,15 +253,15 @@
     # get total number of photons per pixel
     # ^ would be per radian, but no need to put it here, would anyway cancel out below
 
     pred *= alpha * (min_lambda_m ** -1 - max_lambda_m ** -1)
     pred *= pixel_diameter_rad / radius_rad
     # multiply by angle (in radians) subtended by pixel width as seen from ring center
 
-    pred *= np.sin(2 * radius_rad)
+    pred *= 0.5 * np.sin(2 * radius_rad)
 
     # multiply by gaussian weight, to account for "fraction of muon ring" which falls
     # within the pixel
     pred *= gauss
 
     # Now it would be the total light in an area S delimited by: two radii of the
     # ring, tangent to the sides of the pixel in question, and two circles concentric
@@ -271,76 +273,58 @@
     # diameter. In any case, since in the end we do a data-MC comparison of the muon
     # ring analysis outputs, it is not critical that this value is exact.
     pred *= CIRCLE_SQUARE_AREA_RATIO
 
     return pred
 
 
-def calc_likelihood(image, pred, spe_width, ped):
-    """Calculate likelihood of prediction given the measured signal,
-    gaussian approx from [denaurois2009]_
-
-    Parameters
-    ----------
-    image: ndarray
-        Pixel amplitudes from image
-    pred: ndarray
-        Predicted pixel amplitudes from model
-    spe_width: ndarray
-        width of single p.e. distribution
-    ped: ndarray
-        width of pedestal
-
-    Returns
-    -------
-    ndarray: likelihood for each pixel
-
-    """
-
-    sq = 1 / np.sqrt(2 * np.pi * (ped ** 2 + pred * (1 + spe_width ** 2)))
-    diff = (image - pred) ** 2
-    denom = 2 * (ped ** 2 + pred * (1 + spe_width ** 2))
-    expo = np.exp(-diff / denom) + 1e-16  # add small epsilon to avoid nans
-
-    log_value = sq * expo
-
-    likelihood_value = -2 * np.log(log_value)
-
-    return likelihood_value
-
-
 def build_negative_log_likelihood(
     image,
     telescope_description,
+    mask,
     oversampling,
     min_lambda,
     max_lambda,
     spe_width,
     pedestal,
     hole_radius=0 * u.m,
 ):
     """Create an efficient negative log_likelihood function that does
     not rely on astropy units internally by defining needed values as closures
-    in this function
+    in this function.
+
+    The likelihood is the gaussian approximation,
+    i.e. the unnumbered equation on page 22 between (24) and (25), from [denaurois2009]_
+
+    The logarithm of the likelihood is calculated analytically as far as possible
+    and terms constant under differentation are discarded.
     """
 
     # get all the neeed values and transform them into appropriate units
     optics = telescope_description.optics
     mirror_area = optics.mirror_area.to_value(u.m ** 2)
     mirror_radius = np.sqrt(mirror_area / np.pi)
 
     focal_length = optics.equivalent_focal_length
 
     cam = telescope_description.camera.geometry
     camera_frame = CameraFrame(focal_length=focal_length, rotation=cam.cam_rotation)
     cam_coords = SkyCoord(x=cam.pix_x, y=cam.pix_y, frame=camera_frame)
     tel_coords = cam_coords.transform_to(TelescopeFrame())
 
+    # Use only a subset of pixels, indicated by mask:
     pixel_x = tel_coords.fov_lon.to_value(u.rad)
     pixel_y = tel_coords.fov_lat.to_value(u.rad)
+
+    if mask is not None:
+        pixel_x = pixel_x[mask]
+        pixel_y = pixel_y[mask]
+        image = image[mask]
+        pedestal = pedestal[mask]
+
     pixel_diameter = 2 * (
         np.sqrt(cam.pix_area[0] / np.pi) / focal_length * u.rad
     ).to_value(u.rad)
 
     min_lambda = min_lambda.to_value(u.m)
     max_lambda = max_lambda.to_value(u.m)
 
@@ -373,20 +357,14 @@
         optical_efficiency_muon: float
             Efficiency of the optical system
 
         Returns
         -------
         float: Likelihood that model matches data
         """
-        # center_x *= self.unit
-        # center_y *= self.unit
-        # radius *= self.unit
-        # ring_width *= self.unit
-        # impact_parameter *= u.m
-        # phi *= u.rad
 
         # Generate model prediction
         prediction = image_prediction_no_units(
             mirror_radius_m=mirror_radius,
             hole_radius_m=hole_radius_m,
             impact_parameter_m=impact_parameter,
             phi_rad=phi,
@@ -398,26 +376,27 @@
             pixel_y_rad=pixel_y,
             pixel_diameter_rad=pixel_diameter,
             oversampling=oversampling,
             min_lambda_m=min_lambda,
             max_lambda_m=max_lambda,
         )
 
-        # scale prediction by optical efficiency of array
+        # scale prediction by optical efficiency of the telescope
         prediction *= optical_efficiency_muon
 
-        sq = 1 / np.sqrt(
-            2 * np.pi * (pedestal ** 2 + prediction * (1 + spe_width ** 2))
-        )
-        diff = (image - prediction) ** 2
-        denom = 2 * (pedestal ** 2 + prediction * (1 + spe_width ** 2))
-        expo = np.exp(-diff / denom) + 1e-16  # add small epsilon to avoid nans
-        value = sq * expo
+        # A gaussian approximation is used here, where the total
+        # standard deviation is the pedestal standard deviation (e.g. by NSB) and
+        # the single photon resolution times the image magnitude.
+        sigma2 = pedestal ** 2 + prediction * (1 + spe_width ** 2)
+
+        # gaussian negative log-likelihood, analytically simplified and
+        # constant terms discarded
+        neg_log_l = np.log(sigma2) + (image - prediction) ** 2 / sigma2
 
-        return -2 * np.log(value).sum()
+        return neg_log_l.sum()
 
     return negative_log_likelihood
 
 
 def create_initial_guess(center_x, center_y, radius, telescope_description):
     geometry = telescope_description.camera.geometry
     optics = telescope_description.optics
@@ -442,19 +421,19 @@
 
 class MuonIntensityFitter(TelescopeComponent):
     spe_width = FloatTelescopeParameter(
         help="Width of a single photo electron distribution", default_value=0.5
     ).tag(config=True)
 
     min_lambda_m = FloatTelescopeParameter(
-        help="Minimum wavelength for Cherenkov light in m", default_value=300e-9,
+        help="Minimum wavelength for Cherenkov light in m", default_value=300e-9
     ).tag(config=True)
 
     max_lambda_m = FloatTelescopeParameter(
-        help="Minimum wavelength for Cherenkov light in m", default_value=600e-9,
+        help="Minimum wavelength for Cherenkov light in m", default_value=600e-9
     ).tag(config=True)
 
     hole_radius_m = FloatTelescopeParameter(
         help="Hole radius of the reflector in m",
         default_value=[
             ("type", "LST_*", 0.308),
             ("type", "MST_*", 0.244),
@@ -462,17 +441,16 @@
         ],
     ).tag(config=True)
 
     oversampling = IntTelescopeParameter(
         help="Oversampling for the line integration", default_value=3
     ).tag(config=True)
 
-    def __call__(
-        self, tel_id, center_x, center_y, radius, image, pedestal,
-    ):
+
+    def __call__(self, tel_id, center_x, center_y, radius, image, pedestal, mask=None):
         """
 
         Parameters
         ----------
         center_x: Angle quantity
             Initial guess for muon ring center in telescope frame
         center_y: Angle quantity
@@ -481,14 +459,16 @@
             Radius of muon ring from circle fitting
         pixel_x: ndarray
             X position of pixels in image from circle fitting
         pixel_y: ndarray
             Y position of pixel in image from circle fitting
         image: ndarray
             Amplitude of image pixels
+        mask: ndarray
+            mask marking the pixels to be used in the likelihood fit
 
         Returns
         -------
         MuonEfficiencyContainer
         """
         telescope = self.subarray.tel[tel_id]
         if telescope.optics.num_mirrors != 1:
@@ -496,23 +476,24 @@
                 "Currently only single mirror telescopes"
                 f" are supported in {self.__class__.__name__}"
             )
 
         negative_log_likelihood = build_negative_log_likelihood(
             image,
             telescope,
+            mask,
             oversampling=self.oversampling.tel[tel_id],
             min_lambda=self.min_lambda_m.tel[tel_id] * u.m,
             max_lambda=self.max_lambda_m.tel[tel_id] * u.m,
             spe_width=self.spe_width.tel[tel_id],
             pedestal=pedestal,
             hole_radius=self.hole_radius_m.tel[tel_id] * u.m,
         )
 
-        initial_guess = create_initial_guess(center_x, center_y, radius, telescope,)
+        initial_guess = create_initial_guess(center_x, center_y, radius, telescope)
 
         step_sizes = {}
         step_sizes["error_impact_parameter"] = 0.5
         step_sizes["error_phi"] = np.deg2rad(0.5)
         step_sizes["error_ring_width"] = 0.001 * radius.to_value(u.rad)
         step_sizes["error_optical_efficiency_muon"] = 0.05
```

### Comparing `ctapipe-0.8.0/ctapipe/image/muon/ring_fitter.py` & `ctapipe-0.9.1/ctapipe/image/muon/ring_fitter.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/muon/tests/test_intensity_fit.py` & `ctapipe-0.9.1/ctapipe/image/muon/tests/test_intensity_fit.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/muon/tests/test_muon_features.py` & `ctapipe-0.9.1/ctapipe/image/muon/tests/test_muon_features.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/muon/tests/test_muon_fitting.py` & `ctapipe-0.9.1/ctapipe/image/muon/tests/test_muon_fitting.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/muon/tests/test_ring_fitter.py` & `ctapipe-0.9.1/ctapipe/image/muon/tests/test_ring_fitter.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/pixel_likelihood.py` & `ctapipe-0.9.1/ctapipe/image/pixel_likelihood.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/reducer.py` & `ctapipe-0.9.1/ctapipe/image/reducer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,45 @@
 """
 Algorithms for the data volume reduction.
 """
 from abc import abstractmethod
 import numpy as np
 from ctapipe.image import TailcutsImageCleaner
 from ctapipe.core import TelescopeComponent
-from ctapipe.core.traits import IntTelescopeParameter, BoolTelescopeParameter
-from ctapipe.image.extractor import NeighborPeakWindowSum
+from ctapipe.core.traits import IntTelescopeParameter, BoolTelescopeParameter, Unicode
+from ctapipe.image.extractor import ImageExtractor
 from ctapipe.image.cleaning import dilate
 
 __all__ = [
     "DataVolumeReducer",
     "NullDataVolumeReducer",
     "TailCutsDataVolumeReducer",
 ]
 
 
 class DataVolumeReducer(TelescopeComponent):
     """
     Base component for data volume reducers.
     """
 
-    def __init__(
-        self, config=None, parent=None, subarray=None, image_extractor=None, **kwargs
-    ):
+    def __init__(self, subarray, config=None, parent=None, **kwargs):
         """
         Parameters
         ----------
+        subarray: ctapipe.instrument.SubarrayDescription
+            Description of the subarray
         config: traitlets.loader.Config
             Configuration specified by config file or cmdline arguments.
             Used to set traitlet values.
             Set to None if no configuration to pass.
-        subarray: ctapipe.instrument.SubarrayDescription
-            Description of the subarray
-        image_extractor: ctapipe.image.extractor.ImageExtractor
-            The ImageExtractor to use for 'TailCutsDataVolumeReducer'.
-            If None, then NeighborPeakWindowSum will be used by default.
         kwargs
         """
-
         self.subarray = subarray
         super().__init__(config=config, parent=parent, subarray=subarray, **kwargs)
 
-        if image_extractor is None:
-            image_extractor = NeighborPeakWindowSum(parent=self, subarray=subarray)
-        self.image_extractor = image_extractor
-
-        self.cleaner = TailcutsImageCleaner(parent=self, subarray=subarray)
-
     def __call__(self, waveforms, telid=None, selected_gain_channel=None):
         """
         Call the relevant functions to perform data volume reduction on the
         waveforms.
 
         Parameters
         ----------
@@ -67,15 +55,14 @@
             extraction.
 
         Returns
         -------
         mask: array
             Mask of selected pixels.
         """
-
         mask = self.select_pixels(
             waveforms, telid=telid, selected_gain_channel=selected_gain_channel
         )
         return mask
 
     @abstractmethod
     def select_pixels(self, waveforms, telid=None, selected_gain_channel=None):
@@ -116,25 +103,60 @@
     """
     Reduce the time integrated shower image in 3 Steps:
 
     1) Select pixels with tailcuts_clean.
     2) Add iteratively all pixels with Signal S >= boundary_thresh
        with ctapipe module dilate until no new pixels were added.
     3) Adding new pixels with dilate to get more conservative.
-    """
 
+    Attributes
+    ----------
+    image_extractor_type: String
+        Name of the image_extractor to be used.
+    n_end_dilates: IntTelescopeParameter
+        Number of how many times to dilate at the end.
+    do_boundary_dilation: BoolTelescopeParameter
+        If set to 'False', the iteration steps in 2) are skipped and
+        normal TailcutCleaning is used.
+    """
+    image_extractor_type = Unicode(
+        default_value="NeighborPeakWindowSum", help="Name of the image_extractor"
+        "to be used.",
+    ).tag(config=True)
     n_end_dilates = IntTelescopeParameter(
         default_value=1, help="Number of how many times to dilate at the end."
     ).tag(config=True)
     do_boundary_dilation = BoolTelescopeParameter(
         default_value=True,
         help="If set to 'False', the iteration steps in 2) are skipped and"
         "normal TailcutCleaning is used.",
     ).tag(config=True)
 
+    def __init__(self, subarray, config=None, parent=None, **kwargs):
+        """
+        Parameters
+        ----------
+        subarray: ctapipe.instrument.SubarrayDescription
+            Description of the subarray
+        config: traitlets.loader.Config
+            Configuration specified by config file or cmdline arguments.
+            Used to set traitlet values.
+            Set to None if no configuration to pass.
+        kwargs
+        """
+        super().__init__(config=config, parent=parent, subarray=subarray, **kwargs)
+
+        self.cleaner = TailcutsImageCleaner(parent=self, subarray=self.subarray)
+
+        self.image_extractor = ImageExtractor.from_name(
+            self.image_extractor_type,
+            subarray=self.subarray,
+            parent=self
+        )
+
     def select_pixels(self, waveforms, telid=None, selected_gain_channel=None):
         camera_geom = self.subarray.tel[telid].camera.geometry
         # Pulse-integrate waveforms
         charge, _ = self.image_extractor(
             waveforms, telid=telid, selected_gain_channel=selected_gain_channel
         )
```

### Comparing `ctapipe-0.8.0/ctapipe/image/statistics.py` & `ctapipe-0.9.1/ctapipe/image/statistics.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_cleaning.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_cleaning.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_concentration.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_concentration.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_extractor.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     neighbor_average_waveform,
     subtract_baseline,
     integration_correction,
     ImageExtractor,
     FixedWindowSum,
     NeighborPeakWindowSum,
     TwoPassWindowSum,
+    FullWaveformSum,
 )
 from ctapipe.image.toymodel import WaveformModel
 from ctapipe.instrument import SubarrayDescription, TelescopeDescription
 
 extractors = non_abstract_children(ImageExtractor)
 # FixedWindowSum has no peak finding and need to be set manually
 extractors.remove(FixedWindowSum)
@@ -154,28 +155,39 @@
         waveforms, peak_index, width, shift, sampling_rate_ghz
     )
     assert_equal(charge, n_samples)
 
 
 def test_neighbor_average_waveform(toymodel):
     waveforms, subarray, telid, _, _, _ = toymodel
-    nei = subarray.tel[telid].camera.geometry.neighbor_matrix_where
-    average_wf = neighbor_average_waveform(waveforms, nei, 0)
+    neighbors = subarray.tel[telid].camera.geometry.neighbor_matrix_sparse
+    average_wf = neighbor_average_waveform(
+        waveforms,
+        neighbors_indices=neighbors.indices,
+        neighbors_indptr=neighbors.indptr,
+        lwt=0,
+    )
 
     pixel = 0
-    nei_pixel = list((np.unique(nei[np.where(nei == pixel)[0]])))
-    nei_pixel.remove(pixel)
+    _, nei_pixel = np.where(neighbors[pixel].A)
     expected_average = waveforms[nei_pixel].sum(0) / len(nei_pixel)
     assert_allclose(average_wf[pixel], expected_average, rtol=1e-3)
 
+    lwt = 4
+    average_wf = neighbor_average_waveform(
+        waveforms,
+        neighbors_indices=neighbors.indices,
+        neighbors_indptr=neighbors.indptr,
+        lwt=lwt,
+    )
+
     pixel = 1
-    nei_pixel = list((np.unique(nei[np.where(nei == pixel)[0]])))
-    nei_pixel.extend([pixel] * 3)
+    _, nei_pixel = np.where(neighbors[pixel].A)
+    nei_pixel = np.concatenate([nei_pixel, [pixel] * lwt])
     expected_average = waveforms[nei_pixel].sum(0) / len(nei_pixel)
-    average_wf = neighbor_average_waveform(waveforms, nei, 4)
     assert_allclose(average_wf[pixel], expected_average, rtol=1e-3)
 
 
 def test_extract_peak_time_within_range():
     x = np.arange(100)
     # Generic waveform that goes from positive to negative in window
     # Can cause extreme values with incorrect handling of weighted average
@@ -248,17 +260,34 @@
     waveforms, subarray, telid, selected_gain_channel, true_charge, true_time = toymodel
     extractor = Extractor(subarray=subarray)
     charge, peak_time = extractor(waveforms, telid, selected_gain_channel)
     assert_allclose(charge, true_charge, rtol=0.1)
     assert_allclose(peak_time, true_time, rtol=0.1)
 
 
+@pytest.mark.parametrize("Extractor", extractors)
+def test_integration_correction_off(Extractor, toymodel):
+    # full waveform extractor does not have an integration correction
+    if Extractor is FullWaveformSum:
+        return
+
+    waveforms, subarray, telid, selected_gain_channel, true_charge, true_time = toymodel
+    extractor = Extractor(subarray=subarray, apply_integration_correction=False)
+    charge, peak_time = extractor(waveforms, telid, selected_gain_channel)
+
+    # peak time should stay the same
+    assert_allclose(peak_time, true_time, rtol=0.1)
+
+    # charge should be too small without correction
+    assert np.all(charge <= true_charge)
+
+
 def test_fixed_window_sum(toymodel):
     waveforms, subarray, telid, selected_gain_channel, true_charge, true_time = toymodel
-    extractor = FixedWindowSum(subarray=subarray, window_start=47)
+    extractor = FixedWindowSum(subarray=subarray, peak_index=47)
     charge, peak_time = extractor(waveforms, telid, selected_gain_channel)
     assert_allclose(charge, true_charge, rtol=0.1)
     assert_allclose(peak_time, true_time, rtol=0.1)
 
 
 def test_neighbor_peak_window_sum_lwt(toymodel):
     waveforms, subarray, telid, selected_gain_channel, true_charge, true_time = toymodel
@@ -280,16 +309,16 @@
             subarray,
             telid,
             selected_gain_channel,
             true_charge,
             true_time,
         ) = toymodel
         charge, pulse_time = extractor(waveforms, telid, selected_gain_channel)
-        assert_allclose(charge, true_charge, rtol=0.07)
-        assert_allclose(pulse_time, true_time, rtol=0.07)
+        assert_allclose(charge, true_charge, rtol=0.1)
+        assert_allclose(pulse_time, true_time, rtol=0.1)
 
 
 def test_waveform_extractor_factory(toymodel):
     waveforms, subarray, telid, selected_gain_channel, true_charge, true_time = toymodel
     extractor = ImageExtractor.from_name("LocalPeakWindowSum", subarray=subarray)
     charge, peak_time = extractor(waveforms, telid, selected_gain_channel)
     assert_allclose(charge, true_charge, rtol=0.1)
@@ -316,28 +345,28 @@
     waveforms, subarray, _, _, _, _ = toymodel
     _, n_samples = waveforms.shape
 
     config = Config(
         {
             "ImageExtractor": {
                 "window_width": [("type", "*", n_samples), ("id", "2", n_samples // 2)],
-                "window_start": 0,
+                "peak_index": 0,
             }
         }
     )
 
     waveforms, subarray, _, _, _, _ = toymodel
     n_pixels, n_samples = waveforms.shape
     extractor = ImageExtractor.from_name(
         "FixedWindowSum", subarray=subarray, config=config
     )
 
-    assert extractor.window_start.tel[None] == 0
-    assert extractor.window_start.tel[1] == 0
-    assert extractor.window_start.tel[2] == 0
+    assert extractor.peak_index.tel[None] == 0
+    assert extractor.peak_index.tel[1] == 0
+    assert extractor.peak_index.tel[2] == 0
     assert extractor.window_width.tel[None] == n_samples
     assert extractor.window_width.tel[1] == n_samples
     assert extractor.window_width.tel[2] == n_samples // 2
 
 
 @pytest.mark.parametrize("Extractor", non_abstract_children(ImageExtractor))
 def test_dtype(Extractor, subarray):
```

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_geometry_converter.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_geometry_converter.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_hillas.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_hillas.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_image_cleaner_component.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_image_cleaner_component.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_leakage.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_leakage.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_morphology.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_morphology.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,31 +6,37 @@
 def test_number_of_islands():
     from ctapipe.image import number_of_islands
 
     # test with LST geometry (1855 pixels)
     geom = CameraGeometry.from_name("LSTCam")
 
     # create 18 triggered pixels grouped to 5 clusters
-    island_mask_true = np.zeros(geom.n_pixels)
     mask = np.zeros(geom.n_pixels).astype("bool")
     triggered_pixels = np.array(
         [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 37, 38, 111, 222]
     )
-    island_mask_true[[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13]] = 1
-    island_mask_true[14] = 2
-    island_mask_true[[37, 38]] = 3
-    island_mask_true[111] = 4
-    island_mask_true[222] = 5
-    mask[triggered_pixels] = 1
+    mask[triggered_pixels] = True
 
-    n_islands, island_mask = number_of_islands(geom, mask)
+    island_labels_true = np.zeros(geom.n_pixels, dtype=np.int16)
+    island_labels_true[[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13]] = 1
+    island_labels_true[14] = 2
+    island_labels_true[[37, 38]] = 3
+    island_labels_true[111] = 4
+    island_labels_true[222] = 5
+
+    n_islands, island_labels = number_of_islands(geom, mask)
     n_islands_true = 5
+    # non cleaning pixels should be zero
+    assert np.all(island_labels[~mask] == 0)
+    # all other should have some label
+    assert np.all(island_labels[mask] > 0)
+
     assert n_islands == n_islands_true
-    assert_allclose(island_mask, island_mask_true)
-    assert island_mask.dtype == np.int32
+    assert_allclose(island_labels, island_labels_true)
+    assert island_labels.dtype == np.int16
 
 
 def test_number_of_island_sizes():
     from ctapipe.image import number_of_island_sizes
 
     island_labels = np.array(
         100 * [0]
```

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_pixel_likelihood.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_pixel_likelihood.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_reducer.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_reducer.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             "TailCutsDataVolumeReducer": {
                 "TailcutsImageCleaner": {
                     "picture_threshold_pe": 700.0,
                     "boundary_threshold_pe": 350.0,
                     "min_picture_neighbors": 0,
                     "keep_isolated_pixels": True,
                 },
+                "image_extractor_type": "NeighborPeakWindowSum",
                 "n_end_dilates": 1,
                 "do_boundary_dilation": True,
             }
         }
     )
     reducer = TailCutsDataVolumeReducer(config=reduction_param, subarray=subarray)
     reduced_waveforms = waveforms_signal.copy()
```

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_statistics.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_timing_parameters.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_timing_parameters.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/tests/test_toy.py` & `ctapipe-0.9.1/ctapipe/image/tests/test_toy.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/image/timing.py` & `ctapipe-0.9.1/ctapipe/image/timing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 """
 Image timing-based shower image parametrization.
 """
 
 import numpy as np
 import astropy.units as u
-from numpy.polynomial.polynomial import polyval
 from ..containers import TimingParametersContainer
 from .hillas import camera_to_shower_coordinates
 from ..utils.quantities import all_to_value
+from ..fitting import lts_linear_regression
 
-from scipy.stats import siegelslopes
+from numba import njit
 
 
 __all__ = ["timing_parameters"]
 
 
+@njit
+def rmse(truth, prediction):
+    """Root mean squared error"""
+    return np.sqrt(np.mean((truth - prediction) ** 2))
+
+
 def timing_parameters(geom, image, peak_time, hillas_parameters, cleaning_mask=None):
     """
     Function to extract timing parameters from a cleaned image.
 
     Parameters
     ----------
     geom: ctapipe.instrument.CameraGeometry
@@ -36,14 +42,17 @@
     Returns
     -------
     timing_parameters: TimingParametersContainer
     """
 
     unit = geom.pix_x.unit
 
+    # numba needs arguments to be the same type, so upcast to float64 if necessary
+    peak_time = peak_time.astype(np.float64)
+
     if cleaning_mask is not None:
         image = image[cleaning_mask]
         geom = geom[cleaning_mask]
         peak_time = peak_time[cleaning_mask]
 
     if (image < 0).any():
         raise ValueError("The non-masked pixels must verify signal >= 0")
@@ -58,18 +67,20 @@
     )
 
     # use polyfit just to get the covariance matrix and errors
     (_s, _i), cov = np.polyfit(longi, peak_time, deg=1, w=np.sqrt(image), cov=True)
     slope_err, intercept_err = np.sqrt(np.diag(cov))
 
     # re-fit using a robust-to-outlier algorithm
-    slope, intercept = siegelslopes(x=longi, y=peak_time)
-    predicted_time = polyval(longi, (intercept, slope))
-    deviation = np.sqrt(np.sum((peak_time - predicted_time) ** 2) / peak_time.size)
+    beta, error = lts_linear_regression(x=longi, y=peak_time, samples=5)
+
+    # error from lts_linear_regression is only for the used points,
+    # recalculate for all points
+    deviation = rmse(longi * beta[0] + beta[1], peak_time)
 
     return TimingParametersContainer(
-        slope=slope / unit,
-        intercept=intercept,
+        slope=beta[0] / unit,
+        intercept=beta[1],
         deviation=deviation,
         slope_err=slope_err / unit,
         intercept_err=intercept_err,
     )
```

### Comparing `ctapipe-0.8.0/ctapipe/image/toymodel.py` & `ctapipe-0.9.1/ctapipe/image/toymodel.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/instrument/__init__.py` & `ctapipe-0.9.1/ctapipe/instrument/__init__.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/instrument/atmosphere.py` & `ctapipe-0.9.1/ctapipe/instrument/atmosphere.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/instrument/camera/description.py` & `ctapipe-0.9.1/ctapipe/instrument/camera/description.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/instrument/camera/geometry.py` & `ctapipe-0.9.1/ctapipe/instrument/camera/geometry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 Utilities for reading or working with Camera geometry files
 """
 import logging
+import warnings
+from typing import TypeVar
 
 import numpy as np
 from astropy import units as u
 from astropy.coordinates import Angle, SkyCoord
+from astropy.coordinates import BaseCoordinateFrame
 from astropy.table import Table
 from astropy.utils import lazyproperty
-from scipy.spatial import cKDTree as KDTree
 from scipy.sparse import lil_matrix, csr_matrix
-import warnings
+from scipy.spatial import cKDTree as KDTree
 
+from ctapipe.coordinates import CameraFrame
 from ctapipe.utils import get_table_dataset
 from ctapipe.utils.linalg import rotation_matrix_2d
-from ctapipe.coordinates import CameraFrame
-
 
 __all__ = ["CameraGeometry", "UnknownPixelShapeWarning"]
 
 logger = logging.getLogger(__name__)
+CG = TypeVar("CG", bound="CameraGeometry")  # for forward-referencing type hints
 
 
 class CameraGeometry:
     """`CameraGeometry` is a class that stores information about a
     Cherenkov Camera that us useful for imaging algorithms and
     displays. It contains lists of pixel positions, areas, pixel
     shapes, as well as a neighbor (adjacency) list and matrix for each pixel.
@@ -130,15 +132,15 @@
         if self.pix_type != other.pix_type:
             return False
 
         if self.pix_rotation != other.pix_rotation:
             return False
 
         return all(
-            [(self.pix_x == other.pix_x).all(), (self.pix_y == other.pix_y).all(),]
+            [(self.pix_x == other.pix_x).all(), (self.pix_y == other.pix_y).all()]
         )
 
     def guess_radius(self):
         """
         Guess the camera radius as mean distance of the border pixels from
         the center pixel
         """
@@ -146,59 +148,77 @@
         cx = self.pix_x.mean()
         cy = self.pix_y.mean()
 
         return np.sqrt(
             (self.pix_x[border] - cx) ** 2 + (self.pix_y[border] - cy) ** 2
         ).mean()
 
-    def transform_to(self, frame):
-        """
-        Transform the pixel coordinates stored in this geometry
-        and the pixel and camera rotations to another camera coordinate frame.
+    def transform_to(self, frame: BaseCoordinateFrame) -> CG:
+        """Transform the pixel coordinates stored in this geometry and the pixel
+        and camera rotations to another camera coordinate frame.
+
+        Note that `geom.frame` must contain all the necessary attributes needed
+        to transform into the requested frame, i.e. if going from `CameraFrame`
+        to `TelescopeFrame`, it should contain a `focal_length` attribute.
 
         Parameters
         ----------
         frame: ctapipe.coordinates.CameraFrame
             The coordinate frame to transform to.
+
+        Returns
+        -------
+        CameraGeometry:
+            new instance in the requested Frame
         """
         if self.frame is None:
             self.frame = CameraFrame()
 
-        coord = SkyCoord(x=self.pix_x, y=self.pix_y, frame=self.frame)
+        coord = SkyCoord(self.pix_x, self.pix_y, frame=self.frame)
         trans = coord.transform_to(frame)
 
         # also transform the unit vectors, to get rotation / mirroring
-        uv = SkyCoord(x=[1, 0], y=[0, 1], unit=u.m, frame=self.frame)
+        uv = SkyCoord([1, 0], [0, 1], unit=self.pix_x.unit, frame=self.frame)
         uv_trans = uv.transform_to(frame)
-        rot = np.arctan2(uv_trans[0].y, uv_trans[1].y)
-        det = np.linalg.det([uv_trans.x.value, uv_trans.y.value])
 
-        cam_rotation = rot + det * self.cam_rotation
-        pix_rotation = rot + det * self.pix_rotation
+        # some trickery has to be done to deal with the fact that not all frames
+        # use the same x/y attributes. Therefore we get the component names, and
+        # access them by string:
+        frame_attrs = list(uv_trans.frame.get_representation_component_names().keys())
+        uv_x = getattr(uv_trans, frame_attrs[0])
+        uv_y = getattr(uv_trans, frame_attrs[1])
+        trans_x = getattr(trans, frame_attrs[0])
+        trans_y = getattr(trans, frame_attrs[1])
+
+        rot = np.arctan2(uv_y[0], uv_y[1])
+        det = np.linalg.det([uv_x.value, uv_y.value])
+
+        cam_rotation = rot - self.cam_rotation
+        pix_rotation = rot - self.pix_rotation
 
         return CameraGeometry(
             camera_name=self.camera_name,
             pix_id=self.pix_id,
-            pix_x=trans.x,
-            pix_y=trans.y,
-            pix_area=self.pix_area,
+            pix_x=trans_x,
+            pix_y=trans_y,
+            pix_area=self.guess_pixel_area(trans_x, trans_y, self.pix_type),
             pix_type=self.pix_type,
             pix_rotation=pix_rotation,
             cam_rotation=cam_rotation,
-            neighbors=None,
+            neighbors=self._neighbors,
             apply_derotation=False,
             frame=frame,
         )
 
     def __hash__(self):
         return hash(
             (
                 self.camera_name,
-                self.pix_x[0].to_value(u.m),
-                self.pix_y[0].to_value(u.m),
+                self.pix_x[0].value,
+                self.pix_y[0].value,
                 self.pix_type,
                 self.pix_rotation.deg,
             )
         )
 
     def __len__(self):
         return self.n_pixels
@@ -292,17 +312,15 @@
 
         Returns
         -------
         kdtree
 
         """
 
-        pixel_centers = np.column_stack(
-            [self.pix_x.to_value(u.m), self.pix_y.to_value(u.m)]
-        )
+        pixel_centers = np.column_stack([self.pix_x.value, self.pix_y.value])
         return KDTree(pixel_centers)
 
     @lazyproperty
     def _all_pixel_areas_equal(self):
         """
         Pre-calculated kdtree of all pixel centers inside camera
 
@@ -484,27 +502,14 @@
                 warnings.warn(
                     "Neighbor matrix is not symmetric. Is camera geometry irregular?"
                 )
 
         return neighbors.tocsr()
 
     @lazyproperty
-    def neighbor_matrix_where(self):
-        """
-        Obtain a 2D array, where each row is [pixel index, one neighbour
-        of that pixel].
-
-        Returns
-        -------
-        ndarray
-        """
-        coo = self.neighbor_matrix_sparse.tocoo()
-        return np.column_stack([coo.row, coo.col])
-
-    @lazyproperty
     def pixel_moment_matrix(self):
         """
         Pre-calculated matrix needed for higher-order moment calculation,
         up to 4th order.
 
         Note this is *not* recalculated if the CameraGeometry is modified.
 
@@ -680,17 +685,17 @@
                     outside camera
         """
 
         if not self._all_pixel_areas_equal:
             logger.warning(
                 " Method not implemented for cameras with varying pixel sizes"
             )
-
-        points_searched = np.dstack([x.to_value(u.m), y.to_value(u.m)])
-        circum_rad = self._pixel_circumferences[0].to_value(u.m)
+        unit = x.unit
+        points_searched = np.dstack([x.to_value(unit), y.to_value(unit)])
+        circum_rad = self._pixel_circumferences[0].to_value(unit)
         kdtree = self._kdtree
         dist, pix_indices = kdtree.query(
             points_searched, distance_upper_bound=circum_rad
         )
         del dist
         pix_indices = pix_indices.flatten()
 
@@ -714,21 +719,21 @@
             insidepix_index = np.where(~border_mask)[0][0]
             # Check in detail whether location is in border pixel or outside camera:
             for borderpix_index in borderpix_indices_in_list:
                 index = np.where(pix_indices == borderpix_index)[0][0]
                 # compare with inside pixel:
                 xprime = (
                     points_searched[0][index, 0]
-                    - self.pix_x[borderpix_index].to_value(u.m)
-                    + self.pix_x[insidepix_index].to_value(u.m)
+                    - self.pix_x[borderpix_index].to_value(unit)
+                    + self.pix_x[insidepix_index].to_value(unit)
                 )
                 yprime = (
                     points_searched[0][index, 1]
-                    - self.pix_y[borderpix_index].to_value(u.m)
-                    + self.pix_y[insidepix_index].to_value(u.m)
+                    - self.pix_y[borderpix_index].to_value(unit)
+                    + self.pix_y[insidepix_index].to_value(unit)
                 )
                 dist_check, index_check = kdtree.query(
                     [xprime, yprime], distance_upper_bound=circum_rad
                 )
                 del dist_check
                 if index_check != insidepix_index:
                     pix_indices[index] = -1
```

### Comparing `ctapipe-0.8.0/ctapipe/instrument/camera/readout.py` & `ctapipe-0.9.1/ctapipe/instrument/camera/readout.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/instrument/camera/tests/test_geometry.py` & `ctapipe-0.9.1/ctapipe/instrument/camera/tests/test_geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,18 +40,15 @@
     assert len(geom.pix_x) == 1855
     assert geom.pix_type == "hexagonal"
 
 
 def test_position_to_pix_index():
     """ test that we can lookup a pixel from a coordinate"""
     geom = CameraGeometry.from_name("LSTCam")
-    x, y = (
-        0.80 * u.m,
-        0.79 * u.m,
-    )
+    x, y = (0.80 * u.m, 0.79 * u.m)
     pix_id = geom.position_to_pix_index(x, y)
     assert pix_id == 1790
 
 
 def test_find_neighbor_pixels():
     """ test basic neighbor functionality """
     n_pixels = 5
@@ -174,15 +171,15 @@
     """
     geom = CameraGeometry(
         camera_name="TestCam",
         pix_id=np.arange(3),
         pix_x=np.arange(3) * u.deg,
         pix_y=np.arange(3) * u.deg,
         pix_area=np.ones(3) * u.deg ** 2,
-        neighbors=[[1,], [0, 2], [1,]],
+        neighbors=[[1], [0, 2], [1]],
         pix_type="rectangular",
         pix_rotation="0deg",
         cam_rotation="0deg",
     )
 
     neigh = geom.neighbors
     assert len(neigh) == len(geom.pix_x)
@@ -281,23 +278,37 @@
     camera = CameraGeometry.from_name(camera_name)
     assert str(camera) == camera_name
 
 
 @pytest.mark.parametrize("camera_name", camera_names)
 def test_camera_coordinate_transform(camera_name):
     """test conversion of the coordinates stored in a camera frame"""
-    from ctapipe.coordinates import EngineeringCameraFrame
+    from ctapipe.coordinates import EngineeringCameraFrame, CameraFrame, TelescopeFrame
 
     geom = CameraGeometry.from_name(camera_name)
     trans_geom = geom.transform_to(EngineeringCameraFrame())
 
     unit = geom.pix_x.unit
     assert np.allclose(geom.pix_x.to_value(unit), -trans_geom.pix_y.to_value(unit))
     assert np.allclose(geom.pix_y.to_value(unit), -trans_geom.pix_x.to_value(unit))
 
+    # also test converting into a spherical frame:
+    focal_length = 1.2 * u.m
+    geom.frame = CameraFrame(focal_length=focal_length)
+    telescope_frame = TelescopeFrame()
+    sky_geom = geom.transform_to(telescope_frame)
+
+    x = sky_geom.pix_x.to_value(u.deg)
+    assert len(x) == len(geom.pix_x)
+
+    # and test going backward from spherical to cartesian:
+
+    geom_cam = sky_geom.transform_to(CameraFrame(focal_length=focal_length))
+    assert np.allclose(geom_cam.pix_x.to_value(unit), geom.pix_x.to_value(unit))
+
 
 def test_guess_area():
     x = u.Quantity([0, 1, 2], u.cm)
     y = u.Quantity([0, 0, 0], u.cm)
     n_pixels = len(x)
 
     geom = CameraGeometry(
```

### Comparing `ctapipe-0.8.0/ctapipe/instrument/camera/tests/test_readout.py` & `ctapipe-0.9.1/ctapipe/instrument/camera/tests/test_readout.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/instrument/guess.py` & `ctapipe-0.9.1/ctapipe/instrument/guess.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 
 GuessingKey = namedtuple("GuessingKey", ["n_pixels", "focal_length"])
 GuessingResult = namedtuple(
     "GuessingResult", ["type", "name", "camera_name", "n_mirrors"]
 )
 
 
+# focal length must have at most two digits after period
+# as we round the lookup to two digits
 TELESCOPE_NAMES = {
     GuessingKey(2048, 2.28): GuessingResult("SST", "GCT", "CHEC", 2),
     GuessingKey(2368, 2.15): GuessingResult("SST", "ASTRI", "ASTRICam", 2),
     GuessingKey(2048, 2.15): GuessingResult("SST", "ASTRI", "CHEC", 2),
     GuessingKey(1296, 5.60): GuessingResult("SST", "1M", "DigiCam", 1),
     GuessingKey(1764, 16.0): GuessingResult("MST", "MST", "FlashCam", 1),
     GuessingKey(1855, 16.0): GuessingResult("MST", "MST", "NectarCam", 1),
     GuessingKey(1855, 28.0): GuessingResult("LST", "LST", "LSTCam", 1),
     GuessingKey(11328, 5.59): GuessingResult("MST", "SCT", "SCTCam", 1),
     # Non-CTA Telescopes
     GuessingKey(1039, 16.97): GuessingResult("LST", "MAGIC", "MAGICCam", 1),
     GuessingKey(960, 15.0): GuessingResult("MST", "HESS-I", "HESS-I", 1),
     GuessingKey(2048, 36.0): GuessingResult("LST", "HESS-II", "HESS-II", 1),
-    GuessingKey(1440, 4.998): GuessingResult("SST", "FACT", "FACT", 1),
+    GuessingKey(1440, 4.89): GuessingResult("SST", "FACT", "FACT", 1),
 }
 
 UNKNOWN_TELESCOPE = GuessingResult("UNKNOWN", "UNKNOWN", "UNKNOWN", -1)
 
 
 def guess_telescope(n_pixels, focal_length):
     """
```

### Comparing `ctapipe-0.8.0/ctapipe/instrument/optics.py` & `ctapipe-0.9.1/ctapipe/instrument/optics.py`

 * *Files 24% similar despite different names*

```diff
@@ -91,21 +91,44 @@
 
         Returns
         -------
         OpticsDescription
 
         """
         table = get_table_dataset(optics_table, role="dl0.tel.svc.optics")
-        mask = table["tel_description"] == name
-        if mask.sum() == 0:
+
+        version = table.meta.get("TAB_VER")
+
+        # we introduced the TAB_VER after switching to the second version
+        # of this table, so when the version is missing, it can be either 1 or 2
+        # we guess the version by looking for the mirror_type attribute.
+        if version is None:
+            if "mirror_type" in table.colnames:
+                version = "1.0"
+            else:
+                version = "2.0"
+
+        if version not in {"1.0", "2.0"}:
+            raise ValueError(f"Unsupported version of optics table: {version}")
+
+        if version == "1.0":
+            mask = table["tel_description"] == name
+        elif version == "2.0":
+            mask = table["description"] == name
+
+        if np.count_nonzero(mask) == 0:
             raise ValueError(f"Unknown telescope name {name}")
 
+        if version == "1.0":
+            num_mirrors = 1 if table["mirror_type"][mask][0] == "DC" else 2
+        elif version == "2.0":
+            num_mirrors = table["num_mirrors"][mask][0]
+
         flen = table["equivalent_focal_length"][mask].quantity[0]
 
-        num_mirrors = 1 if table["mirror_type"][mask][0] == "DC" else 2
         optics = cls(
             name=name,
             num_mirrors=num_mirrors,
             equivalent_focal_length=flen,
             mirror_area=table["mirror_area"][mask].quantity[0],
             num_mirror_tiles=table["num_mirror_tiles"][mask][0],
         )
```

### Comparing `ctapipe-0.8.0/ctapipe/instrument/subarray.py` & `ctapipe-0.9.1/ctapipe/instrument/subarray.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """
 Description of Arrays or Subarrays of telescopes
 """
 
 __all__ = ["SubarrayDescription"]
 
 from collections import defaultdict
+from pathlib import Path
 
 import numpy as np
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 from astropy.table import Table
 from astropy.utils import lazyproperty
+import tables
 
 import ctapipe
 
 from ..coordinates import GroundFrame
-from . import TelescopeDescription
+from .telescope import TelescopeDescription
+from .camera import CameraDescription, CameraReadout, CameraGeometry
+from .optics import OpticsDescription
 
 
 class SubarrayDescription:
     """
     Collects the `TelescopeDescription` of all telescopes along with their
     positions on the ground.
 
@@ -215,14 +219,15 @@
                     name=tel_names,
                     type=tel_types,
                     num_mirrors=num_mirrors,
                     camera_type=cam_types,
                     tel_description=descs,
                 )
             )
+            tab.meta["TAB_VER"] = "1.0"
 
         elif kind == "optics":
             unique_types = set(self.tels.values())
 
             mirror_area = u.Quantity(
                 [t.optics.mirror_area.to_value(u.m ** 2) for t in unique_types],
                 u.m ** 2,
@@ -237,14 +242,15 @@
                 "type": [t.type for t in unique_types],
                 "mirror_area": mirror_area,
                 "num_mirrors": [t.optics.num_mirrors for t in unique_types],
                 "num_mirror_tiles": [t.optics.num_mirror_tiles for t in unique_types],
                 "equivalent_focal_length": focal_length,
             }
             tab = Table(cols)
+            tab.meta["TAB_VER"] = "2.0"
 
         else:
             raise ValueError(f"Table type '{kind}' not known")
 
         tab.meta.update(meta)
         return tab
 
@@ -331,7 +337,142 @@
         """
         if isinstance(tel_type, TelescopeDescription):
             tel_str = str(tel_type)
         else:
             tel_str = tel_type
 
         return [id for id, descr in self.tels.items() if str(descr) == tel_str]
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+
+        if self.name != other.name:
+            return False
+
+        if self.tels.keys() != other.tels.keys():
+            return False
+
+        if self.positions.keys() != other.positions.keys():
+            return False
+
+        for tel_id in self.tels.keys():
+            if self.tels[tel_id] != other.tels[tel_id]:
+                return False
+
+        for tel_id in self.tels.keys():
+            if np.any(self.positions[tel_id] != other.positions[tel_id]):
+                return False
+        return True
+
+    def to_hdf(self, output_path, overwrite=False):
+        """write the SubarrayDescription
+
+        Parameters
+        ----------
+        subarray : ctapipe.instrument.SubarrayDescription
+            subarray description
+        """
+        serialize_meta = True
+
+        if Path(output_path).suffix not in (".h5", ".hdf", ".hdf5"):
+            raise ValueError("This function can only write to hdf files.")
+
+        self.to_table().write(
+            output_path,
+            path="/configuration/instrument/subarray/layout",
+            serialize_meta=serialize_meta,
+            append=True,
+            overwrite=overwrite,
+        )
+        self.to_table(kind="optics").write(
+            output_path,
+            path="/configuration/instrument/telescope/optics",
+            append=True,
+            serialize_meta=serialize_meta,
+            overwrite=overwrite,
+        )
+        for camera in self.camera_types:
+            camera.geometry.to_table().write(
+                output_path,
+                path=f"/configuration/instrument/telescope/camera/geometry_{camera}",
+                append=True,
+                serialize_meta=serialize_meta,
+                overwrite=overwrite,
+            )
+            camera.readout.to_table().write(
+                output_path,
+                path=f"/configuration/instrument/telescope/camera/readout_{camera}",
+                append=True,
+                serialize_meta=serialize_meta,
+                overwrite=overwrite,
+            )
+
+        with tables.open_file(output_path, mode="r+") as f:
+            f.root.configuration.instrument.subarray._v_attrs.name = self.name
+
+    @classmethod
+    def from_hdf(cls, path):
+        layout = Table.read(path, path="/configuration/instrument/subarray/layout")
+
+        optics_table = Table.read(
+            path, path="/configuration/instrument/telescope/optics"
+        )
+
+        cameras = {}
+        for name in set(layout["camera_type"]):
+            geometry = CameraGeometry.from_table(
+                Table.read(
+                    path,
+                    path=f"/configuration/instrument/telescope/camera/geometry_{name}",
+                )
+            )
+            readout = CameraReadout.from_table(
+                Table.read(
+                    path,
+                    path=f"/configuration/instrument/telescope/camera/readout_{name}",
+                )
+            )
+            cameras[name] = CameraDescription(
+                camera_name=name, readout=readout, geometry=geometry
+            )
+
+        # iterating over the rows of a table does not play well
+        # with units, convert to dict of quantity arrays
+        optics_quantities = {
+            name: optics_table[name].quantity
+            if optics_table[name].unit
+            else optics_table[name]
+            for name in optics_table.colnames
+            if name not in {"description", "type"}
+        }
+        optics = {}
+        for row, desc in enumerate(optics_table["description"]):
+            kwargs = {k: v[row] for k, v in optics_quantities.items()}
+            optics[desc] = OpticsDescription(**kwargs)
+
+        telescope_descriptions = {
+            row["tel_id"]: TelescopeDescription(
+                name=row["name"],
+                tel_type=row["type"],
+                optics=optics[row["tel_description"]],
+                camera=cameras[row["camera_type"]],
+            )
+            for row in layout
+        }
+
+        positions = np.column_stack([layout[f"pos_{c}"].quantity for c in "xyz"])
+
+        with tables.open_file(path, mode="r") as f:
+            attrs = f.root.configuration.instrument.subarray._v_attrs
+            if "name" in attrs:
+                name = str(attrs.name)
+            else:
+                name = "Unknown"
+
+        return cls(
+            name=name,
+            tel_positions={
+                tel_id: pos for tel_id, pos in zip(layout["tel_id"], positions)
+            },
+            tel_descriptions=telescope_descriptions,
+        )
```

### Comparing `ctapipe-0.8.0/ctapipe/instrument/telescope.py` & `ctapipe-0.9.1/ctapipe/instrument/telescope.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/instrument/tests/test_guessing.py` & `ctapipe-0.9.1/ctapipe/instrument/tests/test_guessing.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/instrument/tests/test_telescope.py` & `ctapipe-0.9.1/ctapipe/instrument/tests/test_telescope.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/io/__init__.py` & `ctapipe-0.9.1/ctapipe/io/__init__.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/io/array.py` & `ctapipe-0.9.1/ctapipe/io/array.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/io/eventseeker.py` & `ctapipe-0.9.1/ctapipe/io/eventsource.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,281 +1,337 @@
 """
-Handles seeking to a particular event in a
-`ctapipe.io.eventfilereader.EventFileReader`
+Handles reading of different event/waveform containing files
 """
-from copy import deepcopy
-from ctapipe.core import Component
+from abc import abstractmethod
+from traitlets.config.loader import LazyConfigValue
 
-__all__ = [
-    "EventSeeker",
-]
+from ctapipe.core import Component, non_abstract_children, ToolConfigurationError
+from ctapipe.core import Provenance
+from ctapipe.core.plugins import detect_and_import_io_plugins
+from ctapipe.core.traits import Path, Int, Set
 
+__all__ = ["EventSource", "event_source"]
 
-class EventSeeker(Component):
+
+def event_source(input_url, **kwargs):
+    """
+    Helper function for EventSource.from_url
+
+    Find compatible EventSource for input_url via the `is_compatible` method
+    of the EventSource
+
+    Parameters
+    ----------
+    input_url : str
+        Filename or URL pointing to an event file
+    kwargs
+        Named arguments for the EventSource
+
+    Returns
+    -------
+    instance
+        Instance of a compatible EventSource subclass
     """
-    Provides the functionality to seek through a
-    `ctapipe.io.eventfilereader.EventSource` to find a particular event.
+    return EventSource.from_url(input_url, **kwargs)
+
+
+class EventSource(Component):
+    """
+    Parent class for EventFileReaders of different sources.
+
+    A new EventFileReader should be created for each type of event file read
+    into ctapipe, e.g. sim_telarray files are read by the `SimTelEventSource`.
+
+    EventFileReader provides a common high-level interface for accessing event
+    information from different data sources (simulation or different camera
+    file formats). Creating an EventFileReader for a new
+    file format ensures that data can be accessed in a common way,
+    irregardless of the file format.
+
+    EventFileReader itself is an abstract class. To use an EventFileReader you
+    must use a subclass that is relevant for the file format you
+    are reading (for example you must use
+    `ctapipe.io.SimTelEventSource` to read a hessio format
+    file). Alternatively you can use `event_source()` to automatically
+    select the correct EventFileReader subclass for the file format you wish
+    to read.
+
+    To create an instance of an EventFileReader you must pass the traitlet
+    configuration (containing the input_url) and the
+    `ctapipe.core.tool.Tool`. Therefore from inside a Tool you would do:
+
+    >>> event_source = EventSource(self.config, self)
+
+    An example of how to use `ctapipe.core.tool.Tool` and `event_source()`
+    can be found in ctapipe/tools/display_dl1.py.
+
+    However if you are not inside a Tool, you can still create an instance and
+    supply an input_url via:
+
+    >>> event_source = EventSource( input_url="/path/to/file")
+
+    To loop through the events in a file:
+
+    >>> event_source = EventSource( input_url="/path/to/file")
+    >>> for event in event_source:
+    >>>    print(event.count)
+
+    **NOTE**: Every time a new loop is started through the event_source, it restarts
+    from the first event.
+
+    Alternatively one can use EventFileReader in a `with` statement to ensure
+    the correct cleanups are performed when you are finished with the event_source:
+
+    >>> with EventSource( input_url="/path/to/file") as event_source:
+    >>>    for event in event_source:
+    >>>       print(event.count)
+
+    **NOTE**: The "event" that is returned from the generator is a pointer.
+    Any operation that progresses that instance of the generator further will
+    change the data pointed to by "event". If you wish to ensure a particular
+    event is kept, you should perform a `event_copy = copy.deepcopy(event)`.
 
-    By default, this will loop through events from the start of the file
-    (unless the requested event is the same as the previous requested event,
-    or occurs later in the file). However if the
-    `ctapipe.io.eventfilereader.EventSource` has defined a `__getitem__`
-    method itself, then it will use that method, thereby taking advantage of
-    the random event access some file formats provide.
-
-    To create an instance of an EventSeeker you must provide it a sub-class of
-    `ctapipe.io.eventfilereader.EventSource` (such as
-    `ctapipe.io.hessiofilereader.HessioFileReader`), which will be used to
-    loop through the file and provide the event container, filled with the
-    event information using the methods defined in the event_source for that
-    file format.
-
-    To obtain a particular event in a hessio file:
-
-    >>> from ctapipe.io.hessioeventsource import SimTelEventSource
-    >>> event_source = SimTelEventSource(input_url="/path/to/file")
-    >>> seeker = EventSeeker(event_source=event_source)
-    >>> event = seeker[2]
-    >>> print(event.count)
-
-    To obtain a particular event in a hessio file from its event_id:
-
-    >>> from ctapipe.io.hessioeventsource import SimTelEventSource
-    >>> event_source = SimTelEventSource(input_url="/path/to/file")
-    >>> seeker = EventSeeker(event_source=event_source)
-    >>> event = seeker["101"]
-    >>> print(event.count)
-
-    **NOTE**: Event_index refers to the number associated to the event
-    assigned by ctapipe (`event.count`), based on the order the events are
-    read from the file.
-    Whereas the event_id refers to the ID attatched to the event from the
-    external source of the file (software or camera or CTA array).
-
-    To obtain a slice of events in a hessio file:
-
-    >>> from ctapipe.io import SimTelEventSource
-    >>> event_source = SimTelEventSource(input_url="/path/to/file")
-    >>> seeker = EventSeeker(event_source=event_source)
-    >>> event_list = seeker[3:6]
-    >>> print([event.count for event in event_list])
-
-    To obtain a list of events in a hessio file:
-
-    >>> from ctapipe.io import SimTelEventSource
-    >>> event_source = SimTelEventSource(input_url="/path/to/file")
-    >>> seeker = EventSeeker(event_source)
-    >>> event_indicis = [2, 6, 8]
-    >>> event_list = seeker[event_indicis]
-    >>> print([event.count for event in event_list])
+
+    Attributes
+    ----------
+    input_url : str
+        Path to the input event file.
+    max_events : int
+        Maximum number of events to loop through in generator
     """
 
-    def __init__(self, reader, config=None, parent=None, **kwargs):
+    input_url = Path(
+        directory_ok=False,
+        exists=True,
+        help="Path to the input file containing events.",
+    ).tag(config=True)
+
+    max_events = Int(
+        None,
+        allow_none=True,
+        help="Maximum number of events that will be read from the file",
+    ).tag(config=True)
+
+    allowed_tels = Set(
+        default_value=None,
+        allow_none=True,
+        help=(
+            "list of allowed tel_ids, others will be ignored. "
+            "If None, all telescopes in the input stream "
+            "will be included"
+        ),
+    ).tag(config=True)
+
+    def __init__(self, input_url=None, config=None, parent=None, **kwargs):
         """
         Class to handle generic input files. Enables obtaining the "source"
         generator, regardless of the type of file (either hessio or camera
         file).
 
         Parameters
         ----------
-        reader : `ctapipe.io.eventfilereader.EventSource`
-            A subclass of `ctapipe.io.eventfilereader.EventFileReader` that
-            defines how the event container is filled for a particular file
-            format
         config : traitlets.loader.Config
             Configuration specified by config file or cmdline arguments.
             Used to set traitlet values.
             Set to None if no configuration to pass.
         tool : ctapipe.core.Tool
             Tool executable that is calling this component.
             Passes the correct logger to the component.
             Set to None if no Tool to pass.
         kwargs
         """
-        super().__init__(config=config, parent=parent, **kwargs)
+        super().__init__(config=config, parent=parent, input_url=input_url, **kwargs)
 
-        if reader.is_stream:
-            raise IOError(
-                "Reader is not compatible as input to the "
-                "event_source is a stream (seeking not possible)"
-            )
+        self.metadata = dict(is_simulation=False)
+        self.log.info(f"INPUT PATH = {self.input_url}")
 
-        self._reader = reader
+        if self.max_events:
+            self.log.info(f"Max events being read = {self.max_events}")
 
-        self._num_events = None
-        self._source = self._reader.__iter__()
-        self._current_event = None
-        self._has_fast_seek = False  # By default seeking iterates through
-        self._getevent_warn = True
+        Provenance().add_input_file(str(self.input_url), role="DL0/Event")
 
-    def _reset(self):
+    @staticmethod
+    @abstractmethod
+    def is_compatible(file_path):
         """
-        Recreate the generator so it starts from the beginning
+        Abstract method to be defined in child class.
+
+        Perform a set of checks to see if the input file is compatible
+        with this file event_source.
+
+        Parameters
+        ----------
+        file_path : str
+            File path to the event file.
+
+        Returns
+        -------
+        compatible : bool
+            True if file is compatible, False if it is incompatible
         """
-        self._source = self._reader.__iter__()
-        self._current_event = None
 
-    def __iter__(self):
-        # Always reset generator when starting a new iteration
-        self._reset()
-        for event in self._source:
-            self._current_event = event
-            yield event
+    @property
+    def is_stream(self):
+        """
+        Bool indicating if input is a stream. If it is then it is incompatible
+        with `ctapipe.io.eventseeker.EventSeeker`.
+
+        TODO: Define a method to detect if it is a stream
 
-    def __getitem__(self, item):
+        Returns
+        -------
+        bool
+            If True, then input is a stream.
         """
-        Obtain a particular event
+        return False
 
-        Parameters
-        ----------
-        item : int or str
-            If `item` is an int, then this is the event_index for the event
-            obtained. If `item` is a str, then this is the event_id for the
-            event obtained.
+    @property
+    @abstractmethod
+    def subarray(self):
+        """
+        Obtain the subarray from the EventSource
 
         Returns
         -------
-        event : ctapipe.io.container
-            The event container filled with the requested event's information
+        ctapipe.instrument.SubarrayDecription
 
         """
 
-        # Handling of different input types (int, string, slice, list)
-        current = None
-        use_event_id = False
-        if isinstance(item, int):
-            if self._current_event:
-                current = self._current_event.count
-            if item < 0:
-                item = len(self) + item
-                if item < 0 or item >= len(self):
-                    msg = "Event index {} out of range [0, {}]".format(item, len(self))
-                    raise IndexError(msg)
-        elif isinstance(item, str):
-            item = int(item)
-            use_event_id = True
-            if self._current_event:
-                current = self._current_event.index.event_id
-        elif isinstance(item, slice):
-            it = range(item.start or 0, item.stop or len(self), item.step or 1)
-            events = [self[i] for i in it]
-            return events
-        elif isinstance(item, list):
-            events = [self[i] for i in item]
-            return events
-        else:
-            raise TypeError("{} indexing is not supported".format(type(item)))
-
-        # Return a copy of the current event if we have already reached it
-        if current is not None and item == current:
-            return deepcopy(self._current_event)
-
-        # If requested event is less than the current event position: reset
-        if current is not None and item < current:
-            self._reset()
-
-        # Check we are within max_events range
-        max_events = self._reader.max_events
-        if not use_event_id and max_events and item >= max_events:
-            msg = "Event index {} outside of specified max_events {}".format(
-                item, max_events
-            )
-            raise IndexError(msg)
-
-        try:
-            if not use_event_id:
-                event = self._reader._get_event_by_index(item)
-            else:
-                event = self._reader._get_event_by_id(item)
-        except AttributeError:
-            if self._getevent_warn:
-                self.log.warning(
-                    "Seeking to event by looping through "
-                    "events... (potentially long process)"
-                )
-                self._getevent_warn = False
-            if not use_event_id:
-                event = self._get_event_by_index(item)
-            else:
-                event = self._get_event_by_id(item)
-
-        self._current_event = event
-        return deepcopy(event)
-
-    def _get_event_by_index(self, index):
-        """
-        Method for extracting a particular event by looping through events
-        until it finds the requested event index.
-        If a file format allows random event access, then is can define its
-        own `get_event_by_index` method in its
-        `ctapipe.io.eventfilereader.EventSource` to allow this class to
-        utilise that method instead.
+    @property
+    @abstractmethod
+    def is_simulation(self):
+        """
+        Weither the currently opened file is simulated
 
-        Parameters
-        ----------
-        index : int
-            The event_index to seek.
+        Returns
+        -------
+        bool
+
+        """
+
+    @property
+    @abstractmethod
+    def datalevels(self):
+        """
+        The datalevels provided by this event source
+
+        Returns
+        -------
+        tuple[ctapipe.io.DataLevel]
+        """
+
+    @property
+    @abstractmethod
+    def obs_id(self):
+        """
+        The current observation id
+
+        Returns
+        -------
+        int
+        """
+
+    @abstractmethod
+    def _generator(self):
+        """
+        Abstract method to be defined in child class.
+
+        Generator where the filling of the `ctapipe.containers` occurs.
+
+        Returns
+        -------
+        generator
+        """
+
+    def __iter__(self):
+        """
+        Generator that iterates through `_generator`, but keeps track of
+        `self.max_events`.
 
         Returns
         -------
-        event : ctapipe.io.container
-            The event container filled with the requested event's information
+        generator
+        """
+        for event in self._generator():
+            yield event
+            if self.max_events and event.count >= self.max_events - 1:
+                break
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
 
+    @classmethod
+    def from_url(cls, input_url, **kwargs):
         """
-        for event in self._source:
-            if event.count == index:
-                return event
-        raise IndexError(f"Event index {index} not found in file")
-
-    def _get_event_by_id(self, event_id):
-        """
-        Method for extracting a particular event by looping through events
-        until it finds the requested event id.
-        If a file format allows random event access, then is can define its
-        own `get_event_by_id` method in its
-        `ctapipe.io.eventfilereader.EventSource` to allow this class to
-        utilise that method instead.
+        Find compatible EventSource for input_url via the `is_compatible`
+        method of the EventSource
 
         Parameters
         ----------
-        event_id : int
-            The event_id to seek.
+        input_url : str
+            Filename or URL pointing to an event file
+        kwargs
+            Named arguments for the EventSource
 
         Returns
         -------
-        event : ctapipe.io.container
-            The event container filled with the requested event's information
+        instance
+            Instance of a compatible EventSource subclass
+        """
+        if input_url == "" or input_url is None:
+            raise ToolConfigurationError("EventSource: No input_url was specified")
 
+        # validate input url with the traitel validate method
+        # to make sure it's compatible and to raise the correct error
+        input_url = EventSource.input_url.validate(obj=None, value=input_url)
+
+        detect_and_import_io_plugins()
+        available_classes = non_abstract_children(cls)
+
+        for subcls in available_classes:
+            if subcls.is_compatible(input_url):
+                return subcls(input_url=input_url, **kwargs)
+
+        raise ValueError(
+            "Cannot find compatible EventSource for \n"
+            "\turl:{}\n"
+            "in available EventSources:\n"
+            "\t{}".format(input_url, [c.__name__ for c in available_classes])
+        )
+
+    @classmethod
+    def from_config(cls, config=None, parent=None, **kwargs):
         """
-        for event in self:  # Event Ids may not be in order
-            if event.index.event_id == event_id:
-                return event
-        raise IndexError(f"Event id {event_id} not found in file")
-
-    def __len__(self):
-        """
-        Method for getting number of events in file. By default this is
-        obtained by looping through the file and counting the events. If a
-        file format has a more efficient method of supplying this information,
-        the `ctapipe.io.eventfilereader.EventSource` for that file format
-        can define its own `__len__` method, which this class will then
-        use instead.
+        Find compatible EventSource for the EventSource.input_url traitlet
+        specified via the config.
+
+        This method is typically used in Tools, where the input_url is chosen via
+        the command line using the traitlet configuration system.
+
+        Parameters
+        ----------
+        config : traitlets.config.loader.Config
+            Configuration created in the Tool
+        kwargs
+            Named arguments for the EventSource
 
         Returns
         -------
-        self._num_events : int
-            Number of events in the file
+        instance
+            Instance of a compatible EventSource subclass
         """
-        # Only need to calculate once
-        if not self._num_events:
-            try:
-                count = len(self._reader)
-            except TypeError:
-                self.log.warning(
-                    "Obtaining length of file by looping through "
-                    "all events... (potentially long process)"
-                )
-                count = 0
-                for _ in self:
-                    count += 1
-            self._num_events = count
-        return self._num_events
+        if config is None and parent is None:
+            raise ValueError("One of config or parent must be provided")
+
+        if config is not None and parent is not None:
+            raise ValueError("Only one of config or parent must be provided")
+
+        if config is None:
+            config = parent.config
+
+        if isinstance(config.EventSource.input_url, LazyConfigValue):
+            config.EventSource.input_url = cls.input_url.default_value
+
+        return event_source(config.EventSource.input_url, config=config, **kwargs)
```

### Comparing `ctapipe-0.8.0/ctapipe/io/files.py` & `ctapipe-0.9.1/ctapipe/io/files.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/io/hdf5tableio.py` & `ctapipe-0.9.1/ctapipe/io/hdf5tableio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Implementations of TableWriter and -Reader for HDF5 files"""
 import enum
 from functools import partial
 from pathlib import PurePath
+import re
 
 import numpy as np
 import tables
 from astropy.time import Time
 from astropy.units import Quantity
 
 import ctapipe
@@ -153,24 +154,32 @@
 
             for col_name, value in container.items(add_prefix=self.add_prefix):
 
                 typename = ""
                 shape = 1
 
                 if self._is_column_excluded(table_name, col_name):
-                    self.log.debug("excluded column: %s/%s", table_name, col_name)
+                    self.log.debug(f"excluded column: {table_name}/{col_name}")
                     continue
 
                 if col_name in Schema.columns:
                     self.log.warning(f"Found duplicated column {col_name}, skipping")
                     continue
 
                 # apply any user-defined transforms first
                 value = self._apply_col_transform(table_name, col_name, value)
 
+                # add desription to metadata
+                if self.add_prefix:
+                    meta[f"{col_name}_DESC"] = container.fields[
+                        re.sub(f"^{container.prefix}_", "", col_name)
+                    ].description
+                else:
+                    meta[f"{col_name}_DESC"] = container.fields[col_name].description
+
                 if isinstance(value, enum.Enum):
 
                     def transform(enum_value):
                         """transform enum instance into its (integer) value"""
                         return enum_value.value
 
                     meta[f"{col_name}_ENUM"] = value.__class__
@@ -204,28 +213,25 @@
                 elif type(value).__name__ in PYTABLES_TYPE_MAP:
                     typename = type(value).__name__
                     coltype = PYTABLES_TYPE_MAP[typename]
                     Schema.columns[col_name] = coltype(pos=pos)
 
                 else:
                     self.log.warning(
-                        f"Column {col_name} of"
-                        f" container {container.__class__.__name__}"
-                        f" in table {table_name}"
-                        " not writable, skipping"
+                        f"Column {col_name} of "
+                        f"container {container.__class__.__name__} in "
+                        f"table {table_name} not writable, skipping"
                     )
                     continue
 
                 pos += 1
                 self.log.debug(
-                    "Table %s: added col: %s type: %s shape: %s",
-                    table_name,
-                    col_name,
-                    typename,
-                    shape,
+                    f"Table {table_name}: "
+                    f"added col: {col_name} type: "
+                    f"{typename} shape: {shape}"
                 )
 
         self._schemas[table_name] = Schema
         meta["CTAPIPE_VERSION"] = ctapipe.__version__
         return meta
 
     def _setup_new_table(self, table_name, containers):
@@ -250,15 +256,15 @@
             title="Storage of {}".format(
                 ",".join(c.__class__.__name__ for c in containers)
             ),
             description=self._schemas[table_name],
             createparents=True,
             filters=self.filters,
         )
-        self.log.debug("CREATED TABLE: %s", table)
+        self.log.debug(f"CREATED TABLE: {table}")
         for key, val in meta.items():
             table.attrs[key] = val
 
         self._tables[table_name] = table
 
     def _append_row(self, table_name, containers):
         """
@@ -276,16 +282,16 @@
             for colname, value in selected_fields:
 
                 try:
                     value = self._apply_col_transform(table_name, colname, value)
                     row[colname] = value
                 except Exception:
                     self.log.error(
-                        f'Error writing col "{colname}" of'
-                        f' container "{container.__class__.__name__}"'
+                        f"Error writing col {colname} of "
+                        f"container {container.__class__.__name__}"
                     )
                     raise
         row.append()
 
     def write(self, table_name, containers):
         """
         Write the contents of the given container or containers to a table.
@@ -329,18 +335,14 @@
     event at a time* into a container, which is not very I/O efficient. For
     some other use cases, it may be much more efficient to access the
     table data directly, for example to read an entire column or table at
     once (which means not using the Container data structure).
 
     Todo:
     - add ability to synchronize reading of multiple tables on a key
-
-    - add ability (also with TableWriter) to read a row into n containers at
-        once, assuming no naming conflicts (so we can add e.g. event_id)
-
     """
 
     def __init__(self, filename, **kwargs):
         """
         Parameters
         ----------
         filename: str
@@ -360,18 +362,18 @@
 
         self._h5file = tables.open_file(filename, **kwargs)
 
     def close(self):
 
         self._h5file.close()
 
-    def _setup_table(self, table_name, container):
+    def _setup_table(self, table_name, containers, prefixes):
         tab = self._h5file.get_node(table_name)
         self._tables[table_name] = tab
-        self._map_table_to_container(table_name, container)
+        self._map_table_to_containers(table_name, containers, prefixes)
         self._map_transforms_from_table_header(table_name)
         return tab
 
     def _map_transforms_from_table_header(self, table_name):
         """
         create any transforms needed to "undo" ones in the writer
         """
@@ -389,79 +391,112 @@
                 def transform_int_to_enum(int_val):
                     """transform integer 'code' into enum instance"""
                     enum_class = tab.attrs[attr]
                     return enum_class(int_val)
 
                 self.add_column_transform(table_name, colname, transform_int_to_enum)
 
-    def _map_table_to_container(self, table_name, container):
-        """ identifies which columns in the table to read into the container,
-        by comparing their names."""
+    def _map_table_to_containers(self, table_name, containers, prefixes):
+        """ identifies which columns in the table to read into the containers,
+        by comparing their names including an optional prefix."""
         tab = self._tables[table_name]
-        for colname in tab.colnames:
-            if colname in container.fields:
-                self._cols_to_read[table_name].append(colname)
-            else:
-                self.log.warning(
-                    "Table '%s' has column '%s' that is not in "
-                    "container %s. It will be skipped",
-                    table_name,
-                    colname,
-                    container.__class__.__name__,
-                )
+        self._cols_to_read[table_name] = []
+        for container, prefix in zip(containers, prefixes):
+            for colname in tab.colnames:
+                if prefix and colname.startswith(prefix):
+                    colname_without_prefix = colname[len(prefix) + 1 :]
+                else:
+                    colname_without_prefix = colname
+                if colname_without_prefix in container.fields:
+                    self._cols_to_read[table_name].append(colname)
+                else:
+                    self.log.warning(
+                        f"Table {table_name} has column {colname_without_prefix} that is not in "
+                        f"container {container.__class__.__name__}. It will be skipped."
+                    )
 
-        # also check that the container doesn't have fields that are not
-        # in the table:
-        for colname in container.fields:
-            if colname not in self._cols_to_read[table_name]:
-                self.log.warning(
-                    "Table '%s' is missing column '%s' that is "
-                    "in container %s. It will be skipped.",
-                    table_name,
-                    colname,
-                    container.__class__.__name__,
-                )
+            # also check that the container doesn't have fields that are not
+            # in the table:
+            for colname in container.fields:
+                if prefix:
+                    colname_with_prefix = f"{prefix}_{colname}"
+                else:
+                    colname_with_prefix = colname
+                if colname_with_prefix not in self._cols_to_read[table_name]:
+                    self.log.warning(
+                        f"Table {table_name} is missing column {colname_with_prefix}"
+                        f"that is in container {container.__class__.__name__}. It will be skipped."
+                    )
 
-        # copy all user-defined attributes back to Container.mets
-        for key in tab.attrs._f_list():
-            container.meta[key] = tab.attrs[key]
+            # copy all user-defined attributes back to Container.mets
+            for key in tab.attrs._f_list():
+                container.meta[key] = tab.attrs[key]
 
-    def read(self, table_name: str, container: Container):
+    def read(self, table_name, containers, prefixes=False):
         """
         Returns a generator that reads the next row from the table into the
-        given container.  The generator returns the same container. Note that
+        given container. The generator returns the same container. Note that
         no containers are copied, the data are overwritten inside.
 
         Parameters
         ----------
         table_name: str
             name of table to read from
         container : ctapipe.core.Container
             Container instance to fill
+        prefix: bool, str or list
+            Prefix that was added while writing the file.
+            If True, the container prefix is taken into consideration, when
+            comparing column names and container fields.
+            If False, no prefix is used.
+            If a string is provided, it is used as prefix for all containers.
+            If a list is provided, the length needs to match th number
+            of containers.
         """
+
+        return_iterable = True
+        if isinstance(containers, Container):
+            containers = (containers,)
+            return_iterable = False
+
+        if prefixes is False:
+            prefixes = ["" for container in containers]
+        elif prefixes is True:
+            prefixes = [container.prefix for container in containers]
+        elif isinstance(prefixes, str):
+            prefixes = [prefixes for container in containers]
+        assert len(prefixes) == len(containers)
+
         if table_name not in self._tables:
-            tab = self._setup_table(table_name, container)
+            tab = self._setup_table(table_name, containers, prefixes)
         else:
             tab = self._tables[table_name]
 
         row_count = 0
 
         while 1:
-
             try:
                 row = tab[row_count]
             except IndexError:
                 return  # stop generator when done
-
-            for colname in self._cols_to_read[table_name]:
-                container[colname] = self._apply_col_transform(
-                    table_name, colname, row[colname]
-                )
-
-            yield container
+            for container, prefix in zip(containers, prefixes):
+                for fieldname in container.keys():
+                    if prefix:
+                        colname = f"{prefix}_{fieldname}"
+                    else:
+                        colname = fieldname
+                    if colname not in self._cols_to_read[table_name]:
+                        continue
+                    container[fieldname] = self._apply_col_transform(
+                        table_name, colname, row[colname]
+                    )
+            if return_iterable:
+                yield containers
+            else:
+                yield containers[0]
             row_count += 1
 
 
 def tr_convert_and_strip_unit(quantity, unit):
     return quantity.to_value(unit)
```

### Comparing `ctapipe-0.8.0/ctapipe/io/metadata.py` & `ctapipe-0.9.1/ctapipe/io/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,15 @@
     some_astropy_table.write("output.ecsv")
 
 """
 import uuid
 import warnings
 from collections import OrderedDict
 
-from traitlets import (
-    Enum,
-    Unicode,
-    Int,
-    HasTraits,
-    default,
-    Instance,
-)
+from traitlets import Enum, Unicode, Int, HasTraits, default, Instance
 
 from ctapipe.core.provenance import _ActivityProvenance
 from ctapipe.core.traits import AstroTime
 
 __all__ = [
     "Reference",
     "Contact",
@@ -47,14 +40,17 @@
     "Instrument",
     "write_to_hdf5",
 ]
 
 from astropy.time import Time
 
 
+CONVERSIONS = {Time: lambda t: t.utc.iso}
+
+
 class Contact(HasTraits):
     """ Contact information """
 
     name = Unicode("unknown")
     email = Unicode("unknown")
     organization = Unicode("unknown")
 
@@ -165,40 +161,51 @@
     id_ = Unicode("unspecified")
 
 
 def _to_dict(hastraits_instance, prefix=""):
     """ helper to convert a HasTraits to a dict with keys
     in the required CTA format (upper-case, space separated)
     """
-    return {
-        (prefix + k.upper().replace("_", " "))
-        .replace("  ", " ")
-        .strip(): tr.get(hastraits_instance)
-        for k, tr in hastraits_instance.traits().items()
-    }
+    res = {}
+
+    for k, tr in hastraits_instance.traits().items():
+        key = (prefix + k.upper().replace("_", " ")).replace("  ", " ").strip()
+        val = tr.get(hastraits_instance)
+
+        # apply type conversions
+        val = CONVERSIONS.get(type(val), lambda v: v)(val)
+        res[key] = val
+
+    return res
 
 
 class Reference(HasTraits):
     """ All the reference Metadata required for a CTA output file, plus a way to turn
     it into a dict() for easy addition to the header of a file """
 
     contact = Instance(Contact)
     product = Instance(Product)
     process = Instance(Process)
     activity = Instance(Activity)
     instrument = Instance(Instrument)
 
-    def to_dict(self):
-        """ convert Reference metadata to a flat dict"""
-        meta = OrderedDict({"CTA REFERENCE VERSION": "1"})
-        meta.update(_to_dict(self.contact, prefix="CTA CONTACT "))
-        meta.update(_to_dict(self.product, prefix="CTA PRODUCT "))
-        meta.update(_to_dict(self.process, prefix="CTA PROCESS "))
-        meta.update(_to_dict(self.activity, prefix="CTA ACTIVITY "))
-        meta.update(_to_dict(self.instrument, prefix="CTA INSTRUMENT "))
+    def to_dict(self, fits=False):
+        """
+        convert Reference metadata to a flat dict.
+
+        If `fits=True`, this will include the `HIERARCH` keyword in front.
+        """
+        prefix = "CTA " if fits is False else "HIERARCH CTA "
+
+        meta = OrderedDict({prefix + "REFERENCE VERSION": "1"})
+        meta.update(_to_dict(self.contact, prefix=prefix + "CONTACT "))
+        meta.update(_to_dict(self.product, prefix=prefix + "PRODUCT "))
+        meta.update(_to_dict(self.process, prefix=prefix + "PROCESS "))
+        meta.update(_to_dict(self.activity, prefix=prefix + "ACTIVITY "))
+        meta.update(_to_dict(self.instrument, prefix=prefix + "INSTRUMENT "))
         return meta
 
 
 def write_to_hdf5(metadata, h5file):
     """
     Write metadata fields to a PyTables HDF5 file handle.
```

### Comparing `ctapipe-0.8.0/ctapipe/io/simteleventsource.py` & `ctapipe-0.9.1/ctapipe/io/simteleventsource.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,31 @@
 from astropy.coordinates import Angle
 from astropy.time import Time
 from eventio.file_types import is_eventio
 from eventio.simtel.simtelfile import SimTelFile
 from traitlets import observe
 from io import BufferedReader
 
-from ..calib.camera.gainselection import ThresholdGainSelector
+from ..calib.camera.gainselection import GainSelector
 from ..containers import EventAndMonDataContainer, EventType
-from ..core.traits import Bool, CaselessStrEnum
+from ..core.traits import Bool, CaselessStrEnum, create_class_enum_trait
 from ..instrument import (
     TelescopeDescription,
     SubarrayDescription,
     CameraDescription,
     CameraGeometry,
     CameraReadout,
     OpticsDescription,
 )
 from ..instrument.camera import UnknownPixelShapeWarning
 from ..instrument.guess import guess_telescope, UNKNOWN_TELESCOPE
 from ..containers import MCHeaderContainer
 from .eventsource import EventSource
 from .datalevels import DataLevel
+from ..coordinates import CameraFrame
 
 X_MAX_UNIT = u.g / (u.cm ** 2)
 
 
 __all__ = ["SimTelEventSource"]
 
 # Mapping of SimTelArray Calibration trigger types to EventType:
@@ -49,15 +50,15 @@
         u.Quantity(simtel_time[0], u.s),
         u.Quantity(simtel_time[1], u.ns),
         format="unix",
         scale="utc",
     )
 
 
-def build_camera(cam_settings, pixel_settings, telescope):
+def build_camera(cam_settings, pixel_settings, telescope, frame):
     pixel_shape = cam_settings["pixel_shape"][0]
     try:
         pix_type, pix_rotation = CameraGeometry.simtel_shape_to_type(pixel_shape)
     except ValueError:
         warnings.warn(
             f"Unkown pixel_shape {pixel_shape} for camera_type {telescope.camera_name}",
             UnknownPixelShapeWarning,
@@ -71,20 +72,23 @@
         pix_x=u.Quantity(cam_settings["pixel_x"], u.m),
         pix_y=u.Quantity(cam_settings["pixel_y"], u.m),
         pix_area=u.Quantity(cam_settings["pixel_area"], u.m ** 2),
         pix_type=pix_type,
         pix_rotation=pix_rotation,
         cam_rotation=-Angle(cam_settings["cam_rot"], u.rad),
         apply_derotation=True,
+        frame=frame,
     )
     readout = CameraReadout(
         telescope.camera_name,
         sampling_rate=u.Quantity(1 / pixel_settings["time_slice"], u.GHz),
         reference_pulse_shape=pixel_settings["ref_shape"].astype("float64", copy=False),
-        reference_pulse_sample_width=u.Quantity(pixel_settings["ref_step"], u.ns),
+        reference_pulse_sample_width=u.Quantity(
+            pixel_settings["ref_step"], u.ns, dtype="float64"
+        ),
     )
 
     return CameraDescription(
         camera_name=telescope.camera_name, geometry=geometry, readout=readout
     )
 
 
@@ -156,17 +160,19 @@
             "SubarrayDescription (which will be used in CameraFrame to TelescopeFrame "
             "coordinate transforms. The 'nominal' focal length is the one used during "
             "the simulation, the 'effective' focal length is computed using specialized "
             "ray-tracing from a point light source"
         ),
     ).tag(config=True)
 
-    def __init__(
-        self, input_url, config=None, parent=None, gain_selector=None, **kwargs
-    ):
+    gain_selector_type = create_class_enum_trait(
+        base_class=GainSelector, default_value="ThresholdGainSelector"
+    ).tag(config=True)
+
+    def __init__(self, input_url, config=None, parent=None, **kwargs):
         """
         EventSource for simtelarray files using the pyeventio library.
 
         Parameters
         ----------
         config : traitlets.loader.Config
             Configuration specified by config file or cmdline arguments.
@@ -194,20 +200,18 @@
 
         self._subarray_info = self.prepare_subarray_info(
             self.file_.telescope_descriptions, self.file_.header
         )
         self._mc_header = self._parse_mc_header()
         self.start_pos = self.file_.tell()
 
-        # Waveforms from simtelarray have both gain channels
-        # Gain selection is performed by this EventSource to produce R1 waveforms
-        if gain_selector is None:
-            gain_selector = ThresholdGainSelector(parent=self)
-
-        self.gain_selector = gain_selector
+        self.gain_selector = GainSelector.from_name(
+            self.gain_selector_type, parent=self
+        )
+        self.log.debug(f"Using gain selector {self.gain_selector}")
 
     @observe("allowed_tels")
     def _observe_allowed_tels(self, change):
         # this can run in __init__ before file_ is created
         if hasattr(self, "file_"):
             allowed_tels = set(self.allowed_tels) if self.allowed_tels else None
             self.file_.allowed_telescopes = allowed_tels
@@ -220,15 +224,15 @@
 
     @property
     def is_simulation(self):
         return True
 
     @property
     def datalevels(self):
-        return (DataLevel.R0, DataLevel.R1, DataLevel.DL0)
+        return (DataLevel.R0, DataLevel.R1)
 
     @property
     def obs_id(self):
         return self.file_.header["run"]
 
     @property
     def mc_header(self):
@@ -279,27 +283,32 @@
                     )
 
             try:
                 telescope = guess_telescope(n_pixels, focal_length)
             except ValueError:
                 telescope = UNKNOWN_TELESCOPE
 
-            camera = self._camera_cache.get(telescope.camera_name)
-            if camera is None:
-                camera = build_camera(cam_settings, pixel_settings, telescope)
-                self._camera_cache[telescope.camera_name] = camera
-
             optics = OpticsDescription(
                 name=telescope.name,
                 num_mirrors=telescope.n_mirrors,
                 equivalent_focal_length=focal_length,
                 mirror_area=u.Quantity(cam_settings["mirror_area"], u.m ** 2),
                 num_mirror_tiles=cam_settings["n_mirrors"],
             )
 
+            camera = self._camera_cache.get(telescope.camera_name)
+            if camera is None:
+                camera = build_camera(
+                    cam_settings,
+                    pixel_settings,
+                    telescope,
+                    frame=CameraFrame(focal_length=optics.equivalent_focal_length),
+                )
+                self._camera_cache[telescope.camera_name] = camera
+
             tel_descriptions[tel_id] = TelescopeDescription(
                 name=telescope.name,
                 tel_type=telescope.type,
                 optics=optics,
                 camera=camera,
             )
 
@@ -384,15 +393,15 @@
                 mc.true_image = (
                     array_event.get("photoelectrons", {})
                     .get(tel_id - 1, {})
                     .get("photoelectrons", np.zeros(n_pixels, dtype="float32"))
                 )
 
                 self._fill_event_pointing(
-                    data.pointing.tel[tel_id], mc, tracking_positions[tel_id],
+                    data.pointing.tel[tel_id], mc, tracking_positions[tel_id]
                 )
 
                 r0 = data.r0.tel[tel_id]
                 r1 = data.r1.tel[tel_id]
                 r0.waveform = adc_samples
                 r1.waveform, r1.selected_gain_channel = apply_simtel_r1_calibration(
                     adc_samples, mc.pedestal, mc.dc_to_pe, self.gain_selector
@@ -464,16 +473,16 @@
 
         return MCHeaderContainer(
             corsika_version=mc_run_head["shower_prog_vers"],
             simtel_version=mc_run_head["detector_prog_vers"],
             energy_range_min=mc_run_head["E_range"][0] * u.TeV,
             energy_range_max=mc_run_head["E_range"][1] * u.TeV,
             prod_site_B_total=mc_run_head["B_total"] * u.uT,
-            prod_site_B_declination=Angle(mc_run_head["B_declination"], u.rad,),
-            prod_site_B_inclination=Angle(mc_run_head["B_inclination"], u.rad,),
+            prod_site_B_declination=Angle(mc_run_head["B_declination"], u.rad),
+            prod_site_B_inclination=Angle(mc_run_head["B_inclination"], u.rad),
             prod_site_alt=mc_run_head["obsheight"] * u.m,
             spectral_index=mc_run_head["spectral_index"],
             shower_prog_start=mc_run_head["shower_prog_start"],
             shower_prog_id=mc_run_head["shower_prog_id"],
             detector_prog_start=mc_run_head["detector_prog_start"],
             detector_prog_id=mc_run_head["detector_prog_id"],
             num_showers=mc_run_head["n_showers"],
```

### Comparing `ctapipe-0.8.0/ctapipe/io/tableio.py` & `ctapipe-0.9.1/ctapipe/io/tableio.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from abc import ABCMeta, abstractmethod
 from collections import defaultdict
 
-from ctapipe.core import Component, Container
+from ctapipe.core import Component
 
 __all__ = ["TableReader", "TableWriter"]
 
 
 class TableWriter(Component, metaclass=ABCMeta):
     """
     Base class for writing  Container classes as rows of an output table,
@@ -43,15 +43,15 @@
             regular expression string to match column name
         """
         table_name = table_name.lstrip("/")
         self._exclusions[table_name].append(re.compile(pattern))
 
     def _is_column_excluded(self, table_name, col_name):
         for pattern in self._exclusions[table_name]:
-            if pattern.match(col_name):
+            if pattern.fullmatch(col_name):
                 return True
         return False
 
     def add_column_transform(self, table_name, col_name, transform):
         """
         Add a transformation function for a column. This function will be
         called on the value in the container before it is written to the
@@ -80,16 +80,16 @@
         The shape of data within the container must not change between calls,
         since variable-length arrays are not supported.
 
         Parameters
         ----------
         table_name: str
             name of table to write to
-        container: `ctapipe.core.Container`
-            container to write
+        containers: ctapipe.core.Container or iterable thereof
+            container instance(s) to write
         **kwargs:
             may be passed to a lower level implementation to set options
         """
         pass
 
     @abstractmethod
     def open(self, filename, **kwargs):
@@ -125,15 +125,15 @@
     full table at once are preferred to this method, since they are faster,
     but this can be used to re-play a table row by row into a
     `ctapipe.core.Container` class (the opposite of TableWriter)
     """
 
     def __init__(self):
         super().__init__()
-        self._cols_to_read = defaultdict(list)
+        self._cols_to_read = defaultdict(dict)
         self._transforms = defaultdict(dict)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
@@ -164,26 +164,28 @@
         """
         if col_name in self._transforms[table_name]:
             tr = self._transforms[table_name][col_name]
             value = tr(value)
         return value
 
     @abstractmethod
-    def read(self, table_name: str, container: Container):
+    def read(self, table_name, containers, prefixes, **kwargs):
         """
         Returns a generator that reads the next row from the table into the
         given container.  The generator returns the same container. Note that
         no containers are copied, the data are overwritten inside.
 
         Parameters
         ----------
         table_name: str
             name of table to read from
-        container : ctapipe.core.Container
-            Container instance to fill
+        containers: ctapipe.core.Container or iterable thereof
+            Container instance(s) to fill
+        prefixes: bool, str or iterable of str
+            prefixes used during writing of the table
         """
         pass
 
     @abstractmethod
     def open(self, filename, **kwargs):
         pass
```

### Comparing `ctapipe-0.8.0/ctapipe/io/tests/test_event_source.py` & `ctapipe-0.9.1/ctapipe/io/tests/test_event_source.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/io/tests/test_hdf5.py` & `ctapipe-0.9.1/ctapipe/io/tests/test_hdf5.py`

 * *Files 24% similar despite different names*

```diff
@@ -46,33 +46,205 @@
             mc.core_y = np.random.uniform(-1, 1) * u.m
 
             writer.write("tel_001", r0tel)
             writer.write("tel_002", r0tel)  # write a second table too
             writer.write("MC", mc)
 
 
-def test_prefix(tmp_path):
-    tmp_file = tmp_path / "test_prefix.hdf5"
+def test_read_multiple_containers():
     hillas_parameter_container = HillasParametersContainer(
         x=1 * u.m, y=1 * u.m, length=1 * u.m, width=1 * u.m
     )
 
     leakage_container = LeakageContainer(
         pixels_width_1=0.1,
         pixels_width_2=0.1,
         intensity_width_1=0.1,
         intensity_width_2=0.1,
     )
+    with tempfile.NamedTemporaryFile() as f:
+        with HDF5TableWriter(f.name, group_name="dl1", add_prefix=True) as writer:
+            writer.write("params", [hillas_parameter_container, leakage_container])
+
+        df = pd.read_hdf(f.name, key="/dl1/params")
+        assert "hillas_x" in df.columns
+        assert "leakage_pixels_width_1" in df.columns
+
+        # test reading both containers separately
+        with HDF5TableReader(f.name) as reader:
+            generator = reader.read(
+                "/dl1/params",
+                HillasParametersContainer(),
+                prefixes=True
+            )
+            hillas = next(generator)
+        for value, read_value in zip(
+            hillas_parameter_container.as_dict().values(),
+            hillas.as_dict().values()
+        ):
+            np.testing.assert_equal(value, read_value)
+
+        with HDF5TableReader(f.name) as reader:
+            generator = reader.read(
+                "/dl1/params",
+                LeakageContainer(),
+                prefixes=True
+            )
+            leakage = next(generator)
+        for value, read_value in zip(
+                leakage_container.as_dict().values(),
+                leakage.as_dict().values()
+        ):
+            np.testing.assert_equal(value, read_value)
+
+        # test reading both containers simultaneously
+        with HDF5TableReader(f.name) as reader:
+            generator = reader.read(
+                "/dl1/params",
+                [HillasParametersContainer(), LeakageContainer()],
+                prefixes=True,
+            )
+            hillas_, leakage_ = next(generator)
+
+        for value, read_value in zip(
+            leakage_container.as_dict().values(),
+            leakage_.as_dict().values()
+        ):
+            np.testing.assert_equal(value, read_value)
+
+        for value, read_value in zip(
+            hillas_parameter_container.as_dict().values(),
+            hillas_.as_dict().values()
+        ):
+            np.testing.assert_equal(value, read_value)
+
+
+def test_read_without_prefixes():
+    hillas_parameter_container = HillasParametersContainer(
+        x=1 * u.m, y=1 * u.m, length=1 * u.m, width=1 * u.m
+    )
+
+    leakage_container = LeakageContainer(
+        pixels_width_1=0.1,
+        pixels_width_2=0.1,
+        intensity_width_1=0.1,
+        intensity_width_2=0.1,
+    )
+    with tempfile.NamedTemporaryFile() as f:
+        with HDF5TableWriter(f.name, group_name="dl1", add_prefix=False) as writer:
+            writer.write("params", [hillas_parameter_container, leakage_container])
+
+        df = pd.read_hdf(f.name, key="/dl1/params")
+        assert "x" in df.columns
+        assert "pixels_width_1" in df.columns
+
+        # call with prefixes=False
+        with HDF5TableReader(f.name) as reader:
+            generator = reader.read(
+                "/dl1/params",
+                [HillasParametersContainer(), LeakageContainer()],
+                prefixes=False,
+            )
+            hillas_, leakage_ = next(generator)
+
+        for value, read_value in zip(
+            leakage_container.as_dict().values(),
+            leakage_.as_dict().values()
+        ):
+            np.testing.assert_equal(value, read_value)
+
+        for value, read_value in zip(
+            hillas_parameter_container.as_dict().values(),
+            hillas_.as_dict().values()
+        ):
+            np.testing.assert_equal(value, read_value)
 
-    with HDF5TableWriter(tmp_file.name, group_name="blabla", add_prefix=True) as writer:
-        writer.write("events", [hillas_parameter_container, leakage_container])
+        # call with manually removed prefixes
+        with HDF5TableReader(f.name) as reader:
+            generator = reader.read(
+                "/dl1/params",
+                [HillasParametersContainer(prefix=""), LeakageContainer(prefix="")],
+                prefixes=True,
+            )
+            hillas_, leakage_ = next(generator)
+
+        for value, read_value in zip(
+            leakage_container.as_dict().values(),
+            leakage_.as_dict().values()
+        ):
+            np.testing.assert_equal(value, read_value)
+
+        for value, read_value in zip(
+            hillas_parameter_container.as_dict().values(),
+            hillas_.as_dict().values()
+        ):
+            np.testing.assert_equal(value, read_value)
+
+
+def test_read_duplicated_container_types():
+    hillas_config_1 = HillasParametersContainer(
+        x=1 * u.m, y=2 * u.m, length=3 * u.m, width=4 * u.m,
+        prefix='hillas_1',
+    )
+    hillas_config_2 = HillasParametersContainer(
+        x=2 * u.m, y=3 * u.m, length=4 * u.m, width=5 * u.m,
+        prefix='hillas_2',
+    )
+
+    with tempfile.NamedTemporaryFile() as f:
+        with HDF5TableWriter(f.name, group_name="dl1", add_prefix=True) as writer:
+            writer.write("params", [hillas_config_1, hillas_config_2])
 
-    df = pd.read_hdf(tmp_file.name, key="/blabla/events")
-    assert "hillas_x" in df.columns
-    assert "leakage_pixels_width_1" in df.columns
+        df = pd.read_hdf(f.name, key="/dl1/params")
+        assert "hillas_1_x" in df.columns
+        assert "hillas_2_x" in df.columns
+
+        with HDF5TableReader(f.name) as reader:
+            generator = reader.read(
+                "/dl1/params",
+                [HillasParametersContainer(), HillasParametersContainer()],
+                prefixes=['hillas_1', 'hillas_2']
+            )
+            hillas_1, hillas_2 = next(generator)
+
+        for value, read_value in zip(
+            hillas_config_1.as_dict().values(),
+            hillas_1.as_dict().values()
+        ):
+            np.testing.assert_equal(value, read_value)
+
+        for value, read_value in zip(
+            hillas_config_2.as_dict().values(),
+            hillas_2.as_dict().values()
+        ):
+            np.testing.assert_equal(value, read_value)
+
+
+def test_custom_prefix():
+    container = HillasParametersContainer(
+        x=1 * u.m, y=1 * u.m, length=1 * u.m, width=1 * u.m
+    )
+    container.prefix = "custom"
+    with tempfile.NamedTemporaryFile() as f:
+        with HDF5TableWriter(f.name, group_name="dl1", add_prefix=True) as writer:
+            writer.write("params", container)
+
+        with HDF5TableReader(f.name) as reader:
+            generator = reader.read(
+                "/dl1/params",
+                HillasParametersContainer(),
+                prefixes="custom"
+            )
+            read_container = next(generator)
+        assert isinstance(read_container, HillasParametersContainer)
+        for value, read_value in zip(
+            container.as_dict().values(),
+            read_container.as_dict().values()
+        ):
+            np.testing.assert_equal(value, read_value)
 
 
 def test_units():
     class WithUnits(Container):
         inverse_length = Field(5 / u.m, "foo")
         time = Field(1 * u.s, "bar", unit=u.s)
         grammage = Field(2 * u.g / u.cm ** 2, "baz", unit=u.g / u.cm ** 2)
@@ -153,22 +325,24 @@
     r0tel1 = R0CameraContainer()
     r0tel2 = R0CameraContainer()
     mc = MCEventContainer()
 
     with HDF5TableReader(temp_h5_file) as reader:
 
         # get the generators for each table
-        mctab = reader.read("/R0/MC", mc)
+        # test supplying a single container as well as an
+        # iterable with one entry only
+        mctab = reader.read("/R0/MC", (mc,))
         r0tab1 = reader.read("/R0/tel_001", r0tel1)
         r0tab2 = reader.read("/R0/tel_002", r0tel2)
 
         # read all 3 tables in sync
         for ii in range(3):
 
-            m = next(mctab)
+            m = next(mctab)[0]
             r0_1 = next(r0tab1)
             r0_2 = next(r0tab2)
 
             print("MC:", m)
             print("t0:", r0_1.waveform)
             print("t1:", r0_2.waveform)
             print("---------------------------")
```

### Comparing `ctapipe-0.8.0/ctapipe/io/tests/test_metadata.py` & `ctapipe-0.9.1/ctapipe/io/tests/test_metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             data_level="DL1",
             data_association="Subarray",
             data_model_name="Unofficial DL1",
             data_model_version="1.0",
             data_model_url="http://google.com",
             format="hdf5",
         ),
-        process=meta.Process(_type="Simulation", subtype="Prod3b", _id=423442,),
+        process=meta.Process(type_="Simulation", subtype="Prod3b", id_=423442),
         activity=meta.Activity.from_provenance(prov_activity.provenance),
         instrument=meta.Instrument(
             site="CTA-North",
             class_="Array",
             type_="Layout H1B",
             version="1.0",
             id_="threshold",
@@ -48,17 +48,24 @@
     assert str(uuid.UUID(ref_dict["CTA PRODUCT ID"])) == ref_dict["CTA PRODUCT ID"]
 
     # check that we can write this to the header of a typical table file in multiple
     # formats:
     from astropy.table import Table  # pylint: disable=import-outside-toplevel
 
     table = Table(dict(x=[1, 2, 3], y=[15.2, 15.2, 14.5]))
-    table.meta = ref_dict
-    for file_name in [tmp_path / "test.fits", tmp_path / "test.ecsv"]:
-        table.write(file_name)
+    for path in [tmp_path / "test.fits", tmp_path / "test.ecsv"]:
+        if ".fits" in path.suffixes:
+            reference.format = "fits"
+            ref_dict = reference.to_dict(fits=True)
+        else:
+            reference.format = "ecsv"
+            ref_dict = reference.to_dict()
+
+        table.meta = ref_dict
+        table.write(path)
 
     # write to pytables file
 
     import tables  # pylint: disable=import-outside-toplevel
 
     with tables.open_file(tmp_path / "test.h5", mode="w") as h5file:
         meta.write_to_hdf5(ref_dict, h5file)
```

### Comparing `ctapipe-0.8.0/ctapipe/io/tests/test_simteleventsource.py` & `ctapipe-0.9.1/ctapipe/io/tests/test_simteleventsource.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
 
 def test_properties():
     source = SimTelEventSource(input_url=gamma_test_large_path)
 
     assert source.is_simulation
     assert source.mc_header.corsika_version == 6990
-    assert source.datalevels == (DataLevel.R0, DataLevel.R1, DataLevel.DL0)
+    assert source.datalevels == (DataLevel.R0, DataLevel.R1)
     assert source.obs_id == 7514
 
 
 def test_gamma_file():
     dataset = gamma_test_path
 
     with SimTelEventSource(input_url=dataset) as reader:
@@ -203,15 +203,15 @@
         EventType.SINGLE_PE,
         EventType.FLATFIELD,
         EventType.FLATFIELD,
         EventType.SUBARRAY,
         EventType.SUBARRAY,
     ]
     with SimTelEventSource(
-        input_url=calib_events_path, skip_calibration_events=False,
+        input_url=calib_events_path, skip_calibration_events=False
     ) as reader:
 
         for event, expected_type in zip_longest(reader, expected_types):
             assert event.trigger.event_type is expected_type
 
 
 def test_trigger_times():
```

### Comparing `ctapipe-0.8.0/ctapipe/io/tests/test_toysource.py` & `ctapipe-0.9.1/ctapipe/io/tests/test_toysource.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/io/toymodel.py` & `ctapipe-0.9.1/ctapipe/io/toymodel.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/plotting/bokeh_event_viewer.py` & `ctapipe-0.9.1/ctapipe/plotting/bokeh_event_viewer.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/plotting/charge_resolution.py` & `ctapipe-0.9.1/ctapipe/plotting/charge_resolution.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/plotting/tests/test_bokeh_event_viewer.py` & `ctapipe-0.9.1/ctapipe/plotting/tests/test_bokeh_event_viewer.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/plotting/tests/test_charge_resolution.py` & `ctapipe-0.9.1/ctapipe/plotting/tests/test_charge_resolution.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/HillasReconstructor.py` & `ctapipe-0.9.1/ctapipe/reco/HillasReconstructor.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/ImPACT.py` & `ctapipe-0.9.1/ctapipe/reco/ImPACT.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/energy_regressor.py` & `ctapipe-0.9.1/ctapipe/reco/energy_regressor.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/event_classifier.py` & `ctapipe-0.9.1/ctapipe/reco/event_classifier.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/hillas_intersection.py` & `ctapipe-0.9.1/ctapipe/reco/hillas_intersection.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/reco_algorithms.py` & `ctapipe-0.9.1/ctapipe/reco/reco_algorithms.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/regressor_classifier_base.py` & `ctapipe-0.9.1/ctapipe/reco/regressor_classifier_base.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/shower_max.py` & `ctapipe-0.9.1/ctapipe/reco/shower_max.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/tests/test_HillasReconstructor.py` & `ctapipe-0.9.1/ctapipe/reco/tests/test_HillasReconstructor.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/tests/test_ImPACT.py` & `ctapipe-0.9.1/ctapipe/reco/tests/test_ImPACT.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/tests/test_energy_regressor.py` & `ctapipe-0.9.1/ctapipe/reco/tests/test_energy_regressor.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/tests/test_event_classifier.py` & `ctapipe-0.9.1/ctapipe/reco/tests/test_event_classifier.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/tests/test_hillas_intersection.py` & `ctapipe-0.9.1/ctapipe/reco/tests/test_hillas_intersection.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/tests/test_reconstruction_methods.py` & `ctapipe-0.9.1/ctapipe/reco/tests/test_reconstruction_methods.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/tests/test_regressor_classifier_base.py` & `ctapipe-0.9.1/ctapipe/reco/tests/test_regressor_classifier_base.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/reco/tests/test_showermaxestimator.py` & `ctapipe-0.9.1/ctapipe/reco/tests/test_showermaxestimator.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/tests/coveragerc` & `ctapipe-0.9.1/ctapipe/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/tools/bokeh/file_viewer.py` & `ctapipe-0.9.1/ctapipe/tools/bokeh/file_viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,26 +149,26 @@
     @property
     def event_index(self):
         return self._event_index
 
     @event_index.setter
     def event_index(self, val):
         try:
-            self.event = self.seeker[val]
+            self.event = self.seeker.get_event_index(val)
         except IndexError:
             self.log.warning(f"Event Index {val} does not exist")
 
     @property
     def event_id(self):
         return self._event_id
 
     @event_id.setter
     def event_id(self, val):
         try:
-            self.event = self.seeker[str(val)]
+            self.event = self.seeker.get_event_id(val)
         except IndexError:
             self.log.warning(f"Event ID {val} does not exist")
 
     @property
     def telid(self):
         return self._telid
```

### Comparing `ctapipe-0.8.0/ctapipe/tools/bokeh/templates/index.html` & `ctapipe-0.9.1/ctapipe/tools/bokeh/templates/index.html`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/tools/camdemo.py` & `ctapipe-0.9.1/ctapipe/tools/camdemo.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/tools/display_dl1.py` & `ctapipe-0.9.1/ctapipe/tools/display_dl1.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/tools/display_events_single_tel.py` & `ctapipe-0.9.1/ctapipe/tools/display_events_single_tel.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,21 +26,23 @@
 class SingleTelEventDisplay(Tool):
     name = "ctapipe-display-televents"
     description = Unicode(__doc__)
 
     infile = Path(help="input file to read", exists=True, directory_ok=False).tag(
         config=True
     )
-    tel = Int(help="Telescope ID to display", default=0).tag(config=True)
-    write = Bool(help="Write out images to PNG files", default=False).tag(config=True)
-    clean = Bool(help="Apply image cleaning", default=False).tag(config=True)
-    hillas = Bool(help="Apply and display Hillas parametrization", default=False).tag(
+    tel = Int(help="Telescope ID to display", default_value=0).tag(config=True)
+    write = Bool(help="Write out images to PNG files", default_value=False).tag(
         config=True
     )
-    samples = Bool(help="Show each sample", default=False).tag(config=True)
+    clean = Bool(help="Apply image cleaning", default_value=False).tag(config=True)
+    hillas = Bool(
+        help="Apply and display Hillas parametrization", default_value=False
+    ).tag(config=True)
+    samples = Bool(help="Show each sample", default_value=False).tag(config=True)
     display = Bool(
         help="Display results in interactive window", default_value=True
     ).tag(config=True)
     delay = Float(help="delay between events in s", default_value=0.01, min=0.001).tag(
         config=True
     )
     progress = Bool(help="display progress bar", default_value=True).tag(config=True)
@@ -66,17 +68,15 @@
         super().__init__(**kwargs)
 
     def setup(self):
         print("TOLLES INFILE", self.infile)
         self.event_source = self.add_component(
             EventSource.from_url(self.infile, parent=self)
         )
-        self.event_source.allowed_tels = {
-            self.tel,
-        }
+        self.event_source.allowed_tels = {self.tel}
 
         self.calibrator = self.add_component(
             CameraCalibrator(parent=self, subarray=self.event_source.subarray)
         )
 
         self.log.info(f"SELECTING EVENTS FROM TELESCOPE {self.tel}")
 
@@ -159,14 +159,14 @@
         self.log.info("FINISHED READING DATA FILE")
 
         if disp is None:
             self.log.warning(
                 "No events for tel {} were found in {}. Try a "
                 "different EventIO file or another telescope".format(
                     self.tel, self.infile
-                ),
+                )
             )
 
 
 def main():
     tool = SingleTelEventDisplay()
     tool.run()
```

### Comparing `ctapipe-0.8.0/ctapipe/tools/display_integrator.py` & `ctapipe-0.9.1/ctapipe/tools/display_integrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,18 +270,18 @@
         self.calibrate = self.add_component(
             CameraCalibrator(
                 parent=self, image_extractor=self.extractor, subarray=self.subarray
             )
         )
 
     def start(self):
-        event_num = self.event_index
         if self.use_event_id:
-            event_num = str(event_num)
-        event = self.eventseeker[event_num]
+            event = self.eventseeker.get_event_id(self.event_index)
+        else:
+            event = self.eventseeker.get_event_index(self.event_index)
 
         # Calibrate
         self.calibrate(event)
 
         # Select telescope
         tels = list(event.r0.tels_with_data)
         telid = self.telescope
```

### Comparing `ctapipe-0.8.0/ctapipe/tools/display_summed_images.py` & `ctapipe-0.9.1/ctapipe/tools/display_summed_images.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/tools/dump_instrument.py` & `ctapipe-0.9.1/ctapipe/tools/dump_instrument.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,45 +48,46 @@
     )
 
     def setup(self):
         with event_source(self.infile) as source:
             self.subarray = source.subarray
 
     def start(self):
-        self.write_camera_geometries()
-        self.write_optics_descriptions()
-        self.write_subarray_description()
+        if self.format == "hdf5":
+            self.subarray.to_hdf("subarray.h5")
+        else:
+            self.write_camera_geometries()
+            self.write_optics_descriptions()
+            self.write_subarray_description()
 
     def finish(self):
         pass
 
     @staticmethod
     def _get_file_format_info(format_name, table_type, table_name):
         """ returns file extension + dict of required parameters for
         Table.write"""
         if format_name == "fits":
             return "fits.gz", dict()
         elif format_name == "ecsv":
             return "ecsv.txt", dict(format="ascii.ecsv")
-        elif format_name == "hdf5":
-            return "h5", dict(path="/" + table_type + "/" + table_name)
         else:
-            raise NameError("format not supported")
+            raise NameError(f"format {format_name} not supported")
 
     def write_camera_geometries(self):
         cam_types = get_camera_types(self.subarray)
         self.subarray.info(printer=self.log.info)
         for cam_name in cam_types:
             ext, args = self._get_file_format_info(self.format, "CAMGEOM", cam_name)
 
             self.log.debug(f"writing {cam_name}")
             tel_id = cam_types[cam_name].pop()
             geom = self.subarray.tel[tel_id].camera.geometry
             table = geom.to_table()
-            table.meta["SOURCE"] = self.infile
+            table.meta["SOURCE"] = str(self.infile)
             filename = f"{cam_name}.camgeom.{ext}"
 
             try:
                 table.write(filename, **args)
                 Provenance().add_output_file(filename, "dl0.tel.svc.camera")
             except IOError as err:
                 self.log.warning(
@@ -94,29 +95,29 @@
                 )
 
     def write_optics_descriptions(self):
         sub = self.subarray
         ext, args = self._get_file_format_info(self.format, sub.name, "optics")
 
         tab = sub.to_table(kind="optics")
-        tab.meta["SOURCE"] = self.infile
+        tab.meta["SOURCE"] = str(self.infile)
         filename = f"{sub.name}.optics.{ext}"
         try:
             tab.write(filename, **args)
             Provenance().add_output_file(filename, "dl0.sub.svc.optics")
         except IOError as err:
             self.log.warning(
                 "couldn't write optics description '%s' because: %s", filename, err
             )
 
     def write_subarray_description(self):
         sub = self.subarray
         ext, args = self._get_file_format_info(self.format, sub.name, "subarray")
         tab = sub.to_table(kind="subarray")
-        tab.meta["SOURCE"] = self.infile
+        tab.meta["SOURCE"] = str(self.infile)
         filename = f"{sub.name}.subarray.{ext}"
         try:
             tab.write(filename, **args)
             Provenance().add_output_file(filename, "dl0.sub.svc.subarray")
         except IOError as err:
             self.log.warning(
                 "couldn't write subarray description '%s' because: %s", filename, err
```

### Comparing `ctapipe-0.8.0/ctapipe/tools/dump_triggers.py` & `ctapipe-0.9.1/ctapipe/tools/dump_triggers.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/tools/extract_charge_resolution.py` & `ctapipe-0.9.1/ctapipe/tools/extract_charge_resolution.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/tools/info.py` & `ctapipe-0.9.1/ctapipe/tools/info.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/tools/muon_reconstruction.py` & `ctapipe-0.9.1/ctapipe/tools/muon_reconstruction.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/tools/plot_charge_resolution.py` & `ctapipe-0.9.1/ctapipe/tools/plot_charge_resolution.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/tools/stage1.py` & `ctapipe-0.9.1/ctapipe/tools/stage1.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import tables
 import tables.filters
 from astropy import units as u
 from tqdm.autonotebook import tqdm
 from collections import defaultdict
 
-from ctapipe.io import metadata as meta
+from ..io import metadata as meta, DataLevel
 from ..calib.camera import CameraCalibrator, GainSelector
 from ..containers import (
     ImageParametersContainer,
     TelEventIndexContainer,
     SimulatedShowerDistribution,
     IntensityStatisticsContainer,
     PeakTimeStatisticsContainer,
@@ -73,15 +73,15 @@
         SubarrayDescription to get metadata from
     writer: HDF5TableWriter
         output
     """
     activity = PROV.current_activity.provenance
 
     reference = meta.Reference(
-        contact=meta.Contact(name="", email="", organization="CTA Consortium",),
+        contact=meta.Contact(name="", email="", organization="CTA Consortium"),
         product=meta.Product(
             description="DL1 Data Product",
             data_category="S",
             data_level="DL1",
             data_association="Subarray",
             data_model_name="ASWG DL1",
             data_model_version=DL1_DATA_MODEL_VERSION,
@@ -95,26 +95,25 @@
             class_="Subarray",
             type_="unknown",
             version="unknown",
             id_=subarray.name,
         ),
     )
 
-    # convert all values to strings, since hdf5 can't handle Times, etc.:
     # TODO: add activity_stop_time?
-    headers = {k: str(v) for k, v in reference.to_dict().items()}
+    headers = reference.to_dict()
     meta.write_to_hdf5(headers, writer._h5file)
 
 
 class ImageQualityQuery(QualityQuery):
     """ for configuring image-wise data checks """
 
     quality_criteria = List(
         default_value=[
-            ("size_greater_0", "lambda image_selected: image_selected.sum() > 0"),
+            ("size_greater_0", "lambda image_selected: image_selected.sum() > 0")
         ],
         help=QualityQuery.quality_criteria.help,
     ).tag(config=True)
 
 
 class Stage1ProcessorTool(Tool):
     name = "ctapipe-stage1-process"
@@ -160,18 +159,14 @@
 
     image_extractor_type = create_class_enum_trait(
         base_class=ImageExtractor,
         default_value="NeighborPeakWindowSum",
         help="Method to use to turn a waveform into a single charge value",
     ).tag(config=True)
 
-    gain_selector_type = create_class_enum_trait(
-        base_class=GainSelector, default_value="ThresholdGainSelector"
-    ).tag(config=True)
-
     image_cleaner_type = create_class_enum_trait(
         base_class=ImageCleaner, default_value="TailcutsImageCleaner"
     )
 
     write_index_tables = Bool(
         help=(
             "Generate PyTables index datasets for all tables that contain an "
@@ -187,15 +182,14 @@
 
     aliases = {
         "input": "EventSource.input_url",
         "output": "Stage1ProcessorTool.output_path",
         "allowed-tels": "EventSource.allowed_tels",
         "max-events": "EventSource.max_events",
         "image-extractor-type": "Stage1ProcessorTool.image_extractor_type",
-        "gain-selector-type": "Stage1ProcessorTool.gain_selector_type",
         "image-cleaner-type": "Stage1ProcessorTool.image_cleaner_type",
     }
 
     flags = {
         "write-images": (
             {"Stage1ProcessorTool": {"write_images": True}},
             "store DL1/Event/Telescope images in output",
@@ -246,21 +240,24 @@
             raise ToolConfigurationError(
                 "The options 'write_parameters' and 'write_images' are "
                 "both set to False. No output will be generated in that case. "
                 "Please enable one or both of these options."
             )
 
         # setup components:
+        self.event_source = self.add_component(EventSource.from_config(parent=self))
+
+        datalevels = self.event_source.datalevels
+        if DataLevel.R1 not in datalevels and DataLevel.DL0 not in datalevels:
+            self.log.critical(
+                f"{self.name} needs the EventSource to provide either R1 or DL0 data"
+                f", {self.event_source} provides only {datalevels}"
+            )
+            sys.exit(1)
 
-        self.gain_selector = self.add_component(
-            GainSelector.from_name(self.gain_selector_type, parent=self)
-        )
-        self.event_source = self.add_component(
-            EventSource.from_config(parent=self, gain_selector=self.gain_selector)
-        )
         self.image_extractor = self.add_component(
             ImageExtractor.from_name(
                 self.image_extractor_type,
                 parent=self,
                 subarray=self.event_source.subarray,
             )
         )
@@ -276,16 +273,20 @@
                 self.image_cleaner_type,
                 parent=self,
                 subarray=self.event_source.subarray,
             )
         )
         self.check_image = self.add_component(ImageQualityQuery(parent=self))
 
-        # check component setup
-        if self.event_source.max_events and self.event_source.max_events > 0:
+        # warn if max_events prevents writing the histograms
+        if (
+            isinstance(self.event_source, SimTelEventSource)
+            and self.event_source.max_events
+            and self.event_source.max_events > 0
+        ):
             self.log.warning(
                 "No Simulated shower distributions will be written because "
                 "EventSource.max_events is set to a non-zero number (and therefore "
                 "shower distributions read from the input MC file are invalid)."
             )
 
         # setup HDF5 compression:
@@ -368,55 +369,14 @@
                 if hist["id"] == 6:
                     fill_from_simtel(self.event_source.obs_id, hist, hist_container)
                     writer.write(
                         table_name="simulation/service/shower_distribution",
                         containers=hist_container,
                     )
 
-    def _write_instrument_configuration(self, subarray):
-        """write the SubarrayDescription
-
-        Parameters
-        ----------
-        subarray : ctapipe.instrument.SubarrayDescription
-            subarray description
-        """
-        self.log.debug("Writing instrument configuration")
-        serialize_meta = True
-
-        subarray.to_table().write(
-            self.output_path,
-            path="/configuration/instrument/subarray/layout",
-            serialize_meta=serialize_meta,
-            append=True,
-        )
-        subarray.to_table(kind="optics").write(
-            self.output_path,
-            path="/configuration/instrument/telescope/optics",
-            append=True,
-            serialize_meta=serialize_meta,
-        )
-        for telescope_type in subarray.telescope_types:
-            ids = set(subarray.get_tel_ids_for_type(telescope_type))
-            if len(ids) > 0:  # only write if there is a telescope with this camera
-                tel_id = list(ids)[0]
-                camera = subarray.tel[tel_id].camera
-                camera.geometry.to_table().write(
-                    self.output_path,
-                    path=f"/configuration/instrument/telescope/camera/geometry_{camera}",
-                    append=True,
-                    serialize_meta=serialize_meta,
-                )
-                camera.readout.to_table().write(
-                    self.output_path,
-                    path=f"/configuration/instrument/telescope/camera/readout_{camera}",
-                    append=True,
-                    serialize_meta=serialize_meta,
-                )
-
     def _write_processing_statistics(self):
         """ write out the event selection stats, etc. """
         image_stats = self.check_image.to_table(functions=True)
         image_stats.write(
             self.output_path,
             path="/dl1/service/image_statistics",
             append=True,
@@ -452,20 +412,20 @@
             list(zip(self.check_image.criteria_names[1:], image_criteria)),
         )
 
         # parameterize the event if all criteria pass:
         if all(image_criteria):
             geom_selected = geometry[signal_pixels]
 
-            hillas = hillas_parameters(geom=geom_selected, image=image_selected,)
+            hillas = hillas_parameters(geom=geom_selected, image=image_selected)
             leakage = leakage_parameters(
                 geom=geometry, image=image, cleaning_mask=signal_pixels
             )
             concentration = concentration_parameters(
-                geom=geom_selected, image=image_selected, hillas_parameters=hillas,
+                geom=geom_selected, image=image_selected, hillas_parameters=hillas
             )
             morphology = morphology_parameters(geom=geometry, image_mask=signal_pixels)
             intensity_statistics = descriptive_statistics(
                 image_selected, container_class=IntensityStatisticsContainer
             )
 
             if peak_time is not None:
@@ -522,31 +482,31 @@
             current_pointing = (p.array_azimuth, p.array_altitude)
             if current_pointing != last_pointing:
                 p.prefix = ""
                 writer.write("dl1/monitoring/subarray/pointing", [event.trigger, p])
                 last_pointing = current_pointing
 
             # write the subarray tables
-            writer.write(
-                table_name="simulation/event/subarray/shower",
-                containers=[event.index, event.mc],
-            )
+            if self.event_source.is_simulation:
+                writer.write(
+                    table_name="simulation/event/subarray/shower",
+                    containers=[event.index, event.mc],
+                )
             writer.write(
                 table_name="dl1/event/subarray/trigger",
                 containers=[event.index, event.trigger],
             )
             # write the telescope tables
             self._write_telescope_event(writer, event)
 
     def _write_telescope_event(self, writer, event):
         """
         add entries to the event/telescope tables for each telescope in a single
         event
         """
-
         # write the telescope tables
         for tel_id, dl1_camera in event.dl1.tel.items():
             dl1_camera.prefix = ""  # don't want a prefix for this container
             telescope = self.event_source.subarray.tel[tel_id]
             tel_type = str(telescope)
 
             tel_index = TelEventIndexContainer(
@@ -655,15 +615,15 @@
 
     def _generate_indices(self, writer):
 
         if self.write_images:
             self._generate_table_indices(writer._h5file, "/dl1/event/telescope/images")
         self._generate_table_indices(writer._h5file, "/dl1/event/subarray")
 
-    def _setup_writer(self, writer):
+    def _setup_writer(self, writer: HDF5TableWriter):
         writer.add_column_transform(
             table_name="dl1/event/subarray/trigger",
             col_name="tels_with_trigger",
             transform=self.event_source.subarray.tel_ids_to_mask,
         )
 
         # exclude some columns that are not writable
@@ -694,24 +654,24 @@
                 writer.exclude(
                     f"/simulation/event/telescope/parameters/{table_name}",
                     r"peak_time_.*",
                 )
                 writer.exclude(
                     f"/simulation/event/telescope/parameters/{table_name}", r"timing_.*"
                 )
-                writer.exclude(f"/simulation/event/subarray/shower", "true_tel")
+                writer.exclude("/simulation/event/subarray/shower", "true_tel")
 
     def start(self):
 
         # FIXME: this uses astropy tables hdf5 io, internally using h5py,
         # and must thus be done before the table writer opens the file or it might lead
         # to "Resource temporary unavailable" if h5py and tables are not linked
         # against the same libhdf (happens when using the pre-build pip wheels)
         # should be replaced by writing the table using tables
-        self._write_instrument_configuration(self.event_source.subarray)
+        self.event_source.subarray.to_hdf(self.output_path)
 
         with HDF5TableWriter(
             self.output_path,
             parent=self,
             mode="a",
             add_prefix=True,
             filters=self._hdf5_filters,
```

### Comparing `ctapipe-0.8.0/ctapipe/tools/tests/test_tools.py` & `ctapipe-0.9.1/ctapipe/tools/tests/test_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import tempfile
 import pandas as pd
 import tables
 
 from ctapipe.utils import get_dataset_path
 from ctapipe.core import run_tool
+from ctapipe.io import DataLevel
 import numpy as np
 
 
 GAMMA_TEST_LARGE = get_dataset_path("gamma_test_large.simtel.gz")
 LST_MUONS = get_dataset_path("lst_muons.simtel.zst")
 
 
@@ -88,30 +89,88 @@
             assert tf.root.dl1.event.telescope.images.tel_001
             dl1_image = tf.root.dl1.event.telescope.images.tel_001
             assert "image_mask" in dl1_image.dtype.names
             assert "image" in dl1_image.dtype.names
             assert "peak_time" in dl1_image.dtype.names
 
 
+def test_stage1_datalevels():
+    """test the dl1 tool on a file not providing r1 or dl0"""
+    from ctapipe.io import EventSource
+    from ctapipe.tools.stage1 import Stage1ProcessorTool
+
+    class DummyEventSource(EventSource):
+        @classmethod
+        def is_compatible(cls, path):
+            with open(path, "rb") as f:
+                dummy = f.read(5)
+                return dummy == b"dummy"
+
+        @property
+        def datalevels(self):
+            return (DataLevel.R0,)
+
+        @property
+        def is_simulation(self):
+            return True
+
+        @property
+        def obs_id(self):
+            return 1
+
+        @property
+        def subarray(self):
+            return None
+
+        def _generator(self):
+            return None
+
+    with tempfile.NamedTemporaryFile(mode="wb", suffix=".dummy") as f:
+        with tempfile.NamedTemporaryFile(mode="wb", suffix=".h5") as out:
+            f.write(b"dummy")
+            f.flush()
+
+            tool = Stage1ProcessorTool()
+            assert (
+                run_tool(
+                    tool,
+                    argv=[
+                        "--config=./examples/stage1_config.json",
+                        f"--input={f.name}",
+                        f"--output={out.name}",
+                        "--write-images",
+                        "--overwrite",
+                    ],
+                )
+                == 1
+            )
+            # make sure the dummy event source was really used
+            assert isinstance(tool.event_source, DummyEventSource)
+
+            # we need to "touch" the output file again, otherwise tempfile will
+            # complain it no longer exists as the tool removed it
+            open(out.name, mode="a").close()
+
+
 def test_muon_reconstruction(tmpdir):
     from ctapipe.tools.muon_reconstruction import MuonAnalysis
 
     with tempfile.NamedTemporaryFile(suffix=".hdf5") as f:
         assert (
             run_tool(
                 MuonAnalysis(),
-                argv=[f"--input={LST_MUONS}", f"--output={f.name}", "--overwrite",],
+                argv=[f"--input={LST_MUONS}", f"--output={f.name}", "--overwrite"],
             )
             == 0
         )
 
-        t = tables.open_file(f.name)
-        table = t.root.dl1.event.telescope.parameters.muons[:]
-        assert len(table) > 20
-        assert np.count_nonzero(np.isnan(table["muonring_radius"])) == 0
+        with tables.open_file(f.name) as t:
+            table = t.root.dl1.event.telescope.parameters.muons[:]
+            assert len(table) > 20
+            assert np.count_nonzero(np.isnan(table["muonring_radius"])) == 0
 
     assert run_tool(MuonAnalysis(), ["--help-all"]) == 0
 
 
 def test_display_summed_images(tmpdir):
     from ctapipe.tools.display_summed_images import ImageSumDisplayerTool
 
@@ -199,18 +258,25 @@
 
 def test_dump_instrument(tmpdir):
     from ctapipe.tools.dump_instrument import DumpInstrumentTool
 
     sys.argv = ["dump_instrument"]
     tmpdir.chdir()
 
-    tool = DumpInstrumentTool(infile=GAMMA_TEST_LARGE,)
+    tool = DumpInstrumentTool()
 
-    assert run_tool(tool) == 0
+    assert run_tool(tool, [f"--infile={GAMMA_TEST_LARGE}"]) == 0
     assert tmpdir.join("FlashCam.camgeom.fits.gz").exists()
+
+    assert run_tool(tool, [f"--infile={GAMMA_TEST_LARGE}", "--format=ecsv"]) == 0
+    assert tmpdir.join("MonteCarloArray.optics.ecsv.txt").exists()
+
+    assert run_tool(tool, [f"--infile={GAMMA_TEST_LARGE}", "--format=hdf5"]) == 0
+    assert tmpdir.join("subarray.h5").exists()
+
     assert run_tool(tool, ["--help-all"]) == 0
 
 
 def test_camdemo():
     from ctapipe.tools.camdemo import CameraDemo
 
     sys.argv = ["camera_demo"]
```

### Comparing `ctapipe-0.8.0/ctapipe/tools/utils.py` & `ctapipe-0.9.1/ctapipe/tools/utils.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/CutFlow.py` & `ctapipe-0.9.1/ctapipe/utils/CutFlow.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/__init__.py` & `ctapipe-0.9.1/ctapipe/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/astro.py` & `ctapipe-0.9.1/ctapipe/utils/astro.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/datasets.py` & `ctapipe-0.9.1/ctapipe/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/fitshistogram.py` & `ctapipe-0.9.1/ctapipe/utils/fitshistogram.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/linalg.py` & `ctapipe-0.9.1/ctapipe/utils/linalg.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from astropy.coordinates import Angle
-from astropy import units as u
 
 import numpy as np
-from numpy import cos, sin, arctan2 as atan2, arccos as acos
+from numpy import cos, sin
 
 __all__ = ["rotation_matrix_2d", "length", "normalise", "angle"]
 
 
 def rotation_matrix_2d(angle):
     """construct a 2D rotation matrix as a numpy NDArray that rotates a
     vector clockwise. Angle should be any object that can be converted
```

### Comparing `ctapipe-0.8.0/ctapipe/utils/rgbtohex.py` & `ctapipe-0.9.1/ctapipe/utils/rgbtohex.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/table_interpolator.py` & `ctapipe-0.9.1/ctapipe/utils/table_interpolator.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/template_network_interpolator.py` & `ctapipe-0.9.1/ctapipe/utils/template_network_interpolator.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/tests/test_CutFlow.py` & `ctapipe-0.9.1/ctapipe/utils/tests/test_CutFlow.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/tests/test_astro.py` & `ctapipe-0.9.1/ctapipe/utils/tests/test_astro.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/tests/test_datasets.py` & `ctapipe-0.9.1/ctapipe/utils/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/tests/test_fitshistogram.py` & `ctapipe-0.9.1/ctapipe/utils/tests/test_fitshistogram.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/tests/test_linalg.py` & `ctapipe-0.9.1/ctapipe/utils/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/tests/test_quantities.py` & `ctapipe-0.9.1/ctapipe/utils/tests/test_quantities.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/tests/test_rgbtohex.py` & `ctapipe-0.9.1/ctapipe/utils/tests/test_rgbtohex.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/tests/test_unstructured_interpolator.py` & `ctapipe-0.9.1/ctapipe/utils/tests/test_unstructured_interpolator.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/utils/unstructured_interpolator.py` & `ctapipe-0.9.1/ctapipe/utils/unstructured_interpolator.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/version.py` & `ctapipe-0.9.1/ctapipe/version.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/visualization/bokeh.py` & `ctapipe-0.9.1/ctapipe/visualization/bokeh.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/visualization/mpl_array.py` & `ctapipe-0.9.1/ctapipe/visualization/mpl_array.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/visualization/mpl_camera.py` & `ctapipe-0.9.1/ctapipe/visualization/mpl_camera.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,28 +91,29 @@
         ax=None,
         title=None,
         norm="lin",
         cmap=None,
         allow_pick=False,
         autoupdate=True,
         autoscale=True,
+        show_frame=True,
     ):
         self.axes = ax if ax is not None else plt.gca()
         self.pixels = None
         self.colorbar = None
         self.autoupdate = autoupdate
         self.autoscale = autoscale
         self._active_pixel = None
         self._active_pixel_label = None
         self._axes_overlays = []
 
         self.geom = geometry
 
         if title is None:
-            title = geometry.camera_name
+            title = f"{geometry.camera_name}"
 
         # initialize the plot and generate the pixels as a
         # RegularPolyCollection
 
         patches = []
 
         if hasattr(self.geom, "mask"):
@@ -154,18 +155,18 @@
         self.pixel_highlighting.set_linewidth(0)
         self.axes.add_collection(self.pixel_highlighting)
 
         # Set up some nice plot defaults
 
         self.axes.set_aspect("equal", "datalim")
         self.axes.set_title(title)
-        self.axes.set_xlabel(f"X position ({self.geom.pix_x.unit})")
-        self.axes.set_ylabel(f"Y position ({self.geom.pix_y.unit})")
         self.axes.autoscale_view()
 
+        if show_frame:
+            self.add_frame_name()
         # set up a patch to display when a pixel is clicked (and
         # pixel_picker is enabled):
 
         self._active_pixel = copy.copy(patches[0])
         self._active_pixel.set_facecolor("r")
         self._active_pixel.set_alpha(0.5)
         self._active_pixel.set_linewidth(2.0)
@@ -189,14 +190,15 @@
 
         if image is not None:
             self.image = image
         else:
             self.image = np.zeros_like(self.geom.pix_id, dtype=np.float)
 
         self.norm = norm
+        self.auto_set_axes_labels()
 
     def highlight_pixels(self, pixels, color="g", linewidth=1, alpha=0.75):
         """
         Highlight the given pixels with a colored line around them
 
         Parameters
         ----------
@@ -467,7 +469,37 @@
         """virtual function to overide in sub-classes to do something special
         when a pixel is clicked
         """
         print(f"Clicked pixel_id {pix_id}")
 
     def show(self):
         self.axes.figure.show()
+
+    def auto_set_axes_labels(self):
+        """ set the axes labels based on the Frame attribute"""
+        axes_labels = ("X", "Y")
+        if self.geom.frame is not None:
+            axes_labels = list(
+                self.geom.frame.get_representation_component_names().keys()
+            )
+
+        self.axes.set_xlabel(f"{axes_labels[0]}  ({self.geom.pix_x.unit})")
+        self.axes.set_ylabel(f"{axes_labels[1]}  ({self.geom.pix_y.unit})")
+
+    def add_frame_name(self, color="grey"):
+        """ label the frame type of the display (e.g. CameraFrame) """
+
+        frame_name = (
+            self.geom.frame.__class__.__name__
+            if self.geom.frame is not None
+            else "Unknown Frame"
+        )
+        self.axes.text(  # position text relative to Axes
+            1.0,
+            0.0,
+            frame_name,
+            ha="right",
+            va="bottom",
+            transform=self.axes.transAxes,
+            color=color,
+            fontsize="smaller",
+        )
```

### Comparing `ctapipe-0.8.0/ctapipe/visualization/tests/test_bokeh.py` & `ctapipe-0.9.1/ctapipe/visualization/tests/test_bokeh.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe/visualization/tests/test_mpl.py` & `ctapipe-0.9.1/ctapipe/visualization/tests/test_mpl.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe.egg-info/PKG-INFO` & `ctapipe-0.9.1/ctapipe.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,72 @@
 Metadata-Version: 2.1
 Name: ctapipe
-Version: 0.8.0
+Version: 0.9.1
 Summary: CTA Python pipeline experimental version
 Home-page: https://github.com/cta-observatory/ctapipe
 Author: ctapipe developers
 Author-email: karl.kosack@cea.fr
 License: BSD 3-Clause License
-Description: =========================================================
-        ctapipe |teststatus| |codacy| |coverage| |conda| |doiv07|
-        =========================================================
+Description: ============================================================
+        ctapipe |teststatus| |codacy| |coverage| |conda| |doilatest|
+        ============================================================
         
         .. |teststatus| image:: https://travis-ci.com/cta-observatory/ctapipe.svg?branch=master
             :target: https://travis-ci.com/cta-observatory/ctapipe
             :alt: Test Status
         .. |codacy|  image:: https://api.codacy.com/project/badge/Grade/6192b471956b4cc684130c80c8214115   
           :target: https://www.codacy.com/gh/cta-observatory/ctapipe?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cta-observatory/ctapipe&amp;utm_campaign=Badge_Grade
         .. |conda| image:: https://anaconda.org/cta-observatory/ctapipe/badges/installer/conda.svg
         .. |coverage| image:: https://codecov.io/gh/cta-observatory/ctapipe/branch/master/graph/badge.svg
           :target: https://codecov.io/gh/cta-observatory/ctapipe
-        .. |doiv07| image:: https://zenodo.org/badge/37927055.svg
+        .. |doilatest| image:: https://zenodo.org/badge/37927055.svg
           :target: https://zenodo.org/badge/latestdoi/37927055
+        .. |doiv07| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3372211.svg
+           :target: https://doi.org/10.5281/zenodo.3372211
+        .. |doiv08| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3837306.svg
+           :target: https://doi.org/10.5281/zenodo.3837306
         
         Low-level data processing pipeline software for
         `CTA <www.cta-observatory.org>`_ (the Cherenkov Telescope Array)
         
         This is code is a prototype data processing framework and is under rapid
         development. It is not recommended for production use unless you are an
         expert or developer!
         
         * Code: https://github.com/cta-observatory/ctapipe
         * Docs: https://cta-observatory.github.io/ctapipe/
         * Slack: Contact Karl Kosack for invite
         
         Citing this software
         --------------------
-        If you use this software for a publication, please cite using the following DOIs: 
+        If you use this software for a publication, please cite the proper version using the following DOIs:
         
         - v0.7.0 : |doiv07|
-        
+        - v0.8.0 : |doiv08|
         
         Installation for Users
         ----------------------
         
         *ctapipe* and its dependencies may be installed using the *Anaconda* or
         *Miniconda* package system. We recommend creating a conda virtual environment
         first, to isolate the installed version and dependencies from your master
         environment (this is optional).
         
         
         The following command will set up a conda virtual environment, add the
-        necessary package channels, and download ctapipe and its dependencies. The
-        file *environment.yml* can be found in this repo. 
-        Note this is *pre-alpha* software and is not yet stable enough for end-users (expect large API changes until the first stable 1.0 release).
-        
-        ::
+        necessary package channels, and install ctapipe specified version and its dependencies::
         
+          CTAPIPE_VER=0.8.0
+          wget https://raw.githubusercontent.com/cta-observatory/ctapipe/v$CTAPIPE_VER/environment.yml
           conda env create -n cta -f environment.yml
           conda activate cta
-          conda install -c cta-observatory ctapipe
+          conda install -c cta-observatory ctapipe=$CTAPIPE_VER
         
+        The file *environment.yml* can be found in this repo. 
+        Note this is *pre-alpha* software and is not yet stable enough for end-users (expect large API changes until the first stable 1.0 release).
         
         Developers should follow the development install instructions found in the
         `documentation <https://cta-observatory.github
         .io/ctapipe/getting_started>`_.
         
         
 Platform: UNKNOWN
```

### Comparing `ctapipe-0.8.0/ctapipe.egg-info/SOURCES.txt` & `ctapipe-0.9.1/ctapipe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 setup.py
 .github/release-drafter.yml
 ci/install.sh
 ctapipe/__init__.py
 ctapipe/_version_cache.py
 ctapipe/conftest.py
 ctapipe/containers.py
+ctapipe/fitting.py
 ctapipe/version.py
 ctapipe.egg-info/PKG-INFO
 ctapipe.egg-info/SOURCES.txt
 ctapipe.egg-info/dependency_links.txt
 ctapipe.egg-info/entry_points.txt
 ctapipe.egg-info/not-zip-safe
 ctapipe.egg-info/requires.txt
@@ -132,24 +133,26 @@
 ctapipe/instrument/tests/__init__.py
 ctapipe/instrument/tests/test_guessing.py
 ctapipe/instrument/tests/test_optics.py
 ctapipe/instrument/tests/test_subarray.py
 ctapipe/instrument/tests/test_telescope.py
 ctapipe/io/__init__.py
 ctapipe/io/array.py
+ctapipe/io/astropy_helpers.py
 ctapipe/io/datalevels.py
 ctapipe/io/eventseeker.py
 ctapipe/io/eventsource.py
 ctapipe/io/files.py
 ctapipe/io/hdf5tableio.py
 ctapipe/io/metadata.py
 ctapipe/io/simteleventsource.py
 ctapipe/io/tableio.py
 ctapipe/io/toymodel.py
 ctapipe/io/tests/__init__.py
+ctapipe/io/tests/test_astropy_helpers.py
 ctapipe/io/tests/test_available_sources.py
 ctapipe/io/tests/test_event_source.py
 ctapipe/io/tests/test_eventseeker.py
 ctapipe/io/tests/test_files.py
 ctapipe/io/tests/test_hdf5.py
 ctapipe/io/tests/test_metadata.py
 ctapipe/io/tests/test_prod2.py
@@ -178,14 +181,15 @@
 ctapipe/reco/tests/test_hillas_intersection.py
 ctapipe/reco/tests/test_reconstruction_methods.py
 ctapipe/reco/tests/test_regressor_classifier_base.py
 ctapipe/reco/tests/test_showermaxestimator.py
 ctapipe/tests/__init__.py
 ctapipe/tests/coveragerc
 ctapipe/tests/setup_package.py
+ctapipe/tests/test_fitting.py
 ctapipe/tools/__init__.py
 ctapipe/tools/camdemo.py
 ctapipe/tools/display_dl1.py
 ctapipe/tools/display_events_single_tel.py
 ctapipe/tools/display_integrator.py
 ctapipe/tools/display_summed_images.py
 ctapipe/tools/dump_instrument.py
@@ -251,14 +255,15 @@
 docs/ctapipe_api/calib/index_camera.rst
 docs/ctapipe_api/containers/index.rst
 docs/ctapipe_api/coordinates/index.rst
 docs/ctapipe_api/core/corediagram.dot
 docs/ctapipe_api/core/index.rst
 docs/ctapipe_api/core/tool-component.pdf
 docs/ctapipe_api/core/tool-component.png
+docs/ctapipe_api/image/TwoPassWindowSum_1st_pass_example.png
 docs/ctapipe_api/image/cleaning.rst
 docs/ctapipe_api/image/dilate.png
 docs/ctapipe_api/image/extractor.rst
 docs/ctapipe_api/image/geometry_converter.rst
 docs/ctapipe_api/image/hillas.rst
 docs/ctapipe_api/image/index.rst
 docs/ctapipe_api/image/muon.rst
```

### Comparing `ctapipe-0.8.0/ctapipe.egg-info/entry_points.txt` & `ctapipe-0.9.1/ctapipe.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/ctapipe.egg-info/requires.txt` & `ctapipe-0.9.1/ctapipe.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/FAQ.rst` & `ctapipe-0.9.1/docs/FAQ.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/Makefile` & `ctapipe-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/cameras.png` & `ctapipe-0.9.1/docs/cameras.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/changelog.rst` & `ctapipe-0.9.1/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/conf.py` & `ctapipe-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/calib/index.rst` & `ctapipe-0.9.1/docs/ctapipe_api/calib/index.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/calib/index_camera.rst` & `ctapipe-0.9.1/docs/ctapipe_api/calib/index_camera.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/coordinates/index.rst` & `ctapipe-0.9.1/docs/ctapipe_api/coordinates/index.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/core/corediagram.dot` & `ctapipe-0.9.1/docs/ctapipe_api/core/corediagram.dot`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/core/index.rst` & `ctapipe-0.9.1/docs/ctapipe_api/core/index.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/core/tool-component.pdf` & `ctapipe-0.9.1/docs/ctapipe_api/core/tool-component.pdf`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/core/tool-component.png` & `ctapipe-0.9.1/docs/ctapipe_api/core/tool-component.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/image/dilate.png` & `ctapipe-0.9.1/docs/ctapipe_api/image/dilate.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/image/extractor.rst` & `ctapipe-0.9.1/docs/ctapipe_api/image/extractor.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 .. _image_charge_extractors:
 
 #########################################
 Image Extraction (waveform cube to image)
 #########################################
 
+.. contents::
+   :depth: 1
+   :local:
+
 The main operation in the event processing from DL0 to Dl1 is the reducing of the
 waveforms into per-pixel signal-summarising parameters, from which image analysis
 can be performed to reconstruct the Cherenkov shower. This summary is
 performed for three reasons:
 
 * The amount of useful information is arguably a small fraction of
   the total waveform volume (across all pixels in the Cherenkov camera).
@@ -67,10 +71,20 @@
 samples to account for the percentage of the pulse missed by the the window.
 This way, if a single photoelectron exists in the waveform (and no noise) then
 the result of the `ImageExtractor` will equal 1, no matter the window size.
 
 The extracted pulse time is corrected for the waveform sampling rate to be
 provided in units of nanoseconds.
 
+********
+Examples
+********
 
-.. automodapi:: ctapipe.image.extractor
+TwoPassWindowSum
+----------------
+
+Example of 1st pass integration:
 
+.. image:: ./TwoPassWindowSum_1st_pass_example.png
+
+
+.. automodapi:: ctapipe.image.extractor
```

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/image/index.rst` & `ctapipe-0.9.1/docs/ctapipe_api/image/index.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/instrument/camera_geometry.rst` & `ctapipe-0.9.1/docs/ctapipe_api/instrument/camera_geometry.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/instrument/camera_readout.rst` & `ctapipe-0.9.1/docs/ctapipe_api/instrument/camera_readout.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/instrument/config.dot` & `ctapipe-0.9.1/docs/ctapipe_api/instrument/config.dot`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/instrument/index.rst` & `ctapipe-0.9.1/docs/ctapipe_api/instrument/index.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/instrument/subarray.rst` & `ctapipe-0.9.1/docs/ctapipe_api/instrument/subarray.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/io/index.rst` & `ctapipe-0.9.1/docs/ctapipe_api/io/index.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/io/shower.png` & `ctapipe-0.9.1/docs/ctapipe_api/io/shower.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/reco/ImPACT.rst` & `ctapipe-0.9.1/docs/ctapipe_api/reco/ImPACT.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/reco/images/ImageTemplates.png` & `ctapipe-0.9.1/docs/ctapipe_api/reco/images/ImageTemplates.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/reco/images/goodness.png` & `ctapipe-0.9.1/docs/ctapipe_api/reco/images/goodness.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/reco/images/likelihood.png` & `ctapipe-0.9.1/docs/ctapipe_api/reco/images/likelihood.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/reco/images/predictions.png` & `ctapipe-0.9.1/docs/ctapipe_api/reco/images/predictions.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/reco/index.rst` & `ctapipe-0.9.1/docs/ctapipe_api/reco/index.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/tools/index.rst` & `ctapipe-0.9.1/docs/ctapipe_api/tools/index.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/utils/index.rst` & `ctapipe-0.9.1/docs/ctapipe_api/utils/index.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_api/visualization/index.rst` & `ctapipe-0.9.1/docs/ctapipe_api/visualization/index.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/ctapipe_logo.png` & `ctapipe-0.9.1/docs/ctapipe_logo.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/data_models/dl1.rst` & `ctapipe-0.9.1/docs/data_models/dl1.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/development/code-guidelines.rst` & `ctapipe-0.9.1/docs/development/code-guidelines.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/development/maintainer-info.rst` & `ctapipe-0.9.1/docs/development/maintainer-info.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/development/pullrequests.rst` & `ctapipe-0.9.1/docs/development/pullrequests.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/development/py-pipe-dependencies.pdf` & `ctapipe-0.9.1/docs/development/py-pipe-dependencies.pdf`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/development/py-pipe-dependencies.png` & `ctapipe-0.9.1/docs/development/py-pipe-dependencies.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/development/rootmigration.rst` & `ctapipe-0.9.1/docs/development/rootmigration.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/development/style-guide.rst` & `ctapipe-0.9.1/docs/development/style-guide.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/development/support-libraries.rst` & `ctapipe-0.9.1/docs/development/support-libraries.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/event.png` & `ctapipe-0.9.1/docs/event.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/examples/.ipynb_checkpoints/InstrumentDescription-checkpoint.ipynb` & `ctapipe-0.9.1/docs/examples/.ipynb_checkpoints/InstrumentDescription-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/examples/.ipynb_checkpoints/Tools-checkpoint.ipynb` & `ctapipe-0.9.1/docs/examples/Tools.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/examples/.ipynb_checkpoints/convert_hex_to_square-checkpoint.ipynb` & `ctapipe-0.9.1/docs/examples/.ipynb_checkpoints/convert_hex_to_square-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/examples/InstrumentDescription.ipynb` & `ctapipe-0.9.1/docs/examples/InstrumentDescription.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/examples/Tools.ipynb` & `ctapipe-0.9.1/docs/examples/.ipynb_checkpoints/Tools-checkpoint.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998558118899734%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(27, '    \\n'), (28, '    def __init__(self, config=None, "*

 * *            "parent=None, **kwargs):\\n'), (29, '        super().__init__(config=config, "*

 * *            "parent=parent, **kwargs)\\n'), (30, '        # components can have sub components, "*

 * *            "but these must have \\n'), (31, '        # then parent=self as argument and be "*

 * *            "assigned as member\\n'), (32, '        # so the full config can be received "*

 * *            "later\\n'), (33, '         […]*

```diff
@@ -79,14 +79,21 @@
                 "        exists=None,  # set to True to require existing, False for requiring non-existing\n",
                 "        directory_ok=False,\n",
                 "    ).tag(config=True)\n",
                 "    outfile = Path(\n",
                 "        help=\"output file name\",\n",
                 "        exists=False, directory_ok=False\n",
                 "    ).tag(config=True)\n",
+                "    \n",
+                "    def __init__(self, config=None, parent=None, **kwargs):\n",
+                "        super().__init__(config=config, parent=parent, **kwargs)\n",
+                "        # components can have sub components, but these must have \n",
+                "        # then parent=self as argument and be assigned as member\n",
+                "        # so the full config can be received later\n",
+                "        self.subcompent = MyComponent(parent=self)\n",
                 "\n",
                 "    @observe(\"outfile\")\n",
                 "    def on_outfile_changed(self, change):\n",
                 "        self.log.warning(\"Outfile was changed to '{}'\".format(change))\n",
                 "\n",
                 "\n",
                 "class TelescopeWiseComponent(TelescopeComponent):\n",
@@ -192,29 +199,20 @@
                 "\n",
                 "    # Which classes are registered for configuration\n",
                 "    classes = List([MyComponent, AdvancedComponent, SecondaryMyComponent, TelescopeWiseComponent])\n",
                 "\n",
                 "    # local configuration parameters\n",
                 "    iterations = Integer(5,help=\"Number of times to run\",allow_none=False).tag(config=True)\n",
                 "\n",
-                "    def setup_comp(self):\n",
-                "        # when constructing Components, you must add them to the \n",
-                "        # list of registered instances using add_component. This allows\n",
-                "        # the full configuration to be tracked\n",
-                "        self.comp = self.add_component(MyComponent(parent=self))\n",
-                "        self.comp2 = self.add_component(SecondaryMyComponent(parent=self))\n",
-                "\n",
-                "    def setup_advanced(self):\n",
-                "        self.advanced = self.add_component(AdvancedComponent(parent=self))\n",
-                "        self.comp3 = self.add_component(TelescopeWiseComponent(parent=self, subarray=subarray))\n",
-                "\n",
-                "\n",
                 "    def setup(self):\n",
-                "        self.setup_comp()\n",
-                "        self.setup_advanced()\n",
+                "        self.comp = MyComponent(parent=self)\n",
+                "        self.comp2 = SecondaryMyComponent(parent=self)\n",
+                "        self.comp3 = TelescopeWiseComponent(parent=self, subarray=subarray)\n",
+                "        self.advanced = AdvancedComponent(parent=self)\n",
+                "\n",
                 "\n",
                 "    def start(self):\n",
                 "        self.log.info(\"Performing {} iterations...\".format(self.iterations))\n",
                 "        for ii in range(self.iterations):\n",
                 "            self.log.info(\"ITERATION {}\".format(ii))\n",
                 "            self.comp.do_thing()\n",
                 "            self.comp2.do_thing()\n",
```

### Comparing `ctapipe-0.8.0/docs/examples/camera_display.ipynb` & `ctapipe-0.9.1/docs/examples/camera_display.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/examples/container.h5` & `ctapipe-0.9.1/docs/examples/container.h5`

 * *Command `'h5dump {}'` failed with exit code 1. Standard output:*

 * *    h5dump error: unable to print data*

 * *    h5dump error: unable to print data*

 * *Files 5% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 00000ad0: 0300 1000 0000 0000 666c 6574 6368 6572  ........fletcher
 00000ae0: 3332 0000 0000 0000 017d 0800 0100 0700  32.......}......
 00000af0: 626c 6f73 6300 0000 0200 0000 0200 0000  blosc...........
 00000b00: 2200 0000 eeff 0000 0500 0000 0100 0000  "...............
 00000b10: 0500 0000 0000 0000 0800 1800 0000 0000  ................
 00000b20: 0302 0208 1100 0000 0000 0087 0700 0022  ..............."
 00000b30: 0000 0000 0000 0000 1200 0800 0000 0000  ................
-00000b40: 0100 0000 588a be5e 0000 0000 0000 0000  ....X..^........
+00000b40: 0100 0000 45a8 1a5f 0000 0000 0000 0000  ....E.._........
 00000b50: 534e 4f44 0100 0100 0800 0000 0000 0000  SNOD............
 00000b60: 1809 0000 0000 0000 0000 0000 0000 0000  ................
 00000b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -260,17 +260,17 @@
 00001030: 1400 0000 0100 0000 0000 0800 0000 0000  ................
 00001040: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0c00 3000 0000 0000 0100 0d00 0800 0800  ..0.............
 00001060: 615f 666c 6f61 745f 554e 4954 0000 0000  a_float_UNIT....
 00001070: 1310 0000 0100 0000 0100 0000 0000 0000  ................
 00001080: 6d00 0000 0000 0000 0c00 4000 0000 0000  m.........@.....
 00001090: 0100 1000 0800 0800 4354 4150 4950 455f  ........CTAPIPE_
-000010a0: 5645 5253 494f 4e00 1310 0000 1800 0000  VERSION.........
-000010b0: 0100 0000 0000 0000 302e 372e 302e 706f  ........0.7.0.po
-000010c0: 7374 3232 382b 6769 7432 3331 3639 3739  st228+git2316979
+000010a0: 5645 5253 494f 4e00 1310 0000 1700 0000  VERSION.........
+000010b0: 0100 0000 0000 0000 302e 382e 302e 706f  ........0.8.0.po
+000010c0: 7374 3230 2b67 6974 3531 6265 6361 6500  st20+git51becae.
 000010d0: 0c00 3000 0000 0000 0100 0600 0c00 0800  ..0.............
 000010e0: 4e52 4f57 5300 0000 1008 0000 0800 0000  NROWS...........
 000010f0: 0000 4000 0000 0000 0100 0000 0000 0000  ..@.............
 00001100: 0a00 0000 0000 0000 5452 4545 0100 0100  ........TREE....
 00001110: ffff ffff ffff ffff ffff ffff ffff ffff  ................
 00001120: c300 0000 0000 0000 0000 0000 0000 0000  ................
 00001130: 0000 0000 0000 0000 3819 0000 0000 0000  ........8.......
@@ -501,16 +501,16 @@
 00001f40: 0000 0001 0200 0000 0000 0003 0010 0000  ................
 00001f50: 0000 0066 6c65 7463 6865 7233 3200 0000  ...fletcher32...
 00001f60: 0000 0001 7d08 0001 0007 0062 6c6f 7363  ....}......blosc
 00001f70: 0000 0002 0000 0002 0000 0022 0000 00ee  ..........."....
 00001f80: ff00 0005 0000 0001 0000 0005 0000 0000  ................
 00001f90: 0000 0008 0018 0000 0000 0003 0202 8325  ...............%
 00001fa0: 0000 0000 0000 8707 0000 2200 0000 0000  ..........".....
-00001fb0: 0000 0012 0008 0000 0000 0001 0000 0058  ...............X
-00001fc0: 8abe 5e00 0000 0000 0000 0053 4e4f 4401  ..^........SNOD.
+00001fb0: 0000 0012 0008 0000 0000 0001 0000 0045  ...............E
+00001fc0: a81a 5f00 0000 0000 0000 0053 4e4f 4401  .._........SNOD.
 00001fd0: 0001 0008 0000 0000 0000 0093 1d00 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -588,17 +588,17 @@
 000024b0: 0000 0000 0008 0000 0000 0001 0000 0000  ................
 000024c0: 0000 0000 0000 0000 0000 000c 0030 0000  .............0..
 000024d0: 0000 0001 000d 0008 0008 0061 5f66 6c6f  ...........a_flo
 000024e0: 6174 5f55 4e49 5400 0000 0013 1000 0001  at_UNIT.........
 000024f0: 0000 0001 0000 0000 0000 006d 0000 0000  ...........m....
 00002500: 0000 000c 0040 0000 0000 0001 0010 0008  .....@..........
 00002510: 0008 0043 5441 5049 5045 5f56 4552 5349  ...CTAPIPE_VERSI
-00002520: 4f4e 0013 1000 0018 0000 0001 0000 0000  ON..............
-00002530: 0000 0030 2e37 2e30 2e70 6f73 7432 3238  ...0.7.0.post228
-00002540: 2b67 6974 3233 3136 3937 390c 0030 0000  +git2316979..0..
+00002520: 4f4e 0013 1000 0017 0000 0001 0000 0000  ON..............
+00002530: 0000 0030 2e38 2e30 2e70 6f73 7432 302b  ...0.8.0.post20+
+00002540: 6769 7435 3162 6563 6165 000c 0030 0000  git51becae...0..
 00002550: 0000 0001 0006 000c 0008 004e 524f 5753  ...........NROWS
 00002560: 0000 0010 0800 0008 0000 0000 0040 0000  .............@..
 00002570: 0000 0001 0000 0000 0000 000a 0000 0000  ................
 00002580: 0000 0054 5245 4501 0001 00ff ffff ffff  ...TREE.........
 00002590: ffff ffff ffff ffff ffff ffc3 0000 0000  ................
 000025a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000025b0: 0000 00b3 2d00 0000 0000 0000 0000 0000  ....-...........
```

### Comparing `ctapipe-0.8.0/docs/examples/containers.ipynb` & `ctapipe-0.9.1/docs/examples/containers.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/examples/containers_with_enums_and_table_writer.ipynb` & `ctapipe-0.9.1/docs/examples/containers_with_enums_and_table_writer.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/examples/convert_hex_to_square.ipynb` & `ctapipe-0.9.1/docs/examples/convert_hex_to_square.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/examples/dilate_image.ipynb` & `ctapipe-0.9.1/docs/examples/dilate_image.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/examples/nd_interpolation.ipynb` & `ctapipe-0.9.1/docs/examples/nd_interpolation.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/examples/provenance.ipynb` & `ctapipe-0.9.1/docs/examples/provenance.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/examples/provenance.log` & `ctapipe-0.9.1/docs/examples/provenance.log`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8409507575757577%*

 * *Differences: {'0': "{'activity_uuid': '8168267e-5e2c-4a7d-a27f-f7a1ca9efa13', 'start': {'time_utc': "*

 * *      "'2020-07-24T09:21:40.994'}, 'stop': {'time_utc': '2020-07-24T09:21:41.527'}, 'system': "*

 * *      "{'ctapipe_version': '0.8.0.post20+git51becae', 'eventio_version': '1.4.1', 'platform': "*

 * *      "{'version': '#1 SMP PREEMPT Thu, 16 Jul 2020 19:34:49 +0000', 'release': '5.7.9-arch1-1', "*

 * *      "'boot_time': '2020-07-24T07:57:22.000'}, 'environment': {'PATH': "*

 * *      "'/home/maxnoe/.local/anaconda3/envs/ctapipe/bin:/ho […]*

```diff
@@ -1,11 +1,11 @@
 [
     {
         "activity_name": "mytool",
-        "activity_uuid": "6a51ce24-1a6c-4810-a7a5-0c32456c592a",
+        "activity_uuid": "8168267e-5e2c-4a7d-a27f-f7a1ca9efa13",
         "config": {
             "AdvancedComponent": {
                 "infile": null,
                 "outfile": null,
                 "value1": -1
             },
             "MyComponent": {
@@ -27,82 +27,82 @@
                         "type",
                         "*",
                         5.0
                     ]
                 ]
             }
         },
-        "duration_min": 0.009033333333352545,
+        "duration_min": 0.008883333333411514,
         "input": [],
         "output": [],
         "start": {
-            "time_utc": "2020-05-15T12:25:28.496"
+            "time_utc": "2020-07-24T09:21:40.994"
         },
         "status": "completed",
         "stop": {
-            "time_utc": "2020-05-15T12:25:29.038"
+            "time_utc": "2020-07-24T09:21:41.527"
         },
         "system": {
             "arguments": [
                 "/home/maxnoe/.local/anaconda3/envs/ctapipe/lib/python3.7/site-packages/ipykernel_launcher.py",
                 "-f",
-                "/tmp/tmpcaadij8l.json",
+                "/tmp/tmpaz6gy5fv.json",
                 "--HistoryManager.hist_file=:memory:"
             ],
             "ctapipe_resources_version": "0.3.0",
             "ctapipe_svc_path": null,
-            "ctapipe_version": "0.7.0.post228+git2316979",
+            "ctapipe_version": "0.8.0.post20+git51becae",
             "environment": {
                 "CONDA_DEFAULT_ENV": "ctapipe",
                 "CONDA_EXE": "/home/maxnoe/.local/anaconda3/bin/conda",
                 "CONDA_PREFIX": "/home/maxnoe/.local/anaconda3/envs/ctapipe",
                 "CONDA_PROMPT_MODIFIER": "(ctapipe) ",
                 "CONDA_PYTHON_EXE": "/home/maxnoe/.local/anaconda3/bin/python",
                 "CONDA_SHLVL": "1",
                 "DYLD_LIBRARY_PATH": null,
                 "HOME": "/home/maxnoe",
                 "LD_LIBRARY_PATH": null,
-                "PATH": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.local/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/anaconda3/condabin:/usr/local/sbin:/usr/local/bin:/usr/bin:/usr/lib/jvm/default/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl",
-                "SHELL": "/bin/bash",
+                "PATH": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/anaconda3/condabin:/home/maxnoe/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/bin:/usr/lib/jvm/default/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl",
+                "SHELL": "/bin/zsh",
                 "USER": "maxnoe"
             },
-            "eventio_version": "1.1.1",
+            "eventio_version": "1.4.1",
             "executable": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin/python",
             "platform": {
                 "architecture_bits": "64bit",
                 "architecture_linkage": "ELF",
-                "boot_time": "2020-05-15T07:53:07.000",
+                "boot_time": "2020-07-24T07:57:22.000",
                 "libcver": [
                     "glibc",
                     "2.10"
                 ],
                 "machine": "x86_64",
                 "node": "max-desktop",
                 "num_cpus": 8,
                 "processor": "",
-                "release": "5.6.12-arch1-1",
+                "release": "5.7.9-arch1-1",
                 "system": "Linux",
-                "version": "#1 SMP PREEMPT Sun, 10 May 2020 10:43:42 +0000"
+                "version": "#1 SMP PREEMPT Thu, 16 Jul 2020 19:34:49 +0000"
             },
             "python": {
                 "compiler": "GCC 7.3.0",
                 "implementation": "CPython",
                 "version": [
                     "3",
                     "7",
                     "7"
                 ],
                 "version_string": "3.7.7 (default, Mar 23 2020, 22:36:06) \n[GCC 7.3.0]"
             },
-            "start_time_utc": "2020-05-15T12:25:28.522"
+            "start_time_utc": "2020-07-24T09:21:41.020"
         }
     },
     {
         "activity_name": "mytool",
-        "activity_uuid": "410c7420-2879-4ba4-bcae-628c03fe03f8",
+        "activity_uuid": "a3d65bc6-5ef2-43af-9f7b-d5d96c343a4d",
         "config": {
             "AdvancedComponent": {
                 "infile": null,
                 "outfile": null,
                 "value1": -1
             },
             "MyComponent": {
@@ -124,82 +124,82 @@
                         "type",
                         "*",
                         5.0
                     ]
                 ]
             }
         },
-        "duration_min": 0.005666666666623854,
+        "duration_min": 0.005533333333449519,
         "input": [],
         "output": [],
         "start": {
-            "time_utc": "2020-05-15T12:25:29.076"
+            "time_utc": "2020-07-24T09:21:41.540"
         },
         "status": "completed",
         "stop": {
-            "time_utc": "2020-05-15T12:25:29.416"
+            "time_utc": "2020-07-24T09:21:41.872"
         },
         "system": {
             "arguments": [
                 "/home/maxnoe/.local/anaconda3/envs/ctapipe/lib/python3.7/site-packages/ipykernel_launcher.py",
                 "-f",
-                "/tmp/tmpcaadij8l.json",
+                "/tmp/tmpaz6gy5fv.json",
                 "--HistoryManager.hist_file=:memory:"
             ],
             "ctapipe_resources_version": "0.3.0",
             "ctapipe_svc_path": null,
-            "ctapipe_version": "0.7.0.post228+git2316979",
+            "ctapipe_version": "0.8.0.post20+git51becae",
             "environment": {
                 "CONDA_DEFAULT_ENV": "ctapipe",
                 "CONDA_EXE": "/home/maxnoe/.local/anaconda3/bin/conda",
                 "CONDA_PREFIX": "/home/maxnoe/.local/anaconda3/envs/ctapipe",
                 "CONDA_PROMPT_MODIFIER": "(ctapipe) ",
                 "CONDA_PYTHON_EXE": "/home/maxnoe/.local/anaconda3/bin/python",
                 "CONDA_SHLVL": "1",
                 "DYLD_LIBRARY_PATH": null,
                 "HOME": "/home/maxnoe",
                 "LD_LIBRARY_PATH": null,
-                "PATH": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.local/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/anaconda3/condabin:/usr/local/sbin:/usr/local/bin:/usr/bin:/usr/lib/jvm/default/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl",
-                "SHELL": "/bin/bash",
+                "PATH": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/anaconda3/condabin:/home/maxnoe/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/bin:/usr/lib/jvm/default/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl",
+                "SHELL": "/bin/zsh",
                 "USER": "maxnoe"
             },
-            "eventio_version": "1.1.1",
+            "eventio_version": "1.4.1",
             "executable": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin/python",
             "platform": {
                 "architecture_bits": "64bit",
                 "architecture_linkage": "ELF",
-                "boot_time": "2020-05-15T07:53:07.000",
+                "boot_time": "2020-07-24T07:57:22.000",
                 "libcver": [
                     "glibc",
                     "2.10"
                 ],
                 "machine": "x86_64",
                 "node": "max-desktop",
                 "num_cpus": 8,
                 "processor": "",
-                "release": "5.6.12-arch1-1",
+                "release": "5.7.9-arch1-1",
                 "system": "Linux",
-                "version": "#1 SMP PREEMPT Sun, 10 May 2020 10:43:42 +0000"
+                "version": "#1 SMP PREEMPT Thu, 16 Jul 2020 19:34:49 +0000"
             },
             "python": {
                 "compiler": "GCC 7.3.0",
                 "implementation": "CPython",
                 "version": [
                     "3",
                     "7",
                     "7"
                 ],
                 "version_string": "3.7.7 (default, Mar 23 2020, 22:36:06) \n[GCC 7.3.0]"
             },
-            "start_time_utc": "2020-05-15T12:25:29.104"
+            "start_time_utc": "2020-07-24T09:21:41.566"
         }
     },
     {
         "activity_name": "mytool",
-        "activity_uuid": "c65f7de6-2888-429f-af01-f07df9557c44",
+        "activity_uuid": "5fe66c58-6543-43df-9bb1-8c293219ad42",
         "config": {
             "AdvancedComponent": {
                 "infile": null,
                 "outfile": null,
                 "value1": -1
             },
             "MyComponent": {
@@ -221,82 +221,82 @@
                         "type",
                         "*",
                         5.0
                     ]
                 ]
             }
         },
-        "duration_min": 0.005983333333432483,
+        "duration_min": 0.005583333333269991,
         "input": [],
         "output": [],
         "start": {
-            "time_utc": "2020-05-15T12:25:29.471"
+            "time_utc": "2020-07-24T09:21:41.886"
         },
         "status": "completed",
         "stop": {
-            "time_utc": "2020-05-15T12:25:29.830"
+            "time_utc": "2020-07-24T09:21:42.221"
         },
         "system": {
             "arguments": [
                 "/home/maxnoe/.local/anaconda3/envs/ctapipe/lib/python3.7/site-packages/ipykernel_launcher.py",
                 "-f",
-                "/tmp/tmpcaadij8l.json",
+                "/tmp/tmpaz6gy5fv.json",
                 "--HistoryManager.hist_file=:memory:"
             ],
             "ctapipe_resources_version": "0.3.0",
             "ctapipe_svc_path": null,
-            "ctapipe_version": "0.7.0.post228+git2316979",
+            "ctapipe_version": "0.8.0.post20+git51becae",
             "environment": {
                 "CONDA_DEFAULT_ENV": "ctapipe",
                 "CONDA_EXE": "/home/maxnoe/.local/anaconda3/bin/conda",
                 "CONDA_PREFIX": "/home/maxnoe/.local/anaconda3/envs/ctapipe",
                 "CONDA_PROMPT_MODIFIER": "(ctapipe) ",
                 "CONDA_PYTHON_EXE": "/home/maxnoe/.local/anaconda3/bin/python",
                 "CONDA_SHLVL": "1",
                 "DYLD_LIBRARY_PATH": null,
                 "HOME": "/home/maxnoe",
                 "LD_LIBRARY_PATH": null,
-                "PATH": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.local/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/anaconda3/condabin:/usr/local/sbin:/usr/local/bin:/usr/bin:/usr/lib/jvm/default/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl",
-                "SHELL": "/bin/bash",
+                "PATH": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/anaconda3/condabin:/home/maxnoe/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/bin:/usr/lib/jvm/default/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl",
+                "SHELL": "/bin/zsh",
                 "USER": "maxnoe"
             },
-            "eventio_version": "1.1.1",
+            "eventio_version": "1.4.1",
             "executable": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin/python",
             "platform": {
                 "architecture_bits": "64bit",
                 "architecture_linkage": "ELF",
-                "boot_time": "2020-05-15T07:53:07.000",
+                "boot_time": "2020-07-24T07:57:22.000",
                 "libcver": [
                     "glibc",
                     "2.10"
                 ],
                 "machine": "x86_64",
                 "node": "max-desktop",
                 "num_cpus": 8,
                 "processor": "",
-                "release": "5.6.12-arch1-1",
+                "release": "5.7.9-arch1-1",
                 "system": "Linux",
-                "version": "#1 SMP PREEMPT Sun, 10 May 2020 10:43:42 +0000"
+                "version": "#1 SMP PREEMPT Thu, 16 Jul 2020 19:34:49 +0000"
             },
             "python": {
                 "compiler": "GCC 7.3.0",
                 "implementation": "CPython",
                 "version": [
                     "3",
                     "7",
                     "7"
                 ],
                 "version_string": "3.7.7 (default, Mar 23 2020, 22:36:06) \n[GCC 7.3.0]"
             },
-            "start_time_utc": "2020-05-15T12:25:29.513"
+            "start_time_utc": "2020-07-24T09:21:41.912"
         }
     },
     {
         "activity_name": "mytool",
-        "activity_uuid": "b8994f69-4c79-461b-8a23-37de80ce4ad7",
+        "activity_uuid": "45c06fe6-670e-414c-83fb-8ca46439b7f4",
         "config": {
             "AdvancedComponent": {
                 "infile": null,
                 "outfile": null,
                 "value1": -1
             },
             "MyComponent": {
@@ -318,82 +318,82 @@
                         "type",
                         "*",
                         5.0
                     ]
                 ]
             }
         },
-        "duration_min": 0.005816666666724757,
+        "duration_min": 0.005583333333269991,
         "input": [],
         "output": [],
         "start": {
-            "time_utc": "2020-05-15T12:25:29.856"
+            "time_utc": "2020-07-24T09:21:42.240"
         },
         "status": "completed",
         "stop": {
-            "time_utc": "2020-05-15T12:25:30.205"
+            "time_utc": "2020-07-24T09:21:42.575"
         },
         "system": {
             "arguments": [
                 "/home/maxnoe/.local/anaconda3/envs/ctapipe/lib/python3.7/site-packages/ipykernel_launcher.py",
                 "-f",
-                "/tmp/tmpcaadij8l.json",
+                "/tmp/tmpaz6gy5fv.json",
                 "--HistoryManager.hist_file=:memory:"
             ],
             "ctapipe_resources_version": "0.3.0",
             "ctapipe_svc_path": null,
-            "ctapipe_version": "0.7.0.post228+git2316979",
+            "ctapipe_version": "0.8.0.post20+git51becae",
             "environment": {
                 "CONDA_DEFAULT_ENV": "ctapipe",
                 "CONDA_EXE": "/home/maxnoe/.local/anaconda3/bin/conda",
                 "CONDA_PREFIX": "/home/maxnoe/.local/anaconda3/envs/ctapipe",
                 "CONDA_PROMPT_MODIFIER": "(ctapipe) ",
                 "CONDA_PYTHON_EXE": "/home/maxnoe/.local/anaconda3/bin/python",
                 "CONDA_SHLVL": "1",
                 "DYLD_LIBRARY_PATH": null,
                 "HOME": "/home/maxnoe",
                 "LD_LIBRARY_PATH": null,
-                "PATH": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.local/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/anaconda3/condabin:/usr/local/sbin:/usr/local/bin:/usr/bin:/usr/lib/jvm/default/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl",
-                "SHELL": "/bin/bash",
+                "PATH": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/anaconda3/condabin:/home/maxnoe/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/bin:/usr/lib/jvm/default/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl",
+                "SHELL": "/bin/zsh",
                 "USER": "maxnoe"
             },
-            "eventio_version": "1.1.1",
+            "eventio_version": "1.4.1",
             "executable": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin/python",
             "platform": {
                 "architecture_bits": "64bit",
                 "architecture_linkage": "ELF",
-                "boot_time": "2020-05-15T07:53:07.000",
+                "boot_time": "2020-07-24T07:57:22.000",
                 "libcver": [
                     "glibc",
                     "2.10"
                 ],
                 "machine": "x86_64",
                 "node": "max-desktop",
                 "num_cpus": 8,
                 "processor": "",
-                "release": "5.6.12-arch1-1",
+                "release": "5.7.9-arch1-1",
                 "system": "Linux",
-                "version": "#1 SMP PREEMPT Sun, 10 May 2020 10:43:42 +0000"
+                "version": "#1 SMP PREEMPT Thu, 16 Jul 2020 19:34:49 +0000"
             },
             "python": {
                 "compiler": "GCC 7.3.0",
                 "implementation": "CPython",
                 "version": [
                     "3",
                     "7",
                     "7"
                 ],
                 "version_string": "3.7.7 (default, Mar 23 2020, 22:36:06) \n[GCC 7.3.0]"
             },
-            "start_time_utc": "2020-05-15T12:25:29.894"
+            "start_time_utc": "2020-07-24T09:21:42.266"
         }
     },
     {
         "activity_name": "mytool",
-        "activity_uuid": "6f444821-e49e-4492-bdaf-20855bc157f6",
+        "activity_uuid": "c6caed62-c837-4558-aaec-40f33655e9e4",
         "config": {
             "AdvancedComponent": {
                 "infile": null,
                 "outfile": null,
                 "value1": -1
             },
             "MyComponent": {
@@ -415,73 +415,73 @@
                         "type",
                         "*",
                         5.0
                     ]
                 ]
             }
         },
-        "duration_min": 0.009150000000079928,
+        "duration_min": 0.008966666666765377,
         "input": [],
         "output": [],
         "start": {
-            "time_utc": "2020-05-15T12:25:30.244"
+            "time_utc": "2020-07-24T09:21:42.608"
         },
         "status": "completed",
         "stop": {
-            "time_utc": "2020-05-15T12:25:30.793"
+            "time_utc": "2020-07-24T09:21:43.146"
         },
         "system": {
             "arguments": [
                 "/home/maxnoe/.local/anaconda3/envs/ctapipe/lib/python3.7/site-packages/ipykernel_launcher.py",
                 "-f",
-                "/tmp/tmpcaadij8l.json",
+                "/tmp/tmpaz6gy5fv.json",
                 "--HistoryManager.hist_file=:memory:"
             ],
             "ctapipe_resources_version": "0.3.0",
             "ctapipe_svc_path": null,
-            "ctapipe_version": "0.7.0.post228+git2316979",
+            "ctapipe_version": "0.8.0.post20+git51becae",
             "environment": {
                 "CONDA_DEFAULT_ENV": "ctapipe",
                 "CONDA_EXE": "/home/maxnoe/.local/anaconda3/bin/conda",
                 "CONDA_PREFIX": "/home/maxnoe/.local/anaconda3/envs/ctapipe",
                 "CONDA_PROMPT_MODIFIER": "(ctapipe) ",
                 "CONDA_PYTHON_EXE": "/home/maxnoe/.local/anaconda3/bin/python",
                 "CONDA_SHLVL": "1",
                 "DYLD_LIBRARY_PATH": null,
                 "HOME": "/home/maxnoe",
                 "LD_LIBRARY_PATH": null,
-                "PATH": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.local/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/anaconda3/condabin:/usr/local/sbin:/usr/local/bin:/usr/bin:/usr/lib/jvm/default/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl",
-                "SHELL": "/bin/bash",
+                "PATH": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/bin:/home/maxnoe/.local/texlive/2020/bin/x86_64-linux:/home/maxnoe/.local/go/bin:/home/maxnoe/.local/bin:/home/maxnoe/.gem/ruby/2.7.0/bin:/home/maxnoe/.pyenv/shims:/home/maxnoe/.local/anaconda3/condabin:/home/maxnoe/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/bin:/usr/lib/jvm/default/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl",
+                "SHELL": "/bin/zsh",
                 "USER": "maxnoe"
             },
-            "eventio_version": "1.1.1",
+            "eventio_version": "1.4.1",
             "executable": "/home/maxnoe/.local/anaconda3/envs/ctapipe/bin/python",
             "platform": {
                 "architecture_bits": "64bit",
                 "architecture_linkage": "ELF",
-                "boot_time": "2020-05-15T07:53:07.000",
+                "boot_time": "2020-07-24T07:57:22.000",
                 "libcver": [
                     "glibc",
                     "2.10"
                 ],
                 "machine": "x86_64",
                 "node": "max-desktop",
                 "num_cpus": 8,
                 "processor": "",
-                "release": "5.6.12-arch1-1",
+                "release": "5.7.9-arch1-1",
                 "system": "Linux",
-                "version": "#1 SMP PREEMPT Sun, 10 May 2020 10:43:42 +0000"
+                "version": "#1 SMP PREEMPT Thu, 16 Jul 2020 19:34:49 +0000"
             },
             "python": {
                 "compiler": "GCC 7.3.0",
                 "implementation": "CPython",
                 "version": [
                     "3",
                     "7",
                     "7"
                 ],
                 "version_string": "3.7.7 (default, Mar 23 2020, 22:36:06) \n[GCC 7.3.0]"
             },
-            "start_time_utc": "2020-05-15T12:25:30.269"
+            "start_time_utc": "2020-07-24T09:21:42.634"
         }
     }
 ]
```

### Comparing `ctapipe-0.8.0/docs/examples/table_writer_reader.ipynb` & `ctapipe-0.9.1/docs/examples/table_writer_reader.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/getting_started/index.rst` & `ctapipe-0.9.1/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/index.html` & `ctapipe-0.9.1/docs/index.html`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/index.rst` & `ctapipe-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/make.bat` & `ctapipe-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/calibrated_data_exploration-checkpoint.ipynb` & `ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/calibrated_data_exploration-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/coordinates_example-checkpoint.ipynb` & `ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/coordinates_example-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/ctapipe_handson-checkpoint.ipynb` & `ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/ctapipe_handson-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/lst_analysis_bootcamp_2018-checkpoint.ipynb` & `ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/lst_analysis_bootcamp_2018-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/raw_data_exploration-checkpoint.ipynb` & `ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/raw_data_exploration-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/.ipynb_checkpoints/theta_square-checkpoint.ipynb` & `ctapipe-0.9.1/docs/tutorials/.ipynb_checkpoints/theta_square-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/calibrated_data_exploration.ipynb` & `ctapipe-0.9.1/docs/tutorials/calibrated_data_exploration.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/coordinates_example.ipynb` & `ctapipe-0.9.1/docs/tutorials/coordinates_example.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/ctapipe_handson.ipynb` & `ctapipe-0.9.1/docs/tutorials/ctapipe_handson.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/ground_frame.png` & `ctapipe-0.9.1/docs/tutorials/ground_frame.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/hillas.h5` & `ctapipe-0.9.1/docs/tutorials/hillas.h5`

 * *Command `'h5dump {}'` failed with exit code 1. Standard output:*

 * *    h5dump error: unable to print data*

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 8948 4446 0d0a 1a0a 0000 0000 0008 0800  .HDF............
 00000010: 0400 1000 0000 0000 0000 0000 0000 0000  ................
-00000020: ffff ffff ffff ffff 9153 0000 0000 0000  .........S......
+00000020: ffff ffff ffff ffff d451 0000 0000 0000  .........Q......
 00000030: ffff ffff ffff ffff 0000 0000 0000 0000  ................
 00000040: 6000 0000 0000 0000 0100 0000 0000 0000  `...............
 00000050: 8800 0000 0000 0000 a802 0000 0000 0000  ................
 00000060: 0100 0700 0100 0000 1800 0000 0000 0000  ................
 00000070: 1000 1000 0000 0000 2003 0000 0000 0000  ........ .......
 00000080: 1801 0000 0000 0000 5452 4545 0000 0100  ........TREE....
 00000090: ffff ffff ffff ffff ffff ffff ffff ffff  ................
@@ -141,16 +141,16 @@
 000008c0: 5645 5253 494f 4e00 1310 0000 0300 0000  VERSION.........
 000008d0: 0100 0000 0000 0000 312e 3000 0000 0000  ........1.0.....
 000008e0: 0c00 3000 0000 0000 0100 0800 0c00 0800  ..0.............
 000008f0: 4649 4c54 4552 5300 1008 0000 0800 0000  FILTERS.........
 00000900: 0000 4000 0000 0000 0100 0000 0000 0000  ..@.............
 00000910: 050a 0300 0000 0000 0100 5900 0100 0000  ..........Y.....
 00000920: 4008 0000 0000 0000 1000 1000 0000 0000  @...............
-00000930: b012 0000 0000 0000 6814 0000 0000 0000  ........h.......
-00000940: 0300 8007 0100 0000 161e 0000 ec00 0000  ................
+00000930: b012 0000 0000 0000 5814 0000 0000 0000  ........X.......
+00000940: 0300 8007 0100 0000 161e 0000 e400 0000  ................
 00000950: 6576 656e 745f 6964 0000 0000 0000 0000  event_id........
 00000960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000980: 1008 0000 0800 0000 0000 4000 6f62 735f  ..........@.obs_
 00000990: 6964 0000 0800 0000 0000 0000 0000 0000  id..............
 000009a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000009b0: 0000 0000 1008 0000 0400 0000 0000 2000  .............. .
@@ -235,51 +235,51 @@
 00000ea0: 7069 7865 6c73 5f77 6964 7468 5f32 0000  pixels_width_2..
 00000eb0: ac00 0000 0000 0000 0000 0000 0000 0000  ................
 00000ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ed0: 1120 3f00 0800 0000 0000 4000 340b 0034  . ?.......@.4..4
 00000ee0: ff03 0000 696e 7465 6e73 6974 795f 7769  ....intensity_wi
 00000ef0: 6474 685f 3100 0000 0000 0000 b400 0000  dth_1...........
 00000f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f10: 0000 0000 0000 0000 0000 0000 1120 3f00  ............. ?.
-00000f20: 0800 0000 0000 4000 340b 0034 ff03 0000  ......@.4..4....
+00000f10: 0000 0000 0000 0000 0000 0000 1120 1f00  ............. ..
+00000f20: 0400 0000 0000 2000 1708 0017 7f00 0000  ...... .........
 00000f30: 696e 7465 6e73 6974 795f 7769 6474 685f  intensity_width_
-00000f40: 3200 0000 0000 0000 bc00 0000 0000 0000  2...............
+00000f40: 3200 0000 0000 0000 b800 0000 0000 0000  2...............
 00000f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f60: 0000 0000 0000 0000 1120 3f00 0800 0000  ......... ?.....
-00000f70: 0000 4000 340b 0034 ff03 0000 736c 6f70  ..@.4..4....slop
-00000f80: 6500 0000 c400 0000 0000 0000 0000 0000  e...............
+00000f60: 0000 0000 0000 0000 1120 1f00 0400 0000  ......... ......
+00000f70: 0000 2000 1708 0017 7f00 0000 736c 6f70  .. .........slop
+00000f80: 6500 0000 bc00 0000 0000 0000 0000 0000  e...............
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 1120 3f00 0800 0000 0000 4000  ..... ?.......@.
 00000fb0: 340b 0034 ff03 0000 736c 6f70 655f 6572  4..4....slope_er
-00000fc0: 7200 0000 0000 0000 cc00 0000 0000 0000  r...............
+00000fc0: 7200 0000 0000 0000 c400 0000 0000 0000  r...............
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 1120 3f00 0800 0000  ......... ?.....
 00000ff0: 0000 4000 340b 0034 ff03 0000 696e 7465  ..@.4..4....inte
-00001000: 7263 6570 7400 0000 0000 0000 d400 0000  rcept...........
+00001000: 7263 6570 7400 0000 0000 0000 cc00 0000  rcept...........
 00001010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001020: 0000 0000 0000 0000 0000 0000 1120 3f00  ............. ?.
 00001030: 0800 0000 0000 4000 340b 0034 ff03 0000  ......@.4..4....
 00001040: 696e 7465 7263 6570 745f 6572 7200 0000  intercept_err...
-00001050: dc00 0000 0000 0000 0000 0000 0000 0000  ................
+00001050: d400 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 1120 3f00 0800 0000 0000 4000 340b 0034  . ?.......@.4..4
 00001080: ff03 0000 6465 7669 6174 696f 6e00 0000  ....deviation...
-00001090: 0000 0000 e400 0000 0000 0000 0000 0000  ................
+00001090: 0000 0000 dc00 0000 0000 0000 0000 0000  ................
 000010a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010b0: 0000 0000 1120 3f00 0800 0000 0000 4000  ..... ?.......@.
 000010c0: 340b 0034 ff03 0000 0500 0800 0100 0000  4..4............
 000010d0: 0203 0001 0000 0000 0b00 5000 0100 0000  ..........P.....
 000010e0: 0102 0000 0000 0000 0300 1000 0000 0000  ................
 000010f0: 666c 6574 6368 6572 3332 0000 0000 0000  fletcher32......
 00001100: 017d 0800 0100 0700 626c 6f73 6300 0000  .}......blosc...
-00001110: 0200 0000 0200 0000 ec00 0000 5cff 0000  ............\...
+00001110: 0200 0000 0200 0000 e400 0000 9cff 0000  ................
 00001120: 0500 0000 0100 0000 0500 0000 0000 0000  ................
-00001130: 0800 1800 0000 0000 0302 0218 2700 0000  ............'...
-00001140: 0000 0015 0100 00ec 0000 0000 0000 0000  ................
-00001150: 1200 0800 0000 0000 0100 0000 a48a be5e  ...............^
+00001130: 0800 1800 0000 0000 0302 0208 2700 0000  ............'...
+00001140: 0000 001f 0100 00e4 0000 0000 0000 0000  ................
+00001150: 1200 0800 0000 0000 0100 0000 90a8 1a5f  ..............._
 00001160: 0000 0000 0000 0000 534e 4f44 0100 0100  ........SNOD....
 00001170: 0800 0000 0000 0000 1809 0000 0000 0000  ................
 00001180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -526,21 +526,21 @@
 000020d0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 000020e0: 0c00 4000 0000 0000 0100 0e00 1400 0800  ..@.............
 000020f0: 4649 454c 445f 3232 5f46 494c 4c00 0000  FIELD_22_FILL...
 00002100: 1120 3f00 0800 0000 0000 4000 340b 0034  . ?.......@.4..4
 00002110: ff03 0000 0000 0000 0100 0000 0000 0000  ................
 00002120: 0000 0000 0000 0000 0c00 4000 0000 0000  ..........@.....
 00002130: 0100 0e00 1400 0800 4649 454c 445f 3233  ........FIELD_23
-00002140: 5f46 494c 4c00 0000 1120 3f00 0800 0000  _FILL.... ?.....
-00002150: 0000 4000 340b 0034 ff03 0000 0000 0000  ..@.4..4........
+00002140: 5f46 494c 4c00 0000 1120 1f00 0400 0000  _FILL.... ......
+00002150: 0000 2000 1708 0017 7f00 0000 0000 0000  .. .............
 00002160: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 00002170: 0c00 4000 0000 0000 0100 0e00 1400 0800  ..@.............
 00002180: 4649 454c 445f 3234 5f46 494c 4c00 0000  FIELD_24_FILL...
-00002190: 1120 3f00 0800 0000 0000 4000 340b 0034  . ?.......@.4..4
-000021a0: ff03 0000 0000 0000 0100 0000 0000 0000  ................
+00002190: 1120 1f00 0400 0000 0000 2000 1708 0017  . ........ .....
+000021a0: 7f00 0000 0000 0000 0100 0000 0000 0000  ................
 000021b0: 0000 0000 0000 0000 0c00 4000 0000 0000  ..........@.....
 000021c0: 0100 0e00 1400 0800 4649 454c 445f 3235  ........FIELD_25
 000021d0: 5f46 494c 4c00 0000 1120 3f00 0800 0000  _FILL.... ?.....
 000021e0: 0000 4000 340b 0034 ff03 0000 0000 0000  ..@.4..4........
 000021f0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 00002200: 0c00 4000 0000 0000 0100 0e00 1400 0800  ..@.............
 00002210: 4649 454c 445f 3236 5f46 494c 4c00 0000  FIELD_26_FILL...
@@ -579,16 +579,16 @@
 00002420: 0100 0000 0000 0000 6d00 0000 0000 0000  ........m.......
 00002430: 0c00 3800 0000 0000 0100 1100 0800 0800  ..8.............
 00002440: 685f 6669 7273 745f 696e 745f 554e 4954  h_first_int_UNIT
 00002450: 0000 0000 0000 0000 1310 0000 0100 0000  ................
 00002460: 0100 0000 0000 0000 6d00 0000 0000 0000  ........m.......
 00002470: 0c00 3000 0000 0000 0100 0b00 0800 0800  ..0.............
 00002480: 785f 6d61 785f 554e 4954 0000 0000 0000  x_max_UNIT......
-00002490: 1310 0000 0700 0000 0100 0000 0000 0000  ................
-000024a0: 6720 2f20 636d 3200 0c00 2800 0000 0000  g / cm2...(.....
+00002490: 1310 0000 0600 0000 0100 0000 0000 0000  ................
+000024a0: 636d 2d32 2067 0000 0c00 2800 0000 0000  cm-2 g....(.....
 000024b0: 0100 0700 0800 0800 785f 554e 4954 0000  ........x_UNIT..
 000024c0: 1310 0000 0100 0000 0100 0000 0000 0000  ................
 000024d0: 6d00 0000 0000 0000 0c00 2800 0000 0000  m.........(.....
 000024e0: 0100 0700 0800 0800 795f 554e 4954 0000  ........y_UNIT..
 000024f0: 1310 0000 0100 0000 0100 0000 0000 0000  ................
 00002500: 6d00 0000 0000 0000 0c00 2800 0000 0000  m.........(.....
 00002510: 0100 0700 0800 0800 725f 554e 4954 0000  ........r_UNIT..
@@ -603,36 +603,36 @@
 000025a0: 6d00 0000 0000 0000 0c00 3000 0000 0000  m.........0.....
 000025b0: 0100 0b00 0800 0800 7769 6474 685f 554e  ........width_UN
 000025c0: 4954 0000 0000 0000 1310 0000 0100 0000  IT..............
 000025d0: 0100 0000 0000 0000 6d00 0000 0000 0000  ........m.......
 000025e0: 0c00 3000 0000 0000 0100 0900 0800 0800  ..0.............
 000025f0: 7073 695f 554e 4954 0000 0000 0000 0000  psi_UNIT........
 00002600: 1310 0000 0300 0000 0100 0000 0000 0000  ................
-00002610: 6465 6700 0000 0000 0c00 3800 0000 0000  deg.......8.....
+00002610: 6465 6700 0000 0000 0c00 3000 0000 0000  deg.......0.....
 00002620: 0100 0b00 0800 0800 736c 6f70 655f 554e  ........slope_UN
-00002630: 4954 0000 0000 0000 1310 0000 0900 0000  IT..............
-00002640: 0100 0000 0000 0000 312e 3020 3120 2f20  ........1.0 1 / 
-00002650: 6d00 0000 0000 0000 0c00 3800 0000 0000  m.........8.....
-00002660: 0100 0f00 0800 0800 736c 6f70 655f 6572  ........slope_er
-00002670: 725f 554e 4954 0000 1310 0000 0900 0000  r_UNIT..........
-00002680: 0100 0000 0000 0000 312e 3020 3120 2f20  ........1.0 1 / 
-00002690: 6d00 0000 0000 0000 0c00 4000 0000 0000  m.........@.....
-000026a0: 0100 1000 0800 0800 4354 4150 4950 455f  ........CTAPIPE_
-000026b0: 5645 5253 494f 4e00 1310 0000 1800 0000  VERSION.........
-000026c0: 0100 0000 0000 0000 302e 372e 302e 706f  ........0.7.0.po
-000026d0: 7374 3232 382b 6769 7432 3331 3639 3739  st228+git2316979
-000026e0: 0c00 3000 0000 0000 0100 0600 0c00 0800  ..0.............
-000026f0: 4e52 4f57 5300 0000 1008 0000 0800 0000  NROWS...........
-00002700: 0000 4000 0000 0000 0100 0000 0000 0000  ..@.............
-00002710: 3500 0000 0000 0000 5452 4545 0100 0100  5.......TREE....
-00002720: ffff ffff ffff ffff ffff ffff ffff ffff  ................
-00002730: 4924 0000 0000 0000 0000 0000 0000 0000  I$..............
-00002740: 0000 0000 0000 0000 482f 0000 0000 0000  ........H/......
-00002750: 0000 0000 0000 0000 1501 0000 0000 0000  ................
-00002760: ec00 0000 0000 0000 0000 0000 0000 0000  ................
+00002630: 4954 0000 0000 0000 1310 0000 0300 0000  IT..............
+00002640: 0100 0000 0000 0000 6d2d 3100 0000 0000  ........m-1.....
+00002650: 0c00 3000 0000 0000 0100 0f00 0800 0800  ..0.............
+00002660: 736c 6f70 655f 6572 725f 554e 4954 0000  slope_err_UNIT..
+00002670: 1310 0000 0300 0000 0100 0000 0000 0000  ................
+00002680: 6d2d 3100 0000 0000 0c00 4000 0000 0000  m-1.......@.....
+00002690: 0100 1000 0800 0800 4354 4150 4950 455f  ........CTAPIPE_
+000026a0: 5645 5253 494f 4e00 1310 0000 1700 0000  VERSION.........
+000026b0: 0100 0000 0000 0000 302e 382e 302e 706f  ........0.8.0.po
+000026c0: 7374 3230 2b67 6974 3531 6265 6361 6500  st20+git51becae.
+000026d0: 0c00 3000 0000 0000 0100 0600 0c00 0800  ..0.............
+000026e0: 4e52 4f57 5300 0000 1008 0000 0800 0000  NROWS...........
+000026f0: 0000 4000 0000 0000 0100 0000 0000 0000  ..@.............
+00002700: 3500 0000 0000 0000 5452 4545 0100 0100  5.......TREE....
+00002710: ffff ffff ffff ffff ffff ffff ffff ffff  ................
+00002720: 9c22 0000 0000 0000 0000 0000 0000 0000  ."..............
+00002730: 0000 0000 0000 0000 382f 0000 0000 0000  ........8/......
+00002740: 0000 0000 0000 0000 1f01 0000 0000 0000  ................
+00002750: e400 0000 0000 0000 0000 0000 0000 0000  ................
+00002760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000027a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000027b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000027c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000027d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -749,590 +749,562 @@
 00002ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f40: 0000 0000 0000 0000 0201 91ec 60ff 0000  ............`...
-00002f50: 5cff 0000 4924 0000 1800 0000 4124 0000  \...I$......A$..
-00002f60: 2524 0000 28b5 2ffd 605c fedd 2001 ccf9  %$..(./.`\.. ...
-00002f70: 0124 2422 220e 2121 2121 fafa fa48 48f3  .$$"".!!!!...HH.
-00002f80: f3be 13e3 d4c0 1717 1717 e2e2 e200 0000  ................
-00002f90: 00c4 c4c4 3131 3162 6262 d8d8 cab2 b2b2  ....111bbb......
-00002fa0: b2a8 a0eb ebeb 0079 7963 6358 f1f1 f1f1  .......yyccX....
-00002fb0: 6363 639d 9dcf cfa2 aeeb 3911 4646 4646  ccc.......9.FFFF
-00002fc0: 6f6f 6f5b 5b5b 5b86 8686 3d3d 3dbc bcbc  ooo[[[[...===...
-00002fd0: 9292 9deb ebeb eb2f 95a4 a4a4 0001 0102  ......./........
-00002fe0: 0303 0304 0405 0507 0709 0b0d 0e0f 0f0f  ................
-00002ff0: 1010 1011 1111 1818 1818 1900 5a00 1d00  ............Z...
-00003000: 0203 0204 0101 0203 0401 0204 0204 0203  ................
-00003010: 0402 0303 0102 0304 0060 6020 2040 8080  .........``  @..
-00003020: 8080 6060 60e0 e0e0 e000 e080 4000 0000  ..```.......@...
-00003030: a0a0 a0a0 c0c0 c000 0000 e0c0 2020 2020  ............    
-00003040: 00e0 ebeb e2e2 e3f7 f7f7 f779 7979 1d1d  ...........yyy..
-00003050: aeae f45f c46b 8832 3232 3264 6464 7373  ..._.k.2222dddss
-00003060: 7373 8989 89eb ebeb 9999 9924 247f e8e8  ss.........$$...
-00003070: e8e8 4fd1 cece ce00 d1d1 f0f0 fde9 e9e9  ..O.............
-00003080: e938 3838 3333 3a3a 6802 d9fa 42c3 c3c3  .88833::h...B...
-00003090: c34e 4e4e d6d6 d6d0 d0d0 b9b9 b905 0578  .NNN...........x
-000030a0: 3636 3636 1dc0 a3a3 a3fd fd90 9084 bebe  6666............
-000030b0: bebe a0a0 a0b4 b4c0 c0ba b4b0 9083 cfcf  ................
-000030c0: cfcf 1515 15da dada daa2 a2a2 9494 94e6  ................
-000030d0: e6e6 acac a0c8 c8c8 c8a3 bcd4 d4d4 3f40  ..............?@
-000030e0: 4040 007e 7e86 86e7 eeee eeee 8b8b 8b66  @@.~~..........f
-000030f0: 6644 4478 2c28 76c7 3939 3939 9b9b 9bae  fDDx,(v.9999....
-00003100: aeae aebc bcbc 9191 919b 9b9b 6a6a 32b8  ............jj2.
-00003110: 997f 7f7f 0033 3319 19e3 6565 6565 6a6a  .....33...eeeejj
-00003120: 6aaf af25 25a5 fea9 fcf7 c5c5 c5dd dddd  j..%%...........
-00003130: b5b5 b517 1717 4444 1c2c 2c2c 2c3b 6360  ......DD.,,,,;c`
-00003140: 6060 0067 6798 98ef 7979 7979 2121 218a  ``.gg...yyyy!!!.
-00003150: 8a7b 7b0e 499c a68d 8585 8585 3939 390c  .{{.I.......999.
-00003160: 0c0c 0cb4 b4b4 e6e6 e6f9 f9f9 4444 7a3c  ............DDz<
-00003170: 3c3c 3c9c 6e14 1414 0093 9357 5743 a1a1  <<<.n......WWC..
-00003180: a190 90a7 a7db b3d4 4e5f e4e4 e4e4 a4a4  ........N_......
-00003190: a41c 1c1c 1c64 6464 1d1d 1d80 8080 c7c7  .....ddd........
-000031a0: 506a 6a6a 6a9a cec3 c3c3 00a7 a747 47cc  Pjjjj........GG.
-000031b0: d8d8 d8d8 d3d3 d369 69d4 d4ef a566 744a  .......ii....ftJ
-000031c0: 3131 3131 9d9d 9d05 0505 b7b7 b785 8585  1111............
-000031d0: dddd 16f6 f6f6 f6e5 97f0 f0f0 1e1e abab  ................
-000031e0: 3cd2 d2d2 d2ef efef 0202 8c8c b232 2d76  <............2-v
-000031f0: aefc fcfc fcc9 c9c9 4c4c 4c4c 2020 20a5  ........LLLL   .
-00003200: a5a5 d3d3 d393 9310 a4a4 a4a4 bf95 5858  ..............XX
-00003210: 5851 5050 5050 5151 0040 00da da33 8282  XQPPPPQQ.@...3..
-00003220: 8282 9696 9691 91da da35 4901 a2a0 1b1b  .........5I.....
-00003230: 1b1b 2e2e 2ee3 e3e3 e397 9797 6363 63d1  ............ccc.
-00003240: d1d1 1a1a e0c2 c2c2 c2d3 d2dd dddd 00af  ................
-00003250: af92 922a 3a3a 3a3a 3f3f 3fce ce5a 5a3b  ...*::::???..ZZ;
-00003260: 85a3 f45a f3f3 f3f3 6868 68e8 e8e8 6161  ...Z....hhh...aa
-00003270: 61f8 f8f8 4545 4438 3838 388c 5392 9292  a...EED8888.S...
-00003280: 00b7 b742 428e 6868 6868 6e6e 6e2d 2d71  ...BB.hhhhnnn--q
-00003290: 7103 239f 49d5 9494 9494 baba ba04 0404  q.#.I...........
-000032a0: 043e 3e3e 8e8e 8e0c 0c0c dddd 64e9 315e  .>>>........d.1^
-000032b0: 5e5e 0014 146e 6eb8 0101 0101 0f0f 0f5e  ^^...nn........^
-000032c0: 5e58 5839 aa9a b3c9 2929 2967 6767 9191  ^XX9....)))ggg..
-000032d0: 91e7 e7e7 1010 67d1 d1d1 d18f ced2 d2d2  ......g.........
-000032e0: 004f 4ffd fd59 2727 2727 4141 41bb bb19  .OO..Y''''AAA...
-000032f0: 197b 60f7 3873 2f2f 2f9b 9b9b 9b18 1818  .{`.8s///.......
-00003300: 9f9f 9fee eeee bbbb 00f8 f8f8 f893 06f7  ................
-00003310: f7f7 0089 89db db54 7b7b 7b7b 7575 7595  .......T{{{{uuu.
-00003320: 9533 33d8 8720 2e5d 7c7c 7c7c 6363 63e1  .33.. .]||||ccc.
-00003330: e1e1 7c7c 7c4d 4d4d 8686 5a49 4949 4915  ..|||MMM..ZIIII.
-00003340: 117b 7b7b 0019 1908 0805 7618 1876 7610  .{{{......v..vv.
-00003350: 1021 2121 7575 7575 f1f1 f176 7676 2323  .!!!uuuu...vvv##
-00003360: 231c 1c04 7676 7600 4000 8020 8080 2020  #...vvv.@.. ..  
-00003370: c080 4080 2040 4040 8080 00a0 a06a 6a57  ..@. @@@.....jjW
-00003380: 57fe 0909 0909 9292 92ff ffa2 a291 8df7  W...............
-00003390: 6898 4747 4747 5151 5197 9797 6060 601f  h.GGGGQQQ...```.
-000033a0: 1f1f bcbc 011f 1f1f 1f7c bad1 d1d1 d6d6  .........|......
-000033b0: 7575 c377 7777 7775 7575 1e1e afaf d45d  uu.wwwwuuu.....]
-000033c0: 390a 66c7 c7c7 6363 6363 5b5b 5b1f 1f1f  9.f...cccc[[[...
-000033d0: 0808 08ac ac87 4848 4848 ffcc 0202 0200  ......HHHH......
-000033e0: 4949 5c5c 4925 2525 6868 3838 6f5f 4431  II\\I%%%hh88o_D1
-000033f0: 524a 4a4a 4a75 7575 5d5d 5d5d 6464 64e2  RJJJJuuu]]]]ddd.
-00003400: e2e2 7474 7442 426c 4b4b 4b4b 4952 6868  ..tttBBlKKKKIRhh
-00003410: 6800 4040 c040 c0c0 4000 00e0 80c0 0060  h.@@.@..@......`
-00003420: 8080 8080 c0c0 a0a0 c0e0 dbdb 0101 2aab  ..............*.
-00003430: abab ab6b 6b6b 4f4f 8383 d670 40cf 2327  ...kkkOO...p@.#'
-00003440: 2727 6c6c 6c6c 7878 788a 8a8a 9191 916c  ''llllxxx......l
-00003450: 6ca9 7272 7272 99b7 5c5c 5c00 6969 cbcb  l.rrrr..\\\.ii..
-00003460: b036 3636 5454 2e2e 104c ed4d 10fa fafa  .666TT...L.M....
-00003470: faef efef 0f0f 0f0f 7676 7663 6363 2121  ........vvvccc!!
-00003480: 21a6 a66e c1c1 c1c1 9e8f 1c1c 1c51 5161  !..n.........QQa
-00003490: 615a 5353 5353 4c4c 4c56 5668 6857 622a  aZSSSSLLLVVhhWb*
-000034a0: 645f 6262 6243 4343 6666 666a 6a6a 6c6c  d_bbbCCCfffjjjll
-000034b0: 4a55 5555 554d 7269 6969 0040 00a0 8080  JUUUUMriii.@....
-000034c0: e0c0 a080 c0c0 c0a0 a000 80ee ee06 0624  ...............$
-000034d0: 2222 2222 9595 9574 7447 47e7 cefd b2db  """"...ttGG.....
-000034e0: 2929 2929 2020 208e 8e8e 8e54 5454 5d5d  ))))   ....TTT]]
-000034f0: 5d40 4040 d5d5 8f87 8787 8791 d295 9595  ]@@@............
-00003500: bebe d0d0 5cbb bbbb bbda dada 4444 7c7c  ....\.......DD||
-00003510: 73d3 bd22 a255 5555 9090 9028 2828 8484  s..".UUU...(((..
-00003520: 84ff ffc2 1a1a 1a1a 1631 3030 3000 d1d1  .........1000...
-00003530: cece d3d7 d7d7 d7d0 d0d0 dada e4e4 e9d5  ................
-00003540: d5cb cddc dcdc dcd3 d3d3 e2e2 e2e2 e0e0  ................
-00003550: e0d8 d8d8 dfdf dfcc ccd7 d4da 40a0 e0a0  ............@...
-00003560: e0e0 e080 6000 9d9d 7474 8eec ecec ecaa  ....`...tt......
-00003570: aaaa 0000 6262 0000 aa50 8b42 4242 0000  ....bb...P.BBB..
-00003580: 002b 2b2b 4949 aa61 6161 6128 00b8 b811  .+++II.aaaa(....
-00003590: 1123 3232 3248 487a 7ae0 542a be4e 0b0b  .#222HHzz.T*.N..
-000035a0: 4b4b 4ba8 a8a8 dbdb db92 922a ef00 3636  KKK........*..66
-000035b0: 3600 7777 6767 6e66 6666 6675 7575 6c6c  6.wwggnffffuuull
-000035c0: 6161 6570 6c70 706e 6e6e 6e78 7878 7070  aaeplppnnnnxxxpp
-000035d0: 7070 6868 6871 7171 7263 6369 7575 7500  pphhhqqqrcciuuu.
-000035e0: 4000 05cc 7296 d6f2 c158 eb19 b3a8 40a7  @...r....X....@.
-000035f0: 7f5a 582a d4b5 22e2 f9e9 e42c 4298 c36f  .ZX*.."....,B..o
-00003600: 9a88 9c30 433c 9a6c 2662 c2b0 0bed 647f  ...0C<.l&b....d.
-00003610: 3a04 ece2 a469 6400 beae 783e 93f4 aeb9  :....id...x>....
-00003620: c228 24d2 cf71 a53d c5b3 76fe db38 d271  .($..q.=..v..8.q
-00003630: cf84 1d8d 1936 954c aed5 cb69 8d0d 24a0  .....6.L...i..$.
-00003640: e832 bfac 54b1 c021 048b 112c 0a00 5431  .2..T..!...,..T1
-00003650: 042e 44ad 90a2 f1f5 a1a7 6011 746b a7ee  ..D.......`.tk..
-00003660: 8d0f d1b2 7023 108d 30c4 1fee 7dbf 0be2  ....p#..0...}...
-00003670: 27bf 3e71 42c4 0975 1301 3406 eb8d 6764  '.>qB..u..4...gd
-00003680: 8c93 c600 5786 9187 3be0 b06e 84b6 51b9  ....W...;..n..Q.
-00003690: e6ca 7695 528b dee4 b39b da43 306b 9cc3  ..v.R......C0k..
-000036a0: 51f3 2894 f812 c2bf ace9 3149 800a 638c  Q.(.......1I..c.
-000036b0: 14b6 f4b5 431c 1d06 9300 4383 8613 7cd9  ....C.....C...|.
-000036c0: ec0a c527 b897 eef4 c984 a3b3 125f af1d  ...'........._..
-000036d0: 2f82 d330 8a9c df42 ffe8 5c03 e96c b299  /..0...B..\..l..
-000036e0: 69ee 9a52 445b d085 e953 b7b6 e728 8e00  i..RD[...S...(..
-000036f0: b585 b2ac 1154 f915 8ffc 2c35 2b3c cdc7  .....T....,5+<..
-00003700: 09cc eb2b 8afa ba1c 54f0 db44 c298 9cd5  ...+....T..D....
-00003710: 1aa2 88d0 56f2 7df9 7122 9061 5a2c 0ecb  ....V.}.q".aZ,..
-00003720: 2b2d 3100 8400 7dd7 535b 5360 704e 5366  +-1...}.S[S`pNSf
-00003730: 6864 5562 7e51 5880 6045 5672 9a66 72ad  hdUb~QX.`EVr.fr.
-00003740: 80bb 8070 7889 5e5b 5b49 624f 5f56 8361  ...px.^[[IbO_V.a
-00003750: 5262 8991 9296 5a5c 844a 7f00 4000 d85a  Rb....Z\.J..@..Z
-00003760: c983 394f 8714 8cef 0533 6edf 1a29 162c  ..9O.....3n..).,
-00003770: 4076 b850 884c b788 3f4d 84bb 1faa 3a19  @v.P.L..?M....:.
-00003780: eb4e 24cd fd20 3f0f 42f0 b686 a80e c125  .N$.. ?.B......%
-00003790: df7c 4500 438b 0018 33d2 bf1d 6048 51c9  .|E.C...3...`HQ.
-000037a0: 861c f24d 83b3 a13d 2b9a 6260 df70 84b4  ...M...=+.b`.p..
-000037b0: 0cc3 f75c 995f 122f 6b50 cc48 d10e 0663  ...\._./kP.H...c
-000037c0: b8c6 9e6f 6f0b bb3e db00 85a0 ae0f 3b72  ...oo..>......;r
-000037d0: 1722 cec6 271c aa36 5d10 47f5 8056 15bc  ."..'..6].G..V..
-000037e0: 8a7f c271 8efe c8a8 5411 b526 a25a 8ffc  ...q....T..&.Z..
-000037f0: 6c45 34e8 6cc2 2804 490c f6ec 5bdc f400  lE4.l.(.I...[...
-00003800: 2dce 0dc1 f25c 4f8a cdfb 027b cfa4 b0c5  -....\O....{....
-00003810: c5eb cc29 ce9a 7370 061f 7701 b431 ef3d  ...)..sp..w..1.=
-00003820: 619c 45d0 667a 4ca6 61cc c37a 6799 102e  a.E.fzL.a..zg...
-00003830: 4b0c 653a b000 366e affd 7667 62c4 79ee  K.e:..6n..vgb.y.
-00003840: d2ad fa38 894e 7093 b0fc 84a1 86eb dd68  ...8.Np........h
-00003850: f4aa a7f9 06a9 fc8b d1ae bffc 5635 b0d0  ............V5..
-00003860: 5fd7 0f44 2372 6d0a a475 c700 d261 0ddd  _..D#rm..u...a..
-00003870: 4259 2c9d 54b5 857c 3259 f17b 4cbf ee5b  BY,.T..|2Y.{L..[
-00003880: a1fa eb66 696f 6573 f20f 2952 4f6d 3c8e  ...fioes..)ROm<.
-00003890: 7fbb 1f1a 131d 82e2 d98a adc3 99db 87ca  ................
-000038a0: 4500 eee2 e2d5 ddf0 f0ea f2e7 e8da e2e5  E...............
-000038b0: 84cd e7d5 dfc5 b0e8 e8f0 e0b1 dfb4 b17e  ...............~
-000038c0: cfd6 e1dd e5c9 ddb8 daa4 9da1 d4e6 d8db  ................
-000038d0: e5b5 dbd2 d0db b400 bfbf 3f3f bf3f 3f3f  ..........??.???
-000038e0: 0001 6d5a c715 d569 7aa1 f5b3 778b 7140  ..mZ...iz...w.q@
-000038f0: 6b1f ff7e 7806 10ed 3ce4 9ad0 d4cc 65f3  k..~x...<.....e.
-00003900: 8345 3dda 33aa b07e 0e1e 67d8 8866 00c7  .E=.3..~..g..f..
-00003910: de6a d6fc c110 007c 167c ce97 df7d 61c7  .j.....|.|...}a.
-00003920: b083 3efc 6e3f 2e00 155d 5da4 a1c9 7b7f  ..>.n?...]]...{.
-00003930: 529c d368 0f13 c63b 1106 d3e6 3182 a0d5  R..h...;....1...
-00003940: 5fea 404c 134b fb4f 1924 6af5 0049 fe8f  _.@L.K.O.$j..I..
-00003950: 3c9c a45e 093a d5ac 09a4 3508 87da 5a70  <..^.:....5...Zp
-00003960: a191 f55c 1deb 1709 14d8 bc8a 6843 094a  ...\........hC.J
-00003970: e9ed c2ac 734e cbf7 0fc1 3d09 c660 4fd9  ....sN....=..`O.
-00003980: ad58 00e8 130a d9d2 8dd6 a2b6 3903 81bf  .X..........9...
-00003990: ea57 ebb6 26d0 d4c5 0923 1c95 d2a8 86b8  .W..&....#......
-000039a0: d1e5 8f23 effa da42 eb90 daeb 9c0d 24ce  ...#...B......$.
-000039b0: 61ef f13f 56d6 5f15 0075 15f0 49db 6ba5  a..?V._..u..I.k.
-000039c0: de50 4ceb 1740 02b8 00c7 05f2 52ea 8c45  .PL..@......R..E
-000039d0: 64d6 21c7 e7a9 7026 0e50 1117 d2d5 604a  d.!...p&.P....`J
-000039e0: ac9a 69c6 ac15 9706 db0e 8c2f 71e7 002c  ..i......../q..,
-000039f0: 517f c641 5458 0b92 b941 b250 ec3c 1944  Q..ATX...A.P.<.D
-00003a00: 794b 32ad e7a3 5b77 a1e8 3fec f6fe 333d  yK2...[w..?...3=
-00003a10: e208 c431 dc6e 4016 1f96 c317 ca34 206c  ...1.n@......4 l
-00003a20: fd6a 2bba 00da e7e6 eceb d0a0 bfc1 b2e1  .j+.............
-00003a30: d3ea ead9 dfe6 eff0 d5e0 e3d1 d4dc e7ef  ................
-00003a40: eae9 efee efd6 b8d0 e5dc dff0 ecec e6df  ................
-00003a50: e0c0 dfd4 d2eb efdd e2e6 003f 3f3f 3f3f  ...........?????
-00003a60: bfbf 6d0e 8ff7 408f e46b 2d60 5a9b 6860  ..m...@..k-`Z.h`
-00003a70: f9c0 69df b522 8b5c 213b e046 96ee 1f88  ..i..".\!;.F....
-00003a80: 0e0b aa9d fb2e 27f3 4542 d688 5c59 404b  ......'.EB..\Y@K
-00003a90: d532 710c b214 8f39 d64a 56e5 20b8 5fef  .2q....9.JV. ._.
-00003aa0: 3cc2 051e 08a5 6dbc 2e18 6352 77da 2262  <.....m...cRw."b
-00003ab0: dbb4 810d 1ab5 b521 8d00 a115 a881 6a8e  .......!......j.
-00003ac0: 587f 8d98 3ccb 3b32 5499 5654 b0d6 05ac  X...<.;2T.VT....
-00003ad0: f2d0 ab92 4a9a c451 90cd b6be b4d0 4fb7  ....J..Q......O.
-00003ae0: 88ec 5911 e80f fe8a 7765 4968 6618 8157  ..Y.....weIhf..W
-00003af0: 2b39 2f3c 9aaf bcd0 2f55 623c ae56 af4c  +9/<..../Ub<.V.L
-00003b00: 373a f60c 728c d6d9 7f71 f643 2ee4 9e6a  7:..r....q.C...j
-00003b10: 1ae6 a2cf 945d d627 9203 9a40 c5be 5e63  .....].'...@..^c
-00003b20: c651 f190 2871 61a1 c5e0 bd50 153c 206d  .Q..(qa....P.< m
-00003b30: 6b14 8267 cbd9 02b9 e823 6ce9 72d0 0b6e  k..g.....#l.r..n
-00003b40: 86ef 6ef7 e40e 5430 9d28 f48b 3866 d1ce  ..n...T0.(..8f..
-00003b50: f4b2 77a9 f162 7106 2fe8 2b49 5bd2 5d07  ..w..bq./.+I[.].
-00003b60: d98a 2ad7 1f5f d5e4 debf f3be b0d8 c8ef  ..*.._..........
-00003b70: d92e e576 d3fc 80fe 2d3e 351d a625 bcce  ...v....->5..%..
-00003b80: f06f 2cb9 bac7 5f05 f6f4 9193 14b3 af67  .o,..._........g
-00003b90: 3aae 471a 26d4 5e1e 07ea edb2 acde dfde  :.G.&.^.........
-00003ba0: f0ed ecee eeed e0ef f1d9 e1f0 f0f2 d7e0  ................
-00003bb0: efea f1e5 e7f1 eaea efef f0e4 dee6 e6e4  ................
-00003bc0: e0f1 ecec e6e2 ecda e5e7 d2ee f0e0 e634  ...............4
-00003bd0: 2ded b3c6 6cd8 d3c2 fd32 656d faf2 eea9  -...l....2em....
-00003be0: a3b7 2d2c 99d1 f269 634a 2e3e c87a 26e3  ..-,...icJ.>.z&.
-00003bf0: e3cd e681 991b fe5b 074a bfa6 e273 60d9  .......[.J...s`.
-00003c00: e98e f03d 68cd e5b0 e17c 9d62 e6c7 d105  ...=h....|.b....
-00003c10: 295c f308 9937 3ef2 e6a1 1837 0179 edf7  )\...7>....7.y..
-00003c20: bd70 e81d 7f40 10fa 1371 2b0c b184 35dc  .p...@...q+...5.
-00003c30: af82 3f4b fcb0 a812 0424 fc10 d8e8 bfe9  ..?K.....$......
-00003c40: a7e2 9d8a dcbd da17 775c 0e2e 5f41 87fa  ........w\.._A..
-00003c50: de44 75d2 2f2f 0490 217c 6925 f18c 18ce  .Du.//..!|i%....
-00003c60: b0ea 42fc 2d64 f896 7b56 8104 b102 e0b4  ..B.-d..{V......
-00003c70: fc23 389a 65a7 a466 c275 cde3 0edd f3c2  .#8.e..f.u......
-00003c80: 4d70 3943 62eb 4a97 1fcd 7548 f78f b5eb  Mp9Cb.J...uH....
-00003c90: 8e37 ee12 5326 a454 3252 b736 508b fa65  .7..S&.T2R.6P..e
-00003ca0: 9052 bbcb f5e4 7353 5a1c 8a57 b153 33cd  .R....sSZ..W.S3.
-00003cb0: 3c13 d86e e04c 2f4f 56fd f756 bece 008b  <..n.L/OV..V....
-00003cc0: 0e04 cd32 0b4b 2038 f141 f66a d1ca dbc9  ...2.K 8.A.j....
-00003cd0: 988b cfbc 143b df20 9f07 a04c 8ebf 4676  .....;. ...L..Fv
-00003ce0: a58c 9151 2a0d df28 0943 06a1 b946 7c3c  ...Q*..(.C...F|<
-00003cf0: 772e e6e4 bc65 f96b 6902 ea69 da3e eb22  w....e.ki..i.>."
-00003d00: 09ce 80f8 f08c fc52 a465 554b 1763 6049  .......R.eUK.c`I
-00003d10: 515d 6466 6565 1641 425f 6056 5061 5b5d  Q]dfee.AB_`VPa[]
-00003d20: 4f54 4333 3144 554f 5757 5652 5b62 6563  OTC31DUOWWVR[bec
-00003d30: 5245 595b 5756 554c 6131 4838 524f 524e  REY[WVULa1H8RORN
-00003d40: 4a58 40c0 40c0 c0b6 108f 0afa 136e 9aa7  JX@.@........n..
-00003d50: daf6 9f9e 0a79 2e73 b3b6 0989 fcaa 7cf4  .....y.s......|.
-00003d60: 50e4 08bd bd61 54a8 c4df 532f 2ecd ce9f  P....aT...S/....
-00003d70: 60e1 f24c a522 e841 4881 507b 65f6 04b6  `..L.".AH.P{e...
-00003d80: a5b3 f9b2 bd48 f922 7890 84c4 ceee d658  .....H."x......X
-00003d90: 4000 d880 9fee d141 69d2 845e d071 4195  @......Ai..^.qA.
-00003da0: 6f32 a5e5 e71b a499 152f a8c7 5153 49dd  o2......./..QSI.
-00003db0: f97c 9a0f 57ec 3fc0 9cf7 2287 fb10 87ac  .|..W.?...".....
-00003dc0: 555f 5790 719f 6243 a7e2 6614 1129 50f9  U_W.q.bC..f..)P.
-00003dd0: 3333 b247 9504 ca60 65b3 d847 3321 77b4  33.G...`e..G3!w.
-00003de0: 32ad 7f9e b65b 3f23 7a35 b505 3255 9bcc  2....[?#z5..2U..
-00003df0: 3553 5fd4 1c4a 4d15 7a5c 7f24 97b5 5cc6  5S_..JM.z\.$..\.
-00003e00: 3edd bd14 b61a 2911 54e8 a526 9bc3 d79f  >.....).T..&....
-00003e10: c9cd 318a d468 d6d1 e04e 6dc0 70eb e91e  ..1..h...Nm.p...
-00003e20: 9080 036c fd02 92ee 65a6 cf22 fc92 e5de  ...l....e.."....
-00003e30: c22d 6f07 e05c 7707 b373 5cff f3f8 d7b5  .-o..\w..s\.....
-00003e40: 2eb5 4ebd 3041 bbc7 2158 081f 4d76 0968  ..N.0A..!X..Mv.h
-00003e50: be3c 0c9e 9a05 23eb dc95 622a 628a 9462  .<....#...b*b..b
-00003e60: 47b4 ef21 31ef ae46 37dd 1776 7dbb 6756  G..!1..F7..v}.gV
-00003e70: 39bb a161 97dd 8ad2 b0a7 b89b 8c31 154c  9..a.........1.L
-00003e80: c6e4 624b accd caa2 a9a6 aeb0 a4a5 abb2  ..bK............
-00003e90: b4ad b0cd a3b1 b6a7 a29c bdbf a8b8 d6c3  ................
-00003ea0: d6c2 b8bc b3a9 b0a6 a5b0 a6b3 aecb aba6  ................
-00003eb0: a3bb b5bd b9a0 a7c7 a4c2 3f6c bb8c 6e16  ..........?l..n.
-00003ec0: c6d9 c31a a688 b0b1 3956 f475 b287 f6e9  ........9V.u....
-00003ed0: 6b92 d0e1 e047 bc0f 340b 9247 ba80 7c35  k....G..4..G..|5
-00003ee0: 1e33 d2e2 c0fd 49f9 8ec9 2b0d 7f63 6d57  .3....I...+..cmW
-00003ef0: e8e2 24dd 06fd b900 0862 e35f 6e8b 33c7  ..$......b._n.3.
-00003f00: e3d4 a2d3 fbdc 4137 0954 5c30 73ae 7f14  ......A7.T\0s...
-00003f10: 3481 fe20 7698 9c47 d089 549d e1a7 e3d1  4.. v..G..T.....
-00003f20: 93db 2546 46a9 c2e5 d16a 99f2 4460 9829  ..%FF....j..D`.)
-00003f30: 34ee 2bd6 946d dc9d 4f07 0c98 9ebe 32c4  4.+..m..O.....2.
-00003f40: 44fa 2f3d 867e 3fe3 0957 9dce 462d 78f5  D./=.~?..W..F-x.
-00003f50: 8f6c 0a32 774f 8b25 2905 a554 3b0b 09dd  .l.2wO.%)..T;...
-00003f60: 0f00 9253 2b07 79c9 f5af 67fe 1a22 f18f  ...S+.y...g.."..
-00003f70: bed7 0f46 6c3d 98ae 7996 c707 6357 c145  ...Fl=..y...cW.E
-00003f80: b70f 9f6a c44c 13a2 b80e 29e0 226d 1f02  ...j.L....)."m..
-00003f90: 969e afa1 150a 80d8 0e32 a1dd 5aff 226e  .........2..Z."n
-00003fa0: 9338 fc77 4b26 ba0c 58d3 56b5 b401 8a1a  .8.wK&..X.V.....
-00003fb0: f984 6f40 4c68 7927 9029 4998 f392 a321  ..o@Lhy'.)I....!
-00003fc0: 1472 4957 a071 6b04 c567 9724 6942 dc9e  .rIW.qk..g.$iB..
-00003fd0: 4b80 368d 8058 8561 a9a9 3c16 4a07 fcf4  K.6..X.a..<.J...
-00003fe0: ffed ac29 fb0f e3a5 9c9b cf24 96c0 5e24  ...).......$..^$
-00003ff0: b468 4fda b4e8 e883 8aa6 b492 9994 a1a8  .hO.............
-00004000: 9b91 a19d 999c a0a1 9ba1 a497 9493 a3a3  ................
-00004010: a1a0 aea4 b3a3 a9a7 a594 98a2 9895 91a0  ................
-00004020: a1a6 94a4 9a9f a9a2 a296 9aa1 9aa5 7cde  ..............|.
-00004030: 30df c7f9 a4eb c46f 7147 29a9 ef24 a38f  0......oqG)..$..
-00004040: bc4d 8e8f 4201 d665 dac8 acca 5daa e4b5  .M..B..e....]...
-00004050: 1815 2d39 e7fd 9af8 f5ef 3e9f 9797 b6df  ..-9......>.....
-00004060: 8700 af94 3d94 1247 e0d2 1d62 d406 16f1  ....=..G...b....
-00004070: b3bd cb82 147d d74b e34d 1f31 7c4e fbd4  .....}.K.M.1|N..
-00004080: ac5d 5084 b6ec 7eae f318 8a00 a34c 9de3  .]P...~......L..
-00004090: 96e4 d059 dbfe e363 5c60 a319 076d 1a6a  ...Y...c\`...m.j
-000040a0: 89ba 8108 b7de 33ab 5d91 ead8 4a44 5f27  ......3.]...JD_'
-000040b0: dd3f 7447 594d 076c 8850 409b 3843 4c84  .?tGYM.l.P@.8CL.
-000040c0: 941a 744b cad9 f058 16c6 7694 50f8 1a65  ..tK...X..v.P..e
-000040d0: 4d1f 84f8 94f6 90eb 59c4 583d b2dc a8f5  M.......Y.X=....
-000040e0: 698c c796 d92c 8947 3b5c d1ea c098 28b0  i....,.G;\....(.
-000040f0: f9b5 0b1b 5e9b 07f1 f0d2 7dea 3b0e 221f  ....^.....}.;.".
-00004100: 9d8b 815e c241 541b 8c9a af87 7f0c d8e2  ...^.AT.........
-00004110: e9ff 0ecb cfee ec8e 4562 a2c3 73c0 c66a  ........Eb..s..j
-00004120: 4329 d629 d3d9 38f7 80db 889e 2e2c 6c17  C).)..8......,l.
-00004130: 034c daf5 a3da 309b dfd9 9652 3f04 2184  .L....0....R?.!.
-00004140: bad9 6fa6 5a88 7a7f b705 70cd 107e e583  ..o.Z.z...p..~..
-00004150: ed1f 9de9 bd26 15dd ffae 6d0b a9c3 996a  .....&....m....j
-00004160: 2057 80a0 afc1 70ac 957b 9c6b 4e52 4954   W....p..{.kNRIT
-00004170: 5250 2543 4b30 5136 4a4d 5354 343e 5345  RP%CK0Q6JMST4>SE
-00004180: 4f50 4b52 4440 3541 5149 3f52 ff2b 2b53  OPKRD@5AQI?R.++S
-00004190: 4d48 244a 454e 503d 5427 434b 5551 4649  MH$JENP=T'CKUQFI
-000041a0: 5340 c03f c0c0 00a2 a862 dfd0 c853 5bd5  S@.?.....b...S[.
-000041b0: 251a 5a14 2d77 0fff ffb5 04a0 3734 cabd  %.Z.-w......74..
-000041c0: 75e8 0203 f86a 0d25 a362 c4af bb91 240c  u....j.%.b....$.
-000041d0: 917b bee6 9003 8a42 533e 496f 00fe e6cf  .{.....BS>Io....
-000041e0: 9789 9dc6 f6a5 b433 48c3 5376 0f96 4eb2  .......3H.Sv..N.
-000041f0: f036 df27 0bf8 3639 a29f 2886 590a d48a  .6.'..69..(.Y...
-00004200: 442d a1e4 1e00 4e43 f6bb 23fb 5c3d 6bbf  D-....NC..#.\=k.
-00004210: 2578 d3bc 8a8f 1657 825e d783 f820 1383  %x.....W.^... ..
-00004220: 6d88 dc82 cc43 2373 0d63 f296 33ec 3ea3  m....C#s.c..3.>.
-00004230: b52a 38b6 0b32 a8a8 e908 b0b0 6f6a 1364  .*8..2......oj.d
-00004240: c85e 342a 13e3 80f2 f65f 2675 71ca 1ca9  .^4*....._&uq...
-00004250: 52e0 16ea badb b8df d19c 0e72 8be7 a19a  R..........r....
-00004260: 3634 b68e 6ac8 6172 458b d109 4d4a d927  64..j.arE...MJ.'
-00004270: 634d ff45 1047 8816 f636 4c24 f3bb bb8e  cM.E.G...6L$....
-00004280: ae5b eb74 326b 0c7f 04d1 f982 2805 9b61  .[.t2k......(..a
-00004290: e5a6 5279 3954 52e5 8cc8 2d9a 5cb5 e2be  ..Ry9TR...-.\...
-000042a0: 6ecc c8c7 161e 1d6a 7653 e858 c69b 279f  n......jvS.X..'.
-000042b0: 6f00 ff99 e632 ebdf 17db d847 37f0 598c  o....2.....G7.Y.
-000042c0: e4d6 1b8c bf43 c45e 4ab5 c60c f24a 8693  .....C.^J....J..
-000042d0: c7d3 25c1 d42d 145b 5bca 996d 0c28 5568  ..%..-.[[..m.(Uh
-000042e0: 6a0b b69b 47cd f9ac a9d3 a1d8 bfe4 cac7  j...G...........
-000042f0: c8b6 b0b1 cac2 cbdd d6b3 e7e7 c0c3 cfba  ................
-00004300: ead3 e2d9 d491 e5e0 cfd5 b2c9 b8e7 ccd3  ................
-00004310: c4e8 f0e8 e2c2 a4d4 ddcc bfbf bff9 3c91  ..............<.
-00004320: 8693 30ab 20c0 e48b 763d 54a9 f397 c25c  ..0. ...v=T....\
-00004330: 2089 a2da 9ed7 81aa 8fc4 e724 f67a 424e   ..........$.zBN
-00004340: b111 bd40 fc1c 6c62 ff8d 18ff a99a 1ce8  ...@..lb........
-00004350: 4060 2662 3a09 da5c a6d7 44fb 2e34 6b6c  @`&b:..\..D..4kl
-00004360: 3231 7608 aaa7 f2e9 747e 5c09 04e5 adc1  21v.....t~\.....
-00004370: 726f 63d7 ca4b 80a6 7b1e 8ae3 2b1f 9caf  roc..K..{...+...
-00004380: b1ee 9221 3dd4 31ab e492 9f10 7350 81d3  ...!=.1.....sP..
-00004390: 9dbf ca8b 1730 cc53 142f 62da 2bd6 a593  .....0.S./b.+...
-000043a0: 9d07 e22d 03ed 9682 8476 aef2 46a4 55b7  ...-.....v..F.U.
-000043b0: 60d6 aab1 b449 6d2a 2be1 6f2a fd6a 392f  `....Im*+.o*.j9/
-000043c0: d262 ee9b 4665 54b5 14b8 a07e 9dc8 86a4  .b..FeT....~....
-000043d0: 8aba 3c6f e0e4 ec70 1214 b6ea ee82 43cd  ..<o...p......C.
-000043e0: 3564 378c 4640 b365 7d90 a64e ab01 bad3  5d7.F@.e}..N....
-000043f0: 7354 04c5 798c c5f8 3629 8474 cf36 4693  sT..y...6).t.6F.
-00004400: 3432 d2e7 0e8c 3c25 3aef e8ad 2319 315a  42....<%:...#.1Z
-00004410: 9e7b cd8d 27a7 d436 0896 b646 c439 895e  .{..'..6...F.9.^
-00004420: 6493 6a7e d15a 506c 90b1 22a8 85d3 7d9c  d.j~.ZPl.."...}.
-00004430: b808 0b8b 4017 3385 a9e2 af16 3f27 ec4f  ....@.3.....?'.O
-00004440: e3c7 ae39 1d51 141d a494 5b30 7e89 14c9  ...9.Q....[0~...
-00004450: 457b 2c90 623c 4f0c 780b 4b00 1703 0006  E{,.b<O.x.K.....
-00004460: 0705 0202 03fd 01fd 00fd 01f8 02fe fd03  ................
-00004470: 0607 ff00 0100 06fe 0104 0103 0407 0002  ................
-00004480: 01f9 fb04 0300 0509 0906 0703 0302 0601  ................
-00004490: 3f3f 0081 ca00 0000 dd4b 00dd 4b00 004b  ??.......K..K..K
-000044a0: 0294 9400 dddd 26dd 024b 9402 00dd 002a  ......&..K.....*
-000044b0: 3a9e 00be 9e00 009e 8eae ae00 bebe 96be  :...............
-000044c0: 8e9e ae8e 009e be00 3427 3b00 273b 0000  ........4';.';..
-000044d0: 3b45 3131 0027 2740 2745 3b45 003b 2700  ;E11.''@'E;E.;'.
-000044e0: fab2 0000 0020 b000 20b0 0000 b0f8 6868  ..... .. .....hh
-000044f0: 0020 20d4 20f8 b0f8 00b0 2000 55cb 0000  .  . ..... .U...
-00004500: 0029 3d00 293d 0000 3dc7 b3b3 0029 2982  .)=.)=..=....)).
-00004510: 29c7 3db3 c700 2900 2fc4 0000 00aa 7f00  ).=...)./.......
-00004520: aa7f 0000 7fe9 1414 00aa aab4 aae9 7f14  ................
-00004530: e900 7faa 0087 8200 0000 615a 0061 5a00  ..........aZ.aZ.
-00004540: 005a 6e66 0000 6a00 6600 7181 7c51 6e6a  .Znf..j.f.q.|Qnj
-00004550: 666e 0051 003f 3f3f 3f00 3f00 d3b8 dd00  fn.Q.????.?.....
-00004560: 4b02 dd00 00ef 00b8 00ef 1402 dd26 2626  K............&&&
-00004570: 00b8 94fc b600 0000 aebe 009e 8ebe 0000  ................
-00004580: 4200 b600 4212 8ebe 9696 a696 00b6 ae28  B...B..........(
-00004590: 2c00 0000 3127 003b 4527 0000 2500 2c00  ,...1'.;E'..%.,.
-000045a0: 2543 4527 4040 3640 002c 3169 4420 00b0  %CE'@@6@.,1iD ..
-000045b0: f820 4400 8e66 f820 d4d4 8c00 d400 4468  . D..f. ......Dh
-000045c0: 7a6e 0000 00b3 2900 3dc7 2900 0086 006e  zn....).=.)....n
-000045d0: 0086 25c7 2982 82f8 8200 6eb3 37df aa00  ..%.).....n.7...
-000045e0: 7fe9 aa00 008f 00df 008f cfe9 aab4 b449  ...............I
-000045f0: b400 df14 9276 7100 6600 5100 5a6e 0000  .....vq.f.Q.Zn..
-00004600: 6681 7100 0080 0073 0080 8d8e 617c 7c78  f.q....s....a||x
-00004610: 7c00 7366 3f00 3f7c 886d 002c 9000 00a8  |.sf?.?|.m.,....
-00004620: 617b 0000 b700 df00 99ea 5403 0160 fadd  a{........T..`..
-00004630: 00d8 f400 b63c b200 eb75 0000 cac5 1600  .....<...u......
-00004640: 00d8 007f 0092 3422 213b 34fb 7e00 7242  ......4"!;4.~.rB
-00004650: 00e6 cd00 0000 0b2b 1f00 0071 caaa 1500  .......+...q....
-00004660: ea73 50bf 76c7 a27b 00e7 7800 c97a e700  .sP.v..{..x..z..
-00004670: 4b55 0000 43ce 8700 00f9 005b 0020 91de  KU..C......[. ..
-00004680: b31c daf0 2800 ca03 00e0 e749 000b 4400  ....(......I..D.
-00004690: 0081 fb05 0000 f500 2e00 8213 ca68 7bf9  .............h{.
-000046a0: d800 5096 00da 34c3 0083 3500 00a1 cb38  ..P...4...5....8
-000046b0: 0000 d900 a800 da5c 3a68 e9dd 5c56 00ce  .......\:h..\V..
-000046c0: d700 e4bd 0000 00ce ba00 ecd3 0000 d1c7  ................
-000046d0: e800 00b8 00e3 00ad e6c1 b4dc c5cb e200  ................
-000046e0: bac7 006d ee98 00df 7f00 0010 cc00 6500  ...m..........e.
-000046f0: 23b4 d8a5 c408 d9b7 0023 9c00 00a0 00ae  #........#......
-00004700: fe09 0000 0006 0005 bb00 00ae 0d00 4b00  ..............K.
-00004710: 502e 0b8b 2456 ffaa bb00 00ca c05d 0000  P...$V.......]..
-00004720: 00f7 bc00 35a5 0000 104d 009c 0074 45c1  ....5....M...tE.
-00004730: a8e7 c27b 9800 88c3 0000 7400 9eba 8600  ...{......t.....
-00004740: 0000 1100 b2f3 0000 8ae1 0b00 53e0 733c  ............S.s<
-00004750: df09 16df 00fb 9000 0052 00eb b99f 00e2  .........R......
-00004760: d800 00a6 c800 ba00 0b39 7e10 101f 86e6  .........9~.....
-00004770: 006b ac00 0097 7091 009f c600 0059 2a00  .k....p......Y*.
-00004780: 8b00 dfa6 b677 02fb 0492 001a 1700 00ae  .....w..........
-00004790: 00eb e8d5 00f0 00b2 00d0 e200 00de def0  ................
-000047a0: 0000 db00 ed00 bdee cfc5 e7d8 deed 00d2  ................
-000047b0: e400 0097 0065 dc39 5df7 71c1 517b 3402  .....e.9].q.Q{4.
-000047c0: 9eaf 854b dce3 2fca 4fcf 5c54 fbb9 8e5d  ...K../.O.\T...]
-000047d0: 35e6 b544 8c68 74b8 0b5c c016 bc07 2036  5..D.ht..\.... 6
-000047e0: d405 efbd 573d e53b bdd0 d49f df81 ba9f  ....W=.;........
-000047f0: 99d4 26a3 92f1 6d2b 0530 b1d5 df12 82f2  ..&...m+.0......
-00004800: 6698 62d2 0d04 74fd 8499 443b 8270 1795  f.b...t...D;.p..
-00004810: 1831 5810 8646 76c7 2848 ddf5 3ff8 ff45  .1X..Fv.(H..?..E
-00004820: 4d40 ca51 1da7 f09a f326 0c03 3452 9b60  M@.Q.....&..4R.`
-00004830: 7699 089d 501e 288d 9df6 599e 4c57 938f  v...P.(...Y.LW..
-00004840: bc71 64a6 f9e8 c82f 41ba 0f72 83f5 eb2e  .qd..../A..r....
-00004850: d635 b735 0777 431f 1274 e56a 6d88 1de1  .5.5.wC..t.jm...
-00004860: 3f1b 36f5 ef78 f2cb 1c83 e152 7f7e c98d  ?.6..x.....R.~..
-00004870: 3dae b29c fa61 d2e3 cd4e 6920 976f fcb9  =....a...Ni .o..
-00004880: f5a0 da89 4a93 9c96 94d9 780b 312b 9916  ....J.....x.1+..
-00004890: dfe7 f533 3059 12a7 adfe 92a5 b5dc 5d0e  ...30Y........].
-000048a0: 9998 0e34 0f60 a1bc cd7d 6a44 fda8 206d  ...4.`...}jD.. m
-000048b0: ef1e 9f1f 085b dce7 bb25 a6c8 fcea 918a  .....[...%......
-000048c0: 5263 60ba 4a8f f29a 96ef 6eea 3c55 a23b  Rc`.J.....n.<U.;
-000048d0: cd24 89b4 e759 79d2 f244 54e5 14ef ab00  .$...Yy..DT.....
-000048e0: ef4c d49b 42d4 61f5 9c2e 1c2f b4ad 2b45  .L..B.a..../..+E
-000048f0: c882 3912 f018 e012 2511 2401 18f9 1b10  ..9.....%.$.....
-00004900: 9d10 e3f0 e403 1210 21f2 1a1f 3233 2924  ........!...23)$
-00004910: 1422 1606 e723 fbf3 0927 392f 1122 0406  ."...#...'9/."..
-00004920: 0e09 f504 1922 2922 c03f 403f bfc0 403f  .....")".?@?..@?
-00004930: c03f bfbf bf3f 3f40 c040 3feb ce4c e4a6  .?...??@.@?..L..
-00004940: 6d30 9266 5f6b da9b 2956 5008 7592 9c06  m0.f_k..)VP.u...
-00004950: a60c e5c0 8a6f e407 592b 684d 3cc1 2c34  .....o..Y+hM<.,4
-00004960: ae3d de47 5dde 3d47 9c83 3410 f9e4 e73e  .=.G].=G..4....>
-00004970: 1eb8 5042 8462 1e81 e81e e3a8 2cb0 42f8  ..PB.b......,.B.
-00004980: 538c 5111 4921 0507 d3f1 151b 98e1 1226  S.Q.I!.........&
-00004990: 0a97 00b3 f8cc c9e9 3ffa 02b0 4cb3 d00d  ........?...L...
-000049a0: 01a8 dc9d 3b4b 5bb1 736f 5f68 46d4 b222  ....;K[.so_hF.."
-000049b0: 5ba3 80fe d25e bf68 c2d5 3faf 15b8 9bd6  [....^.h..?.....
-000049c0: 988a 3002 dd00 b762 2a37 22f5 f95d 7762  ..0....b*7"..]wb
-000049d0: 8b72 0dfe f71f 4ac4 085f 14d8 30a0 e744  .r....J.._..0..D
-000049e0: db56 23c9 bcb5 9456 b456 6301 09bf 59c3  .V#....V.Vc...Y.
-000049f0: eb09 411f 60d6 c77a 5171 a98d bbe4 0892  ..A.`..zQq......
-00004a00: 4dc9 9727 e7a6 cf62 7ffc 7417 29b0 55b6  M..'...b..t.).U.
-00004a10: b588 4385 7c48 3969 f0d0 31e0 9b20 c357  ..C.|H9i..1.. .W
-00004a20: 0f40 247b 2413 3631 1c06 607a cb5c 439c  .@${$.61..`z.\C.
-00004a30: d949 fc0a 1773 9950 f358 339a c9a2 7413  .I...s.P.X3...t.
-00004a40: f7d4 9f11 df3a f71a f4d0 a730 1e10 2ba5  .....:.....0..+.
-00004a50: d597 52c9 ef14 fb4a 5121 97c5 33b6 1eea  ..R....JQ!..3...
-00004a60: 0b91 4fe9 e96b 4483 1b5a 0bdb 5189 4285  ..O..kD..Z..Q.B.
-00004a70: cfee 0acb 49a9 a3a9 ddbd 0001 e9f2 f5fe  ....I...........
-00004a80: 13f7 f2f8 fef3 d604 fce4 f914 0cee d207  ................
-00004a90: ebbc e2b8 e4fc e6e9 f1ff 1016 ea07 02fb  ................
-00004aa0: d201 0d02 e0e6 dade f1ff da11 de40 4040  .............@@@
-00004ab0: 403f 4040 4040 6694 9a45 b396 0f0d 62ef  @?@@@@f..E....b.
-00004ac0: f36d fffc b01d 3949 eb48 df4b d35d 9e66  .m....9I.H.K.].f
-00004ad0: 97ea 1cad c200 ead7 f713 d735 5167 cf5f  ...........5Qg._
-00004ae0: 6f67 ef8a a93f 3b4d 3ffd 70b3 c8a1 ef03  og...?;M?.p.....
-00004af0: 6222 29ba 2bad 7c19 f173 8787 0705 d3ee  b").+.|..s......
-00004b00: 72bb b404 7378 a688 f990 4ad7 b408 41ae  r...sx....J...A.
-00004b10: 03a2 b134 ba38 8cb8 845f 9461 050d 4697  ...4.8..._.a..F.
-00004b20: 3a33 1842 3a50 8697 64c5 fc55 b463 8b5b  :3.B:P..d..U.c.[
-00004b30: 4436 86c6 bea4 0831 86b0 370b e1a5 8357  D6.....1..7....W
-00004b40: 60ff 08a4 74a2 18c5 6e61 1bb4 d634 df31  `...t...na...4.1
-00004b50: 9384 b6ab 33a6 534e d3cb b493 597d 690c  ....3.SN....Y}i.
-00004b60: 2815 a705 629d bf85 3d88 47f8 6070 6af4  (...b...=.G.`pj.
-00004b70: 7c63 b517 9a34 2ec3 9844 27a9 97d4 2ef8  |c...4...D'.....
-00004b80: ab95 ce38 956b 4241 305c 9449 9225 28f3  ...8.kBA0\.I.%(.
-00004b90: cc08 15e7 2942 85fc 7ece 46bb cd5e 77b8  ....)B..~.F..^w.
-00004ba0: 3e31 5b3b f2a2 caf8 d8ef 0233 8555 c91b  >1[;.......3.U..
-00004bb0: 9aee 257a c13a 2278 1d78 b9a1 cbd8 e283  ..%z.:"x.x......
-00004bc0: d0a5 8c7c 06fe 7b2c 67d2 2157 0a9d 9503  ...|..{,g.!W....
-00004bd0: 6fcd e16f 4cb2 1871 b209 ee12 a690 da8b  o..oL..q........
-00004be0: 77a2 491f d99e 8f9b 940f b89a e645 3d48  w.I..........E=H
-00004bf0: b2a1 fb29 2528 2221 2123 221f 2122 2322  ...)%("!!#".!"#"
-00004c00: 2222 2524 2224 2321 2224 2622 232c 2c30  ""%$"$#!"$&"#,,0
-00004c10: 2824 2526 241e 241f 2a23 2122 2625 2525  ($%&$.$.*#!"&%%%
-00004c20: 2322 271b 4010 601f fa5a 6f0d 6f01 ec32  #"'.@.`..Zo.o..2
-00004c30: 9f09 a40f 6cb3 6664 b7b0 9875 a5e9 e6b4  ....l.fd...u....
-00004c40: 9a56 7d98 ff54 d806 2c83 2ae4 436b 8b1c  .V}..T..,.*.Ck..
-00004c50: a50f ac28 3f68 4304 4238 a0b6 349b 0137  ...(?hC.B8..4..7
-00004c60: b4a0 2161 85db 60c4 f86e e525 2f9b 6d91  ..!a..`..n.%/.m.
-00004c70: 57f0 da37 5a59 bbd2 82ea d450 e5c1 54c4  W..7ZY.....P..T.
-00004c80: 02fd 82f6 f8ee 7e21 94ec 2738 ca7c ecde  ......~!..'8.|..
-00004c90: 1de7 8b19 5b49 dd2e b44b c842 3888 3207  ....[I...K.B8.2.
-00004ca0: 4de9 e641 2459 4d6e 8db2 5cc8 2adc 2af1  M..A$YMn..\.*.*.
-00004cb0: 9f29 3d69 cf38 d263 8c47 a169 f9b4 69a6  .)=i.8.c.G.i..i.
-00004cc0: ba5d a967 ea16 750d fb0d 1d39 96ab 24fd  .].g..u....9..$.
-00004cd0: 3c83 3b24 9795 6403 634b a9c6 df7e 0d70  <.;$..d.cK...~.p
-00004ce0: 231d eee2 05e7 3e3e 8df5 56ce 7059 1ba1  #.....>>..V.pY..
-00004cf0: 58cb f81a 2dba 2b69 9dfa 3027 37f4 89e3  X...-.+i..0'7...
-00004d00: ada4 05b9 1473 7357 055c e62b 1bf6 00c9  .....ssW.\.+....
-00004d10: 3ba9 b993 ed1e 1c88 d966 3d87 cb67 4a15  ;........f=..gJ.
-00004d20: 7971 2ded 8222 865d b0ce ba35 839d 047e  yq-..".]...5...~
-00004d30: 4fc5 bac8 0009 37ee c177 2481 e29f 16b5  O.....7..w$.....
-00004d40: c2c7 ec5d f2e5 0326 53ed 2bad 0896 3db0  ...]...&S.+...=.
-00004d50: 3ac1 7f82 6a0c 51ee f860 7236 7abf a75b  :...j.Q..`r6z..[
-00004d60: 7c5f e4bb 98b2 bca1 b1b6 b4ca b3b4 bebc  |_..............
-00004d70: b4b4 b8bf adb2 c7b8 bca1 c1b5 a4b6 a0b8  ................
-00004d80: c5b4 aeac c0c7 cdab c0c6 bab0 bdc4 b6ac  ................
-00004d90: aea8 a7a2 b7b3 c6b1 3f75 c00b 2d26 20fe  ........?u..-& .
-00004da0: 758b 2b0b b53a c049 86b2 4174 d1a7 2968  u.+..:.I..At..)h
-00004db0: 879c 822f 479c b35e 6361 e113 8cc0 b790  .../G..^ca......
-00004dc0: 95be fc99 c24f 3537 3725 42fe 89ad 675d  .....O577%B...g]
-00004dd0: 19e5 0c86 4045 2f46 a8ba cc0f b564 c320  ....@E/F.....d. 
-00004de0: 9e41 781a 3d91 7181 a286 32dc 8585 4020  .Ax.=.q...2...@ 
-00004df0: d34e 787f d269 8cf0 27e0 e59a 477f e977  .Nx..i..'...G..w
-00004e00: eca6 4fa4 11a6 8e4c 5396 3a24 07a1 0caa  ..O....LS.:$....
-00004e10: b753 f73d 05b7 fe72 5dd4 a292 7d1b 0c45  .S.=...r]...}..E
-00004e20: d6cc eac0 b7e3 263a e43d a5f6 dce2 632c  ......&:.=....c,
-00004e30: e408 4cc3 b240 177b 2ce2 b7ff 3b26 97f3  ..L..@.{,...;&..
-00004e40: 2d79 22c8 7abb 3518 b9e1 9032 627e 8d0f  -y".z.5....2b~..
-00004e50: 410c 5773 a558 97ce 133a ba3c da1c d674  A.Ws.X...:.<...t
-00004e60: e612 f041 3e25 dc37 cc4e 8ed5 b295 d886  ...A>%.7.N......
-00004e70: c6c0 841e 724f 51b9 2834 55c8 47f6 2b89  ....rOQ.(4U.G.+.
-00004e80: c3d7 a6bd 2de2 1127 d305 d576 0312 feec  ....-..'...v....
-00004e90: dad8 be0b 422a 1db1 e51c 33f8 c35a 6bef  ....B*....3..Zk.
-00004ea0: 7000 486a 641e f477 3c7a 3ec7 1461 6715  p.Hjd..w<z>..ag.
-00004eb0: fa43 552b 34f4 9812 a767 59c6 f027 8215  .CU+4....gY..'..
-00004ec0: 756a 7193 7202 313a f5b2 7ba7 aa68 7a02  ujq.r.1:..{..hz.
-00004ed0: 1937 edf1 2814 ace7 e7c5 dcb8 cbdd c7dc  .7..(...........
-00004ee0: d2d7 e0d5 d7e2 ccd9 d5cc d8d2 e7d9 dfd9  ................
-00004ef0: e7e1 ebe9 efe1 ddc3 dce4 e2ce d2e2 d9e0  ................
-00004f00: d4e1 d8dc e1d7 e2c0 d0e2 dbe0 3f81 e9a8  ............?...
-00004f10: b12c e688 3100 0600 0000 6400 023c 9105  .,..1.....d..<..
-00004f20: 1231 2602 11ab 6e12 0084 3485 220c 0000  .1&...n...4."...
-00004f30: 0084 4038 00c2 8170 2004 4898 1d00 5d04  ..@8...p .H...].
-00004f40: 02ae ae5a 5daa ba54 7551 754f d54d d59d  ...Z]..TuQuO.M..
-00004f50: ba06 8475 756d 75a9 ea4e d5ad aa9b aaab  ...uumu..N......
-00004f60: aa6e eade 2068 97f7 f34d df00 369d d5ed  .n.. h...M..6...
-00004f70: ab1b 5677 5557 54dd 55dd 43de a9b8 e2da  ..VwUWT.U.C.....
-00004f80: af1b c5c5 b19e c921 34eb ebaa 2b55 77aa  .......!4...+Uw.
-00004f90: ee55 dd45 5d51 7907 493c 6951 3fea 4815  .U.E]Qy.I<iQ?.H.
-00004fa0: b6cf 4b4b 2d93 de94 7d38 8e54 57ac eeaa  ..KK-...}8.TW...
-00004fb0: aea8 baab ba51 75ad ea0e 5a12 5321 0017  .....Qu...Z.S!..
-00004fc0: cef4 86af 72a7 3517 2569 8297 4879 12fa  ....r.5.%i..Hy..
-00004fd0: 86a0 df6b a36a bdb6 b408 2d19 ec95 03d5  ...k.j....-.....
-00004fe0: 16fa 6c40 8dc2 4521 4df3 8904 27e6 837a  ..l@..E!M...'..z
-00004ff0: fee6 9224 4df0 12c9 0b2c ff57 fe1e bbc2  ...$M....,.W....
-00005000: 4361 9b91 4678 9a8f 7b5c 6f2e 09d7 4378  Ca..Fx..{\o...Cx
-00005010: 8383 4f36 e8be 863f 494c 45d9 2fe5 a044  ..O6...?ILE./..D
-00005020: 6f9a 1fb4 bf24 8526 2813 7968 3bfa c9ff  o....$.&(.yh;...
-00005030: 02bb 13a4 f8d0 079a d484 f88b eb80 f121  ...............!
-00005040: 72e5 86bf 084a 9320 d1e4 3551 c630 c57f  r....J. ..5Q.0..
-00005050: 2926 a582 d3f0 4063 489e bf94 0230 9ebb  )&....@cH....0..
-00005060: 37bd 376e 99dd 2a20 825d a172 c105 3d12  7.7n..* .].r..=.
-00005070: 89c0 ae00 2c35 2c29 9bde 7262 1fb4 2a95  ....,5,)..rb..*.
-00005080: 6057 0096 7a4b caa6 b7c2 89e5 6057 9435  `W..zK......`W.5
-00005090: a059 62c1 b301 4e14 56f6 a960 57c4 953a  .Yb...N.V..`W..:
-000050a0: 4bca a687 c289 e560 5714 8c0e c134 4e2f  K......`W....4N/
-000050b0: 8513 eb60 5784 0b00 46a3 acb6 e444 0993  ...`W...F....D..
-000050c0: 21f2 979f 6603 3573 14be dd42 b362 0ac0  !...f.5s...B.b..
-000050d0: 5440 7f79 dc93 05d8 4dee c1f9 0b89 5092  T@.y....M.....P.
-000050e0: 4a63 b7d5 e0fa 0b59 6407 3bf2 4472 9b0d  Jc.....Yd.;.Dr..
-000050f0: ce5f 1029 a984 a8c9 cf1e 90f4 a542 b2b7  ._.).........B..
-00005100: 9a92 dfc7 3d78 007f d195 6640 2292 8d81  ....=x....f@"...
-00005110: 23fc c6c9 979a c336 8f27 e5dc 6683 930b  #......6.'..f...
-00005120: 2d0c 78a0 d8cf 07a0 00ad 0ae3 e4f2 9aea  -.x.............
-00005130: 72ab 8baa 0b55 77aa 6e54 dd23 ef54 1cb1  r....Uw.nT.#.T..
-00005140: 26d9 facc 9375 6521 7b4e f2e3 a801 6bef  &....ue!{N....k.
-00005150: f355 175b dd55 ddab ba52 7507 445e 8cc9  .U.[.U...Ru.D^..
-00005160: b847 5c60 c172 3710 46f6 a7cc 064c 9ead  .G\`.r7.F....L..
-00005170: 713f 7375 abea deea beaa 9baa 1b55 57aa  q?su.........UW.
-00005180: 6ed4 6d01 438d 5b75 a3ea 5ad5 bdaa 9baa  n.m.C.[u..Z.....
-00005190: 2baa 6eea 9e25 e8ea bed5 a5aa 6b55 1755  +.n..%......kU.U
-000051a0: 7754 dd54 dd43 de51 8185 b492 58e5 dea8  wT.T.C.Q....X...
-000051b0: fef4 46f9 e48d 045c d555 d575 ab3b 5537  ..F....\.U.u.;U7
-000051c0: aa6e aaae a8ba a97b 2aa0 3091 57b1 3ea7  .n.....{*.0.W.>.
-000051d0: 2254 dd58 ddaa ba53 75ab eaa6 ea3a 253c  "T.X...Su....:%<
-000051e0: 69a9 97b6 5761 ec1f 4c54 f888 89cf b8ca  i...Wa..LT......
-000051f0: b8ad 7125 e356 c64d c655 1977 c485 418d  ..q%.V.M.U.w..A.
-00005200: 3293 bf01 7a53 c156 4ee3 32c6 858c ab8c  2...zS.VN.2.....
-00005210: 3b32 ee32 6e64 5c8b 1b22 dfb8 5ee3 2ee3  ;2.2nd\.."..^...
-00005220: 5ec6 958c 1b19 3719 57aa 0833 26ff b8e8  ^.....7.W..3&...
-00005230: e91b 2f94 0be2 88f2 63bd 1915 cec4 b797  ../.....c.......
-00005240: cb88 6014 2163 1b55 2600 26bf 34b6 5968  ..`.!c.U&.&.4.Yh
-00005250: 2b63 cd8b c6e3 e24f 6c15 8952 b082 16fb  +c.....Ol..R....
-00005260: 740a 9eaf 9b86 e006 d6e9 7f9b 332e 6893  t...........3.h.
-00005270: 2148 75bb 20aa 2b05 3c15 c297 5bb8 cd0a  !Hu. .+.<...[...
-00005280: 5ec0 0755 3113 252a 4b88 228a 48b0 0d90  ^..U1.%*K.".H...
-00005290: dcbe d8fe 1dec 47c4 9f0a c862 1530 c045  ......G....b.0.E
-000052a0: 31df 9255 ba1f 88dd a089 f162 5c0a 3337  1..U.......b\.37
-000052b0: dd6c 8858 b447 4572 3a45 86d6 2d29 7be2  .l.X.GEr:E..-){.
-000052c0: 6e0c 0932 c7d3 1efc e452 2bf3 ae38 0763  n..2.....R+..8.c
-000052d0: 2077 7691 6352 2ec8 5c23 2dc6 4537 9d80   wv.cR..\#-.E7..
-000052e0: b2cb 964c 0533 9742 20da 5744 0b28 d443  ...L.3.B .WD.(.C
-000052f0: 3bd0 06e8 5326 9420 c127 3720 4f6e 5df1  ;...S&. .'7 On].
-00005300: 05b9 7081 197b fc41 d7a0 c105 c106 e19b  ..p..{.A........
-00005310: 7129 cce9 5589 cb63 caa8 5aae 2197 a2e1  q)..U..c..Z.!...
-00005320: 08b2 1997 c246 7b69 e24e 2f4e f4dc 3d02  .....F{i.N/N..=.
-00005330: f4ec 8637 6302 525d 9f5d b224 1a95 592e  ...7c.R].].$..Y.
-00005340: 0ad3 70cb b896 c205 b31f 874a 90cb 7c43  ..p........J..|C
-00005350: a97f 5c22 d11f 0fc8 ea4e ed62 25e3 781b  ..\".....N.b%.x.
-00005360: 37d4 da81 c2cf b210 4bd7 4191 096f 97d3  7.......K.A..o..
-00005370: cb2d 0a9b 4418 3493 9e6b 4b74 2a72 df9b  .-..D.4..kKt*r..
-00005380: 70d3 4de6 7d8c 6b71 a504 0000 0057 3122  p.M.}.kq.....W1"
-00005390: fe                                       .
+00002f30: 0000 0000 0000 0000 0201 91e4 a0ff 0000  ................
+00002f40: 9cff 0000 9c22 0000 1800 0000 9422 0000  ....."......."..
+00002f50: 7822 0000 28b5 2ffd 609c fe75 1301 fce2  x"..(./.`..u....
+00002f60: 0124 2422 220e 2121 2121 fafa fa48 48f3  .$$"".!!!!...HH.
+00002f70: f3be 13e3 d4c0 1717 1717 e2e2 e200 0000  ................
+00002f80: 00c4 c4c4 3131 3162 6262 d8d8 cab2 b2b2  ....111bbb......
+00002f90: b2a8 a0eb ebeb 0079 7963 6358 f1f1 f1f1  .......yyccX....
+00002fa0: 6363 639d 9dcf cfa2 aeeb 3911 4646 4646  ccc.......9.FFFF
+00002fb0: 6f6f 6f5b 5b5b 5b86 8686 3d3d 3dbc bcbc  ooo[[[[...===...
+00002fc0: 9292 9deb ebeb eb2f 95a4 a4a4 0001 0102  ......./........
+00002fd0: 0303 0304 0405 0507 0709 0b0d 0e0f 0f0f  ................
+00002fe0: 1010 1011 1111 1818 1818 1900 5a00 1d00  ............Z...
+00002ff0: 0203 0204 0101 0203 0401 0204 0204 0203  ................
+00003000: 0402 0303 0102 0304 0060 6020 2040 8080  .........``  @..
+00003010: 8080 6060 60e0 e0e0 e000 e080 4000 0000  ..```.......@...
+00003020: a0a0 a0a0 c0c0 c000 0000 e0c0 2020 2020  ............    
+00003030: 00e0 ebeb e2e2 e3f7 f7f7 f779 7979 1d1d  ...........yyy..
+00003040: aeae f45f c46b 8832 3232 3264 6464 7373  ..._.k.2222dddss
+00003050: 7373 8989 89eb ebeb 9999 9924 247f e8e8  ss.........$$...
+00003060: e8e8 4fd1 cece ce00 d1d1 f0f0 fde9 e9e9  ..O.............
+00003070: e938 3838 3333 3a3a 6802 d9fa 42c3 c3c3  .88833::h...B...
+00003080: c34e 4e4e d6d6 d6d0 d0d0 b9b9 b905 0578  .NNN...........x
+00003090: 3636 3636 1dc0 a3a3 a3fd fd90 9084 bebe  6666............
+000030a0: bebe a0a0 a0b4 b4c0 c0ba b4b0 9083 cfcf  ................
+000030b0: cfcf 1515 15da dada daa2 a2a2 9494 94e6  ................
+000030c0: e6e6 acac a0c8 c8c8 c8a3 bcd4 d4d4 3f40  ..............?@
+000030d0: 4040 007e 7e86 86e7 eeee eeee 8b8b 8b66  @@.~~..........f
+000030e0: 6644 4478 2c28 76c7 3939 3939 9b9b 9bae  fDDx,(v.9999....
+000030f0: aeae aebc bcbc 9191 919b 9b9b 6a6a 32b8  ............jj2.
+00003100: 997f 7f7f 0033 3319 19e3 6565 6565 6a6a  .....33...eeeejj
+00003110: 6aaf af25 25a5 fea9 fcf7 c5c5 c5dd dddd  j..%%...........
+00003120: b5b5 b517 1717 4444 1c2c 2c2c 2c3b 6360  ......DD.,,,,;c`
+00003130: 6060 0067 6798 98ef 7979 7979 2121 218a  ``.gg...yyyy!!!.
+00003140: 8a7b 7b0e 499c a68d 8585 8585 3939 390c  .{{.I.......999.
+00003150: 0c0c 0cb4 b4b4 e6e6 e6f9 f9f9 4444 7a3c  ............DDz<
+00003160: 3c3c 3c9c 6e14 1414 0093 9357 5743 a1a1  <<<.n......WWC..
+00003170: a190 90a7 a7db b3d4 4e5f e4e4 e4e4 a4a4  ........N_......
+00003180: a41c 1c1c 1c64 6464 1d1d 1d80 8080 c7c7  .....ddd........
+00003190: 506a 6a6a 6a9a cec3 c3c3 00a7 a747 47cc  Pjjjj........GG.
+000031a0: d8d8 d8d8 d3d3 d369 69d4 d4ef a566 744a  .......ii....ftJ
+000031b0: 3131 3131 9d9d 9d05 0505 b7b7 b785 8585  1111............
+000031c0: dddd 16f6 f6f6 f6e5 97f0 f0f0 1e1e abab  ................
+000031d0: 3cd2 d2d2 d2ef efef 0202 8c8c b232 2d76  <............2-v
+000031e0: aefc fcfc fcc9 c9c9 4c4c 4c4c 2020 20a5  ........LLLL   .
+000031f0: a5a5 d3d3 d393 9310 a4a4 a4a4 bf95 5858  ..............XX
+00003200: 5851 5050 5050 5151 0040 00da da33 8282  XQPPPPQQ.@...3..
+00003210: 8282 9696 9691 91da da35 4901 a2a0 1b1b  .........5I.....
+00003220: 1b1b 2e2e 2ee3 e3e3 e397 9797 6363 63d1  ............ccc.
+00003230: d1d1 1a1a e0c2 c2c2 c2d3 d2dd dddd 00af  ................
+00003240: af92 922a 3a3a 3a3a 3f3f 3fce ce5a 5a3b  ...*::::???..ZZ;
+00003250: 85a3 f45a f3f3 f3f3 6868 68e8 e8e8 6161  ...Z....hhh...aa
+00003260: 61f8 f8f8 4545 4438 3838 388c 5392 9292  a...EED8888.S...
+00003270: 00b7 b742 428e 6868 6868 6e6e 6e2d 2d71  ...BB.hhhhnnn--q
+00003280: 7103 239f 49d5 9494 9494 baba ba04 0404  q.#.I...........
+00003290: 043e 3e3e 8e8e 8e0c 0c0c dddd 64e9 315e  .>>>........d.1^
+000032a0: 5e5e 0014 146e 6eb8 0101 0101 0f0f 0f5e  ^^...nn........^
+000032b0: 5e58 5839 aa9a b3c9 2929 2967 6767 9191  ^XX9....)))ggg..
+000032c0: 91e7 e7e7 1010 67d1 d1d1 d18f ced2 d2d2  ......g.........
+000032d0: 004f 4ffd fd59 2727 2727 4141 41bb bb19  .OO..Y''''AAA...
+000032e0: 197b 60f7 3873 2f2f 2f9b 9b9b 9b18 1818  .{`.8s///.......
+000032f0: 9f9f 9fee eeee bbbb 00f8 f8f8 f893 06f7  ................
+00003300: f7f7 0089 89db db54 7b7b 7b7b 7575 7595  .......T{{{{uuu.
+00003310: 9533 33d8 8720 2e5d 7c7c 7c7c 6363 63e1  .33.. .]||||ccc.
+00003320: e1e1 7c7c 7c4d 4d4d 8686 5a49 4949 4915  ..|||MMM..ZIIII.
+00003330: 117b 7b7b 0019 1908 0805 7618 1876 7610  .{{{......v..vv.
+00003340: 1021 2121 7575 7575 f1f1 f176 7676 2323  .!!!uuuu...vvv##
+00003350: 231c 1c04 7676 7600 4000 8020 8080 2020  #...vvv.@.. ..  
+00003360: c080 4080 2040 4040 8080 00a0 a06a 6a57  ..@. @@@.....jjW
+00003370: 57fe 0909 0909 9292 92ff ffa2 a291 8df7  W...............
+00003380: 6898 4747 4747 5151 5197 9797 6060 601f  h.GGGGQQQ...```.
+00003390: 1f1f bcbc 011f 1f1f 1f7c bad1 d1d1 d6d6  .........|......
+000033a0: 7575 c377 7777 7775 7575 1e1e afaf d45d  uu.wwwwuuu.....]
+000033b0: 390a 66c7 c7c7 6363 6363 5b5b 5b1f 1f1f  9.f...cccc[[[...
+000033c0: 0808 08ac ac87 4848 4848 ffcc 0202 0200  ......HHHH......
+000033d0: 4949 5c5c 4925 2525 6868 3838 6f5f 4431  II\\I%%%hh88o_D1
+000033e0: 524a 4a4a 4a75 7575 5d5d 5d5d 6464 64e2  RJJJJuuu]]]]ddd.
+000033f0: e2e2 7474 7442 426c 4b4b 4b4b 4952 6868  ..tttBBlKKKKIRhh
+00003400: 6800 4040 c040 c0c0 4000 00e0 80c0 0060  h.@@.@..@......`
+00003410: 8080 8080 c0c0 a0a0 c0e0 dbdb 0101 2aab  ..............*.
+00003420: abab ab6b 6b6b 4f4f 8383 d670 40cf 2327  ...kkkOO...p@.#'
+00003430: 2727 6c6c 6c6c 7878 788a 8a8a 9191 916c  ''llllxxx......l
+00003440: 6ca9 7272 7272 99b7 5c5c 5c00 6969 cbcb  l.rrrr..\\\.ii..
+00003450: b036 3636 5454 2e2e 104c ed4d 10fa fafa  .666TT...L.M....
+00003460: faef efef 0f0f 0f0f 7676 7663 6363 2121  ........vvvccc!!
+00003470: 21a6 a66e c1c1 c1c1 9e8f 1c1c 1c51 5161  !..n.........QQa
+00003480: 615a 5353 5353 4c4c 4c56 5668 6857 622a  aZSSSSLLLVVhhWb*
+00003490: 645f 6262 6243 4343 6666 666a 6a6a 6c6c  d_bbbCCCfffjjjll
+000034a0: 4a55 5555 554d 7269 6969 0040 00a0 8080  JUUUUMriii.@....
+000034b0: e0c0 a080 c0c0 c0a0 a000 80ee ee06 0624  ...............$
+000034c0: 2222 2222 9595 9574 7447 47e7 cefd b2db  """"...ttGG.....
+000034d0: 2929 2929 2020 208e 8e8e 8e54 5454 5d5d  ))))   ....TTT]]
+000034e0: 5d40 4040 d5d5 8f87 8787 8791 d295 9595  ]@@@............
+000034f0: bebe d0d0 5cbb bbbb bbda dada 4444 7c7c  ....\.......DD||
+00003500: 73d3 bd22 a255 5555 9090 9028 2828 8484  s..".UUU...(((..
+00003510: 84ff ffc2 1a1a 1a1a 1631 3030 3000 d1d1  .........1000...
+00003520: cece d3d7 d7d7 d7d0 d0d0 dada e4e4 e9d5  ................
+00003530: d5cb cddc dcdc dcd3 d3d3 e2e2 e2e2 e0e0  ................
+00003540: e0d8 d8d8 dfdf dfcc ccd7 d4da 40a0 e0a0  ............@...
+00003550: e0e0 e080 6000 9d9d 7474 8eec ecec ecaa  ....`...tt......
+00003560: aaaa 0000 6262 0000 aa50 8b42 4242 0000  ....bb...P.BBB..
+00003570: 002b 2b2b 4949 aa61 6161 6128 00b8 b811  .+++II.aaaa(....
+00003580: 1123 3232 3248 487a 7ae0 542a be4e 0b0b  .#222HHzz.T*.N..
+00003590: 4b4b 4ba8 a8a8 dbdb db92 922a ef00 3636  KKK........*..66
+000035a0: 3600 7777 6767 6e66 6666 6675 7575 6c6c  6.wwggnffffuuull
+000035b0: 6161 6570 6c70 706e 6e6e 6e78 7878 7070  aaeplppnnnnxxxpp
+000035c0: 7070 6868 6871 7171 7263 6369 7575 7500  pphhhqqqrcciuuu.
+000035d0: 4000 c04d 8000 00a0 00c0 3040 ece0 c0c0  @..M......0@....
+000035e0: 2040 30a0 0000 5986 8e8e 46e0 b270 84ae   @0...Y...F..p..
+000035f0: 50b7 e2ca 6a9a 528b e6e8 ae9c dc42 326c  P...j.R......B2l
+00003600: 9dc2 4ff7 288e fc16 c2c4 a6dc 324b 820b  ..O.(.......2K..
+00003610: 628b 12b3 f2b1 5420 2000 9543 8386 137c  b.....T  ..C...|
+00003620: d9ec 0ac5 27b8 97ee f4c9 84a3 b312 5faf  ....'........._.
+00003630: 1d2f 82d3 308a 9cdf 42ff e85c 03e9 6cb2  ./..0...B..\..l.
+00003640: 9969 ee9a 5244 5bd0 85e9 53b7 b6e7 288e  .i..RD[...S...(.
+00003650: b585 b2ac 1154 f915 8ffc 2c35 2b3c cdc7  .....T....,5+<..
+00003660: 09cc eb2b 8afa ba1c 54f0 db44 c298 9cd5  ...+....T..D....
+00003670: 1aa2 88d0 56f2 7df9 7122 9061 5a2c 0ecb  ....V.}.q".aZ,..
+00003680: 2b2d 3100 8400 007d d753 5b53 6070 4e53  +-1....}.S[S`pNS
+00003690: 6668 6455 627e 5158 8060 4556 729a 6672  fhdUb~QX.`EVr.fr
+000036a0: ad80 bb80 7078 895e 5b5b 4962 4f5f 5683  ....px.^[[IbO_V.
+000036b0: 6152 6289 9192 965a 5c84 4a7f 3458 ecf1  aRb....Z\.J.4X..
+000036c0: 2da3 ccff 8223 a6f9 0130 810b bfe8 ebc9  -....#...0......
+000036d0: 0288 ca36 d984 43ee c4d7 a1af d111 bd67  ...6..C........g
+000036e0: 9034 c74e 9163 5f3e bf14 9f56 2645 0c3c  .4.N.c_>...V&E.<
+000036f0: 87ef be36 c355 81dd 2842 b75e 0cac 5707  ...6.U..(B.^..W.
+00003700: 652f 5c72 e592 57ed abc5 6bc0 5775 a5dd  e/\r..W...k.Wu..
+00003710: 05a0 0bd0 ff87 559a 6020 6754 0efb 146a  ......U.` gT...j
+00003720: b990 65c4 4dc2 10a6 f9f5 5983 4af2 e000  ..e.M.....Y.J...
+00003730: dd3f a197 1d0d d1c8 51ec 5e7b 4f55 81f9  .?......Q.^{OU..
+00003740: 27a6 6b63 1454 0caa 7f1b d114 beff b0c0  '.kc.T..........
+00003750: 4cea b810 2893 bed8 a59b 882e ce0d c0f2  L...(...........
+00003760: 5c4f 89cd fc01 7acf a4b5 c5c5 eccc 28cd  \O....z.......(.
+00003770: 9a73 7006 1c77 01b8 e9ef 3d62 9d45 cf66  .sp..w....=b.E.f
+00003780: 7c4c a043 cfc3 7a67 9910 2d4b 0c64 3aaf  |L.C..zg..-K.d:.
+00003790: 366e affd 7667 62c4 79ee d2ad fa38 894e  6n..vgb.y....8.N
+000037a0: 7093 b0fc 84a1 86eb dd68 f4aa a7f8 06a9  p........h......
+000037b0: fc8b d1ae bffc 5635 b0d0 5fd7 0f44 2372  ......V5.._..D#r
+000037c0: 6d0a a475 c7d2 610d dd42 592c 9d54 b585  m..u..a..BY,.T..
+000037d0: 7c32 59f1 7b4c bfee 5ba1 faeb 6669 6f65  |2Y.{L..[...fioe
+000037e0: 73f2 0f29 524f 6d3c 8e7f bb1f 1a13 1d82  s..)ROm<........
+000037f0: e2d9 8aad c399 db87 ca45 eee2 e2d5 ddf0  .........E......
+00003800: f0ea f2e7 e8da e2e5 84cd e7d5 dfc5 b0e8  ................
+00003810: e8f0 e0b1 dfb4 b17e cfd6 e1dd e5c9 ddb8  .......~........
+00003820: daa4 9da1 d4e6 d8db e5b5 dbd2 d0db b4bf  ................
+00003830: bf3f 3fbf 3f3f 3f00 0a43 6d61 f69e 4659  .??.???..Cma..FY
+00003840: 770e 542d b52c 7f43 f005 8415 ef09 365a  w.T-.,.C......6Z
+00003850: f1ff 7b00 a0e7 1ffb 31c0 d283 10a4 2f4b  ..{.....1...../K
+00003860: 81c0 549a 867b 01d3 074e a78a 2200 9c4a  ..T..{...N.."..J
+00003870: ecdf 543b 0807 182f 9d7e 3559 5d8a 82cb  ..T;.../.~5Y]...
+00003880: babf 5267 d816 cdb4 1183 b4be e1e2 80d8  ..Rg............
+00003890: cc99 a41e c99b 2f6d d231 2a0e e031 ebc8  ....../m.1*..1..
+000038a0: c55b 9d00 944c a522 aa70 c78e b269 249a  .[...L.".p...i$.
+000038b0: 41c1 f620 bf43 93b0 aadb 1c4f 304d 7c27  A.. .C.....O0M|'
+000038c0: 274f a024 4fe7 10ce 9634 9683 ca0f 7a2b  'O.$O....4....z+
+000038d0: cae6 0e5f 4743 1c8b 4700 e714 0ad9 d28e  ..._GC..G.......
+000038e0: d3a1 b539 0481 bfea 55eb b626 d0d4 c50a  ...9....U..&....
+000038f0: 241d 96d2 a886 b9d2 e58f 23f1 fada 41ec  $.........#...A.
+00003900: 90da ea9d 0d24 ce60 eff1 3f56 d65f 1500  .....$.`..?V._..
+00003910: 7515 f049 db6b a5de 504c eb17 4002 b800  u..I.k..PL..@...
+00003920: c705 f252 ea8c 4564 d621 c7e7 a970 260e  ...R..Ed.!...p&.
+00003930: 5011 17d2 d560 4aac 9a69 c6ac 1597 06db  P....`J..i......
+00003940: 0e8c 2f71 e700 2c51 7fc6 4154 580b 92b9  ../q..,Q..ATX...
+00003950: 41b2 50ec 3c19 4479 4b32 ade7 a35b 77a1  A.P.<.DyK2...[w.
+00003960: e83f ecf6 fe33 3de2 08c4 31dc 6e40 161f  .?...3=...1.n@..
+00003970: 96c3 17ca 3420 6cfd 6a2b ba00 dae7 e6ec  ....4 l.j+......
+00003980: ebd0 a0bf c1b2 e1d3 eaea d9df e6ef f0d5  ................
+00003990: e0e3 d1d4 dce7 efea e9ef eeef d6b8 d0e5  ................
+000039a0: dcdf f0ec ece6 dfe0 c0df d4d2 ebef dde2  ................
+000039b0: e600 3f3f 3f3f 3fbf bfdc b67f dde9 b216  ..?????.........
+000039c0: 463b 259f fd64 c8c9 39f2 c253 853f cafc  F;%..d..9..S.?..
+000039d0: e015 589f 7f13 221c 2142 b72f 885a 85f4  ..X...".!B./.Z..
+000039e0: eb55 6a36 0533 e6fb daa2 e7f0 5a09 d416  .Uj6.3......Z...
+000039f0: dc98 20a1 29b2 a80d 6763 050d d7be 58d8  .. .)...gc....X.
+00003a00: aa6c fe9e c7f0 e8c1 b608 17b9 ea5c acd5  .l...........\..
+00003a10: d91a 643f dea1 5885 6810 350c e025 d982  ..d?..X.h.5..%..
+00003a20: ea8e 0dde 1845 8f06 ecde 605a d3cd 2339  .....E....`Z..#9
+00003a30: 22a5 8fdd d669 ad9d 4842 ffcd 3e26 9cd0  "....i..HB..>&..
+00003a40: f75b 4eb2 b956 27cc 7822 480e f57f 01ba  .[N..V'.x"H.....
+00003a50: 3845 d08b 4f30 1d21 3af7 0c72 8dd6 d97f  8E..O0.!:..r....
+00003a60: 71f6 432e e49f 691a e6a2 cf94 5dd7 2791  q.C...i.....].'.
+00003a70: 039a 41c5 be5e 63c6 51f2 9028 7061 a1c5  ..A..^c.Q..(pa..
+00003a80: e0bd 5016 3c20 6d6a 1482 67cb d902 b9e8  ..P.< mj..g.....
+00003a90: 236c e972 d00b 6e86 ef6e f7e4 0e54 309d  #l.r..n..n...T0.
+00003aa0: 28f4 8b38 66d1 cef4 b277 a9f1 6271 062f  (..8f....w..bq./
+00003ab0: e82b 495b d25d 07d9 8a2a d71f 5fd5 e4de  .+I[.]...*.._...
+00003ac0: bff3 beb0 d8c8 efd9 2ee5 76d3 fc80 fe2d  ..........v....-
+00003ad0: 3e35 1da6 25bc cef0 6f2c b9ba c75f 05f6  >5..%...o,..._..
+00003ae0: f491 9314 b3af 673a ae47 1a26 d45e 1e07  ......g:.G.&.^..
+00003af0: eaed b2ac dedf def0 edec eeee ede0 eff1  ................
+00003b00: d9e1 f0f0 f2d7 e0ef eaf1 e5e7 f1ea eaef  ................
+00003b10: eff0 e4de e6e6 e4e0 f1ec ece6 e2ec dae5  ................
+00003b20: e7d2 eef0 e0e6 4626 37ac 037e b640 dcc0  ......F&7..~.@..
+00003b30: c1f5 e82f be5a 94dd b9f1 78db 4d2c 6acd  .../.Z....x.M,j.
+00003b40: 65ed 88ca 99a5 ecf8 e75f deab a939 776c  e........_...9wl
+00003b50: fbcf dae5 72dc 1b35 89fe 3de3 4c96 e905  ....r..5..=.L...
+00003b60: 3d80 9b4e bb4e 044f 1f84 48fe 2c9a 12cd  =..N.N.O..H.,...
+00003b70: 4994 e7c4 f9c5 02d3 b25d 9012 8cb1 54cb  I........]....T.
+00003b80: 3110 00ce 3c9c 1674 e2e8 960b 5dfe 76e4  1...<..t....].v.
+00003b90: 41f2 e4d9 ecac f3a9 eae4 11b4 d3d8 3165  A.............1e
+00003ba0: 753c 19a1 574d e8fa 9ea7 2029 6b45 9a38  u<..WM.... )kE.8
+00003bb0: 8b51 291d bd2d e485 6027 dc2e 0ccb bd7a  .Q)..-..`'.....z
+00003bc0: 6484 3cb7 e6e0 b4fb 2338 9a65 a7a4 65c3  d.<.....#8.e..e.
+00003bd0: 76cd e30e ddf3 c24d 7039 4463 ec4a 9720  v......Mp9Dc.J. 
+00003be0: cd75 48f7 8fb5 eb8e 38ed 1253 26a5 5432  .uH.....8..S&.T2
+00003bf0: 52b7 3650 8bfa 6590 52ba cbf5 e473 535a  R.6P..e.R....sSZ
+00003c00: 1c8a 57b1 5333 cd3c 13d8 6ee0 4c2f 4f56  ..W.S3.<..n.L/OV
+00003c10: fdf7 56be ce00 8b0e 04cd 320b 4b20 38f1  ..V.......2.K 8.
+00003c20: 41f6 6ad1 cadb c998 8bcf bc14 3bdf 209f  A.j.........;. .
+00003c30: 07a0 4c8e bf46 76a5 8c91 512a 0ddf 2809  ..L..Fv...Q*..(.
+00003c40: 4306 a1b9 467c 3c77 2ee6 e4bc 65f9 6b69  C...F|<w....e.ki
+00003c50: 02ea 69da 3eeb 2209 ce80 f8f0 8cfc 52a4  ..i.>.".......R.
+00003c60: 6555 4b17 6360 4951 5d64 6665 6516 4142  eUK.c`IQ]dfee.AB
+00003c70: 5f60 5650 615b 5d4f 5443 3331 4455 4f57  _`VPa[]OTC31DUOW
+00003c80: 5756 525b 6265 6352 4559 5b57 5655 4c61  WVR[becREY[WVULa
+00003c90: 3148 3852 4f52 4e4a 5840 c040 c0c0 e0d5  1H8RORNJX@.@....
+00003ca0: b4f7 ec6a df29 02f0 e961 3b2b 4675 8fb4  ...j.)...a;+Fu..
+00003cb0: eca4 e64c 0357 dbb7 eca3 98e1 9dc0 cd62  ...L.W.........b
+00003cc0: 0a7f d3de 39ed 4553 cc76 09da a66b e628  ....9.ES.v...k.(
+00003cd0: dc09 8ac9 da91 69d9 ea41 66c6 c86c 05b9  ......i..Af..l..
+00003ce0: 4d02 25f0 de01 8304 d48d 439b 6acb 6667  M.%.......C.j.fg
+00003cf0: 0f1e 68c7 4527 fce8 20f4 3807 97a7 f04b  ..h.E'.. .8....K
+00003d00: 15c3 1345 0a92 ba2a 1701 5336 06fb 435c  ...E...*..S6..C\
+00003d10: 60e0 4428 9b84 5c34 cfe6 978e 5c12 da9c  `.D(..\4....\...
+00003d20: d586 1552 5a77 c0a2 d455 7e1f f80b ab37  ...RZw...U~....7
+00003d30: f035 c557 90e9 af1f 820b cdf3 603f 247b  .5.W........`?${
+00003d40: 35b6 0232 569c ce37 5360 d11e 484d 127b  5..2V..7S`..HM.{
+00003d50: 5c79 2594 b660 c73c ddbe 12b8 1b24 0e55  \y%..`.<.....$.U
+00003d60: e6a7 299c c1d6 9dc9 cd2e 8ad1 69d0 d1df  ..).........i...
+00003d70: 516c c070 ebe9 1e90 8003 6cfd 0292 ee65  Ql.p......l....e
+00003d80: a6cf 22fc 92e5 dec2 2d6f 07e0 5c77 07b3  ..".....-o..\w..
+00003d90: 735c fff3 f8d7 b52e b54e bd30 41bb c721  s\.......N.0A..!
+00003da0: 5808 1f4d 7609 68be 3c0c 9e9a 0523 ebdc  X..Mv.h.<....#..
+00003db0: 9562 2a62 8a94 6247 b4ef 2131 efae 4637  .b*b..bG..!1..F7
+00003dc0: dd17 767d bb67 5639 bba1 6197 dd8a d2b0  ..v}.gV9..a.....
+00003dd0: a7b8 9b8c 3115 4cc6 e462 4bac cdca a2a9  ....1.L..bK.....
+00003de0: a6ae b0a4 a5ab b2b4 adb0 cda3 b1b6 a7a2  ................
+00003df0: 9cbd bfa8 b8d6 c3d6 c2b8 bcb3 a9b0 a6a5  ................
+00003e00: b0a6 b3ae cbab a6a3 bbb5 bdb9 a0a7 c7a4  ................
+00003e10: c23f f772 844a b05a c0a7 d4f6 4c81 229b  .?.r.J.Z....L.".
+00003e20: 0f24 7d7d 88c2 b1c0 3741 a0d5 119e 5e7a  .$}}....7A....^z
+00003e30: 296c 9891 3ec9 c336 63b7 6769 83a8 5637  )l..>..6c.gi..V7
+00003e40: 04b3 62e5 74df deaa 00b6 ab73 082b afc2  ..b.t......s.+..
+00003e50: 0f57 151c 91f9 72c9 8944 b2fe 5c77 f900  .W....r..D..\w..
+00003e60: fc28 fd30 0034 b4d8 d734 4a28 ab6a a24a  .(.0.4...4J(.j.J
+00003e70: e987 dce0 2776 5013 c247 dae3 f3b7 831c  ....'vP..G......
+00003e80: a353 05ac eafc 444b 57f0 2542 1d00 3540  .S....DKW.%B..5@
+00003e90: 1ded 89b7 2771 6884 da0f 85df 7c98 090b  ....'qh.....|...
+00003ea0: 8520 68b1 92b6 6de9 8cb5 8212 699f 7e31  . h...m.....i.~1
+00003eb0: d3a3 543b 0b05 da12 fe92 542b 0676 c9f7  ..T;......T+.v..
+00003ec0: ad66 fe1e 21ed 8fbd d60f 456f 3d96 ad79  .f..!.....Eo=..y
+00003ed0: 98c7 0863 54c0 48b7 0fa1 69c3 4c12 a1b8  ...cT.H...i.L...
+00003ee0: 0f22 df20 6f1e 0296 9eaf a115 0a7f d80e  .". o...........
+00003ef0: 32a1 dd5a ff22 6e93 38fc 774b 26ba 0c58  2..Z."n.8.wK&..X
+00003f00: d356 b5b4 018a 1af9 846f 404c 6879 2790  .V.......o@Lhy'.
+00003f10: 2949 98f3 92a3 2114 7249 57a0 716b 04c5  )I....!.rIW.qk..
+00003f20: 6797 2469 42dc 9e4b 8036 8d80 5885 61a9  g.$iB..K.6..X.a.
+00003f30: a93c 164a 07fc f4ff edac 29fb 0fe3 a59c  .<.J......).....
+00003f40: 9bcf 2496 c05e 24b4 684f dab4 e8e8 838a  ..$..^$.hO......
+00003f50: a6b4 9299 94a1 a89b 91a1 9d99 9ca0 a19b  ................
+00003f60: a1a4 9794 93a3 a3a1 a0ae a4b3 a3a9 a7a5  ................
+00003f70: 9498 a298 9591 a0a1 a694 a49a 9fa9 a2a2  ................
+00003f80: 969a a19a a57b 32f1 ceda ceeb db2e f790  .....{2.........
+00003f90: e035 2913 d8ad 50bd 5f47 51ae a6eb f8a2  .5)...P._GQ.....
+00003fa0: 3750 91cd 3285 f7ee 3285 d55c a5fb 977f  7P..2...2..\....
+00003fb0: 45bf 77b9 3c41 51d0 a89f ceba ba86 729b  E.w.<AQ.......r.
+00003fc0: 9200 3e0a a5e4 8d5b 48d8 bf49 407a 5ba1  ..>....[H..I@z[.
+00003fd0: 9fbd 64bd 3388 80a0 71ab 8288 ad27 68de  ..d.3...q....'h.
+00003fe0: 8fdf 3b13 30ed d344 701a 869d 571b c18d  ..;.0..Dp...W...
+00003ff0: 834a b29e dab4 c6ed eb1d 7897 9851 cf4d  .J........x..Q.M
+00004000: 1e44 4722 92ca d820 9efa 5ea2 d223 6f92  .DG"... ..^..#o.
+00004010: 1043 1c08 5042 0908 5cc4 b914 4c48 daee  .C..PB..\...LH..
+00004020: 423c 59ca f71a 6d4c 1f86 dd9a f58b eb5c  B<Y...mL.......\
+00004030: c259 3db7 dba8 f772 92c6 95de 2e89 473b  .Y=....r......G;
+00004040: 5ccf eec1 df38 b1fd b509 145b 9c07 ec0b  \....8.....[....
+00004050: d388 ea3a 1623 1fa1 8b81 5ec2 4154 1b8c  ...:.#....^.AT..
+00004060: 9aaf 877f 0cd8 e2e9 ff0e cbcf eeec 8e45  ...............E
+00004070: 62a2 c373 c0c6 6a43 29d6 29d3 d938 f780  b..s..jC).)..8..
+00004080: db88 9e2e 2d6c 1703 4cda f5a3 da30 9bdf  ....-l..L....0..
+00004090: d996 523f 0421 84ba d96f a65a 887a 7fb7  ..R?.!...o.Z.z..
+000040a0: 0570 cd10 7ee5 83ed 1f9d e9bd 2615 ddff  .p..~.......&...
+000040b0: ae6d 0ba9 c399 6a20 5780 a0af c170 ac95  .m....j W....p..
+000040c0: 7b9c 6b4e 5249 5452 5025 434b 3051 364a  {.kNRITRP%CK0Q6J
+000040d0: 4d53 5434 3e53 454f 504b 5244 4035 4151  MST4>SEOPKRD@5AQ
+000040e0: 493f 52ff 2b2b 534d 4824 4a45 4e50 3d54  I?R.++SMH$JENP=T
+000040f0: 2743 4b55 5146 4953 40c0 3fc0 c000 2780  'CKUQFIS@.?...'.
+00004100: eb62 be9e 049e 7c84 76fd 736e e947 517e  .b....|.v.sn.GQ~
+00004110: 2583 e1b2 bbeb 0ce2 e44b 439b 9347 912b  %........KC..G.+
+00004120: 698c 7fa4 edda 86ea a518 f110 367c 2bf4  i...........6|+.
+00004130: 32dd 6d00 2925 7707 37d8 6f07 ed4a be56  2.m.)%w.7.o..J.V
+00004140: 5b0a ce75 b494 b1f9 1a09 ede5 4d0b 9b31  [..u........M..1
+00004150: f2ac 8acc d168 28a4 e60a ef8d 3caa 3014  .....h(.....<.0.
+00004160: 4887 7ad2 eaa1 10da 8000 e1d9 bfb3 69db  H.z...........i.
+00004170: 04fe ee60 07a7 75e6 ae45 0d63 0b8e 4043  ...`..u..E.c..@C
+00004180: 883c 7ca3 df36 fb29 dfa0 c352 3f32 af62  .<|..6.)...R?2.b
+00004190: 2864 c8dc 3994 5b42 a3e1 3cf4 ee57 b300  (d..9.[B..<..W..
+000041a0: 7ff3 890c 0218 5ab8 269c 2afe 0a1e ac97  ......Z.&.*.....
+000041b0: e40f f277 c069 8305 9c9c 1335 b99e 71c8  ...w.i.....5..q.
+000041c0: f67f 48a7 c782 1f8a d417 70fa 0742 1946  ..H.......p..B.F
+000041d0: 7620 ea37 5800 24f3 bdbc 8eaf 5beb 7432  v .7X.$.....[.t2
+000041e0: 6b0c 7f05 d1f9 8229 059b 60e5 a653 7939  k......)..`..Sy9
+000041f0: 5452 e58c c82d 985c b5e2 be6d ccc8 c716  TR...-.\...m....
+00004200: 1e1c 6b76 53e8 58c6 9b27 9f00 6f00 ff99  ..kvS.X..'..o...
+00004210: e632 ebdf 17db d847 37f0 598c e4d6 1b8c  .2.....G7.Y.....
+00004220: bf43 c45e 4ab5 c60c f24a 8693 c7d3 25c1  .C.^J....J....%.
+00004230: d42d 145b 5bca 996d 0c28 5568 6a0b b69b  .-.[[..m.(Uhj...
+00004240: 4700 cdf9 aca9 d3a1 d8bf e4ca c7c8 b6b0  G...............
+00004250: b1ca c2cb ddd6 b3e7 e7c0 c3cf baea d3e2  ................
+00004260: d9d4 91e5 e0cf d5b2 c9b8 e7cc d3c4 e8f0  ................
+00004270: e8e2 c2a4 d4dd cc00 bfbf bf83 f342 e362  .............B.b
+00004280: 2eec f462 4f79 4ffa 7d49 e8cd a62a 9fcd  ...bOyO.}I...*..
+00004290: eb0e 1758 d276 640e 3613 c4d4 80a6 6e2b  ...X.vd.6.....n+
+000042a0: 6dba ea36 22d6 f1fa e1d5 d556 0f24 4ffe  m..6"......V.$O.
+000042b0: e07b 35d2 edbf 3370 2c1a 6ca1 e136 d314  .{5...3p,.l..6..
+000042c0: 1ba4 50be f21e af75 a5b7 8d69 d36b 9fb1  ..P....u...i.k..
+000042d0: 42b8 f0b3 0b86 2758 958e 6052 d733 f615  B.....'X..`R.3..
+000042e0: 96aa 3e5f c344 a56a 0522 c129 39ef 8d24  ..>_.D.j.".)9..$
+000042f0: c406 01b4 7fdc 5a3a c7e4 5166 b63c b199  ......Z:..Qf.<..
+00004300: 9863 b068 75a7 851b 6990 cdbd 6a5b a98c  .c.hu...i...j[..
+00004310: 6153 5505 350a 6e6d e8fd 6b3d 2bd2 67ec  aSU.5.nm..k=+.g.
+00004320: 9a49 654f b911 bc9e 7c9c cc8c 9d91 b63b  .IeO....|......;
+00004330: 67dd e3ec 700f 1bb6 e8f2 8942 d130 6233  g...p......B.0b3
+00004340: 9046 42b2 6e82 8ead 4dab 00ba cb73 5404  .FB.n...M....sT.
+00004350: c579 8cc5 f836 2984 74cf 3646 9334 32d2  .y...6).t.6F.42.
+00004360: e70e 8c3c 253a efe8 ad23 1931 5a9e 7bcd  ...<%:...#.1Z.{.
+00004370: 8d27 a7d4 3608 96b6 46c4 3989 5e64 936a  .'..6...F.9.^d.j
+00004380: 7ed1 5a50 6c90 b122 a885 d37d 9cb8 080b  ~.ZPl.."...}....
+00004390: 8b40 1733 85a9 e2af 163f 27ec 4fe3 c7ae  .@.3.....?'.O...
+000043a0: 391d 5114 1da4 945b 307e 8914 c945 7b2c  9.Q....[0~...E{,
+000043b0: 9062 3c4f 0c78 0b4b 0017 0300 0607 0502  .b<O.x.K........
+000043c0: 0203 fd01 fd00 fd01 f802 fefd 0306 07ff  ................
+000043d0: 0001 0006 fe01 0401 0304 0700 0201 f9fb  ................
+000043e0: 0403 0005 0909 0607 0303 0206 013f 3f00  .............??.
+000043f0: 81dd 4b00 dd4b 0000 4b02 9494 00dd dd26  ..K..K..K......&
+00004400: dd02 4b94 0200 dd00 2a3a 9e00 be9e 0000  ..K.....*:......
+00004410: 9e8e aeae 00be be96 be8e 9eae 8e00 9ebe  ................
+00004420: 0034 273b 0027 3b00 003b 4531 3100 2727  .4';.';..;E11.''
+00004430: 4027 453b 3145 003b 2700 fab2 0000 0020  @'E;1E.;'...... 
+00004440: b000 20b0 0000 b0f8 6868 0020 20d4 20f8  .. .....hh.  . .
+00004450: b0f8 00b0 2000 55cb 3d00 293d 0000 3dc7  .... .U.=.)=..=.
+00004460: b3b3 0029 2982 29c7 3dc7 003d 2900 2fc4  ...)).).=..=)./.
+00004470: 7f00 aa7f 0000 7fe9 1414 00aa aab4 aae9  ................
+00004480: 7f14 e900 7faa 0087 8200 0000 615a 0061  ............aZ.a
+00004490: 5a00 005a 6e66 0000 6a00 6600 7181 7c51  Z..Znf..j.f.q.|Q
+000044a0: 6e6a 666e 0051 003f 3f3f 3f00 3f00 d3b8  njfn.Q.????.?...
+000044b0: dd00 4b02 dd00 00ef 00b8 00ef 1402 dd26  ..K............&
+000044c0: 266f 2600 b894 fcb6 0000 00ae be00 9e8e  &o&.............
+000044d0: be00 0042 00b6 0042 128e be96 96a6 9600  ...B...B........
+000044e0: b6ae 282c 0000 0031 2700 3b45 2700 0025  ..(,...1'.;E'..%
+000044f0: 002c 0025 4345 2740 4036 4000 2c31 6944  .,.%CE'@@6@.,1iD
+00004500: 0000 0068 2000 b0f8 2044 008e 66f8 20d4  ...h ... D..f. .
+00004510: d48c 00d4 0044 687a 6e00 0000 b329 003d  .....Dhzn....).=
+00004520: c729 0000 8600 6e00 8625 c729 8282 f882  .)....n..%.)....
+00004530: 006e b337 dfaa 007f e9aa 0000 8f00 df00  .n.7............
+00004540: 8fcf e9aa b4b4 49b4 00df 1492 9300 0000  ......I.........
+00004550: 7671 0066 0051 005a 6e00 0066 8171 7300  vq.f.Q.Zn..f.qs.
+00004560: 808d 8e61 7c7c 787c 0066 3f00 3f07 3c4f  ...a||x|.f?.?.<O
+00004570: 005a 2300 000a e02b 7200 119c 5747 d7cf  .Z#....+r...WG..
+00004580: 7fc1 0087 b100 d7af 1a00 18aa 0000 0c5f  ..............._
+00004590: c000 00cf 0041 00d4 e0d6 434b efe5 b600  .....A....CK....
+000045a0: 72bc 0026 e9d6 0064 9900 008d 3e41 0000  r..&...d....>A..
+000045b0: c600 1d00 6e32 09a3 e72e 1200 d63e 003f  ....n2.......>.?
+000045c0: 3d3d 003f 3e00 003e 3e3f 0000 3d3f 3e3d  ==.?>..>>?..=?>=
+000045d0: 3e3e 3f00 3d5e ce4c 0000 00f9 0016 c800  >>?.=^.L........
+000045e0: 0034 4800 0000 5d00 d000 5ace f383 86f9  .4H...]...Z.....
+000045f0: 3037 0061 6500 001a 00bf cd88 ff36 0000  07.ae........6..
+00004600: cdfe 5d00 f831 b3b8 10d8 2497 00d3 bd00  ..]..1....$.....
+00004610: 005c 40ac 0080 0093 0084 1600 00f2 f780  .\@.............
+00004620: 0000 d900 6c00 ee75 7d2b 38c7 f06c 0090  ....l..u}+8..l..
+00004630: 203f 3e3e 3f3e 3e3f 3e3f 0000 3c27 9bc9   ?>>?>>?>?..<'..
+00004640: fe3c 11a2 7c40 628e b3ec a5ee bc17 5806  .<..|@b.......X.
+00004650: 331a 262c 5a5e a83f 120a ea18 a494 9ac0  3.&,Z^.?........
+00004660: bedf 587b 46b6 1dc5 cf8d 4e8e 60be 767f  ..X{F.....N.`.v.
+00004670: 90be e8b5 03a2 d217 59f0 52fe eae3 17b7  ........Y.R.....
+00004680: ad07 428d d137 5fb0 efd5 e6e3 4f6a 0b6f  ..B..7_.....Oj.o
+00004690: d4ae 0315 60f4 a602 5ab5 0965 2516 15ab  ....`...Z..e%...
+000046a0: 42b6 e56b 557b 3a44 262f 7d52 bb0d 7fd1  B..kU{:D&/}R....
+000046b0: 280b 0e0c 32cd 5ff4 c1a3 2a23 d756 88e9  (...2._...*#.V..
+000046c0: efcd 964a fae0 becd 0a0e 34da d6af 44f9  ...J......4...D.
+000046d0: e539 c01e ac48 86c1 202f 99a9 7f45 b403  .9...H.. /...E..
+000046e0: 9c31 df0f 0d4e 893c 047b 1f9e dde2 1891  .1...N.<.{......
+000046f0: 12b5 609b b996 4a45 ddee 09cd c789 1cbe  ..`...JE........
+00004700: 01a7 b80d 14be 251e ac34 3087 4a8e dea2  ......%..40.J...
+00004710: ce11 f65f 85ae 8aec 8db3 5326 e8b2 712e  ..._......S&..q.
+00004720: 3d89 f296 a167 171f c594 c326 2a98 50b5  =....g.....&*.P.
+00004730: 5cab 3a63 f618 af69 a955 672b 194f 7f76  \.:c...i.Ug+.O.v
+00004740: 1f55 5fa9 123a 6f0b 361f a713 348f fd51  .U_..:o.6...4..Q
+00004750: 4107 40c5 6e5f 6fe3 d591 beb5 2602 3a9f  A.@.n_o.....&.:.
+00004760: 2407 2cc1 b859 48c0 76c2 ae57 e7d3 8284  $.,..YH.v..W....
+00004770: a8be 2697 4084 7ef9 7fe5 4010 ff19 0111  ..&.@.~...@.....
+00004780: 2609 22fa 1901 1c0b d711 fa03 c0fe 0103  &.".............
+00004790: 21f0 021d 3234 2923 dc21 180b f814 15f3  !...24)#.!......
+000047a0: 142a 392e 0423 d4ff 110a fc03 1023 2321  .*9..#.......##!
+000047b0: c03f bfc0 bfc0 3fbf 40c0 c0bf 3f40 3f3f  .?....?.@...?@??
+000047c0: 3fc4 cf3f 4b1e 4367 4467 bb36 5363 032e  ?..?K.CgDg.6Sc..
+000047d0: 357a 4b25 29aa 00f1 03a0 5f1b e12c 720d  5zK%)....._..,r.
+000047e0: ca71 111f f7f4 d37a 42fb 8f34 4ff4 99fc  .q.....zB..4O...
+000047f0: a3af 4582 fc28 c0ff 3b0a 1942 c856 d8e0  ..E..(..;..B.V..
+00004800: bc49 5a12 8086 7f17 b22c 5c8d 4750 0350  .IZ......,\.GP.P
+00004810: 0fe6 7198 c846 41a3 7de8 bc57 54c6 18c4  ..q..FA.}..WT...
+00004820: bf51 70be cf07 f961 75f7 8594 09a6 774e  .Qp....au.....wN
+00004830: 00be 84ff 4b32 63d5 00b6 27b2 c8eb 3f41  ....K2c...'...?A
+00004840: 5e73 0c6f d6a8 33f4 137d dadc 918b ea7d  ^s.o..3..}.....}
+00004850: 5f6e d3a6 c6c4 ceca f1f8 e804 4991 6383  _n..........I.c.
+00004860: a3cc 52b9 5b21 54f1 2ebe 8ded b5e6 394d  ..R.[!T.......9M
+00004870: db32 bad0 3c23 9b64 a059 336d d023 a30c  .2..<#.d.Y3m.#..
+00004880: d425 df6e cd3b 8882 a2cc 2986 856e 68da  .%.n.;....)..nh.
+00004890: b20e 2f50 b7b5 b587 4386 7c47 3969 f0d0  ../P....C.|G9i..
+000048a0: 31e0 9b21 c257 0e3f 257b 2413 3631 1c06  1..!.W.?%{$.61..
+000048b0: 607b cb5c 419b d949 fb0a 1772 9950 f358  `{.\A..I...r.P.X
+000048c0: 339a c9a1 7413 f7d4 9f11 df3a f71a f4d0  3...t......:....
+000048d0: a730 1e10 2ba5 d597 52c9 ef14 fb4a 5121  .0..+...R....JQ!
+000048e0: 97c5 33b6 1eea 0b91 4fe9 e96b 4483 1b5a  ..3.....O..kD..Z
+000048f0: 0bdb 5189 4285 cfee 0acb 49a9 a3a9 ddbd  ..Q.B.....I.....
+00004900: 0001 e9f2 f5fe 13f7 f2f8 fef3 d604 fce4  ................
+00004910: f914 0cee d207 ebbc e2b8 e4fc e6e9 f1ff  ................
+00004920: 1016 ea07 02fb d201 0d02 e0e6 dade f1ff  ................
+00004930: da11 de40 403f 4040 4040 d8e3 4d8c 119d  ...@@?@@@@..M...
+00004940: 4e04 3744 010e c25a 1c09 98aa 8c24 5464  N.7D...Z.....$Td
+00004950: 9ed7 2a2d 4722 c6f6 b426 ad38 1ff9 1984  ..*-G"...&.8....
+00004960: 5631 bdfd dc07 fd94 97ea 34e6 4c1e d6aa  V1........4.L...
+00004970: 9d15 a0ac c316 0161 b574 494e 7c40 1b68  .......a.tIN|@.h
+00004980: ea6d 4a1b 9958 6c22 32d9 d66a 48fc 90ff  .mJ..Xl"2..jH...
+00004990: 0c73 2724 cdd9 4773 bb91 54e9 e3ab 3655  .s'$..Gs..T...6U
+000049a0: 2d92 c3b0 9603 ffe7 d9a9 920f 8384 df55  -..............U
+000049b0: b39d 8e9c 1d09 3493 224c 94e0 08e7 6abf  ......4."L....j.
+000049c0: 6f6e d50a 0cb7 c919 2ac3 b900 0888 106d  on......*......m
+000049d0: 8338 85f5 5064 7138 6b4d 8ac9 fc29 b1da  .8..Pdq8kM...)..
+000049e0: b424 cf8a 9704 9503 d7fa 06e1 d26b 8d23  .$...........k.#
+000049f0: d774 aca6 3702 6b7c 20fb b17f 411e b9cc  .t..7.k| ...A...
+00004a00: 3d14 235f 9f61 8727 1e8b 65f0 6d26 1e98  =.#_.a.'..e.m&..
+00004a10: 2b47 8589 a1bd 9217 be90 8220 8fd7 768c  +G......... ..v.
+00004a20: 8d10 c2a0 6f45 67e1 7a8d 834a 5983 43f5  ....oEg.z..JY.C.
+00004a30: e8f7 a452 6558 68b8 98cd 1808 5213 de97  ...ReXh.....R...
+00004a40: ff36 abae edce b475 3411 8627 55bf 077f  .6.....u4..'U...
+00004a50: e75c 76f7 46b5 d26c 61db 4660 defa 0024  .\v.F..la.F`...$
+00004a60: 34b6 ff9b 9bb3 5917 af9b a4b6 bf20 9ea1  4.....Y...... ..
+00004a70: db6b 6241 84d3 1f3f 2528 2221 2123 231f  .kbA...?%("!!##.
+00004a80: 2122 2322 2221 2524 2124 2321 2224 2622  !"#""!%$!$#!"$&"
+00004a90: 232c 2b31 2824 2526 241e 241f 2a23 2122  #,+1($%&$.$.*#!"
+00004aa0: 2625 2525 2322 271c 40f4 399d 563d 31c1  &%%%#"'.@.9.V=1.
+00004ab0: 6cef d45a 0dc9 6763 cb8e 235b 0038 50fc  l..Z..gc..#[.8P.
+00004ac0: b8ab d257 bd72 e178 5523 ecb9 4ef8 0205  ...W.r.xU#..N...
+00004ad0: ac41 393a d75a de8c 991e 7652 4d95 8211  .A9:.Z....vRM...
+00004ae0: 1f8b ee97 60d9 5841 f150 6323 2ec6 f2b5  ....`.XA.Pc#....
+00004af0: 0055 967b 6971 b948 0e4b 0841 1714 a7a6  .U.{iq.H.K.A....
+00004b00: 46d2 ce82 ba90 d0f2 c8ca f28a b533 8272  F............3.r
+00004b10: ae1e a1a5 3af1 a1c7 5d5e 73e6 239d d70a  ....:...]^s.#...
+00004b20: 13b7 c433 1636 37f9 ecb3 3ff1 2c8c ed13  ...3.67...?.,...
+00004b30: 2553 70fd ee76 f6ec 1572 2c26 06d6 2e94  %Sp..v...r,&....
+00004b40: 6f42 c572 ded2 e3ea 29dc e14a c541 2fa3  oB.r....)..J.A/.
+00004b50: 6536 e03d 43d7 25dc 1348 2fc2 c719 8261  e6.=C.%..H/....a
+00004b60: 5391 2379 1e5e 1591 7718 afce 711d 4b08  S.#y.^..w...q.K.
+00004b70: 4eb8 1928 1b4f fc99 d874 3c99 9efb 2f26  N..(.O...t<.../&
+00004b80: 36f4 89e3 aca4 06b8 1573 7357 055c e62b  6........ssW.\.+
+00004b90: 1af6 00c9 3baa b993 ed1e 1c89 d963 3d87  ....;........c=.
+00004ba0: ca66 4b15 7971 2ded 8222 865d afcd ba35  .fK.yq-..".]...5
+00004bb0: 839d 047e 4fc5 bac8 0009 37ee c177 2481  ...~O.....7..w$.
+00004bc0: e29f 16b5 c2c7 ec5d f2e5 0326 53ed 2bad  .......]...&S.+.
+00004bd0: 0896 3db0 3ac1 7f82 6a0c 51ee f860 7236  ..=.:...j.Q..`r6
+00004be0: 7abf a75b 7c5f e4bb 98b2 bca1 b1b6 b4ca  z..[|_..........
+00004bf0: b3b4 bebc b4b4 b8bf adb2 c7b8 bca1 c1b5  ................
+00004c00: a4b6 a0b8 c5b4 aeac c0c7 cdab c0c6 bab0  ................
+00004c10: bdc4 b6ac aea8 a7a2 b7b3 c6b1 8a87 b5f6  ................
+00004c20: 0b2b b06d fdbd e668 1c70 037c 5b4b 5a1c  .+.m...h.p.|[KZ.
+00004c30: 3095 eeca 8d34 175f a3a3 0ced 9aeb 44de  0....4._......D.
+00004c40: b184 dc6b bdc5 e2ac 25a0 a7af 0862 ec05  ...k....%....b..
+00004c50: 180d 5893 fb19 cc5e ceab 772c 17de 8741  ..X....^..w,...A
+00004c60: 71eb 39a5 76fa a043 4899 b323 81be 427f  q.9.v..CH..#..B.
+00004c70: 3f29 2fed 4ee2 8098 f22d 255d ddf1 bdd7  ?)/.N....-%]....
+00004c80: eecc 33d5 4792 765c 4162 98ff 565c d5bb  ..3.G.v\Ab..V\..
+00004c90: c4b6 4b78 1b15 8eb5 bc51 ec0c 4bfc bd8e  ..Kx.....Q..K...
+00004ca0: 086b cbdc a8d7 581f b201 5877 3db7 ca9e  .k....X...Xw=...
+00004cb0: d6a5 ee7e e84a 075e a7ff 14b5 6fe9 5c0d  ...~.J.^....o.\.
+00004cc0: 499b e72d e2e2 766a 0b24 c1e5 1849 47f6  I..-..vj.$...IG.
+00004cd0: e1e9 70b6 ac2e e791 8cd9 2803 7406 8c92  ..p.......(.t...
+00004ce0: bf8f 235c 6dc2 d8e6 9437 2d13 0776 d891  ..#\m....7-..v..
+00004cf0: addb b170 ad37 a9dc 7df0 f3ea 03fe 2e55  ...p.7..}......U
+00004d00: e325 1f57 cd51 1e37 193f 2e02 98ec 721a  .%.W.Q.7.?....r.
+00004d10: 544c 079b bad3 a747 78b4 46f8 621b aaf6  TL.....Gx.F.b...
+00004d20: 8c94 8019 123b f873 322d 931a 3a42 48e1  .....;.s2-..:BH.
+00004d30: 6168 1f45 ee66 80d1 445a d803 ed4d 612f  ah.E.f..DZ...Ma/
+00004d40: a590 d8ae ee49 6be1 5554 d54d 9406 74b9  .....Ik.UT.M..t.
+00004d50: e976 00b0 d709 1a88 9be1 e7e2 c7dd bacb  .v..............
+00004d60: dec7 dcd2 d7e0 d6d7 e3cf d8d3 cbda d3e6  ................
+00004d70: d9de dae7 e2ea e9f0 e1dc c4db e4e2 ced3  ................
+00004d80: e3d9 e1d3 e1db dfe1 d7e1 c1d4 e1dd e03f  ...............?
+00004d90: 81d1 a8c1 28e7 0831 0004 0208 0000 0640  ....(..1.......@
+00004da0: 000f 9105 5231 1400 8058 7500 12c0 a334  ....R1...Xu....4
+00004db0: 4622 0c00 0000 8440 3800 c281 7020 0448  F".....@8...p .H
+00004dc0: 981d 0067 0402 a8b3 ac33 5f67 5267 5ee7  ...g.....3_gRg^.
+00004dd0: a3ce bdce e32c 686a a1a7 ce8a 3a57 9dfb  .....,hj....:W..
+00004de0: 3a8b 3af7 758e b38d 86a9 417f a1f4 1ccc  :.:.u.....A.....
+00004df0: 2368 9db7 ce7d 9d47 9df7 3a47 9dbd a3d7  #h...}.G..:G....
+00004e00: d520 d7b9 701b 9f8a fc20 4fc0 ee14 994a  . ..p.... O....J
+00004e10: 973a 2f3a ef85 1e75 ee75 36ea 3cbe 1e1f  .:/:...u.u6.<...
+00004e20: 530c cbf0 8a30 076f a390 6215 da66 2152  S....0.o..b..f!R
+00004e30: 9db3 ce7f 9d47 9dff 3a47 9dfd 750e 3aff  .....G..:G..u.:.
+00004e40: 28e7 76f1 fd41 b630 2843 1c21 326b 5fe2  (.v..A.0(C.!2k_.
+00004e50: b496 7317 40fa d074 fc83 968c 0d5c 8892  ..s.@..t.....\..
+00004e60: 6fbc 5343 c466 20bf 379c e5bf ad45 041c  o.SC.f .7....E..
+00004e70: 6041 788d 9803 cbfe 9aa6 9d96 c2ad 2a82  `Ax...........*.
+00004e80: 507a 9768 9a61 4c49 fc4b 0104 49b3 0c2a  Pz.h.aLI.K..I..*
+00004e90: d803 7814 4309 c31e 7412 98fd 3eb4 a9fd  ..x.C...t...>...
+00004ea0: 5115 1195 c139 b9c6 3367 81da 1f0f 4f07  Q....9..3g....O.
+00004eb0: 24c9 5d2f b163 87be 1a46 b53f 8a98 fa2f  $.]/.c...F.?.../
+00004ec0: 695a 070a 3be0 d5fe e81f 92a0 282b df51  iZ..;.......(+.Q
+00004ed0: c20e f86a 7fbc 3c1d 4c92 bf9e 0a3b b6ab  ...j..<.L....;..
+00004ee0: fd51 fca9 3749 c33a 56d8 015d ed8f dfa7  .Q..7I.:V..]....
+00004ef0: a349 72d6 5bec d851 d011 4cb3 a37d 4cfb  .Ir.[..Q..L..}L.
+00004f00: ce03 ab85 9e1f 9887 5eb1 9926 a069 d946  ........^..&.i.F
+00004f10: 6472 38c0 a4a9 70ea b0a4 712c 1268 4286  dr8...p...q,.hB.
+00004f20: a669 c8ec 5738 48f2 8304 fa54 556a 1a3b  .i..W8H....TUj.;
+00004f30: 5bca e922 fd40 11ca a449 381d 5b92 3b36  [..".@...I8.[.;6
+00004f40: 71c9 71a3 49a3 3674 5049 fed8 14c0 4286  q.q.I.6tPI....B.
+00004f50: 72d3 cc92 a1da 1149 de58 c43d 7a28 31a3  r......I.X.=z(1.
+00004f60: a085 3430 e3e5 40f0 d0ac a4e2 5a67 7c9d  ..40..@.....Zg|.
+00004f70: a5ce 7c9d 4f9d 7b3a 5f91 1e7c 7069 b980  ..|.O.{:_..|pi..
+00004f80: e53a 9b3c ca21 b70e ecea 8906 a4e7 0a98  .:.<.!..........
+00004f90: 59cc 5c98 5999 7937 7398 d96e e681 190c  Y.\.Y.y7s..n....
+00004fa0: 6323 101c 10b6 6b5d aa53 6b38 5f57 af33  c#....k].Sk8_W.3
+00004fb0: 55e7 50e7 5567 bdce a3ce bdce c639 a8cc  U.P.Ug.......9..
+00004fc0: 6a8b 3a07 75be 3afb eb1c 75ce eb2c ce63  j.:.u.:...u..,.c
+00004fd0: 1bb4 ce4e 9d59 9dfd 3a43 9de7 758e 3a1f  ...N.Y..:C..u.:.
+00004fe0: 478f 0f96 6e49 2daa 2f54 7b72 a17a d342  G...nI-./T{r.z.B
+00004ff0: e543 756e 7506 eaec eaec ebfc d4b9 d739  .Cunu..........9
+00005000: 9c6d 294c 82dc fb28 a7e7 43d4 b9ae 33d4  .m)L...(..C...3.
+00005010: d95f e7a9 f35f 6707 ebd9 4c49 52e0 2091  ._..._g...LIR. .
+00005020: fd83 8e8a be01 becc eccc 1ccc 2c99 b99b  ............,...
+00005030: 3998 5937 f380 196a 7564 320e 300d 4fee  9.Y7...jud2.0.O.
+00005040: 2c0c a9f3 5c67 a9f3 bece 51e7 bece a2ce  ,...\g....Q.....
+00005050: 63bc c77c a42b 8f2a 0375 be3a fba7 dac8  c..|.+.*.u.:....
+00005060: 4d83 e0d9 72b6 7046 6217 6492 68c8 41b1  M...r.pFb.d.h.A.
+00005070: f168 464b 21bb ad66 1045 197f 4cfa a821  .hFK!..f.E..L..!
+00005080: 3a1a 3ee5 4446 cda0 c2bc 54e5 6a35 b18a  :.>.DF....T.j5..
+00005090: 64c5 602f 3878 e8b4 8d11 bfa3 8c70 40f3  d.`/8x.......p@.
+000050a0: 1494 992b 30b5 faf3 9b83 2a35 92df e8d0  ...+0.....*5....
+000050b0: cccc 0fd5 50d4 9cc3 d659 9a7a 3e02 2fd0  ....P....Y.z>./.
+000050c0: 8898 1f92 c00c f230 1d26 5e49 8d27 6d0c  .......0.&^I.'m.
+000050d0: c610 941c 0ea9 fe5d c637 d6ce 4711 df07  .......].7..G...
+000050e0: 7499 51ce d022 d512 c0e1 b995 1671 2633  t.Q..".......q&3
+000050f0: e53b a170 9cc1 7cfa f191 72dd 0343 3b96  .;.p..|...r..C;.
+00005100: b4dd 7136 8809 7cd0 1aa3 3efb 2854 f2fe  ..q6..|...>.(T..
+00005110: 08f8 6060 38a7 1746 a919 8f4e 29cd 6446  ..``8..F...N).dF
+00005120: 7bc9 61f7 bc3a cc87 dfcc cf10 2b5d 62f5  {.a..:......+]b.
+00005130: 68cc 6103 095c c8d5 357c ce04 0d0c 51ae  h.a..\..5|....Q.
+00005140: 2dfa c305 0e9b 1933 5638 8611 4c64 c6f3  -......3V8..Ld..
+00005150: 46c2 9fcc 946f 10bb c3cc 7fca a472 cf9d  F....o.......r..
+00005160: 99a7 6165 629a 1975 83c4 9fcc 1a1d 4aae  ..aeb..u......J.
+00005170: 79db 007d c3c0 84a1 12a9 b3eb 33ec 709b  y..}........3.p.
+00005180: f7d4 cc07 cd3c 61e6 3099 c1ef eaa3 4e67  .....<a.0.....Ng
+00005190: 66b6 21dc 4e33 45d8 0b0f 569d 2d3d 5324  f.!.N3E...V.-=S$
+000051a0: c9f9 667e 93b5 a0fe af1b 4a24 07f1 c8b0  ..f~......J$....
+000051b0: a523 14b5 8938 7346 92e6 a49a 6d89 ce02  .#...8sF....m...
+000051c0: 5dc6 2d7a 95d3 d0ad 9941 2e14 0400 0000  ].-z.....A......
+000051d0: 9882 652b                                ..e+
```

### Comparing `ctapipe-0.8.0/docs/tutorials/lst_analysis_bootcamp_2018.ipynb` & `ctapipe-0.9.1/docs/tutorials/lst_analysis_bootcamp_2018.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/raw_data_exploration.ipynb` & `ctapipe-0.9.1/docs/tutorials/raw_data_exploration.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996666666666667%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(0, 'event = seeker.get_event_index(0)  # get first "*

 * *            "event\\n')], delete: [0]}}, 13: {'source': {insert: [(0, 'event = "*

 * *            "seeker.get_event_index(1) # get the next event\\n')], delete: [0]}}}"}*

```diff
@@ -62,15 +62,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "event = seeker[0]  # get first event\n",
+                "event = seeker.get_event_index(0)  # get first event\n",
                 "event"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -120,15 +120,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "event = seeker[1] # get the next event\n",
+                "event = seeker.get_event_index(1) # get the next event\n",
                 "print(event.r0.tels_with_data)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `ctapipe-0.8.0/docs/tutorials/theta_square.ipynb` & `ctapipe-0.9.1/docs/tutorials/theta_square.ipynb`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/docs/tutorials/tilted_ground_frame.png` & `ctapipe-0.9.1/docs/tutorials/tilted_ground_frame.png`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/environment.yml` & `ctapipe-0.9.1/environment.yml`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/array_display.py` & `ctapipe-0.9.1/examples/array_display.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/calc_pedestals.py` & `ctapipe-0.9.1/examples/calc_pedestals.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/camera_animation.py` & `ctapipe-0.9.1/examples/camera_animation.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/camera_display_multi.py` & `ctapipe-0.9.1/examples/camera_display_multi.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/camera_norms.py` & `ctapipe-0.9.1/examples/camera_norms.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/camera_rotation.py` & `ctapipe-0.9.1/examples/camera_rotation.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/coordinate_transformations.py` & `ctapipe-0.9.1/examples/coordinate_transformations.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/highlight_pixel.py` & `ctapipe-0.9.1/examples/highlight_pixel.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/instrument_info.py` & `ctapipe-0.9.1/examples/instrument_info.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/load_one_event.py` & `ctapipe-0.9.1/examples/load_one_event.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/plot_all_cameras.py` & `ctapipe-0.9.1/examples/plot_all_cameras.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/plot_array_hillas.py` & `ctapipe-0.9.1/examples/plot_array_hillas.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/plot_camera_frames.py` & `ctapipe-0.9.1/examples/plot_camera_frames.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/plot_hillas_parameters.py` & `ctapipe-0.9.1/examples/plot_hillas_parameters.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/plot_showers_in_nominal.py` & `ctapipe-0.9.1/examples/plot_showers_in_nominal.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/plot_theta_square.py` & `ctapipe-0.9.1/examples/plot_theta_square.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/simple_event_writer.py` & `ctapipe-0.9.1/examples/simple_event_writer.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/stereo_reconstruction.py` & `ctapipe-0.9.1/examples/stereo_reconstruction.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/examples/tool_example.py` & `ctapipe-0.9.1/examples/tool_example.py`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/setup.cfg` & `ctapipe-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ctapipe-0.8.0/setup.py` & `ctapipe-0.9.1/setup.py`

 * *Files identical despite different names*

