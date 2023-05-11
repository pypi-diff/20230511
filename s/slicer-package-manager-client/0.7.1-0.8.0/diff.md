# Comparing `tmp/slicer-package-manager-client-0.7.1.tar.gz` & `tmp/slicer-package-manager-client-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicer-package-manager-client-0.7.1.tar", last modified: Sat May 21 04:10:52 2022, max compression
+gzip compressed data, was "slicer-package-manager-client-0.8.0.tar", last modified: Thu May 11 02:54:45 2023, max compression
```

## Comparing `slicer-package-manager-client-0.7.1.tar` & `slicer-package-manager-client-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:52.520706 slicer-package-manager-client-0.7.1/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1876 2022-05-21 04:10:52.520706 slicer-package-manager-client-0.7.1/PKG-INFO
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1070 2022-05-20 21:48:20.000000 slicer-package-manager-client-0.7.1/README.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1437 2022-05-21 04:08:53.000000 slicer-package-manager-client-0.7.1/pyproject.toml
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       38 2022-05-21 04:10:52.520706 slicer-package-manager-client-0.7.1/setup.cfg
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      191 2022-05-20 20:46:19.000000 slicer-package-manager-client-0.7.1/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:52.520706 slicer-package-manager-client-0.7.1/slicer_package_manager_client/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    26039 2022-05-21 04:10:04.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       70 2022-05-20 20:46:19.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client/__main__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:52.520706 slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2022-05-20 20:46:19.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/__init__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:52.520706 slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/bson/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      631 2022-05-20 20:46:19.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/bson/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1159 2022-05-20 20:46:19.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/bson/errors.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     9397 2022-05-20 20:46:19.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/bson/objectid.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2815 2022-05-20 20:46:19.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/bson/py3compat.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1518 2022-05-20 20:46:19.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/bson/tz_util.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    26264 2022-05-20 20:46:19.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client/cli.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2022-05-21 04:10:52.520706 slicer-package-manager-client-0.7.1/slicer_package_manager_client.egg-info/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1876 2022-05-21 04:10:52.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client.egg-info/PKG-INFO
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      850 2022-05-21 04:10:52.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client.egg-info/SOURCES.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2022-05-21 04:10:52.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client.egg-info/dependency_links.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       89 2022-05-21 04:10:52.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client.egg-info/entry_points.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2022-05-19 14:26:57.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client.egg-info/not-zip-safe
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       53 2022-05-21 04:10:52.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client.egg-info/requires.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       30 2022-05-21 04:10:52.000000 slicer-package-manager-client-0.7.1/slicer_package_manager_client.egg-info/top_level.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:45.621388 slicer-package-manager-client-0.8.0/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1924 2023-05-11 02:54:45.621388 slicer-package-manager-client-0.8.0/PKG-INFO
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1070 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/README.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1515 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/pyproject.toml
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       38 2023-05-11 02:54:45.621388 slicer-package-manager-client-0.8.0/setup.cfg
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      196 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:45.617388 slicer-package-manager-client-0.8.0/slicer_package_manager_client/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    26004 2023-05-11 02:52:30.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       70 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/__main__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:45.621388 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/__init__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:45.621388 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      631 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1159 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/errors.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     9397 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/objectid.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2815 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/py3compat.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1518 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/tz_util.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    26208 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/cli.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:45.621388 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1924 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/PKG-INFO
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      850 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       89 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/entry_points.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/not-zip-safe
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       74 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/requires.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       30 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/top_level.txt
```

### Comparing `slicer-package-manager-client-0.7.1/PKG-INFO` & `slicer-package-manager-client-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: slicer-package-manager-client
-Version: 0.7.1
+Version: 0.8.0
 Summary: Python client for interacting with the Slicer package manager endpoint.
 Author-email: Pierre Assemat <pierre.assemat@kitware.com>, Jean-Christophe Fillion-Robin <jchris.fillionr@kitware.com>
 Maintainer-email: Jean-Christophe Fillion-Robin <jchris.fillionr@kitware.com>
 Project-URL: Documentation, https://slicer-package-manager.readthedocs.io/en/latest/commands_shell.html#slicer-package-manager-client
 Project-URL: Source, https://github.com/girder/slicer_package_manager/tree/main/python_client
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 
 Slicer package manager Python Client
 ====================================
