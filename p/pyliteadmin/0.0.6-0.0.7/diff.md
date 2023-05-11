# Comparing `tmp/pyliteadmin-0.0.6.tar.gz` & `tmp/pyliteadmin-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyliteadmin-0.0.6.tar", last modified: Thu May 11 18:19:32 2023, max compression
+gzip compressed data, was "pyliteadmin-0.0.7.tar", last modified: Thu May 11 18:25:04 2023, max compression
```

## Comparing `pyliteadmin-0.0.6.tar` & `pyliteadmin-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 18:19:32.174721 pyliteadmin-0.0.6/
--rw-rw-rw-   0        0        0    11545 2023-05-04 19:06:23.000000 pyliteadmin-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2199 2023-05-11 18:19:32.173720 pyliteadmin-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1648 2023-05-04 19:06:17.000000 pyliteadmin-0.0.6/README.md
--rw-rw-rw-   0        0        0      730 2023-05-11 18:19:14.000000 pyliteadmin-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 18:19:32.174721 pyliteadmin-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 18:19:32.153717 pyliteadmin-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 18:19:32.160718 pyliteadmin-0.0.6/src/pyliteadmin/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:16:00.000000 pyliteadmin-0.0.6/src/pyliteadmin/__init__.py
--rw-rw-rw-   0        0        0     3937 2023-05-04 17:37:19.000000 pyliteadmin-0.0.6/src/pyliteadmin/db.py
--rw-rw-rw-   0        0        0    16751 2023-05-11 18:14:51.000000 pyliteadmin-0.0.6/src/pyliteadmin/pyliteadmin.py
-drwxrwxrwx   0        0        0        0 2023-05-11 18:19:32.172721 pyliteadmin-0.0.6/src/pyliteadmin.egg-info/
--rw-rw-rw-   0        0        0     2199 2023-05-11 18:19:32.000000 pyliteadmin-0.0.6/src/pyliteadmin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-05-11 18:19:32.000000 pyliteadmin-0.0.6/src/pyliteadmin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 18:19:32.000000 pyliteadmin-0.0.6/src/pyliteadmin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-11 18:19:32.000000 pyliteadmin-0.0.6/src/pyliteadmin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2023-05-11 18:19:32.000000 pyliteadmin-0.0.6/src/pyliteadmin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 18:25:04.533472 pyliteadmin-0.0.7/
+-rw-rw-rw-   0        0        0    11545 2023-05-04 19:06:23.000000 pyliteadmin-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2199 2023-05-11 18:25:04.533472 pyliteadmin-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1648 2023-05-04 19:06:17.000000 pyliteadmin-0.0.7/README.md
+-rw-rw-rw-   0        0        0      752 2023-05-11 18:24:37.000000 pyliteadmin-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 18:25:04.533472 pyliteadmin-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 18:25:04.503463 pyliteadmin-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 18:25:04.515467 pyliteadmin-0.0.7/src/pyliteadmin/
+-rw-rw-rw-   0        0        0        0 2023-05-11 17:16:00.000000 pyliteadmin-0.0.7/src/pyliteadmin/__init__.py
+-rw-rw-rw-   0        0        0     3937 2023-05-04 17:37:19.000000 pyliteadmin-0.0.7/src/pyliteadmin/db.py
+-rw-rw-rw-   0        0        0    16758 2023-05-11 18:24:38.000000 pyliteadmin-0.0.7/src/pyliteadmin/pyliteadmin.py
+drwxrwxrwx   0        0        0        0 2023-05-11 18:25:04.531471 pyliteadmin-0.0.7/src/pyliteadmin.egg-info/
+-rw-rw-rw-   0        0        0     2199 2023-05-11 18:25:04.000000 pyliteadmin-0.0.7/src/pyliteadmin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-05-11 18:25:04.000000 pyliteadmin-0.0.7/src/pyliteadmin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 18:25:04.000000 pyliteadmin-0.0.7/src/pyliteadmin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-11 18:25:04.000000 pyliteadmin-0.0.7/src/pyliteadmin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-11 18:25:04.000000 pyliteadmin-0.0.7/src/pyliteadmin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 18:25:04.000000 pyliteadmin-0.0.7/src/pyliteadmin.egg-info/top_level.txt
```

### Comparing `pyliteadmin-0.0.6/LICENSE` & `pyliteadmin-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyliteadmin-0.0.6/PKG-INFO` & `pyliteadmin-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyliteadmin
-Version: 0.0.6
+Version: 0.0.7
 Summary: A TUI for viewing and CRUDing sqlite databases.
 Author-email: Brandon Demelo <brandon@brandondemelo.com>
 Project-URL: Homepage, https://github.com/The-Bush/pyliteadmin
 Project-URL: Bug Tracker, https://github.com/The-Bush/pyliteadmin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyliteadmin-0.0.6/README.md` & `pyliteadmin-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyliteadmin-0.0.6/pyproject.toml` & `pyliteadmin-0.0.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [build-system]
 requires = [
     "setuptools",
     "wheel",
-    "textual"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyliteadmin"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Brandon Demelo", email="brandon@brandondemelo.com" },
 ]
 description = "A TUI for viewing and CRUDing sqlite databases."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "textual",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/The-Bush/pyliteadmin"
 "Bug Tracker" = "https://github.com/The-Bush/pyliteadmin/issues"
 
 [project.scripts]
 pyliteadmin = "pyliteadmin.pyliteadmin:main"
```

### Comparing `pyliteadmin-0.0.6/src/pyliteadmin/db.py` & `pyliteadmin-0.0.7/src/pyliteadmin/db.py`

 * *Files identical despite different names*

### Comparing `pyliteadmin-0.0.6/src/pyliteadmin/pyliteadmin.py` & `pyliteadmin-0.0.7/src/pyliteadmin/pyliteadmin.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ListView,
     ListItem,
     Label,
     OptionList,
     Input,
 )
 from textual.screen import ModalScreen
-import db
+from . import db
 
 # Set the table cursor to a cycle of three different cursor types
 cursors = cycle(["row", "cell"])
 
 # Dict of keys and their related row values for currently viewed table
 keys: dict[int, list] = {}
 # Dict of columns and  their related column values for currently viewed table
```

### Comparing `pyliteadmin-0.0.6/src/pyliteadmin.egg-info/PKG-INFO` & `pyliteadmin-0.0.7/src/pyliteadmin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyliteadmin
-Version: 0.0.6
+Version: 0.0.7
 Summary: A TUI for viewing and CRUDing sqlite databases.
 Author-email: Brandon Demelo <brandon@brandondemelo.com>
 Project-URL: Homepage, https://github.com/The-Bush/pyliteadmin
 Project-URL: Bug Tracker, https://github.com/The-Bush/pyliteadmin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

