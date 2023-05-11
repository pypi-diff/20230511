# Comparing `tmp/computation-graph-7.tar.gz` & `tmp/computation-graph-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/computation-graph-7.tar", last modified: Thu Apr  1 14:37:35 2021, max compression
+gzip compressed data, was "dist/computation-graph-9.tar", last modified: Thu Apr 29 18:25:23 2021, max compression
```

## Comparing `computation-graph-7.tar` & `computation-graph-9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-01 14:37:35.590687 computation-graph-7/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1756 2021-04-01 14:37:35.590687 computation-graph-7/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1305 2021-04-01 14:36:50.000000 computation-graph-7/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-01 14:37:35.590687 computation-graph-7/computation_graph/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-01 14:36:50.000000 computation-graph-7/computation_graph/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1540 2021-04-01 14:36:50.000000 computation-graph-7/computation_graph/base_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7025 2021-04-01 14:36:50.000000 computation-graph-7/computation_graph/composers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      882 2021-04-01 14:36:50.000000 computation-graph-7/computation_graph/debug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1189 2021-04-01 14:36:50.000000 computation-graph-7/computation_graph/debug_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3981 2021-04-01 14:36:50.000000 computation-graph-7/computation_graph/graph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16471 2021-04-01 14:36:50.000000 computation-graph-7/computation_graph/graph_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15582 2021-04-01 14:36:50.000000 computation-graph-7/computation_graph/run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4499 2021-04-01 14:36:50.000000 computation-graph-7/computation_graph/visualization.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-01 14:37:35.590687 computation-graph-7/computation_graph.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1756 2021-04-01 14:37:35.000000 computation-graph-7/computation_graph.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      508 2021-04-01 14:37:35.000000 computation-graph-7/computation_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-04-01 14:37:35.000000 computation-graph-7/computation_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       52 2021-04-01 14:37:35.000000 computation-graph-7/computation_graph.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2021-04-01 14:37:35.000000 computation-graph-7/computation_graph.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2021-04-01 14:36:50.000000 computation-graph-7/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-04-01 14:37:35.590687 computation-graph-7/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      409 2021-04-01 14:36:50.000000 computation-graph-7/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-29 18:25:23.729852 computation-graph-9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1063 2021-04-29 18:24:42.000000 computation-graph-9/LICENSE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1756 2021-04-29 18:25:23.729852 computation-graph-9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1305 2021-04-29 18:24:42.000000 computation-graph-9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-29 18:25:23.729852 computation-graph-9/computation_graph/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-29 18:24:42.000000 computation-graph-9/computation_graph/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1540 2021-04-29 18:24:42.000000 computation-graph-9/computation_graph/base_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7025 2021-04-29 18:24:42.000000 computation-graph-9/computation_graph/composers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      882 2021-04-29 18:24:42.000000 computation-graph-9/computation_graph/debug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1189 2021-04-29 18:24:42.000000 computation-graph-9/computation_graph/debug_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3981 2021-04-29 18:24:42.000000 computation-graph-9/computation_graph/graph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16782 2021-04-29 18:24:42.000000 computation-graph-9/computation_graph/graph_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15541 2021-04-29 18:24:42.000000 computation-graph-9/computation_graph/run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4499 2021-04-29 18:24:42.000000 computation-graph-9/computation_graph/visualization.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-29 18:25:23.729852 computation-graph-9/computation_graph.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1756 2021-04-29 18:25:23.000000 computation-graph-9/computation_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      519 2021-04-29 18:25:23.000000 computation-graph-9/computation_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-04-29 18:25:23.000000 computation-graph-9/computation_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       52 2021-04-29 18:25:23.000000 computation-graph-9/computation_graph.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       18 2021-04-29 18:25:23.000000 computation-graph-9/computation_graph.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       46 2021-04-29 18:24:42.000000 computation-graph-9/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-04-29 18:25:23.729852 computation-graph-9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      409 2021-04-29 18:24:42.000000 computation-graph-9/setup.py
```

### Comparing `computation-graph-7/PKG-INFO` & `computation-graph-9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computation-graph
-Version: 7
+Version: 9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.com/hyroai/computation-graph.svg?branch=master)](https://travis-ci.com/hyroai/computation-graph)
         
         A functional composition framework that supports:
```

### Comparing `computation-graph-7/README.md` & `computation-graph-9/README.md`

 * *Files identical despite different names*

### Comparing `computation-graph-7/computation_graph/base_types.py` & `computation-graph-9/computation_graph/base_types.py`

 * *Files identical despite different names*

### Comparing `computation-graph-7/computation_graph/composers.py` & `computation-graph-9/computation_graph/composers.py`

 * *Files identical despite different names*

### Comparing `computation-graph-7/computation_graph/debug.py` & `computation-graph-9/computation_graph/debug.py`

 * *Files identical despite different names*

### Comparing `computation-graph-7/computation_graph/debug_test.py` & `computation-graph-9/computation_graph/debug_test.py`

 * *Files identical despite different names*

### Comparing `computation-graph-7/computation_graph/graph.py` & `computation-graph-9/computation_graph/graph.py`

 * *Files identical despite different names*

### Comparing `computation-graph-7/computation_graph/graph_test.py` & `computation-graph-9/computation_graph/graph_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,25 @@
     )
     result = cg(arg1=_ROOT_VALUE)
 
     assert isinstance(result, base_types.ComputationResult)
     assert result.result == f"node2(node1({_ROOT_VALUE}))"
 
 
+def test_none_as_input():
+    cg = run.to_callable(
+        (graph.make_edge(source=node1, destination=node2, key="arg1"),),
+        frozenset([GraphTestException]),
+    )
+    result = cg(arg1=None)
+
+    assert isinstance(result, base_types.ComputationResult)
+    assert result.result == "node2(node1(None))"
+
+
 async def test_simple_async():
     cg = run.to_callable(
         (graph.make_edge(source=node1_async, destination=node2, key="arg1"),),
         frozenset([GraphTestException]),
     )
     result = await cg(arg1=_ROOT_VALUE)
```

### Comparing `computation-graph-7/computation_graph/run.py` & `computation-graph-9/computation_graph/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,19 +111,20 @@
 
 
 def _get_outer_kwargs(
     unbound_signature: base_types.NodeSignature,
     unbound_input: base_types.ComputationInput,
 ) -> Dict[Text, Any]:
     return gamla.pipe(
-        unbound_signature.kwargs,
-        gamla.remove(gamla.equals("state")),
-        gamla.map(gamla.pair_right(unbound_input.kwargs.get)),
-        gamla.remove(gamla.compose_left(gamla.second, gamla.equals(None))),
-        dict,
+        unbound_input.kwargs,
+        gamla.keyfilter(
+            gamla.alljuxt(
+                gamla.not_equals("state"), gamla.contains(unbound_signature.kwargs)
+            )
+        ),
     )
 
 
 _get_inner_kwargs = gamla.compose_left(
     gamla.keyfilter(_get_edge_key),
     dict.items,
     gamla.groupby(gamla.compose_left(gamla.head, _get_edge_key)),
```

### Comparing `computation-graph-7/computation_graph/visualization.py` & `computation-graph-9/computation_graph/visualization.py`

 * *Files identical despite different names*

### Comparing `computation-graph-7/computation_graph.egg-info/PKG-INFO` & `computation-graph-9/computation_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computation-graph
-Version: 7
+Version: 9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.com/hyroai/computation-graph.svg?branch=master)](https://travis-ci.com/hyroai/computation-graph)
         
         A functional composition framework that supports:
```

