# Comparing `tmp/backendpy-0.2.4a5.tar.gz` & `tmp/backendpy-0.2.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backendpy-0.2.4a5.tar", last modified: Wed Apr 19 22:57:18 2023, max compression
+gzip compressed data, was "backendpy-0.2.5a1.tar", last modified: Thu May 11 10:58:33 2023, max compression
```

## Comparing `backendpy-0.2.4a5.tar` & `backendpy-0.2.5a1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.722996 backendpy-0.2.4a5/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1517 2022-01-24 11:39:51.000000 backendpy-0.2.4a5/LICENSE
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3810 2023-04-19 22:57:18.722996 backendpy-0.2.4a5/PKG-INFO
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2543 2022-12-24 20:09:28.000000 backendpy-0.2.4a5/README.md
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.507008 backendpy-0.2.4a5/backendpy/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       27 2022-02-20 19:27:36.000000 backendpy-0.2.4a5/backendpy/__init__.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1965 2022-08-26 21:11:09.000000 backendpy-0.2.4a5/backendpy/app.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    10027 2023-01-02 18:54:04.000000 backendpy-0.2.4a5/backendpy/asgi.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.511008 backendpy-0.2.4a5/backendpy/cli/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2020-06-05 08:33:23.000000 backendpy-0.2.4a5/backendpy/cli/__init__.py
--rwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)    15657 2022-12-27 08:15:36.000000 backendpy-0.2.4a5/backendpy/cli/admin.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2601 2022-12-10 12:10:57.000000 backendpy-0.2.4a5/backendpy/config.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.603003 backendpy-0.2.4a5/backendpy/data_handler/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2020-08-27 14:31:27.000000 backendpy-0.2.4a5/backendpy/data_handler/__init__.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3476 2023-01-04 01:03:30.000000 backendpy-0.2.4a5/backendpy/data_handler/data.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5370 2023-01-03 19:42:13.000000 backendpy-0.2.4a5/backendpy/data_handler/fields.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4609 2023-01-12 22:24:35.000000 backendpy-0.2.4a5/backendpy/data_handler/filters.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    21377 2023-04-02 12:48:01.000000 backendpy-0.2.4a5/backendpy/data_handler/validators.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4099 2022-12-10 12:07:53.000000 backendpy-0.2.4a5/backendpy/db.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5125 2023-01-03 03:06:50.000000 backendpy-0.2.4a5/backendpy/error.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5129 2023-01-03 03:06:50.000000 backendpy-0.2.4a5/backendpy/exception.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3090 2022-02-27 14:42:53.000000 backendpy-0.2.4a5/backendpy/hook.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1453 2022-08-26 21:56:05.000000 backendpy-0.2.4a5/backendpy/initializer.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1598 2022-05-20 16:53:26.000000 backendpy-0.2.4a5/backendpy/logging.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.647000 backendpy-0.2.4a5/backendpy/middleware/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       35 2022-12-27 07:51:13.000000 backendpy-0.2.4a5/backendpy/middleware/__init__.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.662999 backendpy-0.2.4a5/backendpy/middleware/defaults/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2022-12-27 07:51:11.000000 backendpy-0.2.4a5/backendpy/middleware/defaults/__init__.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5825 2022-12-27 08:01:32.000000 backendpy-0.2.4a5/backendpy/middleware/defaults/cors.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3973 2022-12-27 08:01:32.000000 backendpy-0.2.4a5/backendpy/middleware/middleware.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     9319 2023-01-04 01:13:10.000000 backendpy-0.2.4a5/backendpy/request.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    14077 2023-01-03 03:01:46.000000 backendpy-0.2.4a5/backendpy/response.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    13275 2023-03-20 19:22:31.000000 backendpy-0.2.4a5/backendpy/router.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2918 2022-06-04 13:28:58.000000 backendpy-0.2.4a5/backendpy/templating.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      908 2022-05-20 16:53:26.000000 backendpy-0.2.4a5/backendpy/unittest.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.710996 backendpy-0.2.4a5/backendpy/utils/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2019-10-11 09:00:54.000000 backendpy-0.2.4a5/backendpy/utils/__init__.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      258 2022-01-23 06:37:37.000000 backendpy-0.2.4a5/backendpy/utils/bytes.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    11834 2023-04-19 22:52:27.000000 backendpy-0.2.4a5/backendpy/utils/file.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4630 2023-01-29 02:21:14.000000 backendpy-0.2.4a5/backendpy/utils/http.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      477 2022-02-27 20:01:42.000000 backendpy-0.2.4a5/backendpy/utils/json.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-04-19 22:57:18.511008 backendpy-0.2.4a5/backendpy.egg-info/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3810 2023-04-19 22:57:18.000000 backendpy-0.2.4a5/backendpy.egg-info/PKG-INFO
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1042 2023-04-19 22:57:18.000000 backendpy-0.2.4a5/backendpy.egg-info/SOURCES.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        1 2023-04-19 22:57:18.000000 backendpy-0.2.4a5/backendpy.egg-info/dependency_links.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       55 2023-04-19 22:57:18.000000 backendpy-0.2.4a5/backendpy.egg-info/entry_points.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      100 2023-04-19 22:57:18.000000 backendpy-0.2.4a5/backendpy.egg-info/requires.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       10 2023-04-19 22:57:18.000000 backendpy-0.2.4a5/backendpy.egg-info/top_level.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      105 2021-09-12 18:23:47.000000 backendpy-0.2.4a5/pyproject.toml
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1426 2023-04-19 22:57:18.726996 backendpy-0.2.4a5/setup.cfg
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-11 10:58:33.159316 backendpy-0.2.5a1/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1517 2022-01-24 11:39:51.000000 backendpy-0.2.5a1/LICENSE
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3810 2023-05-11 10:58:33.159316 backendpy-0.2.5a1/PKG-INFO
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2543 2022-12-24 20:09:28.000000 backendpy-0.2.5a1/README.md
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-11 10:58:33.143317 backendpy-0.2.5a1/backendpy/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       27 2022-02-20 19:27:36.000000 backendpy-0.2.5a1/backendpy/__init__.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1965 2022-08-26 21:11:09.000000 backendpy-0.2.5a1/backendpy/app.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    10027 2023-01-02 18:54:04.000000 backendpy-0.2.5a1/backendpy/asgi.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-11 10:58:33.151316 backendpy-0.2.5a1/backendpy/cli/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2020-06-05 08:33:23.000000 backendpy-0.2.5a1/backendpy/cli/__init__.py
+-rwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)    15657 2022-12-27 08:15:36.000000 backendpy-0.2.5a1/backendpy/cli/admin.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2601 2022-12-10 12:10:57.000000 backendpy-0.2.5a1/backendpy/config.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-11 10:58:33.155316 backendpy-0.2.5a1/backendpy/data_handler/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2020-08-27 14:31:27.000000 backendpy-0.2.5a1/backendpy/data_handler/__init__.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3476 2023-01-04 01:03:30.000000 backendpy-0.2.5a1/backendpy/data_handler/data.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5370 2023-01-03 19:42:13.000000 backendpy-0.2.5a1/backendpy/data_handler/fields.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4609 2023-01-12 22:24:35.000000 backendpy-0.2.5a1/backendpy/data_handler/filters.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    21377 2023-04-02 12:48:01.000000 backendpy-0.2.5a1/backendpy/data_handler/validators.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4099 2022-12-10 12:07:53.000000 backendpy-0.2.5a1/backendpy/db.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5125 2023-01-03 03:06:50.000000 backendpy-0.2.5a1/backendpy/error.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5129 2023-01-03 03:06:50.000000 backendpy-0.2.5a1/backendpy/exception.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3090 2022-02-27 14:42:53.000000 backendpy-0.2.5a1/backendpy/hook.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1453 2022-08-26 21:56:05.000000 backendpy-0.2.5a1/backendpy/initializer.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1598 2022-05-20 16:53:26.000000 backendpy-0.2.5a1/backendpy/logging.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-11 10:58:33.155316 backendpy-0.2.5a1/backendpy/middleware/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       35 2022-12-27 07:51:13.000000 backendpy-0.2.5a1/backendpy/middleware/__init__.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-11 10:58:33.155316 backendpy-0.2.5a1/backendpy/middleware/defaults/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2022-12-27 07:51:11.000000 backendpy-0.2.5a1/backendpy/middleware/defaults/__init__.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5825 2022-12-27 08:01:32.000000 backendpy-0.2.5a1/backendpy/middleware/defaults/cors.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3973 2022-12-27 08:01:32.000000 backendpy-0.2.5a1/backendpy/middleware/middleware.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     9319 2023-01-04 01:13:10.000000 backendpy-0.2.5a1/backendpy/request.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    17355 2023-05-11 10:44:24.000000 backendpy-0.2.5a1/backendpy/response.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    13275 2023-03-20 19:22:31.000000 backendpy-0.2.5a1/backendpy/router.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2918 2022-06-04 13:28:58.000000 backendpy-0.2.5a1/backendpy/templating.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      908 2022-05-20 16:53:26.000000 backendpy-0.2.5a1/backendpy/unittest.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-11 10:58:33.159316 backendpy-0.2.5a1/backendpy/utils/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2019-10-11 09:00:54.000000 backendpy-0.2.5a1/backendpy/utils/__init__.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      258 2022-01-23 06:37:37.000000 backendpy-0.2.5a1/backendpy/utils/bytes.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    12916 2023-05-11 09:06:30.000000 backendpy-0.2.5a1/backendpy/utils/file.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4630 2023-01-29 02:21:14.000000 backendpy-0.2.5a1/backendpy/utils/http.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      477 2022-02-27 20:01:42.000000 backendpy-0.2.5a1/backendpy/utils/json.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-11 10:58:33.147317 backendpy-0.2.5a1/backendpy.egg-info/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3810 2023-05-11 10:58:33.000000 backendpy-0.2.5a1/backendpy.egg-info/PKG-INFO
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1042 2023-05-11 10:58:33.000000 backendpy-0.2.5a1/backendpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        1 2023-05-11 10:58:33.000000 backendpy-0.2.5a1/backendpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       55 2023-05-11 10:58:33.000000 backendpy-0.2.5a1/backendpy.egg-info/entry_points.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      100 2023-05-11 10:58:33.000000 backendpy-0.2.5a1/backendpy.egg-info/requires.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       10 2023-05-11 10:58:33.000000 backendpy-0.2.5a1/backendpy.egg-info/top_level.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      105 2021-09-12 18:23:47.000000 backendpy-0.2.5a1/pyproject.toml
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1426 2023-05-11 10:58:33.163315 backendpy-0.2.5a1/setup.cfg
```

### Comparing `backendpy-0.2.4a5/LICENSE` & `backendpy-0.2.5a1/LICENSE`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/PKG-INFO` & `backendpy-0.2.5a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backendpy
-Version: 0.2.4a5
+Version: 0.2.5a1
 Summary: Async (ASGI) Python web framework
 Home-page: https://github.com/savangco/backendpy
 Author: Savang Co.
 Author-email: backendpy@savang.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/savangco/backendpy/issues
 Project-URL: Documentation, https://backendpy.readthedocs.io
```

