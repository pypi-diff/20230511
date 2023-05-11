# Comparing `tmp/sqle-0.0.0a0.tar.gz` & `tmp/sqle-0.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqle-0.0.0a0.tar", max compression
+gzip compressed data, was "sqle-0.0.0a1.tar", max compression
```

## Comparing `sqle-0.0.0a0.tar` & `sqle-0.0.0a1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-04-13 11:39:12.312030 sqle-0.0.0a0/LICENSE
--rw-r--r--   0        0        0      150 2023-04-13 11:38:09.353891 sqle-0.0.0a0/README.md
--rw-r--r--   0        0        0      454 2023-04-15 11:56:58.394936 sqle-0.0.0a0/pyproject.toml
--rw-r--r--   0        0        0      146 2023-04-11 16:45:03.469232 sqle-0.0.0a0/sqle/__init__.py
--rw-r--r--   0        0        0     3019 2023-04-13 11:31:41.739519 sqle-0.0.0a0/sqle/adapter.py
--rw-r--r--   0        0        0        0 2023-03-11 12:58:20.091961 sqle-0.0.0a0/sqle/contrib/__init__.py
--rw-r--r--   0        0        0      150 2023-03-08 11:10:17.217492 sqle-0.0.0a0/sqle/contrib/class_property.py
--rw-r--r--   0        0        0      157 2023-04-12 15:49:20.785386 sqle-0.0.0a0/sqle/contrib/text.py
--rw-r--r--   0        0        0      435 2023-04-08 13:03:01.529379 sqle-0.0.0a0/sqle/exceptions.py
--rw-r--r--   0        0        0     2331 2023-04-12 15:50:05.438389 sqle-0.0.0a0/sqle/query.py
--rw-r--r--   0        0        0       46 2023-02-15 15:56:29.472877 sqle-0.0.0a0/sqle/settings.py
--rw-r--r--   0        0        0     3166 2023-04-14 12:53:03.034804 sqle-0.0.0a0/sqle/sql.py
--rw-r--r--   0        0        0      739 2023-04-15 12:00:40.576809 sqle-0.0.0a0/setup.py
--rw-r--r--   0        0        0      527 2023-04-15 12:00:40.577069 sqle-0.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-13 11:39:12.312030 sqle-0.0.0a1/LICENSE
+-rw-r--r--   0        0        0      150 2023-04-15 12:19:38.626033 sqle-0.0.0a1/README.md
+-rw-r--r--   0        0        0      454 2023-05-11 13:05:52.210381 sqle-0.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-05-11 13:05:41.995233 sqle-0.0.0a1/sqle/__init__.py
+-rw-r--r--   0        0        0     3116 2023-05-11 12:53:41.995931 sqle-0.0.0a1/sqle/adapter.py
+-rw-r--r--   0        0        0        0 2023-03-11 12:58:20.091961 sqle-0.0.0a1/sqle/contrib/__init__.py
+-rw-r--r--   0        0        0      150 2023-03-08 11:10:17.217492 sqle-0.0.0a1/sqle/contrib/class_property.py
+-rw-r--r--   0        0        0      157 2023-04-12 15:49:20.785386 sqle-0.0.0a1/sqle/contrib/text.py
+-rw-r--r--   0        0        0      435 2023-04-08 13:03:01.529379 sqle-0.0.0a1/sqle/exceptions.py
+-rw-r--r--   0        0        0     2331 2023-04-15 12:21:27.817079 sqle-0.0.0a1/sqle/query.py
+-rw-r--r--   0        0        0       46 2023-02-15 15:56:29.472877 sqle-0.0.0a1/sqle/settings.py
+-rw-r--r--   0        0        0     3166 2023-04-15 12:21:27.830628 sqle-0.0.0a1/sqle/sql.py
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 sqle-0.0.0a1/PKG-INFO
```

### Comparing `sqle-0.0.0a0/LICENSE` & `sqle-0.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqle-0.0.0a0/sqle/adapter.py` & `sqle-0.0.0a1/sqle/adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from abc import ABC, abstractclassmethod
 from functools import cached_property
-from typing import Callable, TYPE_CHECKING, Type, TypeVar, Any, Protocol
-from functools import cached_property
+from typing import TYPE_CHECKING, Any, Callable, Protocol, Type, TypeVar
+
 from .exceptions import SerizlierNotFound
 
 if TYPE_CHECKING:
     from .sql import SQLEnvironment
 
 
 class StringRepresentation(Protocol):
@@ -20,18 +20,22 @@
 
 class AdapterSerializer:
     def serialize_params(self, values: dict[str, Any]) -> dict[str, Any]:
         return {param: self.serialize_param(value) for param, value in values.items()}
 
     def serialize_param(self, value: Any, name: str = NO_NAME_PARAM_NAME) -> Any:
         match value:
+            case bool():
+                _value = "true" if value else "false"
             case int() | float():
                 _value = str(value)
             case str():
                 _value = self.serialize_string(value)
+            case None:
+                _value = "NULL"
             case _:
                 _value = self.serialize_other_object(value)
 
         return _value
 
     @staticmethod
     def serialize_number(value: int | float) -> str:
```

### Comparing `sqle-0.0.0a0/sqle/query.py` & `sqle-0.0.0a1/sqle/query.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from inspect import stack
 from os.path import isabs
 from pathlib import Path
 from typing import Type, TypeVar
 
 from jinja2 import Environment, FileSystemLoader
-from .contrib.text import clear_text
 
+from .contrib.text import clear_text
 from .exceptions import TSQLValueError
 
 T = TypeVar("T", bound="Query")
 
 
 class Query:
     TEXT_OR_PATH_MUST_BE_PASSER_ERROR = TSQLValueError(
```

### Comparing `sqle-0.0.0a0/sqle/sql.py` & `sqle-0.0.0a1/sqle/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from collections.abc import Mapping
 from inspect import isclass, stack
 from os.path import isabs
 from pathlib import Path
-from typing import Callable, Type, TypeVar, Any
+from typing import Any, Callable, Type, TypeVar
 
 from jinja2 import Environment
 from typing_extensions import get_type_hints
 
 from .adapter import AdapterFactory
 from .contrib.class_property import classproperty
 from .exceptions import TSQLValueError
```

### Comparing `sqle-0.0.0a0/PKG-INFO` & `sqle-0.0.0a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: sqle
-Version: 0.0.0a0
+Version: 0.0.0a1
 Summary: 
 License: MIT
 Author: acrius
 Author-email: acrius@mail.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Description-Content-Type: text/markdown
 
-# TSQL
+# SQLE
 
 Python package designed to execute pure sql queries.
 
 | :exclamation:  This is alpha version    |
 |-----------------------------------------|
```

