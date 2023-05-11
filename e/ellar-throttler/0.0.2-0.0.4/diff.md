# Comparing `tmp/ellar-throttler-0.0.2.tar.gz` & `tmp/ellar-throttler-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellar-throttler-0.0.2.tar", last modified: Sun Mar 26 13:42:02 2023, max compression
+gzip compressed data, was "ellar-throttler-0.0.4.tar", last modified: Thu May 11 21:51:59 2023, max compression
```

## Comparing `ellar-throttler-0.0.2.tar` & `ellar-throttler-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0       65 2023-03-26 13:41:46.729100 ellar-throttler-0.0.2/.dockerignore
--rw-r--r--   0        0        0      140 2023-03-26 13:41:46.729100 ellar-throttler-0.0.2/.flake8
--rw-r--r--   0        0        0      205 2023-03-26 13:41:46.729100 ellar-throttler-0.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0      571 2023-03-26 13:41:46.729100 ellar-throttler-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      545 2023-03-26 13:41:46.729100 ellar-throttler-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0     1162 2023-03-26 13:41:46.729100 ellar-throttler-0.0.2/.github/workflows/test_full.yml
--rw-r--r--   0        0        0     1891 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/.gitignore
--rw-r--r--   0        0        0       53 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/.isort.cfg
--rw-r--r--   0        0        0     1073 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1083 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/LICENSE
--rw-r--r--   0        0        0     1097 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/Makefile
--rw-r--r--   0        0        0     6666 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/README.md
--rwxr-xr-x   0        0        0    25915 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/docs/img/EllarLogoB.png
--rwxr-xr-x   0        0        0    36744 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/docs/img/EllarLogoIconOnly.png
--rwxr-xr-x   0        0        0    26456 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/docs/img/EllarLogoW.png
--rwxr-xr-x   0        0        0     3888 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/docs/img/Icon.svg
--rwxr-xr-x   0        0        0     4781 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/docs/img/Logo.svg
--rw-r--r--   0        0        0     1496 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/docs/index.md
--rw-r--r--   0        0        0       57 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      575 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/__init__.py
--rw-r--r--   0        0        0      149 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/constants.py
--rw-r--r--   0        0        0     1666 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/decorators.py
--rw-r--r--   0        0        0      981 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/exception.py
--rw-r--r--   0        0        0       89 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/interfaces/__init__.py
--rw-r--r--   0        0        0      815 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/interfaces/throttler_storage.py
--rw-r--r--   0        0        0     1482 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/module.py
--rw-r--r--   0        0        0        0 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/py.typed
--rw-r--r--   0        0        0     3311 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/throttler_guard.py
--rw-r--r--   0        0        0      519 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/throttler_module_options.py
--rw-r--r--   0        0        0     3544 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/throttler_service.py
--rw-r--r--   0        0        0      126 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/throttler_storage_options.py
--rw-r--r--   0        0        0      265 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/ellar_throttler/throttler_storage_record.py
--rw-r--r--   0        0        0      660 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/mypy.ini
--rw-r--r--   0        0        0     1910 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      207 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/pytest.ini
--rw-r--r--   0        0        0        0 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/tests/app/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/tests/app/controller/__init__.py
--rw-r--r--   0        0        0      476 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/tests/app/controller/app.py
--rw-r--r--   0        0        0      294 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/tests/app/controller/default.py
--rw-r--r--   0        0        0      723 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/tests/app/controller/limit.py
--rw-r--r--   0        0        0      412 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/tests/app/controller/module.py
--rw-r--r--   0        0        0      179 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/tests/app/controller/service.py
--rw-r--r--   0        0        0      146 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/tests/app/module.py
--rw-r--r--   0        0        0      193 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/tests/app/server.py
--rw-r--r--   0        0        0     5940 2023-03-26 13:41:46.733101 ellar-throttler-0.0.2/tests/test_throttler.py
--rw-r--r--   0        0        0     8723 1970-01-01 00:00:00.000000 ellar-throttler-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/.dockerignore
+-rw-r--r--   0        0        0      140 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/.flake8
+-rw-r--r--   0        0        0      205 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      571 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      545 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1162 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0     1891 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/.gitignore
+-rw-r--r--   0        0        0       53 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/.isort.cfg
+-rw-r--r--   0        0        0     1073 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1083 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1097 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/Makefile
+-rw-r--r--   0        0        0     6668 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/README.md
+-rwxr-xr-x   0        0        0    25915 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/docs/img/EllarLogoB.png
+-rwxr-xr-x   0        0        0    36744 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/docs/img/EllarLogoIconOnly.png
+-rwxr-xr-x   0        0        0    26456 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/docs/img/EllarLogoW.png
+-rwxr-xr-x   0        0        0     3888 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/docs/img/Icon.svg
+-rwxr-xr-x   0        0        0     4781 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/docs/img/Logo.svg
+-rw-r--r--   0        0        0     1496 2023-05-11 21:51:41.652568 ellar-throttler-0.0.4/docs/index.md
+-rw-r--r--   0        0        0       57 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      575 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/__init__.py
+-rw-r--r--   0        0        0      149 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/constants.py
+-rw-r--r--   0        0        0     1666 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/decorators.py
+-rw-r--r--   0        0        0      972 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/exception.py
+-rw-r--r--   0        0        0       89 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/interfaces/__init__.py
+-rw-r--r--   0        0        0      815 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/interfaces/throttler_storage.py
+-rw-r--r--   0        0        0     1459 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/module.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/py.typed
+-rw-r--r--   0        0        0     3325 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/throttler_guard.py
+-rw-r--r--   0        0        0      493 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/throttler_module_options.py
+-rw-r--r--   0        0        0     3544 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/throttler_service.py
+-rw-r--r--   0        0        0      122 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/throttler_storage_options.py
+-rw-r--r--   0        0        0      261 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/ellar_throttler/throttler_storage_record.py
+-rw-r--r--   0        0        0      660 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/mypy.ini
+-rw-r--r--   0        0        0     1910 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/pytest.ini
+-rw-r--r--   0        0        0        0 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/tests/app/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/tests/app/controller/__init__.py
+-rw-r--r--   0        0        0      476 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/tests/app/controller/app.py
+-rw-r--r--   0        0        0      294 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/tests/app/controller/default.py
+-rw-r--r--   0        0        0      723 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/tests/app/controller/limit.py
+-rw-r--r--   0        0        0      412 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/tests/app/controller/module.py
+-rw-r--r--   0        0        0      179 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/tests/app/controller/service.py
+-rw-r--r--   0        0        0      146 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/tests/app/module.py
+-rw-r--r--   0        0        0      193 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/tests/app/server.py
+-rw-r--r--   0        0        0     5911 2023-05-11 21:51:41.656568 ellar-throttler-0.0.4/tests/test_throttler.py
+-rw-r--r--   0        0        0     8725 1970-01-01 00:00:00.000000 ellar-throttler-0.0.4/PKG-INFO
```

### Comparing `ellar-throttler-0.0.2/.github/workflows/publish.yml` & `ellar-throttler-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/.github/workflows/test.yml` & `ellar-throttler-0.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/.github/workflows/test_full.yml` & `ellar-throttler-0.0.4/.github/workflows/test_full.yml`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/.gitignore` & `ellar-throttler-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/.pre-commit-config.yaml` & `ellar-throttler-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/LICENSE` & `ellar-throttler-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/Makefile` & `ellar-throttler-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/README.md` & `ellar-throttler-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,21 +66,21 @@
 **NOTE**: If you add the `ThrottlerGuard` to your application `global_guards`, then all the incoming requests will be throttled by default. 
 This can also be omitted in favor of `@guards(ThrottlerGuard)`. 
 The global guard check can be skipped using the `@skip_throttle()` decorator mentioned later.
 
 Example with `@guards(ThrottlerGuard)`
 ```python
 # project_name/controller.py
