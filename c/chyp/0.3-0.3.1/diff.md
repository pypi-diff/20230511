# Comparing `tmp/chyp-0.3.tar.gz` & `tmp/chyp-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chyp-0.3.tar", last modified: Tue May  9 19:17:03 2023, max compression
+gzip compressed data, was "chyp-0.3.1.tar", last modified: Thu May 11 20:31:48 2023, max compression
```

## Comparing `chyp-0.3.tar` & `chyp-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-09 19:17:03.482142 chyp-0.3/
--rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.3/LICENSE
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9798 2023-05-09 19:17:03.482142 chyp-0.3/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9259 2023-05-07 21:30:27.000000 chyp-0.3/README.md
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-09 19:17:03.482142 chyp-0.3/chyp/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      727 2023-05-01 10:30:52.000000 chyp-0.3/chyp/__init__.py
--rw-r--r--   0 aleger    (1000) aleger    (1000)      699 2023-05-01 10:09:37.000000 chyp-0.3/chyp/__main__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    16930 2023-05-08 13:24:18.000000 chyp-0.3/chyp/graph.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-09 19:17:03.482142 chyp-0.3/chyp/gui/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      634 2023-05-01 10:14:39.000000 chyp-0.3/chyp/gui/__init__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3739 2023-05-09 07:10:05.000000 chyp-0.3/chyp/gui/app.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1108 2023-05-06 10:32:00.000000 chyp-0.3/chyp/gui/codeview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     5868 2023-05-06 15:16:34.000000 chyp-0.3/chyp/gui/document.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    15080 2023-05-08 20:46:38.000000 chyp-0.3/chyp/gui/editor.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2283 2023-05-08 16:45:36.000000 chyp-0.3/chyp/gui/errorlist.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     7056 2023-05-05 22:42:20.000000 chyp-0.3/chyp/gui/graphscene.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1242 2023-05-05 22:33:30.000000 chyp-0.3/chyp/gui/graphview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2357 2023-05-08 12:36:17.000000 chyp-0.3/chyp/gui/highlighter.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1672 2023-05-05 22:32:53.000000 chyp-0.3/chyp/gui/mainwindow.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9883 2023-05-05 09:52:49.000000 chyp-0.3/chyp/layout.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    10418 2023-05-09 07:19:39.000000 chyp-0.3/chyp/matcher.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     8707 2023-05-08 16:34:40.000000 chyp-0.3/chyp/parser.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3774 2023-05-07 18:11:57.000000 chyp-0.3/chyp/rewrite.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1775 2023-05-08 10:53:38.000000 chyp-0.3/chyp/rule.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.3/chyp/scraps.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4554 2023-05-08 12:31:13.000000 chyp-0.3/chyp/state.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4064 2023-04-23 21:13:55.000000 chyp-0.3/chyp/term.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-09 19:17:03.482142 chyp-0.3/chyp.egg-info/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9798 2023-05-09 19:17:03.000000 chyp-0.3/chyp.egg-info/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      588 2023-05-09 19:17:03.000000 chyp-0.3/chyp.egg-info/SOURCES.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-09 19:17:03.000000 chyp-0.3/chyp.egg-info/dependency_links.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-09 19:17:03.000000 chyp-0.3/chyp.egg-info/entry_points.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-09 19:17:03.000000 chyp-0.3/chyp.egg-info/requires.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-09 19:17:03.000000 chyp-0.3/chyp.egg-info/top_level.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.3/pyproject.toml
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-09 19:17:03.482142 chyp-0.3/setup.cfg
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1063 2023-05-09 19:16:13.000000 chyp-0.3/setup.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-11 20:31:48.578058 chyp-0.3.1/
+-rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.3.1/LICENSE
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9800 2023-05-11 20:31:48.578058 chyp-0.3.1/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9259 2023-05-07 21:30:27.000000 chyp-0.3.1/README.md
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-11 20:31:48.574058 chyp-0.3.1/chyp/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      727 2023-05-01 10:30:52.000000 chyp-0.3.1/chyp/__init__.py
+-rw-r--r--   0 aleger    (1000) aleger    (1000)      699 2023-05-01 10:09:37.000000 chyp-0.3.1/chyp/__main__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    16930 2023-05-08 13:24:18.000000 chyp-0.3.1/chyp/graph.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-11 20:31:48.578058 chyp-0.3.1/chyp/gui/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      634 2023-05-01 10:14:39.000000 chyp-0.3.1/chyp/gui/__init__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3739 2023-05-09 07:10:05.000000 chyp-0.3.1/chyp/gui/app.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1108 2023-05-06 10:32:00.000000 chyp-0.3.1/chyp/gui/codeview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     5986 2023-05-11 09:13:14.000000 chyp-0.3.1/chyp/gui/document.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    15296 2023-05-11 09:14:44.000000 chyp-0.3.1/chyp/gui/editor.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2283 2023-05-08 16:45:36.000000 chyp-0.3.1/chyp/gui/errorlist.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     7056 2023-05-05 22:42:20.000000 chyp-0.3.1/chyp/gui/graphscene.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1242 2023-05-05 22:33:30.000000 chyp-0.3.1/chyp/gui/graphview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2357 2023-05-08 12:36:17.000000 chyp-0.3.1/chyp/gui/highlighter.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1672 2023-05-05 22:32:53.000000 chyp-0.3.1/chyp/gui/mainwindow.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    10405 2023-05-11 20:29:46.000000 chyp-0.3.1/chyp/layout.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11254 2023-05-10 22:12:14.000000 chyp-0.3.1/chyp/matcher.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     8707 2023-05-08 16:34:40.000000 chyp-0.3.1/chyp/parser.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3774 2023-05-07 18:11:57.000000 chyp-0.3.1/chyp/rewrite.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1775 2023-05-08 10:53:38.000000 chyp-0.3.1/chyp/rule.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.3.1/chyp/scraps.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4602 2023-05-11 09:04:26.000000 chyp-0.3.1/chyp/state.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4143 2023-05-11 20:25:03.000000 chyp-0.3.1/chyp/term.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-11 20:31:48.578058 chyp-0.3.1/chyp.egg-info/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9800 2023-05-11 20:31:48.000000 chyp-0.3.1/chyp.egg-info/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      588 2023-05-11 20:31:48.000000 chyp-0.3.1/chyp.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-11 20:31:48.000000 chyp-0.3.1/chyp.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-11 20:31:48.000000 chyp-0.3.1/chyp.egg-info/entry_points.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-11 20:31:48.000000 chyp-0.3.1/chyp.egg-info/requires.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-11 20:31:48.000000 chyp-0.3.1/chyp.egg-info/top_level.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.3.1/pyproject.toml
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-11 20:31:48.578058 chyp-0.3.1/setup.cfg
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1065 2023-05-11 20:31:14.000000 chyp-0.3.1/setup.py
```

### Comparing `chyp-0.3/LICENSE` & `chyp-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chyp-0.3/PKG-INFO` & `chyp-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.3
+Version: 0.3.1
 Summary: An interactive theorem prover for monoidal categories
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chyp-0.3/README.md` & `chyp-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/__init__.py` & `chyp-0.3.1/chyp/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/__main__.py` & `chyp-0.3.1/chyp/__main__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/graph.py` & `chyp-0.3.1/chyp/graph.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/gui/__init__.py` & `chyp-0.3.1/chyp/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/gui/app.py` & `chyp-0.3.1/chyp/gui/app.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/gui/codeview.py` & `chyp-0.3.1/chyp/gui/codeview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/gui/document.py` & `chyp-0.3.1/chyp/gui/document.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from PySide6.QtWidgets import QFileDialog, QMessageBox, QPlainTextDocumentLayout, QWidget
 
 from .highlighter import ChypHighlighter
 
 class ChypDocument(QTextDocument):
     recentFilesChanged = Signal()
     fileNameChanged = Signal()
