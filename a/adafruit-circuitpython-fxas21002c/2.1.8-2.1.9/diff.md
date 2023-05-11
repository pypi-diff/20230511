# Comparing `tmp/adafruit-circuitpython-fxas21002c-2.1.8.tar.gz` & `tmp/adafruit-circuitpython-fxas21002c-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-fxas21002c-2.1.8.tar", last modified: Thu Apr 29 17:13:22 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-fxas21002c-2.1.9.tar", last modified: Tue May  4 18:03:35 2021, max compression
```

## Comparing `adafruit-circuitpython-fxas21002c-2.1.8.tar` & `adafruit-circuitpython-fxas21002c-2.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:13:22.014131 adafruit-circuitpython-fxas21002c-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:13:22.010131 adafruit-circuitpython-fxas21002c-2.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:13:22.010131 adafruit-circuitpython-fxas21002c-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:13:22.010131 adafruit-circuitpython-fxas21002c-2.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4119 2021-04-29 17:13:22.014131 adafruit-circuitpython-fxas21002c-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:13:22.014131 adafruit-circuitpython-fxas21002c-2.1.8/adafruit_circuitpython_fxas21002c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4119 2021-04-29 17:13:21.000000 adafruit-circuitpython-fxas21002c-2.1.8/adafruit_circuitpython_fxas21002c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      793 2021-04-29 17:13:21.000000 adafruit-circuitpython-fxas21002c-2.1.8/adafruit_circuitpython_fxas21002c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-29 17:13:21.000000 adafruit-circuitpython-fxas21002c-2.1.8/adafruit_circuitpython_fxas21002c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-04-29 17:13:21.000000 adafruit-circuitpython-fxas21002c-2.1.8/adafruit_circuitpython_fxas21002c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-04-29 17:13:21.000000 adafruit-circuitpython-fxas21002c-2.1.8/adafruit_circuitpython_fxas21002c.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6953 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/adafruit_fxas21002c.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:13:22.014131 adafruit-circuitpython-fxas21002c-2.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:13:22.014131 adafruit-circuitpython-fxas21002c-2.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5520 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:13:22.014131 adafruit-circuitpython-fxas21002c-2.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/examples/fxas21002c_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-29 17:13:22.014131 adafruit-circuitpython-fxas21002c-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2021-04-29 17:13:12.000000 adafruit-circuitpython-fxas21002c-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:03:35.037727 adafruit-circuitpython-fxas21002c-2.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:03:35.029727 adafruit-circuitpython-fxas21002c-2.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:03:35.033727 adafruit-circuitpython-fxas21002c-2.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:03:35.033727 adafruit-circuitpython-fxas21002c-2.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4119 2021-05-04 18:03:35.037727 adafruit-circuitpython-fxas21002c-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2634 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:03:35.033727 adafruit-circuitpython-fxas21002c-2.1.9/adafruit_circuitpython_fxas21002c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4119 2021-05-04 18:03:34.000000 adafruit-circuitpython-fxas21002c-2.1.9/adafruit_circuitpython_fxas21002c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      793 2021-05-04 18:03:34.000000 adafruit-circuitpython-fxas21002c-2.1.9/adafruit_circuitpython_fxas21002c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 18:03:34.000000 adafruit-circuitpython-fxas21002c-2.1.9/adafruit_circuitpython_fxas21002c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-05-04 18:03:34.000000 adafruit-circuitpython-fxas21002c-2.1.9/adafruit_circuitpython_fxas21002c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-05-04 18:03:34.000000 adafruit-circuitpython-fxas21002c-2.1.9/adafruit_circuitpython_fxas21002c.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7034 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/adafruit_fxas21002c.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:03:35.037727 adafruit-circuitpython-fxas21002c-2.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:03:35.037727 adafruit-circuitpython-fxas21002c-2.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5520 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:03:35.037727 adafruit-circuitpython-fxas21002c-2.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/examples/fxas21002c_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-04 18:03:35.037727 adafruit-circuitpython-fxas21002c-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1967 2021-05-04 18:03:24.000000 adafruit-circuitpython-fxas21002c-2.1.9/setup.py
```

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-fxas21002c-2.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-fxas21002c-2.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-fxas21002c-2.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/.pylintrc` & `adafruit-circuitpython-fxas21002c-2.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-fxas21002c-2.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/LICENSE` & `adafruit-circuitpython-fxas21002c-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-fxas21002c-2.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-fxas21002c-2.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-fxas21002c-2.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/PKG-INFO` & `adafruit-circuitpython-fxas21002c-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fxas21002c
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for NXP FXAS21002C gyroscope.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_FXAS21002C
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/README.rst` & `adafruit-circuitpython-fxas21002c-2.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/adafruit_circuitpython_fxas21002c.egg-info/PKG-INFO` & `adafruit-circuitpython-fxas21002c-2.1.9/adafruit_circuitpython_fxas21002c.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fxas21002c
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for NXP FXAS21002C gyroscope.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_FXAS21002C
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/adafruit_circuitpython_fxas21002c.egg-info/SOURCES.txt` & `adafruit-circuitpython-fxas21002c-2.1.9/adafruit_circuitpython_fxas21002c.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/adafruit_fxas21002c.py` & `adafruit-circuitpython-fxas21002c-2.1.9/adafruit_fxas21002c.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,20 +106,21 @@
 
     # Class-level buffer for reading and writing data with the sensor.
     # This reduces memory allocations but means the code is not re-entrant or
     # thread safe!
     _BUFFER = bytearray(7)
 
     def __init__(self, i2c, address=_FXAS21002C_ADDRESS, gyro_range=GYRO_RANGE_250DPS):
-        assert gyro_range in (
+        if gyro_range not in (
             GYRO_RANGE_250DPS,
             GYRO_RANGE_500DPS,
             GYRO_RANGE_1000DPS,
             GYRO_RANGE_2000DPS,
-        )
+        ):
+            raise Exception("gyro_range option selected is not a valid option")
         self._gyro_range = gyro_range
         self._device = i2c_dev.I2CDevice(i2c, address)
         # Check for chip ID value.
         if self._read_u8(_GYRO_REGISTER_WHO_AM_I) != _FXAS21002C_ID:
             raise RuntimeError("Failed to find FXAS21002C, check wiring!")
         ctrl_reg0 = 0x00
         if gyro_range == GYRO_RANGE_250DPS:
```

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-fxas21002c-2.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/docs/conf.py` & `adafruit-circuitpython-fxas21002c-2.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/docs/index.rst` & `adafruit-circuitpython-fxas21002c-2.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/examples/fxas21002c_simpletest.py` & `adafruit-circuitpython-fxas21002c-2.1.9/examples/fxas21002c_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-2.1.8/setup.py` & `adafruit-circuitpython-fxas21002c-2.1.9/setup.py`

 * *Files identical despite different names*

