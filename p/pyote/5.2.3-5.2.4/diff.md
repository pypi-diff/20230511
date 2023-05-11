# Comparing `tmp/pyote-5.2.3.tar.gz` & `tmp/pyote-5.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyote-5.2.3.tar", last modified: Wed May  3 02:51:35 2023, max compression
+gzip compressed data, was "pyote-5.2.4.tar", last modified: Thu May 11 18:22:27 2023, max compression
```

## Comparing `pyote-5.2.3.tar` & `pyote-5.2.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 02:51:35.614187 pyote-5.2.3/
--rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.2.3/LICENSE
--rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1190 2023-05-03 02:51:35.614187 pyote-5.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.2.3/README.rst
--rw-rw-rw-   0        0        0       80 2023-05-03 02:51:35.618196 pyote-5.2.3/setup.cfg
--rw-rw-rw-   0        0        0     2912 2023-02-11 21:30:43.000000 pyote-5.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:51:35.518649 pyote-5.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 02:51:35.524634 pyote-5.2.3/src/pyote.egg-info/
--rw-rw-rw-   0        0        0     1190 2023-05-03 02:51:35.000000 pyote-5.2.3/src/pyote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1690 2023-05-03 02:51:35.000000 pyote-5.2.3/src/pyote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 02:51:35.000000 pyote-5.2.3/src/pyote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.2.3/src/pyote.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      250 2023-05-03 02:51:35.000000 pyote-5.2.3/src/pyote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 02:51:35.000000 pyote-5.2.3/src/pyote.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 02:51:35.610199 pyote-5.2.3/src/pyoteapp/
--rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.2.3/src/pyoteapp/PYOTE.bat
--rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.2.3/src/pyoteapp/SER.py
--rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.2.3/src/pyoteapp/__init__.py
--rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.2.3/src/pyoteapp/autocorrtools.py
--rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.2.3/src/pyoteapp/blockIntegrateUtils.py
--rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.2.3/src/pyoteapp/checkForNewerVersion.py
--rw-rw-rw-   0        0        0    11897 2023-03-07 02:00:12.000000 pyote-5.2.3/src/pyoteapp/csvreader.py
--rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.2.3/src/pyoteapp/diffraction-table.p
--rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.2.3/src/pyoteapp/errorBarUtils.py
--rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.2.3/src/pyoteapp/example-penumbral.csv
--rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.2.3/src/pyoteapp/exponentialEdgeUtilities.py
--rw-rw-rw-   0        0        0     6829 2022-02-04 15:30:43.000000 pyote-5.2.3/src/pyoteapp/false_positive.py
--rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.2.3/src/pyoteapp/fixedPrecision.py
--rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.2.3/src/pyoteapp/genDiffraction.py
--rw-rw-rw-   0        0        0   371192 2023-04-12 22:16:10.000000 pyote-5.2.3/src/pyoteapp/gui.py
--rw-rw-rw-   0        0        0     2157 2022-07-18 16:06:30.000000 pyote-5.2.3/src/pyoteapp/helpDialog.py
--rw-rw-rw-   0        0        0    25547 2023-05-03 02:37:23.000000 pyote-5.2.3/src/pyoteapp/iterative_logl_functions.py
--rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.2.3/src/pyoteapp/likelihood_calculations.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:51:35.613187 pyote-5.2.3/src/pyoteapp/model-examples/
--rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.2.3/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.2.3/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.2.3/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.2.3/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
--rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.2.3/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.2.3/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.2.3/src/pyoteapp/model-help.pdf
--rw-rw-rw-   0        0        0     1646 2023-05-03 00:27:00.000000 pyote-5.2.3/src/pyoteapp/noiseUtils.py
--rw-rw-rw-   0        0        0   441632 2023-05-03 02:49:09.000000 pyote-5.2.3/src/pyoteapp/pyote-info.pdf
--rw-rw-rw-   0        0        0   428283 2023-05-03 00:27:00.000000 pyote-5.2.3/src/pyoteapp/pyote.py
--rw-rw-rw-   0        0        0    79660 2023-05-03 00:27:00.000000 pyote-5.2.3/src/pyoteapp/pyote_modelling_utility_functions.py
--rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.2.3/src/pyoteapp/run-pyote-mac.bat
--rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.2.3/src/pyoteapp/showVideoFrames.py
--rw-rw-rw-   0        0        0    23481 2023-05-03 00:27:00.000000 pyote-5.2.3/src/pyoteapp/solverUtils.py
--rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.2.3/src/pyoteapp/subframe_timing_utilities.py
--rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.2.3/src/pyoteapp/timestampDialog.py
--rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.2.3/src/pyoteapp/timestampUtils.py
--rw-rw-rw-   0        0        0       34 2023-04-20 22:40:23.000000 pyote-5.2.3/src/pyoteapp/version.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:22:27.879060 pyote-5.2.4/
+-rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.2.4/LICENSE
+-rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1190 2023-05-11 18:22:27.879060 pyote-5.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.2.4/README.rst
+-rw-rw-rw-   0        0        0       80 2023-05-11 18:22:27.883072 pyote-5.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     2912 2023-02-11 21:30:43.000000 pyote-5.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:22:27.849859 pyote-5.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 18:22:27.856060 pyote-5.2.4/src/pyote.egg-info/
+-rw-rw-rw-   0        0        0     1190 2023-05-11 18:22:27.000000 pyote-5.2.4/src/pyote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1690 2023-05-11 18:22:27.000000 pyote-5.2.4/src/pyote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 18:22:27.000000 pyote-5.2.4/src/pyote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.2.4/src/pyote.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      250 2023-05-11 18:22:27.000000 pyote-5.2.4/src/pyote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-11 18:22:27.000000 pyote-5.2.4/src/pyote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 18:22:27.875059 pyote-5.2.4/src/pyoteapp/
+-rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.2.4/src/pyoteapp/PYOTE.bat
+-rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.2.4/src/pyoteapp/SER.py
+-rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.2.4/src/pyoteapp/__init__.py
+-rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.2.4/src/pyoteapp/autocorrtools.py
+-rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.2.4/src/pyoteapp/blockIntegrateUtils.py
+-rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.2.4/src/pyoteapp/checkForNewerVersion.py
+-rw-rw-rw-   0        0        0    11897 2023-03-07 02:00:12.000000 pyote-5.2.4/src/pyoteapp/csvreader.py
+-rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.2.4/src/pyoteapp/diffraction-table.p
+-rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.2.4/src/pyoteapp/errorBarUtils.py
+-rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.2.4/src/pyoteapp/example-penumbral.csv
+-rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.2.4/src/pyoteapp/exponentialEdgeUtilities.py
+-rw-rw-rw-   0        0        0     6829 2022-02-04 15:30:43.000000 pyote-5.2.4/src/pyoteapp/false_positive.py
+-rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.2.4/src/pyoteapp/fixedPrecision.py
+-rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.2.4/src/pyoteapp/genDiffraction.py
+-rw-rw-rw-   0        0        0   371192 2023-04-12 22:16:10.000000 pyote-5.2.4/src/pyoteapp/gui.py
+-rw-rw-rw-   0        0        0     2157 2022-07-18 16:06:30.000000 pyote-5.2.4/src/pyoteapp/helpDialog.py
+-rw-rw-rw-   0        0        0    25547 2023-05-03 02:37:23.000000 pyote-5.2.4/src/pyoteapp/iterative_logl_functions.py
+-rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.2.4/src/pyoteapp/likelihood_calculations.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:22:27.878060 pyote-5.2.4/src/pyoteapp/model-examples/
+-rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.2.4/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.2.4/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.2.4/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.2.4/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
+-rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.2.4/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.2.4/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.2.4/src/pyoteapp/model-help.pdf
+-rw-rw-rw-   0        0        0     1926 2023-05-11 18:15:42.000000 pyote-5.2.4/src/pyoteapp/noiseUtils.py
+-rw-rw-rw-   0        0        0   443122 2023-05-11 18:20:34.000000 pyote-5.2.4/src/pyoteapp/pyote-info.pdf
+-rw-rw-rw-   0        0        0   428283 2023-05-03 00:27:00.000000 pyote-5.2.4/src/pyoteapp/pyote.py
+-rw-rw-rw-   0        0        0    79660 2023-05-03 00:27:00.000000 pyote-5.2.4/src/pyoteapp/pyote_modelling_utility_functions.py
+-rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.2.4/src/pyoteapp/run-pyote-mac.bat
+-rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.2.4/src/pyoteapp/showVideoFrames.py
+-rw-rw-rw-   0        0        0    23481 2023-05-03 00:27:00.000000 pyote-5.2.4/src/pyoteapp/solverUtils.py
+-rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.2.4/src/pyoteapp/subframe_timing_utilities.py
+-rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.2.4/src/pyoteapp/timestampDialog.py
+-rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.2.4/src/pyoteapp/timestampUtils.py
+-rw-rw-rw-   0        0        0       34 2023-05-03 13:43:42.000000 pyote-5.2.4/src/pyoteapp/version.py
```

### Comparing `pyote-5.2.3/LICENSE` & `pyote-5.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/PKG-INFO` & `pyote-5.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.2.3
+Version: 5.2.4
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.2.3/setup.py` & `pyote-5.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyote.egg-info/PKG-INFO` & `pyote-5.2.4/src/pyote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.2.3
+Version: 5.2.4
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.2.3/src/pyote.egg-info/SOURCES.txt` & `pyote-5.2.4/src/pyote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/SER.py` & `pyote-5.2.4/src/pyoteapp/SER.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/autocorrtools.py` & `pyote-5.2.4/src/pyoteapp/autocorrtools.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/blockIntegrateUtils.py` & `pyote-5.2.4/src/pyoteapp/blockIntegrateUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/checkForNewerVersion.py` & `pyote-5.2.4/src/pyoteapp/checkForNewerVersion.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/csvreader.py` & `pyote-5.2.4/src/pyoteapp/csvreader.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/diffraction-table.p` & `pyote-5.2.4/src/pyoteapp/diffraction-table.p`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/errorBarUtils.py` & `pyote-5.2.4/src/pyoteapp/errorBarUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/example-penumbral.csv` & `pyote-5.2.4/src/pyoteapp/example-penumbral.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/exponentialEdgeUtilities.py` & `pyote-5.2.4/src/pyoteapp/exponentialEdgeUtilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/false_positive.py` & `pyote-5.2.4/src/pyoteapp/false_positive.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/fixedPrecision.py` & `pyote-5.2.4/src/pyoteapp/fixedPrecision.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/genDiffraction.py` & `pyote-5.2.4/src/pyoteapp/genDiffraction.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/gui.py` & `pyote-5.2.4/src/pyoteapp/gui.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/helpDialog.py` & `pyote-5.2.4/src/pyoteapp/helpDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/iterative_logl_functions.py` & `pyote-5.2.4/src/pyoteapp/iterative_logl_functions.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/likelihood_calculations.py` & `pyote-5.2.4/src/pyoteapp/likelihood_calculations.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.2.4/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.2.4/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.2.4/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv` & `pyote-5.2.4/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.2.4/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.2.4/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/model-help.pdf` & `pyote-5.2.4/src/pyoteapp/model-help.pdf`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/noiseUtils.py` & `pyote-5.2.4/src/pyoteapp/noiseUtils.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,20 @@
     return np.polyval(poly, x)
 
 
 def getCorCoefs(x, y):
     combo = list(zip(x, y))
     combo.sort()
     yvalsConcat = np.array([item[1] for item in combo])
