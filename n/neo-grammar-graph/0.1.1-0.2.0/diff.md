# Comparing `tmp/neo_grammar_graph-0.1.1.tar.gz` & `tmp/neo_grammar_graph-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo_grammar_graph-0.1.1.tar", last modified: Wed May  3 15:17:29 2023, max compression
+gzip compressed data, was "neo_grammar_graph-0.2.0.tar", last modified: Thu May 11 08:11:11 2023, max compression
```

## Comparing `neo_grammar_graph-0.1.1.tar` & `neo_grammar_graph-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-05-03 15:17:29.281249 neo_grammar_graph-0.1.1/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    35149 2021-03-30 13:41:15.000000 neo_grammar_graph-0.1.1/LICENSE
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44218 2023-05-03 15:17:29.281456 neo_grammar_graph-0.1.1/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2878 2023-05-03 09:20:51.000000 neo_grammar_graph-0.1.1/README.md
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      775 2023-05-03 15:14:42.000000 neo_grammar_graph-0.1.1/pyproject.toml
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1104 2023-05-03 15:17:29.282168 neo_grammar_graph-0.1.1/setup.cfg
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:29:50.000000 neo_grammar_graph-0.1.1/setup.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-05-03 15:17:29.272453 neo_grammar_graph-0.1.1/src/
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-05-03 15:17:29.277675 neo_grammar_graph-0.1.1/src/neo_grammar_graph/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      102 2023-05-03 15:14:46.000000 neo_grammar_graph-0.1.1/src/neo_grammar_graph/__init__.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    73661 2023-05-03 15:14:34.000000 neo_grammar_graph-0.1.1/src/neo_grammar_graph/gg.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2917 2023-04-19 14:21:50.000000 neo_grammar_graph-0.1.1/src/neo_grammar_graph/helpers.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1990 2023-05-03 09:02:43.000000 neo_grammar_graph-0.1.1/src/neo_grammar_graph/nodes.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1065 2023-05-03 08:55:53.000000 neo_grammar_graph-0.1.1/src/neo_grammar_graph/type_defs.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-05-03 15:17:29.279911 neo_grammar_graph-0.1.1/src/neo_grammar_graph.egg-info/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44218 2023-05-03 15:17:29.000000 neo_grammar_graph-0.1.1/src/neo_grammar_graph.egg-info/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      476 2023-05-03 15:17:29.000000 neo_grammar_graph-0.1.1/src/neo_grammar_graph.egg-info/SOURCES.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2023-05-03 15:17:29.000000 neo_grammar_graph-0.1.1/src/neo_grammar_graph.egg-info/dependency_links.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      252 2023-05-03 15:17:29.000000 neo_grammar_graph-0.1.1/src/neo_grammar_graph.egg-info/requires.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       18 2023-05-03 15:17:29.000000 neo_grammar_graph-0.1.1/src/neo_grammar_graph.egg-info/top_level.txt
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-05-03 15:17:29.280996 neo_grammar_graph-0.1.1/tests/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      551 2023-04-25 10:17:21.000000 neo_grammar_graph-0.1.1/tests/test_doctests.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     3324 2023-05-03 15:10:10.000000 neo_grammar_graph-0.1.1/tests/test_gg.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-05-11 08:11:11.376208 neo_grammar_graph-0.2.0/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    35149 2021-03-30 13:41:15.000000 neo_grammar_graph-0.2.0/LICENSE
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44218 2023-05-11 08:11:11.376866 neo_grammar_graph-0.2.0/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2878 2023-05-03 09:20:51.000000 neo_grammar_graph-0.2.0/README.md
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      775 2023-05-11 08:10:18.000000 neo_grammar_graph-0.2.0/pyproject.toml
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1104 2023-05-11 08:11:11.378231 neo_grammar_graph-0.2.0/setup.cfg
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:29:50.000000 neo_grammar_graph-0.2.0/setup.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-05-11 08:11:11.366750 neo_grammar_graph-0.2.0/src/
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-05-11 08:11:11.371793 neo_grammar_graph-0.2.0/src/neo_grammar_graph/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      102 2023-05-11 08:10:10.000000 neo_grammar_graph-0.2.0/src/neo_grammar_graph/__init__.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    75800 2023-05-11 08:06:11.000000 neo_grammar_graph-0.2.0/src/neo_grammar_graph/gg.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2917 2023-04-19 14:21:50.000000 neo_grammar_graph-0.2.0/src/neo_grammar_graph/helpers.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1990 2023-05-03 09:02:43.000000 neo_grammar_graph-0.2.0/src/neo_grammar_graph/nodes.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1065 2023-05-03 08:55:53.000000 neo_grammar_graph-0.2.0/src/neo_grammar_graph/type_defs.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-05-11 08:11:11.374462 neo_grammar_graph-0.2.0/src/neo_grammar_graph.egg-info/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44218 2023-05-11 08:11:11.000000 neo_grammar_graph-0.2.0/src/neo_grammar_graph.egg-info/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      476 2023-05-11 08:11:11.000000 neo_grammar_graph-0.2.0/src/neo_grammar_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2023-05-11 08:11:11.000000 neo_grammar_graph-0.2.0/src/neo_grammar_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      252 2023-05-11 08:11:11.000000 neo_grammar_graph-0.2.0/src/neo_grammar_graph.egg-info/requires.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       18 2023-05-11 08:11:11.000000 neo_grammar_graph-0.2.0/src/neo_grammar_graph.egg-info/top_level.txt
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-05-11 08:11:11.375823 neo_grammar_graph-0.2.0/tests/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      551 2023-04-25 10:17:21.000000 neo_grammar_graph-0.2.0/tests/test_doctests.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     4788 2023-05-11 07:56:35.000000 neo_grammar_graph-0.2.0/tests/test_gg.py
```

### Comparing `neo_grammar_graph-0.1.1/LICENSE` & `neo_grammar_graph-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neo_grammar_graph-0.1.1/PKG-INFO` & `neo_grammar_graph-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo_grammar_graph
-Version: 0.1.1
+Version: 0.2.0
 Summary: Graphs from Context-Free Grammars.
 Home-page: https://github.com/rindPHI/NeoGrammarGraph
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `neo_grammar_graph-0.1.1/README.md` & `neo_grammar_graph-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `neo_grammar_graph-0.1.1/pyproject.toml` & `neo_grammar_graph-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neo_grammar_graph"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Dominic Steinhöfel", email="dominic.steinhoefel@cispa.de" },
 ]
 description = "Graphs from Context-Free Grammars."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `neo_grammar_graph-0.1.1/setup.cfg` & `neo_grammar_graph-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `neo_grammar_graph-0.1.1/src/neo_grammar_graph/gg.py` & `neo_grammar_graph-0.2.0/src/neo_grammar_graph/gg.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with NeoGrammarGraph.  If not, see <http://www.gnu.org/licenses/>.
 import os.path
 from functools import lru_cache
