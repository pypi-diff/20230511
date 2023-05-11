# Comparing `tmp/metal_sdk-1.0.1.tar.gz` & `tmp/metal_sdk-1.0.2.tar.gz`

## Comparing `metal_sdk-1.0.1.tar` & `metal_sdk-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/examples/example.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/examples/example_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/src/metal_sdk/__init__.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/src/metal_sdk/metal.py
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/src/metal_sdk/metal_async.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/src/metal_sdk/typings.py
--rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/tests/test_metal.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/tests/test_metal_async.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/.gitignore
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/LICENSE
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/examples/example.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/examples/example_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/src/metal_sdk/__init__.py
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/src/metal_sdk/metal.py
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/src/metal_sdk/metal_async.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/src/metal_sdk/typings.py
+-rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/tests/test_metal.py
+-rw-r--r--   0        0        0     7180 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/tests/test_metal_async.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/.gitignore
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/LICENSE
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.2/PKG-INFO
```

### Comparing `metal_sdk-1.0.1/.github/workflows/publish.yml` & `metal_sdk-1.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.1/.github/workflows/test.yml` & `metal_sdk-1.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.1/examples/example.py` & `metal_sdk-1.0.2/examples/example.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.1/examples/example_async.py` & `metal_sdk-1.0.2/examples/example_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.1/src/metal_sdk/metal.py` & `metal_sdk-1.0.2/src/metal_sdk/metal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import httpx
-from .typings import IndexPayload, SearchPayload, TunePayload
+from typing import List
+from .typings import IndexPayload, SearchPayload, TunePayload, BulkIndexItem
 
 
 BASE_API = "https://api.getmetal.io"
 
 
 class Metal(httpx.Client):
     api_key: str
@@ -65,14 +66,22 @@
         data = self.__getData(index, payload)
         url = "/v1/index"
 
         res = self.request("post", url, json=data)
         res.raise_for_status()
         return res.json()
 
+    def index_many(self, payload: List[BulkIndexItem]):
+        url = "/v1/index/bulk"
+        data = {"data": payload}
+
+        res = self.request("post", url, json=data)
+        res.raise_for_status()
+        return res.json()
+
     def search(
         self, payload: SearchPayload = {}, index_id=None, ids_only=False, limit=1
     ):
         index = index_id or self.index_id
         self.__validateIndexAndSearch(index, payload)
         data = self.__getData(index, payload)
 
@@ -120,7 +129,17 @@
             raise TypeError("id required")
 
         url = "/v1/documents/" + id
 
         res = self.request("delete", url)
         res.raise_for_status()
         return res.json()
+
+    def delete_many(self, ids: List[str], index_id=None):
+        if ids is None:
+            raise TypeError("ids required")
+
+        url = "/v1/documents/bulk"
+
+        res = self.request("delete", url, json={"ids": ids})
+        res.raise_for_status()
+        return res.json()
```

### Comparing `metal_sdk-1.0.1/src/metal_sdk/metal_async.py` & `metal_sdk-1.0.2/src/metal_sdk/metal_async.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from typing import List
 import httpx
-from .typings import IndexPayload, SearchPayload, TunePayload
+from .typings import IndexPayload, SearchPayload, TunePayload, BulkIndexItem
 
 
 BASE_API = "https://api.getmetal.io"
 
 
 class Metal(httpx.AsyncClient):
     api_key: str
@@ -65,14 +66,22 @@
         data = self.__getData(index, payload)
         url = "/v1/index"
 
         res = await self.request("post", url, json=data)
         res.raise_for_status()
         return res.json()
 
+    async def index_many(self, payload: List[BulkIndexItem]):
+        url = "/v1/index/bulk"
+        data = {"data": payload}
+        res = await self.request("post", url, json=data)
+
+        res.raise_for_status()
+        return res.json()
+
     async def search(
         self, payload: SearchPayload = {}, index_id=None, ids_only=False, limit=1
     ):
         index = index_id or self.index_id
         self.__validateIndexAndSearch(index, payload)
         data = self.__getData(index, payload)
 
@@ -120,7 +129,17 @@
             raise TypeError("id required")
 
         url = "/v1/documents/" + id
 
         res = await self.request("delete", url)
         res.raise_for_status()
         return res.json()
+
+    async def delete_many(self, ids: List[str]):
+        if ids is None:
+            raise TypeError("ids required")
+
+        url = "/v1/documents/bulk"
+
+        res = await self.request("delete", url, json={"ids": ids})
+        res.raise_for_status()
+        return res.json()
```

### Comparing `metal_sdk-1.0.1/src/metal_sdk/typings.py` & `metal_sdk-1.0.2/src/metal_sdk/typings.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,28 @@
     imageBase64: NotRequired[str]
     imageUrl: NotRequired[str]
     text: NotRequired[str]
     embedding: NotRequired[List[float]]
     metadata: NotRequired[dict]
 
 
