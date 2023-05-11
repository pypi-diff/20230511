# Comparing `tmp/djungle-rulesengine-client-0.3.0.tar.gz` & `tmp/djungle-rulesengine-client-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djungle-rulesengine-client-0.3.0.tar", last modified: Tue May  9 14:06:38 2023, max compression
+gzip compressed data, was "djungle-rulesengine-client-0.3.3.tar", last modified: Thu May 11 09:45:56 2023, max compression
```

## Comparing `djungle-rulesengine-client-0.3.0.tar` & `djungle-rulesengine-client-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 14:06:38.225423 djungle-rulesengine-client-0.3.0/
--rw-r--r--   0 fabio      (501) admin       (80)     1071 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.3.0/LICENSE
--rw-r--r--   0 fabio      (501) admin       (80)     1995 2023-05-09 14:06:38.225585 djungle-rulesengine-client-0.3.0/PKG-INFO
--rw-r--r--   0 fabio      (501) admin       (80)      350 2023-05-09 14:05:15.000000 djungle-rulesengine-client-0.3.0/README.md
--rw-r--r--   0 fabio      (501) admin       (80)      259 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.3.0/pyproject.toml
--rw-r--r--   0 fabio      (501) admin       (80)      746 2023-05-09 14:06:38.226251 djungle-rulesengine-client-0.3.0/setup.cfg
--rw-r--r--   0 fabio      (501) admin       (80)       38 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.3.0/setup.py
-drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 14:06:38.220424 djungle-rulesengine-client-0.3.0/src/
-drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 14:06:38.223941 djungle-rulesengine-client-0.3.0/src/djungle_rulesengine_client.egg-info/
--rw-r--r--   0 fabio      (501) admin       (80)     1995 2023-05-09 14:06:38.000000 djungle-rulesengine-client-0.3.0/src/djungle_rulesengine_client.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) admin       (80)      448 2023-05-09 14:06:38.000000 djungle-rulesengine-client-0.3.0/src/djungle_rulesengine_client.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) admin       (80)        1 2023-05-09 14:06:38.000000 djungle-rulesengine-client-0.3.0/src/djungle_rulesengine_client.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) admin       (80)        1 2023-05-09 14:06:38.000000 djungle-rulesengine-client-0.3.0/src/djungle_rulesengine_client.egg-info/not-zip-safe
--rw-r--r--   0 fabio      (501) admin       (80)       17 2023-05-09 14:06:38.000000 djungle-rulesengine-client-0.3.0/src/djungle_rulesengine_client.egg-info/requires.txt
--rw-r--r--   0 fabio      (501) admin       (80)       12 2023-05-09 14:06:38.000000 djungle-rulesengine-client-0.3.0/src/djungle_rulesengine_client.egg-info/top_level.txt
-drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 14:06:38.224687 djungle-rulesengine-client-0.3.0/src/rulesengine/
--rw-r--r--   0 fabio      (501) admin       (80)        0 2023-05-05 13:15:54.000000 djungle-rulesengine-client-0.3.0/src/rulesengine/__init__.py
--rw-r--r--   0 fabio      (501) admin       (80)     3186 2023-05-09 14:05:23.000000 djungle-rulesengine-client-0.3.0/src/rulesengine/client.py
-drwxr-xr-x   0 fabio      (501) admin       (80)        0 2023-05-09 14:06:38.225145 djungle-rulesengine-client-0.3.0/tests/
--rw-r--r--   0 fabio      (501) admin       (80)     9251 2023-05-09 14:05:23.000000 djungle-rulesengine-client-0.3.0/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:45:56.400789 djungle-rulesengine-client-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-11 09:45:56.400789 djungle-rulesengine-client-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-11 09:45:56.400789 djungle-rulesengine-client-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:45:56.396789 djungle-rulesengine-client-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:45:56.396789 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-11 09:45:56.000000 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-11 09:45:56.000000 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:45:56.000000 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:45:56.000000 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 09:45:56.000000 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 09:45:56.000000 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:45:56.400789 djungle-rulesengine-client-0.3.3/src/rulesengine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/src/rulesengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/src/rulesengine/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:45:56.400789 djungle-rulesengine-client-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/tests/test_client.py
```

### Comparing `djungle-rulesengine-client-0.3.0/LICENSE` & `djungle-rulesengine-client-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `djungle-rulesengine-client-0.3.0/PKG-INFO` & `djungle-rulesengine-client-0.3.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djungle-rulesengine-client
-Version: 0.3.0
+Version: 0.3.3
 Summary: A client to Djungle Studio rulesengine API
 Home-page: https://github.com/djungle-io/djungle-rulesengine-client
 Author: Djungle s.r.l.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,14 +23,35 @@
 simply run the command `tox` in the root of the repository.
 
 ## Release
 This project uses `tox` to release a version to PyPI.
 Run `tox -e release -- <env>`, where `<env>` is an index identifier in
 your `~/.pypirc` file.
 
+Alternatively, push a tag to the `main` branch to make a release
+using GitHub Actions.
+
+## Usage examples
+```python
+from rulesengine.client import EngineClient
+
+engine = EngineClient(base_url="https://example.com", token="abcde")
+
+# To push an action to the engine:
+engine.push_action(subject_id="sys-1", action="my-action", payload={"key": "value"})
+
+# To get a pluggable prop from the engine
+prop_value = engine.get_pluggable_props(subject_id="sys-1", props="my-prop")
+
+# To make a "direct" call to the engine
+return_value = engine.direct_post(
+    subject_id="sys-1", path="/my/path/", params={"key": "value"}, data={"my": "payload"}
+)
+```
+
 MIT License
 
 Copyright (c) 2023 Djungle s.r.l.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
```

