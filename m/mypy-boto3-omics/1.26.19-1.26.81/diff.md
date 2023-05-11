# Comparing `tmp/mypy-boto3-omics-1.26.19.tar.gz` & `tmp/mypy-boto3-omics-1.26.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-omics-1.26.19.tar", last modified: Tue Nov 29 20:35:12 2022, max compression
+gzip compressed data, was "mypy-boto3-omics-1.26.81.tar", last modified: Tue Feb 28 20:28:07 2023, max compression
```

## Comparing `mypy-boto3-omics-1.26.19.tar` & `mypy-boto3-omics-1.26.81.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.137234 mypy-boto3-omics-1.26.19/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-29 20:34:52.000000 mypy-boto3-omics-1.26.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    27582 2022-11-29 20:35:12.129234 mypy-boto3-omics-1.26.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    26153 2022-11-29 20:34:52.000000 mypy-boto3-omics-1.26.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.125234 mypy-boto3-omics-1.26.19/mypy_boto3_omics/
--rw-r--r--   0 runner    (1001) docker     (122)     6987 2022-11-29 20:34:52.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6986 2022-11-29 20:34:52.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      900 2022-11-29 20:34:53.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    55773 2022-11-29 20:34:53.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    55669 2022-11-29 20:34:53.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    14643 2022-11-29 20:34:54.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    14641 2022-11-29 20:34:54.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    19505 2022-11-29 20:34:53.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)    19486 2022-11-29 20:34:53.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 20:34:53.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    87464 2022-11-29 20:34:56.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    87324 2022-11-29 20:34:55.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-29 20:34:52.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/version.py
--rw-r--r--   0 runner    (1001) docker     (122)    15061 2022-11-29 20:34:53.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/waiter.py
--rw-r--r--   0 runner    (1001) docker     (122)    15045 2022-11-29 20:34:53.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.129234 mypy-boto3-omics-1.26.19/mypy_boto3_omics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    27582 2022-11-29 20:35:11.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      697 2022-11-29 20:35:11.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 20:35:11.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 20:35:11.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-29 20:35:11.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-29 20:35:11.000000 mypy-boto3-omics-1.26.19/mypy_boto3_omics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 20:35:12.137234 mypy-boto3-omics-1.26.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1939 2022-11-29 20:34:52.000000 mypy-boto3-omics-1.26.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.510319 mypy-boto3-omics-1.26.81/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27631 2023-02-28 20:28:07.510319 mypy-boto3-omics-1.26.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26152 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.510319 mypy-boto3-omics-1.26.81/mypy_boto3_omics/
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55790 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55686 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-02-28 20:27:56.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-02-28 20:27:56.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    87788 2023-02-28 20:27:58.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87646 2023-02-28 20:27:57.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.510319 mypy-boto3-omics-1.26.81/mypy_boto3_omics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27631 2023-02-28 20:28:07.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-02-28 20:28:07.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:28:07.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:28:07.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-28 20:28:07.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-28 20:28:07.000000 mypy-boto3-omics-1.26.81/mypy_boto3_omics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 20:28:07.510319 mypy-boto3-omics-1.26.81/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-28 20:27:55.000000 mypy-boto3-omics-1.26.81/setup.py
```

### Comparing `mypy-boto3-omics-1.26.19/LICENSE` & `mypy-boto3-omics-1.26.81/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.26.19/PKG-INFO` & `mypy-boto3-omics-1.26.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.26.19
-Summary: Type annotations for boto3.Omics 1.26.19 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.81
+Summary: Type annotations for boto3.Omics 1.26.81 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-omics?color=blue)](https://pypistats.org/packages/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-omics-1.26.19/README.md` & `mypy-boto3-omics-1.26.81/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-omics?color=blue)](https://pypistats.org/packages/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/__init__.py` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/__init__.pyi` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/__main__.py` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Omics 1.26.19\nVersion:         1.26.19\nBuilder version:"
-        " 7.11.11\nDocs:           "
+        "Type annotations for boto3.Omics 1.26.81\nVersion:         1.26.81\nBuilder version:"
+        " 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.19")
+    print("1.26.81")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/client.py` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .literals import (
     ReadSetFileType,
     ReferenceFileType,
     RunLogLevelType,
     StoreFormatType,
     TaskStatusType,
     WorkflowEngineType,
+    WorkflowTypeType,
 )
 from .paginator import (
     ListAnnotationImportJobsPaginator,
     ListAnnotationStoresPaginator,
     ListReadSetActivationJobsPaginator,
     ListReadSetExportJobsPaginator,
     ListReadSetImportJobsPaginator,
@@ -586,15 +587,15 @@
         """
 
     def get_workflow(
         self,
         *,
         id: str,
         export: Sequence[Literal["DEFINITION"]] = ...,
-        type: Literal["PRIVATE"] = ...
+        type: WorkflowTypeType = ...
     ) -> GetWorkflowResponseTypeDef:
         """
         Gets information about a workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#get_workflow)
         """
@@ -827,15 +828,15 @@
 
     def list_workflows(
         self,
         *,
         maxResults: int = ...,
         name: str = ...,
         startingToken: str = ...,
-        type: Literal["PRIVATE"] = ...
+        type: WorkflowTypeType = ...
     ) -> ListWorkflowsResponseTypeDef:
         """
         Retrieves a list of workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_workflows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#list_workflows)
         """
@@ -860,15 +861,15 @@
         self,
         *,
         sequenceStoreId: str,
         sources: Sequence[StartReadSetActivationJobSourceItemTypeDef],
         clientToken: str = ...
     ) -> StartReadSetActivationJobResponseTypeDef:
         """
-        Starts a read set activation job.
+        Activates an archived read set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_activation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#start_read_set_activation_job)
         """
 
     def start_read_set_export_job(
         self,
@@ -876,15 +877,15 @@
         destination: str,
         roleArn: str,
         sequenceStoreId: str,
         sources: Sequence[ExportReadSetTypeDef],
         clientToken: str = ...
     ) -> StartReadSetExportJobResponseTypeDef:
         """
-        Starts a read set export job.
+        Exports a read set to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#start_read_set_export_job)
         """
 
     def start_read_set_import_job(
         self,
@@ -927,15 +928,15 @@
         parameters: Mapping[str, Any] = ...,
         priority: int = ...,
         runGroupId: str = ...,
         runId: str = ...,
         storageCapacity: int = ...,
         tags: Mapping[str, str] = ...,
         workflowId: str = ...,
-        workflowType: Literal["PRIVATE"] = ...
+        workflowType: WorkflowTypeType = ...
     ) -> StartRunResponseTypeDef:
         """
         Starts a run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#start_run)
         """
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/client.pyi` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .literals import (
     ReadSetFileType,
     ReferenceFileType,
     RunLogLevelType,
     StoreFormatType,
     TaskStatusType,
     WorkflowEngineType,
+    WorkflowTypeType,
 )
 from .paginator import (
     ListAnnotationImportJobsPaginator,
     ListAnnotationStoresPaginator,
     ListReadSetActivationJobsPaginator,
     ListReadSetExportJobsPaginator,
     ListReadSetImportJobsPaginator,
@@ -543,15 +544,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#get_variant_store)
         """
     def get_workflow(
         self,
         *,
         id: str,
         export: Sequence[Literal["DEFINITION"]] = ...,
-        type: Literal["PRIVATE"] = ...
+        type: WorkflowTypeType = ...
     ) -> GetWorkflowResponseTypeDef:
         """
         Gets information about a workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.get_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#get_workflow)
         """
@@ -767,15 +768,15 @@
         """
     def list_workflows(
         self,
         *,
         maxResults: int = ...,
         name: str = ...,
         startingToken: str = ...,
-        type: Literal["PRIVATE"] = ...
+        type: WorkflowTypeType = ...
     ) -> ListWorkflowsResponseTypeDef:
         """
         Retrieves a list of workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.list_workflows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#list_workflows)
         """
@@ -798,30 +799,30 @@
         self,
         *,
         sequenceStoreId: str,
         sources: Sequence[StartReadSetActivationJobSourceItemTypeDef],
         clientToken: str = ...
     ) -> StartReadSetActivationJobResponseTypeDef:
         """
-        Starts a read set activation job.
+        Activates an archived read set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_activation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#start_read_set_activation_job)
         """
     def start_read_set_export_job(
         self,
         *,
         destination: str,
         roleArn: str,
         sequenceStoreId: str,
         sources: Sequence[ExportReadSetTypeDef],
         clientToken: str = ...
     ) -> StartReadSetExportJobResponseTypeDef:
         """
-        Starts a read set export job.
+        Exports a read set to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_read_set_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#start_read_set_export_job)
         """
     def start_read_set_import_job(
         self,
         *,
@@ -861,15 +862,15 @@
         parameters: Mapping[str, Any] = ...,
         priority: int = ...,
         runGroupId: str = ...,
         runId: str = ...,
         storageCapacity: int = ...,
         tags: Mapping[str, str] = ...,
         workflowId: str = ...,
-        workflowType: Literal["PRIVATE"] = ...
+        workflowType: WorkflowTypeType = ...
     ) -> StartRunResponseTypeDef:
         """
         Starts a run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.start_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#start_run)
         """
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/literals.py` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,17 @@
     "CHR_START_END_REF_ALT_ZERO_BASE",
     "CHR_START_END_ZERO_BASE",
     "GENERIC",
 ]
 EncryptionTypeType = Literal["KMS"]
 FileTypeType = Literal["BAM", "CRAM", "FASTQ"]
 FormatToHeaderKeyType = Literal["ALT", "CHR", "END", "POS", "REF", "START"]
-JobStatusType = Literal["CANCELLED", "COMPLETED", "FAILED", "IN_PROGRESS", "SUBMITTED"]
+JobStatusType = Literal[
+    "CANCELLED", "COMPLETED", "COMPLETED_WITH_FAILURES", "FAILED", "IN_PROGRESS", "SUBMITTED"
+]
 ListAnnotationImportJobsPaginatorName = Literal["list_annotation_import_jobs"]
 ListAnnotationStoresPaginatorName = Literal["list_annotation_stores"]
 ListReadSetActivationJobsPaginatorName = Literal["list_read_set_activation_jobs"]
 ListReadSetExportJobsPaginatorName = Literal["list_read_set_export_jobs"]
 ListReadSetImportJobsPaginatorName = Literal["list_read_set_import_jobs"]
 ListReadSetsPaginatorName = Literal["list_read_sets"]
 ListReferenceImportJobsPaginatorName = Literal["list_reference_import_jobs"]
@@ -184,16 +186,16 @@
 ]
 VariantImportJobCreatedWaiterName = Literal["variant_import_job_created"]
 VariantStoreCreatedWaiterName = Literal["variant_store_created"]
 VariantStoreDeletedWaiterName = Literal["variant_store_deleted"]
 WorkflowActiveWaiterName = Literal["workflow_active"]
 WorkflowEngineType = Literal["NEXTFLOW", "WDL"]
 WorkflowExportType = Literal["DEFINITION"]
-WorkflowStatusType = Literal["ACTIVE", "CREATING", "DELETED", "FAILED", "UPDATING"]
-WorkflowTypeType = Literal["PRIVATE"]
+WorkflowStatusType = Literal["ACTIVE", "CREATING", "DELETED", "FAILED", "INACTIVE", "UPDATING"]
+WorkflowTypeType = Literal["PRIVATE", "SERVICE"]
 OmicsServiceName = Literal["omics"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -230,27 +232,30 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -279,14 +284,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -331,14 +337,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -353,30 +360,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -425,14 +435,15 @@
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -460,14 +471,16 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -501,14 +514,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/literals.pyi` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,17 @@
     "CHR_START_END_REF_ALT_ZERO_BASE",
     "CHR_START_END_ZERO_BASE",
     "GENERIC",
 ]
 EncryptionTypeType = Literal["KMS"]
 FileTypeType = Literal["BAM", "CRAM", "FASTQ"]
 FormatToHeaderKeyType = Literal["ALT", "CHR", "END", "POS", "REF", "START"]
