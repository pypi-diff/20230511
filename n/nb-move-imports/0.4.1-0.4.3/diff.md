# Comparing `tmp/nb_move_imports-0.4.1.tar.gz` & `tmp/nb_move_imports-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_move_imports-0.4.1.tar", max compression
+gzip compressed data, was "nb_move_imports-0.4.3.tar", max compression
```

## Comparing `nb_move_imports-0.4.1.tar` & `nb_move_imports-0.4.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1629 2022-09-16 10:04:16.816357 nb_move_imports-0.4.1/README.md
--rw-r--r--   0        0        0     1003 2022-09-16 10:04:16.812357 nb_move_imports-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       97 2022-09-16 10:04:16.808357 nb_move_imports-0.4.1/src/nb_move_imports/__init__.py
--rw-r--r--   0        0        0     3326 2022-09-16 10:04:11.028232 nb_move_imports-0.4.1/src/nb_move_imports/main.py
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 nb_move_imports-0.4.1/setup.py
--rw-r--r--   0        0        0     2153 1970-01-01 00:00:00.000000 nb_move_imports-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1629 2023-05-10 21:55:28.270127 nb_move_imports-0.4.3/README.md
+-rw-r--r--   0        0        0     1078 2023-05-10 21:55:28.266127 nb_move_imports-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0       97 2023-05-10 21:55:28.266127 nb_move_imports-0.4.3/src/nb_move_imports/__init__.py
+-rw-r--r--   0        0        0     3326 2023-05-10 21:55:16.657936 nb_move_imports-0.4.3/src/nb_move_imports/main.py
+-rw-r--r--   0        0        0     2224 1970-01-01 00:00:00.000000 nb_move_imports-0.4.3/PKG-INFO
```

### Comparing `nb_move_imports-0.4.1/README.md` & `nb_move_imports-0.4.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 
 ## Precommit Hook
 
 Add this section to your `pre-commit-config.yaml` so that the nb_move_imports script is executed before each commit with pre-commit.
 
 ```yaml
 - repo: https://github.com/AnH0ang/nb_move_imports
-  rev: 0.4.1
+  rev: 0.4.3
   hooks:
     - id: nb_move_imports
       name: nb_move_imports
 ```
```

### Comparing `nb_move_imports-0.4.1/pyproject.toml` & `nb_move_imports-0.4.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [tool.poetry]
 name = "nb_move_imports"
-version = "0.4.1"
+version = "0.4.3"
 description = "Move import statements in jupyter notebook to the first cell"
 authors = ["An Hoang <anhoang31415@gmail.com>"]
 readme = "README.md"
 
+
 [tool.poetry.dependencies]
 python = ">=3.8.9,<4.0.0"
 
 # === USER DEFINED DEPENDENCIES HERE ===
-nbformat = "^5.4.0"
-isort = "^5.10.1"
-click = "^8.1.3"
+nbformat = ">=5.4.0"
+click = ">=8.1.3"
+isort = { version = ">=5.10.1", optional = true }
+
+[tool.poetry.extras]
+isort = ["isort"]
 
 [tool.poetry.dev-dependencies]
 # Runnings notebook in vscode
 ipykernel = ">=6.9.2"
 
 # Testing
 pytest = ">=7.1.0"
