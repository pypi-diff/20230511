# Comparing `tmp/transformlib-0.2.0.tar.gz` & `tmp/transformlib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformlib-0.2.0.tar", last modified: Tue Apr 25 15:33:09 2023, max compression
+gzip compressed data, was "transformlib-0.2.3.tar", last modified: Thu May 11 16:04:58 2023, max compression
```

## Comparing `transformlib-0.2.0.tar` & `transformlib-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:33:09.363041 transformlib-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-25 15:33:09.363041 transformlib-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-25 15:32:54.000000 transformlib-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 15:33:09.363041 transformlib-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-25 15:32:54.000000 transformlib-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:33:09.359041 transformlib-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:33:09.363041 transformlib-0.2.0/src/transformlib/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:33:09.363041 transformlib-0.2.0/src/transformlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-25 15:33:09.000000 transformlib-0.2.0/src/transformlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-25 15:33:09.000000 transformlib-0.2.0/src/transformlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:33:09.000000 transformlib-0.2.0/src/transformlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 15:33:09.000000 transformlib-0.2.0/src/transformlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-25 15:33:09.000000 transformlib-0.2.0/src/transformlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 15:33:09.000000 transformlib-0.2.0/src/transformlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:33:09.363041 transformlib-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-25 15:32:54.000000 transformlib-0.2.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-25 15:32:54.000000 transformlib-0.2.0/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-25 15:32:54.000000 transformlib-0.2.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-25 15:32:54.000000 transformlib-0.2.0/tests/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:04:58.683405 transformlib-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-11 16:04:58.683405 transformlib-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-11 16:04:43.000000 transformlib-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:04:58.683405 transformlib-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-11 16:04:43.000000 transformlib-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:04:58.679404 transformlib-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:04:58.679404 transformlib-0.2.3/src/transformlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-11 16:04:43.000000 transformlib-0.2.3/src/transformlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-11 16:04:43.000000 transformlib-0.2.3/src/transformlib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-11 16:04:43.000000 transformlib-0.2.3/src/transformlib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-11 16:04:43.000000 transformlib-0.2.3/src/transformlib/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-05-11 16:04:43.000000 transformlib-0.2.3/src/transformlib/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-11 16:04:43.000000 transformlib-0.2.3/src/transformlib/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:04:58.683405 transformlib-0.2.3/src/transformlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-11 16:04:58.000000 transformlib-0.2.3/src/transformlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-11 16:04:58.000000 transformlib-0.2.3/src/transformlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:04:58.000000 transformlib-0.2.3/src/transformlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 16:04:58.000000 transformlib-0.2.3/src/transformlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-11 16:04:58.000000 transformlib-0.2.3/src/transformlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 16:04:58.000000 transformlib-0.2.3/src/transformlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:04:58.683405 transformlib-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-11 16:04:43.000000 transformlib-0.2.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-11 16:04:43.000000 transformlib-0.2.3/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-11 16:04:43.000000 transformlib-0.2.3/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-11 16:04:43.000000 transformlib-0.2.3/tests/test_transform.py
```

### Comparing `transformlib-0.2.0/PKG-INFO` & `transformlib-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformlib
-Version: 0.2.0
+Version: 0.2.3
 Summary: Enables the user to organize transformations of data as a regular Python package.
 Home-page: https://github.com/laegsgaardTroels/transformlib
 Author: Troels Lægsgaard
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `transformlib-0.2.0/README.md` & `transformlib-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `transformlib-0.2.0/src/transformlib/__main__.py` & `transformlib-0.2.3/src/transformlib/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,48 @@
 import argparse
+from typing import List
 import logging
 import sys
 from pathlib import Path
 
 from transformlib import Pipeline
 
+logger = logging.getLogger(__name__)
 