-JobStatusType = Literal["CANCELLED", "COMPLETED", "FAILED", "IN_PROGRESS", "SUBMITTED"]
+JobStatusType = Literal[
+    "CANCELLED", "COMPLETED", "COMPLETED_WITH_FAILURES", "FAILED", "IN_PROGRESS", "SUBMITTED"
+]
 ListAnnotationImportJobsPaginatorName = Literal["list_annotation_import_jobs"]
 ListAnnotationStoresPaginatorName = Literal["list_annotation_stores"]
 ListReadSetActivationJobsPaginatorName = Literal["list_read_set_activation_jobs"]
 ListReadSetExportJobsPaginatorName = Literal["list_read_set_export_jobs"]
 ListReadSetImportJobsPaginatorName = Literal["list_read_set_import_jobs"]
 ListReadSetsPaginatorName = Literal["list_read_sets"]
 ListReferenceImportJobsPaginatorName = Literal["list_reference_import_jobs"]
@@ -182,16 +184,16 @@
 ]
 VariantImportJobCreatedWaiterName = Literal["variant_import_job_created"]
 VariantStoreCreatedWaiterName = Literal["variant_store_created"]
 VariantStoreDeletedWaiterName = Literal["variant_store_deleted"]
 WorkflowActiveWaiterName = Literal["workflow_active"]
 WorkflowEngineType = Literal["NEXTFLOW", "WDL"]
 WorkflowExportType = Literal["DEFINITION"]
