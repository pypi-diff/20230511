# Comparing `tmp/negotium-0.2.0.tar.gz` & `tmp/negotium-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negotium-0.2.0.tar", last modified: Sat May  6 00:31:21 2023, max compression
+gzip compressed data, was "negotium-0.2.1.tar", last modified: Thu May 11 10:23:25 2023, max compression
```

## Comparing `negotium-0.2.0.tar` & `negotium-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.970488 negotium-0.2.0/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       57 2023-05-06 00:17:07.000000 negotium-0.2.0/.gitignore
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3771 2023-05-06 00:31:21.970488 negotium-0.2.0/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3604 2023-05-06 00:30:37.000000 negotium-0.2.0/README.md
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.962485 negotium-0.2.0/negotium/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.2.0/negotium/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3603 2023-05-05 23:38:22.000000 negotium-0.2.0/negotium/base.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.966486 negotium-0.2.0/negotium/mq/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.2.0/negotium/mq/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     5985 2023-05-06 00:27:04.000000 negotium-0.2.0/negotium/mq/consumer.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     2947 2023-05-06 00:27:04.000000 negotium-0.2.0/negotium/mq/publisher.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1838 2023-05-06 00:25:28.000000 negotium-0.2.0/negotium/mq/trackers.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.966486 negotium-0.2.0/negotium/schedules/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       29 2023-05-05 23:42:01.000000 negotium-0.2.0/negotium/schedules/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1992 2023-05-06 00:23:30.000000 negotium-0.2.0/negotium/schedules/crontab.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      616 2023-05-06 00:27:04.000000 negotium-0.2.0/negotium/settings.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      867 2023-05-05 23:47:12.000000 negotium-0.2.0/negotium/task.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.966486 negotium-0.2.0/negotium/utils/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.2.0/negotium/utils/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.2.0/negotium/utils/logger.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.966486 negotium-0.2.0/negotium.egg-info/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3771 2023-05-06 00:31:21.000000 negotium-0.2.0/negotium.egg-info/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      515 2023-05-06 00:31:21.000000 negotium-0.2.0/negotium.egg-info/SOURCES.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-06 00:31:21.000000 negotium-0.2.0/negotium.egg-info/dependency_links.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      117 2023-05-06 00:31:21.000000 negotium-0.2.0/negotium.egg-info/requires.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-06 00:31:21.000000 negotium-0.2.0/negotium.egg-info/top_level.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      429 2023-05-06 00:30:49.000000 negotium-0.2.0/pyproject.toml
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-06 00:28:29.000000 negotium-0.2.0/requirements.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-06 00:31:21.970488 negotium-0.2.0/setup.cfg
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.970488 negotium-0.2.0/tests/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.2.0/tests/__init__.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-11 10:23:25.436830 negotium-0.2.1/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       57 2023-05-06 00:17:07.000000 negotium-0.2.1/.gitignore
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     4095 2023-05-11 10:23:25.436830 negotium-0.2.1/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3919 2023-05-11 10:22:50.000000 negotium-0.2.1/README.md
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-11 10:23:25.432829 negotium-0.2.1/negotium/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.2.1/negotium/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3458 2023-05-11 09:59:40.000000 negotium-0.2.1/negotium/base.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-11 10:23:25.436830 negotium-0.2.1/negotium/brokers/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       25 2023-05-11 09:52:44.000000 negotium-0.2.1/negotium/brokers/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      586 2023-05-11 10:02:30.000000 negotium-0.2.1/negotium/brokers/main.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      609 2023-05-11 10:12:52.000000 negotium-0.2.1/negotium/brokers/redis.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-11 10:23:25.436830 negotium-0.2.1/negotium/mq/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.2.1/negotium/mq/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     6386 2023-05-11 10:07:07.000000 negotium-0.2.1/negotium/mq/consumer.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3242 2023-05-11 10:07:38.000000 negotium-0.2.1/negotium/mq/publisher.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     2305 2023-05-11 09:52:02.000000 negotium-0.2.1/negotium/mq/trackers.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-11 10:23:25.436830 negotium-0.2.1/negotium/schedules/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       29 2023-05-05 23:42:01.000000 negotium-0.2.1/negotium/schedules/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1992 2023-05-06 00:23:30.000000 negotium-0.2.1/negotium/schedules/crontab.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      616 2023-05-06 00:27:04.000000 negotium-0.2.1/negotium/settings.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      867 2023-05-05 23:47:12.000000 negotium-0.2.1/negotium/task.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-11 10:23:25.436830 negotium-0.2.1/negotium/utils/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.2.1/negotium/utils/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.2.1/negotium/utils/logger.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-11 10:23:25.436830 negotium-0.2.1/negotium.egg-info/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     4095 2023-05-11 10:23:25.000000 negotium-0.2.1/negotium.egg-info/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      595 2023-05-11 10:23:25.000000 negotium-0.2.1/negotium.egg-info/SOURCES.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-11 10:23:25.000000 negotium-0.2.1/negotium.egg-info/dependency_links.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      117 2023-05-11 10:23:25.000000 negotium-0.2.1/negotium.egg-info/requires.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-11 10:23:25.000000 negotium-0.2.1/negotium.egg-info/top_level.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      438 2023-05-11 10:19:26.000000 negotium-0.2.1/pyproject.toml
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-06 00:28:29.000000 negotium-0.2.1/requirements.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-11 10:23:25.436830 negotium-0.2.1/setup.cfg
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-11 10:23:25.436830 negotium-0.2.1/tests/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.2.1/tests/__init__.py
```

### Comparing `negotium-0.2.0/PKG-INFO` & `negotium-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,10 @@
-Metadata-Version: 2.1
-Name: negotium
-Version: 0.2.0
-Summary: A very simple asynchronous task/job queue
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Negotium
 
