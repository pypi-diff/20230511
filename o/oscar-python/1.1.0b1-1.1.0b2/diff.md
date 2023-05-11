# Comparing `tmp/oscar_python-1.1.0b1.tar.gz` & `tmp/oscar_python-1.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oscar_python-1.1.0b1.tar", last modified: Thu May 11 08:09:28 2023, max compression
+gzip compressed data, was "oscar_python-1.1.0b2.tar", last modified: Thu May 11 09:07:42 2023, max compression
```

## Comparing `oscar_python-1.1.0b1.tar` & `oscar_python-1.1.0b2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:28.925472 oscar_python-1.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-11 08:09:28.925472 oscar_python-1.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:28.925472 oscar_python-1.1.0b1/oscar_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:28.925472 oscar_python-1.1.0b1/oscar_python/_providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/_providers/_minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/_providers/_onedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/_providers/_providers_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/_providers/_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/_providers/_webdav.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/oscar_python/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:28.925472 oscar_python-1.1.0b1/oscar_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-11 08:09:28.000000 oscar_python-1.1.0b1/oscar_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-11 08:09:28.000000 oscar_python-1.1.0b1/oscar_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:09:28.000000 oscar_python-1.1.0b1/oscar_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:09:28.000000 oscar_python-1.1.0b1/oscar_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 08:09:28.000000 oscar_python-1.1.0b1/oscar_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 08:09:28.000000 oscar_python-1.1.0b1/oscar_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:09:28.925472 oscar_python-1.1.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-11 08:09:19.000000 oscar_python-1.1.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:07:42.624426 oscar_python-1.1.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-11 09:07:42.624426 oscar_python-1.1.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:07:42.624426 oscar_python-1.1.0b2/oscar_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:07:42.624426 oscar_python-1.1.0b2/oscar_python/_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/_providers/_minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/_providers/_onedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/_providers/_providers_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/_providers/_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/_providers/_webdav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/oscar_python/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:07:42.624426 oscar_python-1.1.0b2/oscar_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-11 09:07:42.000000 oscar_python-1.1.0b2/oscar_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-11 09:07:42.000000 oscar_python-1.1.0b2/oscar_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:07:42.000000 oscar_python-1.1.0b2/oscar_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:07:42.000000 oscar_python-1.1.0b2/oscar_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 09:07:42.000000 oscar_python-1.1.0b2/oscar_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 09:07:42.000000 oscar_python-1.1.0b2/oscar_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:07:42.624426 oscar_python-1.1.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-11 09:07:26.000000 oscar_python-1.1.0b2/setup.py
```

### Comparing `oscar_python-1.1.0b1/LICENSE` & `oscar_python-1.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b1/PKG-INFO` & `oscar_python-1.1.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscar_python
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: OSCAR API for python
 Home-page: https://github.com/grycap/oscar_python
 Author: GRyCAP - Universitat Politecnica de Valencia
 Author-email: calarcon@i3m.upv.es
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `oscar_python-1.1.0b1/README.md` & `oscar_python-1.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b1/oscar_python/_providers/_minio.py` & `oscar_python-1.1.0b2/oscar_python/_providers/_minio.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b1/oscar_python/_providers/_onedata.py` & `oscar_python-1.1.0b2/oscar_python/_providers/_onedata.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b1/oscar_python/_providers/_providers_base.py` & `oscar_python-1.1.0b2/oscar_python/_providers/_providers_base.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b1/oscar_python/_providers/_s3.py` & `oscar_python-1.1.0b2/oscar_python/_providers/_s3.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b1/oscar_python/_providers/_webdav.py` & `oscar_python-1.1.0b2/oscar_python/_providers/_webdav.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b1/oscar_python/_utils.py` & `oscar_python-1.1.0b2/oscar_python/_utils.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b1/oscar_python/client.py` & `oscar_python-1.1.0b2/oscar_python/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,37 +38,33 @@
         self.set_auth_type(options)
         if self._AUTH_TYPE == 'basicauth':
             self.basic_auth_client(options)
         if self._AUTH_TYPE == 'oidc':
             self.oidc_client(options)
 
     def basic_auth_client(self, options):
-        self.id = self.id
+        self.id = options['cluster_id']
         self.endpoint = options['endpoint']
         self.user = options['user']
         self.password = options['password']
         self.ssl = bool(options['ssl'])
 
     def oidc_client(self, options):
-        self.id = self.id
+        self.id = options['cluster_id']
         self.endpoint = options['endpoint']
         self.shortname = options['shortname']
         self.ssl = bool(options['ssl'])
 
     def set_auth_type(self, options):
         if 'user' in options:
             self._AUTH_TYPE = "basicauth"
-            try:
-                self.get_cluster_info()
-            except:
-               print("")
         elif 'shortname' in options:
             self._AUTH_TYPE = "oidc"
             try:
-                agent.get_access_token(self.shortname)
+                agent.get_access_token(options['shortname'])
             except agent.OidcAgentError as e:
                 print("ERROR oidc-agent: {}".format(e))
         else:
             raise ValueError("Unrecognized authentication credentials in options")
 
     """ Creates a generic storage client to interact with the storage providers 
     defined on a specific service of the refered OSCAR cluster """
```

### Comparing `oscar_python-1.1.0b1/oscar_python/storage.py` & `oscar_python-1.1.0b2/oscar_python/storage.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b1/oscar_python.egg-info/PKG-INFO` & `oscar_python-1.1.0b2/oscar_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscar-python
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: OSCAR API for python
 Home-page: https://github.com/grycap/oscar_python
 Author: GRyCAP - Universitat Politecnica de Valencia
 Author-email: calarcon@i3m.upv.es
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `oscar_python-1.1.0b1/oscar_python.egg-info/SOURCES.txt` & `oscar_python-1.1.0b2/oscar_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oscar_python-1.1.0b1/setup.py` & `oscar_python-1.1.0b2/setup.py`

 * *Files identical despite different names*