```

### Comparing `slicer-package-manager-client-0.7.1/README.rst` & `slicer-package-manager-client-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `slicer-package-manager-client-0.7.1/pyproject.toml` & `slicer-package-manager-client-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,29 @@
     {name = "Jean-Christophe Fillion-Robin", email = "jchris.fillionr@kitware.com"},
 ]
 readme = "README.rst"
 classifiers = [
     "Environment :: Console",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
 ]
 requires-python = ">=3.7"
 dynamic = ["version"]
 dependencies = [
     "click>=6.7",
     "girder_client",
     "tabulate",
 ]
 
 [project.optional-dependencies]
 test = [
+    "pytest",
     "pytest-vcr",
+    "pytest-girder",
 ]
 
 [project.urls]
 Documentation = "https://slicer-package-manager.readthedocs.io/en/latest/commands_shell.html#slicer-package-manager-client"
 Source = "https://github.com/girder/slicer_package_manager/tree/main/python_client"
 
 [project.scripts]
```

### Comparing `slicer-package-manager-client-0.7.1/slicer_package_manager_client/__init__.py` & `slicer-package-manager-client-0.8.0/slicer_package_manager_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# -*- coding: utf-8 -*-
-
 import os
 
 from girder_client import GirderClient
 
 from ._vendor.bson.objectid import ObjectId
 
 
-__version__ = '0.7.1'
+__version__ = '0.8.0'
 __license__ = 'Apache 2.0'
 
 appName = 'Slicer'
 
 
 class Constant:
     """
@@ -34,34 +32,34 @@
 
 class SlicerPackageManagerError(Exception):
     pass
 
 
 class SlicerPackageClient(GirderClient):
     """
-    The SlicerPackageClient allows to use the slicer_package_manager plugin of Girder.
-    This allow to manage 5 top level entities:
+    The SlicerPackageClient allows to use the slicer_package_manager plugin of Girder,
+    which allows you to manage the following top-level entities:
 
         * Application
         * Release
         * Draft
         * Package
         * Extension
 
-    It's now possible to choose the collection within create the application. It's also
-    possible to get an existing collection by ID for creating the application inside.
+    You may also choose the collection in which to create the application. It's also
+    possible to provide a collection ID to use as the parent collection for creating the application.
 
-    In this case, you must provide the ``coll_id`` argument to be able to use all the
-    commands on these application. By default all the command look for application
-    which are under the *Applications* collection.
+    In this case, you must provide the ``coll_id`` argument to use all the
+    commands on these applications. By default, all commands look for applications
+    that are under a collection named ``Applications``.
     """
 
     def __init__(self, host=None, port=None, apiRoot=None, scheme=None, apiUrl=None,
                  progressReporterCls=None):
-        super(SlicerPackageClient, self).__init__(
+        super().__init__(
             host=host, port=port, apiRoot=apiRoot, scheme=scheme, apiUrl=apiUrl,
             progressReporterCls=progressReporterCls)
 
     def createApp(self, name, desc=None, coll_id=None, coll_name=None, coll_desc=None,
                   public=None):
         """
         Create a new application in the collection which correspond to ``coll_id``,
