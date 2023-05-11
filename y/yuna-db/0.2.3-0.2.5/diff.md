# Comparing `tmp/yuna-db-0.2.3.tar.gz` & `tmp/yuna-db-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuna-db-0.2.3.tar", last modified: Mon May  8 07:33:07 2023, max compression
+gzip compressed data, was "yuna-db-0.2.5.tar", last modified: Thu May 11 07:47:19 2023, max compression
```

## Comparing `yuna-db-0.2.3.tar` & `yuna-db-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.2.3/LICENSE
--rw-r--r--   0        0        0     1615 2023-05-08 07:27:32.741832 yuna-db-0.2.3/README.md
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.3/__init__.py
--rwxr-xr-x   0        0        0     3470 2023-05-08 07:32:52.780510 yuna-db-0.2.3/example.py
--rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.2.3/requirements.txt
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.3/src/__init__.py
--rw-r--r--   0        0        0    26645 2023-05-08 07:24:34.918122 yuna-db-0.2.3/src/yuna/__init__.py
--rw-r--r--   0        0        0     8915 2023-05-08 05:34:13.855559 yuna-db-0.2.3/src/yuna/lmdb_util.py
--rw-r--r--   0        0        0    31439 2023-05-08 06:49:57.398627 yuna-db-0.2.3/src/yuna/plugins.py
--rwxr-xr-x   0        0        0     1066 2023-05-08 05:37:29.051656 yuna-db-0.2.3/src/yuna/yuna_repack
--rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.2.3/tests/__init__.py
--rwxr-xr-x   0        0        0     9470 2023-05-02 23:48:28.489421 yuna-db-0.2.3/tests/test_yuna.py
--rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.2.3/version.txt
--rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 yuna-db-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4361 2023-05-11 07:30:49.745381 yuna-db-0.2.5/README.md
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.5/__init__.py
+-rwxr-xr-x   0        0        0     3464 2023-05-11 06:45:00.404430 yuna-db-0.2.5/example.py
+-rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.2.5/requirements.txt
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.5/src/__init__.py
+-rw-r--r--   0        0        0    26835 2023-05-11 07:45:07.799042 yuna-db-0.2.5/src/yuna/__init__.py
+-rw-r--r--   0        0        0     8899 2023-05-11 07:44:51.486706 yuna-db-0.2.5/src/yuna/lmdb_util.py
+-rw-r--r--   0        0        0    31439 2023-05-11 07:47:10.981581 yuna-db-0.2.5/src/yuna/plugins.py
+-rwxr-xr-x   0        0        0     1066 2023-05-08 05:37:29.051656 yuna-db-0.2.5/src/yuna/yuna_repack
+-rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.2.5/tests/__init__.py
+-rwxr-xr-x   0        0        0     9470 2023-05-02 23:48:28.489421 yuna-db-0.2.5/tests/test_yuna.py
+-rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.2.5/version.txt
+-rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 yuna-db-0.2.5/PKG-INFO
```

### Comparing `yuna-db-0.2.3/LICENSE` & `yuna-db-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yuna-db-0.2.3/example.py` & `yuna-db-0.2.5/example.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 delete_file_or_dir(TEST_FILE)
 with Yuna(TEST_FILE, "test", 1, create=True) as db:
     db.new_table("a26", serialize=yuna.SERIALIZE_STR, compress=yuna.COMPRESS_LZ4)
     tbl_a26 = db.tables.a26
     tbl_a26.put("a", "1")
     tbl_a26.put("b", "2")
     #tbl_a26.put("c", "3")
-    tbl_a26.put("d", "4")
-    tbl_a26.put("e", "5")
+    tbl_a26["d"] = "4"
+    tbl_a26["e"] = "5"
 
     lst = list(tbl_a26.keys())
     print(f"a26 keys: {lst}")
     lst = list(tbl_a26.keys(start='c'))
     print(f"a26 keys from 'c': {lst}")
     lst = list(tbl_a26.keys(start='c', stop='e'))
     print(f"a26 keys from 'c' to < 'e': {lst}")
