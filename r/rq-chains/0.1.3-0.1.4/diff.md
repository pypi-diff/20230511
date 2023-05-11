# Comparing `tmp/rq-chains-0.1.3.tar.gz` & `tmp/rq-chains-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rq-chains-0.1.3.tar", last modified: Wed May 10 17:41:52 2023, max compression
+gzip compressed data, was "rq-chains-0.1.4.tar", last modified: Wed May 10 17:52:25 2023, max compression
```

## Comparing `rq-chains-0.1.3.tar` & `rq-chains-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 xaled     (1000) xaled     (1000)        0 2023-05-11 09:41:52.911855 rq-chains-0.1.3/
--rw-rw-r--   0 xaled     (1000) xaled     (1000)     1070 2023-05-09 10:10:58.000000 rq-chains-0.1.3/LICENSE
--rw-rw-r--   0 xaled     (1000) xaled     (1000)     5131 2023-05-11 09:41:52.911855 rq-chains-0.1.3/PKG-INFO
--rw-rw-r--   0 xaled     (1000) xaled     (1000)     4665 2023-05-11 09:16:51.000000 rq-chains-0.1.3/README.md
-drwxrwxr-x   0 xaled     (1000) xaled     (1000)        0 2023-05-11 09:41:52.907855 rq-chains-0.1.3/rq_chains/
--rw-rw-r--   0 xaled     (1000) xaled     (1000)       79 2023-05-10 14:47:28.000000 rq-chains-0.1.3/rq_chains/__init__.py
--rw-rw-r--   0 xaled     (1000) xaled     (1000)     2080 2023-05-10 13:48:59.000000 rq-chains-0.1.3/rq_chains/chains_job.py
--rw-rw-r--   0 xaled     (1000) xaled     (1000)    10350 2023-05-11 08:58:20.000000 rq-chains-0.1.3/rq_chains/decorators.py
--rw-rw-r--   0 xaled     (1000) xaled     (1000)      114 2023-05-10 13:38:25.000000 rq-chains-0.1.3/rq_chains/exceptions.py
--rw-rw-r--   0 xaled     (1000) xaled     (1000)      434 2023-05-10 10:31:37.000000 rq-chains-0.1.3/rq_chains/redis_ops.py
--rw-rw-r--   0 xaled     (1000) xaled     (1000)      875 2023-05-11 09:00:14.000000 rq-chains-0.1.3/rq_chains/walk.py
-drwxrwxr-x   0 xaled     (1000) xaled     (1000)        0 2023-05-11 09:41:52.911855 rq-chains-0.1.3/rq_chains.egg-info/
--rw-rw-r--   0 xaled     (1000) xaled     (1000)     5131 2023-05-11 09:41:52.000000 rq-chains-0.1.3/rq_chains.egg-info/PKG-INFO
--rw-rw-r--   0 xaled     (1000) xaled     (1000)      325 2023-05-11 09:41:52.000000 rq-chains-0.1.3/rq_chains.egg-info/SOURCES.txt
--rw-rw-r--   0 xaled     (1000) xaled     (1000)        1 2023-05-11 09:41:52.000000 rq-chains-0.1.3/rq_chains.egg-info/dependency_links.txt
--rw-rw-r--   0 xaled     (1000) xaled     (1000)       24 2023-05-11 09:41:52.000000 rq-chains-0.1.3/rq_chains.egg-info/requires.txt
--rw-rw-r--   0 xaled     (1000) xaled     (1000)       10 2023-05-11 09:41:52.000000 rq-chains-0.1.3/rq_chains.egg-info/top_level.txt
--rw-rw-r--   0 xaled     (1000) xaled     (1000)       38 2023-05-11 09:41:52.911855 rq-chains-0.1.3/setup.cfg
--rw-rw-r--   0 xaled     (1000) xaled     (1000)     1362 2023-05-11 09:41:46.000000 rq-chains-0.1.3/setup.py
+drwxrwxr-x   0 xaled     (1000) xaled     (1000)        0 2023-05-11 09:52:25.265190 rq-chains-0.1.4/
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)     1070 2023-05-09 10:10:58.000000 rq-chains-0.1.4/LICENSE
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)     5268 2023-05-11 09:52:25.265190 rq-chains-0.1.4/PKG-INFO
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)     4665 2023-05-11 09:16:51.000000 rq-chains-0.1.4/README.md
+drwxrwxr-x   0 xaled     (1000) xaled     (1000)        0 2023-05-11 09:52:25.265190 rq-chains-0.1.4/rq_chains/
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)       79 2023-05-10 14:47:28.000000 rq-chains-0.1.4/rq_chains/__init__.py
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)     2080 2023-05-10 13:48:59.000000 rq-chains-0.1.4/rq_chains/chains_job.py
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)    10350 2023-05-11 08:58:20.000000 rq-chains-0.1.4/rq_chains/decorators.py
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)      114 2023-05-10 13:38:25.000000 rq-chains-0.1.4/rq_chains/exceptions.py
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)      434 2023-05-10 10:31:37.000000 rq-chains-0.1.4/rq_chains/redis_ops.py
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)      875 2023-05-11 09:00:14.000000 rq-chains-0.1.4/rq_chains/walk.py
+drwxrwxr-x   0 xaled     (1000) xaled     (1000)        0 2023-05-11 09:52:25.265190 rq-chains-0.1.4/rq_chains.egg-info/
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)     5268 2023-05-11 09:52:25.000000 rq-chains-0.1.4/rq_chains.egg-info/PKG-INFO
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)      325 2023-05-11 09:52:25.000000 rq-chains-0.1.4/rq_chains.egg-info/SOURCES.txt
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)        1 2023-05-11 09:52:25.000000 rq-chains-0.1.4/rq_chains.egg-info/dependency_links.txt
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)       24 2023-05-11 09:52:25.000000 rq-chains-0.1.4/rq_chains.egg-info/requires.txt
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)       10 2023-05-11 09:52:25.000000 rq-chains-0.1.4/rq_chains.egg-info/top_level.txt
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)       38 2023-05-11 09:52:25.265190 rq-chains-0.1.4/setup.cfg
+-rw-rw-r--   0 xaled     (1000) xaled     (1000)     1661 2023-05-11 09:52:19.000000 rq-chains-0.1.4/setup.py
```

### Comparing `rq-chains-0.1.3/LICENSE` & `rq-chains-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rq-chains-0.1.3/PKG-INFO` & `rq-chains-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: rq-chains
-Version: 0.1.3
+Version: 0.1.4
 Summary: RQ Chains is a Python library that extends RQ (Redis Queue) with a publisher-subscriber model for job chains. By Khalid Grandi (github.com/xaled).
 Home-page: https://github.com/xaled/rq-chains
 Author: Khalid Grandi
 Author-email: kh.grandi@gmail.com
