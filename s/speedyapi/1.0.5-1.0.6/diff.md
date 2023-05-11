# Comparing `tmp/speedyapi-1.0.5.tar.gz` & `tmp/speedyapi-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedyapi-1.0.5.tar", last modified: Thu May 11 15:52:28 2023, max compression
+gzip compressed data, was "speedyapi-1.0.6.tar", last modified: Thu May 11 21:00:06 2023, max compression
```

## Comparing `speedyapi-1.0.5.tar` & `speedyapi-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:52:28.956896 speedyapi-1.0.5/
--rw-rw-rw-   0        0        0     4832 2023-05-11 15:52:28.955398 speedyapi-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4084 2023-03-14 17:49:52.000000 speedyapi-1.0.5/README.md
--rw-rw-rw-   0        0        0     1029 2023-05-11 15:14:10.000000 speedyapi-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 15:52:28.957395 speedyapi-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 15:52:28.917449 speedyapi-1.0.5/speedyapi/
--rw-rw-rw-   0        0        0     1318 2023-03-14 16:16:19.000000 speedyapi-1.0.5/speedyapi/__init__.py
--rw-rw-rw-   0        0        0    17926 2023-03-13 16:24:03.000000 speedyapi-1.0.5/speedyapi/color.py
--rw-rw-rw-   0        0        0       95 2023-03-09 11:09:35.000000 speedyapi-1.0.5/speedyapi/exceptions.py
--rw-rw-rw-   0        0        0     1912 2023-03-13 16:26:43.000000 speedyapi-1.0.5/speedyapi/handler.py
--rw-rw-rw-   0        0        0     2533 2023-03-13 16:40:21.000000 speedyapi-1.0.5/speedyapi/limiter.py
--rw-rw-rw-   0        0        0     1353 2023-03-13 16:43:52.000000 speedyapi-1.0.5/speedyapi/logging.py
--rw-rw-rw-   0        0        0    46067 2023-05-11 15:47:56.000000 speedyapi-1.0.5/speedyapi/main.py
--rw-rw-rw-   0        0        0     9762 2023-05-11 15:12:58.000000 speedyapi-1.0.5/speedyapi/parameters.py
--rw-rw-rw-   0        0        0     7881 2023-05-11 15:12:58.000000 speedyapi-1.0.5/speedyapi/respond.py
--rw-rw-rw-   0        0        0     5882 2023-05-11 15:12:58.000000 speedyapi-1.0.5/speedyapi/swagger.py
--rw-rw-rw-   0        0        0   115148 2023-03-12 17:02:26.000000 speedyapi-1.0.5/speedyapi/swagger_objects.py
--rw-rw-rw-   0        0        0     7072 2023-05-11 15:12:58.000000 speedyapi-1.0.5/speedyapi/tests.py
--rw-rw-rw-   0        0        0      284 2023-03-14 11:04:16.000000 speedyapi-1.0.5/speedyapi/types.py
--rw-rw-rw-   0        0        0    12793 2023-05-11 15:12:58.000000 speedyapi-1.0.5/speedyapi/util.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:52:28.953401 speedyapi-1.0.5/speedyapi.egg-info/
--rw-rw-rw-   0        0        0     4832 2023-05-11 15:52:28.000000 speedyapi-1.0.5/speedyapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2023-05-11 15:52:28.000000 speedyapi-1.0.5/speedyapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:52:28.000000 speedyapi-1.0.5/speedyapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-11 15:52:28.000000 speedyapi-1.0.5/speedyapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 15:52:28.000000 speedyapi-1.0.5/speedyapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 21:00:06.120364 speedyapi-1.0.6/
+-rw-rw-rw-   0        0        0     4832 2023-05-11 21:00:06.119365 speedyapi-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4084 2023-03-14 17:49:52.000000 speedyapi-1.0.6/README.md
+-rw-rw-rw-   0        0        0     1029 2023-05-11 20:59:36.000000 speedyapi-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 21:00:06.120863 speedyapi-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 21:00:06.082415 speedyapi-1.0.6/speedyapi/
+-rw-rw-rw-   0        0        0     1318 2023-03-14 16:16:19.000000 speedyapi-1.0.6/speedyapi/__init__.py
+-rw-rw-rw-   0        0        0    17926 2023-03-13 16:24:03.000000 speedyapi-1.0.6/speedyapi/color.py
+-rw-rw-rw-   0        0        0       95 2023-03-09 11:09:35.000000 speedyapi-1.0.6/speedyapi/exceptions.py
+-rw-rw-rw-   0        0        0     1912 2023-03-13 16:26:43.000000 speedyapi-1.0.6/speedyapi/handler.py
+-rw-rw-rw-   0        0        0     2533 2023-03-13 16:40:21.000000 speedyapi-1.0.6/speedyapi/limiter.py
+-rw-rw-rw-   0        0        0     1353 2023-03-13 16:43:52.000000 speedyapi-1.0.6/speedyapi/logging.py
+-rw-rw-rw-   0        0        0    46108 2023-05-11 20:59:18.000000 speedyapi-1.0.6/speedyapi/main.py
+-rw-rw-rw-   0        0        0     9762 2023-05-11 15:12:58.000000 speedyapi-1.0.6/speedyapi/parameters.py
+-rw-rw-rw-   0        0        0     7881 2023-05-11 15:12:58.000000 speedyapi-1.0.6/speedyapi/respond.py
+-rw-rw-rw-   0        0        0     5834 2023-05-11 15:58:04.000000 speedyapi-1.0.6/speedyapi/swagger.py
+-rw-rw-rw-   0        0        0   115148 2023-03-12 17:02:26.000000 speedyapi-1.0.6/speedyapi/swagger_objects.py
+-rw-rw-rw-   0        0        0     7072 2023-05-11 15:12:58.000000 speedyapi-1.0.6/speedyapi/tests.py
+-rw-rw-rw-   0        0        0      284 2023-03-14 11:04:16.000000 speedyapi-1.0.6/speedyapi/types.py
+-rw-rw-rw-   0        0        0    12793 2023-05-11 15:12:58.000000 speedyapi-1.0.6/speedyapi/util.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:00:06.116869 speedyapi-1.0.6/speedyapi.egg-info/
+-rw-rw-rw-   0        0        0     4832 2023-05-11 21:00:05.000000 speedyapi-1.0.6/speedyapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2023-05-11 21:00:05.000000 speedyapi-1.0.6/speedyapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 21:00:05.000000 speedyapi-1.0.6/speedyapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-11 21:00:05.000000 speedyapi-1.0.6/speedyapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 21:00:05.000000 speedyapi-1.0.6/speedyapi.egg-info/top_level.txt
```

### Comparing `speedyapi-1.0.5/PKG-INFO` & `speedyapi-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedyapi
-Version: 1.0.5
+Version: 1.0.6
 Summary: An easy to use Python module for creating API.
 Author: CodingYuno
 Project-URL: Source Code, https://github.com/CodingYuno/speedyapi/
 Project-URL: Issue Tracker, https://github.com/CodingYuno/speedyapi/issues/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `speedyapi-1.0.5/README.md` & `speedyapi-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.5/pyproject.toml` & `speedyapi-1.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "speedyapi"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="CodingYuno"},
 ]
 description = "An easy to use Python module for creating API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `speedyapi-1.0.5/speedyapi/__init__.py` & `speedyapi-1.0.6/speedyapi/__init__.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.5/speedyapi/color.py` & `speedyapi-1.0.6/speedyapi/color.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.5/speedyapi/handler.py` & `speedyapi-1.0.6/speedyapi/handler.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.5/speedyapi/limiter.py` & `speedyapi-1.0.6/speedyapi/limiter.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.5/speedyapi/logging.py` & `speedyapi-1.0.6/speedyapi/logging.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.5/speedyapi/main.py` & `speedyapi-1.0.6/speedyapi/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         )
         self.override_swagger = {}  # If an override swagger.json is used when the API is run it is stored here
 
         # Async and Sync default authentication functions for the API (These can be made to support all authentication methods in the standard OpenAPI specification)
         self.auth_function, self.auth_function_require_key = None, False
         self.async_auth_function, self.async_auth_function_require_key = None, False
 