-from typing import Dict, List, Callable, Optional, Tuple, Any, cast
+from typing import Dict, List, Callable, Optional, Tuple, Any, cast, Sequence
 
 from bidict import MutableBidict, bidict
 from graph_tool import Graph, Vertex, Edge, GraphView
 from graph_tool.search import bfs_search, BFSVisitor, StopSearch
 from graph_tool.topology import transitive_closure, all_paths
 from orderedset import OrderedSet
 
@@ -151,15 +151,15 @@
                 self.graph.ep.label[nonterminal_choice_edge] = alternative_nr
 
                 # If `alternative` is the empty expansion (epsilon), we still have to
                 # ensure that an epsilon terminal node is added even though
                 # `split_expansion` would return an empty list. Thus, we keep a custom
                 # singleton list containing an empty string in that case.
                 for elem_nr, expansion_element in enumerate(
-                    split_expansion(alternative) or ['']
+                    split_expansion(alternative) or [""]
                 ):
                     ident = len(
                         self.symbol_to_vertices.setdefault(
                             expansion_element, OrderedSet()
                         )
                     )
 
@@ -877,36 +877,36 @@
         ...     "<digit>": list(string.digits)
         ... }
         >>> graph = NeoGrammarGraph(grammar)
 
         The shortest path between :code:`<stmt>` and :code:`<digit>` in the above
         grammar consists of four nonterminals:
 
-        >>> print(", ".join(map(str, graph.shortest_path("<stmt>", "<digit>"))))
+        >>> print(path_to_str(graph.shortest_path("<stmt>", "<digit>")))
         <stmt> (0), <assgn> (0), <rhs> (0), <digit> (0)
 
         If we relax the default :code:`node_filter`, we are also presented the
         "choice nodes:"
 
