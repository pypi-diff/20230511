# Comparing `tmp/el_decko_core-2023.5.8.tar.gz` & `tmp/el_decko_core-2023.5.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "el_decko_core-2023.5.8.tar", last modified: Mon May  8 15:52:52 2023, max compression
+gzip compressed data, was "el_decko_core-2023.5.8.1.tar", last modified: Mon May  8 21:06:47 2023, max compression
```

## Comparing `el_decko_core-2023.5.8.tar` & `el_decko_core-2023.5.8.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-08 15:52:52.965257 el_decko_core-2023.5.8/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)    35149 2023-03-22 10:21:15.000000 el_decko_core-2023.5.8/LICENSE
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4804 2023-05-08 15:52:52.965257 el_decko_core-2023.5.8/PKG-INFO
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4440 2023-05-06 21:00:41.000000 el_decko_core-2023.5.8/README.md
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-08 15:52:52.965257 el_decko_core-2023.5.8/ed_core/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1315 2023-05-08 14:49:14.000000 el_decko_core-2023.5.8/ed_core/__init__.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1660 2023-03-22 10:21:16.000000 el_decko_core-2023.5.8/ed_core/dyn_data.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2015 2023-05-08 14:09:42.000000 el_decko_core-2023.5.8/ed_core/streamdeck.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2694 2023-03-22 10:21:16.000000 el_decko_core-2023.5.8/ed_core/streamdeck_config.py
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-08 15:52:52.965257 el_decko_core-2023.5.8/el_decko_core.egg-info/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4804 2023-05-08 15:52:52.000000 el_decko_core-2023.5.8/el_decko_core.egg-info/PKG-INFO
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      347 2023-05-08 15:52:52.000000 el_decko_core-2023.5.8/el_decko_core.egg-info/SOURCES.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        1 2023-05-08 15:52:52.000000 el_decko_core-2023.5.8/el_decko_core.egg-info/dependency_links.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       40 2023-05-08 15:52:52.000000 el_decko_core-2023.5.8/el_decko_core.egg-info/entry_points.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      112 2023-05-08 15:52:52.000000 el_decko_core-2023.5.8/el_decko_core.egg-info/requires.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        8 2023-05-08 15:52:52.000000 el_decko_core-2023.5.8/el_decko_core.egg-info/top_level.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      740 2023-05-07 16:57:24.000000 el_decko_core-2023.5.8/pyproject.toml
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       38 2023-05-08 15:52:52.965257 el_decko_core-2023.5.8/setup.cfg
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-08 21:06:47.276672 el_decko_core-2023.5.8.1/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)    35149 2023-03-22 10:21:15.000000 el_decko_core-2023.5.8.1/LICENSE
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4806 2023-05-08 21:06:47.276672 el_decko_core-2023.5.8.1/PKG-INFO
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4440 2023-05-06 21:00:41.000000 el_decko_core-2023.5.8.1/README.md
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-08 21:06:47.276672 el_decko_core-2023.5.8.1/ed_core/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1317 2023-05-08 20:55:16.000000 el_decko_core-2023.5.8.1/ed_core/__init__.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1660 2023-03-22 10:21:16.000000 el_decko_core-2023.5.8.1/ed_core/dyn_data.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      806 2023-05-08 21:02:31.000000 el_decko_core-2023.5.8.1/ed_core/query_deck.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1813 2023-05-08 20:52:23.000000 el_decko_core-2023.5.8.1/ed_core/streamdeck.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2694 2023-03-22 10:21:16.000000 el_decko_core-2023.5.8.1/ed_core/streamdeck_config.py
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-08 21:06:47.276672 el_decko_core-2023.5.8.1/el_decko_core.egg-info/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4806 2023-05-08 21:06:47.000000 el_decko_core-2023.5.8.1/el_decko_core.egg-info/PKG-INFO
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      369 2023-05-08 21:06:47.000000 el_decko_core-2023.5.8.1/el_decko_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        1 2023-05-08 21:06:47.000000 el_decko_core-2023.5.8.1/el_decko_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       40 2023-05-08 21:06:47.000000 el_decko_core-2023.5.8.1/el_decko_core.egg-info/entry_points.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      112 2023-05-08 21:06:47.000000 el_decko_core-2023.5.8.1/el_decko_core.egg-info/requires.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        8 2023-05-08 21:06:47.000000 el_decko_core-2023.5.8.1/el_decko_core.egg-info/top_level.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      740 2023-05-07 16:57:24.000000 el_decko_core-2023.5.8.1/pyproject.toml
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       38 2023-05-08 21:06:47.276672 el_decko_core-2023.5.8.1/setup.cfg
```

### Comparing `el_decko_core-2023.5.8/LICENSE` & `el_decko_core-2023.5.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.5.8/PKG-INFO` & `el_decko_core-2023.5.8.1/el_decko_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: el_decko_core
-Version: 2023.5.8
+Name: el-decko-core
+Version: 2023.5.8.1
 Summary: El Decko Core
 License: GPL-3
 Project-URL: Homepage, https://github.com/Z-Ray-Entertainment/el_decko_core
 Project-URL: Bug Tracker, https://github.com/Z-Ray-Entertainment/el_decko_core/issues
 Platform: Linux
 Description-Content-Type: text/markdown
 Provides-Extra: backends
