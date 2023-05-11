# Comparing `tmp/sbcoyote-1.4.2.tar.gz` & `tmp/sbcoyote-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbcoyote-1.4.2.tar", max compression
+gzip compressed data, was "sbcoyote-1.4.3.tar", max compression
```

## Comparing `sbcoyote-1.4.2.tar` & `sbcoyote-1.4.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1090 2023-01-10 20:04:27.423064 sbcoyote-1.4.2/LICENSE
--rw-r--r--   0        0        0     1826 2023-05-02 21:40:04.275319 sbcoyote-1.4.2/pyproject.toml
--rw-r--r--   0        0        0    10368 2023-05-02 21:32:36.743811 sbcoyote-1.4.2/README.md
--rw-r--r--   0        0        0       23 2021-09-10 21:55:36.689271 sbcoyote-1.4.2/rkviewer/__init__.py
--rw-r--r--   0        0        0        0 2021-09-10 21:55:36.690269 sbcoyote-1.4.2/rkviewer/canvas/__init__.py
--rw-r--r--   0        0        0    91711 2023-04-05 20:30:56.859645 sbcoyote-1.4.2/rkviewer/canvas/canvas.py
--rw-r--r--   0        0        0    32394 2023-03-29 18:22:43.731567 sbcoyote-1.4.2/rkviewer/canvas/data.py
--rw-r--r--   0        0        0    59253 2023-02-16 03:57:51.512804 sbcoyote-1.4.2/rkviewer/canvas/elements.py
--rw-r--r--   0        0        0    17929 2023-02-16 03:57:51.514828 sbcoyote-1.4.2/rkviewer/canvas/geometry.py
--rw-r--r--   0        0        0     8408 2021-09-10 21:55:36.694258 sbcoyote-1.4.2/rkviewer/canvas/overlays.py
--rw-r--r--   0        0        0     1731 2021-09-10 21:55:36.695255 sbcoyote-1.4.2/rkviewer/canvas/state.py
--rw-r--r--   0        0        0     6751 2022-12-13 22:58:03.646205 sbcoyote-1.4.2/rkviewer/canvas/utils.py
--rw-r--r--   0        0        0    18996 2023-04-11 18:08:06.351143 sbcoyote-1.4.2/rkviewer/config.py
--rw-r--r--   0        0        0    23001 2023-03-29 18:22:41.234242 sbcoyote-1.4.2/rkviewer/controller.py
--rw-r--r--   0        0        0    13105 2021-09-10 21:55:36.697250 sbcoyote-1.4.2/rkviewer/events.py
--rw-r--r--   0        0        0    98431 2023-04-14 18:57:17.020026 sbcoyote-1.4.2/rkviewer/forms.py
--rw-r--r--   0        0        0    94813 2023-04-12 23:20:38.517372 sbcoyote-1.4.2/rkviewer/iodine.py
--rw-r--r--   0        0        0     3329 2023-04-14 20:43:22.448825 sbcoyote-1.4.2/rkviewer/json/.default-settings.json
--rw-r--r--   0        0        0     1817 2021-09-10 21:55:36.655349 sbcoyote-1.4.2/rkviewer/json/dark-settings.json
--rw-r--r--   0        0        0      727 2021-09-10 21:55:36.653177 sbcoyote-1.4.2/rkviewer/json/settings.json
--rw-r--r--   0        0        0     3399 2023-02-10 23:42:55.235161 sbcoyote-1.4.2/rkviewer/main.py
--rw-r--r--   0        0        0    12295 2021-09-10 21:55:36.701263 sbcoyote-1.4.2/rkviewer/mvc.py
--rw-r--r--   0        0        0        0 2021-09-10 21:55:36.701263 sbcoyote-1.4.2/rkviewer/plugin/__init__.py
--rw-r--r--   0        0        0    57933 2023-03-29 18:22:16.274177 sbcoyote-1.4.2/rkviewer/plugin/api.py
--rw-r--r--   0        0        0      513 2021-09-10 21:55:36.703235 sbcoyote-1.4.2/rkviewer/plugin/canvas.py
--rw-r--r--   0        0        0     9684 2023-03-27 18:05:44.898125 sbcoyote-1.4.2/rkviewer/plugin/classes.py
--rw-r--r--   0        0        0      154 2021-09-10 21:55:36.704231 sbcoyote-1.4.2/rkviewer/plugin/events.py
--rw-r--r--   0        0        0    18945 2023-01-26 22:34:13.868916 sbcoyote-1.4.2/rkviewer/plugin_manage.py
--rw-r--r--   0        0        0        0 2021-09-10 21:55:36.706226 sbcoyote-1.4.2/rkviewer/resources/__init__.py
--rw-r--r--   0        0        0      335 2021-09-10 21:55:36.705228 sbcoyote-1.4.2/rkviewer/resources/AlignBottom_XP.png
--rw-r--r--   0        0        0      312 2021-09-10 21:55:36.706226 sbcoyote-1.4.2/rkviewer/resources/alignHorizCenter_XP.png
--rw-r--r--   0        0        0      298 2021-09-10 21:55:36.707254 sbcoyote-1.4.2/rkviewer/resources/alignHorizEqually_XP.png
--rw-r--r--   0        0        0      379 2021-09-10 21:55:36.707254 sbcoyote-1.4.2/rkviewer/resources/alignLeft_XP.png
--rw-r--r--   0        0        0      238 2021-09-10 21:55:36.708254 sbcoyote-1.4.2/rkviewer/resources/alignOnGrid_XP.png
--rw-r--r--   0        0        0      602 2021-09-10 21:55:36.709251 sbcoyote-1.4.2/rkviewer/resources/alignRight_XP.png
--rw-r--r--   0        0        0      366 2021-09-10 21:55:36.709251 sbcoyote-1.4.2/rkviewer/resources/alignTop_XP.png
--rw-r--r--   0        0        0      280 2021-09-10 21:55:36.709251 sbcoyote-1.4.2/rkviewer/resources/alignVertCenter_XP.png
--rw-r--r--   0        0        0      308 2021-09-10 21:55:36.710248 sbcoyote-1.4.2/rkviewer/resources/alignVertEqually_XP.png
--rw-r--r--   0        0        0      389 2021-09-10 21:55:36.710248 sbcoyote-1.4.2/rkviewer/resources/info-2-16.png
--rw-r--r--   0        0        0     8227 2023-01-23 21:52:33.720240 sbcoyote-1.4.2/rkviewer/utils.py
--rw-r--r--   0        0        0    47660 2023-05-02 21:40:08.024102 sbcoyote-1.4.2/rkviewer/view.py
--rw-r--r--   0        0        0     8420 2023-04-10 20:09:02.114349 sbcoyote-1.4.2/rkviewer_plugins/addReaction.py
--rw-r--r--   0        0        0     7700 2023-03-27 21:04:32.885475 sbcoyote-1.4.2/rkviewer_plugins/align_circle.py
--rw-r--r--   0        0        0    10023 2023-01-24 01:05:59.812128 sbcoyote-1.4.2/rkviewer_plugins/arrow_designer.py
--rw-r--r--   0        0        0     7910 2023-03-27 23:00:15.322399 sbcoyote-1.4.2/rkviewer_plugins/exportAntimony.py
--rw-r--r--   0        0        0    70514 2023-05-02 17:16:00.570787 sbcoyote-1.4.2/rkviewer_plugins/exportSBML.py
--rw-r--r--   0        0        0   156402 2023-05-02 21:09:10.632510 sbcoyote-1.4.2/rkviewer_plugins/importSBML.py
--rw-r--r--   0        0        0     1152 2023-04-05 18:58:00.989843 sbcoyote-1.4.2/rkviewer_plugins/modelMetrics.py
--rw-r--r--   0        0        0    16762 2023-03-27 21:03:50.201865 sbcoyote-1.4.2/rkviewer_plugins/networkX.py
--rw-r--r--   0        0        0    17554 2023-03-27 21:03:22.666400 sbcoyote-1.4.2/rkviewer_plugins/randomNetwork.py
--rw-r--r--   0        0        0    12839 2023-03-27 21:03:31.309823 sbcoyote-1.4.2/rkviewer_plugins/structuralAnalysis.py
--rw-r--r--   0        0        0    11909 1970-01-01 00:00:00.000000 sbcoyote-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-01-10 20:04:27.423064 sbcoyote-1.4.3/LICENSE
+-rw-r--r--   0        0        0     1826 2023-05-09 22:38:30.357468 sbcoyote-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0    10368 2023-05-02 21:32:36.743811 sbcoyote-1.4.3/README.md
+-rw-r--r--   0        0        0       23 2021-09-10 21:55:36.689271 sbcoyote-1.4.3/rkviewer/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-10 21:55:36.690269 sbcoyote-1.4.3/rkviewer/canvas/__init__.py
+-rw-r--r--   0        0        0    91711 2023-04-05 20:30:56.859645 sbcoyote-1.4.3/rkviewer/canvas/canvas.py
+-rw-r--r--   0        0        0    32394 2023-03-29 18:22:43.731567 sbcoyote-1.4.3/rkviewer/canvas/data.py
+-rw-r--r--   0        0        0    59253 2023-02-16 03:57:51.512804 sbcoyote-1.4.3/rkviewer/canvas/elements.py
+-rw-r--r--   0        0        0    17929 2023-02-16 03:57:51.514828 sbcoyote-1.4.3/rkviewer/canvas/geometry.py
+-rw-r--r--   0        0        0     8408 2021-09-10 21:55:36.694258 sbcoyote-1.4.3/rkviewer/canvas/overlays.py
+-rw-r--r--   0        0        0     1731 2021-09-10 21:55:36.695255 sbcoyote-1.4.3/rkviewer/canvas/state.py
+-rw-r--r--   0        0        0     6751 2022-12-13 22:58:03.646205 sbcoyote-1.4.3/rkviewer/canvas/utils.py
+-rw-r--r--   0        0        0    18996 2023-04-11 18:08:06.351143 sbcoyote-1.4.3/rkviewer/config.py
+-rw-r--r--   0        0        0    23001 2023-03-29 18:22:41.234242 sbcoyote-1.4.3/rkviewer/controller.py
+-rw-r--r--   0        0        0    13105 2021-09-10 21:55:36.697250 sbcoyote-1.4.3/rkviewer/events.py
+-rw-r--r--   0        0        0    98452 2023-05-09 19:17:43.589453 sbcoyote-1.4.3/rkviewer/forms.py
+-rw-r--r--   0        0        0    94813 2023-04-12 23:20:38.517372 sbcoyote-1.4.3/rkviewer/iodine.py
+-rw-r--r--   0        0        0     3329 2023-04-14 20:43:22.448825 sbcoyote-1.4.3/rkviewer/json/.default-settings.json
+-rw-r--r--   0        0        0     1817 2021-09-10 21:55:36.655349 sbcoyote-1.4.3/rkviewer/json/dark-settings.json
+-rw-r--r--   0        0        0      727 2021-09-10 21:55:36.653177 sbcoyote-1.4.3/rkviewer/json/settings.json
+-rw-r--r--   0        0        0     3399 2023-02-10 23:42:55.235161 sbcoyote-1.4.3/rkviewer/main.py
+-rw-r--r--   0        0        0    12295 2021-09-10 21:55:36.701263 sbcoyote-1.4.3/rkviewer/mvc.py
+-rw-r--r--   0        0        0        0 2021-09-10 21:55:36.701263 sbcoyote-1.4.3/rkviewer/plugin/__init__.py
+-rw-r--r--   0        0        0    57933 2023-03-29 18:22:16.274177 sbcoyote-1.4.3/rkviewer/plugin/api.py
+-rw-r--r--   0        0        0      513 2021-09-10 21:55:36.703235 sbcoyote-1.4.3/rkviewer/plugin/canvas.py
+-rw-r--r--   0        0        0     9684 2023-03-27 18:05:44.898125 sbcoyote-1.4.3/rkviewer/plugin/classes.py
+-rw-r--r--   0        0        0      154 2021-09-10 21:55:36.704231 sbcoyote-1.4.3/rkviewer/plugin/events.py
+-rw-r--r--   0        0        0    18945 2023-01-26 22:34:13.868916 sbcoyote-1.4.3/rkviewer/plugin_manage.py
+-rw-r--r--   0        0        0        0 2021-09-10 21:55:36.706226 sbcoyote-1.4.3/rkviewer/resources/__init__.py
+-rw-r--r--   0        0        0      335 2021-09-10 21:55:36.705228 sbcoyote-1.4.3/rkviewer/resources/AlignBottom_XP.png
+-rw-r--r--   0        0        0      312 2021-09-10 21:55:36.706226 sbcoyote-1.4.3/rkviewer/resources/alignHorizCenter_XP.png
+-rw-r--r--   0        0        0      298 2021-09-10 21:55:36.707254 sbcoyote-1.4.3/rkviewer/resources/alignHorizEqually_XP.png
+-rw-r--r--   0        0        0      379 2021-09-10 21:55:36.707254 sbcoyote-1.4.3/rkviewer/resources/alignLeft_XP.png
+-rw-r--r--   0        0        0      238 2021-09-10 21:55:36.708254 sbcoyote-1.4.3/rkviewer/resources/alignOnGrid_XP.png
+-rw-r--r--   0        0        0      602 2021-09-10 21:55:36.709251 sbcoyote-1.4.3/rkviewer/resources/alignRight_XP.png
+-rw-r--r--   0        0        0      366 2021-09-10 21:55:36.709251 sbcoyote-1.4.3/rkviewer/resources/alignTop_XP.png
+-rw-r--r--   0        0        0      280 2021-09-10 21:55:36.709251 sbcoyote-1.4.3/rkviewer/resources/alignVertCenter_XP.png
+-rw-r--r--   0        0        0      308 2021-09-10 21:55:36.710248 sbcoyote-1.4.3/rkviewer/resources/alignVertEqually_XP.png
+-rw-r--r--   0        0        0      389 2021-09-10 21:55:36.710248 sbcoyote-1.4.3/rkviewer/resources/info-2-16.png
+-rw-r--r--   0        0        0     8227 2023-01-23 21:52:33.720240 sbcoyote-1.4.3/rkviewer/utils.py
+-rw-r--r--   0        0        0    47660 2023-05-09 22:38:35.239386 sbcoyote-1.4.3/rkviewer/view.py
+-rw-r--r--   0        0        0     8420 2023-04-10 20:09:02.114349 sbcoyote-1.4.3/rkviewer_plugins/addReaction.py
+-rw-r--r--   0        0        0     7700 2023-03-27 21:04:32.885475 sbcoyote-1.4.3/rkviewer_plugins/align_circle.py
+-rw-r--r--   0        0        0    10023 2023-01-24 01:05:59.812128 sbcoyote-1.4.3/rkviewer_plugins/arrow_designer.py
+-rw-r--r--   0        0        0     7910 2023-03-27 23:00:15.322399 sbcoyote-1.4.3/rkviewer_plugins/exportAntimony.py
+-rw-r--r--   0        0        0    72928 2023-05-08 23:25:17.738537 sbcoyote-1.4.3/rkviewer_plugins/exportSBML.py
+-rw-r--r--   0        0        0   165908 2023-05-11 21:25:55.997909 sbcoyote-1.4.3/rkviewer_plugins/importSBML.py
+-rw-r--r--   0        0        0     1152 2023-04-05 18:58:00.989843 sbcoyote-1.4.3/rkviewer_plugins/modelMetrics.py
+-rw-r--r--   0        0        0    16762 2023-03-27 21:03:50.201865 sbcoyote-1.4.3/rkviewer_plugins/networkX.py
+-rw-r--r--   0        0        0    17554 2023-03-27 21:03:22.666400 sbcoyote-1.4.3/rkviewer_plugins/randomNetwork.py
+-rw-r--r--   0        0        0    12839 2023-03-27 21:03:31.309823 sbcoyote-1.4.3/rkviewer_plugins/structuralAnalysis.py
+-rw-r--r--   0        0        0    11909 1970-01-01 00:00:00.000000 sbcoyote-1.4.3/PKG-INFO
```

### Comparing `sbcoyote-1.4.2/LICENSE` & `sbcoyote-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/pyproject.toml` & `sbcoyote-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SBcoyote"
-version = "1.4.2"
+version = "1.4.3"
 description = "SBcoyote: An Extensible Python Based Reaction Editor and Viewer."
 readme = "README.md"
 authors = ["Jin Xu and Gary Geng et al <jxu2019@uw.edu>"]
 packages = [
     #{ include = "*" }
     { include = "rkviewer"},
     { include = "rkviewer_plugins"},
```

### Comparing `sbcoyote-1.4.2/README.md` & `sbcoyote-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/canvas/canvas.py` & `sbcoyote-1.4.3/rkviewer/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/canvas/data.py` & `sbcoyote-1.4.3/rkviewer/canvas/data.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/canvas/elements.py` & `sbcoyote-1.4.3/rkviewer/canvas/elements.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/canvas/geometry.py` & `sbcoyote-1.4.3/rkviewer/canvas/geometry.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/canvas/overlays.py` & `sbcoyote-1.4.3/rkviewer/canvas/overlays.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/canvas/state.py` & `sbcoyote-1.4.3/rkviewer/canvas/state.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/canvas/utils.py` & `sbcoyote-1.4.3/rkviewer/canvas/utils.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/config.py` & `sbcoyote-1.4.3/rkviewer/config.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/controller.py` & `sbcoyote-1.4.3/rkviewer/controller.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/events.py` & `sbcoyote-1.4.3/rkviewer/events.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/forms.py` & `sbcoyote-1.4.3/rkviewer/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1233,14 +1233,15 @@
                         return
                     try:
                         self.controller.set_node_size(self.net_index, i, Vec2(float(hw[0]), float(hw[1])))
                     except:
                         self.main_section.SetValidationState(
                         False, ctrl_id, 'Should be in the form of "width, height" or "(w1, h1); (w2, h2)"')   
                         return
+                   
 
         self.main_section.SetValidationState(True, self.size_ctrl.GetId())
 
     def OnNodeStatusChoice(self, evt):
         """Callback for the change node status, floating or boundary."""
         selected = self.nodeStatusDropDown.GetSelection()
         if selected == 0:
```

### Comparing `sbcoyote-1.4.2/rkviewer/iodine.py` & `sbcoyote-1.4.3/rkviewer/iodine.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/json/.default-settings.json` & `sbcoyote-1.4.3/rkviewer/json/.default-settings.json`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/json/dark-settings.json` & `sbcoyote-1.4.3/rkviewer/json/dark-settings.json`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/json/settings.json` & `sbcoyote-1.4.3/rkviewer/json/settings.json`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/main.py` & `sbcoyote-1.4.3/rkviewer/main.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/mvc.py` & `sbcoyote-1.4.3/rkviewer/mvc.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/plugin/api.py` & `sbcoyote-1.4.3/rkviewer/plugin/api.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/plugin/canvas.py` & `sbcoyote-1.4.3/rkviewer/plugin/canvas.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/plugin/classes.py` & `sbcoyote-1.4.3/rkviewer/plugin/classes.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/plugin_manage.py` & `sbcoyote-1.4.3/rkviewer/plugin_manage.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/resources/alignRight_XP.png` & `sbcoyote-1.4.3/rkviewer/resources/alignRight_XP.png`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/utils.py` & `sbcoyote-1.4.3/rkviewer/utils.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer/view.py` & `sbcoyote-1.4.3/rkviewer/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -701,15 +701,15 @@
         self.Bind(wx.EVT_MENU, callback, item)
         self.menu_events.append((callback, item))
         return item
 
     def onAboutDlg(self, event):
         info = wx.adv.AboutDialogInfo()
         info.SetName("SBcoyote")
-        info.SetVersion("1.4.2")
+        info.SetVersion("1.4.3")
         info.SetCopyright("(c) 2023 UW Sauro Lab")
         info.SetDescription("An Extensible Python-Based Reaction Editor and Viewer.")
         info.SetWebSite("https://github.com/sys-bio/SBcoyote",
                         "Home Page")  # TODO update home page?
         info.SetDevelopers(["Jin Xu", "Gary Geng", "Nhan D. Nguyen", "Carmen Perena-Corte","Claire Samuels", "Herbert M. Sauro"])# TODO update authors
         info.SetLicense("MIT")
```

### Comparing `sbcoyote-1.4.2/rkviewer_plugins/addReaction.py` & `sbcoyote-1.4.3/rkviewer_plugins/addReaction.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer_plugins/align_circle.py` & `sbcoyote-1.4.3/rkviewer_plugins/align_circle.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer_plugins/arrow_designer.py` & `sbcoyote-1.4.3/rkviewer_plugins/arrow_designer.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer_plugins/exportAntimony.py` & `sbcoyote-1.4.3/rkviewer_plugins/exportAntimony.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer_plugins/exportSBML.py` & `sbcoyote-1.4.3/rkviewer_plugins/exportSBML.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Export the network on canvas to an SBML string as save it as a file.
-Version 1.0.8: Author: Jin Xu (2023)
+Version 1.1.8: Author: Jin Xu (2023)
 """
 
 
 # pylint: disable=maybe-no-member
 
 from inspect import Parameter
 import wx
@@ -12,20 +12,21 @@
 from rkviewer.plugin.classes import PluginMetadata, WindowedPlugin, PluginCategory
 from rkviewer.plugin import api
 from rkviewer.plugin.api import Node, Vec2, Reaction, Color, get_node_by_index
 import os
 from libsbml import * # does not have to import in the main.py too
 import re # to process kinetic_law string
 from rkviewer.config import get_theme
+from rkviewer.mvc import ModifierTipStyle
 
 class ExportSBML(WindowedPlugin):
     metadata = PluginMetadata(
         name='ExportSBML',
         author='Jin Xu',
-        version='1.0.8',
+        version='1.1.8',
         short_desc='Export SBML.',
         long_desc='Export the SBML String from the network on canvas and save it to a file.',
         category=PluginCategory.MODELS
     )
 
 
     def create_window(self, dialog):
@@ -208,18 +209,21 @@
                     comp_border_color = [comp.border_color.r, comp.border_color.g, comp.border_color.b]
                     if comp_fill_color != [255, 255, 255] or comp_border_color != [255, 255, 255]:
                         if (comp.position.x + comp.size.x) > pos[0]:
                             pos[0] = comp.position.x + comp.size.x
                         if (comp.position.y + comp.size.y) > pos[1]:
                             pos[1] = comp.position.y + comp.size.y
             for rxn in allReactions:
-                if rxn.center_pos.x > pos[0]:
-                    pos[0] = rxn.center_pos.x
-                if rxn.center_pos.y > pos[1]:
-                    pos[1] = rxn.center_pos.y
+                try:
+                    if rxn.center_pos.x > pos[0]:
+                        pos[0] = rxn.center_pos.x
+                    if rxn.center_pos.y > pos[1]:
+                        pos[1] = rxn.center_pos.y
+                except:
+                    pass
                 idx = rxn.index
                 handle_pos = api.get_reaction_center_handle(netIn, idx)
                 if handle_pos.x > pos[0]:
                     pos[0] = handle_pos.x
                 if handle_pos.y > pos[1]:
                     pos[1] = handle_pos.y
                 src = rxn.sources
@@ -262,17 +266,22 @@
 
             # create the Compartment and species
 
             comp_id_list = []
             for i in range(numCompartments):
                 comp_id_list.append(allcompartments[i].id) 
 
+            flag_comp_def = 0
+            for i in range(numNodes):
+                comp_idx = allNodes[i].comp_idx
+                if comp_idx == -1:
+                    flag_comp_def = 1
 
             if numCompartments != 0:
-                if "_compartment_default_" not in comp_id_list:
+                if "_compartment_default_" not in comp_id_list and flag_comp_def == 1:
                     compartment = model.createCompartment()
                     comp_id="_compartment_default_"
                     compartment.setId(comp_id)
                     compartment.setConstant(True)
                     compartment.setVolume(1.)
                 
                 for i in range(numCompartments):   
@@ -336,14 +345,15 @@
                         species.setBoundaryCondition(False)
                         species.setConstant(False)             
                         if allNodes[i].floating_node == False:
                             species.setBoundaryCondition(True)
                             species.setConstant(True)
             # create reactions:
             parameter_id_value_dict_self_pre = {}  
+            parameter_id_value_dict = api.get_parameters(netIn)
             
             for i in range(numReactions):
                 reaction_id = allReactions[i].id
                 rct = [] # id list of the rcts
                 prd = []
                 mod = []
                 rct_num = len(allReactions[i].sources)
@@ -363,41 +373,41 @@
                     temp_spec_id = get_node_by_index(netIn, list(allReactions[i].modifiers)[j]).id
                     if ' ' in temp_spec_id:
                         temp_spec_id = temp_spec_id.replace(' ', '_')
                     mod.append(temp_spec_id)
 
                 kinetic_law_from_user = allReactions[i].rate_law
                 
-                if kinetic_law_from_user == '':
-                    kinetic_law = ''
-                    kinetic_law = kinetic_law + 'E' + str (i) + '*(k' + str (i) 
-                    parameter_id_value_dict_self_pre['E' + str(i)] = 0.1
-                    parameter_id_value_dict_self_pre['k' + str(i)] = 0.1
+                # if kinetic_law_from_user == '':
+                #     kinetic_law = ''
+                #     kinetic_law = kinetic_law + 'E' + str (i) + '*(k' + str (i) 
+                #     parameter_id_value_dict_self_pre['E' + str(i)] = 0.1
+                #     parameter_id_value_dict_self_pre['k' + str(i)] = 0.1
 
-                    for j in range(rct_num):
-                        kinetic_law = kinetic_law + '*' + rct[j]
+                #     for j in range(rct_num):
+                #         kinetic_law = kinetic_law + '*' + rct[j]
                         
-                    if isReversible:
-                        kinetic_law = kinetic_law + ' - k' + str (i) + 'r'
-                        parameter_id_value_dict_self_pre['k' + str (i) + 'r'] = 0.1
-                        for j in range(prd_num):
-                            kinetic_law = kinetic_law + '*' + prd[j]
-                    kinetic_law = kinetic_law + ')'
-                else:
-                    kinetic_law = kinetic_law_from_user
+                #     if isReversible:
+                #         kinetic_law = kinetic_law + ' - k' + str (i) + 'r'
+                #         parameter_id_value_dict_self_pre['k' + str (i) + 'r'] = 0.1
+                #         for j in range(prd_num):
+                #             kinetic_law = kinetic_law + '*' + prd[j]
+                #     kinetic_law = kinetic_law + ')'
+                # else:
+                kinetic_law = kinetic_law_from_user
 
                 reaction = model.createReaction()
                 reaction.setId(allReactions[i].id)
                 reaction.setReversible(False)
                 reaction.setFast(False)
                 if isReversible:
                     reaction.setReversible(True)
-                
-                kinetics = reaction.createKineticLaw()
-                kinetics.setFormula(kinetic_law)
+                if kinetic_law != "" and len(parameter_id_value_dict) != 0:  
+                    kinetics = reaction.createKineticLaw()
+                    kinetics.setFormula(kinetic_law)
                 
                 for j in range(rct_num):
                     reference = reaction.createReactant()
                     reference.setSpecies(rct[j])
                     ref_id = "SpecRef_" + reaction_id + "_rct" + str(j)
                     reference.setId(ref_id)
                     #reference.setStoichiometry(1.)
@@ -413,15 +423,15 @@
 
                 for j in range(mod_num):
                     reference = reaction.createModifier()
                     reference.setSpecies(mod[j])
                     ref_id = "SpecRef_" + reaction_id + "_mod" + str(j)
                     reference.setId(ref_id)
 
-            parameter_id_value_dict = api.get_parameters(netIn)
+
             parameter_id_value_dict.update(parameter_id_value_dict_self_pre)
             for name,dict_ in parameter_id_value_dict.items():
                 parameters = model.createParameter()
                 parameters.setId(name)
                 parameters.setValue(dict_)
                 parameters.setConstant(True)
             
@@ -592,15 +602,15 @@
                     bb_id  = "bb_spec_text_" + spec_id + '_idx_' + str(spec_index)
                     textGlyph.setBoundingBox(BoundingBox(layoutns, bb_id, pos_x_text, pos_y_text, width, height))
                     #textGlyph.setOriginOfTextId(specG_id)
                     textGlyph.setGraphicalObjectId(specG_id)
 
             # create the ReactionGlyphs and SpeciesReferenceGlyphs
             for i in range(numReactions):
-                if allReactions[i].using_bezier == True:
+                if allReactions[i].using_bezier == True: #bezier curve
                     reaction_id = allReactions[i].id
                     center_pos = allReactions[i].center_pos
                     centroid = api.compute_centroid(netIn, allReactions[i].sources, allReactions[i].targets)
                     try:
                         center_value = [center_pos.x,center_pos.y]
                     except:
                         center_value = [centroid.x,centroid.y]
@@ -622,14 +632,15 @@
                     mod = []
                     rct_index = []
                     prd_index = []
                     mod_index = []
                     rct_num = len(allReactions[i].sources)
                     prd_num = len(allReactions[i].targets)
                     mod_num = len(allReactions[i].modifiers)
+                    mod_type = allReactions[i].modifier_tip_style
 
                     for j in range(rct_num):
                         temp_spec_id = get_node_by_index(netIn, allReactions[i].sources[j]).id
                         if ' ' in temp_spec_id:
                             temp_spec_id = temp_spec_id.replace(' ', '_')
                         rct.append(temp_spec_id)
                         rct_index.append(get_node_by_index(netIn, allReactions[i].sources[j]).index)
@@ -729,16 +740,18 @@
                         ref_id = "SpecRef_" + reaction_id + "_mod" + str(j)
                         speciesReferenceGlyph = reactionGlyph.createSpeciesReferenceGlyph()
                         specsRefG_id = "SpecRefG_" + reaction_id + "_mod" + str(j)
                         specG_id = "SpecG_" + mod[j]  + '_idx_' + str(mod_index[j])
                         speciesReferenceGlyph.setId(specsRefG_id)
                         speciesReferenceGlyph.setSpeciesGlyphId(specG_id)
                         speciesReferenceGlyph.setSpeciesReferenceId(ref_id)
-                        speciesReferenceGlyph.setRole(SPECIES_ROLE_MODIFIER)
-
+                        if mod_type == ModifierTipStyle.TEE:
+                            speciesReferenceGlyph.setRole(SPECIES_ROLE_INHIBITOR)
+                        else:
+                            speciesReferenceGlyph.setRole(SPECIES_ROLE_MODIFIER)
                         speciesReferenceCurve = speciesReferenceGlyph.getCurve()
                         mod_ls = speciesReferenceCurve.createLineSegment()
 
                         pos_x = get_node_by_index(netIn, list(allReactions[i].modifiers)[j]).position.x
                         pos_y = get_node_by_index(netIn, list(allReactions[i].modifiers)[j]).position.y
                         width = get_node_by_index(netIn, list(allReactions[i].modifiers)[j]).size.x
                         height = get_node_by_index(netIn, list(allReactions[i].modifiers)[j]).size.y
@@ -763,17 +776,18 @@
                             [mod_end_x, mod_end_y] = center_value
                         try:
                             mod_ls.setEnd(Point(layoutns, mod_end_x, mod_end_y))
                         except:
                             mod_ls.setEnd(Point(layoutns, center_value[0], center_value[1]))
             
 
-                else:
+                else: #straight line
                     reaction_id = allReactions[i].id
                     center_pos = allReactions[i].center_pos
+                    reaction_line_thickness = allReactions[i].line_thickness
                     centroid = api.compute_centroid(netIn, allReactions[i].sources, allReactions[i].targets)
                     handles = api.default_handle_positions(netIn,i)
 
                     try:
                         center_value = [center_pos.x,center_pos.y]
                     except:
                         center_value = [centroid.x,centroid.y]
@@ -794,14 +808,15 @@
                     mod = []
                     rct_index = []
                     prd_index = []
                     mod_index = []
                     rct_num = len(allReactions[i].sources)
                     prd_num = len(allReactions[i].targets)
                     mod_num = len(allReactions[i].modifiers)
+                    mod_type = allReactions[i].modifier_tip_style
 
                     # for j in range(rct_num):
                     #     rct.append(get_node_by_index(netIn, allReactions[i].sources[j]).id)
                     #     rct_index.append(get_node_by_index(netIn, allReactions[i].sources[j]).index)
                     # for j in range(prd_num):
                     #     prd.append(get_node_by_index(netIn, allReactions[i].targets[j]).id)
                     #     prd_index.append(get_node_by_index(netIn, allReactions[i].targets[j]).index)
@@ -836,91 +851,111 @@
                         specsRefG_id = "SpecRefG_" + reaction_id + "_rct" + str(j)
                         specG_id = "SpecG_" + rct[j] + '_idx_' + str(rct_index[j])
                         speciesReferenceGlyph.setId(specsRefG_id)
                         speciesReferenceGlyph.setSpeciesGlyphId(specG_id)
                         speciesReferenceGlyph.setSpeciesReferenceId(ref_id)
                         speciesReferenceGlyph.setRole(SPECIES_ROLE_SUBSTRATE)
                         speciesReferenceCurve = speciesReferenceGlyph.getCurve()
-                        cb = speciesReferenceCurve.createCubicBezier()
-                        # handle1 = api.get_reaction_center_handle(netIn, allReactions[i].index)
-                        # handle2 = api.get_reaction_node_handle(netIn, allReactions[i].index,
+                        # cb = speciesReferenceCurve.createCubicBezier()
+                        # #handle1 = api.get_reaction_center_handle(netIn, allReactions[i].index)
+                        # #handle2 = api.get_reaction_node_handle(netIn, allReactions[i].index,
                         #     allReactions[i].sources[j],is_source=True)
                         handle1 = handles[0]
                         handle2 = handles[1+j]
+                        rct_ls = speciesReferenceCurve.createLineSegment()
                         
                         pos_x = get_node_by_index(netIn,allReactions[i].sources[j]).position.x
                         pos_y = get_node_by_index(netIn,allReactions[i].sources[j]).position.y
                         width = get_node_by_index(netIn,allReactions[i].sources[j]).size.x
                         height = get_node_by_index(netIn,allReactions[i].sources[j]).size.y
 
                         line_end_pt = _cross_point(handle2, 
                         [pos_x-reaction_line_thickness, pos_y-reaction_line_thickness], 
                         [width+2.*reaction_line_thickness,height+2.*reaction_line_thickness])
                         if line_end_pt == None:
                             line_end_pt = _cross_point(center_value, 
                             [pos_x-reaction_line_thickness, pos_y-reaction_line_thickness], 
                             [width+2.*reaction_line_thickness,height+2.*reaction_line_thickness])
+                        # try:
+                        #     cb.setStart(Point(layoutns, line_end_pt[0], line_end_pt[1]))
+                        # except:     
+                        #     cb.setStart(Point(layoutns, pos_x + 0.5*width, pos_y + 0.5*height))
+
+                        # cb.setBasePoint1(Point(layoutns, handle2.x, handle2.y))
+                        # cb.setBasePoint2(Point(layoutns, handle1.x, handle1.y))
+                        # cb.setEnd(Point(layoutns, center_value[0], center_value[1]))
+                        
                         try:
-                            cb.setStart(Point(layoutns, line_end_pt[0], line_end_pt[1]))
+                            rct_ls.setStart(Point(layoutns, line_end_pt[0], line_end_pt[1]))
                         except:     
-                            cb.setStart(Point(layoutns, pos_x + 0.5*width, pos_y + 0.5*height))
+                            rct_ls.setStart(Point(layoutns, pos_x + 0.5*width, pos_y + 0.5*height))
 
-                        cb.setBasePoint1(Point(layoutns, handle2.x, handle2.y))
-                        cb.setBasePoint2(Point(layoutns, handle1.x, handle1.y))
-                        cb.setEnd(Point(layoutns, center_value[0], center_value[1]))
+                        rct_ls.setEnd(Point(layoutns, center_value[0], center_value[1]))
 
                     for j in range(prd_num):
                         ref_id = "SpecRef_" + reaction_id + "_prd" + str(j)
                         speciesReferenceGlyph = reactionGlyph.createSpeciesReferenceGlyph()
                         specsRefG_id = "SpecRefG_" + reaction_id + "_prd" + str(j)
                         specG_id = "SpecG_" + prd[j]  + '_idx_' + str(prd_index[j])
                         speciesReferenceGlyph.setId(specsRefG_id)
                         speciesReferenceGlyph.setSpeciesGlyphId(specG_id)
                         speciesReferenceGlyph.setSpeciesReferenceId(ref_id)
                         speciesReferenceGlyph.setRole(SPECIES_ROLE_PRODUCT)
 
                         speciesReferenceCurve = speciesReferenceGlyph.getCurve()
-                        cb = speciesReferenceCurve.createCubicBezier()
-                        cb.setStart(Point(layoutns, center_value[0], center_value[1]))
+                        # cb = speciesReferenceCurve.createCubicBezier()
+                        # cb.setStart(Point(layoutns, center_value[0], center_value[1]))
 
-                        # handle1 = api.get_reaction_center_handle(netIn, allReactions[i].index)
-                        # handle2 = api.get_reaction_node_handle(netIn, allReactions[i].index,
-                        #     allReactions[i].targets[j],is_source=False)
+                        # # handle1 = api.get_reaction_center_handle(netIn, allReactions[i].index)
+                        # # handle2 = api.get_reaction_node_handle(netIn, allReactions[i].index,
+                        # #     allReactions[i].targets[j],is_source=False)
 
                         handle1 = [2.*center_value[0]-handles[0].x, 2.*center_value[1]-handles[0].y]
                         handle2 = handles[1+rct_num+j]
-                        cb.setBasePoint1(Point(layoutns, handle1[0], handle1[1]))
-                        cb.setBasePoint2(Point(layoutns, handle2.x, handle2.y))
+                        # cb.setBasePoint1(Point(layoutns, handle1[0], handle1[1]))
+                        # cb.setBasePoint2(Point(layoutns, handle2.x, handle2.y))
+
+                        prd_ls = speciesReferenceCurve.createLineSegment()
 
                         pos_x = get_node_by_index(netIn, allReactions[i].targets[j]).position.x
                         pos_y = get_node_by_index(netIn, allReactions[i].targets[j]).position.y
                         width = get_node_by_index(netIn, allReactions[i].targets[j]).size.x
                         height = get_node_by_index(netIn, allReactions[i].targets[j]).size.y
 
                         line_head_pt = _cross_point(handle2, 
                         [pos_x-reaction_line_thickness, pos_y-reaction_line_thickness], 
                         [width+2.*reaction_line_thickness,height+2.*reaction_line_thickness])
                         if line_head_pt == None:
                             line_head_pt = _cross_point(center_value, 
                             [pos_x-reaction_line_thickness, pos_y-reaction_line_thickness], 
                             [width+2.*reaction_line_thickness,height+2.*reaction_line_thickness])                   
+                        # try:
+                        #     cb.setEnd(Point(layoutns, line_head_pt[0], line_head_pt[1]))
+                        # except:
+                        #     cb.setEnd(Point(layoutns, pos_x + 0.5*width, pos_y + 0.5*height))
+
+                        prd_ls.setStart(Point(layoutns, center_value[0], center_value[1]))
                         try:
-                            cb.setEnd(Point(layoutns, line_head_pt[0], line_head_pt[1]))
+                            prd_ls.setEnd(Point(layoutns, line_head_pt[0], line_head_pt[1]))
                         except:
-                            cb.setEnd(Point(layoutns, pos_x + 0.5*width, pos_y + 0.5*height))
+                            prd_ls.setEnd(Point(layoutns, pos_x + 0.5*width, pos_y + 0.5*height))
+
 
                     for j in range(mod_num):
                         ref_id = "SpecRef_" + reaction_id + "_mod" + str(j)
                         speciesReferenceGlyph = reactionGlyph.createSpeciesReferenceGlyph()
                         specsRefG_id = "SpecRefG_" + reaction_id + "_mod" + str(j)
                         specG_id = "SpecG_" + mod[j]  + '_idx_' + str(mod_index[j])
                         speciesReferenceGlyph.setId(specsRefG_id)
                         speciesReferenceGlyph.setSpeciesGlyphId(specG_id)
                         speciesReferenceGlyph.setSpeciesReferenceId(ref_id)
-                        speciesReferenceGlyph.setRole(SPECIES_ROLE_MODIFIER)
+                        if mod_type == ModifierTipStyle.TEE:
+                            speciesReferenceGlyph.setRole(SPECIES_ROLE_INHIBITOR)
+                        else:
+                            speciesReferenceGlyph.setRole(SPECIES_ROLE_MODIFIER)
 
                         speciesReferenceCurve = speciesReferenceGlyph.getCurve()
                         mod_ls = speciesReferenceCurve.createLineSegment()
 
                         pos_x = get_node_by_index(netIn, list(allReactions[i].modifiers)[j]).position.x
                         pos_y = get_node_by_index(netIn, list(allReactions[i].modifiers)[j]).position.y
                         width = get_node_by_index(netIn, list(allReactions[i].modifiers)[j]).size.x
@@ -1157,14 +1192,15 @@
                     style.addType("REACTIONGLYPH")
                     style.addId(reactionG_id)
                     #style.addId(reaction_id)
 
                     rct_num = len(allReactions[i].sources)
                     prd_num = len(allReactions[i].targets)
                     mod_num = len(allReactions[i].modifiers)
+                    mod_type = allReactions[i].modifier_tip_style
 
                     lineEnding = rInfo.createLineEnding()
                     lineEnding_id = '_line_ending_default_NONE_' + rxn_id
                     lineEnding.setId(lineEnding_id)
                     bb_id = "bb_" + lineEnding_id
                     [pos_x, pos_y] = [0., 0.]
                     [width, height] = [0., 0.]
@@ -1258,18 +1294,23 @@
 
                     border_color_str = reaction_fill_color_str
                     color = rInfo.createColorDefinition()
                     color.setId("lineEnding_border_color" + "_" + lineEnding_mod_id)
                     color.setColorValue(border_color_str)
                     #lineEnding.getGroup().setStroke('lineEnding_border_color' + '_' + lineEnding_mod_id)
                     lineEnding.getGroup().setStroke("_default_modifier_color_")
-
-                    ellipse = lineEnding.getGroup().createEllipse()
-                    ellipse.setCenter2D(RelAbsVector(0, 0.), RelAbsVector(0, 0.))
-                    ellipse.setRadii(RelAbsVector(0, 100.), RelAbsVector(0, 100.))
+                    if mod_type == ModifierTipStyle.TEE:
+                        rectangle = lineEnding.getGroup().createRectangle()
+                        rectangle.setCoordinatesAndSize(RelAbsVector(0,0),
+                        RelAbsVector(0,-100),RelAbsVector(0,50),
+                        RelAbsVector(0,50),RelAbsVector(0,200))
+                    else:
+                        ellipse = lineEnding.getGroup().createEllipse()
+                        ellipse.setCenter2D(RelAbsVector(0, 0.), RelAbsVector(0, 0.))
+                        ellipse.setRadii(RelAbsVector(0, 50.), RelAbsVector(0, 50.))
 
                     for j in range(mod_num):
                         specsRefG_id = "SpecRefG_" + rxn_id + "_mod" + str(j)
                         style = rInfo.createStyle("specRefGlyphStyle" + rxn_id + "_mod" + str(j))
                         style.getGroup().setEndHead(lineEnding_mod_id)
                         #style.getGroup().setStroke("reaction_fill_color" + "_" + rxn_id)
                         #style.getGroup().setFill("lineEnding_fill_color" + "_" + lineEnding_mod_id)
```

### Comparing `sbcoyote-1.4.2/rkviewer_plugins/importSBML.py` & `sbcoyote-1.4.3/rkviewer_plugins/importSBML.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Import an SBML string from a file and visualize it to a network on canvas.
-Version 1.1.8: Author: Jin Xu (2023)
+Version 1.2.8: Author: Jin Xu (2023)
 """
 
 
 # pylint: disable=maybe-no-member
 
 from ast import Num
 from inspect import Parameter
@@ -20,20 +20,22 @@
 import simplesbml # does not have to import in the main.py too
 from libsbml import *
 import math
 import random as _random
 import pandas as pd
 from rkviewer.config import get_theme
 import SBMLDiagrams
+import re # Extract substrings between brackets
+from rkviewer.mvc import ModifierTipStyle
 
 class IMPORTSBML(WindowedPlugin):
     metadata = PluginMetadata(
         name='ImportSBML',
         author='Jin Xu',
-        version='1.1.8',
+        version='1.2.8',
         short_desc='Import SBML.',
         long_desc='Import an SBML String from a file and visualize it as a network on canvas.',
         category=PluginCategory.MODELS
     )
 
     def create_window(self, dialog):
         """
@@ -124,15 +126,14 @@
 
         color_data = {"decimal_rgb": ['[240,248,255]', '[250,235,215]', '[0,255,255]', '[127,255,212]', '[240,255,255]', '[245,245,220]', '[255,228,196]', '[0,0,0]', '[255,235,205]', '[0,0,255]', '[138,43,226]', '[165,42,42]', '[222,184,135]', '[95,158,160]', '[127,255,0]', '[210,105,30]', '[255,127,80]', '[100,149,237]', '[255,248,220]', '[220,20,60]', '[0,255,255]', '[0,0,139]', '[0,139,139]', '[184,134,11]', '[169,169,169]', '[0,100,0]', '[189,183,107]', '[139,0,139]', '[85,107,47]', '[255,140,0]', '[153,50,204]', '[139,0,0]', '[233,150,122]', '[143,188,143]', '[72,61,139]', '[47,79,79]', '[0,206,209]', '[148,0,211]', '[255,20,147]', '[0,191,255]', '[105,105,105]', '[30,144,255]', '[178,34,34]', '[255,250,240]', '[34,139,34]', '[255,0,255]', '[220,220,220]', '[248,248,255]', '[255,215,0]', '[218,165,32]', '[128,128,128]', '[0,128,0]', '[173,255,47]', '[240,255,240]', '[255,105,180]', '[205,92,92]', '[75,0,130]', '[255,255,240]', '[240,230,140]', '[230,230,250]', '[255,240,245]', '[124,252,0]', '[255,250,205]', '[173,216,230]', '[240,128,128]', '[224,255,255]', '[250,250,210]', '[144,238,144]', '[211,211,211]', '[255,182,193]', '[255,160,122]', '[32,178,170]', '[135,206,250]', '[119,136,153]', '[176,196,222]', '[255,255,224]', '[0,255,0]', '[50,205,50]', '[250,240,230]', '[255,0,255]', '[128,0,0]', '[102,205,170]', '[0,0,205]', '[186,85,211]', '[147,112,219]', '[60,179,113]', '[123,104,238]', '[0,250,154]', '[72,209,204]', '[199,21,133]', '[25,25,112]', '[245,255,250]', '[255,228,225]', '[255,228,181]', '[255,222,173]', '[0,0,128]', '[253,245,230]', '[128,128,0]', '[107,142,35]', '[255,165,0]', '[255,69,0]', '[218,112,214]', '[238,232,170]', '[152,251,152]', '[175,238,238]', '[219,112,147]', '[255,239,213]', '[255,218,185]', '[205,133,63]', '[255,192,203]', '[221,160,221]', '[176,224,230]', '[128,0,128]', '[255,0,0]', '[188,143,143]', '[65,105,225]', '[139,69,19]', '[250,128,114]', '[244,164,96]', '[46,139,87]', '[255,245,238]', '[160,82,45]', '[192,192,192]', '[135,206,235]', '[106,90,205]', '[112,128,144]', '[255,250,250]', '[0,255,127]', '[70,130,180]', '[210,180,140]', '[0,128,128]', '[216,191,216]', '[255,99,71]', '[64,224,208]', '[238,130,238]', '[245,222,179]', '[255,255,255]', '[245,245,245]', '[255,255,0]', '[154,205,50]'],\
             "html_name":['AliceBlue', 'AntiqueWhite', 'Aqua', 'Aquamarine', 'Azure', 'Beige', 'Bisque', 'Black', 'BlanchedAlmond', 'Blue', 'BlueViolet', 'Brown', 'BurlyWood', 'CadetBlue', 'Chartreuse', 'Chocolate', 'Coral', 'CornflowerBlue', 'Cornsilk', 'Crimson', 'Cyan', 'DarkBlue', 'DarkCyan', 'DarkGoldenrod', 'DarkGray', 'DarkGreen', 'DarkKhaki', 'DarkMagenta', 'DarkOliveGreen', 'DarkOrange', 'DarkOrchid', 'DarkRed', 'DarkSalmon', 'DarkSeaGreen', 'DarkSlateBlue', 'DarkSlateGray', 'DarkTurquoise', 'DarkViolet', 'DeepPink', 'DeepSkyBlue', 'DimGray', 'DodgerBlue', 'FireBrick', 'FloralWhite', 'ForestGreen', 'Fuchsia', 'Gainsboro', 'GhostWhite', 'Gold', 'Goldenrod', 'Gray', 'Green', 'GreenYellow', 'Honeydew', 'HotPink', 'IndianRed', 'Indigo', 'Ivory', 'Khaki', 'Lavender', 'LavenderBlush', 'LawnGreen', 'LemonChiffon', 'LightBlue', 'LightCoral', 'LightCyan', 'LightGoldenrodYellow', 'LightGreen', 'LightGrey', 'LightPink', 'LightSalmon', 'LightSeaGreen', 'LightSkyBlue', 'LightSlateGray', 'LightSteelBlue', 'LightYellow', 'Lime', 'LimeGreen', 'Linen', 'Magenta', 'Maroon', 'MediumAquamarine', 'MediumBlue', 'MediumOrchid', 'MediumPurple', 'MediumSeaGreen', 'MediumSlateBlue', 'MediumSpringGreen', 'MediumTurquoise', 'MediumVioletRed', 'MidnightBlue', 'MintCream', 'MistyRose', 'Moccasin', 'NavajoWhite', 'Navy', 'OldLace', 'Olive', 'OliveDrab', 'Orange', 'OrangeRed', 'Orchid', 'PaleGoldenrod', 'PaleGreen', 'PaleTurquoise', 'PaleVioletRed', 'PapayaWhip', 'PeachPuff', 'Peru', 'Pink', 'Plum', 'PowderBlue', 'Purple', 'Red', 'RosyBrown', 'RoyalBlue', 'SaddleBrown', 'Salmon', 'SandyBrown', 'SeaGreen', 'Seashell', 'Sienna', 'Silver', 'SkyBlue', 'SlateBlue', 'SlateGray', 'Snow', 'SpringGreen', 'SteelBlue', 'Tan', 'Teal', 'Thistle', 'Tomato', 'Turquoise', 'Violet', 'Wheat', 'White', 'WhiteSmoke', 'Yellow', 'YellowGreen'],\
             "hex_string":['#F0F8FF', '#FAEBD7', '#00FFFF', '#7FFFD4', '#F0FFFF', '#F5F5DC', '#FFE4C4', '#000000', '#FFEBCD', '#0000FF', '#8A2BE2', '#A52A2A', '#DEB887', '#5F9EA0', '#7FFF00', '#D2691E', '#FF7F50', '#6495ED', '#FFF8DC', '#DC143C', '#00FFFF', '#00008B', '#008B8B', '#B8860B', '#A9A9A9', '#006400', '#BDB76B', '#8B008B', '#556B2F', '#FF8C00', '#9932CC', '#8B0000', '#E9967A', '#8FBC8F', '#483D8B', '#2F4F4F', '#00CED1', '#9400D3', '#FF1493', '#00BFFF', '#696969', '#1E90FF', '#B22222', '#FFFAF0', '#228B22', '#FF00FF', '#DCDCDC', '#F8F8FF', '#FFD700', '#DAA520', '#808080', '#008000', '#ADFF2F', '#F0FFF0', '#FF69B4', '#CD5C5C', '#4B0082', '#FFFFF0', '#F0E68C', '#E6E6FA', '#FFF0F5', '#7CFC00', '#FFFACD', '#ADD8E6', '#F08080', '#E0FFFF', '#FAFAD2', '#90EE90', '#D3D3D3', '#FFB6C1', '#FFA07A', '#20B2AA', '#87CEFA', '#778899', '#B0C4DE', '#FFFFE0', '#00FF00', '#32CD32', '#FAF0E6', '#FF00FF', '#800000', '#66CDAA', '#0000CD', '#BA55D3', '#9370DB', '#3CB371', '#7B68EE', '#00FA9A', '#48D1CC', '#C71585', '#191970', '#F5FFFA', '#FFE4E1', '#FFE4B5', '#FFDEAD', '#000080', '#FDF5E6', '#808000', '#6B8E23', '#FFA500', '#FF4500', '#DA70D6', '#EEE8AA', '#98FB98', '#AFEEEE', '#DB7093', '#FFEFD5', '#FFDAB9', '#CD853F', '#FFC0CB', '#DDA0DD', '#B0E0E6', '#800080', '#FF0000', '#BC8F8F', '#4169E1', '#8B4513', '#FA8072', '#F4A460', '#2E8B57', '#FFF5EE', '#A0522D', '#C0C0C0', '#87CEEB', '#6A5ACD', '#708090', '#FFFAFA', '#00FF7F', '#4682B4', '#D2B48C', '#008080', '#D8BFD8', '#FF6347', '#40E0D0', '#EE82EE', '#F5DEB3', '#FFFFFF', '#F5F5F5', '#FFFF00', '#9ACD32']}
         df_color = pd.DataFrame(color_data)
         df_color["html_name"] = df_color["html_name"].str.lower()
 
-
         # if len(sbmlStr) == 0:
         #   if showDialogues:
         #     wx.MessageBox("Please import an SBML file.", "Message", wx.OK | wx.ICON_INFORMATION)
         # else:
         if len(sbmlStr) != 0:
             net_index = 0
             api.clear_network(net_index)
@@ -189,14 +190,19 @@
                     raise Exception("Errors in SBML Model: ", errMsgRead)
                         
                 model_layout = document.getModel()
                 try:
                     mplugin = model_layout.getPlugin("layout")
                 except:
                     raise Exception("There is no layout.") 
+                
+                sbml_definitions =[model_layout.getFunctionDefinition(n) for n 
+                    in range(model_layout.getNumFunctionDefinitions())]
+                function_definitions = [FunctionDefinition(s) for s in sbml_definitions]
+                
                 # Get the first Layout object via LayoutModelPlugin object.
                 #
                 # if mplugin is None:
                 #     if showDialogues:
                 #         wx.MessageBox("There is no layout information, so positions are randomly assigned.", "Message", wx.OK | wx.ICON_INFORMATION)
                 # else:
                 #def_canvas_width = 10000.
@@ -241,14 +247,21 @@
                             boundingbox = compGlyph.getBoundingBox()
                             height = boundingbox.getHeight()
                             width = boundingbox.getWidth()
                             pos_x = boundingbox.getX()
                             pos_y = boundingbox.getY()
                             comp_dimension_list.append([width,height])
                             comp_position_list.append([pos_x,pos_y])
+                        if "_compartment_default_" in comp_id_list:
+                            numCompGlyphs -= 1
+                            idx = comp_id_list.index("_compartment_default_")
+                            comp_id_list.remove("_compartment_default_")
+                            del compGlyph_id_list[idx]
+                            del comp_dimension_list[idx]
+                            del comp_position_list[idx]                      
 
 
                         reaction_id_list = []
                         reactionGlyph_id_list = []
                         reaction_center_list = []
                         kinetics_list = []
                         #rct_specGlyph_list = []
@@ -256,16 +269,18 @@
                         reaction_center_handle_list = []
                         rct_specGlyph_handle_list = []
                         prd_specGlyph_handle_list = []
                         reaction_mod_list = []
                         reaction_rct_list = []
                         reaction_prd_list = []
                         mod_specGlyph_list = []
+                        reaction_type_list = []  
 
                         for i in range(numReactionGlyphs):
+                            reaction_straight_flag = 1
                             reactionGlyph = layout.getReactionGlyph(i)
                             reaction_id = reactionGlyph.getReactionId()
                             reactionGlyph_id = reactionGlyph.getId()
                             curve = reactionGlyph.getCurve()
                             # listOfCurveSegments = curve.getListOfCurveSegments()
                             # for j in range(len(listOfCurveSegments)):
                             #     #center_x = curve.getCurveSegment(j).getStart().x()
@@ -333,14 +348,17 @@
                             reaction_id = reactionGlyph.getReactionId()
                            
                             reaction_id_list.append(reaction_id)
                             reactionGlyph_id_list.append(reactionGlyph_id)
                             reaction = model_layout.getReaction(reaction_id)
                             try:
                                 kinetics = reaction.getKineticLaw().getFormula()
+                                if len(function_definitions) > 0:
+                                    #kinetics = _expandFormula(kinetics, function_definitions)
+                                    kinetics = ""
                             except:
                                 kinetics = ""
                             kinetics_list.append(kinetics)
 
                             temp_mod_list = []
                             for j in range(len(reaction.getListOfModifiers())):
                                 modSpecRef = reaction.getModifier(j)
@@ -407,25 +425,34 @@
                                     #if math.sqrt(line_start_pt, center_pt) <= math.dist(line_end_pt, center_pt):
                                     if dist_start_center <= dist_end_center:
                                         #line starts from center
                                         spec_lineend_pos = line_end_pt
                                         modifier_lineend_pos = line_start_pt
                                         
                                         if num_curve == 1:
+                                            try_flag = 0
                                             try: #bezier
                                                 center_handle_candidate = [segment.getBasePoint1().getXOffset(), 
                                                                 segment.getBasePoint1().getYOffset()]                                
                                                 spec_handle = [segment.getBasePoint2().getXOffset(),
-                                                            segment.getBasePoint2().getYOffset()] 
+                                                            segment.getBasePoint2().getYOffset()]
+                                                
                                             except: #straight
                                                 spec_handle = [.5*(center_pt[0]+line_end_pt[0]),
                                                 .5*(center_pt[1]+line_end_pt[1])]
                                                 center_handle_candidate = center_pt
-                                                #spec_handle = center_pt         
-                                        else:  
+                                                try_flag = 1
+                                                #spec_handle = []
+                                                #center_handle_candidate = []
+                                                #spec_handle = center_pt 
+                                            if try_flag == 0:
+                                                reaction_straight_flag = 0 
+
+                                        else:
+                                            reaction_straight_flag = 0  
                                             try: #bezier
                                                 center_handle_candidate = []  
                                                 flag_bezier = 0  
                                                 for segment in curve.getListOfCurveSegments():
                                                     if segment.getTypeCode() == 102:
                                                         flag_bezier = 1
                                                 for segment in curve.getListOfCurveSegments():
@@ -447,25 +474,30 @@
                                                 #spec_handle = center_pt 
                                     else:
                                         #line starts from species
                                         spec_lineend_pos = line_start_pt
                                         modifier_lineend_pos = line_end_pt
                                         
                                         if num_curve == 1:
+                                            try_flag = 0
                                             try: #bezier
                                                 spec_handle = [segment.getBasePoint1().getXOffset(), 
                                                                     segment.getBasePoint1().getYOffset()]                                
                                                 center_handle_candidate = [segment.getBasePoint2().getXOffset(),
                                                                 segment.getBasePoint2().getYOffset()]
                                             except: #straight
                                                 spec_handle = [.5*(center_pt[0]+line_start_pt[0]),
                                                 .5*(center_pt[1]+line_start_pt[1])]
                                                 center_handle_candidate = center_pt
                                                 #spec_handle = center_pt
+                                                try_flag = 1
+                                            if try_flag == 0:
+                                                reaction_straight_flag = 0 
                                         else:
+                                            reaction_straight_flag = 0 
                                             try: #bezier
                                                 center_handle_candidate = [] 
                                                 flag_bezier = 0  
                                                 for segment in curve.getListOfCurveSegments():
                                                     if segment.getTypeCode() == 102:
                                                         flag_bezier = 1
                                                 for segment in curve.getListOfCurveSegments():
@@ -483,14 +515,15 @@
                                             except: #straight
                                                 spec_handle = [.5*(center_pt[0]+line_start_pt[0]),
                                                 .5*(center_pt[1]+line_start_pt[1])]
                                                 center_handle_candidate = center_pt
                                                 #spec_handle = center_pt
 
                                 except:
+                                    reaction_straight_flag = 0 
                                     center_handle_candidate = []
                                     spec_handle = []
 
                                 role = specRefGlyph.getRoleString()
                                 specGlyph_id = specRefGlyph.getSpeciesGlyphId()
                                 specGlyph = layout.getSpeciesGlyph(specGlyph_id)
                                 
@@ -589,30 +622,34 @@
                                     #rct_specGlyph_temp_list.append(specGlyph_id)
                                     rct_specGlyph_handles_temp_list.append([specGlyph_id,spec_handle,specRefGlyph_id,spec_lineend_pos])
                                 elif role == "product" or role == "sideproduct": #it is a prd
                                     #prd_specGlyph_temp_list.append(specGlyph_id)
                                     if center_handle[1] == []:
                                         center_handle[1] = center_handle_candidate
                                     prd_specGlyph_handles_temp_list.append([specGlyph_id,spec_handle,specRefGlyph_id,spec_lineend_pos])
-                                elif role == "modifier" or role == 'activator': #it is a modifier
-                                    mod_specGlyph_temp_list.append(specGlyph_id)
+                                elif role == "modifier" or role == 'activator' or role == "inhibitor": #it is a modifier
+                                    mod_specGlyph_temp_list.append([specGlyph_id, role])
                             #rct_specGlyph_list.append(rct_specGlyph_temp_list)
                             #prd_specGlyph_list.append(prd_specGlyph_temp_list)
                             try:
                                 if center_handle[0] != []:
                                     reaction_center_handle_list.append(center_handle[0])
                                 else:
                                     reaction_center_handle_list.append(center_handle[1])
                             except:
                                 #raise Exception("Can not find center handle information to process.")
                                 reaction_center_handle_list.append([])
                             rct_specGlyph_handle_list.append(rct_specGlyph_handles_temp_list)
                             prd_specGlyph_handle_list.append(prd_specGlyph_handles_temp_list)    
                             mod_specGlyph_list.append(mod_specGlyph_temp_list)
-                         
+                            if reaction_straight_flag == 1:
+                                reaction_type_list.append(False)#straight line
+                            else:
+                                reaction_type_list.append(True)#bezier curve
+
                         #orphan nodes
                         for i in range(numSpecGlyphs):
                             specGlyph = layout.getSpeciesGlyph(i)
                             specGlyph_id = specGlyph.getId()
                             if specGlyph_id not in specGlyph_id_list:
                                 specGlyph_id_list.append(specGlyph_id)
                                 spec_id = specGlyph.getSpeciesId()
@@ -1169,15 +1206,19 @@
                 FloatingNodes_ids = model.getListOfFloatingSpecies()
                 numBoundaryNodes  = model.getNumBoundarySpecies()
                 BoundaryNodes_ids = model.getListOfBoundarySpecies()
                 numRxns   = model.getNumReactions()
                 Rxns_ids  = model.getListOfReactionIds()
                 numComps  = model.getNumCompartments()
                 Comps_ids = model.getListOfCompartmentIds()
-                numNodes = numFloatingNodes + numBoundaryNodes
+                if "_compartment_default_" in Comps_ids:
+                    numComps -= 1
+                    Comps_ids.remove("_compartment_default_")
+                numNodes = model.getNumSpecies()
+                Nodes_ids = model.getListOfAllSpecies()
 
                 parameter_list = model.getListOfParameterIds()
 
                 for p in parameter_list:
                     if model.isParameterValueSet(p): 
                     #if there is only parameter id without parameter value, it won't be considered 
                         api.set_parameter_value(net_index, p, model.getParameterValue(p))
@@ -1233,32 +1274,33 @@
                     for i in range(numComps):
                         temp_id = Comps_ids[i]
                         
                         vol= model.getCompartmentVolume(i)
                         if math.isnan(vol):
                             vol = 1.
                         if temp_id == "_compartment_default_":
-                            if len(comp_id_list) != 0:
-                                dimension = [def_comp_width, def_comp_height]
-                                position = [10, 10]                  
-                                for j in range(numCompGlyphs):
-                                    if comp_id_list[j] == temp_id:
-                                        dimension = comp_dimension_list[j]
-                                        position = comp_position_list[j]
-                                api.add_compartment(net_index, id=temp_id, volume = vol,
-                                size=Vec2(dimension[0],dimension[1]), position=Vec2(position[0],position[1]),
-                                fill_color = api.Color(255, 255, 255, 0), #the last digit for transparent
-                                border_color = api.Color(255, 255, 255, 0),
-                                border_width = comp_border_width)  
-                            else:
-                                api.add_compartment(net_index, id=temp_id, volume = vol,
-                                size=Vec2(def_comp_width,def_comp_height), position=Vec2(10,10),
-                                fill_color = api.Color(255, 255, 255, 0), #the last digit for transparent
-                                border_color = api.Color(255, 255, 255, 0),
-                                border_width = comp_border_width)
+                            pass
+                            # if len(comp_id_list) != 0:
+                            #     dimension = [def_comp_width, def_comp_height]
+                            #     position = [10, 10]                  
+                            #     for j in range(numCompGlyphs):
+                            #         if comp_id_list[j] == temp_id:
+                            #             dimension = comp_dimension_list[j]
+                            #             position = comp_position_list[j]
+                            #     api.add_compartment(net_index, id=temp_id, volume = vol,
+                            #     size=Vec2(dimension[0],dimension[1]), position=Vec2(position[0],position[1]),
+                            #     fill_color = api.Color(255, 255, 255, 0), #the last digit for transparent
+                            #     border_color = api.Color(255, 255, 255, 0),
+                            #     border_width = comp_border_width)  
+                            # else:
+                            #     api.add_compartment(net_index, id=temp_id, volume = vol,
+                            #     size=Vec2(def_comp_width,def_comp_height), position=Vec2(10,10),
+                            #     fill_color = api.Color(255, 255, 255, 0), #the last digit for transparent
+                            #     border_color = api.Color(255, 255, 255, 0),
+                            #     border_width = comp_border_width)
                         else:
                             if len(comp_id_list) != 0:
                             #if mplugin is not None:                    
                                 for j in range(numCompGlyphs):
                                     if comp_id_list[j] == temp_id:
                                         dimension = comp_dimension_list[j]
                                         position = comp_position_list[j]
@@ -1504,68 +1546,74 @@
                                     #api.set_node_shape_property(net_index, nodeIdx_temp, -1, "font_size", int(text_font_size))
                                     id_list.append(temp_id)
                                     nodeIdx_list.append(nodeIdx_temp)
                                     nodeIdx_specGlyph_alias_list.append([nodeIdx_temp,tempGlyph_id])
                                 
                                 comp_id = model.getCompartmentIdSpeciesIsIn(temp_id)
                                 for xx in range(numComps):
-                                    if comp_id == Comps_ids[xx]:            
-                                        api.set_compartment_of_node(net_index=net_index, node_index=nodeIdx_temp, comp_index=xx)             
-                                     
+                                    if comp_id == Comps_ids[xx]: 
+                                        try:           
+                                            api.set_compartment_of_node(net_index=net_index, node_index=nodeIdx_temp, comp_index=xx)             
+                                        except:
+                                            pass                                   
                                 for k in range(numCompGlyphs):
                                     if len(comp_id) != 0 and comp_id == comp_id_list[k]:
                                         comp_node_list[k].append(nodeIdx_temp)
 
                     if len(comp_id_list) != 0 or numComps != 0:
                         for i in range(numComps):
                             temp_id = Comps_ids[i]
                             if temp_id == '_compartment_default_': 
-                                #numNodes is different from len(nodeIdx_list) because of alias node
+                                # #numNodes is different from len(nodeIdx_list) because of alias node
                                 node_list_default = [item for item in range(len(nodeIdx_list))]
+                                # for j in range(len(node_list_default)):
+                                #     try:
+                                #         api.set_compartment_of_node(net_index=net_index, node_index=node_list_default[j], comp_index=i)
+                                #     except:
+                                #         pass # Orphan nodes are removed
                                 for j in range(len(node_list_default)):
-                                    try:
-                                        api.set_compartment_of_node(net_index=net_index, node_index=node_list_default[j], comp_index=i)
-                                    except:
-                                        pass # Orphan nodes are removed
+                                    api.set_compartment_of_node(net_index=net_index, node_index=node_list_default[j], comp_index=-1)
                             for j in range(numCompGlyphs):
                                 if comp_id_list[j] == temp_id:
                                     node_list_temp = comp_node_list[j]
                                 else:
                                     node_list_temp = []
                         
                                 for k in range(len(node_list_temp)):
                                     try:
                                         api.set_compartment_of_node(net_index=net_index, node_index=node_list_temp[k], comp_index=i)
                                     except:
                                         pass
                     else:
                         for i in range(len(nodeIdx_list)):
-                            api.set_compartment_of_node(net_index=net_index, node_index=nodeIdx_list[i], comp_index=0)
-
+                            #api.set_compartment_of_node(net_index=net_index, node_index=nodeIdx_list[i], comp_index=0)
+                            api.set_compartment_of_node(net_index=net_index, node_index=nodeIdx_list[i], comp_index=-1)
 
                     nodeIdx_specGlyph_whole_list = nodeIdx_specGlyph_list + nodeIdx_specGlyph_alias_list
 
                     dummy_node_id_index = 0
                     allNodes = api.get_nodes(net_index)
                     allCompartments = api.get_compartments(net_index)
                     for i in range (numReactionGlyphs):
                         src = []
                         dst = []
                         mod = []
+                        mod_type = ModifierTipStyle.CIRCLE
                         src_handle = []
                         dst_handle = []
                         src_lineend_pos = []
                         dst_lineend_pos = []
                         temp_id = reaction_id_list[i]
                         kinetics = kinetics_list[i]
                         rct_num = len(rct_specGlyph_handle_list[i])
                         prd_num = len(prd_specGlyph_handle_list[i])
                         #mod_num = max(len(mod_specGlyph_list[i]),len(reaction_mod_list[i]))
                         mod_num = len(mod_specGlyph_list[i])
-
+                        reaction_type = reaction_type_list[i]
+                        
                         # for j in range(rct_num):
                         #     temp_specGlyph_id = rct_specGlyph_list[i][j]
                         #     for k in range(numSpec_in_reaction):
                         #         if temp_specGlyph_id == nodeIdx_specGlyph_whole_list[k][1]:
                         #             rct_idx = nodeIdx_specGlyph_whole_list[k][0]
                                     
                         #     src.append(rct_idx)
@@ -1594,27 +1642,30 @@
                                         prd_idx = nodeIdx_specGlyph_whole_list[k][0]
                                 dst.append(prd_idx)
                                 dst_handle.append(prd_specGlyph_handle_list[i][j][1])
                                 dst_lineend_pos.append(prd_specGlyph_handle_list[i][j][3])
 
                             for j in range(mod_num):
                                 if len(mod_specGlyph_list[i]) != 0:
-                                    temp_specGlyph_id = mod_specGlyph_list[i][j]
+                                    temp_specGlyph_id = mod_specGlyph_list[i][j][0]
                                     for k in range(numSpec_in_reaction):
                                         if temp_specGlyph_id == nodeIdx_specGlyph_whole_list[k][1]:
                                             mod_idx = nodeIdx_specGlyph_whole_list[k][0]
                                     mod.append(mod_idx)
+                                    if mod_specGlyph_list[i][j][1] == "inhibitor":
+                                        mod_type = ModifierTipStyle.TEE
                                 else:
                                     for k in range(len(spec_specGlyph_id_list)):
                                         if reaction_mod_list[i][j] == spec_specGlyph_id_list[k][0]:
                                             temp_specGlyph_id = spec_specGlyph_id_list[k][1]
                                     for k in range(numSpec_in_reaction):
                                         if temp_specGlyph_id == nodeIdx_specGlyph_whole_list[k][1]:
                                             mod_idx = nodeIdx_specGlyph_whole_list[k][0]
                                     mod.append(mod_idx)
+                                    
                         else:
                             rct_num = model.getNumReactants(i)
                             prd_num = model.getNumProducts(i)
                             mod_num = model.getNumModifiers(temp_id)
                     
                             for j in range(rct_num):
                                 rct_id = model.getReactant(temp_id,j)
@@ -1634,15 +1685,47 @@
                                         tempGlyph_id = spec_specGlyph_id_list[k][1]
                                 for k in range(numSpec_in_reaction):
                                     if nodeIdx_specGlyph_whole_list[k][1] == tempGlyph_id:
                                         prd_idx = nodeIdx_specGlyph_whole_list[k][0]
                                 dst.append(prd_idx)
                                 #dst_handle.append(prd_specGlyph_handle_list[i][j][1])
 
-                            modifiers = model.getListOfModifiers(temp_id)
+                            #modifiers = model.getListOfModifiers(temp_id) 
+                            #simple sbml bug with repeated first modifiers
+                            reaction = model_layout.getReaction(temp_id)
+                            modifiers = []
+                            for j in range(len(reaction.getListOfModifiers())):
+                                modSpecRef = reaction.getModifier(j)
+                                modifiers.append(modSpecRef.getSpecies())
+
+                            #parameter in kinetic law 
+                            try:  
+                                kineticLaw = reaction.getKineticLaw()
+                                kinetic_parameter_list = []
+                                kinetic_parameter_value_list = []
+                                for j in range(len(kineticLaw.getListOfParameters())):
+                                    parameter = kineticLaw.getParameter(j)
+                                    name = parameter.getName()
+                                    if parameter.isSetValue():
+                                        value = kineticLaw.getParameter(j).getValue()
+                                    else:
+                                        value = 0.
+                                    kinetic_parameter_list.append(name)
+                                    kinetic_parameter_value_list.append(value)
+                                for j in range(len(kinetic_parameter_list)):
+                                    p = kinetic_parameter_list[j]
+                                    v = kinetic_parameter_value_list[j]
+                                    try:
+                                        api.set_parameter_value(net_index, p, v)
+                                    except:
+                                        pass
+                            except:
+                                pass
+
+
                             for j in range(mod_num):
                                 mod_id = modifiers[j]
                                 for k in range(len(spec_specGlyph_id_list)):
                                     if spec_specGlyph_id_list[k][0] == mod_id:
                                         tempGlyph_id = spec_specGlyph_id_list[k][1]
                                 for k in range(numSpec_in_reaction):
                                     if nodeIdx_specGlyph_whole_list[k][1] == tempGlyph_id:
@@ -1823,30 +1906,35 @@
 
 
                             handles.extend(src_handle_shift)
                             handles.extend(dst_handle_shift)
                             
                             if len(reaction_line_color) == 3:
                                 reaction_line_color.append(255)
-                            
-                            idx = api.add_reaction(net_index, id=temp_id, reactants=src_corr, products=dst_corr,
+                            idx = api.add_reaction(net_index, id=temp_id, 
+                            reactants=src_corr, products=dst_corr,
                             fill_color=api.Color(reaction_line_color[0],reaction_line_color[1],reaction_line_color[2],reaction_line_color[3]),
-                            line_thickness=reaction_line_width, modifiers = mod)
+                            line_thickness=reaction_line_width, 
+                            modifiers = mod)
+                            
                             api.update_reaction(net_index, idx, ratelaw = kinetics)
-                            handles_Vec2 = []  
-                            if [] not in handles:      
-                                for i in range(len(handles)):
-                                    handles_Vec2.append(Vec2(handles[i][0],handles[i][1]))
+                            if reaction_type == False:
                                 api.update_reaction(net_index, idx, 
-                                center_pos = Vec2(center_position[0],center_position[1]), 
-                                handle_positions=handles_Vec2, 
-                                fill_color=api.Color(reaction_line_color[0],reaction_line_color[1],reaction_line_color[2],reaction_line_color[3]))
-                                
-                        except: #There is no info about the center/handle positions, so set as default 
+                                center_pos = Vec2(center_position[0],center_position[1]),
+                                use_bezier = reaction_type)
+                            else:
+                                handles_Vec2 = [] 
+                                if [] not in handles:      
+                                    for i in range(len(handles)):
+                                        handles_Vec2.append(Vec2(handles[i][0],handles[i][1]))
+                                    api.update_reaction(net_index, idx, center_pos = Vec2(center_position[0],center_position[1]),
+                                    handle_positions=handles_Vec2)
+                            api.update_reaction(net_index, idx, modifier_tip_style = mod_type)  
                             
+                        except: #There is no info about the center/handle positions, so set as default 
                             src_corr = []
                             [src_corr.append(x) for x in src if x not in src_corr]
                             dst_corr = []
                             [dst_corr.append(x) for x in dst if x not in dst_corr]
 
                             #set the information for handle positions, center positions look as straight line
                             #the default positions of center and handles positions sometimes look quite strange.
@@ -2002,15 +2090,15 @@
                             dst_corr.sort()
 
                             handles.extend(src_handles)
                             handles.extend(dst_handles)
 
                             if len(reaction_line_color)==3:
                                 reaction_line_color.append(255)
-
+                    
                             try: 
                                 idx = api.add_reaction(net_index, id=temp_id, reactants=src_corr, products=dst_corr,
                                 fill_color=api.Color(reaction_line_color[0],reaction_line_color[1],reaction_line_color[2],reaction_line_color[3]),
                                 line_thickness=reaction_line_width, modifiers = mod)
                                 api.update_reaction(net_index, idx, ratelaw = kinetics,
                                 fill_color=api.Color(reaction_line_color[0],reaction_line_color[1],reaction_line_color[2],reaction_line_color[3]))
                             except:
@@ -2029,15 +2117,16 @@
                             if [] not in handles:      
                                 for i in range(len(handles)):
                                     handles_Vec2.append(Vec2(handles[i][0],handles[i][1]))
                                 api.update_reaction(net_index, idx, 
                                 center_pos = Vec2(center_position[0],center_position[1]), 
                                 handle_positions=handles_Vec2, 
                                 fill_color=api.Color(reaction_line_color[0],reaction_line_color[1],reaction_line_color[2],reaction_line_color[3]))
-
+                            
+                            api.update_reaction(net_index, idx, modifier_tip_style = mod_type)
 
                 else: # there is no layout information, assign position randomly and size as default
                     
                     comp_id_list = Comps_ids
 
                     for i in range(numComps):
                         temp_id = Comps_ids[i]
@@ -2049,48 +2138,74 @@
 
                         api.add_compartment(net_index, id=temp_id, volume = vol,
                         size=Vec2(dimension[0],dimension[1]),position=Vec2(position[0],position[1]),
                         fill_color = api.Color(comp_fill_color[0],comp_fill_color[1],comp_fill_color[2],comp_fill_color[3]),
                         border_color = api.Color(comp_border_color[0],comp_border_color[1],comp_border_color[2],comp_border_color[3]),
                         border_width = comp_border_width)
 
-                    for i in range (numFloatingNodes):
-                        temp_id = FloatingNodes_ids[i]
-                        comp_id = model.getCompartmentIdSpeciesIsIn(temp_id)
-                        try:
-                            temp_concentration = model.getSpeciesInitialConcentration(temp_id)
-                            if math.nan(temp_concentration):
-                                temp_concentration = 1
-                        except:
-                            temp_concentration = 1.
-                        if spec_border_width == 0.:
-                            spec_border_width = 0.001
-                            spec_border_color = spec_fill_color
-                        nodeIdx_temp = api.add_node(net_index, id=temp_id, size=Vec2(60,40), floating_node = True,
-                        position=Vec2(40 + math.trunc (_random.random()*800), 40 + math.trunc (_random.random()*800)),
-                        fill_color=api.Color(spec_fill_color[0],spec_fill_color[1],spec_fill_color[2],spec_fill_color[3]),
-                        border_color=api.Color(spec_border_color[0],spec_border_color[1],spec_border_color[2],spec_border_color[3]),
-                        border_width=spec_border_width, shape_index=shapeIdx, concentration=temp_concentration)
-                        for j in range(numComps):
-                            if comp_id == comp_id_list[j]:
-                                comp_node_list[j].append(nodeIdx_temp)
+                    # for i in range (numFloatingNodes):
+                    #     temp_id = FloatingNodes_ids[i]
+                    #     comp_id = model.getCompartmentIdSpeciesIsIn(temp_id)
+                    #     try:
+                    #         temp_concentration = model.getSpeciesInitialConcentration(temp_id)
+                    #         if math.nan(temp_concentration):
+                    #             temp_concentration = 1
+                    #     except:
+                    #         temp_concentration = 1.
+                    #     if spec_border_width == 0.:
+                    #         spec_border_width = 0.001
+                    #         spec_border_color = spec_fill_color
+                    #     nodeIdx_temp = api.add_node(net_index, id=temp_id, size=Vec2(60,40), floating_node = True,
+                    #     position=Vec2(40 + math.trunc (_random.random()*800), 40 + math.trunc (_random.random()*800)),
+                    #     fill_color=api.Color(spec_fill_color[0],spec_fill_color[1],spec_fill_color[2],spec_fill_color[3]),
+                    #     border_color=api.Color(spec_border_color[0],spec_border_color[1],spec_border_color[2],spec_border_color[3]),
+                    #     border_width=spec_border_width, shape_index=shapeIdx, concentration=temp_concentration)
+                    #     for j in range(numComps):
+                    #         if comp_id == comp_id_list[j]:
+                    #             comp_node_list[j].append(nodeIdx_temp)
+
+                    # for i in range (numBoundaryNodes):
+                    #     temp_id = BoundaryNodes_ids[i]
+                    #     comp_id = model.getCompartmentIdSpeciesIsIn(temp_id)
+                    #     try:
+                    #         temp_concentration = model.getSpeciesInitialConcentration(temp_id)
+                    #         if math.nan(temp_concentration):
+                    #             temp_concentration = 1
+                    #     except:
+                    #         temp_concentration = 1.0
+                    #     if spec_border_width == 0.:
+                    #         spec_border_width = 0.001
+                    #         spec_border_color = spec_fill_color
+                    #     nodeIdx_temp = api.add_node(net_index, id=temp_id, size=Vec2(60,40), floating_node = False,
+                    #     position=Vec2(40 + math.trunc (_random.random()*800), 40 + math.trunc (_random.random()*800)),
+                    #     fill_color=api.Color(spec_fill_color[0],spec_fill_color[1],spec_fill_color[2],spec_fill_color[3]),
+                    #     border_color=api.Color(spec_border_color[0],spec_border_color[1],spec_border_color[2],spec_border_color[3]),
+                    #     border_width=spec_border_width, shape_index=shapeIdx, concentration=temp_concentration)
+                    #     for j in range(numComps):
+                    #         if comp_id == comp_id_list[j]:
+                    #             comp_node_list[j].append(nodeIdx_temp)
 
-                    for i in range (numBoundaryNodes):
-                        temp_id = BoundaryNodes_ids[i]
+                    for i in range (numNodes):
+                        temp_id = Nodes_ids[i]
                         comp_id = model.getCompartmentIdSpeciesIsIn(temp_id)
                         try:
                             temp_concentration = model.getSpeciesInitialConcentration(temp_id)
                             if math.nan(temp_concentration):
                                 temp_concentration = 1
                         except:
-                            temp_concentration = 1.0
+                            temp_concentration = 1.
                         if spec_border_width == 0.:
                             spec_border_width = 0.001
                             spec_border_color = spec_fill_color
-                        nodeIdx_temp = api.add_node(net_index, id=temp_id, size=Vec2(60,40), floating_node = False,
+                        node_status = True
+                        for j in range(numBoundaryNodes):
+                            temp_b_id = BoundaryNodes_ids[j]
+                            if temp_id == temp_b_id:
+                                node_status = False
+                        nodeIdx_temp = api.add_node(net_index, id=temp_id, size=Vec2(60,40), floating_node = node_status,
                         position=Vec2(40 + math.trunc (_random.random()*800), 40 + math.trunc (_random.random()*800)),
                         fill_color=api.Color(spec_fill_color[0],spec_fill_color[1],spec_fill_color[2],spec_fill_color[3]),
                         border_color=api.Color(spec_border_color[0],spec_border_color[1],spec_border_color[2],spec_border_color[3]),
                         border_width=spec_border_width, shape_index=shapeIdx, concentration=temp_concentration)
                         for j in range(numComps):
                             if comp_id == comp_id_list[j]:
                                 comp_node_list[j].append(nodeIdx_temp)
@@ -2113,40 +2228,74 @@
                     for i in range (numRxns):
                         src = []
                         dst = []
                         mod = []
                         temp_id = Rxns_ids[i]
                         try: 
                             kinetics = model.getRateLaw(i)
+                            if len(function_definitions) > 0:
+                                #kinetics = _expandFormula(kinetics, function_definitions)
+                                kinetics = ""
                         except:
                             kinetics = ""
-                        rct_num = model.getNumReactants(i)
-                        prd_num = model.getNumProducts(i)
+                    
+                        rct_num = model.getNumReactants(temp_id)
+                        prd_num = model.getNumProducts(temp_id)
                         mod_num = model.getNumModifiers(temp_id)
 
                         for j in range(rct_num):
                             rct_id = model.getReactant(temp_id,j)
                             for k in range(numNodes):
                                 if allNodes[k].id == rct_id:
                                     src.append(allNodes[k].index)
 
                         for j in range(prd_num):
                             prd_id = model.getProduct(temp_id,j)
                             for k in range(numNodes):
                                 if allNodes[k].id == prd_id:
                                     dst.append(allNodes[k].index)                   
 
-                        modifiers = model.getListOfModifiers(temp_id)
+                        #modifiers = model.getListOfModifiers(temp_id)
+                        #simple sbml bug with repeated first modifiers
+                        reaction = model_layout.getReaction(temp_id)
+                        modifiers = []
+                        for j in range(len(reaction.getListOfModifiers())):
+                           modSpecRef = reaction.getModifier(j)
+                           modifiers.append(modSpecRef.getSpecies())
+
+                        #parameter in kinetic law
+                        try:
+                            kineticLaw = reaction.getKineticLaw()
+                            kinetic_parameter_list = []
+                            kinetic_parameter_value_list = []
+                            for j in range(len(kineticLaw.getListOfParameters())):
+                                parameter = kineticLaw.getParameter(j)
+                                name = parameter.getName()
+                                if parameter.isSetValue():
+                                    value = kineticLaw.getParameter(j).getValue()
+                                else:
+                                    value = 0.
+                                kinetic_parameter_list.append(name)
+                                kinetic_parameter_value_list.append(value)
+                            for j in range(len(kinetic_parameter_list)):
+                                p = kinetic_parameter_list[j]
+                                v = kinetic_parameter_value_list[j]
+                                try:
+                                    api.set_parameter_value(net_index, p, v)
+                                except:
+                                    pass
+                        except:
+                            pass
+
                         for j in range(mod_num):
                             mod_id = modifiers[j]
                             for k in range(numNodes):
                                 if allNodes[k].id == mod_id:
                                     mod.append(allNodes[k].index) 
-                        mod = set(mod)
-
+                   
                         try: 
                             src_corr = []
                             [src_corr.append(x) for x in src if x not in src_corr]
 
                             dst_corr = []
                             [dst_corr.append(x) for x in dst if x not in dst_corr]
 
@@ -2234,14 +2383,15 @@
                                 dst_position = allNodes[dst_corr[j]].position
                                 dst_dimension = allNodes[dst_corr[j]].size
                                 dst_handle_x = .5*(center_position[0] + dst_position[0] + .5*dst_dimension[0])
                                 dst_handle_y = .5*(center_position[1] + dst_position[1] + .5*dst_dimension[1])
                                 handles.append([dst_handle_x,dst_handle_y])
 
                             handles_Vec2 = []  
+                            
                             if [] not in handles:      
                                 for i in range(len(handles)):
                                     handles_Vec2.append(Vec2(handles[i][0],handles[i][1]))
                                 api.update_reaction(net_index, idx, 
                                 center_pos = Vec2(center_position[0],center_position[1]), 
                                 handle_positions=handles_Vec2, 
                                 fill_color=api.Color(reaction_line_color[0],reaction_line_color[1],reaction_line_color[2],reaction_line_color[3]))
@@ -2257,8 +2407,7 @@
                 if showDialogues:
                     wx.MessageBox("Imported SBML file is invalid.", "Message", wx.OK | wx.ICON_INFORMATION)
 
 
             # except Exception as e:
             #     raise Exception (e) 
 
-
```

### Comparing `sbcoyote-1.4.2/rkviewer_plugins/modelMetrics.py` & `sbcoyote-1.4.3/rkviewer_plugins/modelMetrics.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer_plugins/networkX.py` & `sbcoyote-1.4.3/rkviewer_plugins/networkX.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer_plugins/randomNetwork.py` & `sbcoyote-1.4.3/rkviewer_plugins/randomNetwork.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/rkviewer_plugins/structuralAnalysis.py` & `sbcoyote-1.4.3/rkviewer_plugins/structuralAnalysis.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.4.2/PKG-INFO` & `sbcoyote-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcoyote
-Version: 1.4.2
+Version: 1.4.3
 Summary: SBcoyote: An Extensible Python Based Reaction Editor and Viewer.
 Author: Jin Xu and Gary Geng et al
 Author-email: jxu2019@uw.edu
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