-        >>> print(", ".join(map(str,
-        ...     graph.shortest_path("<stmt>", "<digit>", lambda _: True))))
+        >>> print(path_to_str(
+        ...     graph.shortest_path("<stmt>", "<digit>", lambda _: True)))
         <stmt> (0), <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (1), <digit> (0)
 
         For unconnected nonterminals (grammar graphs are directed!), we obtain an empty
         list.
 
         >>> graph.shortest_path("<digit>", "<stmt>")
         []
 
         For nonterminals reachable by themselves, the end node might be a different
         one than the start node (though they share the same nonterminal symbol), since
         the nonterminal is reached via a different context.
 
-        >>> print(", ".join(map(str,
-        ...     graph.shortest_path("<stmt>", "<stmt>", lambda _: True))))
+        >>> print(path_to_str(
+        ...     graph.shortest_path("<stmt>", "<stmt>", lambda _: True)))
         <stmt> (0), <stmt>-choice (0), <stmt> (1)
 
         Reachability is not reflexive: If there is no path of at least one edge between
         a nonterminal and itself, an empty list is returned.
 
         >>> graph.shortest_path("<digit>", "<digit>")
         []
@@ -915,20 +915,20 @@
         returned.
         >>> graph.shortest_path("<single-digit>", "<digit>") is None
         True
 
         Nodes in the result can be arbitrarily filtered; let's take out the source
         nonterminal:
 
-        >>> print(", ".join(map(str, graph.shortest_path(
+        >>> print(path_to_str(graph.shortest_path(
         ...     "<stmt>",
         ...     "<digit>",
         ...     lambda node: (
         ...         not isinstance(node, NonterminalNode) or
-        ...         node.value != "<stmt>")))))
+        ...         node.value != "<stmt>"))))
         <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (1), <digit> (0)
 
         :param source_symbol: The start nonterminal for the computation of a
             shortest path.
         :param target_symbol: The destination nonterminal for the computation of
             a shortest path.
         :param node_filter: A function for filtering out elements of the returned path,
@@ -992,25 +992,25 @@
         ...     "<digit>": list(string.digits)
         ... }
         >>> graph = NeoGrammarGraph(grammar)
 
         The shortest path between :code:`<stmt>` and :code:`<digit>` in the above
         grammar consists of four nonterminals:
 
-        >>> print(", ".join(map(str, graph.shortest_path_between_nodes(
-        ...     NonterminalNode(0, "<stmt>"), NonterminalNode(0, "<digit>")))))
+        >>> print(path_to_str(graph.shortest_path_between_nodes(
+        ...     NonterminalNode(0, "<stmt>"), NonterminalNode(0, "<digit>"))))
         <stmt> (0), <assgn> (0), <rhs> (0), <digit> (0)
 
         If we relax the default :code:`node_filter`, we are also presented the
         "choice nodes:"
 
-        >>> print(", ".join(map(str, graph.shortest_path_between_nodes(
+        >>> print(path_to_str(graph.shortest_path_between_nodes(
         ...     NonterminalNode(0, "<stmt>"),
         ...     NonterminalNode(0, "<digit>"),
-        ...     lambda node: True))))
+        ...     lambda node: True)))
         <stmt> (0), <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (1), <digit> (0)
 
         For unconnected nonterminals (grammar graphs are directed!), we obtain an empty
         list.
 
         >>> graph.shortest_path_between_nodes(
         ...     NonterminalNode(0, "<digit>"), NonterminalNode(0, "<stmt>"))
@@ -1045,20 +1045,20 @@
         ...     NonterminalNode(0, "<single-digit>"),
         ...     NonterminalNode(0, "<digit>")) is None
         True
 
         Nodes in the result can be arbitrarily filtered; let's take out the source
         nonterminal:
 
-        >>> print(", ".join(map(str, graph.shortest_path_between_nodes(
+        >>> print(path_to_str(graph.shortest_path_between_nodes(
         ...     NonterminalNode(0, "<stmt>"),
         ...     NonterminalNode(0, "<digit>"),
         ...     lambda node: (
         ...         not isinstance(node, NonterminalNode) or
-        ...         node.value != "<stmt>")))))
+        ...         node.value != "<stmt>"))))
         <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (1), <digit> (0)
 
         :param source_node: The start node for the computation of a shortest path.
         :param target_node: The destination node for the computation of a shortest path.
         :param node_filter: A function for filtering out elements of the returned path,
             if any. The function must accept two arguments, the first will be an
             integer, the position of the path element, and the second a string, the path
