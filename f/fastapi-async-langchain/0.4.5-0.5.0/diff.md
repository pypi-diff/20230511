# Comparing `tmp/fastapi_async_langchain-0.4.5.tar.gz` & `tmp/fastapi_async_langchain-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_async_langchain-0.4.5.tar", max compression
+gzip compressed data, was "fastapi_async_langchain-0.5.0.tar", max compression
```

## Comparing `fastapi_async_langchain-0.4.5.tar` & `fastapi_async_langchain-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,19 @@
--rw-r--r--   0        0        0     1073 2023-05-10 20:56:34.058386 fastapi_async_langchain-0.4.5/LICENSE
--rw-r--r--   0        0        0     1818 2023-05-10 20:56:34.058386 fastapi_async_langchain-0.4.5/README.md
--rw-r--r--   0        0        0        0 2023-05-10 20:56:34.270398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/__init__.py
--rw-r--r--   0        0        0      502 2023-05-10 20:56:34.270398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/callbacks/__init__.py
--rw-r--r--   0        0        0      934 2023-05-10 20:56:34.270398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/callbacks/base.py
--rw-r--r--   0        0        0      773 2023-05-10 20:56:34.270398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/callbacks/llm.py
--rw-r--r--   0        0        0     1964 2023-05-10 20:56:34.270398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0      309 2023-05-10 20:56:34.270398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/responses/__init__.py
--rw-r--r--   0        0        0     2605 2023-05-10 20:56:34.270398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/responses/base.py
--rw-r--r--   0        0        0      819 2023-05-10 20:56:34.270398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/responses/conversational_retrieval.py
--rw-r--r--   0        0        0      727 2023-05-10 20:56:34.270398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/responses/llm.py
--rw-r--r--   0        0        0      782 2023-05-10 20:56:34.274398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/responses/retrieval_qa.py
--rw-r--r--   0        0        0      536 2023-05-10 20:56:34.274398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/schemas.py
--rw-r--r--   0        0        0       69 2023-05-10 20:56:34.274398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/testing/__init__.py
--rw-r--r--   0        0        0     2496 2023-05-10 20:56:34.274398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-10 20:56:34.274398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/testing/settings.py
--rw-r--r--   0        0        0      331 2023-05-10 20:56:34.274398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/websockets/__init__.py
--rw-r--r--   0        0        0     2907 2023-05-10 20:56:34.274398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/websockets/base.py
--rw-r--r--   0        0        0      928 2023-05-10 20:56:34.274398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/websockets/llm.py
--rw-r--r--   0        0        0      985 2023-05-10 20:56:34.274398 fastapi_async_langchain-0.4.5/fastapi_async_langchain/websockets/retrieval_qa.py
--rw-r--r--   0        0        0      558 2023-05-10 20:56:34.274398 fastapi_async_langchain-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-10 22:24:45.315242 fastapi_async_langchain-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2583 2023-05-10 22:24:45.315242 fastapi_async_langchain-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/__init__.py
+-rw-r--r--   0        0        0     2098 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/__init__.py
+-rw-r--r--   0        0        0      956 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/base.py
+-rw-r--r--   0        0        0     1389 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/llm.py
+-rw-r--r--   0        0        0     2180 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/qa_with_sources.py
+-rw-r--r--   0        0        0     2882 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0     1332 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/register.py
+-rw-r--r--   0        0        0       74 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/responses/__init__.py
+-rw-r--r--   0        0        0     2787 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/responses/streaming.py
+-rw-r--r--   0        0        0      536 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/testing/__init__.py
+-rw-r--r--   0        0        0     2496 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/websockets/__init__.py
+-rw-r--r--   0        0        0     3661 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/websockets/base.py
+-rw-r--r--   0        0        0      558 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.5.0/PKG-INFO
```

### Comparing `fastapi_async_langchain-0.4.5/LICENSE` & `fastapi_async_langchain-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.5/README.md` & `fastapi_async_langchain-0.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,57 @@
 # fastapi-async-langchain
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fastapi-async-langchain.svg)](https://pypi.org/project/fastapi-async-langchain/)
 
 Ship production-ready [LangChain](https://github.com/hwchase17/langchain) projects with [FastAPI](https://github.com/tiangolo/fastapi).
 
-## :rocket: Features
+## 🚀 Features
 
 - supports token streaming over HTTP and Websocket
-- supports multiple langchain `Chain` types (ongoing...)
+- supports multiple langchain `Chain` types
 - simple gradio chatbot UI for fast prototyping
+- follows FastAPI responses naming convention
 
 ## 💾 Installation
 
 The library is available on PyPI and can be installed via `pip`.
 
 ```bash
 pip install fastapi-async-langchain
 ```
 
-## 🎯 Demo Examples
+## 🔥 Deploy in under 20 lines of code
 
-See [`examples/`](examples/README.md) for list of available demo examples.
+```python
+from dotenv import load_dotenv
+from fastapi import FastAPI
+from langchain import ConversationChain
+from langchain.chat_models import ChatOpenAI
+from pydantic import BaseModel
+from fastapi_async_langchain.responses import StreamingResponse
+
+load_dotenv()
+app = FastAPI()
+
+class Request(BaseModel):
+    query: str
+
+@app.post("/chat")
+async def chat(request: Request) -> StreamingResponse:
+    chain = ConversationChain(llm=ChatOpenAI(temperature=0, streaming=True), verbose=True)
+    return StreamingResponse.from_chain(chain, request.query, media_type="text/event-stream")
+```
+
+See [`examples/`](https://github.com/ajndkr/fastapi-async-langchain/blob/main/examples/README.md) for list of available demo examples.
 
 Create a `.env` file using `.env.sample` and add your OpenAI API key to it
 before running the examples.
 
-![demo](assets/demo.gif)
+![demo](https://raw.githubusercontent.com/ajndkr/fastapi-async-langchain/main/assets/demo.gif)
 
 ## 🤝 Contributing
 
 [![Code check](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/code-check.yaml/badge.svg)](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/code-check.yaml)
 [![Publish](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/publish.yaml/badge.svg)](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/publish.yaml)
 
 Contributions are more than welcome! If you have an idea for a new feature or want to help improve fastapi-async-langchain, please create an issue or submit a pull request
```

### Comparing `fastapi_async_langchain-0.4.5/fastapi_async_langchain/callbacks/base.py` & `fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from fastapi import WebSocket
 from langchain.callbacks.base import AsyncCallbackHandler
 from pydantic import BaseModel, Field
 from starlette.types import Send
 
-from ..schemas import WebsocketResponse
+from fastapi_async_langchain.schemas import WebsocketResponse
 
 
 class AsyncStreamingResponseCallback(AsyncCallbackHandler, BaseModel):
     """Async Callback handler for FastAPI StreamingResponse."""
 
     send: Send = Field(...)
```

### Comparing `fastapi_async_langchain-0.4.5/fastapi_async_langchain/callbacks/retrieval_qa.py` & `fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/retrieval_qa.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from typing import Any, Dict
 
+from fastapi_async_langchain.register import (
+    register_streaming_callback,
+    register_websocket_callback,
+)
+
 from .llm import AsyncLLMChainStreamingCallback, AsyncLLMChainWebsocketCallback
 
 SOURCE_DOCUMENT_TEMPLATE = """
 page content: {page_content}
 source: {source}
 """
 
 
-class AsyncRetrievalQAStreamingCallback(AsyncLLMChainStreamingCallback):
-    """AsyncStreamingResponseCallback handler for RetrievalQA."""
+class AsyncBaseRetrievalQAStreamingCallback(AsyncLLMChainStreamingCallback):
+    """AsyncStreamingResponseCallback handler for BaseRetrievalQA."""
 
     source_document_template: str = SOURCE_DOCUMENT_TEMPLATE
 
     async def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> None:
         """Run when chain ends running."""
         if "source_documents" in outputs:
             await self.send("\n\nSOURCE DOCUMENTS: \n")
@@ -22,16 +27,16 @@
                     self.source_document_template.format(
                         page_content=document.page_content,
                         source=document.metadata["source"],
                     )
                 )
 
 
-class AsyncRetrievalQAWebsocketCallback(AsyncLLMChainWebsocketCallback):
-    """AsyncWebsocketCallback handler for RetrievalQA."""
+class AsyncBaseRetrievalQAWebsocketCallback(AsyncLLMChainWebsocketCallback):
+    """AsyncWebsocketCallback handler for BaseRetrievalQA."""
 
     source_document_template: str = SOURCE_DOCUMENT_TEMPLATE
 
     async def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> None:
         """Run when chain ends running."""
         if "source_documents" in outputs:
             await self.websocket.send_json(
@@ -47,7 +52,35 @@
                 )
                 await self.websocket.send_json(
                     {
                         **self.response.dict(),
                         **{"message": source_document},
                     }
                 )
+
+
+@register_streaming_callback("RetrievalQA")
+class AsyncRetrievalQAStreamingCallback(AsyncBaseRetrievalQAStreamingCallback):
+    """AsyncStreamingResponseCallback handler for RetrievalQA."""
+
+    pass
+
+
+@register_streaming_callback("VectorDBQA")
+class AsyncVectorDBQAStreamingCallback(AsyncBaseRetrievalQAStreamingCallback):
+    """AsyncStreamingResponseCallback handler for VectorDBQA."""
+
+    pass
+
+
+@register_websocket_callback("RetrievalQA")
+class AsyncRetrievalQAWebsocketCallback(AsyncBaseRetrievalQAWebsocketCallback):
+    """AsyncWebsocketCallback handler for RetrievalQA."""
+
+    pass
+
+
+@register_websocket_callback("VectorDBQA")
+class AsyncVectorDBQAWebsocketCallback(AsyncBaseRetrievalQAWebsocketCallback):
+    """AsyncWebsocketCallback handler for VectorDBQA."""
+
+    pass
```

### Comparing `fastapi_async_langchain-0.4.5/fastapi_async_langchain/responses/base.py` & `fastapi_async_langchain-0.5.0/fastapi_async_langchain/responses/streaming.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Credits:
 - https://gist.github.com/ninely/88485b2e265d852d3feb8bd115065b1a
 - https://github.com/hwchase17/langchain/discussions/1706
 """
-from abc import abstractstaticmethod
 from typing import Any, Awaitable, Callable, Dict, Optional, Union
 
-from fastapi.responses import StreamingResponse
+from fastapi.responses import StreamingResponse as _StreamingResponse
 from langchain.chains.base import Chain
 from starlette.background import BackgroundTask
 from starlette.types import Send
 
+from fastapi_async_langchain.callbacks import get_streaming_callback
 
-class BaseLangchainStreamingResponse(StreamingResponse):
-    """Base StreamingResponse class wrapper for langchain chains."""
+
+class StreamingResponse(_StreamingResponse):
+    """StreamingResponse class wrapper for langchain chains."""
 
     def __init__(
         self,
         chain_executor: Callable[[Send], Awaitable[Any]],
         background: Optional[BackgroundTask] = None,
         **kwargs: Any,
     ) -> None:
@@ -53,28 +54,33 @@
                     "more_body": False,
                 }
             )
             return
 
         await send({"type": "http.response.body", "body": b"", "more_body": False})
 
-    @abstractstaticmethod
+    @staticmethod
     def _create_chain_executor(
         chain: Chain, inputs: Union[Dict[str, Any], Any]
     ) -> Callable[[Send], Awaitable[Any]]:
-        raise NotImplementedError
+        async def wrapper(send: Send):
+            return await chain.acall(
+                inputs=inputs, callbacks=[get_streaming_callback(chain, send=send)]
+            )
+
+        return wrapper
 
     @classmethod
     def from_chain(
         cls,
         chain: Chain,
         inputs: Union[Dict[str, Any], Any],
         background: Optional[BackgroundTask] = None,
         **kwargs: Any,
-    ) -> "BaseLangchainStreamingResponse":
+    ) -> "StreamingResponse":
         chain_executor = cls._create_chain_executor(chain, inputs)
 
         return cls(
             chain_executor=chain_executor,
             background=background,
             **kwargs,
         )
```

### Comparing `fastapi_async_langchain-0.4.5/fastapi_async_langchain/schemas.py` & `fastapi_async_langchain-0.5.0/fastapi_async_langchain/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.5/fastapi_async_langchain/testing/gradio.py` & `fastapi_async_langchain-0.5.0/fastapi_async_langchain/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.5/fastapi_async_langchain/websockets/base.py` & `fastapi_async_langchain-0.5.0/fastapi_async_langchain/websockets/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,20 +7,26 @@
 from abc import abstractstaticmethod
 from typing import Any, Awaitable, Callable
 
 from fastapi import WebSocket, WebSocketDisconnect
 from langchain.chains.base import Chain
 from pydantic import BaseModel, Field
 
-from ..schemas import Message, MessageType, Sender, WebsocketResponse
+from fastapi_async_langchain.callbacks import get_websocket_callback
+from fastapi_async_langchain.schemas import (
+    Message,
+    MessageType,
+    Sender,
+    WebsocketResponse,
+)
 
 logger = logging.getLogger(__name__)
 
 
-class BaseLangchainWebsocketConnection(BaseModel):
+class BaseWebsocketConnection(BaseModel):
     websocket: WebSocket = Field(...)
     chain_executor: Callable[[], Awaitable[Any]] = Field(...)
 
     class Config:
         arbitrary_types_allowed = True
 
     async def connect(self):
@@ -72,20 +78,42 @@
         raise NotImplementedError
 
     @classmethod
     def from_chain(
         cls,
         chain: Chain,
         websocket: WebSocket,
-    ) -> "BaseLangchainWebsocketConnection":
+    ) -> "BaseWebsocketConnection":
         chain_executor = cls._create_chain_executor(
             chain,
             websocket,
             WebsocketResponse(
                 sender=Sender.BOT, message=Message.NULL, message_type=MessageType.STREAM
             ),
         )
 
         return cls(
             chain_executor=chain_executor,
             websocket=websocket,
         )
+
+
+class WebsocketConnection(BaseWebsocketConnection):
+    """BaseLangchainStreamingResponse class wrapper for LLMChain instances."""
+
+    @staticmethod
+    def _create_chain_executor(
+        chain: Chain,
+        websocket: WebSocket,
+        response: WebsocketResponse,
+    ) -> Callable[[], Awaitable[Any]]:
+        async def wrapper(user_message: str):
+            return await chain.acall(
+                inputs=user_message,
+                callbacks=[
+                    get_websocket_callback(
+                        chain=chain, websocket=websocket, response=response
+                    )
+                ],
+            )
+
+        return wrapper
```

### Comparing `fastapi_async_langchain-0.4.5/pyproject.toml` & `fastapi_async_langchain-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-async-langchain"
-version = "0.4.5"
+version = "0.5.0"
 description = "FastAPI async components for streaming LLM chains."
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_async_langchain"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `fastapi_async_langchain-0.4.5/PKG-INFO` & `fastapi_async_langchain-0.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-async-langchain
-Version: 0.4.5
+Version: 0.5.0
 Summary: FastAPI async components for streaming LLM chains.
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,36 +18,57 @@
 # fastapi-async-langchain
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fastapi-async-langchain.svg)](https://pypi.org/project/fastapi-async-langchain/)
 
 Ship production-ready [LangChain](https://github.com/hwchase17/langchain) projects with [FastAPI](https://github.com/tiangolo/fastapi).
 
-## :rocket: Features
+## 🚀 Features
 
 - supports token streaming over HTTP and Websocket
-- supports multiple langchain `Chain` types (ongoing...)
+- supports multiple langchain `Chain` types
 - simple gradio chatbot UI for fast prototyping
+- follows FastAPI responses naming convention
 
 ## 💾 Installation
 
 The library is available on PyPI and can be installed via `pip`.
 
 ```bash
 pip install fastapi-async-langchain
 ```
 
-## 🎯 Demo Examples
+## 🔥 Deploy in under 20 lines of code
 
-See [`examples/`](examples/README.md) for list of available demo examples.
+```python
+from dotenv import load_dotenv
+from fastapi import FastAPI
+from langchain import ConversationChain
+from langchain.chat_models import ChatOpenAI
+from pydantic import BaseModel
+from fastapi_async_langchain.responses import StreamingResponse
+
+load_dotenv()
+app = FastAPI()
+
+class Request(BaseModel):
+    query: str
+
+@app.post("/chat")
+async def chat(request: Request) -> StreamingResponse:
+    chain = ConversationChain(llm=ChatOpenAI(temperature=0, streaming=True), verbose=True)
+    return StreamingResponse.from_chain(chain, request.query, media_type="text/event-stream")
+```
+
+See [`examples/`](https://github.com/ajndkr/fastapi-async-langchain/blob/main/examples/README.md) for list of available demo examples.
 
 Create a `.env` file using `.env.sample` and add your OpenAI API key to it
 before running the examples.
 
-![demo](assets/demo.gif)
+![demo](https://raw.githubusercontent.com/ajndkr/fastapi-async-langchain/main/assets/demo.gif)
 
 ## 🤝 Contributing
 
 [![Code check](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/code-check.yaml/badge.svg)](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/code-check.yaml)
 [![Publish](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/publish.yaml/badge.svg)](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/publish.yaml)
 
 Contributions are more than welcome! If you have an idea for a new feature or want to help improve fastapi-async-langchain, please create an issue or submit a pull request
```

