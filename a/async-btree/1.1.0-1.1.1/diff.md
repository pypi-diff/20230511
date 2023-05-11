# Comparing `tmp/async_btree-1.1.0.tar.gz` & `tmp/async_btree-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_btree-1.1.0.tar", last modified: Fri Nov 20 12:16:24 2020, max compression
+gzip compressed data, was "async_btree-1.1.1.tar", last modified: Fri Nov 20 23:55:52 2020, max compression
```

## Comparing `async_btree-1.1.0.tar` & `async_btree-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1100 2020-11-15 19:49:37.652307 async_btree-1.1.0/LICENSE.md
--rw-r--r--   0        0        0     8240 2020-11-20 12:15:21.912484 async_btree-1.1.0/README.md
--rw-r--r--   0        0        0     1484 2020-11-20 12:15:21.912725 async_btree-1.1.0/async_btree/__init__.py
--rw-r--r--   0        0        0     4169 2020-11-20 12:15:21.913088 async_btree-1.1.0/async_btree/analyze.py
--rw-r--r--   0        0        0     4728 2020-11-20 12:16:01.831414 async_btree-1.1.0/async_btree/control.py
--rw-r--r--   0        0        0     7425 2020-11-20 12:16:01.853771 async_btree-1.1.0/async_btree/decorator.py
--rw-r--r--   0        0        0     3685 2020-11-20 12:16:01.815071 async_btree-1.1.0/async_btree/definition.py
--rw-r--r--   0        0        0     1463 2020-11-20 12:16:01.788091 async_btree-1.1.0/async_btree/leaf.py
--rw-r--r--   0        0        0     1716 2020-11-20 12:16:01.794322 async_btree-1.1.0/async_btree/parallele.py
--rw-r--r--   0        0        0     3473 2020-11-20 12:16:01.820366 async_btree-1.1.0/async_btree/utils.py
--rw-r--r--   0        0        0     4027 2020-11-20 12:15:21.921124 async_btree-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     9098 2020-11-20 12:16:24.858466 async_btree-1.1.0/setup.py
--rw-r--r--   0        0        0     9317 2020-11-20 12:16:24.858948 async_btree-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1100 2020-11-15 19:49:37.652307 async_btree-1.1.1/LICENSE.md
+-rw-r--r--   0        0        0     8240 2020-11-20 12:15:21.912484 async_btree-1.1.1/README.md
+-rw-r--r--   0        0        0     1484 2020-11-20 12:15:21.912725 async_btree-1.1.1/async_btree/__init__.py
+-rw-r--r--   0        0        0     4286 2020-11-20 23:55:34.264766 async_btree-1.1.1/async_btree/analyze.py
+-rw-r--r--   0        0        0     4717 2020-11-20 23:55:34.254649 async_btree-1.1.1/async_btree/control.py
+-rw-r--r--   0        0        0     7425 2020-11-20 23:55:34.279792 async_btree-1.1.1/async_btree/decorator.py
+-rw-r--r--   0        0        0     3685 2020-11-20 23:55:34.245506 async_btree-1.1.1/async_btree/definition.py
+-rw-r--r--   0        0        0     1463 2020-11-20 23:55:34.214580 async_btree-1.1.1/async_btree/leaf.py
+-rw-r--r--   0        0        0     1710 2020-11-20 23:55:10.642138 async_btree-1.1.1/async_btree/parallele.py
+-rw-r--r--   0        0        0     3397 2020-11-20 23:55:34.245587 async_btree-1.1.1/async_btree/utils.py
+-rw-r--r--   0        0        0     4027 2020-11-20 23:55:10.648198 async_btree-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9098 2020-11-20 23:55:52.553634 async_btree-1.1.1/setup.py
+-rw-r--r--   0        0        0     9317 2020-11-20 23:55:52.554114 async_btree-1.1.1/PKG-INFO
```

### Comparing `async_btree-1.1.0/LICENSE.md` & `async_btree-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `async_btree-1.1.0/README.md` & `async_btree-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `async_btree-1.1.0/async_btree/__init__.py` & `async_btree-1.1.1/async_btree/__init__.py`

 * *Files identical despite different names*

### Comparing `async_btree-1.1.0/async_btree/analyze.py` & `async_btree-1.1.1/async_btree/analyze.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Analyze definition."""
 from inspect import getclosurevars
-from typing import Any, List, NamedTuple, Optional, Tuple, no_type_check
+from typing import Any, Callable, List, NamedTuple, Optional, Tuple, no_type_check
 
 from .definition import CallableFunction, get_node_metadata
 
 __all__ = ["analyze", "stringify_analyze", "Node"]
 
 _DEFAULT_EDGES = ['child', 'children', '_child', '_children']
 
@@ -33,14 +33,31 @@
     # https://github.com/python/mypy/issues/731
     edges: List[Tuple[str, List[Any]]]
 
     def __str__(self):
         return stringify_analyze(target=self)
 
 
+def _get_function_name(target: Callable) -> str:
+    return target.__name__.lstrip("_") if hasattr(target, "__name__") else "anonymous"
+
+
+def _get_target_propertie_name(value):
+    if value and callable(value):
+        return get_node_metadata(target=value).name if hasattr(value, "__node_metadata") else _get_function_name(value)
+    return value
+
+
+def _analyze_target_edges(edges):
+    if edges:
+        # it could be a collection of node or a single node
+        return list(map(analyze, edges if hasattr(edges, "__iter__") else [edges]))
+    return None
+
+
 # pylint: disable=protected-access
 @no_type_check  # it's a shortcut for hasattr ...
 def analyze(target: CallableFunction) -> Node:
     """Analyze specified target and return a Node representation.
 
     Args:
         target (CallableFunction): async function to analyze.
