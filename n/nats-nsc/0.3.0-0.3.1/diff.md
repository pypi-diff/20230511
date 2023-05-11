# Comparing `tmp/nats_nsc-0.3.0.tar.gz` & `tmp/nats_nsc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats_nsc-0.3.0.tar", last modified: Tue May  9 18:35:05 2023, max compression
+gzip compressed data, was "nats_nsc-0.3.1.tar", last modified: Thu May 11 18:07:26 2023, max compression
```

## Comparing `nats_nsc-0.3.0.tar` & `nats_nsc-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-09 18:34:39.741829 nats_nsc-0.3.0/LICENSE
--rw-r--r--   0        0        0      191 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/README.md
--rw-r--r--   0        0        0      777 2023-05-09 18:35:05.242029 nats_nsc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      157 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/src/nats_nsc/__init__.py
--rw-r--r--   0        0        0     6302 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/src/nats_nsc/common.py
--rw-r--r--   0        0        0     3945 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/src/nats_nsc/create_user.py
--rw-r--r--   0        0        0     3327 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nats.cfg
--rw-r--r--   0        0        0       68 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/.gitignore
--rw-r--r--   0        0        0       71 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/keys/DO_NOT_USE
--rw-r--r--   0        0        0       75 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/.nsc
--rw-r--r--   0        0        0     1582 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt
--rw-r--r--   0        0        0      646 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt
--rw-r--r--   0        0        0      745 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      562 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      668 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      175 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nsc.json
--rw-r--r--   0        0        0      980 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/test_basic.py
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 nats_nsc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/LICENSE
+-rw-r--r--   0        0        0       88 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/README.md
+-rw-r--r--   0        0        0      777 2023-05-11 18:07:26.446614 nats_nsc-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/src/nats_nsc/__init__.py
+-rw-r--r--   0        0        0     6302 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/src/nats_nsc/common.py
+-rw-r--r--   0        0        0     4011 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/src/nats_nsc/create_user.py
+-rw-r--r--   0        0        0     3327 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nats.cfg
+-rw-r--r--   0        0        0       68 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/.gitignore
+-rw-r--r--   0        0        0       71 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/keys/DO_NOT_USE
+-rw-r--r--   0        0        0       75 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/.nsc
+-rw-r--r--   0        0        0     1582 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt
+-rw-r--r--   0        0        0      646 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt
+-rw-r--r--   0        0        0      745 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      562 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      668 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      175 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/nsc_workdir/nsc.json
+-rw-r--r--   0        0        0      980 2023-05-11 18:06:59.594298 nats_nsc-0.3.1/tests/test_basic.py
+-rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 nats_nsc-0.3.1/PKG-INFO
```

### Comparing `nats_nsc-0.3.0/LICENSE` & `nats_nsc-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.0/pyproject.toml` & `nats_nsc-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [tool.pytest.ini_options]
 pythonpath = [
     "src/",
 ]
 
 [project]
 name = "nats-nsc"
-version = "0.3.0"
+version = "0.3.1"
 description = "Limited python nsc utility equivalent, for user creation and signing JWTs."
 authors = [
     { name = "Mikołaj Nowak", email = "12396461+m3nowak@users.noreply.github.com" },
 ]
 dependencies = [
     "pyJWT~=2.6.0",
     "aiofiles~=23.1.0",
```

### Comparing `nats_nsc-0.3.0/src/nats_nsc/common.py` & `nats_nsc-0.3.1/src/nats_nsc/common.py`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.0/src/nats_nsc/create_user.py` & `nats_nsc-0.3.1/src/nats_nsc/create_user.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 HEADER = {
   "typ": "JWT",
   "alg": "ed25519-nkey"
 }
 
 def create_user(user_name: str, account: common.Account,
-                pub_key: str,
+                pub_key: str, *, jwt_id: ty.Optional[str] = None,
                 allow_pub: ty.Optional[ty.List[str]] = None,
                 allow_pub_response: ty.Optional[int] = None,
                 allow_pubsub: ty.Optional[ty.List[str]] = None,
                 allow_sub: ty.Optional[ty.List[str]] = None,
                 bearer: bool = False,
                 deny_pub: ty.Optional[ty.List[str]] = None,
                 deny_pubsub: ty.Optional[ty.List[str]] = None,
@@ -74,15 +74,15 @@
             response_ttl = timedelta(seconds=0)
         resp = {
             'max': allow_pub_response,
             'ttl': response_ttl.total_seconds() * common.TTL_SCALE
         }
     
     payload = {
-        'jti': uuid.uuid4().hex,
+        'jti': uuid.uuid4().hex if jwt_id is None else jwt_id,
         'iat': int(issued_at.timestamp()),
         'iss': account.pub_key,
         'name': user_name,
         'sub': pub_key,
         'nats': {
             'sub': sub,
             'pub': pub,
```

### Comparing `nats_nsc-0.3.0/tests/nats.cfg` & `nats_nsc-0.3.1/tests/nats.cfg`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt` & `nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt` & `nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt` & `nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt` & `nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt` & `nats_nsc-0.3.1/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.3.0/tests/test_basic.py` & `nats_nsc-0.3.1/tests/test_basic.py`

 * *Files identical despite different names*

