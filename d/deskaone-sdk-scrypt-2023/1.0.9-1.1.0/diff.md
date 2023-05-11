# Comparing `tmp/deskaone_sdk_scrypt_2023-1.0.9.tar.gz` & `tmp/deskaone_sdk_scrypt_2023-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deskaone_sdk_scrypt_2023-1.0.9.tar", max compression
+gzip compressed data, was "deskaone_sdk_scrypt_2023-1.1.0.tar", max compression
```

## Comparing `deskaone_sdk_scrypt_2023-1.0.9.tar` & `deskaone_sdk_scrypt_2023-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,22 @@
--rw-r--r--   0        0        0      775 2023-05-06 12:26:27.329651 deskaone_sdk_scrypt_2023-1.0.9/pyproject.toml
--rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.0.9/README.md
--rw-r--r--   0        0        0      450 2023-05-06 12:25:31.217555 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/__init__.py
--rw-r--r--   0        0        0     5993 2023-05-04 07:01:51.651028 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Client/__init__.py
--rw-r--r--   0        0        0    15982 2023-05-06 12:22:42.678315 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/__init__.py
--rw-r--r--   0        0        0    10598 2023-05-06 12:05:48.683289 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Captcha/2captcha.py
--rw-r--r--   0        0        0     7722 2023-05-06 12:07:19.570712 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Captcha/9kw.py
--rw-r--r--   0        0        0     1556 2023-05-06 12:10:22.514658 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Captcha/__init__.py
--rw-r--r--   0        0        0     6113 2023-05-06 12:08:24.979983 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Captcha/anticaptcha.py
--rw-r--r--   0        0        0     6104 2023-05-06 12:10:29.220637 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Captcha/capmonster.py
--rw-r--r--   0        0        0     6015 2023-05-06 12:10:28.593535 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Captcha/capsolver.py
--rw-r--r--   0        0        0     8628 2023-05-06 12:10:07.098006 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Captcha/deathbycaptcha.py
--rw-r--r--   0        0        0    20015 2023-05-06 12:23:05.640599 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/cloudflare.py
--rw-r--r--   0        0        0     2170 2023-05-06 12:22:23.671093 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/help.py
--rw-r--r--   0        0        0     1811 2023-05-06 12:15:20.960488 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Interpreters/__init__.py
--rw-r--r--   0        0        0     3353 2023-05-06 12:11:26.435943 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Interpreters/chakracore.py
--rw-r--r--   0        0        0     1994 2023-05-06 12:12:06.860623 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Interpreters/encapsulated.py
--rw-r--r--   0        0        0     1354 2023-05-06 12:12:26.418324 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Interpreters/js2py.py
--rw-r--r--   0        0        0     3601 2023-05-06 12:12:45.889879 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Interpreters/jsunfuck.py
--rw-r--r--   0        0        0     8647 2023-05-06 12:14:54.271362 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Interpreters/native.py
--rw-r--r--   0        0        0     2082 2023-05-06 12:13:21.682559 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Interpreters/nodejs.py
--rw-r--r--   0        0        0     1003 2023-05-06 12:13:43.034786 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/Interpreters/v8.py
--rw-r--r--   0        0        0     5407 2023-05-06 12:19:08.221540 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/user_agent/__init__.py
--rw-r--r--   0        0        0  1214512 2023-05-06 12:19:51.073477 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/CloudFlare/user_agent/browsers.json
--rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Database/__init__.py
--rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
--rw-r--r--   0        0        0     2939 2023-05-02 07:26:37.562775 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
--rw-r--r--   0        0        0      491 2023-05-06 12:26:25.967590 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
--rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
--rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Color.py
--rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
--rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
--rw-r--r--   0        0        0    26122 2023-05-05 20:11:15.157841 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
--rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Random.py
--rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
--rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
--rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
--rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
--rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
--rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
--rw-r--r--   0        0        0     1569 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.0.9/setup.py
--rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-05-11 18:39:54.324494 deskaone_sdk_scrypt_2023-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.1.0/README.md
+-rw-r--r--   0        0        0      450 2023-05-06 12:25:31.217555 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/__init__.py
+-rw-r--r--   0        0        0     6046 2023-05-09 16:58:57.983045 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Client/__init__.py
+-rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Database/__init__.py
+-rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-09 16:39:36.272506 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
+-rw-r--r--   0        0        0      491 2023-05-11 18:39:43.007859 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
+-rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
+-rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Color.py
+-rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
+-rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
+-rw-r--r--   0        0        0    26122 2023-05-05 20:11:15.157841 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
+-rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Random.py
+-rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
+-rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
+-rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
+-rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
+-rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
+-rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
+-rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.0/setup.py
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.0/PKG-INFO
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/pyproject.toml` & `deskaone_sdk_scrypt_2023-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deskaone-sdk-scrypt-2023"
-version = "1.0.9"
+version = "1.1.0"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "deskaone_sdk_scrypt_2023", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -15,15 +15,14 @@
 random-user-agent = "^1.0.1"
 pycryptodome = "^3.17"
 install-jdk = "^0.3.0"
 python-dotenv = "^1.0.0"
 pysocks = "^1.7.1"
 flask = "^2.2.3"
 gunicorn = "^20.1.0"
