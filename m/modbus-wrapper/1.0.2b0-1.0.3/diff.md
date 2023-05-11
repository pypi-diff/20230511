# Comparing `tmp/modbus-wrapper-1.0.2b0.tar.gz` & `tmp/modbus-wrapper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modbus-wrapper-1.0.2b0.tar", last modified: Wed Apr  5 07:24:50 2023, max compression
+gzip compressed data, was "modbus-wrapper-1.0.3.tar", last modified: Thu May 11 14:36:58 2023, max compression
```

## Comparing `modbus-wrapper-1.0.2b0.tar` & `modbus-wrapper-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-05 07:24:50.174574 modbus-wrapper-1.0.2b0/
--rw-r--r--   0 bubba     (1000) bubba     (1000)      277 2023-04-05 07:24:50.174574 modbus-wrapper-1.0.2b0/PKG-INFO
--rw-r--r--   0 bubba     (1000) bubba     (1000)     1977 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/README.md
-drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-05 07:24:50.158574 modbus-wrapper-1.0.2b0/modbus_wrapper/
--rw-r--r--   0 bubba     (1000) bubba     (1000)       71 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/__init__.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)     6132 2023-04-05 07:20:35.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/client.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)     6564 2023-04-05 07:20:11.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/function_argument.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)      233 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/modbus_function_code.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)     1700 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/object_factory.py
-drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-05 07:24:50.170574 modbus-wrapper-1.0.2b0/modbus_wrapper/objects/
--rw-r--r--   0 bubba     (1000) bubba     (1000)       77 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/objects/__init__.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)      366 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/objects/config.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)     3273 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/objects/fatek_object.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)     3085 2023-04-05 07:18:55.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/objects/modbus_object.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)     2569 2023-04-04 08:12:14.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/objects/modbus_value.py
-drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-05 07:24:50.166574 modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/
--rw-r--r--   0 bubba     (1000) bubba     (1000)      277 2023-04-05 07:24:50.000000 modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 bubba     (1000) bubba     (1000)      589 2023-04-05 07:24:50.000000 modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 bubba     (1000) bubba     (1000)        1 2023-04-05 07:24:50.000000 modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 bubba     (1000) bubba     (1000)       12 2023-04-05 07:24:50.000000 modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/requires.txt
--rw-r--r--   0 bubba     (1000) bubba     (1000)       15 2023-04-05 07:24:50.000000 modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/top_level.txt
--rw-r--r--   0 bubba     (1000) bubba     (1000)       38 2023-04-05 07:24:50.174574 modbus-wrapper-1.0.2b0/setup.cfg
--rw-r--r--   0 bubba     (1000) bubba     (1000)      393 2023-04-05 07:23:46.000000 modbus-wrapper-1.0.2b0/setup.py
-drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-05 07:24:50.174574 modbus-wrapper-1.0.2b0/tests/
--rw-r--r--   0 bubba     (1000) bubba     (1000)     1992 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/tests/test_modbus_client_wrapper.py
+drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-05-11 14:36:58.415916 modbus-wrapper-1.0.3/
+-rw-r--r--   0 bubba     (1000) bubba     (1000)      299 2023-05-11 14:36:58.415916 modbus-wrapper-1.0.3/PKG-INFO
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     1977 2023-05-11 14:28:50.000000 modbus-wrapper-1.0.3/README.md
+drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-05-11 14:36:58.415916 modbus-wrapper-1.0.3/modbus_wrapper/
+-rw-r--r--   0 bubba     (1000) bubba     (1000)       71 2023-05-11 14:28:50.000000 modbus-wrapper-1.0.3/modbus_wrapper/__init__.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     6132 2023-05-11 14:28:50.000000 modbus-wrapper-1.0.3/modbus_wrapper/client.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     6564 2023-05-11 14:28:50.000000 modbus-wrapper-1.0.3/modbus_wrapper/function_argument.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)      233 2023-05-11 14:28:50.000000 modbus-wrapper-1.0.3/modbus_wrapper/modbus_function_code.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     1700 2023-05-11 14:28:50.000000 modbus-wrapper-1.0.3/modbus_wrapper/object_factory.py
+drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-05-11 14:36:58.415916 modbus-wrapper-1.0.3/modbus_wrapper/objects/
+-rw-r--r--   0 bubba     (1000) bubba     (1000)       77 2023-05-11 14:28:50.000000 modbus-wrapper-1.0.3/modbus_wrapper/objects/__init__.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)      366 2023-05-11 14:28:50.000000 modbus-wrapper-1.0.3/modbus_wrapper/objects/config.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     3273 2023-05-11 14:28:50.000000 modbus-wrapper-1.0.3/modbus_wrapper/objects/fatek_object.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     3085 2023-05-11 14:28:50.000000 modbus-wrapper-1.0.3/modbus_wrapper/objects/modbus_object.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     2569 2023-05-11 14:28:50.000000 modbus-wrapper-1.0.3/modbus_wrapper/objects/modbus_value.py
+drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-05-11 14:36:58.415916 modbus-wrapper-1.0.3/modbus_wrapper.egg-info/
+-rw-r--r--   0 bubba     (1000) bubba     (1000)      299 2023-05-11 14:36:58.000000 modbus-wrapper-1.0.3/modbus_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 bubba     (1000) bubba     (1000)      553 2023-05-11 14:36:58.000000 modbus-wrapper-1.0.3/modbus_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 bubba     (1000) bubba     (1000)        1 2023-05-11 14:36:58.000000 modbus-wrapper-1.0.3/modbus_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 bubba     (1000) bubba     (1000)       12 2023-05-11 14:36:58.000000 modbus-wrapper-1.0.3/modbus_wrapper.egg-info/requires.txt
+-rw-r--r--   0 bubba     (1000) bubba     (1000)       15 2023-05-11 14:36:58.000000 modbus-wrapper-1.0.3/modbus_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 bubba     (1000) bubba     (1000)       38 2023-05-11 14:36:58.415916 modbus-wrapper-1.0.3/setup.cfg
+-rw-r--r--   0 bubba     (1000) bubba     (1000)      419 2023-05-11 14:36:07.000000 modbus-wrapper-1.0.3/setup.py
```

### Comparing `modbus-wrapper-1.0.2b0/README.md` & `modbus-wrapper-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `modbus-wrapper-1.0.2b0/modbus_wrapper/client.py` & `modbus-wrapper-1.0.3/modbus_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `modbus-wrapper-1.0.2b0/modbus_wrapper/function_argument.py` & `modbus-wrapper-1.0.3/modbus_wrapper/function_argument.py`

 * *Files identical despite different names*

### Comparing `modbus-wrapper-1.0.2b0/modbus_wrapper/object_factory.py` & `modbus-wrapper-1.0.3/modbus_wrapper/object_factory.py`

 * *Files identical despite different names*

### Comparing `modbus-wrapper-1.0.2b0/modbus_wrapper/objects/fatek_object.py` & `modbus-wrapper-1.0.3/modbus_wrapper/objects/fatek_object.py`

 * *Files identical despite different names*

### Comparing `modbus-wrapper-1.0.2b0/modbus_wrapper/objects/modbus_object.py` & `modbus-wrapper-1.0.3/modbus_wrapper/objects/modbus_object.py`

 * *Files identical despite different names*

### Comparing `modbus-wrapper-1.0.2b0/modbus_wrapper/objects/modbus_value.py` & `modbus-wrapper-1.0.3/modbus_wrapper/objects/modbus_value.py`

 * *Files identical despite different names*

### Comparing `modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/SOURCES.txt` & `modbus-wrapper-1.0.3/modbus_wrapper.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,9 +10,8 @@
 modbus_wrapper.egg-info/dependency_links.txt
 modbus_wrapper.egg-info/requires.txt
 modbus_wrapper.egg-info/top_level.txt
 modbus_wrapper/objects/__init__.py
 modbus_wrapper/objects/config.py
 modbus_wrapper/objects/fatek_object.py
 modbus_wrapper/objects/modbus_object.py
-modbus_wrapper/objects/modbus_value.py
-tests/test_modbus_client_wrapper.py
+modbus_wrapper/objects/modbus_value.py
```

