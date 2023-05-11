# Comparing `tmp/eswrap-0.3.1.tar.gz` & `tmp/eswrap-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eswrap-0.3.1.tar", last modified: Mon May  8 18:42:09 2023, max compression
+gzip compressed data, was "eswrap-0.4.tar", last modified: Thu May 11 11:44:31 2023, max compression
```

## Comparing `eswrap-0.3.1.tar` & `eswrap-0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:42:09.648972 eswrap-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-05-08 18:41:55.000000 eswrap-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-08 18:42:09.648972 eswrap-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 18:41:55.000000 eswrap-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:42:09.644972 eswrap-0.3.1/eswrap/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 18:42:09.000000 eswrap-0.3.1/eswrap/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-08 18:41:55.000000 eswrap-0.3.1/eswrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:42:09.648972 eswrap-0.3.1/eswrap/common/
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-08 18:41:55.000000 eswrap-0.3.1/eswrap/common/EsHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:41:55.000000 eswrap-0.3.1/eswrap/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-08 18:41:55.000000 eswrap-0.3.1/eswrap/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:42:09.648972 eswrap-0.3.1/eswrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-08 18:42:09.000000 eswrap-0.3.1/eswrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-08 18:42:09.000000 eswrap-0.3.1/eswrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:42:09.000000 eswrap-0.3.1/eswrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 18:42:09.000000 eswrap-0.3.1/eswrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 18:42:09.000000 eswrap-0.3.1/eswrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:42:09.648972 eswrap-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-08 18:41:55.000000 eswrap-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:44:31.900946 eswrap-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-05-11 11:44:18.000000 eswrap-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-11 11:44:31.900946 eswrap-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 11:44:18.000000 eswrap-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:44:31.900946 eswrap-0.4/eswrap/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-11 11:44:31.000000 eswrap-0.4/eswrap/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-11 11:44:18.000000 eswrap-0.4/eswrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:44:31.900946 eswrap-0.4/eswrap/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-11 11:44:18.000000 eswrap-0.4/eswrap/common/EsHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:44:18.000000 eswrap-0.4/eswrap/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-11 11:44:18.000000 eswrap-0.4/eswrap/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:44:31.900946 eswrap-0.4/eswrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-11 11:44:31.000000 eswrap-0.4/eswrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-11 11:44:31.000000 eswrap-0.4/eswrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:44:31.000000 eswrap-0.4/eswrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 11:44:31.000000 eswrap-0.4/eswrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 11:44:31.000000 eswrap-0.4/eswrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 11:44:31.904946 eswrap-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-11 11:44:18.000000 eswrap-0.4/setup.py
```

### Comparing `eswrap-0.3.1/LICENSE` & `eswrap-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eswrap-0.3.1/PKG-INFO` & `eswrap-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.3.1
+Version: 0.4
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.3.1/eswrap/__init__.py` & `eswrap-0.4/eswrap/__init__.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.3.1/eswrap/common/EsHandler.py` & `eswrap-0.4/eswrap/common/EsHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,53 +10,56 @@
 
     def __init__(self, es_connection: Elasticsearch, index: str):
         self.es_connection = es_connection
         self.index = index
 
     def search(self, filter: dict = None, skip: int = 0, limit: int = 10):
         """
-        Query the api.
+        Search the index.
         """
-
         return EsCursor(self, filter, limit=limit, skip=skip).search()
 
     def find(self, filter: dict = None):
         """
-        Query the api.
+        Query the index.
         """
-
         return EsCursor(self, filter)
 
     def find_one(self, filter: dict = None):
         """
-        Query the api and return the first result.
+        Query the index and return the first result.
         """
-
         for result in self.find(filter).limit(1):
             return result
         return None
 
-    def count(self, filter: dict = None):
+    def count(self, filter: dict = None, **kwargs):
         """ """
         if filter is None:
             data = {"query": {"match_all": {}}}
         else:
             data = {"query": {"match": filter}}
 
-        return self.es_connection.count(index=self.index, body=data)["count"]
+        return self.es_connection.count(index=self.index, body=data, **kwargs)["count"]
 
-    def upsert(self, document: dict, doc_id: Optional[str] = None):
+    def upsert(self, document: dict, doc_id: Optional[str] = None, **kwargs):
         """ """
         if doc_id is None:
-            return self.es_connection.index(index=self.index, document=document)
+            return self.es_connection.index(index=self.index, document=document, **kwargs)
         else:
             return self.es_connection.index(
-                index=self.index, id=doc_id, document=document
+                index=self.index, id=doc_id, document=document, **kwargs
             )
 
+    def delete(self, doc_id: str, **kwargs):
+        return self.es_connection.delete(index=self.index, id=doc_id, **kwargs)
+
+    def delete_by_query(self, filter: dict, **kwargs):
+        return self.es_connection.delete_by_query(index=self.index, body=filter, **kwargs)
+
     def __repr__(self):
         """return a string representation of the obj EsHandler"""
         return "<< EsHandler: {} >>".format(self.index)
 
 
 class EsCursor(object):
     """
```

### Comparing `eswrap-0.3.1/eswrap/main.py` & `eswrap-0.4/eswrap/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import logging
 import os
 from typing import Optional
 
+import elastic_transport
 import urllib3
 from elasticsearch import Elasticsearch
 from urllib3.exceptions import InsecureRequestWarning
 
 from eswrap.common.EsHandler import EsHandler
 
 urllib3.disable_warnings(InsecureRequestWarning)
@@ -22,21 +24,28 @@
     def __init__(
         self, host: str = "localhost", port: int = 9200, scheme: str = "http", **kwargs
     ):
         self.__version = VERSION
 
         self.connection_details = {"host": host, "port": port, "scheme": scheme}
 
+        self.logger = logging.getLogger(__name__)
+
         self.__es_client = Elasticsearch([self.connection_details], **kwargs)
 
-        for each in self.__es_client.indices.get(index="*").keys():
-            if not each.startswith("."):
-                setattr(
-                    self, each, EsHandler(es_connection=self.__es_client, index=each)
-                )
+        try:
+            for each in self.__es_client.indices.get(index="*").keys():
+                if not each.startswith("."):
+                    setattr(
+                        self, each, EsHandler(es_connection=self.__es_client, index=each)
+                    )
+        except elastic_transport.ConnectionError as err:
+            self.logger.warning(f"Cannot connect to elasticsearch, error encountered: {err}")
+        except Exception as err:
+            self.logger.error(f"Uncaught exeption encountered: {err}")
 
     @property
     def es_client(self):
         return self.__es_client
 
     @property
     def version(self):
```

### Comparing `eswrap-0.3.1/eswrap.egg-info/PKG-INFO` & `eswrap-0.4/eswrap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.3.1
+Version: 0.4
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.3.1/setup.py` & `eswrap-0.4/setup.py`

 * *Files identical despite different names*