### Comparing `backendpy-0.2.4a5/README.md` & `backendpy-0.2.5a1/README.md`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/app.py` & `backendpy-0.2.5a1/backendpy/app.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/asgi.py` & `backendpy-0.2.5a1/backendpy/asgi.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/cli/admin.py` & `backendpy-0.2.5a1/backendpy/cli/admin.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/config.py` & `backendpy-0.2.5a1/backendpy/config.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/data_handler/data.py` & `backendpy-0.2.5a1/backendpy/data_handler/data.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/data_handler/fields.py` & `backendpy-0.2.5a1/backendpy/data_handler/fields.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/data_handler/filters.py` & `backendpy-0.2.5a1/backendpy/data_handler/filters.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/data_handler/validators.py` & `backendpy-0.2.5a1/backendpy/data_handler/validators.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/db.py` & `backendpy-0.2.5a1/backendpy/db.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/error.py` & `backendpy-0.2.5a1/backendpy/error.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/exception.py` & `backendpy-0.2.5a1/backendpy/exception.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/hook.py` & `backendpy-0.2.5a1/backendpy/hook.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/initializer.py` & `backendpy-0.2.5a1/backendpy/initializer.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/logging.py` & `backendpy-0.2.5a1/backendpy/logging.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/middleware/defaults/cors.py` & `backendpy-0.2.5a1/backendpy/middleware/defaults/cors.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/middleware/middleware.py` & `backendpy-0.2.5a1/backendpy/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/request.py` & `backendpy-0.2.5a1/backendpy/request.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/response.py` & `backendpy-0.2.5a1/backendpy/response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import datetime
 import gzip
 import os
 import types
 import zlib
 from collections.abc import Iterable, AsyncGenerator
 from enum import IntEnum
 from mimetypes import guess_type
