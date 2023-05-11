# Comparing `tmp/testservices-0.1.0.tar.gz` & `tmp/testservices-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testservices-0.1.0.tar", last modified: Tue May  9 07:12:50 2023, max compression
+gzip compressed data, was "testservices-0.2.0.tar", last modified: Thu May 11 06:56:11 2023, max compression
```

## Comparing `testservices-0.1.0.tar` & `testservices-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      242 2023-05-09 07:12:38.000000 testservices-0.1.0/.carthorse.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1839 2023-05-09 07:12:38.000000 testservices-0.1.0/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-09 07:12:38.000000 testservices-0.1.0/.coveragerc
--rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-05-09 07:12:38.000000 testservices-0.1.0/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      152 2023-05-09 07:12:38.000000 testservices-0.1.0/.readthedocs.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2023-05-09 07:12:38.000000 testservices-0.1.0/CHANGELOG.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-05-09 07:12:38.000000 testservices-0.1.0/LICENSE.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-09 07:12:50.887726 testservices-0.1.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-05-09 07:12:38.000000 testservices-0.1.0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2575 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/api.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/changes.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1739 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/development.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/license.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2023-05-09 07:12:38.000000 testservices-0.1.0/docs/use.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2023-05-09 07:12:38.000000 testservices-0.1.0/pytest.ini
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-09 07:12:50.887726 testservices-0.1.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1442 2023-05-09 07:12:38.000000 testservices-0.1.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:38.000000 testservices-0.1.0/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1699 2023-05-09 07:12:38.000000 testservices-0.1.0/tests/test_containers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3254 2023-05-09 07:12:38.000000 testservices-0.1.0/tests/test_databases.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2023-05-09 07:12:38.000000 testservices-0.1.0/tests/test_imports.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-05-09 07:12:38.000000 testservices-0.1.0/tests/test_service.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/testservices/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/collection.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/provider.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/service.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/testservices/services/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/services/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.883726 testservices-0.1.0/testservices/services/config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/testservices/services/config/clickhouse/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/services/config/clickhouse/docker_related_config.xml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2738 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/services/containers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4661 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/services/databases.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-09 07:12:38.000000 testservices-0.1.0/testservices/supplier.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 07:12:50.887726 testservices-0.1.0/testservices.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-09 07:12:50.000000 testservices-0.1.0/testservices.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-09 07:12:50.000000 testservices-0.1.0/testservices.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 07:12:50.000000 testservices-0.1.0/testservices.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 07:12:46.000000 testservices-0.1.0/testservices.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-05-09 07:12:50.000000 testservices-0.1.0/testservices.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-09 07:12:50.000000 testservices-0.1.0/testservices.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.077491 testservices-0.2.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      242 2023-05-11 06:55:59.000000 testservices-0.2.0/.carthorse.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1839 2023-05-11 06:55:59.000000 testservices-0.2.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-11 06:55:59.000000 testservices-0.2.0/.coveragerc
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-05-11 06:55:59.000000 testservices-0.2.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      152 2023-05-11 06:55:59.000000 testservices-0.2.0/.readthedocs.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      349 2023-05-11 06:55:59.000000 testservices-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-05-11 06:55:59.000000 testservices-0.2.0/LICENSE.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-11 06:56:11.073491 testservices-0.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-05-11 06:55:59.000000 testservices-0.2.0/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2575 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/api.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/changes.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1739 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/development.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/license.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/use.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2023-05-11 06:55:59.000000 testservices-0.2.0/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-11 06:56:11.077491 testservices-0.2.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1471 2023-05-11 06:55:59.000000 testservices-0.2.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1699 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/test_containers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7290 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/test_databases.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/test_imports.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2621 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/test_provider.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/test_service.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1182 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/test_tcp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/testservices/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/collection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/provider.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      849 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/service.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/testservices/services/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/services/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.069491 testservices-0.2.0/testservices/services/config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/testservices/services/config/clickhouse/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/services/config/clickhouse/docker_related_config.xml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2738 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/services/containers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6021 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/services/databases.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/supplier.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/tcp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/testservices.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-11 06:56:11.000000 testservices-0.2.0/testservices.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      938 2023-05-11 06:56:11.000000 testservices-0.2.0/testservices.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-11 06:56:11.000000 testservices-0.2.0/testservices.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-11 06:56:10.000000 testservices-0.2.0/testservices.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      155 2023-05-11 06:56:11.000000 testservices-0.2.0/testservices.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-11 06:56:11.000000 testservices-0.2.0/testservices.egg-info/top_level.txt
```

### Comparing `testservices-0.1.0/.circleci/config.yml` & `testservices-0.2.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `testservices-0.1.0/LICENSE.rst` & `testservices-0.2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `testservices-0.1.0/PKG-INFO` & `testservices-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testservices
-Version: 0.1.0
+Version: 0.2.0
 Summary: Orchestrating services for testing and development.
 Home-page: https://github.com/simplistix/testservices
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `testservices-0.1.0/docs/Makefile` & `testservices-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `testservices-0.1.0/docs/conf.py` & `testservices-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `testservices-0.1.0/docs/development.rst` & `testservices-0.2.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `testservices-0.1.0/setup.py` & `testservices-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # See license.txt for license details.
-# Copyright (c) 2023, Chris Withers
+# Copyright (c) 2023 onwards Chris Withers
 
 import os
 
 from setuptools import setup, find_packages
 
 base_dir = os.path.dirname(__file__)
 
 setup(
     name='testservices',
-    version='0.1.0',
+    version='0.2.0',
     author='Chris Withers',
     author_email='chris@withers.org',
     license='MIT',
     description=(
         "Orchestrating services for testing and development."
     ),
     long_description=open('README.rst').read(),
@@ -24,32 +24,34 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.11',
     ],
     packages=find_packages(exclude=["tests"]),
     zip_safe=False,
     include_package_data=True,
     python_requires=">=3.8",
