# Comparing `tmp/aiofauna-0.1.7.tar.gz` & `tmp/aiofauna-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofauna-0.1.7.tar", max compression
+gzip compressed data, was "aiofauna-0.1.8.tar", max compression
```

## Comparing `aiofauna-0.1.7.tar` & `aiofauna-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1126 2023-05-08 06:43:22.972944 aiofauna-0.1.7/LICENSE
--rw-r--r--   0        0        0     2678 2023-05-08 04:44:25.192212 aiofauna-0.1.7/README.md
--rw-r--r--   0        0        0     3656 2023-05-08 06:40:40.439634 aiofauna-0.1.7/aiofauna/__init__.py
--rw-r--r--   0        0        0    16832 2023-05-10 08:11:24.200112 aiofauna-0.1.7/aiofauna/api.py
--rw-r--r--   0        0        0     3304 2023-05-08 02:52:55.686757 aiofauna-0.1.7/aiofauna/asgi.py
--rw-r--r--   0        0        0     7679 2023-05-08 06:40:32.547771 aiofauna-0.1.7/aiofauna/client.py
--rw-r--r--   0        0        0     3678 2023-05-08 02:23:17.855099 aiofauna-0.1.7/aiofauna/datastructures.py
--rw-r--r--   0        0        0      493 2023-05-06 09:16:36.202849 aiofauna-0.1.7/aiofauna/deprecated.py
--rw-r--r--   0        0        0     8153 2023-05-08 02:23:18.327095 aiofauna-0.1.7/aiofauna/errors.py
--rw-r--r--   0        0        0     4056 2023-05-08 06:40:40.455633 aiofauna-0.1.7/aiofauna/helpers.py
--rw-r--r--   0        0        0     6728 2023-05-08 03:17:10.714267 aiofauna-0.1.7/aiofauna/json.py
--rw-r--r--   0        0        0     5841 2023-05-08 02:23:18.171096 aiofauna-0.1.7/aiofauna/objects.py
--rw-r--r--   0        0        0    14644 2023-05-08 16:22:07.056807 aiofauna-0.1.7/aiofauna/odm.py
--rw-r--r--   0        0        0     2672 2023-05-08 02:26:21.521409 aiofauna-0.1.7/aiofauna/page.py
--rw-r--r--   0        0        0    41561 2023-05-08 02:26:13.437479 aiofauna-0.1.7/aiofauna/query.py
--rw-r--r--   0        0        0      661 2023-05-10 08:02:31.870474 aiofauna-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3597 2023-05-10 08:11:32.956275 aiofauna-0.1.7/setup.py
--rw-r--r--   0        0        0     3697 2023-05-10 08:11:32.957198 aiofauna-0.1.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1126 2023-05-08 06:43:22.972944 aiofauna-0.1.8/LICENSE
+-rwxr-xr-x   0        0        0     2678 2023-05-08 04:44:25.192212 aiofauna-0.1.8/README.md
+-rwxr-xr-x   0        0        0     3698 2023-05-11 08:26:07.398242 aiofauna-0.1.8/aiofauna/__init__.py
+-rwxr-xr-x   0        0        0    16796 2023-05-11 08:26:00.406228 aiofauna-0.1.8/aiofauna/api.py
+-rwxr-xr-x   0        0        0     3304 2023-05-08 02:52:55.686757 aiofauna-0.1.8/aiofauna/asgi.py
+-rwxr-xr-x   0        0        0     7679 2023-05-08 06:40:32.547771 aiofauna-0.1.8/aiofauna/client.py
+-rwxr-xr-x   0        0        0     3678 2023-05-08 02:23:17.855099 aiofauna-0.1.8/aiofauna/datastructures.py
+-rwxr-xr-x   0        0        0      493 2023-05-06 09:16:36.202849 aiofauna-0.1.8/aiofauna/deprecated.py
+-rwxr-xr-x   0        0        0     8153 2023-05-08 02:23:18.327095 aiofauna-0.1.8/aiofauna/errors.py
+-rwxr-xr-x   0        0        0     4056 2023-05-08 06:40:40.455633 aiofauna-0.1.8/aiofauna/helpers.py
+-rwxr-xr-x   0        0        0     6728 2023-05-08 03:17:10.714267 aiofauna-0.1.8/aiofauna/json.py
+-rwxr-xr-x   0        0        0     5841 2023-05-08 02:23:18.171096 aiofauna-0.1.8/aiofauna/objects.py
+-rwxr-xr-x   0        0        0    21874 2023-05-11 21:04:02.733525 aiofauna-0.1.8/aiofauna/odm.py
+-rwxr-xr-x   0        0        0     2672 2023-05-08 02:26:21.521409 aiofauna-0.1.8/aiofauna/page.py
+-rwxr-xr-x   0        0        0    41561 2023-05-08 02:26:13.437479 aiofauna-0.1.8/aiofauna/query.py
+-rwxr-xr-x   0        0        0      661 2023-05-11 08:23:40.249922 aiofauna-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3597 2023-05-11 21:05:02.670231 aiofauna-0.1.8/setup.py
+-rw-r--r--   0        0        0     3697 2023-05-11 21:05:02.671110 aiofauna-0.1.8/PKG-INFO
```

### Comparing `aiofauna-0.1.7/LICENSE` & `aiofauna-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.7/README.md` & `aiofauna-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.7/aiofauna/__init__.py` & `aiofauna-0.1.8/aiofauna/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 """
+AioFauna
+"""
+
+__version__ = (0, 1, 8)
+__author__ = "obahamonde"
+__license__ = "MIT"
+__doc__ = """
 ---
 title: AioFauna
 ---
 # AioFauna
 
 🚀 Introducing aiofauna: A full-stack framework built on top of Aiohttp, Pydantic and FaunaDB.
 
@@ -41,35 +48,26 @@
 📚 [Documentation](https://obahamonde-aiofauna-docs.smartpro.solutions) (Built with aiofauna)
 
 📦 [PyPi](https://pypi.org/project/aiofauna/)
 
 📦 [GitHub](https://github.com/obahamonde/aiofauna)
 
 📦 [Demo](https://aiofaunastreams-fwuw7gz7oq-uc.a.run.app/) (Real time Latency Monitoring between FaunaDB and Google Cloud Run)
-
 """
 
