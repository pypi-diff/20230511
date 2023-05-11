# Comparing `tmp/prr-0.2.0.tar.gz` & `tmp/prr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prr-0.2.0.tar", max compression
+gzip compressed data, was "prr-0.2.1.tar", max compression
```

## Comparing `prr-0.2.0.tar` & `prr-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1074 2023-05-07 19:46:47.449469 prr-0.2.0/LICENSE
--rw-r--r--   0        0        0    17547 2023-05-09 20:17:46.813089 prr-0.2.0/README.md
--rwxr-xr-x   0        0        0     2529 2023-05-09 21:12:10.689188 prr-0.2.0/prr/__init__.py
--rw-r--r--   0        0        0      878 2023-05-08 12:56:49.389217 prr-0.2.0/prr/options.py
--rw-r--r--   0        0        0     7525 2023-05-09 12:57:31.506982 prr-0.2.0/prr/prompt.py
--rw-r--r--   0        0        0      644 2023-05-08 12:56:45.364127 prr-0.2.0/prr/prompt_run.py
--rw-r--r--   0        0        0      954 2023-05-08 12:56:45.364389 prr-0.2.0/prr/prompt_run_result.py
--rw-r--r--   0        0        0      886 2023-05-08 12:56:45.364621 prr-0.2.0/prr/request.py
--rw-r--r--   0        0        0      810 2023-05-08 12:56:45.364894 prr-0.2.0/prr/response.py
--rw-r--r--   0        0        0     1086 2023-05-08 12:56:45.365164 prr-0.2.0/prr/runner.py
--rw-r--r--   0        0        0     2797 2023-05-08 12:56:45.365480 prr-0.2.0/prr/saver.py
--rw-r--r--   0        0        0      486 2023-05-08 12:56:45.365733 prr-0.2.0/prr/service_config.py
--rw-r--r--   0        0        0      634 2023-05-09 21:03:08.802103 prr-0.2.0/prr/service_registry.py
--rw-r--r--   0        0        0     2288 2023-05-09 21:02:46.089911 prr-0.2.0/prr/services/providers/anthropic/complete.py
--rw-r--r--   0        0        0     1625 2023-05-09 21:15:11.978888 prr-0.2.0/prr/services/providers/openai/chat.py
--rwxr-xr-x   0        0        0     4309 2023-05-09 21:16:34.883528 prr-0.2.0/prr/utils/run.py
--rwxr-xr-x   0        0        0     2392 2023-05-09 21:16:27.264161 prr-0.2.0/prr/utils/watch.py
--rw-r--r--   0        0        0      793 2023-05-09 21:17:52.412966 prr-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    18279 1970-01-01 00:00:00.000000 prr-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-07 19:46:47.449469 prr-0.2.1/LICENSE
+-rw-r--r--   0        0        0    18072 2023-05-11 16:48:22.364108 prr-0.2.1/README.md
+-rwxr-xr-x   0        0        0     2621 2023-05-11 16:48:22.364465 prr-0.2.1/prr/__init__.py
+-rw-r--r--   0        0        0      143 2023-05-11 16:48:22.364670 prr-0.2.1/prr/config.py
+-rw-r--r--   0        0        0      931 2023-05-11 16:48:21.982369 prr-0.2.1/prr/options.py
+-rw-r--r--   0        0        0     7489 2023-05-11 16:48:21.982538 prr-0.2.1/prr/prompt.py
+-rw-r--r--   0        0        0      644 2023-05-11 16:48:21.982660 prr-0.2.1/prr/prompt_run.py
+-rw-r--r--   0        0        0      954 2023-05-11 16:48:21.982771 prr-0.2.1/prr/prompt_run_result.py
+-rw-r--r--   0        0        0      886 2023-05-11 16:48:21.982881 prr-0.2.1/prr/request.py
+-rw-r--r--   0        0        0      810 2023-05-11 16:48:21.982989 prr-0.2.1/prr/response.py
+-rw-r--r--   0        0        0     1086 2023-05-11 16:48:21.983099 prr-0.2.1/prr/runner.py
+-rw-r--r--   0        0        0     2797 2023-05-11 16:48:21.983230 prr-0.2.1/prr/saver.py
+-rw-r--r--   0        0        0      486 2023-05-11 16:48:21.983364 prr-0.2.1/prr/service_config.py
+-rw-r--r--   0        0        0      634 2023-05-11 16:48:21.983486 prr-0.2.1/prr/service_registry.py
+-rw-r--r--   0        0        0     2343 2023-05-11 16:48:22.365057 prr-0.2.1/prr/services/providers/anthropic/complete.py
+-rw-r--r--   0        0        0     1684 2023-05-11 16:48:22.365446 prr-0.2.1/prr/services/providers/openai/chat.py
+-rwxr-xr-x   0        0        0     4293 2023-05-11 16:48:22.365824 prr-0.2.1/prr/utils/run.py
+-rwxr-xr-x   0        0        0     2333 2023-05-11 16:48:22.366102 prr-0.2.1/prr/utils/watch.py
+-rw-r--r--   0        0        0      807 2023-05-11 16:48:22.366351 prr-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    18807 1970-01-01 00:00:00.000000 prr-0.2.1/PKG-INFO
```

### Comparing `prr-0.2.0/LICENSE` & `prr-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prr-0.2.0/README.md` & `prr-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,37 @@
 - [ ] Support multiple completions
 
 
 ## Getting started
 
 Here's a quick run through on what you need to know to use `prr` effectively.
 
