# Comparing `tmp/journify-python-sdk-2.2.3.tar.gz` & `tmp/journify-python-sdk-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "journify-python-sdk-2.2.3.tar", last modified: Thu May 11 13:34:27 2023, max compression
+gzip compressed data, was "journify-python-sdk-2.2.4.tar", last modified: Thu May 11 13:44:52 2023, max compression
```

## Comparing `journify-python-sdk-2.2.3.tar` & `journify-python-sdk-2.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 slimane    (501) staff       (20)        0 2023-05-11 13:34:27.830491 journify-python-sdk-2.2.3/
--rw-r--r--   0 slimane    (501) staff       (20)     1079 2023-05-11 12:57:01.000000 journify-python-sdk-2.2.3/LICENSE
--rw-r--r--   0 slimane    (501) staff       (20)     1158 2023-05-11 13:34:27.830557 journify-python-sdk-2.2.3/PKG-INFO
--rw-r--r--   0 slimane    (501) staff       (20)     5536 2023-05-08 12:44:35.000000 journify-python-sdk-2.2.3/README.md
-drwxr-xr-x   0 slimane    (501) staff       (20)        0 2023-05-11 13:34:27.828272 journify-python-sdk-2.2.3/journify/
--rw-r--r--   0 slimane    (501) staff       (20)     2029 2023-05-09 11:58:31.000000 journify-python-sdk-2.2.3/journify/__init__.py
--rw-r--r--   0 slimane    (501) staff       (20)     9425 2023-05-10 14:15:28.000000 journify-python-sdk-2.2.3/journify/client.py
--rw-r--r--   0 slimane    (501) staff       (20)     4490 2023-05-10 16:09:24.000000 journify-python-sdk-2.2.3/journify/consumer.py
--rw-r--r--   0 slimane    (501) staff       (20)     2230 2023-05-10 16:09:24.000000 journify-python-sdk-2.2.3/journify/request.py
-drwxr-xr-x   0 slimane    (501) staff       (20)        0 2023-05-11 13:34:27.829517 journify-python-sdk-2.2.3/journify/test/
--rw-r--r--   0 slimane    (501) staff       (20)     2406 2023-05-10 16:02:37.000000 journify-python-sdk-2.2.3/journify/test/__init__.py
--rw-r--r--   0 slimane    (501) staff       (20)    10852 2023-05-10 15:17:34.000000 journify-python-sdk-2.2.3/journify/test/client.py
--rw-r--r--   0 slimane    (501) staff       (20)     3004 2023-05-10 16:06:08.000000 journify-python-sdk-2.2.3/journify/test/consumer.py
--rw-r--r--   0 slimane    (501) staff       (20)     1030 2023-05-10 16:03:27.000000 journify-python-sdk-2.2.3/journify/test/module.py
--rw-r--r--   0 slimane    (501) staff       (20)     2156 2023-05-10 15:13:26.000000 journify-python-sdk-2.2.3/journify/test/request.py
--rw-r--r--   0 slimane    (501) staff       (20)     2151 2023-05-09 15:30:54.000000 journify-python-sdk-2.2.3/journify/test/utils.py
--rw-r--r--   0 slimane    (501) staff       (20)     2425 2023-05-09 12:16:28.000000 journify-python-sdk-2.2.3/journify/utils.py
--rw-r--r--   0 slimane    (501) staff       (20)       41 2023-05-11 13:30:52.000000 journify-python-sdk-2.2.3/journify/version.py
-drwxr-xr-x   0 slimane    (501) staff       (20)        0 2023-05-11 13:34:27.830379 journify-python-sdk-2.2.3/journify_python_sdk.egg-info/
--rw-r--r--   0 slimane    (501) staff       (20)     1158 2023-05-11 13:34:27.000000 journify-python-sdk-2.2.3/journify_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 slimane    (501) staff       (20)      517 2023-05-11 13:34:27.000000 journify-python-sdk-2.2.3/journify_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 slimane    (501) staff       (20)        1 2023-05-11 13:34:27.000000 journify-python-sdk-2.2.3/journify_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 slimane    (501) staff       (20)       85 2023-05-11 13:34:27.000000 journify-python-sdk-2.2.3/journify_python_sdk.egg-info/requires.txt
--rw-r--r--   0 slimane    (501) staff       (20)        9 2023-05-11 13:34:27.000000 journify-python-sdk-2.2.3/journify_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 slimane    (501) staff       (20)       67 2023-05-11 13:34:27.830866 journify-python-sdk-2.2.3/setup.cfg
--rw-r--r--   0 slimane    (501) staff       (20)     1872 2023-05-11 13:05:19.000000 journify-python-sdk-2.2.3/setup.py
+drwxr-xr-x   0 slimane    (501) staff       (20)        0 2023-05-11 13:44:52.226623 journify-python-sdk-2.2.4/
+-rw-r--r--   0 slimane    (501) staff       (20)     1079 2023-05-11 12:57:01.000000 journify-python-sdk-2.2.4/LICENSE
+-rw-r--r--   0 slimane    (501) staff       (20)     1158 2023-05-11 13:44:52.226711 journify-python-sdk-2.2.4/PKG-INFO
+-rw-r--r--   0 slimane    (501) staff       (20)     5536 2023-05-08 12:44:35.000000 journify-python-sdk-2.2.4/README.md
+drwxr-xr-x   0 slimane    (501) staff       (20)        0 2023-05-11 13:44:52.224402 journify-python-sdk-2.2.4/journify/
+-rw-r--r--   0 slimane    (501) staff       (20)     2029 2023-05-09 11:58:31.000000 journify-python-sdk-2.2.4/journify/__init__.py
+-rw-r--r--   0 slimane    (501) staff       (20)     9425 2023-05-10 14:15:28.000000 journify-python-sdk-2.2.4/journify/client.py
+-rw-r--r--   0 slimane    (501) staff       (20)     4490 2023-05-10 16:09:24.000000 journify-python-sdk-2.2.4/journify/consumer.py
+-rw-r--r--   0 slimane    (501) staff       (20)     2230 2023-05-10 16:09:24.000000 journify-python-sdk-2.2.4/journify/request.py
+drwxr-xr-x   0 slimane    (501) staff       (20)        0 2023-05-11 13:44:52.225768 journify-python-sdk-2.2.4/journify/test/
+-rw-r--r--   0 slimane    (501) staff       (20)     2406 2023-05-10 16:02:37.000000 journify-python-sdk-2.2.4/journify/test/__init__.py
+-rw-r--r--   0 slimane    (501) staff       (20)    10852 2023-05-10 15:17:34.000000 journify-python-sdk-2.2.4/journify/test/client.py
+-rw-r--r--   0 slimane    (501) staff       (20)     3004 2023-05-10 16:06:08.000000 journify-python-sdk-2.2.4/journify/test/consumer.py
+-rw-r--r--   0 slimane    (501) staff       (20)     1030 2023-05-10 16:03:27.000000 journify-python-sdk-2.2.4/journify/test/module.py
+-rw-r--r--   0 slimane    (501) staff       (20)     2156 2023-05-10 15:13:26.000000 journify-python-sdk-2.2.4/journify/test/request.py
+-rw-r--r--   0 slimane    (501) staff       (20)     2151 2023-05-09 15:30:54.000000 journify-python-sdk-2.2.4/journify/test/utils.py
+-rw-r--r--   0 slimane    (501) staff       (20)     2425 2023-05-09 12:16:28.000000 journify-python-sdk-2.2.4/journify/utils.py
+-rw-r--r--   0 slimane    (501) staff       (20)       41 2023-05-11 13:44:18.000000 journify-python-sdk-2.2.4/journify/version.py
+drwxr-xr-x   0 slimane    (501) staff       (20)        0 2023-05-11 13:44:52.226504 journify-python-sdk-2.2.4/journify_python_sdk.egg-info/
+-rw-r--r--   0 slimane    (501) staff       (20)     1158 2023-05-11 13:44:52.000000 journify-python-sdk-2.2.4/journify_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 slimane    (501) staff       (20)      517 2023-05-11 13:44:52.000000 journify-python-sdk-2.2.4/journify_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 slimane    (501) staff       (20)        1 2023-05-11 13:44:52.000000 journify-python-sdk-2.2.4/journify_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 slimane    (501) staff       (20)       85 2023-05-11 13:44:52.000000 journify-python-sdk-2.2.4/journify_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 slimane    (501) staff       (20)        9 2023-05-11 13:44:52.000000 journify-python-sdk-2.2.4/journify_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 slimane    (501) staff       (20)       67 2023-05-11 13:44:52.227075 journify-python-sdk-2.2.4/setup.cfg
+-rw-r--r--   0 slimane    (501) staff       (20)     1945 2023-05-11 13:44:25.000000 journify-python-sdk-2.2.4/setup.py
```

### Comparing `journify-python-sdk-2.2.3/LICENSE` & `journify-python-sdk-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/PKG-INFO` & `journify-python-sdk-2.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journify-python-sdk
-Version: 2.2.3
+Version: 2.2.4
 Summary: The hassle-free way to integrate Journify into any python application.
 Home-page: https://github.com/journifyio/journify-python-sdk
 Author: Journify
 Author-email: integrations@journify.io
 Maintainer: Journify
 Maintainer-email: integrations@journify.io
 License: MIT License
