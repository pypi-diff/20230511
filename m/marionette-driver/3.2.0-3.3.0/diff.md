# Comparing `tmp/marionette_driver-3.2.0.tar.gz` & `tmp/marionette_driver-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marionette_driver-3.2.0.tar", last modified: Mon Feb 20 11:04:17 2023, max compression
+gzip compressed data, was "marionette_driver-3.3.0.tar", last modified: Thu May 11 06:59:50 2023, max compression
```

## Comparing `marionette_driver-3.2.0.tar` & `marionette_driver-3.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-02-20 11:04:17.022887 marionette_driver-3.2.0/
--rw-r--r--   0 henrik     (501) staff       (20)      955 2023-02-20 11:04:17.022740 marionette_driver-3.2.0/PKG-INFO
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-02-20 11:04:17.021376 marionette_driver-3.2.0/marionette_driver/
--rw-r--r--   0 henrik     (501) staff       (20)      549 2023-02-11 14:12:25.000000 marionette_driver-3.2.0/marionette_driver/__init__.py
--rw-r--r--   0 henrik     (501) staff       (20)     2540 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/addons.py
--rw-r--r--   0 henrik     (501) staff       (20)      857 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/by.py
--rw-r--r--   0 henrik     (501) staff       (20)     1524 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/date_time_value.py
--rw-r--r--   0 henrik     (501) staff       (20)     2214 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/decorators.py
--rw-r--r--   0 henrik     (501) staff       (20)     5195 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/errors.py
--rw-r--r--   0 henrik     (501) staff       (20)     9697 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/expected.py
--rw-r--r--   0 henrik     (501) staff       (20)    26001 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/geckoinstance.py
--rw-r--r--   0 henrik     (501) staff       (20)     2384 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/keys.py
--rw-r--r--   0 henrik     (501) staff       (20)     2282 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/localization.py
--rw-r--r--   0 henrik     (501) staff       (20)    77513 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/marionette.py
--rw-r--r--   0 henrik     (501) staff       (20)     3087 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/timeout.py
--rw-r--r--   0 henrik     (501) staff       (20)    13614 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/transport.py
--rw-r--r--   0 henrik     (501) staff       (20)     6206 2023-01-24 07:51:21.000000 marionette_driver-3.2.0/marionette_driver/wait.py
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-02-20 11:04:17.022548 marionette_driver-3.2.0/marionette_driver.egg-info/
--rw-r--r--   0 henrik     (501) staff       (20)      955 2023-02-20 11:04:16.000000 marionette_driver-3.2.0/marionette_driver.egg-info/PKG-INFO
--rw-r--r--   0 henrik     (501) staff       (20)      691 2023-02-20 11:04:16.000000 marionette_driver-3.2.0/marionette_driver.egg-info/SOURCES.txt
--rw-r--r--   0 henrik     (501) staff       (20)        1 2023-02-20 11:04:16.000000 marionette_driver-3.2.0/marionette_driver.egg-info/dependency_links.txt
--rw-r--r--   0 henrik     (501) staff       (20)        1 2023-02-11 14:13:30.000000 marionette_driver-3.2.0/marionette_driver.egg-info/not-zip-safe
--rw-r--r--   0 henrik     (501) staff       (20)       39 2023-02-20 11:04:16.000000 marionette_driver-3.2.0/marionette_driver.egg-info/requires.txt
--rw-r--r--   0 henrik     (501) staff       (20)       18 2023-02-20 11:04:16.000000 marionette_driver-3.2.0/marionette_driver.egg-info/top_level.txt
--rw-r--r--   0 henrik     (501) staff       (20)       43 2022-10-11 19:23:51.000000 marionette_driver-3.2.0/requirements.txt
--rw-r--r--   0 henrik     (501) staff       (20)       38 2023-02-20 11:04:17.022933 marionette_driver-3.2.0/setup.cfg
--rw-r--r--   0 henrik     (501) staff       (20)     1791 2023-02-11 14:12:25.000000 marionette_driver-3.2.0/setup.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-05-11 06:59:50.141397 marionette_driver-3.3.0/
+-rw-r--r--   0 henrik     (501) staff       (20)      955 2023-05-11 06:59:50.141218 marionette_driver-3.3.0/PKG-INFO
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-05-11 06:59:50.140055 marionette_driver-3.3.0/marionette_driver/
+-rw-r--r--   0 henrik     (501) staff       (20)      549 2023-05-11 06:58:48.000000 marionette_driver-3.3.0/marionette_driver/__init__.py
+-rw-r--r--   0 henrik     (501) staff       (20)     2540 2023-04-11 15:20:28.000000 marionette_driver-3.3.0/marionette_driver/addons.py
+-rw-r--r--   0 henrik     (501) staff       (20)      857 2023-04-11 15:20:28.000000 marionette_driver-3.3.0/marionette_driver/by.py
+-rw-r--r--   0 henrik     (501) staff       (20)     1524 2023-04-11 15:20:28.000000 marionette_driver-3.3.0/marionette_driver/date_time_value.py
+-rw-r--r--   0 henrik     (501) staff       (20)     2214 2023-04-11 15:20:28.000000 marionette_driver-3.3.0/marionette_driver/decorators.py
+-rw-r--r--   0 henrik     (501) staff       (20)     5195 2023-04-11 15:20:28.000000 marionette_driver-3.3.0/marionette_driver/errors.py
+-rw-r--r--   0 henrik     (501) staff       (20)     9697 2023-04-11 15:20:28.000000 marionette_driver-3.3.0/marionette_driver/expected.py
+-rw-r--r--   0 henrik     (501) staff       (20)    25935 2023-04-25 15:37:57.000000 marionette_driver-3.3.0/marionette_driver/geckoinstance.py
+-rw-r--r--   0 henrik     (501) staff       (20)     2384 2023-04-11 15:20:28.000000 marionette_driver-3.3.0/marionette_driver/keys.py
+-rw-r--r--   0 henrik     (501) staff       (20)     2282 2023-04-11 15:20:28.000000 marionette_driver-3.3.0/marionette_driver/localization.py
+-rw-r--r--   0 henrik     (501) staff       (20)    79105 2023-04-25 15:37:57.000000 marionette_driver-3.3.0/marionette_driver/marionette.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3087 2023-04-11 15:20:28.000000 marionette_driver-3.3.0/marionette_driver/timeout.py
+-rw-r--r--   0 henrik     (501) staff       (20)    13614 2023-04-11 15:20:28.000000 marionette_driver-3.3.0/marionette_driver/transport.py
+-rw-r--r--   0 henrik     (501) staff       (20)     6206 2023-04-11 15:20:28.000000 marionette_driver-3.3.0/marionette_driver/wait.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-05-11 06:59:50.140958 marionette_driver-3.3.0/marionette_driver.egg-info/
+-rw-r--r--   0 henrik     (501) staff       (20)      955 2023-05-11 06:59:50.000000 marionette_driver-3.3.0/marionette_driver.egg-info/PKG-INFO
+-rw-r--r--   0 henrik     (501) staff       (20)      691 2023-05-11 06:59:50.000000 marionette_driver-3.3.0/marionette_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        1 2023-05-11 06:59:50.000000 marionette_driver-3.3.0/marionette_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        1 2023-05-11 06:59:40.000000 marionette_driver-3.3.0/marionette_driver.egg-info/not-zip-safe
+-rw-r--r--   0 henrik     (501) staff       (20)       39 2023-05-11 06:59:50.000000 marionette_driver-3.3.0/marionette_driver.egg-info/requires.txt
+-rw-r--r--   0 henrik     (501) staff       (20)       18 2023-05-11 06:59:50.000000 marionette_driver-3.3.0/marionette_driver.egg-info/top_level.txt
+-rw-r--r--   0 henrik     (501) staff       (20)       43 2022-10-11 19:23:51.000000 marionette_driver-3.3.0/requirements.txt
+-rw-r--r--   0 henrik     (501) staff       (20)       38 2023-05-11 06:59:50.141443 marionette_driver-3.3.0/setup.cfg
+-rw-r--r--   0 henrik     (501) staff       (20)     1791 2023-04-25 15:37:57.000000 marionette_driver-3.3.0/setup.py
```

### Comparing `marionette_driver-3.2.0/PKG-INFO` & `marionette_driver-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marionette_driver
-Version: 3.2.0
+Version: 3.3.0
 Summary: Marionette Driver
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Marionette
 Author: Auto-tools
 Author-email: dev-webdriver@mozilla.org
 License: MPL
 Keywords: mozilla
 Platform: UNKNOWN