@@ -1130,28 +1130,24 @@
         ...     "<var>": list(string.ascii_lowercase),
         ...     "<digit>": list(string.digits)
         ... }
         >>> graph = NeoGrammarGraph(grammar)
 
         There are three paths from :code:`<stmt>` to :code:`digit`:
 
-        >>> print("\n".join(map(
-        ...     lambda path: ", ".join(map(str, path)),
-        ...     graph.paths_between("<stmt>", "<digit>"))))
+        >>> print(paths_to_str(graph.paths_between("<stmt>", "<digit>")))
         <stmt> (0), <assgn> (0), <rhs> (0), <digit> (0)
         <stmt> (0), <stmt> (1), <assgn> (1), <rhs> (0), <digit> (0)
         <stmt> (0), <assgn> (1), <rhs> (0), <digit> (0)
 
         Per default, we only look up paths from the first node corresponding to a
         :code:`start_node` passed as string. However, this method also accepts
         Node objects for one or both source/target arguments:
 
-        >>> print("\n".join(map(
-        ...     lambda path: ", ".join(map(str, path)),
-        ...     graph.paths_between(NonterminalNode(1, "<stmt>"), "<digit>"))))
+        >>> print(paths_to_str(graph.paths_between(NonterminalNode(1, "<stmt>"), "<digit>")))
         <stmt> (1), <assgn> (0), <rhs> (0), <digit> (0)
         <stmt> (1), <assgn> (1), <rhs> (0), <digit> (0)
 
         Note that although :code:`<stmt> (1)` has the same children as
         :code:`<stmt> (0)`, the results are different (as in the below example),
         since :code:`<stmt> (1), <stmt> (1)` would not be a *path* (it has repetitions
         of one edge).
@@ -1159,17 +1155,15 @@
         There is no path from :code:`<digit>` to itself:
 
         >>> str(graph.paths_between("<digit>", "<digit>"))
         '{}'
 
         Path computation for self-reachable symbols works as expected.
 
-        >>> print("\n".join(map(
-        ...     lambda path: ", ".join(map(str, path)),
-        ...     graph.paths_between("<stmt>", "<stmt>", lambda _: True))))
+        >>> print(paths_to_str(graph.paths_between("<stmt>", "<stmt>", lambda _: True)))
         <stmt> (0), <stmt>-choice (0), <stmt> (1)
 
         If a symbol does not exist, we obtain :code:`None`:
 
         >>> graph.paths_between("<some-digit>", "<digit>") is None
         True
 
