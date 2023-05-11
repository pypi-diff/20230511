# Comparing `tmp/sca_rhythm-0.4.2.tar.gz` & `tmp/sca_rhythm-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sca_rhythm-0.4.2.tar", max compression
+gzip compressed data, was "sca_rhythm-0.4.3.tar", max compression
```

## Comparing `sca_rhythm-0.4.2.tar` & `sca_rhythm-0.4.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.2/LICENSE.md
--rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.2/README.md
--rw-r--r--   0        0        0      357 2023-05-11 04:45:07.913259 sca_rhythm-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    15285 2023-05-11 04:15:42.637455 sca_rhythm-0.4.2/sca_rhythm/__init__.py
--rw-r--r--   0        0        0     4750 2023-05-11 04:44:44.748497 sca_rhythm-0.4.2/sca_rhythm/progress.py
--rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 sca_rhythm-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.3/LICENSE.md
+-rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.3/README.md
+-rw-r--r--   0        0        0      357 2023-05-11 14:15:04.199621 sca_rhythm-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    15285 2023-05-11 04:15:42.637455 sca_rhythm-0.4.3/sca_rhythm/__init__.py
+-rw-r--r--   0        0        0     5865 2023-05-11 09:33:08.441589 sca_rhythm-0.4.3/sca_rhythm/progress.py
+-rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 sca_rhythm-0.4.3/PKG-INFO
```

### Comparing `sca_rhythm-0.4.2/LICENSE.md` & `sca_rhythm-0.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.2/README.md` & `sca_rhythm-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.2/sca_rhythm/__init__.py` & `sca_rhythm-0.4.3/sca_rhythm/__init__.py`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.2/sca_rhythm/progress.py` & `sca_rhythm-0.4.3/sca_rhythm/progress.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import math
 import time
+from functools import wraps
+
+from sca_rhythm import WorkflowTask
 
 
 class ExponentialWeightedAverage:
     def __init__(self, alpha: float = 0.9, start: float = 0):
         """
         Class for computing an exponential moving average.
 
@@ -85,43 +88,76 @@
         # calculate avg_rate of progress - fractions / second
         total_time_elapsed = time.perf_counter() - self.start_time
         self.avg_rate = progress / (1e-6 + total_time_elapsed)
 
         return remaining_time
 
 
+def throttle(wait_time):
+    """
+    Decorator that will throttle a function so that it is called only once every wait_time seconds
+    If it is called multiple times, will run only the first time.
+    """
+
+    def decorator(f):
+        decorator.last_call_time = 0
+
+        @wraps(f)
+        def wrapped(*args, **kwargs):
+            current_time = time.perf_counter()
+            elapsed_since_last_call = current_time - decorator.last_call_time
+            if elapsed_since_last_call >= wait_time:
+                val = f(*args, **kwargs)
+                decorator.last_call_time = time.perf_counter()
+                return val
+
+        return wrapped
+
+    return decorator
+
+
 class Progress:
-    def __init__(self, name: str, total: int = None, units: str = None):
+    def __init__(self,
+                 celery_task: WorkflowTask = None,
+                 name: str = '',
+                 total: int = None,
+                 units: str = None,
+                 throttle_time: float = 1.0):
+        self.celery_task = celery_task
         self.name = name
         self.units = units
         self.total = total
         self.eta = ETA()
+        self.update = throttle(throttle_time)(self.update)
 
-    def update(self, done: int):
+    def update(self, done: int) -> dict:
         fraction_done = None
         time_remaining_sec = None
         wt_avg_rate = None
         avg_rate = None
         if self.total:
             fraction_done = done * 1.0 / self.total
             time_remaining_sec = self.eta.update(fraction_done)
             if self.eta.wt_avg_rate:
                 wt_avg_rate = self.total * self.eta.wt_avg_rate
             if self.eta.avg_rate:
                 avg_rate = self.total * self.eta.avg_rate
-        return {
+        prog_obj = {
             'name': self.name,
             'fraction_done': fraction_done,
             'done': done,
             'total': self.total,
             'units': self.units,
             'time_remaining_sec': time_remaining_sec,
             'wt_avg_rate': wt_avg_rate,
             'avg_rate': avg_rate
         }
+        if self.celery_task:
+            self.celery_task.update_progress(prog_obj)
+        return prog_obj
 
 
 if __name__ == '__main__':
     import random
 
     total = 100
     done = 0
```

### Comparing `sca_rhythm-0.4.2/PKG-INFO` & `sca_rhythm-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sca-rhythm
-Version: 0.4.2
+Version: 0.4.3
 Summary: Create and manage workflows using Celery tasks
 Author: Deepak Duggirala
 Author-email: deepakduggi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