```

### Comparing `yuna-db-0.2.3/src/yuna/__init__.py` & `yuna-db-0.2.5/src/yuna/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 db.tables.foo.put(key, x)
 
 After that .put() you can call .get():
 
 x = db.tables.foo.get(key)
 """
 
-__version__ = "0.2.3"
+__version__ = "0.2.5"
 
 import os
 import types
 
 from typing import Any, Iterator, Optional
 
 import lmdb
@@ -418,23 +418,23 @@
         if name in shared.tables_map:
             raise ValueError(f"table '{name}' is already open in this database")
 
         # TODO: check key_serialize to see if we are doing integer keys here
         try:
             temp = plugins.get_serialize_plugins(key_serialize)
         except ValueError:
-            raise ValueError("unknown serialization format for key_serialize: {repr(key_serialize)}")
+            raise ValueError("unknown serialization format for key_serialize: {key_serialize!r}")
         try:
             temp = plugins.get_serialize_plugins(serialize)
         except ValueError:
-            raise ValueError("unknown serialization format for serialize: {repr(serialize)}")
+            raise ValueError("unknown serialization format for serialize: {serialize!r}")
         try:
             temp = plugins.get_compress_plugins(compress)
         except ValueError:
-            raise ValueError("unknown compression format for compress: {repr(compress)}")
+            raise ValueError("unknown compression format for compress: {compress!r}")
 
         meta = YunaTableMetadata(
             name=name,
             key_serialize=key_serialize, serialize=serialize, compress=compress
         )
         self._shared = shared
 
@@ -494,14 +494,23 @@
         self._shared.tables_map[name] = self
         if create:
             self._shared.metadata["tables"][name] = vars(self.meta)
             _yuna_put_meta(self._shared.env, self._shared.metadata)
         else:
             assert self._shared.metadata["tables"][name] == vars(self.meta)
 
+    def __delitem__(self, key):
+        return self.delet(key)
+
+    def __getitem__(self, key):
+        return self.get(key)
+
+    def __setitem__(self, key, value):
+        return self.put(key, value)
+
     def drop(self):
         """
         Drop a table.  Delete all key/value pairs and the table itself.
         """
         if self._shared.read_only:
             raise RuntimeError("database was opened read-only; cannot drop table")
```

### Comparing `yuna-db-0.2.3/src/yuna/lmdb_util.py` & `yuna-db-0.2.5/src/yuna/lmdb_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,35 +206,35 @@
     Raises YunaInvalidDB on any error.
     """
     # Try to retrieve the metadata, always stored in the reserved table.
     key = bytes(YUNA_DB_META_KEY, "utf-8")
     value = _lmdb_reserved_get(env, key, default=None)
     if value is None:
         fname = env.path()
-        raise YunaInvalidDB(f"LMDB file is not a Yuna DB file: {repr(fname)}")
+        raise YunaInvalidDB(f"LMDB file is not a Yuna DB file: {fname!r}")
 
     # We got something... does it decode as valid JSON?
     try:
         meta = json.loads(value)
         if not isinstance(meta, dict):
             # whatever was stored there wasn't a JSON-encoded metadata dictionary
             raise ValueError
     except (ValueError, TypeError, json.decoder.JSONDecodeError):
         fname = env.path()
-        raise YunaInvalidDB(f"Yuna DB has corrupted metadata: {repr(fname)}")
+        raise YunaInvalidDB(f"Yuna DB has corrupted metadata: {fname!r}")
 
     # If user provided name and/or version, make appropriate checks.
     if name is not None:
         temp = meta.get("name", None)
         if temp != name:
-            raise YunaInvalidDB(f"LMDB file name mismatch: expected {repr(name)}, got {repr(temp)}")
+            raise YunaInvalidDB(f"LMDB file 'name' mismatch: expected {name!r}, got {temp!r}")
     if version is not None:
         temp = meta.get("version", None)
         if temp != version:
-            raise YunaInvalidDB(f"LMDB file version mismatch: expected {version}, got {temp}")
+            raise YunaInvalidDB(f"LMDB file 'version' mismatch: expected {version}, got {temp}")
     return meta
 
 
 def _yuna_put_meta(
     env: lmdb.Environment,
     meta: dict,
 ) -> None:
@@ -259,15 +259,15 @@
     extra_args: Optional[dict]=None,
 ):
     """
     @safety_mode: legal values are 'a' (ACID safety)  'u' (unsafe; fastest)
     """
     if safety_mode not in _VALID_SAFETY_MODES:
         mesg = f"safety_mode must be one of {_VALID_SAFETY_MODES} "\
-            "but instead was {repr(safety_mode)}"
+            "but instead was {safety_mode!r}"
         raise ValueError(mesg)
 
     if not create:
         if not os.path.exists(fname) and not fname.endswith(YUNA_FILE_EXTENSION):
             temp = fname + YUNA_FILE_EXTENSION
             if os.path.exists(fname):
                 fname = temp
```

### Comparing `yuna-db-0.2.3/src/yuna/plugins.py` & `yuna-db-0.2.5/src/yuna/plugins.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.2.3/src/yuna/yuna_repack` & `yuna-db-0.2.5/src/yuna/yuna_repack`

 * *Files identical despite different names*

### Comparing `yuna-db-0.2.3/tests/test_yuna.py` & `yuna-db-0.2.5/tests/test_yuna.py`

 * *Files identical despite different names*