@@ -48,49 +65,37 @@
     Returns:
         (Node): a node instance representation of target function
     """
 
     nonlocals = getclosurevars(target).nonlocals
 
     def _get_nonlocals_value_for(name):
-        return nonlocals[name] if name in nonlocals else None
+        return nonlocals.get(name, None)
 
     def _analyze_property(p):
         """Return a tuple (name, value) or (name, function name) as property."""
         value = _get_nonlocals_value_for(name=p)
-        p_name = p.lstrip('_')
-        if value and callable(value):
-            return p_name, get_node_metadata(target=value).name if hasattr(value, "__node_metadata") else value.__name__
-        return p_name, value
+        return p.lstrip('_'), _get_target_propertie_name(value=value)
 
     def _analyze_edges(egde_name):
         """Lookup children node from egde_name local var."""
-        value = None
-        edge = _get_nonlocals_value_for(name=egde_name)
-        if edge:
-            # it could be a collection of node
-            if hasattr(edge, "__iter__"):
-                value = list(map(analyze, edge))
-            else:  # or a single node
-                value = [analyze(edge)]
-        return (egde_name.lstrip('_'), value)
+        edges = _get_nonlocals_value_for(name=egde_name)
+        return (egde_name.lstrip('_'), _analyze_target_edges(edges=edges))
 
     if hasattr(target, "__node_metadata"):
         node = get_node_metadata(target=target)
         return Node(
             name=node.name,
             properties=list(map(_analyze_property, node.properties)) if node.properties else [],
             edges=list(filter(lambda p: p is not None, map(_analyze_edges, node.edges or _DEFAULT_EDGES))),
         )
 
     # simple function
     return Node(
-        name=target.__name__.lstrip("_") if hasattr(target, "__name__") else "anonymous",
-        properties=list(map(_analyze_property, nonlocals.keys())),
-        edges=[],
+        name=_get_function_name(target=target), properties=list(map(_analyze_property, nonlocals.keys())), edges=[]
     )
 
 
 def stringify_analyze(target: Node, indent: int = 0, label: Optional[str] = None) -> str:
     """Stringify node representation of specified target.
 
     Args:
```

### Comparing `async_btree-1.1.0/async_btree/control.py` & `async_btree-1.1.1/async_btree/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from .definition import FAILURE, SUCCESS, AsyncInnerFunction, CallableFunction, node_metadata
 from .utils import to_async
 
 __all__ = ['sequence', 'fallback', 'selector', 'decision', 'repeat_until']
 
 
-def sequence(children: List[CallableFunction], succes_threshold: int = -1) -> AsyncInnerFunction:
+def sequence(children: List[CallableFunction], succes_threshold: Optional[int] = None) -> AsyncInnerFunction:
     """Return a function which execute children in sequence.
 
     succes_threshold parameter generalize traditional sequence/fallback and
     must be in [0, len(children)]. Default value is (-1) means len(children)
 
     if #success = succes_threshold, return a success
 
@@ -27,35 +27,35 @@
 
     Returns:
         (AsyncInnerFunction): an awaitable function.
 
     Raises:
         (AssertionError): if succes_threshold is invalid
     """
-    succes_threshold = succes_threshold if succes_threshold != -1 else len(children)
-    if not (0 <= succes_threshold <= len(children)):
+    _succes_threshold = succes_threshold or len(children)
+    if not (0 <= _succes_threshold <= len(children)):
         raise AssertionError('succes_threshold')
 
-    failure_threshold = len(children) - succes_threshold + 1
+    failure_threshold = len(children) - _succes_threshold + 1
 
     _children = [to_async(child) for child in children]
 
-    @node_metadata(properties=['succes_threshold'])
+    @node_metadata(properties=['_succes_threshold'])
     async def _sequence():
         success = 0
         failure = 0
         results = []
 
         for child in _children:
             last_result = await child()
             results.append(last_result)
 
             if bool(last_result):
                 success += 1
-                if success == succes_threshold:
+                if success == _succes_threshold:
                     # last evaluation is a success
                     return results
             else:
                 failure += 1
                 if failure == failure_threshold:
                     # last evaluation is a failure
                     return last_result
```

### Comparing `async_btree-1.1.0/async_btree/decorator.py` & `async_btree-1.1.1/async_btree/decorator.py`

 * *Files identical despite different names*

### Comparing `async_btree-1.1.0/async_btree/definition.py` & `async_btree-1.1.1/async_btree/definition.py`

 * *Files identical despite different names*

### Comparing `async_btree-1.1.0/async_btree/leaf.py` & `async_btree-1.1.1/async_btree/leaf.py`

 * *Files identical despite different names*

### Comparing `async_btree-1.1.0/async_btree/parallele.py` & `async_btree-1.1.1/async_btree/parallele.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Curiosity module define special construct with curio framework."""
 
-from typing import List
+from typing import List, Optional
 
-from .definition import FAILURE, SUCCESS, AsyncInnerFunction, CallableFunction, node_metadata
-from .utils import amap, to_async
+from .definition import AsyncInnerFunction, CallableFunction, node_metadata
+from .utils import to_async
 
 __all__ = ['parallele']
 
 
 try:
-    from curio import gather, spawn
+    from curio import TaskGroup
 
-    def parallele(children: List[CallableFunction], succes_threshold: int = -1) -> AsyncInnerFunction:
+    def parallele(children: List[CallableFunction], succes_threshold: Optional[int] = None) -> AsyncInnerFunction:
         """Return an awaitable function which run children in parallele.
 
         `succes_threshold` parameter generalize traditional sequence/fallback,
         and must be in [0, len(children)], default value is len(children)
 
         if #success = succes_threshold, return a success
 
