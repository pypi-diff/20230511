# Comparing `tmp/jupyter_ai_magics-0.6.1.tar.gz` & `tmp/jupyter_ai_magics-0.7.0.tar.gz`

## Comparing `jupyter_ai_magics-0.6.1.tar` & `jupyter_ai_magics-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/setup.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/jupyter_ai_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/jupyter_ai_magics/_version.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/jupyter_ai_magics/exception.py
--rw-r--r--   0        0        0     8841 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/jupyter_ai_magics/magics.py
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/jupyter_ai_magics/providers.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/jupyter_ai_magics/tests/__init__.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/LICENSE
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/README.md
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/setup.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/jupyter_ai_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/jupyter_ai_magics/_version.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/jupyter_ai_magics/aliases.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/jupyter_ai_magics/embedding_providers.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/jupyter_ai_magics/exception.py
+-rw-r--r--   0        0        0    14961 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/jupyter_ai_magics/magics.py
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/jupyter_ai_magics/providers.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/jupyter_ai_magics/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/jupyter_ai_magics/tests/__init__.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/LICENSE
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/README.md
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.0/PKG-INFO
```

### Comparing `jupyter_ai_magics-0.6.1/package.json` & `jupyter_ai_magics-0.7.0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.7.0'"}*

```diff
@@ -16,9 +16,9 @@
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-ai.git"
     },
     "scripts": {
         "dev-install": "pip install -e \".[all]\"",
         "dev-uninstall": "pip uninstall jupyter_ai_magics -y"
     },
-    "version": "0.6.1"
+    "version": "0.7.0"
 }
```

### Comparing `jupyter_ai_magics-0.6.1/jupyter_ai_magics/__init__.py` & `jupyter_ai_magics-0.7.0/jupyter_ai_magics/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,16 +6,23 @@
 from .providers import (
     AI21Provider,
     AnthropicProvider,
     CohereProvider,
     HfHubProvider,
     OpenAIProvider,
     ChatOpenAIProvider,
+    ChatOpenAINewProvider,
     SmEndpointProvider
 )
+# expose embedding model providers on the package root
+from .embedding_providers import (
+    OpenAIEmbeddingsProvider,
+    CohereEmbeddingsProvider,
+    HfHubEmbeddingsProvider
+)
 from .providers import BaseProvider
 
 def load_ipython_extension(ipython):
     ipython.register_magics(AiMagics)
     ipython.set_custom_exc((BaseException,), store_exception)
 
 def unload_ipython_extension(ipython):
```

### Comparing `jupyter_ai_magics-0.6.1/jupyter_ai_magics/exception.py` & `jupyter_ai_magics-0.7.0/jupyter_ai_magics/exception.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.6.1/.gitignore` & `jupyter_ai_magics-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.6.1/LICENSE` & `jupyter_ai_magics-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.6.1/pyproject.toml` & `jupyter_ai_magics-0.7.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 dependencies = [
     "ipython",
     "pydantic",
     "importlib_metadata~=5.2.0",
-    "langchain~=0.0.144"
+    "langchain==0.0.158"
 ]
 
 [project.optional-dependencies]
 test = [
     "coverage",
     "pytest",
     "pytest-asyncio",
@@ -38,27 +38,34 @@
 
 all = [
     "ai21",
     "anthropic",
     "cohere",
     "huggingface_hub",
     "ipywidgets",
+    "pillow",
     "openai",
     "boto3"
 ]
 
 [project.entry-points."jupyter_ai.model_providers"]
 ai21 = "jupyter_ai_magics:AI21Provider"
 anthropic = "jupyter_ai_magics:AnthropicProvider"
 cohere = "jupyter_ai_magics:CohereProvider"
 huggingface_hub = "jupyter_ai_magics:HfHubProvider"
 openai = "jupyter_ai_magics:OpenAIProvider"
 openai-chat = "jupyter_ai_magics:ChatOpenAIProvider"
+openai-chat-new = "jupyter_ai_magics:ChatOpenAINewProvider"
 sagemaker-endpoint = "jupyter_ai_magics:SmEndpointProvider"
 
+[project.entry-points."jupyter_ai.embeddings_model_providers"]
+cohere = "jupyter_ai_magics:CohereEmbeddingsProvider"
+huggingface_hub = "jupyter_ai_magics:HfHubEmbeddingsProvider"
+openai = "jupyter_ai_magics:OpenAIEmbeddingsProvider"
+
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
 fields = ["description", "authors", "urls"]
 
 [tool.hatch.build.hooks.version]
```

### Comparing `jupyter_ai_magics-0.6.1/PKG-INFO` & `jupyter_ai_magics-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_magics
-Version: 0.6.1
+Version: 0.7.0
 Summary: Jupyter AI magics Python package. Not published on NPM.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -44,24 +44,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata~=5.2.0
 Requires-Dist: ipython
-Requires-Dist: langchain~=0.0.144
+Requires-Dist: langchain==0.0.158
 Requires-Dist: pydantic
 Provides-Extra: all
 Requires-Dist: ai21; extra == 'all'
 Requires-Dist: anthropic; extra == 'all'
 Requires-Dist: boto3; extra == 'all'
 Requires-Dist: cohere; extra == 'all'
 Requires-Dist: huggingface-hub; extra == 'all'
 Requires-Dist: ipywidgets; extra == 'all'
 Requires-Dist: openai; extra == 'all'
+Requires-Dist: pillow; extra == 'all'
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
```

