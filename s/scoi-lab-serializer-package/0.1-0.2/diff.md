# Comparing `tmp/scoi_lab_serializer_package-0.1.tar.gz` & `tmp/scoi_lab_serializer_package-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoi_lab_serializer_package-0.1.tar", last modified: Wed May 10 14:53:59 2023, max compression
+gzip compressed data, was "scoi_lab_serializer_package-0.2.tar", last modified: Wed May 10 15:07:40 2023, max compression
```

## Comparing `scoi_lab_serializer_package-0.1.tar` & `scoi_lab_serializer_package-0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:53:59.728988 scoi_lab_serializer_package-0.1/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      433 2023-05-10 14:53:59.728988 scoi_lab_serializer_package-0.1/PKG-INFO
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:53:59.728988 scoi_lab_serializer_package-0.1/scoi_lab_serializer_package.egg-info/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      433 2023-05-10 14:53:59.000000 scoi_lab_serializer_package-0.1/scoi_lab_serializer_package.egg-info/PKG-INFO
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      577 2023-05-10 14:53:59.000000 scoi_lab_serializer_package-0.1/scoi_lab_serializer_package.egg-info/SOURCES.txt
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        1 2023-05-10 14:53:59.000000 scoi_lab_serializer_package-0.1/scoi_lab_serializer_package.egg-info/dependency_links.txt
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)       64 2023-05-10 14:53:59.000000 scoi_lab_serializer_package-0.1/scoi_lab_serializer_package.egg-info/top_level.txt
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:53:59.728988 scoi_lab_serializer_package-0.1/serializers/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:50:53.000000 scoi_lab_serializer_package-0.1/serializers/__init__.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      322 2023-05-08 08:54:46.000000 scoi_lab_serializer_package-0.1/serializers/factory.py
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:53:59.728988 scoi_lab_serializer_package-0.1/serializers/json/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-04 14:49:50.000000 scoi_lab_serializer_package-0.1/serializers/json/__init__.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     1741 2023-05-08 08:45:06.000000 scoi_lab_serializer_package-0.1/serializers/json/json_parser.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      523 2023-05-08 07:17:50.000000 scoi_lab_serializer_package-0.1/serializers/json/json_serializer.py
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:53:59.728988 scoi_lab_serializer_package-0.1/serializers/source/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-04 10:05:02.000000 scoi_lab_serializer_package-0.1/serializers/source/__init__.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     1004 2023-05-08 10:34:14.000000 scoi_lab_serializer_package-0.1/serializers/source/constants.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     6682 2023-05-08 10:44:42.000000 scoi_lab_serializer_package-0.1/serializers/source/serializer.py
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:53:59.728988 scoi_lab_serializer_package-0.1/serializers/xml/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-08 07:41:47.000000 scoi_lab_serializer_package-0.1/serializers/xml/__init__.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      682 2023-05-09 09:48:58.000000 scoi_lab_serializer_package-0.1/serializers/xml/xml_constants.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     2332 2023-05-09 09:48:58.000000 scoi_lab_serializer_package-0.1/serializers/xml/xml_parser.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      549 2023-05-08 20:08:32.000000 scoi_lab_serializer_package-0.1/serializers/xml/xml_serializer.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)       38 2023-05-10 14:53:59.728988 scoi_lab_serializer_package-0.1/setup.cfg
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      581 2023-05-10 14:53:19.000000 scoi_lab_serializer_package-0.1/setup.py
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 15:07:40.632916 scoi_lab_serializer_package-0.2/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      433 2023-05-10 15:07:40.632916 scoi_lab_serializer_package-0.2/PKG-INFO
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 15:07:40.632916 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:50:53.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/__init__.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      322 2023-05-08 08:54:46.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/factory.py
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 15:07:40.632916 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/json/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-04 14:49:50.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/json/__init__.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     1741 2023-05-08 08:45:06.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/json/json_parser.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      548 2023-05-10 15:04:52.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/json/json_serializer.py
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 15:07:40.632916 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/source/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-04 10:05:02.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/source/__init__.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     1004 2023-05-08 10:34:14.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/source/constants.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     6698 2023-05-10 15:04:23.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/source/serializer.py
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 15:07:40.632916 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/xml/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-08 07:41:47.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/xml/__init__.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      682 2023-05-09 09:48:58.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/xml/xml_constants.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     2348 2023-05-10 15:05:15.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/xml/xml_parser.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      581 2023-05-10 15:05:37.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/xml/xml_serializer.py
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 15:07:40.632916 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package.egg-info/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      433 2023-05-10 15:07:40.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package.egg-info/PKG-INFO
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      769 2023-05-10 15:07:40.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        1 2023-05-10 15:07:40.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      128 2023-05-10 15:07:40.000000 scoi_lab_serializer_package-0.2/scoi_lab_serializer_package.egg-info/top_level.txt
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)       38 2023-05-10 15:07:40.632916 scoi_lab_serializer_package-0.2/setup.cfg
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      645 2023-05-10 15:07:12.000000 scoi_lab_serializer_package-0.2/setup.py
```

### Comparing `scoi_lab_serializer_package-0.1/serializers/json/json_parser.py` & `scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/json/json_parser.py`

 * *Files identical despite different names*

### Comparing `scoi_lab_serializer_package-0.1/serializers/json/json_serializer.py` & `scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/json/json_serializer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from serializers.json.json_parser import parse_json
-from serializers.source.serializer import serialize, deserialize
+from scoi_lab_serializer_package.json.json_parser import parse_json
+from scoi_lab_serializer_package.serializer import serialize, deserialize
 
 
 class JsonSerializer:
     @staticmethod
     def dumps(item):
         return str(serialize(item)).replace("\n", "\\n")
