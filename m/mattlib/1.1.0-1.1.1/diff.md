# Comparing `tmp/mattlib-1.1.0.tar.gz` & `tmp/mattlib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mattlib-1.1.0.tar", last modified: Thu Feb  9 10:30:10 2023, max compression
+gzip compressed data, was "mattlib-1.1.1.tar", last modified: Thu May 11 13:51:43 2023, max compression
```

## Comparing `mattlib-1.1.0.tar` & `mattlib-1.1.1.tar`

### file list

```diff
@@ -1,54 +1,62 @@
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.588549 mattlib-1.1.0/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)    35149 2023-02-07 06:18:37.000000 mattlib-1.1.0/COPYING
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      629 2023-02-09 10:30:10.588549 mattlib-1.1.0/PKG-INFO
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      147 2023-02-07 06:18:37.000000 mattlib-1.1.0/README.md
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      104 2023-02-07 06:18:37.000000 mattlib-1.1.0/pyproject.toml
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      807 2023-02-09 10:30:10.588549 mattlib-1.1.0/setup.cfg
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.548553 mattlib-1.1.0/src/
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.558552 mattlib-1.1.0/src/mattlib/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      733 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/API_factory.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     3228 2023-02-09 10:15:23.000000 mattlib-1.1.0/src/mattlib/BaseAPI.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      193 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/__init__.py
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.568551 mattlib-1.1.0/src/mattlib/adobe/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     3332 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/adobe/AdobeAPI.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)       30 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/adobe/__init__.py
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.568551 mattlib-1.1.0/src/mattlib/clockify/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      751 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/clockify/ClockifyAPI.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)       26 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/clockify/__init__.py
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.568551 mattlib-1.1.0/src/mattlib/fourmatters/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     8016 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/fourmatters/virtual_machine.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     2964 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/fourmatters/virtual_network.py
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.568551 mattlib-1.1.0/src/mattlib/gcp/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      484 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/gcp/PubSub.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)       21 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/gcp/__init__.py
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.568551 mattlib-1.1.0/src/mattlib/google/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     1116 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/google/BaseGoogleAPI.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     1061 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/google/GCPAPI.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     1175 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/google/GoogleWorkspaceAPI.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      484 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/google/PubSub.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     1483 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/google/SQL.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      750 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/google/Storage.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      139 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/google/__init__.py
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.568551 mattlib-1.1.0/src/mattlib/microsoft/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)    18681 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/microsoft/AzureAPI.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     2022 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/microsoft/BaseMicrosoftAPI.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     5469 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/microsoft/GraphAPI.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)       61 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/microsoft/__init__.py
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.568551 mattlib-1.1.0/src/mattlib/network/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     1373 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/network/HttpListener.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)       39 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/network/__init__.py
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.568551 mattlib-1.1.0/src/mattlib/salesforce/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     6366 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/salesforce/SalesForceAPI.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)       41 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/salesforce/__init__.py
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.578550 mattlib-1.1.0/src/mattlib/system/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     1370 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/system/Logger.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)       27 2023-02-08 14:26:16.000000 mattlib-1.1.0/src/mattlib/system/__init__.py
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.568551 mattlib-1.1.0/src/mattlib.egg-info/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      629 2023-02-09 10:30:10.000000 mattlib-1.1.0/src/mattlib.egg-info/PKG-INFO
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)     1173 2023-02-09 10:30:10.000000 mattlib-1.1.0/src/mattlib.egg-info/SOURCES.txt
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)        1 2023-02-09 10:30:10.000000 mattlib-1.1.0/src/mattlib.egg-info/dependency_links.txt
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)       91 2023-02-09 10:30:10.000000 mattlib-1.1.0/src/mattlib.egg-info/requires.txt
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)        8 2023-02-09 10:30:10.000000 mattlib-1.1.0/src/mattlib.egg-info/top_level.txt
-drwxr-xr-x   0 henrique_furst  (1000) henrique_furst  (1000)        0 2023-02-09 10:30:10.588549 mattlib-1.1.0/test/
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      628 2023-02-07 06:18:37.000000 mattlib-1.1.0/test/test_salesforce.py
--rw-r--r--   0 henrique_furst  (1000) henrique_furst  (1000)      766 2023-02-07 06:18:37.000000 mattlib-1.1.0/test/test_vm_size.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:43.161818 mattlib-1.1.1/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)    35149 2023-03-10 11:27:09.000000 mattlib-1.1.1/COPYING
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      629 2023-05-11 13:51:43.165368 mattlib-1.1.1/PKG-INFO
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      147 2023-03-10 11:27:09.000000 mattlib-1.1.1/README.md
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      104 2023-03-10 11:27:09.000000 mattlib-1.1.1/pyproject.toml
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      807 2023-05-11 13:51:43.180780 mattlib-1.1.1/setup.cfg
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:37.394494 mattlib-1.1.1/src/
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:38.060405 mattlib-1.1.1/src/mattlib/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      733 2023-03-10 11:27:09.000000 mattlib-1.1.1/src/mattlib/API_factory.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     2143 2023-03-10 11:27:09.000000 mattlib-1.1.1/src/mattlib/BaseAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      193 2023-03-10 11:27:09.000000 mattlib-1.1.1/src/mattlib/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:38.779850 mattlib-1.1.1/src/mattlib/adobe/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     3332 2023-03-10 11:27:09.000000 mattlib-1.1.1/src/mattlib/adobe/AdobeAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       30 2023-03-10 11:27:09.000000 mattlib-1.1.1/src/mattlib/adobe/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:39.465165 mattlib-1.1.1/src/mattlib/apis/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)    10010 2023-03-10 11:27:10.000000 mattlib-1.1.1/src/mattlib/apis/AzureAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1917 2023-03-10 11:27:10.000000 mattlib-1.1.1/src/mattlib/apis/GraphAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     4355 2023-03-10 11:27:10.000000 mattlib-1.1.1/src/mattlib/apis/SalesForceAPI.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:39.732568 mattlib-1.1.1/src/mattlib/clockify/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      751 2023-03-10 11:27:10.000000 mattlib-1.1.1/src/mattlib/clockify/ClockifyAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       26 2023-03-10 11:27:10.000000 mattlib-1.1.1/src/mattlib/clockify/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:40.099769 mattlib-1.1.1/src/mattlib/fourmatters/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     8016 2023-03-10 11:27:10.000000 mattlib-1.1.1/src/mattlib/fourmatters/virtual_machine.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     2964 2023-03-10 11:27:10.000000 mattlib-1.1.1/src/mattlib/fourmatters/virtual_network.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:40.325999 mattlib-1.1.1/src/mattlib/gcp/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      484 2023-03-10 11:27:10.000000 mattlib-1.1.1/src/mattlib/gcp/PubSub.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       21 2023-03-10 11:27:10.000000 mattlib-1.1.1/src/mattlib/gcp/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:41.309523 mattlib-1.1.1/src/mattlib/google/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1116 2023-03-10 11:27:10.000000 mattlib-1.1.1/src/mattlib/google/BaseGoogleAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1061 2023-03-10 11:27:10.000000 mattlib-1.1.1/src/mattlib/google/GCPAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1175 2023-03-10 11:27:10.000000 mattlib-1.1.1/src/mattlib/google/GoogleWorkspaceAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      484 2023-03-10 11:27:11.000000 mattlib-1.1.1/src/mattlib/google/PubSub.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1483 2023-03-10 11:27:11.000000 mattlib-1.1.1/src/mattlib/google/SQL.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      750 2023-03-10 11:27:11.000000 mattlib-1.1.1/src/mattlib/google/Storage.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      139 2023-03-10 11:27:11.000000 mattlib-1.1.1/src/mattlib/google/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:41.360427 mattlib-1.1.1/src/mattlib/http/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1302 2023-03-10 11:27:11.000000 mattlib-1.1.1/src/mattlib/http/HttpListener.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:41.429593 mattlib-1.1.1/src/mattlib/logger/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1370 2023-03-10 11:27:11.000000 mattlib-1.1.1/src/mattlib/logger/Logger.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:41.885645 mattlib-1.1.1/src/mattlib/microsoft/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)    18681 2023-03-16 17:34:31.000000 mattlib-1.1.1/src/mattlib/microsoft/AzureAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     2053 2023-03-16 17:46:32.000000 mattlib-1.1.1/src/mattlib/microsoft/BaseMicrosoftAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     5150 2023-05-11 13:24:14.000000 mattlib-1.1.1/src/mattlib/microsoft/GraphAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       61 2023-03-10 11:27:11.000000 mattlib-1.1.1/src/mattlib/microsoft/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:42.151879 mattlib-1.1.1/src/mattlib/network/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1373 2023-03-10 11:27:11.000000 mattlib-1.1.1/src/mattlib/network/HttpListener.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       39 2023-03-10 11:27:11.000000 mattlib-1.1.1/src/mattlib/network/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:42.611659 mattlib-1.1.1/src/mattlib/salesforce/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     6292 2023-05-09 22:10:30.000000 mattlib-1.1.1/src/mattlib/salesforce/SalesForceAPI.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       41 2023-03-10 11:27:11.000000 mattlib-1.1.1/src/mattlib/salesforce/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:42.877521 mattlib-1.1.1/src/mattlib/system/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1370 2023-03-10 11:27:11.000000 mattlib-1.1.1/src/mattlib/system/Logger.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       27 2023-03-10 11:27:11.000000 mattlib-1.1.1/src/mattlib/system/__init__.py
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:38.429556 mattlib-1.1.1/src/mattlib.egg-info/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      629 2023-05-11 13:51:36.000000 mattlib-1.1.1/src/mattlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 livia     (1000) livia     (1000)     1327 2023-05-11 13:51:37.000000 mattlib-1.1.1/src/mattlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 livia     (1000) livia     (1000)        1 2023-05-11 13:51:36.000000 mattlib-1.1.1/src/mattlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 livia     (1000) livia     (1000)       91 2023-05-11 13:51:36.000000 mattlib-1.1.1/src/mattlib.egg-info/requires.txt
+-rwxrwxrwx   0 livia     (1000) livia     (1000)        8 2023-05-11 13:51:36.000000 mattlib-1.1.1/src/mattlib.egg-info/top_level.txt
+drwxrwxrwx   0 livia     (1000) livia     (1000)        0 2023-05-11 13:51:43.065086 mattlib-1.1.1/test/
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      628 2023-03-10 11:27:11.000000 mattlib-1.1.1/test/test_salesforce.py
+-rwxrwxrwx   0 livia     (1000) livia     (1000)      766 2023-03-10 11:27:11.000000 mattlib-1.1.1/test/test_vm_size.py
```

### Comparing `mattlib-1.1.0/COPYING` & `mattlib-1.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/PKG-INFO` & `mattlib-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattlib
-Version: 1.1.0
+Version: 1.1.1
 Summary: API data extraction and formatting utilities.
 Home-page: https://source.cloud.google.com/mtz-repos-global/mattlib
 Author: 4matt
 Author-email: mattzero@4matt.com.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mattlib-1.1.0/setup.cfg` & `mattlib-1.1.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mattlib
