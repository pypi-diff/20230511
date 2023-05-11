# Comparing `tmp/robotframework-processcube-2.2.0a1.tar.gz` & `tmp/robotframework-processcube-2.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-processcube-2.2.0a1.tar", last modified: Thu Sep 15 20:44:09 2022, max compression
+gzip compressed data, was "robotframework-processcube-2.4.0a1.tar", last modified: Thu May 11 19:23:25 2023, max compression
```

## Comparing `robotframework-processcube-2.2.0a1.tar` & `robotframework-processcube-2.4.0a1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-15 20:44:09.441604 robotframework-processcube-2.2.0a1/
--rw-r--r--   0 runner    (1001) docker     (116)    15969 2022-09-15 20:44:09.441604 robotframework-processcube-2.2.0a1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-15 20:44:09.437604 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/
--rw-r--r--   0 runner    (1001) docker     (116)     3393 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/ProcessCubeLibrary.py
--rw-r--r--   0 runner    (1001) docker     (116)       50 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2347 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/docker_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-15 20:44:09.437604 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/
--rw-r--r--   0 runner    (1001) docker     (116)      425 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      384 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/_fields_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     2100 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/_retry_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)      737 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/deploy_keyword.py
--rw-r--r--   0 runner    (1001) docker     (116)     1813 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/empty_task_keyword.py
--rw-r--r--   0 runner    (1001) docker     (116)      264 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/engine_keyword.py
--rw-r--r--   0 runner    (1001) docker     (116)     2034 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/external_task_keyword.py
--rw-r--r--   0 runner    (1001) docker     (116)     1720 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/manual_task_keyword.py
--rw-r--r--   0 runner    (1001) docker     (116)     2842 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/process_instance_keyword.py
--rw-r--r--   0 runner    (1001) docker     (116)     1069 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/send_keyword.py
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/start_keyword.py
--rw-r--r--   0 runner    (1001) docker     (116)     1888 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/user_task_keyword.py
--rw-r--r--   0 runner    (1001) docker     (116)    15231 2022-09-15 20:42:37.000000 robotframework-processcube-2.2.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-15 20:44:09.437604 robotframework-processcube-2.2.0a1/robotframework_processcube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    15969 2022-09-15 20:44:09.000000 robotframework-processcube-2.2.0a1/robotframework_processcube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      947 2022-09-15 20:44:09.000000 robotframework-processcube-2.2.0a1/robotframework_processcube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-15 20:44:09.000000 robotframework-processcube-2.2.0a1/robotframework_processcube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       92 2022-09-15 20:44:09.000000 robotframework-processcube-2.2.0a1/robotframework_processcube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2022-09-15 20:44:09.000000 robotframework-processcube-2.2.0a1/robotframework_processcube.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-09-15 20:44:09.441604 robotframework-processcube-2.2.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1336 2022-09-15 20:44:08.000000 robotframework-processcube-2.2.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:23:25.494953 robotframework-processcube-2.4.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    15969 2023-05-11 19:23:25.494953 robotframework-processcube-2.4.0a1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:23:25.490953 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/ProcessCubeLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/docker_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:23:25.494953 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/_fields_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/_retry_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/deploy_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/empty_task_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/engine_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/external_task_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/manual_task_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/process_instance_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/send_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/start_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/user_task_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-05-11 19:23:06.000000 robotframework-processcube-2.4.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:23:25.494953 robotframework-processcube-2.4.0a1/robotframework_processcube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15969 2023-05-11 19:23:25.000000 robotframework-processcube-2.4.0a1/robotframework_processcube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-11 19:23:25.000000 robotframework-processcube-2.4.0a1/robotframework_processcube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:23:25.000000 robotframework-processcube-2.4.0a1/robotframework_processcube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-11 19:23:25.000000 robotframework-processcube-2.4.0a1/robotframework_processcube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 19:23:25.000000 robotframework-processcube-2.4.0a1/robotframework_processcube.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:23:25.494953 robotframework-processcube-2.4.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-11 19:23:24.000000 robotframework-processcube-2.4.0a1/setup.py
```

### Comparing `robotframework-processcube-2.2.0a1/PKG-INFO` & `robotframework-processcube-2.4.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-processcube
-Version: 2.2.0a1
+Version: 2.4.0a1
 Summary: Robot Framework Keywords for processcube workflow engine.
 Home-page: https://github.com/atlas-engine-contrib/robotframework-processcube
 Author: 5Minds IT-Solutions GmbH & Co. KG
 Author-email: processcube@5minds.de
 License: MIT Licence
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `robotframework-processcube-2.2.0a1/ProcessCubeLibrary/ProcessCubeLibrary.py` & `robotframework-processcube-2.4.0a1/ProcessCubeLibrary/ProcessCubeLibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.2.0a1/ProcessCubeLibrary/docker_handler.py` & `robotframework-processcube-2.4.0a1/ProcessCubeLibrary/docker_handler.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/_retry_helper.py` & `robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/_retry_helper.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/deploy_keyword.py` & `robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/deploy_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/empty_task_keyword.py` & `robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/empty_task_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/external_task_keyword.py` & `robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/external_task_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/manual_task_keyword.py` & `robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/manual_task_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/process_instance_keyword.py` & `robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/process_instance_keyword.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,14 +17,42 @@
     def __init__(self, client, **kwargs):
         self._client = client
 
         self._max_retries = kwargs.get('max_retries', 5)
         self._backoff_factor = kwargs.get('backoff_factor', 2)
         self._delay = kwargs.get('delay', 0.1)
 
+    def get_active_processinstances_by_correlation(self, correlation) -> FlowNodeInstanceResponse:
+        query_dict = {
+            'state': 'running',
+            'correlation_id': correlation
+        }
+
+        logger.info(f"query_dict: {query_dict}")
+
+        result = self.get_processinstances_by_query(**query_dict)
+
+        return result
+
+    def get_active_processinstances_by_processmodel(self, process_model) -> FlowNodeInstanceResponse:
+        query_dict = {
+            'state': 'running',
+            'process_model_id': process_model
+        }
+
+        result = self.get_processinstances_by_query(**query_dict)
+
+        return result
+
+    @retry_on_exception
+    def get_processinstances_by_query(self, **query_dict) -> FlowNodeInstanceResponse:
+        result = self._client.process_instanceq_query(FlowNodeInstancesQuery(**query_dict))
+
+        return result
+
     @retry_on_exception
     def get_processinstance(self, **kwargs) -> FlowNodeInstanceResponse:
         return self._get_processinstance(**kwargs)
 
     @retry_on_exception
     def get_processinstance_result(self, **kwargs) -> Dict[str, Any]:
         result = self._get_processinstance(**kwargs)
```