@@ -25,28 +25,30 @@
             children (List[CallableFunction]): list of Awaitable
             succes_threshold (int): succes threshold value, default len(children)
 
         Returns:
             (AsyncInnerFunction): an awaitable function.
 
         """
-        succes_threshold = succes_threshold if succes_threshold != -1 else len(children)
-        if not (0 <= succes_threshold <= len(children)):
+        _succes_threshold = succes_threshold or len(children)
+        if not (0 <= _succes_threshold <= len(children)):
             raise AssertionError('succes_threshold')
 
         _children = [to_async(child) for child in children]
 
-        @node_metadata(properties=['succes_threshold'])
+        @node_metadata(properties=['_succes_threshold'])
         async def _parallele():
 
-            results = await gather([task async for task in amap(spawn, _children)])
+            async with TaskGroup(wait=all) as g:
+                for child in _children:
+                    await g.spawn(child)
 
-            success = len(list(filter(bool, results)))
+            success = len(list(filter(bool, g.results)))
 
-            return SUCCESS if success >= succes_threshold else FAILURE
+            return success >= _succes_threshold
 
         return _parallele
 
 
 except Exception:  # pragma: no cover
     # default to a simple sequence
     from .control import sequence as parallele
```

### Comparing `async_btree-1.1.0/async_btree/utils.py` & `async_btree-1.1.1/async_btree/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Returns:
         AsyncGenerator[T]: an async iterator of corofunc(item)
 
     Example:
         ```[i async for i in amap(inc, afilter(even, [0, 1, 2, 3, 4]))]```
 
     """
-    if isinstance(iterable, AsyncIterable):  # if hasattr(iterable, '__aiter__'):
+    if isinstance(iterable, AsyncIterable):
         async for item in iterable:
             yield await corofunc(item)
     else:
         for item in iterable:
             yield await corofunc(item)
 
 
