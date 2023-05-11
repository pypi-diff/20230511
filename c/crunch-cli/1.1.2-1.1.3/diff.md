# Comparing `tmp/crunch-cli-1.1.2.tar.gz` & `tmp/crunch-cli-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.1.2.tar", last modified: Thu May 11 10:18:14 2023, max compression
+gzip compressed data, was "crunch-cli-1.1.3.tar", last modified: Thu May 11 15:41:58 2023, max compression
```

## Comparing `crunch-cli-1.1.2.tar` & `crunch-cli-1.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:18:14.329499 crunch-cli-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-11 10:18:14.329499 crunch-cli-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:18:14.325499 crunch-cli-1.1.2/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:18:14.325499 crunch-cli-1.1.2/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:18:14.325499 crunch-cli-1.1.2/crunch/demo-project/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/demo-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/demo-project/files.json
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/demo-project/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/demo-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:18:14.329499 crunch-cli-1.1.2/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-11 10:18:14.000000 crunch-cli-1.1.2/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-11 10:18:14.000000 crunch-cli-1.1.2/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:18:14.000000 crunch-cli-1.1.2/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 10:18:14.000000 crunch-cli-1.1.2/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:18:14.000000 crunch-cli-1.1.2/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:18:14.000000 crunch-cli-1.1.2/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 10:18:14.000000 crunch-cli-1.1.2/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 10:18:14.329499 crunch-cli-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-11 10:18:06.000000 crunch-cli-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:41:58.201945 crunch-cli-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-11 15:41:58.201945 crunch-cli-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:41:58.197945 crunch-cli-1.1.3/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:41:58.197945 crunch-cli-1.1.3/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:41:58.201945 crunch-cli-1.1.3/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:41:58.201945 crunch-cli-1.1.3/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-11 15:41:58.000000 crunch-cli-1.1.3/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-11 15:41:58.000000 crunch-cli-1.1.3/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:41:58.000000 crunch-cli-1.1.3/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 15:41:58.000000 crunch-cli-1.1.3/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:41:58.000000 crunch-cli-1.1.3/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 15:41:58.000000 crunch-cli-1.1.3/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 15:41:58.000000 crunch-cli-1.1.3/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:41:58.201945 crunch-cli-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-11 15:41:52.000000 crunch-cli-1.1.3/setup.py
```

### Comparing `crunch-cli-1.1.2/crunch/command/convert.py` & `crunch-cli-1.1.3/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/crunch/command/download.py` & `crunch-cli-1.1.3/crunch/command/download.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/crunch/command/push.py` & `crunch-cli-1.1.3/crunch/command/push.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/crunch/command/setup.py` & `crunch-cli-1.1.3/crunch/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/crunch/command/test.py` & `crunch-cli-1.1.3/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/crunch/constants.py` & `crunch-cli-1.1.3/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/crunch/demo-project/.gitignore` & `crunch-cli-1.1.3/crunch/demo-project/.gitignore`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/crunch/demo-project/main.py` & `crunch-cli-1.1.3/crunch/demo-project/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/crunch/ensure.py` & `crunch-cli-1.1.3/crunch/ensure.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         logging.error(f"`%s` must be a dataframe", name)
         raise click.Abort()
 
 
 def return_infer(result) -> pandas.DataFrame:
     is_dataframe(result, "prediction")
 
-    expected = ["id", "date", "value"]
-    got: typing.List[str] = list(result.columns)
+    expected = {"id", "date", "value"}
+    got: typing.Set[str] = set(result.columns)
 
     if got != expected:
         logging.error(f"prediction expected columns: `{expected}` but got `{got}`")
         raise click.Abort()
 
     return result
```

### Comparing `crunch-cli-1.1.2/crunch/inline.py` & `crunch-cli-1.1.3/crunch/inline.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/crunch/main.py` & `crunch-cli-1.1.3/crunch/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/crunch/tester.py` & `crunch-cli-1.1.3/crunch/tester.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/crunch/utils.py` & `crunch-cli-1.1.3/crunch/utils.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.1.3/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.1.2/setup.py` & `crunch-cli-1.1.3/setup.py`

 * *Files identical despite different names*

