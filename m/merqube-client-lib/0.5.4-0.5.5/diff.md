# Comparing `tmp/merqube_client_lib-0.5.4.tar.gz` & `tmp/merqube_client_lib-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.5.4.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.5.5.tar", max compression
```

## Comparing `merqube_client_lib-0.5.4.tar` & `merqube_client_lib-0.5.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/LICENSE
--rw-r--r--   0        0        0      377 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/README.md
--rw-r--r--   0        0        0        0 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0      367 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      482 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0     1934 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/logging.py
--rw-r--r--   0        0        0     3028 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/mocker.py
--rw-r--r--   0        0        0        0 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/py.typed
--rw-r--r--   0        0        0        0 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/secapi/__init__.py
--rw-r--r--   0        0        0    12490 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/secapi/client.py
--rw-r--r--   0        0        0    11754 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/session.py
--rw-r--r--   0        0        0      351 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/types/__init__.py
--rw-r--r--   0        0        0      418 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/types/secapi.py
--rw-r--r--   0        0        0      677 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/util.py
--rw-r--r--   0        0        0     1713 2023-05-10 17:25:12.601589 merqube_client_lib-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-10 22:13:35.855969 merqube_client_lib-0.5.5/LICENSE
+-rw-r--r--   0        0        0      377 2023-05-10 22:13:35.855969 merqube_client_lib-0.5.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 22:13:35.855969 merqube_client_lib-0.5.5/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0      367 2023-05-10 22:13:35.855969 merqube_client_lib-0.5.5/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      482 2023-05-10 22:13:35.859969 merqube_client_lib-0.5.5/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0     1934 2023-05-10 22:13:35.859969 merqube_client_lib-0.5.5/merqube_client_lib/logging.py
+-rw-r--r--   0        0        0     3476 2023-05-10 22:13:35.859969 merqube_client_lib-0.5.5/merqube_client_lib/mocker.py
+-rw-r--r--   0        0        0        0 2023-05-10 22:13:35.859969 merqube_client_lib-0.5.5/merqube_client_lib/py.typed
+-rw-r--r--   0        0        0        0 2023-05-10 22:13:35.859969 merqube_client_lib-0.5.5/merqube_client_lib/secapi/__init__.py
+-rw-r--r--   0        0        0    12490 2023-05-10 22:13:35.859969 merqube_client_lib-0.5.5/merqube_client_lib/secapi/client.py
+-rw-r--r--   0        0        0    11754 2023-05-10 22:13:35.859969 merqube_client_lib-0.5.5/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      351 2023-05-10 22:13:35.859969 merqube_client_lib-0.5.5/merqube_client_lib/types/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-10 22:13:35.859969 merqube_client_lib-0.5.5/merqube_client_lib/types/secapi.py
+-rw-r--r--   0        0        0      677 2023-05-10 22:13:35.859969 merqube_client_lib-0.5.5/merqube_client_lib/util.py
+-rw-r--r--   0        0        0     1713 2023-05-10 22:13:35.859969 merqube_client_lib-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.5.5/PKG-INFO
```

### Comparing `merqube_client_lib-0.5.4/LICENSE` & `merqube_client_lib-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.4/merqube_client_lib/logging.py` & `merqube_client_lib-0.5.5/merqube_client_lib/logging.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.4/merqube_client_lib/mocker.py` & `merqube_client_lib-0.5.5/merqube_client_lib/mocker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """
 Module for mocking secapi, mostly for unit testing, but also for other components testing against secapi
 """
-
 import importlib
+import logging
 from typing import Any, Callable, Optional
 from unittest.mock import MagicMock
 
 from cachetools import Cache
 
+from merqube_client_lib.logging import get_module_logger
+
+logger = get_module_logger(__name__, level=logging.DEBUG)
+
 
 def _sec_types() -> list[dict[str, str]]:
     """fixed map for mocking valid sectypes"""
     return [
         {"name": "crypto_asset"},
         {"name": "custom"},
         {"name": "equity"},
@@ -62,31 +66,37 @@
     client_module = importlib.import_module(client_function_module_name)
 
     def mock_secapi(monkeypatch, method_name_function_map: dict[str, Callable[..., Any]]) -> None:
         """
         get a client with some methods patched with swapout functions
         """
         if secapi_client_cache is not None:
+            logger.debug("Clearing client cache")
             secapi_client_cache.clear()
+        else:
+            logger.debug("No client cache to clear")
 
         sess = MagicMock()
+        logger.debug(f"Mocking session at {get_session_function_path}")
         monkeypatch.setattr(get_session_function_path, MagicMock(return_value=sess))
 
         client = client_module.get_client()
 
         if "get_supported_secapi_types" not in method_name_function_map:
             setattr(client, "get_supported_secapi_types", _sec_types)
 
         # inside
 
         for method_name, func in method_name_function_map.items():
             if getattr(client, method_name) is None:
                 raise ValueError("Trying to patch a function that doesnt exist in the client")
+            logger.debug(f"Mocking method {method_name}")
             setattr(client, method_name, func)
 
         def get_client(*args: Any, **kwargs: Any):
             return client
 
         # now a get_client call from the main code will return this mocked client:
+        logger.debug(f"Mocking client at {get_client_function_path}")
         monkeypatch.setattr(get_client_function_path, get_client)
 
     return mock_secapi
```

### Comparing `merqube_client_lib-0.5.4/merqube_client_lib/secapi/client.py` & `merqube_client_lib-0.5.5/merqube_client_lib/secapi/client.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.4/merqube_client_lib/session.py` & `merqube_client_lib-0.5.5/merqube_client_lib/session.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.4/merqube_client_lib/util.py` & `merqube_client_lib-0.5.5/merqube_client_lib/util.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.4/pyproject.toml` & `merqube_client_lib-0.5.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.5.4"
+version = "0.5.5"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
 readme = "README.md"
 license = "APACHE-2.0"
 homepage = "https://github.com/merqube/merqube-client-lib"
 include = [
     "LICENSE",
```

### Comparing `merqube_client_lib-0.5.4/PKG-INFO` & `merqube_client_lib-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merqube-client-lib
-Version: 0.5.4
+Version: 0.5.5
 Summary: MerQube IndexAPI + SecAPI client library
 Home-page: https://github.com/merqube/merqube-client-lib
 License: Apache-2.0
 Author: Merqube
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

