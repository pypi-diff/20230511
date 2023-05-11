# Comparing `tmp/exoscale-0.7.1.tar.gz` & `tmp/exoscale-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exoscale-0.7.1.tar", last modified: Mon Oct 18 07:56:03 2021, max compression
+gzip compressed data, last modified: Thu May 11 14:44:45 2023, max compression
```

## Comparing `exoscale-0.7.1.tar` & `exoscale-0.8.0.tar`

### file list

```diff
@@ -1,48 +1,15 @@
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2021-10-18 07:56:03.130705 exoscale-0.7.1/
--rw-r--r--   0 marc       (501) staff       (20)       14 2020-09-29 11:13:10.000000 exoscale-0.7.1/MANIFEST.in
--rw-r--r--   0 marc       (501) staff       (20)     1930 2021-10-18 07:56:03.130292 exoscale-0.7.1/PKG-INFO
--rw-r--r--   0 marc       (501) staff       (20)      995 2020-09-29 11:13:10.000000 exoscale-0.7.1/README.md
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2021-10-18 07:56:03.110395 exoscale-0.7.1/exoscale/
--rw-r--r--   0 marc       (501) staff       (20)     8381 2021-03-15 10:14:35.000000 exoscale-0.7.1/exoscale/__init__.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2021-10-18 07:56:03.120193 exoscale-0.7.1/exoscale/api/
--rw-r--r--   0 marc       (501) staff       (20)     4356 2021-04-21 09:14:57.000000 exoscale-0.7.1/exoscale/api/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)   111074 2021-10-18 07:49:58.000000 exoscale-0.7.1/exoscale/api/compute.py
--rw-r--r--   0 marc       (501) staff       (20)     8356 2021-04-21 09:14:57.000000 exoscale-0.7.1/exoscale/api/dns.py
--rw-r--r--   0 marc       (501) staff       (20)     4528 2021-04-21 09:14:57.000000 exoscale-0.7.1/exoscale/api/iam.py
--rw-r--r--   0 marc       (501) staff       (20)     6915 2021-09-13 07:11:53.000000 exoscale-0.7.1/exoscale/api/polling.py
--rw-r--r--   0 marc       (501) staff       (20)    24523 2020-09-29 11:13:10.000000 exoscale-0.7.1/exoscale/api/runstatus.py
--rw-r--r--   0 marc       (501) staff       (20)    23431 2021-04-21 09:14:57.000000 exoscale-0.7.1/exoscale/api/storage.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2021-10-18 07:56:03.111965 exoscale-0.7.1/exoscale.egg-info/
--rw-r--r--   0 marc       (501) staff       (20)     1930 2021-10-18 07:56:03.000000 exoscale-0.7.1/exoscale.egg-info/PKG-INFO
--rw-r--r--   0 marc       (501) staff       (20)     1125 2021-10-18 07:56:03.000000 exoscale-0.7.1/exoscale.egg-info/SOURCES.txt
--rw-r--r--   0 marc       (501) staff       (20)        1 2021-10-18 07:56:03.000000 exoscale-0.7.1/exoscale.egg-info/dependency_links.txt
--rw-r--r--   0 marc       (501) staff       (20)       99 2021-10-18 07:56:03.000000 exoscale-0.7.1/exoscale.egg-info/requires.txt
--rw-r--r--   0 marc       (501) staff       (20)        9 2021-10-18 07:56:03.000000 exoscale-0.7.1/exoscale.egg-info/top_level.txt
--rw-r--r--   0 marc       (501) staff       (20)      159 2021-04-21 09:14:57.000000 exoscale-0.7.1/requirements.dev.txt
--rw-r--r--   0 marc       (501) staff       (20)       99 2021-03-15 14:52:43.000000 exoscale-0.7.1/requirements.txt
--rw-r--r--   0 marc       (501) staff       (20)       38 2021-10-18 07:56:03.130849 exoscale-0.7.1/setup.cfg
--rw-r--r--   0 marc       (501) staff       (20)     1398 2021-10-18 07:50:16.000000 exoscale-0.7.1/setup.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2021-10-18 07:56:03.129595 exoscale-0.7.1/tests/
--rw-r--r--   0 marc       (501) staff       (20)        0 2021-05-10 12:31:07.000000 exoscale-0.7.1/tests/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)    16171 2021-09-13 09:27:02.000000 exoscale-0.7.1/tests/conftest.py
--rw-r--r--   0 marc       (501) staff       (20)    42480 2021-05-10 16:05:40.000000 exoscale-0.7.1/tests/test_compute.py
--rw-r--r--   0 marc       (501) staff       (20)     1018 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_compute_anti_affinity_group.py
--rw-r--r--   0 marc       (501) staff       (20)    10220 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_compute_elastic_ip.py
--rw-r--r--   0 marc       (501) staff       (20)    22686 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_compute_instance.py
--rw-r--r--   0 marc       (501) staff       (20)    11174 2021-05-10 16:05:40.000000 exoscale-0.7.1/tests/test_compute_instance_pool.py
--rw-r--r--   0 marc       (501) staff       (20)     3163 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_compute_instance_volume_snapshot.py
--rw-r--r--   0 marc       (501) staff       (20)     7436 2021-05-10 16:05:40.000000 exoscale-0.7.1/tests/test_compute_network_load_balancer.py
--rw-r--r--   0 marc       (501) staff       (20)     7670 2021-05-10 16:05:40.000000 exoscale-0.7.1/tests/test_compute_network_load_balancer_service.py
--rw-r--r--   0 marc       (501) staff       (20)     6741 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_compute_private_network.py
--rw-r--r--   0 marc       (501) staff       (20)     5388 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_compute_security_group.py
--rw-r--r--   0 marc       (501) staff       (20)     2964 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_compute_security_group_rule.py
--rw-r--r--   0 marc       (501) staff       (20)      946 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_compute_ssh_key.py
--rw-r--r--   0 marc       (501) staff       (20)     3376 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_config.py
--rw-r--r--   0 marc       (501) staff       (20)     1821 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_dns.py
--rw-r--r--   0 marc       (501) staff       (20)     2724 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_dns_domain.py
--rw-r--r--   0 marc       (501) staff       (20)     2773 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_dns_domain_record.py
--rw-r--r--   0 marc       (501) staff       (20)     2717 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_iam.py
--rw-r--r--   0 marc       (501) staff       (20)      720 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_iam_apikey.py
--rw-r--r--   0 marc       (501) staff       (20)     9646 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_storage.py
--rw-r--r--   0 marc       (501) staff       (20)    12196 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_storage_bucket.py
--rw-r--r--   0 marc       (501) staff       (20)     8532 2021-05-10 12:31:04.000000 exoscale-0.7.1/tests/test_storage_bucket_file.py
+-rw-r--r--   0        0        0     8652 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/__init__.py
+-rw-r--r--   0        0        0   526553 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/openapi.json
+-rw-r--r--   0        0        0     4471 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/__init__.py
+-rw-r--r--   0        0        0   112258 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/compute.py
+-rw-r--r--   0        0        0     8501 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/dns.py
+-rw-r--r--   0        0        0     4578 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/iam.py
+-rw-r--r--   0        0        0     6915 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/polling.py
+-rw-r--r--   0        0        0    24928 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/runstatus.py
+-rw-r--r--   0        0        0    23936 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/storage.py
+-rw-r--r--   0        0        0     8534 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/v2.py
+-rw-r--r--   0        0        0       50 2023-05-11 14:44:45.000000 exoscale-0.8.0/.gitignore
+-rw-r--r--   0        0        0      746 2023-05-11 14:44:45.000000 exoscale-0.8.0/LICENSE
+-rw-r--r--   0        0        0      995 2023-05-11 14:44:45.000000 exoscale-0.8.0/README.md
+-rw-r--r--   0        0        0     1474 2023-05-11 14:44:45.000000 exoscale-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2457 2023-05-11 14:44:45.000000 exoscale-0.8.0/PKG-INFO
```

### Comparing `exoscale-0.7.1/PKG-INFO` & `exoscale-0.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,62 @@
 Metadata-Version: 2.1
 Name: exoscale
