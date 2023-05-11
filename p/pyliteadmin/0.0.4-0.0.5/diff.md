# Comparing `tmp/pyliteadmin-0.0.4.tar.gz` & `tmp/pyliteadmin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyliteadmin-0.0.4.tar", last modified: Thu May 11 18:05:18 2023, max compression
+gzip compressed data, was "pyliteadmin-0.0.5.tar", last modified: Thu May 11 18:15:17 2023, max compression
```

## Comparing `pyliteadmin-0.0.4.tar` & `pyliteadmin-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 18:05:18.203416 pyliteadmin-0.0.4/
--rw-rw-rw-   0        0        0    11545 2023-05-04 19:06:23.000000 pyliteadmin-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2199 2023-05-11 18:05:18.202417 pyliteadmin-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1648 2023-05-04 19:06:17.000000 pyliteadmin-0.0.4/README.md
--rw-rw-rw-   0        0        0      702 2023-05-11 18:04:59.000000 pyliteadmin-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 18:05:18.204416 pyliteadmin-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 18:05:18.175906 pyliteadmin-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 18:05:18.188413 pyliteadmin-0.0.4/src/pyliteadmin/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:16:00.000000 pyliteadmin-0.0.4/src/pyliteadmin/__init__.py
--rw-rw-rw-   0        0        0     3937 2023-05-04 17:37:19.000000 pyliteadmin-0.0.4/src/pyliteadmin/db.py
--rw-rw-rw-   0        0        0    16856 2023-05-11 18:05:01.000000 pyliteadmin-0.0.4/src/pyliteadmin/pyliteadmin.py
-drwxrwxrwx   0        0        0        0 2023-05-11 18:05:18.201415 pyliteadmin-0.0.4/src/pyliteadmin.egg-info/
--rw-rw-rw-   0        0        0     2199 2023-05-11 18:05:18.000000 pyliteadmin-0.0.4/src/pyliteadmin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-05-11 18:05:18.000000 pyliteadmin-0.0.4/src/pyliteadmin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 18:05:18.000000 pyliteadmin-0.0.4/src/pyliteadmin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-11 18:05:18.000000 pyliteadmin-0.0.4/src/pyliteadmin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2023-05-11 18:05:18.000000 pyliteadmin-0.0.4/src/pyliteadmin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 18:15:17.922372 pyliteadmin-0.0.5/
+-rw-rw-rw-   0        0        0    11545 2023-05-04 19:06:23.000000 pyliteadmin-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2199 2023-05-11 18:15:17.922372 pyliteadmin-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1648 2023-05-04 19:06:17.000000 pyliteadmin-0.0.5/README.md
+-rw-rw-rw-   0        0        0      714 2023-05-11 18:14:50.000000 pyliteadmin-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 18:15:17.923373 pyliteadmin-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 18:15:17.889367 pyliteadmin-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 18:15:17.905369 pyliteadmin-0.0.5/src/pyliteadmin/
+-rw-rw-rw-   0        0        0        0 2023-05-11 17:16:00.000000 pyliteadmin-0.0.5/src/pyliteadmin/__init__.py
+-rw-rw-rw-   0        0        0     3937 2023-05-04 17:37:19.000000 pyliteadmin-0.0.5/src/pyliteadmin/db.py
+-rw-rw-rw-   0        0        0    16751 2023-05-11 18:14:51.000000 pyliteadmin-0.0.5/src/pyliteadmin/pyliteadmin.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:15:17.921372 pyliteadmin-0.0.5/src/pyliteadmin.egg-info/
+-rw-rw-rw-   0        0        0     2199 2023-05-11 18:15:17.000000 pyliteadmin-0.0.5/src/pyliteadmin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-05-11 18:15:17.000000 pyliteadmin-0.0.5/src/pyliteadmin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 18:15:17.000000 pyliteadmin-0.0.5/src/pyliteadmin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-11 18:15:17.000000 pyliteadmin-0.0.5/src/pyliteadmin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 18:15:17.000000 pyliteadmin-0.0.5/src/pyliteadmin.egg-info/top_level.txt
```

### Comparing `pyliteadmin-0.0.4/LICENSE` & `pyliteadmin-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyliteadmin-0.0.4/PKG-INFO` & `pyliteadmin-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyliteadmin
-Version: 0.0.4
+Version: 0.0.5
 Summary: A TUI for viewing and CRUDing sqlite databases.
 Author-email: Brandon Demelo <brandon@brandondemelo.com>
 Project-URL: Homepage, https://github.com/The-Bush/pyliteadmin
 Project-URL: Bug Tracker, https://github.com/The-Bush/pyliteadmin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyliteadmin-0.0.4/README.md` & `pyliteadmin-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyliteadmin-0.0.4/pyproject.toml` & `pyliteadmin-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyliteadmin"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Brandon Demelo", email="brandon@brandondemelo.com" },
 ]
 description = "A TUI for viewing and CRUDing sqlite databases."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -21,8 +21,8 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/The-Bush/pyliteadmin"
 "Bug Tracker" = "https://github.com/The-Bush/pyliteadmin/issues"
 
 [project.scripts]
-pyliteadmin = "pyliteadmin:main"
+pyliteadmin = "pyliteadmin.pyliteadmin:main"
```

### Comparing `pyliteadmin-0.0.4/src/pyliteadmin/db.py` & `pyliteadmin-0.0.5/src/pyliteadmin/db.py`

 * *Files identical despite different names*

### Comparing `pyliteadmin-0.0.4/src/pyliteadmin/pyliteadmin.py` & `pyliteadmin-0.0.5/src/pyliteadmin/pyliteadmin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import os
 from abc import ABC, abstractmethod
 from itertools import cycle
 from typing import Optional
 from textual.app import App, ComposeResult
 from textual.containers import Container, Grid, Horizontal
-from textual.reactive import reactive
-from textual.message import Message, MessageTarget
 from textual.widget import Widget
 from textual.widgets import (
     Button,
     Header,
     Footer,
     DataTable,
     Static,
     ListView,
     ListItem,
     Label,
     OptionList,
     Input,
 )
-from textual.screen import Screen, ModalScreen
-import sqlite3
+from textual.screen import ModalScreen
 import db
 
 # Set the table cursor to a cycle of three different cursor types
 cursors = cycle(["row", "cell"])
 
 # Dict of keys and their related row values for currently viewed table
 keys: dict[int, list] = {}
@@ -452,8 +449,10 @@
 
     def action_quit(self) -> None:
         self.exit()
 
 def main():
     app = PyLiteAdmin()
     if __name__ == "__main__":
-        app.run()
+        app.run()
+
+main()
```

### Comparing `pyliteadmin-0.0.4/src/pyliteadmin.egg-info/PKG-INFO` & `pyliteadmin-0.0.5/src/pyliteadmin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyliteadmin
-Version: 0.0.4
+Version: 0.0.5
 Summary: A TUI for viewing and CRUDing sqlite databases.
 Author-email: Brandon Demelo <brandon@brandondemelo.com>
 Project-URL: Homepage, https://github.com/The-Bush/pyliteadmin
 Project-URL: Bug Tracker, https://github.com/The-Bush/pyliteadmin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

