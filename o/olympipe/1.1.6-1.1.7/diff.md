# Comparing `tmp/olympipe-1.1.6.tar.gz` & `tmp/olympipe-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olympipe-1.1.6.tar", max compression
+gzip compressed data, was "olympipe-1.1.7.tar", max compression
```

## Comparing `olympipe-1.1.6.tar` & `olympipe-1.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-05-11 17:40:16.450558 olympipe-1.1.6/LICENSE
--rw-r--r--   0        0        0     3887 2023-05-11 17:40:16.454558 olympipe-1.1.6/README.md
--rw-r--r--   0        0        0    10410 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/__init__.py
--rw-r--r--   0        0        0     2277 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/dispatcher.py
--rw-r--r--   0        0        0        0 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/pipes/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/pipes/batch.py
--rw-r--r--   0        0        0      530 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/pipes/explode.py
--rw-r--r--   0        0        0      524 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/pipes/filter.py
--rw-r--r--   0        0        0     2275 2023-05-11 17:40:16.454558 olympipe-1.1.6/olympipe/pipes/generic.py
--rw-r--r--   0        0        0     1649 2023-05-11 17:40:16.455559 olympipe-1.1.6/olympipe/pipes/instance.py
--rw-r--r--   0        0        0     1270 2023-05-11 17:40:16.455559 olympipe-1.1.6/olympipe/pipes/reduce.py
--rw-r--r--   0        0        0      408 2023-05-11 17:40:16.455559 olympipe-1.1.6/olympipe/pipes/task.py
--rw-r--r--   0        0        0     1895 2023-05-11 17:40:16.455559 olympipe-1.1.6/olympipe/pipes/timebatch.py
--rw-r--r--   0        0        0        0 2023-05-11 17:40:16.455559 olympipe-1.1.6/olympipe/py.typed
--rw-r--r--   0        0        0      646 2023-05-11 17:40:16.455559 olympipe-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 olympipe-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-11 20:44:35.079416 olympipe-1.1.7/LICENSE
+-rw-r--r--   0        0        0     3887 2023-05-11 20:44:35.083416 olympipe-1.1.7/README.md
+-rw-r--r--   0        0        0    10410 2023-05-11 20:44:35.083416 olympipe-1.1.7/olympipe/__init__.py
+-rw-r--r--   0        0        0     2253 2023-05-11 20:44:35.083416 olympipe-1.1.7/olympipe/dispatcher.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/__init__.py
+-rw-r--r--   0        0        0     1718 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/batch.py
+-rw-r--r--   0        0        0      530 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/explode.py
+-rw-r--r--   0        0        0      524 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/filter.py
+-rw-r--r--   0        0        0     2185 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/generic.py
+-rw-r--r--   0        0        0     1649 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/instance.py
+-rw-r--r--   0        0        0     1180 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/reduce.py
+-rw-r--r--   0        0        0      408 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/task.py
+-rw-r--r--   0        0        0     1899 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/timebatch.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/py.typed
+-rw-r--r--   0        0        0      646 2023-05-11 20:44:35.084416 olympipe-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 olympipe-1.1.7/PKG-INFO
```

### Comparing `olympipe-1.1.6/LICENSE` & `olympipe-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.6/README.md` & `olympipe-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.6/olympipe/__init__.py` & `olympipe-1.1.7/olympipe/__init__.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.6/olympipe/dispatcher.py` & `olympipe-1.1.7/olympipe/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import queue
 import time
 from multiprocessing import Process, Queue
 from threading import Timer
 from typing import Any, Generic, Iterable, List, TypeVar
 
 from .pipes.generic import GenericPipe
 
@@ -56,13 +57,13 @@
             try:
                 packet = self._source.get(timeout=0.1)
                 if GenericPipe.is_death_packet(packet):
                     if self._kill(packet):
                         return
                     else:
                         continue
+            except queue.Empty:
+                continue
             except Exception as e:
-                if str(e.__class__) == "<class '_queue.Empty'>":
-                    continue
                 print("Error", e)
                 return
             self._dispatch([packet])
