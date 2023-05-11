# Comparing `tmp/gportal-0.3.0.tar.gz` & `tmp/gportal-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gportal-0.3.0.tar", max compression
+gzip compressed data, was "gportal-0.4.0.tar", max compression
```

## Comparing `gportal-0.3.0.tar` & `gportal-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1073 2023-04-11 12:05:29.006972 gportal-0.3.0/LICENSE
--rw-r--r--   0        0        0     1937 2023-04-11 12:05:29.006972 gportal-0.3.0/README.md
--rw-r--r--   0        0        0      286 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/__init__.py
--rw-r--r--   0        0        0    28946 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/data/datasets.json
--rw-r--r--   0        0        0     1663 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/dataset.py
--rw-r--r--   0        0        0      422 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/http_client.py
--rw-r--r--   0        0        0     5257 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/product.py
--rw-r--r--   0        0        0     4192 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/search.py
--rw-r--r--   0        0        0     4894 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/sftp.py
--rw-r--r--   0        0        0     1357 2023-04-11 12:05:29.042973 gportal-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 gportal-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-11 16:14:12.056443 gportal-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2271 2023-05-11 16:14:12.056443 gportal-0.4.0/README.md
+-rw-r--r--   0        0        0      286 2023-05-11 16:14:12.136444 gportal-0.4.0/gportal/__init__.py
+-rw-r--r--   0        0        0    28946 2023-05-11 16:14:12.136444 gportal-0.4.0/gportal/data/datasets.json
+-rw-r--r--   0        0        0     1663 2023-05-11 16:14:12.136444 gportal-0.4.0/gportal/dataset.py
+-rw-r--r--   0        0        0       54 2023-05-11 16:14:12.136444 gportal-0.4.0/gportal/file/__init__.py
+-rw-r--r--   0        0        0     9584 2023-05-11 16:14:12.136444 gportal-0.4.0/gportal/file/gcomc.py
+-rw-r--r--   0        0        0      422 2023-05-11 16:14:12.136444 gportal-0.4.0/gportal/http_client.py
+-rw-r--r--   0        0        0     5257 2023-05-11 16:14:12.136444 gportal-0.4.0/gportal/product.py
+-rw-r--r--   0        0        0     4204 2023-05-11 16:14:12.136444 gportal-0.4.0/gportal/search.py
+-rw-r--r--   0        0        0     5634 2023-05-11 16:14:12.136444 gportal-0.4.0/gportal/sftp.py
+-rw-r--r--   0        0        0     1602 2023-05-11 16:14:12.140444 gportal-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 gportal-0.4.0/PKG-INFO
```

### Comparing `gportal-0.3.0/LICENSE` & `gportal-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gportal-0.3.0/README.md` & `gportal-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,19 @@
 gportal.download(products, local_dir="path/to/download/dir")
 ```
 
 ## Documentation
 
 https://gportal.readthedocs.io/
 
+## Contributing
+
+Bug reports and pull requests are welcome on GitHub at https://github.com/sankichi92/gportal-python.
+This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [code of conduct](https://github.com/sankichi92/gportal-python/blob/main/CODE_OF_CONDUCT.md).
+
 ## Development
 
 This project uses [Poetry](https://python-poetry.org/).
 
 ### Install dependencies
 
     $ poetry install
```

### Comparing `gportal-0.3.0/gportal/data/datasets.json` & `gportal-0.4.0/gportal/data/datasets.json`

 * *Files identical despite different names*

### Comparing `gportal-0.3.0/gportal/dataset.py` & `gportal-0.4.0/gportal/dataset.py`

 * *Files identical despite different names*

### Comparing `gportal-0.3.0/gportal/product.py` & `gportal-0.4.0/gportal/product.py`

 * *Files identical despite different names*

### Comparing `gportal-0.3.0/gportal/search.py` & `gportal-0.4.0/gportal/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         A [Search][gportal.search.Search] instance that represents deferred query.
     """
     params = params.copy()
 
     if dataset_ids:
         params["datasetId"] = ",".join(map(str, dataset_ids))
 
-    if bbox:
+    if bbox is not None:
         params["bbox"] = ",".join(map(str, bbox))
 
     if isinstance(start_time, datetime):
         params["startTime"] = start_time.isoformat()
     elif start_time:
         params["startTime"] = start_time
```

### Comparing `gportal-0.3.0/gportal/sftp.py` & `gportal-0.4.0/gportal/sftp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,57 @@
 import os.path
 import re
 from collections.abc import Iterable
-from typing import Optional, Union
+from typing import Optional, Union, overload
 
 from paramiko.sftp_client import SFTPClient
 from paramiko.transport import Transport
 
 import gportal
 
 from .product import Product
 
 
+@overload
 def download(
-    target: Union[str, Product, Iterable[Union[str, Product]]],
+    target: Union[str, Product],
+    local_dir: str = ".",
+    username: Optional[str] = None,
+    password: Optional[str] = None,
+) -> str:
+    ...
+
+
+@overload
+def download(
+    target: Iterable[Union[str, Product]],
     local_dir: str = ".",
     username: Optional[str] = None,
     password: Optional[str] = None,
 ) -> list[str]:
+    ...
+
+
+def download(
+    target: Union[str, Product, Iterable[Union[str, Product]]],
+    local_dir: str = ".",
+    username: Optional[str] = None,
+    password: Optional[str] = None,
+) -> Union[str, list[str]]:
     """Downloads files to a local directory via SFTP.
 
     Args:
         target: Remote path, Product object, or a list of them.
         local_dir: Local directory to download to.
         username: G-Portal username. If not provided, the value of `gportal.username` is used.
         password: G-Portal password. If not provided, the value of `gportal.password` is used.
 
     Returns:
-        A list of local paths of the downloaded files.
+        A local path of the downloaded file when `target` is a single path or Product object.
+        A list of local paths of the downloaded files when `target` is a list of paths or Product objects.
     """
     with SFTP.connect(username, password) as sftp:
         return sftp.download(target, local_dir)
 
 
 class SFTP:
     """Wrapper of the G-Portal SFTP interface.
@@ -41,18 +62,18 @@
 
     HOST = "ftp.gportal.jaxa.jp"
     PORT = 2051
 
     def __init__(self, sftp_client: SFTPClient):
         self.client: SFTPClient = sftp_client
 
-    def __enter__(self):  # type: ignore[no-untyped-def]
+    def __enter__(self):
         return self
 
-    def __exit__(self, exc_type, exc_value, traceback):  # type: ignore[no-untyped-def]
+    def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     @classmethod
     def connect(cls, username: Optional[str] = None, password: Optional[str] = None) -> "SFTP":
         """Opens an SFTP session with G-Portal.
 
         Args:
@@ -101,29 +122,34 @@
             entries = [entry for entry in entries if re.search(filter_pattern, entry)]
 
         if fullpath:
             return [os.path.join(path, entry) for entry in entries]
         else:
             return entries
 
+    @overload
+    def download(self, target: Union[str, Product], local_dir: str) -> str:
+        ...
+
+    @overload
+    def download(self, target: Iterable[Union[str, Product]], local_dir: str) -> list[str]:
+        ...
+
     def download(
         self, target: Union[str, Product, Iterable[Union[str, Product]]], local_dir: str
     ) -> Union[str, list[str]]:
         """Downloads files to a local directory.
 
         Args:
             target: Remote path, Product object, or a list of them.
             local_dir: Local directory to download to.
 
         Returns:
-            If `target` is a single path or Product object, returns the local path of the downloaded file.
-            If `target` is a list of paths or Product objects, returns a list of local paths of the downloaded files.
-
-        Raises:
-            ValueError: If the given product has no URL to download.
+            A local path of the downloaded file when `target` is a single path or Product object.
+            A list of local paths of the downloaded files when `target` is a list of paths or Product objects.
         """
         self._reset_cwd()
 
         if isinstance(target, Iterable) and not isinstance(target, str):
             return [self._download_single(t, local_dir) for t in target]
         else:
             return self._download_single(target, local_dir)
@@ -131,13 +157,16 @@
     def _download_single(self, target: Union[str, Product], local_dir: str) -> str:
         if isinstance(target, Product):
             if target.data_path is None:
                 raise ValueError(f"Product {target.id} has no URL to download")
 
             target = target.data_path
 
+        elif target.startswith("https://gportal.jaxa.jp/download/"):
+            target = target.replace("https://gportal.jaxa.jp/download/", "", 1)
+
         local_path = os.path.join(local_dir, os.path.basename(target))
         self.client.get(target, local_path)
         return local_path
 
     def _reset_cwd(self) -> None:
         self.client.chdir()
```

### Comparing `gportal-0.3.0/PKG-INFO` & `gportal-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: gportal
-Version: 0.3.0
+Version: 0.4.0
 Summary: Client for JAXA G-Portal Catalogue Service and SFTP
 Home-page: https://github.com/sankichi92/gportal-python
 License: MIT
 Author: Takahiro Miyoshi
 Author-email: takahiro-miyoshi@sankichi.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: gcomc
+Requires-Dist: h5py (>=3.8.0,<4.0.0) ; extra == "gcomc"
+Requires-Dist: numpy (>=1.18,<2.0) ; extra == "gcomc"
 Requires-Dist: paramiko (>=3.1.0,<4.0.0)
+Requires-Dist: rasterio (>=1.3.6,<2.0.0) ; extra == "gcomc"
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Documentation, https://gportal.readthedocs.io/
 Project-URL: Repository, https://github.com/sankichi92/gportal-python
 Description-Content-Type: text/markdown
 
 # gportal-python
 
@@ -62,14 +66,19 @@
 gportal.download(products, local_dir="path/to/download/dir")
 ```
 
 ## Documentation
 
 https://gportal.readthedocs.io/
 
+## Contributing
+
+Bug reports and pull requests are welcome on GitHub at https://github.com/sankichi92/gportal-python.
+This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [code of conduct](https://github.com/sankichi92/gportal-python/blob/main/CODE_OF_CONDUCT.md).
+
 ## Development
 
 This project uses [Poetry](https://python-poetry.org/).
 
 ### Install dependencies
 
     $ poetry install
```

