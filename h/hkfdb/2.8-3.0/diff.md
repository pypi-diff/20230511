# Comparing `tmp/hkfdb-2.8.tar.gz` & `tmp/hkfdb-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-2.8.tar", last modified: Wed May 10 16:06:40 2023, max compression
+gzip compressed data, was "hkfdb-3.0.tar", last modified: Wed May 10 16:09:13 2023, max compression
```

## Comparing `hkfdb-2.8.tar` & `hkfdb-3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 16:06:40.725525 hkfdb-2.8/
--rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-2.8/LICENSE
--rw-rw-rw-   0        0        0     1651 2023-05-10 16:06:40.725525 hkfdb-2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 16:06:40.714491 hkfdb-2.8/hkfdb/
--rw-rw-rw-   0        0        0    93244 2023-05-10 16:04:53.000000 hkfdb-2.8/hkfdb/Database.py
--rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-2.8/hkfdb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:06:40.723524 hkfdb-2.8/hkfdb.egg-info/
--rw-rw-rw-   0        0        0     1651 2023-05-10 16:06:40.000000 hkfdb-2.8/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-05-10 16:06:40.000000 hkfdb-2.8/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 16:06:40.000000 hkfdb-2.8/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-10 16:06:40.000000 hkfdb-2.8/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 16:06:40.000000 hkfdb-2.8/hkfdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 16:06:40.725525 hkfdb-2.8/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-05-10 16:06:05.000000 hkfdb-2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:09:13.502540 hkfdb-3.0/
+-rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-3.0/LICENSE
+-rw-rw-rw-   0        0        0     1651 2023-05-10 16:09:13.501540 hkfdb-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 16:09:13.495873 hkfdb-3.0/hkfdb/
+-rw-rw-rw-   0        0        0    93244 2023-05-10 16:04:53.000000 hkfdb-3.0/hkfdb/Database.py
+-rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-3.0/hkfdb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:09:13.500527 hkfdb-3.0/hkfdb.egg-info/
+-rw-rw-rw-   0        0        0     1651 2023-05-10 16:09:13.000000 hkfdb-3.0/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-05-10 16:09:13.000000 hkfdb-3.0/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 16:09:13.000000 hkfdb-3.0/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-10 16:09:13.000000 hkfdb-3.0/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 16:09:13.000000 hkfdb-3.0/hkfdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 16:09:13.502540 hkfdb-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-05-10 16:08:55.000000 hkfdb-3.0/setup.py
```

### Comparing `hkfdb-2.8/LICENSE` & `hkfdb-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-2.8/PKG-INFO` & `hkfdb-3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 2.8
+Version: 3.0
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hkfdb-2.8/README.md` & `hkfdb-3.0/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-2.8/hkfdb/Database.py` & `hkfdb-3.0/hkfdb/Database.py`

 * *Files identical despite different names*

### Comparing `hkfdb-2.8/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.0/hkfdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 2.8
+Version: 3.0
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hkfdb-2.8/setup.py` & `hkfdb-3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="2.8",
+    version="3.0",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