-A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. For now, it offers only a minimal set of features, which will be expanded. It also currently only supports Redis as the broker; however, it is planned to support other brokers in the future.
+A simple, lightweight, and easy-to-use task/job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. For now, it offers only a minimal set of features, which will be expanded. It also currently only supports Redis as the broker; however, it is planned to support other brokers in the future.
 
 ## Installation
 
 ```bash
 pip install negotium
 ```
 
@@ -23,16 +16,27 @@
 - Task cancellation: All tasks are cancellable using the UUID returned by the task execution methods: `delay`, `apply_async`, and `apply_periodic_async`
 
 ## Usage
 
 ```python
 # ---- main.py (app entry point) ----
 from negotium import Negotium
+from negotium.brokers import Redis
+
+# create broker
+broker = Redis(
+    host='localhost',
+    port=6379,
+    user='default', # optional
+    password='password', # optional
+    db=0 # optional (defaults to 0)
+)
 
-app = Negotium(broker_url="redis://localhost:6379/0", app_name="my_app")
+# create negotium app
+app = Negotium(app_name="<YOUR_APP_NAME>", broker=broker)
 app.start()
 
 @app.task
 def add(x, y):
     return x + y
 ```
 
@@ -66,15 +70,15 @@
 
 # run the task every minute
 task_id = add.apply_periodic_async(args=(1, 2), cron=Crontab(minute=1))
 
 # with a raw crontab expression
 task_id = add.apply_periodic_async(args=(1, 2), cron=Crontab(expression="* * * * *"))
 
-# to cancel, import the app object and call the `cancel` method
+# to cancel, call the `cancel` method
 app.cancel(task_id)
 ```
 
 ### Using in a Django project
 
 - Create a `negotium.py` file in your Django project directory
 ```
@@ -89,21 +93,30 @@
 ```
 
 - Add the following code to the `negotium.py` file
 ```python
 import os
 
 from negotium import Negotium
+from negotium.brokers import Redis
 
 # Set the django settings module
 os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'my_project.settings')
 
+# Create the broker
+broker = Redis(
+    host='localhost',
+    port=6379,
+    user='default', # optional
+    password='password', # optional
+    db=0 # optional (defaults to 0)
+)
+
 # Create the negotium app