-WorkflowStatusType = Literal["ACTIVE", "CREATING", "DELETED", "FAILED", "UPDATING"]
-WorkflowTypeType = Literal["PRIVATE"]
+WorkflowStatusType = Literal["ACTIVE", "CREATING", "DELETED", "FAILED", "INACTIVE", "UPDATING"]
+WorkflowTypeType = Literal["PRIVATE", "SERVICE"]
 OmicsServiceName = Literal["omics"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -228,27 +230,30 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -277,14 +282,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -329,14 +335,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -351,30 +358,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -423,14 +433,15 @@
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -458,14 +469,16 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -499,14 +512,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/paginator.py` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,20 +45,19 @@
     list_runs_paginator: ListRunsPaginator = client.get_paginator("list_runs")
     list_sequence_stores_paginator: ListSequenceStoresPaginator = client.get_paginator("list_sequence_stores")
     list_variant_import_jobs_paginator: ListVariantImportJobsPaginator = client.get_paginator("list_variant_import_jobs")
     list_variant_stores_paginator: ListVariantStoresPaginator = client.get_paginator("list_variant_stores")
     list_workflows_paginator: ListWorkflowsPaginator = client.get_paginator("list_workflows")
     ```
 """
-import sys
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
-from .literals import TaskStatusType
+from .literals import TaskStatusType, WorkflowTypeType
 from .type_defs import (
     ActivateReadSetFilterTypeDef,
     ExportReadSetFilterTypeDef,
     ImportReadSetFilterTypeDef,
     ImportReferenceFilterTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
     ListAnnotationImportJobsResponseTypeDef,
@@ -83,20 +82,14 @@
     PaginatorConfigTypeDef,
     ReadSetFilterTypeDef,
     ReferenceFilterTypeDef,
     ReferenceStoreFilterTypeDef,
     SequenceStoreFilterTypeDef,
 )
 
-if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
-
 __all__ = (
     "ListAnnotationImportJobsPaginator",
     "ListAnnotationStoresPaginator",
     "ListReadSetActivationJobsPaginator",
     "ListReadSetExportJobsPaginator",
     "ListReadSetImportJobsPaginator",
     "ListReadSetsPaginator",
@@ -408,14 +401,14 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listworkflowspaginator)
     """
 
     def paginate(
         self,
         *,
         name: str = ...,
-        type: Literal["PRIVATE"] = ...,
+        type: WorkflowTypeType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListWorkflows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listworkflowspaginator)
         """
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/paginator.pyi` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,20 +45,19 @@
     list_runs_paginator: ListRunsPaginator = client.get_paginator("list_runs")
     list_sequence_stores_paginator: ListSequenceStoresPaginator = client.get_paginator("list_sequence_stores")
     list_variant_import_jobs_paginator: ListVariantImportJobsPaginator = client.get_paginator("list_variant_import_jobs")
     list_variant_stores_paginator: ListVariantStoresPaginator = client.get_paginator("list_variant_stores")
     list_workflows_paginator: ListWorkflowsPaginator = client.get_paginator("list_workflows")
     ```
 """
-import sys
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
-from .literals import TaskStatusType
+from .literals import TaskStatusType, WorkflowTypeType
 from .type_defs import (
     ActivateReadSetFilterTypeDef,
     ExportReadSetFilterTypeDef,
     ImportReadSetFilterTypeDef,
     ImportReferenceFilterTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
     ListAnnotationImportJobsResponseTypeDef,
@@ -83,19 +82,14 @@
     PaginatorConfigTypeDef,
     ReadSetFilterTypeDef,
     ReferenceFilterTypeDef,
     ReferenceStoreFilterTypeDef,
     SequenceStoreFilterTypeDef,
 )
 
-if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
 __all__ = (
     "ListAnnotationImportJobsPaginator",
     "ListAnnotationStoresPaginator",
     "ListReadSetActivationJobsPaginator",
     "ListReadSetExportJobsPaginator",
     "ListReadSetImportJobsPaginator",
     "ListReadSetsPaginator",
@@ -389,14 +383,14 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listworkflowspaginator)
     """
 
     def paginate(
         self,
         *,
         name: str = ...,
-        type: Literal["PRIVATE"] = ...,
+        type: WorkflowTypeType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListWorkflows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listworkflowspaginator)
         """
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/type_defs.py` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     RunStatusType,
     SchemaValueTypeType,
     StoreFormatType,
     StoreStatusType,
     TaskStatusType,
     WorkflowEngineType,
     WorkflowStatusType,
+    WorkflowTypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -851,21 +852,35 @@
 GetVariantImportRequestRequestTypeDef = TypedDict(
     "GetVariantImportRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
-VariantImportItemDetailTypeDef = TypedDict(
-    "VariantImportItemDetailTypeDef",
+_RequiredVariantImportItemDetailTypeDef = TypedDict(
+    "_RequiredVariantImportItemDetailTypeDef",
     {
         "jobStatus": JobStatusType,
         "source": str,
     },
 )
+_OptionalVariantImportItemDetailTypeDef = TypedDict(
+    "_OptionalVariantImportItemDetailTypeDef",
+    {
+        "statusMessage": str,
+    },
+    total=False,
+)
+
+
+class VariantImportItemDetailTypeDef(
+    _RequiredVariantImportItemDetailTypeDef, _OptionalVariantImportItemDetailTypeDef
+):
+    pass
+
 
 GetVariantStoreRequestRequestTypeDef = TypedDict(
     "GetVariantStoreRequestRequestTypeDef",
     {
         "name": str,
     },
 )
@@ -876,15 +891,15 @@
         "id": str,
     },
 )
 _OptionalGetWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalGetWorkflowRequestRequestTypeDef",
     {
         "export": Sequence[Literal["DEFINITION"]],
-        "type": Literal["PRIVATE"],
+        "type": WorkflowTypeType,
     },
     total=False,
 )
 
 
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
@@ -1222,29 +1237,29 @@
 
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "maxResults": int,
         "name": str,
         "startingToken": str,
-        "type": Literal["PRIVATE"],
+        "type": WorkflowTypeType,
     },
     total=False,
 )
 
 WorkflowListItemTypeDef = TypedDict(
     "WorkflowListItemTypeDef",
     {
         "arn": str,
         "creationTime": datetime,
         "digest": str,
         "id": str,
         "name": str,
         "status": WorkflowStatusType,
-        "type": Literal["PRIVATE"],
+        "type": WorkflowTypeType,
     },
     total=False,
 )
 
 ReadOptionsTypeDef = TypedDict(
     "ReadOptionsTypeDef",
     {
@@ -1308,15 +1323,15 @@
         "parameters": Mapping[str, Any],
         "priority": int,
         "runGroupId": str,
         "runId": str,
         "storageCapacity": int,
         "tags": Mapping[str, str],
         "workflowId": str,
-        "workflowType": Literal["PRIVATE"],
+        "workflowType": WorkflowTypeType,
     },
     total=False,
 )
 
 
 class StartRunRequestRequestTypeDef(
     _RequiredStartRunRequestRequestTypeDef, _OptionalStartRunRequestRequestTypeDef
@@ -1800,15 +1815,15 @@
         "startedBy": str,
         "status": RunStatusType,
         "statusMessage": str,
         "stopTime": datetime,
         "storageCapacity": int,
         "tags": Dict[str, str],
         "workflowId": str,
-        "workflowType": Literal["PRIVATE"],
+        "workflowType": WorkflowTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRunTaskResponseTypeDef = TypedDict(
     "GetRunTaskResponseTypeDef",
     {
@@ -2014,15 +2029,15 @@
         "main": str,
         "name": str,
         "parameterTemplate": Dict[str, WorkflowParameterTypeDef],
         "status": WorkflowStatusType,
         "statusMessage": str,
         "storageCapacity": int,
         "tags": Dict[str, str],
-        "type": Literal["PRIVATE"],
+        "type": WorkflowTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReadSetExportJobResponseTypeDef = TypedDict(
     "GetReadSetExportJobResponseTypeDef",
     {
@@ -2435,15 +2450,15 @@
         "id": str,
     },
 )
 _OptionalGetWorkflowRequestWorkflowActiveWaitTypeDef = TypedDict(
     "_OptionalGetWorkflowRequestWorkflowActiveWaitTypeDef",
     {
         "export": Sequence[Literal["DEFINITION"]],
-        "type": Literal["PRIVATE"],
+        "type": WorkflowTypeType,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 
 class GetWorkflowRequestWorkflowActiveWaitTypeDef(
@@ -2793,15 +2808,15 @@
     total=False,
 )
 
 ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
     "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     {
         "name": str,
-        "type": Literal["PRIVATE"],
+        "type": WorkflowTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef = TypedDict(
     "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/type_defs.pyi` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     RunStatusType,
     SchemaValueTypeType,
     StoreFormatType,
     StoreStatusType,
     TaskStatusType,
     WorkflowEngineType,
     WorkflowStatusType,
+    WorkflowTypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -824,21 +825,33 @@
 GetVariantImportRequestRequestTypeDef = TypedDict(
     "GetVariantImportRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
-VariantImportItemDetailTypeDef = TypedDict(
-    "VariantImportItemDetailTypeDef",
+_RequiredVariantImportItemDetailTypeDef = TypedDict(
+    "_RequiredVariantImportItemDetailTypeDef",
     {
         "jobStatus": JobStatusType,
         "source": str,
     },
 )
+_OptionalVariantImportItemDetailTypeDef = TypedDict(
+    "_OptionalVariantImportItemDetailTypeDef",
+    {
+        "statusMessage": str,
+    },
+    total=False,
+)
+
+class VariantImportItemDetailTypeDef(
+    _RequiredVariantImportItemDetailTypeDef, _OptionalVariantImportItemDetailTypeDef
+):
+    pass
 
 GetVariantStoreRequestRequestTypeDef = TypedDict(
     "GetVariantStoreRequestRequestTypeDef",
     {
         "name": str,
     },
 )
@@ -849,15 +862,15 @@
         "id": str,
     },
 )
 _OptionalGetWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalGetWorkflowRequestRequestTypeDef",
     {
         "export": Sequence[Literal["DEFINITION"]],
-        "type": Literal["PRIVATE"],
+        "type": WorkflowTypeType,
     },
     total=False,
 )
 
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
@@ -1181,29 +1194,29 @@
 
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "maxResults": int,
         "name": str,
         "startingToken": str,
