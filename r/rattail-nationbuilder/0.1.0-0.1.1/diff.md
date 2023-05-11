# Comparing `tmp/rattail-nationbuilder-0.1.0.tar.gz` & `tmp/rattail-nationbuilder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/lance/src/rattail-nationbuilder/dist/.tmp-77mlz1z2/rattail-nationbuilder-0.1.0.tar", last modified: Mon May  8 20:35:50 2023, max compression
+gzip compressed data, was "/home/lance/src/rattail-nationbuilder/dist/.tmp-7o5gr9q5/rattail-nationbuilder-0.1.1.tar", last modified: Thu May 11 20:25:42 2023, max compression
```

## Comparing `rattail-nationbuilder-0.1.0.tar` & `rattail-nationbuilder-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-08 20:35:50.000000 rattail-nationbuilder-0.1.0/
--rw-r--r--   0 lance     (1000) lance     (1000)      335 2023-05-08 20:34:54.000000 rattail-nationbuilder-0.1.0/CHANGELOG.md
--rw-r--r--   0 lance     (1000) lance     (1000)       27 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.0/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)      982 2023-05-08 20:35:50.000000 rattail-nationbuilder-0.1.0/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      290 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.0/README.md
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-08 20:35:50.000000 rattail-nationbuilder-0.1.0/rattail_nationbuilder/
--rw-r--r--   0 lance     (1000) lance     (1000)     1013 2023-05-05 19:43:26.000000 rattail-nationbuilder-0.1.0/rattail_nationbuilder/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.0/rattail_nationbuilder/_version.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-08 20:35:50.000000 rattail-nationbuilder-0.1.0/rattail_nationbuilder/nationbuilder/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2023-05-05 19:45:56.000000 rattail-nationbuilder-0.1.0/rattail_nationbuilder/nationbuilder/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3886 2023-05-08 19:54:10.000000 rattail-nationbuilder-0.1.0/rattail_nationbuilder/nationbuilder/webapi.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-08 20:35:50.000000 rattail-nationbuilder-0.1.0/rattail_nationbuilder.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)      982 2023-05-08 20:35:50.000000 rattail-nationbuilder-0.1.0/rattail_nationbuilder.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      429 2023-05-08 20:35:50.000000 rattail-nationbuilder-0.1.0/rattail_nationbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-05-08 20:35:50.000000 rattail-nationbuilder-0.1.0/rattail_nationbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        8 2023-05-08 20:35:50.000000 rattail-nationbuilder-0.1.0/rattail_nationbuilder.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       22 2023-05-08 20:35:50.000000 rattail-nationbuilder-0.1.0/rattail_nationbuilder.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2023-05-08 20:35:50.000000 rattail-nationbuilder-0.1.0/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     2268 2023-05-05 19:43:42.000000 rattail-nationbuilder-0.1.0/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/
+-rw-r--r--   0 lance     (1000) lance     (1000)      484 2023-05-11 20:25:13.000000 rattail-nationbuilder-0.1.1/CHANGELOG.md
+-rw-r--r--   0 lance     (1000) lance     (1000)       27 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.1/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)      982 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      290 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.1/README.md
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1013 2023-05-05 19:43:26.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-05-11 20:25:19.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder/_version.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder/nationbuilder/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2023-05-05 19:45:56.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder/nationbuilder/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4578 2023-05-09 23:33:43.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder/nationbuilder/webapi.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)      982 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      429 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        8 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       22 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       38 2023-05-11 20:25:42.000000 rattail-nationbuilder-0.1.1/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     2268 2023-05-05 19:43:42.000000 rattail-nationbuilder-0.1.1/setup.py
```

### Comparing `rattail-nationbuilder-0.1.0/PKG-INFO` & `rattail-nationbuilder-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-nationbuilder
-Version: 0.1.0
+Version: 0.1.1
 Summary: Rattail integration package for NationBuilder
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rattail-nationbuilder-0.1.0/rattail_nationbuilder/__init__.py` & `rattail-nationbuilder-0.1.1/rattail_nationbuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-nationbuilder-0.1.0/rattail_nationbuilder/nationbuilder/webapi.py` & `rattail-nationbuilder-0.1.1/rattail_nationbuilder/nationbuilder/webapi.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,27 +26,43 @@
 
 import requests
 
 
 class NationBuilderWebAPI(object):
     """
     Simple web API for NationBuilder.
+
+    https://nationbuilder.com/api_documentation
     """
 
-    def __init__(self, config, base_url=None, access_token=None, **kwargs):
+    def __init__(self, config, base_url=None, access_token=None,
+                 max_retries=None, **kwargs):
         self.config = config
         self.app = self.config.get_app()
+        self.session = None
 
         self.base_url = base_url or self.config.require(
             'nationbuilder', 'api.base_url')
         self.base_url = self.base_url.rstrip('/')
 
         self.access_token = access_token or self.config.require(
             'nationbuilder', 'api.access_token')
 
+        if max_retries is not None:
+            self.max_retries = max_retries
+        else:
+            self.max_retries = self.config.getint('nationbuilder',
+                                                  'api.max_retries')
+
+        self.session = requests.Session()
+
+        if self.max_retries is not None:
+            adapter = requests.adapters.HTTPAdapter(max_retries=self.max_retries)
+            self.session.mount(self.base_url, adapter)
+
     def _request(self, request_method, api_method, params=None):
         """
         Perform a request for the given API method, and return the response.
         """
         api_method = api_method.lstrip('/')
 
         params = params or {}
@@ -90,29 +106,33 @@
             people.extend(data['results'])
             url['next'] = data['next']
 
         self.app.progress_loop(fetch, range(pages), progress,
                                message="Fetching Person data from NationBuilder")
         return people
 
-    def get_people_with_tag(self, tag, page_size=100, **kwargs):
+    def get_people_with_tag(self, tag, page_size=100, max_pages=None, **kwargs):
         """
         Retrieve all Person records with the given tag.
 
         https://apiexplorer.nationbuilder.com/nationbuilder#People
         """
         people = []
 
         # get first page
         api_method = '/api/v1/tags/{}/people'.format(tag)
         api_method = '{}?limit={}'.format(api_method, page_size)
         response = self.get(api_method)
         data = response.json()
         people.extend(data['results'])
+        pages = 1
 
         # get more pages, until complete
         while data['next']:
+            if max_pages and pages >= max_pages:
+                break
             response = self.get(data['next'])
             data = response.json()
             people.extend(data['results'])
+            pages += 1
 
         return people
```

### Comparing `rattail-nationbuilder-0.1.0/rattail_nationbuilder.egg-info/PKG-INFO` & `rattail-nationbuilder-0.1.1/rattail_nationbuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-nationbuilder
-Version: 0.1.0
+Version: 0.1.1
 Summary: Rattail integration package for NationBuilder
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rattail-nationbuilder-0.1.0/setup.py` & `rattail-nationbuilder-0.1.1/setup.py`

 * *Files identical despite different names*

