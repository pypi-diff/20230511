# Comparing `tmp/replit-3.2.7.tar.gz` & `tmp/replit-3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit-3.2.7.tar", max compression
+gzip compressed data, was "replit-3.2.8.tar", max compression
```

## Comparing `replit-3.2.7.tar` & `replit-3.2.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      720 2023-04-07 15:30:56.391990 replit-3.2.7/LICENSE
--rw-r--r--   0        0        0      673 2023-04-07 15:30:56.391990 replit-3.2.7/README.md
--rw-r--r--   0        0        0     1272 2023-04-10 20:20:22.312648 replit-3.2.7/pyproject.toml
--rw-r--r--   0        0        0      410 2023-04-07 15:30:56.397991 replit-3.2.7/src/replit/__init__.py
--rw-r--r--   0        0        0     2868 2023-04-07 15:30:56.397991 replit-3.2.7/src/replit/__main__.py
--rw-r--r--   0        0        0      171 2023-04-07 15:30:56.397991 replit-3.2.7/src/replit/audio/Makefile
--rw-r--r--   0        0        0    13226 2023-04-07 15:30:56.397991 replit-3.2.7/src/replit/audio/__init__.py
--rw-r--r--   0        0        0     1848 2023-04-07 15:30:56.397991 replit-3.2.7/src/replit/audio/test.py
--rw-r--r--   0        0        0     3687 2023-04-07 15:30:56.397991 replit-3.2.7/src/replit/audio/types.py
--rw-r--r--   0        0        0      426 2023-04-07 15:30:56.397991 replit-3.2.7/src/replit/database/__init__.py
--rw-r--r--   0        0        0    18106 2023-04-10 18:56:39.411937 replit-3.2.7/src/replit/database/database.py
--rw-r--r--   0        0        0      467 2023-04-10 20:18:06.370986 replit-3.2.7/src/replit/database/default_db.py
--rw-r--r--   0        0        0     2239 2023-04-07 15:30:56.397991 replit-3.2.7/src/replit/database/server.py
--rw-r--r--   0        0        0       33 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/goval/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/goval/api/__init__.py
--rw-r--r--   0        0        0     5198 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/goval/api/client_pb2.py
--rw-r--r--   0        0        0        0 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/goval/api/features/__init__.py
--rw-r--r--   0        0        0     1516 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/goval/api/features/features_pb2.py
--rw-r--r--   0        0        0        0 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/goval/api/repl/__init__.py
--rw-r--r--   0        0        0     3031 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/goval/api/repl/repl_pb2.py
--rw-r--r--   0        0        0     3563 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/goval/api/signing_pb2.py
--rw-r--r--   0        0        0      135 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/identity/__init__.py
--rw-r--r--   0        0        0      159 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/identity/exceptions.py
--rw-r--r--   0        0        0     9156 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/identity/verify.py
--rw-r--r--   0        0        0     2466 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/info.py
--rw-r--r--   0        0        0      352 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/web/__init__.py
--rw-r--r--   0        0        0     2589 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/web/app.py
--rw-r--r--   0        0        0     3329 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/web/user.py
--rw-r--r--   0        0        0     8552 2023-04-07 15:30:56.398991 replit-3.2.7/src/replit/web/utils.py
--rw-r--r--   0        0        0     1843 2023-04-10 20:20:25.503887 replit-3.2.7/setup.py
--rw-r--r--   0        0        0     1611 2023-04-10 20:20:25.504251 replit-3.2.7/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-05-10 13:20:25.042796 replit-3.2.8/LICENSE
+-rw-r--r--   0        0        0      673 2023-05-10 13:20:25.042796 replit-3.2.8/README.md
+-rw-r--r--   0        0        0     1272 2023-05-10 20:30:28.540145 replit-3.2.8/pyproject.toml
+-rw-r--r--   0        0        0      410 2023-05-10 13:20:25.050797 replit-3.2.8/src/replit/__init__.py
+-rw-r--r--   0        0        0     2868 2023-05-10 13:20:25.050797 replit-3.2.8/src/replit/__main__.py
+-rw-r--r--   0        0        0      171 2023-05-10 13:20:25.050797 replit-3.2.8/src/replit/audio/Makefile
+-rw-r--r--   0        0        0    13226 2023-05-10 13:20:25.050797 replit-3.2.8/src/replit/audio/__init__.py
+-rw-r--r--   0        0        0     1848 2023-05-10 13:20:25.050797 replit-3.2.8/src/replit/audio/test.py
+-rw-r--r--   0        0        0     3687 2023-05-10 13:20:25.050797 replit-3.2.8/src/replit/audio/types.py
+-rw-r--r--   0        0        0      426 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/database/__init__.py
+-rw-r--r--   0        0        0    18096 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/database/database.py
+-rw-r--r--   0        0        0      830 2023-05-10 15:08:20.076504 replit-3.2.8/src/replit/database/default_db.py
+-rw-r--r--   0        0        0     2239 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/database/server.py
+-rw-r--r--   0        0        0       33 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/goval/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/goval/api/__init__.py
+-rw-r--r--   0        0        0     5198 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/goval/api/client_pb2.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/goval/api/features/__init__.py
+-rw-r--r--   0        0        0     1516 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/goval/api/features/features_pb2.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/goval/api/repl/__init__.py
+-rw-r--r--   0        0        0     3031 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/goval/api/repl/repl_pb2.py
+-rw-r--r--   0        0        0     3563 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/goval/api/signing_pb2.py
+-rw-r--r--   0        0        0      135 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/identity/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/identity/exceptions.py
+-rw-r--r--   0        0        0     9156 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/identity/verify.py
+-rw-r--r--   0        0        0     2466 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/info.py
+-rw-r--r--   0        0        0      352 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/web/__init__.py
+-rw-r--r--   0        0        0     2589 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/web/app.py
+-rw-r--r--   0        0        0     3329 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/web/user.py
+-rw-r--r--   0        0        0     8552 2023-05-10 13:20:25.054797 replit-3.2.8/src/replit/web/utils.py
+-rw-r--r--   0        0        0     1843 2023-05-10 20:31:10.372317 replit-3.2.8/setup.py
+-rw-r--r--   0        0        0     1611 2023-05-10 20:31:10.372713 replit-3.2.8/PKG-INFO
```

### Comparing `replit-3.2.7/LICENSE` & `replit-3.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/README.md` & `replit-3.2.8/README.md`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/pyproject.toml` & `replit-3.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit"
-version = "3.2.7"
+version = "3.2.8"
 description = "A library for interacting with features of repl.it"
 authors = ["Repl.it <contact@repl.it>", "mat <pypi@matdoes.dev>", "kennethreitz <me@kennethreitz.org>", "Scoder12 <pypi@scoder12.ml>", "AllAwesome497", ]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/replit/replit-py"
 homepage = "https://github.com/replit/replit-py"
 documentation = "https://replit-py.readthedocs.org/"
```

