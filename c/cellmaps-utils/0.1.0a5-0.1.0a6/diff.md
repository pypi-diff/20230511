# Comparing `tmp/cellmaps_utils-0.1.0a5.tar.gz` & `tmp/cellmaps_utils-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_utils-0.1.0a5.tar", last modified: Wed May 10 00:12:52 2023, max compression
+gzip compressed data, was "dist/cellmaps_utils-0.1.0a6.tar", last modified: Thu May 11 18:39:04 2023, max compression
```

## Comparing `cellmaps_utils-0.1.0a5.tar` & `cellmaps_utils-0.1.0a6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-10 00:12:52.302752 cellmaps_utils-0.1.0a5/
--rw-r--r--   0 churas     (504) staff       (20)      194 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a5/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3611 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a5/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-10 00:12:52.302879 cellmaps_utils-0.1.0a5/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     2813 2023-05-01 21:47:34.000000 cellmaps_utils-0.1.0a5/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-10 00:12:52.295067 cellmaps_utils-0.1.0a5/cellmaps_utils/
--rw-r--r--   0 churas     (504) staff       (20)      156 2023-05-09 23:54:28.000000 cellmaps_utils-0.1.0a5/cellmaps_utils/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     2388 2023-05-10 00:02:40.000000 cellmaps_utils-0.1.0a5/cellmaps_utils/constants.py
--rw-r--r--   0 churas     (504) staff       (20)      234 2023-05-05 00:31:11.000000 cellmaps_utils-0.1.0a5/cellmaps_utils/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)     8281 2023-05-04 23:59:25.000000 cellmaps_utils-0.1.0a5/cellmaps_utils/logutils.py
--rw-r--r--   0 churas     (504) staff       (20)     5947 2023-04-14 17:44:35.000000 cellmaps_utils-0.1.0a5/cellmaps_utils/music_utils.py
--rw-r--r--   0 churas     (504) staff       (20)    11676 2023-05-05 20:36:20.000000 cellmaps_utils-0.1.0a5/cellmaps_utils/provenance.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-10 00:12:52.296383 cellmaps_utils-0.1.0a5/cellmaps_utils.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-10 00:12:52.000000 cellmaps_utils-0.1.0a5/cellmaps_utils.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)      979 2023-05-10 00:12:52.000000 cellmaps_utils-0.1.0a5/cellmaps_utils.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-10 00:12:52.000000 cellmaps_utils-0.1.0a5/cellmaps_utils.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-10 00:12:52.000000 cellmaps_utils-0.1.0a5/cellmaps_utils.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       51 2023-05-10 00:12:52.000000 cellmaps_utils-0.1.0a5/cellmaps_utils.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       15 2023-05-10 00:12:52.000000 cellmaps_utils-0.1.0a5/cellmaps_utils.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-10 00:12:52.301108 cellmaps_utils-0.1.0a5/docs/
--rw-r--r--   0 churas     (504) staff       (20)      615 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-10 00:12:52.290711 cellmaps_utils-0.1.0a5/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-10 00:12:52.290809 cellmaps_utils-0.1.0a5/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-10 00:12:52.301840 cellmaps_utils-0.1.0a5/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a5/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a5/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a5/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)      838 2023-05-05 00:54:50.000000 cellmaps_utils-0.1.0a5/docs/cellmaps_utils.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     5991 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      282 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      852 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      442 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      812 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       73 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4304 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      784 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      182 2023-04-14 18:36:55.000000 cellmaps_utils-0.1.0a5/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      397 2023-05-10 00:12:52.303370 cellmaps_utils-0.1.0a5/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     1787 2023-05-05 21:20:31.000000 cellmaps_utils-0.1.0a5/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-10 00:12:52.302553 cellmaps_utils-0.1.0a5/tests/
--rw-r--r--   0 churas     (504) staff       (20)       69 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a5/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1541 2023-04-14 18:13:18.000000 cellmaps_utils-0.1.0a5/tests/test_logutils.py
--rw-r--r--   0 churas     (504) staff       (20)    12542 2023-05-09 21:54:19.000000 cellmaps_utils-0.1.0a5/tests/test_provenance.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.743704 cellmaps_utils-0.1.0a6/
+-rw-r--r--   0 churas     (504) staff       (20)      194 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a6/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3611 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a6/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-11 18:39:04.743832 cellmaps_utils-0.1.0a6/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     2813 2023-05-01 21:47:34.000000 cellmaps_utils-0.1.0a6/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.736841 cellmaps_utils-0.1.0a6/cellmaps_utils/
+-rw-r--r--   0 churas     (504) staff       (20)      156 2023-05-10 17:28:17.000000 cellmaps_utils-0.1.0a6/cellmaps_utils/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     3858 2023-05-11 18:35:27.000000 cellmaps_utils-0.1.0a6/cellmaps_utils/constants.py
+-rw-r--r--   0 churas     (504) staff       (20)      234 2023-05-05 00:31:11.000000 cellmaps_utils-0.1.0a6/cellmaps_utils/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)     8281 2023-05-04 23:59:25.000000 cellmaps_utils-0.1.0a6/cellmaps_utils/logutils.py
+-rw-r--r--   0 churas     (504) staff       (20)     5947 2023-04-14 17:44:35.000000 cellmaps_utils-0.1.0a6/cellmaps_utils/music_utils.py
+-rw-r--r--   0 churas     (504) staff       (20)    11676 2023-05-05 20:36:20.000000 cellmaps_utils-0.1.0a6/cellmaps_utils/provenance.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.738078 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-11 18:39:04.000000 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)      979 2023-05-11 18:39:04.000000 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-11 18:39:04.000000 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-11 18:39:04.000000 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       51 2023-05-11 18:39:04.000000 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       15 2023-05-11 18:39:04.000000 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.741841 cellmaps_utils-0.1.0a6/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      615 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.732271 cellmaps_utils-0.1.0a6/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.732383 cellmaps_utils-0.1.0a6/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.742818 cellmaps_utils-0.1.0a6/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a6/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a6/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a6/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      838 2023-05-05 00:54:50.000000 cellmaps_utils-0.1.0a6/docs/cellmaps_utils.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     5991 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      282 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      852 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      442 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      812 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       73 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4304 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      784 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      182 2023-04-14 18:36:55.000000 cellmaps_utils-0.1.0a6/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      397 2023-05-11 18:39:04.744266 cellmaps_utils-0.1.0a6/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     1787 2023-05-05 21:20:31.000000 cellmaps_utils-0.1.0a6/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.743511 cellmaps_utils-0.1.0a6/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       69 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1541 2023-04-14 18:13:18.000000 cellmaps_utils-0.1.0a6/tests/test_logutils.py
+-rw-r--r--   0 churas     (504) staff       (20)    12542 2023-05-09 21:54:19.000000 cellmaps_utils-0.1.0a6/tests/test_provenance.py
```

### Comparing `cellmaps_utils-0.1.0a5/CONTRIBUTING.rst` & `cellmaps_utils-0.1.0a6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/LICENSE` & `cellmaps_utils-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/PKG-INFO` & `cellmaps_utils-0.1.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_utils
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: Utilities needed for Cell Maps for AI
 Home-page: https://github.com/idekerlab/cellmaps_utils
 Author: Clara Hu
 Author-email: mhu@health.ucsd.edu
 License: MIT license
 Description: ==============
         cellmaps_utils
