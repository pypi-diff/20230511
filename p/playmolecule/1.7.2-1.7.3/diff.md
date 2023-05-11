# Comparing `tmp/playmolecule-1.7.2.tar.gz` & `tmp/playmolecule-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.7.2.tar", last modified: Wed May  3 16:50:45 2023, max compression
+gzip compressed data, was "playmolecule-1.7.3.tar", last modified: Thu May 11 10:50:54 2023, max compression
```

## Comparing `playmolecule-1.7.2.tar` & `playmolecule-1.7.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:50:45.916590 playmolecule-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-03 16:50:26.000000 playmolecule-1.7.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-03 16:50:26.000000 playmolecule-1.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-03 16:50:45.916590 playmolecule-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-03 16:50:26.000000 playmolecule-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:50:45.916590 playmolecule-1.7.2/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 16:50:45.916590 playmolecule-1.7.2/playmolecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    33507 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/func2argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-03 16:50:26.000000 playmolecule-1.7.2/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:50:45.916590 playmolecule-1.7.2/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-03 16:50:45.000000 playmolecule-1.7.2/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-03 16:50:45.000000 playmolecule-1.7.2/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:50:45.000000 playmolecule-1.7.2/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:50:45.000000 playmolecule-1.7.2/playmolecule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 16:50:45.000000 playmolecule-1.7.2/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 16:50:45.000000 playmolecule-1.7.2/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-03 16:50:26.000000 playmolecule-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:50:45.916590 playmolecule-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 16:50:26.000000 playmolecule-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:50:45.916590 playmolecule-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-03 16:50:26.000000 playmolecule-1.7.2/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-03 16:50:26.000000 playmolecule-1.7.2/tests/test_app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-03 16:50:26.000000 playmolecule-1.7.2/tests/test_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-03 16:50:26.000000 playmolecule-1.7.2/tests/test_func_to_argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:50:54.421156 playmolecule-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-11 10:50:35.000000 playmolecule-1.7.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 10:50:35.000000 playmolecule-1.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-11 10:50:54.421156 playmolecule-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-11 10:50:35.000000 playmolecule-1.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:50:54.421156 playmolecule-1.7.3/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-11 10:50:54.421156 playmolecule-1.7.3/playmolecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33630 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/func2argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-11 10:50:35.000000 playmolecule-1.7.3/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:50:54.421156 playmolecule-1.7.3/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-11 10:50:54.000000 playmolecule-1.7.3/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-11 10:50:54.000000 playmolecule-1.7.3/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:50:54.000000 playmolecule-1.7.3/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:50:54.000000 playmolecule-1.7.3/playmolecule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 10:50:54.000000 playmolecule-1.7.3/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 10:50:54.000000 playmolecule-1.7.3/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-11 10:50:35.000000 playmolecule-1.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 10:50:54.421156 playmolecule-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 10:50:35.000000 playmolecule-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:50:54.421156 playmolecule-1.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-11 10:50:35.000000 playmolecule-1.7.3/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-11 10:50:35.000000 playmolecule-1.7.3/tests/test_app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-11 10:50:35.000000 playmolecule-1.7.3/tests/test_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-11 10:50:35.000000 playmolecule-1.7.3/tests/test_func_to_argparse.py
```

### Comparing `playmolecule-1.7.2/LICENSE.md` & `playmolecule-1.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/PKG-INFO` & `playmolecule-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.7.2
+Version: 1.7.3
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.7.2/playmolecule/__init__.py` & `playmolecule-1.7.3/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/playmolecule/_test_funcs.py` & `playmolecule-1.7.3/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/playmolecule/config.py` & `playmolecule-1.7.3/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/playmolecule/datacenter.py` & `playmolecule-1.7.3/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/playmolecule/devutils.py` & `playmolecule-1.7.3/playmolecule/devutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,18 +428,24 @@
     _pm_try_except(func, SESSION, JOB, standalone, args.debug, args)
 
     if not standalone:
         # set the complete status of the job
         setAsCompleted(args.outdir)
 
 
-def _write_argparser_json(outfile, parser):
+def write_argparser_json(outfile, parser):
     from collections import OrderedDict
     import json
 
+    if not os.path.exists(outfile):
+        manifest = OrderedDict()
+    else:
+        with open(outfile, "r") as f:
+            manifest = json.load(f)
+
     parserargs = []
     parseractions = parser._actions
 
     for action in parseractions:
         # skip the hidden arguments, the excluded args and the help argument
         if action.help == "==SUPPRESS==" or action.dest in ("help",):
             continue
@@ -452,15 +458,14 @@
         actiondict["description"] = action.help
         actiondict["nargs"] = action.nargs if action.nargs != 0 else None
         actiondict["choices"] = action.choices
         actiondict["metavar"] = action.metavar
 
         parserargs.append(actiondict)
 
-    manifest = OrderedDict()
     manifest["description"] = parser.description
     manifest["params"] = parserargs
 
     with open(outfile, "w") as f:
         json.dump(manifest, f, indent=4)
 
 
@@ -578,15 +583,15 @@
     # Import the module/function of the app to call
     pieces = func.split(".")
     top_module = pieces[0]
     module = ".".join(pieces[:-1])
     func = getattr(importlib.import_module(module), pieces[-1])
     parser = func_to_argparser(func)
     if dump_argparser is not None:
-        _write_argparser_json(dump_argparser, parser)
+        write_argparser_json(dump_argparser, parser)
         return
 
     if token is None:
         if input_json is not None:
             with open(input_json, "r") as f:
                 params = json.load(f)
         else:
```

### Comparing `playmolecule-1.7.2/playmolecule/func2argparse.py` & `playmolecule-1.7.3/playmolecule/func2argparse.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/playmolecule/job.py` & `playmolecule-1.7.3/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/playmolecule/jsonlogger.py` & `playmolecule-1.7.3/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/playmolecule/local.py` & `playmolecule-1.7.3/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/playmolecule/playqueue.py` & `playmolecule-1.7.3/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/playmolecule/session.py` & `playmolecule-1.7.3/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/playmolecule/utils.py` & `playmolecule-1.7.3/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.7.3/playmolecule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.7.2
+Version: 1.7.3
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.7.2/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.7.3/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/pyproject.toml` & `playmolecule-1.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/tests/test.py` & `playmolecule-1.7.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/tests/test_app_wrapper.py` & `playmolecule-1.7.3/tests/test_app_wrapper.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/tests/test_datacenter.py` & `playmolecule-1.7.3/tests/test_datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.2/tests/test_func_to_argparse.py` & `playmolecule-1.7.3/tests/test_func_to_argparse.py`

 * *Files identical despite different names*

