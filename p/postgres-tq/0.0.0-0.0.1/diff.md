# Comparing `tmp/postgres-tq-0.0.0.tar.gz` & `tmp/postgres-tq-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgres-tq-0.0.0.tar", last modified: Thu May 11 14:56:40 2023, max compression
+gzip compressed data, was "postgres-tq-0.0.1.tar", last modified: Thu May 11 16:00:24 2023, max compression
```

## Comparing `postgres-tq-0.0.0.tar` & `postgres-tq-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-05-11 14:56:40.899875 postgres-tq-0.0.0/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     4676 2023-05-11 14:56:40.899875 postgres-tq-0.0.0/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)     4460 2023-05-11 14:53:49.000000 postgres-tq-0.0.0/README.md
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-05-11 14:56:40.899875 postgres-tq-0.0.0/postgres_tq.egg-info/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     4676 2023-05-11 14:56:40.000000 postgres-tq-0.0.0/postgres_tq.egg-info/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)      271 2023-05-11 14:56:40.000000 postgres-tq-0.0.0/postgres_tq.egg-info/SOURCES.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)        1 2023-05-11 14:56:40.000000 postgres-tq-0.0.0/postgres_tq.egg-info/dependency_links.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       23 2023-05-11 14:56:40.000000 postgres-tq-0.0.0/postgres_tq.egg-info/requires.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       11 2023-05-11 14:56:40.000000 postgres-tq-0.0.0/postgres_tq.egg-info/top_level.txt
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-05-11 14:56:40.899875 postgres-tq-0.0.0/postgrestq/
--rw-r--r--   0 venthur   (1000) venthur   (1000)       50 2023-05-11 14:53:49.000000 postgres-tq-0.0.0/postgrestq/__init__.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)    16061 2023-05-11 14:53:49.000000 postgres-tq-0.0.0/postgrestq/task_queue.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)      708 2023-05-11 14:53:49.000000 postgres-tq-0.0.0/pyproject.toml
--rw-r--r--   0 venthur   (1000) venthur   (1000)       38 2023-05-11 14:56:40.899875 postgres-tq-0.0.0/setup.cfg
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-05-11 14:56:40.899875 postgres-tq-0.0.0/tests/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     7545 2023-05-11 14:53:49.000000 postgres-tq-0.0.0/tests/test_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:24.033214 postgres-tq-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-11 16:00:24.033214 postgres-tq-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-11 16:00:06.000000 postgres-tq-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:24.033214 postgres-tq-0.0.1/postgres_tq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-11 16:00:24.000000 postgres-tq-0.0.1/postgres_tq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-11 16:00:24.000000 postgres-tq-0.0.1/postgres_tq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:00:24.000000 postgres-tq-0.0.1/postgres_tq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 16:00:24.000000 postgres-tq-0.0.1/postgres_tq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 16:00:24.000000 postgres-tq-0.0.1/postgres_tq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:24.033214 postgres-tq-0.0.1/postgrestq/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 16:00:06.000000 postgres-tq-0.0.1/postgrestq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16061 2023-05-11 16:00:06.000000 postgres-tq-0.0.1/postgrestq/task_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-11 16:00:06.000000 postgres-tq-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:00:24.033214 postgres-tq-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:24.033214 postgres-tq-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-05-11 16:00:06.000000 postgres-tq-0.0.1/tests/test_task_queue.py
```

### Comparing `postgres-tq-0.0.0/PKG-INFO` & `postgres-tq-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgres-tq
-Version: 0.0.0
+Version: 0.0.1
 Summary: Postgres Based Task Queue
 Author-email: FlixTech <open-source@flixbus.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Postgres Task queue
```

### Comparing `postgres-tq-0.0.0/README.md` & `postgres-tq-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `postgres-tq-0.0.0/postgres_tq.egg-info/PKG-INFO` & `postgres-tq-0.0.1/postgres_tq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgres-tq
-Version: 0.0.0
+Version: 0.0.1
 Summary: Postgres Based Task Queue
 Author-email: FlixTech <open-source@flixbus.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Postgres Task queue
```

### Comparing `postgres-tq-0.0.0/postgrestq/task_queue.py` & `postgres-tq-0.0.1/postgrestq/task_queue.py`

 * *Files identical despite different names*

### Comparing `postgres-tq-0.0.0/pyproject.toml` & `postgres-tq-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 
 [project]
 name = "postgres-tq"
-version = "0.0.0"
+version = "0.0.1"
 description = "Postgres Based Task Queue"
 authors = [
     {name = "FlixTech", email = "open-source@flixbus.com"},
 ]
 dependencies = [
     "psycopg[binary]>=3.1.8",
 ]
```

### Comparing `postgres-tq-0.0.0/tests/test_task_queue.py` & `postgres-tq-0.0.1/tests/test_task_queue.py`

 * *Files identical despite different names*