```

### Comparing `el_decko_core-2023.5.8/README.md` & `el_decko_core-2023.5.8.1/README.md`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.5.8/ed_core/__init__.py` & `el_decko_core-2023.5.8.1/ed_core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import threading
 from importlib.metadata import entry_points
 
 from ed_core import streamdeck
 from ed_core.streamdeck_config import load_config, apply_config
 
-VERSION = "2023.5.8"
+VERSION = "2023.5.8.1"
 BACKENDS = {}
 
 
 def run(standalone: bool = True):
     try:
         print("El Decko Core running.")
         load_config()
```

### Comparing `el_decko_core-2023.5.8/ed_core/dyn_data.py` & `el_decko_core-2023.5.8.1/ed_core/dyn_data.py`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.5.8/ed_core/streamdeck.py` & `el_decko_core-2023.5.8.1/ed_core/streamdeck.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from StreamDeck.DeviceManager import DeviceManager
 from StreamDeck.Devices.StreamDeck import StreamDeck
 
-from ed_core import streamdeck_config
+from ed_core import streamdeck_config, query_deck
 
 stream_decks = DeviceManager().enumerate()
 backends = []
 
 
 def initialize(edbs):
     global backends
@@ -34,38 +34,24 @@
 
 
 # Returns a list of all available Stream Decks
 def get_stream_decks():
     return stream_decks
 
 
-def get_supported_image_formats(deck: StreamDeck):
-    deck.key_image_format()
-
-
-def get_key_layout(deck: StreamDeck):
-    deck.key_layout()
-
-
-def get_key_count(deck: StreamDeck):
-    deck.key_count()
-
-
 def set_brightness(deck, brightness: int):
     deck.set_brightness(brightness)
 
 
 def get_key_config(deck_serial: str, key_num: int):
     for index, deck in enumerate(stream_decks):
-        deck.open()
-        if deck.get_serial_number() == deck_serial:
+        serial = query_deck.query_deck(deck, query_deck.QueryType.SERIAL)
+        if serial == deck_serial:
             streamdeck_config.load_config()
-            cfg = streamdeck_config.DECK_CFG[deck_serial]["key_config"][str(key_num)]
-            deck.close()
-            return cfg
+            return streamdeck_config.DECK_CFG[deck_serial]["key_config"][str(key_num)]
 
 
 def __key_change_callback(deck: StreamDeck, key, state):
     if state:
         cfg = streamdeck_config.DECK_CFG[deck.get_serial_number()]
         edb_id: str = cfg["key_config"][str(key)]["backend"]
         edb_event: str = cfg["key_config"][str(key)]["event"]
```

### Comparing `el_decko_core-2023.5.8/ed_core/streamdeck_config.py` & `el_decko_core-2023.5.8.1/ed_core/streamdeck_config.py`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.5.8/el_decko_core.egg-info/PKG-INFO` & `el_decko_core-2023.5.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: el-decko-core
-Version: 2023.5.8
+Name: el_decko_core
+Version: 2023.5.8.1
 Summary: El Decko Core
 License: GPL-3
 Project-URL: Homepage, https://github.com/Z-Ray-Entertainment/el_decko_core
 Project-URL: Bug Tracker, https://github.com/Z-Ray-Entertainment/el_decko_core/issues
 Platform: Linux
 Description-Content-Type: text/markdown
 Provides-Extra: backends
```

### Comparing `el_decko_core-2023.5.8/pyproject.toml` & `el_decko_core-2023.5.8.1/pyproject.toml`

 * *Files identical despite different names*