```

### Comparing `journify-python-sdk-2.2.3/README.md` & `journify-python-sdk-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/journify/__init__.py` & `journify-python-sdk-2.2.4/journify/__init__.py`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/journify/client.py` & `journify-python-sdk-2.2.4/journify/client.py`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/journify/consumer.py` & `journify-python-sdk-2.2.4/journify/consumer.py`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/journify/request.py` & `journify-python-sdk-2.2.4/journify/request.py`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/journify/test/__init__.py` & `journify-python-sdk-2.2.4/journify/test/__init__.py`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/journify/test/client.py` & `journify-python-sdk-2.2.4/journify/test/client.py`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/journify/test/consumer.py` & `journify-python-sdk-2.2.4/journify/test/consumer.py`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/journify/test/module.py` & `journify-python-sdk-2.2.4/journify/test/module.py`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/journify/test/request.py` & `journify-python-sdk-2.2.4/journify/test/request.py`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/journify/test/utils.py` & `journify-python-sdk-2.2.4/journify/test/utils.py`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/journify/utils.py` & `journify-python-sdk-2.2.4/journify/utils.py`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/journify_python_sdk.egg-info/PKG-INFO` & `journify-python-sdk-2.2.4/journify_python_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journify-python-sdk
-Version: 2.2.3
+Version: 2.2.4
 Summary: The hassle-free way to integrate Journify into any python application.
 Home-page: https://github.com/journifyio/journify-python-sdk
 Author: Journify
 Author-email: integrations@journify.io
 Maintainer: Journify
 Maintainer-email: integrations@journify.io
 License: MIT License
```

### Comparing `journify-python-sdk-2.2.3/journify_python_sdk.egg-info/SOURCES.txt` & `journify-python-sdk-2.2.4/journify_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `journify-python-sdk-2.2.3/setup.py` & `journify-python-sdk-2.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 # Don't import journify-python-sdk module here, since deps may not be installed
 sys.path.insert(0, os.path.join(os.path.dirname(__file__), 'journify'))
 from version import VERSION
 
+# with open("README.md", "r") as fh:
+#     long_description = fh.read()
+
 long_description = '''
 Journify lets marketers unify customer data and deliver personalized experiences – no code or engineering favors required.
 
 This is the official python client that wraps the Journify REST API (https://journify.io).
 
 Documentation and more details at https://github.com/journifyio/journify-python-sdk
 '''
```

