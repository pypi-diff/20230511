# Comparing `tmp/rentdynamics-1.0.1.tar.gz` & `tmp/rentdynamics-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rentdynamics-1.0.1.tar", last modified: Tue Mar 12 17:38:02 2019, max compression
+gzip compressed data, was "dist/rentdynamics-1.1.0.tar", last modified: Thu May 11 17:35:26 2023, max compression
```

## Comparing `rentdynamics-1.0.1.tar` & `rentdynamics-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-03-12 17:38:02.000000 rentdynamics-1.0.1/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-03-12 17:38:02.000000 rentdynamics-1.0.1/rentdynamics/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-03-12 17:37:56.000000 rentdynamics-1.0.1/rentdynamics/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5890 2019-03-12 17:37:56.000000 rentdynamics-1.0.1/rentdynamics/client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      275 2019-03-12 17:38:02.000000 rentdynamics-1.0.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      354 2019-03-12 17:37:56.000000 rentdynamics-1.0.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 17:35:26.000000 rentdynamics-1.1.0/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 17:35:26.000000 rentdynamics-1.1.0/rentdynamics/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 17:35:08.000000 rentdynamics-1.1.0/rentdynamics/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6193 2023-05-11 17:35:08.000000 rentdynamics-1.1.0/rentdynamics/client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      354 2023-05-11 17:35:08.000000 rentdynamics-1.1.0/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      275 2023-05-11 17:35:26.000000 rentdynamics-1.1.0/PKG-INFO
```

### Comparing `rentdynamics-1.0.1/rentdynamics/client.py` & `rentdynamics-1.1.0/rentdynamics/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,28 +11,35 @@
 class Client:
     api_key = None
     api_secret = None
     auth_token = None
     development = False
     user_id = None
 
-    def __init__(self, api_key=None, api_secret=None, development=False):
+    def __init__(self, api_key=None, api_secret=None, development=False, base_url=None,
+                 base_development_url=None):
         self.api_key = api_key
         self.api_secret = api_secret
+        self.base_url = base_url
+        self.base_development_url = base_development_url
         self.development = development
 
     def get(self, endpoint):
         headers = self.get_headers(endpoint)
         request_url = self.get_base_url() + endpoint
         return requests.get(request_url, headers=headers)
 
     def get_base_url(self):
         if self.development:
-            return 'https://api-dev.rentdynamics.com'
+            if self.base_development_url:
+                return self.base_development_url
+            return 'https://api.rentdynamics.dev'
         else:
+            if self.base_url:
+                return self.base_url
             return 'https://api.rentdynamics.com'
 
     def get_headers(self, endpoint, body=None):
         timestamp = str(self.get_timestamp_milliseconds())
         nonce = self.get_nonce(timestamp=timestamp, url=endpoint, body=body)
         headers = {
             'x-rd-timestamp': timestamp,
```