@@ -86,30 +84,30 @@
             raise SlicerPackageManagerError('The Application "%s" already exist.' % name)
         return self.post('/app', parameters={
             'name': name,
             'app_description': desc,
             'collection_id': coll_id,
             'collection_name': coll_name,
             'collection_description': coll_desc,
-            'public': public
+            'public': public,
         })
 
     def listApp(self, name=None, coll_id=None):
         """
         List all the applications within a specific collection by providing the option
         ``coll_id``. By default it will list within the collection ``Applications``.
         It can also lead to get the application by name.
 
         :param name: application mame
         :param coll_id: Collection ID
         :return:  A list of applications
         """
         apps = self.get('/app', parameters={
             'collection_id': coll_id,
-            'name': name
+            'name': name,
         })
         return apps
 
     def deleteApp(self, name, coll_id=None):
         """
         Delete the application by ID.
 
@@ -135,15 +133,15 @@
         app = self._getApp(app_name=app_name, coll_id=coll_id)
         releases = self.listRelease(app_name=app_name, name=name)
         if releases:
             raise SlicerPackageManagerError('The release "%s" already exist.' % name)
         return self.post('/app/%s/release' % app['_id'], parameters={
             'name': name,
             'app_revision': revision,
-            'description': desc
+            'description': desc,
         })
 
     def listRelease(self, app_name, name=None, coll_id=None):
         """
         List all the release within an application. It's also able to get
         one specific release by name.
 
@@ -193,15 +191,15 @@
         :param limit: Limit of the number of draft releases listed (see :const:`Constant.DEFAULT_LIMIT`)
         :param offset: offset to list only older revisions
         :return: The list of draft release
         """
         app = self._getApp(app_name=app_name, coll_id=coll_id)
         return self.get(
             '/app/%s/draft' % app['_id'],
-            parameters={'revision': revision, 'limit': limit, 'offset': offset}
+            parameters={'revision': revision, 'limit': limit, 'offset': offset},
         )
 
     def deleteDraftRelease(self, app_name, revision, coll_id=None):
         """
         Delete a specific revision within the Draft release.
 
         :param app_name: Name of the application
@@ -323,15 +321,15 @@
 
                 files = list(self.listFile(extension['_id']))
                 if len(files) == 2:
                     # Remove the oldFIle
                     self.delete('/file/%s' % oldFile['_id'])
                     # Change the name
                     self.put('/file/%s' % newFile['_id'], parameters={
-                        'name': os.path.basename(filepath)
+                        'name': os.path.basename(filepath),
                     })
                     return Constant.EXTENSION_NOW_UP_TO_DATE
             else:
                 return Constant.EXTENSION_AREADY_UP_TO_DATE
 
         return extension
 
@@ -395,15 +393,15 @@
             'arch': arch,
             'baseName': name,
             'app_revision': app_revision,
             'release_id': release_id,
             'q': query,
             'limit': limit,
             'sort': 'created',
-            'sortDir': -1
+            'sortDir': -1,
         })
         return extensions
 
     def deleteExtension(self, app_name, id_or_name, coll_id=None):
         """
         Delete an extension within an application.
 
@@ -454,15 +452,15 @@
                 'arch': arch,
                 'baseName': name,
                 'repository_type': repo_type,
                 'repository_url': repo_url,
                 'revision': revision,
                 'version': version,
                 'description': desc,
-                'pre_release': pre_release
+                'pre_release': pre_release,
             }
             if build_date is not None:
                 parameters['build_date'] = build_date
             package = self.post('/app/%s/package' % app['_id'], parameters=parameters)
 
             # Upload the package
             self.uploadFileToItem(
@@ -495,27 +493,27 @@
                 'os': pkg_os,
                 'arch': arch,
                 'baseName': name,
                 'repository_type': repo_type,
                 'repository_url': repo_url,
                 'revision': revision,
                 'version': version,
-                'description': desc
+                'description': desc,
             }
             if build_date is not None:
                 parameters['build_date'] = build_date
             package = self.post('/app/%s/package' % app['_id'], parameters=parameters)
 
             files = list(self.listFile(package['_id']))
             if len(files) == 2:
                 # Remove the oldFIle
                 self.delete('/file/%s' % oldFile['_id'])
                 # Change the name
                 self.put('/file/%s' % newFile['_id'], parameters={
-                    'name': os.path.basename(filepath)
+                    'name': os.path.basename(filepath),
                 })
                 return Constant.PACKAGE_NOW_UP_TO_DATE
         return package
 
     def downloadApplicationPackage(self, app_name, id_or_name, coll_id=None,
                                    dir_path=Constant.CURRENT_FOLDER):
         """