-psycopg2 = "^2.9.5"
 html5lib = "^1.1"
 bs4 = "^0.0.1"
 polling2 = "^0.5.0"
 polling = "^0.3.2"
 
 
 [build-system]
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Client/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 from requests.auth import AuthBase
 import time, base64, hmac, requests
-from requests import Response
+from requests import PreparedRequest, Response
 from typing import Optional
 from deskaone_sdk_scrypt_2023.Exceptions import Error
 from deskaone_sdk_scrypt_2023.Utils import Crypto, __version_code__
 from deskaone_sdk_scrypt_2023.Internal import Internal
 
 class __Auth__(AuthBase):
     
     def __init__(self, secret_key: str):
         self.secret_key = secret_key
 
-    def __call__(self, request):
+    def __call__(self, request: PreparedRequest) -> PreparedRequest:
         timestamp   = str(int(time.time() * 1000))
         message     = str(timestamp + request.method + request.path_url + (request.body or ''))
         signature   = base64.b64encode(hmac.new(self.secret_key.encode(), message.encode(), 'SHA256').digest()).decode()
         request.headers.update({
             'User-Agent'    : f'DesKaOne-Scrypt-SDK-2023@{__version_code__}',
             'SIGNATURE'     : signature,
             'TIMESTAMP'     : timestamp,
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Database/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Internal/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Random.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Random.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Timer.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Timer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/Typer.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/Typer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.0/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/setup.py` & `deskaone_sdk_scrypt_2023-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 
 package_dir = \
 {'': 'src'}
 
 packages = \
 ['deskaone_sdk_scrypt_2023',
  'deskaone_sdk_scrypt_2023.Client',
- 'deskaone_sdk_scrypt_2023.CloudFlare',
- 'deskaone_sdk_scrypt_2023.CloudFlare.Captcha',
- 'deskaone_sdk_scrypt_2023.CloudFlare.Interpreters',
- 'deskaone_sdk_scrypt_2023.CloudFlare.user_agent',
  'deskaone_sdk_scrypt_2023.Database',
  'deskaone_sdk_scrypt_2023.Exceptions',
  'deskaone_sdk_scrypt_2023.Internal',
  'deskaone_sdk_scrypt_2023.Utils',
  'deskaone_sdk_scrypt_2023.Utils.WebShare']
 
 package_data = \
@@ -26,25 +22,24 @@
  'colorama>=0.4.6,<0.5.0',
  'flask>=2.2.3,<3.0.0',
  'gunicorn>=20.1.0,<21.0.0',
  'html5lib>=1.1,<2.0',
  'install-jdk>=0.3.0,<0.4.0',
  'polling2>=0.5.0,<0.6.0',
  'polling>=0.3.2,<0.4.0',
- 'psycopg2>=2.9.5,<3.0.0',
  'pycryptodome>=3.17,<4.0',
  'pysocks>=1.7.1,<2.0.0',
  'python-dotenv>=1.0.0,<2.0.0',
  'random-user-agent>=1.0.1,<2.0.0',
  'requests[socks]>=2.28.2,<3.0.0',
  'sqlalchemy==1.4.29']
 
 setup_kwargs = {
     'name': 'deskaone-sdk-scrypt-2023',
-    'version': '1.0.9',
+    'version': '1.1.0',
     'description': '',
     'long_description': 'xxxxxxxxxxxxxxxx',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.9/PKG-INFO` & `deskaone_sdk_scrypt_2023-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskaone-sdk-scrypt-2023
-Version: 1.0.9
+Version: 1.1.0
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,15 +15,14 @@
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: flask (>=2.2.3,<3.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: install-jdk (>=0.3.0,<0.4.0)
 Requires-Dist: polling (>=0.3.2,<0.4.0)
 Requires-Dist: polling2 (>=0.5.0,<0.6.0)
-Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Requires-Dist: pycryptodome (>=3.17,<4.0)
 Requires-Dist: pysocks (>=1.7.1,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Requires-Dist: requests[socks] (>=2.28.2,<3.0.0)
 Requires-Dist: sqlalchemy (==1.4.29)
 Description-Content-Type: text/markdown
```