+    install_requires=[
+        # If good non-container uses cases appear, this should move
+        # to an extra:
+        'docker',
+        # https://github.com/docker/docker-py/issues/3113
+        'urllib3<2',
+    ],
     extras_require=dict(
         test=[
             'PyMySQL',
             'clickhouse-driver',
-            'docker',
             'pytest',
             'pytest-cov',
             'sybil',
             'testfixtures',
             'psycopg',
             'sqlalchemy',
-            # https://github.com/docker/docker-py/issues/3113
-            'urllib3<2',
         ],
         build=[
             'furo',
             'sphinx',
             'setuptools-git',
             'twine',
-            # https://github.com/docker/docker-py/issues/3113
-            'urllib3<2',
             'wheel'
         ]
     ),
 )
```

### Comparing `testservices-0.1.0/tests/test_containers.py` & `testservices-0.2.0/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `testservices-0.1.0/tests/test_service.py` & `testservices-0.2.0/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `testservices-0.1.0/testservices/service.py` & `testservices-0.2.0/testservices/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-from typing import List, Sequence, Type, Optional, Any
-
-from .provider import Provider
-from .supplier import Supplier
+from typing import Type, Optional, Any
 
 
 class Service:
-    name: str
-    providers: List[Provider]
-    suppliers: List[Supplier]
 
     def available(self) -> bool:
         """
         Returns ``True`` if this service can be used.
         """
         return True
```

### Comparing `testservices-0.1.0/testservices/services/containers.py` & `testservices-0.2.0/testservices/services/containers.py`

 * *Files identical despite different names*

### Comparing `testservices-0.1.0/testservices/services/databases.py` & `testservices-0.2.0/testservices/services/databases.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+import os
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, Sequence, Dict
+from urllib.parse import urlparse, urlunparse
 from uuid import uuid1
 
 from .containers import Container
+from ..service import Service
+from ..tcp import wait_for_server
 
 
 @dataclass
 class Database:
     host: str
     port: int
     username: str
@@ -20,15 +24,18 @@
     def url(self) -> str:
         auth = self.username
         if self.password:
             auth += f':{self.password}'
         protocol = self.dialect
         if self.driver:
             protocol = f'{protocol}+{self.driver}'
-        return f'{protocol}://{auth}@{self.host}:{self.port}/{self.database}'
+        url_ = f'{protocol}://{auth}@{self.host}:{self.port}'
+        if self.database:
+            url_ = f'{url_}/{self.database}'
+        return url_
 
 
 class DatabaseContainer(Container):
 
     _port = None
 
     username: str
@@ -47,15 +54,15 @@
             env: Optional[Dict[str, str]] = None,
     ):
         self.dialect = dialect
         self.driver = driver
         self.password = str(uuid1())
         super().__init__(image, version, {port: 0}, ready_phrases, volumes, env, always_pull)
 
-    def get(self):
+    def get(self) -> Database:
         return Database(
             host='127.0.0.1',
             port=tuple(self.port_map.values())[0],
             username=self.username,
             password=self.password,
             database=self.database,
             dialect=self.dialect,
@@ -161,7 +168,47 @@
             dialect='clickhouse',
             ready_phrases=ready_phrases,
             driver=driver,
             always_pull=always_pull,
         )
         env['CLICKHOUSE_PASSWORD'] = self.password
         self.env = env
+
+
+class DatabaseFromEnvironment(Service):
+
+    def __init__(
+            self,
+            url='DB_URL',
+            *,
+            check: bool = True,
+            timeout: float = 5,
+            poll_frequency: float = 0.05,
+    ):
+        self.url = url
+        self.check = check
+        self.timeout = timeout
+        self.poll_frequency = poll_frequency
+
+    def available(self) -> bool:
+        return self.url in os.environ
+
+    def get(self) -> Database:
+        parts = urlparse(os.environ[self.url])
+        scheme_parts = parts.scheme.split('+', 1)
+        if len(scheme_parts) == 1:
+            dialect = scheme_parts[0]
+            driver = None
+        else:
+            dialect, driver = scheme_parts
+        database = Database(
+            host=parts.hostname,
+            port=int(parts.port),
+            username=parts.username,
+            password=parts.password,
+            database=parts.path[1:] if parts.path else None,
+            dialect=dialect,
+            driver=driver,
+        )
+        if self.check:
+            wait_for_server(database.port, database.host, self.timeout, self.poll_frequency)
+        return database
```

### Comparing `testservices-0.1.0/testservices.egg-info/PKG-INFO` & `testservices-0.2.0/testservices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testservices
-Version: 0.1.0
+Version: 0.2.0
 Summary: Orchestrating services for testing and development.
 Home-page: https://github.com/simplistix/testservices
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `testservices-0.1.0/testservices.egg-info/SOURCES.txt` & `testservices-0.2.0/testservices.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,23 @@
 docs/index.rst
 docs/license.rst
 docs/use.rst
 tests/__init__.py
 tests/test_containers.py
 tests/test_databases.py
 tests/test_imports.py
+tests/test_provider.py
 tests/test_service.py
+tests/test_tcp.py
 testservices/__init__.py
 testservices/collection.py
 testservices/provider.py
 testservices/service.py
 testservices/supplier.py
+testservices/tcp.py
 testservices.egg-info/PKG-INFO
 testservices.egg-info/SOURCES.txt
 testservices.egg-info/dependency_links.txt
 testservices.egg-info/not-zip-safe
 testservices.egg-info/requires.txt
 testservices.egg-info/top_level.txt
 testservices/services/__init__.py
```

