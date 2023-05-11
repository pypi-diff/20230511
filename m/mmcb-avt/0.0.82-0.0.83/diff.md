# Comparing `tmp/mmcb-avt-0.0.82.tar.gz` & `tmp/mmcb-avt-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.82.tar", last modified: Thu May 11 13:11:38 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.83.tar", last modified: Thu May 11 15:28:06 2023, max compression
```

## Comparing `mmcb-avt-0.0.82.tar` & `mmcb-avt-0.0.83.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 13:11:38.946162 mmcb-avt-0.0.82/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.82/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     8735 2023-05-11 13:11:38.945387 mmcb-avt-0.0.82/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     7512 2023-05-11 08:01:36.000000 mmcb-avt-0.0.82/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.82/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-11 13:11:38.946356 mmcb-avt-0.0.82/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-11 13:11:26.000000 mmcb-avt-0.0.82/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 13:11:38.898757 mmcb-avt-0.0.82/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 13:11:38.936591 mmcb-avt-0.0.82/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.82/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    93094 2023-03-08 11:04:09.000000 mmcb-avt-0.0.82/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.82/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.82/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.82/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33679 2023-05-10 15:18:59.000000 mmcb-avt-0.0.82/src/mmcb/detect.py
--rwx------   0 avt        (501) staff       (20)     3128 2023-05-11 13:10:25.000000 mmcb-avt-0.0.82/src/mmcb/dmm.py
--rw-r--r--   0 avt        (501) staff       (20)     4220 2023-05-11 10:22:49.000000 mmcb-avt-0.0.82/src/mmcb/dmm_interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.82/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 10:19:34.000000 mmcb-avt-0.0.82/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.82/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.82/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.82/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.82/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.82/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.82/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.82/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.82/src/mmcb/sensors_mod.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.82/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.82/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 13:11:38.943956 mmcb-avt-0.0.82/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     8735 2023-05-11 13:11:38.000000 mmcb-avt-0.0.82/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      672 2023-05-11 13:11:38.000000 mmcb-avt-0.0.82/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-11 13:11:38.000000 mmcb-avt-0.0.82/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-11 13:11:38.000000 mmcb-avt-0.0.82/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-11 13:11:38.000000 mmcb-avt-0.0.82/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-11 13:11:38.000000 mmcb-avt-0.0.82/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 15:28:06.692217 mmcb-avt-0.0.83/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.83/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     8735 2023-05-11 15:28:06.691432 mmcb-avt-0.0.83/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     7512 2023-05-11 08:01:36.000000 mmcb-avt-0.0.83/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.83/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-11 15:28:06.692449 mmcb-avt-0.0.83/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-11 15:27:47.000000 mmcb-avt-0.0.83/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 15:28:06.664731 mmcb-avt-0.0.83/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 15:28:06.684954 mmcb-avt-0.0.83/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.83/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    93158 2023-05-11 14:41:48.000000 mmcb-avt-0.0.83/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.83/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.83/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.83/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33679 2023-05-10 15:18:59.000000 mmcb-avt-0.0.83/src/mmcb/detect.py
+-rwx------   0 avt        (501) staff       (20)     3052 2023-05-11 14:44:06.000000 mmcb-avt-0.0.83/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4220 2023-05-11 10:22:49.000000 mmcb-avt-0.0.83/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.83/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.83/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.83/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.83/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.83/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.83/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.83/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.83/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.83/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.83/src/mmcb/sensors_mod.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.83/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.83/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 15:28:06.690024 mmcb-avt-0.0.83/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     8735 2023-05-11 15:28:06.000000 mmcb-avt-0.0.83/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      672 2023-05-11 15:28:06.000000 mmcb-avt-0.0.83/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-11 15:28:06.000000 mmcb-avt-0.0.83/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-11 15:28:06.000000 mmcb-avt-0.0.83/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-11 15:28:06.000000 mmcb-avt-0.0.83/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-11 15:28:06.000000 mmcb-avt-0.0.83/src/mmcb_avt.egg-info/top_level.txt
```

### Comparing `mmcb-avt-0.0.82/LICENSE` & `mmcb-avt-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/PKG-INFO` & `mmcb-avt-0.0.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.82
+Version: 0.0.83
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.82/README.md` & `mmcb-avt-0.0.83/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/setup.py` & `mmcb-avt-0.0.83/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.82",
+    version="0.0.83",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb-avt-0.0.82/src/mmcb/common.py` & `mmcb-avt-0.0.83/src/mmcb/common.py`

 * *Files identical despite different names*

```diff
@@ -1033,21 +1033,25 @@
         compact : bool
             if True remove trailing zeros from number, if the remainder is a
             whole number, remove the trailing decimal point
             e.g.
             103.100 -> 103.1
              10.000 ->  10
     --------------------------------------------------------------------------
