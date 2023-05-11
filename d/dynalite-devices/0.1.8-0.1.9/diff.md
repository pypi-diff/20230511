# Comparing `tmp/dynalite_devices-0.1.8.tar.gz` & `tmp/dynalite_devices-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynalite_devices-0.1.8.tar", last modified: Sun Oct 13 21:36:02 2019, max compression
+gzip compressed data, was "dist/dynalite_devices-0.1.9.tar", last modified: Mon Oct 14 20:13:23 2019, max compression
```

## Comparing `dynalite_devices-0.1.8.tar` & `dynalite_devices-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-13 21:36:03.000000 dynalite_devices-0.1.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-13 21:36:03.000000 dynalite_devices-0.1.8/dynalite_devices.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)        1 2019-10-13 21:36:02.000000 dynalite_devices-0.1.8/dynalite_devices.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)      884 2019-10-13 21:36:02.000000 dynalite_devices-0.1.8/dynalite_devices.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)       17 2019-10-13 21:36:02.000000 dynalite_devices-0.1.8/dynalite_devices.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)      508 2019-10-13 21:36:03.000000 dynalite_devices-0.1.8/dynalite_devices.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)       21 2019-10-13 21:36:02.000000 dynalite_devices-0.1.8/dynalite_devices.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-13 21:36:03.000000 dynalite_devices-0.1.8/dynalite_devices_lib/
--rwxr-xr-x   0 root         (0) root         (0)     1221 2019-10-13 19:54:53.000000 dynalite_devices-0.1.8/dynalite_devices_lib/const.py
--rwxr-xr-x   0 root         (0) root         (0)     5838 2019-10-13 20:21:03.000000 dynalite_devices-0.1.8/dynalite_devices_lib/cover.py
--rwxr-xr-x   0 root         (0) root         (0)     3504 2019-10-13 20:15:02.000000 dynalite_devices-0.1.8/dynalite_devices_lib/dynalitebase.py
--rwxr-xr-x   0 root         (0) root         (0)    22704 2019-10-13 20:24:01.000000 dynalite_devices-0.1.8/dynalite_devices_lib/dynalite_devices.py
--rwxr-xr-x   0 root         (0) root         (0)     1499 2019-10-13 20:02:03.000000 dynalite_devices-0.1.8/dynalite_devices_lib/light.py
--rwxr-xr-x   0 root         (0) root         (0)     3595 2019-10-13 20:01:12.000000 dynalite_devices-0.1.8/dynalite_devices_lib/switch.py
--rwxr-xr-x   0 root         (0) root         (0)      102 2019-10-09 18:14:35.000000 dynalite_devices-0.1.8/dynalite_devices_lib/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       50 2019-10-13 11:16:05.000000 dynalite_devices-0.1.8/dynalite_devices_lib/__version__.py
--rwxr-xr-x   0 root         (0) root         (0)     1088 2019-09-20 06:57:37.000000 dynalite_devices-0.1.8/LICENSE.md
--rwxr-xr-x   0 root         (0) root         (0)       39 2019-09-20 06:57:37.000000 dynalite_devices-0.1.8/MANIFEST.in
--rwxr-xr-x   0 root         (0) root         (0)      884 2019-10-13 21:36:03.000000 dynalite_devices-0.1.8/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)       78 2019-10-05 18:39:23.000000 dynalite_devices-0.1.8/README.md
--rwxr-xr-x   0 root         (0) root         (0)       38 2019-10-13 21:36:03.000000 dynalite_devices-0.1.8/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     8861 2019-10-13 11:15:37.000000 dynalite_devices-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-14 20:13:24.000000 dynalite_devices-0.1.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-14 20:13:24.000000 dynalite_devices-0.1.9/dynalite_devices.egg-info/
+-rwxr-xr-x   0 root         (0) root         (0)        1 2019-10-14 20:13:24.000000 dynalite_devices-0.1.9/dynalite_devices.egg-info/dependency_links.txt
+-rwxr-xr-x   0 root         (0) root         (0)      884 2019-10-14 20:13:24.000000 dynalite_devices-0.1.9/dynalite_devices.egg-info/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)       17 2019-10-14 20:13:24.000000 dynalite_devices-0.1.9/dynalite_devices.egg-info/requires.txt
+-rwxr-xr-x   0 root         (0) root         (0)      508 2019-10-14 20:13:24.000000 dynalite_devices-0.1.9/dynalite_devices.egg-info/SOURCES.txt
+-rwxr-xr-x   0 root         (0) root         (0)       21 2019-10-14 20:13:24.000000 dynalite_devices-0.1.9/dynalite_devices.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-14 20:13:24.000000 dynalite_devices-0.1.9/dynalite_devices_lib/
+-rwxr-xr-x   0 root         (0) root         (0)     1330 2019-10-14 19:19:48.000000 dynalite_devices-0.1.9/dynalite_devices_lib/const.py
+-rwxr-xr-x   0 root         (0) root         (0)     5838 2019-10-13 20:21:03.000000 dynalite_devices-0.1.9/dynalite_devices_lib/cover.py
+-rwxr-xr-x   0 root         (0) root         (0)     3504 2019-10-13 20:15:02.000000 dynalite_devices-0.1.9/dynalite_devices_lib/dynalitebase.py
+-rwxr-xr-x   0 root         (0) root         (0)    22705 2019-10-14 20:12:02.000000 dynalite_devices-0.1.9/dynalite_devices_lib/dynalite_devices.py
+-rwxr-xr-x   0 root         (0) root         (0)     1499 2019-10-13 20:02:03.000000 dynalite_devices-0.1.9/dynalite_devices_lib/light.py
+-rwxr-xr-x   0 root         (0) root         (0)     3595 2019-10-13 20:01:12.000000 dynalite_devices-0.1.9/dynalite_devices_lib/switch.py
+-rwxr-xr-x   0 root         (0) root         (0)     5226 2019-10-14 20:12:01.000000 dynalite_devices-0.1.9/dynalite_devices_lib/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       50 2019-10-14 20:05:19.000000 dynalite_devices-0.1.9/dynalite_devices_lib/__version__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1088 2019-09-20 06:57:37.000000 dynalite_devices-0.1.9/LICENSE.md
+-rwxr-xr-x   0 root         (0) root         (0)       39 2019-09-20 06:57:37.000000 dynalite_devices-0.1.9/MANIFEST.in
+-rwxr-xr-x   0 root         (0) root         (0)      884 2019-10-14 20:13:24.000000 dynalite_devices-0.1.9/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)       78 2019-10-05 18:39:23.000000 dynalite_devices-0.1.9/README.md
+-rwxr-xr-x   0 root         (0) root         (0)       38 2019-10-14 20:13:24.000000 dynalite_devices-0.1.9/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     8861 2019-10-14 20:09:55.000000 dynalite_devices-0.1.9/setup.py
```

### Comparing `dynalite_devices-0.1.8/dynalite_devices.egg-info/PKG-INFO` & `dynalite_devices-0.1.9/dynalite_devices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynalite-devices
-Version: 0.1.8
+Version: 0.1.9
 Summary: An unofficial Dynalite DyNET interface creating devices.
 Home-page: https://github.com/ziv1234/python-dynalite-devices
 Author: Ziv
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ziv1234/python-dynalite-devices/issues
 Project-URL: Source, https://github.com/ziv1234/python-dynalite-devices
 Description: # python-dynalite-devices
