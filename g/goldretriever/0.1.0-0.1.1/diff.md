# Comparing `tmp/goldretriever-0.1.0.tar.gz` & `tmp/goldretriever-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goldretriever-0.1.0.tar", max compression
+gzip compressed data, was "goldretriever-0.1.1.tar", max compression
```

## Comparing `goldretriever-0.1.0.tar` & `goldretriever-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1063 2023-05-08 12:32:32.769675 goldretriever-0.1.0/LICENSE
--rw-r--r--   0        0        0     4064 2023-05-08 12:32:32.769675 goldretriever-0.1.0/README.md
--rw-r--r--   0        0        0      288 2023-05-08 12:33:50.114694 goldretriever-0.1.0/goldretriever/.env
--rw-r--r--   0        0        0      760 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/.well-known/ai-plugin.json
--rw-r--r--   0        0        0      760 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/.well-known/default-ai-plugin.json
--rw-r--r--   0        0        0      836 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/.well-known/logo.png
--rw-r--r--   0        0        0     4737 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/.well-known/openapi.yaml
--rw-r--r--   0        0        0        0 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/__init__.py
--rw-r--r--   0        0        0       98 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/config.yml
--rw-r--r--   0        0        0        0 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/datastore/__init__.py
--rw-r--r--   0        0        0     3046 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/datastore/datastore.py
--rw-r--r--   0        0        0      143 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/datastore/executor/Dockerfile
--rw-r--r--   0        0        0        0 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/datastore/executor/__init__.py
--rw-r--r--   0        0        0      161 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/datastore/executor/config.yml
--rw-r--r--   0        0        0     3193 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/datastore/executor/docarray_v1.py
--rw-r--r--   0        0        0     1220 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/datastore/factory.py
--rw-r--r--   0        0        0      777 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/flow.yml
--rw-r--r--   0        0        0    11289 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/gateway.py
--rw-r--r--   0        0        0        0 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/models/__init__.py
--rw-r--r--   0        0        0      634 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/models/api.py
--rw-r--r--   0        0        0     1460 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/models/models.py
--rw-r--r--   0        0        0    10092 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/retriever.py
--rw-r--r--   0        0        0        0 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/scripts/__init__.py
--rw-r--r--   0        0        0     3016 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/scripts/process_json/README.md
--rw-r--r--   0        0        0        0 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/scripts/process_json/__init__.py
--rw-r--r--   0        0        0      630 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/scripts/process_json/example.json
--rw-r--r--   0        0        0     5356 2023-05-08 12:32:32.769675 goldretriever-0.1.0/goldretriever/scripts/process_json/process_json.py
--rw-r--r--   0        0        0     3091 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/scripts/process_jsonl/README.md
--rw-r--r--   0        0        0        0 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/scripts/process_jsonl/__init__.py
--rw-r--r--   0        0        0      879 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/scripts/process_jsonl/example.jsonl
--rw-r--r--   0        0        0     5253 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/scripts/process_jsonl/process_jsonl.py
--rw-r--r--   0        0        0     2699 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/scripts/process_zip/README.md
--rw-r--r--   0        0        0        0 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/scripts/process_zip/__init__.py
--rw-r--r--   0        0        0    53296 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/scripts/process_zip/example.zip
--rw-r--r--   0        0        0     5668 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/scripts/process_zip/process_zip.py
--rw-r--r--   0        0        0        0 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/services/__init__.py
--rw-r--r--   0        0        0     7609 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/services/chunks.py
--rw-r--r--   0        0        0      793 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/services/date.py
--rw-r--r--   0        0        0     1201 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/services/extract_metadata.py
--rw-r--r--   0        0        0     3674 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/services/file.py
--rw-r--r--   0        0        0     1879 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/services/openai.py
--rw-r--r--   0        0        0     1350 2023-05-08 12:32:32.773675 goldretriever-0.1.0/goldretriever/services/pii_detection.py
--rw-r--r--   0        0        0      997 2023-05-08 12:32:32.773675 goldretriever-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5412 1970-01-01 00:00:00.000000 goldretriever-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-11 10:43:06.373087 goldretriever-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4123 2023-05-11 10:43:06.373087 goldretriever-0.1.1/README.md
+-rw-r--r--   0        0        0      288 2023-05-11 10:44:22.866529 goldretriever-0.1.1/goldretriever/.env
+-rw-r--r--   0        0        0      758 2023-05-11 10:43:06.373087 goldretriever-0.1.1/goldretriever/.well-known/ai-plugin.json
+-rw-r--r--   0        0        0      760 2023-05-11 10:43:06.373087 goldretriever-0.1.1/goldretriever/.well-known/default-ai-plugin.json
+-rw-r--r--   0        0        0      836 2023-05-11 10:43:06.373087 goldretriever-0.1.1/goldretriever/.well-known/logo.png
+-rw-r--r--   0        0        0     4737 2023-05-11 10:43:06.373087 goldretriever-0.1.1/goldretriever/.well-known/openapi.yaml
+-rw-r--r--   0        0        0        0 2023-05-11 10:43:06.373087 goldretriever-0.1.1/goldretriever/__init__.py
+-rw-r--r--   0        0        0       98 2023-05-11 10:43:06.373087 goldretriever-0.1.1/goldretriever/config.yml
+-rw-r--r--   0        0        0        0 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/datastore/__init__.py
+-rw-r--r--   0        0        0     3046 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/datastore/datastore.py
+-rw-r--r--   0        0        0      143 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/datastore/executor/Dockerfile
+-rw-r--r--   0        0        0        0 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/datastore/executor/__init__.py
+-rw-r--r--   0        0        0      161 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/datastore/executor/config.yml
+-rw-r--r--   0        0        0     3193 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/datastore/executor/docarray_v1.py
+-rw-r--r--   0        0        0     1220 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/datastore/factory.py
+-rw-r--r--   0        0        0      777 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/flow.yml
+-rw-r--r--   0        0        0    11289 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/gateway.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/models/__init__.py
+-rw-r--r--   0        0        0      634 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/models/api.py
+-rw-r--r--   0        0        0     1460 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/models/models.py
+-rw-r--r--   0        0        0    10199 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/retriever.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/__init__.py
+-rw-r--r--   0        0        0     3016 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/process_json/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/process_json/__init__.py
+-rw-r--r--   0        0        0      630 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/process_json/example.json
+-rw-r--r--   0        0        0     5356 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/process_json/process_json.py
+-rw-r--r--   0        0        0     3091 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/process_jsonl/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/process_jsonl/__init__.py
+-rw-r--r--   0        0        0      879 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/process_jsonl/example.jsonl
+-rw-r--r--   0        0        0     5253 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/process_jsonl/process_jsonl.py
+-rw-r--r--   0        0        0     2699 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/process_zip/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/process_zip/__init__.py
+-rw-r--r--   0        0        0    53296 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/process_zip/example.zip
+-rw-r--r--   0        0        0     5668 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/scripts/process_zip/process_zip.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/services/__init__.py
+-rw-r--r--   0        0        0     7609 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/services/chunks.py
+-rw-r--r--   0        0        0      793 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/services/date.py
+-rw-r--r--   0        0        0     1201 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/services/extract_metadata.py
+-rw-r--r--   0        0        0     3674 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/services/file.py
+-rw-r--r--   0        0        0     1879 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/services/openai.py
+-rw-r--r--   0        0        0     1350 2023-05-11 10:43:06.377087 goldretriever-0.1.1/goldretriever/services/pii_detection.py
+-rw-r--r--   0        0        0      997 2023-05-11 10:43:06.377087 goldretriever-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5471 1970-01-01 00:00:00.000000 goldretriever-0.1.1/PKG-INFO
```

### Comparing `goldretriever-0.1.0/LICENSE` & `goldretriever-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/README.md` & `goldretriever-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Gold Retriever
+# 🐕 Gold Retriever
 
 Easily empower ChatGPT to store and analyze your data using `goldretriever`, a powerful command-line tool for creating and hosting retrieval plugins in just a few simple steps.
 
 