-__version__ = (0, 1, 5)
-__author__ = "obahamonde"
-__license__ = "MIT"
-
 import json
 from datetime import datetime
 from typing import Any, AsyncGenerator, Callable, Dict, List, Optional, Union
 from uuid import UUID, uuid4
 
 import asyncio
 import aiohttp_cors
-from pydantic import (
-    BaseModel,
-    BaseConfig,
-    BaseSettings,
-    Field,
-)  # pylint: disable=no-name-in-module
+from pydantic import BaseModel,BaseConfig,BaseSettings,Field  # pylint: disable=no-name-in-module
 from aiohttp.web import json_response as jsonify, Request, Response
+from aiohttp.web_request import FileField
 from aiohttp_sse import sse_response
 from .client import ClientSession, AsyncFaunaClient as FaunaClient
 from .errors import AioFaunaException as FaunaException
 from . import query as q
 from .json import (
     FaunaJSONEncoder as JSONEncoder,
     to_json as dumps,
```

### Comparing `aiofauna-0.1.7/aiofauna/api.py` & `aiofauna-0.1.8/aiofauna/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,76 +1,74 @@
 """REST API Module with automatic OpenAPI generation."""
 import json
 import base64
 import asyncio
+from json import JSONDecoder
 from typing import Any, Dict, List, Union
 from inspect import signature
 from uuid import UUID
 from datetime import datetime, date, time
 from functools import singledispatch
 from enum import Enum
 from aiohttp.web import Application, Request, Response, json_response
-from json import JSONDecoder
 from aiohttp.web_request import FileField
-from aiohttp_sse import EventSourceResponse
-from .odm import AsyncFaunaModel
 from pydantic import BaseModel  # pylint: disable=no-name-in-module
-from .json import FaunaJSONEncoder as JSONEncoder, to_json, parse_json_or_none
-
+from .json import FaunaJSONEncoder, parse_json_or_none
+from .odm import AsyncFaunaModel
 
 def jsonable_encoder(
-    obj,
+    obj: Any,
     *,
-    include=None,
-    exclude=None,
-    by_alias=False,
-    skip_defaults=False,
-    custom_encoder=None,
-):
+    include: List[str] = [],
+    exclude: List[str] = [],
+    by_alias: bool = False,
+    skip_defaults: bool = False,
+    custom_encoder: Any = None,
+) -> Any:
     """
     Convert any object to a JSON-serializable object.
 
     This function is used by Aiofauna to convert objects to JSON-serializable objects.
 
     It supports all the types supported by the standard json library, plus:
 
     * datetime.datetime
     * datetime.date
     * datetime.time
     * uuid.UUID
     * enum.Enum
     * pydantic.BaseModel
-
     """
 
     if custom_encoder is None:
