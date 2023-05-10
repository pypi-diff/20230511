# Comparing `tmp/auth_lib_profcomff-2023.5.10.tar.gz` & `tmp/auth_lib_profcomff-2023.5.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_lib_profcomff-2023.5.10.tar", last modified: Tue May  9 23:27:50 2023, max compression
+gzip compressed data, was "auth_lib_profcomff-2023.5.11.tar", last modified: Wed May 10 23:53:57 2023, max compression
```

## Comparing `auth_lib_profcomff-2023.5.10.tar` & `auth_lib_profcomff-2023.5.11.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:27:50.057726 auth_lib_profcomff-2023.5.10/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-09 23:27:50.057726 auth_lib_profcomff-2023.5.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:27:50.053726 auth_lib_profcomff-2023.5.10/auth_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/aiomethods.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:27:50.053726 auth_lib_profcomff-2023.5.10/auth_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/testing/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:27:50.053726 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-09 23:27:50.000000 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-09 23:27:50.000000 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:27:50.000000 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-09 23:27:50.000000 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 23:27:50.000000 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 23:27:50.000000 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 23:27:50.057726 auth_lib_profcomff-2023.5.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:53:57.294563 auth_lib_profcomff-2023.5.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-10 23:53:57.294563 auth_lib_profcomff-2023.5.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:53:57.294563 auth_lib_profcomff-2023.5.11/auth_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/aiomethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:53:57.294563 auth_lib_profcomff-2023.5.11/auth_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/testing/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:53:57.294563 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-10 23:53:57.000000 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-10 23:53:57.000000 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 23:53:57.000000 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 23:53:57.000000 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-10 23:53:57.000000 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 23:53:57.000000 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 23:53:57.294563 auth_lib_profcomff-2023.5.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/setup.py
```

### Comparing `auth_lib_profcomff-2023.5.10/LICENSE` & `auth_lib_profcomff-2023.5.11/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.5.10/PKG-INFO` & `auth_lib_profcomff-2023.5.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth_lib_profcomff
-Version: 2023.5.10
+Version: 2023.5.11
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: fastapi
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `auth_lib_profcomff-2023.5.10/README.md` & `auth_lib_profcomff-2023.5.11/README.md`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.5.10/auth_lib/aiomethods.py` & `auth_lib_profcomff-2023.5.11/auth_lib/aiomethods.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.5.10/auth_lib/exceptions.py` & `auth_lib_profcomff-2023.5.11/auth_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.5.10/auth_lib/fastapi.py` & `auth_lib_profcomff-2023.5.11/auth_lib/fastapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from fastapi.exceptions import HTTPException
 from fastapi.openapi.models import APIKey, APIKeyIn
 from fastapi.security.base import SecurityBase
 from pydantic import BaseSettings
 from starlette.requests import Request
 from starlette.status import HTTP_403_FORBIDDEN
-from starlette.websockets import WebSocket
 
 from auth_lib.aiomethods import AsyncAuthLib
 
 
 class UnionAuthSettings(BaseSettings):
     AUTH_URL: str = "https://api.test.profcomff.com/auth/"
     AUTH_AUTO_ERROR: bool = True
@@ -66,15 +65,15 @@
             return None
         if not token:
             return self._except()
         return await AsyncAuthLib(url=self.auth_url).check_token(token)
 
     async def __call__(
         self,
-        request: Request | WebSocket,
+        request: Request,
     ) -> dict[str, Any] | None:
         token = request.headers.get("Authorization")
         user_session = await self._get_session(token)
         if user_session is None:
             return self._except()
         session_scopes = set(
             [scope["name"].lower() for scope in user_session["session_scopes"]]
```

### Comparing `auth_lib_profcomff-2023.5.10/auth_lib/methods.py` & `auth_lib_profcomff-2023.5.11/auth_lib/methods.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.5.10/auth_lib/testing/testutils.py` & `auth_lib_profcomff-2023.5.11/auth_lib/testing/testutils.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/PKG-INFO` & `auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-lib-profcomff
-Version: 2023.5.10
+Version: 2023.5.11
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: fastapi
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `auth_lib_profcomff-2023.5.10/setup.py` & `auth_lib_profcomff-2023.5.11/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="auth_lib_profcomff",
-    version="2023.05.10",
+    version="2023.05.11",
     author="Semyon Grigoriev",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/profcomff/auth-lib",
     packages=find_packages(),
     install_requires=["requests", "aiohttp", "setuptools"],
     extras_require={
```

