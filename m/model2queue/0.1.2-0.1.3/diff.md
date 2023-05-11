# Comparing `tmp/model2queue-0.1.2.tar.gz` & `tmp/model2queue-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model2queue-0.1.2.tar", last modified: Tue May  9 18:52:58 2023, max compression
+gzip compressed data, was "model2queue-0.1.3.tar", last modified: Thu May 11 13:23:18 2023, max compression
```

## Comparing `model2queue-0.1.2.tar` & `model2queue-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.656476 model2queue-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-09 18:52:58.656476 model2queue-0.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.652476 model2queue-0.1.2/model2queue/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/api_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.652476 model2queue-0.1.2/model2queue/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.652476 model2queue-0.1.2/model2queue/examples/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/examples/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/examples/fastapi/preprocess_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/examples/fastapi/simple_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.652476 model2queue-0.1.2/model2queue/helper/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/helper/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.652476 model2queue-0.1.2/model2queue/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/workers/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/workers/consumer_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-09 18:52:44.000000 model2queue-0.1.2/model2queue/workers/worker_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:52:58.652476 model2queue-0.1.2/model2queue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-09 18:52:58.000000 model2queue-0.1.2/model2queue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-09 18:52:58.000000 model2queue-0.1.2/model2queue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:52:58.000000 model2queue-0.1.2/model2queue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 18:52:58.000000 model2queue-0.1.2/model2queue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 18:52:58.000000 model2queue-0.1.2/model2queue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 18:52:58.656476 model2queue-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-09 18:52:44.000000 model2queue-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:23:18.032736 model2queue-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-11 13:23:18.032736 model2queue-0.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:23:18.032736 model2queue-0.1.3/model2queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 13:23:07.000000 model2queue-0.1.3/model2queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-11 13:23:07.000000 model2queue-0.1.3/model2queue/api_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:23:18.032736 model2queue-0.1.3/model2queue/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 13:23:07.000000 model2queue-0.1.3/model2queue/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:23:18.032736 model2queue-0.1.3/model2queue/examples/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 13:23:07.000000 model2queue-0.1.3/model2queue/examples/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-11 13:23:07.000000 model2queue-0.1.3/model2queue/examples/fastapi/preprocess_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-11 13:23:07.000000 model2queue-0.1.3/model2queue/examples/fastapi/simple_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:23:18.032736 model2queue-0.1.3/model2queue/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 13:23:07.000000 model2queue-0.1.3/model2queue/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-11 13:23:07.000000 model2queue-0.1.3/model2queue/helper/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:23:18.032736 model2queue-0.1.3/model2queue/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-11 13:23:07.000000 model2queue-0.1.3/model2queue/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-11 13:23:07.000000 model2queue-0.1.3/model2queue/workers/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-11 13:23:07.000000 model2queue-0.1.3/model2queue/workers/consumer_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-11 13:23:07.000000 model2queue-0.1.3/model2queue/workers/worker_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:23:18.032736 model2queue-0.1.3/model2queue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-11 13:23:17.000000 model2queue-0.1.3/model2queue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-11 13:23:18.000000 model2queue-0.1.3/model2queue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:23:17.000000 model2queue-0.1.3/model2queue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-11 13:23:17.000000 model2queue-0.1.3/model2queue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 13:23:17.000000 model2queue-0.1.3/model2queue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 13:23:18.032736 model2queue-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-11 13:23:07.000000 model2queue-0.1.3/setup.py
```

### Comparing `model2queue-0.1.2/model2queue/api_tasks.py` & `model2queue-0.1.3/model2queue/api_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,55 +19,56 @@
 
 def start_consumer_producer(
     connection: Connection,
     queue: Queue,
     tgt_exchange: Exchange,
     callback_function: Callable[[str], None],
     routing_key: str,
-    n_workers: int
+    n_workers: int,
 ):
     queue.maybe_bind(connection)
     queue.declare()
     worker = ConsumerProducerTaskWorker(
         connection=connection,
         queue=queue,
         tgt_exchange=tgt_exchange,
         callback_function=callback_function,
         routing_key=routing_key,
-        n_workers=n_workers
+        n_workers=n_workers,
     )
     worker.run()
 
 
 def start_consumer(
     connection: Connection,
     queue: Queue,
     callback_function: Callable[[str], None],
-    n_workers: int
+    n_workers: int,
 ):
     queue.maybe_bind(connection)
     queue.declare()
     worker = ConsumerTaskWorker(
         connection=connection,
         queue=queue,
         callback_function=callback_function,
-        n_workers=n_workers
+        n_workers=n_workers,
     )
     worker.run()
 
 
 def start_api_task_consumer_producer(
     func: Callable,
     conn_url: str = "memory://localhost/",
     in_queue_name: str = "queue_in",
     in_exchange_name: str = "in_excahnge",
     in_routing_key: str = "api_model_input",
     out_queue_name: str = "queue_in",
     out_exchange_name: str = "out_exchange",
     out_routing_key: str = "api_model_output",
+    n_workers: int = 1,
 ) -> None:
     connection = Connection(conn_url)
 
     in_exchange = Exchange(in_exchange_name, type="direct")
     in_queue = Queue(
         name=in_queue_name, exchange=in_exchange, routing_key=in_routing_key
     )
