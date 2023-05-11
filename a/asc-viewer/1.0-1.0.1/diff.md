# Comparing `tmp/asc_viewer-1.0.tar.gz` & `tmp/asc_viewer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asc_viewer-1.0.tar", last modified: Fri Dec 23 07:25:17 2022, max compression
+gzip compressed data, was "asc_viewer-1.0.1.tar", last modified: Fri Dec 23 19:22:49 2022, max compression
```

## Comparing `asc_viewer-1.0.tar` & `asc_viewer-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-23 07:25:17.834395 asc_viewer-1.0/
--rw-r--r--   0 user      (1000) user      (1000)     1059 2022-12-23 07:14:02.000000 asc_viewer-1.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     1517 2022-12-23 07:25:17.834395 asc_viewer-1.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1220 2022-12-23 07:15:40.000000 asc_viewer-1.0/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-23 07:25:17.834395 asc_viewer-1.0/asc_viewer/
--rw-r--r--   0 user      (1000) user      (1000)      250 2022-12-23 06:34:36.000000 asc_viewer-1.0/asc_viewer/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    19486 2022-12-23 06:47:49.000000 asc_viewer-1.0/asc_viewer/asc_canvas.py
--rw-r--r--   0 user      (1000) user      (1000)     1126 2022-12-23 06:48:32.000000 asc_viewer-1.0/asc_viewer/bounded_canvas.py
--rw-r--r--   0 user      (1000) user      (1000)     9334 2022-12-23 06:52:02.000000 asc_viewer-1.0/asc_viewer/symbol.py
--rw-r--r--   0 user      (1000) user      (1000)     3154 2022-12-23 06:48:32.000000 asc_viewer-1.0/asc_viewer/symbol_instance.py
--rwxr-xr-x   0 user      (1000) user      (1000)     4141 2022-12-23 06:48:32.000000 asc_viewer-1.0/asc_viewer/viewport.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-23 07:25:17.834395 asc_viewer-1.0/asc_viewer.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1517 2022-12-23 07:25:17.000000 asc_viewer-1.0/asc_viewer.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      361 2022-12-23 07:25:17.000000 asc_viewer-1.0/asc_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-12-23 07:25:17.000000 asc_viewer-1.0/asc_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       32 2022-12-23 07:25:17.000000 asc_viewer-1.0/asc_viewer.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       11 2022-12-23 07:25:17.000000 asc_viewer-1.0/asc_viewer.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-23 07:25:17.834395 asc_viewer-1.0/bin/
--rw-r--r--   0 user      (1000) user      (1000)     1432 2022-12-23 07:23:48.000000 asc_viewer-1.0/bin/asc_viewer
--rw-r--r--   0 user      (1000) user      (1000)       38 2022-12-23 07:25:17.834395 asc_viewer-1.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      706 2022-12-23 07:20:53.000000 asc_viewer-1.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-23 19:22:49.477247 asc_viewer-1.0.1/
+-rw-r--r--   0 user      (1000) user      (1000)     1059 2022-12-23 07:14:02.000000 asc_viewer-1.0.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     1691 2022-12-23 19:22:49.477247 asc_viewer-1.0.1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1392 2022-12-23 19:21:49.000000 asc_viewer-1.0.1/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-23 19:22:49.477247 asc_viewer-1.0.1/asc_viewer/
+-rw-r--r--   0 user      (1000) user      (1000)      250 2022-12-23 06:34:36.000000 asc_viewer-1.0.1/asc_viewer/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    19610 2022-12-23 19:10:26.000000 asc_viewer-1.0.1/asc_viewer/asc_canvas.py
+-rw-r--r--   0 user      (1000) user      (1000)     1126 2022-12-23 06:48:32.000000 asc_viewer-1.0.1/asc_viewer/bounded_canvas.py
+-rw-r--r--   0 user      (1000) user      (1000)     9334 2022-12-23 06:52:02.000000 asc_viewer-1.0.1/asc_viewer/symbol.py
+-rw-r--r--   0 user      (1000) user      (1000)     3154 2022-12-23 06:48:32.000000 asc_viewer-1.0.1/asc_viewer/symbol_instance.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     4141 2022-12-23 06:48:32.000000 asc_viewer-1.0.1/asc_viewer/viewport.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-23 19:22:49.477247 asc_viewer-1.0.1/asc_viewer.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1691 2022-12-23 19:22:49.000000 asc_viewer-1.0.1/asc_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      361 2022-12-23 19:22:49.000000 asc_viewer-1.0.1/asc_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2022-12-23 19:22:49.000000 asc_viewer-1.0.1/asc_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       32 2022-12-23 19:22:49.000000 asc_viewer-1.0.1/asc_viewer.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       11 2022-12-23 19:22:49.000000 asc_viewer-1.0.1/asc_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-23 19:22:49.477247 asc_viewer-1.0.1/bin/
+-rw-r--r--   0 user      (1000) user      (1000)     2063 2022-12-23 19:20:51.000000 asc_viewer-1.0.1/bin/asc_viewer
+-rw-r--r--   0 user      (1000) user      (1000)       38 2022-12-23 19:22:49.477247 asc_viewer-1.0.1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      708 2022-12-23 18:53:09.000000 asc_viewer-1.0.1/setup.py
```

### Comparing `asc_viewer-1.0/LICENSE` & `asc_viewer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asc_viewer-1.0/PKG-INFO` & `asc_viewer-1.0.1/asc_viewer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
-Name: asc_viewer
-Version: 1.0
+Name: asc-viewer
+Version: 1.0.1
 Summary: A viewer for LTspice ASC schematics implemented in wxPython
 Home-page: http://github.com/ahaensler/asc_viewer
 Author: Adrian Haensler
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # LTspice ASC Viewer
 