@@ -1212,15 +1206,15 @@
         )
 
     @lru_cache(maxsize=None)
     def k_paths(
         self,
         k: int,
         up_to: bool = False,
-        start_node: Optional[str | Node] = None,
+        start_nodes: Optional[Tuple[str | Node, ...]] = None,
         include_terminals=True,
         graph: Optional[Graph] = None,
     ) -> OrderedSet[Tuple[Node, ...]]:
         r"""
         This function computes all paths of length k in the graph, optionally restricted
         to those reachable from the nonterminal :code:`start_nonterminal`. If up_to
         is True, also smaller paths are considered. "Choice nodes" are not considered in
@@ -1243,80 +1237,81 @@
         ...     "<digit>": list(string.digits)
         ... }
         >>> graph = NeoGrammarGraph(grammar)
 
         The 1-paths in the graph correspond to the nonterminal symbols (dictionary
         keys) in the underlying grammar in different contexts.
 
-        >>> print("\n".join(map(
-        ...     lambda path: ", ".join(map(str, path)),
-        ...     graph.k_paths(1, include_terminals=False))))
+        >>> print(paths_to_str(graph.k_paths(1, include_terminals=False)))
         <start> (0)
         <stmt> (0)
         <assgn> (0)
         <stmt> (1)
         <assgn> (1)
         <var> (0)
         <rhs> (0)
         <var> (1)
         <digit> (0)
 
         We can ask for paths starting at a particular nonterminal.
 
-        >>> print("\n".join(map(
-        ...     lambda path: ", ".join(map(str, path)),
-        ...     graph.k_paths(2, start_node="<digit>"))))
+        >>> print(paths_to_str(graph.k_paths(2, start_nodes=("<digit>",))))
         <digit> (0), <digit>-choice (0), '0' (0)
         <digit> (0), <digit>-choice (1), '1' (0)
         <digit> (0), <digit>-choice (2), '2' (0)
         <digit> (0), <digit>-choice (3), '3' (0)
         <digit> (0), <digit>-choice (4), '4' (0)
         <digit> (0), <digit>-choice (5), '5' (0)
         <digit> (0), <digit>-choice (6), '6' (0)
         <digit> (0), <digit>-choice (7), '7' (0)
         <digit> (0), <digit>-choice (8), '8' (0)
         <digit> (0), <digit>-choice (9), '9' (0)
 
         Paths ending in terminal symbols can be excluded on demand.
 
-        >>> print("\n".join(map(
-        ...     lambda path: ", ".join(map(str, path)),
+        >>> print(paths_to_str(
         ...     graph.k_paths(
         ...         3,
-        ...         start_node="<assgn>",
-        ...         include_terminals=False))))
+        ...         start_nodes=("<assgn>",),
+        ...         include_terminals=False)))
+        <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (0), <var> (1)
+        <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (1), <digit> (0)
+        <assgn> (1), <assgn>-choice (0), <rhs> (0), <rhs>-choice (0), <var> (1)
+        <assgn> (1), <assgn>-choice (0), <rhs> (0), <rhs>-choice (1), <digit> (0)
+
+        We can also ask for the paths starting from a particular *node* and not all
+        nodes (including reference nodes) for a nonterminal:
+
+        >>> print(paths_to_str(
+        ...     graph.k_paths(
+        ...         3,
+        ...         start_nodes=(graph.nodes("<assgn>")[0],),
+        ...         include_terminals=False)))
         <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (0), <var> (1)
         <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (1), <digit> (0)
 
         If up_to is set to True, we also obtain paths shorter than the set k.
 
-        >>> print("\n".join(map(
-        ...     lambda path: ", ".join(map(str, path)),
+        >>> print(paths_to_str(
         ...     graph.k_paths(
         ...         3,
-        ...         start_node="<assgn>",
+        ...         start_nodes=(graph.nodes("<assgn>")[0],),
         ...         up_to=True,
-        ...         include_terminals=False))))
+        ...         include_terminals=False)))
         <assgn> (0)
         <assgn> (0), <assgn>-choice (0), <var> (0)
-        <var> (0)
         <assgn> (0), <assgn>-choice (0), <rhs> (0)
-        <rhs> (0)
-        <rhs> (0), <rhs>-choice (0), <var> (1)
         <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (0), <var> (1)
-        <var> (1)
-        <rhs> (0), <rhs>-choice (1), <digit> (0)
         <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (1), <digit> (0)
-        <digit> (0)
 
         For certain configurations, we might obtain an empty set of paths.
 
         >>> print(graph.k_paths(
         ...     4,
-        ...     start_node="<assgn>",
+        ...     start_nodes=("<assgn>",),
         ...     include_terminals=False))
         {}
 
         If the optionally passed graph-tool graph is given, it must have a vertex
         property called "node" pointing to the Node object associated to a given
         vertex.
 
@@ -1339,74 +1334,74 @@
             assert (
                 "node" in graph.vp
             ), "The `node` property is mandatory if you supply a custom Graph object."
 
         # Each path of k terminal/nonterminal nodes includes k-1 choice nodes
         k += k - 1
 
-        path_map: Dict[Vertex, List[Tuple[Vertex, ...]]] = {}
-
-        class PathVisitor(BFSVisitor):
-            def examine_edge(self, e: Edge):
-                path_map.setdefault(e.source(), []).append((e.source(),))
-                path_map.setdefault(e.target(), []).append((e.source(), e.target()))
-
-                prefixes = [
-                    path for path in path_map.get(e.source(), []) if len(path) < k
-                ]
-                if not prefixes:
-                    return
+        if "node" in graph.vp:
 
-                path_map[e.target()].extend(
-                    [prefix + (e.target(),) for prefix in prefixes]
-                )
+            def vertex_to_node(vertex: int | Vertex) -> Node:
+                node = graph.vp.node[vertex]
+                assert isinstance(node, Node)
+                return node
 
-        if start_node is None:
-            start_node = NonterminalNode(0, "<start>")
         else:
-            start_nodes = self.nodes(start_node)
-            assert start_nodes
-            start_node = start_nodes[0]
-
-        if "node" in graph.vp:
 
             def vertex_to_node(vertex: Vertex) -> Node:
-                result = graph.vp.node[vertex]
-                assert isinstance(result, Node)
-                return result
+                return self.vertex_to_node[vertex]
 
-            start_vertex = graph.vertex(0)
-            assert vertex_to_node(start_vertex) == start_node
+        if start_nodes is None:
+            start_vertices = [
+                vertex
+                for vertex in graph.vertices()
+                if isinstance(vertex_to_node(vertex), NonterminalNode)
+            ]
         else:
+            start_vertices = [
+                node for elem in start_nodes for node in self.vertices(elem)
+            ]
 
-            def vertex_to_node(vertex: Vertex) -> Node:
-                return self.vertex_to_node[vertex]
+        result_vertex_paths: OrderedSet[Tuple[Vertex, ...]] = OrderedSet()
 
-            start_vertex = self.vertex_to_node.inverse[start_node]
+        for vertex in start_vertices:
+            result_for_node: Dict[int, OrderedSet[Tuple[Vertex, ...]]] = {
+                1: OrderedSet([(vertex,)])
+            }
 
-        bfs_search(graph, start_vertex, PathVisitor())
+            for depth in range(k - 1):
+                result_for_node[depth + 2] = OrderedSet(
+                    [
+                        path + (child,)
+                        for path in result_for_node[depth + 1]
+                        for child in graph.get_out_neighbors(path[-1])
+                        if include_terminals
+                        or not isinstance(vertex_to_node(child), TerminalNode)
+                    ]
+                )
 
-        # We collect all the paths from `path_map` that do not start or end
-        # in a choice node and have a suitable length. Furthermore, we eliminate
-        # paths ending in terminal symbols if the corresponding flag is set.
-        paths = [
-            path
-            for path_set in path_map.values()
-            for path in path_set
-            if not isinstance(vertex_to_node(path[0]), ChoiceNode)
-            and not isinstance(vertex_to_node(path[-1]), ChoiceNode)
-            and (up_to or len(path) == k)
-            and (
-                include_terminals
-                or not isinstance(vertex_to_node(path[-1]), TerminalNode)
-            )
-        ]
+            if up_to:
+                result_vertex_paths.update(
+                    [
+                        path
+                        for depth, paths in result_for_node.items()
+                        if depth % 2
+                        for path in paths
+                    ]
+                )
+            else:
+                assert k in result_for_node
+                result_vertex_paths.update(result_for_node[k])
 
-        # For the final result, we convert vertex objects to grammar string symbols.
-        return OrderedSet([tuple([vertex_to_node(v) for v in path]) for path in paths])
+        return OrderedSet(
+            [
+                tuple([vertex_to_node(vertex) for vertex in vertex_path])
+                for vertex_path in result_vertex_paths
+            ]
+        )
 
     def parse_tree_to_graph(self, tree: ParseTree) -> Graph:
         r"""
         Converts a ParseTree to a graph-tool Graph object.
 
         Example:
 
