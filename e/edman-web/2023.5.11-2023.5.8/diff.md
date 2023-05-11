# Comparing `tmp/edman_web-2023.5.11.tar.gz` & `tmp/edman_web-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman_web-2023.5.11.tar", last modified: Thu May 11 01:39:35 2023, max compression
+gzip compressed data, was "edman_web-2023.5.8.tar", last modified: Mon May  8 04:41:52 2023, max compression
```

## Comparing `edman_web-2023.5.11.tar` & `edman_web-2023.5.8.tar`

### file list

```diff
@@ -1,34 +1,20 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 01:39:35.173685 edman_web-2023.5.11/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2023.5.11/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2393 2023-05-11 01:39:35.173685 edman_web-2023.5.11/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      626 2023-03-30 03:11:16.000000 edman_web-2023.5.11/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 01:39:35.163685 edman_web-2023.5.11/edman_web/
--rw-r--r--   0 ohno      (1000) ohno      (1000)       80 2023-04-04 05:55:42.000000 edman_web-2023.5.11/edman_web/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     6477 2023-05-08 04:40:18.000000 edman_web-2023.5.11/edman_web/file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2639 2023-03-29 09:20:48.000000 edman_web-2023.5.11/edman_web/search_manager.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 01:39:35.163685 edman_web-2023.5.11/edman_web.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2393 2023-05-11 01:39:35.000000 edman_web-2023.5.11/edman_web.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      627 2023-05-11 01:39:35.000000 edman_web-2023.5.11/edman_web.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-11 01:39:35.000000 edman_web-2023.5.11/edman_web.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       62 2023-05-11 01:39:35.000000 edman_web-2023.5.11/edman_web.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       32 2023-05-11 01:39:35.000000 edman_web-2023.5.11/edman_web.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)      946 2023-05-11 01:36:21.000000 edman_web-2023.5.11/pyproject.toml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      713 2023-05-11 01:39:35.173685 edman_web-2023.5.11/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 01:39:35.163685 edman_web-2023.5.11/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    13863 2023-04-25 08:38:11.000000 edman_web-2023.5.11/tests/test_file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5059 2023-04-04 05:55:42.000000 edman_web-2023.5.11/tests/test_search_manager.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 01:39:35.163685 edman_web-2023.5.11/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-11 01:39:35.173685 edman_web-2023.5.11/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:43:44.000000 edman_web-2023.5.11/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-10 08:18:15.000000 edman_web-2023.5.11/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-10 08:18:15.000000 edman_web-2023.5.11/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-10 08:18:15.000000 edman_web-2023.5.11/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-10 08:18:15.000000 edman_web-2023.5.11/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-10 08:18:15.000000 edman_web-2023.5.11/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-10 08:18:15.000000 edman_web-2023.5.11/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     2180 2023-05-10 08:18:15.000000 edman_web-2023.5.11/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-10 08:18:15.000000 edman_web-2023.5.11/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-10 08:18:15.000000 edman_web-2023.5.11/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-10 08:18:15.000000 edman_web-2023.5.11/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-10 08:18:15.000000 edman_web-2023.5.11/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-10 08:18:15.000000 edman_web-2023.5.11/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 04:41:52.696269 edman_web-2023.5.8/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2023.5.8/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2023-03-29 09:20:48.000000 edman_web-2023.5.8/MANIFEST.in
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1090 2023-05-08 04:41:52.696269 edman_web-2023.5.8/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      626 2023-03-30 03:11:16.000000 edman_web-2023.5.8/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 04:41:52.696269 edman_web-2023.5.8/edman_web/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       80 2023-04-04 05:55:42.000000 edman_web-2023.5.8/edman_web/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6477 2023-05-08 04:40:18.000000 edman_web-2023.5.8/edman_web/file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2639 2023-03-29 09:20:48.000000 edman_web-2023.5.8/edman_web/search_manager.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 04:41:52.696269 edman_web-2023.5.8/edman_web.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1090 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      349 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       61 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       10 2023-05-08 04:41:52.000000 edman_web-2023.5.8/edman_web.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      713 2023-05-08 04:41:52.696269 edman_web-2023.5.8/setup.cfg
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       41 2023-03-29 09:20:48.000000 edman_web-2023.5.8/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 04:41:52.696269 edman_web-2023.5.8/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    13863 2023-04-25 08:38:11.000000 edman_web-2023.5.8/tests/test_file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5059 2023-04-04 05:55:42.000000 edman_web-2023.5.8/tests/test_search_manager.py
```

### Comparing `edman_web-2023.5.11/LICENSE.txt` & `edman_web-2023.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman_web-2023.5.11/README.rst` & `edman_web-2023.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `edman_web-2023.5.11/edman_web/file_manager.py` & `edman_web-2023.5.8/edman_web/file_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.5.11/edman_web/search_manager.py` & `edman_web-2023.5.8/edman_web/search_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.5.11/setup.cfg` & `edman_web-2023.5.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `edman_web-2023.5.11/tests/test_file_manager.py` & `edman_web-2023.5.8/tests/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.5.11/tests/test_search_manager.py` & `edman_web-2023.5.8/tests/test_search_manager.py`

 * *Files identical despite different names*