-[LTspice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) is one of the best schematic entry tools out there.
+[LTspice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) is one of the best schematic entry tools out there. It lets you draw any schematic imaginable. LTspice's simple appearance belies its true power.
 
-It lets you draw any schematic imaginable. LTspice's simplpe appearance belies its true power.
+- You can draw graphs for computer science.
 
-You can draw graphs for computer science.
+- You can define buses.
 
-You can define buses.
-
-You can nest schematics for complex hierarchies.
+- You can nest schematics for complex hierarchies.
 
 **Now if only we could use these schematics in a Python GUI.**
 
+![alt text](https://github.com/ahaensler/asc_viewer/blob/main/screenshot.png "Screenshot")
+
 ## AscCanvas
-AscCanvas lets you import a schematic and show it as a wxPython window. It supports zooming, scrolling, searching and subclassing. It uses [rtreelib](https://github.com/lukas-shawford/rtreelib) to look up symbols and nets under the mouse pointer.
+The AscCanvas class lets you import a schematic and show it as a wxPython window. It supports zooming, scrolling, searching and subclassing. It uses [rtreelib](https://github.com/lukas-shawford/rtreelib) to look up symbols and nets under the mouse pointer.
 
 To show a schematic, you will need to import these files:
 
 - ASY files are symbols, i.e., components, and they are imported in batch by specifying a list of paths. Load them by calling `AscCanvas.load_symbols()`
 
 - ASC files are schematics. They define the connectivity between instances of symbols. Load them by calling `AscCanvas.load_asc()`.
 
 ## asc\_viewer
-`asc_viewer` is a demo executable that lets you opens schematic and shows how to use `AscCanvas`.
+[asc_viewer](https://github.com/ahaensler/asc_viewer/blob/main/bin/asc_viewer) is a demo executable that lets you open schematics and shows how to use `AscCanvas`.
 
 ## Installation
 ```pip install asc_viewer```
```

### Comparing `asc_viewer-1.0/README.md` & `asc_viewer-1.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # LTspice ASC Viewer
 
-[LTspice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) is one of the best schematic entry tools out there.
+[LTspice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) is one of the best schematic entry tools out there. It lets you draw any schematic imaginable. LTspice's simple appearance belies its true power.
 
-It lets you draw any schematic imaginable. LTspice's simplpe appearance belies its true power.
+- You can draw graphs for computer science.
 
-You can draw graphs for computer science.
+- You can define buses.
 
-You can define buses.
-
-You can nest schematics for complex hierarchies.
+- You can nest schematics for complex hierarchies.
 
 **Now if only we could use these schematics in a Python GUI.**
 
+![alt text](https://github.com/ahaensler/asc_viewer/blob/main/screenshot.png "Screenshot")
+
 ## AscCanvas
-AscCanvas lets you import a schematic and show it as a wxPython window. It supports zooming, scrolling, searching and subclassing. It uses [rtreelib](https://github.com/lukas-shawford/rtreelib) to look up symbols and nets under the mouse pointer.
+The AscCanvas class lets you import a schematic and show it as a wxPython window. It supports zooming, scrolling, searching and subclassing. It uses [rtreelib](https://github.com/lukas-shawford/rtreelib) to look up symbols and nets under the mouse pointer.
 
 To show a schematic, you will need to import these files:
 
 - ASY files are symbols, i.e., components, and they are imported in batch by specifying a list of paths. Load them by calling `AscCanvas.load_symbols()`
 
 - ASC files are schematics. They define the connectivity between instances of symbols. Load them by calling `AscCanvas.load_asc()`.
 
 ## asc\_viewer
-`asc_viewer` is a demo executable that lets you opens schematic and shows how to use `AscCanvas`.
+[asc_viewer](https://github.com/ahaensler/asc_viewer/blob/main/bin/asc_viewer) is a demo executable that lets you open schematics and shows how to use `AscCanvas`.
 
 ## Installation
 ```pip install asc_viewer```
```

### Comparing `asc_viewer-1.0/asc_viewer/asc_canvas.py` & `asc_viewer-1.0.1/asc_viewer/asc_canvas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import wx
 import math
-from asc_viewer.viewport import Viewport
-from asc_viewer.symbol_instance import SymbolInstance
 import glob, os
 import rtreelib as rt
-from asc_viewer.symbol import Symbol, window_types
 from asc_viewer.bounded_canvas import BoundedCanvas
+from asc_viewer.symbol import Symbol, window_types
+from asc_viewer.symbol_instance import SymbolInstance
+from asc_viewer.viewport import Viewport
 
+# font sizes available in LTspice
 font_size_factors = [0.625, 1, 1.5, 2, 2.5, 3.5, 5, 7]
 
 
 class Net:
     """A net as used in LtSpice."""
 
     def __init__(self, name):
@@ -58,15 +59,15 @@
 
     Arguments:
     parent -- the parent window
     symbol_paths -- a list of path names where symbols are stored
     instance_name -- the instance name of this schematic, this is only useful it the schematic is an instantiated subcircuit
     """
 
-    def __init__(self, parent, symbol_paths, instance_name=""):
+    def __init__(self, parent, symbol_paths=[], instance_name=""):
         super().__init__(parent)
 
         self.instance_name = instance_name
         self.symbols = {}
         self.filename = None
         self.load_symbols(symbol_paths)
 
@@ -81,31 +82,34 @@
             self.fonts.append(font)
         font_size = 0.8
         self.black_font = self.create_font(font_size, wx.BLACK)
         self.blue_font = self.create_font(font_size, wx.BLUE)
         self.red_font = self.create_font(font_size, wx.RED)
         self.gray_font = self.create_font(font_size, wx.Colour(50, 50, 50, 50))
 
+        self.reset()
+
+        self.find_data = wx.FindReplaceData()
+        self.find_dialog = None  # cannot be initialized here yet
+
+        self.Bind(wx.EVT_CHAR_HOOK, self.on_key)
+        self.Bind(wx.EVT_PAINT, self.on_paint)
+
+    def reset(self):
         self.wires = []
         self.wire_points = {}
         self.net_counter = 0  # for auto-labeling nets
         self.flags = {}  # off-schematic connectors or io pins
         self.texts = []
         self.rtree = rt.RTree()
         self.wire_lookup = rt.RTree()
         self.nets = {}  # name to net
         self.path = self.gc.CreatePath()
         self.symbol_instances = {}
 
-        self.find_data = wx.FindReplaceData()
-        self.find_dialog = None  # cannot be initialized here yet
-
-        self.Bind(wx.EVT_CHAR_HOOK, self.on_key)
-        self.Bind(wx.EVT_PAINT, self.on_paint)
-
     def load_symbols(self, symbol_paths):
         """Loads symbols from a list of paths to asy files."""
         if isinstance(symbol_paths, str):
             symbol_paths = [symbol_paths]
         for path in symbol_paths:
             path = os.path.join(path, "*.asy")
             filenames = glob.glob(path)
@@ -189,16 +193,17 @@
                     neighbor.net = wire_point.net
                     stack.append(neighbor)
 
     def load_asc(self, filename):
         """Loads an LtSpice schematic from the given filename."""
         instances = []
         self.filename = filename
-        f = open(filename, encoding="iso-8859-1")
+        self.reset()
         self.reset_extent()
+        f = open(filename, encoding="iso-8859-1")
         sheet_w, sheet_h = 0, 0
         for line in f:
             line = line.strip()
             if len(line) == 0:
                 continue
             words = line.split(" ")
             if words[0] == "WIRE":
@@ -291,15 +296,14 @@
                     y=y,
                     align=words[4],
                     size=int(words[5]),
                 )
                 instances[-1].windows[window["type"]] = window
 
         # load symbol instances
-        self.symbol_instances = {}
         pin_positions = {}
         for instance in instances:
             s = self.symbols.get(instance.name)
             if s is None:
                 print(f"Symbol not found {instance.name}")
                 self.rtree.insert(
                     instance,
@@ -430,14 +434,17 @@
         try:
             return next(res).data
         except StopIteration:
             return None
 
     def get_net_under_mouse(self, evt):
         """Returns the net under the mouse pointer."""
+        if len(self.wires) == 0:
+            return None
+
         pos = self.mouse_position(evt)
         rect = (pos[0] - 5, pos[1] - 5, pos[0] + 5, pos[1] + 5)
         res = self.wire_lookup.query(rect)
 
         def distance_to_line(x0, y0, x1, y1, x2, y2):
             return (
                 abs((x2 - x1) * (y1 - y0) - (x1 - x0) * (y2 - y1))
```

### Comparing `asc_viewer-1.0/asc_viewer/bounded_canvas.py` & `asc_viewer-1.0.1/asc_viewer/bounded_canvas.py`

 * *Files identical despite different names*

### Comparing `asc_viewer-1.0/asc_viewer/symbol.py` & `asc_viewer-1.0.1/asc_viewer/symbol.py`

 * *Files identical despite different names*

### Comparing `asc_viewer-1.0/asc_viewer/symbol_instance.py` & `asc_viewer-1.0.1/asc_viewer/symbol_instance.py`

 * *Files identical despite different names*

### Comparing `asc_viewer-1.0/asc_viewer/viewport.py` & `asc_viewer-1.0.1/asc_viewer/viewport.py`

 * *Files identical despite different names*

### Comparing `asc_viewer-1.0/asc_viewer.egg-info/PKG-INFO` & `asc_viewer-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
-Name: asc-viewer
-Version: 1.0
+Name: asc_viewer
+Version: 1.0.1
 Summary: A viewer for LTspice ASC schematics implemented in wxPython
 Home-page: http://github.com/ahaensler/asc_viewer
 Author: Adrian Haensler
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # LTspice ASC Viewer
 
-[LTspice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) is one of the best schematic entry tools out there.
+[LTspice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) is one of the best schematic entry tools out there. It lets you draw any schematic imaginable. LTspice's simple appearance belies its true power.
 
-It lets you draw any schematic imaginable. LTspice's simplpe appearance belies its true power.
+- You can draw graphs for computer science.
 
-You can draw graphs for computer science.
+- You can define buses.
 
-You can define buses.
-
-You can nest schematics for complex hierarchies.
+- You can nest schematics for complex hierarchies.
 
 **Now if only we could use these schematics in a Python GUI.**
 
+![alt text](https://github.com/ahaensler/asc_viewer/blob/main/screenshot.png "Screenshot")
+
 ## AscCanvas
-AscCanvas lets you import a schematic and show it as a wxPython window. It supports zooming, scrolling, searching and subclassing. It uses [rtreelib](https://github.com/lukas-shawford/rtreelib) to look up symbols and nets under the mouse pointer.
+The AscCanvas class lets you import a schematic and show it as a wxPython window. It supports zooming, scrolling, searching and subclassing. It uses [rtreelib](https://github.com/lukas-shawford/rtreelib) to look up symbols and nets under the mouse pointer.
 
 To show a schematic, you will need to import these files:
 
 - ASY files are symbols, i.e., components, and they are imported in batch by specifying a list of paths. Load them by calling `AscCanvas.load_symbols()`
 
 - ASC files are schematics. They define the connectivity between instances of symbols. Load them by calling `AscCanvas.load_asc()`.
 
 ## asc\_viewer
-`asc_viewer` is a demo executable that lets you opens schematic and shows how to use `AscCanvas`.
+[asc_viewer](https://github.com/ahaensler/asc_viewer/blob/main/bin/asc_viewer) is a demo executable that lets you open schematics and shows how to use `AscCanvas`.
 
 ## Installation
 ```pip install asc_viewer```
```

### Comparing `asc_viewer-1.0/bin/asc_viewer` & `asc_viewer-1.0.1/bin/asc_viewer`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 #!/bin/python
-import wx
+""" A minimal demo of the asc_viewer package. There is a menu bar for loading schematics,
+and a status bar for showing net names.
+
+Having the user load symbol paths each time is obviously bad design, and in a real project
+you would pass symbol paths to AscCanvas's constructor.
+"""
 
+import wx
 from asc_viewer import AscCanvas
 
 
 class AscViewer(wx.Frame):
-    def __init__(self, *args, **kwds):
+    def __init__(self):
         super().__init__(None, title="LTspice ASC Viewer", size=(400, 300))
 
         # Menu Bar
         self.menu = wx.MenuBar()
-
         menu = wx.Menu()
         entry = menu.Append(wx.ID_ANY, "Open ASY directory...", "Open ASY directory")
-        self.Bind(wx.EVT_MENU, self.set_asy, entry)
+        self.Bind(wx.EVT_MENU, self.open_asy, entry)
         entry = menu.Append(wx.ID_ANY, "Open ASC...", "Open ASC file")
         self.Bind(wx.EVT_MENU, self.open_asc, entry)
         self.menu.Append(menu, "&File")
-
         self.SetMenuBar(self.menu)
 
-        self.asc_canvas = AscCanvas(self, [])
-        self.Layout()
+        # Status Bar
+        self.statusbar = self.CreateStatusBar(1, wx.STB_DEFAULT_STYLE)
 
-        self.asy_directory = None
+        # Canvas for ASC Schematics
+        self.asc_canvas = AscCanvas(self)
+        self.asc_canvas.Bind(wx.EVT_MOTION, self.on_motion)
+        self.Layout()
 
-    def set_asy(self, event):
-        path = wx.DirSelector("Choose a folder")
+    def open_asy(self, event):
+        path = wx.DirSelector("Choose a symbol folder")
         if not path.strip():
             return
         self.asc_canvas.load_symbols([path])
 
     def open_asc(self, event):
         d = wx.FileDialog(
             None, "Select schematic", wildcard="Schematic files (.asc)|*.asc"
@@ -43,12 +50,18 @@
             wx.MessageDialog(
                 None, "Invalid schematic", "Error", wx.OK | wx.ICON_QUESTION
             ).ShowModal()
             return
 
         self.asc_canvas.load_asc(filename)
 
+    def on_motion(self, event):
+        net = self.asc_canvas.get_net_under_mouse(event)
+        status_text = net.name if net else ""
+        self.statusbar.SetStatusText(status_text)
+        event.Skip()
+
 
 app = wx.App()
 frame = AscViewer()
 frame.Show()
 app.MainLoop()
```

### Comparing `asc_viewer-1.0/setup.py` & `asc_viewer-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
 setup(
     name="asc_viewer",
-    version="1.0",
+    version="1.0.1",
     description="A viewer for LTspice ASC schematics implemented in wxPython",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='http://github.com/ahaensler/asc_viewer',
     scripts=["bin/asc_viewer"],
     packages=["asc_viewer"],
     author="Adrian Haensler",
```

