# Comparing `tmp/gotify_handler-1.0.2.tar.gz` & `tmp/gotify_handler-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotify_handler-1.0.2.tar", last modified: Mon Dec  5 03:20:29 2022, max compression
+gzip compressed data, was "gotify_handler-1.0.3.tar", last modified: Thu May 11 20:29:52 2023, max compression
```

## Comparing `gotify_handler-1.0.2.tar` & `gotify_handler-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2022-12-05 03:20:29.521971 gotify_handler-1.0.2/
--rw-r--r--   0 scott     (1000) scott     (1000)     1069 2022-05-25 20:27:36.000000 gotify_handler-1.0.2/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2814 2022-12-05 03:20:29.521971 gotify_handler-1.0.2/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)     1103 2022-12-05 03:19:22.000000 gotify_handler-1.0.2/README.md
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2022-12-05 03:20:29.521971 gotify_handler-1.0.2/gotify_handler/
--rw-r--r--   0 scott     (1000) scott     (1000)      154 2022-05-25 20:27:36.000000 gotify_handler-1.0.2/gotify_handler/__init__.py
--rw-r--r--   0 scott     (1000) scott     (1000)     1991 2022-12-05 00:15:54.000000 gotify_handler-1.0.2/gotify_handler/gotify_handler.py
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2022-12-05 03:20:29.521971 gotify_handler-1.0.2/gotify_handler.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2814 2022-12-05 03:20:29.000000 gotify_handler-1.0.2/gotify_handler.egg-info/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)      281 2022-12-05 03:20:29.000000 gotify_handler-1.0.2/gotify_handler.egg-info/SOURCES.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2022-12-05 03:20:29.000000 gotify_handler-1.0.2/gotify_handler.egg-info/dependency_links.txt
--rw-r--r--   0 scott     (1000) scott     (1000)       14 2022-12-05 03:20:29.000000 gotify_handler-1.0.2/gotify_handler.egg-info/requires.txt
--rw-r--r--   0 scott     (1000) scott     (1000)       15 2022-12-05 03:20:29.000000 gotify_handler-1.0.2/gotify_handler.egg-info/top_level.txt
--rw-r--r--   0 scott     (1000) scott     (1000)      517 2022-12-05 00:16:27.000000 gotify_handler-1.0.2/pyproject.toml
--rw-r--r--   0 scott     (1000) scott     (1000)       38 2022-12-05 03:20:29.521971 gotify_handler-1.0.2/setup.cfg
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-11 20:29:52.968071 gotify_handler-1.0.3/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1069 2022-05-25 20:27:36.000000 gotify_handler-1.0.3/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2816 2023-05-11 20:29:52.968071 gotify_handler-1.0.3/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)     1103 2022-12-05 03:19:22.000000 gotify_handler-1.0.3/README.md
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-11 20:29:52.968071 gotify_handler-1.0.3/gotify_handler/
+-rw-r--r--   0 scott     (1000) scott     (1000)      154 2022-05-25 20:27:36.000000 gotify_handler-1.0.3/gotify_handler/__init__.py
+-rw-r--r--   0 scott     (1000) scott     (1000)     2000 2023-05-11 20:27:34.000000 gotify_handler-1.0.3/gotify_handler/gotify_handler.py
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-11 20:29:52.968071 gotify_handler-1.0.3/gotify_handler.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2816 2023-05-11 20:29:52.000000 gotify_handler-1.0.3/gotify_handler.egg-info/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)      281 2023-05-11 20:29:52.000000 gotify_handler-1.0.3/gotify_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-11 20:29:52.000000 gotify_handler-1.0.3/gotify_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)       14 2023-05-11 20:29:52.000000 gotify_handler-1.0.3/gotify_handler.egg-info/requires.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)       15 2023-05-11 20:29:52.000000 gotify_handler-1.0.3/gotify_handler.egg-info/top_level.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)      519 2023-05-11 20:27:54.000000 gotify_handler-1.0.3/pyproject.toml
+-rw-r--r--   0 scott     (1000) scott     (1000)       38 2023-05-11 20:29:52.968071 gotify_handler-1.0.3/setup.cfg
```

### Comparing `gotify_handler-1.0.2/LICENSE` & `gotify_handler-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gotify_handler-1.0.2/PKG-INFO` & `gotify_handler-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gotify_handler
-Version: 1.0.2
+Version: 1.0.3
 Summary: An extremely simple logging handler for relaying log events to gotify
-Author-email: Scott Conway <me@conway.scot>
+Author-email: Scott Conway <pypi@conway.scot>
 License: MIT License
         
         Copyright (c) 2022 Scott Conway
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `gotify_handler-1.0.2/README.md` & `gotify_handler-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gotify_handler-1.0.2/gotify_handler/gotify_handler.py` & `gotify_handler-1.0.3/gotify_handler/gotify_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 priority = 0  # silent
             else:
                 priority = 5  # causes an alert
 
             res = self.gotify_session.post(
                 f"{self.server_url}/message",
                 json={
-                    "message": record.msg,
+                    "message": record.getMessage(),
                     "title": f"{record.levelname}:{record.name}",
                     "priority": priority,
                     "extras": self.extras,
                 },
             )
             res.raise_for_status()
```

### Comparing `gotify_handler-1.0.2/gotify_handler.egg-info/PKG-INFO` & `gotify_handler-1.0.3/gotify_handler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gotify-handler
-Version: 1.0.2
+Version: 1.0.3
 Summary: An extremely simple logging handler for relaying log events to gotify
-Author-email: Scott Conway <me@conway.scot>
+Author-email: Scott Conway <pypi@conway.scot>
 License: MIT License
         
         Copyright (c) 2022 Scott Conway
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `gotify_handler-1.0.2/pyproject.toml` & `gotify_handler-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "gotify_handler"
 description = "An extremely simple logging handler for relaying log events to gotify"
-version = "1.0.2"
-authors = [{name = "Scott Conway", email = "me@conway.scot"}]
+version = "1.0.3"
+authors = [{name = "Scott Conway", email = "pypi@conway.scot"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only"
 ]
```