-        custom_encoder = JSONEncoder
-    if obj == str:
+        custom_encoder = FaunaJSONEncoder
+
+    if obj is str:
         return "string"
-    if obj in (int, float):
+    if obj is int or obj is float:
         return "integer"
-    if obj == bool:
+    if obj is bool:
         return "boolean"
-    if obj == None:
+    if obj is None:
         return "null"
-    if obj == list:
+    if obj is list:
         return "array"
-    if obj == dict:
+    if obj is dict:
         return "object"
-    if obj == bytes:
+    if obj is bytes:
         return "binary"
-    if obj == datetime:
+    if obj is datetime:
         return "date-time"
-    if obj == date:
+    if obj is date:
         return "date"
-    if obj == time:
+    if obj is time:
         return "time"
-    if obj == UUID:
+    if obj is UUID:
         return "uuid"
-    if obj == Enum:
+    if obj is Enum:
         return "enum"
     if isinstance(obj, (str, int, float, bool, type(None))):
         return obj
     if isinstance(obj, (list, tuple, set, frozenset)):
         return [
             jsonable_encoder(
                 v,
@@ -99,15 +97,14 @@
                 skip_defaults=skip_defaults,
                 custom_encoder=custom_encoder,
             )
             for k, v in obj.items()
         }
     if isinstance(obj, bytes):
         return base64.b64encode(obj).decode()
-
     if isinstance(obj, (set, frozenset)):
         return [
             jsonable_encoder(
                 v,
                 include=include,
                 exclude=exclude,
                 by_alias=by_alias,
@@ -120,15 +117,14 @@
         return obj.isoformat()
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, UUID):
         return str(obj)
     return custom_encoder().default(obj)
 
-
 def extract_params(params: dict, path: str):
     """
     FastAPIesque function to extract the parameters of a function outside of the request context.
     """
 
     open_api_params = {}
 
@@ -157,15 +153,15 @@
             }
 
         elif issubclass(type_, FileField):
             open_api_params[name] = {
                 "in": "formData",
                 "name": name,
                 "required": True,
-                "schema": {"type": "file", "default": param.default, "required": True},
+                "schema": {"type": "file"},
             }
 
         else:
             continue
 
     return open_api_params
 
@@ -219,14 +215,39 @@
                 "summary": func.__name__,
                 "description": func.__doc__,
                 "parameters": _scalars,
                 "responses": {"200": {"description": "OK"}},
             }
 
 
+
+async def inject_signature(request: Request, params: dict):
+    """
+    FastAPIesque function to shape the signature of a function to the request.
+    """
+    args_to_apply = {}
+
+    for name, param in params.items():
+        type_ = param.annotation
+        if type_ in (str, int, float, bool) and name in request.match_info:
+            args_to_apply[name] = request.match_info[name]
+        elif type_ in (str, int, float, bool) and name in request.query:
+            args_to_apply[name] = type_(request.query[name])
+        elif issubclass(type_, BaseModel):
+            data = await request.json(loads=JSONDecoder().decode)
+            if isinstance(data, Union[str,bytes]):
+                data = json.loads(data, object_hook=parse_json_or_none)
+            args_to_apply[name] = type_(**data)
+        elif issubclass(type_, FileField):
+            args_to_apply[name] = await request.post()
+        else:
+            continue
+    return args_to_apply
+
+
 @singledispatch
 def do_response(response: Any) -> Response:
     """
     Flask-esque function to make a response from a function.
     """
     return response
 
@@ -319,64 +340,32 @@
     return Response(
         status=200,
         body=json.dumps(processed_response),
         content_type="application/json",
     )
 
 
