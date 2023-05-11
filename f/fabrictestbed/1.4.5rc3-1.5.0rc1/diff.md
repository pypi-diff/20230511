# Comparing `tmp/fabrictestbed-1.4.5rc3.tar.gz` & `tmp/fabrictestbed-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.4.5rc3.tar", last modified: Thu Apr 27 14:51:56 2023, max compression
+gzip compressed data, was "fabrictestbed-1.5.0rc1.tar", last modified: Thu May 11 18:11:42 2023, max compression
```

## Comparing `fabrictestbed-1.4.5rc3.tar` & `fabrictestbed-1.5.0rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1806 2023-04-27 14:50:00.258551 fabrictestbed-1.4.5rc3/.gitignore
--rw-r--r--   0        0        0     1071 2023-04-26 16:15:21.494794 fabrictestbed-1.4.5rc3/LICENSE
--rw-r--r--   0        0        0       24 2023-04-26 16:15:21.494897 fabrictestbed-1.4.5rc3/MANIFEST.in
--rw-r--r--   0        0        0     5603 2023-04-26 16:15:21.495044 fabrictestbed-1.4.5rc3/README.md
--rw-r--r--   0        0        0       25 2023-04-27 14:50:24.559428 fabrictestbed-1.4.5rc3/fabrictestbed/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 16:15:21.495306 fabrictestbed-1.4.5rc3/fabrictestbed/cli/__init__.py
--rw-r--r--   0        0        0    18087 2023-04-26 16:15:21.495535 fabrictestbed-1.4.5rc3/fabrictestbed/cli/cli.py
--rw-r--r--   0        0        0     1452 2023-04-26 16:15:21.495890 fabrictestbed-1.4.5rc3/fabrictestbed/cli/exceptions.py
--rw-r--r--   0        0        0     1914 2023-04-26 16:15:21.496100 fabrictestbed-1.4.5rc3/fabrictestbed/slice_editor/__init__.py
--rw-r--r--   0        0        0      201 2023-04-26 16:15:21.496284 fabrictestbed-1.4.5rc3/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0        0        0    17886 2023-04-27 14:18:44.441875 fabrictestbed-1.4.5rc3/fabrictestbed/slice_manager/slice_manager.py
--rw-r--r--   0        0        0        0 2023-04-26 16:15:21.496579 fabrictestbed-1.4.5rc3/fabrictestbed/util/__init__.py
--rw-r--r--   0        0        0     1452 2023-04-26 16:15:21.496691 fabrictestbed-1.4.5rc3/fabrictestbed/util/constants.py
--rw-r--r--   0        0        0      906 2023-04-27 14:51:49.373381 fabrictestbed-1.4.5rc3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 16:15:21.497061 fabrictestbed-1.4.5rc3/test/__init__.py
--rw-r--r--   0        0        0     2210 2023-04-26 16:15:21.497240 fabrictestbed-1.4.5rc3/test/test_cli.py
--rw-r--r--   0        0        0     6281 1970-01-01 00:00:00.000000 fabrictestbed-1.4.5rc3/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-05-11 17:40:59.099816 fabrictestbed-1.5.0rc1/.gitignore
+-rw-r--r--   0        0        0     1071 2023-05-11 17:40:59.100151 fabrictestbed-1.5.0rc1/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-11 17:40:59.100302 fabrictestbed-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0        0        0     5603 2023-05-11 17:40:59.100450 fabrictestbed-1.5.0rc1/README.md
+-rw-r--r--   0        0        0       25 2023-05-11 18:11:24.842592 fabrictestbed-1.5.0rc1/fabrictestbed/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:40:59.100987 fabrictestbed-1.5.0rc1/fabrictestbed/cli/__init__.py
+-rw-r--r--   0        0        0    18169 2023-05-11 17:40:59.101162 fabrictestbed-1.5.0rc1/fabrictestbed/cli/cli.py
+-rw-r--r--   0        0        0     1452 2023-05-11 17:40:59.101319 fabrictestbed-1.5.0rc1/fabrictestbed/cli/exceptions.py
+-rw-r--r--   0        0        0     1914 2023-05-11 17:40:59.101479 fabrictestbed-1.5.0rc1/fabrictestbed/slice_editor/__init__.py
+-rw-r--r--   0        0        0      201 2023-05-11 17:40:59.101641 fabrictestbed-1.5.0rc1/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0        0        0    17886 2023-05-11 17:40:59.101856 fabrictestbed-1.5.0rc1/fabrictestbed/slice_manager/slice_manager.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:40:59.101985 fabrictestbed-1.5.0rc1/fabrictestbed/util/__init__.py
+-rw-r--r--   0        0        0     1452 2023-05-11 17:40:59.102200 fabrictestbed-1.5.0rc1/fabrictestbed/util/constants.py
+-rw-r--r--   0        0        0      909 2023-05-11 18:03:35.194348 fabrictestbed-1.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 17:40:59.102597 fabrictestbed-1.5.0rc1/test/__init__.py
+-rw-r--r--   0        0        0     2210 2023-05-11 17:40:59.102713 fabrictestbed-1.5.0rc1/test/test_cli.py
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 fabrictestbed-1.5.0rc1/PKG-INFO
```

### Comparing `fabrictestbed-1.4.5rc3/.gitignore` & `fabrictestbed-1.5.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc3/LICENSE` & `fabrictestbed-1.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc3/README.md` & `fabrictestbed-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc3/fabrictestbed/cli/cli.py` & `fabrictestbed-1.5.0rc1/fabrictestbed/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,27 +276,30 @@
 @slices.command()
 @click.option('--cmhost', help='Credmgr Host', default=None)
 @click.option('--ochost', help='Orchestrator Host', default=None)
 @click.option('--tokenlocation', help='location for the tokens', default=None)
 @click.option('--projectid', default=None, help='project name')
 @click.option('--scope', type=click.Choice(['cf', 'mf', 'all'], case_sensitive=False),
               default='all', help='scope')
