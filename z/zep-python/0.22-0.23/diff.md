# Comparing `tmp/zep_python-0.22.tar.gz` & `tmp/zep_python-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-0.22.tar", max compression
+gzip compressed data, was "zep_python-0.23.tar", max compression
```

## Comparing `zep_python-0.22.tar` & `zep_python-0.23.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-05-10 04:23:10.066776 zep_python-0.22/LICENSE
--rw-r--r--   0        0        0    10560 2023-05-10 04:23:10.066776 zep_python-0.22/README.md
--rw-r--r--   0        0        0      621 2023-05-10 04:23:10.066776 zep_python-0.22/pyproject.toml
--rw-r--r--   0        0        0      282 2023-05-10 04:23:10.066776 zep_python-0.22/zep_python/__init__.py
--rw-r--r--   0        0        0     1236 2023-05-10 04:23:10.066776 zep_python-0.22/zep_python/exceptions.py
--rw-r--r--   0        0        0     6823 2023-05-10 04:23:10.066776 zep_python-0.22/zep_python/models.py
--rw-r--r--   0        0        0        0 2023-05-10 04:23:10.066776 zep_python-0.22/zep_python/py.typed
--rw-r--r--   0        0        0      670 2023-05-10 04:23:10.066776 zep_python-0.22/zep_python/utils.py
--rw-r--r--   0        0        0    10971 2023-05-10 04:23:10.066776 zep_python-0.22/zep_python/zep_client.py
--rw-r--r--   0        0        0    11188 1970-01-01 00:00:00.000000 zep_python-0.22/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-10 23:55:26.241521 zep_python-0.23/LICENSE
+-rw-r--r--   0        0        0    11193 2023-05-10 23:55:26.241521 zep_python-0.23/README.md
+-rw-r--r--   0        0        0      630 2023-05-10 23:55:26.245521 zep_python-0.23/pyproject.toml
+-rw-r--r--   0        0        0      339 2023-05-10 23:55:26.245521 zep_python-0.23/zep_python/__init__.py
+-rw-r--r--   0        0        0     1236 2023-05-10 23:55:26.245521 zep_python-0.23/zep_python/exceptions.py
+-rw-r--r--   0        0        0     6840 2023-05-10 23:55:26.245521 zep_python-0.23/zep_python/models.py
+-rw-r--r--   0        0        0        0 2023-05-10 23:55:26.245521 zep_python-0.23/zep_python/py.typed
+-rw-r--r--   0        0        0      670 2023-05-10 23:55:26.245521 zep_python-0.23/zep_python/utils.py
+-rw-r--r--   0        0        0    11069 2023-05-10 23:55:26.245521 zep_python-0.23/zep_python/zep_client.py
+-rw-r--r--   0        0        0    11830 1970-01-01 00:00:00.000000 zep_python-0.23/PKG-INFO
```

### Comparing `zep_python-0.22/LICENSE` & `zep_python-0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-0.22/README.md` & `zep_python-0.23/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,40 +61,38 @@
 Zep Python has both an async and sync API. We've provided code examples for the async API, but theyre easily enough modified for sync usage.
 
 **Class Attributes**
 
 - `base_url` (str): The base URL of the API.
 - `client` (httpx.AsyncClient): The HTTP client used for making API requests.
 
-**Methods**
+## Methods
 
 - `get_memory(session_id: str, lastn: Optional[int] = None) -> List[Memory]`: Retrieve memory for the specified session.
 - `add_memory(session_id: str, memory_messages: Memory) -> str`: Add memory to the specified session.
 - `delete_memory(session_id: str) -> str`: Delete memory for the specified session.
 - `search_memory(session_id: str, search_payload: SearchPayload, limit: Optional[int] = None) -> List[SearchResult]`: Search memory for the specified session.
 - `close() -> None`: Close the HTTP client.
 
-### `__init__(self, base_url: str) -> None`
-
-Initialize the ZepClient with the specified base URL.
+### Init
+- `__init__(self, base_url: str) -> None` : Initialize the ZepClient with the specified base URL.
 
 **Parameters**
-
 - `base_url` (str): The base URL of the API.
 
 ```python
 base_url = "http://localhost:8000"  # TODO: Replace with your Zep API URL
 async with ZepClient(base_url) as client:
     # ...
 ```
 
 ---
 