-async def inject_signature(request: Request, params: dict):
-    """
-    FastAPIesque function to shape the signature of a function to the request.
-    """
-    args_to_apply = {}
-
-    for name, param in params.items():
-        type_ = param.annotation
-        if type_ in (str, int, float, bool) and name in request.match_info:
-            args_to_apply[name] = request.match_info[name]
-        elif type_ in (str, int, float, bool) and name in request.query:
-            args_to_apply[name] = type_(request.query[name])
-        elif issubclass(type_, BaseModel):
-            data = await request.json(loads=JSONDecoder().decode)
-            if isinstance(data, (str, bytes, bytearray)):
-                data = json.loads(data, object_hook=parse_json_or_none)
-            args_to_apply[name] = type_(**data)
-        elif issubclass(type_, FileField):
-            args_to_apply[name] = await request.post()
-        else:
-            continue
-    return args_to_apply
 
 
 class Api(Application):
     """
 
     Api class to create a fastapi-like api.
 
     """
-    
-    @property
-    def state(self) -> Dict[str,EventSourceResponse]:
-        return {}
-    
-    async def set_state(self, key: str, value: EventSourceResponse) -> None:
-        if key in self.state:
-            self.state[key] = value
-        else:
-            self.state.update({key:value})
-
-    title: str = "aiofauna"
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, title: str = "AioFauna API", **kwargs):
         super().__init__(*args, **kwargs)
+        self.title = title
         self.openapi = {
             "openapi": "3.0.0",
-            "info": {"title": "API", "version": "1.0.0"},
+            "info": {"title": self.title, "version": "1.0.0"},
             "paths": {},
             "components": {"schemas": {}},
+            "description": "AioFauna API",
         }
         self._route_open_api_params = {}
 
         @self.get("/openapi.json")
         async def openapi():
             response = jsonable_encoder(self.openapi)
             return json_response(response)
@@ -478,65 +467,73 @@
 
             wrapper._handler = func
             return wrapper
 
         return decorator
 
     def get(self, path: str, **kwargs):
+        """GET decorator"""
         def decorator(func):
             self.router.add_get(path, self.document(path, "GET")(func), **kwargs)
             return func
 
         return decorator
 
     def post(self, path: str, **kwargs):
+        """POST decorator"""
         def decorator(func):
             self.router.add_post(path, self.document(path, "POST")(func), **kwargs)
             return func
 
         return decorator
 
     def put(self, path: str, **kwargs):
+        """PUT decorator"""
         def decorator(func):
             self.router.add_put(path, self.document(path, "PUT")(func), **kwargs)
             return func
 
         return decorator
 
     def delete(self, path: str, **kwargs):
+        """DELETE decorator"""
         def decorator(func):
             self.router.add_delete(path, self.document(path, "DELETE")(func), **kwargs)
             return func
 
         return decorator
 
     def patch(self, path: str, **kwargs):
+        """PATCH decorator"""
         def decorator(func):
             self.router.add_patch(path, self.document(path, "PATCH")(func), **kwargs)
             return func
 
         return decorator
 
     def head(self, path: str, **kwargs):
+        """HEAD decorator"""
         def decorator(func):
             self.router.add_head(path, self.document(path, "HEAD")(func), **kwargs)
             return func
 
         return decorator
 
     def options(self, path: str, **kwargs):
+        """OPTIONS decorator"""
         def decorator(func):
             self.router.add_options(
                 path, self.document(path, "OPTIONS")(func), **kwargs
             )
             return func
 
         return decorator
 
     def on_event(self, event: str):
+        """On event handler"""
         def decorator(func):
             if event not in ["startup", "shutdown"]:
                 raise ValueError("Event must be startup or shutdown")
             elif event == "startup":
                 self.on_startup.append(func)
             else:
                 self.on_shutdown.append(func)
```

### Comparing `aiofauna-0.1.7/aiofauna/asgi.py` & `aiofauna-0.1.8/aiofauna/asgi.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.7/aiofauna/client.py` & `aiofauna-0.1.8/aiofauna/client.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.7/aiofauna/datastructures.py` & `aiofauna-0.1.8/aiofauna/datastructures.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.7/aiofauna/errors.py` & `aiofauna-0.1.8/aiofauna/errors.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.7/aiofauna/helpers.py` & `aiofauna-0.1.8/aiofauna/helpers.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.7/aiofauna/json.py` & `aiofauna-0.1.8/aiofauna/json.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.7/aiofauna/objects.py` & `aiofauna-0.1.8/aiofauna/objects.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.7/aiofauna/odm.py` & `aiofauna-0.1.8/aiofauna/odm.py`

 * *Files 27% similar despite different names*

```diff
@@ -191,17 +191,15 @@
 
         except AioFaunaException as exc:
             logging.error(exc)
 
             return False
 
     @classmethod
