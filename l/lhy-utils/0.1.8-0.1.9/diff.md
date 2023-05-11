# Comparing `tmp/lhy-utils-0.1.8.tar.gz` & `tmp/lhy-utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lhy-utils-0.1.8.tar", last modified: Tue Mar  1 06:39:46 2022, max compression
+gzip compressed data, was "dist/lhy-utils-0.1.9.tar", last modified: Wed Mar  2 09:34:42 2022, max compression
```

## Comparing `lhy-utils-0.1.8.tar` & `lhy-utils-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lhy        (501) staff       (20)        0 2022-03-01 06:39:46.000000 lhy-utils-0.1.8/
--rw-r--r--   0 lhy        (501) staff       (20)      208 2022-03-01 06:39:46.000000 lhy-utils-0.1.8/PKG-INFO
--rw-r--r--   0 lhy        (501) staff       (20)      109 2022-01-19 10:42:38.000000 lhy-utils-0.1.8/README.md
--rw-r--r--   0 lhy        (501) staff       (20)      305 2022-03-01 06:39:38.000000 lhy-utils-0.1.8/setup.py
-drwxr-xr-x   0 lhy        (501) staff       (20)        0 2022-03-01 06:39:46.000000 lhy-utils-0.1.8/lhy_utils.egg-info/
--rw-r--r--   0 lhy        (501) staff       (20)      208 2022-03-01 06:39:46.000000 lhy-utils-0.1.8/lhy_utils.egg-info/PKG-INFO
--rw-r--r--   0 lhy        (501) staff       (20)      305 2022-03-01 06:39:46.000000 lhy-utils-0.1.8/lhy_utils.egg-info/SOURCES.txt
--rw-r--r--   0 lhy        (501) staff       (20)       10 2022-03-01 06:39:46.000000 lhy-utils-0.1.8/lhy_utils.egg-info/top_level.txt
--rw-r--r--   0 lhy        (501) staff       (20)        1 2022-03-01 06:39:46.000000 lhy-utils-0.1.8/lhy_utils.egg-info/dependency_links.txt
--rw-r--r--   0 lhy        (501) staff       (20)       38 2022-03-01 06:39:46.000000 lhy-utils-0.1.8/setup.cfg
-drwxr-xr-x   0 lhy        (501) staff       (20)        0 2022-03-01 06:39:46.000000 lhy-utils-0.1.8/lhy_utils/
--rw-r--r--   0 lhy        (501) staff       (20)     3786 2022-02-25 02:55:21.000000 lhy-utils-0.1.8/lhy_utils/lhy_tool_utils.py
--rw-r--r--   0 lhy        (501) staff       (20)     1582 2022-02-21 07:58:57.000000 lhy-utils-0.1.8/lhy_utils/lhy_io_utils.py
--rw-r--r--   0 lhy        (501) staff       (20)      132 2022-03-01 06:39:38.000000 lhy-utils-0.1.8/lhy_utils/__init__.py
--rw-r--r--   0 lhy        (501) staff       (20)    71402 2022-02-14 06:31:35.000000 lhy-utils-0.1.8/lhy_utils/nlp_logging.py
--rw-r--r--   0 lhy        (501) staff       (20)      311 2021-11-25 02:06:32.000000 lhy-utils-0.1.8/lhy_utils/lhy_net_utils.py
--rw-r--r--   0 lhy        (501) staff       (20)    11604 2022-03-01 06:39:38.000000 lhy-utils-0.1.8/lhy_utils/lhy_log_utils.py
+drwxr-xr-x   0 lhy        (501) staff       (20)        0 2022-03-02 09:34:42.000000 lhy-utils-0.1.9/
+-rw-r--r--   0 lhy        (501) staff       (20)      208 2022-03-02 09:34:42.000000 lhy-utils-0.1.9/PKG-INFO
+-rw-r--r--   0 lhy        (501) staff       (20)      109 2022-01-19 10:42:38.000000 lhy-utils-0.1.9/README.md
+-rw-r--r--   0 lhy        (501) staff       (20)      305 2022-03-02 09:34:21.000000 lhy-utils-0.1.9/setup.py
+drwxr-xr-x   0 lhy        (501) staff       (20)        0 2022-03-02 09:34:42.000000 lhy-utils-0.1.9/lhy_utils.egg-info/
+-rw-r--r--   0 lhy        (501) staff       (20)      208 2022-03-02 09:34:42.000000 lhy-utils-0.1.9/lhy_utils.egg-info/PKG-INFO
+-rw-r--r--   0 lhy        (501) staff       (20)      305 2022-03-02 09:34:42.000000 lhy-utils-0.1.9/lhy_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 lhy        (501) staff       (20)       10 2022-03-02 09:34:42.000000 lhy-utils-0.1.9/lhy_utils.egg-info/top_level.txt
+-rw-r--r--   0 lhy        (501) staff       (20)        1 2022-03-02 09:34:42.000000 lhy-utils-0.1.9/lhy_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 lhy        (501) staff       (20)       38 2022-03-02 09:34:42.000000 lhy-utils-0.1.9/setup.cfg
+drwxr-xr-x   0 lhy        (501) staff       (20)        0 2022-03-02 09:34:42.000000 lhy-utils-0.1.9/lhy_utils/
+-rw-r--r--   0 lhy        (501) staff       (20)     3927 2022-03-02 09:34:21.000000 lhy-utils-0.1.9/lhy_utils/lhy_tool_utils.py
+-rw-r--r--   0 lhy        (501) staff       (20)     1582 2022-02-21 07:58:57.000000 lhy-utils-0.1.9/lhy_utils/lhy_io_utils.py
+-rw-r--r--   0 lhy        (501) staff       (20)      132 2022-03-01 06:39:38.000000 lhy-utils-0.1.9/lhy_utils/__init__.py
+-rw-r--r--   0 lhy        (501) staff       (20)    71402 2022-02-14 06:31:35.000000 lhy-utils-0.1.9/lhy_utils/nlp_logging.py
+-rw-r--r--   0 lhy        (501) staff       (20)      311 2021-11-25 02:06:32.000000 lhy-utils-0.1.9/lhy_utils/lhy_net_utils.py
+-rw-r--r--   0 lhy        (501) staff       (20)    11604 2022-03-01 06:39:38.000000 lhy-utils-0.1.9/lhy_utils/lhy_log_utils.py
```

### Comparing `lhy-utils-0.1.8/lhy_utils/lhy_tool_utils.py` & `lhy-utils-0.1.9/lhy_utils/lhy_tool_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,19 @@
 # coding: utf-8