+    documentReplaced = Signal()
 
     def __init__(self, parent: QWidget) -> None:
         super().__init__(parent)
         self.parent_widget = parent
         self.setDefaultFont(QFont("monospace", 14))
         self.setDocumentLayout(QPlainTextDocumentLayout(self))
         self.highlighter = ChypHighlighter(self)
@@ -71,14 +72,15 @@
 
     def new(self) -> None:
         if self.confirm_close():
             self.file_name = ''
             self.setPlainText('')
             self.setModified(False)
             self.fileNameChanged.emit()
+            self.documentReplaced.emit()
 
     def open(self, file_name: str='') -> None:
         if self.confirm_close():
             conf = QSettings('chyp', 'chyp')
             if file_name == '':
                 o = conf.value('last_dir')
                 last_dir = o if isinstance(o, str) else QDir.home().absolutePath()
@@ -90,14 +92,15 @@
                 conf.setValue('last_dir', QFileInfo(file_name).absolutePath())
                 self.file_name = file_name
                 with open(file_name) as f:
                     self.setPlainText(f.read())
                 self.add_to_recent_files(self.file_name)
                 self.setModified(False)
                 self.fileNameChanged.emit()
+                self.documentReplaced.emit()
 
     def save(self) -> bool:
         if self.file_name:
             with open(self.file_name, 'w') as f:
                 f.write(self.toPlainText())
             self.add_to_recent_files(self.file_name)
             self.setModified(False)