### Comparing `djungle-rulesengine-client-0.3.0/setup.cfg` & `djungle-rulesengine-client-0.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djungle-rulesengine-client
-version = 0.3.0
+version = 0.3.3
 description = A client to Djungle Studio rulesengine API
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 author = Djungle s.r.l.
 url = https://github.com/djungle-io/djungle-rulesengine-client
```

### Comparing `djungle-rulesengine-client-0.3.0/src/djungle_rulesengine_client.egg-info/PKG-INFO` & `djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djungle-rulesengine-client
-Version: 0.3.0
+Version: 0.3.3
 Summary: A client to Djungle Studio rulesengine API
 Home-page: https://github.com/djungle-io/djungle-rulesengine-client
 Author: Djungle s.r.l.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,14 +23,35 @@
 simply run the command `tox` in the root of the repository.
 
 ## Release
 This project uses `tox` to release a version to PyPI.
 Run `tox -e release -- <env>`, where `<env>` is an index identifier in
 your `~/.pypirc` file.
 
+Alternatively, push a tag to the `main` branch to make a release
+using GitHub Actions.
+
+## Usage examples
+```python
+from rulesengine.client import EngineClient
+
+engine = EngineClient(base_url="https://example.com", token="abcde")
+
+# To push an action to the engine:
+engine.push_action(subject_id="sys-1", action="my-action", payload={"key": "value"})
+
+# To get a pluggable prop from the engine
+prop_value = engine.get_pluggable_props(subject_id="sys-1", props="my-prop")
+
+# To make a "direct" call to the engine
+return_value = engine.direct_post(
+    subject_id="sys-1", path="/my/path/", params={"key": "value"}, data={"my": "payload"}
+)
+```
+
 MIT License
 
 Copyright (c) 2023 Djungle s.r.l.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
```

### Comparing `djungle-rulesengine-client-0.3.0/src/rulesengine/client.py` & `djungle-rulesengine-client-0.3.3/src/rulesengine/client.py`

 * *Files identical despite different names*

### Comparing `djungle-rulesengine-client-0.3.0/tests/test_client.py` & `djungle-rulesengine-client-0.3.3/tests/test_client.py`

 * *Files identical despite different names*