-    returns : string
+    returns : string or None
         value with SI unit prefix
     --------------------------------------------------------------------------
     """
     # make sure the number is in scientific notation
     # then separate value and exponent
-    significand, exponent = f'{float(value):e}'.lower().split('e')
+    try:
+        significand, exponent = f'{float(value):e}'.lower().split('e')
+    except TypeError:
+        return None
+
     significand = float(significand)
     exponent = int(exponent)
 
     # align with 10**3 boundaries
     while exponent % 3 != 0:
         exponent -= 1
         significand *= 10
```

### Comparing `mmcb-avt-0.0.82/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.83/src/mmcb/configure_environment.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.83/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/dat2root.py` & `mmcb-avt-0.0.83/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/detect.py` & `mmcb-avt-0.0.83/src/mmcb/detect.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/dmm.py` & `mmcb-avt-0.0.83/src/mmcb/dmm.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,22 +90,20 @@
 
     for function, required in vars(args).items():
         if not required:
             continue
 
         configure[function]()
 
+        value = None
         for _ in range(retries):
             value = dmm.read_value()
             if value is not None:
                 break
             time.sleep(0.1)
 
-        if value > 9e+37:
-            print(f'{function}, overflow, overflow')
-        else:
-            print(f'{function}, {common.si_prefix(value)}, {value}')
+        print(f'{function}, {common.si_prefix(value)}, {value}')
 
 
 ##############################################################################
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `mmcb-avt-0.0.82/src/mmcb/dmm_interface.py` & `mmcb-avt-0.0.83/src/mmcb/dmm_interface.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/iv.py` & `mmcb-avt-0.0.83/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/lexicon.py` & `mmcb-avt-0.0.83/src/mmcb/lexicon.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import statistics
 import timeit
 statistics.mean(timeit.Timer("lexicon.power('2410', 'read measured vi')",
                              setup='import lexicon').repeat(100,1))
 
 timings are:
 
-    2.043e-05s (uncached)
+    2.043e-05s (un-cached)
     4.207e-07s (cached)
 
 Cache performance for: ./iv.py -200 --hold 1
 
 CacheInfo(hits=82, misses=56, maxsize=128, currsize=56)
 
 callable functions from this file:
@@ -193,15 +193,15 @@
             name of the command to be fetched
         argument1 : numeric/string
             a parameter to substitute into the command string
         argument2 : numeric/string
             a parameter to substitute into the command string
         channel : string
             channel name, the caller is required to use this for
-            multi-channel power supplies, but may omit it for single-channel
+            multichannel power supplies, but may omit it for single-channel
     --------------------------------------------------------------------------
     returns : string
         a valid command that can be sent to the psu over RS232
     --------------------------------------------------------------------------
     """
     terminate = '\n' if model == '2614b' else '\r\n'
```

### Comparing `mmcb-avt-0.0.82/src/mmcb/liveplot.py` & `mmcb-avt-0.0.83/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/log2dat.py` & `mmcb-avt-0.0.83/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/peltier.py` & `mmcb-avt-0.0.83/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/psuset.py` & `mmcb-avt-0.0.83/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/psustat.py` & `mmcb-avt-0.0.83/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/sense.py` & `mmcb-avt-0.0.83/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/sensors.py` & `mmcb-avt-0.0.83/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/sensors_mod.py` & `mmcb-avt-0.0.83/src/mmcb/sensors_mod.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/sequence.py` & `mmcb-avt-0.0.83/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb/ult80.py` & `mmcb-avt-0.0.83/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.82/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.83/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.82
+Version: 0.0.83
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.82/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.83/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

