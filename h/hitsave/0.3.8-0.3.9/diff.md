# Comparing `tmp/hitsave-0.3.8.tar.gz` & `tmp/hitsave-0.3.9.tar.gz`

## Comparing `hitsave-0.3.8.tar` & `hitsave-0.3.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 hitsave-0.3.8/development.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hitsave-0.3.8/requirements.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/__about__.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/__init__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/__main__.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/authenticate.py
--rw-r--r--   0        0        0    16841 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/blobstore.py
--rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/cli.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/cloudutils.py
--rw-r--r--   0        0        0    22250 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/codegraph.py
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/config.py
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/console.py
--rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/decorator.py
--rw-r--r--   0        0        0    14004 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/evalstore.py
--rw-r--r--   0        0        0    11590 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/filesnap.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/graph.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/session.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/support_extra.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/support_pil.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/support_torch.py
--rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/symbol.py
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/types.py
--rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/visualize.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/util/__init__.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/util/config_file.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/util/current.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/util/dispatch.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/util/misc.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/util/ofdict.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 hitsave-0.3.8/src/hitsave/util/type_helpers.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 hitsave-0.3.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hitsave-0.3.8/LICENSE.txt
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 hitsave-0.3.8/README.md
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 hitsave-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 hitsave-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 hitsave-0.3.9/development.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hitsave-0.3.9/requirements.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/__about__.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/__init__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/__main__.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/authenticate.py
+-rw-r--r--   0        0        0    16841 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/blobstore.py
+-rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/cli.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/cloudutils.py
+-rw-r--r--   0        0        0    22250 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/codegraph.py
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/config.py
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/console.py
+-rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/decorator.py
+-rw-r--r--   0        0        0    14391 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/evalstore.py
+-rw-r--r--   0        0        0    11680 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/filesnap.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/graph.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/session.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/support_extra.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/support_pil.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/support_torch.py
+-rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/symbol.py
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/types.py
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/visualize.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/util/__init__.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/util/config_file.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/util/current.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/util/dispatch.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/util/misc.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/util/ofdict.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 hitsave-0.3.9/src/hitsave/util/type_helpers.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 hitsave-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hitsave-0.3.9/LICENSE.txt
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 hitsave-0.3.9/README.md
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 hitsave-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 hitsave-0.3.9/PKG-INFO
```

### Comparing `hitsave-0.3.8/development.md` & `hitsave-0.3.9/development.md`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/__init__.py` & `hitsave-0.3.9/src/hitsave/__init__.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/authenticate.py` & `hitsave-0.3.9/src/hitsave/authenticate.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/blobstore.py` & `hitsave-0.3.9/src/hitsave/blobstore.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/cli.py` & `hitsave-0.3.9/src/hitsave/cli.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/cloudutils.py` & `hitsave-0.3.9/src/hitsave/cloudutils.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/codegraph.py` & `hitsave-0.3.9/src/hitsave/codegraph.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/config.py` & `hitsave-0.3.9/src/hitsave/config.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/console.py` & `hitsave-0.3.9/src/hitsave/console.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/decorator.py` & `hitsave-0.3.9/src/hitsave/decorator.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/evalstore.py` & `hitsave-0.3.9/src/hitsave/evalstore.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 """
                 CREATE TABLE IF NOT EXISTS evals (
                     id INTEGER PRIMARY KEY,
                     fn_key TEXT NOT NULL,
                     fn_hash TEXT NOT NULL,
                     args_hash TEXT NOT NULL,
                     deps TEXT,
-                    result BLOB,
+                    result_digest BLOB,
                     status INTEGER NOT NULL,
                     start_time TEXT
                 );
             """
             )
             conn.execute(
                 """
@@ -75,29 +75,33 @@
 
     def poll_eval(
         self, key: EvalKey, deps: Dict[Symbol, Binding]
     ) -> Union[PollEvalResult, StoreMiss]:
         with localdb() as conn:
             cur = conn.execute(
                 """
-                SELECT result FROM evals
+                SELECT result_digest FROM evals
                 WHERE fn_key = ? AND fn_hash = ? AND args_hash = ? AND status = ?;
             """,
                 (
                     str(key.fn_key),
                     key.fn_hash,
                     key.args_hash,
                     EvalStatus.resolved.value,
                 ),
             )
             result = cur.fetchall()
             if len(result) != 0:
                 # [todo] orderby start time.
                 try:
-                    value = pickle.loads(result[0][0])
+                    result_digest = result[0][0]
+                    assert isinstance(result_digest, str)
+                    assert len(result_digest) > 0
+                    with BlobStore.current().open_blob(result_digest) as tape:
+                        value = pickle.load(tape)
                     return PollEvalResult(value=value, origin="local")
                 except:
                     msg = f"Corrupted result for {str(key)}"
                     logger.error(msg)
                     return StoreMiss(msg)
 
             cur = conn.execute(
@@ -184,23 +188,28 @@
             return id
 
     def resolve_eval(self, key: EvalKey, *, result: Any, elapsed_process_time: int):
         # [todo] fail with friendly error if the result is not picklable.
         # give a list of suggestions: try saving as a file-snapshot.
         # instructions on how to use the pickling system.
         # if the object is defined in a library, tell us and we can support it!
+        with tempfile.SpooledTemporaryFile() as tape:
+            pickle.dump(result, tape)
+            tape.seek(0)
+            info = BlobStore.current().add_blob(tape)
+
         with localdb() as conn:
             conn.execute(
                 """
                 UPDATE evals
-                SET status = ?, result = ?
+                SET status = ?, result_digest = ?
                 WHERE fn_key = ? AND fn_hash = ? AND args_hash = ? AND status = ?; """,
                 (
                     EvalStatus.resolved.value,
-                    pickle.dumps(result),  # [todo] should go to blob
+                    info.digest,
                     str(key.fn_key),
                     key.fn_hash,
                     key.args_hash,
                     EvalStatus.started.value,
                 ),
             )
             # [todo], if this didn't update anything it means that multiple processes or threads evaluated at the same time!
```

