# Comparing `tmp/hubitatcontrol-2.3.2.tar.gz` & `tmp/hubitatcontrol-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubitatcontrol-2.3.2.tar", max compression
+gzip compressed data, was "hubitatcontrol-2.3.3.tar", max compression
```

## Comparing `hubitatcontrol-2.3.2.tar` & `hubitatcontrol-2.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-2.3.2/LICENSE
--rw-r--r--   0        0        0     6311 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.2/README.md
--rw-r--r--   0        0        0     3072 2023-05-09 03:28:26.350568 hubitatcontrol-2.3.2/hubitatcontrol/__init__.py
--rw-r--r--   0        0        0     3824 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.2/hubitatcontrol/__main__.py
--rw-r--r--   0        0        0      172 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.2/hubitatcontrol/environment.py
--rw-r--r--   0        0        0     1060 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.2/hubitatcontrol/generic.py
--rw-r--r--   0        0        0     3073 2023-05-09 06:17:49.007286 hubitatcontrol-2.3.2/hubitatcontrol/hub.py
--rw-r--r--   0        0        0     2774 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.2/hubitatcontrol/lights.py
--rw-r--r--   0        0        0      478 2023-05-09 03:28:26.350568 hubitatcontrol-2.3.2/hubitatcontrol/sensors.py
--rw-r--r--   0        0        0     2606 2023-05-09 06:21:55.280233 hubitatcontrol-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     7193 1970-01-01 00:00:00.000000 hubitatcontrol-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-2.3.3/LICENSE
+-rw-r--r--   0        0        0     6311 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.3/README.md
+-rw-r--r--   0        0        0     3082 2023-05-11 03:27:49.032359 hubitatcontrol-2.3.3/hubitatcontrol/__init__.py
+-rw-r--r--   0        0        0     3824 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.3/hubitatcontrol/__main__.py
+-rw-r--r--   0        0        0      172 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.3/hubitatcontrol/environment.py
+-rw-r--r--   0        0        0     1060 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.3/hubitatcontrol/generic.py
+-rw-r--r--   0        0        0     3073 2023-05-09 06:17:49.007286 hubitatcontrol-2.3.3/hubitatcontrol/hub.py
+-rw-r--r--   0        0        0     2774 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.3/hubitatcontrol/lights.py
+-rw-r--r--   0        0        0      478 2023-05-09 03:28:26.350568 hubitatcontrol-2.3.3/hubitatcontrol/sensors.py
+-rw-r--r--   0        0        0     2606 2023-05-11 03:45:25.239499 hubitatcontrol-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0     7193 1970-01-01 00:00:00.000000 hubitatcontrol-2.3.3/PKG-INFO
```

### Comparing `hubitatcontrol-2.3.2/LICENSE` & `hubitatcontrol-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.2/README.md` & `hubitatcontrol-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.2/hubitatcontrol/__init__.py` & `hubitatcontrol-2.3.3/hubitatcontrol/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,14 @@
     device_list = []
     for i in hub_in.devices:
         if "TemperatureMeasurement" in i["capabilities"]:
             device_list.append(get_device_type(i, hub_in))
     return device_list
 
 
-def get_all_env_sensors(hub_in: hubitatcontrol.hub) -> list[hubitatcontrol.sensors.EnvironmentalSensor]:
+def get_all_environmental_sensors(hub_in: hubitatcontrol.hub) -> list[hubitatcontrol.sensors.EnvironmentalSensor]:
     """Returns list of all hub devices with associated helper functions"""
     device_list = []
     for i in hub_in.devices:
         if ("RelativeHumidityMeasurement" in i["capabilities"]) and ("TemperatureMeasurement" in i["capabilities"]):
             device_list.append(get_device_type(i, hub_in))
     return device_list
```

### Comparing `hubitatcontrol-2.3.2/hubitatcontrol/__main__.py` & `hubitatcontrol-2.3.3/hubitatcontrol/__main__.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.2/hubitatcontrol/generic.py` & `hubitatcontrol-2.3.3/hubitatcontrol/generic.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.2/hubitatcontrol/hub.py` & `hubitatcontrol-2.3.3/hubitatcontrol/hub.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.2/hubitatcontrol/lights.py` & `hubitatcontrol-2.3.3/hubitatcontrol/lights.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.2/pyproject.toml` & `hubitatcontrol-2.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hubitatcontrol"
-version = "v2.3.2"
+version = "v2.3.3"
 description = "Hubitat Maker API Interface"
 authors = ["Jesse Schoepfer <jelloeater@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/Jelloeater/hubitatcontrol"
 keywords = ["hubitat", "makerapi","requests"]
 classifiers = ["Development Status :: 5 - Production/Stable",
```

### Comparing `hubitatcontrol-2.3.2/PKG-INFO` & `hubitatcontrol-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubitatcontrol
-Version: 2.3.2
+Version: 2.3.3
 Summary: Hubitat Maker API Interface
 Home-page: https://github.com/Jelloeater/hubitatcontrol
 License: MIT
 Keywords: hubitat,makerapi,requests
 Author: Jesse Schoepfer
 Author-email: jelloeater@gmail.com
 Requires-Python: >=3.10,<4.0
```