-# If not specified, the broker url defaults to redis://localhost:6379/0
-app = Negotium(broker_url="redis://localhost:6379/0", app_name="my_app")
+app = Negotium(app_name="<YOUR_APP_NAME>", broker=broker)
 app.start()
 ```
 
 - Import the `app` object in your task modules
 ```python
 # --- example/tasks.py ---
 from my_project.negotium import app
```

### Comparing `negotium-0.2.0/README.md` & `negotium-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+Metadata-Version: 2.1
+Name: negotium
+Version: 0.2.1
+Summary: A lightweight and easy to use task queue/scheduler
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # Negotium
 
-A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. For now, it offers only a minimal set of features, which will be expanded. It also currently only supports Redis as the broker; however, it is planned to support other brokers in the future.
+A simple, lightweight, and easy-to-use task/job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. For now, it offers only a minimal set of features, which will be expanded. It also currently only supports Redis as the broker; however, it is planned to support other brokers in the future.
 
 ## Installation
 
 ```bash
 pip install negotium
 ```
 
@@ -16,16 +23,27 @@
 - Task cancellation: All tasks are cancellable using the UUID returned by the task execution methods: `delay`, `apply_async`, and `apply_periodic_async`
 
 ## Usage
 
 ```python
 # ---- main.py (app entry point) ----
 from negotium import Negotium
+from negotium.brokers import Redis
+
+# create broker
+broker = Redis(
+    host='localhost',
+    port=6379,
+    user='default', # optional
+    password='password', # optional
+    db=0 # optional (defaults to 0)
+)
 
-app = Negotium(broker_url="redis://localhost:6379/0", app_name="my_app")
+# create negotium app
+app = Negotium(app_name="<YOUR_APP_NAME>", broker=broker)
 app.start()
 
 @app.task
 def add(x, y):
     return x + y
 ```
 
@@ -59,15 +77,15 @@
 
 # run the task every minute
 task_id = add.apply_periodic_async(args=(1, 2), cron=Crontab(minute=1))
 
 # with a raw crontab expression
 task_id = add.apply_periodic_async(args=(1, 2), cron=Crontab(expression="* * * * *"))
 
-# to cancel, import the app object and call the `cancel` method
+# to cancel, call the `cancel` method
 app.cancel(task_id)
 ```
 
 ### Using in a Django project
 
 - Create a `negotium.py` file in your Django project directory
 ```
@@ -82,21 +100,30 @@
 ```
 
 - Add the following code to the `negotium.py` file
 ```python
 import os
 
 from negotium import Negotium
+from negotium.brokers import Redis
 
 # Set the django settings module
 os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'my_project.settings')
 
+# Create the broker
+broker = Redis(
+    host='localhost',
+    port=6379,
+    user='default', # optional
+    password='password', # optional
+    db=0 # optional (defaults to 0)
+)
+
 # Create the negotium app
-# If not specified, the broker url defaults to redis://localhost:6379/0
-app = Negotium(broker_url="redis://localhost:6379/0", app_name="my_app")
+app = Negotium(app_name="<YOUR_APP_NAME>", broker=broker)
 app.start()
 ```
 
 - Import the `app` object in your task modules
 ```python
 # --- example/tasks.py ---
 from my_project.negotium import app
```

### Comparing `negotium-0.2.0/negotium/base.py` & `negotium-0.2.1/negotium/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import inspect
 from functools import wraps
 
 from .settings import DEFAULT_HOST, DEFAULT_PORT, DEFAULT_LOGFILE
 from .task import _delay, _apply_async, _apply_periodic_async
+from negotium.brokers.main import MessageBroker
 from negotium.mq.consumer import _Consumer
 from negotium.mq.publisher import _Publisher
 from negotium.utils.logger import log
 
 
 class Negotium:
     """This class is the entry point to the negotium application.
@@ -24,28 +25,24 @@
 
         @negotium.task
         def add(x, y):
             return x + y
 
     Note: This class should be instantiated at the entry point of your application.
     """
-    def __init__(self, app_name: str="", broker_url: str="", logfile: str=DEFAULT_LOGFILE):
+    def __init__(self, app_name: str, broker: MessageBroker, logfile: str=DEFAULT_LOGFILE):
         self.app_name = app_name
         if not self.app_name:
             raise ValueError("app_name must be set")
 