+
+    # 5.2.4 We can't calculate sigmaA from just two points - we return None and this causes
+    # sigmaA = sigmaB to be executed when the caller finds no sigmaA was returned
+    if len(yvalsConcat) < 3:
+        return np.array([1.0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]), len(x), None
+
     try:
         trend = savgolTrendLine(yvalsConcat, window=301, degree=1)
         residuals = yvalsConcat - trend
     except ValueError:
         return np.array([1.0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]), len(x), 0.0
 
     # We only compute correlation coefficients if there at least 14 data points
```

### Comparing `pyote-5.2.3/src/pyoteapp/pyote-info.pdf` & `pyote-5.2.4/src/pyoteapp/pyote-info.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 5% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,8 +1,13 @@
 Version history (PyOTE description – out of date - is at end)
+Version 5.2.4
+11 May 2023
+• Fixes an edge case – when only two points were in the event bottom, sigmaA was
+being set to 0.0 (causing an assertion error) rather than setting it to the value
+previously determined for sigmaB.
 Version 5.2.3
 2 May 2023
 • Restores the calculation of timeDelta to 6 digit precision (it had been inadvertently
 limited to 4 digits by a previous change)
 •
 
 Fixes a bug in the calculation of flash edge times that was discovered when very high
@@ -38,20 +43,19 @@
 •
 
 At first ‘read’, a list of all available light curves for display is popped up and all the
 ‘signal’ light curves are populated in the light curves list on the Lightcurves tab.
 This was done so that the user is always made aware of the existence of multiple light
 curves read from the csv file.
 