+class BulkIndexItem(TypedDict):
+    id: NotRequired[str]
+    index: str
+    imageBase64: NotRequired[str]
+    imageUrl: NotRequired[str]
+    text: NotRequired[str]
+    embedding: NotRequired[List[float]]
+    metadata: NotRequired[dict]
+
+
+class BulkIndexPayload(TypedDict):
+    data: List[BulkIndexItem]
+
+
 class SearchFilter(TypedDict):
     field: str
     value: str | int | float
 
 
 class SearchPayload(TypedDict):
     imageBase64: NotRequired[str]
```

### Comparing `metal_sdk-1.0.1/tests/test_metal.py` & `metal_sdk-1.0.2/tests/test_metal.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,23 +38,37 @@
         payload = {"id": mock_id, "text": mock_text, "metadata": mock_metadata}
 
         metal = Metal(API_KEY, CLIENT_ID, my_index)
         metal.request = mock.MagicMock(return_value=mock.Mock(status_code=201))
         metal.index(payload)
 
         self.assertEqual(metal.request.call_count, 1)
-        self.assertEqual(
-            metal.request.call_args[0][0], "post"
-        )
-        self.assertEqual(
-            metal.request.call_args[0][1], "/v1/index"
-        )
+        self.assertEqual(metal.request.call_args[0][0], "post")
+        self.assertEqual(metal.request.call_args[0][1], "/v1/index")
         self.assertEqual(metal.request.call_args[1]["json"]["index"], my_index)
         self.assertEqual(metal.request.call_args[1]["json"]["text"], payload["text"])
-        self.assertEqual(metal.request.call_args[1]["json"]["metadata"], payload["metadata"])
+        self.assertEqual(
+            metal.request.call_args[1]["json"]["metadata"], payload["metadata"]
+        )
+
+    def test_metal_index_many_with_text(self):
+        my_index = "my-index"
+        mock_text = "some text"
+        mock_id = "some-id"
+        mock_metadata = {"some": "metadata"}
+        payload = [{"id": mock_id, "text": mock_text, "metadata": mock_metadata, "index": my_index}]
+
+        metal = Metal(API_KEY, CLIENT_ID, my_index)
+        metal.request = mock.MagicMock(return_value=mock.Mock(status_code=201))
+        metal.index_many(payload)
+
+        self.assertEqual(metal.request.call_count, 1)
+        self.assertEqual(metal.request.call_args[0][0], "post")
+        self.assertEqual(metal.request.call_args[0][1], "/v1/index/bulk")
+        self.assertEqual(metal.request.call_args[1]["json"]["data"], payload)
 
     def test_metal_search_without_index(self):
         metal = Metal(API_KEY, CLIENT_ID)
         with self.assertRaises(TypeError) as ctx:
             metal.search()
         self.assertEqual(str(ctx.exception), "index_id required")
 
@@ -66,15 +80,18 @@
             metal.search()
         self.assertEqual(
             str(ctx.exception), "imageBase64, imageUrl, text, or embedding required"
         )
 
     def test_metal_search_with_text(self):
         my_index = "my-index"
-        payload = {"text": "some text", "filters": [{"field": "number_of_the_beast", "value": 666}]}
+        payload = {
+            "text": "some text",
+            "filters": [{"field": "number_of_the_beast", "value": 666}],
+        }
 
         metal = Metal(API_KEY, CLIENT_ID, my_index)
 
         metal.request = mock.MagicMock(return_value=mock.Mock(status_code=201))
 
         metal.search(payload, ids_only=True)
 
@@ -85,15 +102,17 @@
         )
         self.assertEqual(
             metal.request.call_args[0][1],
             "/v1/search?limit=1&idsOnly=true",
         )
         self.assertEqual(metal.request.call_args[1]["json"]["index"], my_index)
         self.assertEqual(metal.request.call_args[1]["json"]["text"], payload["text"])
-        self.assertEqual(metal.request.call_args[1]["json"]["filters"], payload["filters"])
+        self.assertEqual(
+            metal.request.call_args[1]["json"]["filters"], payload["filters"]
+        )
 
     def test_metal_tune_without_index(self):
         metal = Metal(API_KEY, CLIENT_ID)
         with self.assertRaises(TypeError) as ctx:
             metal.tune()
         self.assertEqual(str(ctx.exception), "index_id required")
 
@@ -104,15 +123,17 @@
             metal.tune()
         self.assertEqual(str(ctx.exception), "idA, idB, and label required")
 
     def test_metal_tune_with_payload(self):
         index_id = "index-id"
         payload = {"idA": "id-a", "idB": "id-b", "label": -1}
         metal = Metal(API_KEY, CLIENT_ID, index_id)