-    async def find_unique(
-        cls, field: str, value: Any
-    ) -> AsyncFaunaModel:
+    async def find_unique(cls, field: str, value: Any) -> AsyncFaunaModel:
         """
 
 
         Finds a document in FaunaDB by a unique field.
 
 
 
@@ -241,15 +239,15 @@
                     "ts": data["ts"] / 1000,
                 }
             )
 
         except AioFaunaException as exc:
             logging.error(exc)
 
-            return None # type: ignore # pylint: disable=unreachable
+            return None  # type: ignore # pylint: disable=unreachable
 
     @classmethod
     async def find_many(cls, field: str, value: Any) -> List[AsyncFaunaModel]:
         """
 
 
         Finds documents in FaunaDB by a field.
@@ -352,15 +350,15 @@
                     "ts": data["ts"] / 1000,
                 }
             )
 
         except AioFaunaException as exc:
             logging.error(exc)
 
-            return None # type: ignore # pylint: disable=unreachable
+            return None  # type: ignore # pylint: disable=unreachable
 
     @classmethod
     async def all(cls) -> List[AsyncFaunaModel]:
         """
 
 
         Finds all documents of the model in FaunaDB.
@@ -518,15 +516,15 @@
             self.ref = data["ref"]["@ref"]["id"]
             self.ts = data["ts"] / 1000
             return self
 
         except AioFaunaException as exc:
             logging.error(exc)
 
-            return None # type: ignore # pylint: disable=unreachable
+            return None  # type: ignore # pylint: disable=unreachable
 
     @classmethod
     async def query(cls, query: str) -> List[AsyncFaunaModel]:
         """
 
 
         Queries FaunaDB using a string query and returns a list of instances of the model.
