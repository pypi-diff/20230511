# Comparing `tmp/mmcb-avt-0.0.79.tar.gz` & `tmp/mmcb-avt-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.79.tar", last modified: Thu May 11 08:02:05 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.80.tar", last modified: Thu May 11 08:06:04 2023, max compression
```

## Comparing `mmcb-avt-0.0.79.tar` & `mmcb-avt-0.0.80.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 08:02:05.223992 mmcb-avt-0.0.79/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.79/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     8735 2023-05-11 08:02:05.223365 mmcb-avt-0.0.79/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     7512 2023-05-11 08:01:36.000000 mmcb-avt-0.0.79/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.79/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-11 08:02:05.224151 mmcb-avt-0.0.79/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-11 08:01:50.000000 mmcb-avt-0.0.79/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 08:02:05.196648 mmcb-avt-0.0.79/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 08:02:05.218546 mmcb-avt-0.0.79/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.79/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    93094 2023-03-08 11:04:09.000000 mmcb-avt-0.0.79/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.79/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.79/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.79/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33679 2023-05-10 15:18:59.000000 mmcb-avt-0.0.79/src/mmcb/detect.py
--rwx------   0 avt        (501) staff       (20)     2096 2023-05-11 07:36:55.000000 mmcb-avt-0.0.79/src/mmcb/dmm.py
--rw-r--r--   0 avt        (501) staff       (20)     4178 2023-05-11 07:39:08.000000 mmcb-avt-0.0.79/src/mmcb/dmm_interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.79/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    23750 2023-05-11 07:13:26.000000 mmcb-avt-0.0.79/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.79/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.79/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.79/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.79/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.79/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.79/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.79/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.79/src/mmcb/sensors_mod.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.79/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.79/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 08:02:05.222351 mmcb-avt-0.0.79/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     8735 2023-05-11 08:02:05.000000 mmcb-avt-0.0.79/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      672 2023-05-11 08:02:05.000000 mmcb-avt-0.0.79/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-11 08:02:05.000000 mmcb-avt-0.0.79/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-11 08:02:05.000000 mmcb-avt-0.0.79/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-11 08:02:05.000000 mmcb-avt-0.0.79/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-11 08:02:05.000000 mmcb-avt-0.0.79/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 08:06:04.270975 mmcb-avt-0.0.80/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.80/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     8735 2023-05-11 08:06:04.270077 mmcb-avt-0.0.80/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     7512 2023-05-11 08:01:36.000000 mmcb-avt-0.0.80/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.80/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-11 08:06:04.271163 mmcb-avt-0.0.80/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-11 08:05:48.000000 mmcb-avt-0.0.80/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 08:06:04.240520 mmcb-avt-0.0.80/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 08:06:04.264066 mmcb-avt-0.0.80/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.80/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    93094 2023-03-08 11:04:09.000000 mmcb-avt-0.0.80/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.80/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.80/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.80/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33679 2023-05-10 15:18:59.000000 mmcb-avt-0.0.80/src/mmcb/detect.py
+-rwx------   0 avt        (501) staff       (20)     2102 2023-05-11 08:03:59.000000 mmcb-avt-0.0.80/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4178 2023-05-11 07:39:08.000000 mmcb-avt-0.0.80/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.80/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    23750 2023-05-11 07:13:26.000000 mmcb-avt-0.0.80/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.80/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.80/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.80/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.80/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.80/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.80/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.80/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.80/src/mmcb/sensors_mod.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.80/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.80/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 08:06:04.268988 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     8735 2023-05-11 08:06:04.000000 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      672 2023-05-11 08:06:04.000000 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-11 08:06:04.000000 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-11 08:06:04.000000 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-11 08:06:04.000000 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-11 08:06:04.000000 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/top_level.txt
```

### Comparing `mmcb-avt-0.0.79/LICENSE` & `mmcb-avt-0.0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/PKG-INFO` & `mmcb-avt-0.0.80/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.79
+Version: 0.0.80
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.79/README.md` & `mmcb-avt-0.0.80/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/setup.py` & `mmcb-avt-0.0.80/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.79",
+    version="0.0.80",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb-avt-0.0.79/src/mmcb/common.py` & `mmcb-avt-0.0.80/src/mmcb/common.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.80/src/mmcb/configure_environment.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.80/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/dat2root.py` & `mmcb-avt-0.0.80/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/detect.py` & `mmcb-avt-0.0.80/src/mmcb/detect.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/dmm.py` & `mmcb-avt-0.0.80/src/mmcb/dmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     --------------------------------------------------------------------------
     """
     parser = argparse.ArgumentParser(
         description='Reads voltage or current from the Keithley DMM6500.'
     )
 
     parser.add_argument(
-        '-c', '--current',
+        '-c', '-i', '--current',
         action='store_true',
         help='Read current (A)')
     parser.add_argument(
         '-v', '--voltage',
         action='store_true',
         help='Read voltage (V)')
```

### Comparing `mmcb-avt-0.0.79/src/mmcb/dmm_interface.py` & `mmcb-avt-0.0.80/src/mmcb/dmm_interface.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/iv.py` & `mmcb-avt-0.0.80/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/lexicon.py` & `mmcb-avt-0.0.80/src/mmcb/lexicon.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/liveplot.py` & `mmcb-avt-0.0.80/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/log2dat.py` & `mmcb-avt-0.0.80/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/peltier.py` & `mmcb-avt-0.0.80/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/psuset.py` & `mmcb-avt-0.0.80/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/psustat.py` & `mmcb-avt-0.0.80/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/sense.py` & `mmcb-avt-0.0.80/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/sensors.py` & `mmcb-avt-0.0.80/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/sensors_mod.py` & `mmcb-avt-0.0.80/src/mmcb/sensors_mod.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/sequence.py` & `mmcb-avt-0.0.80/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb/ult80.py` & `mmcb-avt-0.0.80/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.79/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.80/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.79
+Version: 0.0.80
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.79/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.80/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

