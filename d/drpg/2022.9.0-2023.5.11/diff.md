# Comparing `tmp/drpg-2022.9.0.tar.gz` & `tmp/drpg-2023.5.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drpg-2022.9.0.tar", last modified: Fri Sep 30 21:00:58 2022, max compression
+gzip compressed data, was "drpg-2023.5.11.tar", last modified: Thu May 11 12:09:26 2023, max compression
```

## Comparing `drpg-2022.9.0.tar` & `drpg-2023.5.11.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxr-x   0 grzegorzjanik  (1002) grzegorzjanik  (1002)        0 2022-09-30 21:00:58.637034 drpg-2022.9.0/
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)     1063 2021-09-13 19:57:56.000000 drpg-2022.9.0/LICENSE
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)     2906 2022-09-30 21:00:58.637034 drpg-2022.9.0/PKG-INFO
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)     1738 2021-09-14 10:21:27.000000 drpg-2022.9.0/README.md
-drwxrwxr-x   0 grzegorzjanik  (1002) grzegorzjanik  (1002)        0 2022-09-30 21:00:58.633034 drpg-2022.9.0/drpg/
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)       80 2022-09-30 21:00:51.000000 drpg-2022.9.0/drpg/__init__.py
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)       63 2021-09-13 19:57:56.000000 drpg-2022.9.0/drpg/__main__.py
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)     4064 2022-09-30 20:15:47.000000 drpg-2022.9.0/drpg/api.py
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)     3521 2022-09-30 20:30:40.000000 drpg-2022.9.0/drpg/cmd.py
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)      212 2021-09-13 19:57:56.000000 drpg-2022.9.0/drpg/config.py
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)        0 2021-09-13 19:57:56.000000 drpg-2022.9.0/drpg/py.typed
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)     4139 2022-09-30 20:57:07.000000 drpg-2022.9.0/drpg/sync.py
-drwxrwxr-x   0 grzegorzjanik  (1002) grzegorzjanik  (1002)        0 2022-09-30 21:00:58.637034 drpg-2022.9.0/drpg.egg-info/
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)     2906 2022-09-30 21:00:58.000000 drpg-2022.9.0/drpg.egg-info/PKG-INFO
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)      306 2022-09-30 21:00:58.000000 drpg-2022.9.0/drpg.egg-info/SOURCES.txt
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)        1 2022-09-30 21:00:58.000000 drpg-2022.9.0/drpg.egg-info/dependency_links.txt
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)       39 2022-09-30 21:00:58.000000 drpg-2022.9.0/drpg.egg-info/entry_points.txt
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)       12 2022-09-30 21:00:58.000000 drpg-2022.9.0/drpg.egg-info/requires.txt
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)        5 2022-09-30 21:00:58.000000 drpg-2022.9.0/drpg.egg-info/top_level.txt
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)     1152 2022-09-30 21:00:58.637034 drpg-2022.9.0/setup.cfg
--rw-rw-r--   0 grzegorzjanik  (1002) grzegorzjanik  (1002)      295 2022-09-30 20:15:47.000000 drpg-2022.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:09:26.932302 drpg-2023.5.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 12:09:16.000000 drpg-2023.5.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-11 12:09:26.932302 drpg-2023.5.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-11 12:09:16.000000 drpg-2023.5.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:09:26.932302 drpg-2023.5.11/drpg/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 12:09:16.000000 drpg-2023.5.11/drpg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 12:09:16.000000 drpg-2023.5.11/drpg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-05-11 12:09:16.000000 drpg-2023.5.11/drpg/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-11 12:09:16.000000 drpg-2023.5.11/drpg/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-11 12:09:16.000000 drpg-2023.5.11/drpg/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:09:16.000000 drpg-2023.5.11/drpg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-11 12:09:16.000000 drpg-2023.5.11/drpg/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:09:26.932302 drpg-2023.5.11/drpg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-11 12:09:26.000000 drpg-2023.5.11/drpg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-11 12:09:26.000000 drpg-2023.5.11/drpg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:09:26.000000 drpg-2023.5.11/drpg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:09:26.000000 drpg-2023.5.11/drpg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 12:09:26.000000 drpg-2023.5.11/drpg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 12:09:26.000000 drpg-2023.5.11/drpg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-11 12:09:26.936303 drpg-2023.5.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-11 12:09:16.000000 drpg-2023.5.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:09:26.932302 drpg-2023.5.11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-05-11 12:09:16.000000 drpg-2023.5.11/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-11 12:09:16.000000 drpg-2023.5.11/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-05-11 12:09:16.000000 drpg-2023.5.11/tests/test_sync.py
```

### Comparing `drpg-2022.9.0/LICENSE` & `drpg-2023.5.11/LICENSE`

 * *Files identical despite different names*

### Comparing `drpg-2022.9.0/PKG-INFO` & `drpg-2023.5.11/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,67 @@
 Metadata-Version: 2.1
 Name: drpg