-### `get_memory(self, session_id: str, lastn: Optional[int] = None) -> List[Memory]`
-
+### get_memory
+- `get_memory(self, session_id: str, lastn: Optional[int] = None) -> List[Memory]`  
 Retrieve memory for the specified session. This method is a synchronous wrapper for the asynchronous method `aget_memory`.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session for which to retrieve memory.
 - `lastn` (Optional[int], optional): The number of most recent memory entries to retrieve. Defaults to None (all entries).
 
@@ -105,16 +103,16 @@
 **Raises**
 
 - `APIError`: If the API response format is unexpected.
 - `NotFoundError`: If no results were found.
 
 ---
 
-### `aget_memory(self, session_id: str, lastn: Optional[int] = None) -> List[Memory]`
-
+### aget_memory  
+- `aget_memory(self, session_id: str, lastn: Optional[int] = None) -> List[Memory]`  
 Asynchronously retrieve memory for the specified session.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session for which to retrieve memory.
 - `lastn` (Optional[int], optional): The number of most recent memory entries to retrieve. Defaults to None (all entries).
 
@@ -132,16 +130,16 @@
 for memory in memories:
     for message in memory.messages:
         print(message.to_dict())
 ```
 
 ---
 
-### `search_memory(self, session_id: str, search_payload: SearchPayload, limit: Optional[int] = None) -> List[SearchResult]`
-
+### search_memory  
+- `search_memory(self, session_id: str, search_payload: SearchPayload, limit: Optional[int] = None) -> List[SearchResult]`  
 Search memory for the specified session. This method is a synchronous wrapper for the asynchronous method `asearch_memory`.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session for which memory should be searched.
 - `search_payload` (SearchPayload): A SearchPayload object representing the search query.
 - `limit` (Optional[int], optional): The maximum number of search results to return. Defaults to None (no limit).
@@ -152,15 +150,16 @@
 
 **Raises**
 
 - `APIError`: If the API response format is unexpected.
 
 ---
 
-### `asearch_memory(self, session_id: str, search_payload: SearchPayload, limit: Optional[int] = None) -> List[SearchResult]`
+### asearch_memory  
+- `asearch_memory(self, session_id: str, search_payload: SearchPayload, limit: Optional[int] = None) -> List[SearchResult]`  
 
 Asynchronously search memory for the specified session.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session for which memory should be searched.
 - `search_payload` (SearchPayload): A SearchPayload object representing the search query.
@@ -181,15 +180,16 @@
     # Access the 'content' field within the 'message' object.
     message_content = search_result.message
     print(message_content)
 ```
 
 ---
 
-### `add_memory(self, session_id: str, memory_messages: Memory) -> str`
+### add_memory  
+- `add_memory(self, session_id: str, memory_messages: Memory) -> str`  
 
 Add memory to the specified session. This method is a synchronous wrapper for the asynchronous method `aadd_memory`.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session to which memory should be added.
 - `memory_messages` (Memory): A Memory object representing the memory messages to be added.
@@ -200,15 +200,16 @@
 
 **Raises**
 
 - `APIError`: If the API response format is unexpected.
 
 ---
 
-### `aadd_memory(self, session_id: str, memory_messages: Memory) -> str`
+### aadd_memory  
+- `aadd_memory(self, session_id: str, memory_messages: Memory) -> str`  
 
 Asynchronously add memory to the specified session.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session to which memory should be added.
 - `memory_messages` (Memory): A Memory object representing the memory messages to be added.
