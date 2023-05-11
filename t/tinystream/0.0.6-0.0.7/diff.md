# Comparing `tmp/tinystream-0.0.6.tar.gz` & `tmp/tinystream-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinystream-0.0.6.tar", last modified: Wed May 10 12:29:50 2023, max compression
+gzip compressed data, was "tinystream-0.0.7.tar", last modified: Thu May 11 17:27:38 2023, max compression
```

## Comparing `tinystream-0.0.6.tar` & `tinystream-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-10 12:29:50.024924 tinystream-0.0.6/
--rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.0.6/LICENSE
--rw-r--r--   0 mikereiche   (502) staff       (20)     3829 2023-05-10 12:29:50.024795 tinystream-0.0.6/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     3595 2023-05-10 11:02:57.000000 tinystream-0.0.6/README.md
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-10 12:29:50.024965 tinystream-0.0.6/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      510 2023-05-10 12:17:31.000000 tinystream-0.0.6/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-10 12:29:50.024608 tinystream-0.0.6/tinystream.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3829 2023-05-10 12:29:50.000000 tinystream-0.0.6/tinystream.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      209 2023-05-10 12:29:50.000000 tinystream-0.0.6/tinystream.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-10 12:29:50.000000 tinystream-0.0.6/tinystream.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       19 2023-05-10 12:29:50.000000 tinystream-0.0.6/tinystream.egg-info/requires.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-10 12:29:50.000000 tinystream-0.0.6/tinystream.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)     5950 2023-05-10 10:59:00.000000 tinystream-0.0.6/tinystream.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-11 17:27:38.435296 tinystream-0.0.7/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.0.7/LICENSE
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3795 2023-05-11 17:27:38.435153 tinystream-0.0.7/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3561 2023-05-11 17:04:01.000000 tinystream-0.0.7/README.md
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-11 17:27:38.435340 tinystream-0.0.7/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      490 2023-05-11 17:04:39.000000 tinystream-0.0.7/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-11 17:27:38.434965 tinystream-0.0.7/tinystream.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3795 2023-05-11 17:27:38.000000 tinystream-0.0.7/tinystream.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      176 2023-05-11 17:27:38.000000 tinystream-0.0.7/tinystream.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-11 17:27:38.000000 tinystream-0.0.7/tinystream.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-11 17:27:38.000000 tinystream-0.0.7/tinystream.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5863 2023-05-11 17:23:14.000000 tinystream-0.0.7/tinystream.py
```

### Comparing `tinystream-0.0.6/LICENSE` & `tinystream-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tinystream-0.0.6/PKG-INFO` & `tinystream-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tinystream
-Version: 0.0.6
+Version: 0.0.7
 Summary: Yet another python streams library
 Home-page: https://github.com/mreiche/python-streams
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
-[![Code Coverage Status](https://codecov.io/github/mreiche/python-streams/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-automation-framework)
+[![Code Coverage Status](https://codecov.io/github/mreiche/python-streams/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-streams)
 
 # tinystream / python-streams
 
 This is a simple and lightweight Streams API inspired by Java Streams with support for type hinting.
 
 This package is release as `tinystream` at pypi.
 
@@ -26,15 +26,15 @@
 stream \
     .map(lambda x: x + 1) \       # flatmap(), peek(), map_key()
     .filter(lambda x: x > 2) \    # filter_key()
     .sorted(int, reverse=True) \  # sort()
     .reverse() \                  # collect(), count()
     .limit(2) \
     .concat([4]) \
-    .sum()                        # first, reduce(), max(), min()
+    .sum()                        # reduce(), max(), min()
 ```
 
 ## Typehinting
 
 Since Python does not support typed lambdas, this library implements a workaround.
 
 ```python
@@ -78,20 +78,29 @@
 ```python
 def map_parent(n: Node):
     return n.parent
 
 assert next(stream.map(map_parent)).name == "B"
 ```
 
-## Retrieve optional
+### Typed dictionaries
 
-The `first` property returns a [optional.py:Optional](https://pypi.org/project/optional.py/) 
+Dictionaries are streamed as `tuple(key, value)`
+
+```python
+children = {"a": Node(name="Child")} 
+stream = Stream.of_dict(children)
+for item in stream:
+    # item[0] is known as str
+    # item[1] is known as Node
+```
 
+This is the same like (but without known types):
 ```python
-stream.first.is_present()
+stream = Stream.of(children)
 ```
 
 ## End of stream
 
 Calling methods like `sum()`, `collect()`, `count()`... will end the stream.
 
 ## More features
@@ -119,24 +128,14 @@
 
 ### Collected join
 
 ```python
 all_names = Stream.of([child]).map_key("name").join(", ")
 ```
 
-### Stream dictionaries
-
-Dictionaries are streamed as `tuple(key, value)`
-
-```python
-children = {"a": child} 
-stream = Stream.of_dict(children)
-values = stream.map_key(1, typehint=Node)
-```
-
 ## Comparison with other libraries
 
 There are a couple of other implementation to fulfill similar requirements.
 
 - https://github.com/alemazzo/Python-Java-Stream
 - https://github.com/ramsteak/streams
 - https://pypi.org/project/fluentpy
```

### Comparing `tinystream-0.0.6/README.md` & `tinystream-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
-[![Code Coverage Status](https://codecov.io/github/mreiche/python-streams/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-automation-framework)
+[![Code Coverage Status](https://codecov.io/github/mreiche/python-streams/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-streams)
 
 # tinystream / python-streams
 
 This is a simple and lightweight Streams API inspired by Java Streams with support for type hinting.
 
 This package is release as `tinystream` at pypi.
 
@@ -17,15 +17,15 @@
 stream \
     .map(lambda x: x + 1) \       # flatmap(), peek(), map_key()
     .filter(lambda x: x > 2) \    # filter_key()
     .sorted(int, reverse=True) \  # sort()
     .reverse() \                  # collect(), count()
     .limit(2) \
     .concat([4]) \
-    .sum()                        # first, reduce(), max(), min()
+    .sum()                        # reduce(), max(), min()
 ```
 
 ## Typehinting
 
 Since Python does not support typed lambdas, this library implements a workaround.
 
 ```python
@@ -69,20 +69,29 @@
 ```python
 def map_parent(n: Node):
     return n.parent
 
 assert next(stream.map(map_parent)).name == "B"
 ```
 
-## Retrieve optional
+### Typed dictionaries
 
-The `first` property returns a [optional.py:Optional](https://pypi.org/project/optional.py/) 
+Dictionaries are streamed as `tuple(key, value)`
+
+```python
+children = {"a": Node(name="Child")} 
+stream = Stream.of_dict(children)
+for item in stream:
+    # item[0] is known as str
+    # item[1] is known as Node
+```
 
+This is the same like (but without known types):
 ```python
-stream.first.is_present()
+stream = Stream.of(children)
 ```
 
 ## End of stream
 
 Calling methods like `sum()`, `collect()`, `count()`... will end the stream.
 
 ## More features
@@ -110,24 +119,14 @@
 
 ### Collected join
 
 ```python
 all_names = Stream.of([child]).map_key("name").join(", ")
 ```
 
-### Stream dictionaries
-
-Dictionaries are streamed as `tuple(key, value)`
-
-```python
-children = {"a": child} 
-stream = Stream.of_dict(children)
-values = stream.map_key(1, typehint=Node)
-```
-
 ## Comparison with other libraries
 
 There are a couple of other implementation to fulfill similar requirements.
 
 - https://github.com/alemazzo/Python-Java-Stream
 - https://github.com/ramsteak/streams
 - https://pypi.org/project/fluentpy
```

### Comparing `tinystream-0.0.6/tinystream.egg-info/PKG-INFO` & `tinystream-0.0.7/tinystream.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tinystream
-Version: 0.0.6
+Version: 0.0.7
 Summary: Yet another python streams library
 Home-page: https://github.com/mreiche/python-streams
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
-[![Code Coverage Status](https://codecov.io/github/mreiche/python-streams/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-automation-framework)
+[![Code Coverage Status](https://codecov.io/github/mreiche/python-streams/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-streams)
 
 # tinystream / python-streams
 
 This is a simple and lightweight Streams API inspired by Java Streams with support for type hinting.
 
 This package is release as `tinystream` at pypi.
 
@@ -26,15 +26,15 @@
 stream \
     .map(lambda x: x + 1) \       # flatmap(), peek(), map_key()
     .filter(lambda x: x > 2) \    # filter_key()
     .sorted(int, reverse=True) \  # sort()
     .reverse() \                  # collect(), count()
     .limit(2) \
     .concat([4]) \
-    .sum()                        # first, reduce(), max(), min()
+    .sum()                        # reduce(), max(), min()
 ```
 
 ## Typehinting
 
 Since Python does not support typed lambdas, this library implements a workaround.
 
 ```python
@@ -78,20 +78,29 @@
 ```python
 def map_parent(n: Node):
     return n.parent
 
 assert next(stream.map(map_parent)).name == "B"
 ```
 
-## Retrieve optional
+### Typed dictionaries
 
-The `first` property returns a [optional.py:Optional](https://pypi.org/project/optional.py/) 
+Dictionaries are streamed as `tuple(key, value)`
+
+```python
+children = {"a": Node(name="Child")} 
+stream = Stream.of_dict(children)
+for item in stream:
+    # item[0] is known as str
+    # item[1] is known as Node
+```
 
+This is the same like (but without known types):
 ```python
-stream.first.is_present()
+stream = Stream.of(children)
 ```
 
 ## End of stream
 
 Calling methods like `sum()`, `collect()`, `count()`... will end the stream.
 
 ## More features
@@ -119,24 +128,14 @@
 
 ### Collected join
 
 ```python
 all_names = Stream.of([child]).map_key("name").join(", ")
 ```
 
-### Stream dictionaries
-
-Dictionaries are streamed as `tuple(key, value)`
-
-```python
-children = {"a": child} 
-stream = Stream.of_dict(children)
-values = stream.map_key(1, typehint=Node)
-```
-
 ## Comparison with other libraries
 
 There are a couple of other implementation to fulfill similar requirements.
 
 - https://github.com/alemazzo/Python-Java-Stream
 - https://github.com/ramsteak/streams
 - https://pypi.org/project/fluentpy
```

### Comparing `tinystream-0.0.6/tinystream.py` & `tinystream-0.0.7/tinystream.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import functools
 import itertools
-import logging
-from typing import Iterable, TypeVar, Callable, List, Dict, Tuple, Iterator
+import sys
 import warnings
-from optional import Optional
+from typing import Iterable, TypeVar, Callable, List, Dict, Tuple, Iterator
 
 T = TypeVar("T")
 R = TypeVar("R")
 K = TypeVar("K")
 
 
 class Stream:
@@ -21,29 +20,26 @@
         return IterableStream[Tuple[K, T]](source_dict)
 
     @staticmethod
     def of_many(typehint: T = None, *iterables):
         return IterableStream[T]([]).concat(*iterables)
 
 
-
 class IterableStream(Iterator[T]):
 
-    def __next__(self) -> T|None:
+    def __next__(self) -> T | None:
         try:
             return next(self.__iterable)
         except StopIteration as e:
             return None
 
     def __iter__(self) -> Iterator[T]:
         return self.__iterable.__iter__()
 
     def __normalize_iterator(self, iterable: Iterable[T]) -> Iterable[T]:
-        #if isinstance(iterable, Iterator):
-
         if isinstance(iterable, list):
             return iter(iterable)
         elif isinstance(iterable, dict):
             return iter(iterable.items())
         elif isinstance(iterable, str):
             return iter(iterable)
         else:
@@ -138,18 +134,14 @@
         warnings.warn("Use the stream as iterator instead", DeprecationWarning)
         return self.__iterable
 
     def next(self) -> T | None:
         warnings.warn("Use next(stream) instead", DeprecationWarning)
         return self.__next__()
 
-    @property
-    def first(self):
-        return Optional.of(self.next())
-
     def collect(self):
         """Collects all items to a list and ends the stream"""
         if not self.__collected:
             self.__collected = list(self.__iterable)
         return self.__collected
 
     def join(self, separator: str) -> str:
@@ -162,15 +154,18 @@
 
     def reverse(self):
         copy = self.collect().copy()
         copy.reverse()
         return IterableStream[T](copy)
 
     def reduce(self, cb: Callable[[T, T], R]) -> R:
-        return functools.reduce(cb, self.__iterable)
+        try:
+            return functools.reduce(cb, self.__iterable)
+        except TypeError:
+            return None
 
     def sum(self) -> T:
         """Sums all numbers and ends the stream"""
         return self.reduce(lambda x, y: x + y)
 
     def max(self) -> T:
         return self.reduce(lambda x, y: x if x > y else y)
```