-## Quick Start
+## ⚡ Quick Start
 
-### Installation
+### 📦 Installation
 
 1. Ensure you have Python 3.8 or later.
 2. Install the tool via pip:
   ```bash
   pip install goldretriever
   ```
 
-### Deployment
+### 🚀 Deployment
 1. Run the following command to deploy the plugin:
 ```bash
 goldretriever deploy --key <your openai key>
 ```
 2. Store the "Gateway (Http)" URL and the Bearer token provided in the output.
 ```bash
 ╭──────────────────────── 🎉 Flow is available! ────────────────────────╮
@@ -26,15 +26,15 @@
 │   Gateway (Http)   https://retrieval-plugin-<plugin id>.wolf.jina.ai  │
 │   Dashboard        https://dashboard.wolf.jina.ai/flow/<plugin id>    │
 │                                                                       │
 ╰───────────────────────────────────────────────────────────────────────╯
 Bearer token: <your bearer token>
 ```
 
-### Data Indexing
+### 📚 Data Indexing
 1. Gather relevant text data files (PDF, TXT, DOCX, PPTX, or MD) in a directory.
 2. Index the data:
 ```bash
 goldretriever index --data my_files
 ```
   Or, use `docarray (v0.21.0)` for text data:
 ```python
@@ -45,53 +45,53 @@
 docs.save_binary('docs.bin')
 ```
 And then:
 ```bash
 goldretriever index --data docs.bin
 ```
 
