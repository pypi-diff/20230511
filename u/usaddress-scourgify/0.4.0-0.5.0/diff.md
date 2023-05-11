# Comparing `tmp/usaddress-scourgify-0.4.0.tar.gz` & `tmp/usaddress-scourgify-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fable/CodeProjects/GBR/usaddress-scourgify/dist/tmp7eec17wl/usaddress-scourgify-0.4.0.tar", last modified: Wed Apr 19 18:17:29 2023, max compression
+gzip compressed data, was "/home/fable/CodeProjects/GBR/usaddress-scourgify/dist/tmpc3tr4y23/usaddress-scourgify-0.5.0.tar", last modified: Thu May 11 16:01:01 2023, max compression
```

## Comparing `usaddress-scourgify-0.4.0.tar` & `usaddress-scourgify-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 20:59:14.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      803 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/scourgify/
--rw-r--r--   0 root         (0) root         (0)     1847 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/scourgify/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/scourgify/tests/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/scourgify/tests/test_cleaning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/scourgify/tests/config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/scourgify/tests/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28157 2023-04-19 18:10:27.000000 usaddress-scourgify-0.4.0/scourgify/tests/test_address_normalization.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/scourgify/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4717 2023-04-19 18:09:29.000000 usaddress-scourgify-0.4.0/scourgify/validations.py
--rw-r--r--   0 root         (0) root         (0)     8940 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/scourgify/cleaning.py
--rw-r--r--   0 root         (0) root         (0)    33255 2023-04-19 17:21:34.000000 usaddress-scourgify-0.4.0/scourgify/normalize.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-04-18 16:58:50.000000 usaddress-scourgify-0.4.0/scourgify/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16206 2023-04-18 16:58:50.000000 usaddress-scourgify-0.4.0/scourgify/address_constants.py
--rw-r--r--   0 root         (0) root         (0)      918 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-17 20:22:48.000000 usaddress-scourgify-0.4.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      803 2023-04-19 18:17:29.000000 usaddress-scourgify-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5591 2023-04-19 17:55:25.000000 usaddress-scourgify-0.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 20:59:14.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      803 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/scourgify/
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/scourgify/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/scourgify/tests/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/scourgify/tests/test_cleaning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/scourgify/tests/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/scourgify/tests/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28157 2023-04-28 16:59:53.000000 usaddress-scourgify-0.5.0/scourgify/tests/test_address_normalization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/scourgify/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4717 2023-04-28 16:59:53.000000 usaddress-scourgify-0.5.0/scourgify/validations.py
+-rw-r--r--   0 root         (0) root         (0)     8940 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/scourgify/cleaning.py
+-rw-r--r--   0 root         (0) root         (0)    33653 2023-05-11 15:59:51.000000 usaddress-scourgify-0.5.0/scourgify/normalize.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-18 16:58:50.000000 usaddress-scourgify-0.5.0/scourgify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16359 2023-05-11 15:59:51.000000 usaddress-scourgify-0.5.0/scourgify/address_constants.py
+-rw-r--r--   0 root         (0) root         (0)      918 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-17 20:22:48.000000 usaddress-scourgify-0.5.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      803 2023-05-11 16:01:01.000000 usaddress-scourgify-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5591 2023-04-28 16:59:53.000000 usaddress-scourgify-0.5.0/README.rst
```

### Comparing `usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/SOURCES.txt` & `usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.4.0/usaddress_scourgify.egg-info/PKG-INFO` & `usaddress-scourgify-0.5.0/usaddress_scourgify.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usaddress-scourgify
-Version: 0.4.0
+Version: 0.5.0
 Summary: Clean US addresses following USPS pub 28 and RESO guidelines
 Home-page: https://github.com/GreenBuildingRegistry/usaddress-scourgify
 Author: Fable Turas
 Author-email: fable@rainsoftware.tech
 Maintainer: GreenBuildingRegistry
 Maintainer-email: admin@greenbuildingregistry.com
 License: UNKNOWN
