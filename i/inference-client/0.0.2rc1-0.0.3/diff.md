# Comparing `tmp/inference_client-0.0.2rc1.tar.gz` & `tmp/inference_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference_client-0.0.2rc1.tar", max compression
+gzip compressed data, was "inference_client-0.0.3.tar", max compression
```

## Comparing `inference_client-0.0.2rc1.tar` & `inference_client-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-04-10 13:14:50.023323 inference_client-0.0.2rc1/LICENSE
--rw-r--r--   0        0        0    12002 2023-04-10 13:14:50.023323 inference_client-0.0.2rc1/README.md
--rw-r--r--   0        0        0       27 2023-04-10 13:14:50.027323 inference_client-0.0.2rc1/inference_client/__init__.py
--rw-r--r--   0        0        0      443 2023-04-10 13:14:50.027323 inference_client-0.0.2rc1/inference_client/__version__.py
--rw-r--r--   0        0        0     9590 2023-04-10 13:14:50.027323 inference_client-0.0.2rc1/inference_client/base.py
--rw-r--r--   0        0        0      990 2023-04-10 13:14:50.027323 inference_client-0.0.2rc1/inference_client/client.py
--rw-r--r--   0        0        0     5142 2023-04-10 13:14:50.027323 inference_client-0.0.2rc1/inference_client/helper.py
--rw-r--r--   0        0        0     1316 2023-04-10 13:14:50.027323 inference_client-0.0.2rc1/pyproject.toml
--rw-r--r--   0        0        0    24300 1970-01-01 00:00:00.000000 inference_client-0.0.2rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-11 07:17:40.737259 inference_client-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7176 2023-05-11 07:17:40.737259 inference_client-0.0.3/README.md
+-rw-r--r--   0        0        0      101 2023-05-11 07:17:40.797263 inference_client-0.0.3/inference_client/__init__.py
+-rw-r--r--   0        0        0      373 2023-05-11 07:17:40.797263 inference_client-0.0.3/inference_client/__version__.py
+-rw-r--r--   0        0        0      499 2023-05-11 07:17:40.797263 inference_client-0.0.3/inference_client/base.py
+-rw-r--r--   0        0        0      991 2023-05-11 07:17:40.797263 inference_client-0.0.3/inference_client/client.py
+-rw-r--r--   0        0        0      719 2023-05-11 07:17:40.797263 inference_client-0.0.3/inference_client/config.py
+-rw-r--r--   0        0        0     3191 2023-05-11 07:17:40.797263 inference_client-0.0.3/inference_client/helper.py
+-rw-r--r--   0        0        0      250 2023-05-11 07:17:40.797263 inference_client-0.0.3/inference_client/logging.py
+-rw-r--r--   0        0        0     3522 2023-05-11 07:17:40.797263 inference_client-0.0.3/inference_client/tasks/caption.py
+-rw-r--r--   0        0        0     5819 2023-05-11 07:17:40.797263 inference_client-0.0.3/inference_client/tasks/encode.py
+-rw-r--r--   0        0        0     2378 2023-05-11 07:17:40.797263 inference_client-0.0.3/inference_client/tasks/helper.py
+-rw-r--r--   0        0        0     6127 2023-05-11 07:17:40.797263 inference_client-0.0.3/inference_client/tasks/rank.py
+-rw-r--r--   0        0        0     3904 2023-05-11 07:17:40.797263 inference_client-0.0.3/inference_client/tasks/vqa.py
+-rw-r--r--   0        0        0     1355 2023-05-11 07:17:40.797263 inference_client-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    19556 1970-01-01 00:00:00.000000 inference_client-0.0.3/PKG-INFO
```

### Comparing `inference_client-0.0.2rc1/LICENSE` & `inference_client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.2rc1/pyproject.toml` & `inference_client-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inference_client"
-version = "0.0.2rc1"
+version = "0.0.3"
 description = "Python Client for Jina Inference API"
 
 license = "Apache-2.0"
 
 authors = [
     "Jina AI <hello@jina.ai>"
 ]
