# Comparing `tmp/oscar_python-1.0.4.tar.gz` & `tmp/oscar_python-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oscar_python-1.0.4.tar", last modified: Fri May  5 09:48:09 2023, max compression
+gzip compressed data, was "oscar_python-1.1.0b1.tar", last modified: Thu May 11 08:09:28 2023, max compression
```

## Comparing `oscar_python-1.0.4.tar` & `oscar_python-1.1.0b1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:09.684764 oscar_python-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-05 09:47:59.000000 oscar_python-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-05 09:48:09.684764 oscar_python-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-05 09:47:59.000000 oscar_python-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:09.684764 oscar_python-1.0.4/oscar_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:09.684764 oscar_python-1.0.4/oscar_python/_providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/_providers/_minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/_providers/_onedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/_providers/_providers_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/_providers/_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/_providers/_webdav.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:09.684764 oscar_python-1.0.4/oscar_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-05 09:48:09.000000 oscar_python-1.0.4/oscar_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-05 09:48:09.000000 oscar_python-1.0.4/oscar_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:48:09.000000 oscar_python-1.0.4/oscar_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:48:09.000000 oscar_python-1.0.4/oscar_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 09:48:09.000000 oscar_python-1.0.4/oscar_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 09:48:09.000000 oscar_python-1.0.4/oscar_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:48:09.684764 oscar_python-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-05 09:47:59.000000 oscar_python-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:28.925472 oscar_python-1.1.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-11 08:09:28.925472 oscar_python-1.1.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:28.925472 oscar_python-1.1.0b1/oscar_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:28.925472 oscar_python-1.1.0b1/oscar_python/_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/_providers/_minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/_providers/_onedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/_providers/_providers_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/_providers/_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/_providers/_webdav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:28.925472 oscar_python-1.1.0b1/oscar_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-11 08:09:28.000000 oscar_python-1.1.0b1/oscar_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-11 08:09:28.000000 oscar_python-1.1.0b1/oscar_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:09:28.000000 oscar_python-1.1.0b1/oscar_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:09:28.000000 oscar_python-1.1.0b1/oscar_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 08:09:28.000000 oscar_python-1.1.0b1/oscar_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 08:09:28.000000 oscar_python-1.1.0b1/oscar_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:09:28.925472 oscar_python-1.1.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/setup.py
```

### Comparing `oscar_python-1.0.4/LICENSE` & `oscar_python-1.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.4/PKG-INFO` & `oscar_python-1.1.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscar_python
-Version: 1.0.4
+Version: 1.1.0b1
 Summary: OSCAR API for python
 Home-page: https://github.com/grycap/oscar_python
 Author: GRyCAP - Universitat Politecnica de Valencia
 Author-email: calarcon@i3m.upv.es
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `oscar_python-1.0.4/README.md` & `oscar_python-1.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.4/oscar_python/_providers/_minio.py` & `oscar_python-1.1.0b1/oscar_python/_providers/_minio.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.4/oscar_python/_providers/_onedata.py` & `oscar_python-1.1.0b1/oscar_python/_providers/_onedata.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.4/oscar_python/_providers/_providers_base.py` & `oscar_python-1.1.0b1/oscar_python/_providers/_providers_base.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.4/oscar_python/_providers/_s3.py` & `oscar_python-1.1.0b1/oscar_python/_providers/_s3.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.4/oscar_python/_providers/_webdav.py` & `oscar_python-1.1.0b1/oscar_python/_providers/_webdav.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.4/oscar_python/_utils.py` & `oscar_python-1.1.0b1/oscar_python/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License. 
 
 import base64
-import json
 import os
 import requests
-_DEFAULT_TIMEOUT = 30
+import liboidcagent as agent
+_DEFAULT_TIMEOUT = 60
 
 """ Generic http request """
 def make_request(c , path, method, **kwargs):
 
     if "timeout" in kwargs.keys() and kwargs["timeout"]: 
         timeout = kwargs["timeout"]
-        print("timeout set to: ", timeout)
     else: 
         timeout = _DEFAULT_TIMEOUT
 
     url = c.endpoint+path
     headers = get_headers(c)  
     if method in ["post", "put"]:
         if "token" in kwargs.keys() and kwargs["token"]: 
@@ -39,19 +38,23 @@
 
     if "handle" in kwargs.keys() and kwargs["handle"] == False:
         return result
     
     result.raise_for_status()
     return result
 
-""" Function to generate headers with basic authentication """
+""" Function to generate headers with basic authentication or OIDC """
 def get_headers(c):
-    usr_pass_as_bytes = bytes(c.user+":"+c.password,"utf-8")
-    usr_pass_base_64 = base64.b64encode(usr_pass_as_bytes).decode("utf-8")
-    return {"Authorization": "Basic "+ usr_pass_base_64}
+    if c._AUTH_TYPE == "basicauth":
+        usr_pass_as_bytes = bytes(c.user+":"+c.password,"utf-8")
+        usr_pass_base_64 = base64.b64encode(usr_pass_as_bytes).decode("utf-8")
+        return {"Authorization": "Basic "+ usr_pass_base_64}
+    if c._AUTH_TYPE == "oidc":
+        token = agent.get_access_token(c.shortname)
+        return get_headers_with_token(token)
 
 """ Function to generate headers with token auth """
 def get_headers_with_token(token):
     return {"Authorization": "Bearer "+ str(token)}
 
 def write_text_file(content, file_path):
     with open(file_path, 'w') as f:
@@ -100,8 +103,8 @@
     if(isBase64(output)):
         decode_b64(output, file_path)
         return
     if(isinstance(output,str)):
         write_text_file(output,file_path)
         return
 
- 
+
```