-version = 1.1.0
+version = 1.1.1
 author = 4matt
 author_email = mattzero@4matt.com.br
 description = API data extraction and formatting utilities.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://source.cloud.google.com/mtz-repos-global/mattlib
 classifiers =
```

### Comparing `mattlib-1.1.0/src/mattlib/API_factory.py` & `mattlib-1.1.1/src/mattlib/API_factory.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib/adobe/AdobeAPI.py` & `mattlib-1.1.1/src/mattlib/adobe/AdobeAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib/clockify/ClockifyAPI.py` & `mattlib-1.1.1/src/mattlib/clockify/ClockifyAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib/fourmatters/virtual_machine.py` & `mattlib-1.1.1/src/mattlib/fourmatters/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib/fourmatters/virtual_network.py` & `mattlib-1.1.1/src/mattlib/fourmatters/virtual_network.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib/google/BaseGoogleAPI.py` & `mattlib-1.1.1/src/mattlib/google/BaseGoogleAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib/google/GCPAPI.py` & `mattlib-1.1.1/src/mattlib/google/GCPAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib/google/GoogleWorkspaceAPI.py` & `mattlib-1.1.1/src/mattlib/google/GoogleWorkspaceAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib/google/SQL.py` & `mattlib-1.1.1/src/mattlib/google/SQL.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib/google/Storage.py` & `mattlib-1.1.1/src/mattlib/google/Storage.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib/microsoft/AzureAPI.py` & `mattlib-1.1.1/src/mattlib/microsoft/AzureAPI.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib/microsoft/BaseMicrosoftAPI.py` & `mattlib-1.1.1/src/mattlib/microsoft/BaseMicrosoftAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         auth = {
             'grant_type': 'client_credentials',
             'client_id': self.app_ID,
             'client_secret': self.secret_key,
             'scope': self.scope,
         }
         response = requests.post(token_url, data=auth)
