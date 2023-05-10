# Comparing `tmp/catppuccin-1.2.0.tar.gz` & `tmp/catppuccin-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catppuccin-1.2.0.tar", max compression
+gzip compressed data, was "catppuccin-1.3.0.tar", max compression
```

## Comparing `catppuccin-1.2.0.tar` & `catppuccin-1.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-04-26 08:50:30.147193 catppuccin-1.2.0/LICENSE
--rw-r--r--   0        0        0     3975 2023-04-26 08:50:30.147193 catppuccin-1.2.0/README.md
--rw-r--r--   0        0        0      142 2023-04-26 08:50:30.147193 catppuccin-1.2.0/catppuccin/__init__.py
--rw-r--r--   0        0        0     2003 2023-04-26 08:50:30.147193 catppuccin-1.2.0/catppuccin/colour.py
--rw-r--r--   0        0        0        0 2023-04-26 08:50:30.147193 catppuccin-1.2.0/catppuccin/extras/__init__.py
--rw-r--r--   0        0        0     2138 2023-04-26 08:50:30.147193 catppuccin-1.2.0/catppuccin/extras/pygments.py
--rw-r--r--   0        0        0     5641 2023-04-26 08:50:30.147193 catppuccin-1.2.0/catppuccin/flavour.py
--rw-r--r--   0        0        0     1129 2023-04-26 08:51:09.760223 catppuccin-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5248 1970-01-01 00:00:00.000000 catppuccin-1.2.0/setup.py
--rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 catppuccin-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-10 21:52:44.603080 catppuccin-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3975 2023-05-10 21:52:44.603080 catppuccin-1.3.0/README.md
+-rw-r--r--   0        0        0      142 2023-05-10 21:52:44.603080 catppuccin-1.3.0/catppuccin/__init__.py
+-rw-r--r--   0        0        0     2003 2023-05-10 21:52:44.603080 catppuccin-1.3.0/catppuccin/colour.py
+-rw-r--r--   0        0        0        0 2023-05-10 21:52:44.603080 catppuccin-1.3.0/catppuccin/extras/__init__.py
+-rw-r--r--   0        0        0     2138 2023-05-10 21:52:44.603080 catppuccin-1.3.0/catppuccin/extras/pygments.py
+-rw-r--r--   0        0        0     1577 2023-05-10 21:52:44.603080 catppuccin-1.3.0/catppuccin/extras/rich_ctp.py
+-rw-r--r--   0        0        0     5641 2023-05-10 21:52:44.603080 catppuccin-1.3.0/catppuccin/flavour.py
+-rw-r--r--   0        0        0     1193 2023-05-10 21:53:32.125824 catppuccin-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 catppuccin-1.3.0/setup.py
+-rw-r--r--   0        0        0     4622 1970-01-01 00:00:00.000000 catppuccin-1.3.0/PKG-INFO
```

### Comparing `catppuccin-1.2.0/LICENSE` & `catppuccin-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `catppuccin-1.2.0/README.md` & `catppuccin-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `catppuccin-1.2.0/catppuccin/colour.py` & `catppuccin-1.3.0/catppuccin/colour.py`

 * *Files identical despite different names*

### Comparing `catppuccin-1.2.0/catppuccin/extras/pygments.py` & `catppuccin-1.3.0/catppuccin/extras/pygments.py`

 * *Files identical despite different names*

### Comparing `catppuccin-1.2.0/catppuccin/flavour.py` & `catppuccin-1.3.0/catppuccin/flavour.py`

 * *Files identical despite different names*

### Comparing `catppuccin-1.2.0/pyproject.toml` & `catppuccin-1.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "catppuccin"
-version = "1.2.0"
+version = "1.3.0"
 description = "🐍 Soothing pastel theme for Python."
 authors = ["backwardspy <backwardspy@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.plugins."pygments.styles"]
 catppuccin-latte = "catppuccin.extras.pygments:LatteStyle"
 catppuccin-frappe = "catppuccin.extras.pygments:FrappeStyle"
 catppuccin-macchiato = "catppuccin.extras.pygments:MacchiatoStyle"
 catppuccin-mocha = "catppuccin.extras.pygments:MochaStyle"
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
 pygments = { version = "^2.13.0", optional = true }
+rich = { version = "^13.3.5", optional = true }
 
 [tool.poetry.extras]
 pygments = ["pygments"]
+rich = ["rich"]
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.15.5"
 mypy = "^0.982"
 black = "^22.10.0"
 isort = "^5.10.1"
 pytest = "^7.2.0"
```

### Comparing `catppuccin-1.2.0/setup.py` & `catppuccin-1.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 packages = \
 ['catppuccin', 'catppuccin.extras']
 
 package_data = \
 {'': ['*']}
 
 extras_require = \
-{'pygments': ['pygments>=2.13.0,<3.0.0']}
+{'pygments': ['pygments>=2.13.0,<3.0.0'], 'rich': ['rich>=13.3.5,<14.0.0']}
 
 entry_points = \
 {'pygments.styles': ['catppuccin-frappe = '
                      'catppuccin.extras.pygments:FrappeStyle',
                      'catppuccin-latte = catppuccin.extras.pygments:LatteStyle',
                      'catppuccin-macchiato = '
                      'catppuccin.extras.pygments:MacchiatoStyle',
                      'catppuccin-mocha = '
                      'catppuccin.extras.pygments:MochaStyle']}
 
 setup_kwargs = {
     'name': 'catppuccin',
-    'version': '1.2.0',
+    'version': '1.3.0',
     'description': '🐍 Soothing pastel theme for Python.',
     'long_description': '<h3 align="center">\n\t<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>\n\t<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>\n\tCatppuccin for <a href="https://www.python.org/">Python</a>\n\t<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>\n</h3>\n\n<p align="center">\n\t<a href="https://github.com/catppuccin/python/stargazers"><img src="https://img.shields.io/github/stars/catppuccin/python?colorA=363a4f&colorB=b7bdf8&style=for-the-badge"></a>\n\t<a href="https://github.com/catppuccin/python/issues"><img src="https://img.shields.io/github/issues/catppuccin/python?colorA=363a4f&colorB=f5a97f&style=for-the-badge"></a>\n\t<a href="https://github.com/catppuccin/python/contributors"><img src="https://img.shields.io/github/contributors/catppuccin/python?colorA=363a4f&colorB=a6da95&style=for-the-badge"></a>\n</p>\n\n## Installation\n\nInstall with `pip` or your preferred dependency management tool.\n\n```bash\npip install catppuccin\n```\n\n## Usage\n\n```python\n>>> from catppuccin import Flavour\n>>> Flavour.latte().mauve.hex\n\'8839ef\'\n>>> Flavour.mocha().teal.rgb\n(148, 226, 213)\n```\n\n`Flavour` is a [`dataclass`](https://docs.python.org/3/library/dataclasses.html),\nso you can inspect its fields to get access to the full set of colour names and values:\n\n```python\n>>> from dataclasses import fields\n>>> flavour = Flavour.frappe()\n>>> for field in fields(flavour):\n        colour = getattr(flavour, field.name)\n        print(f"{field.name}: #{colour.hex}")\nrosewater: #f2d5cf\nflamingo: #eebebe\npink: #f4b8e4\n...\nbase: #303446\nmantle: #292c3c\ncrust: #232634\n```\n\n## Pygments Styles\n\nThis package provides a Pygments style for each of the four Catppuccin flavours.\n\nInstall Catppuccin with the `pygments` feature to include the relevant dependencies:\n\n```bash\npip install catppuccin[pygments]\n```\n\nThe styles are registered as importlib entrypoints, which allows Pygments to\nfind them by name:\n\n```python\n>>> from pygments.styles import get_style_by_name\n>>> get_style_by_name("catppuccin-frappe")\ncatppuccin.extras.pygments.FrappeStyle\n```\n\nThe following style names are available:\n\n - `catppuccin-latte`\n - `catppuccin-frappe`\n - `catppuccin-macchiato`\n - `catppuccin-mocha`\n\nThey can also be accessed by directly importing them:\n\n```python\nfrom catppuccin.extras.pygments import MacchiatoStyle\n```\n\n## Contribution\n\nIf you are looking to contribute, please read through our\n[CONTRIBUTING.md](https://github.com/catppuccin/.github/blob/main/CONTRIBUTING.md)\nfirst!\n\n### Development\n\nThis project is maintained with [Poetry](https://python-poetry.org). If you\ndon\'t have Poetry yet, you can install it using the [installation\ninstructions](https://python-poetry.org/docs/#installation).\n\nInstall the project\'s dependencies including extras:\n\n```bash\npoetry install -E pygments\n```\n\n#### Code Standards\n\nBefore committing changes, it is recommended to run the following tools to\nensure consistency in the codebase.\n\n```bash\nisort .\nblack .\npylint catppuccin\nmypy .\npytest --cov catppuccin\n```\n\nThese tools are all installed as part of the `dev` dependency group with\nPoetry. You can use `poetry shell` to automatically put these tools in your\npath.\n\n\n## 💝 Thanks to\n\n-   [backwardspy](https://github.com/backwardspy)\n\n&nbsp;\n\n<p align="center">\n\t<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/footers/gray0_ctp_on_line.svg?sanitize=true" />\n</p>\n<p align="center">\n\tCopyright &copy; 2022-present <a href="https://github.com/catppuccin" target="_blank">Catppuccin Org</a>\n</p>\n<p align="center">\n\t<a href="https://github.com/catppuccin/catppuccin/blob/main/LICENSE"><img src="https://img.shields.io/static/v1.svg?style=for-the-badge&label=License&message=MIT&logoColor=d9e0ee&colorA=363a4f&colorB=b7bdf8"/></a>\n</p>\n',
     'author': 'backwardspy',
     'author_email': 'backwardspy@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['catppuccin', 'catppuccin.extras'] package_data = \ {'': ['*']} extras_require
-= \ {'pygments': ['pygments>=2.13.0,<3.0.0']} entry_points = \
-{'pygments.styles': ['catppuccin-frappe = ' 'catppuccin.extras.pygments:
-FrappeStyle', 'catppuccin-latte = catppuccin.extras.pygments:LatteStyle',
-'catppuccin-macchiato = ' 'catppuccin.extras.pygments:MacchiatoStyle',
-'catppuccin-mocha = ' 'catppuccin.extras.pygments:MochaStyle']} setup_kwargs =
-{ 'name': 'catppuccin', 'version': '1.2.0', 'description': 'ð Soothing
-pastel theme for Python.', 'long_description': '
+= \ {'pygments': ['pygments>=2.13.0,<3.0.0'], 'rich': ['rich>=13.3.5,<14.0.0']}
+entry_points = \ {'pygments.styles': ['catppuccin-frappe = '
+'catppuccin.extras.pygments:FrappeStyle', 'catppuccin-latte =
+catppuccin.extras.pygments:LatteStyle', 'catppuccin-macchiato = '
+'catppuccin.extras.pygments:MacchiatoStyle', 'catppuccin-mocha = '
+'catppuccin.extras.pygments:MochaStyle']} setup_kwargs = { 'name':
+'catppuccin', 'version': '1.3.0', 'description': 'ð Soothing pastel theme
+for Python.', 'long_description': '
                                 **** \n\t[Logo]
 \n\t[https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/
             transparent.png]\n\tCatppuccin for Python\n\t[https://
        raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/
                             transparent.png]\n ****
 \n\n
              \n\t[https://img.shields.io/github/stars/catppuccin/
```

### Comparing `catppuccin-1.2.0/PKG-INFO` & `catppuccin-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: catppuccin
-Version: 1.2.0
+Version: 1.3.0
 Summary: 🐍 Soothing pastel theme for Python.
 Author: backwardspy
 Author-email: backwardspy@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: pygments
+Provides-Extra: rich
 Requires-Dist: pygments (>=2.13.0,<3.0.0); extra == "pygments"
+Requires-Dist: rich (>=13.3.5,<14.0.0); extra == "rich"
 Description-Content-Type: text/markdown
 
 <h3 align="center">
 	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
 	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
 	Catppuccin for <a href="https://www.python.org/">Python</a>
 	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: catppuccin Version: 1.2.0 Summary: ð Soothing
+Metadata-Version: 2.1 Name: catppuccin Version: 1.3.0 Summary: ð Soothing
 pastel theme for Python. Author: backwardspy Author-email:
 backwardspy@gmail.com Requires-Python: >=3.7.2,<4.0.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: pygments Requires-Dist: pygments (>=2.13.0,<3.0.0); extra ==
-"pygments" Description-Content-Type: text/markdown
+Provides-Extra: pygments Provides-Extra: rich Requires-Dist: pygments
+(>=2.13.0,<3.0.0); extra == "pygments" Requires-Dist: rich (>=13.3.5,<14.0.0);
+extra == "rich" Description-Content-Type: text/markdown
                                   **** [Logo]
   [https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/
   transparent.png] Catppuccin for Python [https://raw.githubusercontent.com/
          catppuccin/catppuccin/main/assets/misc/transparent.png] ****
                [https://img.shields.io/github/stars/catppuccin/
        python?colorA=363a4f&colorB=b7bdf8&style=for-the-badge] [https://
                    img.shields.io/github/issues/catppuccin/
```

