# Comparing `tmp/winkeyerserial-23.2.17.tar.gz` & `tmp/winkeyerserial-23.5.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winkeyerserial-23.2.17.tar", last modified: Fri Feb 17 22:00:40 2023, max compression
+gzip compressed data, was "winkeyerserial-23.5.11.tar", last modified: Thu May 11 19:55:09 2023, max compression
```

## Comparing `winkeyerserial-23.2.17.tar` & `winkeyerserial-23.5.11.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 22:00:40.532129 winkeyerserial-23.2.17/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2021-04-26 00:57:26.000000 winkeyerserial-23.2.17/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2857 2023-02-17 22:00:40.532129 winkeyerserial-23.2.17/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2062 2023-02-17 21:58:17.000000 winkeyerserial-23.2.17/README.md
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1093 2023-02-17 21:59:53.000000 winkeyerserial-23.2.17/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-02-17 22:00:40.532129 winkeyerserial-23.2.17/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 22:00:40.531129 winkeyerserial-23.2.17/winkeyerserial/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-13 06:27:07.000000 winkeyerserial-23.2.17/winkeyerserial/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-01-13 06:27:07.000000 winkeyerserial-23.2.17/winkeyerserial/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15053 2023-02-17 21:47:49.000000 winkeyerserial-23.2.17/winkeyerserial/__main__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13458 2023-02-17 21:44:58.000000 winkeyerserial-23.2.17/winkeyerserial/k6gte-winkeyerserial-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1631 2023-02-17 21:44:22.000000 winkeyerserial-23.2.17/winkeyerserial/k6gte-winkeyerserial-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4652 2023-02-17 21:44:37.000000 winkeyerserial-23.2.17/winkeyerserial/k6gte-winkeyerserial-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      235 2023-02-17 21:46:11.000000 winkeyerserial-23.2.17/winkeyerserial/k6gte-winkeyerserial.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7773 2023-01-13 06:27:07.000000 winkeyerserial-23.2.17/winkeyerserial/main.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 22:00:40.532129 winkeyerserial-23.2.17/winkeyerserial.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2857 2023-02-17 22:00:40.000000 winkeyerserial-23.2.17/winkeyerserial.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      554 2023-02-17 22:00:40.000000 winkeyerserial-23.2.17/winkeyerserial.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-02-17 22:00:40.000000 winkeyerserial-23.2.17/winkeyerserial.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-02-17 22:00:40.000000 winkeyerserial-23.2.17/winkeyerserial.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       15 2023-02-17 22:00:40.000000 winkeyerserial-23.2.17/winkeyerserial.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       24 2023-02-17 22:00:40.000000 winkeyerserial-23.2.17/winkeyerserial.egg-info/top_level.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-11 19:55:09.792730 winkeyerserial-23.5.11/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2021-04-26 00:57:26.000000 winkeyerserial-23.5.11/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2905 2023-05-11 19:55:09.791730 winkeyerserial-23.5.11/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2110 2023-05-11 19:54:52.000000 winkeyerserial-23.5.11/README.md
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1093 2023-05-11 19:52:32.000000 winkeyerserial-23.5.11/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-11 19:55:09.792730 winkeyerserial-23.5.11/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-11 19:55:09.790730 winkeyerserial-23.5.11/winkeyerserial/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-13 06:27:07.000000 winkeyerserial-23.5.11/winkeyerserial/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-01-13 06:27:07.000000 winkeyerserial-23.5.11/winkeyerserial/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15176 2023-05-11 19:47:47.000000 winkeyerserial-23.5.11/winkeyerserial/__main__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13458 2023-02-17 21:44:58.000000 winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1631 2023-02-17 21:44:22.000000 winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4652 2023-02-17 21:44:37.000000 winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      235 2023-02-17 21:46:11.000000 winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7773 2023-01-13 06:27:07.000000 winkeyerserial-23.5.11/winkeyerserial/main.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-11 19:55:09.791730 winkeyerserial-23.5.11/winkeyerserial.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2905 2023-05-11 19:55:09.000000 winkeyerserial-23.5.11/winkeyerserial.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      554 2023-05-11 19:55:09.000000 winkeyerserial-23.5.11/winkeyerserial.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-11 19:55:09.000000 winkeyerserial-23.5.11/winkeyerserial.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-11 19:55:09.000000 winkeyerserial-23.5.11/winkeyerserial.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       15 2023-05-11 19:55:09.000000 winkeyerserial-23.5.11/winkeyerserial.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       24 2023-05-11 19:55:09.000000 winkeyerserial-23.5.11/winkeyerserial.egg-info/top_level.txt
```

### Comparing `winkeyerserial-23.2.17/LICENSE` & `winkeyerserial-23.5.11/LICENSE`

 * *Files identical despite different names*

### Comparing `winkeyerserial-23.2.17/PKG-INFO` & `winkeyerserial-23.5.11/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winkeyerserial
-Version: 23.2.17
+Version: 23.5.11
 Summary: Talk to K1EL winkeyer
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/PyWinKeyerSerial
 Project-URL: Bug Tracker, https://github.com/mbridak/PyWinKeyerSerial/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -50,11 +50,12 @@
 
 # remove
 pip uninstall winkeyerserial
 ```
 
 ## What's new
 
+- [23-5-11] Added xmlrpc function to set speed.
 - [23-2-17] Added serial device descriptions (hover tooltip) to the detected serial devices in the dropdown.
 - Added an XMLRPC server. So now my [Winter Field Day](https://github.com/mbridak/WinterFieldDayLogger), [Field Day](https://github.com/mbridak/FieldDayLogger) and [K1USNSST](https://github.com/mbridak/k1usnsst) Loggers will be able to send CW macros to this. The interface for the client is dead simple:
  `xmlrpc.client.ServerProxy("http://localhost:8000").k1elsendstring("Hello World")`
  That's it...
```