@@ -277,61 +278,116 @@
 
     def __init__(
             self,
             path: str,
             status: Status = Status.OK,
             headers: Optional[Iterable[[bytes, bytes]]] = None,
             stream: bool = True,
-            compress: bool = False):
+            compress: bool = False,
+            partial: bool = False,
+            last_modified: Optional[int] = None,
+            entity_tag: Optional[str] = None):
         """
         Initialize response instance.
 
         :param path: The file path inside the project media path
         :param status: The HTTP response status
         :param headers: The HTTP response headers
         :param stream: Determines whether or not to stream the response
         :param compress: Determines whether or not to compress (gzip) the response
+        :param partial: Determines whether to support partial response
+        :param last_modified: Specifies the Last-Modified HTTP header and uses it in the if-range condition check
+        :param entity_tag: Specifies the ETag HTTP header and uses it in the if-range condition check
         """
         super().__init__(
             body=b'',
             status=status,
             headers=headers,
             content_type=b'application/octet-stream',
             compress=compress)
         self.path = path
         self.stream = stream
+        self.partial = partial
+        self.last_modified = last_modified
+        self.entity_tag = entity_tag
 
     async def __call__(self, request: Request) \
             -> tuple[bytes | AsyncGenerator[bytes],
                      int,
                      list[[bytes, bytes]],
                      bool]:
         path = os.path.join(request.app.config['environment']['media_path'], unquote(self.path))
         if not os.path.isfile(path):
             raise FileNotFoundError
 
         self.headers = list(self.headers) if self.headers else []
         content_type, encoding = guess_type(path)
