# Comparing `tmp/mmcb-avt-0.0.77.tar.gz` & `tmp/mmcb-avt-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.77.tar", last modified: Wed May 10 15:13:50 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.78.tar", last modified: Thu May 11 07:41:14 2023, max compression
```

## Comparing `mmcb-avt-0.0.77.tar` & `mmcb-avt-0.0.78.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-10 15:13:50.133997 mmcb-avt-0.0.77/
--rw-r--r--   0 avt       (1000) avt       (1000)    13827 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/LICENSE
--rw-r--r--   0 avt       (1000) avt       (1000)     8108 2023-05-10 15:13:50.129997 mmcb-avt-0.0.77/PKG-INFO
--rw-r--r--   0 avt       (1000) avt       (1000)     6885 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/README.md
--rw-r--r--   0 avt       (1000) avt       (1000)      104 2023-01-25 09:49:54.000000 mmcb-avt-0.0.77/pyproject.toml
--rw-r--r--   0 avt       (1000) avt       (1000)       38 2023-05-10 15:13:50.133997 mmcb-avt-0.0.77/setup.cfg
--rw-r--r--   0 avt       (1000) avt       (1000)     2591 2023-05-10 15:03:35.000000 mmcb-avt-0.0.77/setup.py
-drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-10 15:13:50.113998 mmcb-avt-0.0.77/src/
-drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-10 15:13:50.125997 mmcb-avt-0.0.77/src/mmcb/
--rw-r--r--   0 avt       (1000) avt       (1000)        0 2023-01-25 09:49:54.000000 mmcb-avt-0.0.77/src/mmcb/__init__.py
--rw-r--r--   0 avt       (1000) avt       (1000)    93094 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/common.py
--rw-r--r--   0 avt       (1000) avt       (1000)    32486 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    14416 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)     9078 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    33679 2023-05-09 15:58:31.000000 mmcb-avt-0.0.77/src/mmcb/detect.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)     6415 2023-05-10 15:10:15.000000 mmcb-avt-0.0.77/src/mmcb/dmm.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)   112129 2023-01-25 09:49:54.000000 mmcb-avt-0.0.77/src/mmcb/iv.py
--rw-r--r--   0 avt       (1000) avt       (1000)    23744 2023-05-10 15:00:25.000000 mmcb-avt-0.0.77/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    12231 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)     7040 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)     7889 2023-01-25 09:49:54.000000 mmcb-avt-0.0.77/src/mmcb/peltier.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    33621 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/psuset.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    21883 2023-01-25 09:49:54.000000 mmcb-avt-0.0.77/src/mmcb/psustat.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    13517 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/sense.py
--rw-r--r--   0 avt       (1000) avt       (1000)    40226 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/sensors.py
--rw-r--r--   0 avt       (1000) avt       (1000)    17705 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/sequence.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    17659 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/ult80.py
-drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-10 15:13:50.129997 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt       (1000) avt       (1000)     8108 2023-05-10 15:13:50.000000 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt       (1000) avt       (1000)      622 2023-05-10 15:13:50.000000 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt       (1000) avt       (1000)        1 2023-05-10 15:13:50.000000 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt       (1000) avt       (1000)      330 2023-05-10 15:13:50.000000 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt       (1000) avt       (1000)      226 2023-05-10 15:13:50.000000 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt       (1000) avt       (1000)        5 2023-05-10 15:13:50.000000 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 07:41:14.080617 mmcb-avt-0.0.78/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.78/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     8108 2023-05-11 07:41:14.079782 mmcb-avt-0.0.78/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     6885 2023-03-06 09:10:49.000000 mmcb-avt-0.0.78/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.78/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-11 07:41:14.080801 mmcb-avt-0.0.78/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-11 07:40:01.000000 mmcb-avt-0.0.78/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 07:41:14.030484 mmcb-avt-0.0.78/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 07:41:14.072147 mmcb-avt-0.0.78/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.78/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    93094 2023-03-08 11:04:09.000000 mmcb-avt-0.0.78/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.78/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.78/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.78/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33679 2023-05-10 15:18:59.000000 mmcb-avt-0.0.78/src/mmcb/detect.py
+-rwx------   0 avt        (501) staff       (20)     2096 2023-05-11 07:36:55.000000 mmcb-avt-0.0.78/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4178 2023-05-11 07:39:08.000000 mmcb-avt-0.0.78/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.78/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    23750 2023-05-11 07:13:26.000000 mmcb-avt-0.0.78/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.78/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.78/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.78/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.78/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.78/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.78/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.78/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.78/src/mmcb/sensors_mod.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.78/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.78/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 07:41:14.078570 mmcb-avt-0.0.78/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     8108 2023-05-11 07:41:14.000000 mmcb-avt-0.0.78/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      672 2023-05-11 07:41:14.000000 mmcb-avt-0.0.78/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-11 07:41:14.000000 mmcb-avt-0.0.78/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-11 07:41:14.000000 mmcb-avt-0.0.78/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-11 07:41:14.000000 mmcb-avt-0.0.78/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-11 07:41:14.000000 mmcb-avt-0.0.78/src/mmcb_avt.egg-info/top_level.txt
```

### Comparing `mmcb-avt-0.0.77/LICENSE` & `mmcb-avt-0.0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/PKG-INFO` & `mmcb-avt-0.0.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.77
+Version: 0.0.78
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.77/README.md` & `mmcb-avt-0.0.78/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/setup.py` & `mmcb-avt-0.0.78/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.77",
+    version="0.0.78",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb-avt-0.0.77/src/mmcb/common.py` & `mmcb-avt-0.0.78/src/mmcb/common.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.78/src/mmcb/configure_environment.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.78/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/dat2root.py` & `mmcb-avt-0.0.78/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/detect.py` & `mmcb-avt-0.0.78/src/mmcb/detect.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/iv.py` & `mmcb-avt-0.0.78/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/lexicon.py` & `mmcb-avt-0.0.78/src/mmcb/lexicon.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,24 +520,24 @@
     --------------------------------------------------------------------------
     """
     terminate = '\r\n'
 
     ##########################################################################
     # Language: Standard Commands for Programmable Instruments (SCPI)
     dmm6500 = {
-        'identify': '*IDN?',
-        'set up to read voltage': (
-            'dmm.measure.func = dmm.FUNC_DC_VOLTAGE;'
+        'configure to read current': (
+            'dmm.measure.func = dmm.FUNC_DC_CURRENT;'
             'dmm.measure.autorange = dmm.ON'
         ),
-        'read value': 'print(dmm.measure.read())',
-        'set up to read current': (
-            'dmm.measure.func = dmm.FUNC_DC_CURRENT;'
+        'configure to read voltage': (
+            'dmm.measure.func = dmm.FUNC_DC_VOLTAGE;'
             'dmm.measure.autorange = dmm.ON'
         ),
+        'identify': '*IDN?',
+        'read value': 'print(dmm.measure.read())',
     }
 
     instructions = {
         'dmm6500': dmm6500,
     }
 
     # sanity checks
```

### Comparing `mmcb-avt-0.0.77/src/mmcb/liveplot.py` & `mmcb-avt-0.0.78/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/log2dat.py` & `mmcb-avt-0.0.78/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/peltier.py` & `mmcb-avt-0.0.78/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/psuset.py` & `mmcb-avt-0.0.78/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/psustat.py` & `mmcb-avt-0.0.78/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/sense.py` & `mmcb-avt-0.0.78/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/sensors.py` & `mmcb-avt-0.0.78/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/sequence.py` & `mmcb-avt-0.0.78/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb/ult80.py` & `mmcb-avt-0.0.78/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.77/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.78/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.77
+Version: 0.0.78
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.77/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.78/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 src/mmcb/__init__.py
 src/mmcb/common.py
 src/mmcb/configure_environment.py
 src/mmcb/dat2plot.py
 src/mmcb/dat2root.py
 src/mmcb/detect.py
 src/mmcb/dmm.py
+src/mmcb/dmm_interface.py
 src/mmcb/iv.py
 src/mmcb/lexicon.py
 src/mmcb/liveplot.py
 src/mmcb/log2dat.py
 src/mmcb/peltier.py
 src/mmcb/psuset.py
 src/mmcb/psustat.py
 src/mmcb/sense.py
 src/mmcb/sensors.py
+src/mmcb/sensors_mod.py
 src/mmcb/sequence.py
 src/mmcb/ult80.py
 src/mmcb_avt.egg-info/PKG-INFO
 src/mmcb_avt.egg-info/SOURCES.txt
 src/mmcb_avt.egg-info/dependency_links.txt
 src/mmcb_avt.egg-info/entry_points.txt
 src/mmcb_avt.egg-info/requires.txt
```

