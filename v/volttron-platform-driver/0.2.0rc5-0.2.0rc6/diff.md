# Comparing `tmp/volttron_platform_driver-0.2.0rc5.tar.gz` & `tmp/volttron_platform_driver-0.2.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_platform_driver-0.2.0rc5.tar", max compression
+gzip compressed data, was "volttron_platform_driver-0.2.0rc6.tar", max compression
```

## Comparing `volttron_platform_driver-0.2.0rc5.tar` & `volttron_platform_driver-0.2.0rc6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10255 2023-05-11 17:28:07.675208 volttron_platform_driver-0.2.0rc5/LICENSE
--rw-r--r--   0        0        0     2777 2023-05-11 17:28:07.675208 volttron_platform_driver-0.2.0rc5/README.md
--rw-r--r--   0        0        0     2111 2023-05-11 17:28:52.210895 volttron_platform_driver-0.2.0rc5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 17:28:07.675208 volttron_platform_driver-0.2.0rc5/src/platform_driver/__init__.py
--rw-r--r--   0        0        0    34550 2023-05-11 17:28:07.675208 volttron_platform_driver-0.2.0rc5/src/platform_driver/agent.py
--rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 volttron_platform_driver-0.2.0rc5/PKG-INFO
+-rw-r--r--   0        0        0    10255 2023-05-11 17:29:22.428852 volttron_platform_driver-0.2.0rc6/LICENSE
+-rw-r--r--   0        0        0     2777 2023-05-11 17:29:22.428852 volttron_platform_driver-0.2.0rc6/README.md
+-rw-r--r--   0        0        0     2111 2023-05-11 17:30:25.745203 volttron_platform_driver-0.2.0rc6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 17:29:22.428852 volttron_platform_driver-0.2.0rc6/src/platform_driver/__init__.py
+-rw-r--r--   0        0        0    34550 2023-05-11 17:29:22.428852 volttron_platform_driver-0.2.0rc6/src/platform_driver/agent.py
+-rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 volttron_platform_driver-0.2.0rc6/PKG-INFO
```

### Comparing `volttron_platform_driver-0.2.0rc5/LICENSE` & `volttron_platform_driver-0.2.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_platform_driver-0.2.0rc5/README.md` & `volttron_platform_driver-0.2.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `volttron_platform_driver-0.2.0rc5/pyproject.toml` & `volttron_platform_driver-0.2.0rc6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 warn_return_any = true
 warn_unused_configs = true
 show_error_codes = true
 exclude = ['docs/']
 
 [tool.poetry]
 name = "volttron-platform-driver"
-version = "0.2.0rc5"
+version = "0.2.0rc6"
 description = "The Platform Driver agent is a special purpose agent that manages communication between the Volttron platform and devices. The Platform driver features a number of endpoints for collecting data and sending control signals using the message bus and automatically publishes data to the bus on a specified interval."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/platform-driver-agent"
 homepage = "https://github.com/eclipse-volttron/platform-driver-agent"
 keywords = []
```

### Comparing `volttron_platform_driver-0.2.0rc5/src/platform_driver/agent.py` & `volttron_platform_driver-0.2.0rc6/src/platform_driver/agent.py`

 * *Files identical despite different names*

### Comparing `volttron_platform_driver-0.2.0rc5/PKG-INFO` & `volttron_platform_driver-0.2.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-platform-driver
-Version: 0.2.0rc5
+Version: 0.2.0rc6
 Summary: The Platform Driver agent is a special purpose agent that manages communication between the Volttron platform and devices. The Platform driver features a number of endpoints for collecting data and sending control signals using the message bus and automatically publishes data to the bus on a specified interval.
 Home-page: https://github.com/eclipse-volttron/platform-driver-agent
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

