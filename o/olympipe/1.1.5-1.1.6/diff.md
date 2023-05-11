# Comparing `tmp/olympipe-1.1.5.tar.gz` & `tmp/olympipe-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olympipe-1.1.5.tar", max compression
+gzip compressed data, was "olympipe-1.1.6.tar", max compression
```

## Comparing `olympipe-1.1.5.tar` & `olympipe-1.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-03-19 15:19:05.456089 olympipe-1.1.5/LICENSE
--rw-r--r--   0        0        0     3887 2023-03-19 15:19:05.456089 olympipe-1.1.5/README.md
--rw-r--r--   0        0        0    10411 2023-03-19 15:19:05.456089 olympipe-1.1.5/olympipe/__init__.py
--rw-r--r--   0        0        0     2276 2023-03-19 16:25:53.753350 olympipe-1.1.5/olympipe/dispatcher.py
--rw-r--r--   0        0        0        0 2023-03-19 16:42:59.596303 olympipe-1.1.5/olympipe/pipes/__init__.py
--rw-r--r--   0        0        0     1647 2023-03-19 15:19:05.456089 olympipe-1.1.5/olympipe/pipes/batch.py
--rw-r--r--   0        0        0      530 2023-03-19 15:19:05.456089 olympipe-1.1.5/olympipe/pipes/explode.py
--rw-r--r--   0        0        0      523 2023-03-19 15:19:05.456089 olympipe-1.1.5/olympipe/pipes/filter.py
--rw-r--r--   0        0        0     2210 2023-03-19 16:25:53.753350 olympipe-1.1.5/olympipe/pipes/generic.py
--rw-r--r--   0        0        0     1522 2023-03-19 15:25:07.506841 olympipe-1.1.5/olympipe/pipes/instance.py
--rw-r--r--   0        0        0     1203 2023-03-19 15:19:05.456089 olympipe-1.1.5/olympipe/pipes/reduce.py
--rw-r--r--   0        0        0      407 2023-03-19 15:19:05.456089 olympipe-1.1.5/olympipe/pipes/task.py
--rw-r--r--   0        0        0     1829 2023-03-19 15:19:05.456089 olympipe-1.1.5/olympipe/pipes/timebatch.py
--rw-r--r--   0        0        0        0 2023-03-19 16:42:59.596303 olympipe-1.1.5/olympipe/py.typed
--rw-r--r--   0        0        0      646 2023-03-19 16:25:53.753350 olympipe-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 olympipe-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-11 17:40:16.450558 olympipe-1.1.6/LICENSE
+-rw-r--r--   0        0        0     3887 2023-05-11 17:40:16.454558 olympipe-1.1.6/README.md
+-rw-r--r--   0        0        0    10410 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/__init__.py
+-rw-r--r--   0        0        0     2277 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/dispatcher.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/pipes/__init__.py
+-rw-r--r--   0        0        0     1648 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/pipes/batch.py
+-rw-r--r--   0        0        0      530 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/pipes/explode.py
+-rw-r--r--   0        0        0      524 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/pipes/filter.py
+-rw-r--r--   0        0        0     2275 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/pipes/generic.py
+-rw-r--r--   0        0        0     1649 2023-05-11 17:40:16.455559 olympipe-1.1.6/olympipe/pipes/instance.py
+-rw-r--r--   0        0        0     1270 2023-05-11 17:40:16.455559 olympipe-1.1.6/olympipe/pipes/reduce.py
+-rw-r--r--   0        0        0      408 2023-05-11 17:40:16.455559 olympipe-1.1.6/olympipe/pipes/task.py
+-rw-r--r--   0        0        0     1895 2023-05-11 17:40:16.455559 olympipe-1.1.6/olympipe/pipes/timebatch.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:40:16.455559 olympipe-1.1.6/olympipe/py.typed
+-rw-r--r--   0        0        0      646 2023-05-11 17:40:16.455559 olympipe-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 olympipe-1.1.6/PKG-INFO
```

### Comparing `olympipe-1.1.5/LICENSE` & `olympipe-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.5/README.md` & `olympipe-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.5/olympipe/__init__.py` & `olympipe-1.1.6/olympipe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,23 @@
     List,
     Optional,
     Tuple,
     TypeVar,
     cast,
 )
 