### Comparing `robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/send_keyword.py` & `robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/send_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.2.0a1/ProcessCubeLibrary/keywords/user_task_keyword.py` & `robotframework-processcube-2.4.0a1/ProcessCubeLibrary/keywords/user_task_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.2.0a1/README.md` & `robotframework-processcube-2.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.2.0a1/robotframework_processcube.egg-info/PKG-INFO` & `robotframework-processcube-2.4.0a1/robotframework_processcube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-processcube
-Version: 2.2.0a1
+Version: 2.4.0a1
 Summary: Robot Framework Keywords for processcube workflow engine.
 Home-page: https://github.com/atlas-engine-contrib/robotframework-processcube
 Author: 5Minds IT-Solutions GmbH & Co. KG
 Author-email: processcube@5minds.de
 License: MIT Licence
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `robotframework-processcube-2.2.0a1/robotframework_processcube.egg-info/SOURCES.txt` & `robotframework-processcube-2.4.0a1/robotframework_processcube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.2.0a1/setup.py` & `robotframework-processcube-2.4.0a1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 name = "5Minds IT-Solutions GmbH & Co. KG"
 
 setuptools.setup(
     name="robotframework-processcube",
-    version=setuptools.sic('2.2.0-alpha.1'),
+    version=setuptools.sic('2.4.0-alpha.1'),
     description="Robot Framework Keywords for processcube workflow engine.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=name,
     author_email="processcube@5minds.de",
     url="https://github.com/atlas-engine-contrib/robotframework-processcube",
     packages=setuptools.find_packages(),
```

