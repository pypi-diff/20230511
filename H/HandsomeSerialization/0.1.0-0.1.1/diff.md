# Comparing `tmp/HandsomeSerialization-0.1.0.tar.gz` & `tmp/HandsomeSerialization-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandsomeSerialization-0.1.0.tar", last modified: Wed May 10 21:38:00 2023, max compression
+gzip compressed data, was "HandsomeSerialization-0.1.1.tar", last modified: Wed May 10 21:57:28 2023, max compression
```

## Comparing `HandsomeSerialization-0.1.0.tar` & `HandsomeSerialization-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 21:38:00.953035 HandsomeSerialization-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-05-10 21:38:00.943040 HandsomeSerialization-0.1.0/HandsomeSerialization.egg-info/
--rw-rw-rw-   0        0        0      438 2023-05-10 21:38:00.000000 HandsomeSerialization-0.1.0/HandsomeSerialization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-05-10 21:38:00.000000 HandsomeSerialization-0.1.0/HandsomeSerialization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 21:38:00.000000 HandsomeSerialization-0.1.0/HandsomeSerialization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 21:38:00.000000 HandsomeSerialization-0.1.0/HandsomeSerialization.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-10 21:38:00.000000 HandsomeSerialization-0.1.0/HandsomeSerialization.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      438 2023-05-10 21:38:00.952032 HandsomeSerialization-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-10 21:25:44.000000 HandsomeSerialization-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 21:38:00.950042 HandsomeSerialization-0.1.0/Serialization/
--rw-rw-rw-   0        0        0      642 2023-05-10 19:07:24.000000 HandsomeSerialization-0.1.0/Serialization/__init__.py
--rw-rw-rw-   0        0        0     1145 2023-05-10 18:38:24.000000 HandsomeSerialization-0.1.0/Serialization/base_serializer.py
--rw-rw-rw-   0        0        0     9475 2023-05-10 19:07:24.000000 HandsomeSerialization-0.1.0/Serialization/dict_serializer.py
--rw-rw-rw-   0        0        0     3988 2023-05-10 18:46:32.000000 HandsomeSerialization-0.1.0/Serialization/json_serializer.py
--rw-rw-rw-   0        0        0      508 2023-05-10 18:46:32.000000 HandsomeSerialization-0.1.0/Serialization/serializers_factory.py
--rw-rw-rw-   0        0        0     1264 2023-05-10 19:08:39.000000 HandsomeSerialization-0.1.0/Serialization/type_constants.py
--rw-rw-rw-   0        0        0     4194 2023-05-10 18:46:32.000000 HandsomeSerialization-0.1.0/Serialization/xml_serializer.py
--rw-rw-rw-   0        0        0       42 2023-05-10 21:38:00.953035 HandsomeSerialization-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1048 2023-05-10 21:37:03.000000 HandsomeSerialization-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 21:38:00.951043 HandsomeSerialization-0.1.0/tests/
--rw-rw-rw-   0        0        0      948 2023-04-26 01:27:36.000000 HandsomeSerialization-0.1.0/tests/test_constants.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:57:28.371519 HandsomeSerialization-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-05-10 21:57:28.359530 HandsomeSerialization-0.1.1/HandsomeSerialization.egg-info/
+-rw-rw-rw-   0        0        0      438 2023-05-10 21:57:28.000000 HandsomeSerialization-0.1.1/HandsomeSerialization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-05-10 21:57:28.000000 HandsomeSerialization-0.1.1/HandsomeSerialization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 21:57:28.000000 HandsomeSerialization-0.1.1/HandsomeSerialization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 21:57:28.000000 HandsomeSerialization-0.1.1/HandsomeSerialization.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-10 21:57:28.000000 HandsomeSerialization-0.1.1/HandsomeSerialization.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      438 2023-05-10 21:57:28.371519 HandsomeSerialization-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-10 21:25:44.000000 HandsomeSerialization-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 21:57:28.369530 HandsomeSerialization-0.1.1/Serialization/
+-rw-rw-rw-   0        0        0      642 2023-05-10 19:07:24.000000 HandsomeSerialization-0.1.1/Serialization/__init__.py
+-rw-rw-rw-   0        0        0     1145 2023-05-10 18:38:24.000000 HandsomeSerialization-0.1.1/Serialization/base_serializer.py
+-rw-rw-rw-   0        0        0     9475 2023-05-10 19:07:24.000000 HandsomeSerialization-0.1.1/Serialization/dict_serializer.py
+-rw-rw-rw-   0        0        0     3988 2023-05-10 18:46:32.000000 HandsomeSerialization-0.1.1/Serialization/json_serializer.py
+-rw-rw-rw-   0        0        0      508 2023-05-10 18:46:32.000000 HandsomeSerialization-0.1.1/Serialization/serializers_factory.py
+-rw-rw-rw-   0        0        0     1264 2023-05-10 19:08:39.000000 HandsomeSerialization-0.1.1/Serialization/type_constants.py
+-rw-rw-rw-   0        0        0     4194 2023-05-10 18:46:32.000000 HandsomeSerialization-0.1.1/Serialization/xml_serializer.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 21:57:28.371519 HandsomeSerialization-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1048 2023-05-10 21:57:16.000000 HandsomeSerialization-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:57:28.369530 HandsomeSerialization-0.1.1/tests/
+-rw-rw-rw-   0        0        0      948 2023-04-26 01:27:36.000000 HandsomeSerialization-0.1.1/tests/test_constants.py
```

### Comparing `HandsomeSerialization-0.1.0/Serialization/__init__.py` & `HandsomeSerialization-0.1.1/Serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `HandsomeSerialization-0.1.0/Serialization/base_serializer.py` & `HandsomeSerialization-0.1.1/Serialization/base_serializer.py`

 * *Files identical despite different names*

### Comparing `HandsomeSerialization-0.1.0/Serialization/dict_serializer.py` & `HandsomeSerialization-0.1.1/Serialization/dict_serializer.py`

 * *Files identical despite different names*

### Comparing `HandsomeSerialization-0.1.0/Serialization/json_serializer.py` & `HandsomeSerialization-0.1.1/Serialization/json_serializer.py`

 * *Files identical despite different names*

### Comparing `HandsomeSerialization-0.1.0/Serialization/type_constants.py` & `HandsomeSerialization-0.1.1/Serialization/type_constants.py`

 * *Files identical despite different names*

### Comparing `HandsomeSerialization-0.1.0/Serialization/xml_serializer.py` & `HandsomeSerialization-0.1.1/Serialization/xml_serializer.py`

 * *Files identical despite different names*

### Comparing `HandsomeSerialization-0.1.0/setup.py` & `HandsomeSerialization-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="HandsomeSerialization",
-    version="0.1.0",
+    version="0.1.1",
     description="Library for class and function serialization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="KiryaHandsome",
     author_email="kirill19962003@gmail.com",
     license="MIT",
     classifiers=[
```

### Comparing `HandsomeSerialization-0.1.0/tests/test_constants.py` & `HandsomeSerialization-0.1.1/tests/test_constants.py`

 * *Files identical despite different names*

