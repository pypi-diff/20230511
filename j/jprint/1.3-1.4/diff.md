# Comparing `tmp/jprint-1.3.tar.gz` & `tmp/jprint-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jprint-1.3.tar", max compression
+gzip compressed data, was "jprint-1.4.tar", max compression
```

## Comparing `jprint-1.3.tar` & `jprint-1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1449 2023-04-15 14:20:06.268592 jprint-1.3/README.md
--rw-r--r--   0        0        0       67 2023-04-15 13:54:50.797872 jprint-1.3/jprint/__init__.py
--rw-r--r--   0        0        0     1012 2023-04-30 11:37:34.068427 jprint-1.3/jprint/jprint.py
--rw-r--r--   0        0        0      694 2023-04-30 11:40:53.972767 jprint-1.3/pyproject.toml
--rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 jprint-1.3/PKG-INFO
+-rw-r--r--   0        0        0     1449 2023-04-15 14:20:06.268592 jprint-1.4/README.md
+-rw-r--r--   0        0        0       67 2023-04-15 13:54:50.797872 jprint-1.4/jprint/__init__.py
+-rw-r--r--   0        0        0     1019 2023-05-11 10:52:34.841137 jprint-1.4/jprint/jprint.py
+-rw-r--r--   0        0        0      694 2023-05-11 10:53:18.947363 jprint-1.4/pyproject.toml
+-rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 jprint-1.4/PKG-INFO
```

### Comparing `jprint-1.3/README.md` & `jprint-1.4/README.md`

 * *Files identical despite different names*

### Comparing `jprint-1.3/jprint/jprint.py` & `jprint-1.4/jprint/jprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     kwargs["indent"] = kwargs.get("indent", 4)
     kwargs["default"] = kwargs.get("default", str)
     kwargs["sort_keys"] = kwargs.get("sort_keys", True)
     return json.dumps(obj, **kwargs)
 
 
-def jprint(obj: Union[dict, list, str], **kwargs):
+def jprint(obj: Union[dict, list, tuple, str], **kwargs):
     """
     Pretty print Python dictionaries, lists, and JSON strings.
     If str is not valid json it will be printed as is.
     """
     if isinstance(obj, (dict, list)):
         json_str = format(obj, **kwargs)
     else:
```

### Comparing `jprint-1.3/pyproject.toml` & `jprint-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "jprint"
-version = "1.3"
+version = "1.4"
 authors = [ "John Furr <gnulnx@gmail.com>",]
 description = "A simple JSON and python dictionary pretty printer"
 readme = "README.md"
 license = "MIT"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 
 [tool.poetry.dependencies]
```

### Comparing `jprint-1.3/PKG-INFO` & `jprint-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jprint
-Version: 1.3
+Version: 1.4
 Summary: A simple JSON and python dictionary pretty printer
 License: MIT
 Author: John Furr
 Author-email: gnulnx@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

