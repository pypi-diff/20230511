# Comparing `tmp/types-aioboto3-lite-9.6.0.post1.tar.gz` & `tmp/types-aioboto3-lite-9.6.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aioboto3-lite-9.6.0.post1.tar", last modified: Fri Jul 15 14:40:32 2022, max compression
+gzip compressed data, was "types-aioboto3-lite-9.6.0.post2.tar", last modified: Sat Jul 23 22:01:37 2022, max compression
```

## Comparing `types-aioboto3-lite-9.6.0.post1.tar` & `types-aioboto3-lite-9.6.0.post2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 14:40:32.076518 types-aioboto3-lite-9.6.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)    69230 2022-07-15 14:40:32.076518 types-aioboto3-lite-9.6.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    59350 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 14:40:32.072518 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-07-15 14:40:25.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 14:40:32.072518 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/dynamodb/table.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 14:40:32.072518 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/experimental/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/experimental/async_chalice.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 14:40:25.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 14:40:32.072518 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/resources/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/resources/action.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/resources/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/resources/collection.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/resources/factory.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/resources/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 14:40:32.072518 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/s3/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3860 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/s3/cse.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1961 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/s3/inject.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3156 2022-07-15 14:40:24.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-07-15 14:40:25.000000 types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/version.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-15 14:40:32.076518 types-aioboto3-lite-9.6.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    33164 2022-07-15 14:40:25.000000 types-aioboto3-lite-9.6.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 14:40:32.072518 types-aioboto3-lite-9.6.0.post1/types_aioboto3_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    69230 2022-07-15 14:40:32.000000 types-aioboto3-lite-9.6.0.post1/types_aioboto3_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-07-15 14:40:32.000000 types-aioboto3-lite-9.6.0.post1/types_aioboto3_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 14:40:32.000000 types-aioboto3-lite-9.6.0.post1/types_aioboto3_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 14:40:32.000000 types-aioboto3-lite-9.6.0.post1/types_aioboto3_lite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)    22662 2022-07-15 14:40:32.000000 types-aioboto3-lite-9.6.0.post1/types_aioboto3_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-15 14:40:32.000000 types-aioboto3-lite-9.6.0.post1/types_aioboto3_lite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 22:01:37.604332 types-aioboto3-lite-9.6.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-07-23 22:01:30.000000 types-aioboto3-lite-9.6.0.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    69204 2022-07-23 22:01:37.604332 types-aioboto3-lite-9.6.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    59351 2022-07-23 22:01:30.000000 types-aioboto3-lite-9.6.0.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 22:01:37.604332 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      706 2022-07-23 22:01:30.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 22:01:37.604332 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/dynamodb/table.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 22:01:37.604332 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/experimental/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/experimental/async_chalice.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 22:01:30.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 22:01:37.604332 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/resources/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/resources/action.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/resources/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/resources/collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      596 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/resources/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/resources/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 22:01:37.604332 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/s3/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3860 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/s3/cse.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1961 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/s3/inject.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3167 2022-07-23 22:01:29.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-07-23 22:01:30.000000 types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-23 22:01:37.604332 types-aioboto3-lite-9.6.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)    33133 2022-07-23 22:01:30.000000 types-aioboto3-lite-9.6.0.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 22:01:37.604332 types-aioboto3-lite-9.6.0.post2/types_aioboto3_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    69204 2022-07-23 22:01:37.000000 types-aioboto3-lite-9.6.0.post2/types_aioboto3_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-07-23 22:01:37.000000 types-aioboto3-lite-9.6.0.post2/types_aioboto3_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 22:01:37.000000 types-aioboto3-lite-9.6.0.post2/types_aioboto3_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 22:01:37.000000 types-aioboto3-lite-9.6.0.post2/types_aioboto3_lite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)    22662 2022-07-23 22:01:37.000000 types-aioboto3-lite-9.6.0.post2/types_aioboto3_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-23 22:01:37.000000 types-aioboto3-lite-9.6.0.post2/types_aioboto3_lite.egg-info/top_level.txt
```

### Comparing `types-aioboto3-lite-9.6.0.post1/PKG-INFO` & `types-aioboto3-lite-9.6.0.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aioboto3-lite
-Version: 9.6.0.post1
-Summary: Type annotations for aioboto3 9.6.0 generated with mypy-boto3-builder 7.9.1
+Version: 9.6.0.post2
+Summary: Type annotations for aioboto3 9.6.0 generated with mypy-boto3-builder 7.10.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aioboto3_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -14,24 +14,23 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: essential
 Provides-Extra: accessanalyzer
 Provides-Extra: account
 Provides-Extra: acm
 Provides-Extra: acm-pca
