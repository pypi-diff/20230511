# Comparing `tmp/atas_client-0.0.3.tar.gz` & `tmp/atas_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atas_client-0.0.3.tar", last modified: Thu Dec  8 01:19:32 2022, max compression
+gzip compressed data, was "atas_client-0.0.4.tar", last modified: Thu May 11 06:29:36 2023, max compression
```

## Comparing `atas_client-0.0.3.tar` & `atas_client-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 01:19:32.734126 atas_client-0.0.3/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1073 2022-12-05 06:04:48.000000 atas_client-0.0.3/LICENSE
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2022-12-08 01:19:32.734007 atas_client-0.0.3/PKG-INFO
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       23 2022-12-05 06:50:55.000000 atas_client-0.0.3/README.md
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      551 2022-12-08 01:19:27.000000 atas_client-0.0.3/pyproject.toml
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       38 2022-12-08 01:19:32.734164 atas_client-0.0.3/setup.cfg
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 01:19:32.732920 atas_client-0.0.3/src/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:17.000000 atas_client-0.0.3/src/__init__.py
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 01:19:32.733388 atas_client-0.0.3/src/atas_client/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     2274 2022-12-08 01:19:04.000000 atas_client-0.0.3/src/atas_client/CoreATASApi.py
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1301 2022-12-06 03:09:47.000000 atas_client-0.0.3/src/atas_client/HttpUtil.py
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:10.000000 atas_client-0.0.3/src/atas_client/__init__.py
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      960 2022-12-08 01:19:04.000000 atas_client-0.0.3/src/atas_client/atas_client.py
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 01:19:32.733860 atas_client-0.0.3/src/atas_client.egg-info/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2022-12-08 01:19:32.000000 atas_client-0.0.3/src/atas_client.egg-info/PKG-INFO
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      322 2022-12-08 01:19:32.000000 atas_client-0.0.3/src/atas_client.egg-info/SOURCES.txt
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        1 2022-12-08 01:19:32.000000 atas_client-0.0.3/src/atas_client.egg-info/dependency_links.txt
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       21 2022-12-08 01:19:32.000000 atas_client-0.0.3/src/atas_client.egg-info/top_level.txt
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2023-05-11 06:29:36.888454 atas_client-0.0.4/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1073 2022-12-05 06:04:48.000000 atas_client-0.0.4/LICENSE
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2023-05-11 06:29:36.888331 atas_client-0.0.4/PKG-INFO
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       23 2022-12-05 06:50:55.000000 atas_client-0.0.4/README.md
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      551 2023-05-11 06:13:09.000000 atas_client-0.0.4/pyproject.toml
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       38 2023-05-11 06:29:36.888499 atas_client-0.0.4/setup.cfg
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2023-05-11 06:29:36.886418 atas_client-0.0.4/src/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:17.000000 atas_client-0.0.4/src/__init__.py
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2023-05-11 06:29:36.887433 atas_client-0.0.4/src/atas_client/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     2274 2022-12-08 01:19:04.000000 atas_client-0.0.4/src/atas_client/CoreATASApi.py
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1357 2023-05-11 06:11:15.000000 atas_client-0.0.4/src/atas_client/HttpUtil.py
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:10.000000 atas_client-0.0.4/src/atas_client/__init__.py
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      960 2022-12-08 01:19:04.000000 atas_client-0.0.4/src/atas_client/atas_client.py
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2023-05-11 06:29:36.888167 atas_client-0.0.4/src/atas_client.egg-info/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2023-05-11 06:29:36.000000 atas_client-0.0.4/src/atas_client.egg-info/PKG-INFO
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      322 2023-05-11 06:29:36.000000 atas_client-0.0.4/src/atas_client.egg-info/SOURCES.txt
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        1 2023-05-11 06:29:36.000000 atas_client-0.0.4/src/atas_client.egg-info/dependency_links.txt
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       21 2023-05-11 06:29:36.000000 atas_client-0.0.4/src/atas_client.egg-info/top_level.txt
```

### Comparing `atas_client-0.0.3/LICENSE` & `atas_client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atas_client-0.0.3/PKG-INFO` & `atas_client-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atas_client
-Version: 0.0.3
+Version: 0.0.4
 Summary: ATAS Automation API
 Author-email: "tao.ding" <tao.ding@rakuten.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `atas_client-0.0.3/pyproject.toml` & `atas_client-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atas_client"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="tao.ding", email="tao.ding@rakuten.com" },
 ]
 description = "ATAS Automation API"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `atas_client-0.0.3/src/atas_client/CoreATASApi.py` & `atas_client-0.0.4/src/atas_client/CoreATASApi.py`

 * *Files identical despite different names*

### Comparing `atas_client-0.0.3/src/atas_client/HttpUtil.py` & `atas_client-0.0.4/src/atas_client/HttpUtil.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 
 
 class HttpUtil:
     @staticmethod
     def http_post(url, parameters, headers):
         if headers is None:
             headers = {"Content-Type": "application/json"}
-        res = requests.post(url, data=parameters, headers=headers)
+        res = requests.post(url, data=parameters, headers=headers, verify=False)
         if res.status_code != 200:
             raise Exception("Request exception")
         result = json.loads(res.text)
         return result
 
     @staticmethod
     def http_get(url, parameters, headers):
-        res = requests.get(url, data=parameters, headers=headers)
+        res = requests.get(url, data=parameters, headers=headers, verify=False)
         if res.status_code != 200:
             raise Exception(u"Request exception")
         result = json.loads(res.text)
         return result
 
     @staticmethod
     def http_request(url, method, params, data, body, **kwargs):
-        response = requests.request(method, url, params=params, data=data, json=body, **kwargs)
+        response = requests.request(method, url, params=params, data=data, json=body, **kwargs, verify=False)
         if response.status_code != 200:
             raise Exception(u"Request exception")
         result = response.text
         return result
 
     @staticmethod
     def http_multipart_request(url, data, files, auth_key):
         headers = {
             'auth-key': auth_key
         }
-        response = requests.request("POST", url, headers=headers, data=data, files=files)
+        response = requests.request("POST", url, headers=headers, data=data, files=files, verify=False)
         result = response.text
         return result
```

### Comparing `atas_client-0.0.3/src/atas_client/atas_client.py` & `atas_client-0.0.4/src/atas_client/atas_client.py`

 * *Files identical despite different names*

### Comparing `atas_client-0.0.3/src/atas_client.egg-info/PKG-INFO` & `atas_client-0.0.4/src/atas_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atas-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: ATAS Automation API
 Author-email: "tao.ding" <tao.ding@rakuten.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

