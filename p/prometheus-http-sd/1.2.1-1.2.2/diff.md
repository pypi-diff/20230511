# Comparing `tmp/prometheus_http_sd-1.2.1.tar.gz` & `tmp/prometheus_http_sd-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_http_sd-1.2.1.tar", max compression
+gzip compressed data, was "prometheus_http_sd-1.2.2.tar", max compression
```

## Comparing `prometheus_http_sd-1.2.1.tar` & `prometheus_http_sd-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-04-27 08:34:14.317610 prometheus_http_sd-1.2.1/LICENSE
--rw-r--r--   0        0        0    11097 2023-04-27 08:34:14.317610 prometheus_http_sd-1.2.1/README.md
--rw-r--r--   0        0        0        0 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/__init__.py
--rw-r--r--   0        0        0     3400 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/app.py
--rw-r--r--   0        0        0     2398 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/cli.py
--rw-r--r--   0        0        0      110 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/config.py
--rw-r--r--   0        0        0       45 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/const.py
--rw-r--r--   0        0        0     6504 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/decorator.py
--rw-r--r--   0        0        0        0 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/exceptions.py
--rw-r--r--   0        0        0     1165 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/mem_perf.py
--rw-r--r--   0        0        0     6265 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/sd.py
--rw-r--r--   0        0        0      147 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/targets.py
--rw-r--r--   0        0        0     1148 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/templates/admin.html
--rw-r--r--   0        0        0     2118 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/validate.py
--rw-r--r--   0        0        0       18 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/version.py
--rw-r--r--   0        0        0      566 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    11787 1970-01-01 00:00:00.000000 prometheus_http_sd-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-11 03:51:33.194050 prometheus_http_sd-1.2.2/LICENSE
+-rw-r--r--   0        0        0    11097 2023-05-11 03:51:33.194050 prometheus_http_sd-1.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/__init__.py
+-rw-r--r--   0        0        0     3400 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/app.py
+-rw-r--r--   0        0        0     2398 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/cli.py
+-rw-r--r--   0        0        0      110 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/config.py
+-rw-r--r--   0        0        0       45 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/const.py
+-rw-r--r--   0        0        0     6443 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/decorator.py
+-rw-r--r--   0        0        0        0 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/exceptions.py
+-rw-r--r--   0        0        0     1165 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/mem_perf.py
+-rw-r--r--   0        0        0     4964 2023-05-11 03:51:33.202050 prometheus_http_sd-1.2.2/prometheus_http_sd/sd.py
+-rw-r--r--   0        0        0      147 2023-05-11 03:51:33.202050 prometheus_http_sd-1.2.2/prometheus_http_sd/targets.py
+-rw-r--r--   0        0        0     1148 2023-05-11 03:51:33.202050 prometheus_http_sd-1.2.2/prometheus_http_sd/templates/admin.html
+-rw-r--r--   0        0        0     2118 2023-05-11 03:51:33.202050 prometheus_http_sd-1.2.2/prometheus_http_sd/validate.py
+-rw-r--r--   0        0        0       18 2023-05-11 03:51:33.202050 prometheus_http_sd-1.2.2/prometheus_http_sd/version.py
+-rw-r--r--   0        0        0      648 2023-05-11 03:51:33.202050 prometheus_http_sd-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    11866 1970-01-01 00:00:00.000000 prometheus_http_sd-1.2.2/PKG-INFO
```

### Comparing `prometheus_http_sd-1.2.1/LICENSE` & `prometheus_http_sd-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.1/README.md` & `prometheus_http_sd-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.1/prometheus_http_sd/app.py` & `prometheus_http_sd-1.2.2/prometheus_http_sd/app.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.1/prometheus_http_sd/cli.py` & `prometheus_http_sd-1.2.2/prometheus_http_sd/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.1/prometheus_http_sd/decorator.py` & `prometheus_http_sd-1.2.2/prometheus_http_sd/decorator.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,16 @@
     pass
 
 
 class TimeoutDecorator:
     def __init__(
         self,
         timeout=None,
-        cache_time=60 * 5,
+        cache_time=0,
+        name="",
         garbage_collection_interval=5,
         garbage_collection_count=30,
     ):
         """
         Use threading and cache to store the function result.
 
         Garbage Collection time complexity:
@@ -52,27 +53,28 @@
         ----------
         timeout: int
             function timeout. if exceed, raise TimeoutException (in sec).
         cache_time: int
             after function return normally,
                 how long should we cache the result (in sec).
         name: str
-            prometheus_client metrics label
+            prometheus_client metrics prefix
         garbage_collection_count: int
             garbage collection threshold
         garbage_collection_interval: int
             the second to avoid collection too often.
 
         Returns
         -------
         TimeoutDecorator
             decorator class.
         """
         self.timeout = timeout
         self.cache_time = cache_time
