# Comparing `tmp/mmcb-avt-0.0.80.tar.gz` & `tmp/mmcb-avt-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.80.tar", last modified: Thu May 11 08:06:04 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.81.tar", last modified: Thu May 11 10:26:02 2023, max compression
```

## Comparing `mmcb-avt-0.0.80.tar` & `mmcb-avt-0.0.81.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 08:06:04.270975 mmcb-avt-0.0.80/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.80/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     8735 2023-05-11 08:06:04.270077 mmcb-avt-0.0.80/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     7512 2023-05-11 08:01:36.000000 mmcb-avt-0.0.80/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.80/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-11 08:06:04.271163 mmcb-avt-0.0.80/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-11 08:05:48.000000 mmcb-avt-0.0.80/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 08:06:04.240520 mmcb-avt-0.0.80/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 08:06:04.264066 mmcb-avt-0.0.80/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.80/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    93094 2023-03-08 11:04:09.000000 mmcb-avt-0.0.80/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.80/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.80/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.80/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33679 2023-05-10 15:18:59.000000 mmcb-avt-0.0.80/src/mmcb/detect.py
--rwx------   0 avt        (501) staff       (20)     2102 2023-05-11 08:03:59.000000 mmcb-avt-0.0.80/src/mmcb/dmm.py
--rw-r--r--   0 avt        (501) staff       (20)     4178 2023-05-11 07:39:08.000000 mmcb-avt-0.0.80/src/mmcb/dmm_interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.80/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    23750 2023-05-11 07:13:26.000000 mmcb-avt-0.0.80/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.80/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.80/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.80/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.80/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.80/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.80/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.80/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.80/src/mmcb/sensors_mod.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.80/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.80/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 08:06:04.268988 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     8735 2023-05-11 08:06:04.000000 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      672 2023-05-11 08:06:04.000000 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-11 08:06:04.000000 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-11 08:06:04.000000 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-11 08:06:04.000000 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-11 08:06:04.000000 mmcb-avt-0.0.80/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 10:26:02.384197 mmcb-avt-0.0.81/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.81/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     8735 2023-05-11 10:26:02.383331 mmcb-avt-0.0.81/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     7512 2023-05-11 08:01:36.000000 mmcb-avt-0.0.81/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.81/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-11 10:26:02.384410 mmcb-avt-0.0.81/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-11 10:24:51.000000 mmcb-avt-0.0.81/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 10:26:02.334293 mmcb-avt-0.0.81/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 10:26:02.374838 mmcb-avt-0.0.81/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.81/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    93094 2023-03-08 11:04:09.000000 mmcb-avt-0.0.81/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.81/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.81/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.81/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33679 2023-05-10 15:18:59.000000 mmcb-avt-0.0.81/src/mmcb/detect.py
+-rwx------   0 avt        (501) staff       (20)     3708 2023-05-11 10:22:20.000000 mmcb-avt-0.0.81/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4220 2023-05-11 10:22:49.000000 mmcb-avt-0.0.81/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.81/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 10:19:34.000000 mmcb-avt-0.0.81/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.81/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.81/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.81/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.81/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.81/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.81/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.81/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.81/src/mmcb/sensors_mod.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.81/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.81/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-11 10:26:02.381929 mmcb-avt-0.0.81/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     8735 2023-05-11 10:26:02.000000 mmcb-avt-0.0.81/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      672 2023-05-11 10:26:02.000000 mmcb-avt-0.0.81/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-11 10:26:02.000000 mmcb-avt-0.0.81/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-11 10:26:02.000000 mmcb-avt-0.0.81/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-11 10:26:02.000000 mmcb-avt-0.0.81/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-11 10:26:02.000000 mmcb-avt-0.0.81/src/mmcb_avt.egg-info/top_level.txt
```

### Comparing `mmcb-avt-0.0.80/LICENSE` & `mmcb-avt-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/PKG-INFO` & `mmcb-avt-0.0.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.80
+Version: 0.0.81
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.80/README.md` & `mmcb-avt-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/setup.py` & `mmcb-avt-0.0.81/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.80",
+    version="0.0.81",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb-avt-0.0.80/src/mmcb/common.py` & `mmcb-avt-0.0.81/src/mmcb/common.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.81/src/mmcb/configure_environment.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.81/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/dat2root.py` & `mmcb-avt-0.0.81/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/detect.py` & `mmcb-avt-0.0.81/src/mmcb/detect.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/dmm_interface.py` & `mmcb-avt-0.0.81/src/mmcb/dmm_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,53 +82,56 @@
         self._finalizer()
 
     @property
     def removed(self):
         """check (indirectly) if the serial port has been closed"""
         return not self._finalizer.alive
 
-    def configure_read_current(self):
+    def _send_command(self, command):
         """
-        Read the current as measured at the output terminals.
+        Issue command to instrument.
 
         --------------------------------------------------------------------------
-        args : none
+        args
+            command : string
         --------------------------------------------------------------------------
-        returns
-            value : float or None
+        returns : none
         --------------------------------------------------------------------------
         """
         common.send_command(
             self.pipeline,
             self.ser,
             self.channel,
-            lexicon.instrument(self.channel.model, 'configure to read current'),
+            lexicon.instrument(self.channel.model, command),
         )
 