@@ -228,15 +229,16 @@
 memory.messages = [message]
 
 result = await client.aadd_memory(session_id, memory)
 ```
 
 ---
 
-### `delete_memory(self, session_id: str) -> str`
+### delete_memory  
+- `delete_memory(self, session_id: str) -> str`  
 
 Delete memory for the specified session. This method is a synchronous wrapper for the asynchronous method `adelete_memory`.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session for which memory should be deleted.
 
@@ -246,31 +248,33 @@
 
 **Raises**
 
 - `APIError`: If the API response format is unexpected.
 
 ---
 
-### `adelete_memory(self, session_id: str) -> str`
+### adelete_memory  
+- `adelete_memory(self, session_id: str) -> str`  
 
 Asynchronously delete memory for the specified session.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session for which memory should be deleted
 
 ```python
 result = await client.adelete_memory(session_id)
 ```
 
 ---
 
-### `close(self) -> None`
+### close  
+- `close(self) -> None`  
 
-Asynchronously close the HTTP client.
+Asynchronously close the HTTP client. This is Optional. 
 
 **Note**: This method may be called when the ZepClient is no longer needed to release resources.
 
 ## Models
 
 ### Memory
 
@@ -283,15 +287,15 @@
 - `summary` (Optional[Dict[str, Any]]): A dictionary containing a summary of the memory.
 - `uuid` (Optional[str]): A unique identifier for the memory.
 - `created_at` (Optional[str]): The timestamp when the memory was created.
 - `token_count` (Optional[int]): The token count of the memory.
 
 ---
 
-### `Message`
+### Message
 
 Represents a message in a conversation.
 
 **Attributes**:
 
 - `uuid` (Optional[str]): The unique identifier of the message.
 - `created_at` (Optional[str]): The timestamp of when the message was created.
@@ -301,15 +305,15 @@
 
 **Methods**:
 
 - `to_dict() -> Dict[str, Any]`: Returns a dictionary representation of the message.
 
 ---
 
-### `Summary`
+### Summary
 
 Represents a summary of a conversation.
 
 **Attributes**:
 
 - `uuid` (str): The unique identifier of the summary.
 - `created_at` (str): The timestamp of when the summary was created.
@@ -319,40 +323,64 @@
 
 **Methods**:
 
 - `to_dict() -> Dict[str, Any]`: Returns a dictionary representation of the summary.
 
 ---
 
-### `SearchPayload`
+### SearchPayload
 
 Represents a search payload for querying memory.
 
 **Attributes**:
 
 - `meta` (Dict[str, Any]): Metadata associated with the search query.
 - `text` (str): The text of the search query.
 
 ---
 
-### `SearchResult`
+### SearchResult
 
 Represents a search result from querying memory.
 
 **Attributes**:
 
 - `message` (Optional[Dict[str, Any]]): The message associated with the search result.
 - `meta` (Optional[Dict[str, Any]]): Metadata associated with the search result.
 - `score` (Optional[float]): The score of the search result.
 - `summary` (Optional[str]): The summary of the search result.
 - `dist` (Optional[float]): The distance metric of the search result.
 
 ---
+## Exceptions
 
-### `APIError`
+### APIError
 
 Represents an API error.
 
 **Attributes**:
 
 - `code` (int): The error code associated with the API error.
 - `message` (str): The error message associated with the API error.
+---
+
+### ZepClientError
+
+Base exception class for ZepClient errors.
+
+**Attributes**:
+
+- `message`: str - The error message associated with the ZepClient error.
+- `response_data`: Optional[dict] - The response data associated with the ZepClient error.
+---
+
+### NotFoundError
+
+Raised when the API response contains no results.
+
+Inherits from ZepClientError.
+
+**Attributes**:
+
+- `message`: str - The error message to be set for the exception.
+
+---
```

### Comparing `zep_python-0.22/pyproject.toml` & `zep_python-0.23/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "zep-python"
-version = "0.22"
-description = "Zep stores, manages, enriches, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
+version = "0.23"
+description = "Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.0"
```

### Comparing `zep_python-0.22/zep_python/exceptions.py` & `zep_python-0.23/zep_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.22/zep_python/models.py` & `zep_python-0.23/zep_python/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,17 +177,17 @@
     ----------
     meta : Dict[str, Any]
         Metadata associated with the search query.
     text : str
         The text of the search query.
     """
 
-    def __init__(self, meta: Dict[str, Any], text: str):
-        self.meta = meta
+    def __init__(self, text: str, meta: Optional[Dict[str, Any]] = None):
         self.text = text
+        self.meta = meta
 
 
 class SearchResult:
     """
     Represents a search result from querying memory.
 
     Attributes