-from ellar.common import Controller, guards
+from ellar.common import Controller, Guards
 from ellar_throttler import throttle, ThrottlerGuard
 
 @Controller()
 class AppController:
 
-  @guards(ThrottlerGuard)
+  @Guards(ThrottlerGuard)
   @throttle(limit=5, ttl=30)
   def normal(self):
       pass
 
 ```
 ### Decorators
 #### @throttle()
@@ -174,15 +174,15 @@
 ```
 
 ### Working with WebSockets
 To work with Websockets you can extend the `ThrottlerGuard` and override the `handle_request` method with the code below:
 ```python
 from ellar_throttler import ThrottlerGuard
 from ellar.di import injectable
-from ellar.core import IExecutionContext
+from ellar.common import IExecutionContext
 from ellar_throttler import ThrottledException
 
 @injectable()
 class WsThrottleGuard(ThrottlerGuard):
     async def handle_request(self, context: IExecutionContext, limit: int, ttl: int) -> bool:
         websocket_client = context.switch_to_websocket().get_client()
```

### Comparing `ellar-throttler-0.0.2/docs/img/EllarLogoB.png` & `ellar-throttler-0.0.4/docs/img/EllarLogoB.png`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/docs/img/EllarLogoIconOnly.png` & `ellar-throttler-0.0.4/docs/img/EllarLogoIconOnly.png`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/docs/img/EllarLogoW.png` & `ellar-throttler-0.0.4/docs/img/EllarLogoW.png`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/docs/img/Icon.svg` & `ellar-throttler-0.0.4/docs/img/Icon.svg`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/docs/img/Logo.svg` & `ellar-throttler-0.0.4/docs/img/Logo.svg`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/docs/index.md` & `ellar-throttler-0.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/ellar_throttler/__init__.py` & `ellar-throttler-0.0.4/ellar_throttler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A rate limiting module for Ellar"""
 