```

### Comparing `scoi_lab_serializer_package-0.1/serializers/source/constants.py` & `scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/source/constants.py`

 * *Files identical despite different names*

### Comparing `scoi_lab_serializer_package-0.1/serializers/source/serializer.py` & `scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/source/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 import types
 from types import CodeType, FunctionType
 from pydoc import locate
 
-from serializers.source.constants import *
+from scoi_lab_serializer_package.source.constants import *
 
 
 def get_type(item):
     item_type = str(type(item))
 
     return item_type[8:len(item_type) - 2]
```

### Comparing `scoi_lab_serializer_package-0.1/serializers/xml/xml_constants.py` & `scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/xml/xml_constants.py`

 * *Files identical despite different names*

### Comparing `scoi_lab_serializer_package-0.1/serializers/xml/xml_parser.py` & `scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/xml/xml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import types
 import regex
 
-from serializers.xml.xml_constants import *
+from scoi_lab_serializer_package.xml.xml_constants import *
 
 
 def dumps_from_dict(obj, is_first=False) -> str:
     if type(obj) in (int, float, bool, types.NoneType):
         return create_xml_element(type(obj).__name__, str(obj), is_first)
     elif type(obj) is str:
         data = mask_symbols(obj)
```

### Comparing `scoi_lab_serializer_package-0.1/serializers/xml/xml_serializer.py` & `scoi_lab_serializer_package-0.2/scoi_lab_serializer_package/xml/xml_serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from serializers.xml.xml_parser import dumps_from_dict, loads_to_dict
-from serializers.source.serializer import serialize, deserialize
+from scoi_lab_serializer_package.xml.xml_parser import dumps_from_dict, loads_to_dict
+from scoi_lab_serializer_package.source.serializer import serialize, deserialize
 
 
 class XmlSerializer:
     @staticmethod
     def dumps(obj):
         obj = serialize(obj)
```

### Comparing `scoi_lab_serializer_package-0.1/setup.py` & `scoi_lab_serializer_package-0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 setup(
     name="scoi_lab_serializer_package",
-    version="0.1",
+    version="0.2",
     description="package for python (de)serialization in .json and .xml",
     url="https://github.com/DrVaroZ/SCoL_labs/tree/lab3",
     author="Vadim Zhur",
     author_email="vadim10zhur@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ],
-    packages=["serializers/json", "serializers/source", "serializers/xml", "serializers"],
+    packages=["scoi_lab_serializer_package/json", "scoi_lab_serializer_package/source", "scoi_lab_serializer_package/xml", "scoi_lab_serializer_package"],
     include_package_data=True
 )
```