```

### Comparing `chyp-0.3/chyp/gui/editor.py` & `chyp-0.3.1/chyp/gui/editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 
         self.code_view = CodeView()
         self.doc = ChypDocument(self)
         self.code_view.setDocument(self.doc)
         self.doc.fileNameChanged.connect(self.update_file_name)
         self.doc.modificationChanged.connect(self.update_file_name)
         self.doc.recentFilesChanged.connect(self.update_recent_files)
+        self.doc.documentReplaced.connect(self.reset_state)
         self.update_file_name()
 
         self.splitter.addWidget(self.code_view)
         self.code_view.setFocus()
 
         self.error_view = QTreeView()
         self.error_view.setModel(ErrorListModel())
@@ -187,14 +188,19 @@
 
         self.file_open_recent.clear()
         for f in self.doc.recent_files():
             fi = QFileInfo(f)
             action = self.file_open_recent.addAction(fi.fileName())
             action.triggered.connect(open_recent(f))
 
+    def reset_state(self) -> None:
+        cursor = self.code_view.textCursor()
+        cursor.setPosition(0)
+        self.code_view.setTextCursor(cursor)
+
     def invalidate_text(self) -> None:
         self.parsed = False
         self.graph_cache = dict()
         self.code_view.set_current_region(None)
         self.update_state(quiet=True)
 
     def next_part(self, step:int=1) -> None:
```

### Comparing `chyp-0.3/chyp/gui/errorlist.py` & `chyp-0.3.1/chyp/gui/errorlist.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/gui/graphscene.py` & `chyp-0.3.1/chyp/gui/graphscene.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/gui/graphview.py` & `chyp-0.3.1/chyp/gui/graphview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/gui/highlighter.py` & `chyp-0.3.1/chyp/gui/highlighter.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/gui/mainwindow.py` & `chyp-0.3.1/chyp/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/layout.py` & `chyp-0.3.1/chyp/layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def convex_layout(g: Graph) -> None:
     """A layout based on `layer_decomp` and convex optimisation
 
     Vertices and edges are placed in layers according to `layer_decomp`. Their
     y-coordinates are chosen by convex optimation to try to make connections as
     straight as possible subject to the constraints:
-      1. vertices must be in order and at least 1.0 apart
+      1. inputs and outputs must be in order and at least 1.0 apart
       2. edges must be in order and not overlapping
     """
     v_layers, e_layers = layer_decomp(g)
 
     # initialise x-coordinates and rough y-coordinates
     x = -(len(v_layers) - 1) * 1.5
     for layer in range(len(v_layers)):
@@ -58,37 +58,50 @@
     ey = Variable(g.num_edges(), 'ey')
 
     # maintain a table from vertex/edge names to variable indices
     vtab = { v : i for i, v in enumerate(g.vertices()) }
     etab = { e : i for i, e in enumerate(g.edges()) }
 
     constr = []
-    opt = [Constant(0.1) * vy[i] for i in range(g.num_edges())]
-    for layer in range(len(v_layers)):
-        v_layer = v_layers[layer]
-        for i in range(len(v_layer)-1):
-            v1 = v_layer[i]
-            v2 = v_layer[i+1]
-            constr.append(vy[vtab[v2]] - vy[vtab[v1]] >= Constant(1))
+    opt = []
+    # opt = [Constant(0.1) * vy[i] for i in range(g.num_edges())]
 
-        # break if this is the final v_layer (hence no more e_layers)
-        if layer >= len(e_layers): break
-        e_layer = e_layers[layer]
+    for vlist in (g.inputs(), g.outputs()):
+        for i in range(len(vlist) - 1):
+            v1 = vlist[i]
+            v2 = vlist[i+1]
+            constr.append(vy[vtab[v2]] - vy[vtab[v1]] >= Constant(1))
+            opt.append(Constant(0.1) * (vy[vtab[v2]] - vy[vtab[v1]]))
 
+    for e_layer in e_layers:
         for i in range(len(e_layer)):
             e1 = e_layer[i]
