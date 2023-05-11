# Comparing `tmp/iconoclast-2.0.0.tar.gz` & `tmp/iconoclast-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iconoclast-2.0.0.tar", max compression
+gzip compressed data, was "iconoclast-2.0.1.tar", max compression
```

## Comparing `iconoclast-2.0.0.tar` & `iconoclast-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1091 2023-05-06 01:57:32.474808 iconoclast-2.0.0/LICENSE.md
--rw-r--r--   0        0        0     1254 2023-05-06 01:57:32.474808 iconoclast-2.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/cli/__init__.py
--rw-r--r--   0        0        0     3662 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/cli/app.py
--rw-r--r--   0        0        0      247 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/cli/context.py
--rw-r--r--   0        0        0      285 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/cli/exceptions.py
--rw-r--r--   0        0        0       96 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/cli/graphql/__init__.py
--rw-r--r--   0        0        0    12875 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/cli/graphql/schema.py
--rw-r--r--   0        0        0      298 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/cli/iconokit/iconokit/__init__.py
--rw-r--r--   0        0        0      209 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/cli/iconokit/pyproject.toml
--rw-r--r--   0        0        0     1665 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/cli/prompts.py
--rw-r--r--   0        0        0        0 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/plugins/__init__.py
--rw-r--r--   0        0        0      584 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/plugins/iconocards.py
--rw-r--r--   0        0        0     3203 2023-05-06 01:57:32.478808 iconoclast-2.0.0/iconoclast/plugins/iconoclast.py
--rw-r--r--   0        0        0     1907 2023-05-06 01:57:32.478808 iconoclast-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 iconoclast-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-05-11 17:01:03.168348 iconoclast-2.0.1/LICENSE.md
+-rw-r--r--   0        0        0     1254 2023-05-11 17:01:03.168348 iconoclast-2.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/__init__.py
+-rw-r--r--   0        0        0     3674 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/app.py
+-rw-r--r--   0        0        0      247 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/context.py
+-rw-r--r--   0        0        0      285 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/exceptions.py
+-rw-r--r--   0        0        0       96 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/graphql/__init__.py
+-rw-r--r--   0        0        0    12875 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/graphql/schema.py
+-rw-r--r--   0        0        0      298 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/iconokit/iconokit/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/iconokit/pyproject.toml
+-rw-r--r--   0        0        0     1665 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/cli/prompts.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/plugins/__init__.py
+-rw-r--r--   0        0        0      584 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/plugins/iconocards.py
+-rw-r--r--   0        0        0     3203 2023-05-11 17:01:03.172348 iconoclast-2.0.1/iconoclast/plugins/iconoclast.py
+-rw-r--r--   0        0        0     1907 2023-05-11 17:01:03.176348 iconoclast-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 iconoclast-2.0.1/PKG-INFO
```

### Comparing `iconoclast-2.0.0/LICENSE.md` & `iconoclast-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.0/README.md` & `iconoclast-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.0/iconoclast/cli/app.py` & `iconoclast-2.0.1/iconoclast/cli/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from sgqlc.endpoint.requests import RequestsEndpoint
 from sgqlc.operation import Operation
 from yarl import URL
 
 from iconoclast.cli.context import set_context
 from iconoclast.cli.exceptions import Iconoquit
 from iconoclast.cli.graphql.schema import fontawesome_schema as schema
-from iconoclast.plugin import IconokitConfig
+from iconoclast.plugins.iconoclast import IconokitConfig
 
 app = typer.Typer(rich_markup_mode="rich")
 
 here = Path(__file__).parent
 
 
 @app.command(
```

### Comparing `iconoclast-2.0.0/iconoclast/cli/graphql/schema.py` & `iconoclast-2.0.1/iconoclast/cli/graphql/schema.py`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.0/iconoclast/cli/prompts.py` & `iconoclast-2.0.1/iconoclast/cli/prompts.py`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.0/iconoclast/plugins/iconocards.py` & `iconoclast-2.0.1/iconoclast/plugins/iconocards.py`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.0/iconoclast/plugins/iconoclast.py` & `iconoclast-2.0.1/iconoclast/plugins/iconoclast.py`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.0/pyproject.toml` & `iconoclast-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iconoclast"
-version = "2.0.0"
+version = "2.0.1"
 description = "Font Awesome Pro integration for Material for MkDocs"
 authors = ["celsius narhwal <hello@celsiusnarhwal.dev>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `iconoclast-2.0.0/PKG-INFO` & `iconoclast-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconoclast
-Version: 2.0.0
+Version: 2.0.1
 Summary: Font Awesome Pro integration for Material for MkDocs
 License: MIT
 Author: celsius narhwal
 Author-email: hello@celsiusnarhwal.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