@@ -328,14 +327,15 @@
 Provides-Extra: workdocs
 Provides-Extra: worklink
 Provides-Extra: workmail
 Provides-Extra: workmailmessageflow
 Provides-Extra: workspaces
 Provides-Extra: workspaces-web
 Provides-Extra: xray
+License-File: LICENSE
 
 <a id="types-aioboto3-lite"></a>
 
 # types-aioboto3-lite
 
 [![PyPI - types-aioboto3-lite](https://img.shields.io/pypi/v/types-aioboto3-lite.svg?color=blue)](https://pypi.org/project/types-aioboto3-lite)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aioboto3-lite.svg?color=blue)](https://pypi.org/project/types-aioboto3-lite)
@@ -349,15 +349,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.9.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.10.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [types-aioboto3-lite docs](https://youtype.github.io/types_aioboto3_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `types-aioboto3-lite-9.6.0.post1/README.md` & `types-aioboto3-lite-9.6.0.post2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.9.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.10.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [types-aioboto3-lite docs](https://youtype.github.io/types_aioboto3_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/__main__.py` & `types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3 9.6.0\n"
-        "Version:         9.6.0.post1\n"
-        "Builder version: 7.9.1\n"
+        "Version:         9.6.0.post2\n"
+        "Builder version: 7.10.0\n"
         "Docs:            https://pypi.org/project/types-aioboto3-lite/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("9.6.0.post1")
+    print("9.6.0.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/dynamodb/table.pyi` & `types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/dynamodb/table.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 _R = TypeVar("_R")
 
 def register_table_methods(base_classes: List[Any], **kwargs: Any) -> None: ...
 
 class CustomTableResource(TableResource):
     # FIXME: Signature of "batch_writer" incompatible with supertype "TableResource"
-    def batch_writer(  # type: ignore
+    def batch_writer(  # type: ignore [override]
         self,
         overwrite_by_pkeys: Optional[List[str]] = ...,
         flush_amount: int = ...,
         on_exit_loop_sleep: int = ...,
     ) -> "BatchWriter": ...
 
 class BatchWriter:
```

### Comparing `types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/experimental/async_chalice.pyi` & `types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/experimental/async_chalice.pyi`

 * *Files identical despite different names*

### Comparing `types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/resources/action.pyi` & `types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/resources/action.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 class AIOServiceAction(ServiceAction):
     def __init__(
         self,
         action_model: Action,
         factory: Optional[ResourceFactory] = ...,
         service_context: Optional[ServiceContext] = ...,
     ) -> None: ...
-    async def __call__(  # type: ignore
+    async def __call__(  # type: ignore [override]
         self, parent: ServiceResource, *args: Any, **kwargs: Any
     ) -> Union[ServiceResource, List[ServiceResource], Dict[str, Any]]: ...
 
 class AioBatchAction(ServiceAction):
-    async def __call__(  # type: ignore
+    async def __call__(  # type: ignore [override]
         self, parent: ServiceResource, *args: Any, **kwargs: Any
     ) -> List[Dict[str, Any]]: ...
 
 class AIOWaiterAction(WaiterAction):
-    async def __call__(  # type: ignore
+    async def __call__(  # type: ignore [override]
         self, parent: ServiceResource, *args: Any, **kwargs: Any
     ) -> None: ...
```

### Comparing `types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/resources/collection.pyi` & `types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/resources/collection.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Converted the __iter__
     """
 
     async def __anext__(self) -> Iterator[Any]: ...
     def __aiter__(self) -> Iterator[Any]: ...
     def __iter__(self) -> Iterator[Any]: ...
-    async def pages(self) -> Iterator[List[Any]]: ...  # type: ignore
+    async def pages(self) -> Iterator[List[Any]]: ...  # type: ignore [override]
 
 class AIOCollectionManager(CollectionManager):
     def __init__(
         self,
         collection_model: Collection,
         parent: ServiceResource,
         factory: ResourceFactory,
```

### Comparing `types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/resources/factory.pyi` & `types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/resources/factory.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 from boto3.utils import ServiceContext
 from botocore.hooks import BaseEventHooks
 
 logger: logging.Logger
 
 class AIOBoto3ResourceFactory(ResourceFactory):
     def __init__(self, emitter: BaseEventHooks) -> None: ...
-    async def load_from_definition(  # type: ignore
+    async def load_from_definition(  # type: ignore [override]
         self,
         resource_name: str,
         single_resource_json_definition: Any,
         service_context: ServiceContext,
     ) -> AIOBoto3ServiceResource: ...
```

### Comparing `types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/resources/response.pyi` & `types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/resources/response.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Union
 
 from boto3.resources.base import ServiceResource
 from boto3.resources.response import RawHandler, ResourceHandler
 
 class AIOResourceHandler(ResourceHandler):
-    async def __call__(  # type: ignore
+    async def __call__(  # type: ignore [override]
         self, parent: ServiceResource, params: Dict[str, Any], response: Dict[str, Any]
     ) -> Union[ServiceResource, List[ServiceResource]]: ...
 
 class AIORawHandler(RawHandler):
-    async def __call__(  # type: ignore
+    async def __call__(  # type: ignore [override]
         self, parent: ServiceResource, params: Dict[str, Any], response: Dict[str, Any]
     ) -> Dict[str, Any]: ...
```

### Comparing `types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/s3/cse.pyi` & `types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/s3/cse.pyi`

 * *Files identical despite different names*

### Comparing `types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/s3/inject.pyi` & `types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/s3/inject.pyi`

 * *Files identical despite different names*

### Comparing `types-aioboto3-lite-9.6.0.post1/aioboto3-stubs/session.pyi` & `types-aioboto3-lite-9.6.0.post2/aioboto3-stubs/session.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self,
         service_name: str,
         partition_name: str = "aws",
         allow_non_regional: bool = False,
     ) -> List[str]: ...
     def get_credentials(self) -> Credentials: ...
     def _register_default_handlers(self) -> None: ...
-    def client(  # type: ignore
+    def client(  # type: ignore [override]
         self,
         service_name: str,
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[str, bool, None] = ...,
         endpoint_url: Optional[str] = ...,
```

### Comparing `types-aioboto3-lite-9.6.0.post1/setup.py` & `types-aioboto3-lite-9.6.0.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,44 +3,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="types-aioboto3-lite",
-    version="9.6.0.post1",
+    version="9.6.0.post2",
     packages=["aioboto3-stubs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for aioboto3 9.6.0 generated with mypy-boto3-builder 7.9.1",
+    description="Type annotations for aioboto3 9.6.0 generated with mypy-boto3-builder 7.10.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Stubs Only",
     ],
     keywords="aioboto3 type-annotations aioboto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"aioboto3-stubs": ["py.typed", "*.pyi", "*/*.pyi"]},
-    python_requires=">=3.6",
+    package_data={"": ["LICENSE"], "aioboto3-stubs": ["py.typed", "*.pyi", "*/*.pyi"]},
+    python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aioboto3_docs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         "botocore-stubs",
```

### Comparing `types-aioboto3-lite-9.6.0.post1/types_aioboto3_lite.egg-info/PKG-INFO` & `types-aioboto3-lite-9.6.0.post2/types_aioboto3_lite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aioboto3-lite
-Version: 9.6.0.post1
-Summary: Type annotations for aioboto3 9.6.0 generated with mypy-boto3-builder 7.9.1
+Version: 9.6.0.post2
+Summary: Type annotations for aioboto3 9.6.0 generated with mypy-boto3-builder 7.10.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aioboto3_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -14,24 +14,23 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: essential
 Provides-Extra: accessanalyzer
 Provides-Extra: account
 Provides-Extra: acm
 Provides-Extra: acm-pca
@@ -328,14 +327,15 @@
 Provides-Extra: workdocs
 Provides-Extra: worklink
 Provides-Extra: workmail
 Provides-Extra: workmailmessageflow
 Provides-Extra: workspaces
 Provides-Extra: workspaces-web
 Provides-Extra: xray
+License-File: LICENSE
 
 <a id="types-aioboto3-lite"></a>
 
 # types-aioboto3-lite
 
 [![PyPI - types-aioboto3-lite](https://img.shields.io/pypi/v/types-aioboto3-lite.svg?color=blue)](https://pypi.org/project/types-aioboto3-lite)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aioboto3-lite.svg?color=blue)](https://pypi.org/project/types-aioboto3-lite)
@@ -349,15 +349,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.9.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.10.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [types-aioboto3-lite docs](https://youtype.github.io/types_aioboto3_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `types-aioboto3-lite-9.6.0.post1/types_aioboto3_lite.egg-info/SOURCES.txt` & `types-aioboto3-lite-9.6.0.post2/types_aioboto3_lite.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 aioboto3-stubs/__init__.pyi
 aioboto3-stubs/__main__.py
 aioboto3-stubs/py.typed
 aioboto3-stubs/session.pyi
 aioboto3-stubs/version.py
```

### Comparing `types-aioboto3-lite-9.6.0.post1/types_aioboto3_lite.egg-info/requires.txt` & `types-aioboto3-lite-9.6.0.post2/types_aioboto3_lite.egg-info/requires.txt`

 * *Files identical despite different names*