@@ -550,29 +548,28 @@
         :param revision: Revision of the application
         :param version: Version of the application
         :param release: Name or ID of the release
         :param limit: Limit of the number of applications listed (see :const:`Constant.DEFAULT_LIMIT`)
         :return: A list of application package filtered by optional parameters
         """
         app = self._getApp(app_name=app_name, coll_id=coll_id)
-        if release and not ObjectId.is_valid(release):
-            if not self.listRelease(app_name, release):
-                raise SlicerPackageManagerError(
-                    'The release "%s" doesn\'t exist.' % release)
+        if release and not ObjectId.is_valid(release) and not self.listRelease(app_name, release):
+            raise SlicerPackageManagerError(
+                'The release "%s" does not exist.' % release)
 
         pkg = self.get('/app/%s/package' % app['_id'], parameters={
             'os': pkg_os,
             'arch': arch,
             'baseName': name,
             'revision': revision,
             'version': version,
             'release_id_or_name': release,
             'limit': limit,
             'sort': 'created',
-            'sortDir': -1
+            'sortDir': -1,
         })
         return pkg
 
     def deleteApplicationPackage(self, app_name, id_or_name, coll_id=None):
         """
         Delete an application package within an application.
```

### Comparing `slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/bson/__init__.py` & `slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/__init__.py`

 * *Files identical despite different names*

### Comparing `slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/bson/errors.py` & `slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/errors.py`

 * *Files identical despite different names*

### Comparing `slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/bson/objectid.py` & `slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/objectid.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         needed explicitly because __slots__() defined.
         """
         return self.__id
 
     def __setstate__(self, value):
         """explicit state set from pickling
         """
-        # Provide backwards compatability with OIDs
+        # Provide backwards compatibility with OIDs
         # pickled with pymongo-1.9 or older.
         if isinstance(value, dict):
             oid = value["_ObjectId__id"]
         else:
             oid = value
         # ObjectIds pickled in python 2.x used `str` for __id.
         # In python 3.x this has to be converted to `bytes`
```

### Comparing `slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/bson/py3compat.py` & `slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/py3compat.py`

 * *Files identical despite different names*

### Comparing `slicer-package-manager-client-0.7.1/slicer_package_manager_client/_vendor/bson/tz_util.py` & `slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/tz_util.py`

 * *Files identical despite different names*

### Comparing `slicer-package-manager-client-0.7.1/slicer_package_manager_client/cli.py` & `slicer-package-manager-client-0.8.0/slicer_package_manager_client/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,20 @@
 from tabulate import tabulate
 
 from girder_client import GirderClient
 from . import SlicerPackageManagerError, SlicerPackageClient, __version__, Constant
 
 w = Constant.WIDTH
 
-
-# ---------------- UTILITIES ---------------- #
-
 def _getOs():
-    os = platform.system()
-    if os == 'Linux':
-        return 'linux'
-    elif os == 'Darwin':
-        return 'macosx'
-    elif os == 'Windows':
-        return 'win'
-
-# ------------------------------------------- #
+    return {
+        "Linux": "linux",
+        "Darwin": "macosx",
+        "Windows": "win",
+        }.get(platform.system(), None)
 
 
 class SlicerPackageCli(SlicerPackageClient):
     """
     A command line Python client for interacting with a Girder instance's
     RESTful api, specifically for performing uploads into a Girder instance.
     """
@@ -43,24 +36,24 @@
         def _progressBar(*args, **kwargs):
             bar = click.progressbar(*args, **kwargs)
             bar.bar_template = "[%(bar)s]  %(info)s  %(label)s"
             bar.show_percent = True
             bar.show_pos = True
             return bar
 
-        super(SlicerPackageCli, self).__init__(host=host, port=port, apiRoot=apiRoot, scheme=scheme, apiUrl=apiUrl,
-                                               progressReporterCls=_progressBar)
+        super().__init__(host=host, port=port, apiRoot=apiRoot, scheme=scheme, apiUrl=apiUrl,
+                         progressReporterCls=_progressBar)
         interactive = password is None
         if apiKey:
             self.authenticate(apiKey=apiKey)
         elif username:
             self.authenticate(username, password, interactive=interactive)
 
     def _requestFunc(self, *args, **kwargs):
-        return super(SlicerPackageCli, self)._requestFunc(*args, **kwargs)
+        return super()._requestFunc(*args, **kwargs)
 
 
 class _HiddenOption(click.Option):
     def get_help_record(self, ctx):
         pass
 
 
@@ -86,15 +79,15 @@
                 formatter.write_dl(opts)
         if advanced_opts:
             with formatter.section('Advanced Options'):
                 formatter.write_dl(advanced_opts)
         self.format_commands(ctx, formatter)
 
 
-_CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+_CONTEXT_SETTINGS = {'help_option_names': ['-h', '--help']}
 
 
 @click.group(context_settings=_CONTEXT_SETTINGS)
 @click.option('--api-url', default=None,
               help='RESTful API URL '
                    '(e.g https://girder.example.com:443/%s)' % GirderClient.DEFAULT_API_ROOT)
 @click.option('--api-key', envvar='GIRDER_API_KEY', default=None,
@@ -147,57 +140,56 @@
     """
     # --api-url and URL by part arguments are mutually exclusive
     url_part_options = ['host', 'scheme', 'port', 'api_root']
     has_api_url = ctx.params.get('api_url', None)
     for name in url_part_options:
         has_url_part = ctx.params.get(name, None)
         if has_api_url and has_url_part:
-            raise click.BadArgumentUsage(
-                'Option "--api-url" and option "--%s" are mutually exclusive.' %
-                name.replace("_", "-"))
+            msg = f'Option "--api-url" and option "--{name.replace("_", "-")}" are mutually exclusive.'
+            raise click.BadArgumentUsage(msg)
     if certificate and no_ssl_verify:
-        raise click.BadArgumentUsage(
-            'Option "--no-ssl-verify" and option "--certificate" are mutually exclusive.')
+        msg = 'Option "--no-ssl-verify" and option "--certificate" are mutually exclusive.'
+        raise click.BadArgumentUsage(msg)
 
     ctx.obj = SlicerPackageCli(
         username, password, host=host, port=port, apiRoot=api_root,
         scheme=scheme, apiUrl=api_url, apiKey=api_key)
 
     if certificate and ctx.obj.scheme != 'https':
-        raise click.BadArgumentUsage(
-            'A URI scheme of "https" is required for option "--certificate"')
+        msg = 'A URI scheme of "https" is required for option "--certificate"'
+        raise click.BadArgumentUsage(msg)
 
 
 @main.group(context_settings=_CONTEXT_SETTINGS)
 @click.pass_obj
-def app(sc):
+def app(_sc):
     pass
 
 
 @main.group(context_settings=_CONTEXT_SETTINGS)
 @click.pass_obj
-def release(sc):
+def release(_sc):
     pass
 
 
 @main.group(context_settings=_CONTEXT_SETTINGS)
 @click.pass_obj
-def draft(sc):
+def draft(_sc):
     pass
 
 
 @main.group(context_settings=_CONTEXT_SETTINGS)
 @click.pass_obj
-def extension(sc):
+def extension(_sc):
     pass
 
 
 @main.group(context_settings=_CONTEXT_SETTINGS)
 @click.pass_obj