-        self.headers += [[b'content-type', to_bytes(content_type) if content_type else self.content_type]]
-
-        if self.stream:
-            self.body = read_file_chunks(path, int(request.app.config['networking']['stream_size']))
-            if self.compress:
-                self.body = self._gzip_stream(self.body)
-                self.headers += [[b'content-encoding', b'deflate']]
+        self.headers += [[b'content-type', to_bytes(content_type) if content_type else self.content_type],
+                         [b'accept-ranges', b'bytes' if self.partial else b'none']]
+        try:
+            partial = self.partial \
+                      and 'range' in request.headers \
+                      and request.headers['range'].startswith('bytes=') \
+                      and ('if-range' not in request.headers
+                           or (self.entity_tag is not None
+                               and not self.entity_tag.startswith('/W')
+                               and not request.headers['if-range'].startswith('/W')
+                               and request.headers['if-range'] == self.entity_tag)
+                           or (self.entity_tag is None
+                               and self.last_modified is not None
+                               and datetime.datetime.utcfromtimestamp(self.last_modified).replace(microsecond=0) ==
+                               datetime.datetime.strptime(request.headers['if-range'], '%a, %d %b %Y %H:%M:%S %Z')))
+        except ValueError:
+            partial = False
+        if partial:
+            total_length = (await aiofiles.os.stat(path)).st_size
+            try:
+                ranges = request.headers['range'][6:].split(',')
+                range_ = ranges[0].split('-')
+                range_start = int(range_[0]) if range_[0] != '' else 0
+                range_end = int(range_[1]) if range_[1] != '' else total_length - 1
+                is_invalid_range = range_start > range_end or range_end > total_length
+            except (ValueError, IndexError):
+                is_invalid_range = True
+            if is_invalid_range:
+                self.status = Status.REQUESTED_RANGE_NOT_SATISFIABLE
+                return self.body, self.status.value, self.headers, False
+            self.status = Status.PARTIAL_CONTENT
+            if self.stream:
+                self.body = read_file_chunks(
+                    path,
+                    chunk_size=int(request.app.config['networking']['stream_size']),
+                    start_index=range_start,
+                    end_index=range_end)
             else:
-                file_stat = await aiofiles.os.stat(path)
-                self.headers += [[b'content-length', to_bytes(file_stat.st_size)]]
+                self.body = await read_file(
+                    path,
+                    start_index=range_start,
+                    end_index=range_end)
+            self.headers += [[b'content-range', to_bytes(f'bytes {range_start}-{range_end}/{total_length}')],
+                             [b'content-length', to_bytes(range_end-range_start+1)]]
         else:
-            self.body = await read_file(path)
-            if self.compress:
-                self.body = self._gzip(self.body)
-                self.headers += [[b'content-encoding', b'gzip']]
-            self.headers += [[b'content-length', to_bytes(len(self.body))]]
-
+            if self.stream:
+                self.body = read_file_chunks(path, int(request.app.config['networking']['stream_size']))
+                if self.compress:
+                    self.body = self._gzip_stream(self.body)
+                    self.headers += [[b'content-encoding', b'deflate']]
+                else:
+                    file_stat = await aiofiles.os.stat(path)
+                    self.headers += [[b'content-length', to_bytes(file_stat.st_size)]]
+            else:
+                self.body = await read_file(path)
+                if self.compress:
+                    self.body = self._gzip(self.body)
+                    self.headers += [[b'content-encoding', b'gzip']]
+                self.headers += [[b'content-length', to_bytes(len(self.body))]]
+        if self.last_modified is not None:
+            self.headers += [[b'last-modified', to_bytes(self.last_modified)]]
+        if self.entity_tag is not None:
+            self.headers += [[b'etag', to_bytes(self.entity_tag)]]
         return self.body, self.status.value, self.headers, self.stream
 
 
 class Redirect(Response):
     """Redirect response class inherited from :class:`~backendpy.response.Response` class."""
 
     def __init__(
```

### Comparing `backendpy-0.2.4a5/backendpy/router.py` & `backendpy-0.2.5a1/backendpy/router.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/templating.py` & `backendpy-0.2.5a1/backendpy/templating.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/unittest.py` & `backendpy-0.2.5a1/backendpy/unittest.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy/utils/file.py` & `backendpy-0.2.5a1/backendpy/utils/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,61 @@
 
 import binascii
 import hashlib
 import io
 import mimetypes
 import os
 import types
-from typing import Literal, AnyStr
+from typing import Literal, AnyStr, Optional
 
 import aiofiles
 import aiofiles.os
 
 READ_MODES = Literal['r', 'rb', 'rt']
 WRITE_MODES = Literal['w', 'w+', 'wb', 'wb+', 'wt', 'wt+']
 
 
-async def read_file_chunks(path, chunk_size=32768, mode: READ_MODES = 'rb'):
+async def read_file_chunks(
+        path,
+        chunk_size=32768,
+        mode: READ_MODES = 'rb',
+        start_index: Optional[int] = None,
+        end_index: Optional[int] = None):
     async with aiofiles.open(path, mode) as f:
+        remaining_size = None
+        if start_index is not None:
+            await f.seek(start_index)
+            if end_index is not None:
+                remaining_size = end_index-start_index+1
+                if remaining_size < chunk_size:
+                    chunk_size = remaining_size
+        elif end_index is not None:
+            remaining_size = end_index+1
+            if remaining_size < chunk_size:
+                chunk_size = remaining_size
         while chunk := await f.read(chunk_size):
             yield chunk
+            if remaining_size is not None:
+                remaining_size -= chunk_size
+                if remaining_size < chunk_size:
+                    chunk_size = remaining_size
 
 
-async def read_file(path, mode: READ_MODES = 'rb'):
+async def read_file(
+        path,
+        mode: READ_MODES = 'rb',
+        start_index: Optional[int] = None,
+        end_index: Optional[int] = None):
     async with aiofiles.open(path, mode) as f:
+        if start_index:
+            await f.seek(start_index)
+            if end_index:
+                return await f.read(end_index-start_index+1)
+        elif end_index:
+            return await f.read(end_index+1)
         return await f.read()
 
 
 async def read_file_lines(path, mode: READ_MODES = 'rb'):
     async with aiofiles.open(path, mode) as f:
         return await f.readlines()
```

### Comparing `backendpy-0.2.4a5/backendpy/utils/http.py` & `backendpy-0.2.5a1/backendpy/utils/http.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/backendpy.egg-info/PKG-INFO` & `backendpy-0.2.5a1/backendpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backendpy
-Version: 0.2.4a5
+Version: 0.2.5a1
 Summary: Async (ASGI) Python web framework
 Home-page: https://github.com/savangco/backendpy
 Author: Savang Co.
 Author-email: backendpy@savang.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/savangco/backendpy/issues
 Project-URL: Documentation, https://backendpy.readthedocs.io
```

### Comparing `backendpy-0.2.4a5/backendpy.egg-info/SOURCES.txt` & `backendpy-0.2.5a1/backendpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.4a5/setup.cfg` & `backendpy-0.2.5a1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = backendpy
-version = v0.2.4-alpha.5
+version = v0.2.5-alpha.1
 author = Savang Co.
 author_email = backendpy@savang.com
 description = Async (ASGI) Python web framework
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Backendpy, Web, Framework, Python, Async, ASGI
 license = BSD 3-Clause License
```

