# Comparing `tmp/onedep_biocuration_api-0.2.tar.gz` & `tmp/onedep_biocuration_api-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onedep_biocuration_api-0.2.tar", last modified: Tue May 31 16:58:15 2022, max compression
+gzip compressed data, was "onedep_biocuration_api-0.3.tar", last modified: Thu May 11 12:32:29 2023, max compression
```

## Comparing `onedep_biocuration_api-0.2.tar` & `onedep_biocuration_api-0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-05-31 16:58:15.066101 onedep_biocuration_api-0.2/
--rw-r--r--   0 peisach    (502) staff       (20)      145 2022-05-31 16:57:03.000000 onedep_biocuration_api-0.2/HISTORY.txt
--rw-r--r--   0 peisach    (502) staff       (20)      603 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.2/LICENSE
--rw-r--r--   0 peisach    (502) staff       (20)       73 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.2/MANIFEST.in
--rw-r--r--   0 peisach    (502) staff       (20)      860 2022-05-31 16:58:15.066244 onedep_biocuration_api-0.2/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)     4656 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.2/README.md
--rw-r--r--   0 peisach    (502) staff       (20)       16 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.2/README.txt
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-05-31 16:58:15.061209 onedep_biocuration_api-0.2/onedep_biocuration/
--rw-r--r--   0 peisach    (502) staff       (20)      209 2022-05-31 16:56:27.000000 onedep_biocuration_api-0.2/onedep_biocuration/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-05-31 16:58:15.061786 onedep_biocuration_api-0.2/onedep_biocuration/api/
--rw-r--r--   0 peisach    (502) staff       (20)     5082 2022-05-27 11:54:22.000000 onedep_biocuration_api-0.2/onedep_biocuration/api/ContentRequest.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.2/onedep_biocuration/api/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-05-31 16:58:15.062385 onedep_biocuration_api-0.2/onedep_biocuration/cli/
--rw-r--r--   0 peisach    (502) staff       (20)        0 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.2/onedep_biocuration/cli/__init__.py
--rw-r--r--   0 peisach    (502) staff       (20)    11967 2022-05-31 16:54:37.000000 onedep_biocuration_api-0.2/onedep_biocuration/cli/biocuration_cli.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-05-31 16:58:15.063059 onedep_biocuration_api-0.2/onedep_biocuration/utils/
--rw-r--r--   0 peisach    (502) staff       (20)    18854 2022-05-27 12:00:28.000000 onedep_biocuration_api-0.2/onedep_biocuration/utils/ApiBase.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.2/onedep_biocuration/utils/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-05-31 16:58:15.065850 onedep_biocuration_api-0.2/onedep_biocuration_api.egg-info/
--rw-r--r--   0 peisach    (502) staff       (20)      860 2022-05-31 16:58:14.000000 onedep_biocuration_api-0.2/onedep_biocuration_api.egg-info/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)      651 2022-05-31 16:58:15.000000 onedep_biocuration_api-0.2/onedep_biocuration_api.egg-info/SOURCES.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2022-05-31 16:58:14.000000 onedep_biocuration_api-0.2/onedep_biocuration_api.egg-info/dependency_links.txt
--rw-r--r--   0 peisach    (502) staff       (20)       78 2022-05-31 16:58:14.000000 onedep_biocuration_api-0.2/onedep_biocuration_api.egg-info/entry_points.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2022-05-27 11:37:16.000000 onedep_biocuration_api-0.2/onedep_biocuration_api.egg-info/not-zip-safe
--rw-r--r--   0 peisach    (502) staff       (20)       52 2022-05-31 16:58:14.000000 onedep_biocuration_api-0.2/onedep_biocuration_api.egg-info/requires.txt
--rw-r--r--   0 peisach    (502) staff       (20)       19 2022-05-31 16:58:14.000000 onedep_biocuration_api-0.2/onedep_biocuration_api.egg-info/top_level.txt
--rwxr-xr-x   0 peisach    (502) staff       (20)      108 2022-05-31 16:58:15.066946 onedep_biocuration_api-0.2/setup.cfg
--rwxr-xr-x   0 peisach    (502) staff       (20)     1984 2022-05-27 11:54:22.000000 onedep_biocuration_api-0.2/setup.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-05-11 12:32:29.583937 onedep_biocuration_api-0.3/
+-rw-r--r--   0 peisach    (502) staff       (20)      194 2023-05-11 12:31:38.000000 onedep_biocuration_api-0.3/HISTORY.txt
+-rw-r--r--   0 peisach    (502) staff       (20)      603 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.3/LICENSE
+-rw-r--r--   0 peisach    (502) staff       (20)       73 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.3/MANIFEST.in
+-rw-r--r--   0 peisach    (502) staff       (20)      860 2023-05-11 12:32:29.584068 onedep_biocuration_api-0.3/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)     4656 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.3/README.md
+-rw-r--r--   0 peisach    (502) staff       (20)       16 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.3/README.txt
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-05-11 12:32:29.577885 onedep_biocuration_api-0.3/onedep_biocuration/
+-rw-r--r--   0 peisach    (502) staff       (20)      209 2023-05-11 12:31:03.000000 onedep_biocuration_api-0.3/onedep_biocuration/__init__.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-05-11 12:32:29.578759 onedep_biocuration_api-0.3/onedep_biocuration/api/
+-rw-r--r--   0 peisach    (502) staff       (20)     5082 2022-05-27 11:54:22.000000 onedep_biocuration_api-0.3/onedep_biocuration/api/ContentRequest.py
+-rw-r--r--   0 peisach    (502) staff       (20)        0 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.3/onedep_biocuration/api/__init__.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-05-11 12:32:29.579381 onedep_biocuration_api-0.3/onedep_biocuration/cli/
+-rw-r--r--   0 peisach    (502) staff       (20)        0 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.3/onedep_biocuration/cli/__init__.py
+-rw-r--r--   0 peisach    (502) staff       (20)    11967 2022-05-31 16:54:37.000000 onedep_biocuration_api-0.3/onedep_biocuration/cli/biocuration_cli.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-05-11 12:32:29.580308 onedep_biocuration_api-0.3/onedep_biocuration/utils/
+-rw-r--r--   0 peisach    (502) staff       (20)    18854 2022-05-27 12:00:28.000000 onedep_biocuration_api-0.3/onedep_biocuration/utils/ApiBase.py
+-rw-r--r--   0 peisach    (502) staff       (20)        0 2022-05-27 11:33:01.000000 onedep_biocuration_api-0.3/onedep_biocuration/utils/__init__.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-05-11 12:32:29.583619 onedep_biocuration_api-0.3/onedep_biocuration_api.egg-info/
+-rw-r--r--   0 peisach    (502) staff       (20)      860 2023-05-11 12:32:29.000000 onedep_biocuration_api-0.3/onedep_biocuration_api.egg-info/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)      651 2023-05-11 12:32:29.000000 onedep_biocuration_api-0.3/onedep_biocuration_api.egg-info/SOURCES.txt
+-rw-r--r--   0 peisach    (502) staff       (20)        1 2023-05-11 12:32:29.000000 onedep_biocuration_api-0.3/onedep_biocuration_api.egg-info/dependency_links.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       78 2023-05-11 12:32:29.000000 onedep_biocuration_api-0.3/onedep_biocuration_api.egg-info/entry_points.txt
+-rw-r--r--   0 peisach    (502) staff       (20)        1 2022-05-27 11:37:16.000000 onedep_biocuration_api-0.3/onedep_biocuration_api.egg-info/not-zip-safe
+-rw-r--r--   0 peisach    (502) staff       (20)       52 2023-05-11 12:32:29.000000 onedep_biocuration_api-0.3/onedep_biocuration_api.egg-info/requires.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       19 2023-05-11 12:32:29.000000 onedep_biocuration_api-0.3/onedep_biocuration_api.egg-info/top_level.txt
+-rwxr-xr-x   0 peisach    (502) staff       (20)      108 2023-05-11 12:32:29.584584 onedep_biocuration_api-0.3/setup.cfg
+-rwxr-xr-x   0 peisach    (502) staff       (20)     1984 2022-05-27 11:54:22.000000 onedep_biocuration_api-0.3/setup.py
```

### Comparing `onedep_biocuration_api-0.2/LICENSE` & `onedep_biocuration_api-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `onedep_biocuration_api-0.2/PKG-INFO` & `onedep_biocuration_api-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedep_biocuration_api
-Version: 0.2
+Version: 0.3
 Summary: wwPDB OneDep Biocuration Web Service API.
 Home-page: http://wwpdb.org/
 Author: wwPDB OneDep Development Team
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `onedep_biocuration_api-0.2/README.md` & `onedep_biocuration_api-0.3/README.md`

 * *Files identical despite different names*

### Comparing `onedep_biocuration_api-0.2/onedep_biocuration/api/ContentRequest.py` & `onedep_biocuration_api-0.3/onedep_biocuration/api/ContentRequest.py`

 * *Files identical despite different names*

### Comparing `onedep_biocuration_api-0.2/onedep_biocuration/cli/biocuration_cli.py` & `onedep_biocuration_api-0.3/onedep_biocuration/cli/biocuration_cli.py`

 * *Files identical despite different names*

### Comparing `onedep_biocuration_api-0.2/onedep_biocuration/utils/ApiBase.py` & `onedep_biocuration_api-0.3/onedep_biocuration/utils/ApiBase.py`

 * *Files identical despite different names*

### Comparing `onedep_biocuration_api-0.2/onedep_biocuration_api.egg-info/PKG-INFO` & `onedep_biocuration_api-0.3/onedep_biocuration_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedep-biocuration-api
-Version: 0.2
+Version: 0.3
 Summary: wwPDB OneDep Biocuration Web Service API.
 Home-page: http://wwpdb.org/
 Author: wwPDB OneDep Development Team
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `onedep_biocuration_api-0.2/onedep_biocuration_api.egg-info/SOURCES.txt` & `onedep_biocuration_api-0.3/onedep_biocuration_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onedep_biocuration_api-0.2/setup.py` & `onedep_biocuration_api-0.3/setup.py`

 * *Files identical despite different names*

