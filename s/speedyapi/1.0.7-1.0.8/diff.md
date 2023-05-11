# Comparing `tmp/speedyapi-1.0.7.tar.gz` & `tmp/speedyapi-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedyapi-1.0.7.tar", last modified: Thu May 11 21:14:15 2023, max compression
+gzip compressed data, was "speedyapi-1.0.8.tar", last modified: Thu May 11 21:17:38 2023, max compression
```

## Comparing `speedyapi-1.0.7.tar` & `speedyapi-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 21:14:15.394033 speedyapi-1.0.7/
--rw-rw-rw-   0        0        0     4832 2023-05-11 21:14:15.392537 speedyapi-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4084 2023-03-14 17:49:52.000000 speedyapi-1.0.7/README.md
--rw-rw-rw-   0        0        0     1029 2023-05-11 21:13:53.000000 speedyapi-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 21:14:15.394533 speedyapi-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 21:14:15.359079 speedyapi-1.0.7/speedyapi/
--rw-rw-rw-   0        0        0     1318 2023-03-14 16:16:19.000000 speedyapi-1.0.7/speedyapi/__init__.py
--rw-rw-rw-   0        0        0    17926 2023-03-13 16:24:03.000000 speedyapi-1.0.7/speedyapi/color.py
--rw-rw-rw-   0        0        0       95 2023-03-09 11:09:35.000000 speedyapi-1.0.7/speedyapi/exceptions.py
--rw-rw-rw-   0        0        0     1912 2023-03-13 16:26:43.000000 speedyapi-1.0.7/speedyapi/handler.py
--rw-rw-rw-   0        0        0     2533 2023-03-13 16:40:21.000000 speedyapi-1.0.7/speedyapi/limiter.py
--rw-rw-rw-   0        0        0     1353 2023-03-13 16:43:52.000000 speedyapi-1.0.7/speedyapi/logging.py
--rw-rw-rw-   0        0        0    46106 2023-05-11 21:13:53.000000 speedyapi-1.0.7/speedyapi/main.py
--rw-rw-rw-   0        0        0     9762 2023-05-11 15:12:58.000000 speedyapi-1.0.7/speedyapi/parameters.py
--rw-rw-rw-   0        0        0     7881 2023-05-11 15:12:58.000000 speedyapi-1.0.7/speedyapi/respond.py
--rw-rw-rw-   0        0        0     5834 2023-05-11 15:58:04.000000 speedyapi-1.0.7/speedyapi/swagger.py
--rw-rw-rw-   0        0        0   115148 2023-03-12 17:02:26.000000 speedyapi-1.0.7/speedyapi/swagger_objects.py
--rw-rw-rw-   0        0        0     7072 2023-05-11 15:12:58.000000 speedyapi-1.0.7/speedyapi/tests.py
--rw-rw-rw-   0        0        0      284 2023-03-14 11:04:16.000000 speedyapi-1.0.7/speedyapi/types.py
--rw-rw-rw-   0        0        0    12793 2023-05-11 15:12:58.000000 speedyapi-1.0.7/speedyapi/util.py
-drwxrwxrwx   0        0        0        0 2023-05-11 21:14:15.390539 speedyapi-1.0.7/speedyapi.egg-info/
--rw-rw-rw-   0        0        0     4832 2023-05-11 21:14:15.000000 speedyapi-1.0.7/speedyapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2023-05-11 21:14:15.000000 speedyapi-1.0.7/speedyapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 21:14:15.000000 speedyapi-1.0.7/speedyapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-11 21:14:15.000000 speedyapi-1.0.7/speedyapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 21:14:15.000000 speedyapi-1.0.7/speedyapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 21:17:38.495496 speedyapi-1.0.8/
+-rw-rw-rw-   0        0        0     4832 2023-05-11 21:17:38.494497 speedyapi-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4084 2023-03-14 17:49:52.000000 speedyapi-1.0.8/README.md
+-rw-rw-rw-   0        0        0     1029 2023-05-11 21:17:19.000000 speedyapi-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 21:17:38.495496 speedyapi-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 21:17:38.466534 speedyapi-1.0.8/speedyapi/
+-rw-rw-rw-   0        0        0     1318 2023-03-14 16:16:19.000000 speedyapi-1.0.8/speedyapi/__init__.py
+-rw-rw-rw-   0        0        0    17926 2023-03-13 16:24:03.000000 speedyapi-1.0.8/speedyapi/color.py
+-rw-rw-rw-   0        0        0       95 2023-03-09 11:09:35.000000 speedyapi-1.0.8/speedyapi/exceptions.py
+-rw-rw-rw-   0        0        0     1912 2023-03-13 16:26:43.000000 speedyapi-1.0.8/speedyapi/handler.py
+-rw-rw-rw-   0        0        0     2533 2023-03-13 16:40:21.000000 speedyapi-1.0.8/speedyapi/limiter.py
+-rw-rw-rw-   0        0        0     1353 2023-03-13 16:43:52.000000 speedyapi-1.0.8/speedyapi/logging.py
+-rw-rw-rw-   0        0        0    46112 2023-05-11 21:17:19.000000 speedyapi-1.0.8/speedyapi/main.py
+-rw-rw-rw-   0        0        0     9762 2023-05-11 15:12:58.000000 speedyapi-1.0.8/speedyapi/parameters.py
+-rw-rw-rw-   0        0        0     7881 2023-05-11 15:12:58.000000 speedyapi-1.0.8/speedyapi/respond.py
+-rw-rw-rw-   0        0        0     5834 2023-05-11 15:58:04.000000 speedyapi-1.0.8/speedyapi/swagger.py
+-rw-rw-rw-   0        0        0   115148 2023-03-12 17:02:26.000000 speedyapi-1.0.8/speedyapi/swagger_objects.py
+-rw-rw-rw-   0        0        0     7072 2023-05-11 15:12:58.000000 speedyapi-1.0.8/speedyapi/tests.py
+-rw-rw-rw-   0        0        0      284 2023-03-14 11:04:16.000000 speedyapi-1.0.8/speedyapi/types.py
+-rw-rw-rw-   0        0        0    12793 2023-05-11 15:12:58.000000 speedyapi-1.0.8/speedyapi/util.py
+drwxrwxrwx   0        0        0        0 2023-05-11 21:17:38.492500 speedyapi-1.0.8/speedyapi.egg-info/
+-rw-rw-rw-   0        0        0     4832 2023-05-11 21:17:38.000000 speedyapi-1.0.8/speedyapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2023-05-11 21:17:38.000000 speedyapi-1.0.8/speedyapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 21:17:38.000000 speedyapi-1.0.8/speedyapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-11 21:17:38.000000 speedyapi-1.0.8/speedyapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 21:17:38.000000 speedyapi-1.0.8/speedyapi.egg-info/top_level.txt
```

### Comparing `speedyapi-1.0.7/PKG-INFO` & `speedyapi-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedyapi
-Version: 1.0.7
+Version: 1.0.8
 Summary: An easy to use Python module for creating API.
 Author: CodingYuno
 Project-URL: Source Code, https://github.com/CodingYuno/speedyapi/
 Project-URL: Issue Tracker, https://github.com/CodingYuno/speedyapi/issues/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `speedyapi-1.0.7/README.md` & `speedyapi-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.7/pyproject.toml` & `speedyapi-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "speedyapi"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="CodingYuno"},
 ]
 description = "An easy to use Python module for creating API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `speedyapi-1.0.7/speedyapi/__init__.py` & `speedyapi-1.0.8/speedyapi/__init__.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.7/speedyapi/color.py` & `speedyapi-1.0.8/speedyapi/color.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.7/speedyapi/handler.py` & `speedyapi-1.0.8/speedyapi/handler.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.7/speedyapi/limiter.py` & `speedyapi-1.0.8/speedyapi/limiter.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.7/speedyapi/logging.py` & `speedyapi-1.0.8/speedyapi/logging.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.7/speedyapi/main.py` & `speedyapi-1.0.8/speedyapi/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         async def swagger():
             swagger_json = self.override_swagger if self.override_swagger else self.swagger.json()
             return json(swagger_json)
 
         # The base path is used for Redoc documentation based on an automatically generated or manually set swagger.json file
         @self.endpoint(path=f"/", method="GET", docs_ignore=True)
         async def docs():