-@click.option('--sliceid', help='Slice Id', required=True)
+@click.option('--sliceid', help='Slice Id', required=False)
 @click.pass_context
 def delete(ctx, cmhost: str, ochost: str, tokenlocation: str, projectid: str, scope: str, sliceid: str):
     """ Delete slice_editor slice
     """
     try:
         slice_manager = __get_slice_manager(cm_host=cmhost, oc_host=ochost, project_id=projectid, scope=scope,
                                             token_location=tokenlocation)
-        status, response = slice_manager.slices(slice_id=sliceid)
-        if status != Status.OK or isinstance(response, Exception):
-            click.echo(f'Delete Slice failed: {status.interpret(exception=response)}')
-            return
-        slice_object = response[0]
+        slice_object = None
+        if sliceid is not None:
+            status, response = slice_manager.slices(slice_id=sliceid)
+            if status != Status.OK or isinstance(response, Exception):
+                click.echo(f'Delete Slice failed: {status.interpret(exception=response)}')
+                return
+            slice_object = response[0]
+
         status, response = slice_manager.delete(slice_object=slice_object)
 
         if status == Status.OK:
             click.echo(response)
         else:
             click.echo(f'Delete Slice failed: {status.interpret(exception=response)}')
```

### Comparing `fabrictestbed-1.4.5rc3/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.5.0rc1/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc3/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.5.0rc1/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc3/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.5.0rc1/fabrictestbed/slice_manager/slice_manager.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc3/fabrictestbed/util/constants.py` & `fabrictestbed-1.5.0rc1/fabrictestbed/util/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc3/pyproject.toml` & `fabrictestbed-1.5.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 dynamic = ["version"]
 
 keywords = ["Swagger", "FABRIC Python Client Library with CLI"]
 
 requires-python = '>=3.9'
 dependencies = [
     "click",
-    "fabric-credmgr-client==1.3.2",
-    "fabric-orchestrator-client==1.4.5rc2",
+    "fabric-credmgr-client==1.5.0rc1",
+    "fabric-orchestrator-client==1.5.0rc1",
     "paramiko"
     ]
 
 scripts = {"fabric-cli" = "fabrictestbed.cli.cli:cli"}
 
 [project.urls]
 Home = "https://fabric-testbed.net/"
```

### Comparing `fabrictestbed-1.4.5rc3/test/test_cli.py` & `fabrictestbed-1.5.0rc1/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.4.5rc3/PKG-INFO` & `fabrictestbed-1.5.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.4.5rc3
+Version: 1.5.0rc1
 Summary: FABRIC Python Client Library with CLI
 Keywords: Swagger,FABRIC Python Client Library with CLI
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: click
-Requires-Dist: fabric-credmgr-client==1.3.2
-Requires-Dist: fabric-orchestrator-client==1.4.5rc2
+Requires-Dist: fabric-credmgr-client==1.5.0rc1
+Requires-Dist: fabric-orchestrator-client==1.5.0rc1
 Requires-Dist: paramiko
 Project-URL: Home, https://fabric-testbed.net/
 Project-URL: Sources, https://github.com/fabric-testbed/fabric-cli
 
 [![PyPI](https://img.shields.io/pypi/v/fabrictestbed?style=plastic)](https://pypi.org/project/fabrictestbed/)
```

