# Comparing `tmp/fortifyapi-3.1.5.tar.gz` & `tmp/fortifyapi-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortifyapi-3.1.5.tar", last modified: Wed May 10 17:53:03 2023, max compression
+gzip compressed data, was "fortifyapi-3.1.6.tar", last modified: Wed May 10 18:48:59 2023, max compression
```

## Comparing `fortifyapi-3.1.5.tar` & `fortifyapi-3.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 17:53:03.502205 fortifyapi-3.1.5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1046 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       29 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-05-10 17:53:03.502205 fortifyapi-3.1.5/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2228 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 17:53:03.502205 fortifyapi-3.1.5/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7460 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/docs/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/docs/couscous.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 17:53:03.502205 fortifyapi-3.1.5/fortifyapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6749 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27850 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39227 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/fortify.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7013 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/template.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 17:53:03.502205 fortifyapi-3.1.5/fortifyapi.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-05-10 17:53:03.000000 fortifyapi-3.1.5/fortifyapi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-05-10 17:53:03.000000 fortifyapi-3.1.5/fortifyapi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-10 17:53:03.000000 fortifyapi-3.1.5/fortifyapi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-05-10 17:53:03.000000 fortifyapi-3.1.5/fortifyapi.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-05-10 17:53:03.000000 fortifyapi-3.1.5/fortifyapi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-10 17:53:03.000000 fortifyapi-3.1.5/fortifyapi.egg-info/zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-05-10 17:53:03.502205 fortifyapi-3.1.5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 18:48:59.901475 fortifyapi-3.1.6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1046 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       29 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-05-10 18:48:59.901475 fortifyapi-3.1.6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2228 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 18:48:59.901475 fortifyapi-3.1.6/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7460 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/docs/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/docs/couscous.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 18:48:59.901475 fortifyapi-3.1.6/fortifyapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/fortifyapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6749 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/fortifyapi/api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27850 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/fortifyapi/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/fortifyapi/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    39607 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/fortifyapi/fortify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/fortifyapi/query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7013 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/fortifyapi/template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 18:48:59.901475 fortifyapi-3.1.6/fortifyapi.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-05-10 18:48:59.000000 fortifyapi-3.1.6/fortifyapi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-05-10 18:48:59.000000 fortifyapi-3.1.6/fortifyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-10 18:48:59.000000 fortifyapi-3.1.6/fortifyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-05-10 18:48:59.000000 fortifyapi-3.1.6/fortifyapi.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-05-10 18:48:59.000000 fortifyapi-3.1.6/fortifyapi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-10 18:48:59.000000 fortifyapi-3.1.6/fortifyapi.egg-info/zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-05-10 18:48:59.901475 fortifyapi-3.1.6/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2023-05-10 18:48:52.000000 fortifyapi-3.1.6/setup.py
```

### Comparing `fortifyapi-3.1.5/LICENSE.txt` & `fortifyapi-3.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.5/PKG-INFO` & `fortifyapi-3.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fortifyapi
-Version: 3.1.5
+Version: 3.1.6
 Summary: Python library for Fortify Software Security Center (SSC) RESTFul API
 Home-page: https://github.com/fortifyadmin/fortifyapi
 Author: Brandon Spruth, Matthew Gill
 Author-email: brandon@spruth.co, mgill@c0ffee.me
 License: MIT
-Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.5
+Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.6
 Description: .. image:: https://img.shields.io/pypi/v/fortifyapi.svg
         .. image:: https://img.shields.io/pypi/pyversions/fortifyapi.svg
         .. image:: https://img.shields.io/circleci/build/github/fortifyadmin/fortifyapi/master?logo=CircleCI
         
         Fortify API
         ***********
```

### Comparing `fortifyapi-3.1.5/README.rst` & `fortifyapi-3.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.5/docs/README.md` & `fortifyapi-3.1.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.5/fortifyapi/api.py` & `fortifyapi-3.1.6/fortifyapi/api.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.5/fortifyapi/client.py` & `fortifyapi-3.1.6/fortifyapi/client.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.5/fortifyapi/fortify.py` & `fortifyapi-3.1.6/fortifyapi/fortify.py`

 * *Files 1% similar despite different names*

```diff
@@ -685,22 +685,26 @@
         """
         url = '/api/v1/projectVersions/' + str(version_id) + '/issues?start=0&limit=-1&' + orderby + '&' \
                                                              'showhidden=false&' \
                                                              'showremoved=false&showsuppressed=false&' \
                                                              'showshortfilenames=false'
         return self._request('GET', url)
 
-    def get_project_version_issue_details(self, issue_id):
+    def get_project_version_issue_details(self, instance_id, project_name, version_name, engine='SCA'):
         """
         Returns trace analysis and other details of a given issue. The issue ID can be found from the /issues or
         projectVersions endpoint.
-        :param issue_id:
+        :param instance_id: application version id
+        :param project_name: project or application name
+        :param version_name: version name
+        :param engine: SCA is the only value that this function would work with
         :return: full detail of a given issue
         """
-        url = "/api/v1/issueDetails/" + str(issue_id)
+        url = f'/api/v1/issueDetails?instanceId={str(instance_id)}&projectName={str(project_name)}' \
+              f'&projectVersionName={str(version_name)}&engineType={str(engine)}'
         return self._request("GET", url)
 
     def get_project_version_source_file(self, version_id, path):
         """
         Returns an object with information on a source file from a specific project version.
         It includes the file content.
         :param version_id: application version id
```

### Comparing `fortifyapi-3.1.5/fortifyapi/query.py` & `fortifyapi-3.1.6/fortifyapi/query.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.5/fortifyapi/template.py` & `fortifyapi-3.1.6/fortifyapi/template.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.5/fortifyapi.egg-info/PKG-INFO` & `fortifyapi-3.1.6/fortifyapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fortifyapi
-Version: 3.1.5
+Version: 3.1.6
 Summary: Python library for Fortify Software Security Center (SSC) RESTFul API
 Home-page: https://github.com/fortifyadmin/fortifyapi
 Author: Brandon Spruth, Matthew Gill
 Author-email: brandon@spruth.co, mgill@c0ffee.me
 License: MIT
-Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.5
+Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.6
 Description: .. image:: https://img.shields.io/pypi/v/fortifyapi.svg
         .. image:: https://img.shields.io/pypi/pyversions/fortifyapi.svg
         .. image:: https://img.shields.io/circleci/build/github/fortifyadmin/fortifyapi/master?logo=CircleCI
         
         Fortify API
         ***********
```

### Comparing `fortifyapi-3.1.5/setup.py` & `fortifyapi-3.1.6/setup.py`

 * *Files identical despite different names*

