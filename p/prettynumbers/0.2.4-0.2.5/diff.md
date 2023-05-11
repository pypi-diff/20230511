# Comparing `tmp/prettynumbers-0.2.4.tar.gz` & `tmp/prettynumbers-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettynumbers-0.2.4.tar", max compression
+gzip compressed data, was "prettynumbers-0.2.5.tar", max compression
```

## Comparing `prettynumbers-0.2.4.tar` & `prettynumbers-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    14849 2023-05-10 11:11:21.340578 prettynumbers-0.2.4/LICENSE.txt
--rw-r--r--   0        0        0     1138 2023-05-10 11:11:21.340578 prettynumbers-0.2.4/README.md
--rw-r--r--   0        0        0      114 2023-05-10 11:11:21.340578 prettynumbers-0.2.4/pretty_numbers/__init__.py
--rwxr-xr-x   0        0        0     1915 2023-05-10 11:11:21.340578 prettynumbers-0.2.4/pretty_numbers/pretty_numbers.py
--rw-r--r--   0        0        0        0 2023-05-10 11:11:21.340578 prettynumbers-0.2.4/pretty_numbers/py.typed
--rwxr-xr-x   0        0        0     3303 2023-05-10 11:11:21.340578 prettynumbers-0.2.4/pretty_numbers/test_pretty_numbers.py
--rw-r--r--   0        0        0      752 2023-05-10 11:11:21.340578 prettynumbers-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 prettynumbers-0.2.4/setup.py
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 prettynumbers-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    14849 2023-05-10 16:25:20.720892 prettynumbers-0.2.5/LICENSE.txt
+-rw-r--r--   0        0        0     1138 2023-05-10 16:25:20.720892 prettynumbers-0.2.5/README.md
+-rw-r--r--   0        0        0      114 2023-05-10 16:25:20.720892 prettynumbers-0.2.5/pretty_numbers/__init__.py
+-rwxr-xr-x   0        0        0     1915 2023-05-10 16:25:20.720892 prettynumbers-0.2.5/pretty_numbers/pretty_numbers.py
+-rw-r--r--   0        0        0        0 2023-05-10 16:25:20.720892 prettynumbers-0.2.5/pretty_numbers/py.typed
+-rw-r--r--   0        0        0      752 2023-05-10 16:25:20.720892 prettynumbers-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 prettynumbers-0.2.5/setup.py
+-rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 prettynumbers-0.2.5/PKG-INFO
```

### Comparing `prettynumbers-0.2.4/LICENSE.txt` & `prettynumbers-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.4/README.md` & `prettynumbers-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.4/pretty_numbers/pretty_numbers.py` & `prettynumbers-0.2.5/pretty_numbers/pretty_numbers.py`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.2.4/pyproject.toml` & `prettynumbers-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prettynumbers"
-version = "0.2.4"
+version = "0.2.5"
 authors = ["gerardk <gerardk@gmail.com>"]
 description="Display a range of numbers in a human readable way"
 license="GNU GENERAL PUBLIC LICENSE"
 packages = [{include = "pretty_numbers"}]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `prettynumbers-0.2.4/setup.py` & `prettynumbers-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['pretty_numbers']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'prettynumbers',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'Display a range of numbers in a human readable way',
     'long_description': '[![vfxGer](https://circleci.com/gh/vfxGer/pretty-numbers.svg?style=svg)](BUILD)\n[![codecov.io](https://codecov.io/gh/vfxGer/pretty-numbers/coverage.svg?branch=master)](https://codecov.io/gh/vfxGer/pretty-numbers)\n[![Code Climate](https://codeclimate.com/github/vfxGer/pretty-numbers/badges/gpa.svg)](https://codeclimate.com/github/vfxGer/pretty-numbers)\n[![PYPI](https://img.shields.io/pypi/v/prettynumbers.svg)](https://pypi.python.org/pypi/prettynumbers)\n\n# Pretty Numbers\n\nPretty Numbers is a simple Python package that displays long series of numbers in a more human readable way.\n\nI have used it for displaying frames of a render in a more human readable way or issues of comic books. It allows the user to quickly see what is included and what is missing.\n\n## Installation\n\nIt is available on [PyPi](https://pypi.python.org/pypi/prettynumbers) meaning you can just:\n\n    pip install prettynumbers\n\n## Usage\n\n```python\nimport pretty_numbers\npretty_numbers.getPrettyTextFromNumbers([1001, 99, 1004, 1005, 1003, 1008,\n                                         1002, 1007, 1010, 1006, 1111, 1009])\n```\n\nReturns:\n\n    "99,1001-1010,1111"\n',
     'author': 'gerardk',
     'author_email': 'gerardk@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `prettynumbers-0.2.4/PKG-INFO` & `prettynumbers-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.2.4
+Version: 0.2.5
 Summary: Display a range of numbers in a human readable way
 License: GNU GENERAL PUBLIC LICENSE
 Author: gerardk
 Author-email: gerardk@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