-
-from olympipe.pipes.reduce import ReducePipe
-from olympipe.pipes.generic import GenericPipe
-from olympipe.pipes.task import TaskPipe
-from olympipe.pipes.filter import FilterPipe
-from olympipe.pipes.explode import ExplodePipe
+from olympipe.dispatcher import Dispatcher
 from olympipe.pipes.batch import BatchPipe
+from olympipe.pipes.explode import ExplodePipe
+from olympipe.pipes.filter import FilterPipe
+from olympipe.pipes.generic import GenericPipe
 from olympipe.pipes.instance import ClassInstancePipe
+from olympipe.pipes.reduce import ReducePipe
+from olympipe.pipes.task import TaskPipe
 from olympipe.pipes.timebatch import TimeBatchPipe
-from olympipe.dispatcher import Dispatcher
 
 R = TypeVar("R")
 S = TypeVar("S")
 T = TypeVar("T")
 
 
 class Pipeline(Generic[R]):
```

### Comparing `olympipe-1.1.5/olympipe/dispatcher.py` & `olympipe-1.1.6/olympipe/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
 from multiprocessing import Process, Queue
 from threading import Timer
 from typing import Any, Generic, Iterable, List, TypeVar
+
 from .pipes.generic import GenericPipe
 
 S = TypeVar("S")
 
 
 class Dispatcher(Process, Generic[S]):
     def __init__(self, queue: "Queue[S]"):
```

### Comparing `olympipe-1.1.5/olympipe/pipes/batch.py` & `olympipe-1.1.6/olympipe/pipes/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from multiprocessing import Queue
 from typing import Iterable, List, Optional, TypeVar