-### Integration
+### 🔗 Integration
 1. Go to OpenAI Plugins.
 2. Select "Develop your own plugin".
 3. Enter the "Gateway (Http)" URL and Bearer token from the deployment step.
 
 
-## Advanced Usage
+## 🎛️ Advanced Usage
 
 
-### Configuration
+### 🛠️ Configuration
 To tailor the plugin to your needs, change the name and description during deployment:
 ```bash
 goldretriever deploy --key <your openai key> --name "Custom Name" --description "Custom description"
 ```
 If not specified, default values will be used.
 
 | Argument    | Description                                   | Default Value                                                                                                                                                                                                                               |
 |:------------|:----------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| name        | Human-readable name, such as the full company name	  | Retrieval Plugin                                                                                                                                                                                                                            |
+| name        | Human-readable name, such as the full company name	  | Gold Retriever                                                                                                                                                                                                                              |
 | description | Description better tailored to the model, such as token context length considerations or keyword usage for improved plugin prompting                                      | Plugin for searching through the user's documents (such as files, emails, and more) to find answers to questions and retrieve relevant information. Use it whenever a user asks something that might be found in their personal information |
 
 
 
-### Listing Plugins
+### 📋 Listing Plugins
 List your plugins and their status:
 ```bash
 goldretriever list
 ```
 
 Output:
 ```bash
 Plugin ID: ece735568f | Status: Serving
 ```
 
-### Deleting Plugins
+### ❌ Deleting Plugins
 Delete a plugin:
 ```bash
 goldretriever delete <plugin id>
 ```
 
-### Indexing Specific Plugins
+### 🔍 Indexing Specific Plugins
 Index data for a specific plugin:
 ```bash
 goldretriever index --data my_files --id <plugin_id>
 ```
 If the plugin ID is not specified, the last created plugin will be indexed.
```

### Comparing `goldretriever-0.1.0/goldretriever/.well-known/ai-plugin.json` & `goldretriever-0.1.1/goldretriever/.well-known/default-ai-plugin.json`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/.well-known/default-ai-plugin.json` & `goldretriever-0.1.1/goldretriever/.well-known/ai-plugin.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'name_for_human'": "'Gold Retriever'"}*

```diff
@@ -9,11 +9,11 @@
         "type": "user_http"
     },
     "contact_email": "hello@contact.com",
     "description_for_human": "Search through your documents.",
     "description_for_model": "Plugin for searching through the user's documents (such as files, emails, and more) to find answers to questions and retrieve relevant information. Use it whenever a user asks something that might be found in their personal information.",
     "legal_info_url": "hello@legal.com",
     "logo_url": "<your_url>/.well-known/logo.png",
-    "name_for_human": "Retrieval Plugin",
+    "name_for_human": "Gold Retriever",
     "name_for_model": "retrieval",
     "schema_version": "v1"
 }
