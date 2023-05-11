# Comparing `tmp/forerunner-0.0.7.tar.gz` & `tmp/forerunner-0.0.8.tar.gz`

## Comparing `forerunner-0.0.7.tar` & `forerunner-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 forerunner-0.0.7/Makefile
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 forerunner-0.0.7/README.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/__init__.py
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/app.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/cli.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/console.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/module.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/server.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/utils.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/dependency/depends.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/dependency/utils.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/job/__init__.py
--rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/job/base.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/job/cron.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/job/sub.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/queue/__init__.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/queue/queue.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 forerunner-0.0.7/.gitignore
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 forerunner-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 forerunner-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 forerunner-0.0.8/Makefile
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 forerunner-0.0.8/README.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/__init__.py
+-rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/app.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/cli.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/console.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/module.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/server.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/utils.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/dependency/depends.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/dependency/utils.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/job/__init__.py
+-rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/job/base.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/job/cron.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/job/sub.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/queue/__init__.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 forerunner-0.0.8/src/forerunner/queue/queue.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 forerunner-0.0.8/.gitignore
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 forerunner-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 forerunner-0.0.8/PKG-INFO
```

### Comparing `forerunner-0.0.7/src/forerunner/app.py` & `forerunner-0.0.8/src/forerunner/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import signal
+from concurrent.futures import ThreadPoolExecutor
 from inspect import iscoroutinefunction
 from typing import Callable, List, Literal
 
 import uvicorn
 from prometheus_client import make_asgi_app
 from structlog import get_logger
 
@@ -19,20 +20,24 @@
 class App:
     def __init__(
         self,
         name: str = "app",
         *,
         modules: List[Module] = [],
         exception_callbacks: List[Callable] = [],
-        prometheus_enabled: bool = False,
+        metrics_server_enabled: bool = False,
+        metrics_server_port: int = 8001,
     ):
         self.name = name
         self.modules = modules
         self.exception_callbacks = exception_callbacks
-        self.prometheus_enabled = prometheus_enabled
+        self.metrics_server_enabled = metrics_server_enabled
+        self.metrics_server_port = metrics_server_port
+
+        self.threadpool_executor = ThreadPoolExecutor(max_workers=5)
 
         self._prometheus_asgi_server: MetricsServer | None = None
         self._prometheus_asgi_task: asyncio.Task | None = None
 
         self.logger = get_logger(app=self.name)
         self.jobs = []
 
@@ -114,18 +119,18 @@
             )
             self.jobs.append(job)
             return func
 
         return _sub_wrapper
 
     async def startup(self):
-        if self.prometheus_enabled:
+        if self.metrics_server_enabled:
             self.logger.debug("Starting prometheus web server...")
             asgi_app = make_asgi_app()
-            config = uvicorn.Config(asgi_app, port=8003)
+            config = uvicorn.Config(asgi_app, port=self.metrics_server_port)
             self._prometheus_asgi_server = MetricsServer(config)
             self._prometheus_asgi_app_task = asyncio.create_task(
                 self._prometheus_asgi_server.serve()
             )
             self.logger.debug("Started prometheus web server")
 
         self.logger.info("Starting...")
@@ -155,15 +160,15 @@
 
         if len(self.shutdown_funcs) > 0:
             self.logger.debug("Running shutdown funcs...")
             for func in self.shutdown_funcs:
                 await func() if iscoroutinefunction(func) else func()
 
         # Shutdown metrics webserver
-        if self.prometheus_enabled and self._prometheus_asgi_server is not None:
+        if self.metrics_server_enabled and self._prometheus_asgi_server is not None:
             self.logger.debug("Stopping prometheus web server...")
             self._prometheus_asgi_server.should_exit = True
             try:
                 await asyncio.wait_for(self._prometheus_asgi_app_task, timeout=30)
             except asyncio.TimeoutError:
                 self._prometheus_asgi_app_task.cancel()
             self.logger.debug("Stopped prometheus webserver")
```

### Comparing `forerunner-0.0.7/src/forerunner/module.py` & `forerunner-0.0.8/src/forerunner/module.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.7/src/forerunner/utils.py` & `forerunner-0.0.8/src/forerunner/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import importlib
 from typing import Any, Callable, List
 
-
 from .app import Module
 
 
 def init_module_jobs(
     *,
     app_name: str,
     exception_callbacks: List[Callable],
@@ -14,15 +13,15 @@
     """Recursively instantiate jobs for a Module
 
     The `app_name` and `exception_callbacks` kwargs are appended to each module's jobs
     and recursively updated to each modules children modules.
     """
     jobs = []
 
-    parent_app_name = f"{app_name}.{module.name}"
+    parent_app_name = f"{app_name}_{module.name}"
     parent_exception_callbacks = [
         *exception_callbacks,
         *module.exception_callbacks,
     ]
 
     for job_partial in module.job_partials:
         job_partial.keywords["app_name"] = parent_app_name
```

### Comparing `forerunner-0.0.7/src/forerunner/dependency/depends.py` & `forerunner-0.0.8/src/forerunner/dependency/depends.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.7/src/forerunner/dependency/utils.py` & `forerunner-0.0.8/src/forerunner/dependency/utils.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.7/src/forerunner/job/base.py` & `forerunner-0.0.8/src/forerunner/job/base.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.7/src/forerunner/job/cron.py` & `forerunner-0.0.8/src/forerunner/job/cron.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.7/src/forerunner/job/sub.py` & `forerunner-0.0.8/src/forerunner/job/sub.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.7/src/forerunner/queue/queue.py` & `forerunner-0.0.8/src/forerunner/queue/queue.py`

 * *Files identical despite different names*