-def package(sc):
+def package(_sc):
     pass
 
 
 @app.command('create')
 @click.argument('name')
 @click.option('--desc', default=None,
               help='Description of the application',
@@ -216,15 +208,15 @@
               show_default=True,
               cls=_AdvancedOption)
 @click.option('--public/--private', is_flag=True, default=None,
               help='Whether the collection should be publicly visible [default: public]',
               show_default=False,
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_createApp(sc, *args, **kwargs):
+def _cli_createApp(sc: SlicerPackageClient, *args, **kwargs):
     """
     Create a new application.
     """
     try:
         application = sc.createApp(*args, **kwargs)
         print('%s (%s) %s' % (application['_id'], application['name'], 'CREATED'))
     except SlicerPackageManagerError as exc_info:
@@ -236,15 +228,15 @@
               help='ID of an existing collection',
               show_default=True,
               cls=_AdvancedOption)
 @click.option('--name', default=None,
               help='Name of the application',
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_listApp(sc, *args, **kwargs):
+def _cli_listApp(sc: SlicerPackageClient, *args, **kwargs):
     """
     List all the applications.
     """
     applications = sc.listApp(*args, **kwargs)
     table = []
     for application in applications:
         table.append([application['name'], application['_id']])
@@ -257,15 +249,15 @@
 @app.command('delete')
 @click.argument('name')
 @click.option('--coll_id', default=None, envvar='COLLECTION_ID',
               help='ID of an existing collection',
               show_default=True,
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_deleteApp(sc, *args, **kwargs):
+def _cli_deleteApp(sc: SlicerPackageClient, *args, **kwargs):
     """
     Delete an application.
     """
     try:
         application = sc.deleteApp(*args, **kwargs)
         print('%s (%s) %s' % (application['name'], application['_id'], 'DELETED'))
     except SlicerPackageManagerError as exc_info:
@@ -280,15 +272,15 @@
               help='ID of an existing collection',
               show_default=True,
               cls=_AdvancedOption)
 @click.option('--desc', default=None,
               help='Description of the release',
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_createRelease(sc, *args, **kwargs):
+def _cli_createRelease(sc: SlicerPackageClient, *args, **kwargs):
     """
     Create a new release.
     """
     try:
         rls = sc.createRelease(*args, **kwargs)
         print('%s %s (%s) %s' % (rls['name'], rls['meta']['revision'], rls['_id'], 'CREATED'))
     except SlicerPackageManagerError as exc_info:
@@ -298,26 +290,23 @@
 @release.command('list')
 @click.argument('app_name')
 @click.option('--coll_id', default=None, envvar='COLLECTION_ID',
               help='ID of an existing collection',
               show_default=True,
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_listRelease(sc, *args, **kwargs):
+def _cli_listRelease(sc: SlicerPackageClient, *args, **kwargs):
     """
     List all the releases within an application.
     """
     try:
         releases = sc.listRelease(*args, **kwargs)
         table = []
         for rls in releases:
-            if 'meta' in rls and 'revision' in rls['meta']:
-                revision = rls['meta']['revision']
-            else:
-                revision = ''
+            revision = rls.get('meta', {}).get('revision', '')
             table.append([revision, rls['name'], rls['_id']])
         print(tabulate(
             table,
             headers=['APP REVISION', 'NAME', 'RELEASE ID'],
             tablefmt="simple", numalign="left"))
     except SlicerPackageManagerError as exc_info:
         print(exc_info)
@@ -327,15 +316,15 @@
 @click.argument('app_name')
 @click.argument('name')
 @click.option('--coll_id', default=None, envvar='COLLECTION_ID',
               help='ID of an existing collection',
               show_default=True,
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_deleteRelease(sc, *args, **kwargs):
+def _cli_deleteRelease(sc: SlicerPackageClient, *args, **kwargs):
     """
     Delete a release.
     """
     try:
         rls = sc.deleteRelease(*args, **kwargs)
         print('%s %s (%s) %s' % (rls['name'], rls['meta']['revision'], rls['_id'], 'DELETED'))
     except SlicerPackageManagerError as exc_info:
@@ -354,26 +343,23 @@
 @click.option('--limit', default=Constant.DEFAULT_LIMIT,
               help='The limit number of listed releases',
               cls=_AdvancedOption)
 @click.option('--offset', default=0,
               help='Offset of the list',
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_listDraftRelease(sc, *args, **kwargs):
+def _cli_listDraftRelease(sc: SlicerPackageClient, *args, **kwargs):
     """
     List all the revisions of the default preview within an application.
     """
     try:
         releases = sc.listDraftRelease(*args, **kwargs)
         table = []
         for rls in releases:
-            if 'meta' in rls and 'revision' in rls['meta']:
-                revision = rls['meta']['revision']
-            else:
-                revision = ''
+            revision = rls.get('meta', {}).get('revision', '')
             table.append([revision, rls['name'], rls['_id']])
         print(tabulate(
             table,
             headers=['APP REVISION', 'NAME', 'RELEASE ID'],
             tablefmt="simple", numalign="left"))
     except SlicerPackageManagerError as exc_info:
         print(exc_info)
@@ -383,15 +369,15 @@
 @click.argument('app_name')
 @click.argument('revision')
 @click.option('--coll_id', default=None, envvar='COLLECTION_ID',
               help='ID of an existing collection',
               show_default=True,
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_deleteDraftRelease(sc, *args, **kwargs):
+def _cli_deleteDraftRelease(sc: SlicerPackageClient, *args, **kwargs):
     """
     Delete a specific revision within the Draft release.
     """
     try:
         rls = sc.deleteDraftRelease(*args, **kwargs)
         print('%s %s (%s) %s' % (rls['name'], rls['meta']['revision'], rls['_id'], 'DELETED'))
     except SlicerPackageManagerError as exc_info:
@@ -447,15 +433,15 @@
               help='ID of an existing collection',
               show_default=True,
               cls=_AdvancedOption)
 @click.option('--force', default=False,
               help='Force the upload',
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_uploadExtension(sc, *args, **kwargs):
+def _cli_uploadExtension(sc: SlicerPackageClient, *args, **kwargs):
     """
     Upload an extension.
     """
     try:
         print('Create the extension %s' % kwargs['name'])
         ext = sc.uploadExtension(*args, **kwargs)
         if ext == Constant.EXTENSION_AREADY_UP_TO_DATE:
@@ -475,15 +461,15 @@
               help='ID of an existing collection',
               show_default=True,
               cls=_AdvancedOption)
 @click.option('--dir_path', default=Constant.CURRENT_FOLDER,
               help='Path to the directory where will be downloaded the extension',
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_downloadExtension(sc, *args, **kwargs):
+def _cli_downloadExtension(sc: SlicerPackageClient, *args, **kwargs):
     """
     Download an extension.
     """
     try:
         print('Start download...')
         ext = sc.downloadExtension(*args, **kwargs)
         print('%s (%s) %s [%s]' % (ext['name'], ext['_id'], 'DOWNLOADED', kwargs['dir_path']))
@@ -515,15 +501,15 @@
               help='The limit number of listed extensions ',
               cls=_AdvancedOption)
 @click.option('--all', is_flag=True,
               default=False,
               help='List all the extension of the application',
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_listExtension(sc, *args, **kwargs):
+def _cli_listExtension(sc: SlicerPackageClient, *args, **kwargs):
     """
     List all the extensions within an application.
     """
     try:
         extensions = sc.listExtension(*args, **kwargs)
         rls_list = sc.listRelease(app_name=kwargs['app_name'], coll_id=kwargs['coll_id'])
         table = []
@@ -549,15 +535,15 @@
 @click.argument('app_name')
 @click.argument('id_or_name')
 @click.option('--coll_id', default=None, envvar='COLLECTION_ID',
               help='ID of an existing collection',
               show_default=True,
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_deleteExtension(sc, *args, **kwargs):
+def _cli_deleteExtension(sc: SlicerPackageClient, *args, **kwargs):
     """
     Delete an extension by ID or Name.
     """
     try:
         ext = sc.deleteExtension(*args, **kwargs)
         print('%s %s (%s) %s' % (ext['name'], ext['meta']['revision'], ext['_id'], 'DELETED'))
     except SlicerPackageManagerError as exc_info:
@@ -598,15 +584,15 @@
 @click.option('--desc', default='',
               help='Description of the package',
               cls=_AdvancedOption)
 @click.option('--pre_release', is_flag=True, default=None,
               help='Boolean to specify if the package is ready to be distributed',
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_uploadApplicationPackage(sc, *args, **kwargs):
+def _cli_uploadApplicationPackage(sc: SlicerPackageClient, *args, **kwargs):
     """
     Upload an application package.
     """
     try:
         print('Create the application package %s' % kwargs['name'])
         pkg = sc.uploadApplicationPackage(*args, **kwargs)
         if pkg == Constant.PACKAGE_NOW_UP_TO_DATE:
@@ -624,15 +610,15 @@
               help='ID of an existing collection',
               show_default=True,
               cls=_AdvancedOption)
 @click.option('--dir_path', default=Constant.CURRENT_FOLDER,
               help='Path to the directory where will be downloaded the package',
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_downloadApplicationPackage(sc, *args, **kwargs):
+def _cli_downloadApplicationPackage(sc: SlicerPackageClient, *args, **kwargs):
     """
     Download an application package.
     """
     try:
         print('Start download...')
         pkg = sc.downloadApplicationPackage(*args, **kwargs)
         print('%s (%s) %s [%s]' % (pkg['name'], pkg['_id'], 'DOWNLOADED', kwargs['dir_path']))
@@ -660,15 +646,15 @@
 @click.option('--release', default=None,
               help='List all packages within the release',
               cls=_AdvancedOption)
 @click.option('--limit', default=Constant.DEFAULT_LIMIT,
               help='The limit number of listed packages ',
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_listApplicationPackage(sc, *args, **kwargs):
+def _cli_listApplicationPackage(sc: SlicerPackageClient, *args, **kwargs):
     """
     List all the application packages within an application.
     """
     try:
         packages = sc.listApplicationPackage(*args, **kwargs)
         rls_list = sc.listRelease(app_name=kwargs['app_name'], coll_id=kwargs['coll_id'])
         table = []
@@ -693,15 +679,15 @@
 @click.argument('app_name')
 @click.argument('id_or_name')
 @click.option('--coll_id', default=None, envvar='COLLECTION_ID',
               help='ID of an existing collection',
               show_default=True,
               cls=_AdvancedOption)
 @click.pass_obj
-def _cli_deleteApplicationPackage(sc, *args, **kwargs):
+def _cli_deleteApplicationPackage(sc: SlicerPackageClient, *args, **kwargs):
     """
     Delete an application package by ID or Name.
     """
     try:
         pkg = sc.deleteApplicationPackage(*args, **kwargs)
         print('%s %s (%s) %s' % (pkg['name'], pkg['meta']['revision'], pkg['_id'], 'DELETED'))
     except SlicerPackageManagerError as exc_info:
```

### Comparing `slicer-package-manager-client-0.7.1/slicer_package_manager_client.egg-info/PKG-INFO` & `slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: slicer-package-manager-client
-Version: 0.7.1
+Version: 0.8.0
 Summary: Python client for interacting with the Slicer package manager endpoint.
 Author-email: Pierre Assemat <pierre.assemat@kitware.com>, Jean-Christophe Fillion-Robin <jchris.fillionr@kitware.com>
 Maintainer-email: Jean-Christophe Fillion-Robin <jchris.fillionr@kitware.com>
 Project-URL: Documentation, https://slicer-package-manager.readthedocs.io/en/latest/commands_shell.html#slicer-package-manager-client
 Project-URL: Source, https://github.com/girder/slicer_package_manager/tree/main/python_client
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 
 Slicer package manager Python Client
 ====================================
```

### Comparing `slicer-package-manager-client-0.7.1/slicer_package_manager_client.egg-info/SOURCES.txt` & `slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

