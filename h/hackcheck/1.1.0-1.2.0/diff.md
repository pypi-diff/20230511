# Comparing `tmp/hackcheck-1.1.0.tar.gz` & `tmp/hackcheck-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hackcheck-1.1.0.tar", max compression
+gzip compressed data, was "hackcheck-1.2.0.tar", max compression
```

## Comparing `hackcheck-1.1.0.tar` & `hackcheck-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2022-10-21 18:09:39.084802 hackcheck-1.1.0/README.md
--rw-r--r--   0        0        0      144 2022-10-21 18:18:10.477863 hackcheck-1.1.0/hackcheck/__init__.py
--rw-r--r--   0        0        0     2327 2022-10-21 18:22:54.889536 hackcheck-1.1.0/hackcheck/aio.py
--rw-r--r--   0        0        0       82 2022-10-21 18:09:39.084802 hackcheck-1.1.0/hackcheck/errors.py
--rw-r--r--   0        0        0     1906 2022-10-21 18:16:27.292570 hackcheck-1.1.0/hackcheck/hackcheck.py
--rw-r--r--   0        0        0      332 2022-10-21 18:09:39.084802 hackcheck-1.1.0/hackcheck/types.py
--rw-r--r--   0        0        0      453 2022-10-21 18:13:05.875408 hackcheck-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1807 2022-10-21 18:29:19.150481 hackcheck-1.1.0/setup.py
--rw-r--r--   0        0        0     1696 2022-10-21 18:29:19.150728 hackcheck-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      148 2023-05-11 00:41:17.177284 hackcheck-1.2.0/hackcheck/__init__.py
+-rw-r--r--   0        0        0     2402 2023-05-11 00:41:17.177284 hackcheck-1.2.0/hackcheck/aio.py
+-rw-r--r--   0        0        0       88 2023-05-11 00:41:17.177284 hackcheck-1.2.0/hackcheck/errors.py
+-rw-r--r--   0        0        0     1965 2023-05-11 00:41:17.178283 hackcheck-1.2.0/hackcheck/hackcheck.py
+-rw-r--r--   0        0        0      373 2023-05-11 00:41:17.178283 hackcheck-1.2.0/hackcheck/types.py
+-rw-r--r--   0        0        0      478 2023-05-11 00:41:17.178283 hackcheck-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1119 2023-05-11 00:41:17.177284 hackcheck-1.2.0/README.md
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 hackcheck-1.2.0/setup.py
+-rw-r--r--   0        0        0     1753 1970-01-01 00:00:00.000000 hackcheck-1.2.0/PKG-INFO
```

### Comparing `hackcheck-1.1.0/README.md` & `hackcheck-1.2.0/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-# Hackcheck-py
-Official python library for the [hackcheck.io](https://hackcheck.io) API
-
-- [Hackcheck-py](#hackcheck-py)
-  - [Installation](#installation)
-  - [Quick start](#quick-start)
-  - [Methods](#methods)
-
-
-## Installation
-
-Install with pip
-
-```sh
-pip install hackcheck
-```
-
-## Quick start
-
-```py
-from hackcheck import Hackcheck
-
-# Get an api key by purchasing a developer plan https://hackcheck.io/plans
-hc = Hackcheck("MY_API_KEY")
-
-result = hc.lookup_email("your@email.com")
-
-for r in result:
-    print(f"Database: {r.source.name}")
-    print(f"Date: {r.source.date}")
-    print(f"Password: {r.password}")
-    print(f"Username: {r.username}")
-    print(f"IP: {r.ip}")
-    print("------")
-
-# Check your ratelimits
-print(f"Current rate limit: {hc.current_rate_limit}")
-print(f"Allowed rate limit: {hc.allowed_rate_limit}")
-```
-
-## Methods
-
-```py
-hc.lookup_email("your@email.com")
-hc.lookup_username("username")
-hc.lookup_password("password")
-hc.lookup_name("Full Name")
-hc.lookup_ip("8.8.8.8")
-hc.lookup_phone("1234567890")
-hc.lookup_domain("hackcheck.io")
-```
+# Hackcheck-py
+Official python library for the [hackcheck.io](https://hackcheck.io) API
+
+- [Hackcheck-py](#hackcheck-py)
+  - [Installation](#installation)
+  - [Quick start](#quick-start)
+  - [Methods](#methods)
+
+
+## Installation
+
+Install with pip
+
+```sh
+pip install hackcheck
+```
+
+## Quick start
+
+```py
+from hackcheck import Hackcheck
+
+# Get an api key by purchasing a developer plan https://hackcheck.io/plans
+hc = Hackcheck("MY_API_KEY")
+
+result = hc.lookup_email("your@email.com")
+
+for r in result:
+    print(f"Database: {r.source.name}")
+    print(f"Date: {r.source.date}")
+    print(f"Password: {r.password}")
+    print(f"Username: {r.username}")
+    print(f"IP: {r.ip}")
+    print("------")
+
+# Check your ratelimits
+print(f"Current rate limit: {hc.current_rate_limit}")
+print(f"Allowed rate limit: {hc.allowed_rate_limit}")
+```
+
+## Methods
+
+```py
+hc.lookup_email("your@email.com")
+hc.lookup_username("username")
+hc.lookup_password("password")
+hc.lookup_name("Full Name")
+hc.lookup_ip("8.8.8.8")
+hc.lookup_phone("1234567890")
+hc.lookup_domain("hackcheck.io")
+```
```

### Comparing `hackcheck-1.1.0/hackcheck/aio.py` & `hackcheck-1.2.0/hackcheck/aio.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import aiohttp
-
-from .errors import InvalidApiKey
-from .types import Result, Source
-
-BASE_URL = "https://api.hackcheck.io/v3/lookup"
-
-_without = lambda d, w: {k: v for k, v in d.items() if k != w}
-
-
-class AIOHackcheck:
-    def __init__(self, api_key: str):
-        self.api_key = api_key
-        self.allowed_rate_limit = 0
-        self.current_rate_limit = 0
-
-        self._session = aiohttp.ClientSession()
-
-        assert self.api_key != ""
-
-    async def close(self) -> None:
-        await self._session.close()
-
-    async def __aenter__(self):
-        return self
-
-    async def __aexit__(self, *_):
-        await self.close()
-
-    async def _lookup_request(self, q: str, inp: str) -> list[Result]:
-        async with self._session.get(
-            f"{BASE_URL}/{self.api_key}/{q}/{inp}"
-        ) as response:
-            if response.status == 401:
-                raise InvalidApiKey(
-                    "failed to lookup, this may be to your IP address not being linked, or your api key is invalid"
-                )
-
-            self.allowed_rate_limit = int(response.headers["hc-allowed-rate"])
-            self.current_rate_limit = int(response.headers["hc-current-rate"])
-
-            data = await response.json()
-
-            if not data["success"]:
-                raise Exception(data["message"])
-
-            return [
-                Result(**_without(x, "source"), source=Source(**x["source"]))
-                for x in data["results"]
-            ]
-
-    async def lookup_email(self, email: str) -> list[Result]:
-        return await self._lookup_request("email", email)
-
-    async def lookup_username(self, username: str) -> list[Result]:
-        return await self._lookup_request("username", username)
-
-    async def lookup_name(self, name: str) -> list[Result]:
-        return await self._lookup_request("name", name)
-
-    async def lookup_ip(self, ip: str) -> list[Result]:
-        return await self._lookup_request("ip", ip)
-
-    async def lookup_password(self, password: str) -> list[Result]:
-        return await self._lookup_request("password", password)
-
-    async def lookup_phone(self, phone: str) -> list[Result]:
-        return await self._lookup_request("phone", phone)
-
-    async def lookup_domain(self, domain: str) -> list[Result]:
-        return await self._lookup_request("domain", domain)
+import aiohttp
+
+from .errors import InvalidApiKey
+from .types import Result, Source
+
+BASE_URL = "https://api.hackcheck.io/v3/lookup"
+
+_without = lambda d, w: {k: v for k, v in d.items() if k != w}
+
+
+class AIOHackcheck:
+    def __init__(self, api_key: str):
+        self.api_key = api_key
+        self.allowed_rate_limit = 0
+        self.current_rate_limit = 0
+
+        self._session = aiohttp.ClientSession()
+
+        assert self.api_key != ""
+
+    async def close(self) -> None:
+        await self._session.close()
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, *_):
+        await self.close()
+
+    async def _lookup_request(self, q: str, inp: str) -> list[Result]:
+        async with self._session.get(
+            f"{BASE_URL}/{self.api_key}/{q}/{inp}"
+        ) as response:
+            if response.status == 401:
+                raise InvalidApiKey(
+                    "failed to lookup, this may be to your IP address not being linked, or your api key is invalid"
+                )
+
+            self.allowed_rate_limit = int(response.headers["hc-allowed-rate"])
+            self.current_rate_limit = int(response.headers["hc-current-rate"])
+
+            data = await response.json()
+
+            if not data["success"]:
+                raise Exception(data["message"])
+
+            return [
+                Result(**_without(x, "source"), source=Source(**x["source"]))
+                for x in data["results"]
+            ]
+
+    async def lookup_email(self, email: str) -> list[Result]:
+        return await self._lookup_request("email", email)
+
+    async def lookup_username(self, username: str) -> list[Result]:
+        return await self._lookup_request("username", username)
+    
+    async def lookup_name(self, name: str) -> list[Result]:
+        return await self._lookup_request("name", name)
+
+    async def lookup_ip(self, ip: str) -> list[Result]:
+        return await self._lookup_request("ip", ip)
+
+    async def lookup_password(self, password: str) -> list[Result]:
+        return await self._lookup_request("password", password)
+
+    async def lookup_phone(self, phone: str) -> list[Result]:
+        return await self._lookup_request("phone", phone)
+
+    async def lookup_domain(self, domain: str) -> list[Result]:
+        return await self._lookup_request("domain", domain)
```

### Comparing `hackcheck-1.1.0/hackcheck/hackcheck.py` & `hackcheck-1.2.0/hackcheck/hackcheck.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import requests
-
-from .errors import InvalidApiKey
-from .types import Result, Source
-
-BASE_URL = "https://api.hackcheck.io/v3/lookup"
-
-_without = lambda d, w: {k: v for k, v in d.items() if k != w}
-
-
-class Hackcheck:
-    def __init__(self, api_key: str):
-        self.api_key = api_key
-        self.allowed_rate_limit = 0
-        self.current_rate_limit = 0
-
-        assert self.api_key != ""
-
-    def _lookup_request(self, q: str, inp: str) -> list[Result]:
-        response = requests.get(f"{BASE_URL}/{self.api_key}/{q}/{inp}")
-
-        if response.status_code == 401:
-            raise InvalidApiKey(
-                "failed to lookup, this may be to your IP address not being linked, or your api key is invalid"
-            )
-
-        self.allowed_rate_limit = int(response.headers["hc-allowed-rate"])
-        self.current_rate_limit = int(response.headers["hc-current-rate"])
-
-        data = response.json()
-
-        if not data["success"]:
-            raise Exception(data["message"])
-
-        return [
-            Result(**_without(x, "source"), source=Source(**x["source"]))
-            for x in data["results"]
-        ]
-
-    def lookup_email(self, email: str) -> list[Result]:
-        return self._lookup_request("email", email)
-
-    def lookup_username(self, username: str) -> list[Result]:
-        return self._lookup_request("username", username)
-
-    def lookup_name(self, name: str) -> list[Result]:
-        return self._lookup_request("name", name)
-
-    def lookup_ip(self, ip: str) -> list[Result]:
-        return self._lookup_request("ip", ip)
-
-    def lookup_password(self, password: str) -> list[Result]:
-        return self._lookup_request("password", password)
-
-    def lookup_phone(self, phone: str) -> list[Result]:
-        return self._lookup_request("phone", phone)
-
-    def lookup_domain(self, domain: str) -> list[Result]:
-        return self._lookup_request("domain", domain)
+import requests
+
+from .errors import InvalidApiKey
+from .types import Result, Source
+
+BASE_URL = "https://api.hackcheck.io/v3/lookup"
+
+_without = lambda d, w: {k: v for k, v in d.items() if k != w}
+
+
+class Hackcheck:
+    def __init__(self, api_key: str):
+        self.api_key = api_key
+        self.allowed_rate_limit = 0
+        self.current_rate_limit = 0
+
+        assert self.api_key != ""
+
+    def _lookup_request(self, q: str, inp: str) -> list[Result]:
+        response = requests.get(f"{BASE_URL}/{self.api_key}/{q}/{inp}")
+
+        if response.status_code == 401:
+            raise InvalidApiKey(
+                "failed to lookup, this may be to your IP address not being linked, or your api key is invalid"
+            )
+
+        self.allowed_rate_limit = int(response.headers["hc-allowed-rate"])
+        self.current_rate_limit = int(response.headers["hc-current-rate"])
+
+        data = response.json()
+
+        if not data["success"]:
+            raise Exception(data["message"])
+
+        return [
+            Result(**_without(x, "source"), source=Source(**x["source"]))
+            for x in data["results"]
+        ]
+
+    def lookup_email(self, email: str) -> list[Result]:
+        return self._lookup_request("email", email)
+
+    def lookup_username(self, username: str) -> list[Result]:
+        return self._lookup_request("username", username)
+
+    def lookup_name(self, name: str) -> list[Result]:
+        return self._lookup_request("name", name)
+
+    def lookup_ip(self, ip: str) -> list[Result]:
+        return self._lookup_request("ip", ip)
+
+    def lookup_password(self, password: str) -> list[Result]:
+        return self._lookup_request("password", password)
+
+    def lookup_phone(self, phone: str) -> list[Result]:
+        return self._lookup_request("phone", phone)
+
+    def lookup_domain(self, domain: str) -> list[Result]:
+        return self._lookup_request("domain", domain)
```

### Comparing `hackcheck-1.1.0/setup.py` & `hackcheck-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.3,<4.0.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'hackcheck',
-    'version': '1.1.0',
+    'version': '1.2.0',
     'description': 'Official API wrapper for hackcheck.io',
     'long_description': '# Hackcheck-py\nOfficial python library for the [hackcheck.io](https://hackcheck.io) API\n\n- [Hackcheck-py](#hackcheck-py)\n  - [Installation](#installation)\n  - [Quick start](#quick-start)\n  - [Methods](#methods)\n\n\n## Installation\n\nInstall with pip\n\n```sh\npip install hackcheck\n```\n\n## Quick start\n\n```py\nfrom hackcheck import Hackcheck\n\n# Get an api key by purchasing a developer plan https://hackcheck.io/plans\nhc = Hackcheck("MY_API_KEY")\n\nresult = hc.lookup_email("your@email.com")\n\nfor r in result:\n    print(f"Database: {r.source.name}")\n    print(f"Date: {r.source.date}")\n    print(f"Password: {r.password}")\n    print(f"Username: {r.username}")\n    print(f"IP: {r.ip}")\n    print("------")\n\n# Check your ratelimits\nprint(f"Current rate limit: {hc.current_rate_limit}")\nprint(f"Allowed rate limit: {hc.allowed_rate_limit}")\n```\n\n## Methods\n\n```py\nhc.lookup_email("your@email.com")\nhc.lookup_username("username")\nhc.lookup_password("password")\nhc.lookup_name("Full Name")\nhc.lookup_ip("8.8.8.8")\nhc.lookup_phone("1234567890")\nhc.lookup_domain("hackcheck.io")\n```\n',
-    'author': 'balluh',
-    'author_email': 'revoked@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'author': 'HackCheck',
+    'author_email': 'support@hackcheck.io',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/hackcheckio/hackcheck-py/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8.0,<4.0.0',
 }
```

### Comparing `hackcheck-1.1.0/PKG-INFO` & `hackcheck-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: hackcheck
-Version: 1.1.0
+Version: 1.2.0
 Summary: Official API wrapper for hackcheck.io
 Home-page: https://github.com/hackcheckio/hackcheck-py/
-Author: balluh
-Author-email: revoked@gmail.com
+Author: HackCheck
+Author-email: support@hackcheck.io
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/hackcheckio/hackcheck-py/
 Description-Content-Type: text/markdown
 
 # Hackcheck-py
 Official python library for the [hackcheck.io](https://hackcheck.io) API
```

