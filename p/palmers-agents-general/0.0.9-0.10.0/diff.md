# Comparing `tmp/palmers_agents_general-0.0.9.tar.gz` & `tmp/palmers_agents_general-0.10.0.tar.gz`

## Comparing `palmers_agents_general-0.0.9.tar` & `palmers_agents_general-0.10.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/palmers_agents_general/__init__.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/palmers_agents_general/base_mq_consumer.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/palmers_agents_general/base_mq_worker.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/palmers_agents_general/blobs_handler.py
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/palmers_agents_general/db_handler.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/palmers_agents_general/models_handler.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.10.0/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.10.0/palmers_agents_general/__init__.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 palmers_agents_general-0.10.0/palmers_agents_general/base_mq_consumer.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 palmers_agents_general-0.10.0/palmers_agents_general/base_mq_worker.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 palmers_agents_general-0.10.0/palmers_agents_general/blobs_handler.py
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 palmers_agents_general-0.10.0/palmers_agents_general/db_handler.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.10.0/palmers_agents_general/models_handler.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.10.0/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_agents_general-0.10.0/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.10.0/README.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 palmers_agents_general-0.10.0/pyproject.toml
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 palmers_agents_general-0.10.0/PKG-INFO
```

### Comparing `palmers_agents_general-0.0.9/palmers_agents_general/base_mq_consumer.py` & `palmers_agents_general-0.10.0/palmers_agents_general/base_mq_consumer.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.9/palmers_agents_general/base_mq_worker.py` & `palmers_agents_general-0.10.0/palmers_agents_general/base_mq_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,16 +45,17 @@
         self.__channel.basic_qos(prefetch_count=1)
         self.__channel.basic_consume(
             queue=self._consume_queue, on_message_callback=self.__callback)
 
         return self
 
     
-    def publish(self, message, queue=None):
+    def publish(self, message, queue=None, persistent=True):
         queue = queue or self._produce_queue
 
         self.__channel.basic_publish(exchange='',
                               routing_key=queue,
-                              body=json.dumps(message))
+                              body=json.dumps(message),
+                              properties=pika.BasicProperties(delivery_mode=pika.spec.PERSISTENT_DELIVERY_MODE, ) if persistent else None)
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.__connection.close()
```

### Comparing `palmers_agents_general-0.0.9/palmers_agents_general/blobs_handler.py` & `palmers_agents_general-0.10.0/palmers_agents_general/blobs_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.9/palmers_agents_general/db_handler.py` & `palmers_agents_general-0.10.0/palmers_agents_general/db_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.9/palmers_agents_general/models_handler.py` & `palmers_agents_general-0.10.0/palmers_agents_general/models_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.9/LICENSE` & `palmers_agents_general-0.10.0/LICENSE`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.9/pyproject.toml` & `palmers_agents_general-0.10.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_agents_general"
-version = "0.0.9"
+version = "0.10.0"
 authors = [
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

### Comparing `palmers_agents_general-0.0.9/PKG-INFO` & `palmers_agents_general-0.10.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmers_agents_general
-Version: 0.0.9
+Version: 0.10.0
 Summary: A package to preprocess data for Palmer's project
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Assaf <assafm@sdatta.ai>, Roy  <roy@sdatta.ai>, Guy <assafm@sdatta.ai>, Oran <assafm@sdatta.ai>, Yotam <assafm@sdatta.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

