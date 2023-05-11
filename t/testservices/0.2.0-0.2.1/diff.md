# Comparing `tmp/testservices-0.2.0.tar.gz` & `tmp/testservices-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testservices-0.2.0.tar", last modified: Thu May 11 06:56:11 2023, max compression
+gzip compressed data, was "testservices-0.2.1.tar", last modified: Thu May 11 07:21:54 2023, max compression
```

## Comparing `testservices-0.2.0.tar` & `testservices-0.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.077491 testservices-0.2.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      242 2023-05-11 06:55:59.000000 testservices-0.2.0/.carthorse.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1839 2023-05-11 06:55:59.000000 testservices-0.2.0/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-11 06:55:59.000000 testservices-0.2.0/.coveragerc
--rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-05-11 06:55:59.000000 testservices-0.2.0/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      152 2023-05-11 06:55:59.000000 testservices-0.2.0/.readthedocs.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      349 2023-05-11 06:55:59.000000 testservices-0.2.0/CHANGELOG.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-05-11 06:55:59.000000 testservices-0.2.0/LICENSE.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-11 06:56:11.073491 testservices-0.2.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-05-11 06:55:59.000000 testservices-0.2.0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2575 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/api.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/changes.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1739 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/development.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/license.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2023-05-11 06:55:59.000000 testservices-0.2.0/docs/use.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2023-05-11 06:55:59.000000 testservices-0.2.0/pytest.ini
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-11 06:56:11.077491 testservices-0.2.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1471 2023-05-11 06:55:59.000000 testservices-0.2.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1699 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/test_containers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7290 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/test_databases.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/test_imports.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2621 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/test_provider.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/test_service.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1182 2023-05-11 06:55:59.000000 testservices-0.2.0/tests/test_tcp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/testservices/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/collection.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/provider.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      849 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/service.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/testservices/services/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/services/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.069491 testservices-0.2.0/testservices/services/config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/testservices/services/config/clickhouse/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/services/config/clickhouse/docker_related_config.xml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2738 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/services/containers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6021 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/services/databases.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/supplier.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2023-05-11 06:55:59.000000 testservices-0.2.0/testservices/tcp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 06:56:11.073491 testservices-0.2.0/testservices.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-11 06:56:11.000000 testservices-0.2.0/testservices.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      938 2023-05-11 06:56:11.000000 testservices-0.2.0/testservices.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-11 06:56:11.000000 testservices-0.2.0/testservices.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-11 06:56:10.000000 testservices-0.2.0/testservices.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      155 2023-05-11 06:56:11.000000 testservices-0.2.0/testservices.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-11 06:56:11.000000 testservices-0.2.0/testservices.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 07:21:54.397375 testservices-0.2.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      242 2023-05-11 07:21:40.000000 testservices-0.2.1/.carthorse.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 07:21:54.393375 testservices-0.2.1/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1839 2023-05-11 07:21:40.000000 testservices-0.2.1/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-11 07:21:40.000000 testservices-0.2.1/.coveragerc
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-05-11 07:21:40.000000 testservices-0.2.1/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      152 2023-05-11 07:21:40.000000 testservices-0.2.1/.readthedocs.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2023-05-11 07:21:40.000000 testservices-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-05-11 07:21:40.000000 testservices-0.2.1/LICENSE.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-11 07:21:54.397375 testservices-0.2.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-05-11 07:21:40.000000 testservices-0.2.1/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 07:21:54.393375 testservices-0.2.1/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2575 2023-05-11 07:21:40.000000 testservices-0.2.1/docs/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-05-11 07:21:40.000000 testservices-0.2.1/docs/api.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-11 07:21:40.000000 testservices-0.2.1/docs/changes.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2023-05-11 07:21:40.000000 testservices-0.2.1/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1739 2023-05-11 07:21:40.000000 testservices-0.2.1/docs/development.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-05-11 07:21:40.000000 testservices-0.2.1/docs/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-05-11 07:21:40.000000 testservices-0.2.1/docs/license.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2023-05-11 07:21:40.000000 testservices-0.2.1/docs/use.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2023-05-11 07:21:40.000000 testservices-0.2.1/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-11 07:21:54.397375 testservices-0.2.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1471 2023-05-11 07:21:40.000000 testservices-0.2.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 07:21:54.393375 testservices-0.2.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-11 07:21:40.000000 testservices-0.2.1/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1699 2023-05-11 07:21:40.000000 testservices-0.2.1/tests/test_containers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7285 2023-05-11 07:21:40.000000 testservices-0.2.1/tests/test_databases.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2023-05-11 07:21:40.000000 testservices-0.2.1/tests/test_imports.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2621 2023-05-11 07:21:40.000000 testservices-0.2.1/tests/test_provider.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-05-11 07:21:40.000000 testservices-0.2.1/tests/test_service.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1182 2023-05-11 07:21:40.000000 testservices-0.2.1/tests/test_tcp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 07:21:54.397375 testservices-0.2.1/testservices/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-11 07:21:40.000000 testservices-0.2.1/testservices/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-05-11 07:21:40.000000 testservices-0.2.1/testservices/collection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2023-05-11 07:21:40.000000 testservices-0.2.1/testservices/provider.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      849 2023-05-11 07:21:40.000000 testservices-0.2.1/testservices/service.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 07:21:54.397375 testservices-0.2.1/testservices/services/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-11 07:21:40.000000 testservices-0.2.1/testservices/services/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 07:21:54.393375 testservices-0.2.1/testservices/services/config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 07:21:54.397375 testservices-0.2.1/testservices/services/config/clickhouse/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2023-05-11 07:21:40.000000 testservices-0.2.1/testservices/services/config/clickhouse/docker_related_config.xml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2738 2023-05-11 07:21:40.000000 testservices-0.2.1/testservices/services/containers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6139 2023-05-11 07:21:40.000000 testservices-0.2.1/testservices/services/databases.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-11 07:21:40.000000 testservices-0.2.1/testservices/supplier.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2023-05-11 07:21:40.000000 testservices-0.2.1/testservices/tcp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-11 07:21:54.397375 testservices-0.2.1/testservices.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-05-11 07:21:54.000000 testservices-0.2.1/testservices.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      938 2023-05-11 07:21:54.000000 testservices-0.2.1/testservices.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-11 07:21:54.000000 testservices-0.2.1/testservices.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-11 07:21:53.000000 testservices-0.2.1/testservices.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      155 2023-05-11 07:21:54.000000 testservices-0.2.1/testservices.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-11 07:21:54.000000 testservices-0.2.1/testservices.egg-info/top_level.txt
```

### Comparing `testservices-0.2.0/.circleci/config.yml` & `testservices-0.2.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/LICENSE.rst` & `testservices-0.2.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/PKG-INFO` & `testservices-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testservices
-Version: 0.2.0
+Version: 0.2.1
 Summary: Orchestrating services for testing and development.
 Home-page: https://github.com/simplistix/testservices
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `testservices-0.2.0/docs/Makefile` & `testservices-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/docs/conf.py` & `testservices-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/docs/development.rst` & `testservices-0.2.1/docs/development.rst`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/setup.py` & `testservices-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import setup, find_packages
 
 base_dir = os.path.dirname(__file__)
 
 setup(
     name='testservices',
-    version='0.2.0',
+    version='0.2.1',
     author='Chris Withers',
     author_email='chris@withers.org',
     license='MIT',
     description=(
         "Orchestrating services for testing and development."
     ),
     long_description=open('README.rst').read(),
```

### Comparing `testservices-0.2.0/tests/test_containers.py` & `testservices-0.2.1/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/tests/test_databases.py` & `testservices-0.2.1/tests/test_databases.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,21 +147,21 @@
     def test_not_available(self):
         service = DatabaseFromEnvironment(check=False)
         with replace_in_environ('DB_URL', not_there):
             assert not service.available()
 
     def test_url_minimal(self):
         service = DatabaseFromEnvironment(check=False)
-        url = 'postgresql://user@host:1234'
+        url = 'postgresql://user@host'
         with replace_in_environ('DB_URL', url):
             assert service.available()
             with service as db:
                 compare(db, expected=Database(
                     host='host',
-                    port=1234,
+                    port=None,
                     username='user',
                     password=None,
                     database=None,
                     dialect='postgresql',
                     driver=None,
                 ))
                 compare(db.url, expected=url)
```

### Comparing `testservices-0.2.0/tests/test_provider.py` & `testservices-0.2.1/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/tests/test_service.py` & `testservices-0.2.1/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/tests/test_tcp.py` & `testservices-0.2.1/tests/test_tcp.py`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/testservices/provider.py` & `testservices-0.2.1/testservices/provider.py`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/testservices/service.py` & `testservices-0.2.1/testservices/service.py`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/testservices/services/containers.py` & `testservices-0.2.1/testservices/services/containers.py`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/testservices/services/databases.py` & `testservices-0.2.1/testservices/services/databases.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,30 +9,33 @@
 from ..service import Service
 from ..tcp import wait_for_server
 
 
 @dataclass
 class Database:
     host: str
-    port: int
+    port: Optional[int]
     username: str
     password: Optional[str]
     database: Optional[str]
     dialect: Optional[str] = None
     driver: Optional[str] = None
 
     @property
     def url(self) -> str:
         auth = self.username
         if self.password:
             auth += f':{self.password}'
         protocol = self.dialect
         if self.driver:
             protocol = f'{protocol}+{self.driver}'
-        url_ = f'{protocol}://{auth}@{self.host}:{self.port}'
+        netloc = f'{auth}@{self.host}'
+        if self.port:
+            netloc = f'{netloc}:{self.port}'
+        url_ = f'{protocol}://{netloc}'
         if self.database:
             url_ = f'{url_}/{self.database}'
         return url_
 
 
 class DatabaseContainer(Container):
 
@@ -198,15 +201,15 @@
         if len(scheme_parts) == 1:
             dialect = scheme_parts[0]
             driver = None
         else:
             dialect, driver = scheme_parts
         database = Database(
             host=parts.hostname,
-            port=int(parts.port),
+            port=int(parts.port) if parts.port else None,
             username=parts.username,
             password=parts.password,
             database=parts.path[1:] if parts.path else None,
             dialect=dialect,
             driver=driver,
         )
         if self.check:
```

### Comparing `testservices-0.2.0/testservices/tcp.py` & `testservices-0.2.1/testservices/tcp.py`

 * *Files identical despite different names*

### Comparing `testservices-0.2.0/testservices.egg-info/PKG-INFO` & `testservices-0.2.1/testservices.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testservices
-Version: 0.2.0
+Version: 0.2.1
 Summary: Orchestrating services for testing and development.
 Home-page: https://github.com/simplistix/testservices
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `testservices-0.2.0/testservices.egg-info/SOURCES.txt` & `testservices-0.2.1/testservices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