-def main() -> None:
-    """A Command Line Inferface (CLI) for running transforms."""
+
+def main(path: List[Path], verbose: bool) -> None:
+    """A Command Line Inferface (CLI) for running :py:class:`transformlib.Transform`.
+
+    Example usage:
+
+    .. highlight:: bash
+    .. code-block:: bash
+
+        transform path/to/transforms/*.py
+        transform -v path/to/transforms/*.py
+
+    The transform command is install from setup.py when installing the package.
+
+    Args:
+        path: (List[Path]): One or more Paths to Transforms one wish to run in a Pipeline.
+        verbose (bool): Should the Transform be run with logging set to INFO.
+    """
+    if verbose:
+        logging.basicConfig(level=logging.INFO)
+    pipeline = Pipeline(transforms=[])
+    for path in map(Path, path):
+        if path.exists():
+            logger.info(f"Adding transforms from {path}")
+            pipeline.add_transforms_from_path(path)
+        else:
+            raise FileNotFoundError(f"No file found at {path}")
+    pipeline.run()
+
+
+if __name__ == '__main__':
     parser = argparse.ArgumentParser(
         description='Run transforms found on paths.'
     )
     parser.add_argument(
         'path',
         type=Path,
         nargs='+',
@@ -20,18 +51,8 @@
     parser.add_argument(
         '-v',
         '--verbose',
         action=argparse.BooleanOptionalAction,
         help="Should the Transform be run with logging set to INFO.",
     )
     args = parser.parse_args()
-    if args.verbose:
-        logging.basicConfig(level=logging.INFO)
-    pipeline = Pipeline(transforms=[])
-    for path in args.path:
-        print(path)
-        pipeline.add_transforms_from_path(path)
-    pipeline.run()
-
-
-if __name__ == '__main__':
-    sys.exit(main())
+    sys.exit(main(path=args.path, verbose=args.verbose))
```

### Comparing `transformlib-0.2.0/src/transformlib/pipeline.py` & `transformlib-0.2.3/src/transformlib/pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from transformlib import Transform
-
-from transformlib.exceptions import TransformlibCycleException
-from transformlib.exceptions import TransformlibDuplicateTransformException
+from transformlib import Node, Output, Input
 
 from typing import Dict
+from typing import Tuple
 from typing import List
 from typing import Optional
 
 from collections import deque
 from pathlib import Path
 import importlib
 import pkgutil
@@ -20,63 +19,95 @@
 
 
 # A graph is a dictionary of transforms (keys) to a list of transformations (value) which have
 # outputs that are inputs to given transform (key).
 Graph = Dict[Transform, List[Transform]]
 
 
+class TransformlibCycleException(Exception):
+    """Raised when there is a cycle in the Pipeline."""
+
+
+class TransformlibDuplicateTransformException(Exception):
+    """Raised when there is duplicate Transform in the Pipeline."""
+
+
+class TransformlibDuplicateInputException(Exception):
+    """Raised when there is duplicate Input in the Pipeline."""
+
+
+class TransformlibDuplicateOutputException(Exception):
+    """Raised when there is duplicate Output in the Pipeline."""
+
+
 class Pipeline:
-    """A `Pipeline` is a topologically ordered list of transforms.
+    """A Pipeline is a topologically ordered list of :py:class:`transformlib.Transform` objects.
 
-    A `Pipeline` can be run from the command line:
+    A :py:class:`transformlib.Pipeline` can be run from the command line:
 
     .. highlight:: bash
     .. code-block:: bash
 
         transform path/to/transforms/*.py
         transform -v path/to/transforms/*.py
 
-    This will topologically sort and run all Transform objects found in the py files and save/load
-    the data from the `config.ROOT_DIR`.
+    This will topologically sort and run all :py:class:`transformlib.Transform` objects found in
+    the py files.
     """
 
     def __init__(self, transforms: Optional[List[Transform]] = None):
         if transforms is None:
             self.transforms = []
         else:
             self.transforms = transforms
 
     @property
-    def tasks(self):
+    def outputs(self) -> Tuple[Output]:
+        """A tuple with all the Output nodes of the Pipeline."""
+        return tuple(node for transform in self.transforms for node in transform.outputs)
+
+    @property
+    def inputs(self) -> Tuple[Input]:
+        """A tuple with all the Input nodes of the Pipeline."""
+        return tuple(node for transform in self.transforms for node in transform.inputs)
+
+    @property
+    def nodes(self) -> Tuple[Node]:
+        """A tuple with all the Node objects of the Pipeline."""
+        return tuple(node for transform in self.transforms for node in transform.nodes)
+
+    @property
+    def tasks(self) -> List[Transform]:
         """A topologically ordered list of transforms."""
+        if len(set(self.inputs)) != len(self.inputs):
+            raise TransformlibDuplicateInputException(f"Duplicate inputs {self.transforms}")
+        if len(set(self.outputs)) != len(self.outputs):
+            raise TransformlibDuplicateOutputException(f"Duplicate inputs {self.transforms}")
         if len(set(self.transforms)) != len(self.transforms):
             raise TransformlibDuplicateTransformException(f"Duplicate {self.transforms}")
         return _get_tasks(self.transforms)  # Topologically sort the transforms.
 
-    def __repr__(self):
-        return f"Pipeline({', '.join(map(repr, self.tasks))})"
-
     def run(self) -> None:
-        """Used to run all the transforms in the pipeline."""
+        """Used to run all the :py:class:`transformlib.Transform` objects in the pipeline."""
         logger.info(f'Beginning running of {self}.')
         start = time.perf_counter()
         for transform in self.tasks:
             transform.run()
         logger.info(f'Completed running of {self} took {time.perf_counter() - start}.')
 
     @classmethod
     def discover_transforms(cls, *plugins):
         """Find and import all transforms in plugins.
 
         This function will automatically disover transforms from plugins
         using namespace packages e.g. fixed namespace(s), as defined by
         the input plugins args to the function, where plugins are saved.
 
-        Assuming you have a module called `transforms`. You can then find and
-        run all the Transform objects in this module:
+        Assuming one has a module called transforms. Then one can then find and
+        run all the :py:class:`transformlib.Transform` objects in this module:
 
         >>> import transforms
         >>> from transformlib.pipeline import Pipeline
         >>> pipeline = Pipeline.discover_transforms(transforms)
         >>> pipeline.run()
 
         Args:
@@ -88,49 +119,62 @@
         References:
             [1] https://packaging.python.org/guides/creating-and-discovering-plugins/
         """
         transforms = []
         for plugin in plugins:
 
             if isinstance(plugin, Transform):
-                logger.info(f"Discovered {plugin} as plugin input.")
+                logger.info(f"Discovered Transform: {new_attr} as plugin input.")
                 transforms.append(plugin)
                 continue
 
             for _, name, ispkg in pkgutil.walk_packages(
                 path=plugin.__path__,
                 prefix=plugin.__name__ + ".",
             ):
                 plugin_module = importlib.import_module(name)
                 for attrname in dir(plugin_module):
                     new_attr = getattr(plugin_module, attrname)
                     if isinstance(new_attr, Transform):
-                        logger.info(f"Discovered {new_attr} in {name}.")
+                        logger.info(f"Discovered Transform: {new_attr} in {name}.")
                         transforms.append(new_attr)
         return cls(transforms)
 
     def add_transforms_from_path(self, plugin_path: Path) -> None:
-        """Find and import all transform from a file.
+        """Find and import all :py:class:`transformlib.Transform` objects from a file.
+
+        When doing this the plugin parent path is added to PATH and removed
+        after the plugin has been searched for :py:class:`transformlib.Transform` objects.
+
+        Assuming one has a module called transforms. Then one can then find and
+        run all the :py:class:`transformlib.Transform` objects in this module:
+
+        >>> from transformlib.pipeline import Pipeline
+        >>> pipeline = Pipeline.add_transforms_from_path('path/to/transform.py')
+        >>> pipeline.run()
 
         Args:
-            plugin_path (Path): A path to a py file with Transform to
+            plugin_path (Path): A path to a py file with :py:class:`transformlib.Transform` to
                 be added to the Pipeline.
         """
         try:
             sys.path.insert(0, str(plugin_path.parent))
             name = plugin_path.stem
             plugin_module = importlib.import_module(name)
             for attrname in dir(plugin_module):
                 new_attr = getattr(plugin_module, attrname)
                 if isinstance(new_attr, Transform):
-                    logger.info(f"Discovered {new_attr} in {name}.")
+                    logger.info(f"Discovered Transform: {new_attr} in {name}.")
                     self.transforms.append(new_attr)
         finally:
             sys.path.pop(0)
 
+    def __repr__(self) -> str:
+        return f"Pipeline({', '.join(map(repr, self.tasks))})"
+
 
 def _get_tasks(transforms: List[Transform]) -> List[Transform]:
     """Get the tasks in order of execution.
 
     Args:
         transforms (List[Transform]): A list of transforms to be topologically ordered.
 
@@ -143,31 +187,29 @@
     return tasks
 
 
 def _create_graph(transforms: List[Transform]) -> Graph:
     """Create a graph out of a list of transforms.
 
     The graph is encoded as a dict of {from: List[to]}, where from and to are
-    transforms.
+    Transform objects.
 
     Args:
-        transforms (List[Transform]): A list of transforms.
+        transforms (List[Transform]): A list of Transform objects.
 
     Returns:
-        Graph: The list of transforms encoded as a graph. A graph is a dictionary of
-            transforms (keys) to a list of transformations (value) which have outputs
+        Graph: The list of Transform objects encoded as a graph. A graph is a dictionary of
+            transforms (key) to a list of transformations (value) which have outputs
             that are inputs to given transform (key).
     """
     return {
         from_:
         [
             to for to in transforms
-            if any(
-                output in to.inputs for output in from_.outputs
-            )
+            if any(output in to.inputs for output in from_.outputs)
         ]
         for from_ in transforms
     }
 
 
 def _tsort(graph: Graph) -> List[Transform]:
     """Used to sort a directed acyclic graph of tasks in order of execution.
```

### Comparing `transformlib-0.2.0/src/transformlib.egg-info/PKG-INFO` & `transformlib-0.2.3/src/transformlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformlib
-Version: 0.2.0
+Version: 0.2.3
 Summary: Enables the user to organize transformations of data as a regular Python package.
 Home-page: https://github.com/laegsgaardTroels/transformlib
 Author: Troels Lægsgaard
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `transformlib-0.2.0/src/transformlib.egg-info/SOURCES.txt` & `transformlib-0.2.3/src/transformlib.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 README.md
 setup.py
 src/transformlib/__init__.py
 src/transformlib/__main__.py
 src/transformlib/config.py
-src/transformlib/exceptions.py
 src/transformlib/node.py
 src/transformlib/pipeline.py
 src/transformlib/transform.py
 src/transformlib.egg-info/PKG-INFO
 src/transformlib.egg-info/SOURCES.txt
 src/transformlib.egg-info/dependency_links.txt
 src/transformlib.egg-info/entry_points.txt
```

### Comparing `transformlib-0.2.0/tests/test_pipeline.py` & `transformlib-0.2.3/tests/test_pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,122 @@
 import pytest
 
-from tests.utils import ReusedPySparkTestCase
 from transformlib import (
     Transform,
-    Pipeline
+    Pipeline,
+    Input,
+    Output
 )
-from transformlib.exceptions import (
+from transformlib.pipeline import (
     TransformlibDuplicateTransformException,
-    TransformlibCycleException
+    TransformlibCycleException,
+    TransformlibDuplicateInputException,
+    TransformlibDuplicateOutputException,
+    _tsort
 )
-from transformlib.pipeline import _tsort
 
 
-def test_run_tasks_duplicate_testing():
+def test_run_duplicate_transforms():
     """Should raise exception if duplicate Transform."""
     transform = Transform(
         output_kwargs={},
         func=lambda: None,
         input_kwargs={},
     )
     with pytest.raises(TransformlibDuplicateTransformException):
         pipeline = Pipeline([transform, transform])
         pipeline.run()
 
 
-def test_run_tasks_exception_testing():
+def test_run_transform_exception_handling():
     """Should raise an exception if one is raised in a Transform."""
     class TransformlibTestRunTasksException(Exception):
         """Raised in this test case."""
 
     def raise_transform_exception():
         raise TransformlibTestRunTasksException('Transform test.')
 
     transform = Transform(
         output_kwargs={},
         func=raise_transform_exception,
         input_kwargs={},
     )
-
+    pipeline = Pipeline([transform])
     with pytest.raises(TransformlibTestRunTasksException):
-        pipeline = Pipeline([transform])
         pipeline.run()
 
 
-class TestSquares(ReusedPySparkTestCase):
-    """Used to test that transformlib on the squares transforms."""
+def test_run_cycle_exception():
+    """Should raise an exception if a cycle in the DAG."""
+
+    def func1(foo_input, bar_input):
+        return None
+
+    def func2(bar_input, foo_input):
+        return None
+
+    transform1 = Transform(
+        output_kwargs={'foo_input': Output('foo')},
+        func=func1,
+        input_kwargs={'bar_input': Input('bar')},
+    )
+    transform2 = Transform(
+        output_kwargs={'bar_output': Output('bar')},
+        func=func2,
+        input_kwargs={'foo_input': Input('foo')},
+    )
+    pipeline = Pipeline([transform1, transform2])
+    with pytest.raises(TransformlibCycleException):
+        pipeline.run()
+
+
+def test_run_duplicate_output_exception():
+    transform1 = Transform(
+        output_kwargs={'foo_output': Output('foo')},
+        func=lambda foo_output: None,
+        input_kwargs={},
+    )
+    transform2 = Transform(
+        output_kwargs={'foo_output': Output('foo')},
+        func=lambda foo_output: None,
+        input_kwargs={},
+    )
+    pipeline = Pipeline([transform1, transform2])
+    with pytest.raises(TransformlibDuplicateOutputException):
+        pipeline.run()
+
 
-    def test_squares_discover_transforms(self):
-        """"Test that the pipeline runs."""
-        from tests.transforms import squares
-        pipeline = Pipeline.discover_transforms(squares)
+def test_run_duplicate_input_exception():
+    transform1 = Transform(
+        output_kwargs={},
+        func=lambda foo_output: None,
+        input_kwargs={'foo_input': Output('foo')},
+    )
+    transform2 = Transform(
+        output_kwargs={},
+        func=lambda foo_output: None,
+        input_kwargs={'foo_input': Input('foo')},
+    )
+    pipeline = Pipeline([transform1, transform2])
+    with pytest.raises(TransformlibDuplicateInputException):
         pipeline.run()
 
-    def test_squares_with_cycle_discover_transforms(self):
-        """"Test that the pipeline runs and raises an Exception."""
-        from tests.transforms import squares_with_cycle
-        pipeline = Pipeline.discover_transforms(squares_with_cycle)
-        with pytest.raises(TransformlibCycleException):
-            pipeline.run()
+
+def test_discover_transforms(tmp_path, monkeypatch):
+    """"Test that the pipeline runs."""
+    monkeypatch.setenv('TRANSFORMLIB_DATA_DIR', str(tmp_path))
+    (tmp_path / 'mapping.txt').write_text("""1,2
+3,4
+5,6
+7,8
+9,10""")
+    from tests import transforms
+    pipeline = Pipeline.discover_transforms(transforms)
+    pipeline.run()
+    assert (tmp_path / 'mapping.json').exists()
 
 
 def test_tsort():
     """Used to test the topological sort."""
     graph_tasks = {
         "wash the dishes": ["have lunch"],
         "cook food": ["have lunch"],
```

### Comparing `transformlib-0.2.0/tests/test_transform.py` & `transformlib-0.2.3/tests/test_transform.py`

 * *Files identical despite different names*