+        self.name = name
         self.garbage_collection_interval = garbage_collection_interval
         self.garbage_collection_count = garbage_collection_count
 
         self.thread_cache = {}
         self.cache_lock = threading.Lock()
         self.heap = []
         self.heap_lock = threading.Lock()
@@ -84,15 +86,15 @@
         return (
             self.garbage_collection_interval
             + self.garbage_collection_timestamp
             < time.time()
             and len(self.heap) > self.garbage_collection_count
         )
 
-    def _cache_garbage_collection(self, name_label):
+    def _cache_garbage_collection(self):
         def can_iterate():
             with self.heap_lock:
                 if len(self.heap) == 0 or self.heap[0][0] > time.time():
                     return False
             return True
 
         worked_keys = {}
@@ -104,38 +106,36 @@
                 continue
             worked_keys[_key] = True
             with self.cache_lock:
                 if _key not in self.thread_cache:
                     continue
                 if self.is_expired(self.thread_cache[_key]):
                     del self.thread_cache[_key]
-                    _collected_total.labels(name=name_label).inc(1)
+                    _collected_total.labels(name=self.name).inc(1)
         _heap_cache_count.labels(
-            name=name_label,
+            name=self.name,
         ).set(len(self.heap))
         _thread_cache_count.labels(
-            name=name_label,
+            name=self.name,
         ).set(len(self.thread_cache))
         current_time = time.time()
         if self.garbage_collection_timestamp != 0:
             _collection_run_interval.labels(
-                name=name_label,
+                name=self.name,
             ).observe(current_time - self.garbage_collection_timestamp)
         self.garbage_collection_timestamp = current_time
 
     def is_expired(self, cache):
         """Check thread_cache dict is expired."""
         return cache["expired_timestamp"] < time.time()
 
     def _cal_cache_key(*arg, **kwargs):
         return hash(tuple([hash(arg), tuple(sorted(kwargs.items()))]))
 
     def __call__(self, function):
-        name_label = f"{function.__module__}/{function.__funcname__}"
-
         def wrapper(*arg, **kwargs):
             cache = {
                 "thread": None,
                 "error": None,
                 "response": None,
                 "expired_timestamp": float("inf"),
             }
@@ -149,15 +149,15 @@
                             self.heap,
                             (
                                 cache["expired_timestamp"],
                                 key,
                             ),
                         )
                         _heap_cache_count.labels(
-                            name=name_label,
+                            name=self.name,
                         ).set(len(self.heap))
                 except Exception as e:
                     cache["error"] = e
 
             key = self._cal_cache_key(*arg, **kwargs)
             with self.cache_lock:
                 if key in self.thread_cache:
@@ -171,24 +171,24 @@
                     cache["thread"] = threading.Thread(
                         target=target_function,
                         args=(key,),
                     )
                     cache["thread"].start()
                 self.thread_cache[key] = cache
                 _thread_cache_count.labels(
-                    name=name_label,
+                    name=self.name,
                 ).set(len(self.thread_cache))
             cache["thread"].join(self.timeout)
 
             if (
                 self.can_garbage_collection()
                 and self.garbage_collection_lock.acquire(False)
             ):
                 try:
-                    self._cache_garbage_collection(name_label)
+                    self._cache_garbage_collection()
                 finally:
                     self.garbage_collection_lock.release()
             if cache["thread"].is_alive():
                 raise TimeoutException("target function timeout!")
             if cache["error"]:
                 raise cache["error"]
             return cache["response"]
```

### Comparing `prometheus_http_sd-1.2.1/prometheus_http_sd/mem_perf.py` & `prometheus_http_sd-1.2.2/prometheus_http_sd/mem_perf.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.1/prometheus_http_sd/sd.py` & `prometheus_http_sd-1.2.2/prometheus_http_sd/sd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import os
 import json
-import time
 import logging
 import importlib
 import importlib.machinery
 
 import importlib.util
 from pathlib import Path
-from collections import namedtuple
 
 from typing import List
 from .targets import TargetList
 from .const import TEST_ENV_NAME
 from prometheus_client import Gauge, Counter, Histogram
-from threading import Lock
+from prometheus_http_sd.decorator import TimeoutDecorator
 
 import yaml
 
 try:
     from yaml import CLoader as Loader
 except ImportError:
     from yaml import Loader
@@ -142,93 +140,40 @@
 
 
 def run_json(file_path: str) -> TargetList:
     with open(file_path) as jsonf:
         return json.load(jsonf)
 
 
