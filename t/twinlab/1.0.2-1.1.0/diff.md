# Comparing `tmp/twinlab-1.0.2.tar.gz` & `tmp/twinlab-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-1.0.2.tar", max compression
+gzip compressed data, was "twinlab-1.1.0.tar", max compression
```

## Comparing `twinlab-1.0.2.tar` & `twinlab-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1048 2023-04-11 12:00:19.210453 twinlab-1.0.2/README.md
--rw-r--r--   0        0        0      599 2023-04-26 15:55:35.645951 twinlab-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      528 2023-04-19 16:13:39.405689 twinlab-1.0.2/twinlab/__init__.py
--rw-r--r--   0        0        0     4804 2023-04-26 15:55:35.648121 twinlab-1.0.2/twinlab/client.py
--rw-r--r--   0        0        0      505 2023-04-13 16:09:18.757239 twinlab-1.0.2/twinlab/plotting.py
--rw-r--r--   0        0        0      532 2023-04-11 15:58:49.585681 twinlab-1.0.2/twinlab/settings.py
--rw-r--r--   0        0        0     3955 2023-04-26 15:55:35.648860 twinlab-1.0.2/twinlab/utils.py
--rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 twinlab-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1048 2023-04-11 12:00:19.210453 twinlab-1.1.0/README.md
+-rw-r--r--   0        0        0      599 2023-05-11 09:39:31.646748 twinlab-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      528 2023-05-11 09:23:20.908327 twinlab-1.1.0/twinlab/__init__.py
+-rw-r--r--   0        0        0     6650 2023-05-11 09:39:06.665209 twinlab-1.1.0/twinlab/client.py
+-rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.1.0/twinlab/plotting.py
+-rw-r--r--   0        0        0      552 2023-05-10 15:28:55.405307 twinlab-1.1.0/twinlab/settings.py
+-rw-r--r--   0        0        0     3997 2023-05-11 09:39:06.665507 twinlab-1.1.0/twinlab/utils.py
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 twinlab-1.1.0/PKG-INFO
```

### Comparing `twinlab-1.0.2/README.md` & `twinlab-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `twinlab-1.0.2/pyproject.toml` & `twinlab-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "twinlab"
-version = "1.0.2"
+version = "1.1.0"
 description = "Client interface for twinLab"
 authors = ["Alexander Mead <alexander@digilab.co.uk>", "Freddy Wordingham <freddy@digilab.co.uk>"]
 repository = "https://github.com/digiLab-ai/twinLab-client"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.10"
+python = ">=3.9,<3.12"
 pandas = "^1.5.3"
 pydantic = { version = "^1.10.7", extras = ["dotenv"] }
 requests = "^2.28.2"
 
 [tool.poetry.dev-dependencies]
 ipykernel = "^6.22.0"
 IPython = "^8.11"
```

### Comparing `twinlab-1.0.2/twinlab/__init__.py` & `twinlab-1.1.0/twinlab/__init__.py`

 * *Files identical despite different names*

### Comparing `twinlab-1.0.2/twinlab/settings.py` & `twinlab-1.1.0/twinlab/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 class Environment(BaseSettings):
     LOCAL_SERVER: str
     CLOUD_SERVER: str
     GROUP_NAME: str
     USER_NAME: str
+    AUTH_TOKEN: str
 
     class Config:
         env_prefix = ""
         case_sensitive = False
         env_file = ".env"
         env_file_encoding = "utf-8"
```

### Comparing `twinlab-1.0.2/twinlab/utils.py` & `twinlab-1.1.0/twinlab/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 # Project imports
 from .settings import ENV
 
 STANDARD_HEADERS = {
     "X-Group": ENV.GROUP_NAME,
     "X-User": ENV.USER_NAME,
+    "authorizationToken": ENV.AUTH_TOKEN,
 }
 
 TRAIN_CAMPAIGN_CLOUD_URL = "https://4qpjawhm6wlrwe47kigbt2q7j40miizi.lambda-url.eu-west-2.on.aws/"
 
 ### Utility functions ###
```

### Comparing `twinlab-1.0.2/PKG-INFO` & `twinlab-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: twinlab
-Version: 1.0.2
+Version: 1.1.0
 Summary: Client interface for twinLab
 Home-page: https://github.com/digiLab-ai/twinLab-client
 Author: Alexander Mead
 Author-email: alexander@digilab.co.uk
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/digiLab-ai/twinLab-client
 Description-Content-Type: text/markdown
 
 # twinLab Client
```

