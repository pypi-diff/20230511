# Comparing `tmp/prompthub_py-1.0.0.tar.gz` & `tmp/prompthub_py-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompthub_py-1.0.0.tar", max compression
+gzip compressed data, was "prompthub_py-2.0.0.tar", max compression
```

## Comparing `prompthub_py-1.0.0.tar` & `prompthub_py-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11343 2023-03-30 15:50:42.546893 prompthub_py-1.0.0/LICENSE
--rw-r--r--   0        0        0     1633 2023-03-30 15:50:42.546893 prompthub_py-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-03-30 15:50:42.546893 prompthub_py-1.0.0/prompthub_py/__init__.py
--rw-r--r--   0        0        0     1715 2023-03-30 15:50:42.546893 prompthub_py-1.0.0/prompthub_py/prompt.py
--rw-r--r--   0        0        0      442 2023-03-30 15:50:42.550893 prompthub_py-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2198 1970-01-01 00:00:00.000000 prompthub_py-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-05-11 08:12:22.224273 prompthub_py-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1639 2023-05-11 08:12:22.224273 prompthub_py-2.0.0/README.md
+-rw-r--r--   0        0        0       65 2023-05-11 08:12:22.224273 prompthub_py-2.0.0/prompthub/__init__.py
+-rw-r--r--   0        0        0     1504 2023-05-11 08:12:22.224273 prompthub_py-2.0.0/prompthub/prompt.py
+-rw-r--r--   0        0        0      439 2023-05-11 08:12:22.224273 prompthub_py-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 prompthub_py-2.0.0/PKG-INFO
```

### Comparing `prompthub_py-1.0.0/LICENSE` & `prompthub_py-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prompthub_py-1.0.0/README.md` & `prompthub_py-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 ```
 pip install prompthub-py
 ```
 
 Then you can import `Prompt`, that class is all you're going to need.
 
 ```python
-from prompthub_py.prompt import Prompt
+import prompthub
 
 # To load from a JSON file
-p = Prompt.from_json("./path/to/my/prompt.json")
+p = prompthub.from_json("./path/to/my/prompt.json")
 
 
 # To load from a YAML file
-p = Prompt.from_yaml("./path/to/my/prompt.yaml")
+p = prompthub.from_yaml("./path/to/my/prompt.yaml")
 
 
 # To load from Prompt Hub
-p = Prompt.fetch("deepset/question-answering")
+p = prompthub.fetch("deepset/question-answering")
 
-# To get the prompt text
+# To get the prompt text (see Prompt class)
 p.text
 ```
 
 If you want to use a different Prompt Hub you must set the `PROMPTHUB_MAIN_ENDPOINT` environment variable to your main endpoint.
 
 If the environment variable is not set the default `api.prompthub.deepset.ai` will be used.
```

### Comparing `prompthub_py-1.0.0/prompthub_py/prompt.py` & `prompthub_py-2.0.0/prompthub/prompt.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,53 +19,53 @@
     name: str
     tags: List[str]
     meta: Dict[str, str]
     version: str
     text: str
     description: str
 
-    @staticmethod
-    def from_json(file: str):
-        with open(file) as f:
-            data = json.load(f)
-            return Prompt(
-                data["name"],
-                data["tags"],
-                data["meta"],
-                data["version"],
-                data["prompt_text"],
-                data["description"],
-            )
-
-    @staticmethod
-    def from_yaml(file: str):
-        with open(file) as f:
-            data = yaml.safe_load(f)
-            return Prompt(
-                data["name"],
-                data["tags"],
-                data["meta"],
-                data["version"],
-                data["prompt_text"],
-                data["description"],
-            )
-
-    @staticmethod
-    def fetch(name: str):
-        """
-        Fetches the specified prompt from PromptHUB and
-        returns a Prompt instance of it.
-
-        :param name: Name of the prompt to fetch from PromptHUB
-        :return: An instance of Prompt storing all its info
-        """
-        url = f"{MAIN_ENDPOINT}/prompts/{name}"
-        res = requests.get(url, timeout=30)
-        j = res.json()
+
+def from_json(file: str):
+    with open(file) as f:
+        data = json.load(f)
+        return Prompt(
+            data["name"],
+            data["tags"],
+            data["meta"],
+            data["version"],
+            data["prompt_text"],
+            data["description"],
+        )
+
+
+def from_yaml(file: str):
+    with open(file) as f:
+        data = yaml.safe_load(f)
         return Prompt(
-            j["name"],
-            j["tags"],
-            j["meta"],
-            j["version"],
-            j["prompt_text"],
-            j["description"],
+            data["name"],
+            data["tags"],
+            data["meta"],
+            data["version"],
+            data["prompt_text"],
+            data["description"],
         )
+
+
+def fetch(name: str):
+    """
+    Fetches the specified prompt from PromptHUB and
+    returns a Prompt instance of it.
+
+    :param name: Name of the prompt to fetch from PromptHUB
+    :return: An instance of Prompt storing all its info
+    """
+    url = f"{MAIN_ENDPOINT}/prompts/{name}"
+    res = requests.get(url, timeout=30)
+    j = res.json()
+    return Prompt(
+        j["name"],
+        j["tags"],
+        j["meta"],
+        j["version"],
+        j["prompt_text"],
+        j["description"],
+    )
```

### Comparing `prompthub_py-1.0.0/PKG-INFO` & `prompthub_py-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompthub-py
-Version: 1.0.0
+Version: 2.0.0
 Summary: 
 License: Apache-2.0
 Author: deepset.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -28,28 +28,28 @@
 ```
 pip install prompthub-py
 ```
 
 Then you can import `Prompt`, that class is all you're going to need.
 
 ```python
-from prompthub_py.prompt import Prompt
+import prompthub
 
 # To load from a JSON file
-p = Prompt.from_json("./path/to/my/prompt.json")
+p = prompthub.from_json("./path/to/my/prompt.json")
 
 
 # To load from a YAML file
-p = Prompt.from_yaml("./path/to/my/prompt.yaml")
+p = prompthub.from_yaml("./path/to/my/prompt.yaml")
 
 
 # To load from Prompt Hub
-p = Prompt.fetch("deepset/question-answering")
+p = prompthub.fetch("deepset/question-answering")
 
-# To get the prompt text
+# To get the prompt text (see Prompt class)
 p.text
 ```
 
 If you want to use a different Prompt Hub you must set the `PROMPTHUB_MAIN_ENDPOINT` environment variable to your main endpoint.
 
 If the environment variable is not set the default `api.prompthub.deepset.ai` will be used.
```