-__version__ = "0.0.2"
+__version__ = "0.0.4"
 
 from .decorators import skip_throttle, throttle
 from .exception import ThrottledException
 from .interfaces import IThrottlerStorage
 from .module import ThrottlerModule
 from .throttler_guard import ThrottlerGuard
 from .throttler_service import CacheThrottlerStorageService, ThrottlerStorageService
```

### Comparing `ellar-throttler-0.0.2/ellar_throttler/decorators.py` & `ellar-throttler-0.0.4/ellar_throttler/decorators.py`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/ellar_throttler/exception.py` & `ellar-throttler-0.0.4/ellar_throttler/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 import typing as t
 
-from ellar.core.exceptions import APIException
+from ellar.common import APIException
 from starlette import status
 
 
 class ThrottledException(APIException):
     status_code = status.HTTP_429_TOO_MANY_REQUESTS
     default_detail = "Request was throttled."
     extra_detail_singular = "Expected available in {wait} second."
```

### Comparing `ellar-throttler-0.0.2/ellar_throttler/interfaces/throttler_storage.py` & `ellar-throttler-0.0.4/ellar_throttler/interfaces/throttler_storage.py`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/ellar_throttler/module.py` & `ellar-throttler-0.0.4/ellar_throttler/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import typing as t
 
-from ellar.common import Module
-from ellar.core import IExecutionContext
-from ellar.core.modules import DynamicModule, IModuleSetup, ModuleBase
+from ellar.common import IExecutionContext, IModuleSetup, Module
+from ellar.core.modules import DynamicModule, ModuleBase
 from ellar.di import ProviderConfig
 
 from ellar_throttler.interfaces import IThrottlerStorage
 from ellar_throttler.throttler_module_options import ThrottlerModuleOptions
 from ellar_throttler.throttler_service import ThrottlerStorageService
 
 
@@ -25,15 +24,15 @@
         elif storage:
             _provider = ProviderConfig(IThrottlerStorage, use_class=storage)
         else:
             _provider = ProviderConfig(
                 IThrottlerStorage, use_class=ThrottlerStorageService
             )
 