@@ -1687,17 +1682,15 @@
         ...         [('<assgn>',
         ...           [('<var>', [('y', [])]),
         ...            (' := ', []),
         ...            ('<rhs>', [('<var>', [('x', [])])])])])])])
 
         This is the set of all 3-paths in this tree.
 
-        >>> print("\n".join(map(
-        ...     lambda path: ", ".join(map(str, path)),
-        ...     graph.k_paths_in_tree(tree, 3, include_terminals=True))))
+        >>> print(paths_to_str(graph.k_paths_in_tree(tree, 3, include_terminals=True)))
         <start> (0), <start>-choice (0), <stmt> (0), <stmt>-choice (0), <assgn> (0)
         <start> (0), <start>-choice (0), <stmt> (0), <stmt>-choice (0), ' ; ' (0)
         <start> (0), <start>-choice (0), <stmt> (0), <stmt>-choice (0), <stmt> (1)
         <stmt> (0), <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <var> (0)
         <stmt> (0), <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), ' := ' (0)
         <stmt> (0), <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <rhs> (0)
         <stmt> (0), <stmt>-choice (0), <stmt> (1), <stmt>-choice (1), <assgn> (1)
@@ -1709,18 +1702,16 @@
         <rhs> (0), <rhs>-choice (1), <digit> (0), <digit>-choice (1), '1' (0)
         <assgn> (1), <assgn>-choice (0), <var> (0), <var>-choice (24), 'y' (0)
         <assgn> (1), <assgn>-choice (0), <rhs> (0), <rhs>-choice (0), <var> (1)
         <rhs> (0), <rhs>-choice (0), <var> (1), <var>-choice (23), 'x' (0)
 
         Optionally, we can exclude the paths ending in terminal symbols:
 