-            return html(redoc_html(info.title, server=servers[0].url))
+            return html(redoc_html(info.title, server=servers[0].url + "/"))
 
     def endpoint(self, path: str, method: str = "GET", authentication: str | list = None, name: str = None, description: str = None, docs_ignore: bool = False, group: str = None):
         """
         Creation of endpoints for the API
 
         :param path: The path of the endpoint
         :param method: The method of the endpoint e.g. GET, POST, PUT .. (Unlike standard Flask please write separate endpoints for each method type if required)
```

### Comparing `speedyapi-1.0.7/speedyapi/parameters.py` & `speedyapi-1.0.8/speedyapi/parameters.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.7/speedyapi/respond.py` & `speedyapi-1.0.8/speedyapi/respond.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.7/speedyapi/swagger.py` & `speedyapi-1.0.8/speedyapi/swagger.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.7/speedyapi/swagger_objects.py` & `speedyapi-1.0.8/speedyapi/swagger_objects.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.7/speedyapi/tests.py` & `speedyapi-1.0.8/speedyapi/tests.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.7/speedyapi/util.py` & `speedyapi-1.0.8/speedyapi/util.py`

 * *Files identical despite different names*

### Comparing `speedyapi-1.0.7/speedyapi.egg-info/PKG-INFO` & `speedyapi-1.0.8/speedyapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedyapi
-Version: 1.0.7
+Version: 1.0.8
 Summary: An easy to use Python module for creating API.
 Author: CodingYuno
 Project-URL: Source Code, https://github.com/CodingYuno/speedyapi/
 Project-URL: Issue Tracker, https://github.com/CodingYuno/speedyapi/issues/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