-License: UNKNOWN
+License: MIT
 Keywords: library rq redis pubsub
 Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RQ Chains
 RQ Chains is a tiny Python library that extends [RQ (Redis Queue)](https://python-rq.org/) with a publisher-subscriber model for job chains.
 It allows jobs to publish results to channels and other jobs to subscribe to these channels to receive the results.
```

### Comparing `rq-chains-0.1.3/README.md` & `rq-chains-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rq-chains-0.1.3/rq_chains/chains_job.py` & `rq-chains-0.1.4/rq_chains/chains_job.py`

 * *Files identical despite different names*

### Comparing `rq-chains-0.1.3/rq_chains/decorators.py` & `rq-chains-0.1.4/rq_chains/decorators.py`

 * *Files identical despite different names*

### Comparing `rq-chains-0.1.3/rq_chains/walk.py` & `rq-chains-0.1.4/rq_chains/walk.py`

 * *Files identical despite different names*

### Comparing `rq-chains-0.1.3/rq_chains.egg-info/PKG-INFO` & `rq-chains-0.1.4/rq_chains.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: rq-chains
-Version: 0.1.3
+Version: 0.1.4
 Summary: RQ Chains is a Python library that extends RQ (Redis Queue) with a publisher-subscriber model for job chains. By Khalid Grandi (github.com/xaled).
 Home-page: https://github.com/xaled/rq-chains
 Author: Khalid Grandi
 Author-email: kh.grandi@gmail.com
-License: UNKNOWN
+License: MIT
 Keywords: library rq redis pubsub
 Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RQ Chains
 RQ Chains is a tiny Python library that extends [RQ (Redis Queue)](https://python-rq.org/) with a publisher-subscriber model for job chains.
 It allows jobs to publish results to channels and other jobs to subscribe to these channels to receive the results.
```