+        print(response.json())
         token = response.json().get('access_token')
         if token != None:
             headers = {'Authorization': f'Bearer {token}'}
             return headers
         else:
             raise Exception(f' BaseMicrosoftAPI authentication failed.\n'\
                             f'Response: {response}')
```

### Comparing `mattlib-1.1.0/src/mattlib/microsoft/GraphAPI.py` & `mattlib-1.1.1/src/mattlib/microsoft/GraphAPI.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,56 @@
 from .BaseMicrosoftAPI import BaseMicrosoftAPI
 import requests
 
 class GraphAPI(BaseMicrosoftAPI):
-    def connect(self, tenant_ID: str, app_ID: str, secret_key: str) -> None:
+    def connect(self, tenant_ID, app_ID, secret_key):
        super().connect(tenant_ID, app_ID, secret_key,
                         'https://graph.microsoft.com/.default')
 
-    def list_users(self, properties=None) -> dict:
+    def list_users(self, properties=None):
         if properties:
             parameters = ','.join(properties)
             url = f'https://graph.microsoft.com/v1.0/users?$top=999&$select={parameters}'
         else:
-            url = 'https://graph.microsoft.com/v1.0/users'
+            parameters = "userPrincipalName,preferredLanguage,id,officeLocation,mobilePhone,mail,jobTitle,"\
+                "givenName,licenseAssignmentStates,userType,provisionedPlans,assignedPlans"
+            url = f'https://graph.microsoft.com/v1.0/users?$top=999&$select={parameters}'
         response = self.call_api(url)
         return response
 
