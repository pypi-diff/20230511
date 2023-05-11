# Comparing `tmp/deterrers-api-0.4.tar.gz` & `tmp/deterrers-api-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deterrers-api-0.4.tar", last modified: Thu Apr 20 13:51:05 2023, max compression
+gzip compressed data, was "deterrers-api-0.4.1.tar", last modified: Thu May 11 11:15:14 2023, max compression
```

## Comparing `deterrers-api-0.4.tar` & `deterrers-api-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-20 13:51:05.634222 deterrers-api-0.4/
--rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 19:32:41.000000 deterrers-api-0.4/LICENSE
--rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 19:52:33.000000 deterrers-api-0.4/MANIFEST.in
--rw-r--r--   0 lars      (1000) lars      (1000)     1070 2023-04-20 13:51:05.634222 deterrers-api-0.4/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      799 2023-04-13 20:00:47.000000 deterrers-api-0.4/README.md
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-20 13:51:05.633222 deterrers-api-0.4/deterrers_api.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)     1070 2023-04-20 13:51:05.000000 deterrers-api-0.4/deterrers_api.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      264 2023-04-20 13:51:05.000000 deterrers-api-0.4/deterrers_api.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-20 13:51:05.000000 deterrers-api-0.4/deterrers_api.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-20 13:51:05.000000 deterrers-api-0.4/deterrers_api.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-20 13:51:05.000000 deterrers-api-0.4/deterrers_api.egg-info/top_level.txt
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-20 13:51:05.634222 deterrers-api-0.4/deterrersapi/
--rw-r--r--   0 lars      (1000) lars      (1000)     6156 2023-04-20 13:47:06.000000 deterrers-api-0.4/deterrersapi/__init__.py
--rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-04-13 19:34:31.000000 deterrers-api-0.4/requirements.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-20 13:51:05.634222 deterrers-api-0.4/setup.cfg
--rw-r--r--   0 lars      (1000) lars      (1000)      688 2023-04-20 13:47:40.000000 deterrers-api-0.4/setup.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-05-11 11:15:14.025271 deterrers-api-0.4.1/
+-rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-05-11 07:45:30.000000 deterrers-api-0.4.1/LICENSE
+-rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-05-11 07:45:30.000000 deterrers-api-0.4.1/MANIFEST.in
+-rw-r--r--   0 lars      (1000) lars      (1000)     1052 2023-05-11 11:15:14.024271 deterrers-api-0.4.1/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      799 2023-05-11 07:45:30.000000 deterrers-api-0.4.1/README.md
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-05-11 11:15:14.024271 deterrers-api-0.4.1/deterrers_api.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)     1052 2023-05-11 11:15:13.000000 deterrers-api-0.4.1/deterrers_api.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      264 2023-05-11 11:15:14.000000 deterrers-api-0.4.1/deterrers_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-05-11 11:15:13.000000 deterrers-api-0.4.1/deterrers_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-05-11 11:15:13.000000 deterrers-api-0.4.1/deterrers_api.egg-info/requires.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-05-11 11:15:13.000000 deterrers-api-0.4.1/deterrers_api.egg-info/top_level.txt
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-05-11 11:15:14.024271 deterrers-api-0.4.1/deterrersapi/
+-rw-r--r--   0 lars      (1000) lars      (1000)     6673 2023-05-11 11:12:18.000000 deterrers-api-0.4.1/deterrersapi/__init__.py
+-rw-r--r--   0 lars      (1000) lars      (1000)        9 2023-05-11 07:45:30.000000 deterrers-api-0.4.1/requirements.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-05-11 11:15:14.025271 deterrers-api-0.4.1/setup.cfg
+-rw-r--r--   0 lars      (1000) lars      (1000)      690 2023-05-11 11:13:14.000000 deterrers-api-0.4.1/setup.py
```

### Comparing `deterrers-api-0.4/LICENSE` & `deterrers-api-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deterrers-api-0.4/PKG-INFO` & `deterrers-api-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: deterrers-api
-Version: 0.4
+Version: 0.4.1
 Summary: Python API client for DETERRERS
 Home-page: https://github.com/virtUOS/deterrers-api
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Python API client for DETERRERS
 
 This library makes it easy to interact with the DETERRERS perimeter firewall
 portal to automate registration, and configuration of IP addresses and firewall
 profiles.
@@ -42,9 +41,7 @@
 
 # update ip with firewall profile `Multipurpose`
 deterrers.update('192.0.0.1', 'Multipurpose', '')
 
 # activate firewall profile
 deterrers.action('192.0.0.1', 'register')
 ```
-
-
```

