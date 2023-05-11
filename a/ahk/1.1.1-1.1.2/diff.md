# Comparing `tmp/ahk-1.1.1.tar.gz` & `tmp/ahk-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.1.1.tar", last modified: Thu May  4 03:22:38 2023, max compression
+gzip compressed data, was "ahk-1.1.2.tar", last modified: Thu May 11 02:02:00 2023, max compression
```

## Comparing `ahk-1.1.1.tar` & `ahk-1.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:22:38.416175 ahk-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-04 03:22:23.000000 ahk-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-05-04 03:22:38.416175 ahk-1.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:22:38.412175 ahk-1.1.1/ahk/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:22:38.412175 ahk-1.1.1/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179907 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    43081 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (123)    83313 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:22:38.416175 ahk-1.1.1/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   174154 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    26344 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:22:38.416175 ahk-1.1.1/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78662 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-04 03:22:23.000000 ahk-1.1.1/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:22:38.412175 ahk-1.1.1/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-05-04 03:22:38.000000 ahk-1.1.1/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-04 03:22:38.000000 ahk-1.1.1/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:22:38.000000 ahk-1.1.1/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 03:22:38.000000 ahk-1.1.1/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-04 03:22:38.000000 ahk-1.1.1/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-04 03:22:23.000000 ahk-1.1.1/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:22:38.416175 ahk-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    17928 2023-05-04 03:22:23.000000 ahk-1.1.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-04 03:22:23.000000 ahk-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 03:22:38.416175 ahk-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 03:22:23.000000 ahk-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:02:00.959716 ahk-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-11 02:01:45.000000 ahk-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-05-11 02:02:00.959716 ahk-1.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:02:00.955716 ahk-1.1.2/ahk/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:02:00.955716 ahk-1.1.2/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179999 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43081 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83686 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:02:00.959716 ahk-1.1.2/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174245 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26344 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:02:00.959716 ahk-1.1.2/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    79035 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-11 02:01:45.000000 ahk-1.1.2/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:02:00.955716 ahk-1.1.2/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-05-11 02:02:00.000000 ahk-1.1.2/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-11 02:02:00.000000 ahk-1.1.2/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 02:02:00.000000 ahk-1.1.2/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-11 02:02:00.000000 ahk-1.1.2/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-11 02:02:00.000000 ahk-1.1.2/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-11 02:01:45.000000 ahk-1.1.2/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:02:00.959716 ahk-1.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17928 2023-05-11 02:01:45.000000 ahk-1.1.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-11 02:01:45.000000 ahk-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-11 02:02:00.959716 ahk-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 02:01:45.000000 ahk-1.1.2/setup.py
```

### Comparing `ahk-1.1.1/PKG-INFO` & `ahk-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
```

### Comparing `ahk-1.1.1/ahk/__init__.py` & `ahk-1.1.2/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/ahk/_async/engine.py` & `ahk-1.1.2/ahk/_async/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -2694,17 +2694,21 @@
             x2, y2 = lower_bound
         else:
             x2, y2 = ('A_ScreenWidth', 'A_ScreenHeight')
 
         args = [str(x1), str(y1), str(x2), str(y2)]
         if options:
             opts = ' '.join(f'*{opt}' for opt in options)
-            args.append(opts)
+            args.append(opts + f' {image_path}')
         else:
             args.append(image_path)
+
+        if coord_mode is not None:
+            args.append(coord_mode)
+
         resp = await self._transport.function_call('AHKImageSearch', args, blocking=blocking)
         return resp
 
     async def mouse_drag(
         self,
         x: int,
         y: int,
```

### Comparing `ahk-1.1.1/ahk/_async/transport.py` & `ahk-1.1.2/ahk/_async/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/ahk/_async/window.py` & `ahk-1.1.2/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/ahk/_constants.py` & `ahk-1.1.2/ahk/_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,19 +157,21 @@
     }
     current_detect_hw := Format("{}", A_DetectHiddenWindows)
 
     if (detect_hw != "") {
         DetectHiddenWindows, %detect_hw%
     }
 
+
+    WinClose, %title%, %text%, %secondstowait%, %extitle%, %extext%
+
     DetectHiddenWindows, %current_detect_hw%
     SetTitleMatchMode, %current_match_mode%
     SetTitleMatchMode, %current_match_speed%
 
