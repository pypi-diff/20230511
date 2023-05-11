# Comparing `tmp/bulk_directory_tree-1.0.3.tar.gz` & `tmp/bulk_directory_tree-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulk_directory_tree-1.0.3.tar", last modified: Sat Mar 18 23:15:33 2023, max compression
+gzip compressed data, was "bulk_directory_tree-1.0.4.tar", last modified: Thu May 11 10:38:10 2023, max compression
```

## Comparing `bulk_directory_tree-1.0.3.tar` & `bulk_directory_tree-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 23:15:33.845928 bulk_directory_tree-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-18 23:15:21.000000 bulk_directory_tree-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-03-18 23:15:33.845928 bulk_directory_tree-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-03-18 23:15:21.000000 bulk_directory_tree-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 23:15:33.845928 bulk_directory_tree-1.0.3/bulk_directory_tree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-03-18 23:15:33.000000 bulk_directory_tree-1.0.3/bulk_directory_tree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-18 23:15:33.000000 bulk_directory_tree-1.0.3/bulk_directory_tree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 23:15:33.000000 bulk_directory_tree-1.0.3/bulk_directory_tree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-18 23:15:33.000000 bulk_directory_tree-1.0.3/bulk_directory_tree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-18 23:15:33.000000 bulk_directory_tree-1.0.3/bulk_directory_tree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-18 23:15:33.000000 bulk_directory_tree-1.0.3/bulk_directory_tree.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1821 2023-03-18 23:15:21.000000 bulk_directory_tree-1.0.3/bulk_directory_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 23:15:33.845928 bulk_directory_tree-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-18 23:15:21.000000 bulk_directory_tree-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:38:10.885455 bulk_directory_tree-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 10:37:54.000000 bulk_directory_tree-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-11 10:38:10.885455 bulk_directory_tree-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-11 10:37:54.000000 bulk_directory_tree-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:38:10.885455 bulk_directory_tree-1.0.4/bulk_directory_tree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-11 10:38:10.000000 bulk_directory_tree-1.0.4/bulk_directory_tree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-11 10:38:10.000000 bulk_directory_tree-1.0.4/bulk_directory_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:38:10.000000 bulk_directory_tree-1.0.4/bulk_directory_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-11 10:38:10.000000 bulk_directory_tree-1.0.4/bulk_directory_tree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 10:38:10.000000 bulk_directory_tree-1.0.4/bulk_directory_tree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 10:38:10.000000 bulk_directory_tree-1.0.4/bulk_directory_tree.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1821 2023-05-11 10:37:54.000000 bulk_directory_tree-1.0.4/bulk_directory_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 10:38:10.885455 bulk_directory_tree-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-11 10:37:54.000000 bulk_directory_tree-1.0.4/setup.py
```

### Comparing `bulk_directory_tree-1.0.3/LICENSE` & `bulk_directory_tree-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bulk_directory_tree-1.0.3/PKG-INFO` & `bulk_directory_tree-1.0.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk_directory_tree
-Version: 1.0.3
+Version: 1.0.4
 Summary: Create n node d depth bulk directory tree in any directory
 Home-page: https://github.com/saumiko/bulk-directory-tree
 Author: Asif Mohaimen
 Author-email: saumik01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.6, !=3.0.*, !=3.1.*, !=3.2.*, <4
```

### Comparing `bulk_directory_tree-1.0.3/README.md` & `bulk_directory_tree-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bulk_directory_tree-1.0.3/bulk_directory_tree.egg-info/PKG-INFO` & `bulk_directory_tree-1.0.4/bulk_directory_tree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk-directory-tree
-Version: 1.0.3
+Version: 1.0.4
 Summary: Create n node d depth bulk directory tree in any directory
 Home-page: https://github.com/saumiko/bulk-directory-tree
 Author: Asif Mohaimen
 Author-email: saumik01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.6, !=3.0.*, !=3.1.*, !=3.2.*, <4
```

### Comparing `bulk_directory_tree-1.0.3/bulk_directory_tree.py` & `bulk_directory_tree-1.0.4/bulk_directory_tree.py`

 * *Files identical despite different names*

### Comparing `bulk_directory_tree-1.0.3/setup.py` & `bulk_directory_tree-1.0.4/setup.py`

 * *Files identical despite different names*