-        "type": Literal["PRIVATE"],
+        "type": WorkflowTypeType,
     },
     total=False,
 )
 
 WorkflowListItemTypeDef = TypedDict(
     "WorkflowListItemTypeDef",
     {
         "arn": str,
         "creationTime": datetime,
         "digest": str,
         "id": str,
         "name": str,
         "status": WorkflowStatusType,
-        "type": Literal["PRIVATE"],
+        "type": WorkflowTypeType,
     },
     total=False,
 )
 
 ReadOptionsTypeDef = TypedDict(
     "ReadOptionsTypeDef",
     {
@@ -1265,15 +1278,15 @@
         "parameters": Mapping[str, Any],
         "priority": int,
         "runGroupId": str,
         "runId": str,
         "storageCapacity": int,
         "tags": Mapping[str, str],
         "workflowId": str,
-        "workflowType": Literal["PRIVATE"],
+        "workflowType": WorkflowTypeType,
     },
     total=False,
 )
 
 class StartRunRequestRequestTypeDef(
     _RequiredStartRunRequestRequestTypeDef, _OptionalStartRunRequestRequestTypeDef
 ):
@@ -1735,15 +1748,15 @@
         "startedBy": str,
         "status": RunStatusType,
         "statusMessage": str,
         "stopTime": datetime,
         "storageCapacity": int,
         "tags": Dict[str, str],
         "workflowId": str,
