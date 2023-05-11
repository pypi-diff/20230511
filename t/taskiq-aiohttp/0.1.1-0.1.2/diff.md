# Comparing `tmp/taskiq_aiohttp-0.1.1.tar.gz` & `tmp/taskiq_aiohttp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aiohttp-0.1.1.tar", max compression
+gzip compressed data, was "taskiq_aiohttp-0.1.2.tar", max compression
```

## Comparing `taskiq_aiohttp-0.1.1.tar` & `taskiq_aiohttp-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-04-27 14:34:06.091547 taskiq_aiohttp-0.1.1/LICENSE
--rw-r--r--   0        0        0     1067 2023-04-27 14:34:06.091547 taskiq_aiohttp-0.1.1/README.md
--rw-r--r--   0        0        0     1716 2023-04-27 14:34:06.091547 taskiq_aiohttp-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      106 2023-04-27 14:34:06.091547 taskiq_aiohttp-0.1.1/taskiq_aiohttp/__init__.py
--rw-r--r--   0        0        0     3789 2023-04-27 14:34:06.091547 taskiq_aiohttp-0.1.1/taskiq_aiohttp/initializer.py
--rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 taskiq_aiohttp-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-11 12:40:45.933492 taskiq_aiohttp-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1067 2023-05-11 12:40:45.933492 taskiq_aiohttp-0.1.2/README.md
+-rw-r--r--   0        0        0     1716 2023-05-11 12:40:45.933492 taskiq_aiohttp-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-05-11 12:40:45.933492 taskiq_aiohttp-0.1.2/taskiq_aiohttp/__init__.py
+-rw-r--r--   0        0        0     4023 2023-05-11 12:40:45.933492 taskiq_aiohttp-0.1.2/taskiq_aiohttp/initializer.py
+-rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 taskiq_aiohttp-0.1.2/PKG-INFO
```

### Comparing `taskiq_aiohttp-0.1.1/LICENSE` & `taskiq_aiohttp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_aiohttp-0.1.1/README.md` & `taskiq_aiohttp-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_aiohttp-0.1.1/pyproject.toml` & `taskiq_aiohttp-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "taskiq-aiohttp"
 description = "Taskiq integration with AioHTTP framework"
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

### Comparing `taskiq_aiohttp-0.1.1/taskiq_aiohttp/initializer.py` & `taskiq_aiohttp-0.1.2/taskiq_aiohttp/initializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,19 +40,26 @@
         local_app = app
 
         if not isinstance(local_app, web.Application):
             local_app = local_app()
 
         if inspect.iscoroutine(local_app):
             local_app = await local_app
-
         if not isinstance(local_app, web.Application):
             raise ValueError(f"{app_path} is not an AioHTTP application.")
 
-        handler = RequestHandler(local_app._make_handler(), loop=loop)
+        # Starting the application.
+        app_runner = web.AppRunner(local_app)
+        await app_runner.setup()
+
+        if app_runner.server is None:
+            raise ValueError("Cannot construct aiohttp app to mock requests")
+
+        # Creating mocked request
+        handler = RequestHandler(app_runner.server, loop=loop)
         handler.transport = asyncio.Transport()
         request = web.Request(
             RawRequestMessage(
                 "GET",
                 "/",
                 HttpVersion10,
                 headers=CIMultiDictProxy(CIMultiDict()),
@@ -84,32 +91,31 @@
         broker.add_dependency_context(
             {
                 web.Application: local_app,
                 web.Request: request,
             },
         )
 
-        state.aiohttp_app = local_app
+        state.aiohttp_runner = app_runner
         local_app.router._resources = []
-        await local_app.startup()
 
     return startup
 
 
 async def shutdown(state: TaskiqState) -> None:
     """
     Shuts down the app.
 
     It just gets the application
     we created in startup and shuts it down.
 
     :param state: current state.
     """
-    await state.aiohttp_app.shutdown()
-    await state.aiohttp_app.cleanup()
+    await state.aiohttp_runner.shutdown()
+    await state.aiohttp_runner.cleanup()
 
 
 def init(broker: AsyncBroker, app_path: str) -> None:
     """
     Initialize dependencies for your taskiq.
 
     This function imports your application and tries to
```

### Comparing `taskiq_aiohttp-0.1.1/PKG-INFO` & `taskiq_aiohttp-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-aiohttp
-Version: 0.1.1
+Version: 0.1.2
 Summary: Taskiq integration with AioHTTP framework
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
 Maintainer-email: taskiq@no-reply.com
```

