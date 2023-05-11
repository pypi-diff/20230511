# Comparing `tmp/volttron_testing-0.4.1rc0.tar.gz` & `tmp/volttron_testing-0.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_testing-0.4.1rc0.tar", max compression
+gzip compressed data, was "volttron_testing-0.4.1rc1.tar", max compression
```

## Comparing `volttron_testing-0.4.1rc0.tar` & `volttron_testing-0.4.1rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11928 2023-05-11 16:13:06.652872 volttron_testing-0.4.1rc0/LICENSE
--rw-r--r--   0        0        0     3607 2023-05-11 16:14:25.541334 volttron_testing-0.4.1rc0/README.md
--rw-r--r--   0        0        0     1780 2023-05-11 16:24:48.572476 volttron_testing-0.4.1rc0/pyproject.toml
--rw-r--r--   0        0        0     1166 2023-05-11 16:13:06.652872 volttron_testing-0.4.1rc0/src/volttrontesting/__init__.py
--rw-r--r--   0        0        0     5184 2023-05-11 16:13:06.652872 volttron_testing-0.4.1rc0/src/volttrontesting/agent_additions.py
--rw-r--r--   0        0        0     9155 2023-05-11 16:13:06.652872 volttron_testing-0.4.1rc0/src/volttrontesting/certs_utils.py
--rw-r--r--   0        0        0      979 2023-05-11 16:13:06.652872 volttron_testing-0.4.1rc0/src/volttrontesting/client_mock.py
--rw-r--r--   0        0        0        0 2023-05-11 16:13:06.652872 volttron_testing-0.4.1rc0/src/volttrontesting/fixtures/__init__.py
--rw-r--r--   0        0        0     4696 2023-05-11 16:13:06.652872 volttron_testing-0.4.1rc0/src/volttrontesting/fixtures/cert_fixtures.py
--rw-r--r--   0        0        0     4686 2023-05-11 16:14:25.541334 volttron_testing-0.4.1rc0/src/volttrontesting/fixtures/docker_wrapper.py
--rw-r--r--   0        0        0     8103 2023-05-11 16:13:06.652872 volttron_testing-0.4.1rc0/src/volttrontesting/fixtures/rmq_test_setup.py
--rw-r--r--   0        0        0    29475 2023-05-11 16:13:06.652872 volttron_testing-0.4.1rc0/src/volttrontesting/fixtures/volttron_platform_fixtures.py
--rw-r--r--   0        0        0     3422 2023-05-11 16:13:06.652872 volttron_testing-0.4.1rc0/src/volttrontesting/memory_pubsub.py
--rw-r--r--   0        0        0    62220 2023-05-11 16:14:25.541334 volttron_testing-0.4.1rc0/src/volttrontesting/platformwrapper.py
--rw-r--r--   0        0        0    12618 2023-05-11 16:13:06.652872 volttron_testing-0.4.1rc0/src/volttrontesting/server_mock.py
--rw-r--r--   0        0        0     7115 2023-05-11 16:13:06.652872 volttron_testing-0.4.1rc0/src/volttrontesting/utils.py
--rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 volttron_testing-0.4.1rc0/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/LICENSE
+-rw-r--r--   0        0        0     3607 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/README.md
+-rw-r--r--   0        0        0     1780 2023-05-11 16:26:06.424484 volttron_testing-0.4.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     1166 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/__init__.py
+-rw-r--r--   0        0        0     5184 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/agent_additions.py
+-rw-r--r--   0        0        0     9155 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/certs_utils.py
+-rw-r--r--   0        0        0      979 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/client_mock.py
+-rw-r--r--   0        0        0        0 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/fixtures/__init__.py
+-rw-r--r--   0        0        0     4696 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/fixtures/cert_fixtures.py
+-rw-r--r--   0        0        0     4686 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/fixtures/docker_wrapper.py
+-rw-r--r--   0        0        0     8103 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/fixtures/rmq_test_setup.py
+-rw-r--r--   0        0        0    29475 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/fixtures/volttron_platform_fixtures.py
+-rw-r--r--   0        0        0     3422 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/memory_pubsub.py
+-rw-r--r--   0        0        0    62220 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/platformwrapper.py
+-rw-r--r--   0        0        0    12618 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/server_mock.py
+-rw-r--r--   0        0        0     7115 2023-05-11 16:25:14.082310 volttron_testing-0.4.1rc1/src/volttrontesting/utils.py
+-rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 volttron_testing-0.4.1rc1/PKG-INFO
```

### Comparing `volttron_testing-0.4.1rc0/LICENSE` & `volttron_testing-0.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/README.md` & `volttron_testing-0.4.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/pyproject.toml` & `volttron_testing-0.4.1rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volttron-testing"
-version = "0.4.1rc0"
+version = "0.4.1rc1"
 description = "The volttron-testing library contains classes and utilities for interacting with a VOLTTRON instance."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-testing"
 homepage = "https://github.com/eclipse-volttron/volttron-testing"
 keywords = []
```

### Comparing `volttron_testing-0.4.1rc0/src/volttrontesting/__init__.py` & `volttron_testing-0.4.1rc1/src/volttrontesting/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/src/volttrontesting/agent_additions.py` & `volttron_testing-0.4.1rc1/src/volttrontesting/agent_additions.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/src/volttrontesting/certs_utils.py` & `volttron_testing-0.4.1rc1/src/volttrontesting/certs_utils.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/src/volttrontesting/client_mock.py` & `volttron_testing-0.4.1rc1/src/volttrontesting/client_mock.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/src/volttrontesting/fixtures/cert_fixtures.py` & `volttron_testing-0.4.1rc1/src/volttrontesting/fixtures/cert_fixtures.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/src/volttrontesting/fixtures/docker_wrapper.py` & `volttron_testing-0.4.1rc1/src/volttrontesting/fixtures/docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/src/volttrontesting/fixtures/rmq_test_setup.py` & `volttron_testing-0.4.1rc1/src/volttrontesting/fixtures/rmq_test_setup.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/src/volttrontesting/fixtures/volttron_platform_fixtures.py` & `volttron_testing-0.4.1rc1/src/volttrontesting/fixtures/volttron_platform_fixtures.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/src/volttrontesting/memory_pubsub.py` & `volttron_testing-0.4.1rc1/src/volttrontesting/memory_pubsub.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/src/volttrontesting/platformwrapper.py` & `volttron_testing-0.4.1rc1/src/volttrontesting/platformwrapper.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/src/volttrontesting/server_mock.py` & `volttron_testing-0.4.1rc1/src/volttrontesting/server_mock.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/src/volttrontesting/utils.py` & `volttron_testing-0.4.1rc1/src/volttrontesting/utils.py`

 * *Files identical despite different names*

### Comparing `volttron_testing-0.4.1rc0/PKG-INFO` & `volttron_testing-0.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-testing
-Version: 0.4.1rc0
+Version: 0.4.1rc1
 Summary: The volttron-testing library contains classes and utilities for interacting with a VOLTTRON instance.
 Home-page: https://github.com/eclipse-volttron/volttron-testing
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