```

### Comparing `goldretriever-0.1.0/goldretriever/.well-known/logo.png` & `goldretriever-0.1.1/goldretriever/.well-known/logo.png`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/.well-known/openapi.yaml` & `goldretriever-0.1.1/goldretriever/.well-known/openapi.yaml`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/datastore/datastore.py` & `goldretriever-0.1.1/goldretriever/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/datastore/executor/docarray_v1.py` & `goldretriever-0.1.1/goldretriever/datastore/executor/docarray_v1.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/datastore/factory.py` & `goldretriever-0.1.1/goldretriever/datastore/factory.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/flow.yml` & `goldretriever-0.1.1/goldretriever/flow.yml`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/gateway.py` & `goldretriever-0.1.1/goldretriever/gateway.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/models/api.py` & `goldretriever-0.1.1/goldretriever/models/api.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/models/models.py` & `goldretriever-0.1.1/goldretriever/models/models.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/retriever.py` & `goldretriever-0.1.1/goldretriever/retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             "key as an environment variable `RETRIEVAL_OPENAI_KEY` or "
             "provide it through the CLI `--openai-key <your key>`"
         )
     return openai_key
 
 
 def upsert_documents(docs, bearer_token, flow_id, n_docs=5):
-    print(f"Indexing documents into {flow_id}")
+    print(f"Indexing documents for {flow_id}")
     endpoint_url = f"https://{flow_id}.wolf.jina.ai/upsert"
     headers = {
         "accept": "application/json",
         "Content-Type": "application/json",
         "Authorization": f"Bearer {bearer_token}",
     }
     for batch in range(0, len(docs), n_docs):
@@ -141,29 +141,30 @@
                     },
                 }
             )
         response = requests.post(endpoint_url, headers=headers, json=data)
         if response.status_code != 200:
             print("Could not index the documents")
             print(response.text)
+    print(f"{len(docs)} documents have been successfully indexed!")
 
 
 def upsert_files(files, bearer_token, flow_id):
-    print(f"Indexing files into {flow_id}")
+    print(f"Indexing files for {flow_id}")
     endpoint_url = f"https://{flow_id}.wolf.jina.ai/upsert-file"
     headers = {
         "Authorization": f"Bearer {bearer_token}",
     }
     for file in files:
-        print(f"Indexing {file}")
-        files = {"file": (file, open(file, "rb"), mimetypes.guess_type(file)[0])}
-        response = requests.post(endpoint_url, headers=headers, files=files)
+        file_bytes = {"file": (file, open(file, "rb"), mimetypes.guess_type(file)[0])}
+        response = requests.post(endpoint_url, headers=headers, files=file_bytes)
         if response.status_code != 200:
             print("Could not index the file")
             print(response.text)
+    print(f"{len(files)} files have been successfully indexed!")
 
 
 @app.command()
 def index(
     data: str = typer.Option,
     bearer_token: Optional[str] = typer.Option(None),
     id: Optional[str] = typer.Option(None),
```

### Comparing `goldretriever-0.1.0/goldretriever/scripts/process_json/README.md` & `goldretriever-0.1.1/goldretriever/scripts/process_json/README.md`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/scripts/process_json/example.json` & `goldretriever-0.1.1/goldretriever/scripts/process_json/example.json`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/scripts/process_json/process_json.py` & `goldretriever-0.1.1/goldretriever/scripts/process_json/process_json.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/scripts/process_jsonl/README.md` & `goldretriever-0.1.1/goldretriever/scripts/process_jsonl/README.md`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/scripts/process_jsonl/example.jsonl` & `goldretriever-0.1.1/goldretriever/scripts/process_jsonl/example.jsonl`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/scripts/process_jsonl/process_jsonl.py` & `goldretriever-0.1.1/goldretriever/scripts/process_jsonl/process_jsonl.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/scripts/process_zip/README.md` & `goldretriever-0.1.1/goldretriever/scripts/process_zip/README.md`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/scripts/process_zip/example.zip` & `goldretriever-0.1.1/goldretriever/scripts/process_zip/example.zip`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/scripts/process_zip/process_zip.py` & `goldretriever-0.1.1/goldretriever/scripts/process_zip/process_zip.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/services/chunks.py` & `goldretriever-0.1.1/goldretriever/services/chunks.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/services/date.py` & `goldretriever-0.1.1/goldretriever/services/date.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/services/extract_metadata.py` & `goldretriever-0.1.1/goldretriever/services/extract_metadata.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/services/file.py` & `goldretriever-0.1.1/goldretriever/services/file.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/services/openai.py` & `goldretriever-0.1.1/goldretriever/services/openai.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/goldretriever/services/pii_detection.py` & `goldretriever-0.1.1/goldretriever/services/pii_detection.py`

 * *Files identical despite different names*