-        return_value = mock.MagicMock(json=lambda: {"status": "success", "message": "ok"})
+        return_value = mock.MagicMock(
+            json=lambda: {"status": "success", "message": "ok"}
+        )
         metal.request = mock.MagicMock(return_value=return_value)
 
         metal.tune(payload)
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "post")
         self.assertEqual(metal.request.call_args[0][1], "/v1/tune")
         self.assertEqual(metal.request.call_args[1]["json"]["index"], index_id)
@@ -136,10 +157,25 @@
         index_id = "index-id"
         id = "ozzy"
         metal = Metal(API_KEY, CLIENT_ID, index_id)
         return_value = mock.MagicMock(json=lambda: {"ozzy": "black sabbath"})
         metal.request = mock.MagicMock(return_value=return_value)
 
         metal.delete_one(id)
+
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "delete")
         self.assertEqual(metal.request.call_args[0][1], "/v1/documents/ozzy")
+
+    def test_metal_delete_many_with_payload(self):
+        index_id = "index-id"
+        id = "ozzy"
+        metal = Metal(API_KEY, CLIENT_ID, index_id)
+        return_value = mock.MagicMock(json=lambda: {"ozzy": "black sabbath"})
+        metal.request = mock.MagicMock(return_value=return_value)
+
+        metal.delete_many([id])
+
+        self.assertEqual(metal.request.call_count, 1)
+        self.assertEqual(metal.request.call_args[0][0], "delete")
+        self.assertEqual(metal.request.call_args[0][1], "/v1/documents/bulk")
+        self.assertEqual(metal.request.call_args[1]["json"]["ids"], [id])
```

### Comparing `metal_sdk-1.0.1/tests/test_metal_async.py` & `metal_sdk-1.0.2/tests/test_metal_async.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,14 +49,35 @@
         self.assertEqual(
             metal.request.call_args[0][1], "/v1/index"
         )
         self.assertEqual(metal.request.call_args[1]["json"]["index"], my_index)
         self.assertEqual(metal.request.call_args[1]["json"]["text"], payload["text"])
         self.assertEqual(metal.request.call_args[1]["json"]["metadata"], payload["metadata"])
 
+    async def test_metal_index_many_with_text(self):
+        my_index = "my-index"
+        mock_text = "some text"
+        mock_id = "some-id"
+        mock_metadata = {"some": "metadata"}
+
+        payload = [{"id": mock_id, "text": mock_text, "metadata": mock_metadata, "index": my_index}]
+
+        metal = Metal(API_KEY, CLIENT_ID, my_index)
+        metal.request = mock.MagicMock(return_value=mock.Mock(status_code=201))
+        await metal.index_many(payload)
+
+        self.assertEqual(metal.request.call_count, 1)
+        self.assertEqual(
+            metal.request.call_args[0][0], "post"
+        )
+        self.assertEqual(
+            metal.request.call_args[0][1], "/v1/index/bulk"
+        )
+        self.assertEqual(metal.request.call_args[1]["json"]["data"], payload)
+
     async def test_metal_search_without_index(self):
         metal = Metal(API_KEY, CLIENT_ID)
         with self.assertRaises(TypeError) as ctx:
             await metal.search()
         self.assertEqual(str(ctx.exception), "index_id required")
 
     async def test_metal_search_without_payload(self):
@@ -139,7 +160,21 @@
         return_value = mock.MagicMock(json=lambda: {"band": "Megadeth"})
         metal.request = mock.MagicMock(return_value=return_value)
 
         await metal.get_one(id)
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "delete")
         self.assertEqual(metal.request.call_args[0][1], "/v1/documents/dave")
+
+    async def test_metal_delete_many_with_payload(self):
+        index_id = "index-id"
+        id = "ozzy"
+        metal = Metal(API_KEY, CLIENT_ID, index_id)
+        return_value = mock.MagicMock(json=lambda: {"ozzy": "black sabbath"})
+        metal.request = mock.MagicMock(return_value=return_value)
+
+        await metal.delete_many([id])
+
+        self.assertEqual(metal.request.call_count, 1)
+        self.assertEqual(metal.request.call_args[0][0], "delete")
+        self.assertEqual(metal.request.call_args[0][1], "/v1/documents/bulk")
+        self.assertEqual(metal.request.call_args[1]["json"]["ids"], [id])
```

### Comparing `metal_sdk-1.0.1/.gitignore` & `metal_sdk-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.1/LICENSE` & `metal_sdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.1/README.md` & `metal_sdk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.1/pyproject.toml` & `metal_sdk-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metal_sdk"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Metal Technologies Inc", email="james@getmetal.io" },
 ]
 description = "SDK for getmetal.io"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `metal_sdk-1.0.1/PKG-INFO` & `metal_sdk-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metal_sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: SDK for getmetal.io
 Project-URL: Github, https://github.com/getmetal/metal-python
 Author-email: Metal Technologies Inc <james@getmetal.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