```

### Comparing `dynalite_devices-0.1.8/dynalite_devices_lib/const.py` & `dynalite_devices-0.1.9/dynalite_devices_lib/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 
 CONF_AREAOVERRIDE = "areaoverride"
 CONF_CHANNELCOVER = "channelcover"
 CONF_CHANNELTYPE = "type"
 CONF_CHANNELCLASS = "class"
 CONF_FACTOR = "factor"
 CONF_HIDDENENTITY = "hidden"
+CONF_HOST = "host"
+CONF_NAME = "name"
 CONF_NONE = "none"
+CONF_PORT = "port"
 CONF_ROOM = "room"
 CONF_ROOM_ON = "room_on"
 CONF_ROOM_OFF = "room_off"
 CONF_TEMPLATE = "template"
 CONF_TEMPLATEOVERRIDE = "templateoverride"
 CONF_TILTPERCENTAGE = "tilt"
 CONF_TRIGGER = "trigger"
@@ -25,14 +28,16 @@
 ATTR_POSITION = "position"
 ATTR_TILT_POSITION = "tilt_position"
 
 DEFAULT_CHANNELTYPE = "light"
 DEFAULT_COVERCHANNELCLASS = "shutter"
 # cover goes from closed(0.0) to open (1.0). If it needs less than the range, use a lower number
 DEFAULT_COVERFACTOR = 1.0