+### Installation & configuration
+Install it via `pip` 
+```sh
+$ pip install prr
+```
+
+Copy `.env.example` - and save it as `.env`. Fill in your API keys for OpenAI, Anthropic and others:
+
+```bash
+# https://platform.openai.com/account/api-keys
+OPENAI_API_KEY="sk-..."
+
+# https://console.anthropic.com/account/keys
+ANTHROPIC_API_KEY="sk-ant-..."
+
+DEFAULT_SERVICE="openai/chat/gpt-3.5-turbo"
+```
+
+You can also use DEFAULT_SERVICE to specify the model you want to use by default, but otherwise you're good to go!
+
+
+## Development
+
 
 1. Clone the repo
 
 ```sh
 $ git clone https://github.com/Forward-Operators/prr.git
 ```
```

### Comparing `prr-0.2.0/prr/__init__.py` & `prr-0.2.1/prr/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 
+import argparse
 import os
 import sys
 
-sys.path.append(".")
+from prr.config import load_config
 
-import argparse
+from .utils.run import RunPromptCommand
+from .utils.watch import WatchPromptCommand
 
-from dotenv import load_dotenv
+# sys.path.append(".")
 
-load_dotenv()
 
-from .utils.run import RunPromptCommand
-from .utils.watch import WatchPromptCommand
+config = load_config()
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Run a prompt against configured models.",
         prog="prr",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -41,19 +41,23 @@
             action="store_true",
             default=False,
         )
         _parser.add_argument(
             "--service",
             "-s",
             help="Service to use if none is configured (defaults to DEFAULT_SERVICE environment variable)",
-            default=os.environ.get("DEFAULT_SERVICE"),
+            default=config["DEFAULT_SERVICE"],
             type=str,
         )
         _parser.add_argument(
-            "--quiet", "-q", help="Quiet mode, just outputs the completion"
+            "--quiet",
+            "-q",
+            help="Quiet mode, just outputs the completion",
+            action="store_true",
+            default=False,
         )
         _parser.add_argument(
             "--log",
             "-l",
             help="Save each run in <prompt>.runs directory",
             action="store_true",
             default=False,
```

### Comparing `prr-0.2.0/prr/options.py` & `prr-0.2.1/prr/options.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-DEFAULT_OPTIONS = {"temperature": 1.0, "top_k": -1, "top_p": -1, "max_tokens": 256}
+DEFAULT_OPTIONS = {"temperature": 1.0, "top_k": -1, "top_p": -1, "max_tokens": 4000}
 
 ALLOWED_OPTIONS = DEFAULT_OPTIONS.keys()
 
 
 class ModelOptions:
     def __init__(self, options={}):
         self.options_set = []
         self.update_options(DEFAULT_OPTIONS)
         self.update_options(options)
 
     def update_options(self, options):
         for key in options.keys():
             if key in ALLOWED_OPTIONS:
-                self.options_set.append(key)
+                if key not in self.options_set:
+                    self.options_set.append(key)
                 setattr(self, key, options[key])
 
     def description(self):
         return " ".join([f"{key}={self.option(key)}" for key in self.options_set])
 
     def option(self, key):
         return getattr(self, key)
```

### Comparing `prr-0.2.0/prr/prompt.py` & `prr-0.2.1/prr/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,25 +182,25 @@
 
         return "".join(file_contents)
 
     def load_jinja_template_from_string(self, content):
         self.add_dependency_files_from_jinja_template(content)
         return self.template_env.from_string(content)
 
-        def load_jinja_template_from_file(self, template_subpath):
-            try:
-                with open(
-                    os.path.join(os.path.dirname(self.path), template_subpath), "r"
-                ) as stream:
-                    self.add_dependency_files_from_jinja_template(stream.read())
+    def load_jinja_template_from_file(self, template_subpath):
+        try:
+            with open(
+                os.path.join(os.path.dirname(self.path), template_subpath), "r"
+            ) as stream:
+                self.add_dependency_files_from_jinja_template(stream.read())
 
                 return self.template_env.get_template(template_subpath)
-            except FileNotFoundError:
-                print(f"Could not find template file: {template_subpath}")
-                exit(-1)
+        except FileNotFoundError:
+            print(f"Could not find template file: {template_subpath}")
+            exit(-1)
 
     def load_text_file(self, path):
         self.path = path
 
         with open(path, "r") as stream:
             file_contents = self.deal_with_shebang_line(stream)
             self.template = self.template_env.from_string(file_contents)
```

### Comparing `prr-0.2.0/prr/prompt_run.py` & `prr-0.2.1/prr/prompt_run.py`

 * *Files identical despite different names*

### Comparing `prr-0.2.0/prr/prompt_run_result.py` & `prr-0.2.1/prr/prompt_run_result.py`

 * *Files identical despite different names*

### Comparing `prr-0.2.0/prr/request.py` & `prr-0.2.1/prr/request.py`

 * *Files identical despite different names*

### Comparing `prr-0.2.0/prr/response.py` & `prr-0.2.1/prr/response.py`

 * *Files identical despite different names*

### Comparing `prr-0.2.0/prr/runner.py` & `prr-0.2.1/prr/runner.py`

 * *Files identical despite different names*

### Comparing `prr-0.2.0/prr/saver.py` & `prr-0.2.1/prr/saver.py`

 * *Files identical despite different names*

### Comparing `prr-0.2.0/prr/service_registry.py` & `prr-0.2.1/prr/service_registry.py`

 * *Files identical despite different names*

### Comparing `prr-0.2.0/prr/services/providers/anthropic/complete.py` & `prr-0.2.1/prr/services/providers/anthropic/complete.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # https://console.anthropic.com/docs/api/reference
 # https://github.com/anthropics/anthropic-sdk-python/tree/main/examples
 
 import os
 
 import anthropic
 
+from prr.config import load_config
 from prr.request import ServiceRequest
 from prr.response import ServiceResponse
 
+config = load_config()
+
 # https://console.anthropic.com/docs/api/reference
 
 
 # Anthropic model provider class
 class ServiceAnthropicComplete:
     provider = "anthropic"
     service = "complete"
@@ -19,15 +22,15 @@
     def run(self, prompt, service_config):
         self.service_config = service_config
         options = self.service_config.options
         self.prompt = prompt
 
         prompt_text = self.prompt_text()
 
-        client = anthropic.Client(os.environ["ANTHROPIC_API_KEY"])
+        client = anthropic.Client(config["ANTHROPIC_API_KEY"])
 
         service_request = ServiceRequest(self.service_config, prompt_text)
 
         response = client.completion(
             prompt=prompt_text,
             stop_sequences=[anthropic.HUMAN_PROMPT],
             model=service_config.model_name(),
```

### Comparing `prr-0.2.0/prr/services/providers/openai/chat.py` & `prr-0.2.1/prr/services/providers/openai/chat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import openai
 
+from prr.config import load_config
 from prr.request import ServiceRequest
 from prr.response import ServiceResponse
 
+config = load_config()
+
 
 # OpenAI model provider class
 class ServiceOpenAIChat:
     provider = "openai"
     service = "chat"
 
     def run(self, prompt, service_config):
```

### Comparing `prr-0.2.0/prr/utils/run.py` & `prr-0.2.1/prr/utils/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 #!/usr/bin/env python
 
 import os
 import sys
 from io import StringIO
 
-from dotenv import load_dotenv
-
-from prr.prompt import Prompt
-
-load_dotenv()
-
 from rich import print
 from rich.console import Console
 from rich.panel import Panel
 
+# from prr.config import config
+from prr.prompt import Prompt
 from prr.runner import Runner
 
 console = Console(log_time=False, log_path=False)
 
 
 class RunPromptCommand:
     def __init__(self, args, prompt_args=None):
```

### Comparing `prr-0.2.0/prr/utils/watch.py` & `prr-0.2.1/prr/utils/watch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 #!/usr/bin/env python
 
 import datetime
 import os
-import sys
 import time
 
-from dotenv import load_dotenv
-
 from prr.prompt import Prompt
-
-load_dotenv()
-
 from prr.utils.run import RunPromptCommand
 
 
 def timestamp_for_file(path):
     if os.path.exists(path):
         return os.path.getmtime(path)
```

### Comparing `prr-0.2.0/pyproject.toml` & `prr-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "prr"
-version = "0.2.0"
+version = "0.2.1"
 description = "prr - command-line LLM prompt runner"
-authors = ["Zbigniew Sobiecki <zbigniew@sobiecki.name>", "Mateusz Kozak <mateusz@mkozak.pl"]
+authors = [ "Zbigniew Sobiecki <zbigniew@fwdoperators.com>" , "Mateusz Kozak <mateusz@fwdoperators.com>" ]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^0.27.6"
 python-dotenv = "^1.0.0"
```

### Comparing `prr-0.2.0/PKG-INFO` & `prr-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: prr
-Version: 0.2.0
+Version: 0.2.1
 Summary: prr - command-line LLM prompt runner
 License: MIT
 Author: Zbigniew Sobiecki
-Author-email: zbigniew@sobiecki.name
+Author-email: zbigniew@fwdoperators.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
@@ -75,14 +75,37 @@
 - [ ] Support multiple completions
 
 
 ## Getting started
 
 Here's a quick run through on what you need to know to use `prr` effectively.
 
+### Installation & configuration
+Install it via `pip` 
+```sh
+$ pip install prr
+```
+
+Copy `.env.example` - and save it as `.env`. Fill in your API keys for OpenAI, Anthropic and others:
+
+```bash
+# https://platform.openai.com/account/api-keys
+OPENAI_API_KEY="sk-..."
+
+# https://console.anthropic.com/account/keys
+ANTHROPIC_API_KEY="sk-ant-..."
+
+DEFAULT_SERVICE="openai/chat/gpt-3.5-turbo"
+```
+
+You can also use DEFAULT_SERVICE to specify the model you want to use by default, but otherwise you're good to go!
+
+
+## Development
+
 
 1. Clone the repo
 
 ```sh
 $ git clone https://github.com/Forward-Operators/prr.git
 ```
```

