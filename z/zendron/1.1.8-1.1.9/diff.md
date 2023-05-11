# Comparing `tmp/zendron-1.1.8.tar.gz` & `tmp/zendron-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zendron-1.1.8.tar", last modified: Wed May 10 19:28:04 2023, max compression
+gzip compressed data, was "zendron-1.1.9.tar", last modified: Wed May 10 19:33:13 2023, max compression
```

## Comparing `zendron-1.1.8.tar` & `zendron-1.1.9.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.472204 zendron-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 19:27:53.000000 zendron-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-10 19:27:53.000000 zendron-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-10 19:28:04.472204 zendron-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-10 19:27:53.000000 zendron-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.468204 zendron-1.1.8/notes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.468204 zendron-1.1.8/notes/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.468204 zendron-1.1.8/notes/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)   108556 2023-05-10 19:27:53.000000 zendron-1.1.8/notes/assets/images/zotero.api-key.md.zotero-api-key.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.468204 zendron-1.1.8/pods/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.468204 zendron-1.1.8/pods/dendron.markdown/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 19:27:53.000000 zendron-1.1.8/pods/dendron.markdown/config.import.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-10 19:27:53.000000 zendron-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 19:28:04.472204 zendron-1.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.468204 zendron-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.472204 zendron-1.1.8/src/zendron/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/cache_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/comments_deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.468204 zendron-1.1.8/src/zendron/conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.472204 zendron-1.1.8/src/zendron/conf/zendron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/conf/zendron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/front.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.468204 zendron-1.1.8/src/zendron/pods/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.472204 zendron-1.1.8/src/zendron/pods/dendron.markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/pods/dendron.markdown/config.import.yml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/read_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-10 19:27:53.000000 zendron-1.1.8/src/zendron/user_citation_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:28:04.472204 zendron-1.1.8/src/zendron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-10 19:28:04.000000 zendron-1.1.8/src/zendron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-10 19:28:04.000000 zendron-1.1.8/src/zendron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:28:04.000000 zendron-1.1.8/src/zendron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-10 19:28:04.000000 zendron-1.1.8/src/zendron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-10 19:28:04.000000 zendron-1.1.8/src/zendron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 19:28:04.000000 zendron-1.1.8/src/zendron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.975069 zendron-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 19:33:00.000000 zendron-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-10 19:33:00.000000 zendron-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-10 19:33:13.975069 zendron-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-10 19:33:00.000000 zendron-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.959069 zendron-1.1.9/notes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.959069 zendron-1.1.9/notes/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.963069 zendron-1.1.9/notes/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   108556 2023-05-10 19:33:00.000000 zendron-1.1.9/notes/assets/images/zotero.api-key.md.zotero-api-key.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.959069 zendron-1.1.9/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.967069 zendron-1.1.9/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 19:33:00.000000 zendron-1.1.9/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-10 19:33:00.000000 zendron-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 19:33:13.975069 zendron-1.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.963069 zendron-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.971069 zendron-1.1.9/src/zendron/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/cache_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/comments_deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.975069 zendron-1.1.9/src/zendron/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.975069 zendron-1.1.9/src/zendron/conf/zendron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/conf/zendron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.963069 zendron-1.1.9/src/zendron/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.975069 zendron-1.1.9/src/zendron/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/read_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-10 19:33:00.000000 zendron-1.1.9/src/zendron/user_citation_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:33:13.975069 zendron-1.1.9/src/zendron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-10 19:33:13.000000 zendron-1.1.9/src/zendron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-10 19:33:13.000000 zendron-1.1.9/src/zendron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:33:13.000000 zendron-1.1.9/src/zendron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-10 19:33:13.000000 zendron-1.1.9/src/zendron.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-10 19:33:13.000000 zendron-1.1.9/src/zendron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 19:33:13.000000 zendron-1.1.9/src/zendron.egg-info/top_level.txt
```

### Comparing `zendron-1.1.8/LICENSE` & `zendron-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/PKG-INFO` & `zendron-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.1.8
+Version: 1.1.9
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zendron-1.1.8/README.md` & `zendron-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/notes/assets/images/zotero.api-key.md.zotero-api-key.png` & `zendron-1.1.9/notes/assets/images/zotero.api-key.md.zotero-api-key.png`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/pyproject.toml` & `zendron-1.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=67.7.2", "wheel>=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zendron"
-version = "1.1.8"
+version = "1.1.9"
 description = "Import Zotero annotations with Dendron integration"
 readme = "README.md"
 authors = [{ name = "Michael Volk", email = "michaeljvolk7@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `zendron-1.1.8/src/zendron/__main__.py` & `zendron-1.1.9/src/zendron/__main__.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/annotations.py` & `zendron-1.1.9/src/zendron/annotations.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/bibtex.py` & `zendron-1.1.9/src/zendron/bibtex.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/cache.py` & `zendron-1.1.9/src/zendron/cache.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/cache_deprecated.py` & `zendron-1.1.9/src/zendron/cache_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/comments.py` & `zendron-1.1.9/src/zendron/comments.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/comments_deprecated.py` & `zendron-1.1.9/src/zendron/comments_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/config.py` & `zendron-1.1.9/src/zendron/config.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/front.py` & `zendron-1.1.9/src/zendron/front.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/init.py` & `zendron-1.1.9/src/zendron/init.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/items.py` & `zendron-1.1.9/src/zendron/items.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/load.py` & `zendron-1.1.9/src/zendron/load.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/metadata.py` & `zendron-1.1.9/src/zendron/metadata.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/pods/dendron.markdown/config.import.yml` & `zendron-1.1.9/src/zendron/pods/dendron.markdown/config.import.yml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/read_md.py` & `zendron-1.1.9/src/zendron/read_md.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/remove.py` & `zendron-1.1.9/src/zendron/remove.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/scratch.py` & `zendron-1.1.9/src/zendron/scratch.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/sync.py` & `zendron-1.1.9/src/zendron/sync.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron/user_citation_key.py` & `zendron-1.1.9/src/zendron/user_citation_key.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.8/src/zendron.egg-info/PKG-INFO` & `zendron-1.1.9/src/zendron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.1.8
+Version: 1.1.9
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zendron-1.1.8/src/zendron.egg-info/SOURCES.txt` & `zendron-1.1.9/src/zendron.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,10 @@
 src/zendron/user_citation_key.py
 src/zendron.egg-info/PKG-INFO
 src/zendron.egg-info/SOURCES.txt
 src/zendron.egg-info/dependency_links.txt
 src/zendron.egg-info/entry_points.txt
 src/zendron.egg-info/requires.txt
 src/zendron.egg-info/top_level.txt
+src/zendron/conf/__init__.py
 src/zendron/conf/zendron/__init__.py
 src/zendron/pods/dendron.markdown/config.import.yml
```

