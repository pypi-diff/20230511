# Comparing `tmp/mmcb-avt-0.0.75.tar.gz` & `tmp/mmcb-avt-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.75.tar", last modified: Tue May  9 14:12:18 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.77.tar", last modified: Wed May 10 15:13:50 2023, max compression
```

## Comparing `mmcb-avt-0.0.75.tar` & `mmcb-avt-0.0.77.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-09 14:12:18.099981 mmcb-avt-0.0.75/
--rw-r--r--   0 avt       (1000) avt       (1000)    13827 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/LICENSE
--rw-r--r--   0 avt       (1000) avt       (1000)     8108 2023-05-09 14:12:18.099981 mmcb-avt-0.0.75/PKG-INFO
--rw-r--r--   0 avt       (1000) avt       (1000)     6885 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/README.md
--rw-r--r--   0 avt       (1000) avt       (1000)      104 2023-01-25 09:49:54.000000 mmcb-avt-0.0.75/pyproject.toml
--rw-r--r--   0 avt       (1000) avt       (1000)       38 2023-05-09 14:12:18.099981 mmcb-avt-0.0.75/setup.cfg
--rw-r--r--   0 avt       (1000) avt       (1000)     2556 2023-05-09 14:11:36.000000 mmcb-avt-0.0.75/setup.py
-drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-09 14:12:18.079981 mmcb-avt-0.0.75/src/
-drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-09 14:12:18.095981 mmcb-avt-0.0.75/src/mmcb/
--rw-r--r--   0 avt       (1000) avt       (1000)        0 2023-01-25 09:49:54.000000 mmcb-avt-0.0.75/src/mmcb/__init__.py
--rw-r--r--   0 avt       (1000) avt       (1000)    93094 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/common.py
--rw-r--r--   0 avt       (1000) avt       (1000)    32486 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    14416 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)     9078 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    33674 2023-05-09 14:00:27.000000 mmcb-avt-0.0.75/src/mmcb/detect.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)   112129 2023-01-25 09:49:54.000000 mmcb-avt-0.0.75/src/mmcb/iv.py
--rw-r--r--   0 avt       (1000) avt       (1000)    23401 2023-05-09 14:09:42.000000 mmcb-avt-0.0.75/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    12231 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)     7040 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)     7889 2023-01-25 09:49:54.000000 mmcb-avt-0.0.75/src/mmcb/peltier.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    33621 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/psuset.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    21883 2023-01-25 09:49:54.000000 mmcb-avt-0.0.75/src/mmcb/psustat.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    13517 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/sense.py
--rw-r--r--   0 avt       (1000) avt       (1000)    40226 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/sensors.py
--rw-r--r--   0 avt       (1000) avt       (1000)    17705 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/sequence.py
--rwxr-xr-x   0 avt       (1000) avt       (1000)    17659 2023-05-09 12:22:28.000000 mmcb-avt-0.0.75/src/mmcb/ult80.py
-drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-09 14:12:18.099981 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt       (1000) avt       (1000)     8108 2023-05-09 14:12:17.000000 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt       (1000) avt       (1000)      606 2023-05-09 14:12:18.000000 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt       (1000) avt       (1000)        1 2023-05-09 14:12:17.000000 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt       (1000) avt       (1000)      310 2023-05-09 14:12:18.000000 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt       (1000) avt       (1000)      226 2023-05-09 14:12:18.000000 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt       (1000) avt       (1000)        5 2023-05-09 14:12:18.000000 mmcb-avt-0.0.75/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-10 15:13:50.133997 mmcb-avt-0.0.77/
+-rw-r--r--   0 avt       (1000) avt       (1000)    13827 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/LICENSE
+-rw-r--r--   0 avt       (1000) avt       (1000)     8108 2023-05-10 15:13:50.129997 mmcb-avt-0.0.77/PKG-INFO
+-rw-r--r--   0 avt       (1000) avt       (1000)     6885 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/README.md
+-rw-r--r--   0 avt       (1000) avt       (1000)      104 2023-01-25 09:49:54.000000 mmcb-avt-0.0.77/pyproject.toml
+-rw-r--r--   0 avt       (1000) avt       (1000)       38 2023-05-10 15:13:50.133997 mmcb-avt-0.0.77/setup.cfg
+-rw-r--r--   0 avt       (1000) avt       (1000)     2591 2023-05-10 15:03:35.000000 mmcb-avt-0.0.77/setup.py
+drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-10 15:13:50.113998 mmcb-avt-0.0.77/src/
+drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-10 15:13:50.125997 mmcb-avt-0.0.77/src/mmcb/
+-rw-r--r--   0 avt       (1000) avt       (1000)        0 2023-01-25 09:49:54.000000 mmcb-avt-0.0.77/src/mmcb/__init__.py
+-rw-r--r--   0 avt       (1000) avt       (1000)    93094 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/common.py
+-rw-r--r--   0 avt       (1000) avt       (1000)    32486 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    14416 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)     9078 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    33679 2023-05-09 15:58:31.000000 mmcb-avt-0.0.77/src/mmcb/detect.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)     6415 2023-05-10 15:10:15.000000 mmcb-avt-0.0.77/src/mmcb/dmm.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)   112129 2023-01-25 09:49:54.000000 mmcb-avt-0.0.77/src/mmcb/iv.py
+-rw-r--r--   0 avt       (1000) avt       (1000)    23744 2023-05-10 15:00:25.000000 mmcb-avt-0.0.77/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    12231 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)     7040 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)     7889 2023-01-25 09:49:54.000000 mmcb-avt-0.0.77/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    33621 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    21883 2023-01-25 09:49:54.000000 mmcb-avt-0.0.77/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    13517 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/sense.py
+-rw-r--r--   0 avt       (1000) avt       (1000)    40226 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/sensors.py
+-rw-r--r--   0 avt       (1000) avt       (1000)    17705 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt       (1000) avt       (1000)    17659 2023-05-09 12:22:28.000000 mmcb-avt-0.0.77/src/mmcb/ult80.py
+drwxr-xr-x   0 avt       (1000) avt       (1000)        0 2023-05-10 15:13:50.129997 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt       (1000) avt       (1000)     8108 2023-05-10 15:13:50.000000 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt       (1000) avt       (1000)      622 2023-05-10 15:13:50.000000 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt       (1000) avt       (1000)        1 2023-05-10 15:13:50.000000 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt       (1000) avt       (1000)      330 2023-05-10 15:13:50.000000 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt       (1000) avt       (1000)      226 2023-05-10 15:13:50.000000 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt       (1000) avt       (1000)        5 2023-05-10 15:13:50.000000 mmcb-avt-0.0.77/src/mmcb_avt.egg-info/top_level.txt
```

### Comparing `mmcb-avt-0.0.75/LICENSE` & `mmcb-avt-0.0.77/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/PKG-INFO` & `mmcb-avt-0.0.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.75
+Version: 0.0.77
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.75/README.md` & `mmcb-avt-0.0.77/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/setup.py` & `mmcb-avt-0.0.77/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.75",
+    version="0.0.77",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -38,14 +38,15 @@
         "yoctopuce",
     ],
     entry_points={
         "console_scripts": [
             "dat2plot = mmcb.dat2plot:main",
             "dat2root = mmcb.dat2root:main",
             "detect = mmcb.detect:main",
+            "dmm = mmcb.dmm:main",
             "iv = mmcb.iv:main",
             "liveplot = mmcb.liveplot:main",
             "log2dat = mmcb.log2dat:main",
             "peltier = mmcb.peltier:main",
             "psuset = mmcb.psuset:main",
             "psustat = mmcb.psustat:main",
             "sense = mmcb.sense:main",
```

### Comparing `mmcb-avt-0.0.75/src/mmcb/common.py` & `mmcb-avt-0.0.77/src/mmcb/common.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.77/src/mmcb/configure_environment.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.77/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/dat2root.py` & `mmcb-avt-0.0.77/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/detect.py` & `mmcb-avt-0.0.77/src/mmcb/detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -806,15 +806,15 @@
                     # ['KEITHLEY INSTRUMENTS', 'MODEL DMM6500', '04592428', '1.7.12b']
                     model = parts[1].split()[-1]
                     serial_number = parts[2]
                     detected = True
                     channels = ['']
                     settings = ser.get_settings()
                     retval = (
-                        'hvpsu',
+                        'instrument',
                         settings,
                         (
                             port,
                             manufacturer,
                             model,
                             serial_number,
                             detected,
```

### Comparing `mmcb-avt-0.0.75/src/mmcb/iv.py` & `mmcb-avt-0.0.77/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/lexicon.py` & `mmcb-avt-0.0.77/src/mmcb/lexicon.py`

 * *Files 2% similar despite different names*

```diff
@@ -521,14 +521,23 @@
     """
     terminate = '\r\n'
 
     ##########################################################################
     # Language: Standard Commands for Programmable Instruments (SCPI)
     dmm6500 = {
         'identify': '*IDN?',
+        'set up to read voltage': (
+            'dmm.measure.func = dmm.FUNC_DC_VOLTAGE;'
+            'dmm.measure.autorange = dmm.ON'
+        ),
+        'read value': 'print(dmm.measure.read())',
+        'set up to read current': (
+            'dmm.measure.func = dmm.FUNC_DC_CURRENT;'
+            'dmm.measure.autorange = dmm.ON'
+        ),
     }
 
     instructions = {
         'dmm6500': dmm6500,
     }
 
     # sanity checks
```

### Comparing `mmcb-avt-0.0.75/src/mmcb/liveplot.py` & `mmcb-avt-0.0.77/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/log2dat.py` & `mmcb-avt-0.0.77/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/peltier.py` & `mmcb-avt-0.0.77/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/psuset.py` & `mmcb-avt-0.0.77/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/psustat.py` & `mmcb-avt-0.0.77/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/sense.py` & `mmcb-avt-0.0.77/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/sensors.py` & `mmcb-avt-0.0.77/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/sequence.py` & `mmcb-avt-0.0.77/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb/ult80.py` & `mmcb-avt-0.0.77/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.75/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.77/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.75
+Version: 0.0.77
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.75/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.77/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 src/mmcb/__init__.py
 src/mmcb/common.py
 src/mmcb/configure_environment.py
 src/mmcb/dat2plot.py
 src/mmcb/dat2root.py
 src/mmcb/detect.py
+src/mmcb/dmm.py
 src/mmcb/iv.py
 src/mmcb/lexicon.py
 src/mmcb/liveplot.py
 src/mmcb/log2dat.py
 src/mmcb/peltier.py
 src/mmcb/psuset.py
 src/mmcb/psustat.py
```

