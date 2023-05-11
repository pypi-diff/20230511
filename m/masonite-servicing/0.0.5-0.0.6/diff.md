# Comparing `tmp/masonite-servicing-0.0.5.tar.gz` & `tmp/masonite-servicing-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masonite-servicing-0.0.5.tar", last modified: Wed May 10 12:15:28 2023, max compression
+gzip compressed data, was "masonite-servicing-0.0.6.tar", last modified: Thu May 11 07:21:19 2023, max compression
```

## Comparing `masonite-servicing-0.0.5.tar` & `masonite-servicing-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 12:15:28.722514 masonite-servicing-0.0.5/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1066 2023-05-09 08:15:50.000000 masonite-servicing-0.0.5/LICENSE
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-09 08:15:50.000000 masonite-servicing-0.0.5/MANIFEST.in
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1616 2023-05-10 12:15:28.722514 masonite-servicing-0.0.5/PKG-INFO
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      360 2023-05-10 10:46:59.000000 masonite-servicing-0.0.5/README.md
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      289 2023-05-09 08:15:50.000000 masonite-servicing-0.0.5/pyproject.toml
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      232 2023-05-10 12:15:28.726514 masonite-servicing-0.0.5/setup.cfg
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     3651 2023-05-10 12:15:03.000000 masonite-servicing-0.0.5/setup.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 12:15:28.722514 masonite-servicing-0.0.5/src/
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 12:15:28.722514 masonite-servicing-0.0.5/src/masonite_servicing/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      909 2023-05-10 12:07:54.000000 masonite-servicing-0.0.5/src/masonite_servicing/__init__.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 12:15:28.722514 masonite-servicing-0.0.5/src/masonite_servicing/config/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      282 2023-05-09 08:15:49.000000 masonite-servicing-0.0.5/src/masonite_servicing/config/servicing.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 12:15:28.722514 masonite-servicing-0.0.5/src/masonite_servicing/providers/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      520 2023-05-09 08:17:14.000000 masonite-servicing-0.0.5/src/masonite_servicing/providers/ServicingProvider.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       69 2023-05-09 08:15:49.000000 masonite-servicing-0.0.5/src/masonite_servicing/providers/__init__.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 12:15:28.722514 masonite-servicing-0.0.5/src/masonite_servicing.egg-info/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1616 2023-05-10 12:15:28.000000 masonite-servicing-0.0.5/src/masonite_servicing.egg-info/PKG-INFO
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      469 2023-05-10 12:15:28.000000 masonite-servicing-0.0.5/src/masonite_servicing.egg-info/SOURCES.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        1 2023-05-10 12:15:28.000000 masonite-servicing-0.0.5/src/masonite_servicing.egg-info/dependency_links.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       80 2023-05-10 12:15:28.000000 masonite-servicing-0.0.5/src/masonite_servicing.egg-info/requires.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       19 2023-05-10 12:15:28.000000 masonite-servicing-0.0.5/src/masonite_servicing.egg-info/top_level.txt
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-11 07:21:19.814609 masonite-servicing-0.0.6/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1066 2023-05-09 08:15:50.000000 masonite-servicing-0.0.6/LICENSE
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-09 08:15:50.000000 masonite-servicing-0.0.6/MANIFEST.in
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1616 2023-05-11 07:21:19.814609 masonite-servicing-0.0.6/PKG-INFO
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      360 2023-05-10 10:46:59.000000 masonite-servicing-0.0.6/README.md
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      289 2023-05-09 08:15:50.000000 masonite-servicing-0.0.6/pyproject.toml
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      232 2023-05-11 07:21:19.814609 masonite-servicing-0.0.6/setup.cfg
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     3651 2023-05-11 07:20:43.000000 masonite-servicing-0.0.6/setup.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-11 07:21:19.802609 masonite-servicing-0.0.6/src/
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-11 07:21:19.802609 masonite-servicing-0.0.6/src/masonite_servicing/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1064 2023-05-11 07:20:31.000000 masonite-servicing-0.0.6/src/masonite_servicing/__init__.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-11 07:21:19.802609 masonite-servicing-0.0.6/src/masonite_servicing/config/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      282 2023-05-09 08:15:49.000000 masonite-servicing-0.0.6/src/masonite_servicing/config/servicing.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-11 07:21:19.802609 masonite-servicing-0.0.6/src/masonite_servicing/providers/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      520 2023-05-09 08:17:14.000000 masonite-servicing-0.0.6/src/masonite_servicing/providers/ServicingProvider.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       69 2023-05-09 08:15:49.000000 masonite-servicing-0.0.6/src/masonite_servicing/providers/__init__.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-11 07:21:19.802609 masonite-servicing-0.0.6/src/masonite_servicing.egg-info/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1616 2023-05-11 07:21:19.000000 masonite-servicing-0.0.6/src/masonite_servicing.egg-info/PKG-INFO
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      469 2023-05-11 07:21:19.000000 masonite-servicing-0.0.6/src/masonite_servicing.egg-info/SOURCES.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        1 2023-05-11 07:21:19.000000 masonite-servicing-0.0.6/src/masonite_servicing.egg-info/dependency_links.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       80 2023-05-11 07:21:19.000000 masonite-servicing-0.0.6/src/masonite_servicing.egg-info/requires.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       19 2023-05-11 07:21:19.000000 masonite-servicing-0.0.6/src/masonite_servicing.egg-info/top_level.txt
```

### Comparing `masonite-servicing-0.0.5/LICENSE` & `masonite-servicing-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `masonite-servicing-0.0.5/PKG-INFO` & `masonite-servicing-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masonite-servicing
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple and small utility library that aids in constructing service feature in Masonite 4.
 Home-page: https://github.com/lvjhn/masonite-servicing
 Author: LJ S.A.
 Author-email: lvjhn.mx@gmail.com
 License: MIT license
 Keywords: Masonite,Python,Development
 Platform: UNKNOWN
```

### Comparing `masonite-servicing-0.0.5/setup.py` & `masonite-servicing-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name="masonite-servicing",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.0.5",
+    version="0.0.6",
     packages=[
         "masonite_servicing",
         "masonite_servicing.providers",
         "masonite_servicing.config",
     ],
     package_dir={"": "src"},
     description="A simple and small utility library that aids in constructing service feature in Masonite 4.",
```

### Comparing `masonite-servicing-0.0.5/src/masonite_servicing/__init__.py` & `masonite-servicing-0.0.6/src/masonite_servicing/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,7 +33,14 @@
 class SampleService:
     def add(self, x, y): 
         return result("ok", "added", x + y) 
     
 def main():
     sample_service = SampleService()
     sample_service.add(3, 5)
+
+def same(res1, res2): 
+    return (
+        res1.status == res2.status and
+        res1.message == res2.message and
+        res1.data == res2.data 
+    )
```

### Comparing `masonite-servicing-0.0.5/src/masonite_servicing/providers/ServicingProvider.py` & `masonite-servicing-0.0.6/src/masonite_servicing/providers/ServicingProvider.py`

 * *Files identical despite different names*

### Comparing `masonite-servicing-0.0.5/src/masonite_servicing.egg-info/PKG-INFO` & `masonite-servicing-0.0.6/src/masonite_servicing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masonite-servicing
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple and small utility library that aids in constructing service feature in Masonite 4.
 Home-page: https://github.com/lvjhn/masonite-servicing
 Author: LJ S.A.
 Author-email: lvjhn.mx@gmail.com
 License: MIT license
 Keywords: Masonite,Python,Development
 Platform: UNKNOWN
```