-        self.request_logging = False  # This is kept off until after tests have been run over localhost for cleanliness
+        self.request_logging = True  # This is kept off until after tests have been run over localhost for cleanliness
         self.endpoint_tests = {}
         self.test_count = 0
 
         # Storage of the current state of all rate limits across the whole API
         # This is thread safe due to Flask and Async Flask using threading for request handling
         self.rate_limits = ThreadSafeDict(
             paths={},
@@ -708,14 +708,15 @@
                 # If an example is to be added it is set here (May be deprecated in future versions of the OpenAPI specification)
                 if test.example:
                     content["application/json"].schema["example"] = test_response
 
         color_print("-" * 90, color="white")
 
         if tests:
+            self.request_logging = False
             app_thread = Thread(target=run_app, daemon=False)
             app_thread.start()  # API started here
             t0 = time.time()
             success_count, failed_count = 0, 0
 
             test_threads = set()
             for path, methods in self.endpoint_tests.items():
```

### Comparing `speedyapi-1.0.5/speedyapi/parameters.py` & `speedyapi-1.0.6/speedyapi/parameters.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.5/speedyapi/respond.py` & `speedyapi-1.0.6/speedyapi/respond.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.5/speedyapi/swagger.py` & `speedyapi-1.0.6/speedyapi/swagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,12 +152,11 @@
     schema["type"] = type
 
     if type == "object":
         schema["properties"] = {}
         for key, sub_obj in obj.items():
             schema["properties"][key] = recursive_generation_of_json_response_schema(sub_obj)  # Recursion
     elif type == "array":
-        # TODO - needs to work for empty lists
         if len(obj):
             schema["items"] = recursive_generation_of_json_response_schema(obj[0])  # Recursion (Limits to the first object)
 
     return schema
```

### Comparing `speedyapi-1.0.5/speedyapi/swagger_objects.py` & `speedyapi-1.0.6/speedyapi/swagger_objects.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.5/speedyapi/tests.py` & `speedyapi-1.0.6/speedyapi/tests.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.5/speedyapi/util.py` & `speedyapi-1.0.6/speedyapi/util.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.5/speedyapi.egg-info/PKG-INFO` & `speedyapi-1.0.6/speedyapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedyapi
-Version: 1.0.5
+Version: 1.0.6
 Summary: An easy to use Python module for creating API.
 Author: CodingYuno
 Project-URL: Source Code, https://github.com/CodingYuno/speedyapi/
 Project-URL: Issue Tracker, https://github.com/CodingYuno/speedyapi/issues/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