### Comparing `replit-3.2.7/src/replit/__main__.py` & `replit-3.2.8/src/replit/__main__.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/audio/__init__.py` & `replit-3.2.8/src/replit/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/audio/test.py` & `replit-3.2.8/src/replit/audio/test.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/audio/types.py` & `replit-3.2.8/src/replit/audio/types.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/database/database.py` & `replit-3.2.8/src/replit/database/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Async and dict-like interfaces for interacting with Repl.it Database."""
 
 from collections import abc
 import json
-import os
 from typing import (
     AbstractSet,
     Any,
     Callable,
     Dict,
     Iterator,
     List,
```

### Comparing `replit-3.2.7/src/replit/database/server.py` & `replit-3.2.8/src/replit/database/server.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/goval/api/client_pb2.py` & `replit-3.2.8/src/replit/goval/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/goval/api/features/features_pb2.py` & `replit-3.2.8/src/replit/goval/api/features/features_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/goval/api/repl/repl_pb2.py` & `replit-3.2.8/src/replit/goval/api/repl/repl_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/goval/api/signing_pb2.py` & `replit-3.2.8/src/replit/goval/api/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/identity/verify.py` & `replit-3.2.8/src/replit/identity/verify.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/info.py` & `replit-3.2.8/src/replit/info.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/web/app.py` & `replit-3.2.8/src/replit/web/app.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/web/user.py` & `replit-3.2.8/src/replit/web/user.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/src/replit/web/utils.py` & `replit-3.2.8/src/replit/web/utils.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.7/setup.py` & `replit-3.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'typing_extensions>=3.7.4,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['replit = replit.__main__:cli']}
 
 setup_kwargs = {
     'name': 'replit',
-    'version': '3.2.7',
+    'version': '3.2.8',
     'description': 'A library for interacting with features of repl.it',
     'long_description': '### `>>> import replit`\n\n![compute](https://github.com/kennethreitz42/replit-py/blob/kr-cleanup/ext/readme.gif?raw=true)\n\nThis repository is the home for the `replit` Python package, which provides:\n\n- A fully-featured database client for [Replit DB](https://docs.repl.it/misc/database).\n- A Flask–based application framework for accelerating development on the platform.\n- Replit user profile metadata retrieval (more coming here!).\n- A simple audio library that can play tones and audio files!\n\n### Open Source License\n\nThis library is licensed under the [ISC License](https://en.wikipedia.org/wiki/ISC_license) and is free for you to use, change, or even profit from!\n',
     'author': 'Repl.it',
     'author_email': 'contact@repl.it',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/replit/replit-py',
```

### Comparing `replit-3.2.7/PKG-INFO` & `replit-3.2.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit
-Version: 3.2.7
+Version: 3.2.8
 Summary: A library for interacting with features of repl.it
 Home-page: https://github.com/replit/replit-py
 License: ISC
 Author: Repl.it
 Author-email: contact@repl.it
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
```