-Version: 2022.9.0
+Version: 2023.5.11
 Summary: Download and keep up to date your purchases from DriveThruRPG
 Home-page: https://github.com/glujan/drpg
 Author: Grzegorz Janik
-License: UNKNOWN
+License: MIT
 Project-URL: GitHub, https://github.com/glujan/drpg
 Project-URL: Changelog, https://github.com/glujan/drpg/blob/master/CHANGELOG.md
-Description: # dRPG downloads and keeps your purchases from DriveThruRPG up to date
-        [![Maintainability](https://api.codeclimate.com/v1/badges/b3128ba6938f92088135/maintainability)](https://codeclimate.com/github/glujan/drpg/maintainability)
-        ![PyPI](https://img.shields.io/pypi/v/drpg?label=drpg)
-        
-        ## Installation
-        
-        This script runs with Python 3.8 and newer.
-        
-        You can install dRPG from PyPI:
-        ```bash
-        pip install --user drpg
-        drpg --help  # or python -m drpg --help
-        ```
-        
-        ## Usage
-        
-        1. Go to [your account settings](https://www.drivethrurpg.com/account_edit.php)
-           and generate a new application key.
-        2. Copy the key and run the script: `drpg --token <YOUR_DRPG_TOKEN>` - or set
-           `DRPG_TOKEN` env variable and run `drpg`.
-        3. Now just sit, relax and wait. Initial synchronization may take a while so
-           why don't you grab a cup of tea or whatever your favourite beverage is. On
-           consecutive runs the script will download only new and changed files which
-           will be a way faster.
-        
-        ## Compatibility
-        
-        Because of the nature of using an undocumented API, this software may break
-        without a notice. Version number indicates a year and a month when the software
-        was proved to be working with a real DriveThruRPG account.
-        
-        ### Advanced options
-        
-        You can change where your files will be downloaded by using `--library-path
-        path/to/your/directory`.
-        
-        By default the script does not compare files by md5 checksum to save time. You
-        can turn it on by using `--use-checksums`.
-        
-        You can change a log level by using `--log-level=<YOUR_LOG_LEVEL>`. Choices are
-        DEBUG, INFO, WARNING, ERROR, CRITICAL.
-        
-        For more information, run the script with `--help`.
-        
-        ## Found a bug?
-        
-        Pull requests and bug reports are welcomed! See [CONTRIBUTING.md](CONTRIBUTING.md)
-        for more details.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dRPG downloads and keeps your purchases from DriveThruRPG up to date
+[![Maintainability](https://api.codeclimate.com/v1/badges/b3128ba6938f92088135/maintainability)](https://codeclimate.com/github/glujan/drpg/maintainability)
+![PyPI](https://img.shields.io/pypi/v/drpg?label=drpg)
+
+## Installation
+
+This script runs with Python 3.8 and newer.
+
+You can install dRPG from PyPI:
+```bash
+pip install --user drpg
+drpg --help  # or python -m drpg --help
+```
+
+## Usage
+
+1. Go to [your account settings](https://www.drivethrurpg.com/account_edit.php)
+   and generate a new application key.
+2. Copy the key and run the script: `drpg --token <YOUR_DRPG_TOKEN>` - or set
+   `DRPG_TOKEN` env variable and run `drpg`.
+3. Now just sit, relax and wait. Initial synchronization may take a while so
+   why don't you grab a cup of tea or whatever your favourite beverage is. On
+   consecutive runs the script will download only new and changed files which
+   will be a way faster.
+
+## Compatibility
+
+Because of the nature of using an undocumented API, this software may break
+without a notice. Version number indicates a year and a month when the software
+was proved to be working with a real DriveThruRPG account.
+
+### Advanced options
+
+You can change where your files will be downloaded by using `--library-path
+path/to/your/directory`.
+
+By default the script does not compare files by md5 checksum to save time. You
+can turn it on by using `--use-checksums`.
+
+You can change a log level by using `--log-level=<YOUR_LOG_LEVEL>`. Choices are
+DEBUG, INFO, WARNING, ERROR, CRITICAL.
+
+For more information, run the script with `--help`.
+
+## Found a bug?
+
+Pull requests and bug reports are welcomed! See [CONTRIBUTING.md](CONTRIBUTING.md)
+for more details.
```

### Comparing `drpg-2022.9.0/README.md` & `drpg-2023.5.11/README.md`

 * *Files identical despite different names*

### Comparing `drpg-2022.9.0/drpg/api.py` & `drpg-2023.5.11/drpg/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,14 +38,18 @@
 
 
 class DrpgApi:
     """Low-level REST API client for DriveThruRPG"""
 
     API_URL = "https://www.drivethrurpg.com"
 
+    class FileTaskException(Exception):
+        UNEXPECTED_RESPONSE = "Got response with unexpected schema"
+        REQUEST_FAILED = "Got non 2xx response"
+
     def __init__(self, api_key: str):
         self._client = httpx.Client(base_url=self.API_URL, timeout=30.0)
         self._api_key = api_key
         self._customer_id = None
 
     def token(self) -> TokenResponse:
         """
@@ -87,15 +91,43 @@
         resp = self._client.post(
             "/api/v1/file_tasks",
             params=task_params,
             data={"products_id": product_id, "bundle_id": item_id},
             headers={"Content-Type": "application/x-www-form-urlencoded"},
         )
 
-        while (data := resp.json()["message"])["progress"].startswith("Preparing"):
+        def _parse_message(resp):
+            message = resp.json()["message"]
+            if resp.is_success:
+                expected_keys = {"progress", "file_tasks_id", "download_url"}
+                if isinstance(message, dict) and expected_keys.issubset(message.keys()):
+                    logger.debug(
+                        "Got download url for %s - %s: %s", product_id, item_id, message
+                    )
+                else:
+                    logger.debug(
+                        "Got unexpected message when getting download url for %s - %s: %s",
+                        product_id,
+                        item_id,
+                        message,
+                    )
+                    raise self.FileTaskException(
+                        self.FileTaskException.UNEXPECTED_RESPONSE
+                    )
+            else:
+                logger.debug(
+                    "Could not get download link for %s - %s: %s",
+                    product_id,
+                    item_id,
+                    message,
+                )
+                raise self.FileTaskException(self.FileTaskException.REQUEST_FAILED)
+            return message
+
+        while (data := _parse_message(resp))["progress"].startswith("Preparing"):
             logger.debug("Waiting for download link for: %s - %s", product_id, item_id)
             sleep(3)
             task_id = data["file_tasks_id"]
             resp = self._client.get(f"/api/v1/file_tasks/{task_id}", params=task_params)
 
         logger.debug("Got download link for: %s - %s", product_id, item_id)
         return data
```

### Comparing `drpg-2022.9.0/drpg/cmd.py` & `drpg-2023.5.11/drpg/cmd.py`

 * *Files identical despite different names*

### Comparing `drpg-2022.9.0/drpg/sync.py` & `drpg-2023.5.11/drpg/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,38 +11,37 @@
 
 import httpx
 
 from drpg.api import DrpgApi
 
 if TYPE_CHECKING:  # pragma: no cover
     from pathlib import Path
-    from typing import Callable, TypeVar
+    from typing import Any, Callable
 
     from drpg.api import DownloadItem, Product
     from drpg.config import Config
 
-    C = TypeVar("C", bound=Callable)
-    Decorator = Callable[[C], C]
+    NoneCallable = Callable[..., None]
+    Decorator = Callable[[NoneCallable], NoneCallable]
 
 
 _checksum_time_format = "%Y-%m-%d %H:%M:%S"
 logger = logging.getLogger("drpg")
 
 
 def suppress_errors(*errors: type[Exception]) -> Decorator:
     """Silence but log provided errors."""
 
-    def decorator(func: C) -> C:
+    def decorator(func: NoneCallable) -> NoneCallable:
         @functools.wraps(func)
-        def wrapper(*args, **kwargs):
+        def wrapper(*args: Any, **kwargs: Any) -> None:
             try:
-                func(*args, **kwargs)
+                return func(*args, **kwargs)
             except errors as e:
                 logger.exception(e)
-            return None
 
         return wrapper
 
     return decorator
 
 
 class DrpgSync:
@@ -70,15 +69,24 @@
 
     @suppress_errors(httpx.HTTPError, PermissionError)
     def _process_item(self, product: Product, item: DownloadItem) -> None:
         """Prepare for and download the item to the sync directory."""
 
         logger.info("Processing: %s - %s", product["products_name"], item["filename"])
 
-        url_data = self._api.file_task(product["products_id"], item["bundle_id"])
+        try:
+            url_data = self._api.file_task(product["products_id"], item["bundle_id"])
+        except self._api.FileTaskException:
+            logger.warning(
+                "Could not download product: %s - %s",
+                product["products_name"],
+                item["filename"],
+            )
+            return
+
         file_response = httpx.get(
             url_data["download_url"], timeout=30.0, follow_redirects=True
         )
 
         path = self._file_path(product, item)
         path.parent.mkdir(parents=True, exist_ok=True)
         path.write_bytes(file_response.content)
```

### Comparing `drpg-2022.9.0/drpg.egg-info/PKG-INFO` & `drpg-2023.5.11/drpg.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,67 @@
 Metadata-Version: 2.1
 Name: drpg
-Version: 2022.9.0
+Version: 2023.5.11
 Summary: Download and keep up to date your purchases from DriveThruRPG
 Home-page: https://github.com/glujan/drpg
 Author: Grzegorz Janik
-License: UNKNOWN
+License: MIT
 Project-URL: GitHub, https://github.com/glujan/drpg
 Project-URL: Changelog, https://github.com/glujan/drpg/blob/master/CHANGELOG.md
-Description: # dRPG downloads and keeps your purchases from DriveThruRPG up to date
-        [![Maintainability](https://api.codeclimate.com/v1/badges/b3128ba6938f92088135/maintainability)](https://codeclimate.com/github/glujan/drpg/maintainability)
-        ![PyPI](https://img.shields.io/pypi/v/drpg?label=drpg)
-        
-        ## Installation
-        
-        This script runs with Python 3.8 and newer.
-        
-        You can install dRPG from PyPI:
-        ```bash
-        pip install --user drpg
-        drpg --help  # or python -m drpg --help
-        ```
-        
-        ## Usage
-        
-        1. Go to [your account settings](https://www.drivethrurpg.com/account_edit.php)
-           and generate a new application key.
-        2. Copy the key and run the script: `drpg --token <YOUR_DRPG_TOKEN>` - or set
-           `DRPG_TOKEN` env variable and run `drpg`.
-        3. Now just sit, relax and wait. Initial synchronization may take a while so
-           why don't you grab a cup of tea or whatever your favourite beverage is. On
-           consecutive runs the script will download only new and changed files which
-           will be a way faster.
-        
-        ## Compatibility
-        
-        Because of the nature of using an undocumented API, this software may break
-        without a notice. Version number indicates a year and a month when the software
-        was proved to be working with a real DriveThruRPG account.
-        
-        ### Advanced options
-        
-        You can change where your files will be downloaded by using `--library-path
-        path/to/your/directory`.
-        
-        By default the script does not compare files by md5 checksum to save time. You
-        can turn it on by using `--use-checksums`.
-        
-        You can change a log level by using `--log-level=<YOUR_LOG_LEVEL>`. Choices are
-        DEBUG, INFO, WARNING, ERROR, CRITICAL.
-        
-        For more information, run the script with `--help`.
-        
-        ## Found a bug?
-        
-        Pull requests and bug reports are welcomed! See [CONTRIBUTING.md](CONTRIBUTING.md)
-        for more details.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dRPG downloads and keeps your purchases from DriveThruRPG up to date
+[![Maintainability](https://api.codeclimate.com/v1/badges/b3128ba6938f92088135/maintainability)](https://codeclimate.com/github/glujan/drpg/maintainability)
+![PyPI](https://img.shields.io/pypi/v/drpg?label=drpg)
+
+## Installation
+
+This script runs with Python 3.8 and newer.
+
+You can install dRPG from PyPI:
+```bash
+pip install --user drpg
+drpg --help  # or python -m drpg --help
+```
+
+## Usage
+
+1. Go to [your account settings](https://www.drivethrurpg.com/account_edit.php)
+   and generate a new application key.
+2. Copy the key and run the script: `drpg --token <YOUR_DRPG_TOKEN>` - or set
+   `DRPG_TOKEN` env variable and run `drpg`.
+3. Now just sit, relax and wait. Initial synchronization may take a while so
+   why don't you grab a cup of tea or whatever your favourite beverage is. On
+   consecutive runs the script will download only new and changed files which
+   will be a way faster.
+
+## Compatibility
+
+Because of the nature of using an undocumented API, this software may break
+without a notice. Version number indicates a year and a month when the software
+was proved to be working with a real DriveThruRPG account.
+
+### Advanced options
+
+You can change where your files will be downloaded by using `--library-path
+path/to/your/directory`.
+
+By default the script does not compare files by md5 checksum to save time. You
+can turn it on by using `--use-checksums`.
+
+You can change a log level by using `--log-level=<YOUR_LOG_LEVEL>`. Choices are
+DEBUG, INFO, WARNING, ERROR, CRITICAL.
+
+For more information, run the script with `--help`.
+
+## Found a bug?
+
+Pull requests and bug reports are welcomed! See [CONTRIBUTING.md](CONTRIBUTING.md)
+for more details.
```

### Comparing `drpg-2022.9.0/setup.cfg` & `drpg-2023.5.11/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 [metadata]
+name = drpg
+version = attr: drpg.__version__
+description = Download and keep up to date your purchases from DriveThruRPG
+long_description = file: README.md
+long_description_content_type = text/markdown
+url = https://github.com/glujan/drpg
 author = Grzegorz Janik
+license = MIT
+license_file = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
-description = Download and keep up to date your purchases from DriveThruRPG
-long_description_content_type = text/markdown
-long_description = file: README.md
-name = drpg
-url = https://github.com/glujan/drpg
-version = attr: drpg.__version__
+	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: Implementation :: CPython
 project_urls = 
 	GitHub=https://github.com/glujan/drpg
 	Changelog=https://github.com/glujan/drpg/blob/master/CHANGELOG.md
 
-[bdist_wheel]
-universal = 1
-
 [options]
 packages = drpg
-include_package_data = true
 python_requires = >=3.8
+include_package_data = true
 
 [options.entry_points]
 console_scripts = 
 	drpg = drpg.cmd:run
 
 [options.package_data]
 drpg = py.typed
 
+[bdist_wheel]
+universal = 1
+
 [coverage:run]
 branch = True
 include = drpg/*
 omit = 
 	.ropeproject,
 	venv
 
 [coverage:report]
 omit = 
 	.ropeproject,
 	venv
 
 [flake8]
 max-complexity = 10
-max-line-length = 88
+max-line-length = 100
 extend-exclude = 
 	.ropeproject,
 	venv
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