```

### Comparing `zep_python-0.22/zep_python/utils.py` & `zep_python-0.23/zep_python/utils.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.22/zep_python/zep_client.py` & `zep_python-0.23/zep_python/zep_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,14 +325,16 @@
         """
         params = {"limit": limit} if limit is not None else {}
         response = await self.client.post(
             f"{self.base_url}{API_BASEURL}/sessions/{session_id}/search",
             json=search_payload.__dict__,
             params=params,
         )
+        if response.status_code == 404:
+            raise NotFoundError("No query results found")
         if response.status_code != 200:
             raise APIError(f"Unexpected status code: {response.status_code}")
         return [
             SearchResult(**search_result) for search_result in response.json()
         ]
 
     async def close(self) -> None:
```

### Comparing `zep_python-0.22/PKG-INFO` & `zep_python-0.23/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zep-python
-Version: 0.22
-Summary: Zep stores, manages, enriches, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service.
+Version: 0.23
+Summary: Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service.
 Author: Daniel Chalef
 Author-email: daniel.chalef@private.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -76,40 +76,38 @@
 Zep Python has both an async and sync API. We've provided code examples for the async API, but theyre easily enough modified for sync usage.
 
 **Class Attributes**
 
 - `base_url` (str): The base URL of the API.
 - `client` (httpx.AsyncClient): The HTTP client used for making API requests.
 
-**Methods**
+## Methods
 
 - `get_memory(session_id: str, lastn: Optional[int] = None) -> List[Memory]`: Retrieve memory for the specified session.
 - `add_memory(session_id: str, memory_messages: Memory) -> str`: Add memory to the specified session.
 - `delete_memory(session_id: str) -> str`: Delete memory for the specified session.
 - `search_memory(session_id: str, search_payload: SearchPayload, limit: Optional[int] = None) -> List[SearchResult]`: Search memory for the specified session.
 - `close() -> None`: Close the HTTP client.
 
-### `__init__(self, base_url: str) -> None`
-
-Initialize the ZepClient with the specified base URL.
+### Init
+- `__init__(self, base_url: str) -> None` : Initialize the ZepClient with the specified base URL.
 
 **Parameters**
-
 - `base_url` (str): The base URL of the API.
 
 ```python
 base_url = "http://localhost:8000"  # TODO: Replace with your Zep API URL
 async with ZepClient(base_url) as client:
     # ...
 ```
 
 ---
 
-### `get_memory(self, session_id: str, lastn: Optional[int] = None) -> List[Memory]`
-
+### get_memory
+- `get_memory(self, session_id: str, lastn: Optional[int] = None) -> List[Memory]`  
 Retrieve memory for the specified session. This method is a synchronous wrapper for the asynchronous method `aget_memory`.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session for which to retrieve memory.
 - `lastn` (Optional[int], optional): The number of most recent memory entries to retrieve. Defaults to None (all entries).
 
@@ -120,16 +118,16 @@
 **Raises**
 
 - `APIError`: If the API response format is unexpected.
 - `NotFoundError`: If no results were found.
 
 ---
 
-### `aget_memory(self, session_id: str, lastn: Optional[int] = None) -> List[Memory]`
-
+### aget_memory  
+- `aget_memory(self, session_id: str, lastn: Optional[int] = None) -> List[Memory]`  
 Asynchronously retrieve memory for the specified session.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session for which to retrieve memory.
 - `lastn` (Optional[int], optional): The number of most recent memory entries to retrieve. Defaults to None (all entries).
 
@@ -147,16 +145,16 @@
 for memory in memories:
     for message in memory.messages:
         print(message.to_dict())
 ```
 
 ---
 
-### `search_memory(self, session_id: str, search_payload: SearchPayload, limit: Optional[int] = None) -> List[SearchResult]`
-
+### search_memory  
+- `search_memory(self, session_id: str, search_payload: SearchPayload, limit: Optional[int] = None) -> List[SearchResult]`  
 Search memory for the specified session. This method is a synchronous wrapper for the asynchronous method `asearch_memory`.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session for which memory should be searched.
 - `search_payload` (SearchPayload): A SearchPayload object representing the search query.
 - `limit` (Optional[int], optional): The maximum number of search results to return. Defaults to None (no limit).
@@ -167,15 +165,16 @@
 
 **Raises**
 
 - `APIError`: If the API response format is unexpected.
 
 ---
 
-### `asearch_memory(self, session_id: str, search_payload: SearchPayload, limit: Optional[int] = None) -> List[SearchResult]`
+### asearch_memory  
+- `asearch_memory(self, session_id: str, search_payload: SearchPayload, limit: Optional[int] = None) -> List[SearchResult]`  
 
 Asynchronously search memory for the specified session.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session for which memory should be searched.
 - `search_payload` (SearchPayload): A SearchPayload object representing the search query.
@@ -196,15 +195,16 @@
     # Access the 'content' field within the 'message' object.
     message_content = search_result.message
     print(message_content)
 ```
 
 ---
 
-### `add_memory(self, session_id: str, memory_messages: Memory) -> str`
+### add_memory  
+- `add_memory(self, session_id: str, memory_messages: Memory) -> str`  
 
 Add memory to the specified session. This method is a synchronous wrapper for the asynchronous method `aadd_memory`.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session to which memory should be added.
 - `memory_messages` (Memory): A Memory object representing the memory messages to be added.
@@ -215,15 +215,16 @@
 
 **Raises**
 
 - `APIError`: If the API response format is unexpected.
 
 ---
 
-### `aadd_memory(self, session_id: str, memory_messages: Memory) -> str`
+### aadd_memory  
+- `aadd_memory(self, session_id: str, memory_messages: Memory) -> str`  
 
 Asynchronously add memory to the specified session.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session to which memory should be added.
 - `memory_messages` (Memory): A Memory object representing the memory messages to be added.
@@ -243,15 +244,16 @@
 memory.messages = [message]
 
 result = await client.aadd_memory(session_id, memory)
 ```
 
 ---
 
-### `delete_memory(self, session_id: str) -> str`
+### delete_memory  
+- `delete_memory(self, session_id: str) -> str`  
 
 Delete memory for the specified session. This method is a synchronous wrapper for the asynchronous method `adelete_memory`.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session for which memory should be deleted.
 
@@ -261,31 +263,33 @@
 
 **Raises**
 
 - `APIError`: If the API response format is unexpected.
 
 ---
 
-### `adelete_memory(self, session_id: str) -> str`
+### adelete_memory  
+- `adelete_memory(self, session_id: str) -> str`  
 
 Asynchronously delete memory for the specified session.
 
 **Parameters**
 
 - `session_id` (str): The ID of the session for which memory should be deleted
 
 ```python
 result = await client.adelete_memory(session_id)
 ```
 
 ---
 
-### `close(self) -> None`
+### close  
+- `close(self) -> None`  
 
-Asynchronously close the HTTP client.
+Asynchronously close the HTTP client. This is Optional. 
 
 **Note**: This method may be called when the ZepClient is no longer needed to release resources.
 
 ## Models
 
 ### Memory
 
@@ -298,15 +302,15 @@
 - `summary` (Optional[Dict[str, Any]]): A dictionary containing a summary of the memory.
 - `uuid` (Optional[str]): A unique identifier for the memory.
 - `created_at` (Optional[str]): The timestamp when the memory was created.
 - `token_count` (Optional[int]): The token count of the memory.
 
 ---
 
-### `Message`
+### Message
 
 Represents a message in a conversation.
 
 **Attributes**:
 
 - `uuid` (Optional[str]): The unique identifier of the message.
 - `created_at` (Optional[str]): The timestamp of when the message was created.
@@ -316,15 +320,15 @@
 
 **Methods**:
 
 - `to_dict() -> Dict[str, Any]`: Returns a dictionary representation of the message.
 
 ---
 
-### `Summary`
+### Summary
 
 Represents a summary of a conversation.
 
 **Attributes**:
 
 - `uuid` (str): The unique identifier of the summary.
 - `created_at` (str): The timestamp of when the summary was created.
@@ -334,41 +338,65 @@
 
 **Methods**:
 
 - `to_dict() -> Dict[str, Any]`: Returns a dictionary representation of the summary.
 
 ---
 
-### `SearchPayload`
+### SearchPayload
 
 Represents a search payload for querying memory.
 
 **Attributes**:
 
 - `meta` (Dict[str, Any]): Metadata associated with the search query.
 - `text` (str): The text of the search query.
 
 ---
 
-### `SearchResult`
+### SearchResult
 
 Represents a search result from querying memory.
 
 **Attributes**:
 
 - `message` (Optional[Dict[str, Any]]): The message associated with the search result.
 - `meta` (Optional[Dict[str, Any]]): Metadata associated with the search result.
 - `score` (Optional[float]): The score of the search result.
 - `summary` (Optional[str]): The summary of the search result.
 - `dist` (Optional[float]): The distance metric of the search result.
 
 ---
+## Exceptions
 
-### `APIError`
+### APIError
 
 Represents an API error.
 
 **Attributes**:
 
 - `code` (int): The error code associated with the API error.
 - `message` (str): The error message associated with the API error.
+---
+
+### ZepClientError
+
+Base exception class for ZepClient errors.
+
+**Attributes**:
+
+- `message`: str - The error message associated with the ZepClient error.
+- `response_data`: Optional[dict] - The response data associated with the ZepClient error.
+---
+
+### NotFoundError
+
+Raised when the API response contains no results.
+
+Inherits from ZepClientError.
+
+**Attributes**:
+
+- `message`: str - The error message to be set for the exception.
+
+---
```

