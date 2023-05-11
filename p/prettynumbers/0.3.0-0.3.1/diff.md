# Comparing `tmp/prettynumbers-0.3.0.tar.gz` & `tmp/prettynumbers-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettynumbers-0.3.0.tar", max compression
+gzip compressed data, was "prettynumbers-0.3.1.tar", max compression
```

## Comparing `prettynumbers-0.3.0.tar` & `prettynumbers-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    14849 2023-05-11 09:02:29.316650 prettynumbers-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1138 2023-05-11 09:02:29.316650 prettynumbers-0.3.0/README.md
--rw-r--r--   0        0        0      138 2023-05-11 09:02:29.316650 prettynumbers-0.3.0/pretty_numbers/__init__.py
--rwxr-xr-x   0        0        0     2580 2023-05-11 09:02:29.316650 prettynumbers-0.3.0/pretty_numbers/pretty_numbers.py
--rw-r--r--   0        0        0        0 2023-05-11 09:02:29.316650 prettynumbers-0.3.0/pretty_numbers/py.typed
--rw-r--r--   0        0        0      752 2023-05-11 09:02:29.316650 prettynumbers-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 prettynumbers-0.3.0/setup.py
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 prettynumbers-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    14849 2023-05-11 16:46:48.185867 prettynumbers-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     1138 2023-05-11 16:46:48.185867 prettynumbers-0.3.1/README.md
+-rw-r--r--   0        0        0      138 2023-05-11 16:46:48.185867 prettynumbers-0.3.1/pretty_numbers/__init__.py
+-rwxr-xr-x   0        0        0     2580 2023-05-11 16:46:48.185867 prettynumbers-0.3.1/pretty_numbers/pretty_numbers.py
+-rw-r--r--   0        0        0        0 2023-05-11 16:46:48.185867 prettynumbers-0.3.1/pretty_numbers/py.typed
+-rw-r--r--   0        0        0      808 2023-05-11 16:46:48.185867 prettynumbers-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 prettynumbers-0.3.1/setup.py
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 prettynumbers-0.3.1/PKG-INFO
```

### Comparing `prettynumbers-0.3.0/LICENSE.txt` & `prettynumbers-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.0/README.md` & `prettynumbers-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.0/pretty_numbers/pretty_numbers.py` & `prettynumbers-0.3.1/pretty_numbers/pretty_numbers.py`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.0/pyproject.toml` & `prettynumbers-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "prettynumbers"
-version = "0.3.0"
+version = "0.3.1"
 authors = ["gerardk <gerardk@gmail.com>"]
 description="Display a range of numbers in a human readable way"
 license="GNU GENERAL PUBLIC LICENSE"
 packages = [{include = "pretty_numbers"}]
 readme = "README.md"
+repository = "https://github.com/vfxGer/pretty-numbers"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.3"
 isort = "^5.12.0"
```

### Comparing `prettynumbers-0.3.0/setup.py` & `prettynumbers-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 ['pretty_numbers']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'prettynumbers',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Display a range of numbers in a human readable way',
     'long_description': '[![vfxGer](https://circleci.com/gh/vfxGer/pretty-numbers.svg?style=svg)](BUILD)\n[![codecov.io](https://codecov.io/gh/vfxGer/pretty-numbers/coverage.svg?branch=master)](https://codecov.io/gh/vfxGer/pretty-numbers)\n[![Code Climate](https://codeclimate.com/github/vfxGer/pretty-numbers/badges/gpa.svg)](https://codeclimate.com/github/vfxGer/pretty-numbers)\n[![PYPI](https://img.shields.io/pypi/v/prettynumbers.svg)](https://pypi.python.org/pypi/prettynumbers)\n\n# Pretty Numbers\n\nPretty Numbers is a simple Python package that displays long series of numbers in a more human readable way.\n\nI have used it for displaying frames of a render in a more human readable way or issues of comic books. It allows the user to quickly see what is included and what is missing.\n\n## Installation\n\nIt is available on [PyPi](https://pypi.python.org/pypi/prettynumbers) meaning you can just:\n\n    pip install prettynumbers\n\n## Usage\n\n```python\nimport pretty_numbers\npretty_numbers.getPrettyTextFromNumbers([1001, 99, 1004, 1005, 1003, 1008,\n                                         1002, 1007, 1010, 1006, 1111, 1009])\n```\n\nReturns:\n\n    "99,1001-1010,1111"\n',
     'author': 'gerardk',
     'author_email': 'gerardk@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/vfxGer/pretty-numbers',
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.8.0,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `prettynumbers-0.3.0/PKG-INFO` & `prettynumbers-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.3.0
+Version: 0.3.1
 Summary: Display a range of numbers in a human readable way
+Home-page: https://github.com/vfxGer/pretty-numbers
 License: GNU GENERAL PUBLIC LICENSE
 Author: gerardk
 Author-email: gerardk@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/vfxGer/pretty-numbers
 Description-Content-Type: text/markdown
 
 [![vfxGer](https://circleci.com/gh/vfxGer/pretty-numbers.svg?style=svg)](BUILD)
 [![codecov.io](https://codecov.io/gh/vfxGer/pretty-numbers/coverage.svg?branch=master)](https://codecov.io/gh/vfxGer/pretty-numbers)
 [![Code Climate](https://codeclimate.com/github/vfxGer/pretty-numbers/badges/gpa.svg)](https://codeclimate.com/github/vfxGer/pretty-numbers)
 [![PYPI](https://img.shields.io/pypi/v/prettynumbers.svg)](https://pypi.python.org/pypi/prettynumbers)
```

