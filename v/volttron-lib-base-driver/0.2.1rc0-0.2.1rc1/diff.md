# Comparing `tmp/volttron_lib_base_driver-0.2.1rc0.tar.gz` & `tmp/volttron_lib_base_driver-0.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_base_driver-0.2.1rc0.tar", max compression
+gzip compressed data, was "volttron_lib_base_driver-0.2.1rc1.tar", max compression
```

## Comparing `volttron_lib_base_driver-0.2.1rc0.tar` & `volttron_lib_base_driver-0.2.1rc1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11927 2023-05-11 16:41:41.278327 volttron_lib_base_driver-0.2.1rc0/LICENSE
--rw-r--r--   0        0        0     3020 2023-05-11 16:41:41.282327 volttron_lib_base_driver-0.2.1rc0/README.md
--rw-r--r--   0        0        0     1993 2023-05-11 16:42:44.799490 volttron_lib_base_driver-0.2.1rc0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 16:41:41.282327 volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/__init__.py
--rw-r--r--   0        0        0    16976 2023-05-11 16:41:41.282327 volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/driver.py
--rw-r--r--   0        0        0     1019 2023-05-11 16:41:41.282327 volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/driver_exceptions.py
--rw-r--r--   0        0        0     2169 2023-05-11 16:41:41.282327 volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/driver_locks.py
--rw-r--r--   0        0        0    22949 2023-05-11 16:41:41.282327 volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/interfaces.py
--rw-r--r--   0        0        0     4006 1970-01-01 00:00:00.000000 volttron_lib_base_driver-0.2.1rc0/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-05-11 16:43:05.055160 volttron_lib_base_driver-0.2.1rc1/LICENSE
+-rw-r--r--   0        0        0     3020 2023-05-11 16:43:05.055160 volttron_lib_base_driver-0.2.1rc1/README.md
+-rw-r--r--   0        0        0     1993 2023-05-11 16:43:56.208073 volttron_lib_base_driver-0.2.1rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 16:43:05.055160 volttron_lib_base_driver-0.2.1rc1/src/volttron/driver/base/__init__.py
+-rw-r--r--   0        0        0    16976 2023-05-11 16:43:05.055160 volttron_lib_base_driver-0.2.1rc1/src/volttron/driver/base/driver.py
+-rw-r--r--   0        0        0     1019 2023-05-11 16:43:05.055160 volttron_lib_base_driver-0.2.1rc1/src/volttron/driver/base/driver_exceptions.py
+-rw-r--r--   0        0        0     2169 2023-05-11 16:43:05.055160 volttron_lib_base_driver-0.2.1rc1/src/volttron/driver/base/driver_locks.py
+-rw-r--r--   0        0        0    22949 2023-05-11 16:43:05.055160 volttron_lib_base_driver-0.2.1rc1/src/volttron/driver/base/interfaces.py
+-rw-r--r--   0        0        0     4006 1970-01-01 00:00:00.000000 volttron_lib_base_driver-0.2.1rc1/PKG-INFO
```

### Comparing `volttron_lib_base_driver-0.2.1rc0/LICENSE` & `volttron_lib_base_driver-0.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_driver-0.2.1rc0/README.md` & `volttron_lib_base_driver-0.2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_driver-0.2.1rc0/pyproject.toml` & `volttron_lib_base_driver-0.2.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ignore_missing_imports = true
 
 [tool.mypy-volttron]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-lib-base-driver"
-version = "0.2.1rc0"
+version = "0.2.1rc1"
 description = "Volttron Driver libraries used to support development within the Volttron Driver Framework."
 authors = ["Mark Bonicillo <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-base-driver"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-base-driver"
 keywords = []
```

### Comparing `volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/driver.py` & `volttron_lib_base_driver-0.2.1rc1/src/volttron/driver/base/driver.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/driver_exceptions.py` & `volttron_lib_base_driver-0.2.1rc1/src/volttron/driver/base/driver_exceptions.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/driver_locks.py` & `volttron_lib_base_driver-0.2.1rc1/src/volttron/driver/base/driver_locks.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_driver-0.2.1rc0/src/volttron/driver/base/interfaces.py` & `volttron_lib_base_driver-0.2.1rc1/src/volttron/driver/base/interfaces.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_driver-0.2.1rc0/PKG-INFO` & `volttron_lib_base_driver-0.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-base-driver
-Version: 0.2.1rc0
+Version: 0.2.1rc1
 Summary: Volttron Driver libraries used to support development within the Volttron Driver Framework.
 Home-page: https://github.com/eclipse-volttron/volttron-lib-base-driver
 License: Apache-2.0
 Author: Mark Bonicillo
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volttron-lib-base-driver Version: 0.2.1rc0 Summary:
+Metadata-Version: 2.1 Name: volttron-lib-base-driver Version: 0.2.1rc1 Summary:
 Volttron Driver libraries used to support development within the Volttron
 Driver Framework. Home-page: https://github.com/eclipse-volttron/volttron-lib-
 base-driver License: Apache-2.0 Author: Mark Bonicillo Author-email:
 volttron@pnnl.gov Requires-Python: >=3.10,<4.0 Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
```