-    def list_subscribed_skus(self) -> dict:
+    def list_subscribed_skus(self):
         url = 'https://graph.microsoft.com/v1.0/subscribedSkus'
         response = self.call_api(url)
         return response
 
-    def list_organizations(self) -> dict:
+    def list_organizations(self):
         url = 'https://graph.microsoft.com/v1.0/organization'
         response = self.call_api(url)
         return response
 
-    def get_details(self,
-                    listParamsExtract=[
-                        'getOneDriveUsageAccountDetail',
-                        'getOneDriveActivityUserDetail',
-                        'getTeamsDeviceUsageUserDetail',
-                        'getTeamsUserActivityUserDetail',
-                        'getEmailActivityUserDetail',
-                        'getEmailAppUsageUserDetail',
-                        'getSharePointActivityUserDetail',
-                        'getSharePointSiteUsageDetail',
-                    ],
-                    paramsData=('period',7)) -> list:
+    def get_details(self, listParamsExtract, paramsData):
         results = []
-        supported_paramsExtract = [
-            'getOneDriveUsageAccountDetail',
-            'getOneDriveActivityUserDetail',
-            'getTeamsDeviceUsageUserDetail',
-            'getTeamsUserActivityUserDetail',
-            'getEmailActivityUserDetail',
-            'getEmailAppUsageUserDetail',
-            'getSharePointActivityUserDetail',
-            'getSharePointSiteUsageDetail',
-            'getSkypeForBusinessActivityUserDetail',
-            'getSkypeForBusinessDeviceUsageUserDetail',
-            'getYammerActivityUserDetail',
-            'getYammerDeviceUsageUserDetail',
-            'getOffice365ActiveUserDetail'
-        ]
         for item in listParamsExtract:
+
+            supported_paramsExtract = [
+                'getOneDriveUsageAccountDetail',
+                'getOneDriveActivityUserDetail',
+                'getTeamsDeviceUsageUserDetail',
+                'getTeamsUserActivityUserDetail',
+                'getEmailActivityUserDetail',
+                'getEmailAppUsageUserDetail',
+                'getSharePointActivityUserDetail',
+                'getSharePointSiteUsageDetail',
+                'getSkypeForBusinessActivityUserDetail',
+                'getSkypeForBusinessDeviceUsageUserDetail',
+                'getYammerActivityUserDetail',
+                'getYammerDeviceUsageUserDetail',
+                'getOffice365ActiveUserDetail'
+            ]
+
             if paramsData[0] == 'period':
                 supported_paramsExtract+=['getSkypeForBusinessOrganizerActivityUserCounts',\
                     'getMailboxUsageDetail','getMailboxUsageStorage']
 
             if item not in supported_paramsExtract:
                 print(f'Parameter not supported {item} \n'\
                     f'Supported parameters: {supported_paramsExtract}')
@@ -69,44 +62,44 @@
                             f"{item}(period='D{paramsData[1]}')",
                 'date': f"https://graph.microsoft.com/v1.0/reports/"\
                         f"{item}(date={paramsData[1]})"
                 }
 
                 url = urls.get(paramsData[0])
                 response = self.call_api_stream(url)
-                results.append((item, response))
+                results.append(response)
 
         return results
 
-    def office365_active_user_detail(self, params=('period', '7')) -> str:
+    def office365_active_user_detail(self, params=('period', '7')):
         urls = {
             'period': f"https://graph.microsoft.com/v1.0/reports/"\
                       f"getOffice365ActiveUserDetail(period='D{params[1]}')",
             'date': f"http://graph.microsoft.com/v1.0/reports/"\
                     f"getOffice365ActiveUserDetail(date={params[1]})"
         }
 
         url = urls.get(params[0])
         response = self.call_api_stream(url)
         return response
 
-    def office365_mailbox_usage_detail(self, period=7) -> str:
+    def office365_mailbox_usage_detail(self, period=7):
         supported_periods = [7, 30, 90, 180]
         if period not in supported_periods:
             print(f'office_365_mailbox_usage_detail: please use one of'\
                   f'supported periods: {period}')
             # raise error
             return None
         else:
             url = f"https://graph.microsoft.com/v1.0/reports/"\
                   f"getMailboxUsageDetail(period='D{period}')"
             response = self.call_api_stream(url)
             return response
 
-    def methods(self) -> str:
+    def methods(self):
         methods = [
             {
                 'method_name': 'list_users',
                 'method': self.list_users,
                 'format': 'json'
             },
             {
@@ -128,15 +121,15 @@
                 'method_name': 'list_organizations',
                 'method': self.list_organizations,
                 'format': 'json'
             },
             {
                 'method_name': 'get_details',
                 'method': self.get_details,
-                'format': 'csv_list'
+                'format': 'list_csv'
             },
         ]
         return methods
 
 # Possibilities --------------------------------------------------------------
 # users/delta
 #    def office365_services_user_counts(self):