-Version: 0.7.1
-Summary: UNKNOWN
-Home-page: https://github.com/exoscale/python-exoscale
-Author: Exoscale
-Author-email: contact@exoscale.com
-License: ISC
-Description: # python-exoscale: Python bindings for Exoscale API
-        
-        [![Actions Status](https://github.com/exoscale/python-exoscale/workflows/CI/badge.svg)](https://github.com/exoscale/python-exoscale/actions?query=workflow%3ACI)
-        
-        This library allows developpers to use the [Exoscale] cloud platform API with
-        high-level Python bindings. API documentation and usage examples can be found
-        at this address: https://exoscale.github.io/python-exoscale
-        
-        ## Development
-        
-        First create a new virtual environment and run `make installrequirements`.
-        Then create a configuration file with your **production** user's API keys.
-        This file may be create for example in `junk/config.toml`. Here is an example:
-        
-            default_profile = "prod:you"
-        
-            [[profiles]]
-            name       = "prod:you"
-            api_key    = "EXOxxxx"
-            api_secret = "yyyy"
-        
-        Once this file is created you can run pytest with the following command:
-        
-            EXOSCALE_CONFIG_FILE=./junk/config.toml pytest -x -s -vvv tests/*.py
-        
-        [exoscale]: https://www.exoscale.com/
-        
-Platform: any
+Version: 0.8.0
+Summary: Clients for Exoscale IaaS APIs
+Project-URL: Homepage, https://github.com/exoscale/python-exoscale
+Project-URL: Bug Tracker, https://github.com/exoscale/python-exoscale/issues
+Author-email: Exoscale <support@exoscale.com>
+License-Expression: ISC
+License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Requires-Dist: attrs>=20.1.0
+Requires-Dist: boto3>=1.9.176
+Requires-Dist: cs>=2.7.1
+Requires-Dist: requests-exoscale-auth>=1.1.2
+Requires-Dist: requests>=2.22.0
+Requires-Dist: toml>=0.10.0
+Provides-Extra: dev
+Requires-Dist: pytest-timeout>=1.4.2; extra == 'dev'
+Requires-Dist: pytest>=5.0.0; extra == 'dev'
+Requires-Dist: recommonmark>=0.5.0; extra == 'dev'
+Requires-Dist: requests-mock>=1.8.0; extra == 'dev'
+Requires-Dist: sphinx-markdown-parser>=0.1.1; extra == 'dev'
+Requires-Dist: sphinx-rtd-theme>=0.4.3; extra == 'dev'
+Requires-Dist: sphinx>=2.1.2; extra == 'dev'
 Description-Content-Type: text/markdown
+
+# python-exoscale: Python bindings for Exoscale API
+
+[![Actions Status](https://github.com/exoscale/python-exoscale/workflows/CI/badge.svg)](https://github.com/exoscale/python-exoscale/actions?query=workflow%3ACI)
+
+This library allows developpers to use the [Exoscale] cloud platform API with
+high-level Python bindings. API documentation and usage examples can be found
+at this address: https://exoscale.github.io/python-exoscale
+
+## Development
+
+First create a new virtual environment and run `make installrequirements`.
+Then create a configuration file with your **production** user's API keys.
+This file may be create for example in `junk/config.toml`. Here is an example:
+
+    default_profile = "prod:you"
+
+    [[profiles]]
+    name       = "prod:you"
+    api_key    = "EXOxxxx"
+    api_secret = "yyyy"
+
+Once this file is created you can run pytest with the following command:
+
+    EXOSCALE_CONFIG_FILE=./junk/config.toml pytest -x -s -vvv tests/*.py
+
+[exoscale]: https://www.exoscale.com/
```

### Comparing `exoscale-0.7.1/README.md` & `exoscale-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `exoscale-0.7.1/exoscale/__init__.py` & `exoscale-0.8.0/exoscale/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
+__version__ = "0.8.0"
 
-import attr
 import os
 import pathlib
 import toml
+from attr import field
 from .api.compute import ComputeAPI
 from .api.dns import DnsAPI
 from .api.storage import StorageAPI
 from .api.runstatus import RunstatusAPI
 from .api.iam import IamAPI
 
 _API_KEY_ENVVAR = "EXOSCALE_API_KEY"
@@ -63,32 +64,40 @@
         runstatus_api_endpoint=None,
         iam_api_endpoint=None,
         max_retries=3,
         trace=False,
     ):
         # Load settings from a configuration file profile
         config_file = (
-            config_file if config_file else os.getenv(_CONFIG_FILE_ENVVAR, None)
+            config_file
+            if config_file
+            else os.getenv(_CONFIG_FILE_ENVVAR, None)
         )
         if config_file:
             with open(config_file) as f:
                 self._config = toml.load(f)
 
-        if not getattr(self, "_config", None) and os.path.exists(_DEFAULT_CONFIG_FILE):
+        if not getattr(self, "_config", None) and os.path.exists(
+            _DEFAULT_CONFIG_FILE
+        ):
             with open(_DEFAULT_CONFIG_FILE) as f:
                 self._config = toml.load(f)
 
         if getattr(self, "_config", None) is not None:
             profile = self._get_profile(profile)
             for k in {"name", "api_key", "api_secret"}:
                 if k not in profile:
-                    raise ConfigurationError('profile missing "{}" key'.format(k))
+                    raise ConfigurationError(
+                        'profile missing "{}" key'.format(k)
+                    )
 
             api_key = profile["api_key"] if not api_key else api_key
-            api_secret = profile["api_secret"] if not api_secret else api_secret
+            api_secret = (
+                profile["api_secret"] if not api_secret else api_secret
+            )
             compute_api_endpoint = (
                 profile.get("compute_api_endpoint", None)
                 if not compute_api_endpoint
                 else compute_api_endpoint
             )
             dns_api_endpoint = (
                 profile.get("dns_api_endpoint", None)
@@ -97,30 +106,34 @@
             )
             storage_api_endpoint = (
                 profile.get("storage_api_endpoint", None)
                 if not storage_api_endpoint
                 else storage_api_endpoint
             )
             storage_zone = (
-                profile.get("storage_zone", None) if not storage_zone else storage_zone
+                profile.get("storage_zone", None)
+                if not storage_zone
+                else storage_zone
             )
             runstatus_api_endpoint = (
                 profile.get("runstatus_api_endpoint", None)
                 if not runstatus_api_endpoint
                 else runstatus_api_endpoint
             )
             iam_api_endpoint = (
                 profile.get("iam_api_endpoint", None)
                 if not iam_api_endpoint
                 else iam_api_endpoint
             )
 
         # Fallback: load settings from environment variables
         api_key = api_key if api_key else os.getenv(_API_KEY_ENVVAR, None)
-        api_secret = api_secret if api_secret else os.getenv(_API_SECRET_ENVVAR, None)
+        api_secret = (
+            api_secret if api_secret else os.getenv(_API_SECRET_ENVVAR, None)
+        )
         compute_api_endpoint = (
             compute_api_endpoint
             if compute_api_endpoint
             else os.getenv(_COMPUTE_API_ENDPOINT_ENVVAR, None)
         )
         dns_api_endpoint = (
             dns_api_endpoint
@@ -129,15 +142,17 @@
         )
         storage_api_endpoint = (
             storage_api_endpoint
             if storage_api_endpoint
             else os.getenv(_STORAGE_API_ENDPOINT_ENVVAR, None)
         )
         storage_zone = (
-            storage_zone if storage_zone else os.getenv(_STORAGE_ZONE_ENVVAR, None)
+            storage_zone
+            if storage_zone
+            else os.getenv(_STORAGE_ZONE_ENVVAR, None)
         )
         runstatus_api_endpoint = (
             runstatus_api_endpoint
             if runstatus_api_endpoint
             else os.getenv(_RUNSTATUS_API_ENDPOINT_ENVVAR, None)
         )
         iam_api_endpoint = (
@@ -201,15 +216,18 @@
             "trace": trace,
         }
         if iam_api_endpoint is not None:
             kwargs["endpoint"] = iam_api_endpoint
         self.iam = IamAPI(**kwargs)
 
     def _get_profile(self, profile=None):
-        if "profiles" not in self._config or len(self._config["profiles"]) == 0:
+        if (
+            "profiles" not in self._config
+            or len(self._config["profiles"]) == 0
+        ):
             raise ConfigurationError("no profiles configured")
 
         if profile or "default_profile" in self._config:
             if "default_profile" in self._config and not profile:
                 profile = self._config["default_profile"]
 
             for a in self._config["profiles"]:
@@ -228,8 +246,8 @@
 
 
 class ConfigurationError(Exception):
     """
     A generic configuration error.
     """
 
-    reason = attr.ib()
+    reason = field()
```

### Comparing `exoscale-0.7.1/exoscale/api/__init__.py` & `exoscale-0.8.0/exoscale/api/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 """
 Note:
     This module is not intended for standalone use, please use the :code:`exoscale`
     module or the :code:`exoscale.api.*` submodules.
 """
 
 
-import attr
 import pkg_resources
 import platform
 import requests
 import sys
+from attr import asdict, define, field
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from requests.utils import default_user_agent as requests_user_agent
 
 
-@attr.s
+@define
 class API(object):
     """
     An Exoscale API client.
 
     Attributes:
         endpoint (str): the API endpoint
         key (str): the API key
@@ -29,33 +29,35 @@
         session (requests.Session): the API HTTP session
         max_retries (int): the API HTTP session retry policy number of retries to allow
         retry_backoff_factor (int): the API HTTP session retry policy backoff factor to
             apply between attempts after the second try
         trace (bool): API request/response tracing flag
     """
 
-    endpoint = attr.ib()
-    key = attr.ib()
-    secret = attr.ib(repr=False)
-    trace = attr.ib(default=False, repr=False)
-    session = attr.ib(default=requests.Session(), repr=False)
-    max_retries = attr.ib(default=3, repr=False)
-    retry_backoff_factor = attr.ib(default=0.3, repr=False)
+    endpoint = field()
+    key = field()
+    secret = field(repr=False)
+    trace = field(default=False, repr=False)
+    session = field(default=requests.Session(), repr=False)
+    max_retries = field(default=3, repr=False)
+    retry_backoff_factor = field(default=0.3, repr=False)
 
     def __attrs_post_init__(self):
         # HTTP session-related settings
 
         self.user_agent = (
             "Exoscale-Python/{python_exoscale_version} "
             "cs/{cs_version} "
             "{requests_user_agent} "
             "{python_implementation}/{python_version} "
             "{os_name}/{os_version}"
         ).format(
-            python_exoscale_version=pkg_resources.get_distribution("exoscale").version,
+            python_exoscale_version=pkg_resources.get_distribution(
+                "exoscale"
+            ).version,
             cs_version=pkg_resources.get_distribution("cs").version,
             requests_user_agent=requests_user_agent(),
             python_implementation=platform.python_implementation(),
             python_version=platform.python_version(),
             os_name=platform.system(),
             os_version=platform.release(),
         )
@@ -85,68 +87,74 @@
         req = requests.Request(**kwargs).prepare()
 
         if self.trace:
             print(
                 ">>> {method} {url}".format(method=req.method, url=req.url),
                 file=sys.stderr,
             )
-            print("    headers:{headers}".format(headers=req.headers), file=sys.stderr)
+            print(
+                "    headers:{headers}".format(headers=req.headers),
+                file=sys.stderr,
+            )
             if req.body:
                 print("    body:{body}".format(body=req.body), file=sys.stderr)
 
         res = self.session.send(req)
 
         if self.trace:
             print(
                 "<<< {status} {reason}".format(
                     status=res.status_code, reason=res.reason
                 ),
                 file=sys.stderr,
             )
-            print("    headers:{headers}".format(headers=res.headers), file=sys.stderr)
+            print(
+                "    headers:{headers}".format(headers=res.headers),
+                file=sys.stderr,
+            )
             print("    body:{body}".format(body=res.text), file=sys.stderr)
 
         return res
 
 
-@attr.s
+@define
 class Resource(object):
     """
     A resource returned by the Exoscale API.
     """
 
-    res = attr.ib(repr=False)
+    res = field(repr=False)
 
     def _reset(self):
         """
         Reset all attributes.
         """
 
-        for k, v in self.__dict__.items():
+        for k in asdict(self):
             setattr(self, k, None)
 
 
-@attr.s
+@define
 class APIException(Exception):
     """
     A generic API error.
     """
 
-    reason = attr.ib()
-    error = attr.ib(default=None, repr=False)
+    reason = field()
+    error = field(default=None, repr=False)
 
 
-@attr.s
+@define
 class RequestError(Exception):
     """
     An API request error.
     """
 
-    reason = attr.ib()
-    error = attr.ib(default=None, repr=False)
+    reason = field()
+    error = field(default=None, repr=False)
 
 
 class ResourceNotFoundError(APIException):
     """
     An error indicating that requested resource cannot be found.
     """
```

### Comparing `exoscale-0.7.1/exoscale/api/compute.py` & `exoscale-0.8.0/exoscale/api/compute.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 # -*- coding: utf-8 -*-
 
 """
 This submodule represents the Exoscale Compute API.
 """
 
-import json
-import sys
-import time
 from base64 import b64decode, b64encode
 from datetime import datetime
 
-import attr
-import requests
+from attr import asdict, define, field
 from cs import CloudStack, CloudStackApiException
 from exoscale_auth import ExoscaleV2Auth
 
-from . import API, APIException, RequestError, Resource, ResourceNotFoundError, polling
+from . import (
+    API,
+    APIException,
+    RequestError,
+    Resource,
+    ResourceNotFoundError,
+    polling,
+)
 
 
-@attr.s
+@define
 class AntiAffinityGroup(Resource):
     """
     An Anti-Affinity Group.
 
     Attributes:
         id (str): the Anti-Affinity Group unique identifier
         name (str): the Anti-Affinity Group display name
         description (str): the Anti-Affinity Group description
     """
 
-    compute = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    name = attr.ib()
-    description = attr.ib(default="", repr=False)
+    compute = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    name = field()
+    description = field(default="", repr=False)
 
     @classmethod
     def _from_cs(cls, compute, res):
         return cls(
             compute,
             res,
             id=res["id"],
@@ -57,47 +60,47 @@
             self.compute.cs.deleteAffinityGroup(id=self.id)
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         self._reset()
 
 
-@attr.s
+@define
 class DeployTarget(Resource):
     """
     A Deploy Target.
 
     Attributes:
         id (str): the Deploy Target unique identifier
         zone (Zone): the zone in which the Deploy Target is located
         name (str): the Deploy Target name
         description (str): the Deploy Target description
         typ (str): the Deploy Target type
     """
 
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    zone = attr.ib(repr=False)
-    name = attr.ib()
-    typ = attr.ib(repr=False)
-    description = attr.ib(default=None, repr=False)
+    res = field(repr=False)
+    id = field()
+    zone = field(repr=False)
+    name = field()
+    typ = field(repr=False)
+    description = field(default=None, repr=False)
 
     @classmethod
     def _from_api(cls, res, zone):
         return cls(
             res,
             id=res["id"],
             zone=zone,
             name=res["name"],
             description=res.get("description"),
             typ=res["type"],
         )
 
 
-@attr.s
+@define
 class ElasticIP(Resource):
     """
     An Elastic IP.
 
     Attributes:
         id (str): the Elastic IP unique identifier
         zone (Zone): the zone in which the Elastic IP is located
@@ -115,29 +118,29 @@
         healthcheck_strikes_fail (int): the number of unsuccessful healthcheck probes
             before considering the target unhealthy
         healthcheck_tls_sni (str): the TLS SNI domain to present for HTTPS healthchecks
         healthcheck_tls_skip_verify (bool): whether to skip TLS certificate validation
             for HTTPS healthchecks
     """
 
-    compute = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    zone = attr.ib(repr=False)
-    address = attr.ib()
-    description = attr.ib(default=None, repr=False)
-    healthcheck_mode = attr.ib(default=None, repr=False)
-    healthcheck_port = attr.ib(default=None, repr=False)
-    healthcheck_path = attr.ib(default=None, repr=False)
-    healthcheck_interval = attr.ib(default=None, repr=False)
-    healthcheck_timeout = attr.ib(default=None, repr=False)
-    healthcheck_strikes_ok = attr.ib(default=None, repr=False)
-    healthcheck_strikes_fail = attr.ib(default=None, repr=False)
-    healthcheck_tls_sni = attr.ib(default=None, repr=False)
-    healthcheck_tls_skip_verify = attr.ib(default=None, repr=False)
+    compute = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    zone = field(repr=False)
+    address = field()
+    description = field(default=None, repr=False)
+    healthcheck_mode = field(default=None, repr=False)
+    healthcheck_port = field(default=None, repr=False)
+    healthcheck_path = field(default=None, repr=False)
+    healthcheck_interval = field(default=None, repr=False)
+    healthcheck_timeout = field(default=None, repr=False)
+    healthcheck_strikes_ok = field(default=None, repr=False)
+    healthcheck_strikes_fail = field(default=None, repr=False)
+    healthcheck_tls_sni = field(default=None, repr=False)
+    healthcheck_tls_skip_verify = field(default=None, repr=False)
 
     @classmethod
     def _from_cs(cls, compute, res, zone=None):
         if zone is None:
             zone = compute.get_zone(id=res["zoneid"])
 
         return cls(
@@ -146,21 +149,29 @@
             id=res["id"],
             zone=zone,
             address=res["ipaddress"],
             description=res.get("description", ""),
             healthcheck_mode=res.get("healthcheck", {}).get("mode", None),
             healthcheck_port=res.get("healthcheck", {}).get("port", None),
             healthcheck_path=res.get("healthcheck", {}).get("path", None),
-            healthcheck_interval=res.get("healthcheck", {}).get("interval", None),
-            healthcheck_timeout=res.get("healthcheck", {}).get("timeout", None),
-            healthcheck_strikes_ok=res.get("healthcheck", {}).get("strikes-ok", None),
+            healthcheck_interval=res.get("healthcheck", {}).get(
+                "interval", None
+            ),
+            healthcheck_timeout=res.get("healthcheck", {}).get(
+                "timeout", None
+            ),
+            healthcheck_strikes_ok=res.get("healthcheck", {}).get(
+                "strikes-ok", None
+            ),
             healthcheck_strikes_fail=res.get("healthcheck", {}).get(
                 "strikes-fail", None
             ),
-            healthcheck_tls_sni=res.get("healthcheck", {}).get("tls-sni", None),
+            healthcheck_tls_sni=res.get("healthcheck", {}).get(
+                "tls-sni", None
+            ),
             healthcheck_tls_skip_verify=res.get("healthcheck", {}).get(
                 "tls-skip-verify", None
             ),
         )
 
     @property
     def instances(self):
@@ -270,31 +281,37 @@
         self.healthcheck_port = (
             healthcheck_port if healthcheck_port else self.healthcheck_port
         )
         self.healthcheck_path = (
             healthcheck_path if healthcheck_path else self.healthcheck_path
         )
         self.healthcheck_interval = (
-            healthcheck_interval if healthcheck_interval else self.healthcheck_interval
+            healthcheck_interval
+            if healthcheck_interval
+            else self.healthcheck_interval
         )
         self.healthcheck_timeout = (
-            healthcheck_timeout if healthcheck_timeout else self.healthcheck_timeout
+            healthcheck_timeout
+            if healthcheck_timeout
+            else self.healthcheck_timeout
         )
         self.healthcheck_strikes_ok = (
             healthcheck_strikes_ok
             if healthcheck_strikes_ok
             else self.healthcheck_strikes_ok
         )
         self.healthcheck_strikes_fail = (
             healthcheck_strikes_fail
             if healthcheck_strikes_fail
             else self.healthcheck_strikes_fail
         )
         self.healthcheck_tls_sni = (
-            healthcheck_tls_sni if healthcheck_tls_sni else self.healthcheck_tls_sni
+            healthcheck_tls_sni
+            if healthcheck_tls_sni
+            else self.healthcheck_tls_sni
         )
         self.healthcheck_tls_skip_verify = (
             healthcheck_tls_skip_verify
             if healthcheck_tls_skip_verify
             else self.healthcheck_tls_skip_verify
         )
 
@@ -375,15 +392,15 @@
             self.compute.cs.disassociateIpAddress(id=self.id)
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         self._reset()
 
 
-@attr.s
+@define
 class Instance(Resource):
     """
     A Compute instance.
 
     Attributes:
         id (str): the instance unique identifier
         name (str): the instance hostname/display name
@@ -395,45 +412,49 @@
         ipv4_address (str): the instance public network interface IP address
         ipv6_address (str): the instance public network interface IPv6 address,
             or None if IPv6 is not enabled
         ssh_key (SSHKey): the SSH key installed in the instance user account,
         or None if no SSH key specified during instance creation
     """
 
-    compute = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    name = attr.ib()
-    creation_date = attr.ib(repr=False)
-    zone = attr.ib(repr=False)
-    type = attr.ib(repr=False)
-    template = attr.ib(repr=False)
-    volume_id = attr.ib(repr=False)
-    volume_size = attr.ib(repr=False)
-    ipv4_address = attr.ib(repr=False)
-    ipv6_address = attr.ib(default=None, repr=False)
-    ssh_key = attr.ib(default=None, repr=False)
+    compute = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    name = field()
+    creation_date = field(repr=False)
+    zone = field(repr=False)
+    type = field(repr=False)
+    template = field(repr=False)
+    volume_id = field(repr=False)
+    volume_size = field(repr=False)
+    ipv4_address = field(repr=False)
+    ipv6_address = field(default=None, repr=False)
+    ssh_key = field(default=None, repr=False)
 
     @classmethod
     def _from_cs(cls, compute, res, zone=None):
         if zone is None:
             zone = compute.get_zone(id=res["zoneid"])
 
         try:
-            _list = compute.cs.listVolumes(virtualmachineid=res["id"], fetch_list=True)
+            _list = compute.cs.listVolumes(
+                virtualmachineid=res["id"], fetch_list=True
+            )
             volume_res = _list[0]
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         return cls(
             compute,
             res,
             id=res["id"],
             name=res["displayname"],
-            creation_date=datetime.strptime(res["created"], "%Y-%m-%dT%H:%M:%S%z"),
+            creation_date=datetime.strptime(
+                res["created"], "%Y-%m-%dT%H:%M:%S%z"
+            ),
             zone=zone,
             type=compute.get_instance_type(id=res["serviceofferingid"]),
             template=compute.get_instance_template(zone, id=res["templateid"]),
             volume_id=volume_res["id"],
             volume_size=volume_res["size"],
             ipv4_address=next(i for i in res["nic"] if i["isdefault"]).get(
                 "ipaddress", None
@@ -479,15 +500,17 @@
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
         try:
             # FIXME: use `iselastic=True` filter
-            _list = self.compute.cs.listNics(virtualmachineid=self.id, fetch_list=True)
+            _list = self.compute.cs.listNics(
+                virtualmachineid=self.id, fetch_list=True
+            )
             default_nic = self._default_nic(_list)
             for a in default_nic.get("secondaryip", []):
                 yield self.compute.get_elastic_ip(
                     zone=self.zone, address=a["ipaddress"]
                 )
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
@@ -502,15 +525,17 @@
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
         try:
-            _list = self.compute.cs.listNics(virtualmachineid=self.id, fetch_list=True)
+            _list = self.compute.cs.listNics(
+                virtualmachineid=self.id, fetch_list=True
+            )
             for nic in _list:
                 if nic["isdefault"]:
                     continue
                 yield self.compute.get_private_network(
                     zone=self.zone, id=nic["networkid"]
                 )
         except CloudStackApiException as e:
@@ -530,15 +555,17 @@
         """
 
         try:
             res = self.compute.cs.queryReverseDnsForVirtualMachine(id=self.id)
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
-        reverse_dns = self._default_nic(res["virtualmachine"]["nic"])["reversedns"]
+        reverse_dns = self._default_nic(res["virtualmachine"]["nic"])[
+            "reversedns"
+        ]
         if reverse_dns:
             return reverse_dns[0]["domainname"]
 
     @property
     def security_groups(self):
         """
         Security Groups the instance is member of.
@@ -592,15 +619,17 @@
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
         try:
-            [res] = self.compute.cs.listVirtualMachines(id=self.id, fetch_list=True)
+            [res] = self.compute.cs.listVirtualMachines(
+                id=self.id, fetch_list=True
+            )
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         return res["state"].lower()
 
     @property
     def user_data(self):
@@ -612,20 +641,24 @@
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
         try:
-            res = self.compute.cs.getVirtualMachineUserData(virtualmachineid=self.id)
+            res = self.compute.cs.getVirtualMachineUserData(
+                virtualmachineid=self.id
+            )
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         if "userdata" in res["virtualmachineuserdata"]:
-            return b64decode(res["virtualmachineuserdata"]["userdata"]).decode("utf-8")
+            return b64decode(res["virtualmachineuserdata"]["userdata"]).decode(
+                "utf-8"
+            )
 
     @property
     def instance_pool(self):
         """
         Instance Pool the instance is a member of.
 
         Returns:
@@ -633,15 +666,17 @@
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
         if self.res.get("manager") == "instancepool":
-            return self.compute.get_instance_pool(self.zone, id=self.res["managerid"])
+            return self.compute.get_instance_pool(
+                self.zone, id=self.res["managerid"]
+            )
 
     def update(self, name=None, security_groups=None, user_data=None):
         """
         Update the instance properties.
 
         Parameters:
             name (str): an instance hostname/display name
@@ -661,15 +696,16 @@
                 userdata=b64encode(bytes(user_data, encoding="utf-8"))
                 if user_data
                 else None,
             )
 
             if security_groups:
                 self.compute.cs.updateVirtualMachineSecurityGroups(
-                    id=self.id, securitygroupids=list(i.id for i in security_groups)
+                    id=self.id,
+                    securitygroupids=list(i.id for i in security_groups),
                 )
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         if name is not None:
             self.name = name
 
@@ -681,15 +717,17 @@
             type (InstanceType): the type to scale the instance to
 
         Returns:
             None
         """
 
         try:
-            self.compute.cs.scaleVirtualMachine(id=self.id, serviceofferingid=type.id)
+            self.compute.cs.scaleVirtualMachine(
+                id=self.id, serviceofferingid=type.id
+            )
             self.type = type
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
     def start(self):
         """
         Start a stopped instance.
@@ -771,15 +809,17 @@
             elastic_ip (ElasticIP): the Elastic IP to attach
 
         Returns:
             None
         """
 
         try:
-            _list = self.compute.cs.listNics(virtualmachineid=self.id, fetch_list=True)
+            _list = self.compute.cs.listNics(
+                virtualmachineid=self.id, fetch_list=True
+            )
             default_nic = self._default_nic(_list)
             self.compute.cs.addIpToNic(
                 nicid=default_nic["id"], ipaddress=elastic_ip.address
             )
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
@@ -791,15 +831,17 @@
             elastic_ip (ElasticIP): the Elastic IP to detach
 
         Returns:
             None
         """
 
         try:
-            _list = self.compute.cs.listNics(virtualmachineid=self.id, fetch_list=True)
+            _list = self.compute.cs.listNics(
+                virtualmachineid=self.id, fetch_list=True
+            )
             default_nic = self._default_nic(_list)
             for a in default_nic.get("secondaryip", []):
                 if a["ipaddress"] == elastic_ip.address:
                     self.compute.cs.removeIpFromNic(id=a["id"])
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
@@ -830,15 +872,17 @@
 
         Returns:
             None
         """
 
         try:
             [res] = self.compute.cs.listNics(
-                virtualmachineid=self.id, networkid=private_network.id, fetch_list=True
+                virtualmachineid=self.id,
+                networkid=private_network.id,
+                fetch_list=True,
             )
 
             self.compute.cs.removeNicFromVirtualMachine(
                 virtualmachineid=self.id, nicid=res["id"]
             )
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
@@ -891,15 +935,15 @@
 
     def _default_nic(self, nics):
         for nic in nics:
             if nic["isdefault"]:
                 return nic
 
 
-@attr.s
+@define
 class InstanceTemplate(Resource):
     """
     A Compute instance template.
 
     Attributes:
         id (str): the template unique identifier
         name (str): the template name
@@ -915,26 +959,26 @@
 
     References:
         * `Python datetime module`_
 
         .. _Python datetime module: https://docs.python.org/3/library/datetime.html
     """
 
-    compute = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    name = attr.ib()
-    description = attr.ib(repr=False)
-    zone = attr.ib(repr=False)
-    date = attr.ib(repr=False)
-    size = attr.ib(repr=False)
-    boot_mode = attr.ib(repr=False)
-    ssh_key_enabled = attr.ib(default=True, repr=False)
-    password_reset_enabled = attr.ib(default=True, repr=False)
-    username = attr.ib(default=None, repr=False)
+    compute = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    name = field()
+    description = field(repr=False)
+    zone = field(repr=False)
+    date = field(repr=False)
+    size = field(repr=False)
+    boot_mode = field(repr=False)
+    ssh_key_enabled = field(default=True, repr=False)
+    password_reset_enabled = field(default=True, repr=False)
+    username = field(default=None, repr=False)
 
     @classmethod
     def _from_cs(cls, compute, res, zone=None):
         if zone is None:
             zone = compute.get_zone(id=res["zoneid"])
 
         return cls(
@@ -1000,15 +1044,15 @@
             self.compute.cs.deleteTemplate(id=self.id)
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         self._reset()
 
 
-@attr.s
+@define
 class InstanceVolumeSnapshot(Resource):
     """
     A Compute instance storage volume snapshot.
 
     Attributes:
         id (str): the instance storage volume snapshot unique identifier
         date (datetime.datetime): the instance storage volume snapshot creation date
@@ -1016,19 +1060,19 @@
 
     References:
         * `Python datetime module`_
 
         .. _Python datetime module: https://docs.python.org/3/library/datetime.html
     """
 
-    compute = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    date = attr.ib(repr=False)
-    size = attr.ib(repr=False)
+    compute = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    date = field(repr=False)
+    size = field(repr=False)
 
     @classmethod
     def _from_cs(cls, compute, res):
         return cls(
             compute,
             res,
             id=res["id"],
@@ -1099,44 +1143,44 @@
             res = self.compute.cs.exportSnapshot(id=self.id)
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         return res
 
 
-@attr.s
+@define
 class InstanceType(Resource):
     """
     A Compute instance type.
 
     Attributes:
         id (str): the instance type unique identifier
         name (str): the instance type name
         cpu (int): the number of vCPU allocated
         memory (int): the amount of RAM allocated in MB
     """
 
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    name = attr.ib()
-    cpu = attr.ib(repr=False)
-    memory = attr.ib(repr=False)
+    res = field(repr=False)
+    id = field()
+    name = field()
+    cpu = field(repr=False)
+    memory = field(repr=False)
 
     @classmethod
     def _from_cs(cls, res):
         return cls(
             res,
             id=res["id"],
             name=res["name"],
             cpu=res["cpunumber"],
             memory=res["memory"],
         )
 
 
-@attr.s
+@define
 class InstancePool(Resource):
     """
     A Compute Instance Pool.
 
     Attributes:
         description (str): the Instance Pool description
         id (str): the Instance Pool unique identifier
@@ -1156,48 +1200,52 @@
         instance_volume_size (int): the storage volume capacity in bytes to set when
             this Instance Pool creates new instances
         name (str): the Instance Pool name
         size (int): the number of Compute instance members the Instance Pool manages
         zone (Zone): the zone in which the Instance Pool is located
     """
 
-    compute = attr.ib(repr=False)
-    id = attr.ib()
-    instance_template = attr.ib(repr=False)
-    instance_type = attr.ib(repr=False)
-    instance_user_data = attr.ib(repr=False)
-    instance_volume_size = attr.ib(repr=False)
-    name = attr.ib()
-    res = attr.ib(repr=False)
-    size = attr.ib(repr=False)
-    zone = attr.ib(repr=False)
-    description = attr.ib(default=None, repr=False)
-    instance_deploy_target = attr.ib(default=None, repr=False)
-    instance_ipv6_enabled = attr.ib(default=False, repr=False)
-    instance_prefix = attr.ib(default="pool", repr=False)
-    instance_ssh_key = attr.ib(default=None, repr=False)
+    compute = field(repr=False)
+    id = field()
+    instance_template = field(repr=False)
+    instance_type = field(repr=False)
+    instance_user_data = field(repr=False)
+    instance_volume_size = field(repr=False)
+    name = field()
+    res = field(repr=False)
+    size = field(repr=False)
+    zone = field(repr=False)
+    description = field(default=None, repr=False)
+    instance_deploy_target = field(default=None, repr=False)
+    instance_ipv6_enabled = field(default=False, repr=False)
+    instance_prefix = field(default="pool", repr=False)
+    instance_ssh_key = field(default=None, repr=False)
 
     @classmethod
     def _from_api(cls, compute, res, zone):
         return cls(
             compute=compute,
             description=res.get("description"),
             id=res["id"],
             instance_deploy_target=None
             if "deploy-target" not in res
-            else compute.get_deploy_target(zone, id=res["deploy-target"]["id"]),
+            else compute.get_deploy_target(
+                zone, id=res["deploy-target"]["id"]
+            ),
             instance_ipv6_enabled=res["ipv6-enabled"],
             instance_prefix=res["instance-prefix"],
             instance_ssh_key=None
             if "ssh-key" not in res
-            else compute.get_ssh_key(res["ssh-key"]),
+            else compute.get_ssh_key(res["ssh-key"]["name"]),
             instance_template=compute.get_instance_template(
                 zone, id=res["template"]["id"]
             ),
-            instance_type=compute.get_instance_type(id=res["instance-type"]["id"]),
+            instance_type=compute.get_instance_type(
+                id=res["instance-type"]["id"]
+            ),
             instance_user_data=res.get("user-data"),
             instance_volume_size=res["disk-size"],
             name=res["name"],
             res=res,
             size=res["size"],
             zone=zone,
         )
@@ -1428,18 +1476,22 @@
         if instance_enable_ipv6 is not None:
             data["ipv6-enabled"] = instance_enable_ipv6
 
         if instance_prefix is not None:
             data["instance-prefix"] = instance_prefix
 
         if instance_private_networks is not None:
-            data["private-networks"] = [{"id": i.id} for i in instance_private_networks]
+            data["private-networks"] = [
+                {"id": i.id} for i in instance_private_networks
+            ]
 
         if instance_security_groups is not None:
-            data["security-groups"] = [{"id": i.id} for i in instance_security_groups]
+            data["security-groups"] = [
+                {"id": i.id} for i in instance_security_groups
+            ]
 
         if instance_ssh_key is not None:
             data["ssh-key"] = instance_ssh_key.name
 
         if instance_template is not None:
             data["template"] = {"id": instance_template.id}
 
@@ -1495,15 +1547,15 @@
         self.compute._v2_request_async(
             "DELETE", "/instance-pool/" + self.id, self.zone.name
         )
 
         self._reset()
 
 
-@attr.s
+@define
 class NetworkLoadBalancerServiceHealthcheck(Resource):
     """
     A Network Load Balancer service healthcheck.
 
     Attributes:
         mode (str): the healthcheck probing mode (tcp|http|https)
         port (int): the healthcheck service port to probe
@@ -1513,22 +1565,22 @@
         timeout (int): the time in seconds before considering a healthcheck
             probing failed
         retries (int): the number of times to retry a failed healthchecking probe before
             marking the target as failing
         tls_sni (str): the TLS SNI domain to present for HTTPS healthchecks
     """
 
-    res = attr.ib(repr=False)
-    mode = attr.ib()
-    port = attr.ib()
-    uri = attr.ib(default=None, repr=False)
-    interval = attr.ib(default=None, repr=False)
-    timeout = attr.ib(default=None, repr=False)
-    retries = attr.ib(default=None, repr=False)
-    tls_sni = attr.ib(default=None, repr=False)
+    res = field(repr=False)
+    mode = field()
+    port = field()
+    uri = field(default=None, repr=False)
+    interval = field(default=None, repr=False)
+    timeout = field(default=None, repr=False)
+    retries = field(default=None, repr=False)
+    tls_sni = field(default=None, repr=False)
 
     @classmethod
     def _from_api(cls, res):
         return cls(
             res,
             mode=res["mode"],
             port=res["port"],
@@ -1536,15 +1588,15 @@
             interval=res.get("interval"),
             timeout=res.get("timeout"),
             retries=res.get("retries"),
             tls_sni=res.get("tls-sni"),
         )
 
 
-@attr.s
+@define
 class NetworkLoadBalancerService(Resource):
     """
     A Network Load Balancer service.
 
     Attributes:
         nlb (NetworkLoadBalancer): the parent Network Load Balancer instance
         id (str): the Network Load Balancer service uniquer identifier
@@ -1558,26 +1610,26 @@
         protocol (str): the Network Load Balancer service protocol (tcp|udp)
         strategy (str): the Network Load Balancer service dispatch strategy
             (round-robin|source-hash)
         healthcheck (NetworkLoadBalancerServiceHealthcheck): the Network Load Balancer
             service healthcheck
     """
 
-    compute = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    nlb = attr.ib(repr=False)
-    id = attr.ib()
-    name = attr.ib()
-    instance_pool = attr.ib(repr=False)
-    port = attr.ib(repr=False)
-    target_port = attr.ib(repr=False)
-    protocol = attr.ib(repr=False)
-    strategy = attr.ib(repr=False)
-    healthcheck = attr.ib(repr=False)
-    description = attr.ib(default="", repr=False)
+    compute = field(repr=False)
+    res = field(repr=False)
+    nlb = field(repr=False)
+    id = field()
+    name = field()
+    instance_pool = field(repr=False)
+    port = field(repr=False)
+    target_port = field(repr=False)
+    protocol = field(repr=False)
+    strategy = field(repr=False)
+    healthcheck = field(repr=False)
+    description = field(default="", repr=False)
 
     @classmethod
     def _from_api(cls, compute, res, nlb):
         return cls(
             compute,
             res,
             nlb=nlb,
@@ -1691,16 +1743,20 @@
                 "description": description
                 if description is not None
                 else self.description,
                 "port": port if port is not None else self.port,
                 "target-port": target_port
                 if target_port is not None
                 else self.target_port,
-                "protocol": protocol if protocol is not None else self.protocol,
-                "strategy": strategy if strategy is not None else self.strategy,
+                "protocol": protocol
+                if protocol is not None
+                else self.protocol,
+                "strategy": strategy
+                if strategy is not None
+                else self.strategy,
                 "healthcheck": {
                     "mode": healthcheck_mode
                     if healthcheck_mode is not None
                     else self.healthcheck.mode,
                     "port": healthcheck_port
                     if healthcheck_port is not None
                     else self.healthcheck.port,
@@ -1763,47 +1819,49 @@
             "/load-balancer/{}/service/{}".format(self.nlb.id, self.id),
             self.nlb.zone.name,
         )
 
         self._reset()
 
 
-@attr.s
+@define
 class NetworkLoadBalancer(Resource):
     """
     A Network Load Balancer.
 
     Attributes:
         id (str): the Network Load Balancer unique identifier
         name (str): the Network Load Balancer name
         description (str): a Network Load Balancer description
         creation_date (datetime.datetime): the Network Load Balancer creation date
         ip_address (str): the Network Load Balancer public IP address
         zone (Zone): the zone in which the Network Load Balancer is located
     """
 
-    compute = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    name = attr.ib()
-    creation_date = attr.ib(repr=False)
-    ip_address = attr.ib(repr=False)
-    zone = attr.ib(repr=False)
-    description = attr.ib(default="", repr=False)
+    compute = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    name = field()
+    creation_date = field(repr=False)
+    ip_address = field(repr=False)
+    zone = field(repr=False)
+    description = field(default="", repr=False)
 
     @classmethod
     def _from_api(cls, compute, res, zone):
         return cls(
             compute,
             res,
             id=res["id"],
             zone=zone,
             name=res["name"],
             description=res.get("description"),
-            creation_date=datetime.strptime(res["created-at"], "%Y-%m-%dT%H:%M:%SZ"),
+            creation_date=datetime.strptime(
+                res["created-at"], "%Y-%m-%dT%H:%M:%SZ"
+            ),
             ip_address=res["ip"],
         )
 
     @property
     def services(self):
         """
         Services running on the Network Load Balancer.
@@ -1973,15 +2031,15 @@
         self.compute._v2_request_async(
             "DELETE", "/load-balancer/" + self.id, self.zone.name
         )
 
         self._reset()
 
 
-@attr.s
+@define
 class PrivateNetwork(Resource):
     """
     A Private Network.
 
     Attributes:
         id (str): the Private Network unique identifier
         name (str): the Private Network name
@@ -1992,23 +2050,23 @@
         netmask (str): the managed Private Network IP range netmask
 
     Note:
         The ``start_ip``, ``end_ip`` and ``netmask`` attributes are required in
         "managed" mode.
     """
 
-    compute = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    name = attr.ib()
-    zone = attr.ib(repr=False)
-    description = attr.ib(default="", repr=False)
-    start_ip = attr.ib(default=None, repr=False)
-    end_ip = attr.ib(default=None, repr=False)
-    netmask = attr.ib(default=None, repr=False)
+    compute = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    name = field()
+    zone = field(repr=False)
+    description = field(default="", repr=False)
+    start_ip = field(default=None, repr=False)
+    end_ip = field(default=None, repr=False)
+    netmask = field(default=None, repr=False)
 
     @classmethod
     def _from_cs(cls, compute, res, zone=None):
         if zone is None:
             zone = compute.get_zone(id=res["zoneid"])
 
         return cls(
@@ -2035,15 +2093,20 @@
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
         return self.compute.list_instances(zone=self.zone, networkid=self.id)
 
     def update(
-        self, name=None, description=None, start_ip=None, end_ip=None, netmask=None
+        self,
+        name=None,
+        description=None,
+        start_ip=None,
+        end_ip=None,
+        netmask=None,
     ):
         """
         Update the Private Network properties.
 
         Parameters:
             name (str): a Private Network name
             description (str): a Private Network description
@@ -2116,30 +2179,30 @@
             self.compute.cs.deleteNetwork(id=self.id)
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         self._reset()
 
 
-@attr.s
+@define
 class SecurityGroup(Resource):
     """
     A Security Group.
 
     Attributes:
         id (str): the Security Group unique identifier
         name (str): the Security Group name
         description (str): the Security Group description
     """
 
-    compute = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    name = attr.ib()
-    description = attr.ib(default="", repr=False)
+    compute = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    name = field()
+    description = field(default="", repr=False)
 
     @classmethod
     def _from_cs(cls, compute, res):
         return cls(
             compute,
             res,
             id=res["id"],
@@ -2157,15 +2220,17 @@
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
         try:
-            [res] = self.compute.cs.listSecurityGroups(id=self.id, fetch_list=True)
+            [res] = self.compute.cs.listSecurityGroups(
+                id=self.id, fetch_list=True
+            )
             for rule in res.get("ingressrule", []):
                 yield SecurityGroupRule._from_cs(
                     type="ingress", compute=self.compute, res=rule
                 )
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
@@ -2179,15 +2244,17 @@
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
         try:
-            [res] = self.compute.cs.listSecurityGroups(id=self.id, fetch_list=True)
+            [res] = self.compute.cs.listSecurityGroups(
+                id=self.id, fetch_list=True
+            )
             for rule in res.get("egressrule", []):
                 yield SecurityGroupRule._from_cs(
                     type="egress", compute=self.compute, res=rule
                 )
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
@@ -2214,15 +2281,17 @@
             "startport": start_port,
             "endport": end_port,
             "icmpcode": rule.icmp_code,
             "icmptype": rule.icmp_type,
             "protocol": rule.protocol,
         }
         if rule.security_group:
-            rule_kwargs["usersecuritygrouplist"] = {"group": rule.security_group.name}
+            rule_kwargs["usersecuritygrouplist"] = {
+                "group": rule.security_group.name
+            }
 
         try:
             if rule.type == "ingress":
                 self.compute.cs.authorizeSecurityGroupIngress(**rule_kwargs)
             else:
                 self.compute.cs.authorizeSecurityGroupEgress(**rule_kwargs)
         except CloudStackApiException as e:
@@ -2240,15 +2309,15 @@
             self.compute.cs.deleteSecurityGroup(id=self.id)
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         self._reset()
 
 
-@attr.s
+@define
 class SecurityGroupRule:
     """
     A Security Group rule.
 
     Attributes:
         id (str): the Security Group rule unique identifier
         type (str): the Security Group rule type (ingress or egress)
@@ -2259,41 +2328,44 @@
             (conflicts with network_cidr)
         port (str): the source/destination port or port range to match
         protocol (str): a network protocol to match
         icmp_code (int): an ICMP code to match
         icmp_type (int): an ICMP type to match
     """
 
-    type = attr.ib()
-    compute = attr.ib(default=None, repr=False)
-    id = attr.ib(default=None)
-    description = attr.ib(default=None, repr=False)
-    network_cidr = attr.ib(default=None, repr=False)
-    security_group = attr.ib(default=None, repr=False)
-    port = attr.ib(default=None, repr=False)
-    protocol = attr.ib(default="tcp", repr=False)
-    icmp_code = attr.ib(default=None, repr=False)
-    icmp_type = attr.ib(default=None, repr=False)
+    type = field()
+    compute = field(default=None, repr=False)
+    id = field(default=None)
+    description = field(default=None, repr=False)
+    network_cidr = field(default=None, repr=False)
+    security_group = field(default=None, repr=False)
+    port = field(default=None, repr=False)
+    protocol = field(default="tcp", repr=False)
+    icmp_code = field(default=None, repr=False)
+    icmp_type = field(default=None, repr=False)
 
     @classmethod
     def _from_cs(cls, compute, res, type):
         port = str(res.get("startport", ""))
         port = (
             "-".join([port, str(res["endport"])])
-            if res.get("startport", None) is not None and str(res["endport"]) != port
+            if res.get("startport", None) is not None
+            and str(res["endport"]) != port
             else port
         )
 
         return cls(
             type=type,
             compute=compute,
             id=res["ruleid"],
             description=res.get("description", None),
             network_cidr=res.get("cidr", None),
-            security_group=compute.get_security_group(name=res["securitygroupname"])
+            security_group=compute.get_security_group(
+                name=res["securitygroupname"]
+            )
             if "securitygroupname" in res
             else None,
             port=port,
             protocol=res.get("protocol", None),
             icmp_code=res.get("icmp_code", None),
             icmp_type=res.get("icmp_type", None),
         )
@@ -2340,15 +2412,15 @@
             if self.type == "ingress":
                 self.compute.cs.revokeSecurityGroupIngress(id=self.id)
             else:
                 self.compute.cs.revokeSecurityGroupEgress(id=self.id)
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
-        for k, v in self.__dict__.items():
+        for k in asdict(self):
             setattr(self, k, None)
 
     def _parse_port(self):
         """
         Parse the rule port attribute and returns a port range.
 
         Returns:
@@ -2356,38 +2428,40 @@
             int: end port
         """
 
         if not self.port:
             return None, None
 
         start_port, end_port = (
-            self.port.split("-", maxsplit=1) if "-" in self.port else (self.port, None)
+            self.port.split("-", maxsplit=1)
+            if "-" in self.port
+            else (self.port, None)
         )
         if not end_port:
             end_port = start_port
 
         return int(start_port), int(end_port)
 
 
-@attr.s
+@define
 class SSHKey(Resource):
     """
     A SSH key.
 
     Attributes:
         name (str): the SSH key unique name
         fingerprint (str): the SSH key fingerprint
         private_key (str): the SSH private key, or None if registered SSH key
     """
 
-    compute = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    name = attr.ib()
-    fingerprint = attr.ib()
-    private_key = attr.ib(default=None, repr=False)
+    compute = field(repr=False)
+    res = field(repr=False)
+    name = field()
+    fingerprint = field()
+    private_key = field(default=None, repr=False)
 
     @classmethod
     def _from_cs(cls, compute, res):
         return cls(
             compute,
             res,
             name=res["name"],
@@ -2407,27 +2481,27 @@
             self.compute.cs.deleteSSHKeyPair(name=self.name)
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         self._reset()
 
 
-@attr.s
+@define
 class Zone(Resource):
     """
     An Exoscale zone.
 
     Attributes:
         id (str): the zone unique identifier
         name (str): the zone name
     """
 
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    name = attr.ib()
+    res = field(repr=False)
+    id = field()
+    name = field()
 
     @classmethod
     def _from_cs(cls, res):
         return cls(res, id=res["id"], name=res["name"])
 
 
 class ComputeAPI(API):
@@ -2462,26 +2536,31 @@
         self.environment = environment
 
         self.cs = CloudStack(
             key=key,
             secret=secret,
             endpoint=endpoint,
             session=self.session,
-            headers={**self.session.headers, **{"User-Agent": self.user_agent}},
+            headers={
+                **self.session.headers,
+                **{"User-Agent": self.user_agent},
+            },
             trace=self.trace,
             fetch_result=True,
         )
 
     def __repr__(self):
-        return "ComputeAPI(endpoint='{}' key='{}')".format(self.endpoint, self.key)
+        return "ComputeAPI(endpoint='{}' key='{}')".format(
+            self.endpoint, self.key
+        )
 
     def __str__(self):
         return self.__repr__()
 
-    ### Anti-Affinity Group
+    # Anti-Affinity Group
 
     def create_anti_affinity_group(self, name, description=""):
         """
         Create an Anti-Affinity Group.
 
         Parameters:
             name (str): the Anti-Affinity Group name
@@ -2542,15 +2621,15 @@
             raise
 
         if len(anti_affinity_groups) == 0:
             raise ResourceNotFoundError
 
         return anti_affinity_groups[0]
 
-    ## Deploy Target
+    # Deploy Target
 
     def list_deploy_targets(self, zone):
         """
         List Deploy Targets.
 
         Parameters:
             zone (Zone): the zone to list in
@@ -2582,20 +2661,22 @@
         if id:
             res = self._v2_request("GET", "/deploy-target/" + id, zone.name)
             return DeployTarget._from_api(res=res, zone=zone)
 
         _list = self._v2_request("GET", "/deploy-target", zone.name)
         for i in _list["deploy-targets"]:
             if i["name"] == name:
-                res = self._v2_request("GET", "/deploy-target/" + i["id"], zone.name)
+                res = self._v2_request(
+                    "GET", "/deploy-target/" + i["id"], zone.name
+                )
                 return DeployTarget._from_api(res=res, zone=zone)
 
         raise ResourceNotFoundError
 
-    ### Elastic IP
+    # Elastic IP
 
     def create_elastic_ip(
         self,
         zone,
         description=None,
         healthcheck_mode=None,
         healthcheck_port=None,
@@ -2701,26 +2782,28 @@
             ElasticIP: an Elastic IP
         """
 
         if id is None and address is None:
             raise ValueError("either id or address must be specifed")
 
         try:
-            elastic_ips = list(self.list_elastic_ips(zone, id=id, ipaddress=address))
+            elastic_ips = list(
+                self.list_elastic_ips(zone, id=id, ipaddress=address)
+            )
         except APIException as e:
             if "does not exist" in e.error["errortext"]:
                 raise ResourceNotFoundError
             raise
 
         if len(elastic_ips) == 0:
             raise ResourceNotFoundError
 
         return elastic_ips[0]
 
-    ### Instance
+    # Instance
 
     def create_instance(
         self,
         name,
         zone,
         type,
         template,
@@ -2824,26 +2907,28 @@
             not an Elastic IP.
         """
 
         if id is None and ip_address is None:
             raise ValueError("either id or ip_address must be specifed")
 
         try:
-            instances = list(self.list_instances(zone, id=id, ipaddress=ip_address))
+            instances = list(
+                self.list_instances(zone, id=id, ipaddress=ip_address)
+            )
         except APIException as e:
             if "does not exist" in e.error["errortext"]:
                 raise ResourceNotFoundError
             raise
 
         if len(instances) == 0:
             raise ResourceNotFoundError
 
         return instances[0]
 
-    ### Instance Template
+    # Instance Template
 
     def register_instance_template(
         self,
         name,
         url,
         checksum,
         zone,
@@ -2878,15 +2963,17 @@
             zone=zone,
             bootmode=bootmode,
             username=username,
             disable_ssh_key=disable_ssh_key,
             disable_password_reset=disable_password_reset,
         )
 
-    def list_instance_templates(self, zone, name=None, type="exoscale", **kwargs):
+    def list_instance_templates(
+        self, zone, name=None, type="exoscale", **kwargs
+    ):
         """
         List instance templates.
 
         Parameters:
             zone (Zone): the zone to list in
             name (str): an instance template name to restrict results to
             type (str): an instance template type to restrict results to
@@ -2926,26 +3013,28 @@
             id (str): an instance template identifier
 
         Returns:
             InstanceTemplate: an instance template
         """
 
         try:
-            instance_templates = list(self.list_instance_templates(zone, id=id))
+            instance_templates = list(
+                self.list_instance_templates(zone, id=id)
+            )
         except APIException as e:
             if "does not exist" in e.error["errortext"]:
                 raise ResourceNotFoundError
             raise
 
         if len(instance_templates) == 0:
             raise ResourceNotFoundError
 
         return instance_templates[0]
 
-    ### Instance Type
+    # Instance Type
 
     def list_instance_types(self, **kwargs):
         """
         List Compute instance types.
 
         Yields:
             InstanceType: the next instance type
@@ -2982,15 +3071,15 @@
             raise
 
         if len(instance_types) == 0:
             raise ResourceNotFoundError
 
         return instance_types[0]
 
-    ### Instance Pool
+    # Instance Pool
 
     def create_instance_pool(
         self,
         zone,
         name,
         size,
         instance_type,
@@ -3045,54 +3134,58 @@
         """
 
         if size <= 0:
             raise ValueError("size must be > 0")
 
         data = {}
 
+        if description:
+            data["description"] = description
+
         if instance_anti_affinity_groups:
             data["anti-affinity-groups"] = [
                 {"id": i.id} for i in instance_anti_affinity_groups
             ]
 
         if instance_elastic_ips:
             data["elastic-ips"] = [{"id": i.id} for i in instance_elastic_ips]
 
         if instance_security_groups:
-            data["security-groups"] = [{"id": i.id} for i in instance_security_groups]
+            data["security-groups"] = [
+                {"id": i.id} for i in instance_security_groups
+            ]
 
         if instance_private_networks:
-            data["private-networks"] = [{"id": i.id} for i in instance_private_networks]
+            data["private-networks"] = [
+                {"id": i.id} for i in instance_private_networks
+            ]
 
         if instance_ssh_key:
-            data["ssh-key"] = instance_ssh_key.name
+            data["ssh-key"] = {"name": instance_ssh_key.name}
 
         if instance_deploy_target:
             data["deploy-target"] = {"id": instance_deploy_target.id}
 
-        instance_user_data_content = None
-        if instance_user_data is not None:
-            instance_user_data_content = b64encode(
+        if instance_user_data:
+            data["user-data"] = b64encode(
                 bytes(instance_user_data, encoding="utf-8")
             ).decode("ascii")
 
         res = self._v2_request_async(
             "POST",
             "/instance-pool",
             zone=zone.name,
             json={
-                "description": description,
                 "disk-size": instance_volume_size,
                 "instance-prefix": instance_prefix,
                 "instance-type": {"id": instance_type.id},
                 "ipv6-enabled": instance_enable_ipv6,
                 "name": name,
                 "size": size,
                 "template": {"id": instance_template.id},
-                "user-data": instance_user_data_content,
                 **data,
             },
         )
 
         return self.get_instance_pool(zone, id=res["reference"]["id"])
 
     def list_instance_pools(self, zone, **kwargs):
@@ -3130,20 +3223,22 @@
         if id:
             res = self._v2_request("GET", "/instance-pool/" + id, zone.name)
             return InstancePool._from_api(compute=self, res=res, zone=zone)
 
         _list = self._v2_request("GET", "/instance-pool", zone.name)
         for i in _list["instance-pools"]:
             if i["name"] == name:
-                res = self._v2_request("GET", "/instance-pool/" + i["id"], zone.name)
+                res = self._v2_request(
+                    "GET", "/instance-pool/" + i["id"], zone.name
+                )
                 return InstancePool._from_api(compute=self, res=res, zone=zone)
 
         raise ResourceNotFoundError
 
-    ### Network Load Balancer
+    # Network Load Balancer
 
     def create_network_load_balancer(self, zone, name, description=""):
         """
         Create a Network Load Balancer.
 
         Parameters:
             zone (Zone): the zone in which to create the Network Load Balancer
@@ -3192,28 +3287,40 @@
         """
 
         if id is None and name is None:
             raise ValueError("either id or name must be specifed")
 
         if id:
             res = self._v2_request("GET", "/load-balancer/" + id, zone.name)
-            return NetworkLoadBalancer._from_api(compute=self, res=res, zone=zone)
+            return NetworkLoadBalancer._from_api(
+                compute=self, res=res, zone=zone
+            )
 
         _list = self._v2_request("GET", "/load-balancer", zone.name)
         for i in _list["load-balancers"]:
             if i["name"] == name:
-                res = self._v2_request("GET", "/load-balancer/" + i["id"], zone.name)
-                return NetworkLoadBalancer._from_api(compute=self, res=res, zone=zone)
+                res = self._v2_request(
+                    "GET", "/load-balancer/" + i["id"], zone.name
+                )
+                return NetworkLoadBalancer._from_api(
+                    compute=self, res=res, zone=zone
+                )
 
         raise ResourceNotFoundError
 
-    ### Private Network
+    # Private Network
 
     def create_private_network(
-        self, zone, name, description="", start_ip=None, end_ip=None, netmask=None
+        self,
+        zone,
+        name,
+        description="",
+        start_ip=None,
+        end_ip=None,
+        netmask=None,
     ):
         """
         Create a Private Network.
 
         Parameters:
             zone (Zone): the zone in which to create the Private Network
             name (str): the Private Network name
@@ -3250,15 +3357,17 @@
             zone (Zone): the zone to list in
 
         Yields:
             PrivateNetwork: the next Private Network
         """
 
         try:
-            _list = self.cs.listNetworks(fetch_list=True, zoneid=zone.id, **kwargs)
+            _list = self.cs.listNetworks(
+                fetch_list=True, zoneid=zone.id, **kwargs
+            )
 
             for i in _list:
                 yield PrivateNetwork._from_cs(self, i, zone=zone)
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
     def get_private_network(self, zone, id):
@@ -3281,30 +3390,32 @@
             raise
 
         if len(private_networks) == 0:
             raise ResourceNotFoundError
 
         return private_networks[0]
 
-    ### Security Group
+    # Security Group
 
     def create_security_group(self, name, description=""):
         """
         Create a Security Group.
 
         Parameters:
             name (str): the Security group name
             description (str): the Security Group description
 
         Returns:
             SecurityGroup: the Security Group created
         """
 
         try:
-            res = self.cs.createSecurityGroup(name=name, description=description)
+            res = self.cs.createSecurityGroup(
+                name=name, description=description
+            )
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         return SecurityGroup._from_cs(self, res["securitygroup"])
 
     def list_security_groups(self, **kwargs):
         """
@@ -3347,15 +3458,15 @@
             raise
 
         if len(security_groups) == 0:
             raise ResourceNotFoundError
 
         return security_groups[0]
 
-    ### SSH Key
+    # SSH Key
 
     def create_ssh_key(self, name):
         """
         Create an SSH key.
 
         Parameters:
             name (str): the SSH key unique name
@@ -3425,15 +3536,15 @@
             raise
 
         if len(ssh_keys) == 0:
             raise ResourceNotFoundError
 
         return ssh_keys[0]
 
-    ### Zone
+    # Zone
 
     def list_zones(self, **kwargs):
         """
         List zones.
 
         Yields:
             Zone: the next zone
@@ -3470,15 +3581,15 @@
             raise
 
         if len(zones) == 0:
             raise ResourceNotFoundError
 
         return zones[0]
 
-    ### V2 API
+    # V2 API
 
     def _v2_check_response(self, res, *args, **kwargs):
         """
         Check the API response and raise an exception depending on the status code.
         """
 
         if res.status_code >= 500:
@@ -3489,15 +3600,17 @@
 
         if res.status_code >= 400:
             raise RequestError(str(res.text))
 
     def _v2_request(self, method, path, zone=None, **kwargs):
         base_url = "https://api.exoscale/v2"
         if zone:
-            base_url = "https://{}-{}.exoscale.com/v2".format(self.environment, zone)
+            base_url = "https://{}-{}.exoscale.com/v2".format(
+                self.environment, zone
+            )
 
         return API.send(
             self,
             method=method,
             url="/".join((base_url, path.lstrip("/"))),
             auth=ExoscaleV2Auth(self.key, self.secret),
             hooks={"response": self._v2_check_response},
```

### Comparing `exoscale-0.7.1/exoscale/api/dns.py` & `exoscale-0.8.0/exoscale/api/dns.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
 This submodule represents the Exoscale DNS API.
 """
 
-import attr
 from . import API, Resource, APIException, ResourceNotFoundError
+from attr import define, field
 from cs import CloudStack, CloudStackApiException
 
 _SUPPORTED_RECORD_TYPES = {
     "A",
     "AAAA",
     "ALIAS",
     "CAA",
@@ -27,34 +27,38 @@
     "SRV",
     "SSHFP",
     "TXT",
     "URL",
 }
 
 
-@attr.s
+@define
 class Domain(Resource):
     """
     A DNS domain.
 
     Attributes:
         id (int): the DNS domain unique identifier
         name (str): the DNS domain name
     """
 
-    dns = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    name = attr.ib()
-    unicode_name = attr.ib(repr=False)
+    dns = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    name = field()
+    unicode_name = field(repr=False)
 
     @classmethod
     def _from_cs(cls, dns, res):
         return cls(
-            dns, res, id=res["id"], name=res["name"], unicode_name=res["unicodename"]
+            dns,
+            res,
+            id=res["id"],
+            name=res["name"],
+            unicode_name=res["unicodename"],
         )
 
     @property
     def records(self):
         """
         Domain records.
 
@@ -63,15 +67,17 @@
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
         try:
-            _list = self.dns.cs.listDnsDomainRecords(id=self.id, fetch_list=True)
+            _list = self.dns.cs.listDnsDomainRecords(
+                id=self.id, fetch_list=True
+            )
             for i in _list:
                 yield DomainRecord._from_cs(self.dns, domain=self, res=i)
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
     def add_record(self, name, type, content, priority=None, ttl=3600):
         """
@@ -121,38 +127,38 @@
             self.dns.cs.deleteDnsDomain(id=self.id)
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         self._reset()
 
 
-@attr.s
+@define
 class DomainRecord(Resource):
     """
     A DNS domain record.
 
     Attributes:
         id (int): the DNS domain record unique identifier
         domain (Domain): the DNS domain the record belongs to
         type (str): the DNS domain record type
         name (str): the DNS domain record name
         content (str): the DNS domain record content
         priority (int): the DNS domain record priority
         ttl (int): the DNS domain record TTL
     """
 
-    dns = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    domain = attr.ib(repr=False)
-    type = attr.ib()
-    name = attr.ib(repr=False)
-    content = attr.ib(repr=False)
-    priority = attr.ib(default=None, repr=False)
-    ttl = attr.ib(default=3600, repr=False)
+    dns = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    domain = field(repr=False)
+    type = field()
+    name = field(repr=False)
+    content = field(repr=False)
+    priority = field(default=None, repr=False)
+    ttl = field(default=3600, repr=False)
 
     @classmethod
     def _from_cs(cls, dns, res, domain):
         return cls(
             dns,
             res,
             domain=domain,
@@ -201,15 +207,17 @@
         Delete the DNS domain record.
 
         Returns:
             None
         """
 
         try:
-            self.dns.cs.deleteDnsDomainRecord(id=self.domain.id, record_id=self.id)
+            self.dns.cs.deleteDnsDomainRecord(
+                id=self.domain.id, record_id=self.id
+            )
         except CloudStackApiException as e:
             raise APIException(e.error["errortext"], e.error)
 
         self._reset()
 
 
 class DnsAPI(API):
@@ -241,26 +249,29 @@
         )
 
         self.cs = CloudStack(
             key=key,
             secret=secret,
             endpoint=endpoint,
             session=self.session,
-            headers={**self.session.headers, **{"User-Agent": self.user_agent}},
+            headers={
+                **self.session.headers,
+                **{"User-Agent": self.user_agent},
+            },
             trace=self.trace,
             fetch_result=True,
         )
 
     def __repr__(self):
         return "DnsAPI(endpoint='{}' key='{}')".format(self.endpoint, self.key)
 
     def __str__(self):
         return self.__repr__()
 
-    ### Domain
+    # Domain
 
     def create_domain(self, name):
         """
         Create a DNS domain.
 
         Parameters:
             name (str): the domain name
```

### Comparing `exoscale-0.7.1/exoscale/api/iam.py` & `exoscale-0.8.0/exoscale/api/iam.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # -*- coding: utf-8 -*-
 
 """
 This submodule represents the Exoscale IAM API.
 """
 
-import attr
 from . import API, Resource, APIException, ResourceNotFoundError
+from attr import define, field
 from cs import CloudStack, CloudStackApiException
 
 
-@attr.s
+@define
 class APIKey(Resource):
     """
     An API key.
 
     Attributes:
         name (str): the API key display name
         key (str): the API key unique identifier
         type (str): the API key type
         secret (str): the API key secret
         operations ([str]): a list of allowed API operations
     """
 
-    iam = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    name = attr.ib()
-    key = attr.ib()
-    type = attr.ib()
-    secret = attr.ib(repr=False)
-    operations = attr.ib(repr=False)
+    iam = field(repr=False)
+    res = field(repr=False)
+    name = field()
+    key = field()
+    type = field()
+    secret = field(repr=False)
+    operations = field(repr=False)
 
     @classmethod
     def _from_cs(cls, iam, res):
         return cls(
             iam,
             res,
             name=res["name"],
@@ -87,26 +87,29 @@
         )
 
         self.cs = CloudStack(
             key=key,
             secret=secret,
             endpoint=endpoint,
             session=self.session,
-            headers={**self.session.headers, **{"User-Agent": self.user_agent}},
+            headers={
+                **self.session.headers,
+                **{"User-Agent": self.user_agent},
+            },
             trace=self.trace,
             fetch_result=True,
         )
 
     def __repr__(self):
         return "IamAPI(endpoint='{}' key='{}')".format(self.endpoint, self.key)
 
     def __str__(self):
         return self.__repr__()
 
-    ### API key
+    # API key
 
     def create_api_key(self, name, operations=None):
         """
         Create an API key.
 
         Parameters:
             name (str): the API key name
```

### Comparing `exoscale-0.7.1/exoscale/api/polling.py` & `exoscale-0.8.0/exoscale/api/polling.py`

 * *Files identical despite different names*

### Comparing `exoscale-0.7.1/exoscale/api/runstatus.py` & `exoscale-0.8.0/exoscale/api/runstatus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # -*- coding: utf-8 -*-
 
 """
 This submodule represents the Exoscale Runstatus API.
 """
 
-import attr
 from datetime import datetime
 from exoscale_auth import ExoscaleAuth
 from . import API, Resource, APIException, RequestError, ResourceNotFoundError
+from attr import define, field
 
-_SUPPORTED_INCIDENT_STATES = {"major_outage", "partial_outage", "degraded_performance"}
+_SUPPORTED_INCIDENT_STATES = {
+    "major_outage",
+    "partial_outage",
+    "degraded_performance",
+}
 _SUPPORTED_INCIDENT_STATUSES = {"investigating", "identified", "monitoring"}
 _SUPPORTED_MAINTENANCE_STATUSES = {"scheduled", "in-progress"}
 
 
 def rstime_to_datetime(rstime):
     """
     Parses a Runstatus API timestamp and returns the corresponding datetime object.
@@ -21,35 +25,39 @@
 
     try:
         return datetime.strptime(rstime, "%Y-%m-%dT%H:%M:%S.%fZ")
     except ValueError:
         return datetime.strptime(rstime, "%Y-%m-%dT%H:%M:%SZ")
 
 
-@attr.s
+@define
 class Service(Resource):
     """
     A Runstatus service.
 
     Attributes:
         id (int): the service unique identifier
         name (str): the service name
         page (Page): the page the incident belongs to
     """
 
-    runstatus = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    name = attr.ib()
-    page = attr.ib(repr=False)
+    runstatus = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    name = field()
+    page = field(repr=False)
 
     @classmethod
     def _from_rs(cls, runstatus, res, page):
         return cls(
-            runstatus, res, id=res["url"].split("/")[-1], name=res["name"], page=page
+            runstatus,
+            res,
+            id=res["url"].split("/")[-1],
+            name=res["name"],
+            page=page,
         )
 
     @property
     def state(self):
         """
         Service state.
 
@@ -85,37 +93,37 @@
         self.runstatus = None
         self.res = None
         self.id = None
         self.name = None
         self.page = None
 
 
-@attr.s
+@define
 class IncidentEvent(Resource):
     """
     A Runstatus incident event.
 
     Attributes:
         date (datetime.datetime): the event date
         description (str): the event description
         status (str): the target status for the incident
         state (str): the target state for the services impacted
         incident (Incident): the incident the event belongs to
     """
 
-    runstatus = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    date = attr.ib(repr=False)
-    description = attr.ib(repr=False)
-    status = attr.ib(repr=False)
-    state = attr.ib(repr=False)
-    incident = attr.ib(repr=False)
+    runstatus = field(repr=False)
+    res = field(repr=False)
+    date = field(repr=False)
+    description = field(repr=False)
+    status = field(repr=False)
+    state = field(repr=False)
+    incident = field(repr=False)
 
 
-@attr.s
+@define
 class Incident(Resource):
     """
     A Runstatus incident.
 
     Attributes:
         id (int): the incident unique identifier
         title (str): a incident title
@@ -123,24 +131,24 @@
         end_date (datetime.datetime): the incident end date
         services ([str]): a list of services impacted by the incident
         state (str): the incident state
         status (str): the incident status
         page (Page): the page the incident belongs to
     """
 
-    runstatus = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    page = attr.ib(repr=False)
-    state = attr.ib(repr=False)
-    status = attr.ib(repr=False)
-    start_date = attr.ib(repr=False)
-    end_date = attr.ib(default=None, repr=False)
-    title = attr.ib(default=None, repr=False)
-    services = attr.ib(default=None, repr=False)
+    runstatus = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    page = field(repr=False)
+    state = field(repr=False)
+    status = field(repr=False)
+    start_date = field(repr=False)
+    end_date = field(default=None, repr=False)
+    title = field(default=None, repr=False)
+    services = field(default=None, repr=False)
 
     @classmethod
     def _from_rs(cls, runstatus, res, page):
         return cls(
             runstatus,
             res,
             id=res["id"],
@@ -165,15 +173,17 @@
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
         res = self.runstatus._get(
-            url="/pages/{p}/incidents/{i}/events".format(p=self.page.name, i=self.id)
+            url="/pages/{p}/incidents/{i}/events".format(
+                p=self.page.name, i=self.id
+            )
         )
 
         for i in res.json().get("results", []):
             yield IncidentEvent(
                 self.runstatus,
                 i,
                 date=rstime_to_datetime(i["created"]),
@@ -207,15 +217,17 @@
             raise ValueError(
                 "unsupported status; supported statuses are: {}".format(
                     ",".join(_SUPPORTED_INCIDENT_STATUSES)
                 )
             )
 
         self.runstatus._post(
-            url="/pages/{p}/incidents/{i}/events".format(p=self.page.name, i=self.id),
+            url="/pages/{p}/incidents/{i}/events".format(
+                p=self.page.name, i=self.id
+            ),
             json={
                 "text": description,
                 "status": status if status is not None else self.status,
                 "state": state if state is not None else self.state,
             },
         )
 
@@ -258,40 +270,46 @@
             description (str): the incident closing description
 
         Returns:
             None
         """
 
         self.runstatus._post(
-            url="/pages/{p}/incidents/{i}/events".format(p=self.page.name, i=self.id),
-            json={"text": description, "status": "resolved", "state": "operational"},
+            url="/pages/{p}/incidents/{i}/events".format(
+                p=self.page.name, i=self.id
+            ),
+            json={
+                "text": description,
+                "status": "resolved",
+                "state": "operational",
+            },
         )
 
 
-@attr.s
+@define
 class MaintenanceEvent(Resource):
     """
     A Runstatus maintenance event.
 
     Attributes:
         date (datetime.datetime): the event date
         description (str): the event description
         status (str): the target status for the maintenance
         maintenance (Maintenance): the maintenance the event belongs to
     """
 
-    runstatus = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    date = attr.ib(repr=False)
-    description = attr.ib(repr=False)
-    status = attr.ib(repr=False)
-    maintenance = attr.ib(repr=False)
+    runstatus = field(repr=False)
+    res = field(repr=False)
+    date = field(repr=False)
+    description = field(repr=False)
+    status = field(repr=False)
+    maintenance = field(repr=False)
 
 
-@attr.s
+@define
 class Maintenance(Resource):
     """
     A Runstatus maintenance.
 
     Attributes:
         id (int): the maintenance unique identifier
         title (str): a maintenance title
@@ -299,24 +317,24 @@
         services ([str]): a list of services impacted by the maintenance
         start_date (datetime.datetime): a maintenance start date
         end_date (datetime.datetime): a maintenance end date
         status (str): the maintenance status
         page (Page): the page the maintenance belongs to
     """
 
-    runstatus = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    page = attr.ib(repr=False)
-    status = attr.ib(repr=False)
-    start_date = attr.ib(repr=False)
-    end_date = attr.ib(repr=False)
-    title = attr.ib(default=None, repr=False)
-    description = attr.ib(default=None, repr=False)
-    services = attr.ib(default=None, repr=False)
+    runstatus = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    page = field(repr=False)
+    status = field(repr=False)
+    start_date = field(repr=False)
+    end_date = field(repr=False)
+    title = field(default=None, repr=False)
+    description = field(default=None, repr=False)
+    services = field(default=None, repr=False)
 
     @classmethod
     def _from_rs(cls, runstatus, res, page):
         return cls(
             runstatus,
             res,
             id=res["id"],
@@ -339,15 +357,17 @@
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
         res = self.runstatus._get(
-            url="/pages/{p}/maintenances/{m}/events".format(p=self.page.name, m=self.id)
+            url="/pages/{p}/maintenances/{m}/events".format(
+                p=self.page.name, m=self.id
+            )
         )
 
         for i in res.json().get("results", []):
             yield MaintenanceEvent(
                 self.runstatus,
                 i,
                 date=rstime_to_datetime(i["created"]),
@@ -364,15 +384,18 @@
             description (str): the event description
             status (str): a new maintenance status to set
 
         Returns:
             None
         """
 
-        if status is not None and status not in _SUPPORTED_MAINTENANCE_STATUSES:
+        if (
+            status is not None
+            and status not in _SUPPORTED_MAINTENANCE_STATUSES
+        ):
             raise ValueError(
                 "unsupported status; supported statuses are: {}".format(
                     ",".join(_SUPPORTED_MAINTENANCE_STATUSES)
                 )
             )
 
         self.runstatus._post(
@@ -418,15 +441,17 @@
             json["services"] = services
         if start_date is not None:
             json["start_date"] = start_date.isoformat()
         if end_date is not None:
             json["end_date"] = end_date.isoformat()
 
         self.runstatus._patch(
-            url="/pages/{p}/maintenances/{i}".format(p=self.page.name, i=self.id),
+            url="/pages/{p}/maintenances/{i}".format(
+                p=self.page.name, i=self.id
+            ),
             json=json,
         )
 
         if title is not None:
             self.title = title
         if description is not None:
             self.description = description
@@ -452,15 +477,15 @@
             url="/pages/{p}/maintenances/{m}/events".format(
                 p=self.page.name, m=self.id
             ),
             json={"text": description, "status": "completed"},
         )
 
 
-@attr.s
+@define
 class Page(Resource):
     """
     A Runstatus page.
 
     Attributes:
         id (int): the page unique identifier
         name (str): the page name
@@ -470,22 +495,22 @@
         time_zone (str): a time zone
 
     Note:
         The expected time zone format is the tz database (a.k.a "tzdata" or "Olson"
         database): https://en.wikipedia.org/wiki/Tz_database
     """
 
-    runstatus = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    id = attr.ib()
-    name = attr.ib()
-    title = attr.ib(default=None, repr=False)
-    default_status_message = attr.ib(default=None, repr=False)
-    custom_domain = attr.ib(default=None, repr=False)
-    time_zone = attr.ib(default=None, repr=False)
+    runstatus = field(repr=False)
+    res = field(repr=False)
+    id = field()
+    name = field()
+    title = field(default=None, repr=False)
+    default_status_message = field(default=None, repr=False)
+    custom_domain = field(default=None, repr=False)
+    time_zone = field(default=None, repr=False)
 
     @classmethod
     def _from_rs(cls, runstatus, res):
         return cls(runstatus, res, id=res["id"], name=res["subdomain"])
 
     @property
     def services(self):
@@ -496,15 +521,17 @@
             Service: the next service
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
-        res = self.runstatus._get(url="/pages/{p}/services".format(p=self.name))
+        res = self.runstatus._get(
+            url="/pages/{p}/services".format(p=self.name)
+        )
 
         for i in res.json().get("results", []):
             yield Service._from_rs(self.runstatus, i, page=self)
 
     def add_service(self, name):
         """
         Add a service to the page.
@@ -529,15 +556,17 @@
             Incident: the next incident
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
-        res = self.runstatus._get(url="/pages/{p}/incidents".format(p=self.name))
+        res = self.runstatus._get(
+            url="/pages/{p}/incidents".format(p=self.name)
+        )
 
         for i in res.json().get("results", []):
             yield Incident._from_rs(self.runstatus, i, self)
 
     def add_incident(self, title, description, state, status, services=None):
         """
         Open a new incident.
@@ -590,20 +619,24 @@
             Maintenance: the next maintenance
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
-        res = self.runstatus._get(url="/pages/{p}/maintenances".format(p=self.name))
+        res = self.runstatus._get(
+            url="/pages/{p}/maintenances".format(p=self.name)
+        )
 
         for i in res.json().get("results", []):
             yield Maintenance._from_rs(self.runstatus, i, self)
 
-    def add_maintenance(self, title, description, start_date, end_date, services=None):
+    def add_maintenance(
+        self, title, description, start_date, end_date, services=None
+    ):
         """
         Open a new maintenance.
 
         Parameters:
             title (str): the maintenance title
             description (str): the maintenance description
             start_date (datetime.datetime): the maintenance start date
@@ -716,15 +749,17 @@
             max_retries=max_retries,
             trace=trace,
         )
 
         self.auth = ExoscaleAuth(self.key, self.secret)
 
     def __repr__(self):
-        return "RunstatusAPI(endpoint='{}' key='{}')".format(self.endpoint, self.key)
+        return "RunstatusAPI(endpoint='{}' key='{}')".format(
+            self.endpoint, self.key
+        )
 
     def __str__(self):
         return self.__repr__()
 
     def _check_api_response(self, res, *args, **kwargs):
         """
         Check the API response and raise an exception depending on the status code.
@@ -747,15 +782,18 @@
             kwargs: request.Request parameters
 
         Returns:
             request.Response: the HTTP response
         """
 
         return API.send(
-            self, auth=self.auth, hooks={"response": self._check_api_response}, **kwargs
+            self,
+            auth=self.auth,
+            hooks={"response": self._check_api_response},
+            **kwargs,
         )
 
     def _get(self, url, **kwargs):
         """
         Send an HTTP GET request to the Runstatus API.
 
         Parameters:
@@ -783,15 +821,15 @@
             request.Response: the HTTP response received from the Runstatus API
         """
 
         return self._send(
             method="POST",
             url=self.endpoint + "/" + url.lstrip("/"),
             json=json,
-            **kwargs
+            **kwargs,
         )
 
     def _patch(self, url, json, **kwargs):
         """
         Send an HTTP PATCH request to the Runstatus API.
 
         Parameters:
@@ -803,15 +841,15 @@
             request.Response: the HTTP response received from the Runstatus API
         """
 
         return self._send(
             method="PATCH",
             url=self.endpoint + "/" + url.lstrip("/"),
             json=json,
-            **kwargs
+            **kwargs,
         )
 
     def _delete(self, url, **kwargs):
         """
         Send an HTTP DELETE request to the Runstatus API.
 
         Parameters:
@@ -819,18 +857,20 @@
             kwargs: request.Request parameters
 
         Returns:
             request.Response: the HTTP response received from the Runstatus API
         """
 
         return self._send(
-            method="DELETE", url=self.endpoint + "/" + url.lstrip("/"), **kwargs
+            method="DELETE",
+            url=self.endpoint + "/" + url.lstrip("/"),
+            **kwargs,
         )
 
-    ## Page
+    # Page
 
     def create_page(self, name):
         """
         Create a Runstatus page.
 
         Parameters:
             name (str): the page name
```

### Comparing `exoscale-0.7.1/exoscale/api/storage.py` & `exoscale-0.8.0/exoscale/api/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 # -*- coding: utf-8 -*-
 
 """
 This submodule represents the Exoscale Storage API.
 """
 
-import attr
 import boto3
 import botocore
 import logging
 from . import API, Resource, APIException, ResourceNotFoundError
+from attr import define, field
 from os.path import basename
 
 _DEFAULT_ZONE = "ch-gva-2"
 
 _SUPPORTED_CANNED_ACLS = {
     "private",
     "public-read",
     "public-read-write",
     "authenticated-read",
     "bucket-owner-read",
     "bucket-owner-full-control",
 }
 
 ACL_ALL_USERS = "http://acs.amazonaws.com/groups/global/AllUsers"
-ACL_AUTHENTICATED_USERS = "http://acs.amazonaws.com/groups/global/AuthenticatedUsers"
+ACL_AUTHENTICATED_USERS = (
+    "http://acs.amazonaws.com/groups/global/AuthenticatedUsers"
+)
 
 
-@attr.s
+@define
 class CORSRule(Resource):
     """
     A Storage bucket CORS rule.
 
     Attributes:
         allowed_headers ([str]): list of allowed HTTP headers
         allowed_methods ([str]): list of allowed HTTP methods
         allowed_origins ([str]): list of allowed HTTP origins
         expose_headers ([str]): list of HTTP headers allowed to be exposed in response
         max_age_seconds (int): time in seconds that a browser can cache OPTIONS reponse
     """
 
-    res = attr.ib(repr=False)
-    allowed_headers = attr.ib(default=None, repr=False)
-    allowed_methods = attr.ib(default=None, repr=False)
-    allowed_origins = attr.ib(default=None, repr=False)
-    expose_headers = attr.ib(default=None, repr=False)
-    max_age_seconds = attr.ib(default=None, repr=False)
+    res = field(repr=False)
+    allowed_headers = field(default=None, repr=False)
+    allowed_methods = field(default=None, repr=False)
+    allowed_origins = field(default=None, repr=False)
+    expose_headers = field(default=None, repr=False)
+    max_age_seconds = field(default=None, repr=False)
 
     @classmethod
     def _from_s3(cls, res):
         return cls(
             res,
             allowed_headers=res["AllowedHeaders"],
             allowed_methods=res["AllowedMethods"],
@@ -78,35 +80,35 @@
 
         if self.max_age_seconds is not None:
             cors_rule["MaxAgeSeconds"] = self.max_age_seconds
 
         return cors_rule
 
 
-@attr.s
+@define
 class AccessControlPolicy(Resource):
     """
     A Storage Access Control Policy.
 
     Attributes:
         owner (str): entity owner of the resource
         full_control (str): full control grant
         read (str): read permission grant
         write (str): write permission grant
         read_acp (str): Access Control Policy read permission grant
         write_acp (str): Access Control Policy write permission grant
     """
 
-    res = attr.ib(repr=False)
-    owner = attr.ib()
-    full_control = attr.ib(default=None, repr=False)
-    read = attr.ib(default=None, repr=False)
-    write = attr.ib(default=None, repr=False)
-    read_acp = attr.ib(default=None, repr=False)
-    write_acp = attr.ib(default=None, repr=False)
+    res = field(repr=False)
+    owner = field()
+    full_control = field(default=None, repr=False)
+    read = field(default=None, repr=False)
+    write = field(default=None, repr=False)
+    read_acp = field(default=None, repr=False)
+    write_acp = field(default=None, repr=False)
 
     @classmethod
     def _from_s3(cls, res):
         acp = cls(res, owner=res["Owner"]["DisplayName"])
 
         for i in res["Grants"]:
             if i["Permission"] == "FULL_CONTROL":
@@ -129,30 +131,39 @@
 
         References:
             * `boto3 AccessControlPolicy format`_
 
             .. _boto3 AccessControlPolicy format: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_acl
         """
 
-        acp = {"Owner": {"ID": self.owner, "DisplayName": self.owner}, "Grants": []}
+        acp = {
+            "Owner": {"ID": self.owner, "DisplayName": self.owner},
+            "Grants": [],
+        }
 
         if self.full_control is not None:
             acp["Grants"].append(
                 {
                     "Grantee": self._grantee_to_s3(self.full_control),
                     "Permission": "FULL_CONTROL",
                 }
             )
         if self.read is not None:
             acp["Grants"].append(
-                {"Grantee": self._grantee_to_s3(self.read), "Permission": "READ"}
+                {
+                    "Grantee": self._grantee_to_s3(self.read),
+                    "Permission": "READ",
+                }
             )
         if self.write is not None:
             acp["Grants"].append(
-                {"Grantee": self._grantee_to_s3(self.write), "Permission": "WRITE"}
+                {
+                    "Grantee": self._grantee_to_s3(self.write),
+                    "Permission": "WRITE",
+                }
             )
         if self.read_acp is not None:
             acp["Grants"].append(
                 {
                     "Grantee": self._grantee_to_s3(self.read_acp),
                     "Permission": "READ_ACP",
                 }
@@ -197,31 +208,35 @@
         if grantee in {"ALL_USERS", "AUTHENTICATED_USERS"}:
             if grantee == "ALL_USERS":
                 uri = ACL_ALL_USERS
             else:
                 uri = ACL_AUTHENTICATED_USERS
             return {"Type": "Group", "URI": uri}
         else:
-            return {"Type": "CanonicalUser", "ID": grantee, "DisplayName": grantee}
+            return {
+                "Type": "CanonicalUser",
+                "ID": grantee,
+                "DisplayName": grantee,
+            }
 
 
-@attr.s
+@define
 class BucketFile(Resource):
     """
     A file stored in Storage bucket.
 
     Attributes:
         path (str): the stored file path
         bucket (Bucket): the bucket the file is stored into
     """
 
-    storage = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    path = attr.ib()
-    bucket = attr.ib(repr=False)
+    storage = field(repr=False)
+    res = field(repr=False)
+    path = field()
+    bucket = field(repr=False)
 
     @property
     def content(self):
         """
         Stored file content.
 
         Returns:
@@ -240,15 +255,17 @@
         References:
             * `botocore.response API`_
 
             .. _botocore.response API: https://botocore.amazonaws.com/v1/documentation/api/latest/reference/response.html
         """
 
         try:
-            res = self.storage.boto.get_object(Bucket=self.bucket.name, Key=self.path)
+            res = self.storage.boto.get_object(
+                Bucket=self.bucket.name, Key=self.path
+            )
         except Exception as e:
             raise APIException(e)
 
         return res["Body"]
 
     @property
     def size(self):
@@ -263,15 +280,17 @@
             latency.
         """
 
         if "Size" in self.res:
             return self.res["Size"]
 
         try:
-            res = self.storage.boto.get_object(Bucket=self.bucket.name, Key=self.path)
+            res = self.storage.boto.get_object(
+                Bucket=self.bucket.name, Key=self.path
+            )
         except Exception as e:
             raise APIException(e)
 
         return res["ContentLength"]
 
     @property
     def last_modification_date(self):
@@ -291,15 +310,17 @@
             .. _Python datetime module: https://docs.python.org/3/library/datetime.html
         """
 
         if "LastModified" in self.res:
             return self.res["LastModified"]
 
         try:
-            res = self.storage.boto.get_object(Bucket=self.bucket.name, Key=self.path)
+            res = self.storage.boto.get_object(
+                Bucket=self.bucket.name, Key=self.path
+            )
         except Exception as e:
             raise APIException(e)
 
         return res["LastModified"]
 
     @property
     def acl(self):
@@ -334,15 +355,17 @@
 
         Note:
             This property value is dynamically retrieved from the API, incurring extra
             latency.
         """
 
         try:
-            res = self.storage.boto.get_object(Bucket=self.bucket.name, Key=self.path)
+            res = self.storage.boto.get_object(
+                Bucket=self.bucket.name, Key=self.path
+            )
         except Exception as e:
             raise APIException(e)
 
         return res["Metadata"]
 
     @property
     def url(self):
@@ -400,33 +423,35 @@
         Delete the stored file.
 
         Returns:
             None
         """
 
         try:
-            self.storage.boto.delete_object(Bucket=self.bucket.name, Key=self.path)
+            self.storage.boto.delete_object(
+                Bucket=self.bucket.name, Key=self.path
+            )
         except Exception as e:
             raise APIException(e)
 
         self._reset()
 
 
-@attr.s
+@define
 class Bucket(Resource):
     """
     A Storage bucket.
 
     Attributes:
         name (str): the Storage bucket name
     """
 
-    storage = attr.ib(repr=False)
-    res = attr.ib(repr=False)
-    name = attr.ib()
+    storage = field(repr=False)
+    res = field(repr=False)
+    name = field()
 
     @property
     def acl(self):
         """
         Storage bucket Access Control List.
 
         Returns:
@@ -498,15 +523,17 @@
             latency.
         """
 
         return "https://sos-{zone}.exo.io/{bucket}".format(
             zone=self.zone, bucket=self.name
         )
 
-    def put_file(self, src, dst=None, metadata=None, acl=None, transferConfig=None):
+    def put_file(
+        self, src, dst=None, metadata=None, acl=None, transferConfig=None
+    ):
         """
         Store a file in the bucket.
 
         Parameters:
             src (str): the path to the source file
             dst (str): a path to which to store the file in the bucket
             metadata (dict): a dict of metadata to set to the file
@@ -556,15 +583,17 @@
         Yields:
             BucketFile: the next file stored in the bucket
         """
 
         try:
             paginator = self.storage.boto.get_paginator("list_objects_v2")
             pages = paginator.paginate(
-                Bucket=self.name, Prefix=prefix, PaginationConfig={"PageSize": 100}
+                Bucket=self.name,
+                Prefix=prefix,
+                PaginationConfig={"PageSize": 100},
             )
             for page in pages:
                 for i in page["Contents"]:
                     yield BucketFile(self.storage, i, i["Key"], self)
         except Exception as e:
             raise APIException(e)
 
@@ -672,29 +701,31 @@
         Returns:
             None
         """
 
         try:
             self.storage.boto.put_bucket_cors(
                 Bucket=self.name,
-                CORSConfiguration={"CORSRules": list(r._to_s3() for r in rules)},
+                CORSConfiguration={
+                    "CORSRules": list(r._to_s3() for r in rules)
+                },
             )
         except Exception as e:
             raise APIException(e)
 
     def delete(self):
         """
         Delete the Storage bucket.
 
         Returns:
             None
         """
 
         try:
-            res = self.storage.boto.delete_bucket(Bucket=self.name)
+            self.storage.boto.delete_bucket(Bucket=self.name)
         except Exception as e:
             raise APIException(e)
 
         self._reset()
 
 
 class StorageAPI(API):
@@ -707,19 +738,27 @@
         endpoint (str): the Storage API endpoint
         zone (str): the Storage zone
         max_retries (int): the API HTTP session retry policy number of retries to allow
         trace (bool): API request/response tracing flag
     """
 
     def __init__(
-        self, key, secret, endpoint=None, zone=None, max_retries=None, trace=False
+        self,
+        key,
+        secret,
+        endpoint=None,
+        zone=None,
+        max_retries=None,
+        trace=False,
     ):
         self.zone = _DEFAULT_ZONE if zone is None else zone
         endpoint = (
-            "https://sos-{}.exo.io".format(self.zone) if endpoint is None else endpoint
+            "https://sos-{}.exo.io".format(self.zone)
+            if endpoint is None
+            else endpoint
         )
         max_retries = 3 if max_retries is None else max_retries
         super().__init__(
             endpoint=endpoint,
             key=key,
             secret=secret,
             max_retries=max_retries,
```

