# Comparing `tmp/tracers_spans_python-0.0.4.tar.gz` & `tmp/tracers_spans_python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracers_spans_python-0.0.4.tar", last modified: Thu May 11 02:04:40 2023, max compression
+gzip compressed data, was "tracers_spans_python-0.0.5.tar", last modified: Thu May 11 03:21:04 2023, max compression
```

## Comparing `tracers_spans_python-0.0.4.tar` & `tracers_spans_python-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mascarenhas  (1000) mascarenhas  (1000)        0 2023-05-11 02:04:40.278082 tracers_spans_python-0.0.4/
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)     1092 2023-05-10 14:03:52.000000 tracers_spans_python-0.0.4/LICENSE
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      730 2023-05-11 02:04:40.278082 tracers_spans_python-0.0.4/PKG-INFO
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      102 2023-05-11 02:04:40.280082 tracers_spans_python-0.0.4/setup.cfg
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      847 2023-05-11 02:04:31.000000 tracers_spans_python-0.0.4/setup.py
-drwxr-xr-x   0 mascarenhas  (1000) mascarenhas  (1000)        0 2023-05-11 02:04:40.267082 tracers_spans_python-0.0.4/tracers_spans_python/
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)       40 2023-05-11 02:03:23.000000 tracers_spans_python-0.0.4/tracers_spans_python/__init__.py
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)     3895 2023-05-10 22:59:02.000000 tracers_spans_python-0.0.4/tracers_spans_python/tracers_spans_python.py
-drwxr-xr-x   0 mascarenhas  (1000) mascarenhas  (1000)        0 2023-05-11 02:04:40.277082 tracers_spans_python-0.0.4/tracers_spans_python.egg-info/
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      730 2023-05-11 02:04:39.000000 tracers_spans_python-0.0.4/tracers_spans_python.egg-info/PKG-INFO
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      323 2023-05-11 02:04:39.000000 tracers_spans_python-0.0.4/tracers_spans_python.egg-info/SOURCES.txt
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)        1 2023-05-11 02:04:39.000000 tracers_spans_python-0.0.4/tracers_spans_python.egg-info/dependency_links.txt
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)       10 2023-05-11 02:04:39.000000 tracers_spans_python-0.0.4/tracers_spans_python.egg-info/requires.txt
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)       21 2023-05-11 02:04:39.000000 tracers_spans_python-0.0.4/tracers_spans_python.egg-info/top_level.txt
+drwxr-xr-x   0 mascarenhas  (1000) mascarenhas  (1000)        0 2023-05-11 03:21:04.792264 tracers_spans_python-0.0.5/
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)     1092 2023-05-10 14:03:52.000000 tracers_spans_python-0.0.5/LICENSE
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      730 2023-05-11 03:21:04.793264 tracers_spans_python-0.0.5/PKG-INFO
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      102 2023-05-11 03:21:04.796264 tracers_spans_python-0.0.5/setup.cfg
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      847 2023-05-11 03:20:57.000000 tracers_spans_python-0.0.5/setup.py
+drwxr-xr-x   0 mascarenhas  (1000) mascarenhas  (1000)        0 2023-05-11 03:21:04.774264 tracers_spans_python-0.0.5/tracers_spans_python/
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)       40 2023-05-11 02:03:23.000000 tracers_spans_python-0.0.5/tracers_spans_python/__init__.py
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)     4566 2023-05-11 02:30:26.000000 tracers_spans_python-0.0.5/tracers_spans_python/tracers_spans_python.py
+drwxr-xr-x   0 mascarenhas  (1000) mascarenhas  (1000)        0 2023-05-11 03:21:04.791264 tracers_spans_python-0.0.5/tracers_spans_python.egg-info/
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      730 2023-05-11 03:21:04.000000 tracers_spans_python-0.0.5/tracers_spans_python.egg-info/PKG-INFO
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      323 2023-05-11 03:21:04.000000 tracers_spans_python-0.0.5/tracers_spans_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)        1 2023-05-11 03:21:04.000000 tracers_spans_python-0.0.5/tracers_spans_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)       10 2023-05-11 03:21:04.000000 tracers_spans_python-0.0.5/tracers_spans_python.egg-info/requires.txt
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)       21 2023-05-11 03:21:04.000000 tracers_spans_python-0.0.5/tracers_spans_python.egg-info/top_level.txt
```

### Comparing `tracers_spans_python-0.0.4/LICENSE` & `tracers_spans_python-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tracers_spans_python-0.0.4/PKG-INFO` & `tracers_spans_python-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tracers_spans_python
-Version: 0.0.4
+Version: 0.0.5
 Summary: Projeto para facilitar a criação e envios de tracers e spans.
 Home-page: UNKNOWN
 Author: Otávio Mascarenhas
 Author-email: otaviomascarenhaspessoal@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: Tracers Spans tracers spans tracer span OpenTelemetry Zipkin
```

### Comparing `tracers_spans_python-0.0.4/setup.py` & `tracers_spans_python-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name = 'tracers_spans_python',
-    version = '0.0.4',
+    version = '0.0.5',
     author = 'Otávio Mascarenhas',
     author_email = 'otaviomascarenhaspessoal@gmail.com',
     packages = ['tracers_spans_python'],
     description = 'Projeto para facilitar a criação e envios de tracers e spans.',
     license = 'MIT',
     keywords = 'Tracers Spans tracers spans tracer span OpenTelemetry Zipkin',
     classifiers = [
```

### Comparing `tracers_spans_python-0.0.4/tracers_spans_python/tracers_spans_python.py` & `tracers_spans_python-0.0.5/tracers_spans_python/tracers_spans_python.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,34 @@
                     port=self.port,
                     service_name=self.service_name
                 )
                 self.tracer = await tool.create_tracer()
                 with self.tracer.new_trace(sampled=True) as self.span:
                     self.span.name(func.__name__)
                     
+                    result = func(*args, **kwargs)
+
+
+                return result
+            return wrapper
+        return decorator
+    
+    def new_async_tracer(self):
+        def decorator(func):
+            @wraps(func)
+            async def wrapper(*args, **kwargs):
+                tool = Tracer(
+                    host=self.host, ip_application=self.ipv4,
+                    port=self.port,
+                    service_name=self.service_name
+                )
+                self.tracer = await tool.create_tracer()
+                with self.tracer.new_trace(sampled=True) as self.span:
+                    self.span.name(func.__name__)
+                    
                     result = await func(*args, **kwargs)
 
 
                 return result
             return wrapper
         return decorator
```

### Comparing `tracers_spans_python-0.0.4/tracers_spans_python.egg-info/PKG-INFO` & `tracers_spans_python-0.0.5/tracers_spans_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tracers-spans-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: Projeto para facilitar a criação e envios de tracers e spans.
 Home-page: UNKNOWN
 Author: Otávio Mascarenhas
 Author-email: otaviomascarenhaspessoal@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: Tracers Spans tracers spans tracer span OpenTelemetry Zipkin
```

