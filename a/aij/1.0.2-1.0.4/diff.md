# Comparing `tmp/aij-1.0.2.tar.gz` & `tmp/aij-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.0.2.tar", last modified: Wed May 10 20:20:52 2023, max compression
+gzip compressed data, was "aij-1.0.4.tar", last modified: Wed May 10 22:21:55 2023, max compression
```

## Comparing `aij-1.0.2.tar` & `aij-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 20:20:52.000000 aij-1.0.2/
--rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     4137 2023-05-10 20:20:54.000000 aij-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-05 12:30:36.000000 aij-1.0.2/README.md
--rw-rw-rw-   0        0        0     6307 2023-05-10 20:20:40.000000 aij-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 20:20:54.000000 aij-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 20:20:52.000000 aij-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 20:20:52.000000 aij-1.0.2/src/aij.egg-info/
--rw-rw-rw-   0        0        0     4137 2023-05-10 20:20:52.000000 aij-1.0.2/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-05-10 20:20:52.000000 aij-1.0.2/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 20:20:52.000000 aij-1.0.2/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-05-10 20:20:52.000000 aij-1.0.2/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      175 2023-05-10 20:20:52.000000 aij-1.0.2/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-05-10 20:20:52.000000 aij-1.0.2/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 20:20:52.000000 aij-1.0.2/src/custom/
--rw-rw-rw-   0        0        0      440 2023-05-10 19:37:52.000000 aij-1.0.2/src/custom/__init__.py
--rw-rw-rw-   0        0        0     4531 2023-05-10 18:27:28.000000 aij-1.0.2/src/custom/generator.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:20:52.000000 aij-1.0.2/src/intro/
--rw-rw-rw-   0        0        0      440 2023-05-07 13:08:58.000000 aij-1.0.2/src/intro/__init__.py
--rw-rw-rw-   0        0        0     4524 2023-05-07 13:07:50.000000 aij-1.0.2/src/intro/intro.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:20:52.000000 aij-1.0.2/src/news/
--rw-rw-rw-   0        0        0      567 2023-05-07 13:07:50.000000 aij-1.0.2/src/news/__init__.py
--rw-rw-rw-   0        0        0     4492 2023-05-07 13:16:16.000000 aij-1.0.2/src/news/core.py
--rw-rw-rw-   0        0        0     1407 2023-05-07 13:18:00.000000 aij-1.0.2/src/news/publisher.py
--rw-rw-rw-   0        0        0     1196 2023-05-05 12:37:32.000000 aij-1.0.2/src/news/subscriber.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:20:52.000000 aij-1.0.2/src/setup/
--rw-rw-rw-   0        0        0     1162 2023-05-07 21:18:54.000000 aij-1.0.2/src/setup/__init__.py
--rw-rw-rw-   0        0        0     3739 2023-05-07 21:18:28.000000 aij-1.0.2/src/setup/install.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:20:52.000000 aij-1.0.2/src/webcam/
--rw-rw-rw-   0        0        0    17500 2023-05-06 19:32:44.000000 aij-1.0.2/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/
+-rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4137 2023-05-10 22:21:56.000000 aij-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-05-05 12:30:36.000000 aij-1.0.4/README.md
+-rw-rw-rw-   0        0        0     6343 2023-05-10 22:21:42.000000 aij-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 22:21:56.000000 aij-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/
+-rw-rw-rw-   0        0        0     4137 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      197 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-05-10 22:21:56.000000 aij-1.0.4/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/custom/
+-rw-rw-rw-   0        0        0      440 2023-05-10 19:37:52.000000 aij-1.0.4/src/custom/__init__.py
+-rw-rw-rw-   0        0        0     4531 2023-05-10 18:27:28.000000 aij-1.0.4/src/custom/generator.py
+drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/intro/
+-rw-rw-rw-   0        0        0      440 2023-05-07 13:08:58.000000 aij-1.0.4/src/intro/__init__.py
+-rw-rw-rw-   0        0        0     4524 2023-05-07 13:07:50.000000 aij-1.0.4/src/intro/intro.py
+drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/news/
+-rw-rw-rw-   0        0        0      567 2023-05-07 13:07:50.000000 aij-1.0.4/src/news/__init__.py
+-rw-rw-rw-   0        0        0     4492 2023-05-07 13:16:16.000000 aij-1.0.4/src/news/core.py
+-rw-rw-rw-   0        0        0     1407 2023-05-07 13:18:00.000000 aij-1.0.4/src/news/publisher.py
+-rw-rw-rw-   0        0        0     1196 2023-05-05 12:37:32.000000 aij-1.0.4/src/news/subscriber.py
+drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/setup/
+-rw-rw-rw-   0        0        0     1162 2023-05-07 21:18:54.000000 aij-1.0.4/src/setup/__init__.py
+-rw-rw-rw-   0        0        0     3739 2023-05-07 21:18:28.000000 aij-1.0.4/src/setup/install.py
+drwxrwxrwx   0        0        0        0 2023-05-10 22:21:56.000000 aij-1.0.4/src/webcam/
+-rw-rw-rw-   0        0        0    17500 2023-05-06 19:32:44.000000 aij-1.0.4/src/webcam/__init__.py
```

### Comparing `aij-1.0.2/LICENSE.txt` & `aij-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.0.2/PKG-INFO` & `aij-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.0.2
+Version: 1.0.4
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.0.2/README.md` & `aij-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.0.2/pyproject.toml` & `aij-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.2"
+version = "1.0.4"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -108,15 +108,17 @@
     "pytest-cov",
     "opencv-python",
     "mediapipe",
     "pandas",
     "gtts",
     "pygame",
     "cairosvg",
-    "pika"
+    "pika",
+    "newsapi-python",
+    "openai"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
```

### Comparing `aij-1.0.2/src/aij.egg-info/PKG-INFO` & `aij-1.0.4/src/aij.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.0.2
+Version: 1.0.4
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.0.2/src/custom/generator.py` & `aij-1.0.4/src/custom/generator.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.2/src/intro/intro.py` & `aij-1.0.4/src/intro/intro.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.2/src/news/__init__.py` & `aij-1.0.4/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.2/src/news/core.py` & `aij-1.0.4/src/news/core.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.2/src/news/publisher.py` & `aij-1.0.4/src/news/publisher.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.2/src/news/subscriber.py` & `aij-1.0.4/src/news/subscriber.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.2/src/setup/__init__.py` & `aij-1.0.4/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.2/src/setup/install.py` & `aij-1.0.4/src/setup/install.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.2/src/webcam/__init__.py` & `aij-1.0.4/src/webcam/__init__.py`

 * *Files identical despite different names*