```

### Comparing `mattlib-1.1.0/src/mattlib/network/HttpListener.py` & `mattlib-1.1.1/src/mattlib/network/HttpListener.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib/salesforce/SalesForceAPI.py` & `mattlib-1.1.1/src/mattlib/salesforce/SalesForceAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,15 @@
         self.consumer_key = consumer_key.rstrip()
         self.consumer_secret = consumer_secret.rstrip()
         self.username = username.rstrip()
         self.password = password.rstrip()
         self.url = f'https://{self.domain}.my.salesforce.com'
         if self.type == 'username-password':
             self.headers = self.__get_auth_user()
-        if type == 'web server':
-            self.headers = self.__get_auth_web_server(authorization)
+        print(self.headers)
         # headers must be: 
         # { 'Authorization': <token>, 'X-PrettyPrint': 1 }
 
     def __get_auth_user(self):
         domain = self.domain
         auth = {
             'grant_type': 'password',
```

### Comparing `mattlib-1.1.0/src/mattlib/system/Logger.py` & `mattlib-1.1.1/src/mattlib/logger/Logger.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/src/mattlib.egg-info/PKG-INFO` & `mattlib-1.1.1/src/mattlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mattlib
-Version: 1.1.0
+Version: 1.1.1
 Summary: API data extraction and formatting utilities.
 Home-page: https://source.cloud.google.com/mtz-repos-global/mattlib
 Author: 4matt
 Author-email: mattzero@4matt.com.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mattlib-1.1.0/src/mattlib.egg-info/SOURCES.txt` & `mattlib-1.1.1/src/mattlib.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,27 +8,32 @@
 src/mattlib.egg-info/PKG-INFO
 src/mattlib.egg-info/SOURCES.txt
 src/mattlib.egg-info/dependency_links.txt
 src/mattlib.egg-info/requires.txt
 src/mattlib.egg-info/top_level.txt
 src/mattlib/adobe/AdobeAPI.py
 src/mattlib/adobe/__init__.py
+src/mattlib/apis/AzureAPI.py
+src/mattlib/apis/GraphAPI.py
+src/mattlib/apis/SalesForceAPI.py
 src/mattlib/clockify/ClockifyAPI.py
 src/mattlib/clockify/__init__.py
 src/mattlib/fourmatters/virtual_machine.py
 src/mattlib/fourmatters/virtual_network.py
 src/mattlib/gcp/PubSub.py
 src/mattlib/gcp/__init__.py
 src/mattlib/google/BaseGoogleAPI.py
 src/mattlib/google/GCPAPI.py
 src/mattlib/google/GoogleWorkspaceAPI.py
 src/mattlib/google/PubSub.py
 src/mattlib/google/SQL.py
 src/mattlib/google/Storage.py
 src/mattlib/google/__init__.py
+src/mattlib/http/HttpListener.py
+src/mattlib/logger/Logger.py
 src/mattlib/microsoft/AzureAPI.py
 src/mattlib/microsoft/BaseMicrosoftAPI.py
 src/mattlib/microsoft/GraphAPI.py
 src/mattlib/microsoft/__init__.py
 src/mattlib/network/HttpListener.py
 src/mattlib/network/__init__.py
 src/mattlib/salesforce/SalesForceAPI.py
```

### Comparing `mattlib-1.1.0/test/test_salesforce.py` & `mattlib-1.1.1/test/test_salesforce.py`

 * *Files identical despite different names*

### Comparing `mattlib-1.1.0/test/test_vm_size.py` & `mattlib-1.1.1/test/test_vm_size.py`

 * *Files identical despite different names*