@@ -53,15 +53,15 @@
     Returns:
         (AsyncGenerator[T]): an async iterator of item which satisfy corofunc(item) == True
 
     Example:
         ```[i async for i in amap(inc, afilter(even, [0, 1, 2, 3, 4]))]```
 
     """
-    if isinstance(iterable, AsyncIterable):  # if hasattr(iterable, '__aiter__'):
+    if isinstance(iterable, AsyncIterable):
         async for item in iterable:
             if await corofunc(item):
                 yield item
     else:
         for item in iterable:
             if await corofunc(item):
                 yield item
```

### Comparing `async_btree-1.1.0/pyproject.toml` & `async_btree-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "async_btree"
-version = "1.1.0"
+version = "1.1.1"
 description = "Async behavior tree"
 license = "MIT"
 authors = ["Jerome Guibert <jguibert@gmail.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/async_btree"
 documentation = "https://geronimo-iia.github.io/async-btree/"
 repository = "https://github.com/geronimo-iia/async-btree"
```

### Comparing `async_btree-1.1.0/setup.py` & `async_btree-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 extras_require = \
 {'curio': ['curio>=1,<2']}
 
 setup_kwargs = {
     'name': 'async-btree',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'Async behavior tree',
     'long_description': '# Async Behaviour Tree for Python\n\n\n[![Unix Build Status](https://img.shields.io/travis/geronimo-iia/async-btree/master.svg?label=unix)](https://travis-ci.com/geronimo-iia/async-btree)\n[![Coverage Status](https://img.shields.io/coveralls/geronimo-iia/async-btree/master.svg)](https://coveralls.io/r/geronimo-iia/async-btree)\n[![Codacy Badge](https://api.codacy.com/project/badge/Grade/fe669a02b4aa46b5b1faf619ba2bf382)](https://www.codacy.com/app/geronimo-iia/async-btree?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=geronimo-iia/async-btree&amp;utm_campaign=Badge_Grade)\n[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/geronimo-iia/async-btree.svg)](https://scrutinizer-ci.com/g/geronimo-iia/async-btree/?branch=master)\n[![PyPI Version](https://img.shields.io/pypi/v/async-btree.svg)](https://pypi.org/project/async-btree)\n[![PyPI License](https://img.shields.io/pypi/l/async-btree.svg)](https://pypi.org/project/async-btree)\n\nVersions following [Semantic Versioning](https://semver.org/)\n\nSee [documentation](https://geronimo-iia.github.io/async-btree).\n\n\n## Overview\n\n\n### What\'s a behavior tree ?\n\n> Unlike a Finite State Machine, a Behaviour Tree is a tree of hierarchical nodes that controls the flow of decision and the execution of "tasks" or, as we will call them further, "Actions".\n> -- <cite>[behaviortree](https://www.behaviortree.dev/bt_basics/)</cite>\n\nIf your new (or not) about behavior tree, you could spend some time on this few links:\n\n- [Behavior trees for AI: How they work](https://www.gamasutra.com/blogs/ChrisSimpson/20140717/221339/Behavior_trees_for_AI_How_they_work.php) by Chris Simpson\n- [Introduction to BTs](https://www.behaviortree.dev/bt_basics/)\n\nFew implementation libraries:\n\n- [task_behavior_engine](https://github.com/ToyotaResearchInstitute/task_behavior_engine) A behavior tree based task engine written in Python\n- [pi_trees](https://github.com/pirobot/pi_trees/) a Python/ROS library for implementing Behavior Trees\n- [pr_behavior_tree](https://github.com/personalrobotics/pr_behavior_tree) A simple python behavior tree library based on coroutines\n- [btsk](https://github.com/aigamedev/btsk) Behavior Tree Starter Kit\n- [behave](https://github.com/fuchen/behave) A behavior tree implementation in Python\n\n\n### Why another library so ?\n\n__SIMPLICITY__\n\nWhen you study behavior tree implementation, reactive node, dynamic change, runtime execution, etc ...\nAt a moment you\'re build more or less something that mimic an evaluator \'eval/apply\' or a compilator, with a complex hierachical set of class.\n\nAll complexity came with internal state management, using tree of blackboard to avoid global variable, multithreading issue, maybe few callback etc ...\n\nThis break the simplicity and beauty of your initial design.\n\nWhat I find usefull with behavior tree:\n\n- clarity of expression\n- node tree representation\n- possibility to reuse behavior\n- add external measure to dynamicaly change a behavior, a first step on observable pattern...\n\nAs I\'ve used OOP for years (very long time), I will try to avoid class tree and prefer using the power of functionnal programming to obtain what I want: add metadata on a sematic construction, deal with closure, use function in parameters or in return value...\n\nAnd a last reason, more personal, it that i would explore python expressivity.\n\n__SO HOW ?__\n\nIn this module, I purpose you to use the concept of coroutines, and their mecanisms to manage the execution flow.\nBy this way:\n\n- we reuse simple language idiom to manage state, parameter, etc\n- no design constraint on action implementation\n- most of language build block could be reused\n\nYou could build expression like this:\n\n```python\n\nasync def a_func():\n    """A great function"""\n    return "a"\n\nasync def b_decorator(child_value, other=""):\n    """A great decorator..."""\n    return f"b{child_value}{other}"\n\nassert run(decorate(a_func, b_decorator)) == "ba"\n\n```\nThis expression apply ```b_decorator``` on function ```a_func```. \nNote that ```decorate(a_func, b_decorator)``` is not an async function, only action, or condition are async function.\n\n\nFew guidelines of this implementation:\n\n- In order to mimic all NodeStatus (success, failure, running), I replace this by truthy/falsy meaning of evaluation value.\n  A special dedicated exception decorate standard exception in order to give them a Falsy meaning (`ControlFlowException`).\n  By default, exception are raised like happen usually until you catch them.\n- Blackboard pattern, act as a manager of context variable for behavior tree.\n  With python 3, please... simply use [contextvars](https://docs.python.org/3/library/contextvars.html) !\n- In order to be able to build a sematic tree, I\'ve introduce a metadata tuple added on function implementation.\n\nThe rest is just implementation details..\n\n\n\nA little note:\n\n> You should not use this until you\'re ready to think about what you\'re doing :)\n\n\n### Note about \'async\' framework\n\nAs we use async function as underlaying mechanism to manage the execution flow, the standard library asyncio is pretty fine.\nBut, (always a but somewhere isn\'t it...), you should read this [amazing blog post}(https://vorpus.org/blog/some-thoughts-on-asynchronous-api-design-in-a-post-asyncawait-world/) by Nathaniel J. Smith.\nAnd next study [curio](https://github.com/dabeaz/curio) framework in deep.\n\nAs curio say:\n> Don\'t Use Curio if You\'re Allergic to Curio\n\nPersonaly, after few time of testing and reading curio code, I\'m pretty addict.\n\n## Installation\n\nInstall this library directly into an activated virtual environment:\n\n```text\n$ pip install async-btree\n```\n\nor add it to your [Poetry](https://poetry.eustace.io/) project:\n\n```text\n$ poetry add async-btree\n```\n\n## Usage\n\nAfter installation, the package can imported:\n\n```text\n$ python\n>>> import async_btree\n>>> async_btree.__version__\n```\n\nSee [API Reference documentation](https://geronimo-iia.github.io/async-btree).\n\n\nWith this framework, you didn\'t find any configuration file, no Xml, no json, no yaml.\n\nThe main reason (oriented and personal point of view) is that you did not need to introduce an extra level of abtraction \nto declare a composition of functions. I think it\'s true for most of main use case (except using an editor to wrote behaviour tree for example).\n\nSo "If you wrote your function with python, wrote composition in python"... \n_(remember that you did not need XML to do SQL, just write good sql...)_\n\n\nSo, the goal is to:\n - define your business function wich implements actions or conditions, with all test case that you wish/need\n - compose them using those provided by this framework like ```sequence```, ```selector```, ...\n - use them as it is or create a well define python module to reuse them\n\n\nWanna style have an abtract tree of our behaviour tree ?\n\nFunctions from async-btree build an abstract tree for you. \nIf you lookup in code, you should see an annotation "node_metadata" on internal implementation. \nThis decorator add basic information like function name, parameters, and children relation ship.\n\nThis abstract tree can be retreived and stringified with ```analyze``` and ```stringify_analyze```.\nHere the profile:\n\n```python\n  def analyze(target: CallableFunction) -> Node: # here we have our "abtract tree code"\n    ...\n```\n\nFor example:\n\n```python\n\n# your behaviour tree, or a sub tree:\nmy_func = alias(child=repeat_until(child=action(hello), condition=success_until_zero), name="btree_1")\n\n# retrieve meta information and build a Node tree\nabstract_tree_tree_1 = analyze(my_func) \n\n# output the tree:\nprint(stringify_analyze(abstract_tree_tree_1))\n```\n\nThis should print:\n\n```text\n --> btree_1:\n     --(child)--> repeat_until:\n         --(condition)--> success_until_zero:\n         --(child)--> action:\n                      target: hello\n```\n\n\nNote about action and condition method:\n\n - you could use sync or async function\n - you could specify a return value with SUCCESS or FAILURE\n - function with no return value will be evaluated as FAILURE until you decorate them with a `always_success`or `always_failure`\n\nSee this [example/tutorial_1.py](https://raw.githubusercontent.com/geronimo-iia/async-btree/master/examples/tutorial_1.py) for more information.',
     'author': 'Jerome Guibert',
     'author_email': 'jguibert@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://pypi.org/project/async_btree',
```

### Comparing `async_btree-1.1.0/PKG-INFO` & `async_btree-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-btree
-Version: 1.1.0
+Version: 1.1.1
 Summary: Async behavior tree
 Home-page: https://pypi.org/project/async_btree
 License: MIT
 Keywords: behavior-tree,asyncio
 Author: Jerome Guibert
 Author-email: jguibert@gmail.com
 Requires-Python: >=3.7,<4.0
```

