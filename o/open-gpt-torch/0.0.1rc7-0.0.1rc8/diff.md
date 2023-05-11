# Comparing `tmp/open_gpt_torch-0.0.1rc7.tar.gz` & `tmp/open_gpt_torch-0.0.1rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.1rc7.tar", max compression
+gzip compressed data, was "open_gpt_torch-0.0.1rc8.tar", max compression
```

## Comparing `open_gpt_torch-0.0.1rc7.tar` & `open_gpt_torch-0.0.1rc8.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0    10825 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/LICENSE
--rw-r--r--   0        0        0     7531 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/README.md
--rw-r--r--   0        0        0      853 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/__init__.py
--rw-r--r--   0        0        0      107 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/__main__.py
--rw-r--r--   0        0        0      474 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/adapter.py
--rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/cli/__init__.py
--rw-r--r--   0        0        0     1039 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/cli/application.py
--rw-r--r--   0        0        0      508 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/cli/command_loader.py
--rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/cli/commands/__init__.py
--rw-r--r--   0        0        0      567 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/cli/commands/about.py
--rw-r--r--   0        0        0     1232 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/cli/commands/serve.py
--rw-r--r--   0        0        0     2977 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/factory.py
--rw-r--r--   0        0        0     2509 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/helper.py
--rw-r--r--   0        0        0      349 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/hub.py
--rw-r--r--   0        0        0      498 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/logging.py
--rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0     5774 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     8574 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/flamingo_model.py
--rw-r--r--   0        0        0     5309 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     2403 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flan/__init__.py
--rw-r--r--   0        0        0     1074 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flan/loading.py
--rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0     1407 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/llama/modeling.py
--rw-r--r--   0        0        0     4952 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/loading.py
--rw-r--r--   0        0        0     2737 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/modeling.py
--rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/moss/__init__.py
--rw-r--r--   0        0        0      234 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/moss/modeling.py
--rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0     2157 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/pythia/loading.py
--rw-r--r--   0        0        0      239 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/pythia/modeling.py
--rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/stablelm/__init__.py
--rw-r--r--   0        0        0      907 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/stablelm/modeling.py
--rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/vicuna/__init__.py
--rw-r--r--   0        0        0     3372 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/vicuna/loading.py
--rw-r--r--   0        0        0      771 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/vicuna/modeling.py
--rw-r--r--   0        0        0     2862 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/profile.py
--rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/serve/__init__.py
--rw-r--r--   0        0        0       36 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/serve/executors/__init__.py
--rw-r--r--   0        0        0     1742 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/serve/executors/base.py
--rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/serve/executors/flamingo.py
--rw-r--r--   0        0        0      608 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/serve/flow.py
--rw-r--r--   0        0        0      931 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/serve/gateway.py
--rw-r--r--   0        0        0     2279 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/pyproject.toml
--rw-r--r--   0        0        0    19904 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc7/PKG-INFO
+-rw-r--r--   0        0        0    10825 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/LICENSE
+-rw-r--r--   0        0        0     8750 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/README.md
+-rw-r--r--   0        0        0      853 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/__main__.py
+-rw-r--r--   0        0        0      474 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/adapter.py
+-rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/cli/__init__.py
+-rw-r--r--   0        0        0     1039 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/cli/application.py
+-rw-r--r--   0        0        0      508 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/cli/command_loader.py
+-rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/cli/commands/__init__.py
+-rw-r--r--   0        0        0      567 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/cli/commands/about.py
+-rw-r--r--   0        0        0     1229 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/cli/commands/serve.py
+-rw-r--r--   0        0        0     3706 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/factory.py
+-rw-r--r--   0        0        0     2509 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/helper.py
+-rw-r--r--   0        0        0      349 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/hub.py
+-rw-r--r--   0        0        0      498 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/logging.py
+-rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0        0        0     6038 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0        0        0     9043 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/flamingo_model.py
+-rw-r--r--   0        0        0     5644 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0        0        0     2511 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flan/__init__.py
+-rw-r--r--   0        0        0     1074 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flan/loading.py
+-rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/llama/__init__.py
+-rw-r--r--   0        0        0     1407 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/llama/modeling.py
+-rw-r--r--   0        0        0     4952 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/loading.py
+-rw-r--r--   0        0        0     2723 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/moss/__init__.py
+-rw-r--r--   0        0        0      234 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/moss/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0        0        0     2157 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/pythia/loading.py
+-rw-r--r--   0        0        0      239 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/pythia/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/stablelm/__init__.py
+-rw-r--r--   0        0        0      907 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/stablelm/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/vicuna/__init__.py
+-rw-r--r--   0        0        0     3372 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/vicuna/loading.py
+-rw-r--r--   0        0        0      771 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/vicuna/modeling.py
+-rw-r--r--   0        0        0     2862 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/profile.py
+-rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/executors/__init__.py
+-rw-r--r--   0        0        0     1778 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/executors/base.py
+-rw-r--r--   0        0        0     2132 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/executors/flamingo.py
+-rw-r--r--   0        0        0      171 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/executors/utils.py
+-rw-r--r--   0        0        0      931 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/gateway.py
+-rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/playground.py
+-rw-r--r--   0        0        0     2279 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/pyproject.toml
+-rw-r--r--   0        0        0    21123 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc8/PKG-INFO
```

### Comparing `open_gpt_torch-0.0.1rc7/LICENSE` & `open_gpt_torch-0.0.1rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/README.md` & `open_gpt_torch-0.0.1rc8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,80 @@
 # OpenGPT
 
