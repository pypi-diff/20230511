# Comparing `tmp/cushy-storage-1.0.2.tar.gz` & `tmp/cushy-storage-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cushy-storage/cushy-storage/dist/.tmp-ukl_go3c/cushy-storage-1.0.2.tar", last modified: Sat Apr 22 08:52:11 2023, max compression
+gzip compressed data, was "/home/runner/work/cushy-storage/cushy-storage/dist/.tmp-j3ydswem/cushy-storage-1.0.3.tar", last modified: Thu May 11 16:06:00 2023, max compression
```

## Comparing `cushy-storage-1.0.2.tar` & `cushy-storage-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/cushy_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/cushy_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/cushy_storage/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/cushy_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/cushy_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/cushy_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/cushy_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/cushy_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/tests/test_base_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/tests/test_cushy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/tests/test_dict_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/cushy_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/cushy_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/cushy_storage/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/cushy_storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/cushy_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/cushy_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/cushy_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/cushy_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/cushy_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/tests/test_base_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/tests/test_cushy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/tests/test_dict_cache.py
```

### Comparing `cushy-storage-1.0.2/LICENSE` & `cushy-storage-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.2/PKG-INFO` & `cushy-storage-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cushy-storage
-Version: 1.0.2
+Version: 1.0.3
 Summary: A data local persistence framework library
 Home-page: https://github.com/Undertone0809/cushy-storage
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: storage,serialization,json,cushy-storage,cushy_storage
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cushy-storage-1.0.2/README.md` & `cushy-storage-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.2/cushy_storage/__init__.py` & `cushy-storage-1.0.3/cushy_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.2/cushy_storage/_core.py` & `cushy-storage-1.0.3/cushy_storage/_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 import json
 import pickle
 import hashlib
 import threading
 from pathlib import Path
 from typing import MutableMapping, Callable, Tuple, Union, Any
 
+from cushy_storage.utils import get_default_storage_path
+
 __all__ = ['BaseDict', 'CushyDict', 'disk_cache']
 
 # Compression algorithms and their corresponding functions
 _COMPRESS = {
     'zlib': (
         zlib.compress,
         zlib.decompress,
@@ -51,41 +53,52 @@
         lambda x: json.dumps(x, sort_keys=True, ensure_ascii=False, separators=(',', ':')).encode('utf8'),
         json.loads,
     ),
 }
 
 # Locks for each hash value (hexadecimal representation of 0-255)
 _LOCKS = {hex(i)[2:].zfill(2): threading.Lock() for i in range(256)}
-_F = Union[str, Tuple[Callable, Callable], None]
 
 
-def _cf(s: _F, d: dict) -> Tuple[Callable, Callable]:
+def _cf(s: Union[str, Tuple[Callable, Callable], None], d: dict) -> Tuple[Callable, Callable]:
     """
     Helper function to get the compression or serialization functions based on input parameter
     """
     if s is None:
         return lambda x: x, lambda x: x
     elif isinstance(s, str):
         return d[s]
     else:
         return s
 
 
 class BaseDict(MutableMapping[str, bytes]):
-    def __init__(self, path: str, compress: _F = None):
+    def __init__(self, path: str, compress: Union[str, Tuple[Callable, Callable], None] = None):
         self.path = Path(path)
         if self.path.is_file():
             raise Exception('path has exist')  # Raise an exception if the path already exists as a file
         self.path.mkdir(parents=True, exist_ok=True)
         self.dirs = set()
         self.compress, self.decompress = _cf(compress, _COMPRESS)
 
     def __contains__(self, k: str):
         """
         Check if the file exists in the cache
+
+        Args:
+            k: key
+
+        Examples:
+            from cushy_storage import CushyDict
+
+            cache = CushyDict()
+            if 'my_key' in cache:
+                print("[my_key] in my cache")
+            else:
+                print("[my_key] not in my cache")
         """
         return (self.path / k[:2] / (k[2:] + '_')).is_file()
 
     def __getitem__(self, k: str):
         """
         Retrieve the cached item using its key and decompress it
         """
@@ -132,15 +145,20 @@
 
 
 class CushyDict(BaseDict):
     """
     A subclass of BaseDict that can serialize and deserialize values using different algorithms
     """
 
-    def __init__(self, path: str = './data', compress: _F = None, serialize: _F = 'json'):
+    def __init__(
+            self,
+            path: str = get_default_storage_path(),
+            compress: Union[str, Tuple[Callable, Callable], None] = None,
+            serialize: Union[str, Tuple[Callable, Callable], None] = 'json'
+    ):
         """
         Args:
             path: the path to save
             compress: zlib or lzma
             serialize: json or pickle
         """
         super().__init__(path, compress)
```

### Comparing `cushy-storage-1.0.2/cushy_storage.egg-info/PKG-INFO` & `cushy-storage-1.0.3/cushy_storage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cushy-storage
-Version: 1.0.2
+Version: 1.0.3
 Summary: A data local persistence framework library
 Home-page: https://github.com/Undertone0809/cushy-storage
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: storage,serialization,json,cushy-storage,cushy_storage
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cushy-storage-1.0.2/setup.py` & `cushy-storage-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="cushy-storage",
-    version="1.0.2",
+    version="1.0.3",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A data local persistence framework library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/cushy-storage",
     packages=setuptools.find_packages(),
```

### Comparing `cushy-storage-1.0.2/tests/test_base_dict.py` & `cushy-storage-1.0.3/tests/test_base_dict.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.2/tests/test_cushy_dict.py` & `cushy-storage-1.0.3/tests/test_cushy_dict.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.2/tests/test_dict_cache.py` & `cushy-storage-1.0.3/tests/test_dict_cache.py`

 * *Files identical despite different names*

