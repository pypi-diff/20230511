# Comparing `tmp/fastapi_async_langchain-0.5.0.tar.gz` & `tmp/fastapi_async_langchain-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_async_langchain-0.5.0.tar", max compression
+gzip compressed data, was "fastapi_async_langchain-0.5.1.tar", max compression
```

## Comparing `fastapi_async_langchain-0.5.0.tar` & `fastapi_async_langchain-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1073 2023-05-10 22:24:45.315242 fastapi_async_langchain-0.5.0/LICENSE
--rw-r--r--   0        0        0     2583 2023-05-10 22:24:45.315242 fastapi_async_langchain-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/__init__.py
--rw-r--r--   0        0        0     2098 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/__init__.py
--rw-r--r--   0        0        0      956 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/base.py
--rw-r--r--   0        0        0     1389 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/llm.py
--rw-r--r--   0        0        0     2180 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/qa_with_sources.py
--rw-r--r--   0        0        0     2882 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0     1332 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/register.py
--rw-r--r--   0        0        0       74 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/responses/__init__.py
--rw-r--r--   0        0        0     2787 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/responses/streaming.py
--rw-r--r--   0        0        0      536 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/schemas.py
--rw-r--r--   0        0        0       69 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/testing/__init__.py
--rw-r--r--   0        0        0     2496 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/testing/settings.py
--rw-r--r--   0        0        0       73 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/websockets/__init__.py
--rw-r--r--   0        0        0     3661 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/fastapi_async_langchain/websockets/base.py
--rw-r--r--   0        0        0      558 2023-05-10 22:24:45.527241 fastapi_async_langchain-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-10 22:41:03.067890 fastapi_async_langchain-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2938 2023-05-10 22:41:03.067890 fastapi_async_langchain-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 22:41:03.271889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/__init__.py
+-rw-r--r--   0        0        0     2098 2023-05-10 22:41:03.271889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/callbacks/__init__.py
+-rw-r--r--   0        0        0      956 2023-05-10 22:41:03.271889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/callbacks/base.py
+-rw-r--r--   0        0        0     1389 2023-05-10 22:41:03.271889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/callbacks/llm.py
+-rw-r--r--   0        0        0     2180 2023-05-10 22:41:03.271889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/callbacks/qa_with_sources.py
+-rw-r--r--   0        0        0     2882 2023-05-10 22:41:03.271889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0     1332 2023-05-10 22:41:03.271889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/register.py
+-rw-r--r--   0        0        0       74 2023-05-10 22:41:03.271889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/responses/__init__.py
+-rw-r--r--   0        0        0     2787 2023-05-10 22:41:03.271889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/responses/streaming.py
+-rw-r--r--   0        0        0      536 2023-05-10 22:41:03.271889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-10 22:41:03.271889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/testing/__init__.py
+-rw-r--r--   0        0        0     2496 2023-05-10 22:41:03.271889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-10 22:41:03.275889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-05-10 22:41:03.275889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/websockets/__init__.py
+-rw-r--r--   0        0        0     3661 2023-05-10 22:41:03.275889 fastapi_async_langchain-0.5.1/fastapi_async_langchain/websockets/base.py
+-rw-r--r--   0        0        0      705 2023-05-10 22:41:03.275889 fastapi_async_langchain-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3787 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.5.1/PKG-INFO
```

### Comparing `fastapi_async_langchain-0.5.0/LICENSE` & `fastapi_async_langchain-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.0/README.md` & `fastapi_async_langchain-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 # fastapi-async-langchain
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fastapi-async-langchain.svg)](https://pypi.org/project/fastapi-async-langchain/)
 
-Ship production-ready [LangChain](https://github.com/hwchase17/langchain) projects with [FastAPI](https://github.com/tiangolo/fastapi).
+Ship production-ready [LangChain](https://github.com/hwchase17/langchain) projects with
+[FastAPI](https://github.com/tiangolo/fastapi).
 
 ## 🚀 Features
 
 - supports token streaming over HTTP and Websocket
 - supports multiple langchain `Chain` types
 - simple gradio chatbot UI for fast prototyping
 - follows FastAPI responses naming convention
 
+## ❓ Why?
+
+There are great low-code/no-code solutions in the open source to deploy your Langchain projects. However,
+most of them are opinionated in terms of cloud or deployment code. This project aims to provide FastAPI users
+with a cloud-agnostic and deployment-agnostic solution which can be easily integrated into existing
+backend infrastructures.
+
 ## 💾 Installation
 
 The library is available on PyPI and can be installed via `pip`.
 
 ```bash
 pip install fastapi-async-langchain
 ```
```

### Comparing `fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/__init__.py` & `fastapi_async_langchain-0.5.1/fastapi_async_langchain/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/base.py` & `fastapi_async_langchain-0.5.1/fastapi_async_langchain/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/llm.py` & `fastapi_async_langchain-0.5.1/fastapi_async_langchain/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/qa_with_sources.py` & `fastapi_async_langchain-0.5.1/fastapi_async_langchain/callbacks/qa_with_sources.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.0/fastapi_async_langchain/callbacks/retrieval_qa.py` & `fastapi_async_langchain-0.5.1/fastapi_async_langchain/callbacks/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.0/fastapi_async_langchain/register.py` & `fastapi_async_langchain-0.5.1/fastapi_async_langchain/register.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.0/fastapi_async_langchain/responses/streaming.py` & `fastapi_async_langchain-0.5.1/fastapi_async_langchain/responses/streaming.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.0/fastapi_async_langchain/schemas.py` & `fastapi_async_langchain-0.5.1/fastapi_async_langchain/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.0/fastapi_async_langchain/testing/gradio.py` & `fastapi_async_langchain-0.5.1/fastapi_async_langchain/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.0/fastapi_async_langchain/websockets/base.py` & `fastapi_async_langchain-0.5.1/fastapi_async_langchain/websockets/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.0/PKG-INFO` & `fastapi_async_langchain-0.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 Metadata-Version: 2.1
 Name: fastapi-async-langchain
-Version: 0.5.0
-Summary: FastAPI async components for streaming LLM chains.
+Version: 0.5.1
+Summary: Ship production-ready LangChain projects with FastAPI
+Home-page: https://github.com/ajndkr/fastapi-async-langchain
+License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: langchain (>=0.0.164,<0.0.165)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: urllib3 (<=1.26.15)
+Project-URL: Repository, https://github.com/ajndkr/fastapi-async-langchain
 Description-Content-Type: text/markdown
 
 # fastapi-async-langchain
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fastapi-async-langchain.svg)](https://pypi.org/project/fastapi-async-langchain/)
 
-Ship production-ready [LangChain](https://github.com/hwchase17/langchain) projects with [FastAPI](https://github.com/tiangolo/fastapi).
+Ship production-ready [LangChain](https://github.com/hwchase17/langchain) projects with
+[FastAPI](https://github.com/tiangolo/fastapi).
 
 ## 🚀 Features
 
 - supports token streaming over HTTP and Websocket
 - supports multiple langchain `Chain` types
 - simple gradio chatbot UI for fast prototyping
 - follows FastAPI responses naming convention
 
+## ❓ Why?
+
+There are great low-code/no-code solutions in the open source to deploy your Langchain projects. However,
+most of them are opinionated in terms of cloud or deployment code. This project aims to provide FastAPI users
+with a cloud-agnostic and deployment-agnostic solution which can be easily integrated into existing
+backend infrastructures.
+
 ## 💾 Installation
 
 The library is available on PyPI and can be installed via `pip`.
 
 ```bash
 pip install fastapi-async-langchain
 ```
```

