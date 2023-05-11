# Comparing `tmp/aio_pika-9.0.5.tar.gz` & `tmp/aio_pika-9.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_pika-9.0.5.tar", max compression
+gzip compressed data, was "aio_pika-9.0.6.tar", max compression
```

## Comparing `aio_pika-9.0.5.tar` & `aio_pika-9.0.6.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     7585 2023-03-12 07:41:28.001278 aio_pika-9.0.5/README.rst
--rw-r--r--   0        0        0     1153 2023-03-12 07:41:28.001423 aio_pika-9.0.5/aio_pika/__init__.py
--rw-r--r--   0        0        0    24562 2023-03-12 07:41:28.001646 aio_pika-9.0.5/aio_pika/abc.py
--rw-r--r--   0        0        0    13901 2023-03-12 07:41:28.001821 aio_pika-9.0.5/aio_pika/channel.py
--rw-r--r--   0        0        0    10881 2023-03-12 07:41:28.001978 aio_pika-9.0.5/aio_pika/connection.py
--rw-r--r--   0        0        0     1304 2023-03-12 07:41:28.002086 aio_pika-9.0.5/aio_pika/exceptions.py
--rw-r--r--   0        0        0     6389 2023-03-12 07:41:28.002233 aio_pika-9.0.5/aio_pika/exchange.py
--rw-r--r--   0        0        0      246 2023-03-12 07:41:28.002323 aio_pika-9.0.5/aio_pika/log.py
--rw-r--r--   0        0        0    19662 2023-03-12 07:41:28.002529 aio_pika-9.0.5/aio_pika/message.py
--rw-r--r--   0        0        0      233 2023-03-12 07:41:28.002694 aio_pika-9.0.5/aio_pika/patterns/__init__.py
--rw-r--r--   0        0        0     1345 2023-03-12 07:41:28.002797 aio_pika-9.0.5/aio_pika/patterns/base.py
--rw-r--r--   0        0        0     6249 2023-03-12 07:41:28.002916 aio_pika-9.0.5/aio_pika/patterns/master.py
--rw-r--r--   0        0        0    14375 2023-03-12 07:41:28.003053 aio_pika-9.0.5/aio_pika/patterns/rpc.py
--rw-r--r--   0        0        0     4352 2023-03-12 07:41:28.003167 aio_pika-9.0.5/aio_pika/pool.py
--rw-r--r--   0        0        0        1 2023-03-12 07:41:28.003264 aio_pika-9.0.5/aio_pika/py.typed
--rw-r--r--   0        0        0    15564 2023-03-12 07:41:28.003391 aio_pika-9.0.5/aio_pika/queue.py
--rw-r--r--   0        0        0     6980 2023-03-12 07:41:28.003514 aio_pika-9.0.5/aio_pika/robust_channel.py
--rw-r--r--   0        0        0    10358 2023-03-12 07:41:28.003629 aio_pika-9.0.5/aio_pika/robust_connection.py
--rw-r--r--   0        0        0     2727 2023-03-12 07:41:28.003768 aio_pika-9.0.5/aio_pika/robust_exchange.py
--rw-r--r--   0        0        0     4656 2023-03-12 07:41:28.003859 aio_pika-9.0.5/aio_pika/robust_queue.py
--rw-r--r--   0        0        0     7339 2023-03-12 07:41:28.004001 aio_pika-9.0.5/aio_pika/tools.py
--rw-r--r--   0        0        0     1924 2023-03-12 07:41:28.004130 aio_pika-9.0.5/aio_pika/transaction.py
--rw-r--r--   0        0        0     3243 2023-03-12 18:39:48.792851 aio_pika-9.0.5/pyproject.toml
--rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aio_pika-9.0.5/setup.py
--rw-r--r--   0        0        0     9488 1970-01-01 00:00:00.000000 aio_pika-9.0.5/PKG-INFO
+-rw-r--r--   0        0        0     7585 2023-02-18 21:11:58.825819 aio_pika-9.0.6/README.rst
+-rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.0.6/aio_pika/__init__.py
+-rw-r--r--   0        0        0    24987 2023-05-10 18:49:42.382788 aio_pika-9.0.6/aio_pika/abc.py
+-rw-r--r--   0        0        0    13901 2023-05-10 18:49:36.231815 aio_pika-9.0.6/aio_pika/channel.py
+-rw-r--r--   0        0        0    10907 2023-05-10 18:49:42.383574 aio_pika-9.0.6/aio_pika/connection.py
+-rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.0.6/aio_pika/exceptions.py
+-rw-r--r--   0        0        0     6411 2023-05-10 18:49:36.233185 aio_pika-9.0.6/aio_pika/exchange.py
+-rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.0.6/aio_pika/log.py
+-rw-r--r--   0        0        0    19662 2023-05-10 18:49:36.233947 aio_pika-9.0.6/aio_pika/message.py
+-rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.0.6/aio_pika/patterns/__init__.py
+-rw-r--r--   0        0        0     1345 2022-04-21 14:39:37.865181 aio_pika-9.0.6/aio_pika/patterns/base.py
+-rw-r--r--   0        0        0     6249 2023-05-10 18:49:36.235400 aio_pika-9.0.6/aio_pika/patterns/master.py
+-rw-r--r--   0        0        0    14375 2023-05-10 18:49:36.237106 aio_pika-9.0.6/aio_pika/patterns/rpc.py
+-rw-r--r--   0        0        0     4352 2023-05-10 18:49:36.238710 aio_pika-9.0.6/aio_pika/pool.py
+-rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.0.6/aio_pika/py.typed
+-rw-r--r--   0        0        0    16056 2023-05-10 18:49:42.384212 aio_pika-9.0.6/aio_pika/queue.py
+-rw-r--r--   0        0        0     6980 2023-05-10 18:49:36.241668 aio_pika-9.0.6/aio_pika/robust_channel.py
+-rw-r--r--   0        0        0    10367 2023-05-10 18:49:42.384956 aio_pika-9.0.6/aio_pika/robust_connection.py
+-rw-r--r--   0        0        0     2727 2023-05-10 18:49:36.243602 aio_pika-9.0.6/aio_pika/robust_exchange.py
+-rw-r--r--   0        0        0     4656 2023-05-10 18:49:36.244515 aio_pika-9.0.6/aio_pika/robust_queue.py
+-rw-r--r--   0        0        0     7339 2023-03-23 15:08:04.837850 aio_pika-9.0.6/aio_pika/tools.py
+-rw-r--r--   0        0        0     1924 2023-05-10 18:49:36.245307 aio_pika-9.0.6/aio_pika/transaction.py
+-rw-r--r--   0        0        0     3243 2023-05-10 19:00:27.186033 aio_pika-9.0.6/pyproject.toml
+-rw-r--r--   0        0        0     9488 1970-01-01 00:00:00.000000 aio_pika-9.0.6/PKG-INFO
```

### Comparing `aio_pika-9.0.5/README.rst` & `aio_pika-9.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/__init__.py` & `aio_pika-9.0.6/aio_pika/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/abc.py` & `aio_pika-9.0.6/aio_pika/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import asyncio
 import dataclasses
