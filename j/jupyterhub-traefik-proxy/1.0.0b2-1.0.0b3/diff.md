# Comparing `tmp/jupyterhub-traefik-proxy-1.0.0b2.tar.gz` & `tmp/jupyterhub-traefik-proxy-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-traefik-proxy-1.0.0b2.tar", last modified: Tue Mar 28 14:49:04 2023, max compression
+gzip compressed data, was "jupyterhub-traefik-proxy-1.0.0b3.tar", last modified: Thu May 11 14:36:38 2023, max compression
```

## Comparing `jupyterhub-traefik-proxy-1.0.0b2.tar` & `jupyterhub-traefik-proxy-1.0.0b3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 14:49:04.171429 jupyterhub-traefik-proxy-1.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-03-28 14:48:54.000000 jupyterhub-traefik-proxy-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-03-28 14:48:54.000000 jupyterhub-traefik-proxy-1.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-03-28 14:49:04.171429 jupyterhub-traefik-proxy-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2585 2023-03-28 14:48:54.000000 jupyterhub-traefik-proxy-1.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 14:49:04.171429 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-03-28 14:48:54.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5493 2023-03-28 14:48:54.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/consul.py
--rw-r--r--   0 runner    (1001) docker     (122)     6778 2023-03-28 14:48:54.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/etcd.py
--rw-r--r--   0 runner    (1001) docker     (122)     6967 2023-03-28 14:48:54.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/fileprovider.py
--rw-r--r--   0 runner    (1001) docker     (122)     5533 2023-03-28 14:48:54.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/install.py
--rw-r--r--   0 runner    (1001) docker     (122)    11459 2023-03-28 14:48:54.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/kv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)    25044 2023-03-28 14:48:54.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-03-28 14:48:54.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/toml.py
--rw-r--r--   0 runner    (1001) docker     (122)     3917 2023-03-28 14:48:54.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/traefik_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 14:49:04.171429 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-03-28 14:49:04.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-03-28 14:49:04.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 14:49:04.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-03-28 14:49:04.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-03-28 14:49:04.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-03-28 14:49:04.000000 jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 14:49:04.171429 jupyterhub-traefik-proxy-1.0.0b2/performance/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 14:48:55.000000 jupyterhub-traefik-proxy-1.0.0b2/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10504 2023-03-28 14:48:55.000000 jupyterhub-traefik-proxy-1.0.0b2/performance/check_perf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-03-28 14:48:55.000000 jupyterhub-traefik-proxy-1.0.0b2/performance/dummy_http_server.py
--rw-r--r--   0 runner    (1001) docker     (122)    10061 2023-03-28 14:48:55.000000 jupyterhub-traefik-proxy-1.0.0b2/performance/perf_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-03-28 14:48:55.000000 jupyterhub-traefik-proxy-1.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-03-28 14:49:04.175428 jupyterhub-traefik-proxy-1.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-03-28 14:48:55.000000 jupyterhub-traefik-proxy-1.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 14:49:04.171429 jupyterhub-traefik-proxy-1.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-03-28 14:48:55.000000 jupyterhub-traefik-proxy-1.0.0b2/tests/test_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-03-28 14:48:55.000000 jupyterhub-traefik-proxy-1.0.0b2/tests/test_installer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2313 2023-03-28 14:48:55.000000 jupyterhub-traefik-proxy-1.0.0b2/tests/test_kv.py
--rw-r--r--   0 runner    (1001) docker     (122)    14673 2023-03-28 14:48:55.000000 jupyterhub-traefik-proxy-1.0.0b2/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-03-28 14:48:55.000000 jupyterhub-traefik-proxy-1.0.0b2/tests/test_traefik_api_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-03-28 14:48:55.000000 jupyterhub-traefik-proxy-1.0.0b2/tests/test_traefik_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:36:38.764953 jupyterhub-traefik-proxy-1.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-05-11 14:36:38.764953 jupyterhub-traefik-proxy-1.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2585 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:36:38.760954 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5415 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/consul.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7035 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/fileprovider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5533 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11844 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/kv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26372 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5018 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/traefik_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:36:38.760954 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-05-11 14:36:38.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-11 14:36:38.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 14:36:38.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-11 14:36:38.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-11 14:36:38.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-11 14:36:38.000000 jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:36:38.760954 jupyterhub-traefik-proxy-1.0.0b3/performance/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10504 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/performance/check_perf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/performance/dummy_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10061 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/performance/perf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-11 14:36:38.764953 jupyterhub-traefik-proxy-1.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:36:38.764953 jupyterhub-traefik-proxy-1.0.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/tests/test_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/tests/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2461 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/tests/test_kv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15524 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/tests/test_traefik_api_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-05-11 14:36:25.000000 jupyterhub-traefik-proxy-1.0.0b3/tests/test_traefik_utils.py
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/LICENSE` & `jupyterhub-traefik-proxy-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/PKG-INFO` & `jupyterhub-traefik-proxy-1.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-traefik-proxy
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: JupyterHub proxy implementation with traefik
 Home-page: https://jupyterhub-traefik-proxy.readthedocs.io
 Author: Project Jupyter Contributors
 Author-email: jupyter@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://jupyterhub-traefik-proxy.readthedocs.io
 Project-URL: Source, https://github.com/jupyterhub/traefik-proxy/
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/README.md` & `jupyterhub-traefik-proxy-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/consul.py` & `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/consul.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,32 +18,31 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 import base64
 import string
 from urllib.parse import urlparse
 
