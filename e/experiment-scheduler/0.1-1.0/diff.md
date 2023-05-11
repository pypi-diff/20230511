# Comparing `tmp/experiment-scheduler-0.1.tar.gz` & `tmp/experiment-scheduler-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment-scheduler-0.1.tar", last modified: Sun Nov  6 08:37:44 2022, max compression
+gzip compressed data, was "experiment-scheduler-1.0.tar", last modified: Thu May 11 11:36:09 2023, max compression
```

## Comparing `experiment-scheduler-0.1.tar` & `experiment-scheduler-1.0.tar`

### file list

```diff
@@ -1,57 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.915037 experiment-scheduler-0.1/
--rw-rw-rw-   0        0        0     1091 2022-08-05 13:57:22.000000 experiment-scheduler-0.1/LICENSE
--rw-rw-rw-   0        0        0     1009 2022-11-06 08:37:44.914035 experiment-scheduler-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2186 2022-10-17 03:15:22.000000 experiment-scheduler-0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.875441 experiment-scheduler-0.1/experiment_scheduler/
--rw-rw-rw-   0        0        0        0 2022-08-05 13:58:00.000000 experiment-scheduler-0.1/experiment_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.885029 experiment-scheduler-0.1/experiment_scheduler/common/
--rw-rw-rw-   0        0        0        0 2022-09-19 04:36:28.000000 experiment-scheduler-0.1/experiment_scheduler/common/__init__.py
--rw-rw-rw-   0        0        0     1012 2022-10-17 03:15:22.000000 experiment-scheduler-0.1/experiment_scheduler/common/settings.py
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.888029 experiment-scheduler-0.1/experiment_scheduler/master/
--rw-rw-rw-   0        0        0        0 2022-08-05 13:58:00.000000 experiment-scheduler-0.1/experiment_scheduler/master/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.891030 experiment-scheduler-0.1/experiment_scheduler/master/grpc_master/
--rw-rw-rw-   0        0        0        0 2022-09-19 04:36:28.000000 experiment-scheduler-0.1/experiment_scheduler/master/grpc_master/__init__.py
--rw-rw-rw-   0        0        0     4397 2022-11-06 08:24:02.000000 experiment-scheduler-0.1/experiment_scheduler/master/grpc_master/master_pb2.py
--rw-rw-rw-   0        0        0     4325 2022-11-06 08:24:02.000000 experiment-scheduler-0.1/experiment_scheduler/master/grpc_master/master_pb2_grpc.py
--rw-rw-rw-   0        0        0     8344 2022-11-06 08:24:02.000000 experiment-scheduler-0.1/experiment_scheduler/master/master.py
--rw-rw-rw-   0        0        0     3903 2022-11-06 08:24:02.000000 experiment-scheduler-0.1/experiment_scheduler/master/process_monitor.py
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.893031 experiment-scheduler-0.1/experiment_scheduler/resource_monitor/
--rw-rw-rw-   0        0        0        0 2022-09-19 04:31:03.000000 experiment-scheduler-0.1/experiment_scheduler/resource_monitor/__init__.py
--rw-rw-rw-   0        0        0     2857 2022-10-17 03:15:22.000000 experiment-scheduler-0.1/experiment_scheduler/resource_monitor/monitor.py
--rw-rw-rw-   0        0        0      669 2022-10-17 03:15:22.000000 experiment-scheduler-0.1/experiment_scheduler/resource_monitor/setting.py
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.901033 experiment-scheduler-0.1/experiment_scheduler/submitter/
--rw-rw-rw-   0        0        0        0 2022-08-05 13:58:00.000000 experiment-scheduler-0.1/experiment_scheduler/submitter/__init__.py
--rw-rw-rw-   0        0        0       42 2022-11-06 08:24:02.000000 experiment-scheduler-0.1/experiment_scheduler/submitter/delete.py
--rw-rw-rw-   0        0        0       42 2022-08-05 13:58:00.000000 experiment-scheduler-0.1/experiment_scheduler/submitter/edit.py
--rw-rw-rw-   0        0        0     1878 2022-11-06 08:24:02.000000 experiment-scheduler-0.1/experiment_scheduler/submitter/execute.py
--rw-rw-rw-   0        0        0     1305 2022-11-06 08:24:02.000000 experiment-scheduler-0.1/experiment_scheduler/submitter/exs.py
--rw-rw-rw-   0        0        0      772 2022-09-19 04:36:28.000000 experiment-scheduler-0.1/experiment_scheduler/submitter/init_master.py
--rw-rw-rw-   0        0        0      764 2022-09-19 04:36:28.000000 experiment-scheduler-0.1/experiment_scheduler/submitter/init_task_manager.py
--rw-rw-rw-   0        0        0       48 2022-11-06 08:24:02.000000 experiment-scheduler-0.1/experiment_scheduler/submitter/list.py
--rw-rw-rw-   0        0        0       42 2022-11-06 08:24:02.000000 experiment-scheduler-0.1/experiment_scheduler/submitter/status.py
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.903033 experiment-scheduler-0.1/experiment_scheduler/task_manager/
--rw-rw-rw-   0        0        0      137 2022-10-17 03:15:22.000000 experiment-scheduler-0.1/experiment_scheduler/task_manager/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.906034 experiment-scheduler-0.1/experiment_scheduler/task_manager/grpc_task_manager/
--rw-rw-rw-   0        0        0        0 2022-09-19 04:36:28.000000 experiment-scheduler-0.1/experiment_scheduler/task_manager/grpc_task_manager/__init__.py
--rw-rw-rw-   0        0        0     5504 2022-09-19 04:36:28.000000 experiment-scheduler-0.1/experiment_scheduler/task_manager/grpc_task_manager/task_manager_pb2.py
--rw-rw-rw-   0        0        0    10301 2022-09-19 04:36:28.000000 experiment-scheduler-0.1/experiment_scheduler/task_manager/grpc_task_manager/task_manager_pb2_grpc.py
--rw-rw-rw-   0        0        0     5992 2022-11-06 08:24:02.000000 experiment-scheduler-0.1/experiment_scheduler/task_manager/task_manager_server.py
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.884029 experiment-scheduler-0.1/experiment_scheduler.egg-info/
--rw-rw-rw-   0        0        0     1009 2022-11-06 08:37:44.000000 experiment-scheduler-0.1/experiment_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1714 2022-11-06 08:37:44.000000 experiment-scheduler-0.1/experiment_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-06 08:37:44.000000 experiment-scheduler-0.1/experiment_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2022-11-06 08:37:44.000000 experiment-scheduler-0.1/experiment_scheduler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2022-11-06 08:37:44.000000 experiment-scheduler-0.1/experiment_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-06 08:37:44.915037 experiment-scheduler-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1317 2022-11-06 08:37:23.000000 experiment-scheduler-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.907034 experiment-scheduler-0.1/test/
--rw-rw-rw-   0        0        0        0 2022-09-19 04:36:28.000000 experiment-scheduler-0.1/test/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.912035 experiment-scheduler-0.1/test/master/
--rw-rw-rw-   0        0        0        0 2022-08-05 13:57:22.000000 experiment-scheduler-0.1/test/master/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-06 08:37:44.913036 experiment-scheduler-0.1/test/master/example/
--rw-rw-rw-   0        0        0        0 2022-09-19 04:36:28.000000 experiment-scheduler-0.1/test/master/example/__init__.py
--rw-rw-rw-   0        0        0       28 2022-09-19 04:36:28.000000 experiment-scheduler-0.1/test/master/example/test.py
--rw-rw-rw-   0        0        0     3413 2022-09-19 04:36:28.000000 experiment-scheduler-0.1/test/master/master.py
--rw-rw-rw-   0        0        0        0 2022-09-19 04:36:28.000000 experiment-scheduler-0.1/test/master/process_monitor.py
--rw-rw-rw-   0        0        0     5382 2022-10-17 03:15:22.000000 experiment-scheduler-0.1/test/master/test_master.py
--rw-rw-rw-   0        0        0     5483 2022-10-17 03:15:22.000000 experiment-scheduler-0.1/test/master/test_process_monitor.py
+drwxrwxrwx   0 suhwan    (1000) suhwan    (1000)        0 2023-05-11 11:36:09.227212 experiment-scheduler-1.0/
+-rwxrwxrwx   0 suhwan    (1000) suhwan    (1000)     1070 2023-04-20 10:10:25.000000 experiment-scheduler-1.0/LICENSE
+-rwxrwxrwx   0 suhwan    (1000) suhwan    (1000)     4660 2023-05-11 11:36:09.219377 experiment-scheduler-1.0/PKG-INFO
+-rwxrwxrwx   0 suhwan    (1000) suhwan    (1000)     4353 2023-05-11 10:40:26.000000 experiment-scheduler-1.0/README.md
+drwxrwxrwx   0 suhwan    (1000) suhwan    (1000)        0 2023-05-11 11:36:09.124693 experiment-scheduler-1.0/experiment_scheduler.egg-info/
+-rwxrwxrwx   0 suhwan    (1000) suhwan    (1000)     4660 2023-05-11 11:36:08.000000 experiment-scheduler-1.0/experiment_scheduler.egg-info/PKG-INFO
+-rwxrwxrwx   0 suhwan    (1000) suhwan    (1000)      292 2023-05-11 11:36:08.000000 experiment-scheduler-1.0/experiment_scheduler.egg-info/SOURCES.txt
+-rwxrwxrwx   0 suhwan    (1000) suhwan    (1000)        1 2023-05-11 11:36:08.000000 experiment-scheduler-1.0/experiment_scheduler.egg-info/dependency_links.txt
+-rwxrwxrwx   0 suhwan    (1000) suhwan    (1000)       64 2023-05-11 11:36:08.000000 experiment-scheduler-1.0/experiment_scheduler.egg-info/entry_points.txt
+-rwxrwxrwx   0 suhwan    (1000) suhwan    (1000)      133 2023-05-11 11:36:08.000000 experiment-scheduler-1.0/experiment_scheduler.egg-info/requires.txt
+-rwxrwxrwx   0 suhwan    (1000) suhwan    (1000)        1 2023-05-11 11:36:08.000000 experiment-scheduler-1.0/experiment_scheduler.egg-info/top_level.txt
+-rwxrwxrwx   0 suhwan    (1000) suhwan    (1000)       38 2023-05-11 11:36:09.246600 experiment-scheduler-1.0/setup.cfg
+-rwxrwxrwx   0 suhwan    (1000) suhwan    (1000)      777 2023-05-11 11:34:16.000000 experiment-scheduler-1.0/setup.py
```

### Comparing `experiment-scheduler-0.1/LICENSE` & `experiment-scheduler-1.0/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 ddangcoonfire
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 ddangcoonfire
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

