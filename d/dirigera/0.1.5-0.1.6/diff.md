# Comparing `tmp/dirigera-0.1.5.tar.gz` & `tmp/dirigera-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-0.1.5.tar", last modified: Sun Apr 30 09:20:18 2023, max compression
+gzip compressed data, was "dirigera-0.1.6.tar", last modified: Thu May 11 14:49:16 2023, max compression
```

## Comparing `dirigera-0.1.5.tar` & `dirigera-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.025783 dirigera-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-30 09:20:09.000000 dirigera-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-30 09:20:18.025783 dirigera-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-30 09:20:09.000000 dirigera-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-30 09:20:09.000000 dirigera-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 09:20:18.025783 dirigera-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 09:20:09.000000 dirigera-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.021783 dirigera-0.1.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.021783 dirigera-0.1.5/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.025783 dirigera-0.1.5/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/devices/blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/devices/light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.025783 dirigera-0.1.5/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.021783 dirigera-0.1.5/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-30 09:20:18.000000 dirigera-0.1.5/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-30 09:20:18.000000 dirigera-0.1.5/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 09:20:18.000000 dirigera-0.1.5/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-30 09:20:18.000000 dirigera-0.1.5/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-30 09:20:18.000000 dirigera-0.1.5/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-30 09:20:18.000000 dirigera-0.1.5/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.025783 dirigera-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-30 09:20:09.000000 dirigera-0.1.5/tests/test_blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-30 09:20:09.000000 dirigera-0.1.5/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-30 09:20:09.000000 dirigera-0.1.5/tests/test_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.779026 dirigera-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 14:49:03.000000 dirigera-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-11 14:49:16.779026 dirigera-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-11 14:49:03.000000 dirigera-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-11 14:49:03.000000 dirigera-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:49:16.779026 dirigera-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:49:03.000000 dirigera-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.775026 dirigera-0.1.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.775026 dirigera-0.1.6/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.775026 dirigera-0.1.6/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/devices/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/devices/open_close_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.779026 dirigera-0.1.6/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-11 14:49:03.000000 dirigera-0.1.6/src/dirigera/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.775026 dirigera-0.1.6/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-11 14:49:16.000000 dirigera-0.1.6/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-11 14:49:16.000000 dirigera-0.1.6/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:49:16.000000 dirigera-0.1.6/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 14:49:16.000000 dirigera-0.1.6/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 14:49:16.000000 dirigera-0.1.6/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 14:49:16.000000 dirigera-0.1.6/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:16.779026 dirigera-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-11 14:49:03.000000 dirigera-0.1.6/tests/test_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-11 14:49:03.000000 dirigera-0.1.6/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-11 14:49:03.000000 dirigera-0.1.6/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-11 14:49:03.000000 dirigera-0.1.6/tests/test_open_close_sensor.py
```

### Comparing `dirigera-0.1.5/LICENSE` & `dirigera-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.5/PKG-INFO` & `dirigera-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.5
+Version: 0.1.6
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dirigera-0.1.5/README.md` & `dirigera-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.5/pyproject.toml` & `dirigera-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
    "setuptools",
    "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "0.1.5"
+version = "0.1.6"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = ["python", "iot", "smarthome", "hub", "lighting", "ikea", "tradfri", "dirigera"]
 dependencies = [
     "requests >= 2.22.0",
```

### Comparing `dirigera-0.1.5/src/dirigera/devices/blinds.py` & `dirigera-0.1.6/src/dirigera/devices/blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.5/src/dirigera/devices/environment_sensor.py` & `dirigera-0.1.6/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.5/src/dirigera/devices/light.py` & `dirigera-0.1.6/src/dirigera/devices/light.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.5/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-0.1.6/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.5/src/dirigera/hub/auth.py` & `dirigera-0.1.6/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.5/src/dirigera/hub/hub.py` & `dirigera-0.1.6/src/dirigera/hub/hub.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import websocket
 from urllib3.exceptions import InsecureRequestWarning
 
 from .abstract_smart_home_hub import AbstractSmartHomeHub
 from ..devices.light import Light, dict_to_light
 from ..devices.blinds import Blind, dict_to_blind
 from ..devices.environment_sensor import EnvironmentSensor, dict_to_environment_sensor
+from ..devices.open_close_sensor import OpenCloseSensor, dict_to_open_close_sensor
 
 requests.packages.urllib3.disable_warnings(  # pylint: disable=no-member
     category=InsecureRequestWarning
 )
 
 
 class Hub(AbstractSmartHomeHub):
@@ -109,14 +110,24 @@
         """
         devices = self.get("/devices")
         sensors = list(
             filter(lambda x: x["deviceType"] == "environmentSensor", devices)
         )
         return [dict_to_environment_sensor(sensor, self) for sensor in sensors]
 
+    def get_open_close_sensors(self) -> List[OpenCloseSensor]:
+        """
+        Fetches all open/close sensors registered in the Hub
+        """
+        devices = self.get("/devices")
+        sensors = list(
+            filter(lambda x: x["deviceType"] == "openCloseSensor", devices)
+        )
+        return [dict_to_open_close_sensor(sensor, self) for sensor in sensors]
+
     def get_blinds(self) -> List[Blind]:
         """
         Fetches all blinds registered in the Hub
         """
         devices = self.get("/devices")
         blinds = list(filter(lambda x: x["type"] == "blinds", devices))
         return [dict_to_blind(blind, self) for blind in blinds]
```

### Comparing `dirigera-0.1.5/src/dirigera.egg-info/PKG-INFO` & `dirigera-0.1.6/src/dirigera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.5
+Version: 0.1.6
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dirigera-0.1.5/src/dirigera.egg-info/SOURCES.txt` & `dirigera-0.1.6/src/dirigera.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 src/dirigera.egg-info/requires.txt
 src/dirigera.egg-info/top_level.txt
 src/dirigera/devices/__init__.py
 src/dirigera/devices/blinds.py
 src/dirigera/devices/device.py
 src/dirigera/devices/environment_sensor.py
 src/dirigera/devices/light.py
+src/dirigera/devices/open_close_sensor.py
 src/dirigera/hub/__init__.py
 src/dirigera/hub/abstract_smart_home_hub.py
 src/dirigera/hub/auth.py
 src/dirigera/hub/hub.py
 tests/test_blinds.py
 tests/test_environment_sensor.py
-tests/test_light.py
+tests/test_light.py
+tests/test_open_close_sensor.py
```

### Comparing `dirigera-0.1.5/tests/test_blinds.py` & `dirigera-0.1.6/tests/test_blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.5/tests/test_environment_sensor.py` & `dirigera-0.1.6/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.5/tests/test_light.py` & `dirigera-0.1.6/tests/test_light.py`

 * *Files identical despite different names*