+![](https://img.shields.io/badge/Made%20with-JinaAI-blueviolet?style=flat)
+[![PyPI](https://img.shields.io/pypi/v/open_gpt_torch)](https://pypi.org/project/open_gpt_torch/)
+[![PyPI - License](https://img.shields.io/pypi/l/open_gpt_torch)](https://pypi.org/project/open_gpt_torch/)
+
 `OpenGPT` is an open-source _cloud-native_ large **multi-modal models** (LMMs) serving solution. 
 It is designed to simplify the deployment and management of large language models, on a distributed cluster of GPUs.
 
 > **Note**
 > The content of `README.md` is just a placeholder to remind me of what I want to do.
 
+## Table of contents
+
+- [Features](#features)
+- [Supported models](#supported-models)
+- [Get started](#get-started)
+- [Build a model serving in one line](#build-a-model-serving-in-one-line)
+- [Cloud-native deployment](#cloud-native-deployment)
+  - [JCloud](#jcloud)
+  - [Kubernetes](#kubernetes)
+- [Roadmap](#roadmap)
+
 ## Features
 
 OpenGPT provides the following features to make it easy to deploy and serve large multi-modal models (LMMs) in production:
 
 - Support for multi-modal models
 - Scalable architecture for handling high traffic loads
 - Optimized for low-latency inference
 - Automatic model partitioning and distribution across multiple GPUs
 - Centralized model management and monitoring
 - REST API for easy integration with existing applications
 
-You can learn more about OpenGPT’s [architecture in our documentation](https://opengpt.readthedocs.io/en/latest/).
+## Updates
+
+- **2023-05-12**: 🎉 We have released the first version `v0.0.1` of OpenGPT. You can install it with `pip install open_gpt_torch`.
+
+## Supported Models
+
+OpenGPT supports the following models out of the box:
+
+- LLM (Large Language Model)
+
+  - [Llama](https://huggingface.co/facebook/llama-7b)
+  - [Pythia](https://huggingface.co/...)
+  - [StableLM](https://huggingface.co/...)
+  - [Vicuna](https://huggingface.co/...)
+  - [MOSS](https://huggingface.co/...)
+
+- LMM (Large Multi-modal Model)
+
+  - [OpenFlamingo](https://huggingface.co/...)
+  - [MiniGPT4](https://huggingface.co/...) (WIP)
+
+For more details about the supported models, please see the [Model Zoo](./MODEL_ZOO.md).
 
 
 ## Roadmap
 
 You can view our roadmap with features that are planned, started, and completed on the [Roadmap discussion](discussions/categories/roadmap) category.
 
-## Installation
+## Get Started
+
+### Installation
 
 Install the package with pip:
 
 ```bash
 pip install open_gpt_torch
 ```
 
-## Quickstart
+### Quickstart
 
 ```python
 import open_gpt
 
 model = open_gpt.create_model('facebook/llama-7b', device='cuda', precision='fp16')
 
 prompt = "The quick brown fox jumps over the lazy dog."
@@ -57,15 +95,16 @@
 
 - **Offloading**: you can offload parts of the model to CPU to reduce the cost of inference.
 
 - **Quantization**: you can quantize the model to reduce the cost of inference.
 
 For more details, please see the [documentation](https://opengpt.readthedocs.io/en/latest/).
 
-## Serving Models
+
+## Build a model serving in one line
 
 You can serve your models with OpenGPT. To do so, you can use the `serve` command:
 
 ```bash
 opengpt serve facebook/llama-9b --device cuda --precision fp16 --port 5000
 ```
 
@@ -102,15 +141,15 @@
             print(event)
     except ConnectionError:
         pass
 ```
 
 Note that the server will only accept requests from the same machine. If you want to accept requests from other machines, you can use the `--host` flag to specify the host to bind to.
 
-## Deploying Models
+## Cloud-native deployment
 
 You can also deploy the server to a cloud provider like Jina Cloud or AWS.
 To do so, you can use `deploy` command:
 
 - Jina Cloud
 
 ```bash
```

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/__init__.py` & `open_gpt_torch-0.0.1rc8/open_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/cli/application.py` & `open_gpt_torch-0.0.1rc8/open_gpt/cli/application.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/cli/commands/about.py` & `open_gpt_torch-0.0.1rc8/open_gpt/cli/commands/about.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/cli/commands/serve.py` & `open_gpt_torch-0.0.1rc8/open_gpt/cli/commands/serve.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     arguments = [argument("model_name", "The name of the model to serve.")]
     options = [
         option(
             "protocol",
             None,
             "The protocol to serve the model on.",
             flag=False,
-            default="grpc",
+            default="http",
         ),
         option(
             "port", "p", "The port to serve the model on.", flag=False, default=51000
         ),
         option(
             "replicas", "r", "The number of replicas to serve.", flag=False, default=1
         ),
@@ -28,15 +28,15 @@
     This command allows you to start a model serving locally.
     
     To start a model serving locally, you can run:
         
         <comment>opengpt serve facebook/llama-7b</comment>"""
 
     def handle(self) -> int:
-        from open_gpt.serve.flow import create_flow
+        from open_gpt.factory import create_flow
 
         with create_flow(
             self.argument('model_name'),
             protocol=self.option('protocol'),
             port=self.option('port'),
             replicas=self.option('replicas'),
         ) as flow:
```

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/factory.py` & `open_gpt_torch-0.0.1rc8/open_gpt/factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -91,7 +91,30 @@
         return BaseModel(
             model_name,
             device=device,
             precision=precision,
             device_map=device_map,
             **kwargs,
         )
+
+
+def create_flow(
+    model_name_or_path: str, protocol='http', port=51000, replicas: int = 1
+):
+    from jina import Flow
+
+    if 'flamingo' in model_name_or_path:
+        from .serve.executors.flamingo import FlamingoExecutor as Executor
+    else:
+        from serve.executors import CausualLMExecutor as Executor
+
+    # normalize the model name to be used as flow executor name
+    norm_name = model_name_or_path.split('/')[-1]
+    norm_name = norm_name.replace('-', '_').lower()
+
+    return Flow(protocol=protocol, port=port, cors=True).add(
+        uses=Executor,
+        uses_with={'model_name_or_path': model_name_or_path},
+        name=f'{norm_name}_executor',
+        replicas=replicas,
+        timeout_ready=-1,
+    )
```

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/helper.py` & `open_gpt_torch-0.0.1rc8/open_gpt/helper.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/flamingo_lm.py` & `open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         super().__init__()
         self.gated_cross_attn_layer = gated_cross_attn_layer
         self.decoder_layer = decoder_layer
         self.vis_x = None
         self.media_locations = None
         self.device = self.decoder_layer.parameters().__next__().device
 
-        # This is a hack to gaurantee that the gated_cross_attn_layer is on the same device as the decoder_layer
+        # This is a hack to guarantee that the gated_cross_attn_layer is on the same device as the decoder_layer
         if self.gated_cross_attn_layer is not None:
             self.gated_cross_attn_layer.to(self.device)
 
     def is_conditioned(self) -> bool:
         """Check whether the layer is conditioned."""
         return self.vis_x is not None
 
@@ -86,14 +86,15 @@
 
     def init_flamingo(
         self,
         media_token_id,
         vis_hidden_size,
         cross_attn_every_n_layers,
         use_media_placement_augmentation,
+        only_attend_previous: bool,
         device: Optional[Union[str, 'torch.device']] = None,
         dtype: Optional[Union[str, 'torch.dtype']] = None,
     ):
         """
         Initialize Flamingo by adding a new gated cross attn to the decoder. Store the media token id for computing the media locations.
         """
 
@@ -116,14 +117,15 @@
                     )
                 ]
             )
         )
         self.media_token_id = media_token_id
         self.use_media_placement_augmentation = use_media_placement_augmentation
         self.initialized_flamingo = True
+        self.only_attend_previous = only_attend_previous
 
         dtype, device = auto_dtype_and_device(dtype, device)
         if str(dtype) == 'torch.float16':
             self.gated_cross_attn_layers.half()
         # self.gated_cross_attn_layers.to(device)
 
     def forward(self, *input, **kwargs):
@@ -132,17 +134,19 @@
         if not self.initialized_flamingo:
             raise ValueError(
                 "Flamingo layers are not initialized. Please call `init_flamingo` first."
             )
 
         input_ids = kwargs["input_ids"] if "input_ids" in kwargs else input[0]
         media_locations = input_ids == self.media_token_id
-        attend_previous = (
-            (random.random() < 0.5) if self.use_media_placement_augmentation else False
-        )
+        # IMPORTANT: Force `attend_previous` to True when we place training data as <image>caption<|endofchunk|>
+        # attend_previous = (
+        #     (random.random() < 0.5) if self.use_media_placement_augmentation else False
+        # )
+        attend_previous = self.only_attend_previous
 
         for layer in self.get_decoder().layers:
             layer.condition_media_locations(media_locations)
             layer.condition_attend_previous(attend_previous)
 
         return super().forward(
             *input, **kwargs
```

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/flamingo_model.py` & `open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/flamingo_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Callable, Optional, Union
 
 import torch
+from accelerate.hooks import AlignDevicesHook, add_hook_to_module
 from einops import rearrange
 from open_flamingo.src.helpers import PerceiverResampler
 from torch import nn
 
 from open_gpt.logging import logger
 
 from ...helper import auto_dtype_and_device
@@ -52,15 +53,16 @@
             f"media_token_id: {self.media_token_id}, end_chunk_token_id: {self.end_chunk_token_id}"
         )
 
         self.lang_encoder.init_flamingo(
             media_token_id=self.media_token_id,
             vis_hidden_size=model_config['image_size'],
             cross_attn_every_n_layers=model_config['cross_attn_every_n_layers'],
-            use_media_placement_augmentation=False,
+            use_media_placement_augmentation=True,
+            only_attend_previous=True,
             dtype=dtype,
             device=device,
         )
 
     def forward(
         self,
         vision_inputs: 'torch.Tensor',
@@ -130,17 +132,26 @@
         :param num_return_sequences: number of return sequences. Defaults to 1.
         :param do_sample: whether to sample or not. Defaults to False.
         :param early_stopping: whether to stop early or not. Defaults to False.
 
         :return: text_inputs with generated tokens appended to it (batch_size, sequence_length)
         """
 
+        # if hasattr(self, "_hf_hook"):
+        # add a hook to make sure that the output of lang_encoder is mapped to the same device as the text_inputs
+        hook = AlignDevicesHook(
+            execution_device=self.device,
+            io_same_device=True,
+            place_submodules=False,
+        )
+        add_hook_to_module(self.lang_encoder, hook)
+
         vision_inputs = vision_inputs.to(dtype=self.dtype, device=self.device)
-        if attention_mask is not None:
-            attention_mask = attention_mask.to(self.device)
+        # if attention_mask is not None:
+        #     attention_mask = attention_mask.to(self.device)
         text_inputs = text_inputs.to(self.device)
 
         if num_beams > 1:
             vision_inputs = vision_inputs.repeat_interleave(num_beams, dim=0)
 
         _vision_x = self._vision_encode(vision_inputs=vision_inputs)
```

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/loading.py` & `open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/loading.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,22 +27,22 @@
     :param tokenizer_name_or_path: The name or path of the tokenizer to use. If not specified, the tokenizer associated with the model will be used.
     :param decoder_layers_attr_name: The name of the attribute that specifies the decoder layers.
     :param device: The device to load the model on.
     :param dtype: The dtype to load the model with.
     """
 
     from ...helper import cast_precision
-
-    # from ..llama.loading import (
-    #     load_model_and_tokenizer as load_llama_model_and_tokenizer,
-    # )
     from ..loading import load_model_and_tokenizer as load_llama_model_and_tokenizer
     from .flamingo_lm import FlamingoLMMixin
     from .flamingo_model import FlamingoLMModel
 
+    assert (
+        device_map is None
+    ), f"`device_map={device_map}` is not supported for Flamingo models"
+
     # load the vision model
     precision = cast_precision(dtype)
     model_name, *pretrained = vision_model_name_or_path.split("::")
     pretrained = pretrained[0] if len(pretrained) == 1 else 'openai'
     clip_model, _, image_processor = open_clip.create_model_and_transforms(
         model_name, pretrained=pretrained, device=device, precision=precision
     )
@@ -51,29 +51,39 @@
 
     # remove text encoder to save footprint and memory
     if hasattr(clip_model, 'text'):
         del clip_model.text
     elif hasattr(clip_model, 'transformer'):
         del clip_model.transformer
 
+    # patch to load llama models
+    if lang_model_name_or_path.startswith('facebook/llama'):
+        import os
+
+        model_size = lang_model_name_or_path.split('-')[-1]
+        if not os.path.exists(lang_model_name_or_path):
+            lang_model_name_or_path = f"decapoda-research/llama-{model_size}-hf"
+
     # load the language model
     lang_model, tokenizer = load_llama_model_and_tokenizer(
         model_name_or_path=lang_model_name_or_path,
         tokenizer_name_or_path=tokenizer_name_or_path,
         device=device,
         dtype=dtype,
-        device_map=None,  # TODO: fix this to support multi-gpu
+        device_map=device_map,
         no_split_module_classes=no_split_module_classes,
     )
 
     # add Flamingo special tokens to the tokenizer
     tokenizer.add_special_tokens(
         {"additional_special_tokens": ["<|endofchunk|>", "<image>"]}
     )
 
+    tokenizer.add_special_tokens({"pad_token": "<PAD>"})
+
     extend_instance(lang_model, FlamingoLMMixin)
 
     if decoder_layers_attr_name is None:
         decoder_layers_attr_name = _infer_decoder_layers_attr_name(lang_model)
     lang_model.set_decoder_layers_attr_name(decoder_layers_attr_name)
     lang_model.resize_token_embeddings(len(tokenizer))
```

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/modeling.py` & `open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/modeling.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,35 +17,39 @@
         self, model_name_or_path: str, tokenizer_name_or_path: Optional[str] = None
     ):
         from .loading import load_model_and_transforms
 
         self.model, self.tokenizer, self.image_processor = load_model_and_transforms(
             model_name_or_path,
             vision_model_name_or_path='ViT-L-14::openai',
-            lang_model_name_or_path='facebook/llama_7b',
+            lang_model_name_or_path='facebook/llama-7b',
             tokenizer_name_or_path=tokenizer_name_or_path,
             dtype=self._dtype,
             device=self._device,
             device_map=self._device_map,
             no_split_module_classes=self.no_split_module_classes,
         )
 
         self.model.eval()
 
-    def generate(self, prompt: str, interleave_images: List[bytes] = [], **kwargs):
+    def generate(self, prompt: str, inplace_images: List = [], **kwargs):
         """Generate text from the given prompt."""
 
         assert isinstance(prompt, str), "Prompt must be a string."
         prompt_len = len(prompt)
 
         with torch.inference_mode():
             vision_x = []
 
-            for image in interleave_images:
-                vision_x.append(self.image_processor(Image.open(image)).unsqueeze(0))
+            for image in inplace_images:
+                vision_x.append(
+                    self.image_processor(
+                        Image.open(image) if isinstance(image, str) else image
+                    ).unsqueeze(0)
+                )
             vision_x = torch.cat(vision_x, dim=0)
             vision_x = vision_x.unsqueeze(1).unsqueeze(0)
 
             lang_x = self.tokenizer(
                 [prompt],
                 padding=True,
                 return_tensors="pt",
```

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/models/flan/loading.py` & `open_gpt_torch-0.0.1rc8/open_gpt/models/flan/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/models/llama/modeling.py` & `open_gpt_torch-0.0.1rc8/open_gpt/models/llama/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/models/loading.py` & `open_gpt_torch-0.0.1rc8/open_gpt/models/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/models/modeling.py` & `open_gpt_torch-0.0.1rc8/open_gpt/models/modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     ):
         """Create a model of the given name."""
 
         super().__init__()
 
         self._dtype, self._device = auto_dtype_and_device(dtype, device)
 
-        self._device_map = device_map or 'balanced'
+        self._device_map = device_map
 
         self.load_model_and_transforms(
             model_name_or_path, tokenizer_name_or_path=tokenizer_name_or_path
         )
 
     def load_model_and_transforms(
         self, model_name_or_path: str, tokenizer_name_or_path: Optional[str] = None
```

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/models/pythia/loading.py` & `open_gpt_torch-0.0.1rc8/open_gpt/models/pythia/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/models/stablelm/modeling.py` & `open_gpt_torch-0.0.1rc8/open_gpt/models/stablelm/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/models/vicuna/loading.py` & `open_gpt_torch-0.0.1rc8/open_gpt/models/vicuna/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/models/vicuna/modeling.py` & `open_gpt_torch-0.0.1rc8/open_gpt/models/vicuna/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/profile.py` & `open_gpt_torch-0.0.1rc8/open_gpt/profile.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/serve/executors/base.py` & `open_gpt_torch-0.0.1rc8/open_gpt/serve/executors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,20 +34,20 @@
         self.model = create_model(
             model_name_or_path, precision=precision, device_map=device_map, **kwargs
         )
 
         # warmup the model to avoid the first-time slowness
         self.model.generate(['Hello world!'])
 
-    @requests
+    @requests(on='/generate')
     def generate(self, docs: 'DocumentArray', parameters: Dict = {}, **kwargs):
         prompted_da = DocumentArray(
-            [d for d in docs if d.tags.get('prompt') is not None]
+            [d for d in docs if d.tags.get('prompt') or d.text is not None]
         )
-        prompts = [d.tags['prompt'] for d in prompted_da]
+        prompts = [d.tags['prompt'] or d.text for d in prompted_da]
 
         if prompts:
             result = self.model.generate(prompts, **parameters)
             for d, r in zip(prompted_da, result):
                 d.tags['generated_text'] = r
         else:
             logger.warning('No prompts found in the request.')
```

### Comparing `open_gpt_torch-0.0.1rc7/open_gpt/serve/gateway.py` & `open_gpt_torch-0.0.1rc8/open_gpt/serve/gateway.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc7/pyproject.toml` & `open_gpt_torch-0.0.1rc8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open_gpt_torch"
-version = "0.0.1rc7"
+version = "0.0.1rc8"
 description = "An open-source implementation of large-scale language model (LLM)."
 
 license = "Apache-2.0"
 
 authors = [
     "Felix Wang <felix.wang@jina.ai>"
 ]
```

### Comparing `open_gpt_torch-0.0.1rc7/PKG-INFO` & `open_gpt_torch-0.0.1rc8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.1rc7
+Version: 0.0.1rc8
 Summary: An open-source implementation of large-scale language model (LLM).
 Home-page: https://open-gpt.jina.ai
 License: Apache-2.0
 Keywords: Pytorch,LLM,GPT
 Author: Felix Wang
 Author-email: felix.wang@jina.ai
 Requires-Python: >=3.8,<4.0
@@ -34,47 +34,85 @@
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Requires-Dist: transformers (>=4.28.0,<5.0.0)
 Project-URL: Repository, https://github.com/jina-ai/open_gpt
 Description-Content-Type: text/markdown
 
 # OpenGPT
 
+![](https://img.shields.io/badge/Made%20with-JinaAI-blueviolet?style=flat)
+[![PyPI](https://img.shields.io/pypi/v/open_gpt_torch)](https://pypi.org/project/open_gpt_torch/)
+[![PyPI - License](https://img.shields.io/pypi/l/open_gpt_torch)](https://pypi.org/project/open_gpt_torch/)
+
 `OpenGPT` is an open-source _cloud-native_ large **multi-modal models** (LMMs) serving solution. 
 It is designed to simplify the deployment and management of large language models, on a distributed cluster of GPUs.
 
 > **Note**
 > The content of `README.md` is just a placeholder to remind me of what I want to do.
 
+## Table of contents
+
+- [Features](#features)
+- [Supported models](#supported-models)
+- [Get started](#get-started)
+- [Build a model serving in one line](#build-a-model-serving-in-one-line)
+- [Cloud-native deployment](#cloud-native-deployment)
+  - [JCloud](#jcloud)
+  - [Kubernetes](#kubernetes)
+- [Roadmap](#roadmap)
+
 ## Features
 
 OpenGPT provides the following features to make it easy to deploy and serve large multi-modal models (LMMs) in production:
 
 - Support for multi-modal models
 - Scalable architecture for handling high traffic loads
 - Optimized for low-latency inference
 - Automatic model partitioning and distribution across multiple GPUs
 - Centralized model management and monitoring
 - REST API for easy integration with existing applications
 
-You can learn more about OpenGPT’s [architecture in our documentation](https://opengpt.readthedocs.io/en/latest/).
+## Updates
+
+- **2023-05-12**: 🎉 We have released the first version `v0.0.1` of OpenGPT. You can install it with `pip install open_gpt_torch`.
+
+## Supported Models
+
+OpenGPT supports the following models out of the box:
+
+- LLM (Large Language Model)
+
+  - [Llama](https://huggingface.co/facebook/llama-7b)
+  - [Pythia](https://huggingface.co/...)
+  - [StableLM](https://huggingface.co/...)
+  - [Vicuna](https://huggingface.co/...)
+  - [MOSS](https://huggingface.co/...)
+
+- LMM (Large Multi-modal Model)
+
+  - [OpenFlamingo](https://huggingface.co/...)
+  - [MiniGPT4](https://huggingface.co/...) (WIP)
+
+For more details about the supported models, please see the [Model Zoo](./MODEL_ZOO.md).
 
 
 ## Roadmap
 
 You can view our roadmap with features that are planned, started, and completed on the [Roadmap discussion](discussions/categories/roadmap) category.
 
-## Installation
+## Get Started
+
+### Installation
 
 Install the package with pip:
 
 ```bash
 pip install open_gpt_torch
 ```
 
-## Quickstart
+### Quickstart
 
 ```python
 import open_gpt
 
 model = open_gpt.create_model('facebook/llama-7b', device='cuda', precision='fp16')
 
 prompt = "The quick brown fox jumps over the lazy dog."
@@ -95,15 +133,16 @@
 
 - **Offloading**: you can offload parts of the model to CPU to reduce the cost of inference.
 
 - **Quantization**: you can quantize the model to reduce the cost of inference.
 
 For more details, please see the [documentation](https://opengpt.readthedocs.io/en/latest/).
 
-## Serving Models
+
+## Build a model serving in one line
 
 You can serve your models with OpenGPT. To do so, you can use the `serve` command:
 
 ```bash
 opengpt serve facebook/llama-9b --device cuda --precision fp16 --port 5000
 ```
 
@@ -140,15 +179,15 @@
             print(event)
     except ConnectionError:
         pass
 ```
 
 Note that the server will only accept requests from the same machine. If you want to accept requests from other machines, you can use the `--host` flag to specify the host to bind to.
 
-## Deploying Models
+## Cloud-native deployment
 
 You can also deploy the server to a cloud provider like Jina Cloud or AWS.
 To do so, you can use `deploy` command:
 
 - Jina Cloud
 
 ```bash
```