-        >>> print("\n".join(map(
-        ...     lambda path: ", ".join(map(str, path)),
-        ...     graph.k_paths_in_tree(
-        ...         tree, 3, include_terminals=False))))
+        >>> print(paths_to_str(graph.k_paths_in_tree(
+        ...         tree, 3, include_terminals=False)))
         <start> (0), <start>-choice (0), <stmt> (0), <stmt>-choice (0), <assgn> (0)
         <start> (0), <start>-choice (0), <stmt> (0), <stmt>-choice (0), <stmt> (1)
         <stmt> (0), <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <var> (0)
         <stmt> (0), <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <rhs> (0)
         <stmt> (0), <stmt>-choice (0), <stmt> (1), <stmt>-choice (1), <assgn> (1)
         <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (1), <digit> (0)
         <stmt> (1), <stmt>-choice (1), <assgn> (1), <assgn>-choice (0), <var> (0)
@@ -1742,35 +1733,31 @@
         ...           [('<var>', [('y', [])]),
         ...           (' := ', []),
         ...           ('<rhs>', None)])])])])
 
         First, let us inspect the "concrete" paths (without terminal symbols) in this
         cropped tree:
 
-        >>> print("\n".join(map(
-        ...     lambda path: ", ".join(map(str, path)),
-        ...     graph.k_paths_in_tree(
-        ...         tree, 3, include_potential_paths=False, include_terminals=False))))
+        >>> print(paths_to_str(graph.k_paths_in_tree(
+        ...         tree, 3, include_potential_paths=False, include_terminals=False)))
         <start> (0), <start>-choice (0), <stmt> (0), <stmt>-choice (0), <assgn> (0)
         <start> (0), <start>-choice (0), <stmt> (0), <stmt>-choice (0), <stmt> (1)
         <stmt> (0), <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <var> (0)
         <stmt> (0), <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <rhs> (0)
         <stmt> (0), <stmt>-choice (0), <stmt> (1), <stmt>-choice (1), <assgn> (1)
         <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (1), <digit> (0)
         <stmt> (1), <stmt>-choice (1), <assgn> (1), <assgn>-choice (0), <var> (0)
         <stmt> (1), <stmt>-choice (1), <assgn> (1), <assgn>-choice (0), <rhs> (0)
 
         If we additionally ask for the potential paths, the two paths starting from the
         :code:`<assgn> (1)` node and passing the open :code:`<rhs> (0)` node are added
         to the result:
 
-        >>> print("\n".join(map(
-        ...     lambda path: ", ".join(map(str, path)),
-        ...     graph.k_paths_in_tree(
-        ...         tree, 3, include_potential_paths=True, include_terminals=False))))
+        >>> print(paths_to_str(graph.k_paths_in_tree(
+        ...         tree, 3, include_potential_paths=True, include_terminals=False)))
         <start> (0), <start>-choice (0), <stmt> (0), <stmt>-choice (0), <assgn> (0)
         <start> (0), <start>-choice (0), <stmt> (0), <stmt>-choice (0), <stmt> (1)
         <stmt> (0), <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <var> (0)
         <stmt> (0), <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <rhs> (0)
         <stmt> (0), <stmt>-choice (0), <stmt> (1), <stmt>-choice (1), <assgn> (1)
         <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (1), <digit> (0)
         <stmt> (1), <stmt>-choice (1), <assgn> (1), <assgn>-choice (0), <var> (0)
@@ -1800,15 +1787,14 @@
 
         tree_graph = self.parse_tree_to_graph(tree)
 
         tree_k_paths = self.k_paths(
             k,
             graph=tree_graph,
             up_to=False,
-            start_node="<start>",
             include_terminals=include_terminals,
         )
 
         if not include_potential_paths:
             return tree_k_paths
 
         result = OrderedSet(tree_k_paths)