-    WinClose, %title%, %text%, %secondstowait%, %extitle%, %extext%
 
     return FormatNoValueResponse()
     {% endblock AHKWinClose %}
 }
 
 AHKWinKill(ByRef command) {
     {% block AHKWinKill %}
@@ -1573,35 +1575,55 @@
 
     if (detect_hw != "") {
         DetectHiddenWindows, %detect_hw%
     }
 
 
     WinSet, TransColor, %color%, %title%, %text%, %extitle%, %extext%
+
+    DetectHiddenWindows, %current_detect_hw%
+    SetTitleMatchMode, %current_match_mode%
+    SetTitleMatchMode, %current_match_speed%
+
     return FormatNoValueResponse()
     {% endblock AHKWinSetTransColor %}
 }
 
 AHKImageSearch(ByRef command) {
     {% block AHKImageSearch %}
     global COORDINATERESPONSEMESSAGE
     global EXCEPTIONRESPONSEMESSAGE
     imagepath := command[6]
     x1 := command[2]
     y1 := command[3]
     x2 := command[4]
     y2 := command[5]
+    coord_mode := command[7]
+
+    current_mode := Format("{}", A_CoordModePixel)
+
+    if (coord_mode != "") {
+        CoordMode, Pixel, %coord_mode%
+    }
 
     if (x2 = "A_ScreenWidth") {
         x2 := A_ScreenWidth
     }
     if (y2 = "A_ScreenHeight") {
         y2 := A_ScreenHeight
     }
+
     ImageSearch, xpos, ypos,% x1,% y1,% x2,% y2, %imagepath%
+
+
+    if (coord_mode != "") {
+        CoordMode, Pixel, %current_mode%
+    }
+
+
     if (ErrorLevel = 2) {
         s := FormatResponse(EXCEPTIONRESPONSEMESSAGE, "there was a problem that prevented the command from conducting the search (such as failure to open the image file or a badly formatted option)")
     } else if (ErrorLevel = 1) {
         s := FormatNoValueResponse()
     } else {
         s := FormatResponse(COORDINATERESPONSEMESSAGE, Format("({}, {})", xpos, ypos))
     }
```

### Comparing `ahk-1.1.1/ahk/_hotkey.py` & `ahk-1.1.2/ahk/_hotkey.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/ahk/_sync/engine.py` & `ahk-1.1.2/ahk/_sync/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -2683,17 +2683,20 @@
             x2, y2 = lower_bound
         else:
             x2, y2 = ('A_ScreenWidth', 'A_ScreenHeight')
 
         args = [str(x1), str(y1), str(x2), str(y2)]
         if options:
             opts = ' '.join(f'*{opt}' for opt in options)
-            args.append(opts)
+            args.append(opts + f' {image_path}')
         else:
             args.append(image_path)
+
+        if coord_mode is not None:
+            args.append(coord_mode)
         resp = self._transport.function_call('AHKImageSearch', args, blocking=blocking)
         return resp
 
     def mouse_drag(
         self,
         x: int,
         y: int,
```

### Comparing `ahk-1.1.1/ahk/_sync/transport.py` & `ahk-1.1.2/ahk/_sync/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/ahk/_sync/window.py` & `ahk-1.1.2/ahk/_sync/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/ahk/_utils.py` & `ahk-1.1.2/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/ahk/directives.py` & `ahk-1.1.2/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/ahk/keys.py` & `ahk-1.1.2/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/ahk/message.py` & `ahk-1.1.2/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/ahk/templates/daemon.ahk` & `ahk-1.1.2/ahk/templates/daemon.ahk`

 * *Files 0% similar despite different names*

```diff
@@ -154,19 +154,21 @@
     }
     current_detect_hw := Format("{}", A_DetectHiddenWindows)
 
     if (detect_hw != "") {
         DetectHiddenWindows, %detect_hw%
     }
 
+
+    WinClose, %title%, %text%, %secondstowait%, %extitle%, %extext%
+
     DetectHiddenWindows, %current_detect_hw%
     SetTitleMatchMode, %current_match_mode%
     SetTitleMatchMode, %current_match_speed%
 
-    WinClose, %title%, %text%, %secondstowait%, %extitle%, %extext%
 
     return FormatNoValueResponse()
     {% endblock AHKWinClose %}
 }
 
 AHKWinKill(ByRef command) {
     {% block AHKWinKill %}
@@ -1570,35 +1572,55 @@
 
     if (detect_hw != "") {
         DetectHiddenWindows, %detect_hw%
     }
 
 
     WinSet, TransColor, %color%, %title%, %text%, %extitle%, %extext%
+
+    DetectHiddenWindows, %current_detect_hw%
+    SetTitleMatchMode, %current_match_mode%
+    SetTitleMatchMode, %current_match_speed%
+
     return FormatNoValueResponse()
     {% endblock AHKWinSetTransColor %}
 }
 
 AHKImageSearch(ByRef command) {
     {% block AHKImageSearch %}
     global COORDINATERESPONSEMESSAGE
     global EXCEPTIONRESPONSEMESSAGE
     imagepath := command[6]
     x1 := command[2]
     y1 := command[3]
     x2 := command[4]
     y2 := command[5]
+    coord_mode := command[7]
+
+    current_mode := Format("{}", A_CoordModePixel)
+
+    if (coord_mode != "") {
+        CoordMode, Pixel, %coord_mode%
+    }
 
     if (x2 = "A_ScreenWidth") {
         x2 := A_ScreenWidth
     }
     if (y2 = "A_ScreenHeight") {
         y2 := A_ScreenHeight
     }
+
     ImageSearch, xpos, ypos,% x1,% y1,% x2,% y2, %imagepath%
+
+
+    if (coord_mode != "") {
+        CoordMode, Pixel, %current_mode%
+    }
+
+
     if (ErrorLevel = 2) {
         s := FormatResponse(EXCEPTIONRESPONSEMESSAGE, "there was a problem that prevented the command from conducting the search (such as failure to open the image file or a badly formatted option)")
     } else if (ErrorLevel = 1) {
         s := FormatNoValueResponse()
     } else {
         s := FormatResponse(COORDINATERESPONSEMESSAGE, Format("({}, {})", xpos, ypos))
     }
```

### Comparing `ahk-1.1.1/ahk/templates/hotkeys.ahk` & `ahk-1.1.2/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/ahk.egg-info/PKG-INFO` & `ahk-1.1.2/ahk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
```

### Comparing `ahk-1.1.1/ahk.egg-info/SOURCES.txt` & `ahk-1.1.2/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/buildunasync.py` & `ahk-1.1.2/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/docs/README.md` & `ahk-1.1.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `ahk-1.1.1/setup.cfg` & `ahk-1.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.1.1
+version = 1.1.2
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 keywords =
```

