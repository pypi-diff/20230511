# Comparing `tmp/lazycodr-0.1.0.tar.gz` & `tmp/lazycodr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazycodr-0.1.0.tar", max compression
+gzip compressed data, was "lazycodr-0.1.1.tar", max compression
```

## Comparing `lazycodr-0.1.0.tar` & `lazycodr-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-09 20:52:17.876561 lazycodr-0.1.0/README.md
--rw-r--r--   0        0        0      894 2023-05-11 09:18:57.221843 lazycodr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      435 2023-05-11 09:19:38.169467 lazycodr-0.1.0/src/lazycodr/cli/__init__.py
--rw-r--r--   0        0        0      703 2023-05-09 21:08:17.804679 lazycodr-0.1.0/src/lazycodr/cli/config.py
--rw-r--r--   0        0        0      841 2023-05-10 23:34:39.649616 lazycodr-0.1.0/src/lazycodr/cli/pr.py
--rw-r--r--   0        0        0      126 2023-05-10 23:26:25.337695 lazycodr-0.1.0/src/lazycodr/contants.py
--rw-r--r--   0        0        0      513 2023-05-10 23:26:05.445197 lazycodr-0.1.0/src/lazycodr/prompts/__init__.py
--rw-r--r--   0        0        0      295 2023-05-11 09:20:09.661178 lazycodr-0.1.0/src/lazycodr/prompts/templates/pr-generate-refine-init.jinja
--rw-r--r--   0        0        0      586 2023-05-11 09:20:09.661178 lazycodr-0.1.0/src/lazycodr/prompts/templates/pr-generate-refine-loop.jinja
--rw-r--r--   0        0        0     2947 2023-05-11 09:18:03.758339 lazycodr-0.1.0/src/lazycodr/utils.py
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 lazycodr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3282 2023-05-11 10:38:38.530131 lazycodr-0.1.1/README.md
+-rw-r--r--   0        0        0      993 2023-05-11 11:47:31.284359 lazycodr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      435 2023-05-11 09:19:38.169467 lazycodr-0.1.1/src/lazycodr/cli/__init__.py
+-rw-r--r--   0        0        0      708 2023-05-11 11:37:46.377666 lazycodr-0.1.1/src/lazycodr/cli/config.py
+-rw-r--r--   0        0        0      841 2023-05-10 23:34:39.649616 lazycodr-0.1.1/src/lazycodr/cli/pr.py
+-rw-r--r--   0        0        0      126 2023-05-10 23:26:25.337695 lazycodr-0.1.1/src/lazycodr/constants.py
+-rw-r--r--   0        0        0      513 2023-05-10 23:26:05.445197 lazycodr-0.1.1/src/lazycodr/prompts/__init__.py
+-rw-r--r--   0        0        0      295 2023-05-11 09:20:09.661178 lazycodr-0.1.1/src/lazycodr/prompts/templates/pr-generate-refine-init.jinja
+-rw-r--r--   0        0        0      586 2023-05-11 09:20:09.661178 lazycodr-0.1.1/src/lazycodr/prompts/templates/pr-generate-refine-loop.jinja
+-rw-r--r--   0        0        0     2961 2023-05-11 10:16:40.893987 lazycodr-0.1.1/src/lazycodr/utils.py
+-rw-r--r--   0        0        0     4244 1970-01-01 00:00:00.000000 lazycodr-0.1.1/PKG-INFO
```

### Comparing `lazycodr-0.1.0/pyproject.toml` & `lazycodr-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
+[build-system]
+build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core"]
+
+[tool.black]
+line-length = 88
+
+[tool.isort]
+profile = "black"
+
 [tool.poetry]
-name = "lazycodr"
-version = "0.1.0"
-description = "A CLI tool to help lazy coders get the work done with AI (commit messages, pull requests ...)"
 authors = ["JimZer <jimi.vaubien@protonmail.com>"]
+description = "A CLI tool to help lazy coders get the work done with AI (commit messages, pull requests ...)"
+name = "lazycodr"
+packages = [{include = "lazycodr", from = "src"}]
 readme = "README.md"
-packages = [ { include = "lazycodr", from = "src" } ]
+version = "0.1.1"
+repository = "https://github.com/bitswired/lazycodr"
+homepage = "https://github.com/bitswired/lazycodr"
 
 [tool.poetry.dependencies]
-python = "^3.10"
-typer = {extras = ["all"], version = "^0.9.0"}
-pygithub = "^1.58.2"
-langchain = "^0.0.163"
-rich = "^13.3.5"
-pyfiglet = "^0.8.post1"
 httpx = "^0.24.0"
-openai = "^0.27.6"
-tiktoken = "^0.4.0"
 jinja2 = "^3.1.2"
+langchain = "^0.0.163"
+openai = "^0.27.6"
 pydantic = "^1.10.7"
-
+pyfiglet = "^0.8.post1"
+pygithub = "^1.58.2"
+python = "^3.10"
+rich = "^13.3.5"
+tiktoken = "^0.4.0"
+typer = {extras = ["all"], version = "^0.9.0"}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
+flake8 = "^6.0.0"
 isort = "^5.12.0"
-pytest = "^7.3.1"
 pre-commit = "^3.3.1"
-flake8 = "^6.0.0"
+pytest = "^7.3.1"
 
 [tool.poetry.scripts]
 lazycodr = "lazycodr.cli:main"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-
-[tool.black]
-line-length = 88
-
-[tool.isort]
-profile = "black"
```

### Comparing `lazycodr-0.1.0/src/lazycodr/cli/config.py` & `lazycodr-0.1.1/src/lazycodr/cli/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 app = typer.Typer()
 
 console = Console()
 
 
 @app.command()
-def config(
+def credentials(
     openai_api_key: Annotated[str, typer.Option(prompt=True, hide_input=True)],
     github_token: Annotated[str, typer.Option(prompt=True, hide_input=True)],
 ):
     # Save credentials to file json
     credentials = {
         "openai_api_key": openai_api_key,
         "github_token": github_token,
```

### Comparing `lazycodr-0.1.0/src/lazycodr/cli/pr.py` & `lazycodr-0.1.1/src/lazycodr/cli/pr.py`

 * *Files identical despite different names*

### Comparing `lazycodr-0.1.0/src/lazycodr/prompts/__init__.py` & `lazycodr-0.1.1/src/lazycodr/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `lazycodr-0.1.0/src/lazycodr/prompts/templates/pr-generate-refine-loop.jinja` & `lazycodr-0.1.1/src/lazycodr/prompts/templates/pr-generate-refine-loop.jinja`

 * *Files identical despite different names*

### Comparing `lazycodr-0.1.0/src/lazycodr/utils.py` & `lazycodr-0.1.1/src/lazycodr/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from github import Github
 from langchain import LLMChain, PromptTemplate
 from langchain.chains.combine_documents.refine import RefineDocumentsChain
 from langchain.chat_models import ChatOpenAI
 from langchain.text_splitter import TokenTextSplitter
 from rich.console import Console
 
-from lazycodr.contants import PR_REFINE_INIT_TEMPLATE_NAME, PR_REFINE_LOOP_TEMPLATE_NAME
+from lazycodr.constants import (
+    PR_REFINE_INIT_TEMPLATE_NAME,
+    PR_REFINE_LOOP_TEMPLATE_NAME,
+)
 from lazycodr.prompts import load_template
 
 console = Console()
 
 
 def check_credentials():
     """Check if credentials file exists"""
```