```

### Comparing `usaddress-scourgify-0.4.0/LICENSE` & `usaddress-scourgify-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.4.0/scourgify/exceptions.py` & `usaddress-scourgify-0.5.0/scourgify/exceptions.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.4.0/scourgify/tests/test_cleaning.py` & `usaddress-scourgify-0.5.0/scourgify/tests/test_cleaning.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.4.0/scourgify/tests/test_address_normalization.py` & `usaddress-scourgify-0.5.0/scourgify/tests/test_address_normalization.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.4.0/scourgify/validations.py` & `usaddress-scourgify-0.5.0/scourgify/validations.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.4.0/scourgify/cleaning.py` & `usaddress-scourgify-0.5.0/scourgify/cleaning.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.4.0/scourgify/normalize.py` & `usaddress-scourgify-0.5.0/scourgify/normalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 import geocoder
 import usaddress
 
 # Local Imports
 from scourgify.address_constants import (
     ABNORMAL_OCCUPANCY_ABBRVS,
     ADDRESS_KEYS,
+    CITY_ABBREVIATIONS,
     DIRECTIONAL_REPLACEMENTS,
     OCCUPANCY_TYPE_ABBREVIATIONS,
     STATE_ABBREVIATIONS,
     STREET_TYPE_ABBREVIATIONS,
 )
 from scourgify.cleaning import (
     clean_upper,
@@ -576,14 +577,23 @@
     if state:
         state_abbrv = STATE_ABBREVIATIONS.get(state.upper())
         if state_abbrv:
             state = state_abbrv
     return state
 
 
+def normalize_city(city):
+    city = city.split()
+    for i, part in enumerate(city):
+        replacement = CITY_ABBREVIATIONS.get(part.replace('.', ''))
+        if replacement:
+            city[i] = replacement
+    return ' '.join(city)
+
+
 def get_normalized_line_segment(parsed_addr, line_labels):
     # type: (Mapping[str, str], Sequence[str]) -> str
     """
 
     :param parsed_addr: address parsed into ordereddict per usaddress.
     :param line_labels: tuple of str labels of all the potential keys related
         to the desired address segment (ie address_line_1 or address_line_2).
@@ -767,17 +777,15 @@
                 error = err
 
         if parsed_addr:
             parsed_addr = self.normalize_address_components(parsed_addr)
             zipcode = self.get_parsed_values(
                 parsed_addr, zipcode, 'ZipCode', addr_str
             )
-            city = self.get_parsed_values(
-                parsed_addr, city, 'PlaceName', addr_str
-            )
+            city = self.normalize_city(parsed_addr, addr_str, city)
             state = self.get_parsed_values(
                 parsed_addr, state, 'StateName', addr_str
             )
             state = normalize_state(state)
 
             # assumes if line2 is passed in that it need not be parsed from
             # addr_str. Primarily used to allow advanced processing of
@@ -825,7 +833,12 @@
                 addr_dict, comma_separate=True, addr_parts=ADDRESS_KEYS
             )
             address = self.normalize_addr_str(
                 addr_str, city=city, state=state,
                 zipcode=zipcode
             )
         return address
+
+    def normalize_city(self, parsed_addr, addr_str, city=None):
+        return self.get_parsed_values(
+            parsed_addr, city, 'PlaceName', addr_str
+        )
```

### Comparing `usaddress-scourgify-0.4.0/scourgify/address_constants.py` & `usaddress-scourgify-0.5.0/scourgify/address_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,20 @@
     'SOUTH': 'S',
     'NORTHEAST': 'NE',
     'NORTHWEST': 'NW',
     'SOUTHEAST': 'SE',
     'SOUTHWEST': 'SW'
 }
 
+CITY_ABBREVIATIONS = {v: k for k, v in DIRECTIONAL_REPLACEMENTS.items()}
+CITY_ABBRS = {
+    'ST': 'SAINT'
+}
+CITY_ABBREVIATIONS.update(CITY_ABBRS)
+
 STREET_TYPE_ABBREVIATIONS = {
     'ALLEE': 'ALY',
     'ALLEY': 'ALY',
     'ALLY': 'ALY',
     'ALY': 'ALY',
     'ANEX': 'ANX',
     'ANNEX': 'ANX',
```

### Comparing `usaddress-scourgify-0.4.0/setup.cfg` & `usaddress-scourgify-0.5.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = usaddress-scourgify
-version = 0.4.0
+version = 0.5.0
 description = Clean US addresses following USPS pub 28 and RESO guidelines
 author = Fable Turas
 author_email = fable@rainsoftware.tech
 maintainer = GreenBuildingRegistry
 maintainer_email = admin@greenbuildingregistry.com
 keywords = usaddress, normalization, address
 url = https://github.com/GreenBuildingRegistry/usaddress-scourgify
```

### Comparing `usaddress-scourgify-0.4.0/PKG-INFO` & `usaddress-scourgify-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usaddress-scourgify
-Version: 0.4.0
+Version: 0.5.0
 Summary: Clean US addresses following USPS pub 28 and RESO guidelines
 Home-page: https://github.com/GreenBuildingRegistry/usaddress-scourgify
 Author: Fable Turas
 Author-email: fable@rainsoftware.tech
 Maintainer: GreenBuildingRegistry
 Maintainer-email: admin@greenbuildingregistry.com
 License: UNKNOWN
```

### Comparing `usaddress-scourgify-0.4.0/README.rst` & `usaddress-scourgify-0.5.0/README.rst`

 * *Files identical despite different names*

