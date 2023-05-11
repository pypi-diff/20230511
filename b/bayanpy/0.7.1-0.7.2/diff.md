# Comparing `tmp/bayanpy-0.7.1.tar.gz` & `tmp/bayanpy-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.7.1.tar", last modified: Thu May 11 16:42:02 2023, max compression
+gzip compressed data, was "bayanpy-0.7.2.tar", last modified: Thu May 11 16:47:04 2023, max compression
```

## Comparing `bayanpy-0.7.1.tar` & `bayanpy-0.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-11 16:42:02.964459 bayanpy-0.7.1/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.7.1/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-11 16:42:02.964459 bayanpy-0.7.1/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5350 2023-05-07 16:54:32.000000 bayanpy-0.7.1/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-11 16:42:02.964459 bayanpy-0.7.1/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    57755 2023-05-11 16:38:46.000000 bayanpy-0.7.1/bayanpy/BayanImplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.7.1/bayanpy/__init__.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-11 16:42:02.964459 bayanpy-0.7.1/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-11 16:42:02.000000 bayanpy-0.7.1/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-05-11 16:42:02.000000 bayanpy-0.7.1/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-05-11 16:42:02.000000 bayanpy-0.7.1/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-05-11 16:42:02.000000 bayanpy-0.7.1/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-05-11 16:42:02.000000 bayanpy-0.7.1/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-05-11 16:42:02.964459 bayanpy-0.7.1/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-05-11 16:41:41.000000 bayanpy-0.7.1/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-11 16:47:04.403252 bayanpy-0.7.2/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.7.2/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-11 16:47:04.403252 bayanpy-0.7.2/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5350 2023-05-07 16:54:32.000000 bayanpy-0.7.2/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-11 16:47:04.403252 bayanpy-0.7.2/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    57757 2023-05-11 16:44:44.000000 bayanpy-0.7.2/bayanpy/BayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.7.2/bayanpy/__init__.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-11 16:47:04.403252 bayanpy-0.7.2/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-11 16:47:04.000000 bayanpy-0.7.2/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-05-11 16:47:04.000000 bayanpy-0.7.2/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-05-11 16:47:04.000000 bayanpy-0.7.2/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-05-11 16:47:04.000000 bayanpy-0.7.2/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-05-11 16:47:04.000000 bayanpy-0.7.2/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-05-11 16:47:04.403252 bayanpy-0.7.2/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-05-11 16:46:44.000000 bayanpy-0.7.2/setup.py
```

### Comparing `bayanpy-0.7.1/LICENSE` & `bayanpy-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.7.1/README.md` & `bayanpy-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `bayanpy-0.7.1/bayanpy/BayanImplied.py` & `bayanpy-0.7.2/bayanpy/BayanImplied.py`

 * *Files 0% similar despite different names*

```diff
@@ -1026,19 +1026,19 @@
             sub_results[sub_inx] = bayan_output
             optimal_partition += [[mapping[i] for i in com] for com in bayan_output[3]]
             total_preprocessing_time += bayan_output[4]
             total_formulation_time += bayan_output[5]
             total_solve_time += bayan_output[6]
 
         else:
-            optimal_partition += [[mapping[i] for i in com] for com in bayan_output[3]]
+            optimal_partition += [[mapping[i] for i in com] for com in bayan_output[2]]
             total_gap += bayan_output[1]
             total_modeling_time += bayan_output[3]
             total_solve_time += bayan_output[4]
-    print(optimal_partition)
+    # print(optimal_partition)
 
     G = nx.convert_node_labels_to_integers(G, label_attribute="original_label")
     mapping = nx.get_node_attributes(G, 'original_label')
     mapping ={val: key for key, val in mapping.items()}
     int_optimal_partition = [[mapping[i] for i in com] for com in optimal_partition]
     lower_bound = calculate_modularity(int_optimal_partition, G, resolution)
```

### Comparing `bayanpy-0.7.1/setup.py` & `bayanpy-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.7.1",
+    version="0.7.2",
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
```