+
 from .generic import GenericPipe
 
 R = TypeVar("R")
 
 
 class BatchPipe(GenericPipe[R, Iterable[R]]):
     def __init__(
```

### Comparing `olympipe-1.1.5/olympipe/pipes/explode.py` & `olympipe-1.1.6/olympipe/pipes/explode.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.5/olympipe/pipes/filter.py` & `olympipe-1.1.6/olympipe/pipes/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from multiprocessing import Queue
 from typing import Callable, TypeVar
+
 from .generic import GenericPipe
 
 R = TypeVar("R")
 
 
 class FilterPipe(GenericPipe[R, R]):
     def __init__(
```

### Comparing `olympipe-1.1.5/olympipe/pipes/generic.py` & `olympipe-1.1.6/olympipe/pipes/generic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import queue
 import time
 from multiprocessing import Process, Queue
 from queue import Empty
 from threading import Timer
 from typing import Any, Generic, Optional, Tuple, TypeVar, cast
 
 R = TypeVar("R")
@@ -12,15 +13,15 @@
     __kill_word: Any = Empty
 
     def __init__(self, source: "Queue[R]", target: "Queue[S]"):
         super().__init__(daemon=True)
         self._source = source
         self._target = target
         self._timeout: Optional[float] = 0.1
-        Timer(0.015, self.start).start()
+        Timer(0.01, self.start).start()
 
     @staticmethod
     def is_death_packet(p: Any) -> bool:
         try:
             return p[0] is GenericPipe.__kill_word
         except Exception:
             return False
@@ -62,13 +63,15 @@
             try:
                 data = self._source.get(timeout=self._timeout)
                 if GenericPipe.is_death_packet(data):
                     self._kill(data)
                     return
                 processed = self._perform_task(data)
                 self._send_to_next(processed)
+            except queue.Empty:
+                pass
             except Exception as e:
                 if str(e.__class__) == "<class '_queue.Empty'>":
                     continue
                 self._kill(GenericPipe.get_kill_word(), True)
                 print(f"Error_{e.__class__.__name__}_{e.args}")
                 return
```

### Comparing `olympipe-1.1.5/olympipe/pipes/instance.py` & `olympipe-1.1.6/olympipe/pipes/instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from multiprocessing import Queue
-from typing import Optional, TypeVar, Dict, List, Any, Callable
 from multiprocessing.managers import BaseManager
+from typing import Any, Callable, Dict, List, Optional, TypeVar
+
 from .generic import GenericPipe
 
 R = TypeVar("R")
 S = TypeVar("S")
 
 
 class ClassInstancePipe(GenericPipe[R, S]):
@@ -14,31 +15,34 @@
         constructor_class: Any,
         use_method: Callable[[Any, R], S],
         target: "Queue[S]",
         close_method: Optional[Callable[[Any], Any]] = None,
         args_class: List[Any] = [],
         kwargs_class: Dict[str, Any] = {},
     ):
+        BaseManager.register(constructor_class.__name__, constructor_class)
+        self._constructor_class = constructor_class
         self._use_method = use_method
         self._close_method = close_method
         self._args_class = args_class
         self._kwargs_class = kwargs_class
-        self._constructor_class = constructor_class
-        BaseManager.register(self._constructor_class.__name__, self._constructor_class)
-        super().__init__(source, target)
+        self._source = source
+        self._target = target
+        super().__init__(self._source, self._target)
 
-    def start(self):
+    def start(self) -> None:
         self._instance = self._constructor_class(
             *self._args_class, **self._kwargs_class
         )
         self._task = getattr(self._instance, self._use_method.__name__)
         if self._close_method is not None:
             self._close_method = getattr(self._instance, self._close_method.__name__)
-
-        super().start()
+        else:
+            self._close_method = None
+        return super().start()
 
     def _perform_task(self, data: R) -> S:
         return self._task(data)
 
     def _kill(self, data: Any, error: bool = False):
         if self._close_method is not None:
             self._close_method()  # type: ignore
```

### Comparing `olympipe-1.1.5/olympipe/pipes/reduce.py` & `olympipe-1.1.6/olympipe/pipes/reduce.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import queue
 from multiprocessing import Queue
 from typing import Callable, TypeVar
+
 from .generic import GenericPipe
 
 R = TypeVar("R")
 T = TypeVar("T")
 
 
 class ReducePipe(GenericPipe[R, T]):
@@ -26,13 +28,15 @@
             try:
                 data = self._source.get(timeout=self._timeout)
                 if GenericPipe.is_death_packet(data):
                     self._send_to_next(self._accumulator)
                     self._kill(data)
                     return
                 self._perform_task(data)
+            except queue.Empty:
+                pass
             except Exception as e:
                 if str(e.__class__) == "<class '_queue.Empty'>":
                     continue
                 self._kill(GenericPipe.get_kill_word())
                 print(f"Error_{e.__class__.__name__}_{e.args}")
                 return
```

### Comparing `olympipe-1.1.5/olympipe/pipes/timebatch.py` & `olympipe-1.1.6/olympipe/pipes/timebatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import queue
 import time
 from multiprocessing import Queue
 from typing import Iterable, List, Optional, TypeVar
+
 from .generic import GenericPipe
 
 R = TypeVar("R")
 S = TypeVar("S")
 T = TypeVar("T")
 
 
@@ -45,12 +47,13 @@
                     self._send_to_next(self._datas)
                     self._datas = []
                     self._kill(data)
                     return
                 processed = self._perform_task(data)
                 if processed is not None:
                     self._send_to_next(processed)
-
+            except queue.Empty:
+                pass
             except Exception:
                 self._send_to_next(self._datas)
                 self._datas = []
                 self.increment_timeout()
```

### Comparing `olympipe-1.1.5/pyproject.toml` & `olympipe-1.1.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olympipe"
-version = "1.1.5"
+version = "1.1.6"
 description = "A powerful parallel pipelining tool"
 readme = "README.md"
 license = "MIT"
 homepage = "https://gitlab.com/gabraken/olympipe"
 repository = "https://gitlab.com/gabraken/olympipe"
 authors = ["Gabriel Kasser <gabriel.kasser@gmail.com>"]
 keywords = ["pipeline", "multiprocessing"]
```

### Comparing `olympipe-1.1.5/PKG-INFO` & `olympipe-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olympipe
-Version: 1.1.5
+Version: 1.1.6
 Summary: A powerful parallel pipelining tool
 Home-page: https://gitlab.com/gabraken/olympipe
 License: MIT
 Keywords: pipeline,multiprocessing
 Author: Gabriel Kasser
 Author-email: gabriel.kasser@gmail.com
 Requires-Python: >=3.7.2,<4.0
```

