# Comparing `tmp/yasuo-2.0.4.tar.gz` & `tmp/yasuo-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yasuo-2.0.4.tar", last modified: Mon Mar  6 06:41:18 2023, max compression
+gzip compressed data, was "dist/yasuo-3.0.0.tar", last modified: Thu May 11 09:26:39 2023, max compression
```

## Comparing `yasuo-2.0.4.tar` & `yasuo-3.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 06:41:18.000000 yasuo-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-03-06 06:41:18.000000 yasuo-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-03-06 06:41:12.000000 yasuo-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 06:41:18.000000 yasuo-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-06 06:41:12.000000 yasuo-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 06:41:18.000000 yasuo-2.0.4/yasuo/
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-03-06 06:41:12.000000 yasuo-2.0.4/yasuo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 06:41:18.000000 yasuo-2.0.4/yasuo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-03-06 06:41:18.000000 yasuo-2.0.4/yasuo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-06 06:41:18.000000 yasuo-2.0.4/yasuo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 06:41:18.000000 yasuo-2.0.4/yasuo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-06 06:41:18.000000 yasuo-2.0.4/yasuo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-06 06:41:18.000000 yasuo-2.0.4/yasuo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:26:39.000000 yasuo-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-11 09:26:39.000000 yasuo-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-05-11 09:26:26.000000 yasuo-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:26:39.000000 yasuo-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-11 09:26:26.000000 yasuo-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:26:39.000000 yasuo-3.0.0/yasuo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-11 09:26:26.000000 yasuo-3.0.0/yasuo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:26:39.000000 yasuo-3.0.0/yasuo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-11 09:26:39.000000 yasuo-3.0.0/yasuo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-11 09:26:39.000000 yasuo-3.0.0/yasuo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:26:39.000000 yasuo-3.0.0/yasuo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 09:26:39.000000 yasuo-3.0.0/yasuo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 09:26:39.000000 yasuo-3.0.0/yasuo.egg-info/top_level.txt
```

### Comparing `yasuo-2.0.4/PKG-INFO` & `yasuo-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yasuo
-Version: 2.0.4
+Version: 3.0.0
 Summary: A Yasuo Python package
 Home-page: https://github.com/puffer-python/yasuo
 Author: Dung BV
 Author-email: bvdzung@gmail.com
 License: MIT License
 Description: # Yasuo Package
```

### Comparing `yasuo-2.0.4/README.md` & `yasuo-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `yasuo-2.0.4/setup.py` & `yasuo-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `yasuo-2.0.4/yasuo/__init__.py` & `yasuo-3.0.0/yasuo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,37 +15,24 @@
 from datetime import datetime
 
 import pytz
 import unidecode
 from slugify import slugify
 
 __author__ = 'DungBV'
-__patterns = {
-    '[àáảãạăắằẵặẳâầấậẫẩ]': 'a',
-    '[đ]': 'd',
-    '[èéẻẽẹêềếểễệ]': 'e',
-    '[ìíỉĩị]': 'i',
-    '[òóỏõọôồốổỗộơờớởỡợ]': 'o',
-    '[ùúủũụưừứửữự]': 'u',
-    '[ỳýỷỹỵ]': 'y'
-}
 
 
 def convert(text):
     """
     Convert from 'Tieng Viet co dau' thanh 'Tieng Viet khong dau'
     text: input string to be converted
     Return: string converted
     """
-    output = text
-    for regex, replace in __patterns.items():
-        output = re.sub(regex, replace, output)
-        # deal with upper case
-        output = re.sub(regex.upper(), replace.upper(), output)
-    return output
+
+    return unidecode.unidecode(text)
 
 
 def remove_accents(text):
     """
     Convert from 'Tieng Viet co dau' thanh 'Tieng Viet khong dau' using unidecode lib.
     It can process well with multiple percussion
     text: input string to be converted
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yasuo-2.0.4/yasuo.egg-info/PKG-INFO` & `yasuo-3.0.0/yasuo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yasuo
-Version: 2.0.4
+Version: 3.0.0
 Summary: A Yasuo Python package
 Home-page: https://github.com/puffer-python/yasuo
 Author: Dung BV
 Author-email: bvdzung@gmail.com
 License: MIT License
 Description: # Yasuo Package
```

