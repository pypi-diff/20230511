# Comparing `tmp/lendsmart_autotest-1.4.tar.gz` & `tmp/lendsmart_autotest-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lendsmart_autotest-1.4.tar", last modified: Wed May 10 13:22:44 2023, max compression
+gzip compressed data, was "lendsmart_autotest-1.5.tar", last modified: Thu May 11 12:29:19 2023, max compression
```

## Comparing `lendsmart_autotest-1.4.tar` & `lendsmart_autotest-1.5.tar`

### file list

```diff
@@ -1,41 +1,55 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:22:44.140244 lendsmart_autotest-1.4/
--rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-10 13:22:44.140244 lendsmart_autotest-1.4/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:22:44.136244 lendsmart_autotest-1.4/autotest/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 13:20:45.000000 lendsmart_autotest-1.4/autotest/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:22:44.136244 lendsmart_autotest-1.4/autotest/lib/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:22:44.136244 lendsmart_autotest-1.4/autotest/lib/base/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/base/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    13128 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/base/commons.py
--rw-rw-r--   0 user      (1000) user      (1000)     9148 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/base/setup.py
--rw-rw-r--   0 user      (1000) user      (1000)    13311 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/base/webActions.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:22:44.136244 lendsmart_autotest-1.4/autotest/lib/client_builder/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/client_builder/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:22:44.136244 lendsmart_autotest-1.4/autotest/lib/configurations/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/configurations/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6714 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/configurations/common_config.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:22:44.140244 lendsmart_autotest-1.4/autotest/lib/generator/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/generator/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2595 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/generator/generate_test_data.py
--rw-rw-r--   0 user      (1000) user      (1000)    10788 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/generator/graph.py
--rw-rw-r--   0 user      (1000) user      (1000)     9425 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/generator/initialize.py
--rw-rw-r--   0 user      (1000) user      (1000)    13581 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/generator/question_type.py
--rw-rw-r--   0 user      (1000) user      (1000)     4274 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/generator/test_data.py
--rw-rw-r--   0 user      (1000) user      (1000)     1072 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/generator/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:22:44.140244 lendsmart_autotest-1.4/autotest/lib/lib/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/lib/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      162 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/lib/lend_event.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:22:44.140244 lendsmart_autotest-1.4/autotest/lib/runner/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/runner/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1444 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/runner/initializer.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:22:44.140244 lendsmart_autotest-1.4/autotest/lib/utilities/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/utilities/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      440 2023-05-10 12:47:04.000000 lendsmart_autotest-1.4/autotest/lib/utilities/random_email.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:22:44.140244 lendsmart_autotest-1.4/lendsmart_autotest.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-10 13:22:44.000000 lendsmart_autotest-1.4/lendsmart_autotest.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      964 2023-05-10 13:22:44.000000 lendsmart_autotest-1.4/lendsmart_autotest.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-10 13:22:44.000000 lendsmart_autotest-1.4/lendsmart_autotest.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      200 2023-05-10 13:22:44.000000 lendsmart_autotest-1.4/lendsmart_autotest.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-05-10 13:22:44.000000 lendsmart_autotest-1.4/lendsmart_autotest.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-10 13:22:44.140244 lendsmart_autotest-1.4/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1193 2023-05-10 13:21:21.000000 lendsmart_autotest-1.4/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.834175 lendsmart_autotest-1.5/
+-rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-11 12:29:19.834175 lendsmart_autotest-1.5/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.830175 lendsmart_autotest-1.5/base/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/base/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13128 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/base/commons.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9148 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/base/setup.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13311 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/base/webActions.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.830175 lendsmart_autotest-1.5/client_builder/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/client_builder/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.830175 lendsmart_autotest-1.5/client_builder/aws/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/client_builder/aws/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      534 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/client_builder/aws/client.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1139 2023-05-11 12:22:52.000000 lendsmart_autotest-1.5/client_builder/aws/dynamodb.py
+-rw-rw-r--   0 user      (1000) user      (1000)      594 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/client_builder/aws/lambda_obj.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.830175 lendsmart_autotest-1.5/configurations/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/configurations/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6714 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/configurations/common_config.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.834175 lendsmart_autotest-1.5/generator/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/generator/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2595 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/generator/generate_test_data.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10788 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/generator/graph.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9877 2023-05-11 12:22:52.000000 lendsmart_autotest-1.5/generator/initialize.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.834175 lendsmart_autotest-1.5/generator/intent/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/generator/intent/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8755 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/generator/intent/intent.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13581 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/generator/question_type.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4274 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/generator/test_data.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1072 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/generator/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.834175 lendsmart_autotest-1.5/lendsmart_autotest.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-11 12:29:19.000000 lendsmart_autotest-1.5/lendsmart_autotest.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1051 2023-05-11 12:29:19.000000 lendsmart_autotest-1.5/lendsmart_autotest.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-11 12:29:19.000000 lendsmart_autotest-1.5/lendsmart_autotest.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      200 2023-05-11 12:29:19.000000 lendsmart_autotest-1.5/lendsmart_autotest.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       66 2023-05-11 12:29:19.000000 lendsmart_autotest-1.5/lendsmart_autotest.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.834175 lendsmart_autotest-1.5/lib/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/lib/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      162 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/lib/lend_event.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.834175 lendsmart_autotest-1.5/lib/node/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/lib/node/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6021 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/lib/node/action.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1626 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/lib/node/node.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.834175 lendsmart_autotest-1.5/runner/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/runner/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.834175 lendsmart_autotest-1.5/runner/application_overview/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/runner/application_overview/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      319 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/runner/application_overview/runner.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.834175 lendsmart_autotest-1.5/runner/application_workflow/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/runner/application_workflow/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2794 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/runner/application_workflow/runner.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1444 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/runner/initializer.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-11 12:29:19.834175 lendsmart_autotest-1.5/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1193 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:29:19.834175 lendsmart_autotest-1.5/utilities/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/utilities/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      440 2023-05-11 11:37:50.000000 lendsmart_autotest-1.5/utilities/random_email.py
```

### Comparing `lendsmart_autotest-1.4/autotest/lib/base/commons.py` & `lendsmart_autotest-1.5/base/commons.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.4/autotest/lib/base/setup.py` & `lendsmart_autotest-1.5/base/setup.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.4/autotest/lib/base/webActions.py` & `lendsmart_autotest-1.5/base/webActions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.4/autotest/lib/configurations/common_config.py` & `lendsmart_autotest-1.5/configurations/common_config.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.4/autotest/lib/generator/generate_test_data.py` & `lendsmart_autotest-1.5/generator/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.4/autotest/lib/generator/graph.py` & `lendsmart_autotest-1.5/generator/graph.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.4/autotest/lib/generator/initialize.py` & `lendsmart_autotest-1.5/generator/initialize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
     This module will generate the test flows from intent json
 """
-import json
 import random
 import asyncio
 from ramda import path_or
 from autotest.lib.lib.lend_event import LendEvent
 from autotest.lib.generator.intent.intent import Questions
 from autotest.lib.generator.graph import DirectedGraphBuilder
 from autotest.lib.generator.generate_test_data import GenerateTestData
@@ -133,15 +132,18 @@
         """
         return DirectedGraphBuilder(sparse_questions=self.get_matched_questions())
 
     def get_random_combinations(self, combinations: list[list]):
         """
         This function will select random combinations
         """