-# import json
 import math
-import multiprocessing
+import random
 import re
 import subprocess
+import time
 from collections import Counter
+from concurrent.futures import ProcessPoolExecutor
 
 import numpy as np
 
 
-class MultiProcessBase:
-    def __init__(self, data, work_nums=4):
-        self.data = data
-        self.data_num = len(self.data)
-        self.work_nums = work_nums
-        self.result = multiprocessing.Manager().dict()
-
-    def task(self, inputs):
-        # for input in process_inputs:
-        #     data = self.data[input]
-        #     self.result[input] = how to process data
-        raise NotImplemented
-
-    def run(self):
-        inputs = list(cut_list(list(range(self.data_num)), math.ceil(self.data_num / self.work_nums)))
-        jobs = [multiprocessing.Process(target=self.task, args=(inputs[i],)) for i in range(self.work_nums)]
-        for job in jobs:
-            job.start()
-        for job in jobs:
-            job.join()
-        result_list = [0] * self.data_num
-        for key, value in self.result.items():
-            result_list[key] = value
-        return result_list
-
-
 def get_gpu_num():
     try:
         patter = r"[0-9]+MiB"
         all_gpu = []
         popen = subprocess.Popen("nvidia-smi", shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         bz = False
         while popen.poll() is None:
@@ -120,7 +95,45 @@
             else:
                 print.info(line)
     status = p.returncode
     if status != 0:
         # logger.info(f'exec cmd failed. {cmd}', exc_info=True)
         print(f'exec cmd failed. {cmd}')
     return status
+
+
+class MultiProcessBase:
+    def __init__(self, data, work_nums=4, batch_size=None):
+        if batch_size:
+            batch_size = batch_size
+        else:
+            batch_size = math.ceil(len(data) / work_nums)
+        self.input_list = cut_list(data, batch_size)  # 每个进程的数据
+        self.pool = ProcessPoolExecutor(work_nums)
+
+    @staticmethod
+    def task(inputs):
+        raise NotImplemented
+
+    def run(self):
+        obj_list = []
+        for p_id in range(len(self.input_list)):
+            r = self.pool.submit(self.task, self.input_list[p_id])
+            obj_list.append(r)
+        self.pool.shutdown()
+        result_list = []
+        for obj in obj_list:
+            result_list.extend(obj.result())
+        return result_list
+
+
+# class MT(MultiProcessBase):
+#     @staticmethod
+#     def task(inputs):
+#         a = [i ** 8 for i in inputs]
+#         return a
+#
+#
+# if __name__ == '__main__':
+#     data = list(range(10))
+#     m = MT(data)
+#     print(m.run())
```

### Comparing `lhy-utils-0.1.8/lhy_utils/lhy_io_utils.py` & `lhy-utils-0.1.9/lhy_utils/lhy_io_utils.py`

 * *Files identical despite different names*

### Comparing `lhy-utils-0.1.8/lhy_utils/nlp_logging.py` & `lhy-utils-0.1.9/lhy_utils/nlp_logging.py`

 * *Files identical despite different names*

### Comparing `lhy-utils-0.1.8/lhy_utils/lhy_log_utils.py` & `lhy-utils-0.1.9/lhy_utils/lhy_log_utils.py`

 * *Files identical despite different names*