### Comparing `winkeyerserial-23.2.17/README.md` & `winkeyerserial-23.5.11/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -31,11 +31,12 @@
 
 # remove
 pip uninstall winkeyerserial
 ```
 
 ## What's new
 
+- [23-5-11] Added xmlrpc function to set speed.
 - [23-2-17] Added serial device descriptions (hover tooltip) to the detected serial devices in the dropdown.
 - Added an XMLRPC server. So now my [Winter Field Day](https://github.com/mbridak/WinterFieldDayLogger), [Field Day](https://github.com/mbridak/FieldDayLogger) and [K1USNSST](https://github.com/mbridak/k1usnsst) Loggers will be able to send CW macros to this. The interface for the client is dead simple:
  `xmlrpc.client.ServerProxy("http://localhost:8000").k1elsendstring("Hello World")`
  That's it...
```

### Comparing `winkeyerserial-23.2.17/pyproject.toml` & `winkeyerserial-23.5.11/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "winkeyerserial" 
-version = "23.2.17"
+version = "23.5.11"
 description = "Talk to K1EL winkeyer"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `winkeyerserial-23.2.17/winkeyerserial/JetBrainsMono-Regular.ttf` & `winkeyerserial-23.5.11/winkeyerserial/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `winkeyerserial-23.2.17/winkeyerserial/__main__.py` & `winkeyerserial-23.5.11/winkeyerserial/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     def run(self):
         """Doc String"""
         # sleep a little bit to make sure QApplication is running.
         self.sleep(1)
         print("--- starting server…")
         with SimpleXMLRPCServer(("0.0.0.0", 8000), allow_none=True) as self.server:
             self.server.register_function(k1elsendstring)
+            self.server.register_function(setspeed)
             self.server.register_introspection_functions()
             self.server.serve_forever()
 
 
 class RPCWidget(QWidget):
     """Doc String"""
 
@@ -423,14 +424,19 @@
 if keyer.port:
     keyer.setmode()
 rpcwidget = RPCWidget()
 timer = QTimer()
 timer.timeout.connect(keyer.checkmessage)  # Do not do this.
 
 
+def setspeed(speed) -> None:
+    """doc"""
+    keyer.setspeed(speed)
+
+
 def main():
     """Main entry"""
     os.system(
         "xdg-icon-resource install --size 32 --context apps --mode user "
         f"{PATH}/k6gte-winkeyerserial-32.png k6gte-winkeyerserial"
     )
     os.system(
```

### Comparing `winkeyerserial-23.2.17/winkeyerserial/k6gte-winkeyerserial-128.png` & `winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial-128.png`

 * *Files identical despite different names*

### Comparing `winkeyerserial-23.2.17/winkeyerserial/k6gte-winkeyerserial-32.png` & `winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial-32.png`

 * *Files identical despite different names*

### Comparing `winkeyerserial-23.2.17/winkeyerserial/k6gte-winkeyerserial-64.png` & `winkeyerserial-23.5.11/winkeyerserial/k6gte-winkeyerserial-64.png`

 * *Files identical despite different names*

### Comparing `winkeyerserial-23.2.17/winkeyerserial/main.ui` & `winkeyerserial-23.5.11/winkeyerserial/main.ui`

 * *Files identical despite different names*

### Comparing `winkeyerserial-23.2.17/winkeyerserial.egg-info/PKG-INFO` & `winkeyerserial-23.5.11/winkeyerserial.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winkeyerserial
-Version: 23.2.17
+Version: 23.5.11
 Summary: Talk to K1EL winkeyer
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/PyWinKeyerSerial
 Project-URL: Bug Tracker, https://github.com/mbridak/PyWinKeyerSerial/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -50,11 +50,12 @@
 
 # remove
 pip uninstall winkeyerserial
 ```
 
 ## What's new
 
+- [23-5-11] Added xmlrpc function to set speed.
 - [23-2-17] Added serial device descriptions (hover tooltip) to the detected serial devices in the dropdown.
 - Added an XMLRPC server. So now my [Winter Field Day](https://github.com/mbridak/WinterFieldDayLogger), [Field Day](https://github.com/mbridak/FieldDayLogger) and [K1USNSST](https://github.com/mbridak/k1usnsst) Loggers will be able to send CW macros to this. The interface for the client is dead simple:
  `xmlrpc.client.ServerProxy("http://localhost:8000").k1elsendstring("Hello World")`
  That's it...
```

### Comparing `winkeyerserial-23.2.17/winkeyerserial.egg-info/SOURCES.txt` & `winkeyerserial-23.5.11/winkeyerserial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

