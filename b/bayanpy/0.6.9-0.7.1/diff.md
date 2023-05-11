# Comparing `tmp/bayanpy-0.6.9.tar.gz` & `tmp/bayanpy-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.6.9.tar", last modified: Sun May  7 16:47:29 2023, max compression
+gzip compressed data, was "bayanpy-0.7.1.tar", last modified: Thu May 11 16:42:02 2023, max compression
```

## Comparing `bayanpy-0.6.9.tar` & `bayanpy-0.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-07 16:47:29.716472 bayanpy-0.6.9/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.9/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-07 16:47:29.716472 bayanpy-0.6.9/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5041 2023-05-07 15:46:50.000000 bayanpy-0.6.9/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-07 16:47:29.716472 bayanpy-0.6.9/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    57440 2023-05-07 16:46:56.000000 bayanpy-0.6.9/bayanpy/BayanImplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.6.9/bayanpy/__init__.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-07 16:47:29.716472 bayanpy-0.6.9/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-07 16:47:29.000000 bayanpy-0.6.9/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-05-07 16:47:29.000000 bayanpy-0.6.9/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-05-07 16:47:29.000000 bayanpy-0.6.9/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-05-07 16:47:29.000000 bayanpy-0.6.9/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-05-07 16:47:29.000000 bayanpy-0.6.9/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-05-07 16:47:29.716472 bayanpy-0.6.9/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-05-07 16:47:17.000000 bayanpy-0.6.9/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-11 16:42:02.964459 bayanpy-0.7.1/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.7.1/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-11 16:42:02.964459 bayanpy-0.7.1/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5350 2023-05-07 16:54:32.000000 bayanpy-0.7.1/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-11 16:42:02.964459 bayanpy-0.7.1/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    57755 2023-05-11 16:38:46.000000 bayanpy-0.7.1/bayanpy/BayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.7.1/bayanpy/__init__.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-11 16:42:02.964459 bayanpy-0.7.1/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-11 16:42:02.000000 bayanpy-0.7.1/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-05-11 16:42:02.000000 bayanpy-0.7.1/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-05-11 16:42:02.000000 bayanpy-0.7.1/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-05-11 16:42:02.000000 bayanpy-0.7.1/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-05-11 16:42:02.000000 bayanpy-0.7.1/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-05-11 16:42:02.964459 bayanpy-0.7.1/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-05-11 16:41:41.000000 bayanpy-0.7.1/setup.py
```

### Comparing `bayanpy-0.6.9/LICENSE` & `bayanpy-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.9/README.md` & `bayanpy-0.7.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-# Bayanpy: Bayan Algorithm for Community Detection
+# bayanpy: Bayan Algorithm for Community Detection
 
