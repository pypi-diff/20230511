# Comparing `tmp/searchium-0.0.1rc3.tar.gz` & `tmp/searchium-0.0.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchium-0.0.1rc3.tar", max compression
+gzip compressed data, was "searchium-0.0.1rc4.tar", max compression
```

## Comparing `searchium-0.0.1rc3.tar` & `searchium-0.0.1rc4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1423 2023-04-19 16:01:41.103149 searchium-0.0.1rc3/README.md
--rw-r--r--   0        0        0      380 2023-04-04 07:50:38.111647 searchium-0.0.1rc3/pyproject.toml
--rw-r--r--   0        0        0      323 2023-04-18 08:39:12.058174 searchium-0.0.1rc3/searchium/__init__.py
--rw-r--r--   0        0        0       93 2023-04-04 10:24:52.278850 searchium-0.0.1rc3/searchium/client/__init__.py
--rw-r--r--   0        0        0     6395 2023-04-19 16:01:41.123149 searchium-0.0.1rc3/searchium/client/func.py
--rw-r--r--   0        0        0     1176 2023-04-18 14:33:48.839524 searchium-0.0.1rc3/searchium/client/init.py
--rw-r--r--   0        0        0       44 2023-03-31 10:19:23.270220 searchium-0.0.1rc3/searchium/fvs/__init__.py
--rw-r--r--   0        0        0     5331 2023-04-03 12:04:06.397449 searchium-0.0.1rc3/searchium/fvs/client.py
--rw-r--r--   0        0        0     1965 2023-04-19 13:39:57.422802 searchium-0.0.1rc3/searchium/fvs/model.py
--rw-r--r--   0        0        0     1922 1970-01-01 00:00:00.000000 searchium-0.0.1rc3/PKG-INFO
+-rw-r--r--   0        0        0     1423 2023-04-19 16:01:41.103149 searchium-0.0.1rc4/README.md
+-rw-r--r--   0        0        0      380 2023-05-11 13:26:40.561220 searchium-0.0.1rc4/pyproject.toml
+-rw-r--r--   0        0        0      323 2023-05-11 12:14:21.577402 searchium-0.0.1rc4/searchium/__init__.py
+-rw-r--r--   0        0        0       93 2023-04-04 10:24:52.278850 searchium-0.0.1rc4/searchium/client/__init__.py
+-rw-r--r--   0        0        0     6395 2023-05-11 11:27:09.343472 searchium-0.0.1rc4/searchium/client/func.py
+-rw-r--r--   0        0        0     1176 2023-04-18 14:33:48.839524 searchium-0.0.1rc4/searchium/client/init.py
+-rw-r--r--   0        0        0       44 2023-03-31 10:19:23.270220 searchium-0.0.1rc4/searchium/fvs/__init__.py
+-rw-r--r--   0        0        0     5331 2023-04-03 12:04:06.397449 searchium-0.0.1rc4/searchium/fvs/client.py
+-rw-r--r--   0        0        0     1989 2023-05-11 11:18:52.346561 searchium-0.0.1rc4/searchium/fvs/model.py
+-rw-r--r--   0        0        0     1922 1970-01-01 00:00:00.000000 searchium-0.0.1rc4/PKG-INFO
```

### Comparing `searchium-0.0.1rc3/README.md` & `searchium-0.0.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `searchium-0.0.1rc3/searchium/client/func.py` & `searchium-0.0.1rc4/searchium/client/func.py`

 * *Files identical despite different names*

### Comparing `searchium-0.0.1rc3/searchium/client/init.py` & `searchium-0.0.1rc4/searchium/client/init.py`

 * *Files identical despite different names*

### Comparing `searchium-0.0.1rc3/searchium/fvs/client.py` & `searchium-0.0.1rc4/searchium/fvs/client.py`

 * *Files identical despite different names*

### Comparing `searchium-0.0.1rc3/searchium/fvs/model.py` & `searchium-0.0.1rc4/searchium/fvs/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
 
 class DatasetStatus(str, Enum):
     completed = 'completed'
     training = 'training'
     error = 'error'
     loaded = 'loaded'
+    pending = 'pending'
 
 
 class TrainStatus(BaseModel):
     datasetStatus: DatasetStatus
 
 
 class Response(BaseModel):
```

### Comparing `searchium-0.0.1rc3/PKG-INFO` & `searchium-0.0.1rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchium
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: 
 Author: GSI Technology, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