+import sys
 from abc import ABC, abstractmethod
 from datetime import datetime, timedelta
 from enum import Enum, IntEnum, unique
 from functools import singledispatch
 from types import TracebackType
 from typing import (
     Any, AsyncContextManager, AsyncIterable, Awaitable, Callable, Dict,
-    Generator, Iterator, Optional, Type, TypeVar, Union,
+    Generator, Iterator, Optional, Type, TypeVar, Union, overload,
 )
 
-
-try:
-    from typing import TypedDict
-except ImportError:
-    from typing_extensions import TypedDict
+if sys.version_info >= (3, 8):
+    from typing import Literal, TypedDict
+else:
+    from typing_extensions import Literal, TypedDict
 
 import aiormq.abc
 from aiormq.abc import ExceptionType
 from pamqp.common import Arguments, FieldValue
 from yarl import URL
 
 from .pool import PoolInstance
@@ -320,14 +320,28 @@
     async def cancel(
         self, consumer_tag: ConsumerTag,
         timeout: TimeoutType = None,
         nowait: bool = False,
     ) -> aiormq.spec.Basic.CancelOk:
         raise NotImplementedError
 
+    @overload
+    async def get(
+        self, *, no_ack: bool = False,
+        fail: Literal[True] = ..., timeout: TimeoutType = ...,
+    ) -> AbstractIncomingMessage:
+        ...
+
+    @overload
+    async def get(
+        self, *, no_ack: bool = False,
+        fail: Literal[False] = ..., timeout: TimeoutType = ...,
+    ) -> Optional[AbstractIncomingMessage]:
+        ...
+
     @abstractmethod
     async def get(
         self, *, no_ack: bool = False,
         fail: bool = True, timeout: TimeoutType = 5,
     ) -> Optional[AbstractIncomingMessage]:
         raise NotImplementedError