-        if not broker_url:
-            broker_url = f"redis://{DEFAULT_HOST}:{DEFAULT_PORT}/0"
+        if not broker.get_broker_name():
+            raise ValueError("invalid broker")
 
-        db = int(broker_url.split('/')[-1])
-        host = broker_url.split('/')[2].split(':')[0]
-        port = int(broker_url.split('/')[2].split(':')[1])
-
-        self.consumer = _Consumer(db=db, host=host, port=port, app_name=app_name, logfile=logfile)
-        self.publisher = _Publisher(db=db, host=host, port=port, app_name=app_name, logfile=logfile)
+        self.consumer = _Consumer(broker=broker, app_name=app_name, logfile=logfile)
+        self.publisher = _Publisher(broker=broker, app_name=app_name, logfile=logfile)
         self.logfile = logfile
 
     def start(self, *args, **kwargs):
         """Use this method to consume tasks from the message broker
 
         Example:
             negotium.start()
```

### Comparing `negotium-0.2.0/negotium/mq/consumer.py` & `negotium-0.2.1/negotium/mq/consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 import json
 import os
 import signal
 import sys
 import time
 from threading import Thread, Timer
 
+from negotium.brokers.main import MessageBroker, BROKER_REDIS
 from negotium.mq.trackers import _MessageTracker
 from negotium.settings import (
     _MESSAGE_MAIN, _MESSAGE_SCHEDULER, _MESSAGE_SCHEDULER_SORTED_SET, _MESSAGE_PERIODIC_TASKS
 )
 from negotium.utils.logger import log
 
 
 class _Consumer:
-    def __init__(self, db: int, host: str, port: int, app_name: str, logfile: str=None):
-        self.connection = redis.Redis(db=db, host=host, port=port)
-        self._tracker = _MessageTracker(self.connection, app_name)
+    def __init__(self, broker: MessageBroker, app_name: str, logfile: str=None):
+        self.broker = broker
+        self.connection = broker.connect()
+        self._tracker = _MessageTracker(broker, app_name)
         self._is_closed = False
         self.app_name = app_name
         self.logfile = logfile
         self._thread_consume = None
         self._thread_consume_scheduled = None
         self._thread_consume_periodic = None
 
@@ -37,45 +39,56 @@
         """Delete a message
         """
         self._tracker._delete(uuid_)
 
     def _consume(self, *args, **kwargs):
         """Consume messages from the queue
         """
-        while True:
-            if self._is_closed:
-                return
-            message = self.connection.blpop(_MESSAGE_MAIN + "__" + self.app_name)
-            self._callback(message[1])
-            time.sleep(1)
+        if self.broker.get_broker_name() == BROKER_REDIS:
+            while True:
+                if self._is_closed:
+                    return
+                message = self.connection.blpop(_MESSAGE_MAIN + "__" + self.app_name)
+                self._callback(message[1])
+                time.sleep(1)
+        else:
+            raise NotImplementedError("Broker not implemented")
 
     def _consume_scheduled_tasks(self, *args, **kwargs):
         """Load scheduled tasks
         """
-        while True:
-            if self._is_closed:
-                return
-            current_time = datetime.datetime.now().timestamp()
-            tasks = self.connection.zrangebyscore(_MESSAGE_SCHEDULER_SORTED_SET + "__" + self.app_name, 0, current_time)
-            for task in tasks:
-                task = json.loads(task.decode('utf-8'))
-                eta = task.get('_eta')
-                task = task.get('_task')
-                self.connection.zrem(_MESSAGE_SCHEDULER_SORTED_SET + "__" + self.app_name, json.dumps({
-                    '_task': task,
-                    '_eta': eta
-                }))
-                # execute task
-                self._callback_scheduled(json.dumps(task), eta)
-            time.sleep(1)
+        if self.broker.get_broker_name() == BROKER_REDIS:
+            while True:
+                if self._is_closed:
+                    return
+                current_time = datetime.datetime.now().timestamp()
+                tasks = self.connection.zrangebyscore(_MESSAGE_SCHEDULER_SORTED_SET + "__" + self.app_name, 0, current_time)
+                for task in tasks:
+                    task = json.loads(task.decode('utf-8'))
+                    eta = task.get('_eta')
+                    task = task.get('_task')
+                    self.connection.zrem(_MESSAGE_SCHEDULER_SORTED_SET + "__" + self.app_name, json.dumps({
+                        '_task': task,
+                        '_eta': eta
+                    }))
+                    # execute task
+                    self._callback_scheduled(json.dumps(task), eta)
+                time.sleep(1)
+        else:
+            raise NotImplementedError("Broker not implemented")
 
     def _consume_periodic_tasks(self, *args, **kwargs):
         """Load periodic tasks
         """
-        tasks = self.connection.lrange(_MESSAGE_PERIODIC_TASKS + "__" + self.app_name, 0, -1)
+        tasks = []
+        if self.broker.get_broker_name() == BROKER_REDIS:
+            tasks = self.connection.lrange(_MESSAGE_PERIODIC_TASKS + "__" + self.app_name, 0, -1)
+        else:
+            raise NotImplementedError("Broker not implemented")
+
         for task in tasks:
             body = json.loads(task.decode('utf-8'))
             cron = body.get('_cron')
             task = body.get('_task')
 
             # schedule task with the given cron
             croniter_ = croniter.croniter(cron, datetime.datetime.now())
@@ -149,20 +162,12 @@
         self._thread_consume_scheduled = Thread(target=self._consume_scheduled_tasks, daemon=True)
         self._thread_consume_periodic = Thread(target=self._consume_periodic_tasks, daemon=True)
         # start threads
         self._thread_consume.start()
         self._thread_consume_scheduled.start()
         self._thread_consume_periodic.start()
 
-    def _signal_handler(self, sig, frame):
-        """Handle signals
-        """
-        # close the connection
-        self.close()
-        # exit
-        os._exit(1)
-
     def close(self):
         """Close the connection
         """
         self._is_closed = True
         self._close_connection()
```

### Comparing `negotium-0.2.0/negotium/mq/publisher.py` & `negotium-0.2.1/negotium/mq/publisher.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 import datetime
 import json
 import redis
 
+from negotium.brokers.main import MessageBroker, BROKER_REDIS
 from negotium.mq.trackers import _MessageTracker
-from negotium.mq.trackers import _COMMAND_ZREM, _COMMAND_LREM, _COMMAND_BLPOP
+from negotium.mq.trackers import _COMMAND_REDIS_ZREM, _COMMAND_REDIS_LREM, _COMMAND_REDIS_BLPOP
 from negotium.settings import (
     _MESSAGE_MAIN, _MESSAGE_SCHEDULER, _MESSAGE_SCHEDULER_SORTED_SET, _MESSAGE_PERIODIC_TASKS
 )
 from negotium.schedules.crontab import Crontab
 from negotium.utils.logger import log
 
 class _Publisher:
-    def __init__(self, db: int, host: str, port: int, app_name: str, logfile: str=None):
+    def __init__(self, broker: MessageBroker, app_name: str, logfile: str=None):
+        self.broker = broker
         self.connection = None
         self._tracker = None
-        self.db = db
-        self.host = host
-        self.port = port
         self.app_name = app_name
         self.logfile = logfile
 
     def _create_connection(self):
         """Create a connection to the message broker
         """
-        self.connection = redis.Redis(db=self.db, host=self.host, port=self.port)
-        self._tracker = _MessageTracker(self.connection, self.app_name)
+        self.connection = self.broker.connect()
+        self._tracker = _MessageTracker(self.broker, self.app_name)
 
     def _close_connection(self):
         """Close the connection
         """
         self.connection.close()
 
     def _publish(self, data: dict, eta: datetime.datetime=None, cron: Crontab=None) -> str:
         """Publish a message to the queue and return the message id
         """
         log(self.logfile, data.get('app_name'), f"Received task: {data.get('function_name')}")
-        if eta:
-            data = {
-                '_task': data,
-                '_eta': eta.strftime('%Y-%m-%d %H:%M:%S.%f')
-            }
-            self.connection.rpush(_MESSAGE_SCHEDULER + "__" + self.app_name, json.dumps(data))
-            message_id = self._tracker._track(
-                name=_MESSAGE_SCHEDULER + "__" + self.app_name, 
-                identifier=json.dumps(data), 
-                command=_COMMAND_LREM
-            )
-
-            timestamp = datetime.datetime.strptime(eta.strftime('%Y-%m-%d %H:%M:%S.%f'), '%Y-%m-%d %H:%M:%S.%f').timestamp()
-            self.connection.zadd(_MESSAGE_SCHEDULER_SORTED_SET + "__" + self.app_name, {json.dumps(data): timestamp})
-            return self._tracker._track(
-                name=_MESSAGE_SCHEDULER_SORTED_SET + "__" + self.app_name,
-                identifier=json.dumps(data),
-                command=_COMMAND_ZREM,
-                uuid_=message_id
-            )
-        elif cron:
-            data = {
-                '_task': data,
-                '_cron': cron.__str__()
-            }
-            self.connection.rpush(_MESSAGE_PERIODIC_TASKS + "__" + self.app_name, json.dumps(data))
-            return self._tracker._track(
-                name=_MESSAGE_PERIODIC_TASKS + "__" + self.app_name,
-                identifier=json.dumps(data), 
-                command=_COMMAND_LREM
-            )
+        if self.broker.get_broker_name() == BROKER_REDIS:
+            if eta:
+                data = {
+                    '_task': data,
+                    '_eta': eta.strftime('%Y-%m-%d %H:%M:%S.%f')
+                }
+                self.connection.rpush(_MESSAGE_SCHEDULER + "__" + self.app_name, json.dumps(data))
+                message_id = self._tracker._track(
+                    name=_MESSAGE_SCHEDULER + "__" + self.app_name, 
+                    identifier=json.dumps(data), 
+                    command=_COMMAND_REDIS_LREM
+                )
+
+                timestamp = datetime.datetime.strptime(eta.strftime('%Y-%m-%d %H:%M:%S.%f'), '%Y-%m-%d %H:%M:%S.%f').timestamp()
+                self.connection.zadd(_MESSAGE_SCHEDULER_SORTED_SET + "__" + self.app_name, {json.dumps(data): timestamp})
+                return self._tracker._track(
+                    name=_MESSAGE_SCHEDULER_SORTED_SET + "__" + self.app_name,
+                    identifier=json.dumps(data),
+                    command=_COMMAND_REDIS_ZREM,
+                    uuid_=message_id
+                )
+            elif cron:
+                data = {
+                    '_task': data,
+                    '_cron': cron.__str__()
+                }
+                self.connection.rpush(_MESSAGE_PERIODIC_TASKS + "__" + self.app_name, json.dumps(data))
+                return self._tracker._track(
+                    name=_MESSAGE_PERIODIC_TASKS + "__" + self.app_name,
+                    identifier=json.dumps(data), 
+                    command=_COMMAND_REDIS_LREM
+                )
+            else:
+                self.connection.rpush(_MESSAGE_MAIN + "__" + self.app_name, json.dumps(data))
+                return self._tracker._track(
+                    name=_MESSAGE_MAIN + "__" + self.app_name,
+                    command=_COMMAND_REDIS_BLPOP
+                )
         else:
-            self.connection.rpush(_MESSAGE_MAIN + "__" + self.app_name, json.dumps(data))
-            return self._tracker._track(
-                name=_MESSAGE_MAIN + "__" + self.app_name,
-                command=_COMMAND_BLPOP
-            )
-
+            raise NotImplementedError("Broker not implemented")
```

### Comparing `negotium-0.2.0/negotium/schedules/crontab.py` & `negotium-0.2.1/negotium/schedules/crontab.py`

 * *Files identical despite different names*

### Comparing `negotium-0.2.0/negotium/settings.py` & `negotium-0.2.1/negotium/settings.py`

 * *Files identical despite different names*

### Comparing `negotium-0.2.0/negotium/task.py` & `negotium-0.2.1/negotium/task.py`

 * *Files identical despite different names*

### Comparing `negotium-0.2.0/negotium/utils/logger.py` & `negotium-0.2.1/negotium/utils/logger.py`

 * *Files identical despite different names*

### Comparing `negotium-0.2.0/negotium.egg-info/PKG-INFO` & `negotium-0.2.1/negotium.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: negotium
-Version: 0.2.0
-Summary: A very simple asynchronous task/job queue
+Version: 0.2.1
+Summary: A lightweight and easy to use task queue/scheduler
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Negotium
 
-A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. For now, it offers only a minimal set of features, which will be expanded. It also currently only supports Redis as the broker; however, it is planned to support other brokers in the future.
+A simple, lightweight, and easy-to-use task/job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. For now, it offers only a minimal set of features, which will be expanded. It also currently only supports Redis as the broker; however, it is planned to support other brokers in the future.
 
 ## Installation
 
 ```bash
 pip install negotium
 ```
 
@@ -23,16 +23,27 @@
 - Task cancellation: All tasks are cancellable using the UUID returned by the task execution methods: `delay`, `apply_async`, and `apply_periodic_async`
 
 ## Usage
 
 ```python
 # ---- main.py (app entry point) ----
 from negotium import Negotium
+from negotium.brokers import Redis
 
-app = Negotium(broker_url="redis://localhost:6379/0", app_name="my_app")
+# create broker
+broker = Redis(
+    host='localhost',
+    port=6379,
+    user='default', # optional
+    password='password', # optional
+    db=0 # optional (defaults to 0)
+)
+
+# create negotium app
+app = Negotium(app_name="<YOUR_APP_NAME>", broker=broker)
 app.start()
 
 @app.task
 def add(x, y):
     return x + y
 ```
 
@@ -66,15 +77,15 @@
 
 # run the task every minute
 task_id = add.apply_periodic_async(args=(1, 2), cron=Crontab(minute=1))
 
 # with a raw crontab expression
 task_id = add.apply_periodic_async(args=(1, 2), cron=Crontab(expression="* * * * *"))
 
-# to cancel, import the app object and call the `cancel` method
+# to cancel, call the `cancel` method
 app.cancel(task_id)
 ```
 
 ### Using in a Django project
 
 - Create a `negotium.py` file in your Django project directory
 ```
@@ -89,21 +100,30 @@
 ```
 
 - Add the following code to the `negotium.py` file
 ```python
 import os
 
 from negotium import Negotium
+from negotium.brokers import Redis
 
 # Set the django settings module
 os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'my_project.settings')
 
+# Create the broker
+broker = Redis(
+    host='localhost',
+    port=6379,
+    user='default', # optional
+    password='password', # optional
+    db=0 # optional (defaults to 0)
+)
+
 # Create the negotium app
-# If not specified, the broker url defaults to redis://localhost:6379/0
-app = Negotium(broker_url="redis://localhost:6379/0", app_name="my_app")
+app = Negotium(app_name="<YOUR_APP_NAME>", broker=broker)
 app.start()
 ```
 
 - Import the `app` object in your task modules
 ```python
 # --- example/tasks.py ---
 from my_project.negotium import app
```

### Comparing `negotium-0.2.0/negotium.egg-info/SOURCES.txt` & `negotium-0.2.1/negotium.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 negotium/settings.py
 negotium/task.py
 negotium.egg-info/PKG-INFO
 negotium.egg-info/SOURCES.txt
 negotium.egg-info/dependency_links.txt
 negotium.egg-info/requires.txt
 negotium.egg-info/top_level.txt
+negotium/brokers/__init__.py
+negotium/brokers/main.py
+negotium/brokers/redis.py
 negotium/mq/__init__.py
 negotium/mq/consumer.py
 negotium/mq/publisher.py
 negotium/mq/trackers.py
 negotium/schedules/__init__.py
 negotium/schedules/crontab.py
 negotium/utils/__init__.py
```

