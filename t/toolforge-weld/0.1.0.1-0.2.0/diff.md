# Comparing `tmp/toolforge-weld-0.1.0.1.tar.gz` & `tmp/toolforge-weld-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-weld-0.1.0.1.tar", last modified: Tue May  9 08:59:02 2023, max compression
+gzip compressed data, was "toolforge-weld-0.2.0.tar", last modified: Thu May 11 20:08:21 2023, max compression
```

## Comparing `toolforge-weld-0.1.0.1.tar` & `toolforge-weld-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/
--rw-r--r--   0 taavi     (1000) taavi     (1000)    34524 2023-05-05 13:07:36.000000 toolforge-weld-0.1.0.1/LICENSE
--rw-r--r--   0 taavi     (1000) taavi     (1000)      253 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/PKG-INFO
--rw-r--r--   0 taavi     (1000) taavi     (1000)       78 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/README.md
--rw-r--r--   0 taavi     (1000) taavi     (1000)      449 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/pyproject.toml
--rw-r--r--   0 taavi     (1000) taavi     (1000)       38 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/setup.cfg
--rw-r--r--   0 taavi     (1000) taavi     (1000)      454 2023-05-09 08:58:57.000000 toolforge-weld-0.1.0.1/setup.py
-drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/tests/
--rw-r--r--   0 taavi     (1000) taavi     (1000)      385 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/tests/test_kubernetes.py
--rw-r--r--   0 taavi     (1000) taavi     (1000)      418 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/tests/test_utils.py
-drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/toolforge_weld/
--rw-r--r--   0 taavi     (1000) taavi     (1000)      176 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/toolforge_weld/__init__.py
--rw-r--r--   0 taavi     (1000) taavi     (1000)     1590 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/toolforge_weld/errors.py
--rw-r--r--   0 taavi     (1000) taavi     (1000)    10043 2023-05-09 08:56:46.000000 toolforge-weld-0.1.0.1/toolforge_weld/kubernetes.py
-drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/toolforge_weld/logs/
--rw-r--r--   0 taavi     (1000) taavi     (1000)      535 2023-05-09 08:56:46.000000 toolforge-weld-0.1.0.1/toolforge_weld/logs/__init__.py
--rw-r--r--   0 taavi     (1000) taavi     (1000)     2457 2023-05-09 08:56:46.000000 toolforge-weld-0.1.0.1/toolforge_weld/logs/kubernetes.py
--rw-r--r--   0 taavi     (1000) taavi     (1000)      544 2023-05-09 08:56:46.000000 toolforge-weld-0.1.0.1/toolforge_weld/logs/source.py
--rw-r--r--   0 taavi     (1000) taavi     (1000)        0 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/toolforge_weld/py.typed
--rw-r--r--   0 taavi     (1000) taavi     (1000)      182 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/toolforge_weld/utils.py
-drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/toolforge_weld.egg-info/
--rw-r--r--   0 taavi     (1000) taavi     (1000)      253 2023-05-09 08:59:02.000000 toolforge-weld-0.1.0.1/toolforge_weld.egg-info/PKG-INFO
--rw-r--r--   0 taavi     (1000) taavi     (1000)      500 2023-05-09 08:59:02.000000 toolforge-weld-0.1.0.1/toolforge_weld.egg-info/SOURCES.txt
--rw-r--r--   0 taavi     (1000) taavi     (1000)        1 2023-05-09 08:59:02.000000 toolforge-weld-0.1.0.1/toolforge_weld.egg-info/dependency_links.txt
--rw-r--r--   0 taavi     (1000) taavi     (1000)       32 2023-05-09 08:59:02.000000 toolforge-weld-0.1.0.1/toolforge_weld.egg-info/requires.txt
--rw-r--r--   0 taavi     (1000) taavi     (1000)       15 2023-05-09 08:59:02.000000 toolforge-weld-0.1.0.1/toolforge_weld.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:08:21.475040 toolforge-weld-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34524 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-11 20:08:21.475040 toolforge-weld-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 20:08:21.475040 toolforge-weld-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      968 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:08:21.471040 toolforge-weld-0.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/tests/test_kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/tests/test_kubernetes_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:08:21.471040 toolforge-weld-0.2.0/toolforge_weld/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7555 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2673 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/kubernetes_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:08:21.475040 toolforge-weld-0.2.0/toolforge_weld/logs/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/logs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/logs/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/logs/source.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:08:21.471040 toolforge-weld-0.2.0/toolforge_weld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-11 20:08:21.000000 toolforge-weld-0.2.0/toolforge_weld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      597 2023-05-11 20:08:21.000000 toolforge-weld-0.2.0/toolforge_weld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 20:08:21.000000 toolforge-weld-0.2.0/toolforge_weld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-05-11 20:08:21.000000 toolforge-weld-0.2.0/toolforge_weld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-11 20:08:21.000000 toolforge-weld-0.2.0/toolforge_weld.egg-info/top_level.txt
```

### Comparing `toolforge-weld-0.1.0.1/LICENSE` & `toolforge-weld-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.1.0.1/toolforge_weld/errors.py` & `toolforge-weld-0.2.0/toolforge_weld/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.1.0.1/toolforge_weld/kubernetes.py` & `toolforge-weld-0.2.0/toolforge_weld/kubernetes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,25 @@
-import os
 from decimal import Decimal, InvalidOperation
 from pathlib import Path
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from typing import Any, ClassVar, Dict, List, Optional
 