### Comparing `goldretriever-0.1.0/pyproject.toml` & `goldretriever-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goldretriever"
-version = "0.1.0"
+version = "0.1.1"
 description = "Create and host retrieval plugins for ChatGPT in one click"
 authors = ["saba <saba.sturua@jina.ai>", "johannes <johannes.messner@jina.ai>"]
 readme = "README.md"
 include = ["goldretriever/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `goldretriever-0.1.0/PKG-INFO` & `goldretriever-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goldretriever
-Version: 0.1.0
+Version: 0.1.1
 Summary: Create and host retrieval plugins for ChatGPT in one click
 Author: saba
 Author-email: saba.sturua@jina.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,30 +29,30 @@
 Requires-Dist: tiktoken (>=0.3.1,<0.4.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Requires-Dist: urllib3 (>=1.26.7,<2.0.0)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
 Requires-Dist: wheel (>=0.37.0,<0.38.0)
 Description-Content-Type: text/markdown
 
-# Gold Retriever
+# 🐕 Gold Retriever
 
 Easily empower ChatGPT to store and analyze your data using `goldretriever`, a powerful command-line tool for creating and hosting retrieval plugins in just a few simple steps.
 
 
-## Quick Start
+## ⚡ Quick Start
 
-### Installation
+### 📦 Installation
 
 1. Ensure you have Python 3.8 or later.
 2. Install the tool via pip:
   ```bash
   pip install goldretriever
   ```
 
-### Deployment
+### 🚀 Deployment
 1. Run the following command to deploy the plugin:
 ```bash
 goldretriever deploy --key <your openai key>
 ```
 2. Store the "Gateway (Http)" URL and the Bearer token provided in the output.
 ```bash
 ╭──────────────────────── 🎉 Flow is available! ────────────────────────╮
@@ -61,15 +61,15 @@
 │   Gateway (Http)   https://retrieval-plugin-<plugin id>.wolf.jina.ai  │
 │   Dashboard        https://dashboard.wolf.jina.ai/flow/<plugin id>    │
 │                                                                       │
 ╰───────────────────────────────────────────────────────────────────────╯
 Bearer token: <your bearer token>
 ```
 
-### Data Indexing
+### 📚 Data Indexing
 1. Gather relevant text data files (PDF, TXT, DOCX, PPTX, or MD) in a directory.
 2. Index the data:
 ```bash
 goldretriever index --data my_files
 ```
   Or, use `docarray (v0.21.0)` for text data:
 ```python
@@ -80,54 +80,54 @@
 docs.save_binary('docs.bin')
 ```
 And then:
 ```bash
 goldretriever index --data docs.bin
 ```
 
-### Integration
+### 🔗 Integration
 1. Go to OpenAI Plugins.
 2. Select "Develop your own plugin".
 3. Enter the "Gateway (Http)" URL and Bearer token from the deployment step.
 
 
-## Advanced Usage
+## 🎛️ Advanced Usage
 
 
-### Configuration
+### 🛠️ Configuration
 To tailor the plugin to your needs, change the name and description during deployment:
 ```bash
 goldretriever deploy --key <your openai key> --name "Custom Name" --description "Custom description"
 ```
 If not specified, default values will be used.
 
 | Argument    | Description                                   | Default Value                                                                                                                                                                                                                               |
 |:------------|:----------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| name        | Human-readable name, such as the full company name	  | Retrieval Plugin                                                                                                                                                                                                                            |
+| name        | Human-readable name, such as the full company name	  | Gold Retriever                                                                                                                                                                                                                              |
 | description | Description better tailored to the model, such as token context length considerations or keyword usage for improved plugin prompting                                      | Plugin for searching through the user's documents (such as files, emails, and more) to find answers to questions and retrieve relevant information. Use it whenever a user asks something that might be found in their personal information |
 
 
 
-### Listing Plugins
+### 📋 Listing Plugins
 List your plugins and their status:
 ```bash
 goldretriever list
 ```
 
 Output:
 ```bash
 Plugin ID: ece735568f | Status: Serving
 ```
 
-### Deleting Plugins
+### ❌ Deleting Plugins
 Delete a plugin:
 ```bash
 goldretriever delete <plugin id>
 ```
 
-### Indexing Specific Plugins
+### 🔍 Indexing Specific Plugins
 Index data for a specific plugin:
 ```bash
 goldretriever index --data my_files --id <plugin_id>
 ```
 If the plugin ID is not specified, the last created plugin will be indexed.
```