-        "workflowType": Literal["PRIVATE"],
+        "workflowType": WorkflowTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRunTaskResponseTypeDef = TypedDict(
     "GetRunTaskResponseTypeDef",
     {
@@ -1947,15 +1960,15 @@
         "main": str,
         "name": str,
         "parameterTemplate": Dict[str, WorkflowParameterTypeDef],
         "status": WorkflowStatusType,
         "statusMessage": str,
         "storageCapacity": int,
         "tags": Dict[str, str],
-        "type": Literal["PRIVATE"],
+        "type": WorkflowTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReadSetExportJobResponseTypeDef = TypedDict(
     "GetReadSetExportJobResponseTypeDef",
     {
@@ -2336,15 +2349,15 @@
         "id": str,
     },
 )
 _OptionalGetWorkflowRequestWorkflowActiveWaitTypeDef = TypedDict(
     "_OptionalGetWorkflowRequestWorkflowActiveWaitTypeDef",
     {
         "export": Sequence[Literal["DEFINITION"]],
-        "type": Literal["PRIVATE"],
+        "type": WorkflowTypeType,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 class GetWorkflowRequestWorkflowActiveWaitTypeDef(
     _RequiredGetWorkflowRequestWorkflowActiveWaitTypeDef,
@@ -2672,15 +2685,15 @@
     total=False,
 )
 
 ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
     "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     {
         "name": str,
-        "type": Literal["PRIVATE"],
+        "type": WorkflowTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef = TypedDict(
     "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/waiter.py` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     ```
 """
 import sys
 from typing import Sequence
 
 from botocore.waiter import Waiter
 
+from .literals import WorkflowTypeType
 from .type_defs import WaiterConfigTypeDef
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -288,14 +289,14 @@
     """
 
     def wait(
         self,
         *,
         id: str,
         export: Sequence[Literal["DEFINITION"]] = ...,
-        type: Literal["PRIVATE"] = ...,
+        type: WorkflowTypeType = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.WorkflowActive.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/waiters/#workflowactivewaiter)
         """
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics/waiter.pyi` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics/waiter.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     ```
 """
 import sys
 from typing import Sequence
 
 from botocore.waiter import Waiter
 
+from .literals import WorkflowTypeType
 from .type_defs import WaiterConfigTypeDef
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -272,14 +273,14 @@
     """
 
     def wait(
         self,
         *,
         id: str,
         export: Sequence[Literal["DEFINITION"]] = ...,
-        type: Literal["PRIVATE"] = ...,
+        type: WorkflowTypeType = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Waiter.WorkflowActive.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/waiters/#workflowactivewaiter)
         """
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics.egg-info/PKG-INFO` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.26.19
-Summary: Type annotations for boto3.Omics 1.26.19 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.81
+Summary: Type annotations for boto3.Omics 1.26.81 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-omics?color=blue)](https://pypistats.org/packages/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-omics-1.26.19/mypy_boto3_omics.egg-info/SOURCES.txt` & `mypy-boto3-omics-1.26.81/mypy_boto3_omics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.26.19/setup.py` & `mypy-boto3-omics-1.26.81/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-omics",
-    version="1.26.19",
+    version="1.26.81",
     packages=["mypy_boto3_omics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Omics 1.26.19 service generated with mypy-boto3-builder 7.11.11"
+        "Type annotations for boto3.Omics 1.26.81 service generated with mypy-boto3-builder 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 omics type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_omics": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_omics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

