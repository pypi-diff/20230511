# Comparing `tmp/disklru-1.0.1.tar.gz` & `tmp/disklru-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disklru-1.0.1.tar", last modified: Wed May 10 23:24:18 2023, max compression
+gzip compressed data, was "disklru-1.0.2.tar", last modified: Thu May 11 01:43:07 2023, max compression
```

## Comparing `disklru-1.0.1.tar` & `disklru-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 23:24:18.006829 disklru-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-10 23:24:17.954831 disklru-1.0.1/.github/
-drwxrwxrwx   0        0        0        0 2023-05-10 23:24:17.979830 disklru-1.0.1/.github/workflows/
--rw-rw-rw-   0        0        0      855 2023-05-10 22:45:22.000000 disklru-1.0.1/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      801 2023-05-10 22:45:22.000000 disklru-1.0.1/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      803 2023-05-10 22:45:22.000000 disklru-1.0.1/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0      800 2023-05-10 22:45:22.000000 disklru-1.0.1/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     1914 2023-05-10 22:45:22.000000 disklru-1.0.1/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-10 23:24:17.983831 disklru-1.0.1/.vscode/
--rw-rw-rw-   0        0        0     1354 2023-05-10 22:45:22.000000 disklru-1.0.1/.vscode/launch.json
--rw-rw-rw-   0        0        0      819 2023-05-10 22:45:22.000000 disklru-1.0.1/.vscode/settings.json
--rw-rw-rw-   0        0        0     1109 2023-05-10 22:45:22.000000 disklru-1.0.1/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1064 2023-05-10 22:45:22.000000 disklru-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      102 2023-05-10 22:45:22.000000 disklru-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1542 2023-05-10 23:24:18.005830 disklru-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      862 2023-05-10 22:59:34.000000 disklru-1.0.1/README.md
--rw-rw-rw-   0        0        0      415 2023-05-10 22:46:08.000000 disklru-1.0.1/activate.sh
--rw-rw-rw-   0        0        0      435 2023-05-10 22:45:22.000000 disklru-1.0.1/lint.sh
--rw-rw-rw-   0        0        0     2138 2023-05-10 22:45:22.000000 disklru-1.0.1/make_venv.py
--rw-rw-rw-   0        0        0      712 2023-05-10 23:23:33.000000 disklru-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       47 2023-05-10 22:45:22.000000 disklru-1.0.1/requirements.testing.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 23:24:18.006829 disklru-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1090 2023-05-10 22:45:22.000000 disklru-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 23:24:17.957831 disklru-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 23:24:17.985832 disklru-1.0.1/src/disklru/
--rw-rw-rw-   0        0        0       92 2023-05-10 22:45:22.000000 disklru-1.0.1/src/disklru/__init__.py
--rw-rw-rw-   0        0        0     3094 2023-05-10 23:22:28.000000 disklru-1.0.1/src/disklru/disklru.py
-drwxrwxrwx   0        0        0        0 2023-05-10 23:24:18.003828 disklru-1.0.1/src/disklru.egg-info/
--rw-rw-rw-   0        0        0     1542 2023-05-10 23:24:17.000000 disklru-1.0.1/src/disklru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-05-10 23:24:17.000000 disklru-1.0.1/src/disklru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 23:24:17.000000 disklru-1.0.1/src/disklru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 23:24:17.000000 disklru-1.0.1/src/disklru.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 23:24:18.004829 disklru-1.0.1/tests/
--rw-rw-rw-   0        0        0     2717 2023-05-10 22:45:22.000000 disklru-1.0.1/tests/test_disklru.py
--rw-rw-rw-   0        0        0      498 2023-05-10 22:45:22.000000 disklru-1.0.1/tox.ini
--rw-rw-rw-   0        0        0      291 2023-05-10 22:45:22.000000 disklru-1.0.1/upload_package.sh
+drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.781341 disklru-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.698341 disklru-1.0.2/.github/
+drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.750340 disklru-1.0.2/.github/workflows/
+-rw-rw-rw-   0        0        0      855 2023-05-10 22:45:22.000000 disklru-1.0.2/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      801 2023-05-10 22:45:22.000000 disklru-1.0.2/.github/workflows/push_macos.yml
+-rw-rw-rw-   0        0        0      803 2023-05-10 22:45:22.000000 disklru-1.0.2/.github/workflows/push_ubuntu.yml
+-rw-rw-rw-   0        0        0      800 2023-05-10 22:45:22.000000 disklru-1.0.2/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     1914 2023-05-10 22:45:22.000000 disklru-1.0.2/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.754344 disklru-1.0.2/.vscode/
+-rw-rw-rw-   0        0        0     1354 2023-05-10 22:45:22.000000 disklru-1.0.2/.vscode/launch.json
+-rw-rw-rw-   0        0        0      819 2023-05-10 22:45:22.000000 disklru-1.0.2/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1109 2023-05-10 22:45:22.000000 disklru-1.0.2/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1064 2023-05-10 22:45:22.000000 disklru-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      102 2023-05-10 22:45:22.000000 disklru-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1542 2023-05-11 01:43:07.780341 disklru-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2023-05-10 22:59:34.000000 disklru-1.0.2/README.md
+-rw-rw-rw-   0        0        0      415 2023-05-10 22:46:08.000000 disklru-1.0.2/activate.sh
+-rw-rw-rw-   0        0        0      435 2023-05-10 22:45:22.000000 disklru-1.0.2/lint.sh
+-rw-rw-rw-   0        0        0     2138 2023-05-10 22:45:22.000000 disklru-1.0.2/make_venv.py
+-rw-rw-rw-   0        0        0      712 2023-05-11 01:42:54.000000 disklru-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       47 2023-05-10 22:45:22.000000 disklru-1.0.2/requirements.testing.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 01:43:07.781341 disklru-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2023-05-10 22:45:22.000000 disklru-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.700342 disklru-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.757341 disklru-1.0.2/src/disklru/
+-rw-rw-rw-   0        0        0       92 2023-05-10 22:45:22.000000 disklru-1.0.2/src/disklru/__init__.py
+-rw-rw-rw-   0        0        0     3641 2023-05-11 01:42:19.000000 disklru-1.0.2/src/disklru/disklru.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.778342 disklru-1.0.2/src/disklru.egg-info/
+-rw-rw-rw-   0        0        0     1542 2023-05-11 01:43:07.000000 disklru-1.0.2/src/disklru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-05-11 01:43:07.000000 disklru-1.0.2/src/disklru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 01:43:07.000000 disklru-1.0.2/src/disklru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-11 01:43:07.000000 disklru-1.0.2/src/disklru.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 01:43:07.779340 disklru-1.0.2/tests/
+-rw-rw-rw-   0        0        0     2943 2023-05-11 01:41:53.000000 disklru-1.0.2/tests/test_disklru.py
+-rw-rw-rw-   0        0        0      498 2023-05-10 22:45:22.000000 disklru-1.0.2/tox.ini
+-rw-rw-rw-   0        0        0      291 2023-05-10 22:45:22.000000 disklru-1.0.2/upload_package.sh
```

### Comparing `disklru-1.0.1/.github/workflows/lint.yml` & `disklru-1.0.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/.github/workflows/push_macos.yml` & `disklru-1.0.2/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/.github/workflows/push_ubuntu.yml` & `disklru-1.0.2/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/.github/workflows/push_win.yml` & `disklru-1.0.2/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/.gitignore` & `disklru-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/.vscode/launch.json` & `disklru-1.0.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/.vscode/settings.json` & `disklru-1.0.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/.vscode/tasks.json` & `disklru-1.0.2/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/LICENSE` & `disklru-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/PKG-INFO` & `disklru-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disklru
-Version: 1.0.1
+Version: 1.0.2
 Summary: Creates a python disk LRU / cache - great for apps that want to save data
 Home-page: https://github.com/zackees/disklru
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `disklru-1.0.1/README.md` & `disklru-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/make_venv.py` & `disklru-1.0.2/make_venv.py`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/pyproject.toml` & `disklru-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 keywords = ["template-python-cmd"]
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
 ]
 # Change this with the version number bump.
 # Also make the change in zcmds/version.py