```

### Comparing `nb_move_imports-0.4.1/src/nb_move_imports/main.py` & `nb_move_imports-0.4.3/src/nb_move_imports/main.py`

 * *Files identical despite different names*

### Comparing `nb_move_imports-0.4.1/setup.py` & `nb_move_imports-0.4.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,54 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nb-move-imports
+Version: 0.4.3
+Summary: Move import statements in jupyter notebook to the first cell
+Author: An Hoang
+Author-email: anhoang31415@gmail.com
+Requires-Python: >=3.8.9,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: isort
+Requires-Dist: click (>=8.1.3)
+Requires-Dist: isort (>=5.10.1) ; extra == "isort"
+Requires-Dist: nbformat (>=5.4.0)
+Description-Content-Type: text/markdown
+
+# nb_move_imports
+
+------------------------------
+[![PyPI version](https://badge.fury.io/py/nb_move_imports.svg)](https://badge.fury.io/py/nb_move_imports)
+[![Python version](https://img.shields.io/badge/python-≥3.8-blue.svg)](https://pypi.org/project/kedro/)
+[![Release Pipeline](https://github.com/AnH0ang/nb_move_imports/actions/workflows/release.yml/badge.svg)](https://github.com/AnH0ang/nb_move_imports/actions/workflows/release.yml)
+[![Test](https://github.com/AnH0ang/nb_move_imports/actions/workflows/test.yml/badge.svg)](https://github.com/AnH0ang/nb_move_imports/actions/workflows/test.yml)
+[![Code Quality](https://github.com/AnH0ang/nb_move_imports/actions/workflows/code_quality.yml/badge.svg)](https://github.com/AnH0ang/nb_move_imports/actions/workflows/code_quality.yml)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/STATWORX/statworx-theme/blob/master/LICENSE)
+![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
+
+Move import statements in jupyter notebook to the first cell
+
+## Use nb_move_imports
+
+To run the script on a specific jupyter notebook run:
+
+```console
+nb_move_imports path/to/notebook.ipynb
+```
+
+## Skip processing of cells
+
+In order to skip a cell you have to tag it with the `IGNORE_MV_IMPORTS` tag.
+
+## Precommit Hook
+
+Add this section to your `pre-commit-config.yaml` so that the nb_move_imports script is executed before each commit with pre-commit.
+
+```yaml
+- repo: https://github.com/AnH0ang/nb_move_imports
+  rev: 0.4.3
+  hooks:
+    - id: nb_move_imports
+      name: nb_move_imports
+```
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['nb_move_imports']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.1.3,<9.0.0', 'isort>=5.10.1,<6.0.0', 'nbformat>=5.4.0,<6.0.0']
-
-entry_points = \
-{'console_scripts': ['jupyter-nbmoveimports = nb_move_imports.main:main',
-                     'nb_move_imports = nb_move_imports.main:main']}
-
-setup_kwargs = {
-    'name': 'nb-move-imports',
-    'version': '0.4.1',
-    'description': 'Move import statements in jupyter notebook to the first cell',
-    'long_description': '# nb_move_imports\n\n------------------------------\n[![PyPI version](https://badge.fury.io/py/nb_move_imports.svg)](https://badge.fury.io/py/nb_move_imports)\n[![Python version](https://img.shields.io/badge/python-≥3.8-blue.svg)](https://pypi.org/project/kedro/)\n[![Release Pipeline](https://github.com/AnH0ang/nb_move_imports/actions/workflows/release.yml/badge.svg)](https://github.com/AnH0ang/nb_move_imports/actions/workflows/release.yml)\n[![Test](https://github.com/AnH0ang/nb_move_imports/actions/workflows/test.yml/badge.svg)](https://github.com/AnH0ang/nb_move_imports/actions/workflows/test.yml)\n[![Code Quality](https://github.com/AnH0ang/nb_move_imports/actions/workflows/code_quality.yml/badge.svg)](https://github.com/AnH0ang/nb_move_imports/actions/workflows/code_quality.yml)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/STATWORX/statworx-theme/blob/master/LICENSE)\n![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)\n\nMove import statements in jupyter notebook to the first cell\n\n## Use nb_move_imports\n\nTo run the script on a specific jupyter notebook run:\n\n```console\nnb_move_imports path/to/notebook.ipynb\n```\n\n## Skip processing of cells\n\nIn order to skip a cell you have to tag it with the `IGNORE_MV_IMPORTS` tag.\n\n## Precommit Hook\n\nAdd this section to your `pre-commit-config.yaml` so that the nb_move_imports script is executed before each commit with pre-commit.\n\n```yaml\n- repo: https://github.com/AnH0ang/nb_move_imports\n  rev: 0.4.1\n  hooks:\n    - id: nb_move_imports\n      name: nb_move_imports\n```\n',
-    'author': 'An Hoang',
-    'author_email': 'anhoang31415@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.9,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

