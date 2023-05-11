# Comparing `tmp/botcity-ms365-onedrive-plugin-0.1.0.tar.gz` & `tmp/botcity-ms365-onedrive-plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/bot-ms365-onedrive-plugin-python/bot-ms365-onedrive-plugin-python/dist/.tmp-vqd5mfi4/botcity-ms365-onedrive-p", last modified: Wed Mar 22 14:19:57 2023, max compression
+gzip compressed data, was "/home/runner/work/bot-ms365-onedrive-plugin-python/bot-ms365-onedrive-plugin-python/dist/.tmp-927e3xnb/botcity-ms365-onedrive-p", last modified: Thu May 11 12:21:41 2023, max compression
```

## Comparing `botcity-ms365-onedrive-plugin-0.1.0.tar` & `botcity-ms365-onedrive-plugin-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-22 14:19:48.000000 botcity-ms365-onedrive-plugin-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-03-22 14:19:48.000000 botcity-ms365-onedrive-plugin-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity/plugins/ms365/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity/plugins/ms365/onedrive/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-22 14:19:48.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity/plugins/ms365/onedrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity/plugins/ms365/onedrive/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-03-22 14:19:48.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity/plugins/ms365/onedrive/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity_ms365_onedrive_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity_ms365_onedrive_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity_ms365_onedrive_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity_ms365_onedrive_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity_ms365_onedrive_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/botcity_ms365_onedrive_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-22 14:19:48.000000 botcity-ms365-onedrive-plugin-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-22 14:19:48.000000 botcity-ms365-onedrive-plugin-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:19:57.000000 botcity-ms365-onedrive-plugin-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-22 14:19:48.000000 botcity-ms365-onedrive-plugin-0.1.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-22 14:19:48.000000 botcity-ms365-onedrive-plugin-0.1.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-03-22 14:19:48.000000 botcity-ms365-onedrive-plugin-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-11 12:21:28.000000 botcity-ms365-onedrive-plugin-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-11 12:21:28.000000 botcity-ms365-onedrive-plugin-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity/plugins/ms365/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity/plugins/ms365/onedrive/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-11 12:21:28.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity/plugins/ms365/onedrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity/plugins/ms365/onedrive/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-05-11 12:21:28.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity/plugins/ms365/onedrive/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity_ms365_onedrive_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity_ms365_onedrive_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity_ms365_onedrive_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity_ms365_onedrive_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity_ms365_onedrive_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/botcity_ms365_onedrive_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 12:21:28.000000 botcity-ms365-onedrive-plugin-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-11 12:21:28.000000 botcity-ms365-onedrive-plugin-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:21:41.000000 botcity-ms365-onedrive-plugin-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 12:21:28.000000 botcity-ms365-onedrive-plugin-0.2.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-11 12:21:28.000000 botcity-ms365-onedrive-plugin-0.2.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-11 12:21:28.000000 botcity-ms365-onedrive-plugin-0.2.0/versioneer.py
```

### Comparing `botcity-ms365-onedrive-plugin-0.1.0/PKG-INFO` & `botcity-ms365-onedrive-plugin-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-ms365-onedrive-plugin
-Version: 0.1.0
+Version: 0.2.0
 Home-page: https://github.com/botcity-dev/bot-ms365-onedrive-plugin-python.git
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # BotCity Microsoft 365 OneDrive Plugin - Python
 
 ## 🤖 Computer-vision based UI Automation
```

### Comparing `botcity-ms365-onedrive-plugin-0.1.0/README.md` & `botcity-ms365-onedrive-plugin-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `botcity-ms365-onedrive-plugin-0.1.0/botcity_ms365_onedrive_plugin.egg-info/PKG-INFO` & `botcity-ms365-onedrive-plugin-0.2.0/botcity_ms365_onedrive_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-ms365-onedrive-plugin
-Version: 0.1.0
+Version: 0.2.0
 Home-page: https://github.com/botcity-dev/bot-ms365-onedrive-plugin-python.git
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # BotCity Microsoft 365 OneDrive Plugin - Python
 
 ## 🤖 Computer-vision based UI Automation
```

### Comparing `botcity-ms365-onedrive-plugin-0.1.0/setup.py` & `botcity-ms365-onedrive-plugin-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `botcity-ms365-onedrive-plugin-0.1.0/tests/test_plugin.py` & `botcity-ms365-onedrive-plugin-0.2.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `botcity-ms365-onedrive-plugin-0.1.0/versioneer.py` & `botcity-ms365-onedrive-plugin-0.2.0/versioneer.py`

 * *Files identical despite different names*