@@ -83,14 +84,15 @@
 
     worker = ConsumerProducerTaskWorker(
         connection=connection,
         queue=in_queue,
         tgt_exchange=out_exchange,
         callback_function=func,
         routing_key=out_routing_key,
+        n_workers=n_workers,
     )
 
     model_input_reader = WorkerThread(
         worker=worker,
         target=start_worker,
         kwargs={
             "worker": worker,
@@ -102,26 +104,28 @@
 
 def start_api_task_consumer(
     func: Callable,
     conn_url: str = "memory://localhost/",
     in_queue_name: str = "queue_in",
     in_exchange_name: str = "in_excahnge",
     routing_key: str = "api_model_input",
+    n_workers: int = 1,
 ) -> None:
     connection = Connection(conn_url)
 
     in_exchange = Exchange(in_exchange_name, type="direct")
     in_queue = Queue(name=in_queue_name, exchange=in_exchange, routing_key=routing_key)
     in_queue.maybe_bind(connection)
     in_queue.declare()
 
     worker = ConsumerTaskWorker(
         connection=connection,
         queue=in_queue,
         callback_function=func,
+        n_workers=n_workers,
     )
 
     model_input_reader = WorkerThread(
         worker=worker,
         target=start_worker,
         kwargs={
             "worker": worker,
```

### Comparing `model2queue-0.1.2/model2queue/examples/fastapi/preprocess_images.py` & `model2queue-0.1.3/model2queue/examples/fastapi/preprocess_images.py`

 * *Files identical despite different names*

### Comparing `model2queue-0.1.2/model2queue/examples/fastapi/simple_model.py` & `model2queue-0.1.3/model2queue/examples/fastapi/simple_model.py`

 * *Files identical despite different names*

### Comparing `model2queue-0.1.2/model2queue/workers/consumer.py` & `model2queue-0.1.3/model2queue/workers/consumer.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class ConsumerTaskWorker(ConsumerProducerMixin):
     def __init__(
         self,
         connection: Connection,
         queue: str,
         callback_function: Callable,
-        n_workers: int = 1,
+        n_workers: int,
     ):
         self.connection = connection
         self.queue = queue
         self.callback_function = callback_function
         self.n_workers = n_workers
 
     def get_consumers(self, consumer: Consumer, channel: Any) -> List[Consumer]:
```

### Comparing `model2queue-0.1.2/model2queue/workers/consumer_producer.py` & `model2queue-0.1.3/model2queue/workers/consumer_producer.py`

 * *Files identical despite different names*

### Comparing `model2queue-0.1.2/model2queue.egg-info/SOURCES.txt` & `model2queue-0.1.3/model2queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `model2queue-0.1.2/setup.py` & `model2queue-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="model2queue",
     packages=find_packages(),
-    version="0.1.2",
+    version="0.1.3",
     description="A library to expose an api with a queue for batch predictions",
     author="collective.ai",
     author_email="team.collective.ai@gmail.com",
     url="https://github.com/collectiveai-team/model2queue",
     install_requires=["kombu", "fastapi", "uvicorn", "rich"],
     package_data={"": ["*.yml", "*.yaml"]},
     include_package_data=True,
```