-        return DynamicModule(  # type: ignore
+        return DynamicModule(  # type:ignore
             cls,
             providers=[
                 _provider,
                 ProviderConfig(
                     ThrottlerModuleOptions,
                     use_value=ThrottlerModuleOptions(
                         limit=limit,
```

### Comparing `ellar-throttler-0.0.2/ellar_throttler/throttler_guard.py` & `ellar-throttler-0.0.4/ellar_throttler/throttler_guard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import hashlib
 import typing as t
 
-from ellar.core import GuardCanActivate, IExecutionContext, Response
+from ellar.common import GuardCanActivate, IExecutionContext, Response
+from ellar.common.helper import get_name
 from ellar.core.connection import HTTPConnection
+from ellar.core.services import Reflector
 from ellar.di import injectable
-from ellar.helper import get_name
-from ellar.services import Reflector
 
 from .constants import THROTTLER_LIMIT, THROTTLER_SKIP, THROTTLER_TTL
 from .exception import ThrottledException
 from .interfaces import IThrottlerStorage
 from .throttler_module_options import ThrottlerModuleOptions
```

### Comparing `ellar-throttler-0.0.2/ellar_throttler/throttler_service.py` & `ellar-throttler-0.0.4/ellar_throttler/throttler_service.py`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/mypy.ini` & `ellar-throttler-0.0.4/mypy.ini`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/pyproject.toml` & `ellar-throttler-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Framework :: AsyncIO",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 dependencies = [
-    "ellar >= 0.3.4"
+    "ellar >= 0.3.8"
 ]
 
 
 [project.urls]
 Documentation = "https://github.com/eadwinCode/ellar-throttler"
 Source = "https://github.com/eadwinCode/ellar-throttler"
 Homepage = "https://eadwincode.github.io/ellar-throttler/"
```

### Comparing `ellar-throttler-0.0.2/tests/app/controller/limit.py` & `ellar-throttler-0.0.4/tests/app/controller/limit.py`

 * *Files identical despite different names*

### Comparing `ellar-throttler-0.0.2/tests/test_throttler.py` & `ellar-throttler-0.0.4/tests/test_throttler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 
 import pytest
 from app.controller.module import ControllerModule
 from app.server import app
 from ellar.cache import CacheModule
 from ellar.cache.backends.local_cache import LocalMemCacheBackend
-from ellar.core import TestClient, TestClientFactory
+from ellar.testing import Test, TestClient
 
 from ellar_throttler import (
     CacheThrottlerStorageService,
     ThrottlerGuard,
     ThrottlerModule,
     ThrottlerStorageService,
 )
@@ -81,48 +81,48 @@
         assert res.headers["x-ratelimit-limit"] == "5"
         assert res.headers["x-ratelimit-remaining"] == "4"
         assert "x-ratelimit-reset" in res.headers
 
 
 class TestSkipIfConfigure:
     def test_skip_configure(self):
-        test_module = TestClientFactory.create_test_module(
+        test_module = Test.create_test_module(
             modules=(
                 ThrottlerModule.setup(limit=5, ttl=100, skip_if=lambda ctx: True),
                 ControllerModule,
             ),
             global_guards=[ThrottlerGuard],
         )
 
-        _client = test_module.get_client()
+        _client = test_module.get_test_client()
         for i in range(15):
             res = _client.get("/")
 
             assert res.status_code == 200
             assert res.json() == {"success": True}
 
             assert "x-ratelimit-limit" not in res.headers
             assert "x-ratelimit-remaining" not in res.headers
             assert "x-ratelimit-reset" not in res.headers
 
 
 class TestThrottlerStorageServiceConfiguration:
-    test_module_cache = TestClientFactory.create_test_module(
+    test_module_cache = Test.create_test_module(
         modules=(
             ThrottlerModule.setup(
                 limit=5, ttl=100, storage=CacheThrottlerStorageService
             ),
             CacheModule.register_setup(),
             ControllerModule,
         ),
         global_guards=[ThrottlerGuard],
         config_module=dict(CACHES={"default": LocalMemCacheBackend()}),
     )
 
-    test_module_use_value = TestClientFactory.create_test_module(
+    test_module_use_value = Test.create_test_module(
         modules=(
             ThrottlerModule.setup(limit=5, ttl=100, storage=ThrottlerStorageService()),
             ControllerModule,
         ),
         global_guards=[ThrottlerGuard],
     )
 
@@ -134,28 +134,28 @@
 
             assert res.headers["x-ratelimit-limit"] == str(limit)
             assert res.headers["x-ratelimit-remaining"] == str(limit - (i + 1))
             assert "x-ratelimit-reset" in res.headers
 
     @pytest.mark.parametrize("test_module", [test_module_cache, test_module_use_value])
     def test_limit_index(self, test_module):
-        _client = test_module.get_client()
+        _client = test_module.get_test_client()
 
         for url, limit in [("/limit/", 2), ("/limit/higher", 5)]:
             self.request_for_limit(_client, url, limit)
             res = _client.get(url)
             assert res.status_code == 429
             assert (
                 "Request was throttled. Expected available in" in res.json()["detail"]
             )
             assert "retry-after" in res.headers
 
     @pytest.mark.parametrize("test_module", [test_module_cache, test_module_use_value])
     def test_limit_get_shorter(self, test_module):
-        _client = test_module.get_client()
+        _client = test_module.get_test_client()
         limit, url = (
             5,
             "/limit/shorter",
         )
 
         self.request_for_limit(_client, url, limit)
 
@@ -163,15 +163,15 @@
         assert res.status_code == 429
         time.sleep(1)  # quick restart
         res = _client.get(url)
         assert res.headers["x-ratelimit-remaining"] == str(limit - 1)
 
     @pytest.mark.parametrize("test_module", [test_module_use_value])
     def test_limit_get_shorter_cache_clear(self, test_module):
-        _client = test_module.get_client()
+        _client = test_module.get_test_client()
         limit, url = (
             5,
             "/limit/shorter-2",
         )
 
         self.request_for_limit(_client, url, limit)
```

### Comparing `ellar-throttler-0.0.2/PKG-INFO` & `ellar-throttler-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellar-throttler
-Version: 0.0.2
+Version: 0.0.4
 Summary: A rate limiting module for Ellar
 Author-email: Ezeudoh Tochukwu <tochukwu.ezeudoh@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Dist: ellar >= 0.3.4
+Requires-Dist: ellar >= 0.3.8
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest >= 7.1.3,<8.0.0 ; extra == "test"
 Requires-Dist: pytest-cov >= 2.12.0,<5.0.0 ; extra == "test"
 Requires-Dist: mypy == 0.971 ; extra == "test"
 Requires-Dist: flake8 >= 3.8.3,<7.0.0 ; extra == "test"
 Requires-Dist: black ==22.8.0 ; extra == "test"
 Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test"
@@ -111,21 +111,21 @@
 **NOTE**: If you add the `ThrottlerGuard` to your application `global_guards`, then all the incoming requests will be throttled by default. 
 This can also be omitted in favor of `@guards(ThrottlerGuard)`. 
 The global guard check can be skipped using the `@skip_throttle()` decorator mentioned later.
 
 Example with `@guards(ThrottlerGuard)`
 ```python
 # project_name/controller.py
-from ellar.common import Controller, guards
+from ellar.common import Controller, Guards
 from ellar_throttler import throttle, ThrottlerGuard
 
 @Controller()
 class AppController:
 
-  @guards(ThrottlerGuard)
+  @Guards(ThrottlerGuard)
   @throttle(limit=5, ttl=30)
   def normal(self):
       pass
 
 ```
 ### Decorators
 #### @throttle()
@@ -219,15 +219,15 @@
 ```
 
 ### Working with WebSockets
 To work with Websockets you can extend the `ThrottlerGuard` and override the `handle_request` method with the code below:
 ```python
 from ellar_throttler import ThrottlerGuard
 from ellar.di import injectable
-from ellar.core import IExecutionContext
+from ellar.common import IExecutionContext
 from ellar_throttler import ThrottledException
 
 @injectable()
 class WsThrottleGuard(ThrottlerGuard):
     async def handle_request(self, context: IExecutionContext, limit: int, ttl: int) -> bool:
         websocket_client = context.switch_to_websocket().get_client()
```