```

### Comparing `cellmaps_utils-0.1.0a5/README.rst` & `cellmaps_utils-0.1.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/cellmaps_utils/logutils.py` & `cellmaps_utils-0.1.0a6/cellmaps_utils/logutils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/cellmaps_utils/music_utils.py` & `cellmaps_utils-0.1.0a6/cellmaps_utils/music_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/cellmaps_utils/provenance.py` & `cellmaps_utils-0.1.0a6/cellmaps_utils/provenance.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/cellmaps_utils.egg-info/PKG-INFO` & `cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-utils
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: Utilities needed for Cell Maps for AI
 Home-page: https://github.com/idekerlab/cellmaps_utils
 Author: Clara Hu
 Author-email: mhu@health.ucsd.edu
 License: MIT license
 Description: ==============
         cellmaps_utils
```

### Comparing `cellmaps_utils-0.1.0a5/cellmaps_utils.egg-info/SOURCES.txt` & `cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/docs/Makefile` & `cellmaps_utils-0.1.0a6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/docs/cellmaps_utils.rst` & `cellmaps_utils-0.1.0a6/docs/cellmaps_utils.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/docs/conf.py` & `cellmaps_utils-0.1.0a6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/docs/index.rst` & `cellmaps_utils-0.1.0a6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/docs/installation.rst` & `cellmaps_utils-0.1.0a6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/docs/make.bat` & `cellmaps_utils-0.1.0a6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/docs/newrelease.rst` & `cellmaps_utils-0.1.0a6/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/docs/pypircfile.rst` & `cellmaps_utils-0.1.0a6/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/docs/versioningscheme.rst` & `cellmaps_utils-0.1.0a6/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/setup.py` & `cellmaps_utils-0.1.0a6/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/tests/test_logutils.py` & `cellmaps_utils-0.1.0a6/tests/test_logutils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a5/tests/test_provenance.py` & `cellmaps_utils-0.1.0a6/tests/test_provenance.py`

 * *Files identical despite different names*