-version = "1.0.1"
+version = "1.0.2"
 
 [tool.ruff]
 line-length = 200
 
 [tool.pylint."MESSAGES CONTROL"]
 good-names = [
     "c",
```

### Comparing `disklru-1.0.1/setup.py` & `disklru-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/src/disklru/disklru.py` & `disklru-1.0.2/src/disklru/disklru.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 Disk-based LRU cache using SQLite.
 """
 
+import json
 import os
 import sqlite3
 from datetime import datetime
+from typing import Any
 
 # pylint: disable=line-too-long
 
 
 class DiskLRUCache:
     """Disk-based LRU cache using SQLite."""
 
-    def __init__(self, db_path, max_size):
+    def __init__(self, db_path: str, max_size: str) -> None:
         """Initializes the cache."""
         os.makedirs(os.path.dirname(db_path), exist_ok=True)
         self.conn = sqlite3.connect(db_path)
         self.closed = False
         self.cursor = self.conn.cursor()
         self.cursor.execute(
             """
@@ -30,29 +32,36 @@
         self.cursor.execute(
             "CREATE INDEX IF NOT EXISTS idx_timestamp ON cache (timestamp);"
         )
         self.cursor.execute("CREATE INDEX IF NOT EXISTS idx_key ON cache (key);")
         self.conn.commit()
         self.max_size = max_size
 
-    def get(self, key):
+    def get(self, key: str) -> str | None:
         """Returns the value associated with the given key, or None if the key is not in the cache."""
         assert not self.closed
         self.cursor.execute("SELECT value FROM cache WHERE key=?", (key,))
         result = self.cursor.fetchone()
         if result is not None:
             self.cursor.execute(
                 "UPDATE cache SET timestamp=? WHERE key=?",
                 (int(datetime.now().timestamp()), key),
             )
             self.conn.commit()
             return result[0]
         return None
 
-    def put(self, key, value):
+    def get_json(self, key: str) -> Any:
+        """Returns the value associated with the given key, or None if the key is not in the cache."""
+        result = self.get(key)
+        if result is not None:
+            return json.loads(result)
+        return None
+
+    def put(self, key: str, value: str) -> None:
         """Sets the value associated with the given key."""
         assert not self.closed
         self.cursor.execute("SELECT COUNT(*) FROM cache")
         if self.cursor.fetchone()[0] >= self.max_size:
             # Delete the least recently used item
             self.cursor.execute("SELECT key FROM cache ORDER BY timestamp ASC LIMIT 1")
             lru_key = self.cursor.fetchone()[0]
@@ -61,34 +70,38 @@
         timestamp = int(datetime.now().timestamp())
         self.cursor.execute(
             "INSERT OR REPLACE INTO cache (key, timestamp, value) VALUES (?, ?, ?)",
             (key, timestamp, value),
         )
         self.conn.commit()
 
-    def delete(self, key):
+    def put_json(self, key: str, val: Any) -> None:
+        """Sets the value associated with the given key."""
+        self.put(key, json.dumps(val))
+
+    def delete(self, key) -> None:
         """Deletes the given key from the cache."""
         assert not self.closed
         self.cursor.execute("DELETE FROM cache WHERE key=?", (key,))
         self.conn.commit()
 
-    def purge(self, timestamp):
+    def purge(self, timestamp) -> None:
         """Purges all elements less than the timestamp."""
         assert not self.closed
         self.cursor.execute("DELETE FROM cache WHERE timestamp<?", (timestamp,))
         self.conn.commit()
 
-    def clear(self):
+    def clear(self) -> None:
         """Clears the cache."""
         assert not self.closed
         self.cursor.execute("DELETE FROM cache")
         self.conn.commit()
 
-    def __del__(self):
+    def __del__(self) -> None:
         """Destructor."""
         self.close()
 
-    def close(self):
+    def close(self) -> None:
         """Closes the connection to the database."""
         if not self.closed:
             self.conn.close()
             self.closed = True
```

### Comparing `disklru-1.0.1/src/disklru.egg-info/PKG-INFO` & `disklru-1.0.2/src/disklru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disklru
-Version: 1.0.1
+Version: 1.0.2
 Summary: Creates a python disk LRU / cache - great for apps that want to save data
 Home-page: https://github.com/zackees/disklru
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `disklru-1.0.1/src/disklru.egg-info/SOURCES.txt` & `disklru-1.0.2/src/disklru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disklru-1.0.1/tests/test_disklru.py` & `disklru-1.0.2/tests/test_disklru.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,10 +75,15 @@
         # "key1" should be evicted, and the rest should be present.
         self.assertIsNone(self.cache.get("key1"))
         self.assertIsNotNone(self.cache.get("key2"))
         self.assertIsNotNone(self.cache.get("key3"))
         self.assertIsNotNone(self.cache.get("key4"))
         self.assertIsNotNone(self.cache.get("key5"))
 
+    def test_json(self) -> None:
+        """Tests that the cache can store and retrieve JSON objects."""
+        self.cache.put_json("key", {"foo": "bar"})
+        self.assertEqual(self.cache.get_json("key"), {"foo": "bar"})
+
 
 if __name__ == "__main__":
     unittest.main()
```

