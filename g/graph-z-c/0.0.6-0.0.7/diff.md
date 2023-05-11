# Comparing `tmp/graph_z_c-0.0.6.tar.gz` & `tmp/graph_z_c-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_z_c-0.0.6.tar", last modified: Wed May 10 11:46:39 2023, max compression
+gzip compressed data, was "graph_z_c-0.0.7.tar", last modified: Wed May 10 12:30:33 2023, max compression
```

## Comparing `graph_z_c-0.0.6.tar` & `graph_z_c-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-10 11:46:39.844617 graph_z_c-0.0.6/
--rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-10 11:46:39.844354 graph_z_c-0.0.6/PKG-INFO
--rw-r--r--   0 zelpha     (501) staff       (20)        0 2023-05-08 02:13:18.000000 graph_z_c-0.0.6/README.md
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-10 11:46:39.842821 graph_z_c-0.0.6/graph_z/
--rw-r--r--   0 zelpha     (501) staff       (20)       73 2023-05-09 13:29:04.000000 graph_z_c-0.0.6/graph_z/__init__.py
--rw-r--r--   0 zelpha     (501) staff       (20)     5452 2023-05-10 11:44:56.000000 graph_z_c-0.0.6/graph_z/graph_z.py
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-10 11:46:39.844100 graph_z_c-0.0.6/graph_z_c.egg-info/
--rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-10 11:46:39.000000 graph_z_c-0.0.6/graph_z_c.egg-info/PKG-INFO
--rw-r--r--   0 zelpha     (501) staff       (20)      189 2023-05-10 11:46:39.000000 graph_z_c-0.0.6/graph_z_c.egg-info/SOURCES.txt
--rw-r--r--   0 zelpha     (501) staff       (20)        1 2023-05-10 11:46:39.000000 graph_z_c-0.0.6/graph_z_c.egg-info/dependency_links.txt
--rw-r--r--   0 zelpha     (501) staff       (20)        8 2023-05-10 11:46:39.000000 graph_z_c-0.0.6/graph_z_c.egg-info/top_level.txt
--rw-r--r--   0 zelpha     (501) staff       (20)       38 2023-05-10 11:46:39.844680 graph_z_c-0.0.6/setup.cfg
--rw-r--r--   0 zelpha     (501) staff       (20)      174 2023-05-10 11:46:20.000000 graph_z_c-0.0.6/setup.py
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-10 12:30:33.288224 graph_z_c-0.0.7/
+-rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-10 12:30:33.288011 graph_z_c-0.0.7/PKG-INFO
+-rw-r--r--   0 zelpha     (501) staff       (20)        0 2023-05-08 02:13:18.000000 graph_z_c-0.0.7/README.md
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-10 12:30:33.286931 graph_z_c-0.0.7/graph_z/
+-rw-r--r--   0 zelpha     (501) staff       (20)       73 2023-05-09 13:29:04.000000 graph_z_c-0.0.7/graph_z/__init__.py
+-rw-r--r--   0 zelpha     (501) staff       (20)     5492 2023-05-10 12:30:18.000000 graph_z_c-0.0.7/graph_z/graph_z.py
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-10 12:30:33.287801 graph_z_c-0.0.7/graph_z_c.egg-info/
+-rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-10 12:30:33.000000 graph_z_c-0.0.7/graph_z_c.egg-info/PKG-INFO
+-rw-r--r--   0 zelpha     (501) staff       (20)      189 2023-05-10 12:30:33.000000 graph_z_c-0.0.7/graph_z_c.egg-info/SOURCES.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)        1 2023-05-10 12:30:33.000000 graph_z_c-0.0.7/graph_z_c.egg-info/dependency_links.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)        8 2023-05-10 12:30:33.000000 graph_z_c-0.0.7/graph_z_c.egg-info/top_level.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)       38 2023-05-10 12:30:33.288278 graph_z_c-0.0.7/setup.cfg
+-rw-r--r--   0 zelpha     (501) staff       (20)      174 2023-05-10 12:30:28.000000 graph_z_c-0.0.7/setup.py
```

### Comparing `graph_z_c-0.0.6/graph_z/graph_z.py` & `graph_z_c-0.0.7/graph_z/graph_z.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         if id1 not in self.ids or id2 not in self.ids:
             print("Vertices with the given ids do not exist in this graph")
             return None
 
         vertex1, vertex2 = self.get_vertex(id1), self.get_vertex(id2)
         existance_of_copy = False
         for i, path in enumerate(self.all_paths):
-            if path[0] == id1 and path[1] == id2:
+            if (path[0] == id1 and path[1] == id2) or (path[0] == id2 and path[1] == id1):
                 existance_of_copy = True
                 self.all_paths[i] = (id1, id2, path_cost)
                 previous_cost = path[2]
                 break
         if existance_of_copy:
             vertex1.paths[vertex1.paths.index((id2, previous_cost))] = (id2, path_cost)
             vertex2.paths[vertex2.paths.index((id1, previous_cost))] = (id1, path_cost)
@@ -127,15 +127,15 @@
         return pd.DataFrame({
             "IDs": self.ids,
             "Values": values,
             "Paths (id, cost)": paths,
         })
 
 
-def generate_random_graph(num_vertices, num_paths=0, value_range=(0, 10), path_cost_range=(1, 10), random_ids=False,):
+def generate_random_graph(num_vertices, num_paths=0, value_range=(0, 10), path_cost_range=(1, 10), random_ids=False):
 
     vertex_values = np.random.randint(*value_range, size=num_vertices)
     if random_ids:
         vertex_ids = np.random.randint(0, 2**16, size=num_vertices)
     else:
         vertex_ids = np.arange(1, num_vertices+1, 1)
```