+DEFAULT_NAME = "dynalite"
+DEFAULT_PORT = 12345
 DEFAULT_TEMPLATES = {
     CONF_ROOM: {CONF_ROOM_ON: "1", CONF_ROOM_OFF: "4"},
     CONF_TRIGGER: {CONF_TRIGGER: "1"},
     CONF_HIDDENENTITY: {},
     CONF_CHANNELCOVER: {
         CONF_CHANNEL: "1",
         CONF_CHANNELCLASS: DEFAULT_COVERCHANNELCLASS,
```

### Comparing `dynalite_devices-0.1.8/dynalite_devices_lib/cover.py` & `dynalite_devices-0.1.9/dynalite_devices_lib/cover.py`

 * *Files identical despite different names*

### Comparing `dynalite_devices-0.1.8/dynalite_devices_lib/dynalitebase.py` & `dynalite_devices-0.1.9/dynalite_devices_lib/dynalitebase.py`

 * *Files identical despite different names*

### Comparing `dynalite_devices-0.1.8/dynalite_devices_lib/dynalite_devices.py` & `dynalite_devices-0.1.9/dynalite_devices_lib/dynalite_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     EVENT_CONFIGURED,
     CONF_ACTION,
     CONF_ACTION_REPORT,
     CONF_ACTION_CMD,
     CONF_TRGT_LEVEL,
     CONF_ACT_LEVEL,
     CONF_ALL,
-    Dynalite
+    Dynalite,
 )
 
 from .light import DynaliteChannelLightDevice
 from .switch import (
     DynaliteChannelSwitchDevice,
     DynalitePresetSwitchDevice,
     DynaliteDualPresetSwitchDevice,
```

### Comparing `dynalite_devices-0.1.8/dynalite_devices_lib/light.py` & `dynalite_devices-0.1.9/dynalite_devices_lib/light.py`

 * *Files identical despite different names*

### Comparing `dynalite_devices-0.1.8/dynalite_devices_lib/switch.py` & `dynalite_devices-0.1.9/dynalite_devices_lib/switch.py`

 * *Files identical despite different names*

### Comparing `dynalite_devices-0.1.8/LICENSE.md` & `dynalite_devices-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dynalite_devices-0.1.8/PKG-INFO` & `dynalite_devices-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynalite_devices
-Version: 0.1.8
+Version: 0.1.9
 Summary: An unofficial Dynalite DyNET interface creating devices.
 Home-page: https://github.com/ziv1234/python-dynalite-devices
 Author: Ziv
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ziv1234/python-dynalite-devices/issues
 Project-URL: Source, https://github.com/ziv1234/python-dynalite-devices
 Description: # python-dynalite-devices
```

### Comparing `dynalite_devices-0.1.8/setup.py` & `dynalite_devices-0.1.9/setup.py`

 * *Files identical despite different names*