-            for vlist, weight in ((g.source(e1), 1.0), (g.target(e1), 2.0)):
-                for j, v in enumerate(vlist):
-                    y_shift = Constant(0.0 if len(vlist) <= 1 else ((j / (len(vlist) - 1)) - 0.5))
-                    opt.append(Constant(weight) * (vy[vtab[v]] - (ey[etab[e1]] + y_shift)))
-
             if i+1 >= len(e_layer): break
             e2 = e_layer[i+1]
             dist = (g.edge_data(e1).box_size() + g.edge_data(e2).box_size()) * 0.5
             constr.append(ey[etab[e2]] - ey[etab[e1]] >= Constant(dist))
+            opt.append(Constant(0.1) * (ey[etab[e2]] - ey[etab[e1]]))
+
+    for v in g.vertices():
+        pos1 = vy[vtab[v]]
+        pos2 = vy[vtab[v]]
+        if len(g.in_edges(v)) >= 1:
+            e = next(iter(g.in_edges(v)))
+            t = g.target(e)
+            y_shift = Constant(0.0 if len(t) <= 1 else ((t.index(v) / (len(t) - 1)) - 0.5))
+            pos1 = ey[etab[e]] + y_shift
+
+        if len(g.out_edges(v)) >= 1:
+            e = next(iter(g.out_edges(v)))
+            s = g.source(e)
+            y_shift = Constant(0.0 if len(s) <= 1 else ((s.index(v) / (len(s) - 1)) - 0.5))
+            pos2 = ey[etab[e]] + y_shift
+
+        opt.append(pos1 - pos2)
+
 
     # problem = Problem(Minimize(cp.sum_squares(cp.vstack(opt))), constr)
     problem = Problem(Minimize(cp.norm1(cp.vstack(opt))), constr)
     problem.solve()
     min = None
     max = None
     for v,i in vtab.items():
@@ -102,15 +115,20 @@
         for v in g.vertices():
             g.vertex_data(v).y -= yshift
     else:
         yshift = 0
 
     for e,i in etab.items():
         y = ey.value[i]