```

### Comparing `olympipe-1.1.6/olympipe/pipes/batch.py` & `olympipe-1.1.7/olympipe/pipes/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from multiprocessing import Queue
+import queue
 from typing import Iterable, List, Optional, TypeVar
 
 from .generic import GenericPipe
 
 R = TypeVar("R")
 
 
@@ -40,11 +41,13 @@
                 if GenericPipe.is_death_packet(data):
                     if self._keep_incomplete_batch:
                         self._send_to_next(self._datas)
                     self._kill(data)
                     return
                 processed = self._perform_task(data)
                 self._send_to_next(processed)
+            except queue.Empty:
+                continue
             except Exception as e:
                 self._kill(GenericPipe.get_kill_word())
                 print(f"Error_{e.__class__.__name__}_{e.args}")
                 return
```

### Comparing `olympipe-1.1.6/olympipe/pipes/explode.py` & `olympipe-1.1.7/olympipe/pipes/explode.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.6/olympipe/pipes/filter.py` & `olympipe-1.1.7/olympipe/pipes/filter.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.6/olympipe/pipes/generic.py` & `olympipe-1.1.7/olympipe/pipes/generic.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,14 +64,12 @@
                 data = self._source.get(timeout=self._timeout)
                 if GenericPipe.is_death_packet(data):
                     self._kill(data)
                     return
                 processed = self._perform_task(data)
                 self._send_to_next(processed)
             except queue.Empty:
-                pass
+                continue
             except Exception as e:
-                if str(e.__class__) == "<class '_queue.Empty'>":
-                    continue
                 self._kill(GenericPipe.get_kill_word(), True)
                 print(f"Error_{e.__class__.__name__}_{e.args}")
                 return
```

### Comparing `olympipe-1.1.6/olympipe/pipes/instance.py` & `olympipe-1.1.7/olympipe/pipes/instance.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.6/olympipe/pipes/reduce.py` & `olympipe-1.1.7/olympipe/pipes/reduce.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,12 @@
                 data = self._source.get(timeout=self._timeout)
                 if GenericPipe.is_death_packet(data):
                     self._send_to_next(self._accumulator)
                     self._kill(data)
                     return
                 self._perform_task(data)
             except queue.Empty:
-                pass
+                continue
             except Exception as e:
-                if str(e.__class__) == "<class '_queue.Empty'>":
-                    continue
                 self._kill(GenericPipe.get_kill_word())
                 print(f"Error_{e.__class__.__name__}_{e.args}")
                 return
```

### Comparing `olympipe-1.1.6/olympipe/pipes/timebatch.py` & `olympipe-1.1.7/olympipe/pipes/timebatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,12 +48,12 @@
                     self._datas = []
                     self._kill(data)
                     return
                 processed = self._perform_task(data)
                 if processed is not None:
                     self._send_to_next(processed)
             except queue.Empty:
-                pass
+                continue
             except Exception:
                 self._send_to_next(self._datas)
                 self._datas = []
                 self.increment_timeout()
```

### Comparing `olympipe-1.1.6/pyproject.toml` & `olympipe-1.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olympipe"
-version = "1.1.6"
+version = "1.1.7"
 description = "A powerful parallel pipelining tool"
 readme = "README.md"
 license = "MIT"
 homepage = "https://gitlab.com/gabraken/olympipe"
 repository = "https://gitlab.com/gabraken/olympipe"
 authors = ["Gabriel Kasser <gabriel.kasser@gmail.com>"]
 keywords = ["pipeline", "multiprocessing"]
```

### Comparing `olympipe-1.1.6/PKG-INFO` & `olympipe-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olympipe
-Version: 1.1.6
+Version: 1.1.7
 Summary: A powerful parallel pipelining tool
 Home-page: https://gitlab.com/gabraken/olympipe
 License: MIT
 Keywords: pipeline,multiprocessing
 Author: Gabriel Kasser
 Author-email: gabriel.kasser@gmail.com
 Requires-Python: >=3.7.2,<4.0
```

