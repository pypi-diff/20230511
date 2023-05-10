# Comparing `tmp/llamatry-0.1.8.tar.gz` & `tmp/llamatry-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamatry-0.1.8.tar", max compression
+gzip compressed data, was "llamatry-0.1.9.tar", max compression
```

## Comparing `llamatry-0.1.8.tar` & `llamatry-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5687 2023-05-09 20:34:30.290019 llamatry-0.1.8/README.md
--rw-r--r--   0        0        0      123 2023-05-09 20:28:16.877771 llamatry-0.1.8/llamatry/__init__.py
--rw-r--r--   0        0        0     5337 2023-05-09 21:36:38.388807 llamatry-0.1.8/llamatry/openai.py
--rw-r--r--   0        0        0     2588 2023-05-09 21:26:04.302079 llamatry-0.1.8/llamatry/trace.py
--rw-r--r--   0        0        0      650 2023-05-09 21:46:24.030180 llamatry-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6527 1970-01-01 00:00:00.000000 llamatry-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     5691 2023-05-10 22:05:51.679440 llamatry-0.1.9/README.md
+-rw-r--r--   0        0        0      125 2023-05-10 22:11:52.442127 llamatry-0.1.9/llamatry/__init__.py
+-rw-r--r--   0        0        0     5044 2023-05-10 22:16:50.823503 llamatry-0.1.9/llamatry/openai.py
+-rw-r--r--   0        0        0     2593 2023-05-10 22:13:50.119018 llamatry-0.1.9/llamatry/trace.py
+-rw-r--r--   0        0        0      650 2023-05-10 22:16:38.129865 llamatry-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6531 1970-01-01 00:00:00.000000 llamatry-0.1.9/PKG-INFO
```

### Comparing `llamatry-0.1.8/README.md` & `llamatry-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     max_tokens=50,
     temperature=0.5,
 )
 ```
 
 Console Export:
 
-```
+```json
 {
     "name": "ChatCompletion.create",
     "context": {
         "trace_id": "0x6026b10ff364a1954df343ac2e292fd7",
         "span_id": "0x3f04991076717d88",
         "trace_state": "[]"
     },
```

### Comparing `llamatry-0.1.8/llamatry/openai.py` & `llamatry-0.1.9/llamatry/openai.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 from typing import Collection
 from opentelemetry import trace
-from opentelemetry import metrics
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 import openai
+import json
 
 tracer = trace.get_tracer("llamatry")
 
 
 class OpenAIInstrumentor(BaseInstrumentor):
     def _instrument(self, **kwargs):
         self._original_chatcompletion_create = openai.ChatCompletion.create
@@ -48,36 +48,30 @@
         ignoring the prompt and response attributes as they are may be too large
 
         :param span: the span to set attributes on
         :param kwargs: the kwargs passed to the create method
         :param response: the response from the create method
         """
         for key, value in kwargs.items():
-            if isinstance(value, (str, bool, float, int)) and key != "prompt":
-                # Don't set the prompt attribute as it may be too large
+            if isinstance(value, (str, bool, float, int)):
                 span.set_attribute(f"openai.create.{key}", value)
+            elif isinstance(value, (list, dict)):
+                span.set_attribute(f"openai.create.{key}", json.dumps(value))
 
         for key in ["id", "created", "model"]:
             if key in response:
                 span.set_attribute(f"openai.response.{key}", response[key])
 
         usage = response.get("usage", None)
         model = response.get("model", "__unknown__")
         if usage:
             for key in ["completion_tokens", "prompt_tokens", "total_tokens"]:
                 if key in usage:
                     span.set_attribute(f"openai.usage.{key}", usage[key])
-
-                    # Create a counter for the usage metric for each type of prompt token usage
-                    meter = metrics.get_meter(f"openai.{model}")
-                    counter = meter.create_counter(
-                        name=key,
-                        description=f"OpenAI {model} {key}",
-                    )
-                    counter.add(usage[key])
+        span.set_attribute("openai.response", json.dumps(response))
 
     def _trace_create(self, original_create):
         @functools.wraps(original_create)
         def wrapper(*args, **kwargs):
             stream = kwargs.get("stream", False)
 
             with tracer.start_as_current_span(
```

### Comparing `llamatry-0.1.8/llamatry/trace.py` & `llamatry-0.1.9/llamatry/trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
 from opentelemetry import trace
 from typing import Callable, Union
 
 import inspect
 
-tracer = trace.get_tracer("llamatry")
+_tracer = trace.get_tracer("llamatry")
 
 
 def simple_args_to_dict(func, *args, **kwargs):
     """
     Return a dictionary of the arguments
     Does not include default arguments or keyword arguments that are not strings
     This helps avoid sending too much data to the OpenTelemetry backend.
@@ -33,15 +33,15 @@
     return arg_dict
 
 
 def trace_decorator(*args: Union[str, Callable]) -> Union[Callable, None]:
     def _decorator(func: Callable, span_name: str) -> Callable:
         @functools.wraps(func)
         def wrapped(*args, **kwargs):
-            with tracer.start_as_current_span(span_name) as span:
+            with _tracer.start_as_current_span(span_name) as span:
                 result = func(*args, **kwargs)
 
                 arg_dict = simple_args_to_dict(func, *args, **kwargs)
                 for key, value in arg_dict.items():
                     span.set_attribute(key, value)
 
             return result
@@ -65,19 +65,19 @@
         )
 
         return _decorator(args[0], name)
     else:
         raise ValueError("Invalid arguments for trace_decorator")
 
 
-class Trace:
+class tracer:
     @classmethod
-    def trace(cls, *args, **kwargs):
+    def wrap(cls, *args, **kwargs):
         return trace_decorator(*args, **kwargs)
 
     @classmethod
-    def span(self, *args, **kwargs):
-        return tracer.start_as_current_span(*args, **kwargs)
+    def trace(self, *args, **kwargs):
+        return _tracer.start_as_current_span(*args, **kwargs)
 
     @classmethod
     def get_current_span(self):
-        return tracer.get_current_span()
+        return _tracer.get_current_span()
```

### Comparing `llamatry-0.1.8/pyproject.toml` & `llamatry-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llamatry"
-version = "0.1.8"
+version = "0.1.9"
 description = "opentelemetry instrumentation for openai's completions api"
 authors = ["Jason <jason@jxnl.co>"]
 readme = "README.md"
 repository = "https://github.com/jxnl/llamatry"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `llamatry-0.1.8/PKG-INFO` & `llamatry-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamatry
-Version: 0.1.8
+Version: 0.1.9
 Summary: opentelemetry instrumentation for openai's completions api
 Home-page: https://github.com/jxnl/llamatry
 Author: Jason
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -91,15 +91,15 @@
     max_tokens=50,
     temperature=0.5,
 )
 ```
 
 Console Export:
 
-```
+```json
 {
     "name": "ChatCompletion.create",
     "context": {
         "trace_id": "0x6026b10ff364a1954df343ac2e292fd7",
         "span_id": "0x3f04991076717d88",
         "trace_state": "[]"
     },
```