-Version 5.1.6 11 February 2023
+Version 5.1.6 11 February 2023
 • Fixes VizieR file preparation code to detect when lat or long is given with a + sign
 (common when input comes from reading a .xlsx file)and avoid adding a redundant +
 (double) character.
-
-•
+•
 
 Reverts to using pyqtgraph 0.12.4
 
 Version 5.1.0 7 February 2023
 • Changed the way data sets (lightcurves) read from a PyMovie csv file are selected for
 viewing. Whereas previously it was possible to specify a ‘prefix’ to be used when
 reading PyMovie csv files (such as ‘signal’ or ‘appsum’), it was not possible to mix-andmatch data sets with different prefixes. With this version, that now becomes possible.
@@ -86,22 +90,26 @@
 • Fixes squarewave solution display to (once again) honor the checkboxes that control
 camera response, raw light, and edge plotting.
 •
 
 Adds a tab for exporting VizieR archive lightcurves
 
 Version 5.0.3 9 January 2023
-• model-examples folder is now being placed in the Documents folder rather than the
+
+•
+
+model-examples folder is now being placed in the Documents folder rather than the
 Desktop folder.
+
 •
 
 Launch from python3 or python or py now detected and dealt with when checking PyPI
 repository for latest version.
 
-Version 5.0.2 8 January 2023
+Version 5.0.2 8 January 2023
 • Added timing problem report – counts of dropped readings; duplicated readings;
 cadence error. These appear in the log box (lower right corner) and are written to the
 log file.
 •
 
 Made D and R edge time calculations work properly even when there are dropped
 readings in the observation
@@ -130,21 +138,21 @@
 • Added a button to the diffraction tab for use during penumbral fits to do a re-fit.
 Improved (hopefully) the context help regarding the selection of D and R regions for a
 penumbral fit (cautioning the user to only include points from the penumbral transition).
 Version 4.8.9 8 August 2022
 • Timestamp error lines now distinguish between 'cadence jitter' and 'dropped frames' by
 using an additional color.
 Cadence jitter happens when high frame rates create a situation where frame recording cannot keep up and the traffic control implemented by the computer changes the
-arrival/timestamp time of frames so that some appear a little earlier and others a little
+
+arrival/timestamp time of frames so that some appear a little earlier and others a little
 late.
 Cadence jitter is defined as a timing discrepancy of between 20% and 80% of a frame
 time and is represented by a yellow line.
 Timing discrepancies greater than 80% of a frame time continue to be shown as a red
-
-line and are assumed to come from dropped frames. In any case, they deserve
+line and are assumed to come from dropped frames. In any case, they deserve
 attention.
 Version 4.8.8 7 August 2022
 • Added message at normal program close to the effect that QBasicTimer messages
 that appear after the program has closed are harmless artifacts of the order in which
 QUI elements are closed.
 Version 4.8.7 29 July 2022
 • changed numpy version requirement to match that of PyMovie so that ultimately the
@@ -170,24 +178,24 @@
 •
 
 makes pyote install for new version update use pipenv if present
 
 Version 4.8.0
 • adds PyQt5 to list of required packages in support of using pipenv to install PyOTE
 without the need for an Anconda3 installation.
-•
+
+•
 
 removes the writing of the startup batch file as a different method will be used in
 conjunction with pipenv.
 
 Version 4.7.9
 • disables the compiling to C code (which was done to increase execution speed) of
 routines used for finding an event using min/max size. There is compelling (but
-
-indirect) evidence that the C compiler on Win11 (and maybe only for the i5 processor)
+indirect) evidence that the C compiler on Win11 (and maybe only for the i5 processor)
 is generating incorrect code. This issue showed up recently with 2 users who had
 installed Win11 on i5 processor-based computer. On those machines, finding an event
 using min/max would always hang at 99% completion. Allowing the original Python
 code to be used instead of compiling to C-code resolved that issue. As finding an event
 using min/max size minimizes the number of candidate solutions naturally, the loss of
 speed is not so important – it’s fast enough.
 version 4.6.4
