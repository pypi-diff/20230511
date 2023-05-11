# Comparing `tmp/plugnplai-0.0.6.tar.gz` & `tmp/plugnplai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugnplai-0.0.6.tar", max compression
+gzip compressed data, was "plugnplai-0.0.7.tar", max compression
```

## Comparing `plugnplai-0.0.6.tar` & `plugnplai-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-05-06 15:09:14.157127 plugnplai-0.0.6/LICENSE
--rw-r--r--   0        0        0     1943 2023-05-06 15:09:53.922130 plugnplai-0.0.6/README.md
--rw-r--r--   0        0        0      536 2023-05-07 01:14:27.562759 plugnplai-0.0.6/plugnplai/__init__.py
--rw-r--r--   0        0        0     4889 2023-05-06 15:09:14.167127 plugnplai-0.0.6/plugnplai/call_api.py
--rw-r--r--   0        0        0     2533 2023-05-07 01:49:00.904915 plugnplai-0.0.6/plugnplai/embeddings.py
--rw-r--r--   0        0        0     5590 2023-05-07 01:01:39.922701 plugnplai-0.0.6/plugnplai/load.py
--rw-r--r--   0        0        0     5753 2023-05-07 01:01:39.923701 plugnplai-0.0.6/plugnplai/plugin.py
--rw-r--r--   0        0        0        0 2023-05-07 01:02:14.288703 plugnplai-0.0.6/plugnplai/prompt.py
--rw-r--r--   0        0        0      483 2023-05-07 01:56:01.656947 plugnplai-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 plugnplai-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-06 15:09:14.157127 plugnplai-0.0.7/LICENSE
+-rw-r--r--   0        0        0     6082 2023-05-11 21:35:50.830908 plugnplai-0.0.7/README.md
+-rw-r--r--   0        0        0      603 2023-05-11 21:15:22.469816 plugnplai-0.0.7/plugnplai/__init__.py
+-rw-r--r--   0        0        0     4919 2023-05-11 21:14:34.459812 plugnplai-0.0.7/plugnplai/call_api.py
+-rw-r--r--   0        0        0     2534 2023-05-11 16:52:17.358593 plugnplai-0.0.7/plugnplai/embeddings.py
+-rw-r--r--   0        0        0    10646 2023-05-11 21:13:04.224805 plugnplai-0.0.7/plugnplai/plugins.py
+-rw-r--r--   0        0        0     1244 2023-05-11 21:13:47.722808 plugnplai-0.0.7/plugnplai/prompt_templates.py
+-rw-r--r--   0        0        0     7038 2023-05-11 20:23:01.258579 plugnplai-0.0.7/plugnplai/utils.py
+-rw-r--r--   0        0        0      483 2023-05-11 21:36:59.175913 plugnplai-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6829 1970-01-01 00:00:00.000000 plugnplai-0.0.7/PKG-INFO
```

### Comparing `plugnplai-0.0.6/LICENSE` & `plugnplai-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.6/plugnplai/call_api.py` & `plugnplai-0.0.7/plugnplai/call_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import re
 from typing import Any, Callable, Tuple
 
 import requests
 
-from plugnplai.plugin import InstallPlugins
+from plugnplai.plugins import InstallPlugins
 
+#### Under Construction ####
 
 class CallApi:
     def __init__(self, llm_response: str, active_plugins: InstallPlugins):
         self.llm_response = llm_response
         self.active_plugins = active_plugins
 
     def extract_command(self) -> Tuple[str, str]:
```

### Comparing `plugnplai-0.0.6/plugnplai/embeddings.py` & `plugnplai-0.0.7/plugnplai/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.schema import Document
 from langchain.vectorstores import FAISS
-from plugnplai.load import get_plugin_manifest, get_plugins
+from plugnplai.utils import get_plugin_manifest, get_plugins
 
 class PluginRetriever:
     def __init__(self, manifests: list, returnList: list = None):
         """
         manifests: list of manifest objects
         returnList: list of objects to be returned,
             can be a list of urls or a list of objects
```

### Comparing `plugnplai-0.0.6/plugnplai/load.py` & `plugnplai-0.0.7/plugnplai/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 import json
 import os
 
 import jsonref
 import requests
 import yaml
 
+def make_request_get(url: str, timeout=5):
+    try:
+        response = requests.get(url, timeout=timeout)
+        response.raise_for_status()  # Raises stored HTTPError, if one occurred.
+    except requests.exceptions.HTTPError as errh:
+        print ("Http Error:",errh)
+    except requests.exceptions.ConnectionError as errc:
+        print ("Error Connecting:",errc)
+    except requests.exceptions.Timeout as errt:
+        print ("Timeout Error:",errt)
+    except requests.exceptions.RequestException as err:
+        print ("Something went wrong",err)
+        return None
+    return response
 
-def get_plugins(filter: str = None, provider: str = "plugnplai"):
+def get_plugins(filter: str = None, category: str = None, provider: str = "plugnplai"):
     if provider == "plugnplai":
-        base_url = "https://www.plugnplai.com/_functions/getUrls"
-        # Construct the endpoint URL based on the filter argument
+        base_url = "https://www.plugnplai.com/_functions"
+        # Construct the endpoint URL based on the filter and category arguments
         if filter in ["working", "ChatGPT"]:
-            url = f'{base_url.strip("/")}/{filter}'
+            url = f'{base_url.strip("/")}/getUrls/{filter}'
+        elif category is not None:
+            url = f'{base_url.strip("/")}/getCategoryUrls/{category}'
         else:
-            url = base_url
+            url = f'{base_url.strip("/")}/getUrls'
         # Make the HTTP GET request
-        response = requests.get(url)
+        response = make_request_get(url)
         # Check if the response status code is successful (200 OK)
         if response.status_code == 200:
             # Parse the JSON response and return the result
             return response.json()
         else:
             # Handle unsuccessful responses
             return f"An error occurred: {response.status_code} {response.reason}"
@@ -29,20 +45,35 @@
         if response.status_code == 200:
             # Parse the JSON response and return the result
             return [f"https://{entry['domain']}" for entry in response.json()]
         else:
             # Handle unsuccessful responses
             return f"An error occurred: {response.status_code} {response.reason}"
 
+def get_category_names(provider: str = "plugnplai"):
+    if provider == "plugnplai":
+        base_url = "https://www.plugnplai.com/_functions"
+        url = f'{base_url.strip("/")}/categoryNames'
+        # Make the HTTP GET request
+        response = requests.get(url)
+        # Check if the response status code is successful (200 OK)
+        if response.status_code == 200:
+            # Parse the JSON response and return the result
+            return response.json()
+        else:
+            # Handle unsuccessful responses
+            return f"An error occurred: {response.status_code} {response.reason}"
+    else:
+        return "Provider not supported for this operation."
 
 # given a plugin url, get the ai-plugin.json manifest, in "/.well-known/ai-plugin.json"
 def get_plugin_manifest(url: str):
     urlJson = os.path.join(url, ".well-known/ai-plugin.json")
-    response = requests.get(urlJson).json()
-    return response
+    response = make_request_get(urlJson)
+    return response.json()
 
 
 # load the OpenAPI specification for the plugin, given the OpenAPI url described in the manifest file
 def get_openapi_url(url, manifest):
     openapi_url = manifest["api"]["url"]
     if openapi_url.startswith("/"):
         # remove slash in the end of url if present
```