### Comparing `hitsave-0.3.8/src/hitsave/filesnap.py` & `hitsave-0.3.9/src/hitsave/filesnap.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,18 @@
         if self.suffix != path.suffix:
             raise ValueError(
                 f"Refusing to write to {path} since the extension name is different to extension of {self.relpath}"
             )
         if path.is_symlink():
             # [todo] if it links to our local cache then this is fine.
             # double check that the file exists
-            logger.warn(f"restore over a symlink not implemented. {path}")
+            linkpath = path.resolve()
+            if linkpath == self.local_cache_path:
+                logger.debug("already restored")
+                return path
             pass
         if path.exists():
             if overwrite is False:
                 raise FileExistsError(
                     f"Refusing to restore: would overwrite {path} and overwrite is set to False."
                 )
             else:
```

### Comparing `hitsave-0.3.8/src/hitsave/graph.py` & `hitsave-0.3.9/src/hitsave/graph.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/session.py` & `hitsave-0.3.9/src/hitsave/session.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/support_pil.py` & `hitsave-0.3.9/src/hitsave/support_pil.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/symbol.py` & `hitsave-0.3.9/src/hitsave/symbol.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/types.py` & `hitsave-0.3.9/src/hitsave/types.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/visualize.py` & `hitsave-0.3.9/src/hitsave/visualize.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/util/config_file.py` & `hitsave-0.3.9/src/hitsave/util/config_file.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/util/current.py` & `hitsave-0.3.9/src/hitsave/util/current.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/util/dispatch.py` & `hitsave-0.3.9/src/hitsave/util/dispatch.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/util/misc.py` & `hitsave-0.3.9/src/hitsave/util/misc.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/util/ofdict.py` & `hitsave-0.3.9/src/hitsave/util/ofdict.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/src/hitsave/util/type_helpers.py` & `hitsave-0.3.9/src/hitsave/util/type_helpers.py`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/.gitignore` & `hitsave-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/LICENSE.txt` & `hitsave-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/README.md` & `hitsave-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/pyproject.toml` & `hitsave-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hitsave-0.3.8/PKG-INFO` & `hitsave-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hitsave
-Version: 0.3.8
+Version: 0.3.9
 Summary: Holistic data caching system.
 Project-URL: Homepage, https://hitsave.io
 Project-URL: Bug Tracker, https://github.com/hitsave-io/xyz/issues
 Project-URL: Documentation, https://docs.hitsave.io
 Author-email: "E.W.Ayers" <contact@edayers.com>, George Seabridge <seabo@hitsave.io>
 License-Expression: MIT
 License-File: LICENSE.txt
```