### Comparing `deterrers-api-0.4/README.md` & `deterrers-api-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `deterrers-api-0.4/deterrers_api.egg-info/PKG-INFO` & `deterrers-api-0.4.1/deterrers_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: deterrers-api
-Version: 0.4
+Version: 0.4.1
 Summary: Python API client for DETERRERS
 Home-page: https://github.com/virtUOS/deterrers-api
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Python API client for DETERRERS
 
 This library makes it easy to interact with the DETERRERS perimeter firewall
 portal to automate registration, and configuration of IP addresses and firewall
 profiles.
@@ -42,9 +41,7 @@
 
 # update ip with firewall profile `Multipurpose`
 deterrers.update('192.0.0.1', 'Multipurpose', '')
 
 # activate firewall profile
 deterrers.action('192.0.0.1', 'register')
 ```
-
-
```

### Comparing `deterrers-api-0.4/deterrersapi/__init__.py` & `deterrers-api-0.4.1/deterrersapi/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import requests
 
 
 class Deterrers:
     __base_url = None
     __token = None
 
+    timeout = 30
+    '''Request timeout in seconds'''
+
     def __init__(self, base_url: str, token: str) -> None:
         '''Initialize DETERRERS client.
 
         :param base_url: URL of the DETERRERS installation without path
         :type base_url: str
         :param token: API token to use for authentication
         :type token: str
@@ -41,60 +44,70 @@
 
         :param path: Endpoint to request
         :type path: str
         :return: Decoded response data or None
         '''
         response = requests.get(self.__url(path),
                                 headers=self.__header(),
-                                params=params)
+                                params=params,
+                                timeout=self.timeout)
         return response.json() if response.status_code == 200 else None
 
     def __patch(self, path: str, data: dict) -> None:
         '''Execute API PATCH request
 
         :param path: Endpoint to request
         :type path: str
         :param data: Data to send
         :type data: dict
         :raises RuntimeError: if patch did not succeed
         '''
         url: str = self.__url(path)
-        response = requests.patch(url, headers=self.__header(), json=data)
+        response = requests.patch(url,
+                                  headers=self.__header(),
+                                  json=data,
+                                  timeout=self.timeout)
         if response.status_code not in [200]:
             raise RuntimeError(f'Error updating {data}. Response: {response}')
 
     def __post(self, path: str, data: dict) -> None:
         '''Execute API POST request
 
         :param path: Endpoint to request
         :type path: str
         :param data: Data to post
         :type data: dict
         :raises RuntimeError: if adding data did not succeed
         '''
         url: str = self.__url(path)
-        response = requests.post(url, headers=self.__header(), json=data)
+        response = requests.post(url,
+                                 headers=self.__header(),
+                                 json=data,
+                                 timeout=self.timeout)
         if response.status_code not in [200]:
             raise RuntimeError(f'Error adding {data}. Response: {response}')
 
     def __delete(self, path: str, data: dict) -> None:
         '''Execute API DELETE request.
 
         :param path: Endpoint to request
         :type path: str
         :param data: Data identifying entity to delete
         :type data: dict
         :raises RuntimeError: if removal did not succeed
         '''
         url: str = self.__url(path)
-        response = requests.delete(url, headers=self.__header(), json=data)
+        response = requests.delete(url,
+                                   headers=self.__header(),
+                                   json=data,
+                                   timeout=self.timeout)
         if response.status_code not in [200, 404]:
             raise RuntimeError(f'Error deleting {data}. Response: {response}')
 
-    def hosts(self):
+    def hosts(self) -> dict:
         '''Get list of hosts added to DETERRERS
 
         :return: List of hosts
         :rtype: list
         '''
         return self.__get('hosts/')
 
@@ -154,15 +167,15 @@
         :type profile: str | None
         :param firewall: Host firewall. Must be one of the UI options
                          or an empty string.
         :type firewall: str | None
         :param admins: List of admins for address
         :type admins: list[str] | None
         '''
-        data = {'ipv4_addr': ipv4}
+        data: dict[str, str | list[str]] = {'ipv4_addr': ipv4}
         if profile is not None:
             data['service_profile'] = profile
         if firewall is not None:
             data['fw'] = firewall
         if admins is not None:
             data['admin_ids'] = admins
         return self.__patch('host/', data)
```

### Comparing `deterrers-api-0.4/setup.py` & `deterrers-api-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     path = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(path, filename), encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='deterrers-api',
-    version='0.4',
+    version='0.4.1',
     description='Python API client for DETERRERS',
     url='https://github.com/virtUOS/deterrers-api',
     author='Lars Kiesow',
     author_email='lkiesow@uos.de',
     license='MIT',
     packages=['deterrersapi'],
     license_files=('LICENSE'),
```

