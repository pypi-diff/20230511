# Comparing `tmp/mypy-boto3-health-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-health-1.26.133.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-health-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:30 2022, max compression
+gzip compressed data, was "mypy-boto3-health-1.26.133.tar", last modified: Thu May 11 19:32:34 2023, max compression
```

## Comparing `mypy-boto3-health-1.26.0.post1.tar` & `mypy-boto3-health-1.26.133.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:30.592826 mypy-boto3-health-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16259 2022-11-01 21:43:30.588826 mypy-boto3-health-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14822 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:30.588826 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15699 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    15672 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8690 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8688 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9810 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9800 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    21615 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    21590 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:30.588826 mypy-boto3-health-1.26.0.post1/mypy_boto3_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16259 2022-11-01 21:43:30.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-11-01 21:43:30.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:30.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:30.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:30.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-01 21:43:30.000000 mypy-boto3-health-1.26.0.post1/mypy_boto3_health.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:30.592826 mypy-boto3-health-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-11-01 21:35:32.000000 mypy-boto3-health-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:34.953501 mypy-boto3-health-1.26.133/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-11 19:32:34.953501 mypy-boto3-health-1.26.133/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:34.953501 mypy-boto3-health-1.26.133/mypy_boto3_health/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21653 2023-05-11 19:32:12.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21628 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/mypy_boto3_health/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:34.953501 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-11 19:32:34.000000 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-11 19:32:34.000000 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:32:34.000000 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:32:34.000000 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 19:32:34.000000 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 19:32:34.000000 mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:32:34.953501 mypy-boto3-health-1.26.133/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-11 19:32:11.000000 mypy-boto3-health-1.26.133/setup.py
```

### Comparing `mypy-boto3-health-1.26.0.post1/LICENSE` & `mypy-boto3-health-1.26.133/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-health-1.26.0.post1/PKG-INFO` & `mypy-boto3-health-1.26.133/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-health
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Health 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.133
+Summary: Type annotations for boto3.Health 1.26.133 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
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
 
 <a id="mypy-boto3-health"></a>
 
 # mypy-boto3-health
 
 [![PyPI - mypy-boto3-health](https://img.shields.io/pypi/v/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-health?color=blue)](https://pypistats.org/packages/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.26.133](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-health docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,38 +357,38 @@
 `mypy_boto3_health.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_health.type_defs import (
     AffectedEntityTypeDef,
     DateTimeRangeTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
     DescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeAffectedAccountsForOrganizationResponseTypeDef,
     EventAccountFilterTypeDef,
     OrganizationAffectedEntitiesErrorItemTypeDef,
     DescribeEntityAggregatesRequestRequestTypeDef,
     EntityAggregateTypeDef,
     EventAggregateTypeDef,
     OrganizationEventDetailsErrorItemTypeDef,
     DescribeEventDetailsRequestRequestTypeDef,
     EventDetailsErrorItemTypeDef,
     EventTypeFilterTypeDef,
     EventTypeTypeDef,
     OrganizationEventTypeDef,
     EventTypeDef,
+    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventDescriptionTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    DescribeAffectedEntitiesResponseTypeDef,
     EntityFilterTypeDef,
     EventFilterTypeDef,
     OrganizationEventFilterTypeDef,
-    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-    DescribeAffectedAccountsForOrganizationResponseTypeDef,
-    DescribeAffectedEntitiesResponseTypeDef,
-    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     DescribeEventDetailsForOrganizationRequestRequestTypeDef,
     DescribeAffectedEntitiesForOrganizationResponseTypeDef,
     DescribeEntityAggregatesResponseTypeDef,
     DescribeEventAggregatesResponseTypeDef,
     DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef,
@@ -417,42 +418,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-health-1.26.0.post1/README.md` & `mypy-boto3-health-1.26.133/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-health"></a>
 
 # mypy-boto3-health
 
 [![PyPI - mypy-boto3-health](https://img.shields.io/pypi/v/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-health?color=blue)](https://pypistats.org/packages/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.26.133](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-health docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,38 +325,38 @@
 `mypy_boto3_health.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_health.type_defs import (
     AffectedEntityTypeDef,
     DateTimeRangeTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
     DescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeAffectedAccountsForOrganizationResponseTypeDef,
     EventAccountFilterTypeDef,
     OrganizationAffectedEntitiesErrorItemTypeDef,
     DescribeEntityAggregatesRequestRequestTypeDef,
     EntityAggregateTypeDef,
     EventAggregateTypeDef,
     OrganizationEventDetailsErrorItemTypeDef,
     DescribeEventDetailsRequestRequestTypeDef,
     EventDetailsErrorItemTypeDef,
     EventTypeFilterTypeDef,
     EventTypeTypeDef,
     OrganizationEventTypeDef,
     EventTypeDef,
+    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventDescriptionTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    DescribeAffectedEntitiesResponseTypeDef,
     EntityFilterTypeDef,
     EventFilterTypeDef,
     OrganizationEventFilterTypeDef,
-    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-    DescribeAffectedAccountsForOrganizationResponseTypeDef,
-    DescribeAffectedEntitiesResponseTypeDef,
-    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     DescribeEventDetailsForOrganizationRequestRequestTypeDef,
     DescribeAffectedEntitiesForOrganizationResponseTypeDef,
     DescribeEntityAggregatesResponseTypeDef,
     DescribeEventAggregatesResponseTypeDef,
     DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef,
@@ -386,42 +386,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health/__init__.py` & `mypy-boto3-health-1.26.133/mypy_boto3_health/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health/__init__.pyi` & `mypy-boto3-health-1.26.133/mypy_boto3_health/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health/__main__.py` & `mypy-boto3-health-1.26.133/mypy_boto3_health/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Health 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Health 1.26.133\nVersion:         1.26.133\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.133")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health/client.py` & `mypy-boto3-health-1.26.133/mypy_boto3_health/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health/client.pyi` & `mypy-boto3-health-1.26.133/mypy_boto3_health/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health/literals.py` & `mypy-boto3-health-1.26.133/mypy_boto3_health/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -94,27 +95,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
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
@@ -143,14 +148,15 @@
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
@@ -195,51 +201,57 @@
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
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
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
@@ -271,28 +283,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
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
@@ -301,14 +318,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -319,55 +337,63 @@
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
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
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
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health/literals.pyi` & `mypy-boto3-health-1.26.133/mypy_boto3_health/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -92,27 +93,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
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
@@ -141,14 +146,15 @@
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
@@ -193,51 +199,57 @@
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
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
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
@@ -269,28 +281,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
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
@@ -299,14 +316,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -317,55 +335,63 @@
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
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
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
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health/paginator.py` & `mypy-boto3-health-1.26.133/mypy_boto3_health/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 class DescribeAffectedAccountsForOrganizationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedaccountsfororganizationpaginator)
     """
 
     def paginate(
-        self, *, eventArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, eventArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAffectedAccountsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedaccountsfororganizationpaginator)
         """
 
 
@@ -101,15 +101,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EntityFilterTypeDef,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAffectedEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedentitiespaginator)
         """
 
 
@@ -120,15 +120,15 @@
     """
 
     def paginate(
         self,
         *,
         organizationEntityFilters: Sequence[EventAccountFilterTypeDef],
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAffectedEntitiesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntitiesForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedentitiesfororganizationpaginator)
         """
 
 
@@ -139,15 +139,15 @@
     """
 
     def paginate(
         self,
         *,
         aggregateField: Literal["eventTypeCategory"],
         filter: EventFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventAggregates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventaggregatespaginator)
         """
 
 
@@ -158,15 +158,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventTypeFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventtypespaginator)
         """
 
 
@@ -177,15 +177,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventspaginator)
         """
 
 
@@ -196,13 +196,13 @@
     """
 
     def paginate(
         self,
         *,
         filter: OrganizationEventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventsForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventsfororganizationpaginator)
         """
```

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health/paginator.pyi` & `mypy-boto3-health-1.26.133/mypy_boto3_health/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 class DescribeAffectedAccountsForOrganizationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedaccountsfororganizationpaginator)
     """
 
     def paginate(
-        self, *, eventArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, eventArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAffectedAccountsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedaccountsfororganizationpaginator)
         """
 
 class DescribeAffectedEntitiesPaginator(Paginator):
@@ -96,15 +96,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EntityFilterTypeDef,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAffectedEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedentitiespaginator)
         """
 
 class DescribeAffectedEntitiesForOrganizationPaginator(Paginator):