-        g.edge_data(e).y = y - yshift
+        ed = g.edge_data(e)
+        ed.y = y - yshift
+        for j,v in enumerate(ed.t):
+            if not g.is_boundary(v):
+                yshift_v = 0 if len(ed.t) <= 1 else ((j / (len(ed.t) - 1)) - 0.5)
+                g.vertex_data(v).y = ed.y + yshift_v
 
 
 def layer_layout(g: Graph) -> None:
     """A simple layout using `layer_decomp`.
 
     Vertices are evenly spaced around the x-axis and edges are placed
     as close to the average y-coordinate of their inputs as possible.
```

### Comparing `chyp-0.3/chyp/matcher.py` & `chyp-0.3.1/chyp/matcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,20 +150,54 @@
                 all(e in self.emap for e in self.dom.out_edges(v)))
 
     # def cod_nhd_mapped(self, cod_v: int):
     #     """Returns True if nhd(cod_v) is the range of emap"""
     #     return (all(e in self.eimg for e in self.cod.in_edges(cod_v)) and
     #             all(e in self.eimg for e in self.cod.out_edges(cod_v)))
 
+    def map_scalars(self) -> bool:
+        """Try to extend the match by mapping all scalars (i.e. 0 -> 0 edges)
+
+        Returns True if is successful. Note that any matchings of scalars will yield
+        isomorphic results under rewriting, so we don't return a list of all the possible
+        matchings.
+        """
+        cod_sc = []
+        for e in self.cod.edges():
+            ed = self.cod.edge_data(e)
+            if len(ed.s) == 0 and len(ed.t) == 0:
+                cod_sc.append((e, ed.value))
+
+        for e in self.dom.edges():
+            match_log("trying to map scalar edge {}".format(e))
+            ed = self.dom.edge_data(e)
+            if len(ed.s) != 0 or len(ed.t) != 0: continue
+            found = False
+            for i in range(len(cod_sc)):
+                e1, val = cod_sc[i]
+                if val == ed.value:
+                    cod_sc.pop(i)
+                    self.emap[e] = e1
+                    self.eimg.add(e1)
+                    found = True
+                    match_log("successfully mapped scalar {} -> {}".format(e, e1))
+                    break
+            if not found:
+                match_log("match failed: could not map scalar edge {}".format(e))
+                return False
+
+        return True
+
+
 
     def more(self) -> List[Match]:
         # a list of partial matches the same as this one, but matching 1 more vertex or edge
         ms = []
 
-        # first try to complete nhds of vertices already matched
+        # first, try to complete nhds of vertices already matched
         for v in self.vmap:
             # check if a vertex's nhd is already fully mapped
             if self.dom_nhd_mapped(v): continue
             cod_v = self.vmap[v]
 
             # try to extend the match by mapping the next in_edge
             for e in self.dom.in_edges(v):
@@ -209,33 +243,25 @@
     def is_convex(self) -> bool:
         future = self.cod.successors([self.vmap[v] for v in self.dom.outputs() if v in self.vmap])
         for v in self.dom.inputs():
             if v in self.vmap and self.vmap[v] in future:
                 return False
         return True
 
-    # def is_cospan_iso(self) -> bool:
-    #     d_in = self.dom.inputs()
-    #     d_out = self.dom.outputs()
-    #     c_in = self.cod.inputs()
-    #     c_out = self.cod.outputs()
-    #
-    #     return (len(d_in) == len(c_in) and
-    #             len(d_out) == len(c_out) and
-    #             all(self.vmap[d_in[i]] == c_in[i] for i in range(len(d_in))) and
-    #             all(self.vmap[d_out[i]] == c_out[i] for i in range(len(d_out))) and
-    #             self.is_injective() and self.is_surjective())
-
 
 
 class Matches(Iterable):
     def __init__(self, dom: Graph, cod: Graph, initial_match: Optional[Match] = None, convex=True) -> None:
         if initial_match is None: initial_match = Match(dom=dom, cod=cod) 
         self.convex = convex
-        self.match_stack = [initial_match]
+
+        if initial_match.map_scalars():
+            self.match_stack = [initial_match]
+        else:
+            self.match_stack = []
 
     def __iter__(self) -> Iterator:
         return self
 
     def __next__(self) -> Match:
         while len(self.match_stack) > 0:
             m = self.match_stack.pop()
```

### Comparing `chyp-0.3/chyp/parser.py` & `chyp-0.3.1/chyp/parser.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/rewrite.py` & `chyp-0.3.1/chyp/rewrite.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/rule.py` & `chyp-0.3.1/chyp/rule.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/scraps.py` & `chyp-0.3.1/chyp/scraps.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3/chyp/state.py` & `chyp-0.3.1/chyp/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         self.errors = parse_data.errors
 
         for name, (t_start, t_end, equiv, rule, lhs, rhs, lhs_match, rhs_match) in parse_data.rewrites.items():
             stub = not (':' in name)
             self.rewrites[name] = RewriteState((t_start, t_end), equiv, rule, lhs, rhs, lhs_match, rhs_match, stub)
 
     def part_with_index_at(self, pos: int) -> Optional[Tuple[int, Tuple[int,int,str,str]]]:
-        p0 = None
+        p0 = (0, self.parts[0]) if len(self.parts) >= 1 else None
         for (i,p) in enumerate(self.parts):
             if p[0] <= pos:
                 p0 = (i,p)
                 if p[1] >= pos:
                     return (i,p)
         return p0
```

### Comparing `chyp-0.3/chyp/term.py` & `chyp-0.3.1/chyp/term.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,24 @@
 
     v_layers = []
     e_layers = []
 
     v_pos = dict()
     e_pos = dict()
     v_layer = []
+
+    outputs = set(g.outputs())
     for i,v in enumerate(g.inputs()):
+        if v in outputs: g.insert_id_after(v)
         v_layer.append(v)
         v_pos[v] = i
-    edges = set(g.edges())
-    new_ids = set()
     
+    new_ids = set()
+    edges = set(g.edges())
+
     while len(edges) > 0:
         v_layers.append(v_layer)
 
         ready = set()
         for e in edges:
             if all(v in v_pos for v in g.source(e)):
                 ready.add(e)
```

### Comparing `chyp-0.3/chyp.egg-info/PKG-INFO` & `chyp-0.3.1/chyp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.3
+Version: 0.3.1
 Summary: An interactive theorem prover for monoidal categories
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chyp-0.3/chyp.egg-info/SOURCES.txt` & `chyp-0.3.1/chyp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chyp-0.3/setup.py` & `chyp-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 
 data_files = []
 
 setuptools.setup(
     name="chyp",
-    version="0.3",
+    version="0.3.1",
     author="Aleks Kissinger",
     author_email="aleks0@gmail.com",
     description="An interactive theorem prover for monoidal categories",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akissinger/chyp",
     project_urls={
```

