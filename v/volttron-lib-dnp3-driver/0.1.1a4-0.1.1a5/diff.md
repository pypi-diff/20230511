# Comparing `tmp/volttron_lib_dnp3_driver-0.1.1a4.tar.gz` & `tmp/volttron_lib_dnp3_driver-0.1.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_dnp3_driver-0.1.1a4.tar", max compression
+gzip compressed data, was "volttron_lib_dnp3_driver-0.1.1a5.tar", max compression
```

## Comparing `volttron_lib_dnp3_driver-0.1.1a4.tar` & `volttron_lib_dnp3_driver-0.1.1a5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11928 2023-05-11 16:57:50.565540 volttron_lib_dnp3_driver-0.1.1a4/LICENSE
--rw-r--r--   0        0        0    21060 2023-05-11 16:57:50.565540 volttron_lib_dnp3_driver-0.1.1a4/README.md
--rw-r--r--   0        0        0     1579 2023-05-11 16:58:52.637481 volttron_lib_dnp3_driver-0.1.1a4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 16:57:50.565540 volttron_lib_dnp3_driver-0.1.1a4/src/volttron/driver/interfaces/dnp3/__init__.py
--rw-r--r--   0        0        0     9189 2023-05-11 16:57:50.565540 volttron_lib_dnp3_driver-0.1.1a4/src/volttron/driver/interfaces/dnp3/dnp3.py
--rw-r--r--   0        0        0    22079 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.1a4/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-11 17:10:28.016525 volttron_lib_dnp3_driver-0.1.1a5/LICENSE
+-rw-r--r--   0        0        0    21060 2023-05-11 17:10:28.016525 volttron_lib_dnp3_driver-0.1.1a5/README.md
+-rw-r--r--   0        0        0     1579 2023-05-11 17:11:13.220621 volttron_lib_dnp3_driver-0.1.1a5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 17:10:28.016525 volttron_lib_dnp3_driver-0.1.1a5/src/volttron/driver/interfaces/dnp3/__init__.py
+-rw-r--r--   0        0        0     9189 2023-05-11 17:10:28.016525 volttron_lib_dnp3_driver-0.1.1a5/src/volttron/driver/interfaces/dnp3/dnp3.py
+-rw-r--r--   0        0        0    22079 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.1a5/PKG-INFO
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a4/LICENSE` & `volttron_lib_dnp3_driver-0.1.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a4/README.md` & `volttron_lib_dnp3_driver-0.1.1a5/README.md`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a4/pyproject.toml` & `volttron_lib_dnp3_driver-0.1.1a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "volttron-lib-dnp3-driver"
-version = "0.1.1a4"
+version = "0.1.1a5"
 description = "A minimal implementation of a driver for the VOLTTRON platform."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-dnp3-driver"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-dnp3-driver"
 keywords = []
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a4/src/volttron/driver/interfaces/dnp3/dnp3.py` & `volttron_lib_dnp3_driver-0.1.1a5/src/volttron/driver/interfaces/dnp3/dnp3.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a4/PKG-INFO` & `volttron_lib_dnp3_driver-0.1.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-dnp3-driver
-Version: 0.1.1a4
+Version: 0.1.1a5
 Summary: A minimal implementation of a driver for the VOLTTRON platform.
 Home-page: https://github.com/eclipse-volttron/volttron-lib-dnp3-driver
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volttron-lib-dnp3-driver Version: 0.1.1a4 Summary:
+Metadata-Version: 2.1 Name: volttron-lib-dnp3-driver Version: 0.1.1a5 Summary:
 A minimal implementation of a driver for the VOLTTRON platform. Home-page:
 https://github.com/eclipse-volttron/volttron-lib-dnp3-driver License: Apache-
 2.0 Author: VOLTTRON Team Author-email: volttron@pnnl.gov Requires-Python:
 >=3.10,<4.0 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
```

