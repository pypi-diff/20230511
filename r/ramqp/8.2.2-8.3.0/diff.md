# Comparing `tmp/ramqp-8.2.2.tar.gz` & `tmp/ramqp-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramqp-8.2.2.tar", max compression
+gzip compressed data, was "ramqp-8.3.0.tar", max compression
```

## Comparing `ramqp-8.2.2.tar` & `ramqp-8.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0        0        0        0 2023-05-09 10:47:02.065215 ramqp-8.2.2/LICENSES/
--rw-r--r--   0        0        0    15177 2023-05-09 10:47:02.065215 ramqp-8.2.2/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     7466 2023-05-09 10:47:02.066215 ramqp-8.2.2/README.md
--rw-r--r--   0        0        0     1460 2023-05-09 10:47:23.495078 ramqp-8.2.2/pyproject.toml
--rw-r--r--   0        0        0      321 2023-05-09 10:47:02.068215 ramqp-8.2.2/ramqp/__init__.py
--rw-r--r--   0        0        0    13047 2023-05-09 10:47:02.068215 ramqp-8.2.2/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2023-05-09 10:47:02.068215 ramqp-8.2.2/ramqp/amqp.py
--rw-r--r--   0        0        0     2729 2023-05-09 10:47:02.068215 ramqp-8.2.2/ramqp/config.py
--rw-r--r--   0        0        0     8841 2023-05-09 10:47:02.069216 ramqp-8.2.2/ramqp/depends.py
--rw-r--r--   0        0        0     7010 2023-05-09 10:47:02.069216 ramqp-8.2.2/ramqp/metrics.py
--rw-r--r--   0        0        0     8537 2023-05-09 10:47:02.069216 ramqp-8.2.2/ramqp/mo.py
--rw-r--r--   0        0        0        0 2023-05-09 10:47:02.241230 ramqp-8.2.2/ramqp/py.typed
--rw-r--r--   0        0        0     1367 2023-05-09 10:47:02.070216 ramqp-8.2.2/ramqp/utils.py
--rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.2.2/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-05-11 16:14:06.799131 ramqp-8.3.0/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-05-11 16:14:06.799131 ramqp-8.3.0/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     7466 2023-05-11 16:14:06.799131 ramqp-8.3.0/README.md
+-rw-r--r--   0        0        0     1460 2023-05-11 16:14:18.530346 ramqp-8.3.0/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-05-11 16:14:06.801132 ramqp-8.3.0/ramqp/__init__.py
+-rw-r--r--   0        0        0    13047 2023-05-11 16:14:06.801132 ramqp-8.3.0/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2023-05-11 16:14:06.801132 ramqp-8.3.0/ramqp/amqp.py
+-rw-r--r--   0        0        0     2729 2023-05-11 16:14:06.802132 ramqp-8.3.0/ramqp/config.py
+-rw-r--r--   0        0        0    10021 2023-05-11 16:14:06.802132 ramqp-8.3.0/ramqp/depends.py
+-rw-r--r--   0        0        0     7010 2023-05-11 16:14:06.802132 ramqp-8.3.0/ramqp/metrics.py
+-rw-r--r--   0        0        0     8537 2023-05-11 16:14:06.802132 ramqp-8.3.0/ramqp/mo.py
+-rw-r--r--   0        0        0        0 2023-05-11 16:14:06.843136 ramqp-8.3.0/ramqp/py.typed
+-rw-r--r--   0        0        0     1367 2023-05-11 16:14:06.802132 ramqp-8.3.0/ramqp/utils.py
+-rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.3.0/PKG-INFO
```

### Comparing `ramqp-8.2.2/LICENSES/MPL-2.0.txt` & `ramqp-8.3.0/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.2/README.md` & `ramqp-8.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.2/pyproject.toml` & `ramqp-8.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ramqp"
-version = "8.2.2"
+version = "8.3.0"
 description = "Rammearkitektur AMQP library (aio_pika wrapper)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ramqp"
 keywords = ["os2mo", "amqp"]
```

### Comparing `ramqp-8.2.2/ramqp/abstract.py` & `ramqp-8.3.0/ramqp/abstract.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.2/ramqp/amqp.py` & `ramqp-8.3.0/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.2/ramqp/config.py` & `ramqp-8.3.0/ramqp/config.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.2/ramqp/depends.py` & `ramqp-8.3.0/ramqp/depends.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 """This module implement FastAPI dependency injection for RAMQP."""
 import asyncio
 from collections import defaultdict
 from collections.abc import AsyncGenerator
+from collections.abc import Awaitable
 from collections.abc import Callable
 from collections.abc import Hashable
+from contextlib import asynccontextmanager
 from contextlib import AsyncExitStack
 from functools import wraps
 from typing import Annotated
 from typing import Any
 from typing import cast
 from typing import DefaultDict
 from typing import TypeVar
@@ -246,14 +248,50 @@
                 # asynchronous instead of truly concurrent.
                 if not lock.statistics().tasks_waiting:
                     del locks[key_value]
 
     return wrapper
 
 
+def handle_exclusively_decorator(key: Callable[..., Hashable]) -> Callable:
+    """Avoids race conditions in handlers by ensuring exclusivity based on key.
+
+    Basic wrapper for handle_exclusively, allowing it to work as a function decorator.
+
+    Examples:
+        Simple usage::
+
+            @handle_exclusively_decorator(key=lambda x, y, z: x, y)
+            async def f(x, y, z):
+                pass
+
+            await f(x=1, y=2, z=8)
+            await f(x=3, y=4, z=8)  # accepted
+
+    Args:
+        key: A custom key function returning the arguments considered when determining
+            exclusivity.
+
+    Returns:
+        Decorator to be applied to callback functions.
+    """
+
+    exclusive_context_manager = asynccontextmanager(handle_exclusively(key=key))
+
+    def wrapper(coro: Callable[..., Awaitable[T]]) -> Callable[..., Awaitable[T]]:
+        @wraps(coro)
+        async def wrapped(*args: Any, **kwargs: Any) -> T:
+            async with exclusive_context_manager(*args, **kwargs):
+                return await coro(*args, **kwargs)
+
+        return wrapped
+
+    return wrapper
+
+
 def sleep_on_error(delay: int = 30) -> Callable[[], AsyncGenerator[None, None]]:
     """Construct an pseudo-context manager which delays returning on errors.
 
     This is used to prevent race-conditions on writes to MO/LoRa, when the upload times
     out initially but is completed by the backend afterwards. The sleep ensures that
     the AMQP message is not retried immediately, causing the handler to act on
     information which could become stale by the queued write. This happens because the
```

### Comparing `ramqp-8.2.2/ramqp/metrics.py` & `ramqp-8.3.0/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.2/ramqp/mo.py` & `ramqp-8.3.0/ramqp/mo.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.2/ramqp/utils.py` & `ramqp-8.3.0/ramqp/utils.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.2/PKG-INFO` & `ramqp-8.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramqp
-Version: 8.2.2
+Version: 8.3.0
 Summary: Rammearkitektur AMQP library (aio_pika wrapper)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
```