@@ -220,23 +228,20 @@
 • suppressed a 'min event limit too high' message when min event is set to lowest
 possible value of 2
 version 4.5.6
 • removed the 'busy code' which changed the mouse cursor to “I'm busy”. This seems to
 have the side effect (on some computers – but none of mine) of suppressing the cursor
 change when hovering over a splitter. As this is confusing, the busy cursor feature has
 been removed.
-version 4.5.5
+
+version 4.5.5
 • fixes a bug where, if a full D and R light-curve was split (trimmed) into a D-only and an
 R-only light-curve, the R-only result did not apply subframe timing adjustments
 version 4.5.4
-
-•
-
-cleans up the the first bin of the False-Positive histogram
-
+• cleans up the the first bin of the False-Positive histogram
 version 4.5.3
 • adds an option to validate a single point event to the Analysis tab. It uses the falsepositive test procedure to determine if the selected point had a non-zero chance to
 have been caused by baseline noise alone.
 version 4.5.2
 • fixes a bug where transition points (only present in high SNR light-curves) were not
 properly ignored during calculation of event noise. This manifested itself most clearly in
 too large error bars for magDrop
@@ -259,40 +264,37 @@
 *.normalization.PYOTE.log
 version 4.3.8
 • suppressed writing of detectability results and normalization activities to the log file.
 The 'writings' still appear in the normal place, they just don't get written to the log file.
 (Later I may direct such stuff to a separate log file.)
 version 4.3.7
 • removed the Pearson R metric – it was confusing and ineffective compared to the
-simple standard deviation metric
+
+simple standard deviation metric
 •
 
 made it possible to select the points of the normalized target lightcurve to be included
 in the std metric
 
 version 4.3.6
-
-•
-
-added a simple metric as an aid to selecting an appropriate number of readings to use
+• added a simple metric as an aid to selecting an appropriate number of readings to use
 to smooth the reference curve used for normalization. It is printed in green whenever
 normalization is active. It is simply the standard deviation of the normalized target
 lightcurve. Although it is quite simple, it is a value that is minimized the more level and
 the less bumpy the normalized target curve is.
 When normalization is active, at each change, a pair of metrics are printed in the log
 panel.
 The red metric is the Pearson R value of the correlation between the target lightcurve
 and the reference lightcurve; it should be maximized (using the X offset spinbox of the
 reference curve) at the point where the two curves are properly time-aligned. It is also
 affected by the smoothing interval, but this connection should be ignored.
 The green metric is the standard deviation of the target lightcurve – it is lowered when
 the target lightcurve has a minimum slope and the fewest and shallowest bumps. Use
 the spinbox for the number of readings in the smoothing interval to minimize this
 number.
-
 version 4.3.5
 • made the 'step-by' buttons radio buttons so that it is clear what the current step size is.
 •
 
 removed the automatic switch to the Lightcurve panel
 
 version 4.3.3
@@ -308,23 +310,20 @@
 
 activates the 'show' checkbox on reference curves so that the reference curve display
 can be turned off – but it will still be active behind the scenes, just not visible.
 
 version 4.3.1
 • fixes an error message that occurs during the initial installation of a version that has a
 change to the number of tabs in the GUI
-version 4.3.0
+
+version 4.3.0
 • minor cosmetic cleanup to deal with Windows GUI differences (I hope it works – this is
 always a frustrating and mysterious area)
 version 4.2.9
-
-•
-
-adds the lightcurve used to the report generated during the detectability analysis
-
+• adds the lightcurve used to the report generated during the detectability analysis
 •
 
 automatically clears the effect of previous normailzation when the reference lightcurve
 is changed (or deselected)
 
 version 4.2.8
 • fixes 'trim problem'
@@ -366,20 +365,20 @@
 •
 
 adds logging/reporting of the curve (if any) used for normalization and the smoothing
 interval used.
 
 version 4.2.2
 • adds a new tab/panel for controlling the display of lightcurves. From the 'help button'
-on that tab:
+
+on that tab:
 This panel allows up to 10 lightcurves to be displayed at the same time. If the csv file has
 more than 10 lightcurves, the first 10 are displayed.
 The target lightcurve is always drawn with bright blue dots.
-
-If a lightcurve is selected as a reference to be used for normalization, it is always
+If a lightcurve is selected as a reference to be used for normalization, it is always
 drawn with bright green dots.
 Unless a lightcurve is designated as a target (curve to be analyzed for an event) or is
 designated as a reference lightcurve, its dot color depends on the row it is in - every
 row has a unique color other than blue or green.
 Lightcurves can be displaced up or down using the Y offset spinner to control the
 displacement. This affects the display position only; the underlying values are not
 affected. This facility was added to allow the separation of lightcurves that would