```

### Comparing `marionette_driver-3.2.0/marionette_driver/__init__.py` & `marionette_driver-3.3.0/marionette_driver/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "3.2.0"
+__version__ = "3.3.0"
 
 from marionette_driver import (
     addons,
     by,
     date_time_value,
     decorators,
     errors,
```

### Comparing `marionette_driver-3.2.0/marionette_driver/addons.py` & `marionette_driver-3.3.0/marionette_driver/addons.py`

 * *Files identical despite different names*

### Comparing `marionette_driver-3.2.0/marionette_driver/by.py` & `marionette_driver-3.3.0/marionette_driver/by.py`

 * *Files identical despite different names*

### Comparing `marionette_driver-3.2.0/marionette_driver/date_time_value.py` & `marionette_driver-3.3.0/marionette_driver/date_time_value.py`

 * *Files identical despite different names*

### Comparing `marionette_driver-3.2.0/marionette_driver/decorators.py` & `marionette_driver-3.3.0/marionette_driver/decorators.py`

 * *Files identical despite different names*

### Comparing `marionette_driver-3.2.0/marionette_driver/errors.py` & `marionette_driver-3.3.0/marionette_driver/errors.py`

 * *Files identical despite different names*

### Comparing `marionette_driver-3.2.0/marionette_driver/expected.py` & `marionette_driver-3.3.0/marionette_driver/expected.py`

 * *Files identical despite different names*

### Comparing `marionette_driver-3.2.0/marionette_driver/geckoinstance.py` & `marionette_driver-3.3.0/marionette_driver/geckoinstance.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,16 +303,15 @@
         args["preferences"]["marionette.defaultPrefs.port"] = self.marionette_port
 
         if self.prefs:
             args["preferences"].update(self.prefs)
 
         if self.verbose:
             level = "Trace" if self.verbose >= 2 else "Debug"
-            args["preferences"]["marionette.log.level"] = level
-            args["preferences"]["marionette.logging"] = level
+            args["preferences"]["remote.log.level"] = level
 
         if "-jsdebugger" in self.app_args:
             args["preferences"].update(
                 {
                     "devtools.browsertoolbox.panel": "jsdebugger",
                     "devtools.chrome.enabled": True,
                     "devtools.debugger.prompt-connection": False,
```

### Comparing `marionette_driver-3.2.0/marionette_driver/keys.py` & `marionette_driver-3.3.0/marionette_driver/keys.py`

 * *Files identical despite different names*

### Comparing `marionette_driver-3.2.0/marionette_driver/localization.py` & `marionette_driver-3.3.0/marionette_driver/localization.py`

 * *Files identical despite different names*

### Comparing `marionette_driver-3.2.0/marionette_driver/marionette.py` & `marionette_driver-3.3.0/marionette_driver/marionette.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,14 +352,28 @@
     @property
     def shadow_root(self):
         """Gets the shadow root of the current element"""
         return self.marionette._send_message(
             "WebDriver:GetShadowRoot", {"id": self.id}, key="value"
         )
 
+    @property
+    def computed_label(self):
+        """Gets the computed accessibility label of the current element"""
+        return self.marionette._send_message(
+            "WebDriver:GetComputedLabel", {"id": self.id}, key="value"
+        )
+
+    @property
+    def computed_role(self):
+        """Gets the computed accessibility role of the current element"""
+        return self.marionette._send_message(
+            "WebDriver:GetComputedRole", {"id": self.id}, key="value"
+        )
+
     @classmethod
     def _from_json(cls, json, marionette):
         if isinstance(json, dict):
             if WEB_ELEMENT_KEY in json:
                 return cls(marionette, json[WEB_ELEMENT_KEY], WEB_ELEMENT_KEY)
             elif FRAME_KEY in json:
                 return cls(marionette, json[FRAME_KEY], FRAME_KEY)
@@ -385,14 +399,40 @@
     def __eq__(self, other_element):
         return self.id == other_element.id
 
     def __hash__(self):
         # pylint --py3k: W1641
         return hash(self.id)
 
+    def find_element(self, method, target):
+        """Returns an ``HTMLElement`` instance that matches the specified
+        method and target, relative to the current shadow root.
+
+        For more details on this function, see the
+        :func:`~marionette_driver.marionette.Marionette.find_element` method
+        in the Marionette class.
+        """
+        body = {"shadowRoot": self.id, "value": target, "using": method}
+        return self.marionette._send_message(
+            "WebDriver:FindElementFromShadowRoot", body, key="value"
+        )
+
+    def find_elements(self, method, target):
+        """Returns a list of all ``HTMLElement`` instances that match the
+         specified method and target in the current shadow root.
+
+        For more details on this function, see the
+        :func:`~marionette_driver.marionette.Marionette.find_elements` method
+        in the Marionette class.
+        """
+        body = {"shadowRoot": self.id, "value": target, "using": method}
+        return self.marionette._send_message(
+            "WebDriver:FindElementsFromShadowRoot", body
+        )
+
     @classmethod
     def _from_json(cls, json, marionette):
         if isinstance(json, dict):
             if WEB_SHADOW_ROOT_KEY in json:
                 return cls(marionette, json[WEB_SHADOW_ROOT_KEY])
         raise ValueError("Unrecognised shadow root")
```

### Comparing `marionette_driver-3.2.0/marionette_driver/timeout.py` & `marionette_driver-3.3.0/marionette_driver/timeout.py`

 * *Files identical despite different names*

### Comparing `marionette_driver-3.2.0/marionette_driver/transport.py` & `marionette_driver-3.3.0/marionette_driver/transport.py`

 * *Files identical despite different names*

### Comparing `marionette_driver-3.2.0/marionette_driver/wait.py` & `marionette_driver-3.3.0/marionette_driver/wait.py`

 * *Files identical despite different names*

### Comparing `marionette_driver-3.2.0/marionette_driver.egg-info/PKG-INFO` & `marionette_driver-3.3.0/marionette_driver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marionette-driver
-Version: 3.2.0
+Version: 3.3.0
 Summary: Marionette Driver
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Marionette
 Author: Auto-tools
 Author-email: dev-webdriver@mozilla.org
 License: MPL
 Keywords: mozilla
 Platform: UNKNOWN
```

### Comparing `marionette_driver-3.2.0/marionette_driver.egg-info/SOURCES.txt` & `marionette_driver-3.3.0/marionette_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marionette_driver-3.2.0/setup.py` & `marionette_driver-3.3.0/setup.py`

 * *Files identical despite different names*

