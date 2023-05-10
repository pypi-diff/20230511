# Comparing `tmp/verse-core-0.0.3.tar.gz` & `tmp/verse-core-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verse-core-0.0.3.tar", last modified: Wed May 10 21:50:29 2023, max compression
+gzip compressed data, was "verse-core-0.0.4.tar", last modified: Wed May 10 23:53:38 2023, max compression
```

## Comparing `verse-core-0.0.3.tar` & `verse-core-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 21:50:29.549864 verse-core-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-02-12 19:43:35.000000 verse-core-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      593 2023-05-10 21:50:29.548868 verse-core-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-26 23:13:54.000000 verse-core-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 21:50:29.520944 verse-core-0.0.3/core/
--rw-rw-rw-   0        0        0      125 2023-04-27 20:54:44.000000 verse-core-0.0.3/core/__init__.py
--rw-rw-rw-   0        0        0      162 2023-04-26 23:17:00.000000 verse-core-0.0.3/core/async_helper.py
--rw-rw-rw-   0        0        0      402 2023-04-26 23:17:08.000000 verse-core-0.0.3/core/import_helper.py
--rw-rw-rw-   0        0        0      463 2023-05-08 23:41:13.000000 verse-core-0.0.3/core/model.py
--rw-rw-rw-   0        0        0      668 2023-05-10 21:45:59.000000 verse-core-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 21:50:29.549864 verse-core-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 21:50:29.546874 verse-core-0.0.3/verse_core.egg-info/
--rw-rw-rw-   0        0        0      593 2023-05-10 21:50:29.000000 verse-core-0.0.3/verse_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-10 21:50:29.000000 verse-core-0.0.3/verse_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 21:50:29.000000 verse-core-0.0.3/verse_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 21:50:29.000000 verse-core-0.0.3/verse_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 23:53:38.705623 verse-core-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-02-12 19:43:35.000000 verse-core-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      593 2023-05-10 23:53:38.704627 verse-core-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-26 23:13:54.000000 verse-core-0.0.4/README.md
+-rw-rw-rw-   0        0        0      606 2023-05-10 23:52:32.000000 verse-core-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 23:53:38.705623 verse-core-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 23:53:38.657851 verse-core-0.0.4/verse/
+drwxrwxrwx   0        0        0        0 2023-05-10 23:53:38.684684 verse-core-0.0.4/verse/core/
+-rw-rw-rw-   0        0        0      125 2023-04-27 20:54:44.000000 verse-core-0.0.4/verse/core/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-04-26 23:17:00.000000 verse-core-0.0.4/verse/core/async_helper.py
+-rw-rw-rw-   0        0        0      402 2023-04-26 23:17:08.000000 verse-core-0.0.4/verse/core/import_helper.py
+-rw-rw-rw-   0        0        0      463 2023-05-08 23:41:13.000000 verse-core-0.0.4/verse/core/model.py
+drwxrwxrwx   0        0        0        0 2023-05-10 23:53:38.702668 verse-core-0.0.4/verse_core.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-05-10 23:53:38.000000 verse-core-0.0.4/verse_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-10 23:53:38.000000 verse-core-0.0.4/verse_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 23:53:38.000000 verse-core-0.0.4/verse_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 23:53:38.000000 verse-core-0.0.4/verse_core.egg-info/top_level.txt
```

### Comparing `verse-core-0.0.3/LICENSE` & `verse-core-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `verse-core-0.0.3/PKG-INFO` & `verse-core-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verse-core
-Version: 0.0.3
+Version: 0.0.4
 Summary: Core Verse package shared by all Verse packages
 Author-email: Rapidverse <admin@rapidverse.com>
 Project-URL: Homepage, https://github.com/rapidverse/verse
 Project-URL: Bug Tracker, https://github.com/rapidverse/verse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `verse-core-0.0.3/pyproject.toml` & `verse-core-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "verse-core"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "Rapidverse", email = "admin@rapidverse.com" }]
 description = "Core Verse package shared by all Verse packages"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 
-[tool.setuptools]
-package-dir = { "verse.core" = "core" }
-
 [project.urls]
 "Homepage" = "https://github.com/rapidverse/verse"
 "Bug Tracker" = "https://github.com/rapidverse/verse/issues"
```

### Comparing `verse-core-0.0.3/verse_core.egg-info/PKG-INFO` & `verse-core-0.0.4/verse_core.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verse-core
-Version: 0.0.3
+Version: 0.0.4
 Summary: Core Verse package shared by all Verse packages
 Author-email: Rapidverse <admin@rapidverse.com>
 Project-URL: Homepage, https://github.com/rapidverse/verse
 Project-URL: Bug Tracker, https://github.com/rapidverse/verse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