@@ -603,7 +601,148 @@
 
             An instance of the model if saved successfully, None otherwise.
         """
 
         if isinstance(self.ref, str) and len(self.ref) == 18:
             return await self.update(self.ref, kwargs=self.dict())
         return await self.create()
+
+
+    @classmethod
+    def gen_ts(cls):
+        '''Health check endpoint'''
+        schema = cls.schema()
+        ts_config = {}
+        for name_, field in schema["properties"].items():
+            if field.get("type") in ["string", "number", "boolean", "integer", "null"]:    
+                ts_config[name_] = field.get("type") if name_ in schema["required"] else f"{field['type']} | undefined"
+            elif field.get("type") == "array":
+                if field.get("items").get("type") in ["string", "number", "boolean", "integer", "null"]:
+                    ts_config[name_] = f"{field.get('items').get('type')}[]" if name_ in schema["required"] else f"{field.get('items').get('type')}[] | undefined"
+                elif field.get("items").get("$ref"):
+                    ts_config[name_] = f"{field.get('items').get('$ref').split('/')[-1]}[]" if name_ in schema["required"] else f"{field.get('items').get('$ref').split('/')[-1]}[] | undefined"
+                elif field.get("items").get("object"):
+                    ts_config[name_] = f"{field.get('items').get('title')}[]" if name_ in schema["required"] else f"{field.get('items').get('title')}[] | undefined"
+            elif field.get("type") == "object":
+                ts_config[name_] = field.get("title") if name_ in schema["required"] else f"{field.get('title')} | undefined"
+            elif field.get("$ref"):
+                ts_config[name_] = field.get("$ref").split('/')[-1] if name_ in schema["required"] else f"{field.get('$ref').split('/')[-1]} | undefined"
+            elif field.get("object"):   
+                ts_config[name_] = field.get("title") if name_ in schema["required"] else f"{field.get('title')} | undefined"
+            elif field.get("oneOf"):
+                ts_config[name_] = " | ".join([f"{x.get('$ref').split('/')[-1]}" if x.get("$ref") else f"{x.get('title')}" for x in field.get("oneOf")])
+            elif field.get("anyOf"):
+                ts_config[name_] = " | ".join([f"{x.get('$ref').split('/')[-1]}" if x.get("$ref") else f"{x.get('title')}" for x in field.get("anyOf")])
+            elif field.get("allOf"):
+                ts_config[name_] = " & ".join([f"{x.get('$ref').split('/')[-1]}" if x.get("$ref") else f"{x.get('title')}" for x in field.get("allOf")])
+            elif field.get("not"):
+                ts_config[name_] = f"!{field.get('not').get('$ref').split('/')[-1]}" if field.get("not").get("$ref") else f"!{field.get('not').get('title')}"
+            elif field.get("enum"):
+                ts_config[name_] = " | ".join([f"{x}" for x in field.get("enum")])
+            else:
+                ts_config[name_] = "any"
+                
+        ts_type = f"type {cls.__name__} = {ts_config}"
+        
+        return ts_type.replace("'", '')
+    
+
+    @classmethod
+    def gen_store(cls):
+        return f"""
+        import {cls.__name__} from '~/types/{cls.__name__.lower()}'
+        import {{ defineStore, acceptHMRUpdate }} from 'pinia'
+        
+        export const {cls.__name__}Store = defineStore('{cls.__name__.lower()}', () => {{
+            const state = reactive({{
+                {cls.__name__.lower()}s: [] as {cls.__name__}[],
+                {cls.__name__.lower()}: null as {cls.__name__} | null,
+                loading: false,
+                error: null as string | null,
+                notifications: [] as {{message: string, status: 'success' | 'error' | 'warning' | 'info'}}[]
+            }})
+            
+            const api = {{
+                async fetch{cls.__name__}s() {{  
+                    state.loading = true
+                    try {{
+                        const {{ data }} =  await useFetch("/api/{cls.__name__.lower()}s").json()
+                        state.{cls.__name__.lower()}s = unref(data)
+                    }} catch (error) {{
+                        state.error = error.message
+                    }} finally {{
+                        state.loading = false
+                    }}
+                }},
+                async fetch{cls.__name__}(id: string) {{
+                    state.loading = true
+                    try {{
+                        const {{ data }} =  await useFetch("/api/{cls.__name__.lower()}s/" + id).json()
+                        state.{cls.__name__.lower()} = unref(data)
+                    }} catch (error) {{
+                        state.error = error.message
+                    }} finally {{
+                        state.loading = false
+                    }}
+                }},
+                async create{cls.__name__}({cls.__name__.lower()}: {cls.__name__}) {{
+                    state.loading = true
+                    try {{
+                        const {{ data }} =  await useFetch("/api/{cls.__name__.lower()}s", {{
+                            method: "POST",
+                            headers: {{
+                                "Content-Type": "application/json"
+                            }},
+                            body: JSON.stringify({cls.__name__.lower()})
+                        }}).json()
+                        state.{cls.__name__.lower()} = unref(data)
+                    }} catch (error) {{
+                        state.error = error.message
+                    }} finally {{
+                        state.loading = false
+                    }}
+                }},
+                async update{cls.__name__}({cls.__name__.lower()}: {cls.__name__}) {{
+                    state.loading = true
+                    try {{
+                        const {{ data }} =  await useFetch("/api/{cls.__name__.lower()}s/" + {cls.__name__.lower()}.ref, {{
+                            method: "PUT",
+                            headers: {{
+                                "Content-Type": "application/json"
+                            }},
+                            body: JSON.stringify({cls.__name__.lower()})
+                        }}).json()
+                        state.{cls.__name__.lower()} = unref(data)
+                    }} catch (error) {{
+                        state.error = error.message
+                    }} finally {{
+                        state.loading = false
+                    }}
+                }},
+                async delete{cls.__name__}({cls.__name__.lower()}: {cls.__name__}) {{
+                    state.loading = true
+                    try {{
+                        const {{ data }} =  await useFetch("/api/{cls.__name__.lower()}s/" + {cls.__name__.lower()}.ref, {{
+                            method: "DELETE"
+                        }}).json()
+                        state.{cls.__name__.lower()} = unref(data)
+                    }} catch (error) {{
+                        state.error = error.message
+                    }} finally {{
+                        state.loading = false
+                    }}
+                }}
+            }}
+
+        
+            return {{
+                state,
+                api
+            }}
+        }})
+        
+        if (import.meta.hot) {{
+            import.meta.hot.accept(acceptHMRUpdate({cls.__name__}Store, import.meta.hot))
+        }}
+        """
+            
+
```

### Comparing `aiofauna-0.1.7/aiofauna/page.py` & `aiofauna-0.1.8/aiofauna/page.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.7/aiofauna/query.py` & `aiofauna-0.1.8/aiofauna/query.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.7/pyproject.toml` & `aiofauna-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiofauna"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Oscar Bahamonde <oscar.bahamonde.dev@gmail.com>"]
 repository = "https://github.com/obahamonde/aiofauna"
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `aiofauna-0.1.7/setup.py` & `aiofauna-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'aiohttp>=3.8.4,<4.0.0',
  'aiohttp_cors>=0.7.0,<0.8.0',
  'iso8601>=1.1.0,<2.0.0',
  'pydantic[dotenv]>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'aiofauna',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': '',
     'long_description': '---\ntitle: AioFauna\n---\n# AioFauna\n\n🚀 Introducing aiofauna: A full-stack framework built on top of Aiohttp, Pydantic and FaunaDB.\n\n🔥 Inspired by FastAPI focuses on Developer Experience, Productivity and Versatility.\n\n🌟 Features:\n\n✅ Supports Python 3.7+, comes with an opinionated ODM (Object Document Mapper) out of the box for FaunaDB that abstracts out complex FQL expressions into pythonic, fully typed asynchronous methods for all CRUD operations.\n\n✅ Performant and scalable: Built on top of Aiohttp a powerful http server and client and FaunaDB an scalable serverless database for modern applications.\n\n✅ Async/await coroutines: Leverage the power of async programming for enhanced performance and responsiveness, being ASGI compliant is compatible with most async python frameworks.\n\n✅ Automatic Swagger UI generation: Automatic generation of interactive Swagger UI documentation for instant testing of your API.\n\n✅ SSE (Server Sent Events): Built-in support for SSE (Server Sent Events) for real-time streaming of data from FaunaDB to your application.\n\n✅ Robust data validation: Built-in support for Pydantic models for robust data validation and serialization.\n\n✅ Auto-provisioning: Automatic management of indexes, unique indexes, and collections with FaunaModel ODM.\n\n✅ Full JSON communication: Custom encoder to ensure seamless data exchange between your application and FaunaDB backend.\n\n✅ Markdown and Jinja support with live reload: experiment an smooth frontend devserver experience without leaving your backend code.\n\n✅ Inspired by fastapi, you will work with almost the same syntax and features like path operations, path parameters, query parameters, request body, status codes and more.\n\n💡 With aiofauna, you can build fast, scalable, and reliable modern applications, while building seamless integrations thanks to the fastest http client aiohttp and the most versatile database FaunaDB, you will enjoy integrating with third party services such as APIs, Data Sources and Cloud Services.\n\n📚 Check out the aiofauna library, and start building your next-gen applications today! 🚀\n\n#Python #FaunaDB #Async #Pydantic #aiofauna\n\n⚙️ If you are using a synchronous framework check out [Faudantic](https://github.com/obahamonde/faudantic) for a similar experience with FaunaDB and Pydantic.\n\n📚 [Documentation](https://obahamonde-aiofauna-docs.smartpro.solutions) (Built with aiofauna)\n\n📦 [PyPi](https://pypi.org/project/aiofauna/)\n\n📦 [GitHub](https://github.com/obahamonde/aiofauna)\n\n📦 [Demo](https://aiofaunastreams-fwuw7gz7oq-uc.a.run.app/) (Real time Latency Monitoring between FaunaDB and Google Cloud Run)\n',
     'author': 'Oscar Bahamonde',
     'author_email': 'oscar.bahamonde.dev@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/obahamonde/aiofauna',
```

### Comparing `aiofauna-0.1.7/PKG-INFO` & `aiofauna-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiofauna
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Home-page: https://github.com/obahamonde/aiofauna
 License: MIT
 Author: Oscar Bahamonde
 Author-email: oscar.bahamonde.dev@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

