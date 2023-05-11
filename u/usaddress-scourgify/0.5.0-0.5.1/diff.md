# Comparing `tmp/usaddress-scourgify-0.5.0.tar.gz` & `tmp/usaddress-scourgify-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fable/CodeProjects/GBR/usaddress-scourgify/dist/tmpc3tr4y23/usaddress-scourgify-0.5.0.tar", last modified: Thu May 11 16:01:01 2023, max compression
+gzip compressed data, was "/home/fable/CodeProjects/GBR/usaddress-scourgify/dist/tmpxmlbt_kh/usaddress-scourgify-0.5.1.tar", last modified: Thu May 11 16:49:19 2023, max compression
```

## Comparing `usaddress-scourgify-0.5.0.tar` & `usaddress-scourgify-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 20:59:14.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      803 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/scourgify/
--rw-r--r--   0 root         (0) root         (0)     1847 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/scourgify/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/scourgify/tests/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/scourgify/tests/test_cleaning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/scourgify/tests/config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/scourgify/tests/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28157 2023-04-28 16:59:53.000000 usaddress-scourgify-0.5.0/scourgify/tests/test_address_normalization.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/scourgify/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4717 2023-04-28 16:59:53.000000 usaddress-scourgify-0.5.0/scourgify/validations.py
--rw-r--r--   0 root         (0) root         (0)     8940 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/scourgify/cleaning.py
--rw-r--r--   0 root         (0) root         (0)    33653 2023-05-11 15:59:51.000000 usaddress-scourgify-0.5.0/scourgify/normalize.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-04-18 16:58:50.000000 usaddress-scourgify-0.5.0/scourgify/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16359 2023-05-11 15:59:51.000000 usaddress-scourgify-0.5.0/scourgify/address_constants.py
--rw-r--r--   0 root         (0) root         (0)      918 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      803 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5591 2023-04-28 16:59:53.000000 usaddress-scourgify-0.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:49:19.000000 usaddress-scourgify-0.5.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:49:19.000000 usaddress-scourgify-0.5.1/usaddress_scourgify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-11 16:49:19.000000 usaddress-scourgify-0.5.1/usaddress_scourgify.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 16:49:19.000000 usaddress-scourgify-0.5.1/usaddress_scourgify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 20:59:14.000000 usaddress-scourgify-0.5.1/usaddress_scourgify.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-11 16:49:19.000000 usaddress-scourgify-0.5.1/usaddress_scourgify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-11 16:49:19.000000 usaddress-scourgify-0.5.1/usaddress_scourgify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      803 2023-05-11 16:49:19.000000 usaddress-scourgify-0.5.1/usaddress_scourgify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.1/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:49:19.000000 usaddress-scourgify-0.5.1/scourgify/
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.1/scourgify/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:49:19.000000 usaddress-scourgify-0.5.1/scourgify/tests/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.1/scourgify/tests/test_cleaning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:49:19.000000 usaddress-scourgify-0.5.1/scourgify/tests/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.1/scourgify/tests/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28157 2023-04-28 16:59:53.000000 usaddress-scourgify-0.5.1/scourgify/tests/test_address_normalization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.1/scourgify/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4717 2023-04-28 16:59:53.000000 usaddress-scourgify-0.5.1/scourgify/validations.py
+-rw-r--r--   0 root         (0) root         (0)     8940 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.1/scourgify/cleaning.py
+-rw-r--r--   0 root         (0) root         (0)    33653 2023-05-11 15:59:51.000000 usaddress-scourgify-0.5.1/scourgify/normalize.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-18 16:58:50.000000 usaddress-scourgify-0.5.1/scourgify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16421 2023-05-11 16:31:53.000000 usaddress-scourgify-0.5.1/scourgify/address_constants.py
+-rw-r--r--   0 root         (0) root         (0)      918 2023-05-11 16:49:19.000000 usaddress-scourgify-0.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)      803 2023-05-11 16:49:19.000000 usaddress-scourgify-0.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5591 2023-04-28 16:59:53.000000 usaddress-scourgify-0.5.1/README.rst
```

### Comparing `usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/SOURCES.txt` & `usaddress-scourgify-0.5.1/usaddress_scourgify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/PKG-INFO` & `usaddress-scourgify-0.5.1/usaddress_scourgify.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usaddress-scourgify
-Version: 0.5.0
+Version: 0.5.1
 Summary: Clean US addresses following USPS pub 28 and RESO guidelines
 Home-page: https://github.com/GreenBuildingRegistry/usaddress-scourgify
 Author: Fable Turas
 Author-email: fable@rainsoftware.tech
 Maintainer: GreenBuildingRegistry
 Maintainer-email: admin@greenbuildingregistry.com
 License: UNKNOWN
```

### Comparing `usaddress-scourgify-0.5.0/LICENSE` & `usaddress-scourgify-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.5.0/scourgify/exceptions.py` & `usaddress-scourgify-0.5.1/scourgify/exceptions.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.5.0/scourgify/tests/test_cleaning.py` & `usaddress-scourgify-0.5.1/scourgify/tests/test_cleaning.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.5.0/scourgify/tests/test_address_normalization.py` & `usaddress-scourgify-0.5.1/scourgify/tests/test_address_normalization.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.5.0/scourgify/validations.py` & `usaddress-scourgify-0.5.1/scourgify/validations.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.5.0/scourgify/cleaning.py` & `usaddress-scourgify-0.5.1/scourgify/cleaning.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.5.0/scourgify/normalize.py` & `usaddress-scourgify-0.5.1/scourgify/normalize.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.5.0/scourgify/address_constants.py` & `usaddress-scourgify-0.5.1/scourgify/address_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,18 @@
     'NORTHWEST': 'NW',
     'SOUTHEAST': 'SE',
     'SOUTHWEST': 'SW'
 }
 
 CITY_ABBREVIATIONS = {v: k for k, v in DIRECTIONAL_REPLACEMENTS.items()}
 CITY_ABBRS = {
-    'ST': 'SAINT'
+    'ST': 'SAINT',
+    'MT': 'MOUNT',
+    'FT': 'FORT',
+    'VA': 'VIRGINIA'
 }
 CITY_ABBREVIATIONS.update(CITY_ABBRS)
 
 STREET_TYPE_ABBREVIATIONS = {
     'ALLEE': 'ALY',
     'ALLEY': 'ALY',
     'ALLY': 'ALY',
```

### Comparing `usaddress-scourgify-0.5.0/setup.cfg` & `usaddress-scourgify-0.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = usaddress-scourgify
-version = 0.5.0
+version = 0.5.1
 description = Clean US addresses following USPS pub 28 and RESO guidelines
 author = Fable Turas
 author_email = fable@rainsoftware.tech
 maintainer = GreenBuildingRegistry
 maintainer_email = admin@greenbuildingregistry.com
 keywords = usaddress, normalization, address
 url = https://github.com/GreenBuildingRegistry/usaddress-scourgify
```

### Comparing `usaddress-scourgify-0.5.0/PKG-INFO` & `usaddress-scourgify-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usaddress-scourgify
-Version: 0.5.0
+Version: 0.5.1
 Summary: Clean US addresses following USPS pub 28 and RESO guidelines
 Home-page: https://github.com/GreenBuildingRegistry/usaddress-scourgify
 Author: Fable Turas
 Author-email: fable@rainsoftware.tech
 Maintainer: GreenBuildingRegistry
 Maintainer-email: admin@greenbuildingregistry.com
 License: UNKNOWN
```

### Comparing `usaddress-scourgify-0.5.0/README.rst` & `usaddress-scourgify-0.5.1/README.rst`

 * *Files identical despite different names*

