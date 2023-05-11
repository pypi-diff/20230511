# Comparing `tmp/aiormq-6.7.4.tar.gz` & `tmp/aiormq-6.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiormq-6.7.4.tar", max compression
+gzip compressed data, was "aiormq-6.7.5.tar", max compression
```

## Comparing `aiormq-6.7.4.tar` & `aiormq-6.7.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    17426 2023-02-18 21:26:40.811315 aiormq-6.7.4/README.rst
--rw-r--r--   0        0        0     1714 2022-12-15 11:27:13.176542 aiormq-6.7.4/aiormq/__init__.py
--rw-r--r--   0        0        0    17329 2023-03-04 21:14:59.608303 aiormq-6.7.4/aiormq/abc.py
--rw-r--r--   0        0        0      862 2022-12-12 22:30:18.703315 aiormq-6.7.4/aiormq/auth.py
--rw-r--r--   0        0        0     4800 2023-03-04 21:14:59.609646 aiormq-6.7.4/aiormq/base.py
--rw-r--r--   0        0        0    29504 2023-03-04 21:15:04.416263 aiormq-6.7.4/aiormq/channel.py
--rw-r--r--   0        0        0    29488 2023-03-10 11:48:03.537832 aiormq-6.7.4/aiormq/connection.py
--rw-r--r--   0        0        0     5831 2023-02-18 21:25:18.218614 aiormq-6.7.4/aiormq/exceptions.py
--rw-r--r--   0        0        0        0 2022-12-12 22:30:18.707721 aiormq-6.7.4/aiormq/py.typed
--rw-r--r--   0        0        0     3284 2023-03-04 21:14:59.614183 aiormq-6.7.4/aiormq/tools.py
--rw-r--r--   0        0        0      231 2023-03-04 21:14:59.615510 aiormq-6.7.4/aiormq/types.py
--rw-r--r--   0        0        0     2449 2023-03-10 15:39:14.461166 aiormq-6.7.4/pyproject.toml
--rw-r--r--   0        0        0    19407 1970-01-01 00:00:00.000000 aiormq-6.7.4/PKG-INFO
+-rw-r--r--   0        0        0    17426 2023-02-18 21:26:40.811315 aiormq-6.7.5/README.rst
+-rw-r--r--   0        0        0     1714 2022-12-15 11:27:13.176542 aiormq-6.7.5/aiormq/__init__.py
+-rw-r--r--   0        0        0    17329 2023-05-11 09:07:24.799939 aiormq-6.7.5/aiormq/abc.py
+-rw-r--r--   0        0        0      862 2022-12-12 22:30:18.703315 aiormq-6.7.5/aiormq/auth.py
+-rw-r--r--   0        0        0     4800 2023-05-11 09:07:24.801438 aiormq-6.7.5/aiormq/base.py
+-rw-r--r--   0        0        0    29505 2023-05-11 09:16:46.730769 aiormq-6.7.5/aiormq/channel.py
+-rw-r--r--   0        0        0    29886 2023-05-11 11:26:19.689530 aiormq-6.7.5/aiormq/connection.py
+-rw-r--r--   0        0        0     5831 2023-05-11 09:07:24.803621 aiormq-6.7.5/aiormq/exceptions.py
+-rw-r--r--   0        0        0        0 2022-12-12 22:30:18.707721 aiormq-6.7.5/aiormq/py.typed
+-rw-r--r--   0        0        0     3284 2023-05-11 09:07:24.804856 aiormq-6.7.5/aiormq/tools.py
+-rw-r--r--   0        0        0      231 2023-05-11 09:07:24.805425 aiormq-6.7.5/aiormq/types.py
+-rw-r--r--   0        0        0     2449 2023-05-11 11:26:19.690009 aiormq-6.7.5/pyproject.toml
+-rw-r--r--   0        0        0    19407 1970-01-01 00:00:00.000000 aiormq-6.7.5/PKG-INFO
```

### Comparing `aiormq-6.7.4/README.rst` & `aiormq-6.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.4/aiormq/__init__.py` & `aiormq-6.7.5/aiormq/__init__.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.4/aiormq/abc.py` & `aiormq-6.7.5/aiormq/abc.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.4/aiormq/auth.py` & `aiormq-6.7.5/aiormq/auth.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.4/aiormq/base.py` & `aiormq-6.7.5/aiormq/base.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.4/aiormq/channel.py` & `aiormq-6.7.5/aiormq/channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         super().__init__(loop=connector.loop, parent=connector)
 
         self.connection = connector
 
         if (
             publisher_confirms and not connector.publisher_confirms
         ):  # pragma: no cover
-            raise ValueError("Server does't support publisher confirms")
+            raise ValueError("Server doesn't support publisher confirms")
 
         self.consumers: Dict[str, ConsumerCallback] = {}
         self.confirmations = OrderedDict()
         self.message_id_delivery_tag: Dict[str, int] = dict()
 
         self.delivery_tag = 0
```

### Comparing `aiormq-6.7.4/aiormq/connection.py` & `aiormq-6.7.5/aiormq/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,29 +93,51 @@
 
     if exc_class is None:
         return ConnectionClosed(frame.reply_code, frame.reply_text)
 
     return exc_class(frame.reply_text)
 
 
-def parse_bool(v: str) -> bool:
-    return v == "1" or v.lower() in ("true", "yes", "y", "enable", "on")
+def parse_bool(v: Any) -> bool:
+    if isinstance(v, bool):
+        return v
 
+    v = str(v)
+    return v.lower() in (
+        "true", "yes", "y", "enable", "on", "enabled", "1"
+    )
 
-def parse_int(v: str) -> int:
+
+def parse_int(v: Any) -> int:
+    if isinstance(v, int):
+        return v
+
+    v = str(v)
     try:
         return int(v)
     except ValueError:
         return 0
 
 
-def parse_timeout(v: str) -> TimeoutType:
+def parse_timeout(v: Any) -> TimeoutType:
+    if isinstance(v, float):
+        if v.is_integer():
+            return int(v)
+        return v
+
+    if isinstance(v, int):
+        return v
+
+    v = str(v)
     try:
         if "." in v:
-            return float(v)
+            result = float(v)
+            if result.is_integer():
+                return int(result)
+            return result
         return int(v)
     except ValueError:
         return 0
 
 
 def parse_heartbeat(v: str) -> int:
     result = parse_int(v)
```

### Comparing `aiormq-6.7.4/aiormq/exceptions.py` & `aiormq-6.7.5/aiormq/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.4/aiormq/tools.py` & `aiormq-6.7.5/aiormq/tools.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.4/pyproject.toml` & `aiormq-6.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiormq"
-version = "6.7.4"
+version = "6.7.5"
 description = "Pure python AMQP asynchronous client library"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.rst"
 license = "Apache-2.0"
 keywords=["rabbitmq", "asyncio", "amqp", "amqp 0.9.1", "driver", "pamqp"]
 homepage = "https://github.com/mosquito/aiormq"
 classifiers = [
```

### Comparing `aiormq-6.7.4/PKG-INFO` & `aiormq-6.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiormq
-Version: 6.7.4
+Version: 6.7.5
 Summary: Pure python AMQP asynchronous client library
 Home-page: https://github.com/mosquito/aiormq
 License: Apache-2.0
 Keywords: rabbitmq,asyncio,amqp,amqp 0.9.1,driver,pamqp
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
```

