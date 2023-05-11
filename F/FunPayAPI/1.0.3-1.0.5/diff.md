# Comparing `tmp/FunPayAPI-1.0.3.tar.gz` & `tmp/FunPayAPI-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FunPayAPI-1.0.3.tar", last modified: Thu May 11 21:40:35 2023, max compression
+gzip compressed data, was "FunPayAPI-1.0.5.tar", last modified: Thu May 11 21:47:12 2023, max compression
```

## Comparing `FunPayAPI-1.0.3.tar` & `FunPayAPI-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 21:40:35.469508 FunPayAPI-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-11 21:40:35.457508 FunPayAPI-1.0.3/FunPayAPI/
--rw-rw-rw-   0        0        0      162 2023-05-10 15:12:44.000000 FunPayAPI-1.0.3/FunPayAPI/__init__.py
--rw-rw-rw-   0        0        0    56139 2023-05-11 20:44:29.000000 FunPayAPI-1.0.3/FunPayAPI/account.py
--rw-rw-rw-   0        0        0    38990 2023-05-11 19:44:24.000000 FunPayAPI-1.0.3/FunPayAPI/types.py
-drwxrwxrwx   0        0        0        0 2023-05-11 21:40:35.468509 FunPayAPI-1.0.3/FunPayAPI.egg-info/
--rw-rw-rw-   0        0        0      557 2023-05-11 21:40:35.000000 FunPayAPI-1.0.3/FunPayAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-11 21:40:35.000000 FunPayAPI-1.0.3/FunPayAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 21:40:35.000000 FunPayAPI-1.0.3/FunPayAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-11 21:40:35.000000 FunPayAPI-1.0.3/FunPayAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 21:40:35.000000 FunPayAPI-1.0.3/FunPayAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35801 2023-05-11 21:13:41.000000 FunPayAPI-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      557 2023-05-11 21:40:35.469508 FunPayAPI-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-11 21:40:35.469508 FunPayAPI-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      756 2023-05-11 21:40:27.000000 FunPayAPI-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:47:12.591760 FunPayAPI-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-11 21:47:12.574760 FunPayAPI-1.0.5/FunPayAPI/
+-rw-rw-rw-   0        0        0      162 2023-05-10 15:12:44.000000 FunPayAPI-1.0.5/FunPayAPI/__init__.py
+-rw-rw-rw-   0        0        0    56139 2023-05-11 20:44:29.000000 FunPayAPI-1.0.5/FunPayAPI/account.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:47:12.588760 FunPayAPI-1.0.5/FunPayAPI/common/
+-rw-rw-rw-   0        0        0        0 2023-05-11 21:46:28.000000 FunPayAPI-1.0.5/FunPayAPI/common/__init__.py
+-rw-rw-rw-   0        0        0     4667 2023-05-11 19:19:43.000000 FunPayAPI-1.0.5/FunPayAPI/common/enums.py
+-rw-rw-rw-   0        0        0     6458 2023-04-14 18:22:19.000000 FunPayAPI-1.0.5/FunPayAPI/common/exceptions.py
+-rw-rw-rw-   0        0        0     8033 2023-04-14 18:22:19.000000 FunPayAPI-1.0.5/FunPayAPI/common/utils.py
+-rw-rw-rw-   0        0        0    38990 2023-05-11 19:44:24.000000 FunPayAPI-1.0.5/FunPayAPI/types.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:47:12.590759 FunPayAPI-1.0.5/FunPayAPI/updater/
+-rw-rw-rw-   0        0        0        0 2023-05-11 21:46:35.000000 FunPayAPI-1.0.5/FunPayAPI/updater/__init__.py
+-rw-rw-rw-   0        0        0     8216 2023-05-11 19:12:41.000000 FunPayAPI-1.0.5/FunPayAPI/updater/events.py
+-rw-rw-rw-   0        0        0    17300 2023-04-14 18:22:19.000000 FunPayAPI-1.0.5/FunPayAPI/updater/runner.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:47:12.586760 FunPayAPI-1.0.5/FunPayAPI.egg-info/
+-rw-rw-rw-   0        0        0      557 2023-05-11 21:47:12.000000 FunPayAPI-1.0.5/FunPayAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-11 21:47:12.000000 FunPayAPI-1.0.5/FunPayAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 21:47:12.000000 FunPayAPI-1.0.5/FunPayAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-11 21:47:12.000000 FunPayAPI-1.0.5/FunPayAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 21:47:12.000000 FunPayAPI-1.0.5/FunPayAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35801 2023-05-11 21:13:41.000000 FunPayAPI-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      557 2023-05-11 21:47:12.591760 FunPayAPI-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-11 21:47:12.591760 FunPayAPI-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      756 2023-05-11 21:46:59.000000 FunPayAPI-1.0.5/setup.py
```

### Comparing `FunPayAPI-1.0.3/FunPayAPI/account.py` & `FunPayAPI-1.0.5/FunPayAPI/account.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.3/FunPayAPI/types.py` & `FunPayAPI-1.0.5/FunPayAPI/types.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.3/FunPayAPI.egg-info/PKG-INFO` & `FunPayAPI-1.0.5/FunPayAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FunPayAPI
-Version: 1.0.3
+Version: 1.0.5
 Summary: Прослойка между FunPayAPI и клиентом.
 Home-page: https://github.com/woopertail/FunPayAPI
 Author: Woopertail
 Author-email: woopertail@gmail.com
 License: GPL2
 Keywords: funpay bot api tools
 Platform: UNKNOWN
```

### Comparing `FunPayAPI-1.0.3/LICENSE` & `FunPayAPI-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.3/PKG-INFO` & `FunPayAPI-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FunPayAPI
-Version: 1.0.3
+Version: 1.0.5
 Summary: Прослойка между FunPayAPI и клиентом.
 Home-page: https://github.com/woopertail/FunPayAPI
 Author: Woopertail
 Author-email: woopertail@gmail.com
 License: GPL2
 Keywords: funpay bot api tools
 Platform: UNKNOWN
```

### Comparing `FunPayAPI-1.0.3/setup.py` & `FunPayAPI-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 
 setup(name='FunPayAPI',
-      version="1.0.3",
+      version="1.0.5",
       description='Прослойка между FunPayAPI и клиентом.',
       author='Woopertail',
       author_email='woopertail@gmail.com',
       url='https://github.com/woopertail/FunPayAPI',
       packages=find_packages("."),
       license='GPL2',
       keywords='funpay bot api tools',
```

