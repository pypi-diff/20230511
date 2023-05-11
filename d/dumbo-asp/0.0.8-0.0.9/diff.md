# Comparing `tmp/dumbo_asp-0.0.8.tar.gz` & `tmp/dumbo_asp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumbo_asp-0.0.8.tar", max compression
+gzip compressed data, was "dumbo_asp-0.0.9.tar", max compression
```

## Comparing `dumbo_asp-0.0.8.tar` & `dumbo_asp-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-01-09 17:04:55.577097 dumbo_asp-0.0.8/LICENSE
--rw-r--r--   0        0        0        0 2023-01-09 17:12:18.538163 dumbo_asp-0.0.8/dumbo_asp/__init__.py
--rw-r--r--   0        0        0    16433 2023-01-13 07:59:49.520872 dumbo_asp-0.0.8/dumbo_asp/primitives.py
--rw-r--r--   0        0        0     1595 2023-01-12 17:59:15.581184 dumbo_asp-0.0.8/dumbo_asp/utils.py
--rw-r--r--   0        0        0      519 2023-01-13 07:59:49.524872 dumbo_asp-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 dumbo_asp-0.0.8/setup.py
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 dumbo_asp-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-09 17:04:55.577097 dumbo_asp-0.0.9/LICENSE
+-rw-r--r--   0        0        0        0 2023-01-09 17:12:18.538163 dumbo_asp-0.0.9/dumbo_asp/__init__.py
+-rw-r--r--   0        0        0    16440 2023-01-17 16:55:07.470742 dumbo_asp-0.0.9/dumbo_asp/primitives.py
+-rw-r--r--   0        0        0      879 2023-01-17 16:55:07.458742 dumbo_asp-0.0.9/dumbo_asp/utils.py
+-rw-r--r--   0        0        0      468 2023-01-17 17:04:06.998628 dumbo_asp-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 dumbo_asp-0.0.9/setup.py
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 dumbo_asp-0.0.9/PKG-INFO
```

### Comparing `dumbo_asp-0.0.8/LICENSE` & `dumbo_asp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dumbo_asp-0.0.8/dumbo_asp/primitives.py` & `dumbo_asp-0.0.9/dumbo_asp/primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, Callable, Optional, Iterable, Union
 
 import clingo
 import clingo.ast
 import typeguard
 
 from dumbo_asp import utils
-from dumbo_asp.utils import validate, ValidationError
+from dumbo_utils.validation import validate, ValidationError
 
 
 @typeguard.typechecked
 class Parser:
     @dataclasses.dataclass(frozen=True)
     class Error(ValueError):
         parsed_string: str
```

### Comparing `dumbo_asp-0.0.8/setup.py` & `dumbo_asp-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,20 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Pillow>=9.3.0,<10.0.0',
  'cairocffi>=1.4.0,<2.0.0',
  'dateutils>=0.6.12,<0.7.0',
- 'igraph>=0.10.2,<0.11.0',
- 'rich>=13.0.1,<14.0.0',
- 'typeguard>=2.13.3,<3.0.0',
- 'typer>=0.7.0,<0.8.0',
- 'valid8>=5.1.2,<6.0.0']
+ 'dumbo-utils>=0.1.1,<0.2.0',
+ 'igraph>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'dumbo-asp',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Utilities for Answer Set Programming',
     'long_description': 'None',
     'author': 'Mario Alviano',
     'author_email': 'mario.alviano@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dumbo_asp-0.0.8/PKG-INFO` & `dumbo_asp-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: dumbo-asp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for Answer Set Programming
 Author: Mario Alviano
 Author-email: mario.alviano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.3.0,<10.0.0)
 Requires-Dist: cairocffi (>=1.4.0,<2.0.0)
 Requires-Dist: dateutils (>=0.6.12,<0.7.0)
+Requires-Dist: dumbo-utils (>=0.1.1,<0.2.0)
 Requires-Dist: igraph (>=0.10.2,<0.11.0)
-Requires-Dist: rich (>=13.0.1,<14.0.0)
-Requires-Dist: typeguard (>=2.13.3,<3.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
-Requires-Dist: valid8 (>=5.1.2,<6.0.0)
```

