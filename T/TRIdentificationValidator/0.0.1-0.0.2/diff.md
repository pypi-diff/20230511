# Comparing `tmp/TRIdentificationValidator-0.0.1.tar.gz` & `tmp/TRIdentificationValidator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TRIdentificationValidator-0.0.1.tar", last modified: Thu May 11 10:22:16 2023, max compression
+gzip compressed data, was "TRIdentificationValidator-0.0.2.tar", last modified: Thu May 11 10:29:13 2023, max compression
```

## Comparing `TRIdentificationValidator-0.0.1.tar` & `TRIdentificationValidator-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-05-11 10:22:16.138654 TRIdentificationValidator-0.0.1/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 TRIdentificationValidator-0.0.1/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1409 2023-05-11 10:22:16.138534 TRIdentificationValidator-0.0.1/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      840 2023-05-11 09:43:24.000000 TRIdentificationValidator-0.0.1/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-05-11 10:22:16.137587 TRIdentificationValidator-0.0.1/TRIdentification/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      884 2023-05-11 09:40:51.000000 TRIdentificationValidator-0.0.1/TRIdentification/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      343 2023-05-11 00:10:39.000000 TRIdentificationValidator-0.0.1/TRIdentification/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-05-11 10:22:16.138354 TRIdentificationValidator-0.0.1/TRIdentificationValidator.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1409 2023-05-11 10:22:16.000000 TRIdentificationValidator-0.0.1/TRIdentificationValidator.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      329 2023-05-11 10:22:16.000000 TRIdentificationValidator-0.0.1/TRIdentificationValidator.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-05-11 10:22:16.000000 TRIdentificationValidator-0.0.1/TRIdentificationValidator.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       21 2023-05-11 10:22:16.000000 TRIdentificationValidator-0.0.1/TRIdentificationValidator.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       17 2023-05-11 10:22:16.000000 TRIdentificationValidator-0.0.1/TRIdentificationValidator.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-05-11 10:22:16.138697 TRIdentificationValidator-0.0.1/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      913 2023-05-11 10:21:44.000000 TRIdentificationValidator-0.0.1/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-05-11 10:29:13.757183 TRIdentificationValidator-0.0.2/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 TRIdentificationValidator-0.0.2/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1409 2023-05-11 10:29:13.757048 TRIdentificationValidator-0.0.2/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      840 2023-05-11 09:43:24.000000 TRIdentificationValidator-0.0.2/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-05-11 10:29:13.754971 TRIdentificationValidator-0.0.2/TRIdentification/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      884 2023-05-11 10:29:03.000000 TRIdentificationValidator-0.0.2/TRIdentification/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      141 2023-05-11 10:29:00.000000 TRIdentificationValidator-0.0.2/TRIdentification/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-05-11 10:29:13.756006 TRIdentificationValidator-0.0.2/TRIdentification/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       52 2023-05-11 09:34:04.000000 TRIdentificationValidator-0.0.2/TRIdentification/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      873 2023-05-11 09:26:14.000000 TRIdentificationValidator-0.0.2/TRIdentification/service/helper.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     3313 2023-05-11 09:34:04.000000 TRIdentificationValidator-0.0.2/TRIdentification/service/identity_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-05-11 10:29:13.756858 TRIdentificationValidator-0.0.2/TRIdentificationValidator.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1409 2023-05-11 10:29:13.000000 TRIdentificationValidator-0.0.2/TRIdentificationValidator.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      446 2023-05-11 10:29:13.000000 TRIdentificationValidator-0.0.2/TRIdentificationValidator.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-05-11 10:29:13.000000 TRIdentificationValidator-0.0.2/TRIdentificationValidator.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       21 2023-05-11 10:29:13.000000 TRIdentificationValidator-0.0.2/TRIdentificationValidator.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       17 2023-05-11 10:29:13.000000 TRIdentificationValidator-0.0.2/TRIdentificationValidator.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-05-11 10:29:13.757223 TRIdentificationValidator-0.0.2/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      941 2023-05-11 10:29:00.000000 TRIdentificationValidator-0.0.2/setup.py
```

### Comparing `TRIdentificationValidator-0.0.1/LICENSE` & `TRIdentificationValidator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TRIdentificationValidator-0.0.1/PKG-INFO` & `TRIdentificationValidator-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TRIdentificationValidator
-Version: 0.0.1
+Version: 0.0.2
 Summary: TRIdentificationValidator Python package
 Home-page: https://github.com/blueromans/TRIdentificationValidator.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/TRIdentificationValidator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TRIdentificationValidator-0.0.1/README.md` & `TRIdentificationValidator-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `TRIdentificationValidator-0.0.1/TRIdentification/__init__.py` & `TRIdentificationValidator-0.0.2/TRIdentification/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 TRIdentification python library.
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 from TRIdentification.exception import TRIdentificationException
 from TRIdentification.service import IdentificationService
 from TRIdentification.service.helper import IsValidIdentity, IsFromSyrian
 
 
 def TRIdentificationNumberValidator(*args):
```

### Comparing `TRIdentificationValidator-0.0.1/TRIdentificationValidator.egg-info/PKG-INFO` & `TRIdentificationValidator-0.0.2/TRIdentificationValidator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TRIdentificationValidator
-Version: 0.0.1
+Version: 0.0.2
 Summary: TRIdentificationValidator Python package
 Home-page: https://github.com/blueromans/TRIdentificationValidator.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/TRIdentificationValidator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

