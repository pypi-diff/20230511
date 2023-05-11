# Comparing `tmp/ctadata-0.2.5.tar.gz` & `tmp/ctadata-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctadata-0.2.5.tar", max compression
+gzip compressed data, was "ctadata-0.2.6.tar", max compression
```

## Comparing `ctadata-0.2.5.tar` & `ctadata-0.2.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2868 2023-05-05 16:42:21.505294 ctadata-0.2.5/README.md
--rw-r--r--   0        0        0      828 2023-05-05 16:42:21.505294 ctadata-0.2.5/ctadata/__init__.py
--rw-r--r--   0        0        0     4498 2023-05-05 16:42:21.505294 ctadata-0.2.5/ctadata/api.py
--rw-r--r--   0        0        0     1355 2023-05-05 16:42:21.505294 ctadata-0.2.5/ctadata/cli.py
--rw-r--r--   0        0        0      199 2023-05-05 16:42:21.505294 ctadata-0.2.5/ctadata/util.py
--rw-r--r--   0        0        0      369 2023-05-05 16:43:08.137786 ctadata-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 ctadata-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     3026 2023-05-11 14:55:18.314213 ctadata-0.2.6/README.md
+-rw-r--r--   0        0        0      828 2023-05-05 16:42:21.505294 ctadata-0.2.6/ctadata/__init__.py
+-rw-r--r--   0        0        0     5227 2023-05-11 14:54:10.955570 ctadata-0.2.6/ctadata/api.py
+-rw-r--r--   0        0        0     1487 2023-05-11 14:42:48.104116 ctadata-0.2.6/ctadata/cli.py
+-rw-r--r--   0        0        0      199 2023-05-05 16:42:21.505294 ctadata-0.2.6/ctadata/util.py
+-rw-r--r--   0        0        0      369 2023-05-11 14:56:26.788698 ctadata-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3518 1970-01-01 00:00:00.000000 ctadata-0.2.6/PKG-INFO
```

### Comparing `ctadata-0.2.5/README.md` & `ctadata-0.2.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,26 @@
 
 for url in ctadata.list_dir("cta/DL1/20241114/v0.1/"):
     if 'datacheck' not in url and '.0100' in url and '11111' in url:
         print("stored", ctadata.fetch_and_save_file(url)/1024/1024, "Mb")
         print("found keys", h5py.File(url.split("/")[-1]).keys())
 ```
 
+To download a file:
+
+```python
+ctadata.fetch_and_save_file_or_dir("lst/some-data-dir", recursive=True)
+```
+
+or
+
+```bash
+ctadata get -r lst/some-data-dir
+```
+
 ### Uploading files
 
 To upload a file:
 
 ```python
 ctadata.upload_file("latest", "filelists/latest-file-list")
 ```
```

### Comparing `ctadata-0.2.5/ctadata/__init__.py` & `ctadata-0.2.6/ctadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.5/ctadata/api.py` & `ctadata-0.2.6/ctadata/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 logger = logging.getLogger(__name__)
 
 class StorageException(Exception):
     pass
 
 # TODO: move to bravado and rest
 class APIClient:
-    __export_functions__ = ['list_dir', 'fetch_and_save_file', 'upload_file', 'upload_dir']
+    __export_functions__ = ['list_dir', 'fetch_and_save_file', 'upload_file', 'upload_dir', 'fetch_and_save_file_or_dir']
     __class_args__ = ['token', 'downloadservice', 'data_root', 'optional_url_parts', 'chunk_size']
 
     downloadservice = os.getenv("CTADS_URL", "http://hub:5000/services/downloadservice/")
     optional_url_parts = ["services/downloadservice/"]
     
     chunk_size = 10 * 1024 * 1024
 
@@ -99,15 +99,30 @@
                     last_pc = pc
                     
                 out_file.write(r)
                 total_wrote += len(r)
                 i_chunk += 1
 
         return total_wrote
-    
+
+
+    def fetch_and_save_file_or_dir(self, path, recursive=False):
+        if not recursive:
+            return self.fetch_and_save_file(path)
+        else:
+            for entry in self.list_dir(path):
+                if entry['href'] != path:
+                    if entry['type'] == 'file':
+                        logger.info("fetching file %s", entry['href'])
+                        self.fetch_and_save_file(entry['href'], save_to_fn=entry['href'])
+                    else:
+                        logger.info("fetching dir %s", entry['href'])
+                        os.makedirs(entry['href'], exist_ok=True)
+                        self.fetch_and_save_file_or_dir(entry['href'], recursive=True)
+
 
     def upload_file(self, local_fn, path):
         url = self.construct_endpoint_url('upload', path)
         logger.info("uploading %s to %s", local_fn, url)
 
         with open(local_fn, "rb") as f:
             stats = {'total_size': 0}
```

### Comparing `ctadata-0.2.5/ctadata/cli.py` & `ctadata-0.2.6/ctadata/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,17 +28,18 @@
     else:
         logger.warning("problem listing files: %s", r)
 
 
 @cli.command("get")
 @click.pass_context
 @click.argument("path", type=str)
-def get_path(ctx, path):
-    ctx.obj['api'].fetch_and_save_file(path)
-
+@click.option("--recursive", "-r", is_flag=True)
+def get_path(ctx, path, recursive):
+    ctx.obj['api'].fetch_and_save_file_or_dir(path, recursive=recursive)
+    
 
 @cli.command("put")
 @click.pass_context
 @click.argument("local_path", type=click.Path(exists=True))
 @click.argument("path", type=str)
 @click.option("--recursive", "-r", is_flag=True)
 def put_path(ctx, local_path, path, recursive):
@@ -48,8 +49,12 @@
         if recursive:
             ctx.obj['api'].upload_dir(local_path, path)
         else:
             logger.error("can't upload directory without --recursive flag")
 
 
 def main():
-    cli(obj={})
+    cli(obj={})
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `ctadata-0.2.5/PKG-INFO` & `ctadata-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctadata
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Author: Volodymyr Savchenko
 Author-email: contact@volodymyrsavchenko.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -40,14 +40,26 @@
 
 for url in ctadata.list_dir("cta/DL1/20241114/v0.1/"):
     if 'datacheck' not in url and '.0100' in url and '11111' in url:
         print("stored", ctadata.fetch_and_save_file(url)/1024/1024, "Mb")
         print("found keys", h5py.File(url.split("/")[-1]).keys())
 ```
 
+To download a file:
+
+```python
+ctadata.fetch_and_save_file_or_dir("lst/some-data-dir", recursive=True)
+```
+
+or
+
+```bash
+ctadata get -r lst/some-data-dir
+```
+
 ### Uploading files
 
 To upload a file:
 
 ```python
 ctadata.upload_file("latest", "filelists/latest-file-list")
 ```
```