-import requests
-import urllib3
-import yaml
-
-import toolforge_weld
+from toolforge_weld.api_client import ToolforgeClient
 from toolforge_weld.errors import ToolforgeError
+from toolforge_weld.kubernetes_config import Kubeconfig, locate_config_file
 
 
 class ToolforgeKubernetesError(ToolforgeError):
     """Base class for exceptions related to the Kubernetes client."""
 
 
 class KubernetesConfigFileNotFoundException(ToolforgeKubernetesError):
     """Raised when a Kubernetes client is attempted to be created but the configuration file does not exist."""
 
 
-def _find_cfg_obj(config, kind, name):
-    """Lookup a named object in a config."""
-    for obj in config[kind]:
-        if obj["name"] == name:
-            return obj[kind[:-1]]
-    raise ToolforgeKubernetesError(
-        "Key {} not found in {} section of config".format(name, kind)
-    )
-
-
-def _resolve_file_path(base: Path, input: str) -> Path:
-    input_path = Path(input).expanduser()
-    if input_path.is_absolute():
-        return input_path
-    return (base / input_path).resolve()
-
-
-class K8sClient:
+class K8sClient(ToolforgeClient):
     """Kubernetes API client."""
 
     VERSIONS: ClassVar[Dict[str, str]] = {
         "configmaps": "v1",
         "cronjobs": "batch/v1",
         "deployments": "apps/v1",
         "endpoints": "v1",
@@ -53,70 +32,41 @@
         "resourcequotas": "v1",
         "services": "v1",
     }
 
     def __init__(
         self,
         *,
-        server: str,
-        namespace: str,
-        tls_cert_file: Path,
-        tls_key_file: Path,
-        tls_verify_ca: Union[Path, bool],
+        kubeconfig: Kubeconfig,
         user_agent: str,
         timeout: int = 10,
     ):
         """Constructor."""
-        self.timeout = timeout
-        self.server = server
-        self.namespace = namespace
-        self.session = requests.Session()
-
-        self.session.cert = (str(tls_cert_file), str(tls_key_file))
-
-        if isinstance(tls_verify_ca, Path):
-            self.session.verify = str(tls_verify_ca.resolve())
-        else:
-            self.session.verify = tls_verify_ca
-
-            # T253412: Disable warnings about unverifed TLS certs when talking to the
-            # Kubernetes API endpoint
-            urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-
-        self.session.headers[
-            "User-Agent"
-        ] = f"{user_agent} toolforge_weld/{toolforge_weld.__version__} python-requests/{requests.__version__}"
+        self.server = kubeconfig.current_server
+        self.namespace = kubeconfig.current_namespace
+        super().__init__(
+            server=self.server,
+            kubeconfig=kubeconfig,
+            user_agent=user_agent,
+            timeout=timeout,
+        )
 
     @classmethod
     def from_file(cls, file: Path, **kwargs) -> "K8sClient":
-        """Create a client from a kubeconfig file."""
-        if not file.exists():
-            raise KubernetesConfigFileNotFoundException(str(file.resolve()))
-
-        data = yaml.safe_load(file.read_text())
-        context = _find_cfg_obj(data, "contexts", data["current-context"])
-        cluster = _find_cfg_obj(data, "clusters", context["cluster"])
-        user = _find_cfg_obj(data, "users", context["user"])
-
-        return cls(
-            server=cluster["server"],
-            namespace=context["namespace"],
-            tls_cert_file=_resolve_file_path(file.parent, user["client-certificate"]),
-            tls_key_file=_resolve_file_path(file.parent, user["client-key"]),
-            tls_verify_ca=False,
-            **kwargs,
-        )
+        """Deprecated: use regular __init__ instead."""
+        return cls(kubeconfig=Kubeconfig.load(path=file), **kwargs)
 
     @staticmethod
     def locate_config_file() -> Path:
-        """Attempt to locate the Kubernetes config file for this user."""
-        return Path(os.getenv("KUBECONFIG", "~/.kube/config")).expanduser()
+        """Deprecated: use Kubeconfig.load instead."""
+        return locate_config_file()
 
-    def _make_kwargs(self, url: str, **kwargs):
+    def make_kwargs(self, url: str, **kwargs):
         """Setup kwargs for a Requests request."""
+        kwargs = super().make_kwargs(url=url, **kwargs)
         version = kwargs.pop("version", "v1")
         if version == "v1":
             root = "api"
         else:
             root = "apis"
 
         # use "or" syntax in case namespace is present but set as None