@@ -114,15 +114,15 @@
     """
 
     def paginate(
         self,
         *,
         organizationEntityFilters: Sequence[EventAccountFilterTypeDef],
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAffectedEntitiesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntitiesForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedentitiesfororganizationpaginator)
         """
 
 class DescribeEventAggregatesPaginator(Paginator):
@@ -132,15 +132,15 @@
     """
 
     def paginate(
         self,
         *,
         aggregateField: Literal["eventTypeCategory"],
         filter: EventFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventAggregates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventaggregatespaginator)
         """
 
 class DescribeEventTypesPaginator(Paginator):
@@ -150,15 +150,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventTypeFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventtypespaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -168,15 +168,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventspaginator)
         """
 
 class DescribeEventsForOrganizationPaginator(Paginator):
@@ -186,13 +186,13 @@
     """
 
     def paginate(
         self,
         *,
         filter: OrganizationEventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventsForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventsfororganizationpaginator)
         """
```

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health/type_defs.py` & `mypy-boto3-health-1.26.133/mypy_boto3_health/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,42 +27,41 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AffectedEntityTypeDef",
     "DateTimeRangeTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     "DescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
     "EventAccountFilterTypeDef",
     "OrganizationAffectedEntitiesErrorItemTypeDef",
     "DescribeEntityAggregatesRequestRequestTypeDef",
     "EntityAggregateTypeDef",
     "EventAggregateTypeDef",
     "OrganizationEventDetailsErrorItemTypeDef",
     "DescribeEventDetailsRequestRequestTypeDef",
     "EventDetailsErrorItemTypeDef",
     "EventTypeFilterTypeDef",
     "EventTypeTypeDef",
     "OrganizationEventTypeDef",
     "EventTypeDef",
+    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventDescriptionTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "DescribeAffectedEntitiesResponseTypeDef",
     "EntityFilterTypeDef",
     "EventFilterTypeDef",
     "OrganizationEventFilterTypeDef",
-    "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
-    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
-    "DescribeAffectedEntitiesResponseTypeDef",
-    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef",
     "DescribeEventDetailsForOrganizationRequestRequestTypeDef",
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     "DescribeEntityAggregatesResponseTypeDef",
     "DescribeEventAggregatesResponseTypeDef",
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
@@ -104,24 +103,34 @@
     {
         "from": Union[datetime, str],
         "to": Union[datetime, str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "eventArn": str,
+    },
+)
+_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
+    _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
     {
         "eventArn": str,
     },
 )
 _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef = TypedDict(
@@ -129,30 +138,27 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeAffectedAccountsForOrganizationRequestRequestTypeDef(
     _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
     _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
+    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "affectedAccounts": List[str],
+        "eventScopeCode": eventScopeCodeType,
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEventAccountFilterTypeDef = TypedDict(
     "_RequiredEventAccountFilterTypeDef",
     {
         "eventArn": str,
@@ -162,21 +168,19 @@
     "_OptionalEventAccountFilterTypeDef",
     {
         "awsAccountId": str,
     },
     total=False,
 )
 
-
 class EventAccountFilterTypeDef(
     _RequiredEventAccountFilterTypeDef, _OptionalEventAccountFilterTypeDef
 ):
     pass
 
-
 OrganizationAffectedEntitiesErrorItemTypeDef = TypedDict(
     "OrganizationAffectedEntitiesErrorItemTypeDef",
     {
         "awsAccountId": str,
         "eventArn": str,
         "errorName": str,
         "errorMessage": str,
@@ -231,22 +235,20 @@
     "_OptionalDescribeEventDetailsRequestRequestTypeDef",
     {
         "locale": str,
     },
     total=False,
 )
 
-
 class DescribeEventDetailsRequestRequestTypeDef(
     _RequiredDescribeEventDetailsRequestRequestTypeDef,
     _OptionalDescribeEventDetailsRequestRequestTypeDef,
 ):
     pass
 
-
 EventDetailsErrorItemTypeDef = TypedDict(
     "EventDetailsErrorItemTypeDef",
     {
         "eventArn": str,
         "errorName": str,
         "errorMessage": str,
     },
@@ -304,22 +306,67 @@
         "lastUpdatedTime": datetime,
         "statusCode": eventStatusCodeType,
         "eventScopeCode": eventScopeCodeType,
     },
     total=False,
 )
 
+DescribeHealthServiceStatusForOrganizationResponseTypeDef = TypedDict(
+    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
+    {
+        "healthServiceAccessStatusForOrganization": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EventDescriptionTypeDef = TypedDict(
     "EventDescriptionTypeDef",
     {
         "latestDescription": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+DescribeAffectedEntitiesResponseTypeDef = TypedDict(
+    "DescribeAffectedEntitiesResponseTypeDef",
+    {
+        "entities": List[AffectedEntityTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEntityFilterTypeDef = TypedDict(
     "_RequiredEntityFilterTypeDef",
     {
         "eventArns": Sequence[str],
     },
 )
 _OptionalEntityFilterTypeDef = TypedDict(
@@ -330,19 +377,17 @@
         "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
         "tags": Sequence[Mapping[str, str]],
         "statusCodes": Sequence[entityStatusCodeType],
     },
     total=False,
 )
 
-
 class EntityFilterTypeDef(_RequiredEntityFilterTypeDef, _OptionalEntityFilterTypeDef):
     pass
 
-
 EventFilterTypeDef = TypedDict(
     "EventFilterTypeDef",
     {
         "eventArns": Sequence[str],
         "eventTypeCodes": Sequence[str],
         "services": Sequence[str],
         "regions": Sequence[str],
@@ -373,93 +418,35 @@
         "entityValues": Sequence[str],
         "eventTypeCategories": Sequence[eventTypeCategoryType],
         "eventStatusCodes": Sequence[eventStatusCodeType],
     },
     total=False,
 )
 
-_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
-    {
-        "eventArn": str,
-    },
-)
-_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
-    _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-    _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-):
-    pass
-
-
-DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
-    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
-    {
-        "affectedAccounts": List[str],
-        "eventScopeCode": eventScopeCodeType,
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAffectedEntitiesResponseTypeDef = TypedDict(
-    "DescribeAffectedEntitiesResponseTypeDef",
-    {
-        "entities": List[AffectedEntityTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeHealthServiceStatusForOrganizationResponseTypeDef = TypedDict(
-    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
-    {
-        "healthServiceAccessStatusForOrganization": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     {
         "organizationEntityFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = TypedDict(
     "_OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     {
         "locale": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     _OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef",
     {
         "organizationEntityFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef = TypedDict(
@@ -468,77 +455,73 @@
         "locale": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef(
     _RequiredDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     _OptionalDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEventDetailsForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventDetailsForOrganizationRequestRequestTypeDef",
     {
         "organizationEventDetailFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeEventDetailsForOrganizationRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeEventDetailsForOrganizationRequestRequestTypeDef",
     {
         "locale": str,
     },
     total=False,
 )
 
-
 class DescribeEventDetailsForOrganizationRequestRequestTypeDef(
     _RequiredDescribeEventDetailsForOrganizationRequestRequestTypeDef,
     _OptionalDescribeEventDetailsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeAffectedEntitiesForOrganizationResponseTypeDef = TypedDict(
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     {
         "entities": List[AffectedEntityTypeDef],
         "failedSet": List[OrganizationAffectedEntitiesErrorItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEntityAggregatesResponseTypeDef = TypedDict(
     "DescribeEntityAggregatesResponseTypeDef",
     {
         "entityAggregates": List[EntityAggregateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventAggregatesResponseTypeDef = TypedDict(
     "DescribeEventAggregatesResponseTypeDef",
     {
         "eventAggregates": List[EventAggregateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef = TypedDict(
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
     {
         "filter": EventTypeFilterTypeDef,
         "locale": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeEventTypesRequestRequestTypeDef = TypedDict(
     "DescribeEventTypesRequestRequestTypeDef",
     {
@@ -551,33 +534,33 @@
 )
 
 DescribeEventTypesResponseTypeDef = TypedDict(
     "DescribeEventTypesResponseTypeDef",
     {
         "eventTypes": List[EventTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventsForOrganizationResponseTypeDef = TypedDict(
     "DescribeEventsForOrganizationResponseTypeDef",
     {
         "events": List[OrganizationEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "events": List[EventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventDetailsTypeDef = TypedDict(
     "EventDetailsTypeDef",
     {
         "event": EventTypeDef,
@@ -604,27 +587,25 @@
         "filter": EntityFilterTypeDef,
     },
 )
 _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = TypedDict(
     "_OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     {
         "locale": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
     _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAffectedEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesRequestRequestTypeDef",
     {
         "filter": EntityFilterTypeDef,
     },
 )
 _OptionalDescribeAffectedEntitiesRequestRequestTypeDef = TypedDict(
@@ -633,45 +614,41 @@
         "locale": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeAffectedEntitiesRequestRequestTypeDef(
     _RequiredDescribeAffectedEntitiesRequestRequestTypeDef,
     _OptionalDescribeAffectedEntitiesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = TypedDict(
     "_RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     {
         "aggregateField": Literal["eventTypeCategory"],
     },
 )
 _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = TypedDict(
     "_OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef(
     _RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
     _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEventAggregatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventAggregatesRequestRequestTypeDef",
     {
         "aggregateField": Literal["eventTypeCategory"],
     },
 )
 _OptionalDescribeEventAggregatesRequestRequestTypeDef = TypedDict(
@@ -680,28 +657,26 @@
         "filter": EventFilterTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class DescribeEventAggregatesRequestRequestTypeDef(
     _RequiredDescribeEventAggregatesRequestRequestTypeDef,
     _OptionalDescribeEventAggregatesRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
         "locale": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeEventsRequestRequestTypeDef = TypedDict(
     "DescribeEventsRequestRequestTypeDef",
     {
@@ -714,15 +689,15 @@
 )
 
 DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef = TypedDict(
     "DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef",
     {
         "filter": OrganizationEventFilterTypeDef,
         "locale": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeEventsForOrganizationRequestRequestTypeDef = TypedDict(
     "DescribeEventsForOrganizationRequestRequestTypeDef",
     {
@@ -735,19 +710,19 @@
 )
 
 DescribeEventDetailsResponseTypeDef = TypedDict(
     "DescribeEventDetailsResponseTypeDef",
     {
         "successfulSet": List[EventDetailsTypeDef],
         "failedSet": List[EventDetailsErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventDetailsForOrganizationResponseTypeDef = TypedDict(
     "DescribeEventDetailsForOrganizationResponseTypeDef",
     {
         "successfulSet": List[OrganizationEventDetailsTypeDef],
         "failedSet": List[OrganizationEventDetailsErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health/type_defs.pyi` & `mypy-boto3-health-1.26.133/mypy_boto3_health/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,41 +27,42 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AffectedEntityTypeDef",
     "DateTimeRangeTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     "DescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
     "EventAccountFilterTypeDef",
     "OrganizationAffectedEntitiesErrorItemTypeDef",
     "DescribeEntityAggregatesRequestRequestTypeDef",
     "EntityAggregateTypeDef",
     "EventAggregateTypeDef",
     "OrganizationEventDetailsErrorItemTypeDef",
     "DescribeEventDetailsRequestRequestTypeDef",
     "EventDetailsErrorItemTypeDef",
     "EventTypeFilterTypeDef",
     "EventTypeTypeDef",
     "OrganizationEventTypeDef",
     "EventTypeDef",
+    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventDescriptionTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "DescribeAffectedEntitiesResponseTypeDef",
     "EntityFilterTypeDef",
     "EventFilterTypeDef",
     "OrganizationEventFilterTypeDef",
-    "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
-    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
-    "DescribeAffectedEntitiesResponseTypeDef",
-    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef",
     "DescribeEventDetailsForOrganizationRequestRequestTypeDef",
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     "DescribeEntityAggregatesResponseTypeDef",
     "DescribeEventAggregatesResponseTypeDef",
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
@@ -103,24 +104,36 @@
     {
         "from": Union[datetime, str],
         "to": Union[datetime, str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "eventArn": str,
+    },
+)
+_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
+    _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
     {
         "eventArn": str,
     },
 )
 _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef = TypedDict(
@@ -128,28 +141,29 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeAffectedAccountsForOrganizationRequestRequestTypeDef(
     _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
     _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
+    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "affectedAccounts": List[str],
+        "eventScopeCode": eventScopeCodeType,
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEventAccountFilterTypeDef = TypedDict(
     "_RequiredEventAccountFilterTypeDef",
     {
         "eventArn": str,
@@ -159,19 +173,21 @@
     "_OptionalEventAccountFilterTypeDef",
     {
         "awsAccountId": str,
     },
     total=False,
 )
 
+
 class EventAccountFilterTypeDef(
     _RequiredEventAccountFilterTypeDef, _OptionalEventAccountFilterTypeDef
 ):
     pass
 
+
 OrganizationAffectedEntitiesErrorItemTypeDef = TypedDict(
     "OrganizationAffectedEntitiesErrorItemTypeDef",
     {
         "awsAccountId": str,
         "eventArn": str,
         "errorName": str,
         "errorMessage": str,
@@ -226,20 +242,22 @@
     "_OptionalDescribeEventDetailsRequestRequestTypeDef",
     {
         "locale": str,
     },
     total=False,
 )
 
+
 class DescribeEventDetailsRequestRequestTypeDef(
     _RequiredDescribeEventDetailsRequestRequestTypeDef,
     _OptionalDescribeEventDetailsRequestRequestTypeDef,
 ):
     pass
 
+
 EventDetailsErrorItemTypeDef = TypedDict(
     "EventDetailsErrorItemTypeDef",
     {
         "eventArn": str,
         "errorName": str,
         "errorMessage": str,
     },
@@ -297,22 +315,67 @@
         "lastUpdatedTime": datetime,
         "statusCode": eventStatusCodeType,
         "eventScopeCode": eventScopeCodeType,
     },
     total=False,
 )
 
+DescribeHealthServiceStatusForOrganizationResponseTypeDef = TypedDict(
+    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
+    {
+        "healthServiceAccessStatusForOrganization": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EventDescriptionTypeDef = TypedDict(
     "EventDescriptionTypeDef",
     {
         "latestDescription": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+DescribeAffectedEntitiesResponseTypeDef = TypedDict(
+    "DescribeAffectedEntitiesResponseTypeDef",
+    {
+        "entities": List[AffectedEntityTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEntityFilterTypeDef = TypedDict(
     "_RequiredEntityFilterTypeDef",
     {
         "eventArns": Sequence[str],
     },
 )
 _OptionalEntityFilterTypeDef = TypedDict(
@@ -323,17 +386,19 @@
         "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
         "tags": Sequence[Mapping[str, str]],
         "statusCodes": Sequence[entityStatusCodeType],
     },
     total=False,
 )
 
+
 class EntityFilterTypeDef(_RequiredEntityFilterTypeDef, _OptionalEntityFilterTypeDef):
     pass
 
+
 EventFilterTypeDef = TypedDict(
     "EventFilterTypeDef",
     {
         "eventArns": Sequence[str],
         "eventTypeCodes": Sequence[str],
         "services": Sequence[str],
         "regions": Sequence[str],
@@ -364,89 +429,37 @@
         "entityValues": Sequence[str],
         "eventTypeCategories": Sequence[eventTypeCategoryType],
         "eventStatusCodes": Sequence[eventStatusCodeType],
     },
     total=False,
 )
 
-_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
-    {
-        "eventArn": str,
-    },
-)
-_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
-    _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-    _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-):
-    pass
-
-DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
-    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
-    {
-        "affectedAccounts": List[str],
-        "eventScopeCode": eventScopeCodeType,
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAffectedEntitiesResponseTypeDef = TypedDict(
-    "DescribeAffectedEntitiesResponseTypeDef",
-    {
-        "entities": List[AffectedEntityTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeHealthServiceStatusForOrganizationResponseTypeDef = TypedDict(
-    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
-    {
-        "healthServiceAccessStatusForOrganization": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     {
         "organizationEntityFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = TypedDict(
     "_OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     {
         "locale": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     _OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef",
     {
         "organizationEntityFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef = TypedDict(
@@ -455,73 +468,77 @@
         "locale": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef(
     _RequiredDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     _OptionalDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEventDetailsForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventDetailsForOrganizationRequestRequestTypeDef",
     {
         "organizationEventDetailFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeEventDetailsForOrganizationRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeEventDetailsForOrganizationRequestRequestTypeDef",
     {
         "locale": str,
     },
     total=False,
 )
 
+
 class DescribeEventDetailsForOrganizationRequestRequestTypeDef(
     _RequiredDescribeEventDetailsForOrganizationRequestRequestTypeDef,
     _OptionalDescribeEventDetailsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeAffectedEntitiesForOrganizationResponseTypeDef = TypedDict(
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     {
         "entities": List[AffectedEntityTypeDef],
         "failedSet": List[OrganizationAffectedEntitiesErrorItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEntityAggregatesResponseTypeDef = TypedDict(
     "DescribeEntityAggregatesResponseTypeDef",
     {
         "entityAggregates": List[EntityAggregateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventAggregatesResponseTypeDef = TypedDict(
     "DescribeEventAggregatesResponseTypeDef",
     {
         "eventAggregates": List[EventAggregateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef = TypedDict(
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
     {
         "filter": EventTypeFilterTypeDef,
         "locale": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeEventTypesRequestRequestTypeDef = TypedDict(
     "DescribeEventTypesRequestRequestTypeDef",
     {
@@ -534,33 +551,33 @@
 )
 
 DescribeEventTypesResponseTypeDef = TypedDict(
     "DescribeEventTypesResponseTypeDef",
     {
         "eventTypes": List[EventTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventsForOrganizationResponseTypeDef = TypedDict(
     "DescribeEventsForOrganizationResponseTypeDef",
     {
         "events": List[OrganizationEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "events": List[EventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventDetailsTypeDef = TypedDict(
     "EventDetailsTypeDef",
     {
         "event": EventTypeDef,
@@ -587,25 +604,27 @@
         "filter": EntityFilterTypeDef,
     },
 )
 _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = TypedDict(
     "_OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     {
         "locale": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
     _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAffectedEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesRequestRequestTypeDef",
     {
         "filter": EntityFilterTypeDef,
     },
 )
 _OptionalDescribeAffectedEntitiesRequestRequestTypeDef = TypedDict(
@@ -614,41 +633,45 @@
         "locale": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeAffectedEntitiesRequestRequestTypeDef(
     _RequiredDescribeAffectedEntitiesRequestRequestTypeDef,
     _OptionalDescribeAffectedEntitiesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = TypedDict(
     "_RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     {
         "aggregateField": Literal["eventTypeCategory"],
     },
 )
 _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = TypedDict(
     "_OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef(
     _RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
     _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEventAggregatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventAggregatesRequestRequestTypeDef",
     {
         "aggregateField": Literal["eventTypeCategory"],
     },
 )
 _OptionalDescribeEventAggregatesRequestRequestTypeDef = TypedDict(
@@ -657,26 +680,28 @@
         "filter": EventFilterTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class DescribeEventAggregatesRequestRequestTypeDef(
     _RequiredDescribeEventAggregatesRequestRequestTypeDef,
     _OptionalDescribeEventAggregatesRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
         "locale": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeEventsRequestRequestTypeDef = TypedDict(
     "DescribeEventsRequestRequestTypeDef",
     {
@@ -689,15 +714,15 @@
 )
 
 DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef = TypedDict(
     "DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef",
     {
         "filter": OrganizationEventFilterTypeDef,
         "locale": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeEventsForOrganizationRequestRequestTypeDef = TypedDict(
     "DescribeEventsForOrganizationRequestRequestTypeDef",
     {
@@ -710,19 +735,19 @@
 )
 
 DescribeEventDetailsResponseTypeDef = TypedDict(
     "DescribeEventDetailsResponseTypeDef",
     {
         "successfulSet": List[EventDetailsTypeDef],
         "failedSet": List[EventDetailsErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventDetailsForOrganizationResponseTypeDef = TypedDict(
     "DescribeEventDetailsForOrganizationResponseTypeDef",
     {
         "successfulSet": List[OrganizationEventDetailsTypeDef],
         "failedSet": List[OrganizationEventDetailsErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health.egg-info/PKG-INFO` & `mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-health
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Health 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.133
+Summary: Type annotations for boto3.Health 1.26.133 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
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
 
 <a id="mypy-boto3-health"></a>
 
 # mypy-boto3-health
 
 [![PyPI - mypy-boto3-health](https://img.shields.io/pypi/v/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-health?color=blue)](https://pypistats.org/packages/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.26.133](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-health docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,38 +357,38 @@
 `mypy_boto3_health.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_health.type_defs import (
     AffectedEntityTypeDef,
     DateTimeRangeTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
     DescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeAffectedAccountsForOrganizationResponseTypeDef,
     EventAccountFilterTypeDef,
     OrganizationAffectedEntitiesErrorItemTypeDef,
     DescribeEntityAggregatesRequestRequestTypeDef,
     EntityAggregateTypeDef,
     EventAggregateTypeDef,
     OrganizationEventDetailsErrorItemTypeDef,
     DescribeEventDetailsRequestRequestTypeDef,
     EventDetailsErrorItemTypeDef,
     EventTypeFilterTypeDef,
     EventTypeTypeDef,
     OrganizationEventTypeDef,
     EventTypeDef,
+    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventDescriptionTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    DescribeAffectedEntitiesResponseTypeDef,
     EntityFilterTypeDef,
     EventFilterTypeDef,
     OrganizationEventFilterTypeDef,
-    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-    DescribeAffectedAccountsForOrganizationResponseTypeDef,
-    DescribeAffectedEntitiesResponseTypeDef,
-    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     DescribeEventDetailsForOrganizationRequestRequestTypeDef,
     DescribeAffectedEntitiesForOrganizationResponseTypeDef,
     DescribeEntityAggregatesResponseTypeDef,
     DescribeEventAggregatesResponseTypeDef,
     DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef,
@@ -417,42 +418,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-health-1.26.0.post1/mypy_boto3_health.egg-info/SOURCES.txt` & `mypy-boto3-health-1.26.133/mypy_boto3_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.26.0.post1/setup.py` & `mypy-boto3-health-1.26.133/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 """
 Setup script for mypy-boto3-health.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-health",
-    version="1.26.0.post1",
+    version="1.26.133",
     packages=["mypy_boto3_health"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Health 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.Health 1.26.133 service generated with mypy-boto3-builder"
+        " 7.14.5"
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
     keywords="boto3 health type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_health": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_health": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

