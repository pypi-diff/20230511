# Comparing `tmp/taskiq_fastapi-0.1.1.tar.gz` & `tmp/taskiq_fastapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_fastapi-0.1.1.tar", max compression
+gzip compressed data, was "taskiq_fastapi-0.1.2.tar", max compression
```

## Comparing `taskiq_fastapi-0.1.1.tar` & `taskiq_fastapi-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-03-26 01:41:02.474291 taskiq_fastapi-0.1.1/LICENSE
--rw-r--r--   0        0        0     3641 2023-03-26 01:41:02.474291 taskiq_fastapi-0.1.1/README.md
--rw-r--r--   0        0        0     1568 2023-03-26 01:41:02.474291 taskiq_fastapi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      112 2023-03-26 01:41:02.474291 taskiq_fastapi-0.1.1/taskiq_fastapi/__init__.py
--rw-r--r--   0        0        0     2218 2023-03-26 01:41:02.474291 taskiq_fastapi-0.1.1/taskiq_fastapi/initializator.py
--rw-r--r--   0        0        0     4951 1970-01-01 00:00:00.000000 taskiq_fastapi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-11 21:11:59.963935 taskiq_fastapi-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4034 2023-05-11 21:11:59.963935 taskiq_fastapi-0.1.2/README.md
+-rw-r--r--   0        0        0     1568 2023-05-11 21:11:59.967935 taskiq_fastapi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-05-11 21:11:59.967935 taskiq_fastapi-0.1.2/taskiq_fastapi/__init__.py
+-rw-r--r--   0        0        0     2646 2023-05-11 21:11:59.967935 taskiq_fastapi-0.1.2/taskiq_fastapi/initializator.py
+-rw-r--r--   0        0        0     5344 1970-01-01 00:00:00.000000 taskiq_fastapi-0.1.2/PKG-INFO
```

### Comparing `taskiq_fastapi-0.1.1/LICENSE` & `taskiq_fastapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_fastapi-0.1.1/README.md` & `taskiq_fastapi-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -73,16 +73,16 @@
     await app.state.redis_pool.disconnect()
 
 
 # Here we call our magic function.
 taskiq_fastapi.init(broker, "test_script:app")
 
 
-# We use TaskiqDepends here, becuase if we use FastAPIDepends fastapi
-# initilization will fail.
+# We use TaskiqDepends here, because if we use FastAPIDepends fastapi
+# initialization will fail.
 def get_redis_pool(request: Request = TaskiqDepends()) -> ConnectionPool:
     return request.app.state.redis_pool
 
 
 @broker.task
 async def my_redis_task(
     key: str,
@@ -116,7 +116,23 @@
     key: str,
     pool: ConnectionPool = FastAPIDepends(get_redis_pool),
 ) -> str:
     async with Redis(connection_pool=pool, decode_responses=True) as redis:
         return await redis.get(key)
 
 ```
+
+## Manually update dependency context
+
+When using `InMemoryBroker` it may be required to update the dependency context manually. This may also be useful when setting up tests.
+
+```py
+import taskiq_fastapi
+from taskiq import InMemoryBroker
+
+broker = InMemoryBroker()
+
+app = FastAPI()
+
+taskiq_fastapi.init(broker, "test_script:app")
+taskiq_fastapi.populate_dependency_context(broker, app)
+```
```

### Comparing `taskiq_fastapi-0.1.1/pyproject.toml` & `taskiq_fastapi-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "taskiq-fastapi"
 description = "FastAPI integration for taskiq"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `taskiq_fastapi-0.1.1/taskiq_fastapi/initializator.py` & `taskiq_fastapi-0.1.2/taskiq_fastapi/initializator.py`

 * *Files 14% similar despite different names*

```diff
@@ -63,25 +63,41 @@
     app = import_object(app_path)
 
     if not isinstance(app, FastAPI):
         app = app()
 
     if not isinstance(app, FastAPI):
         raise ValueError(f"'{app_path}' is not a FastAPI application.")
-    scope = {"app": app, "type": "http"}
 
-    broker.add_dependency_context(
-        {
-            Request: Request(scope=scope),
-            HTTPConnection: HTTPConnection(scope=scope),
-        },
-    )
+    populate_dependency_context(broker, app)
 
     broker.add_event_handler(
         TaskiqEvents.WORKER_STARTUP,
         startup_event_generator(app),
     )
 
     broker.add_event_handler(
         TaskiqEvents.WORKER_SHUTDOWN,
         shutdown_event_generator(app),
     )
+
+
+def populate_dependency_context(broker: AsyncBroker, app: FastAPI) -> None:
+    """
+    Populate dependency context.
+
+    This function injects the Request and HTTPConnection
+    into the broker's dependency context.
+
+    It may be need to be called manually if you are using InMemoryBroker.
+
+    :param broker: current broker to use.
+    :param app: current application.
+    """
+    scope = {"app": app, "type": "http"}
+
+    broker.add_dependency_context(
+        {
+            Request: Request(scope=scope),
+            HTTPConnection: HTTPConnection(scope=scope),
+        },
+    )
```

### Comparing `taskiq_fastapi-0.1.1/PKG-INFO` & `taskiq_fastapi-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-fastapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: FastAPI integration for taskiq
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async,fastapi
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
 Maintainer-email: taskiq@no-reply.com
@@ -107,16 +107,16 @@
     await app.state.redis_pool.disconnect()
 
 
 # Here we call our magic function.
 taskiq_fastapi.init(broker, "test_script:app")
 
 
-# We use TaskiqDepends here, becuase if we use FastAPIDepends fastapi
-# initilization will fail.
+# We use TaskiqDepends here, because if we use FastAPIDepends fastapi
+# initialization will fail.
 def get_redis_pool(request: Request = TaskiqDepends()) -> ConnectionPool:
     return request.app.state.redis_pool
 
 
 @broker.task
 async def my_redis_task(
     key: str,
@@ -151,7 +151,23 @@
     pool: ConnectionPool = FastAPIDepends(get_redis_pool),
 ) -> str:
     async with Redis(connection_pool=pool, decode_responses=True) as redis:
         return await redis.get(key)
 
 ```
 
+## Manually update dependency context
+
+When using `InMemoryBroker` it may be required to update the dependency context manually. This may also be useful when setting up tests.
+
+```py
+import taskiq_fastapi
+from taskiq import InMemoryBroker
+
+broker = InMemoryBroker()
+
+app = FastAPI()
+
+taskiq_fastapi.init(broker, "test_script:app")
+taskiq_fastapi.populate_dependency_context(broker, app)
+```
+
```

