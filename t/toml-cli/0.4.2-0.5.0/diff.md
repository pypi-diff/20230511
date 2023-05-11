# Comparing `tmp/toml_cli-0.4.2.tar.gz` & `tmp/toml_cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toml_cli-0.4.2.tar", max compression
+gzip compressed data, was "toml_cli-0.5.0.tar", max compression
```

## Comparing `toml_cli-0.4.2.tar` & `toml_cli-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-04-17 18:46:19.815059 toml_cli-0.4.2/LICENSE
--rw-r--r--   0        0        0      780 2023-04-17 18:46:19.815059 toml_cli-0.4.2/README.md
--rw-r--r--   0        0        0      646 2023-04-17 18:46:19.815059 toml_cli-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2619 2023-04-17 18:46:19.815059 toml_cli-0.4.2/toml_cli/__init__.py
--rw-r--r--   0        0        0     1569 1970-01-01 00:00:00.000000 toml_cli-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-11 05:31:22.176220 toml_cli-0.5.0/LICENSE
+-rw-r--r--   0        0        0      841 2023-05-11 05:31:22.176220 toml_cli-0.5.0/README.md
+-rw-r--r--   0        0        0      664 2023-05-11 05:31:22.176220 toml_cli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2889 2023-05-11 05:31:22.176220 toml_cli-0.5.0/toml_cli/__init__.py
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 toml_cli-0.5.0/PKG-INFO
```

### Comparing `toml_cli-0.4.2/LICENSE` & `toml_cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toml_cli-0.4.2/README.md` & `toml_cli-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ## Install
 
 `pip install toml-cli`
 
 ## Get a value
 
 `toml get --toml-path pyproject.toml tool.poetry.name`
+`toml get --toml-path pyproject.toml tool.poetry.authors[0]`
 
 ## Set a value
 
 `toml set --toml-path pyproject.toml tool.poetry.version 0.2.0`
 
 ## Add a section
```

### Comparing `toml_cli-0.4.2/pyproject.toml` & `toml_cli-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "toml-cli"
-version = "0.4.2"
+version = "0.5.0"
 description = "Command line interface to read and write keys/values to/from toml files"
-authors = ["Marc Rijken"]
+authors = ["Marc Rijken <marc@rijken.org>"]
 license = "MIT"
 repository = "https://github.com/mrijken/toml-cli"
 readme = "README.md"
 packages = [{ include = "toml_cli" }]
 
 [tool.poetry.scripts]
 toml = 'toml_cli:main'
```

### Comparing `toml_cli-0.4.2/toml_cli/__init__.py` & `toml_cli-0.5.0/toml_cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import json
 import pathlib
 from typing import Optional
 
 import tomlkit
 import tomlkit.exceptions
 import typer
+import re
 
 app = typer.Typer(no_args_is_help=True)
 
 
 @app.command("get")
 def get(
     key: Optional[str] = typer.Argument(None),
     toml_path: pathlib.Path = typer.Option(pathlib.Path("config.toml")),
 ):
     """Get a value from a toml file"""
     toml_part = tomlkit.parse(toml_path.read_text())
 
     if key is not None:
         for key_part in key.split("."):
-            toml_part = toml_part[key_part]
+            match = re.search(r"(?P<key>.*?)\[(?P<index>\d+)\]", key_part)
+            if match:
+                key = match.group("key")
+                index = int(match.group("index"))
+                toml_part = toml_part[key][index]
+            else:
+                toml_part = toml_part[key_part]
 
     typer.echo(toml_part)
 
 
 @app.command("set")
 def set_(
     key: str,
```

### Comparing `toml_cli-0.4.2/PKG-INFO` & `toml_cli-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: toml-cli
-Version: 0.4.2
+Version: 0.5.0
 Summary: Command line interface to read and write keys/values to/from toml files
 Home-page: https://github.com/mrijken/toml-cli
 License: MIT
 Author: Marc Rijken
+Author-email: marc@rijken.org
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -34,14 +35,15 @@
 ## Install
 
 `pip install toml-cli`
 
 ## Get a value
 
 `toml get --toml-path pyproject.toml tool.poetry.name`
+`toml get --toml-path pyproject.toml tool.poetry.authors[0]`
 
 ## Set a value
 
 `toml set --toml-path pyproject.toml tool.poetry.version 0.2.0`
 
 ## Add a section
```

