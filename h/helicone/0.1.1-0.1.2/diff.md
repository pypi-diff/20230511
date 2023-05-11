# Comparing `tmp/helicone-0.1.1.tar.gz` & `tmp/helicone-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helicone-0.1.1.tar", max compression
+gzip compressed data, was "helicone-0.1.2.tar", max compression
```

## Comparing `helicone-0.1.1.tar` & `helicone-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     4046 2023-04-28 13:52:00.188355 helicone-0.1.1/helicone/__init__.py
--rw-r--r--   0        0        0       20 2023-04-28 13:52:00.188984 helicone-0.1.1/helicone/requirements.txt
--rw-r--r--   0        0        0     1233 2023-04-28 13:52:00.192491 helicone-0.1.1/helicone/test.py
--rw-r--r--   0        0        0        0 2023-04-26 11:31:06.381002 helicone-0.1.1/helicone/utils.py
--rw-r--r--   0        0        0     1032 2023-04-26 11:32:09.425143 helicone-0.1.1/helicone/wrapper.py
--rw-r--r--   0        0        0      386 2023-04-28 14:49:38.256605 helicone-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 helicone-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-04-30 18:04:13.152472 helicone-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6275 2023-05-11 15:44:48.124246 helicone-0.1.2/helicone/__init__.py
+-rw-r--r--   0        0        0       20 2023-04-30 16:18:51.491845 helicone-0.1.2/helicone/requirements.txt
+-rw-r--r--   0        0        0     1233 2023-05-11 13:30:29.675363 helicone-0.1.2/helicone/test.py
+-rw-r--r--   0        0        0        0 2023-04-26 11:31:06.381002 helicone-0.1.2/helicone/utils.py
+-rw-r--r--   0        0        0     1032 2023-04-26 11:32:09.425143 helicone-0.1.2/helicone/wrapper.py
+-rw-r--r--   0        0        0      386 2023-05-11 15:49:49.752565 helicone-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 helicone-0.1.2/PKG-INFO
```

### Comparing `helicone-0.1.1/helicone/test.py` & `helicone-0.1.2/helicone/test.py`

 * *Files identical despite different names*

### Comparing `helicone-0.1.1/helicone/wrapper.py` & `helicone-0.1.2/helicone/wrapper.py`

 * *Files identical despite different names*

### Comparing `helicone-0.1.1/PKG-INFO` & `helicone-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helicone
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python wrapper for the OpenAI API that logs all requests to Helicone.
 Home-page: https://www.helicone.ai
 License: Apache-2.0
 Author: Helicone, Inc.
 Author-email: help@helicone.ai
 Requires-Python: >=3.8.1
 Classifier: License :: OSI Approved :: Apache Software License
```