-    def configure_read_voltage(self):
-        """
-        Read the voltage as measured at the output terminals.
+    def configure_read_capacitance(self):
+        self._send_command('configure to read capacitance')
 
-        --------------------------------------------------------------------------
-        args : none
-        --------------------------------------------------------------------------
-        returns
-            value : float or None
-        --------------------------------------------------------------------------
-        """
-        common.send_command(
-            self.pipeline,
-            self.ser,
-            self.channel,
-            lexicon.instrument(self.channel.model, 'configure to read voltage'),
-        )
+    def configure_read_ac_current(self):
+        self._send_command('configure to read ac current')
+
+    def configure_read_dc_current(self):
+        self._send_command('configure to read dc current')
+
+    def configure_read_resistance(self):
+        self._send_command('configure to read resistance')
+
+    def configure_read_temperature(self):
+        self._send_command('configure to read temperature')
+
+    def configure_read_dc_voltage(self):
+        self._send_command('configure to read dc voltage')
+
+    def configure_read_ac_voltage(self):
+        self._send_command('configure to read ac voltage')
 
     def read_value(self):
         """
-        Read the voltage as measured at the output terminals.
+        Read the value of the previously configured parameter from the instrument.
 
         --------------------------------------------------------------------------
         args : none
         --------------------------------------------------------------------------
         returns
             value : float or None
         --------------------------------------------------------------------------
```

### Comparing `mmcb-avt-0.0.80/src/mmcb/iv.py` & `mmcb-avt-0.0.81/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/lexicon.py` & `mmcb-avt-0.0.81/src/mmcb/lexicon.py`

 * *Files 3% similar despite different names*

```diff
@@ -519,25 +519,54 @@
         a valid command that can be sent to the psu over RS232
     --------------------------------------------------------------------------
     """
     terminate = '\r\n'
 
     ##########################################################################
     # Language: Standard Commands for Programmable Instruments (SCPI)
+    #
+    # Note that front/rear terminal usage can only be set using the front
+    # panel button
     dmm6500 = {
-        'configure to read current': (
-            'dmm.measure.func = dmm.FUNC_DC_CURRENT;'
-            'dmm.measure.autorange = dmm.ON'
-        ),
-        'configure to read voltage': (
-            'dmm.measure.func = dmm.FUNC_DC_VOLTAGE;'
-            'dmm.measure.autorange = dmm.ON'
+        'configure to read capacitance': (
+            'dmm.measure.func=dmm.FUNC_CAPACITANCE;'
+            'dmm.measure.autorange=dmm.ON'
+        ),
+        'configure to read ac current': (
+            'dmm.measure.func=dmm.FUNC_AC_CURRENT;'
+            'dmm.measure.autorange=dmm.ON'
+        ),
+        'configure to read dc current': (
+            'dmm.measure.func=dmm.FUNC_DC_CURRENT;'
+            'dmm.measure.autorange=dmm.ON'
+        ),
+        'configure to read resistance': (
+            'dmm.measure.func=dmm.FUNC_RESISTANCE;'
+            'dmm.measure.autorange=dmm.ON'
+        ),
+        # Auto range not available for this function.
+        # This is just a placeholder, and will need proper configuration later.
+        # See reference manual p.14-68 (p.786 in PDF).
+        'configure to read temperature': (
+            'dmm.measure.func=dmm.FUNC_TEMPERATURE;'
+            'dmm.measure.unit=dmm.UNIT_CELSIUS'
+        ),
+        'configure to read ac voltage': (
+            'dmm.measure.func=dmm.FUNC_AC_VOLTAGE;'
+            'dmm.measure.unit=dmm.UNIT_VOLT;'
+            'dmm.measure.autorange=dmm.ON'
+        ),
+        'configure to read dc voltage': (
+            'dmm.measure.func=dmm.FUNC_DC_VOLTAGE;'
+            'dmm.measure.unit=dmm.UNIT_VOLT;'
+            'dmm.measure.autorange=dmm.ON'
         ),
         'identify': '*IDN?',
         'read value': 'print(dmm.measure.read())',
+        'reset': 'dmm.reset()',
     }
 
     instructions = {
         'dmm6500': dmm6500,
     }
 
     # sanity checks
```

### Comparing `mmcb-avt-0.0.80/src/mmcb/liveplot.py` & `mmcb-avt-0.0.81/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/log2dat.py` & `mmcb-avt-0.0.81/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/peltier.py` & `mmcb-avt-0.0.81/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/psuset.py` & `mmcb-avt-0.0.81/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/psustat.py` & `mmcb-avt-0.0.81/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/sense.py` & `mmcb-avt-0.0.81/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/sensors.py` & `mmcb-avt-0.0.81/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/sensors_mod.py` & `mmcb-avt-0.0.81/src/mmcb/sensors_mod.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/sequence.py` & `mmcb-avt-0.0.81/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb/ult80.py` & `mmcb-avt-0.0.81/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.80/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.81/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.80
+Version: 0.0.81
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.80/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.81/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

