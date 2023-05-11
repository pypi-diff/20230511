# Comparing `tmp/plugnplai-0.0.8.tar.gz` & `tmp/plugnplai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugnplai-0.0.8.tar", max compression
+gzip compressed data, was "plugnplai-0.0.9.tar", max compression
```

## Comparing `plugnplai-0.0.8.tar` & `plugnplai-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-05-06 15:09:14.157127 plugnplai-0.0.8/LICENSE
--rw-r--r--   0        0        0     6082 2023-05-11 21:35:50.830908 plugnplai-0.0.8/README.md
--rw-r--r--   0        0        0      603 2023-05-11 21:15:22.469816 plugnplai-0.0.8/plugnplai/__init__.py
--rw-r--r--   0        0        0     4919 2023-05-11 21:14:34.459812 plugnplai-0.0.8/plugnplai/call_api.py
--rw-r--r--   0        0        0     2534 2023-05-11 16:52:17.358593 plugnplai-0.0.8/plugnplai/embeddings.py
--rw-r--r--   0        0        0    10647 2023-05-11 21:40:24.823929 plugnplai-0.0.8/plugnplai/plugins.py
--rw-r--r--   0        0        0     1244 2023-05-11 21:13:47.722808 plugnplai-0.0.8/plugnplai/prompt_templates.py
--rw-r--r--   0        0        0     7038 2023-05-11 20:23:01.258579 plugnplai-0.0.8/plugnplai/utils.py
--rw-r--r--   0        0        0      483 2023-05-11 21:40:38.169930 plugnplai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6829 1970-01-01 00:00:00.000000 plugnplai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-06 15:09:14.157127 plugnplai-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6082 2023-05-11 21:35:50.830908 plugnplai-0.0.9/README.md
+-rw-r--r--   0        0        0      603 2023-05-11 21:15:22.469816 plugnplai-0.0.9/plugnplai/__init__.py
+-rw-r--r--   0        0        0     5139 2023-05-11 21:42:52.960940 plugnplai-0.0.9/plugnplai/call_api.py
+-rw-r--r--   0        0        0     2534 2023-05-11 16:52:17.358593 plugnplai-0.0.9/plugnplai/embeddings.py
+-rw-r--r--   0        0        0    10647 2023-05-11 21:40:24.823929 plugnplai-0.0.9/plugnplai/plugins.py
+-rw-r--r--   0        0        0     1244 2023-05-11 21:13:47.722808 plugnplai-0.0.9/plugnplai/prompt_templates.py
+-rw-r--r--   0        0        0     7038 2023-05-11 20:23:01.258579 plugnplai-0.0.9/plugnplai/utils.py
+-rw-r--r--   0        0        0      483 2023-05-11 21:43:05.579941 plugnplai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6829 1970-01-01 00:00:00.000000 plugnplai-0.0.9/PKG-INFO
```

### Comparing `plugnplai-0.0.8/LICENSE` & `plugnplai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.8/README.md` & `plugnplai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.8/plugnplai/__init__.py` & `plugnplai-0.0.9/plugnplai/__init__.py`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.8/plugnplai/call_api.py` & `plugnplai-0.0.9/plugnplai/call_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-import json
-import re
-from typing import Any, Callable, Tuple
-
-import requests
-
-from plugnplai.plugins import InstallPlugins
-
-#### Under Construction ####
-
-class CallApi:
-    def __init__(self, llm_response: str, active_plugins: InstallPlugins):
-        self.llm_response = llm_response
-        self.active_plugins = active_plugins
-
-    def extract_command(self) -> Tuple[str, str]:
-        api_split = self.llm_response.split("[API]")
-        if len(api_split) < 3:
-            raise ValueError("API call not found.")
-        api_call = api_split[1]
-
-        body_split = api_split[2].split("[PARAMS]")
-        if len(body_split) < 3:
-            raise ValueError("API body not found.")
-        api_body_str = body_split[1]
-
-        try:
-            api_body = json.loads(api_body_str)
-        except json.JSONDecodeError:
-            print(f"Error: Invalid JSON in the API body. Content: {api_body_str}")
-            return None, None
-
-        self.api_pattern = (
-            "[API]" + api_split[1] + "[API]" + "[PARAMS]" + body_split[1] + "[PARAMS]"
-        )
-        self.api_name = api_split[1].split(".")[0]
-
-        return api_call, api_body
-
-    def get_open_api_spec(self, namespace: str) -> dict:
-        for plugin in self.active_plugins.Plugins:
-            if plugin.name == namespace:
-                return plugin.api_spec, plugin.url
-        return None
-
-    def build_request(self, api_call: str, api_body: dict) -> dict:
-        # Assuming api_call format is "Namespace.Operation", e.g., "KlarnaProducts.productsUsingGET"
-        namespace, operation = api_call.split(".")
-
-        # Locate the API endpoint and method in the OpenAPI spec
-        open_api_spec, plugin_url = self.get_open_api_spec(namespace)
-        for path, methods in open_api_spec["paths"].items():
-            for method, spec in methods.items():
-                if spec["operationId"] == operation:
-                    serverUrl = open_api_spec["servers"][0]["url"] + path
-                    return {
-                        "url": serverUrl,
-                        "method": method.upper(),
-                        # "headers": {"Content-Type": "application/json"},
-                        "data": api_body,
-                    }
-
-    def make_request(self, request):
-        response = requests.request(
-            method=request["method"],
-            url=request["url"],
-            # headers=request["headers"],
-            params=request["data"],
-        )
-
-        # Check if the response content is not empty and valid JSON
-        try:
-            json_data = response.json()
-        except ValueError:
-            print(f"Error: Response is not valid JSON. Content: {response.text}")
-            print(f"Full response: {response}")
-            return None
-
-        return json_data
-
-    def process(self) -> str:
-        try:
-            api_call, api_body = self.extract_command()
-        except ValueError as e:
-            print(e)
-            return self.llm_response.split("[API]")[0] + str(e)
-        if api_call:
-            request = self.build_request(api_call, api_body)
-            response = self.make_request(request)
-            message_to_user = f"Calling {self.api_name} API..."
-
-            return response, re.sub(self.api_pattern, str(response), message_to_user)
-        return self.llm_response
-
-
-class AddPlugins:
-    def __init__(self, active_plugins):
-        self.active_plugins = active_plugins
-
-    def __call__(self, func: Callable[..., Any]) -> Callable[..., Any]:
-        def wrapper(*args, **kwargs) -> Any:
-            print(args)
-            # Call the original function (GPT-4 API call)
-            llm_response = func(*args, **kwargs)
-            content_llm_response = llm_response.content
-            print(f"first llm response: {content_llm_response}")
-
-            # Check for the specific pattern (**) in the response
-            if "[API]" not in content_llm_response:
-                return llm_response
-
-            # Use the CallApi class to make an API call based on the response
-            # print("has [API]")
-            call_api = CallApi(content_llm_response, self.active_plugins)
-            api_response, message_to_user = call_api.process()
-            print(message_to_user)
-            print(api_response)
-
-            human_message = args[0][1].content
-
-            prompt = f"""
-Assistant is a large language model with access to plugins.\nKnowledge Cutoff: 2021-09\nCurrent date: 2023-04-19
-
-Assistant called a plugin in response to the human message bellow. Use the API response to write a comprehensive human-readble response for the human message:
-[Plugin API request]
-{content_llm_response}
-
-[API response]
-{api_response}
-
-[Human message]
-{human_message}"""
-            args[0][0].content = prompt
-            args[0][1].content = ""
-            llm_final_response = func(*args, **kwargs)
+# import json
+# import re
+# from typing import Any, Callable, Tuple
+
+# import requests
+
+# from plugnplai.plugins import InstallPlugins
+
+# #### Under Construction ####
+
+# class CallApi:
+#     def __init__(self, llm_response: str, active_plugins: InstallPlugins):
+#         self.llm_response = llm_response
+#         self.active_plugins = active_plugins
+
+#     def extract_command(self) -> Tuple[str, str]:
+#         api_split = self.llm_response.split("[API]")
+#         if len(api_split) < 3:
+#             raise ValueError("API call not found.")
+#         api_call = api_split[1]
+
+#         body_split = api_split[2].split("[PARAMS]")
+#         if len(body_split) < 3:
+#             raise ValueError("API body not found.")
+#         api_body_str = body_split[1]
+
+#         try:
+#             api_body = json.loads(api_body_str)
+#         except json.JSONDecodeError:
+#             print(f"Error: Invalid JSON in the API body. Content: {api_body_str}")
+#             return None, None
+
+#         self.api_pattern = (
+#             "[API]" + api_split[1] + "[API]" + "[PARAMS]" + body_split[1] + "[PARAMS]"
+#         )
+#         self.api_name = api_split[1].split(".")[0]
+
+#         return api_call, api_body
+
+#     def get_open_api_spec(self, namespace: str) -> dict:
+#         for plugin in self.active_plugins.Plugins:
+#             if plugin.name == namespace:
+#                 return plugin.api_spec, plugin.url
+#         return None
+
+#     def build_request(self, api_call: str, api_body: dict) -> dict:
+#         # Assuming api_call format is "Namespace.Operation", e.g., "KlarnaProducts.productsUsingGET"
+#         namespace, operation = api_call.split(".")
+
+#         # Locate the API endpoint and method in the OpenAPI spec
+#         open_api_spec, plugin_url = self.get_open_api_spec(namespace)
+#         for path, methods in open_api_spec["paths"].items():
+#             for method, spec in methods.items():
+#                 if spec["operationId"] == operation:
+#                     serverUrl = open_api_spec["servers"][0]["url"] + path
+#                     return {
+#                         "url": serverUrl,
+#                         "method": method.upper(),
+#                         # "headers": {"Content-Type": "application/json"},
+#                         "data": api_body,
+#                     }
+
+#     def make_request(self, request):
+#         response = requests.request(
+#             method=request["method"],
+#             url=request["url"],
+#             # headers=request["headers"],
+#             params=request["data"],
+#         )
+
+#         # Check if the response content is not empty and valid JSON
+#         try:
+#             json_data = response.json()
+#         except ValueError:
+#             print(f"Error: Response is not valid JSON. Content: {response.text}")
+#             print(f"Full response: {response}")
+#             return None
+
+#         return json_data
+
+#     def process(self) -> str:
+#         try:
+#             api_call, api_body = self.extract_command()
+#         except ValueError as e:
+#             print(e)
+#             return self.llm_response.split("[API]")[0] + str(e)
+#         if api_call:
+#             request = self.build_request(api_call, api_body)
+#             response = self.make_request(request)
+#             message_to_user = f"Calling {self.api_name} API..."
+
+#             return response, re.sub(self.api_pattern, str(response), message_to_user)
+#         return self.llm_response
+
+
+# class AddPlugins:
+#     def __init__(self, active_plugins):
+#         self.active_plugins = active_plugins
+
+#     def __call__(self, func: Callable[..., Any]) -> Callable[..., Any]:
+#         def wrapper(*args, **kwargs) -> Any:
+#             print(args)
+#             # Call the original function (GPT-4 API call)
+#             llm_response = func(*args, **kwargs)
+#             content_llm_response = llm_response.content
+#             print(f"first llm response: {content_llm_response}")
+
+#             # Check for the specific pattern (**) in the response
+#             if "[API]" not in content_llm_response:
+#                 return llm_response
+
+#             # Use the CallApi class to make an API call based on the response
+#             # print("has [API]")
+#             call_api = CallApi(content_llm_response, self.active_plugins)
+#             api_response, message_to_user = call_api.process()
+#             print(message_to_user)
+#             print(api_response)
+
+#             human_message = args[0][1].content
+
+#             prompt = f"""
+# Assistant is a large language model with access to plugins.\nKnowledge Cutoff: 2021-09\nCurrent date: 2023-04-19
+
+# Assistant called a plugin in response to the human message bellow. Use the API response to write a comprehensive human-readble response for the human message:
+# [Plugin API request]
+# {content_llm_response}
+
+# [API response]
+# {api_response}
+
+# [Human message]
+# {human_message}"""
+#             args[0][0].content = prompt
+#             args[0][1].content = ""
+#             llm_final_response = func(*args, **kwargs)
 
-            return llm_final_response
+#             return llm_final_response
 
-        return wrapper
+#         return wrapper
```

### Comparing `plugnplai-0.0.8/plugnplai/embeddings.py` & `plugnplai-0.0.9/plugnplai/embeddings.py`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.8/plugnplai/plugins.py` & `plugnplai-0.0.9/plugnplai/plugins.py`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.8/plugnplai/prompt_templates.py` & `plugnplai-0.0.9/plugnplai/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.8/plugnplai/utils.py` & `plugnplai-0.0.9/plugnplai/utils.py`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.8/PKG-INFO` & `plugnplai-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugnplai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Connect plugins to AI
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

