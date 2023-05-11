# Comparing `tmp/spei_python-0.5.36.tar.gz` & `tmp/spei_python-0.5.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spei_python-0.5.36.tar", max compression
+gzip compressed data, was "spei_python-0.5.37.tar", max compression
```

## Comparing `spei_python-0.5.36.tar` & `spei_python-0.5.37.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.5.36/README.md
--rw-r--r--   0        0        0      859 2023-04-18 22:11:47.558953 spei_python-0.5.36/pyproject.toml
--rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.5.36/spei/__init__.py
--rw-r--r--   0        0        0     2731 2023-03-09 23:20:37.585774 spei_python-0.5.36/spei/client.py
--rw-r--r--   0        0        0       66 2023-02-28 22:07:27.969521 spei_python-0.5.36/spei/resources/__init__.py
--rw-r--r--   0        0        0     3962 2023-03-13 22:05:56.750212 spei_python-0.5.36/spei/resources/ordenes.py
--rw-r--r--   0        0        0     1703 2023-03-13 21:54:51.240999 spei_python-0.5.36/spei/types.py
--rw-r--r--   0        0        0     2289 2023-03-13 22:05:00.658624 spei_python-0.5.36/spei/utils.py
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 spei_python-0.5.36/PKG-INFO
+-rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.5.37/README.md
+-rw-r--r--   0        0        0      859 2023-05-11 17:12:03.608832 spei_python-0.5.37/pyproject.toml
+-rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.5.37/spei/__init__.py
+-rw-r--r--   0        0        0     2739 2023-05-11 17:06:18.833865 spei_python-0.5.37/spei/client.py
+-rw-r--r--   0        0        0       66 2023-02-28 22:07:27.969521 spei_python-0.5.37/spei/resources/__init__.py
+-rw-r--r--   0        0        0     3962 2023-03-13 22:05:56.750212 spei_python-0.5.37/spei/resources/ordenes.py
+-rw-r--r--   0        0        0     1703 2023-03-13 21:54:51.240999 spei_python-0.5.37/spei/types.py
+-rw-r--r--   0        0        0     2289 2023-03-13 22:05:00.658624 spei_python-0.5.37/spei/utils.py
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 spei_python-0.5.37/PKG-INFO
```

### Comparing `spei_python-0.5.36/README.md` & `spei_python-0.5.37/README.md`

 * *Files identical despite different names*

### Comparing `spei_python-0.5.36/pyproject.toml` & `spei_python-0.5.37/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spei-python"
-version = "0.5.36"
+version = "0.5.37"
 description = ""
 authors = ["gonz <gonzasestopal@gmail.com>"]
 readme = "README.md"
 packages = [{include = "spei"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
@@ -27,14 +27,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.36"
+version = "0.5.37"
 tag_format = "v$version"
 bump_message = "bump: Semantic Release Bot: Release Version: $new_version 🤖🚀 [skip ci]"
 version_files = [
     "pyproject.toml:version",
 ]
```

### Comparing `spei_python-0.5.36/spei/client.py` & `spei_python-0.5.37/spei/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 class BaseClient(object):
 
     def __init__(
         self,
         priv_key,
         priv_key_passphrase,
         host,
-        user,
+        username,
         password,
         verify=False,
         http_client=requests,
     ):
         self.priv_key = priv_key
         self.priv_key_passphrase = priv_key_passphrase or None
         self.host = host
         self.session = http_client.Session()
         self.session.headers.update({'Content-Type': 'application/xml'})
         self.session.verify = verify
-        self.session.auth = (user, password)
+        self.session.auth = (username, password)
 
         if priv_key_passphrase:
             self.priv_key_passphrase = priv_key_passphrase.encode('ascii')
 
         self.pkey = serialization.load_pem_private_key(
             self.priv_key.encode('utf-8'),
             self.priv_key_passphrase,
```

### Comparing `spei_python-0.5.36/spei/resources/ordenes.py` & `spei_python-0.5.37/spei/resources/ordenes.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.5.36/spei/types.py` & `spei_python-0.5.37/spei/types.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.5.36/spei/utils.py` & `spei_python-0.5.37/spei/utils.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.5.36/PKG-INFO` & `spei_python-0.5.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spei-python
-Version: 0.5.36
+Version: 0.5.37
 Summary: 
 Author: gonz
 Author-email: gonzasestopal@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

