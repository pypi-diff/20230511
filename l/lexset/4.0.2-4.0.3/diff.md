# Comparing `tmp/lexset-4.0.2.tar.gz` & `tmp/lexset-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexset-4.0.2.tar", last modified: Wed May 10 23:04:03 2023, max compression
+gzip compressed data, was "lexset-4.0.3.tar", last modified: Wed May 10 23:06:12 2023, max compression
```

## Comparing `lexset-4.0.2.tar` & `lexset-4.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:04:03.754242 lexset-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 23:04:03.754242 lexset-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 23:03:46.000000 lexset-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:04:03.750242 lexset-4.0.2/lexset/
--rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-05-10 23:03:46.000000 lexset-4.0.2/lexset/LexsetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 23:03:46.000000 lexset-4.0.2/lexset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-10 23:03:46.000000 lexset-4.0.2/lexset/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:04:03.754242 lexset-4.0.2/lexset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 23:04:03.000000 lexset-4.0.2/lexset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 23:04:03.000000 lexset-4.0.2/lexset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 23:04:03.000000 lexset-4.0.2/lexset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 23:04:03.000000 lexset-4.0.2/lexset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 23:04:03.000000 lexset-4.0.2/lexset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 23:04:03.754242 lexset-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-10 23:03:46.000000 lexset-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:06:12.053693 lexset-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 23:06:12.053693 lexset-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 23:05:54.000000 lexset-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:06:12.053693 lexset-4.0.3/lexset/
+-rw-r--r--   0 runner    (1001) docker     (123)    29166 2023-05-10 23:05:54.000000 lexset-4.0.3/lexset/LexsetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 23:05:54.000000 lexset-4.0.3/lexset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-10 23:05:54.000000 lexset-4.0.3/lexset/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:06:12.053693 lexset-4.0.3/lexset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 23:06:12.000000 lexset-4.0.3/lexset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 23:06:12.000000 lexset-4.0.3/lexset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 23:06:12.000000 lexset-4.0.3/lexset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 23:06:12.000000 lexset-4.0.3/lexset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 23:06:12.000000 lexset-4.0.3/lexset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 23:06:12.053693 lexset-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-10 23:05:54.000000 lexset-4.0.3/setup.py
```

### Comparing `lexset-4.0.2/lexset/LexsetManager.py` & `lexset-4.0.3/lexset/LexsetManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,16 +136,17 @@
         try:
             id_list = self.dataset_id
         except:
             try:
                 id_list = self.get_dataset_id()
             except:
                 print("\33[1;31;40mNo dataset associated with this simulation. \33[0m")
+                return
+
             print("\33[1;31;40mGetting dataset id. \33[0m")
-            return
 
         #DIVIDE DATASET INTO PARTS
         def divide_into_parts(file_size, num_workers):
             part_size = file_size // num_workers
             part_starts = [i * part_size for i in range(num_workers)]
             part_ends = [(i + 1) * part_size - 1 for i in range(num_workers - 1)] + [file_size - 1]
             return list(zip(part_starts, part_ends))
```

### Comparing `lexset-4.0.2/lexset/credentials.py` & `lexset-4.0.3/lexset/credentials.py`

 * *Files identical despite different names*