@@ -27,14 +27,16 @@
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 # Compatible Python versions
 python = ">=3.8,<4.0.0"
+pydantic = "^1.10.7"
+docarray = "^0.21.0"
 jina  = "^3.14.0"
 jina-hubble-sdk = ">=0.34.0"
 rich = "^13.3.0"
 pillow = "^9.4.0"
 torch = {version = ">=1.10.0", optional = true}
 
 [tool.poetry.extras]
```

### Comparing `inference_client-0.0.2rc1/PKG-INFO` & `inference_client-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: inference-client
-Version: 0.0.2rc1
+Version: 0.0.3
 Summary: Python Client for Jina Inference API
 Home-page: https://inference-api.jina.ai
 License: Apache-2.0
 Keywords: jina,inference,api,client
 Author: Jina AI
 Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: pytorch
+Requires-Dist: docarray (>=0.21.0,<0.22.0)
 Requires-Dist: jina (>=3.14.0,<4.0.0)
 Requires-Dist: jina-hubble-sdk (>=0.34.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: rich (>=13.3.0,<14.0.0)
 Requires-Dist: torch (>=1.10.0) ; extra == "pytorch"
 Project-URL: Repository, https://github.com/jina-ai/inference-client
 Description-Content-Type: text/markdown
 
-# Inference Client
+![Inference Client](/.github/README-img/inference_client.svg)
 
 [![PyPI](https://img.shields.io/pypi/v/inference-client)](https://pypi.org/project/inference-client/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/inference-client)](https://pypi.org/project/inference-client/)
 [![PyPI - License](https://img.shields.io/pypi/l/inference-client)](https://pypi.org/project/inference-client/)
 
 Inference Client is a library that provides a simple and efficient way to use Jina AI's Inference, a powerful platform that offers a range of AI models for common tasks such as visual reasoning, question answering, and embedding modalities like texts and images. 
 With Inference Client, you can easily select the task and model of your choice and integrate the API call into your workflow with zero technical overhead. 
@@ -38,19 +40,19 @@
 
 🔍 **Rank**: Re-rank cross-modal matches according to their joint likelihood
 
 📷 **Caption**: Generate captions for images 
 
 🤔 **VQA**: Answer questions related to images 
 
-In addition to these tasks, the client provides the ability to connect to the inference server and user authentication.
 
 ## Installation
 
-Please note that Inference Client requires Python 3.8 or higher. Inference Client can be installed via pip by executing:
+Inference Client is available on PyPI and can be installed using pip:
+
 ```bash
 pip install inference-client
 ```
 
 ## Getting Started
 
 Before using Inference Client, please create an inference on [Jina AI Cloud](https://cloud.jina.ai/user/inference).
@@ -58,187 +60,96 @@
 After login with your Jina AI Cloud account, you can create an inference by clicking the "Create" button in the inference page.
 From there, you can select the model you want to use.
 
 After the inference is created and the status is "Serving", you can use Inference Client to connect to it.
 This could take a few minutes, depending on the model you selected.
 
 <p align="center">
-    <img src=".github/README-img/jac.png">
+    <img src=".github/README-img/jac.png" width="100%">
 </p>
 
 ### Client Initialization
 
-To initialize the Client object and connect to the inference server, you can choose to pass a valid personal access token to the token parameter.
-A personal access token can be generated at the [Jina AI Cloud](https://cloud.jina.ai/settings/tokens), or via CLI as described in [this guide](https://docs.jina.ai/jina-ai-cloud/login/#create-a-new-pat):
-```bash
-jina auth token create <name of PAT> -e <expiration days>
-```
-
-To pass the token to the client, you can use the following code snippet:
+To use Inference Client, you need to initialize a Client object with the authentication token of your Jina AI Cloud account:
 
 ```python
 from inference_client import Client
 
-# Initialize client with valid token
-client = Client(token='<your token>')
+client = Client(token='<your auth token>')
 ```
 
-If you don't provide a token explicitly, Inference Client will look for a `JINA_AUTH_TOKEN` environment variable, otherwise it will try to authenticate via browser.
-
-```python
-from inference_client import Client
-
-client = Client()
+The token can be generated at the [Jina AI Cloud](https://cloud.jina.ai/settings/tokens), or via CLI as described in [this guide](https://docs.jina.ai/jina-ai-cloud/login/#create-a-new-pat):
+```bash
+jina auth token create <name of PAT> -e <expiration days>
 ```
 
-Please note that while it's possible to login via the Jina AI web UI, this method is intended primarily for development and testing purposes. 
-For production use, we recommend obtaining a long-lived token via the Jina AI web API and providing it to the Client object explicitly. 
-Tokens have a longer lifetime than web sessions and can be securely stored and managed, making them a more suitable choice for production environments.
 
-### Selecting the Model
+### Connecting to Models
 
-To select an inference model, you can use the get_model method of the Client object and specify the name of the model as it appears in Jina AI Cloud. 
-You can connect to as many inference models as you want once they have been created on Jina AI Cloud, and you can use them for multiple tasks.
+Once you have initialized the Client object, you can connect to the models you want to use by calling the `get_model` method, which takes the name of the model as it appears in Jina AI Cloud as an argument.
 
-Here's an example of how to connect to two models and encode some text using each of them:
-    
 ```python
-from inference_client import Client
-
-# Initialize client
-inference_client = Client()
-
-# Connect to CLIP model
-clip_model = inference_client.get_model('ViT-B-32::openai')
-clip_embed = clip_model.encode(text='hello world')[0].embedding
-
-# Connect to BLIP2 model
-blip2_model = inference_client.get_model('Salesforce/blip2-opt-2.7b')
-blip2_embed = blip2_model.encode(text='hello jina')[0].embedding
+# connect to a CLIP model
+model = client.get_model('ViT-B-32::openai')
 ```
+As example, the above code connects to the CLIP model named "ViT-B-32::openai" on Jina AI Cloud.
 
-Now it's time to use the models to perform some tasks!
-We will use the Singapore Skyline with Merlion in the foreground as an example image for the rest of the examples.
-
-<p align="center">
-    <img src=".github/README-img/Singapore_Skyline_2019-10.jpeg" width="50%">
-</p>
-
-### Encoding
-
-To use the encode method of an inference model, you need to initialize the model and provide input data as DocumentArray, plain text, or an image. 
-
-Here are some examples of how to use the encode method:
-
-1. Encode plain text:
-
-```python
-from inference_client import Client
-
-# Initialize client
-inference_client = Client()
+You can connect to as many inference models as you want once they have been created on Jina AI Cloud, and you can use them for multiple tasks.
 
-# Connect to CLIP model
-model = inference_client.get_model('<inference model name>')
 
-# Encode the documents
-response = model.encode(text='hello world')
+### Performing tasks
 
-# Access the embeddings
-print(response[0].embedding)
-```
+Now that you have connected to the models, you can use them to perform the tasks they support.
 
-```bash
-[-5.48706055e-02 -1.10717773e-01  5.13671875e-01 -3.22509766e-01
- -1.40380859e-01  6.23535156e-01  3.07617188e-01  4.26025391e-01
-  ...
-  8.04443359e-02  8.53515625e-01 -5.96008301e-02  3.61633301e-02]
-```
 
-2. Encode an image:
+#### 1. Encoding
 
+The encode task is used to encode data into embeddings using various models.
+For example, you can use the CLIP model to encode text or images into embeddings:
+    
 ```python
-# Encode image URL
-response = model.encode(image='singapore.jpg')
-
-# Access the embedding
-print(response[0].embedding)
+model = client.get_model(
+    '<name of the model that supports encode>'
+)  # e.g. ViT-B-32::openai
 
-# Encode image binary data
-image_bytes = open('singapore.jpg', 'rb').read()
-response = model.encode(image=image_bytes)
+# encode text
+result = model.encode(text='hello world')
 
-# Access the embedding
-print(response[0].embedding)
+# encode image
+result = model.encode(image='hello_world.jpg')
 
-# Encode image tensor data
+# encode image RGB tensor
 from PIL import Image
 from numpy import asarray
 
-image_bytes = Image.open('singapore.jpg')
+image_bytes = Image.open('hello_world.jpg')
 image_tensor = asarray(image_bytes)
-response = model.encode(image=image_tensor)
-
-# Access the embedding
-print(response[0].embedding)
+result = model.encode(image=image_tensor)
 ```
 
-```bash
-
-[-1.70776367e-01 -4.17236328e-01  2.29370117e-01  1.95770264e-02
- -5.86914062e-01  1.30981445e-01 -2.38037109e-01 -1.24328613e-01
-  ...
-  2.59277344e-01  7.36694336e-02  4.23339844e-01 -2.92480469e-01]
-```
-
-3. Encode a `DocumentArray`:
-
-```python
-from docarray import Document, DocumentArray
-
-# Create a DocumentArray with two documents
-docs = DocumentArray([Document(text='hello world'), Document(uri='singapore.jpg')])
-
-# Encode the documents
-response = model.encode(docs=docs)
-
-# Access the embeddings
-for doc in response:
-    print(doc.embedding)
-```
+The output of the encode method is a DocumentArray, which contains the embeddings of the input data.
 
 ```bash
+# print(result[0].embedding)
+
 [-5.48706055e-02 -1.10717773e-01  5.13671875e-01 -3.22509766e-01
  -1.40380859e-01  6.23535156e-01  3.07617188e-01  4.26025391e-01
   ...
   8.04443359e-02  8.53515625e-01 -5.96008301e-02  3.61633301e-02]
-[ 1.26416489e-01  2.53842145e-01  1.32031530e-01 -6.55740649e-02
-  3.77700478e-01  1.34678692e-01  1.94542333e-01  6.93580136e-04
-  ...
-  1.24198742e-01  2.51199156e-02 -1.18231498e-01  1.66848406e-01]
 ```
 
-### Ranking
+### 2. Ranking
 
-To perform similarity-based ranking of candidate matches, you can use the rank method of an inference model. 
+To perform similarity-based ranking of candidate matches, you can use the `rank` method of an inference model. 
 The rank method takes a reference input and a list of candidates, and reorder that list of candidates based on their similarity to the reference input. 
-You can also construct a cross-modal Document where the root contains an image or text and .matches contain images or sentences to rerank.
-
-Here are some examples of how to use the rank method:
-
-1. Rank plain input:
+You can also construct a cross-modal Document where the root contains an image or text and `.matches` contain images or sentences to rerank.
 
 ```python
-from inference_client import Client
-
-# Initialize client
-inference_client = Client()
-
-# Initialize model
-model = Client().get_model('<inference model name>')
+# Connect to a model
+model = client.get_model('<name of the model that supports rank>')
 
 reference = 'singapore.jpg'
 candidates = [
     'a colorful photo of nature',
     'a photo of blue scenery',
     'a black and white photo of a cat',
 ]
@@ -252,163 +163,68 @@
 ```bash
 a photo of blue scenery
 a colorful photo of nature
 a black and white photo of a cat
 ```
 You may also input images as bytes or tensors similarly to the encode method.
 
-2. Rank a `DocumentArray`:
-
-```python
-from docarray import Document, DocumentArray
+**NOTICE**: The following tasks Caption and VQA are BLIP2 exclusive. Calling these methods on other models will fall back to the default encode method.
 
-# Create a DocumentArray with a single document and some candidate matches
-docs = DocumentArray(
-    [
-        Document(
-            uri='singapore.jpg',
-            matches=DocumentArray(
-                [
-                    Document(text='a colorful photo of nature'),
-                    Document(text='a photo of blue scenery'),
-                    Document(text='a black and white photo of a cat'),
-                ]
-            ),
-        ),
-    ]
-)
+### 3. Captioning
 
-# Rank the documents
-response = model.rank(docs=docs)
+You can use caption method to generate natural language descriptions of images.
 
-# Access the matches
-for match in not response[0]:
-    print(match.text)
-```
 
-```bash
-a photo of blue scenery
-a colorful photo of nature
-a black and white photo of a cat
-```
-
-**NOTICE**: The following tasks Caption and VQA are BLIP2 exclusive. Calling these methods on other models will fall back to the default encode method.
-
-### Captioning
-
-You can use caption to generate natural language descriptions of images.
 The caption method takes a DocumentArray containing images or a single plain image as input.
 The plain input image can be in the form of a URL string, an image blob, or an image tensor.
 
-Here are some examples of how to use the caption method:
-
-1. Caption plain input:
+For example, you can use the BLIP2 model to generate captions for images:
 
 ```python
-from inference_client import Client
-
-# Initialize client
-inference_client = Client()
-
 # Initialize model
-model = Client().get_model('<inference model name>')
+model = client.get_model('Salesforce/blip2-opt-2.7b')
 
 response = model.caption(image='singapore.jpg')
 
 # Access the captions
 print(response[0].tags['response'])
 ```
 
 ```bash
 the merlion fountain in singapore at night
 ```
 
-You may also input images as bytes or tensors similarly to the encode method.
-
-2. Caption a `DocumentArray`:
 
-```python
-from docarray import Document, DocumentArray
-
-# Create a DocumentArray with a single image document
-docs = DocumentArray([Document(uri='singapore.jpg')])
-
-# Caption the documents
-response = model.caption(docs=docs)
-
-# Access the captions
-for doc in response:
-    print(doc.tags['response'])
-```
-
-```bash
-the merlion fountain in singapore at night
-```
-
-### Visual Question Answering
+### 4. VQA (Visual Question Answering)
 
 Visual Question Answering (VQA) is a task that involves answering natural language questions about visual content such as images. 
 Given an image and a question, the goal of VQA is to provide a natural language answer.
 The VQA method takes either a DocumentArray of images and questions, or a single plain image and question.
 
-Here are some examples of how to use the VQA method:
-
-2. VQA plain input:
 
 ```python
-from inference_client import Client
-
-# Initialize client
-inference_client = Client()
-
 # Initialize model
-model = Client().get_model('<inference model name>')
+model = client.get_model('Salesforce/blip2-opt-2.7b')
 
 image = 'singapore.jpg'
 question = 'Question: What is this photo about? Answer:'
 
 response = model.vqa(image=image, question=question)
 
 # Access the answers
 print(response[0].tags['response'])
 ```
 
 ```bash
 the merlion fountain in singapore
 ```
 
-You may also input images as bytes or tensors similarly to the encode method.
-Please notice that due to the limitation of the current model, the question must start with 'Question:' and end with 'Answer:'.
-
-2. VQA a `DocumentArray`:
-
-```python
-from docarray import Document, DocumentArray
-
-# Create a DocumentArray with one document
-docs = DocumentArray(
-    [
-        Document(
-            uri='singapore.jpg',
-            tags={'prompt': 'Question: What is this photo about? Answer:'},
-        )
-    ]
-)
-
-# VQA the documents
-response = model.vqa(docs=docs)
+## Documentation
 
-# Access the answers
-for doc in response:
-    print(doc.tags['response'])
-```
-
-```bash
-the merlion fountain in singapore
-```
+For more information about advanced usage of Inference Client, please refer to the [documentation](https://docs.jina.ai/advanced/experimental/inference-client/).
 
 ## Support
 
 - Join our [Slack community](https://slack.jina.ai) and chat with other community members about ideas.
 - Watch our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) to learn Jina's new features and stay up-to-date with the latest AI techniques.
 - Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
```