-from traitlets import Any, Unicode, default
+from traitlets import Any, Dict, Unicode, default
 
 from .kv_proxy import TKvProxy
+from .traefik_utils import deep_merge
 
 
 class TraefikConsulProxy(TKvProxy):
     """JupyterHub Proxy implementation using traefik and Consul"""
 
     provider_name = "consul"
 
     # Consul doesn't accept keys containing // or starting with / so we have to escape them
     key_safe_chars = string.ascii_letters + string.digits + "!@#$%^&*();<>-.+?:"
 
-    consul_client_ca_cert = Unicode(
+    consul_client_kwargs = Dict(
         config=True,
-        allow_none=True,
-        default_value=None,
-        help="""Consul client root certificates""",
+        help="Extra consul client constructor arguments",
     )
 
     consul_url = Unicode(
         "http://127.0.0.1:8500",
         config=True,
         help="URL for the consul endpoint.",
     )
@@ -81,18 +80,19 @@
             raise ImportError(
                 "Please install python-consul2 package to use traefik-proxy with consul"
             )
         consul_service = urlparse(self.consul_url)
         kwargs = {
             "host": consul_service.hostname,
             "port": consul_service.port,
-            "cert": self.consul_client_ca_cert,
         }
         if self.consul_password:
             kwargs.update({"token": self.consul_password})
+        if self.consul_client_kwargs:
+            kwargs.update(self.consul_client_kwargs)
         return consul.aio.Consul(**kwargs)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.log.warning(
             "Using traefik with consul is deprecated in jupyterhub-traefik-proxy 1.0 due to lack of support for the python-consul2 API client. Use etcd instead."
         )
@@ -101,19 +101,17 @@
         provider_config = {
             "consul": {
                 "rootKey": self.kv_traefik_prefix,
                 "endpoints": [urlparse(self.consul_url).netloc],
             }
         }
 
-        # FIXME: Same with the tls info
-        if self.consul_client_ca_cert:
-            provider_config["consul"]["tls"] = {"ca": self.consul_client_ca_cert}
-
-        self.static_config.update({"providers": provider_config})
+        self.static_config = deep_merge(
+            self.static_config, {"providers": provider_config}
+        )
         return super()._setup_traefik_static_config()
 
     def _start_traefik(self):
         if self.consul_password:
             if self.consul_username:
                 self.traefik_env.setdefault(
                     "CONSUL_HTTP_AUTH", f"{self.consul_username}:{self.consul_password}"
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/etcd.py` & `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/etcd.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,62 +18,30 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 from concurrent.futures import ThreadPoolExecutor
 from urllib.parse import urlparse
 
 from tornado.concurrent import run_on_executor
-from traitlets import Any, Bool, List, Unicode, default
+from traitlets import Any, Dict, Unicode, default
 
 from .kv_proxy import TKvProxy
+from .traefik_utils import deep_merge
 
 
 class TraefikEtcdProxy(TKvProxy):
     """JupyterHub Proxy implementation using traefik and etcd"""
 
     executor = Any()
 
     provider_name = "etcd"
 
-    etcd_client_ca_cert = Unicode(
+    etcd_client_kwargs = Dict(
         config=True,
-        allow_none=True,
-        default_value=None,
-        help="""Etcd client root certificates""",
-    )
-
-    etcd_client_cert_crt = Unicode(
-        config=True,
-        allow_none=True,
-        default_value=None,
-        help="""Etcd client certificate chain
-            (etcd_client_cert_key must also be specified)""",
-    )
-
-    etcd_client_cert_key = Unicode(
-        config=True,
-        allow_none=True,
-        default_value=None,
-        help="""Etcd client private key
-            (etcd_client_cert_crt must also be specified)""",
-    )
-
-    # The grpc client (used by the Python etcd library) doesn't allow untrusted
-    # etcd certificates, although traefik does allow them.
-    etcd_insecure_skip_verify = Bool(
-        False,
-        config=True,
-        help="""Traefik will by default validate SSL certificate of etcd backend""",
-    )
-
-    grpc_options = List(
-        config=True,
-        allow_none=True,
-        default_value=None,
-        help="""Any grpc options that need to be passed to the etcd client""",
+        help="""Extra keyword arguments to pass to the etcd Python client constructor""",
     )
 
     @default("executor")
     def _default_executor(self):
         return ThreadPoolExecutor(1)
 
     etcd_url = Unicode(
@@ -116,26 +84,24 @@
         except ImportError:
             raise ImportError(
                 "Please install etcd3 or etcdpy package to use traefik-proxy with etcd3"
             )
         kwargs = {
             'host': etcd_service.hostname,
             'port': etcd_service.port,
-            'ca_cert': self.etcd_client_ca_cert,
-            'cert_cert': self.etcd_client_cert_crt,
-            'cert_key': self.etcd_client_cert_key,
-            'grpc_options': self.grpc_options,
         }
         if self.etcd_password:
             kwargs.update(
                 {
                     "user": self.etcd_username,
                     "password": self.etcd_password,
                 }
             )
+        if self.etcd_client_kwargs:
+            kwargs.update(self.etcd_client_kwargs)
         return etcd3.client(**kwargs)
 
     def _cleanup(self):
         super()._cleanup()
         self.etcd.close()
 
     # low-level etcd APIs
@@ -190,33 +156,26 @@
                 transactions.append(delete(key))
         await self._etcd_transaction(transactions)
 
     # traefik + etcd methods
     def _setup_traefik_static_config(self):
         self.log.debug("Setting up the etcd provider in the static config")
         url = urlparse(self.etcd_url)
-        self.static_config.update(
-            {
-                "providers": {
-                    "etcd": {
-                        "endpoints": [url.netloc],
-                        "rootKey": self.kv_traefik_prefix,
-                    }
-                }
-            }
-        )
+        etcd_config = {
+            "endpoints": [url.netloc],
+            "rootKey": self.kv_traefik_prefix,
+        }
         if url.scheme == "https":
             # If etcd is running over TLS, then traefik needs to know
-            tls_conf = {}
-            if self.etcd_client_ca_cert is not None:
-                tls_conf["ca"] = self.etcd_client_ca_cert
-            tls_conf["insecureSkipVerify"] = self.etcd_insecure_skip_verify
-            self.static_config["providers"]["etcd"]["tls"] = tls_conf
+            etcd_config["tls"] = {}
 
         if self.etcd_username and self.etcd_password:
-            self.static_config["providers"]["etcd"].update(
+            etcd_config.update(
                 {
                     "username": self.etcd_username,
                     "password": self.etcd_password,
                 }
             )
+        self.static_config = deep_merge(
+            self.static_config, {"providers": {"etcd": etcd_config}}
+        )
         return super()._setup_traefik_static_config()
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/fileprovider.py` & `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/fileprovider.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
             dynamic_config = dynamic_config.copy()
             dynamic_config["http"] = http = dynamic_config["http"].copy()
             for key in ("routers", "services"):
                 if not http[key]:
                     http.pop(key)
             if not http:
                 dynamic_config.pop("http")
+        self.log.debug("Writing dynamic config %s", dynamic_config)
         self.dynamic_config_handler.atomic_dump(dynamic_config)
 
     async def _setup_traefik_dynamic_config(self):
         self.log.info(
             f"Creating the dynamic configuration file: {self.dynamic_config_file}"
         )
         await super()._setup_traefik_dynamic_config()
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/install.py` & `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/install.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/kv_proxy.py` & `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/kv_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,21 +315,30 @@
             return len(key.split(sep))
 
         tree = {}
         for key, value in sorted(kv_list, key=by_depth):
             key_path = key.split(sep)
             d = tree
             for parent_key, key in zip(key_path[:-1], key_path[1:]):
-                if parent_key not in d:
+                if parent_key.isdigit():
+                    parent_key = int(parent_key)
+                if isinstance(d, dict) and parent_key not in d:
                     # create container
                     if key.isdigit():
                         # integer keys mean it's a list
                         d[parent_key] = []
                     else:
                         d[parent_key] = {}
+                elif isinstance(d, list):
+                    if key.isdigit():
+                        # integer keys mean it's a list
+                        next_d = []
+                    else:
+                        next_d = {}
+                    d.append(next_d)
                 # walk down to the next level
                 d = d[parent_key]
             if isinstance(d, list):
                 # validate list keys
                 if len(d) != int(key):
                     raise IndexError(
                         f"Got invalid list key {key_path}, missing previous items in {d}"
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/proxy.py` & `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 from jupyterhub.proxy import Proxy
 from jupyterhub.utils import exponential_backoff, new_token, url_path_join
 from tornado.httpclient import AsyncHTTPClient, HTTPClientError
 from traitlets import Any, Bool, Dict, Integer, Unicode, default, observe, validate
 
 from . import traefik_utils
+from .traefik_utils import deep_merge
 
 
 class TraefikProxy(Proxy):
     """JupyterHub Proxy implementation using traefik"""
 
     provider_name = ""  # must be set in subclasses
 
@@ -61,14 +62,33 @@
     def _concurrency_changed(self, change):
         self.semaphore = asyncio.BoundedSemaphore(change.new)
 
     static_config_file = Unicode(
         "traefik.toml", config=True, help="""traefik's static configuration file"""
     )
 
+    extra_static_config = Dict(
+        config=True,
+        help="""Extra static configuration for treafik.
+
+        Merged with the default static config before writing to `.static_config_file`.
+
+        Has no effect if `Proxy.should_start` is False.
+        """,
+    )
+    extra_dynamic_config = Dict(
+        config=True,
+        help="""Extra dynamic configuration for treafik.
+
+        Merged with the default dynamic config during startup.
+
+        Always takes effect.
+        """,
+    )
+
     toml_static_config_file = Unicode(
         config=True,
         help="Deprecated. Use static_config_file",
     ).tag(
         deprecated_in="1.0",
         deprecated_for="static_config_file",
     )
@@ -184,21 +204,14 @@
             if parsed.scheme == 'http':
                 parsed = parsed._replace(netloc=f'{parsed.hostname}:80')
             elif parsed.scheme == 'https':
                 parsed = parsed._replace(netloc=f'{parsed.hostname}:443')
             url = urlunparse(parsed)
         return url
 
-    traefik_cert_resolver = Unicode(
-        config=True,
-        help="""The traefik certificate Resolver to use for requesting certificates""",
-    )
-
-    # FIXME: How best to enable TLS on routers assigned to only select
-    # entrypoints defined here?
     traefik_entrypoint = Unicode(
         help="""The traefik entrypoint name to use.
 
         By default, will be `http` if http or `https` if https.
 
         If running traefik externally with your own specified entrypoint name,
         set this value.
@@ -283,43 +296,46 @@
         )
         path = f"/api/http/{kind}s/{expected}"
         try:
             resp = await self._traefik_api_request(path)
             json.loads(resp.body)
         except HTTPClientError as e:
             if e.code == 404:
-                self.log.debug(f"traefik {expected} not yet in {kind}")
+                self.log.debug(
+                    "Traefik route for %s: %s not yet in %s", routespec, expected, kind
+                )
                 return False
             self.log.exception(f"Error checking traefik api for {kind} {routespec}")
             return False
         except Exception:
             self.log.exception(f"Error checking traefik api for {kind} {routespec}")
             return False
 
         # found the expected endpoint
         return True
 
     async def _wait_for_route(self, routespec):
-        self.log.debug("Waiting for %s to register with traefik", routespec)
+        self.log.debug("Traefik route for %s: waiting to register", routespec)
 
         async def _check_traefik_dynamic_conf_ready():
             """Check if traefik loaded its dynamic configuration yet"""
             if not await self._check_for_traefik_service(routespec, "service"):
                 return False
             if not await self._check_for_traefik_service(routespec, "router"):
                 return False
 
             return True
 
         await exponential_backoff(
             _check_traefik_dynamic_conf_ready,
-            f"Traefik route for {routespec} configuration not available",
+            f"Traefik route for {routespec}: not ready",
             scale_factor=1.2,
             timeout=self.check_route_timeout,
         )
+        self.log.debug("Treafik route for %s: registered", routespec)
 
     async def _traefik_api_request(self, path):
         """Make an API request to traefik"""
         url = url_path_join(self.traefik_api_url, path)
         self.log.debug("Fetching traefik api %s", url)
         resp = await AsyncHTTPClient().fetch(
             url,
@@ -361,20 +377,31 @@
                         self.log.debug(
                             f"traefik api at {e.response.request.url} overview not ready yet"
                         )
                     return False
                 # unexpected
                 self.log.error(f"Error checking for traefik static configuration {e}")
                 return False
-            except (OSError, ssl.SSLError) as e:
+            except ssl.SSLError as e:
                 # Can occur if SSL isn't set up yet
                 self.log.warning(
                     f"SSL Error checking for traefik static configuration: {e}"
                 )
                 return False
+            except OSError as e:
+                # OSError can occur during SSL setup,
+                # e.g. if socket is listening, but SSL isn't ready
+                if self.traefik_api_url.startswith("https:"):
+                    self.log.warning(
+                        f"Error checking for traefik static configuration: {e}"
+                    )
+                    return False
+                else:
+                    # other OSErrors should be fatal
+                    raise
 
             return True
 
         await exponential_backoff(
             _check_traefik_static_conf_ready,
             "Traefik static configuration not available",
             timeout=self.check_route_timeout,
@@ -410,69 +437,99 @@
         """When should_start=True, we are in control of traefik's static configuration
         file. This sets up the entrypoints and api handler in self.static_config, and
         then saves it to :attrib:`self.static_config_file`.
 
         Subclasses should specify any traefik providers themselves, in
         :attrib:`self.static_config["providers"]`
         """
-        self.static_config["providers"][
-            "providersThrottleDuration"
-        ] = self.traefik_providers_throttle_duration
-
+        static_config = {
+            "api": {},
+            "providers": {
+                "providersThrottleDuration": self.traefik_providers_throttle_duration,
+            },
+        }
         if self.traefik_log_level:
-            self.static_config["log"] = {"level": self.traefik_log_level}
+            static_config["log"] = {"level": self.traefik_log_level}
 
-        entrypoints = {
+        entrypoints = static_config["entryPoints"] = {
             self.traefik_entrypoint: {
                 "address": urlparse(self.public_url).netloc,
             },
             self.traefik_api_entrypoint: {
                 "address": urlparse(self.traefik_api_url).netloc,
             },
         }
 
-        self.static_config["entryPoints"] = entrypoints
-        self.static_config["api"] = {}
+        if self.is_https:
+            entrypoints[self.traefik_entrypoint]["http"] = {
+                "tls": {
+                    "options": "default",
+                }
+            }
+
+        # load what we just defined at _lower_ priority
+        # than anything added to self.static_config in a subclass before this
+        self.static_config = deep_merge(static_config, self.static_config)
+        if self.extra_static_config:
+            self.static_config = deep_merge(
+                self.static_config, self.extra_static_config
+            )
 
         self.log.info(f"Writing traefik static config: {self.static_config}")
 
         try:
             handler = traefik_utils.TraefikConfigFileHandler(self.static_config_file)
             handler.atomic_dump(self.static_config)
         except Exception:
             self.log.error("Couldn't set up traefik's static config.")
             raise
 
     async def _setup_traefik_dynamic_config(self):
         self.log.debug("Setting up traefik's dynamic config...")
         self._generate_htpassword()
         api_url = urlparse(self.traefik_api_url)
-        api_path = api_url.path if api_url.path else '/api'
+        api_path = api_url.path if api_url.path.strip("/") else '/api'
         api_credentials = (
             f"{self.traefik_api_username}:{self.traefik_api_hashed_password}"
         )
-        http = self.dynamic_config.setdefault("http", {})
-        routers = http.setdefault("routers", {})
+        dynamic_config = {
+            "http": {
+                "routers": {},
+                "middlewares": {},
+            }
+        }
+        routers = dynamic_config["http"]["routers"]
+        middlewares = dynamic_config["http"]["middlewares"]
         routers["route_api"] = {
             "rule": f"Host(`{api_url.hostname}`) && PathPrefix(`{api_path}`)",
             "entryPoints": [self.traefik_api_entrypoint],
             "service": "api@internal",
             "middlewares": ["auth_api"],
         }
-        middlewares = http.setdefault("middlewares", {})
         middlewares["auth_api"] = {"basicAuth": {"users": [api_credentials]}}
+
+        # add default ssl cert/keys
         if self.ssl_cert and self.ssl_key:
-            tls = self.dynamic_config.setdefault("tls", {})
-            stores = tls.setdefault("stores", {})
-            stores["default"] = {
-                "defaultCertificate": {
-                    "certFile": self.ssl_cert,
-                    "keyFile": self.ssl_key,
+            dynamic_config["tls"] = {
+                "stores": {
+                    "default": {
+                        "defaultCertificate": {
+                            "certFile": self.ssl_cert,
+                            "keyFile": self.ssl_key,
+                        }
+                    }
                 }
             }
+
+        self.dynamic_config = deep_merge(dynamic_config, self.dynamic_config)
+        if self.extra_dynamic_config:
+            self.dynamic_config = deep_merge(
+                self.dynamic_config, self.extra_dynamic_config
+            )
+
         await self._apply_dynamic_config(self.dynamic_config, None)
 
     def validate_routespec(self, routespec):
         """Override jupyterhub's default Proxy.validate_routespec method, as traefik
         can set router rule's on both Host and PathPrefix rules combined.
         """
         if not routespec.endswith("/"):
@@ -552,27 +609,14 @@
             "rule": rule,
             "entryPoints": [self.traefik_entrypoint],
         }
         traefik_config["http"]["services"][service_alias] = {
             "loadBalancer": {"servers": [{"url": target}], "passHostHeader": True}
         }
 
-        # Enable TLS on this router if globally enabled
-        if self.is_https:
-            tls_config = {}
-            if self.traefik_cert_resolver:
-                tls_config["certResolver"] = self.traefik_cert_resolver
-            else:
-                # we need _some_ key to be set
-                # because key-value stores can't store empty dicts.
-                # put a default value here
-                tls_config["options"] = "default"
-
-            router["tls"] = tls_config
-
         # Add the data node to a separate top-level node, so traefik doesn't see it.
         # key needs to be key-value safe (no '/')
         # store original routespec, router, service aliases for easy lookup
         jupyterhub_config["routes"][router_alias] = {
             "data": data,
             "routespec": routespec,
             "target": target,
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/toml.py` & `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/toml.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy/traefik_utils.py` & `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy/traefik_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,22 +18,54 @@
         if "Consul" in proxy_class and u.startswith("/"):
             u = u[1:]
 
         return u
 
 
 def generate_rule(routespec):
+    """Generate a traefik routing rule for a jupyterhub routespec
+
+
+    - if a routespec doesn't start with a `/`, the first part is a hostname.
+    - routespecs always end with `/`
+    - routespecs are a path _prefix_, and should match anything under them
+    - the root of the route without the trailing slash should match the rule,
+      e.g. the routespec `/prefix/` should match `/prefix` and `/prefix/tree`
+
+    Traefik rule documentation: https://doc.traefik.io/traefik/routing/routers/#rule
+    """
+
+    # validate assumption that routespecs always end with '/'
+    if not routespec.endswith("/"):
+        raise ValueError("routespec must end with /")
     routespec = unquote(routespec)
+
+    # traefik won't match /proxy/path to /proxy/path/
+    # so strip trailing slash for consistent behavior
     if routespec.startswith("/"):
         # Path-based route, e.g. /proxy/path/
-        rule = f"PathPrefix(`{routespec}`)"
+        host = ""
+        path = routespec
     else:
         # Host-based routing, e.g. host.tld/proxy/path/
-        host, path_prefix = routespec.split("/", 1)
-        rule = f"Host(`{host}`) && PathPrefix(`/{path_prefix}`)"
+        host, slash, path = routespec.partition("/")
+        path = slash + path
+
+    path_no_slash = path.rstrip("/")
+
+    path_rule = f"PathPrefix(`{path}`)"
+    if path_no_slash:
+        # include exact Path('/prefix') so that both /prefix/ and /prefix
+        # are served correctly
+        path_rule = f"( {path_rule} || Path(`{path_no_slash}`) )"
+
+    if host:
+        rule = f"Host(`{host}`) && {path_rule}"
+    else:
+        rule = path_rule
     return rule
 
 
 _safe = set(string.ascii_letters + string.digits + "-")
 
 
 def generate_alias(routespec, kind=""):
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy.egg-info/PKG-INFO` & `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-traefik-proxy
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: JupyterHub proxy implementation with traefik
 Home-page: https://jupyterhub-traefik-proxy.readthedocs.io
 Author: Project Jupyter Contributors
 Author-email: jupyter@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://jupyterhub-traefik-proxy.readthedocs.io
 Project-URL: Source, https://github.com/jupyterhub/traefik-proxy/
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/jupyterhub_traefik_proxy.egg-info/SOURCES.txt` & `jupyterhub-traefik-proxy-1.0.0b3/jupyterhub_traefik_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/performance/check_perf.py` & `jupyterhub-traefik-proxy-1.0.0b3/performance/check_perf.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/performance/dummy_http_server.py` & `jupyterhub-traefik-proxy-1.0.0b3/performance/dummy_http_server.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/performance/perf_utils.py` & `jupyterhub-traefik-proxy-1.0.0b3/performance/perf_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/pyproject.toml` & `jupyterhub-traefik-proxy-1.0.0b3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 # Ignore thousands of tests in dependencies installed in a virtual environment
 norecursedirs = "lib lib64"
 
 [tool.tbump]
 github_url = "https://github.com/jupyterhub/traefik-proxy"
 
 [tool.tbump.version]
-current = "1.0.0b2"
+current = "1.0.0b3"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/setup.py` & `jupyterhub-traefik-proxy-1.0.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf8") as f:
     readme = f.read()
 
 setup(
     name="jupyterhub-traefik-proxy",
-    version="1.0.0b2",
+    version="1.0.0b3",
     install_requires=open("requirements.txt").read().splitlines(),
     python_requires=">=3.6",
     author="Project Jupyter Contributors",
     author_email="jupyter@googlegroups.com",
     url="https://jupyterhub-traefik-proxy.readthedocs.io",
     project_urls={
         "Documentation": "https://jupyterhub-traefik-proxy.readthedocs.io",
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/tests/test_deprecations.py` & `jupyterhub-traefik-proxy-1.0.0b3/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/tests/test_installer.py` & `jupyterhub-traefik-proxy-1.0.0b3/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/tests/test_kv.py` & `jupyterhub-traefik-proxy-1.0.0b3/tests/test_kv.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,19 @@
             {"key": {"level": "true", "deeper": {"anddeeper": "false"}}},
         ),
         (
             [("key/level", "true"), ("key/deeper/anddeeper", "false")],
             "key/deeper",
             {"anddeeper": "false"},
         ),
+        (
+            [("key/0/x", "true"), ("key/1/y", "false")],
+            "",
+            {"key": [{"x": "true"}, {"y": "false"}]},
+        ),
     ],
 )
 def test_unflatten_dict(flat, root_key, expected):
     proxy = TKvProxy()
     unflat = proxy.unflatten_dict_from_kv(flat, root_key=root_key)
     assert unflat == expected
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/tests/test_proxy.py` & `jupyterhub-traefik-proxy-1.0.0b3/tests/test_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,14 +212,15 @@
 
     backends = await launch_backends(1 + len(existing_routes))
 
     default_backend = backends[0]
     extra_backends = backends[1:]
 
     proxy_url = proxy.public_url.rstrip("/")
+    assert 'https:' in proxy_url
 
     def normalize_spec(spec):
         return proxy.validate_routespec(spec)
 
     def expected_output(spec, url):
         return {
             "routespec": normalize_spec(spec),
@@ -332,14 +333,35 @@
         await exponential_backoff(_wait_for_deletion, "Route still exists")
 
     # Test that other routes are still exist
     for i, spec in enumerate(existing_routes):
         await test_route_exist(spec, extra_backends[i])
 
 
+async def test_trailing_slash(proxy, launch_backends):
+    proxy_url = proxy.public_url.rstrip("/")
+    routespec = "/path/prefix/"
+    default_backend, target_backend = await launch_backends(2)
+    target_port = urlparse(target_backend).port
+    default_port = urlparse(default_backend).port
+
+    await proxy.add_route("/", default_backend, {})
+    await proxy.add_route(routespec, target_backend, {})
+
+    port = await utils.get_responding_backend_port(proxy_url, "/path/prefix/")
+    assert port == target_port
+    port = await utils.get_responding_backend_port(proxy_url, "/path/prefix")
+    assert port == target_port
+    port = await utils.get_responding_backend_port(proxy_url, "/path/prefixnoslash")
+    assert port == default_port
+
+    for route in ["/", routespec]:
+        await proxy.delete_route(route)
+
+
 async def test_get_all_routes(proxy, launch_backends):
     # initial state: no routes
     routes = await proxy.get_all_routes()
     assert routes == {}
 
     routespecs = ["/proxy/path1", "/proxy/path2/", "/proxy/path3/"]
     targets = await launch_backends(len(routespecs))
```

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/tests/test_traefik_api_auth.py` & `jupyterhub-traefik-proxy-1.0.0b3/tests/test_traefik_api_auth.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-traefik-proxy-1.0.0b2/tests/test_traefik_utils.py` & `jupyterhub-traefik-proxy-1.0.0b3/tests/test_traefik_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -72,7 +72,24 @@
 
     # file didn't get overwritten
     with testfile.open("r") as f:
         assert f.read() == "before"
 
     # didn't leave any residue
     assert tmpdir.listdir() == [testfile]
+
+
+@pytest.mark.parametrize(
+    "routespec, expected_rule",
+    [
+        ("/", "PathPrefix(`/`)"),
+        ("/path/prefix/", "( PathPrefix(`/path/prefix/`) || Path(`/path/prefix`) )"),
+        ("host/", "Host(`host`) && PathPrefix(`/`)"),
+        (
+            "host/path/prefix/",
+            "Host(`host`) && ( PathPrefix(`/path/prefix/`) || Path(`/path/prefix`) )",
+        ),
+    ],
+)
+def test_generate_rule(routespec, expected_rule):
+    rule = traefik_utils.generate_rule(routespec)
+    assert rule == expected_rule
```

