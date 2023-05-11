# Comparing `tmp/modernmt-1.2.0.tar.gz` & `tmp/modernmt-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modernmt-1.2.0.tar", last modified: Wed May  3 12:10:24 2023, max compression
+gzip compressed data, was "modernmt-1.2.1.tar", last modified: Thu May 11 09:26:43 2023, max compression
```

## Comparing `modernmt-1.2.0.tar` & `modernmt-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-03 12:10:24.283197 modernmt-1.2.0/
--rw-rw-r--   0 davide    (1000) davide    (1000)     1065 2021-05-05 13:02:28.000000 modernmt-1.2.0/LICENSE
--rw-rw-r--   0 davide    (1000) davide    (1000)      690 2023-05-03 12:10:24.283197 modernmt-1.2.0/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      197 2021-05-05 13:02:28.000000 modernmt-1.2.0/README.md
--rw-rw-r--   0 davide    (1000) davide    (1000)      105 2021-05-05 13:02:28.000000 modernmt-1.2.0/pyproject.toml
--rw-rw-r--   0 davide    (1000) davide    (1000)      648 2023-05-03 12:10:24.283197 modernmt-1.2.0/setup.cfg
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-03 12:10:24.283197 modernmt-1.2.0/src/
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-03 12:10:24.283197 modernmt-1.2.0/src/modernmt/
--rw-rw-r--   0 davide    (1000) davide    (1000)      166 2021-05-05 13:02:28.000000 modernmt-1.2.0/src/modernmt/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)    11241 2023-05-03 12:10:04.000000 modernmt-1.2.0/src/modernmt/modernmt.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-03 12:10:24.283197 modernmt-1.2.0/src/modernmt.egg-info/
--rw-rw-r--   0 davide    (1000) davide    (1000)      690 2023-05-03 12:10:24.000000 modernmt-1.2.0/src/modernmt.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      271 2023-05-03 12:10:24.000000 modernmt-1.2.0/src/modernmt.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-05-03 12:10:24.000000 modernmt-1.2.0/src/modernmt.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        9 2023-05-03 12:10:24.000000 modernmt-1.2.0/src/modernmt.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        9 2023-05-03 12:10:24.000000 modernmt-1.2.0/src/modernmt.egg-info/top_level.txt
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-11 09:26:43.846063 modernmt-1.2.1/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1065 2021-05-05 13:02:28.000000 modernmt-1.2.1/LICENSE
+-rw-rw-r--   0 davide    (1000) davide    (1000)      690 2023-05-11 09:26:43.846063 modernmt-1.2.1/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      197 2021-05-05 13:02:28.000000 modernmt-1.2.1/README.md
+-rw-rw-r--   0 davide    (1000) davide    (1000)      105 2021-05-05 13:02:28.000000 modernmt-1.2.1/pyproject.toml
+-rw-rw-r--   0 davide    (1000) davide    (1000)      648 2023-05-11 09:26:43.846063 modernmt-1.2.1/setup.cfg
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-11 09:26:43.842063 modernmt-1.2.1/src/
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-11 09:26:43.842063 modernmt-1.2.1/src/modernmt/
+-rw-rw-r--   0 davide    (1000) davide    (1000)      166 2021-05-05 13:02:28.000000 modernmt-1.2.1/src/modernmt/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)    10989 2023-05-11 09:26:35.000000 modernmt-1.2.1/src/modernmt/modernmt.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-11 09:26:43.846063 modernmt-1.2.1/src/modernmt.egg-info/
+-rw-rw-r--   0 davide    (1000) davide    (1000)      690 2023-05-11 09:26:43.000000 modernmt-1.2.1/src/modernmt.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      271 2023-05-11 09:26:43.000000 modernmt-1.2.1/src/modernmt.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-05-11 09:26:43.000000 modernmt-1.2.1/src/modernmt.egg-info/dependency_links.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        9 2023-05-11 09:26:43.000000 modernmt-1.2.1/src/modernmt.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        9 2023-05-11 09:26:43.000000 modernmt-1.2.1/src/modernmt.egg-info/top_level.txt
```

### Comparing `modernmt-1.2.0/LICENSE` & `modernmt-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modernmt-1.2.0/PKG-INFO` & `modernmt-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modernmt
-Version: 1.2.0
+Version: 1.2.1
 Summary: ModernMT API wrapper
 Home-page: https://github.com/modernmt/modernmt-python
 Author: ModernMT
 Author-email: info@modernmt.com
 Project-URL: Bug Tracker, https://github.com/modernmt/modernmt-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `modernmt-1.2.0/setup.cfg` & `modernmt-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = modernmt