@@ -413,23 +412,20 @@
 
 eliminates the display of negative drops in the False-Positive histogram
 
 version 4.1.9
 • fixes (hopefully) Win 11 issue involving the directory separator character \
 Win 10 accepts / as a separator – Win 11 apparently does not (unless there is some
 setting that will persuade Win 11 to accept either separator.
-version 4.1.8
+
+version 4.1.8
 • adds option to write sample light-curve from detectability analysis to a csv file that be
 imported to PyOTE.
 version 4.1.7
-
-•
-
-adds the requirement to specify an observation duration when doing a detectability test
-
+• adds the requirement to specify an observation duration when doing a detectability test
 •
 
 during a detectability test, if a detectable event was found, a sample light-curve
 showing such an event is plotted, otherwise the normal False-Positive plot will be
 shown.
 
 version 4.1.6
@@ -475,29 +471,29 @@
 
 •
 
 The noise reduction is not without a small cost however - the edges of an occultation
 light-curve will no longer be a step change. Instead, the edges will follow an
 exponential curve, approaching maximum and minimum intensities asymptotically.
 PyOTE has the ability to fit such an exponential curve to the D and R transitions, so the
-time resolution will be restored during the least squares fit and you should feel free to
+
+time resolution will be restored during the least squares fit and you should feel free to
 use whatever level of noise reduction you may need. It is recommended that you run
 your NE3 at a gamma of 0.75 (1.0 gamma is not available) AND that you use PyMovie
 to linearize the recording (i.e., invert the 0.75 gamma curve of the camera).
-
 •
 
 The D and R exponential curves each have their own time constant, measured in
-
-frames, that control the frame rate of exponential curve growth. The default values
+frames, that control the frame rate of exponential curve growth. The default values
 provided are usually enough to provide the starting point for a good fit. This starting
 point is used by PyOTE during a least-squares driven search for better time constant
 values. If the starting point given is too far from 'correct', the least-squares search may
 settle in a local minimum that produces a fit that is visually bad. In this case, change
 the starting value to something closer to 'correct' and try again.
+
 •
 
 When the exponential curve fit algorithm is in use, the light-curve plot PyOTE displays
 will be changed. Gone is the blue 'camera response' curve, replaced by brown dotted
 'theoretical' exponential edge curves that you can use to judge for yourself the
 goodness of a 'fit'.
 
@@ -527,21 +523,21 @@
 propagate those errors through the ratio A/B to get its error bars and then through the
 ln() function to get the final error bars. The equations I use were verified through
 simulations.
 version 4.0.9
 • fixes issue where PyOTE could not read files that it had written.
 version 4.0.8
 • fixes bug (introduced by a misspelling in version 4.0.7) that kept csv files with more
-than four apertures from runnig.
+
+than four apertures from runnig.
 version 4.0.7
 • adds the ability to select the PyMovie data column type to be analyzed. There are two
 main column types that are likely to be used: signal, which has background subtracted
 and appsum, which has no background subtracted – it's the raw mask pixels summed.
-
-Some others are available: avgbkd (shows the average pixel value in the aperture);
+Some others are available: avgbkd (shows the average pixel value in the aperture);
 stdbkg (shows the pixel noise in the background pixels in the aperture); nmaskpx
 (which shows the nuber of pixels in the sampling mask – there are times when this
 curve can be used to extrat event times).
 Note: this only applies to csv files generated by PyMovie.
 version 4.0.6
 • minor GUI changes
 version 4.0.5
@@ -574,21 +570,24 @@
 
 The 'selected curve to analyze' number and the 'curve to normalize' number are now
 allowed to be the same – no funny jumping around.
 It is even possible to normalize a curve against itself. There may be a use case where
 this is useful, so I didn't lock it out.
 
 version 4.0.2
-• removed a debug print statement that was inadvertently left in. It is responsible for the
+
+•
+
+removed a debug print statement that was inadvertently left in. It is responsible for the
 “mouse event” messages polluting the log file.
+
 version 4.0.1
 • increased width of detectibility plots to (hopefully) deal with Windows tendency to
 truncate the plots. If this doesn't work, then this will be a permanent feature (not a bug)
-
-for Win10 installations.
+for Win10 installations.
 version 4.0.0
 • detectibility graphics plots are now being being put in their own folder. The root folder is
 that of the directory where the light-curve came from. The plots will be found in
 lightCurveDirectory\DetectibilityPlots\
 In addition, if you supply a duration step size, which is the way to ask the detectibilty
 calculator to step from the given duration down until an event of that duration fails the
 False-positive test, only the final plot (where False-positive became non-zero) will be
@@ -614,21 +613,21 @@
 simple-ote-ini file that preserves the 'sticky' values like size and position of the gui and
 a few other things.
 This version refuses to read any existing .ini files. Hopefully you will be able to run the
 program, but nothing will be 'sticky'.
 If this 'cures' the problem, I can restore the use of the .ini file and we can get back the
 sticky stuff.
 This version also removes the 'scrunch' of the lefthand button panel.
-version 3.9.6
+
+version 3.9.6
 • another attempt fix the startup gui size issue on smaller legacy monitors. This version
 has a design size of 1900x1000. It may be necessary to delete the simple-ote.ini file
 that 'remembers' size and position settings. It is located in whatever directory PyOTE
 starts up in.
-
-version 3.9.5
+version 3.9.5
 • adds automation to the 'detectibility' calculator. If a duration step size is entered, a
 series of 'detectibility' calculations will be made at decreasing durations until the falsepositive probability becomes non-zero. A unique .png (incorporates duration and
 magDrop in the file name) will be written to the directory of the light-curve and the final
 plot where detection failed will be left on-screen.
 If the duration step size is left unfilled or is zero, a single 'detectibility' calculation will be
 made as before.
 version 3.9.4
@@ -653,21 +652,21 @@
 experiment.
 version 3.8.9
 • Changed the label on the Write csv file button to Save current light-curve to more
 intuitively suggest what is hiding behind this button.
 version 3.8.8
 • fixed a bug that sometimes kept events that contained a single point at the bottom from
 producing a report.
-version 3.8.7
+
+version 3.8.7
 • changed the way curve to analyze and normalization curve are selected to make it less
 confusing. Now, if there is a conflict (same curve selected for analysis and
 normalization) the other one is set to 0 (a new value) to 'get it out of the way'. It may
 still be a little bit confusing when you need to crossover, but if you set the higher
-
-numbered curve first, it will be easy.
+numbered curve first, it will be easy.
 version 3.8.6
 • checks for only a single light-curve in the csv file which was causing a 'list index out of
 range' error message
 version 3.8.5
 • changed the way QGridLayout was referenced.
 version 3.8.4
 • changed the way QTableWidgetItem and QApplication were referenced to
@@ -695,20 +694,20 @@
 version 3.7.9
 • adds a tool that allows a user to manually specify which baseline points to use for the
 calculation of B (baseline mean) baseline noise (sigmaB) and noise correlation
 coefficients. This was added primarily to support GPS-flash-tagged light-curves where
 the flash itself adversely affects the baseline values. With this new tool, the regions of
 the baseline that are outside the 'flash-zone' can be specified. Look for a button
 labelled Mark baseline region located near the bottom-left of the GUI panel.
-This tool may also be useful for wind-gust situations, headlights from passing cars,
+
+This tool may also be useful for wind-gust situations, headlights from passing cars,
 bumping the telescope, etc. In the past, such accidents might have required extensive
 'clipping' of the light-curve to avoid the affected areas, with a consequent loss of
 information. Hopefully this tool will alleviate those situations.
-
-version 3.7.8
+version 3.7.8
 • added visible left, top, and bottom axes to main plot (with ticks to make easier to
 associate timestamp with point).
 version 3.7.7
 • if timestamps are available in the csv file, they are used as x axis labels in the main
 plot.
 version 3.7.6
 • changed the way QMainWindow and Qapplication were referenced to accommodate
@@ -735,20 +734,20 @@
 was a ‘feature’ of the routine that saved this information that, in the interest of
 efficiency, it would sometimes not write a new folder name to the ‘sticky file’ until
 later – the fix was to force it to update the ‘sticky file’ on every change)
 version 3.7.3
 • adds code line needed by any Mac users that are running Big Sur
 version 3.7.2
 • fixes bug that caused all analysis attempts to 'stall'