-Bayanpy is a Python package implementing the Bayan algorithm, a community detection method capable of providing a globally optimal solution to the modularity maximization problem. Bayan can also be implemented such that it provides an approximation of the maximum modularity with a guarantee of proximity. This algorithm is theoretically grounded by the Integer Programming (IP) formulation of the modularity maximization problem and relies on an exact branch-and-cut scheme for solving the NP-complete optimization problem to global optimality.
+bayanpy is a Python package implementing the Bayan algorithm, a community detection method capable of providing a globally optimal solution to the modularity maximization problem. Bayan can also be implemented such that it provides an approximation of the maximum modularity with a guarantee of proximity. This algorithm is theoretically grounded by the Integer Programming (IP) formulation of the modularity maximization problem and relies on an exact branch-and-cut scheme for solving the NP-complete optimization problem to global optimality.
 
 For more information, visit the [Bayan project website](https://bayanproject.github.io/).
 For a few examples of different ways you can use Bayan see this Google Colab address: [bayanpy Examples](https://tinyurl.com/bayancolab).
 
 
 ## Installation
 
-To install Bayanpy, use pip:
+To install bayanpy, use pip:
 
 ```
 pip install bayanpy
 ```
 
 ## Dependencies
 
-Bayanpy has the following dependencies:
+bayanpy has the following dependencies:
 
 - requests>=2.25.1
 - pandas>=1.3.0
 - networkx>=2.6.3
 - numpy>=1.21.0
 - gurobipy>=9.5
 - joblib>=1.1.0
+- pycombo>=0.1.7
 
-These packages will be automatically installed when you install Bayanpy using pip.
+These packages will be automatically installed when you install bayanpy using pip.
 
 
 
 ### Gurobi Installation with Free Academic License
 
-Bayanpy requires Gurobi Optimizer for models with more than 2000 variables or 2000 constraints. Gurobi is a commercial software, but it can be registered with a free academic license if the user is affiliated with a recognized degree-granting academic institution.
+bayanpy requires Gurobi Optimizer for models with more than 2000 variables or 2000 constraints. Gurobi is a commercial software, but it can be registered with a free academic license if the user is affiliated with a recognized degree-granting academic institution.
 
 Follow these steps to install Gurobi with a free academic license:
 
 1. Download and install Python 3.9 (or a later version) from [the official Python website](https://www.python.org/downloads/).
 2. Register for an account on [the Gurobi registration page](https://pages.gurobi.com/registration) to get a free academic license for using Gurobi.
-3. Download and install Gurobi Optimizer (version 9.5 or later) from [the Gurobi downloads page](https://www.gurobi.com/downloads/gurobi-optimizer-eula/) after reading and agreeing to Gurobi's End User License Agreement.
+3. Download and install Gurobi Optimizer (version 10.0 or later) from [the Gurobi downloads page](https://www.gurobi.com/downloads/gurobi-optimizer-eula/) after reading and agreeing to Gurobi's End User License Agreement.
 4. Install Gurobi into Python by running the following commands in a terminal:
 - Using Conda (recommended for Anaconda users):
 
 ```
 conda config --add channels http://conda.anaconda.org/gurobi
 conda install gurobi
 ```
@@ -50,56 +51,58 @@
 ```
 pip install gurobipy
 ```
 
 
 5. Request an academic license from [the Gurobi academic license page](https://www.gurobi.com/downloads/end-user-license-agreement-academic/) and install the license on your computer following the instructions given on the Gurobi license page.
 
-For detailed installation instructions, refer to the Gurobi Quick Start Guides for [Windows](https://www.gurobi.com/documentation/9.5/quickstart_windows/index.html), [Linux](https://www.gurobi.com/documentation/9.5/quickstart_linux/index.html), or [macOS](https://www.gurobi.com/documentation/9.5/quickstart_mac/index.html).
+For detailed installation instructions, refer to the Gurobi Quick Start Guides for [Windows](https://www.gurobi.com/documentation/10.0/quickstart_windows/index.html), [Linux](https://www.gurobi.com/documentation/10.0/quickstart_linux/index.html), or [macOS](https://www.gurobi.com/documentation/10.0/quickstart_mac/index.html).
 
 ## Usage
 
-You can use Bayanpy as a standalone package. After installing Bayanpy, you can use it directly in your Python code as follows:
+You can use bayanpy as a standalone package. After installing bayanpy, you can use it directly in your Python code as follows:
 
 ```python
 import networkx as nx
 import bayanpy
 
 # Create or load your networkx graph (undirected)
-graph = G = nx.karate_club_graph()
+graph = nx.karate_club_graph()
 
 # Run the Bayan algorithm
-modularity, optimality_gap, community = bayanpy.bayan(graph, threshold=0.001, time_allowed=60, resolution=1)
+modularity, optimality_gap, community, modeling_time, solve_time = bayanpy.bayan(graph, threshold=0.001, time_allowed=60, resolution=1)
 ```
 
 
 
 #### Parameters and acceptable input
 
 - `graph`: Input graph should be an undirected networkx graph. You can use the edge attribute "weight" to represent positive edge weights.
-- `threshold`: The acceptable optimality gap for the algorithm to terminate. If Bayan finds a solution with a modularity value within the specified threshold of the optimal solution, it stops the search and returns the found solution. For example, setting the threshold to 0.001 means Bayan will stop when it finds a solution within 0.1% of the optimal modularity value.
-- `time_allowed`: The maximum allowed execution time in seconds for Bayan to search for a solution. Once this time limit is reached, the algorithm will terminate and return the best solution found so far, even if the optimality gap threshold has not been met.
-- `resolution`: The resolution parameter in the modularity function.
+- `threshold`: The acceptable optimality gap for the algorithm to terminate. If Bayan finds a solution with a modularity value within the specified threshold of the optimal solution, it stops the search and returns the found solution. For example, setting the threshold to 0.01 means Bayan will stop when it finds a solution within 1% of the maximum modularity for that graph.
+- `time_allowed`: The maximum allowed execution time in seconds for Bayan to search for a solution. Shortly after this time limit is reached, the algorithm will terminate and returns the best solution found so far, even if the optimality gap threshold has not been met.
+- `resolution`: The resolution parameter (gamma) used in the modularity function.
 
 #### Returns
 
 - `modularity`: The modularity value of the returned partition.
 - `optimality_gap`: The guaranteed upper bound of the percentage difference between the modularity of the returned partition and the maximum modularity.
 - `community`: A nested list describing the community assignment of the returned partition.
+- `modeling_time`: The seconds taken for pre-processing the input and formulating the optimization model.
+- `solve_time`: The seconds taken for solving the optimization model using the Bayan algorithm.
 
 
 ### Example
 You can find a few examples of different ways Bayan can be used at this Google Colab address: [bayanpy Examples](https://tinyurl.com/bayancolab)
 
 
 ## Contributing
 
-We welcome contributions to the Bayanpy project. If you have any suggestions or encounter any issues, please feel free to open an issue or submit a pull request on the GitHub repository.
+We welcome contributions to the [Bayan project](https://bayanproject.github.io/). If you have any suggestions or encounter any issues, please feel free to open an issue or submit a pull request on this GitHub repository.
 
 ## License
 
-Bayanpy is released under the [GNU General Public License](LICENSE). For more information, please refer to the [LICENSE](LICENSE) file in the repository.
+bayanpy is released under the [GNU General Public License](LICENSE). For more information, please refer to the [LICENSE](LICENSE) file in the repository.
```

### Comparing `bayanpy-0.6.9/bayanpy/BayanImplied.py` & `bayanpy-0.7.1/bayanpy/BayanImplied.py`

 * *Files 0% similar despite different names*

```diff
@@ -999,47 +999,53 @@
     else:
         gap = (upper_bound - lower_bound) / upper_bound
         out = lower_bound, gap, communities, preprocessing_time+formulation_time, solve_time
     return out
 
 
 def bayan(G, threshold=0.001, time_allowed=600, delta=0.7, resolution=1, lp_method=4, develop_mode=False):
-    G = nx.convert_node_labels_to_integers(G, label_attribute="original_label")
-    mapping = nx.get_node_attributes(G, 'original_label')
     # Running Bayan for a network with multiple connected components
     optimal_partition = []
     list_of_subgraphs = [G.subgraph(c).copy() for c in nx.connected_components(G)]
     n_sub = len(list_of_subgraphs)
     sub_results = {}
     total_gap = 0
     total_modeling_time = 0
     total_solve_time = 0
     total_preprocessing_time = 0
     total_formulation_time = 0
     threshold_sub = threshold / n_sub
     for sub_inx, sub_graph in enumerate(list_of_subgraphs):
+
+        sub_graph = nx.convert_node_labels_to_integers(sub_graph, label_attribute="original_label")
+        mapping = nx.get_node_attributes(sub_graph, 'original_label')
+
         bayan_output = alg(sub_graph, threshold=threshold_sub, time_allowed=time_allowed, delta=delta,
               resolution=resolution, lp_method=lp_method, develop_mode=develop_mode)
 
         if develop_mode:
             sub_results[sub_inx] = bayan_output
-            optimal_partition += bayan_output[3]
+            optimal_partition += [[mapping[i] for i in com] for com in bayan_output[3]]
             total_preprocessing_time += bayan_output[4]
             total_formulation_time += bayan_output[5]
             total_solve_time += bayan_output[6]
 
         else:
-            optimal_partition += bayan_output[2]
+            optimal_partition += [[mapping[i] for i in com] for com in bayan_output[3]]
             total_gap += bayan_output[1]
             total_modeling_time += bayan_output[3]
             total_solve_time += bayan_output[4]
     print(optimal_partition)
-    lower_bound = calculate_modularity(optimal_partition, G, resolution)
 
-    optimal_partition = [[mapping[i] for i in com] for com in optimal_partition]
+    G = nx.convert_node_labels_to_integers(G, label_attribute="original_label")
+    mapping = nx.get_node_attributes(G, 'original_label')
+    mapping ={val: key for key, val in mapping.items()}
+    int_optimal_partition = [[mapping[i] for i in com] for com in optimal_partition]
+    lower_bound = calculate_modularity(int_optimal_partition, G, resolution)
+
 
     if develop_mode:
         for sub_inx, sub_graph in enumerate(list_of_subgraphs):
             print(f"Connected component {sub_inx}")
             print(sub_results[sub_inx])
         out = lower_bound, optimal_partition,  total_preprocessing_time, total_formulation_time,total_solve_time
     else:
```

### Comparing `bayanpy-0.6.9/setup.py` & `bayanpy-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.6.9",
+    version="0.7.1",
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
```