@@ -130,52 +80,25 @@
         if name is not None:
             kwargs["url"] = "{}/{}".format(kwargs["url"], name)
 
         subpath = kwargs.pop("subpath", None)
         if subpath is not None:
             kwargs["url"] = "{}{}".format(kwargs["url"], subpath)
 
-        if "timeout" not in kwargs:
-            kwargs["timeout"] = self.timeout
-
         return kwargs
 
-    def _get(self, url, **kwargs):
-        """GET request."""
-        r = self.session.get(**self._make_kwargs(url, **kwargs))
-        r.raise_for_status()
-        return r.json()
-
-    def _post(self, url, **kwargs):
-        """POST request."""
-        r = self.session.post(**self._make_kwargs(url, **kwargs))
-        r.raise_for_status()
-        return r.status_code
-
-    def _put(self, url, **kwargs):
-        """PUT request."""
-        r = self.session.put(**self._make_kwargs(url, **kwargs))
-        r.raise_for_status()
-        return r.status_code
-
-    def _delete(self, url, **kwargs):
-        """DELETE request."""
-        r = self.session.delete(**self._make_kwargs(url, **kwargs))
-        r.raise_for_status()
-        return r.status_code
-
     def get_object(
         self,
         kind: str,
         name: str,
         *,
         namespace: Optional[str] = None,
     ) -> Dict[str, Any]:
         """Get the object with the specified name and of the given kind in the namespace."""
-        return self._get(
+        return self.get(
             kind,
             name=name,
             version=K8sClient.VERSIONS[kind],
             namespace=namespace,
         )
 
     def get_objects(
@@ -192,15 +115,15 @@
         if label_selector:
             params["labelSelector"] = ",".join(
                 [f"{k}={v}" for k, v in label_selector.items()]
             )
         if field_selector:
             params["fieldSelector"] = field_selector
 
-        return self._get(
+        return self.get(
             kind,
             params=params,
             version=K8sClient.VERSIONS[kind],
             namespace=namespace,
         )["items"]
 
     def delete_objects(
@@ -209,37 +132,37 @@
         *,
         label_selector: Optional[Dict[str, str]] = None,
     ):
         """Delete objects of the given kind in the namespace."""
         if kind == "services":
             # Annoyingly Service does not have a Delete Collection option
             for svc in self.get_objects(kind, label_selector=label_selector):
-                self._delete(
+                self.delete(
                     kind,
                     name=svc["metadata"]["name"],
                     version=K8sClient.VERSIONS[kind],
                 )
         else:
-            self._delete(
+            self.delete(
                 kind,
                 params={"labelSelector": label_selector},
                 version=K8sClient.VERSIONS[kind],
             )
 
     def create_object(self, kind: str, spec: Dict[str, Any]):
         """Create an object of the given kind in the namespace."""
-        return self._post(
+        return self.post(
             kind,
             json=spec,
             version=K8sClient.VERSIONS[kind],
         )
 
     def replace_object(self, kind: str, spec: Dict[str, Any]):
         """Replace an object of the given kind in the namespace."""
-        return self._put(
+        return self.put(
             kind,
             json=spec,
             name=spec["metadata"]["name"],
             version=K8sClient.VERSIONS[kind],
         )
```

### Comparing `toolforge-weld-0.1.0.1/toolforge_weld/logs/__init__.py` & `toolforge-weld-0.2.0/toolforge_weld/logs/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Queries logs created by a tool."""
 from toolforge_weld.kubernetes import K8sClient
+from toolforge_weld.kubernetes_config import Kubeconfig
 from toolforge_weld.logs.kubernetes import KubernetesSource
 from toolforge_weld.logs.source import LogEntry, LogSource
 
 
 def get_log_source(user_agent: str) -> LogSource:
     """Gets a suitable log source implementation."""
-    k8s_client = K8sClient.from_file(
-        file=K8sClient.locate_config_file(), user_agent=f"{user_agent} logs"
+    k8s_client = K8sClient(
+        kubeconfig=Kubeconfig.load(),
+        user_agent=f"{user_agent} logs",
     )
 
     return KubernetesSource(client=k8s_client)
 
 
 __all__ = ["LogSource", "LogEntry", "get_log_source"]
```

### Comparing `toolforge-weld-0.1.0.1/toolforge_weld/logs/kubernetes.py` & `toolforge-weld-0.2.0/toolforge_weld/logs/kubernetes.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             "timestamps": True,
         }
         if lines:
             params["tailLines"] = lines
         timeout = None if follow else self.client.timeout
 
         with self.client.session.get(
-            **self.client._make_kwargs(
+            **self.client.make_kwargs(
                 "pods",
                 name=pod_name,
                 subpath="/log",
                 params=params,
                 version=K8sClient.VERSIONS["pods"],
                 timeout=timeout,
             ),
```

### Comparing `toolforge-weld-0.1.0.1/toolforge_weld/logs/source.py` & `toolforge-weld-0.2.0/toolforge_weld/logs/source.py`

 * *Files identical despite different names*