-version 3.7.1
+
+version 3.7.1
 • fixed a bug in the r limb angle entry
 version 3.7.0
 • adds right-click help to ast speed label giving the equation to use if asteroid
-
-speed is not available but asteroid diameter and maximum duration are
+speed is not available but asteroid diameter and maximum duration are
 specified
 •
 
 adds suggestion to right-click help on penumbral fit checkbox for how to find the
 penumbral curve csv file that is provided for practice purposes.
 
 version 3.6.8
@@ -774,21 +773,21 @@
 version 3.6.2
 • In Excel report:
 … at end of filling, I call the OS to open the file. Requires correct association
 of .xlsx file type with Excel or LibreOffice, or whatever you use to examine
 spreadsheets
 … now writing numbers into numeric cells rather than text. This allows the cell
 formatting to control rounding, etc
-… if I can't write to the selected file, I ask whether you might have it open
+
+… if I can't write to the selected file, I ask whether you might have it open
 somewhere else already
 version 3.6.1
 • reduced number of digits in the error bar numbers to 2 written to the Asteroid
 Occultation Report Form so that the resulting number fits within the allotted cell
-
-size. (I'm told that Occult only uses 2 digits anyway.) I also updated the context
+size. (I'm told that Occult only uses 2 digits anyway.) I also updated the context
 help associated with the … fill Excel report button
 version 3.6.0
 • provides the ability to fill entries in the Excel spreadsheet Asteroid Occultation
 Report Form from PyOTE results, thus eliminating transcription errors.
 A button to allow the user to activate this 'fill' has been added just to the right of
 
 the … write report button
@@ -808,26 +807,23 @@
 ...nominal magDrop (entered in Comments cell of the spreadsheet).
 NOTE: you must still open the spreadsheet and enter the exposure setting used for your
 camera; it was not possible to do this from PyOTE.
 After filling in the exposure setting in the spreadsheet, double check the form but it is likely
 that it is ready for submission.
 version 3.5.9
 • fixed another bug in penumbral curve fit and removed diagnostic printouts.
-version 3.5.8
+
+version 3.5.8
 • fixed a number of bugs in the penumbral curve fit code
 version 3.5.7
-
-•
-
-automatically turns off the display of the normalizing lightcurve when a
+• automatically turns off the display of the normalizing lightcurve when a
 normalization is performed. It was a source of confusion to leave the normalizing
 lightcurve visible because it was sometimes the case that the normalization
 appeared not to have occurred (when the normalization effect was
 subtle/minor).
-
 version 3.5.6
 • fixed a bug that kept a user from selecting a new file to read if PyOTE had been
 started from PyMovie. Previously, it had only reopened the same file instead of
 giving the user a file select dialog to choose from.
 version 3.5.5
 • fixed a bug that kept occultations from being extracted from lightcurves 5 and
 up. The lightcurves above 4 could be viewed --- they just couldn't be processed
@@ -852,20 +848,20 @@
 unexpectedly and unrealistically.
 Previously PyOTE treated this as a cosmetic problem and relied on the observer
 to be aware of the end point effects and ignore them. But that puts a burden on
 the user to be well informed about what's going on. As one of the goals of
 PyOTE is to enable infrequent/inexperienced users to get dependable results
 without requiring in-depth understanding of the internal workings of the program,
 we have decided to make the end-point smoothing issue very apparent by doing
-an automatic 'trim' of the points affected by extrapolation.
+
+an automatic 'trim' of the points affected by extrapolation.
 version 3.5.1
 • Added additional references to the North American Excel Spreadsheet report in
 the new section of the final report that bangs on about the start-of-exposure
-
-timing convention.
+timing convention.
 version 3.5.0
 • When PyMovie files are read, the aperture names are now being used in the
 data table (lower left panel) as column headings and used during the 'write csv'
 process. This makes the format of the PyOTE csv file match the PyMovie
 format so that AOTA can read both PyMovie csv files AND PyOTE csv files.
 •
 
@@ -898,19 +894,19 @@
 more and more as A approaches and then becomes smaller than std(A). For example, if A
 happened to be equal to std(A), the normal distribution of A values tells us that 84% of
 possible A values are > 0 and so can be used in the regular magDrop equation. The other
 16% of the time we can only report that the calculation could not be performed.
 The above observation suggests that reliable estimates of magDrop require that A be greater
 than std(A) --- that is the ad hoc reason that we have defined limMagDrop as we have.
 This value is substituted for a calculated magDrop whenever A is less than std(A), i.e.,
-whenever A is at or below std(A).
+
+whenever A is at or below std(A).
 limMagDrop values are reported with a leading > symbol to signify that that value is a
 limMagDrop value. They are easy to spot in the report.
-
-version 3.4.7
+version 3.4.7
 • Automatically loads the correct version of Adv2
 version 3.4.6
 • Adds AAV Version 2 file as a type that can be read (important when Do OCR
 check is enabled)
 version 3.4.5
 • Fixes block integration which was failing when more than 4 lightcurves were
 being processed.
@@ -938,23 +934,24 @@
 user can adjust for the resolution of the screen in use. I design on a 5120x2880
 screen and needed lines to be 3 pixel wide to suit my taste. But some users
 have screens with 1280 horizontal resolution and those same 3 pixels became
 unsightly fat lines --- now there's a choice.
 version 3.4.1
 • Some cosmetic changes: thinner vertical thins for edge position and error bars;
 checkboxes to control whether the underlying lightcurve is plotted, error bars are
-plotted, or edges are plotted --- a cleaner plot is the major result and you have
+
+plotted, or edges are plotted --- a cleaner plot is the major result and you have
 better control over the 'look'
 •
 
 Added a checkbox to disable the automatic display of D and R frames from the
 video for OCR quality control checks. When there are no concerns about OCR
-
-reliability (true for me nearly all the time), it can be annoying to have to close the
+reliability (true for me nearly all the time), it can be annoying to have to close the
 frames all the time.
+
 •
 
 The BIG change is the addition of a penumbral curve fit procedure. It's a bit
 fiddly, so I included a test lightcurve with the download. I can't give you a
 specific location for the file because it depends on details of your particular
 installation. Find where it is by searching for example-penumbral.csv When
 you find it, copy or move it to some other folder because if you process it where
@@ -982,20 +979,20 @@
 version 3.3.7
 • A new button (View frame) with an associated spinner for entry of a frame
 number has been added:
 Use this button to view a frame from the video that was used by PyMovie or Limovie to
 prepare the .csv file that is currently being analyzed. .avi and .ser files are viewable in
 this manner as well as .fits files inside a FITS folder.
 If this button is disabled, it is because the .csv file did not come from PyMovie or
-Limovie or simply cannot be found/opened.
+
+Limovie or simply cannot be found/opened.
 This feature can/should be used as a final quality control check for a video that
 contains timestamps extracted using OCR. It is possible for OCR to fail in manner that
 is not detected by PyOTE because the program only verifies that there is a consistent
-
-step (delta time) between frames. If a high order digit in the timestamp has been
+step (delta time) between frames. If a high order digit in the timestamp has been
 consistently misread, substituting a 8 for a 9 in the minutes field for example, the steps
 can be consistent while the reported time of the event will be seriously in error.
 ALL time reporting is derived from the timestamp(s) associated with D and/or R (the
 integer values, not the sub-frame values). If those timestamps are correct, the reported
 times will be correct even when there may be a few missing or duplicated frames. So
 best practice is to enter the D frame value in the spin box and visually confirm that the
 timestamp that you can see is the same as that extracted by the OCR procedure.
@@ -1023,20 +1020,20 @@
 greater than or equal to the drop value extracted from the actual observation.
 version 3.3.1:
 • Adds a 'false positive' detection to the final report. A new plot has been added
 to the error bar plot. It shows the distribution of drop sizes (B-A) for an event of
 the size (duration) extracted from the actual observation, but with only correlated
 noise in the sample (the number of points in this sample is equal to the number
 of points used in the lightcurve extraction). 50,000 attempts are made to find
-the deepest event that appears (falsely) when there is only noise being
+
+the deepest event that appears (falsely) when there is only noise being
 analyzed. If the drop from the actual observation is greater than the maximum
 size of a 'false drop', we have some assurance that the event extracted from the
 actual observation did not happen 'by chance'.
-
-version 3.2.9
+version 3.2.9
 • Changed main plot so that the scroll wheel only zooms the x axis.
 • Changed lightcurve plot so that it conforms properly to 'start-of-exposure'.
 version 3.2.8
 • Changed font size in help files --- it was fine for Mac but too big for Win10
 version 3.2.7
 • Removed the 'hover-for-help' and replaced it with a 'right-click-on-item' to get
 help. This scheme was introduced in PyMovie and I found it easier to use than
@@ -1065,21 +1062,22 @@
 returned by pip 18.1 and pip 19.0+
 • Added ability to invoke PyOTE from PyMovie with an externally supplied csv file
 that is automatically opened.
 version 3.2.3
 • fixed a long overlooked bug in the loading of the data table (at lower left corner
 of GUI): when there are four lightcurves, LC4 was set in the table from LC3 (i.e.,
 LC3 == LC4 whenever there was an actual LC4. It was correct in the lightcurves
-themselves, so no observation analyses have been affected by this bug. It was
+
+themselves, so no observation analyses have been affected by this bug. It was
 cosmetic only.
 •
 
 Added support for the PyMovie csv format
 
-version 3.2.1
+version 3.2.1
 • this version makes PyOTE more robust to a common 'cockpit error' that users
 have been making with Tangra files. Specifically, if a Tangra csv file is opened
 in a spreadsheet program, then saved from that spreadsheet program, the
 original csv file gets modified and overwritten by the addition of empty fields at
 every row sufficient to match the number of columns in the longest
 header/comment row --- the spreadsheet program did this to satisfy its internal
 requirement that every row have an equal number of columns. The result is
@@ -1109,26 +1107,29 @@
 
 version 3.1.6:
 • Values entered in the Manual Timestamp Entry dialog box are now 'sticky', thus
 making corrections easy to do without requiring re-entry of all data.
 Also trapped is the case where a user has entered a custom frame time but failed to click the
 radio button indicating that it is to be used.
 version 3.1.5:
-• Added additional tests of candidate solutions against a straight line so that there
+
+•
+
+Added additional tests of candidate solutions against a straight line so that there
 should always be agreement between a solution found by a min/max event size
 search and a marked D and R region search of the same area.
-
-Previously it was possible for the min/max search, which searches the entire
+Previously it was possible for the min/max search, which searches the entire
 light curve, to be tripped up by what we call a 'competitor'. A 'competitor' is an
 'event' with good statistics. However, that 'competitor' may have a small
 magDrop and so later be rejected when we compare with a straight line solution.
 That 'competitor' would thus mask an event with slightly worse statistics but a
 larger magDrop. The change was to test every candidate against a straight line
 during the search. This does make the search time longer, but not too much
 longer.
+
 version 3.1.4:
 • Fixed error in new dropped reading detection logic when light curve was
 processed in field mode.
 •
 
 Cleaned up some language in tooltips.
 
@@ -1159,23 +1160,24 @@
 either of those standards.
 version 3.1.1:
 • A convenient way to search for a 'solution' is to set a min and max event size
 rather than mark D and R regions. This is particularly useful in low snr
 situations where the D and R edges may be quite diffuse. However, if one sets
 the min event too large or the max event too small, the resulting 'solution' will be
 artificially constrained and thus be wrong. This situation is now detected and a
-log entry as well as a pop-up alert will tell the user to change the limits and try
+
+log entry as well as a pop-up alert will tell the user to change the limits and try
 again.
 •
 
 Three magDrop values are now calculated for each confidence level: the largest
-
-magDrop calculated using B + err(B) along with A – err(A); the nominal
+magDrop calculated using B + err(B) along with A – err(A); the nominal
 magDrop calculated using B and A; the minimum magDrop calculated using
 B – err(b) along with A + err(A)
+
 •
 
 The labels on the Find Event button and the Calc Err Bar button were changed
 to more clearly suggest that after finding an 'event', one should then press the
 'report' button to the right in order to complete the process.
 
 version 3.1.0:
@@ -1204,19 +1206,22 @@
 with archived Anaconda3 versions.
 version 2.1.6:
 • We now disable the Accept integration button on the first left click in the light
 curve. As such a click removes the color bars that result from the automatic
 block integration analysis, it seems intuitive to disable the Accept integration
 button at that time as well.
 version 2.1.5:
-• Disable the Accept integration button when user overrides an automatic block
+
+•
+
+Disable the Accept integration button when user overrides an automatic block
 analysis with a manual block selection followed by a click on the Block integrate
 button.
 
-version 2.1.4:
+version 2.1.4:
 • Corrected a bug that kept manual selection of block integration from being
 performed after a refusal to accept the automatic block analysis results.
 version 2.1.3:
 • A minor change to how color bars are plotted when the automatic block
 integration feature is employed. The edges now appear between data points so
 the bands are easier to see, particularly for 2 point block sizes.
 version 2.1.2:
@@ -1245,26 +1250,25 @@
 numbers that can result from field processed csv files
 • Flash timing has been verified to work with integrated light curves
 • Made block integration 'sticky' in that a 'Start over' no longer undoes a previous
 block integration. As a result, once block integration has been performed after a
 file read, it cannot be done again; a reread of the original file is now required.
 version 2.0.7
 This version provides several features to ease the processing of light curves that are
-timed with LED flashes from iPhones (John Grismore's AstroFlashTimer) or Android
+
+timed with LED flashes from iPhones (John Grismore's AstroFlashTimer) or Android
 phones (Eric Couto's Occult Flash) rather than VTI timestamped files
 •
-
-Adds a button to calculate the edge position of an LED timing flash.
-
-•
+•
 
 •
 •
 •
 
+Adds a button to calculate the edge position of an LED timing flash.
 Adds a checkbox to enable/disable the tooltip messages that appear when a
 control is hovered over. Tooltip display defaults to 'enabled' because tooltips are
 an important aid for guiding users initially. Later, when such help is no longer
 needed, the user can turn them off (they are annoying when you don't need
 them).
 Adds the ability to select which light curve is to be analyzed. Previous versions
 would only analyze the first light curve for D and R events. This flexibility is
@@ -1299,17 +1303,17 @@
 version 2.0.3
 • detects and handles situations in which fewer than 14 baseline points are
 available for calculation of correlated noise coefficients. When fewer than 14
 points are available, the correlation coefficients are set to: [1, 0, …] (i.e.,
 coefficients are set to 'no correlated noise')
 version 2.0.2
 • Note: this version has many significant changes. If you lose confidence in this
-version, remember that you can always go back to version 1.47 by typing --pip install pyote==1.47
 
-in an Anaconda console. (Be sure to use double == signs in the command.)
+version, remember that you can always go back to version 1.47 by typing --pip install pyote==1.47
+in an Anaconda console. (Be sure to use double == signs in the command.)
 •
 
 improved handling of D and R region selection so that one cannot enter an
 invalid configuration --- automatic corrections/changes are applied.
 
 •
```

### Comparing `pyote-5.2.3/src/pyoteapp/pyote.py` & `pyote-5.2.4/src/pyoteapp/pyote.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/pyote_modelling_utility_functions.py` & `pyote-5.2.4/src/pyoteapp/pyote_modelling_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/showVideoFrames.py` & `pyote-5.2.4/src/pyoteapp/showVideoFrames.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/solverUtils.py` & `pyote-5.2.4/src/pyoteapp/solverUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/subframe_timing_utilities.py` & `pyote-5.2.4/src/pyoteapp/subframe_timing_utilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/timestampDialog.py` & `pyote-5.2.4/src/pyoteapp/timestampDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.3/src/pyoteapp/timestampUtils.py` & `pyote-5.2.4/src/pyoteapp/timestampUtils.py`

 * *Files identical despite different names*