### Comparing `oscar_python-1.0.4/oscar_python/client.py` & `oscar_python-1.1.0b1/oscar_python/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,46 +9,70 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License. 
 
-import os
 import json
 import yaml
+import liboidcagent as agent
 import oscar_python._utils as utils
 from oscar_python.storage import Storage
 
 _INFO_PATH = "/system/info"
 _CONFIG_PATH = "/system/config"
 _SVC_PATH = "/system/services"
 _LOGS_PATH = "/system/logs"
 _RUN_PATH = "/run"
 #_JOB_PATH = "/job"
 
-_MINIO = "minio"
-_S3 = "s3"
-_ONE_DATA = "onedata"
-_WEBDAV = "webdav"
 
 _GET = "get"
 _POST = "post"
 _PUT = "put"
 _DELETE = "delete"
-_DEFAULT_TIMEOUT = 30
 
 class Client:
     #Cluster info 
-    def __init__(self, id, endpoint, user, password, ssl) -> None:
-        self.id = id
-        self.endpoint = endpoint
-        self.user = user
-        self.password = password
-        self.ssl = ssl
+    def __init__(self, options) -> None:
+        self.set_auth_type(options)
+        if self._AUTH_TYPE == 'basicauth':
+            self.basic_auth_client(options)
+        if self._AUTH_TYPE == 'oidc':
+            self.oidc_client(options)
+
+    def basic_auth_client(self, options):
+        self.id = self.id
+        self.endpoint = options['endpoint']
+        self.user = options['user']
+        self.password = options['password']
+        self.ssl = bool(options['ssl'])
+
+    def oidc_client(self, options):
+        self.id = self.id
+        self.endpoint = options['endpoint']
+        self.shortname = options['shortname']
+        self.ssl = bool(options['ssl'])
+
+    def set_auth_type(self, options):
+        if 'user' in options:
+            self._AUTH_TYPE = "basicauth"
+            try:
+                self.get_cluster_info()
+            except:
+               print("")
+        elif 'shortname' in options:
+            self._AUTH_TYPE = "oidc"
+            try:
+                agent.get_access_token(self.shortname)
+            except agent.OidcAgentError as e:
+                print("ERROR oidc-agent: {}".format(e))
+        else:
+            raise ValueError("Unrecognized authentication credentials in options")
 
     """ Creates a generic storage client to interact with the storage providers 
     defined on a specific service of the refered OSCAR cluster """
     def create_storage_client(self, svc):
         return Storage(
                 client_obj=self,
                 svc_name=svc)
@@ -119,15 +143,15 @@
         if "input" in kwargs.keys() and kwargs["input"]:
             exec_input = kwargs["input"]
             token = self._get_token(name) 
             
             send_data = utils.encode_input(exec_input)
 
             if "timeout" in kwargs.keys() and kwargs["timeout"]:
-                response = utils.make_request(self, _RUN_PATH+"/"+name, _POST, data=send_data, token=token, timeout=kwargs["timeout"])
+                response = utils._make_request(self, _RUN_PATH+"/"+name, _POST, data=send_data, token=token, timeout=kwargs["timeout"])
             else:
                 response = utils.make_request(self, _RUN_PATH+"/"+name, _POST, data=send_data, token=token)
             
             if "output" in kwargs.keys() and kwargs["output"]:
                 utils.decode_output(response.text, kwargs["output"])
             return response
```

### Comparing `oscar_python-1.0.4/oscar_python/storage.py` & `oscar_python-1.1.0b1/oscar_python/storage.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.4/oscar_python.egg-info/PKG-INFO` & `oscar_python-1.1.0b1/oscar_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscar-python
-Version: 1.0.4
+Version: 1.1.0b1
 Summary: OSCAR API for python
 Home-page: https://github.com/grycap/oscar_python
 Author: GRyCAP - Universitat Politecnica de Valencia
 Author-email: calarcon@i3m.upv.es
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `oscar_python-1.0.4/oscar_python.egg-info/SOURCES.txt` & `oscar_python-1.1.0b1/oscar_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.4/setup.py` & `oscar_python-1.1.0b1/setup.py`

 * *Files identical despite different names*