-        #return [combinations[47]]
+        selected_combination_index = path_or("",["selected_combination_index"], self.__event_data)
+        if selected_combination_index:
+            selected_combination_index = int(selected_combination_index)
+            return [path_or([],[selected_combination_index], combinations)]
         combination_samples = (
             path_or(5, ["combination_samples"], self.__event_data) or 5
         )
         return random.sample(combinations, int(combination_samples))
 
     def generate_test_actions(self, combo, all_questions, test_case_data):
         """
@@ -204,15 +206,15 @@
         return test_data
 
     async def send_trigger(self, payload):
         """
         This function will send trigger to runner lambda
         """
         lambda_obj = AwsClient().lambda_obj()
-        return lambda_obj.invoke(payload, "e2e_runner")
+        return lambda_obj.invoke(payload, "e2e_runner_dev_handler")
 
     async def create_async_invoke(self, test_data_list: list):
         """
         This function create async invokes
         """
         results = await asyncio.gather(
             *[
@@ -249,17 +251,27 @@
                         "nodes": path_or([], ["data"], data),
                         "combinations": path_or([], ["combination"], data),
                     }
                 }
             )
         return res
 
-    def start(self):
+    def generate_test_data(self):
         """
-        starts the generator
+            Return the test datas
         """
         graph_builder = self.get_directed_graph_builder()
         possible_combinations = graph_builder.build()
-        test_data = self.get_test_datas(combinations=possible_combinations)
-        payload = self.form_payload(test_data=test_data)
-        print(json.dumps(payload))
+        return self.get_test_datas(combinations=possible_combinations)
+
+    def get_payload(self):
+        """
+            This function return the payload
+        """
+        return self.form_payload(test_data=self.generate_test_data())
+
+    def start(self):
+        """
+        starts the generator
+        """
+        payload = self.get_payload()
         return asyncio.run(self.trigger_runner(payload))
```

### Comparing `lendsmart_autotest-1.4/autotest/lib/generator/question_type.py` & `lendsmart_autotest-1.5/generator/question_type.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.4/autotest/lib/generator/test_data.py` & `lendsmart_autotest-1.5/generator/test_data.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.4/autotest/lib/generator/utils.py` & `lendsmart_autotest-1.5/generator/utils.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.4/autotest/lib/runner/initializer.py` & `lendsmart_autotest-1.5/runner/initializer.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.4/setup.py` & `lendsmart_autotest-1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_packages, setup
 
 here = path.abspath(path.dirname(__file__))
 
 setup(
     name="lendsmart_autotest",
-    version="1.4",
+    version="1.5",
     description="The internal SDK for lendsmart autotest",
     url="https://bitbucket.org/lendsmartlabs/lendsmart_py/",
     # Author details
     author="Lendsmart",
     author_email="infos@lendsmart.ai",
     license="MIT",
     classifiers=[
```