-python_targets_cache = {}
-
-CacheEntry = namedtuple("CacheEntry", "created_timestamp value")
-CACHE_TIMEOUT = 60
-
-python_targets_locks = {}
-
-
-def _get_cache(key):
-    result = python_targets_cache.get(key)
-    if not result:
-        return None
-
-    if time.time() - result.created_timestamp > 60:
-        return None
-
-    logger.info("Cache hit for key: %s", key)
-    return result.value
-
-
-def get_lock(path):
-    if path not in python_targets_locks:
-        python_targets_locks[path] = Lock()
-    return python_targets_locks[path]
-
-
-def get_cache_key(path, **extra_args):
-    keys = sorted(extra_args.keys())
-
-    cache_key = path
-    for key in keys:
-        cache_key += f"/{key}:{extra_args[key]}"
-
-    return cache_key
-
-
+@TimeoutDecorator(
+    timeout=60,
+    cache_time=60,
+    name="target_generator",
+    garbage_collection_count=100,
+)
 def run_python(generator_path, **extra_args) -> TargetList:
     logger.debug(f"start to import module {generator_path}...")
 
-    cache_key = get_cache_key(generator_path, **extra_args)
-
-    cached = _get_cache(cache_key)
-    if cached:
-        return cached
-    logger.info("%s Cache not hit", cache_key)
-
-    lock = get_lock(cache_key)
-
-    with lock:
-        cached = _get_cache(cache_key)
-        if cached:
-            logger.info("%s Cache hit in lock", cache_key)
-            return cached
-        logger.info("%s Cache not hit in lock, run script...", cache_key)
+    loader = importlib.machinery.SourceFileLoader("mymodule", generator_path)
+    spec = importlib.util.spec_from_loader("mymodule", loader)
+    if spec:
+        mymodule = importlib.util.module_from_spec(spec)
+        loader.exec_module(mymodule)
+    else:
+        raise Exception("Load a None module!")
+    func = getattr(mymodule, "generate_targets")
 
-        loader = importlib.machinery.SourceFileLoader(
-            "mymodule", generator_path
-        )
-        spec = importlib.util.spec_from_loader("mymodule", loader)
-        if spec:
-            mymodule = importlib.util.module_from_spec(spec)
-            loader.exec_module(mymodule)
+    if os.getenv(TEST_ENV_NAME) == "1":
+        try:
+            test_func = getattr(mymodule, "test_generate_targets")
+        except AttributeError:
+            pass
         else:
-            raise Exception("Load a None module!")
-        func = getattr(mymodule, "generate_targets")
-
-        if os.getenv(TEST_ENV_NAME) == "1":
-            try:
-                test_func = getattr(mymodule, "test_generate_targets")
-            except AttributeError:
-                pass
-            else:
-                func = test_func
-        result = func(**extra_args)
-        python_targets_cache[generator_path] = CacheEntry(
-            created_timestamp=time.time(), value=result
-        )
-
-    return result
+            func = test_func
+    return func(**extra_args)
 
 
 def run_yaml(file_path: str):
     with open(file_path) as yamlf:
         data = yaml.load(yamlf, Loader=Loader)
         return data
```

### Comparing `prometheus_http_sd-1.2.1/prometheus_http_sd/templates/admin.html` & `prometheus_http_sd-1.2.2/prometheus_http_sd/templates/admin.html`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.1/prometheus_http_sd/validate.py` & `prometheus_http_sd-1.2.2/prometheus_http_sd/validate.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.1/pyproject.toml` & `prometheus_http_sd-1.2.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [tool.poetry]
 name = "prometheus-http-sd"
-version = "1.2.1"
+version = "1.2.2"
 description = "Prometheus HTTP SD framework."
 authors = ["laixintao <laixintaoo@gmail.com>"]
 readme = 'README.md'
+homepage = "https://python-poetry.org://github.com/laixintao/prometheus-http-sd"
+
 
 [tool.poetry.dependencies]
 python = "^3.7"
 Flask = "^2.1.3"
 waitress = "^2.1.2"
 prometheus-client = "^0.14.1"
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 flake8 = "^4.0.1"
 
 [build-system]
-requires = ["poetry-core>=1.2.1"]
+requires = ["poetry-core>=1.2.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
 
 [tool.poetry.scripts]
 prometheus-http-sd = 'prometheus_http_sd.cli:main'
```

### Comparing `prometheus_http_sd-1.2.1/PKG-INFO` & `prometheus_http_sd-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: prometheus-http-sd
-Version: 1.2.1
+Version: 1.2.2
 Summary: Prometheus HTTP SD framework.
+Home-page: https://python-poetry.org://github.com/laixintao/prometheus-http-sd
 Author: laixintao
 Author-email: laixintaoo@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

