# Comparing `tmp/nb_move_imports-0.4.3.tar.gz` & `tmp/nb_move_imports-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_move_imports-0.4.3.tar", max compression
+gzip compressed data, was "nb_move_imports-0.4.4.tar", max compression
```

## Comparing `nb_move_imports-0.4.3.tar` & `nb_move_imports-0.4.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1629 2023-05-10 21:55:28.270127 nb_move_imports-0.4.3/README.md
--rw-r--r--   0        0        0     1078 2023-05-10 21:55:28.266127 nb_move_imports-0.4.3/pyproject.toml
--rw-r--r--   0        0        0       97 2023-05-10 21:55:28.266127 nb_move_imports-0.4.3/src/nb_move_imports/__init__.py
--rw-r--r--   0        0        0     3326 2023-05-10 21:55:16.657936 nb_move_imports-0.4.3/src/nb_move_imports/main.py
--rw-r--r--   0        0        0     2224 1970-01-01 00:00:00.000000 nb_move_imports-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1629 2023-05-10 22:00:29.404918 nb_move_imports-0.4.4/README.md
+-rw-r--r--   0        0        0     1078 2023-05-10 22:00:29.400918 nb_move_imports-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0       97 2023-05-10 22:00:29.396917 nb_move_imports-0.4.4/src/nb_move_imports/__init__.py
+-rw-r--r--   0        0        0     3335 2023-05-10 22:00:17.672693 nb_move_imports-0.4.4/src/nb_move_imports/main.py
+-rw-r--r--   0        0        0     2224 1970-01-01 00:00:00.000000 nb_move_imports-0.4.4/PKG-INFO
```

### Comparing `nb_move_imports-0.4.3/README.md` & `nb_move_imports-0.4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 
 ## Precommit Hook
 
 Add this section to your `pre-commit-config.yaml` so that the nb_move_imports script is executed before each commit with pre-commit.
 
 ```yaml
 - repo: https://github.com/AnH0ang/nb_move_imports
-  rev: 0.4.3
+  rev: 0.4.4
   hooks:
     - id: nb_move_imports
       name: nb_move_imports
 ```
```

### Comparing `nb_move_imports-0.4.3/pyproject.toml` & `nb_move_imports-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nb_move_imports"
-version = "0.4.3"
+version = "0.4.4"
 description = "Move import statements in jupyter notebook to the first cell"
 authors = ["An Hoang <anhoang31415@gmail.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.9,<4.0.0"
```

### Comparing `nb_move_imports-0.4.3/src/nb_move_imports/main.py` & `nb_move_imports-0.4.4/src/nb_move_imports/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 from itertools import filterfalse, tee
 from typing import Callable, Iterable, List, Tuple, TypeVar
 
 import click
-import isort
 import nbformat
 from nbformat.notebooknode import NotebookNode
 
 IMPORT_CELL_TAG = "IMPORT_CELL"
 IGNORE_CELL_TAG = "IGNORE_MV_IMPORTS"
 IMPORT_PATTERN = r"(?m)^(?:from[ ]+(.*)[ ]+)?import[ ].*$"
 
@@ -75,14 +74,16 @@
         all_import_lines.extend(i_lines)
         cell["source"] = "\n".join(c_lines)
 
     # add import staments to import cell
     import_statement = "\n".join(all_import_lines)
     new_cell_source = "\n".join([import_statement, import_cell["source"]])
     if apply_isort:
+        import isort
+
         new_cell_source = isort.code(new_cell_source)
     import_cell["source"] = new_cell_source
     return nb
 
 
 @click.command()
 @click.option("--sort", is_flag=True, help="Sort the import with isort")
```

### Comparing `nb_move_imports-0.4.3/PKG-INFO` & `nb_move_imports-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-move-imports
-Version: 0.4.3
+Version: 0.4.4
 Summary: Move import statements in jupyter notebook to the first cell
 Author: An Hoang
 Author-email: anhoang31415@gmail.com
 Requires-Python: >=3.8.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -42,13 +42,13 @@
 
 ## Precommit Hook
 
 Add this section to your `pre-commit-config.yaml` so that the nb_move_imports script is executed before each commit with pre-commit.
 
 ```yaml
 - repo: https://github.com/AnH0ang/nb_move_imports
-  rev: 0.4.3
+  rev: 0.4.4
   hooks:
     - id: nb_move_imports
       name: nb_move_imports
 ```
```

