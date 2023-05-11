# Comparing `tmp/sca_rhythm-0.4.1.tar.gz` & `tmp/sca_rhythm-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sca_rhythm-0.4.1.tar", max compression
+gzip compressed data, was "sca_rhythm-0.4.2.tar", max compression
```

## Comparing `sca_rhythm-0.4.1.tar` & `sca_rhythm-0.4.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.1/LICENSE.md
--rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.1/README.md
--rw-r--r--   0        0        0      375 2023-05-11 04:33:11.313461 sca_rhythm-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    15285 2023-05-11 04:15:42.637455 sca_rhythm-0.4.1/sca_rhythm/__init__.py
--rw-r--r--   0        0        0     4590 2023-05-10 19:37:32.717746 sca_rhythm-0.4.1/sca_rhythm/progress.py
--rw-r--r--   0        0        0     2943 1970-01-01 00:00:00.000000 sca_rhythm-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.2/LICENSE.md
+-rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.2/README.md
+-rw-r--r--   0        0        0      357 2023-05-11 04:45:07.913259 sca_rhythm-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    15285 2023-05-11 04:15:42.637455 sca_rhythm-0.4.2/sca_rhythm/__init__.py
+-rw-r--r--   0        0        0     4750 2023-05-11 04:44:44.748497 sca_rhythm-0.4.2/sca_rhythm/progress.py
+-rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 sca_rhythm-0.4.2/PKG-INFO
```

### Comparing `sca_rhythm-0.4.1/LICENSE.md` & `sca_rhythm-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.1/README.md` & `sca_rhythm-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.1/sca_rhythm/__init__.py` & `sca_rhythm-0.4.2/sca_rhythm/__init__.py`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.1/sca_rhythm/progress.py` & `sca_rhythm-0.4.2/sca_rhythm/progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+import math
 import time
 
-import numpy as np
-
 
 class ExponentialWeightedAverage:
     def __init__(self, alpha: float = 0.9, start: float = 0):
         """
         Class for computing an exponential moving average.
 
         Args:
@@ -61,31 +60,31 @@
 
         if self.start_time is None:
             self.start_time = time.perf_counter()
 
         if self.last_update_time is None:
             self.last_update_time = time.perf_counter()
             self.progress = progress
-            return np.inf
+            return 1e100  # infinity; infinity is not compatible with JSON, use 1e100 instead
 
         diff = progress - self.progress
         self.progress = progress
 
         time_elapsed = time.perf_counter() - self.last_update_time
         self.last_update_time = time.perf_counter()
 
         curr_rate = diff / (1e-6 + time_elapsed)
         self.wt_avg_rate = self.moving_avg.update(curr_rate)
 
         # print(diff, time_elapsed, curr_rate, self.wt_avg_rate)
 
-        if not np.isclose(self.wt_avg_rate, 0):
+        if not math.isclose(self.wt_avg_rate, 0, rel_tol=1e-05, abs_tol=1e-08):
             remaining_time = (1 - progress) / self.wt_avg_rate
         else:
-            remaining_time = np.inf
+            remaining_time = 1e100  # infinity; infinity is not compatible with JSON, use 1e100 instead
 
         # calculate avg_rate of progress - fractions / second
         total_time_elapsed = time.perf_counter() - self.start_time
         self.avg_rate = progress / (1e-6 + total_time_elapsed)
 
         return remaining_time
```

### Comparing `sca_rhythm-0.4.1/PKG-INFO` & `sca_rhythm-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: sca-rhythm
-Version: 0.4.1
+Version: 0.4.2
 Summary: Create and manage workflows using Celery tasks
 Author: Deepak Duggirala
 Author-email: deepakduggi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: celery (>=5.2.7,<6.0.0)
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Rhythm
 Rhythm allows you to design and control workflows made of Celery tasks. A workflow is a sequence of steps to run one after the other. Rhythm simplifies the process of executing workflows consisting of long-running tasks with reliability.
 
 The following are the features of Rhythm workflows:
```

