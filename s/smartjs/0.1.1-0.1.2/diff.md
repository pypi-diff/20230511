# Comparing `tmp/smartjs-0.1.1.tar.gz` & `tmp/smartjs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartjs-0.1.1.tar", max compression
+gzip compressed data, was "smartjs-0.1.2.tar", max compression
```

## Comparing `smartjs-0.1.1.tar` & `smartjs-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      376 2023-05-10 13:12:48.909432 smartjs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      183 2023-05-05 14:06:40.683599 smartjs-0.1.1/smartjs/__init__.py
--rw-r--r--   0        0        0    13770 2023-05-10 13:11:56.805246 smartjs-0.1.1/smartjs/base.py
--rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.1.1/smartjs/constants.py
--rw-r--r--   0        0        0     4970 2023-05-10 13:03:07.134383 smartjs-0.1.1/smartjs/elements.py
--rw-r--r--   0        0        0     5808 2023-05-10 13:03:37.759379 smartjs-0.1.1/smartjs/functions.py
--rw-r--r--   0        0        0    11908 2023-05-10 11:42:41.551886 smartjs-0.1.1/smartjs/javascript.py
--rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.1.1/smartjs/page.py
--rw-r--r--   0        0        0      994 2023-05-07 01:38:04.688449 smartjs-0.1.1/smartjs/path.py
--rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.1.1/smartjs/style.py
--rw-r--r--   0        0        0      658 2023-05-10 13:13:00.510127 smartjs-0.1.1/setup.py
--rw-r--r--   0        0        0      407 2023-05-10 13:13:00.510525 smartjs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      376 2023-05-11 05:41:55.559326 smartjs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-05-11 01:47:48.346629 smartjs-0.1.2/smartjs/__init__.py
+-rw-r--r--   0        0        0    16232 2023-05-11 05:02:23.341856 smartjs-0.1.2/smartjs/base.py
+-rw-r--r--   0        0        0     1277 2023-05-11 05:35:54.145444 smartjs-0.1.2/smartjs/collection.py
+-rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.1.2/smartjs/constants.py
+-rw-r--r--   0        0        0     4970 2023-05-10 13:03:07.134383 smartjs-0.1.2/smartjs/elements.py
+-rw-r--r--   0        0        0     6296 2023-05-11 01:14:16.811102 smartjs-0.1.2/smartjs/functions.py
+-rw-r--r--   0        0        0    11908 2023-05-10 11:42:41.551886 smartjs-0.1.2/smartjs/javascript.py
+-rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.1.2/smartjs/page.py
+-rw-r--r--   0        0        0     1782 2023-05-11 05:41:46.920516 smartjs-0.1.2/smartjs/path.py
+-rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.1.2/smartjs/style.py
+-rw-r--r--   0        0        0      658 2023-05-11 05:42:09.593527 smartjs-0.1.2/setup.py
+-rw-r--r--   0        0        0      407 2023-05-11 05:42:09.593741 smartjs-0.1.2/PKG-INFO
```

### Comparing `smartjs-0.1.1/smartjs/constants.py` & `smartjs-0.1.2/smartjs/constants.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.1/smartjs/elements.py` & `smartjs-0.1.2/smartjs/elements.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.1/smartjs/functions.py` & `smartjs-0.1.2/smartjs/functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,25 +29,32 @@
         'get_group_or_return_value',
         'get_iso_datetimes',
         'get_iso_dates',
         'get_first_iso_datetime',
         'get_first_iso_date',
         'underscore_to_hyphen',
         'list_of_type',
-        'set_filtered'
+        'set_filtered',
+        'first_of_type',
+        'parse_list'
 ]
 
 import calendar
 import re
 import datetime
-from typing import Callable, Optional, Collection, Union
+from typing import Callable, Optional, Collection, Union, Any
+from collections import deque, UserList
 from unidecode import unidecode
 from smartjs.constants import *
 
 
+def parse_list(item: Any) -> list:
+    return [*item] if isinstance(item, (list, set, deque, UserList, tuple)) else [item] if item else []
+
+
 def underscore_to_hyphen(value: str) -> str:
     return value.replace("_", "-")
 
 
 def normalize(string: str) -> str:
     return ' '.join(unidecode(string).split()).lower()
 
@@ -80,14 +87,21 @@
 def set_filtered(items: Collection, func: Callable = lambda x: x not in [None, '']) -> set:
     return set(list_filtered([*items], func))
 
 
 def list_of_type(items: Collection, types: Union[type[GenericType], tuple[type[GenericType]]]) -> list[GenericType]:
     return [item for item in items if isinstance(item, types)]
 
+def first_of_type(items: Collection, types: Union[type[GenericType], tuple[type[GenericType]]]) -> GenericType:
+    gen = (item for item in items if isinstance(item, types))
+    try:
+        return next(gen)
+    except StopIteration:
+        return None
+
 
 def list_of_strings(items: Collection) -> list[str]:
     return [str(i) for i in list_filtered(items)]
 
 
 def join(items: Collection, sep: str = ' ', end: str = '') -> str:
     return sep.join([str(item) for item in items if item not in [None, '']]) + end
```

### Comparing `smartjs-0.1.1/smartjs/javascript.py` & `smartjs-0.1.2/smartjs/javascript.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.1/smartjs/page.py` & `smartjs-0.1.2/smartjs/page.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.1/smartjs/style.py` & `smartjs-0.1.2/smartjs/style.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.1/setup.py` & `smartjs-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'smartjs',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Project for creation of javascript, html and style elements for web pages.',
     'long_description': None,
     'author': 'Daniel Victor',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

