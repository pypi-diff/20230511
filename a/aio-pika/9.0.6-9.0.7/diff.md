# Comparing `tmp/aio_pika-9.0.6.tar.gz` & `tmp/aio_pika-9.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_pika-9.0.6.tar", max compression
+gzip compressed data, was "aio_pika-9.0.7.tar", max compression
```

## Comparing `aio_pika-9.0.6.tar` & `aio_pika-9.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     7585 2023-02-18 21:11:58.825819 aio_pika-9.0.6/README.rst
--rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.0.6/aio_pika/__init__.py
--rw-r--r--   0        0        0    24987 2023-05-10 18:49:42.382788 aio_pika-9.0.6/aio_pika/abc.py
--rw-r--r--   0        0        0    13901 2023-05-10 18:49:36.231815 aio_pika-9.0.6/aio_pika/channel.py
--rw-r--r--   0        0        0    10907 2023-05-10 18:49:42.383574 aio_pika-9.0.6/aio_pika/connection.py
--rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.0.6/aio_pika/exceptions.py
--rw-r--r--   0        0        0     6411 2023-05-10 18:49:36.233185 aio_pika-9.0.6/aio_pika/exchange.py
--rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.0.6/aio_pika/log.py
--rw-r--r--   0        0        0    19662 2023-05-10 18:49:36.233947 aio_pika-9.0.6/aio_pika/message.py
--rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.0.6/aio_pika/patterns/__init__.py
--rw-r--r--   0        0        0     1345 2022-04-21 14:39:37.865181 aio_pika-9.0.6/aio_pika/patterns/base.py
--rw-r--r--   0        0        0     6249 2023-05-10 18:49:36.235400 aio_pika-9.0.6/aio_pika/patterns/master.py
--rw-r--r--   0        0        0    14375 2023-05-10 18:49:36.237106 aio_pika-9.0.6/aio_pika/patterns/rpc.py
--rw-r--r--   0        0        0     4352 2023-05-10 18:49:36.238710 aio_pika-9.0.6/aio_pika/pool.py
--rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.0.6/aio_pika/py.typed
--rw-r--r--   0        0        0    16056 2023-05-10 18:49:42.384212 aio_pika-9.0.6/aio_pika/queue.py
--rw-r--r--   0        0        0     6980 2023-05-10 18:49:36.241668 aio_pika-9.0.6/aio_pika/robust_channel.py
--rw-r--r--   0        0        0    10367 2023-05-10 18:49:42.384956 aio_pika-9.0.6/aio_pika/robust_connection.py
--rw-r--r--   0        0        0     2727 2023-05-10 18:49:36.243602 aio_pika-9.0.6/aio_pika/robust_exchange.py
--rw-r--r--   0        0        0     4656 2023-05-10 18:49:36.244515 aio_pika-9.0.6/aio_pika/robust_queue.py
--rw-r--r--   0        0        0     7339 2023-03-23 15:08:04.837850 aio_pika-9.0.6/aio_pika/tools.py
--rw-r--r--   0        0        0     1924 2023-05-10 18:49:36.245307 aio_pika-9.0.6/aio_pika/transaction.py
--rw-r--r--   0        0        0     3243 2023-05-10 19:00:27.186033 aio_pika-9.0.6/pyproject.toml
--rw-r--r--   0        0        0     9488 1970-01-01 00:00:00.000000 aio_pika-9.0.6/PKG-INFO
+-rw-r--r--   0        0        0     7585 2023-02-18 21:11:58.825819 aio_pika-9.0.7/README.rst
+-rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.0.7/aio_pika/__init__.py
+-rw-r--r--   0        0        0    24987 2023-05-11 12:01:38.489759 aio_pika-9.0.7/aio_pika/abc.py
+-rw-r--r--   0        0        0    13901 2023-05-11 12:01:38.490719 aio_pika-9.0.7/aio_pika/channel.py
+-rw-r--r--   0        0        0    10907 2023-05-11 12:01:38.491492 aio_pika-9.0.7/aio_pika/connection.py
+-rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.0.7/aio_pika/exceptions.py
+-rw-r--r--   0        0        0     6411 2023-05-11 12:01:38.493435 aio_pika-9.0.7/aio_pika/exchange.py
+-rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.0.7/aio_pika/log.py
+-rw-r--r--   0        0        0    19662 2023-05-11 12:01:38.494544 aio_pika-9.0.7/aio_pika/message.py
+-rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.0.7/aio_pika/patterns/__init__.py
+-rw-r--r--   0        0        0     1345 2023-05-11 12:01:38.495119 aio_pika-9.0.7/aio_pika/patterns/base.py
+-rw-r--r--   0        0        0     6249 2023-05-11 12:01:38.495943 aio_pika-9.0.7/aio_pika/patterns/master.py
+-rw-r--r--   0        0        0    14375 2023-05-11 12:01:38.496979 aio_pika-9.0.7/aio_pika/patterns/rpc.py
+-rw-r--r--   0        0        0     4352 2023-05-11 12:01:38.497963 aio_pika-9.0.7/aio_pika/pool.py
+-rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.0.7/aio_pika/py.typed
+-rw-r--r--   0        0        0    16056 2023-05-11 12:01:38.499489 aio_pika-9.0.7/aio_pika/queue.py
+-rw-r--r--   0        0        0     6980 2023-05-11 12:01:38.502999 aio_pika-9.0.7/aio_pika/robust_channel.py
+-rw-r--r--   0        0        0    10367 2023-05-11 12:01:38.505100 aio_pika-9.0.7/aio_pika/robust_connection.py
+-rw-r--r--   0        0        0     2727 2023-05-11 12:01:38.505793 aio_pika-9.0.7/aio_pika/robust_exchange.py
+-rw-r--r--   0        0        0     4656 2023-05-11 12:01:38.506997 aio_pika-9.0.7/aio_pika/robust_queue.py
+-rw-r--r--   0        0        0     7339 2023-05-11 12:01:38.508241 aio_pika-9.0.7/aio_pika/tools.py
+-rw-r--r--   0        0        0     1924 2023-05-11 12:01:38.509992 aio_pika-9.0.7/aio_pika/transaction.py
+-rw-r--r--   0        0        0     3264 2023-05-11 15:25:23.113063 aio_pika-9.0.7/pyproject.toml
+-rw-r--r--   0        0        0     9488 1970-01-01 00:00:00.000000 aio_pika-9.0.7/PKG-INFO
```

### Comparing `aio_pika-9.0.6/README.rst` & `aio_pika-9.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/__init__.py` & `aio_pika-9.0.7/aio_pika/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/abc.py` & `aio_pika-9.0.7/aio_pika/abc.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/channel.py` & `aio_pika-9.0.7/aio_pika/channel.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/connection.py` & `aio_pika-9.0.7/aio_pika/connection.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/exceptions.py` & `aio_pika-9.0.7/aio_pika/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/exchange.py` & `aio_pika-9.0.7/aio_pika/exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/message.py` & `aio_pika-9.0.7/aio_pika/message.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/patterns/base.py` & `aio_pika-9.0.7/aio_pika/patterns/base.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/patterns/master.py` & `aio_pika-9.0.7/aio_pika/patterns/master.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/patterns/rpc.py` & `aio_pika-9.0.7/aio_pika/patterns/rpc.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/pool.py` & `aio_pika-9.0.7/aio_pika/pool.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/queue.py` & `aio_pika-9.0.7/aio_pika/queue.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/robust_channel.py` & `aio_pika-9.0.7/aio_pika/robust_channel.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/robust_connection.py` & `aio_pika-9.0.7/aio_pika/robust_connection.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/robust_exchange.py` & `aio_pika-9.0.7/aio_pika/robust_exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/robust_queue.py` & `aio_pika-9.0.7/aio_pika/robust_queue.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/tools.py` & `aio_pika-9.0.7/aio_pika/tools.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/aio_pika/transaction.py` & `aio_pika-9.0.7/aio_pika/transaction.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.6/pyproject.toml` & `aio_pika-9.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-pika"
-version = "9.0.6"
+version = "9.0.7"
 description = "Wrapper around the aiormq for asyncio and humans"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.rst"
 license = "Apache-2.0"
 keywords=["rabbitmq", "asyncio", "amqp", "amqp 0.9.1", "aiormq"]
 homepage = "https://github.com/mosquito/aio-pika"
 classifiers = [
@@ -33,22 +33,23 @@
 [tool.poetry.urls]
 "Source" = "https://github.com/mosquito/aio-pika"
 "Tracker" = "https://github.com/mosquito/aio-pika/issues"
 "Documentation" = "https://aio-pika.readthedocs.org/"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-aiormq = "~6.7.1"
+aiormq = "~6.7.5"
 yarl = [{ version = '*'}]
 typing_extensions = [{ version = '*', python = "< 3.8" }]
 # for pkg_resources
 setuptools = [{ version = '*', python = "< 3.8" }]
 
 [tool.poetry.group.dev.dependencies]
-aiomisc = "^16.2"
+aiomisc = "^17.2"
+aiomisc-pytest = "*"
 collective-checkdocs = "^0.2"
 coverage = "^6.5.0"
 coveralls = "^3.3.1"
 mypy = "^0.991"
 nox = "^2022.11.21"
 pylama = "^8.4.1"
 pytest = "^7.2.0"
```

### Comparing `aio_pika-9.0.6/PKG-INFO` & `aio_pika-9.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-pika
-Version: 9.0.6
+Version: 9.0.7
 Summary: Wrapper around the aiormq for asyncio and humans
 Home-page: https://github.com/mosquito/aio-pika
 License: Apache-2.0
 Keywords: rabbitmq,asyncio,amqp,amqp 0.9.1,aiormq
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
@@ -29,15 +29,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Dist: aiormq (>=6.7.1,<6.8.0)
+Requires-Dist: aiormq (>=6.7.5,<6.8.0)
 Requires-Dist: setuptools ; python_version < "3.8"
 Requires-Dist: typing_extensions ; python_version < "3.8"
 Requires-Dist: yarl
 Project-URL: Documentation, https://aio-pika.readthedocs.org/
 Project-URL: Source, https://github.com/mosquito/aio-pika
 Project-URL: Tracker, https://github.com/mosquito/aio-pika/issues
 Description-Content-Type: text/x-rst
```

