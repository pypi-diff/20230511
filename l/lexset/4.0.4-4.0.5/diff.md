# Comparing `tmp/lexset-4.0.4.tar.gz` & `tmp/lexset-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexset-4.0.4.tar", last modified: Wed May 10 23:13:04 2023, max compression
+gzip compressed data, was "lexset-4.0.5.tar", last modified: Wed May 10 23:29:39 2023, max compression
```

## Comparing `lexset-4.0.4.tar` & `lexset-4.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:04.941019 lexset-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 23:13:04.941019 lexset-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 23:12:47.000000 lexset-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:04.941019 lexset-4.0.4/lexset/
--rw-r--r--   0 runner    (1001) docker     (123)    29217 2023-05-10 23:12:47.000000 lexset-4.0.4/lexset/LexsetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 23:12:47.000000 lexset-4.0.4/lexset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-10 23:12:47.000000 lexset-4.0.4/lexset/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:04.941019 lexset-4.0.4/lexset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 23:13:04.000000 lexset-4.0.4/lexset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 23:13:04.000000 lexset-4.0.4/lexset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 23:13:04.000000 lexset-4.0.4/lexset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 23:13:04.000000 lexset-4.0.4/lexset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 23:13:04.000000 lexset-4.0.4/lexset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 23:13:04.941019 lexset-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-10 23:12:47.000000 lexset-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:29:39.169370 lexset-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 23:29:39.169370 lexset-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 23:29:18.000000 lexset-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:29:39.169370 lexset-4.0.5/lexset/
+-rw-r--r--   0 runner    (1001) docker     (123)    28981 2023-05-10 23:29:18.000000 lexset-4.0.5/lexset/LexsetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 23:29:18.000000 lexset-4.0.5/lexset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-10 23:29:18.000000 lexset-4.0.5/lexset/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:29:39.169370 lexset-4.0.5/lexset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 23:29:39.000000 lexset-4.0.5/lexset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 23:29:39.000000 lexset-4.0.5/lexset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 23:29:39.000000 lexset-4.0.5/lexset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 23:29:39.000000 lexset-4.0.5/lexset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 23:29:39.000000 lexset-4.0.5/lexset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 23:29:39.169370 lexset-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-10 23:29:18.000000 lexset-4.0.5/setup.py
```

### Comparing `lexset-4.0.4/lexset/LexsetManager.py` & `lexset-4.0.5/lexset/LexsetManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,25 +130,18 @@
         else:
             print("\33[1;31;40mget_organization_simulations() Error: " + str(response.status_code) + "\33[0m")
             return(response.status_code)
 
     def download(self, localPath="NONE", workers=2):
         #CHECK IF DATASET ID IS SET
         try:
-            id_list = self.dataset_ids
+            id_list = self.dataset_id
         except:
-            try:
-                self.get_dataset_id()
-                id_list = self.dataset_ids
-                
-            except:
-                print("\33[1;31;40mNo dataset associated with this simulation. \33[0m")
-                return
-
-            print("\33[1;31;40mGetting dataset id. \33[0m")
+            self.get_dataset_id()
+            id_list = self.dataset_id
 
         #DIVIDE DATASET INTO PARTS
         def divide_into_parts(file_size, num_workers):
             part_size = file_size // num_workers
             part_starts = [i * part_size for i in range(num_workers)]
             part_ends = [(i + 1) * part_size - 1 for i in range(num_workers - 1)] + [file_size - 1]
             return list(zip(part_starts, part_ends))
```

### Comparing `lexset-4.0.4/lexset/credentials.py` & `lexset-4.0.5/lexset/credentials.py`

 * *Files identical despite different names*