-version = 1.2.0
+version = 1.2.1
 author = ModernMT
 author_email = info@modernmt.com
 description = ModernMT API wrapper
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/modernmt/modernmt-python
 project_urls =
```

### Comparing `modernmt-1.2.0/src/modernmt/modernmt.py` & `modernmt-1.2.1/src/modernmt/modernmt.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,17 @@
         self.message = message
 
         if metadata is not None:
             self.metadata = metadata
 
 
 class ModernMT(object):
-    def __init__(self, api_key, platform="modernmt-python", platform_version="1.2.0", api_client=None) -> None:
+    def __init__(self, api_key, platform="modernmt-python", platform_version="1.2.1", api_client=None) -> None:
         self.__batch_public_key = None
-        self.__batch_public_key_timestamp = 0
+        self.__batch_public_key_timestamp_sec = 0
 
         self.__base_url = "https://api.modernmt.com"
         self.__headers = {
             "MMT-ApiKey": api_key,
             "MMT-Platform": platform,
             "MMT-PlatformVersion": platform_version
         }
@@ -117,49 +117,57 @@
             if "alt_translations" in options:
                 data["alt_translations"] = options["alt_translations"]
             if "metadata" in options:
                 data["metadata"] = options["metadata"]
 
         headers = None
         if options is not None and "idempotency_key" in options:
-            headers = { "x-idempotency-key": options["idempotency_key"] }
+            headers = {"x-idempotency-key": options["idempotency_key"]}
 
         res = self.__send("post", "/translate/batch", data=data, headers=headers)
 
         return res["enqueued"]
 
-    def handle_callback(self, data, signature):
+    def handle_callback(self, body, signature):
         if self.__batch_public_key is None:
             self.__refresh_public_key()
 
-        if time.time() - self.__batch_public_key_timestamp > 3600:
+        if time.time() - self.__batch_public_key_timestamp_sec > 3600:
             # noinspection PyBroadException
             try:
                 self.__refresh_public_key()
             except:
                 pass
 
         jwt.decode(signature, self.__batch_public_key, algorithms=["RS256"])
 
-        if isinstance(data, str):
-            data = json.loads(data)
+        if isinstance(body, str):
+            body = json.loads(body)
 
-        result = data["result"]
-        metadata = data.get("metadata", None)
+        result = body["result"]
+        metadata = body.get("metadata", None)
         error = result.get("error", None)
 
         if error is not None:
             raise ModernMTException(result["status"], error["type"], error["message"], metadata)
 
-        return BatchTranslation(data)
+        _data = result["data"]
+        if not isinstance(_data, list):
+            data = Translation(_data)
+        else:
+            data = []
+            for el in _data:
+                data.append(Translation(el))
+
+        return data, metadata
 
     def __refresh_public_key(self):
         data = self.__send("get", "/translate/batch/key")
         self.__batch_public_key = base64.b64decode(data["publicKey"])
-        self.__batch_public_key_timestamp = time.time()
+        self.__batch_public_key_timestamp_sec = time.time()
 
     def get_context_vector(self, source, targets, text, hints=None, limit=None):
         data = {"source": source, "text": text, "targets": targets}
 
         if hints is not None:
             if isinstance(hints, list):
                 hints = ",".join(map(str, hints))
@@ -315,31 +323,14 @@
             "characters",
             "billedCharacters",
             "detectedLanguage",
             "altTranslations"
         ])
 
 
-class BatchTranslation(_Model):
-    def __init__(self, data) -> None:
-        super().__init__({}, [])
-
-        _data = data["result"]["data"]
-
-        if not isinstance(_data, list):
-            self.__dict__["data"] = Translation(_data)
-        else:
-            self.__dict__["data"] = []
-            for el in _data:
-                self.__dict__["data"].append(Translation(el))
-
-        if "metadata" in data:
-            self.__dict__["metadata"] = data["metadata"]
-
-
 class Memory(_Model):
     def __init__(self, data) -> None:
         super().__init__(data, ["id", "name", "description", "creationDate"])
 
 
 class ImportJob(_Model):
     def __init__(self, data) -> None:
```

### Comparing `modernmt-1.2.0/src/modernmt.egg-info/PKG-INFO` & `modernmt-1.2.1/src/modernmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modernmt
-Version: 1.2.0
+Version: 1.2.1
 Summary: ModernMT API wrapper
 Home-page: https://github.com/modernmt/modernmt-python
 Author: ModernMT
 Author-email: info@modernmt.com
 Project-URL: Bug Tracker, https://github.com/modernmt/modernmt-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

