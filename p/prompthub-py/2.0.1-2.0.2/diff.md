# Comparing `tmp/prompthub_py-2.0.1.tar.gz` & `tmp/prompthub_py-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompthub_py-2.0.1.tar", max compression
+gzip compressed data, was "prompthub_py-2.0.2.tar", max compression
```

## Comparing `prompthub_py-2.0.1.tar` & `prompthub_py-2.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11343 2023-05-11 10:01:49.625103 prompthub_py-2.0.1/LICENSE
--rw-r--r--   0        0        0     1639 2023-05-11 10:01:49.625103 prompthub_py-2.0.1/README.md
--rw-r--r--   0        0        0       65 2023-05-11 10:01:49.629103 prompthub_py-2.0.1/prompthub/__init__.py
--rw-r--r--   0        0        0     1642 2023-05-11 10:01:49.629103 prompthub_py-2.0.1/prompthub/prompt.py
--rw-r--r--   0        0        0      439 2023-05-11 10:01:49.629103 prompthub_py-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 prompthub_py-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-05-11 11:45:57.029591 prompthub_py-2.0.2/LICENSE
+-rw-r--r--   0        0        0     1639 2023-05-11 11:45:57.029591 prompthub_py-2.0.2/README.md
+-rw-r--r--   0        0        0       65 2023-05-11 11:45:57.029591 prompthub_py-2.0.2/prompthub/__init__.py
+-rw-r--r--   0        0        0     1669 2023-05-11 11:45:57.029591 prompthub_py-2.0.2/prompthub/prompt.py
+-rw-r--r--   0        0        0      439 2023-05-11 11:45:57.029591 prompthub_py-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 prompthub_py-2.0.2/PKG-INFO
```

### Comparing `prompthub_py-2.0.1/LICENSE` & `prompthub_py-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prompthub_py-2.0.1/README.md` & `prompthub_py-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `prompthub_py-2.0.1/prompthub/prompt.py` & `prompthub_py-2.0.2/prompthub/prompt.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     :param name: Name of the prompt to fetch from PromptHUB
     :param timeout: (optional) How many seconds to wait for the server to send data
         before giving up.
     :return: An instance of Prompt storing all its info
     """
     url = f"{MAIN_ENDPOINT}/prompts/{name}"
     res = requests.get(url, timeout=timeout)
+    res.raise_for_status()
     j = res.json()
     return Prompt(
         j["name"],
         j["tags"],
         j["meta"],
         j["version"],
         j["prompt_text"],
```

### Comparing `prompthub_py-2.0.1/PKG-INFO` & `prompthub_py-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompthub-py
-Version: 2.0.1
+Version: 2.0.2
 Summary: 
 License: Apache-2.0
 Author: deepset.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