```

### Comparing `aio_pika-9.0.5/aio_pika/channel.py` & `aio_pika-9.0.6/aio_pika/channel.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/connection.py` & `aio_pika-9.0.6/aio_pika/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,15 +356,17 @@
             password=password,
             virtualhost=virtualhost,
             ssl=ssl,
             ssl_options=ssl_options,
             client_properties=client_properties,
             **kwargs,
         ),
-        loop=loop, ssl_context=ssl_context,
+        loop=loop,
+        ssl_context=ssl_context,
+        **kwargs,
     )
 
     await connection.connect(timeout=timeout)
     return connection
 
 
 __all__ = ("connect", "Connection", "make_url")
```

### Comparing `aio_pika-9.0.5/aio_pika/exceptions.py` & `aio_pika-9.0.6/aio_pika/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/exchange.py` & `aio_pika-9.0.6/aio_pika/exchange.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,19 +38,19 @@
         self.passive = passive
         self.arguments = arguments or {}
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
-        return "<Exchange(%s): auto_delete=%s, durable=%s, arguments=%r)>" % (
-            self,
-            self.auto_delete,
-            self.durable,
-            self.arguments,
+        return (
+            f"<{self.__class__.__name__}({self}):"
+            f" auto_delete={self.auto_delete},"
+            f" durable={self.durable},"
+            f" arguments={self.arguments!r})>"
         )
 
     async def declare(
         self, timeout: TimeoutType = None,
     ) -> aiormq.spec.Exchange.DeclareOk:
         return await self.channel.exchange_declare(
             self.name,
```

### Comparing `aio_pika-9.0.5/aio_pika/message.py` & `aio_pika-9.0.6/aio_pika/message.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/patterns/base.py` & `aio_pika-9.0.6/aio_pika/patterns/base.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/patterns/master.py` & `aio_pika-9.0.6/aio_pika/patterns/master.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/patterns/rpc.py` & `aio_pika-9.0.6/aio_pika/patterns/rpc.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/pool.py` & `aio_pika-9.0.6/aio_pika/pool.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/queue.py` & `aio_pika-9.0.6/aio_pika/queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
+import sys
 from functools import partial
 from types import TracebackType
-from typing import Any, Callable, Optional, Type
+from typing import Any, Callable, Optional, Type, overload
 
 import aiormq
 from aiormq.abc import DeliveredMessage
 from pamqp.common import Arguments
 
 from .abc import (
     AbstractIncomingMessage, AbstractQueue, AbstractQueueIterator, ConsumerTag,
@@ -14,14 +15,20 @@
 from .exceptions import QueueEmpty
 from .exchange import ExchangeParamType
 from .log import get_logger
 from .message import IncomingMessage
 from .tools import CallbackCollection, create_task
 
 
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
+
 log = get_logger(__name__)
 
 
 async def consumer(
     callback: Callable[[AbstractIncomingMessage], Any],
     msg: DeliveredMessage, *,
     no_ack: bool,
@@ -252,14 +259,28 @@
         :return: Basic.CancelOk when operation completed successfully
         """
 
         return await self.channel.basic_cancel(
             consumer_tag=consumer_tag, nowait=nowait, timeout=timeout,
         )
 
+    @overload
+    async def get(
+        self, *, no_ack: bool = False,
+        fail: Literal[True] = ..., timeout: TimeoutType = ...,
+    ) -> IncomingMessage:
+        ...
+
+    @overload
+    async def get(
+        self, *, no_ack: bool = False,
+        fail: Literal[False] = ..., timeout: TimeoutType = ...,
+    ) -> Optional[IncomingMessage]:
+        ...
+
     async def get(
         self, *, no_ack: bool = False,
         fail: bool = True, timeout: TimeoutType = 5,
     ) -> Optional[IncomingMessage]:
 
         """ Get message from the queue.
```

### Comparing `aio_pika-9.0.5/aio_pika/robust_channel.py` & `aio_pika-9.0.6/aio_pika/robust_channel.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/robust_connection.py` & `aio_pika-9.0.6/aio_pika/robust_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
             password=password,
             virtualhost=virtualhost,
             ssl=ssl,
             ssl_options=ssl_options,
             client_properties=client_properties,
             **kwargs,
         ),
-        loop=loop, ssl_context=ssl_context,
+        loop=loop, ssl_context=ssl_context, **kwargs
     )
 
     await connection.connect(timeout=timeout)
     return connection
 
 
 __all__ = (
```

### Comparing `aio_pika-9.0.5/aio_pika/robust_exchange.py` & `aio_pika-9.0.6/aio_pika/robust_exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/robust_queue.py` & `aio_pika-9.0.6/aio_pika/robust_queue.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/tools.py` & `aio_pika-9.0.6/aio_pika/tools.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/aio_pika/transaction.py` & `aio_pika-9.0.6/aio_pika/transaction.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.0.5/pyproject.toml` & `aio_pika-9.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-pika"
-version = "9.0.5"
+version = "9.0.6"
 description = "Wrapper around the aiormq for asyncio and humans"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.rst"
 license = "Apache-2.0"
 keywords=["rabbitmq", "asyncio", "amqp", "amqp 0.9.1", "aiormq"]
 homepage = "https://github.com/mosquito/aio-pika"
 classifiers = [
```

### Comparing `aio_pika-9.0.5/setup.py` & `aio_pika-9.0.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,336 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aio-pika
+Version: 9.0.6
+Summary: Wrapper around the aiormq for asyncio and humans
+Home-page: https://github.com/mosquito/aio-pika
+License: Apache-2.0
+Keywords: rabbitmq,asyncio,amqp,amqp 0.9.1,aiormq
+Author: Dmitry Orlov
+Author-email: me@mosquito.su
+Requires-Python: >=3.7,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
+Requires-Dist: aiormq (>=6.7.1,<6.8.0)
+Requires-Dist: setuptools ; python_version < "3.8"
+Requires-Dist: typing_extensions ; python_version < "3.8"
+Requires-Dist: yarl
+Project-URL: Documentation, https://aio-pika.readthedocs.org/
+Project-URL: Source, https://github.com/mosquito/aio-pika
+Project-URL: Tracker, https://github.com/mosquito/aio-pika/issues
+Description-Content-Type: text/x-rst
 
-packages = \
-['aio_pika', 'aio_pika.patterns']
+.. _documentation: https://aio-pika.readthedocs.org/
+.. _adopted official RabbitMQ tutorial: https://aio-pika.readthedocs.io/en/latest/rabbitmq-tutorial/1-introduction.html
 
-package_data = \
-{'': ['*']}
+aio-pika
+========
 
-install_requires = \
-['aiormq>=6.7.1,<6.8.0', 'yarl']
-
-extras_require = \
-{':python_version < "3.8"': ['typing_extensions', 'setuptools']}
-
-setup_kwargs = {
-    'name': 'aio-pika',
-    'version': '9.0.5',
-    'description': 'Wrapper around the aiormq for asyncio and humans',
-    'long_description': '.. _documentation: https://aio-pika.readthedocs.org/\n.. _adopted official RabbitMQ tutorial: https://aio-pika.readthedocs.io/en/latest/rabbitmq-tutorial/1-introduction.html\n\naio-pika\n========\n\n.. image:: https://readthedocs.org/projects/aio-pika/badge/?version=latest\n    :target: https://aio-pika.readthedocs.org/\n    :alt: ReadTheDocs\n\n.. image:: https://coveralls.io/repos/github/mosquito/aio-pika/badge.svg?branch=master\n    :target: https://coveralls.io/github/mosquito/aio-pika\n    :alt: Coveralls\n\n.. image:: https://github.com/mosquito/aio-pika/workflows/tests/badge.svg\n    :target: https://github.com/mosquito/aio-pika/actions?query=workflow%3Atests\n    :alt: Github Actions\n\n.. image:: https://img.shields.io/pypi/v/aio-pika.svg\n    :target: https://pypi.python.org/pypi/aio-pika/\n    :alt: Latest Version\n\n.. image:: https://img.shields.io/pypi/wheel/aio-pika.svg\n    :target: https://pypi.python.org/pypi/aio-pika/\n\n.. image:: https://img.shields.io/pypi/pyversions/aio-pika.svg\n    :target: https://pypi.python.org/pypi/aio-pika/\n\n.. image:: https://img.shields.io/pypi/l/aio-pika.svg\n    :target: https://pypi.python.org/pypi/aio-pika/\n\n\nA wrapper around `aiormq`_ for asyncio and humans.\n\nCheck out the examples and the tutorial in the `documentation`_.\n\nIf you are a newcomer to RabbitMQ, please start with the `adopted official RabbitMQ tutorial`_.\n\n.. _aiormq: http://github.com/mosquito/aiormq/\n\n.. note::\n   Since version ``5.0.0`` this library doesn\'t use ``pika`` as AMQP connector.\n   Versions below ``5.0.0`` contains or requires ``pika``\'s source code.\n\n.. note::\n   The version 7.0.0 has breaking API changes, see CHANGELOG.md\n   for migration hints.\n\n\nFeatures\n--------\n\n* Completely asynchronous API.\n* Object oriented API.\n* Transparent auto-reconnects with complete state recovery with `connect_robust`\n  (e.g. declared queues or exchanges, consuming state and bindings).\n* Python 3.7+ compatible.\n* For python 3.5 users available `aio-pika<7`\n* Transparent `publisher confirms`_ support\n* `Transactions`_ support\n* Completely type-hints coverage.\n\n\n.. _Transactions: https://www.rabbitmq.com/semantics.html\n.. _publisher confirms: https://www.rabbitmq.com/confirms.html\n\n\nInstallation\n------------\n\n.. code-block:: shell\n\n    pip install aio-pika\n\n\nUsage example\n-------------\n\nSimple consumer:\n\n.. code-block:: python\n\n    import asyncio\n    import aio_pika\n    import aio_pika.abc\n\n\n    async def main(loop):\n        # Connect with the givien parameters is also valiable.\n        # aio_pika.connect_robust(host="host", login="login", password="password")\n        # You can only choose one option to create a connection, url or kw-based params.\n        connection = await aio_pika.connect_robust(\n            "amqp://guest:guest@127.0.0.1/", loop=loop\n        )\n\n        async with connection:\n            queue_name = "test_queue"\n\n            # Creating channel\n            channel: aio_pika.abc.AbstractChannel = await connection.channel()\n\n            # Declaring queue\n            queue: aio_pika.abc.AbstractQueue = await channel.declare_queue(\n                queue_name,\n                auto_delete=True\n            )\n\n            async with queue.iterator() as queue_iter:\n                # Cancel consuming after __aexit__\n                async for message in queue_iter:\n                    async with message.process():\n                        print(message.body)\n\n                        if queue.name in message.body.decode():\n                            break\n\n\n    if __name__ == "__main__":\n        loop = asyncio.get_event_loop()\n        loop.run_until_complete(main(loop))\n        loop.close()\n\nSimple publisher:\n\n.. code-block:: python\n\n    import asyncio\n    import aio_pika\n    import aio_pika.abc\n\n\n    async def main(loop):\n        # Explicit type annotation\n        connection: aio_pika.RobustConnection = await aio_pika.connect_robust(\n            "amqp://guest:guest@127.0.0.1/", loop=loop\n        )\n\n        routing_key = "test_queue"\n\n        channel: aio_pika.abc.AbstractChannel = await connection.channel()\n\n        await channel.default_exchange.publish(\n            aio_pika.Message(\n                body=\'Hello {}\'.format(routing_key).encode()\n            ),\n            routing_key=routing_key\n        )\n\n        await connection.close()\n\n\n    if __name__ == "__main__":\n        loop = asyncio.get_event_loop()\n        loop.run_until_complete(main(loop))\n        loop.close()\n\n\nGet single message example:\n\n.. code-block:: python\n\n    import asyncio\n    from aio_pika import connect_robust, Message\n\n\n    async def main(loop):\n        connection = await connect_robust(\n            "amqp://guest:guest@127.0.0.1/",\n            loop=loop\n        )\n\n        queue_name = "test_queue"\n        routing_key = "test_queue"\n\n        # Creating channel\n        channel = await connection.channel()\n\n        # Declaring exchange\n        exchange = await channel.declare_exchange(\'direct\', auto_delete=True)\n\n        # Declaring queue\n        queue = await channel.declare_queue(queue_name, auto_delete=True)\n\n        # Binding queue\n        await queue.bind(exchange, routing_key)\n\n        await exchange.publish(\n            Message(\n                bytes(\'Hello\', \'utf-8\'),\n                content_type=\'text/plain\',\n                headers={\'foo\': \'bar\'}\n            ),\n            routing_key\n        )\n\n        # Receiving message\n        incoming_message = await queue.get(timeout=5)\n\n        # Confirm message\n        await incoming_message.ack()\n\n        await queue.unbind(exchange, routing_key)\n        await queue.delete()\n        await connection.close()\n\n\n    if __name__ == "__main__":\n        loop = asyncio.get_event_loop()\n        loop.run_until_complete(main(loop))\n\n\nThere are more examples and the RabbitMQ tutorial in the `documentation`_.\n\n\nVersioning\n==========\n\nThis software follows `Semantic Versioning`_\n\n\nFor contributors\n----------------\n\nSetting up development environment\n__________________________________\n\nClone the project:\n\n.. code-block:: shell\n\n    git clone https://github.com/mosquito/aio-pika.git\n    cd aio-pika\n\nCreate a new virtualenv for `aio-pika`_:\n\n.. code-block:: shell\n\n    python3 -m venv env\n    source env/bin/activate\n\nInstall all requirements for `aio-pika`_:\n\n.. code-block:: shell\n\n    pip install -e \'.[develop]\'\n\n\nRunning Tests\n_____________\n\n**NOTE: In order to run the tests locally you need to run a RabbitMQ instance with default user/password (guest/guest) and port (5672).**\n\n* ProTip: Use Docker for this:\n\n.. code-block:: bash\n\n    docker run -d -p 5671:5671 -p 5672:5672 -p 15671:15671 -p 15672:15672 mosquito/aiormq-rabbitmq\n\nTo test just run:\n\n.. code-block:: bash\n\n    make test\n\n\nEditing Documentation\n_____________________\n\nTo iterate quickly on the documentation live in your browser, try:\n\n.. code-block:: bash\n\n    nox -s docs -- serve\n\nCreating Pull Requests\n______________________\n\nPlease feel free to create pull requests, but you should describe your use cases and add some examples.\n\nChanges should follow a few simple rules:\n\n* When your changes break the public API, you must increase the major version.\n* When your changes are safe for public API (e.g. added an argument with default value)\n* You have to add test cases (see `tests/` folder)\n* You must add docstrings\n* Feel free to add yourself to `"thank\'s to" section`_\n\n\n.. _"thank\'s to" section: https://github.com/mosquito/aio-pika/blob/master/docs/source/index.rst#thanks-for-contributing\n.. _Semantic Versioning: http://semver.org/\n.. _aio-pika: https://github.com/mosquito/aio-pika/\n',
-    'author': 'Dmitry Orlov',
-    'author_email': 'me@mosquito.su',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/mosquito/aio-pika',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+.. image:: https://readthedocs.org/projects/aio-pika/badge/?version=latest
+    :target: https://aio-pika.readthedocs.org/
+    :alt: ReadTheDocs
 
+.. image:: https://coveralls.io/repos/github/mosquito/aio-pika/badge.svg?branch=master
+    :target: https://coveralls.io/github/mosquito/aio-pika
+    :alt: Coveralls
+
+.. image:: https://github.com/mosquito/aio-pika/workflows/tests/badge.svg
+    :target: https://github.com/mosquito/aio-pika/actions?query=workflow%3Atests
+    :alt: Github Actions
+
+.. image:: https://img.shields.io/pypi/v/aio-pika.svg
+    :target: https://pypi.python.org/pypi/aio-pika/
+    :alt: Latest Version
+
+.. image:: https://img.shields.io/pypi/wheel/aio-pika.svg
+    :target: https://pypi.python.org/pypi/aio-pika/
+
+.. image:: https://img.shields.io/pypi/pyversions/aio-pika.svg
+    :target: https://pypi.python.org/pypi/aio-pika/
+
+.. image:: https://img.shields.io/pypi/l/aio-pika.svg
+    :target: https://pypi.python.org/pypi/aio-pika/
+
+
+A wrapper around `aiormq`_ for asyncio and humans.
+
+Check out the examples and the tutorial in the `documentation`_.
+
+If you are a newcomer to RabbitMQ, please start with the `adopted official RabbitMQ tutorial`_.
+
+.. _aiormq: http://github.com/mosquito/aiormq/
+
+.. note::
+   Since version ``5.0.0`` this library doesn't use ``pika`` as AMQP connector.
+   Versions below ``5.0.0`` contains or requires ``pika``'s source code.
+
+.. note::
+   The version 7.0.0 has breaking API changes, see CHANGELOG.md
+   for migration hints.
+
+
+Features
+--------
+
+* Completely asynchronous API.
+* Object oriented API.
+* Transparent auto-reconnects with complete state recovery with `connect_robust`
+  (e.g. declared queues or exchanges, consuming state and bindings).
+* Python 3.7+ compatible.
+* For python 3.5 users available `aio-pika<7`
+* Transparent `publisher confirms`_ support
+* `Transactions`_ support
+* Completely type-hints coverage.
+
+
+.. _Transactions: https://www.rabbitmq.com/semantics.html
+.. _publisher confirms: https://www.rabbitmq.com/confirms.html
+
+
+Installation
+------------
+
+.. code-block:: shell
+
+    pip install aio-pika
+
+
+Usage example
+-------------
+
+Simple consumer:
+
+.. code-block:: python
+
+    import asyncio
+    import aio_pika
+    import aio_pika.abc
+
+
+    async def main(loop):
+        # Connect with the givien parameters is also valiable.
+        # aio_pika.connect_robust(host="host", login="login", password="password")
+        # You can only choose one option to create a connection, url or kw-based params.
+        connection = await aio_pika.connect_robust(
+            "amqp://guest:guest@127.0.0.1/", loop=loop
+        )
+
+        async with connection:
+            queue_name = "test_queue"
+
+            # Creating channel
+            channel: aio_pika.abc.AbstractChannel = await connection.channel()
+
+            # Declaring queue
+            queue: aio_pika.abc.AbstractQueue = await channel.declare_queue(
+                queue_name,
+                auto_delete=True
+            )
+
+            async with queue.iterator() as queue_iter:
+                # Cancel consuming after __aexit__
+                async for message in queue_iter:
+                    async with message.process():
+                        print(message.body)
+
+                        if queue.name in message.body.decode():
+                            break
+
+
+    if __name__ == "__main__":
+        loop = asyncio.get_event_loop()
+        loop.run_until_complete(main(loop))
+        loop.close()
+
+Simple publisher:
+
+.. code-block:: python
+
+    import asyncio
+    import aio_pika
+    import aio_pika.abc
+
+
+    async def main(loop):
+        # Explicit type annotation
+        connection: aio_pika.RobustConnection = await aio_pika.connect_robust(
+            "amqp://guest:guest@127.0.0.1/", loop=loop
+        )
+
+        routing_key = "test_queue"
+
+        channel: aio_pika.abc.AbstractChannel = await connection.channel()
+
+        await channel.default_exchange.publish(
+            aio_pika.Message(
+                body='Hello {}'.format(routing_key).encode()
+            ),
+            routing_key=routing_key
+        )
+
+        await connection.close()
+
+
+    if __name__ == "__main__":
+        loop = asyncio.get_event_loop()
+        loop.run_until_complete(main(loop))
+        loop.close()
+
+
+Get single message example:
+
+.. code-block:: python
+
+    import asyncio
+    from aio_pika import connect_robust, Message
+
+
+    async def main(loop):
+        connection = await connect_robust(
+            "amqp://guest:guest@127.0.0.1/",
+            loop=loop
+        )
+
+        queue_name = "test_queue"
+        routing_key = "test_queue"
+
+        # Creating channel
+        channel = await connection.channel()
+
+        # Declaring exchange
+        exchange = await channel.declare_exchange('direct', auto_delete=True)
+
+        # Declaring queue
+        queue = await channel.declare_queue(queue_name, auto_delete=True)
+
+        # Binding queue
+        await queue.bind(exchange, routing_key)
+
+        await exchange.publish(
+            Message(
+                bytes('Hello', 'utf-8'),
+                content_type='text/plain',
+                headers={'foo': 'bar'}
+            ),
+            routing_key
+        )
+
+        # Receiving message
+        incoming_message = await queue.get(timeout=5)
+
+        # Confirm message
+        await incoming_message.ack()
+
+        await queue.unbind(exchange, routing_key)
+        await queue.delete()
+        await connection.close()
+
+
+    if __name__ == "__main__":
+        loop = asyncio.get_event_loop()
+        loop.run_until_complete(main(loop))
+
+
+There are more examples and the RabbitMQ tutorial in the `documentation`_.
+
+
+Versioning
+==========
+
+This software follows `Semantic Versioning`_
+
+
+For contributors
+----------------
+
+Setting up development environment
+__________________________________
+
+Clone the project:
+
+.. code-block:: shell
+
+    git clone https://github.com/mosquito/aio-pika.git
+    cd aio-pika
+
+Create a new virtualenv for `aio-pika`_:
+
+.. code-block:: shell
+
+    python3 -m venv env
+    source env/bin/activate
+
+Install all requirements for `aio-pika`_:
+
+.. code-block:: shell
+
+    pip install -e '.[develop]'
+
+
+Running Tests
+_____________
+
+**NOTE: In order to run the tests locally you need to run a RabbitMQ instance with default user/password (guest/guest) and port (5672).**
+
+* ProTip: Use Docker for this:
+
+.. code-block:: bash
+
+    docker run -d -p 5671:5671 -p 5672:5672 -p 15671:15671 -p 15672:15672 mosquito/aiormq-rabbitmq
+
+To test just run:
+
+.. code-block:: bash
+
+    make test
+
+
+Editing Documentation
+_____________________
+
+To iterate quickly on the documentation live in your browser, try:
+
+.. code-block:: bash
+
+    nox -s docs -- serve
+
+Creating Pull Requests
+______________________
+
+Please feel free to create pull requests, but you should describe your use cases and add some examples.
+
+Changes should follow a few simple rules:
+
+* When your changes break the public API, you must increase the major version.
+* When your changes are safe for public API (e.g. added an argument with default value)
+* You have to add test cases (see `tests/` folder)
+* You must add docstrings
+* Feel free to add yourself to `"thank's to" section`_
+
+
+.. _"thank's to" section: https://github.com/mosquito/aio-pika/blob/master/docs/source/index.rst#thanks-for-contributing
+.. _Semantic Versioning: http://semver.org/
+.. _aio-pika: https://github.com/mosquito/aio-pika/
 
-setup(**setup_kwargs)
```