@@ -1828,15 +1814,14 @@
         ]
 
         open_leaf_nodes = [tree_graph.vp.node[v] for v in open_leaf_vertices]
 
         grammar_k_paths = self.k_paths(
             k,
             up_to=False,
-            start_node="<start>",
             include_terminals=include_terminals,
         )
 
         for other_path in grammar_k_paths.difference(set(result)):
             if any(
                 other_path[0] == leaf_node or self.reachable(leaf_node, other_path[0])
                 for leaf_node in open_leaf_nodes
@@ -1925,7 +1910,75 @@
 
 class InvalidTreeException(Exception):
     """
     Signals that a parse tree does not conform to the grammar.
     """
 
     pass
+
+
+def path_to_str(path: Sequence[Node], separator: str = ", ") -> str:
+    """
+    Converts a path (list of nodes) to a :code:`separator`-separated string.
+
+    >>> path_to_str([
+    ...     NonterminalNode(ident=0, value='<stmt>'),
+    ...     ChoiceNode(ident=0, parent_nonterminal='<stmt>'),
+    ...     NonterminalNode(ident=0, value='<assgn>'),
+    ...     ChoiceNode(ident=0, parent_nonterminal='<assgn>'),
+    ...     NonterminalNode(ident=0, value='<rhs>'),
+    ...     ChoiceNode(ident=1, parent_nonterminal='<rhs>'),
+    ...     NonterminalNode(ident=0, value='<digit>')])
+    '<stmt> (0), <stmt>-choice (0), <assgn> (0), <assgn>-choice (0), <rhs> (0), <rhs>-choice (1), <digit> (0)'
+
+    :param path: The path to convert.
+    :param separator: The separator to insert between nodes.
+    :return: A string representation of the path.
+    """
+
+    return separator.join(map(str, path))
+
+
+def paths_to_str(
+    paths: Sequence[Sequence[Node]],
+    path_separator: str = "\n",
+    node_separator: str = ", ",
+) -> str:
+    """
+    Converts a list of paths (a path is a list of nodes) to a string.
+
+    >>> print(paths_to_str([
+    ...     (
+    ...         NonterminalNode(ident=0, value='<start>'),
+    ...         ChoiceNode(ident=0, parent_nonterminal='<start>'),
+    ...         NonterminalNode(ident=0, value='<stmt>'),
+    ...         ChoiceNode(ident=0, parent_nonterminal='<stmt>'),
+    ...         NonterminalNode(ident=0, value='<assgn>'),
+    ...     ),
+    ...     (
+    ...         NonterminalNode(ident=0, value='<start>'),
+    ...         ChoiceNode(ident=0, parent_nonterminal='<start>'),
+    ...         NonterminalNode(ident=0, value='<stmt>'),
+    ...         ChoiceNode(ident=0, parent_nonterminal='<stmt>'),
+    ...         TerminalNode(ident=0, value=' ; '),
+    ...     ),
+    ...     (
+    ...         NonterminalNode(ident=0, value='<start>'),
+    ...         ChoiceNode(ident=0, parent_nonterminal='<start>'),
+    ...         NonterminalNode(ident=0, value='<stmt>'),
+    ...         ChoiceNode(ident=0, parent_nonterminal='<stmt>'),
+    ...         NonterminalNode(ident=1, value='<stmt>'),
+    ...     )
+    ... ]))
+    <start> (0), <start>-choice (0), <stmt> (0), <stmt>-choice (0), <assgn> (0)
+    <start> (0), <start>-choice (0), <stmt> (0), <stmt>-choice (0), ' ; ' (0)
+    <start> (0), <start>-choice (0), <stmt> (0), <stmt>-choice (0), <stmt> (1)
+
+    :param paths: The paths to convert to a string.
+    :param path_separator: The separator to insert between paths.
+    :param node_separator: The separator to insert between nodes.
+    :return: A string representation of the paths.
+    """
+
+    return path_separator.join(
+        map(lambda path: path_to_str(path, separator=node_separator), paths)
+    )
```

### Comparing `neo_grammar_graph-0.1.1/src/neo_grammar_graph/helpers.py` & `neo_grammar_graph-0.2.0/src/neo_grammar_graph/helpers.py`

 * *Files identical despite different names*

### Comparing `neo_grammar_graph-0.1.1/src/neo_grammar_graph/nodes.py` & `neo_grammar_graph-0.2.0/src/neo_grammar_graph/nodes.py`

 * *Files identical despite different names*

### Comparing `neo_grammar_graph-0.1.1/src/neo_grammar_graph/type_defs.py` & `neo_grammar_graph-0.2.0/src/neo_grammar_graph/type_defs.py`

 * *Files identical despite different names*

### Comparing `neo_grammar_graph-0.1.1/src/neo_grammar_graph.egg-info/PKG-INFO` & `neo_grammar_graph-0.2.0/src/neo_grammar_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-grammar-graph
-Version: 0.1.1
+Version: 0.2.0
 Summary: Graphs from Context-Free Grammars.
 Home-page: https://github.com/rindPHI/NeoGrammarGraph
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `neo_grammar_graph-0.1.1/tests/test_doctests.py` & `neo_grammar_graph-0.2.0/tests/test_doctests.py`

 * *Files identical despite different names*

