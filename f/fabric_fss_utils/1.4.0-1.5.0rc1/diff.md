# Comparing `tmp/fabric_fss_utils-1.4.0.tar.gz` & `tmp/fabric_fss_utils-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_fss_utils-1.4.0.tar", last modified: Wed Nov  9 15:15:57 2022, max compression
+gzip compressed data, was "fabric_fss_utils-1.5.0rc1.tar", last modified: Wed May 10 22:00:48 2023, max compression
```

## Comparing `fabric_fss_utils-1.4.0.tar` & `fabric_fss_utils-1.5.0rc1.tar`

### file list

```diff
@@ -1,28 +1,21 @@
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-11-09 15:15:57.097590 fabric_fss_utils-1.4.0/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-11-09 14:57:32.000000 fabric_fss_utils-1.4.0/AUTHORS
--rw-r--r--   0 kthare10   (503) staff       (20)     1071 2022-11-09 14:57:32.000000 fabric_fss_utils-1.4.0/LICENSE
--rw-r--r--   0 kthare10   (503) staff       (20)       59 2022-11-09 14:57:32.000000 fabric_fss_utils-1.4.0/MANIFEST.in
--rw-r--r--   0 kthare10   (503) staff       (20)      488 2022-11-09 15:15:57.097347 fabric_fss_utils-1.4.0/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)      851 2022-11-09 14:57:32.000000 fabric_fss_utils-1.4.0/README.md
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-11-09 15:15:57.094357 fabric_fss_utils-1.4.0/fabric_fss_utils.egg-info/
--rw-r--r--   0 kthare10   (503) staff       (20)      488 2022-11-09 15:15:57.000000 fabric_fss_utils-1.4.0/fabric_fss_utils.egg-info/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)      517 2022-11-09 15:15:57.000000 fabric_fss_utils-1.4.0/fabric_fss_utils.egg-info/SOURCES.txt
--rw-r--r--   0 kthare10   (503) staff       (20)        1 2022-11-09 15:15:57.000000 fabric_fss_utils-1.4.0/fabric_fss_utils.egg-info/dependency_links.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       63 2022-11-09 15:15:57.000000 fabric_fss_utils-1.4.0/fabric_fss_utils.egg-info/requires.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       15 2022-11-09 15:15:57.000000 fabric_fss_utils-1.4.0/fabric_fss_utils.egg-info/top_level.txt
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-11-09 15:15:57.095922 fabric_fss_utils-1.4.0/fss_utils/
--rw-r--r--   0 kthare10   (503) staff       (20)       25 2022-11-09 15:15:07.000000 fabric_fss_utils-1.4.0/fss_utils/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3290 2022-11-09 14:57:32.000000 fabric_fss_utils-1.4.0/fss_utils/http_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     8027 2022-11-09 15:11:53.000000 fabric_fss_utils-1.4.0/fss_utils/jwt_manager.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3678 2022-11-09 14:57:32.000000 fabric_fss_utils-1.4.0/fss_utils/jwt_validate.py
--rw-r--r--   0 kthare10   (503) staff       (20)     8429 2022-11-09 14:57:32.000000 fabric_fss_utils-1.4.0/fss_utils/sshkey.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5090 2022-11-09 14:57:32.000000 fabric_fss_utils-1.4.0/fss_utils/vouch_encoder.py
--rw-r--r--   0 kthare10   (503) staff       (20)       62 2022-11-09 15:13:37.000000 fabric_fss_utils-1.4.0/requirements.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       38 2022-11-09 15:15:57.097660 fabric_fss_utils-1.4.0/setup.cfg
--rw-r--r--   0 kthare10   (503) staff       (20)      826 2022-11-09 14:57:32.000000 fabric_fss_utils-1.4.0/setup.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-11-09 15:15:57.097044 fabric_fss_utils-1.4.0/test/
--rw-r--r--   0 kthare10   (503) staff       (20)        2 2022-11-09 14:57:32.000000 fabric_fss_utils-1.4.0/test/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     7805 2022-11-09 15:09:03.000000 fabric_fss_utils-1.4.0/test/jwt_decode_test.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4539 2022-11-09 15:12:57.000000 fabric_fss_utils-1.4.0/test/jwt_manager_test.py
--rw-r--r--   0 kthare10   (503) staff       (20)     6964 2022-11-09 15:08:57.000000 fabric_fss_utils-1.4.0/test/ssh_test.py
--rw-r--r--   0 kthare10   (503) staff       (20)     9404 2022-11-09 15:12:53.000000 fabric_fss_utils-1.4.0/test/vouch_encoder_test.py
+-rw-r--r--   0        0        0        0 2020-12-11 22:04:09.114297 fabric_fss_utils-1.5.0rc1/AUTHORS
+-rw-r--r--   0        0        0     1071 2020-12-11 22:04:42.289179 fabric_fss_utils-1.5.0rc1/LICENSE
+-rw-r--r--   0        0        0       59 2022-06-08 19:53:51.796455 fabric_fss_utils-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0        0        0      851 2021-01-13 21:58:26.743332 fabric_fss_utils-1.5.0rc1/README.md
+-rw-r--r--   0        0        0      121 2023-05-10 22:00:20.624356 fabric_fss_utils-1.5.0rc1/fss_utils/__init__.py
+-rw-r--r--   0        0        0     3290 2021-05-05 20:19:27.853971 fabric_fss_utils-1.5.0rc1/fss_utils/http_errors.py
+-rw-r--r--   0        0        0     8288 2023-05-10 21:50:19.899928 fabric_fss_utils-1.5.0rc1/fss_utils/jwt_manager.py
+-rw-r--r--   0        0        0     3678 2021-01-13 21:34:16.970111 fabric_fss_utils-1.5.0rc1/fss_utils/jwt_validate.py
+-rw-r--r--   0        0        0     8429 2022-06-08 19:53:51.802302 fabric_fss_utils-1.5.0rc1/fss_utils/sshkey.py
+-rw-r--r--   0        0        0     5090 2021-01-13 21:34:16.970600 fabric_fss_utils-1.5.0rc1/fss_utils/vouch_encoder.py
+-rw-r--r--   0        0        0      776 2023-05-10 21:56:38.451610 fabric_fss_utils-1.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-05-10 21:58:14.762074 fabric_fss_utils-1.5.0rc1/requirements.txt
+-rw-r--r--   0        0        0      826 2022-06-08 17:21:57.693221 fabric_fss_utils-1.5.0rc1/setup.py
+-rw-r--r--   0        0        0        2 2020-12-13 06:15:01.062052 fabric_fss_utils-1.5.0rc1/test/__init__.py
+-rw-r--r--   0        0        0     3272 2021-01-13 21:34:16.972211 fabric_fss_utils-1.5.0rc1/test/data/privkey.pem
+-rw-r--r--   0        0        0      800 2021-01-13 21:34:16.972648 fabric_fss_utils-1.5.0rc1/test/data/pubkey.pem
+-rw-r--r--   0        0        0     7811 2023-05-10 21:39:23.714894 fabric_fss_utils-1.5.0rc1/test/jwt_decode_test.py
+-rw-r--r--   0        0        0     4583 2023-05-10 21:33:57.843225 fabric_fss_utils-1.5.0rc1/test/jwt_manager_test.py
+-rw-r--r--   0        0        0     6964 2022-01-09 16:48:43.909205 fabric_fss_utils-1.5.0rc1/test/ssh_test.py
+-rw-r--r--   0        0        0     9404 2021-01-13 21:34:16.974329 fabric_fss_utils-1.5.0rc1/test/vouch_encoder_test.py
+-rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 fabric_fss_utils-1.5.0rc1/PKG-INFO
```

### Comparing `fabric_fss_utils-1.4.0/LICENSE` & `fabric_fss_utils-1.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.4.0/README.md` & `fabric_fss_utils-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.4.0/fss_utils/http_errors.py` & `fabric_fss_utils-1.5.0rc1/fss_utils/http_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.4.0/fss_utils/jwt_manager.py` & `fabric_fss_utils-1.5.0rc1/fss_utils/jwt_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 import enum
 import gzip
 import traceback
 from datetime import timedelta, datetime
 from typing import Tuple, Union
 
 import jwt
-from authlib.jose import jwk
+#from authlib.jose import jwk
+from authlib.jose.rfc7517 import JsonWebKey
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 
 
 @enum.unique
 class ValidateCode(enum.Enum):
     VALID = 1
@@ -102,15 +103,15 @@
         except Exception as e:
             return ValidateCode.UNABLE_TO_LOAD_KEYS, e
 
         claims['iat'] = int(datetime.now().timestamp())
         claims['exp'] = int((datetime.now() + timedelta(seconds=int(validity))).timestamp())
 
         try:
-            encoded_token = str(jwt.encode(claims, private_key, algorithm=algorithm, headers={'kid': kid}), 'utf-8')
+            encoded_token = jwt.encode(claims, private_key, algorithm=algorithm, headers={'kid': kid})
             return ValidateCode.VALID, encoded_token
         except Exception as e:
             return ValidateCode.INVALID, e
 
     @staticmethod
     def encode_jwk(*, key_file_name: str, kid: str, alg: str) -> Tuple[ValidateCode, Union[Exception, dict]]:
         """
@@ -126,15 +127,17 @@
             with open(key_file_name) as public_key_fh:
                 pem_data = public_key_fh.read()
                 public_key_fh.close()
         except Exception as e:
             return ValidateCode.UNABLE_TO_LOAD_KEYS, e
 
         try:
-            result = jwk.dumps(pem_data, kty='RSA')
+            # deprecated
+            #result = authlib.jose.jwk.dumps(pem_data, kty='RSA')
+            result = dict(JsonWebKey.import_key(pem_data, options={'kty': 'RSA'}))
             result["kid"] = kid
             result["alg"] = alg
             result["use"] = "sig"
             return ValidateCode.VALID, result
         except Exception as e:
             return ValidateCode.INVALID, e
 
@@ -152,23 +155,25 @@
         :return ValidateCode or None, exception or None, encoded token or None:
         """
         if validity is not None:
             claims['exp'] = int((datetime.now() + timedelta(seconds=int(validity))).timestamp())
 
         encoded_cookie = None
         try:
+            # produces a string
             encoded_cookie = jwt.encode(claims, secret, algorithm=algorithm)
         except Exception as e:
             return ValidateCode.INVALID, e
 
         try:
             if compression:
-                compressed_cookie = gzip.compress(encoded_cookie)
+                compressed_cookie = gzip.compress(bytes(encoded_cookie, 'utf-8'))
                 encoded_cookie = base64.urlsafe_b64encode(compressed_cookie)
-            encoded_cookie = str(encoded_cookie, 'utf-8')
+                # back to string
+                encoded_cookie = str(encoded_cookie, 'utf-8')
         except Exception as e:
             return ValidateCode.UNABLE_TO_COMPRESS, e
 
         return ValidateCode.VALID, encoded_cookie
 
     @staticmethod
     def decode(*, cookie: str, secret: str = '', verify: bool = True,
@@ -197,12 +202,12 @@
             traceback.print_exc()
             return ValidateCode.UNPARSABLE_TOKEN, e
 
         if algorithm is None:
             return ValidateCode.UNSPECIFIED_ALG, None
 
         try:
-            decoded_token = jwt.decode(cookie, secret, algorithms=[algorithm], verify=verify)
+            decoded_token = jwt.decode(cookie, secret, algorithms=[algorithm], options={'verify_signature': verify})
             return ValidateCode.VALID, decoded_token
         except Exception as e:
             traceback.print_exc()
             return ValidateCode.INVALID, e
```

### Comparing `fabric_fss_utils-1.4.0/fss_utils/jwt_validate.py` & `fabric_fss_utils-1.5.0rc1/fss_utils/jwt_validate.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.4.0/fss_utils/sshkey.py` & `fabric_fss_utils-1.5.0rc1/fss_utils/sshkey.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.4.0/fss_utils/vouch_encoder.py` & `fabric_fss_utils-1.5.0rc1/fss_utils/vouch_encoder.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.4.0/setup.py` & `fabric_fss_utils-1.5.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.4.0/test/jwt_decode_test.py` & `fabric_fss_utils-1.5.0rc1/test/jwt_decode_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         assert vc is ValidateCode.VALID
 
     def testNoExpiredWrongAudience(self):
         """ validate signature, ignore expiration, check audience (fail) """
         self.validator = JWTValidator(url=self.url, refresh_period=self.period,
                                       audience=self.wrong_audience)
         vc, e = self.validator.validate_jwt(token=self.testToken2)
-        assert vc is ValidateCode.INVALID and str(e) == "Invalid audience"
+        assert vc is ValidateCode.INVALID and str(e) == "Audience doesn't match"
 
     def testStrictExpired(self):
         """ test for expiration (fail) """
         # audience is set to None in this case
         vc, e = self.default_validator.validate_jwt(token=self.testToken2, verify_exp=True)
         assert vc is ValidateCode.INVALID and str(e) == "Signature has expired"
```

### Comparing `fabric_fss_utils-1.4.0/test/jwt_manager_test.py` & `fabric_fss_utils-1.5.0rc1/test/jwt_manager_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,24 +69,24 @@
         self.assertTrue(isinstance(token, dict))
 
     def test_encode_and_compress_enabled(self):
         claims = {"foo": "bar"}
         code, token = JWTManager.encode_and_compress(claims=claims, secret="super-secret", validity=500)
         self.assertEqual(code, ValidateCode.VALID)
 
-        code, decoded_token = JWTManager.decode(cookie=token, verify=False, compression=True)
+        code, decoded_token = JWTManager.decode(cookie=token, secret="super-secret", verify=True, compression=True)
 
         self.assertEqual(code, ValidateCode.VALID)
         for key, value in claims.items():
             self.assertIsNotNone(decoded_token.get(key), value)
 
     def test_encode_and_compress_disabled(self):
         claims = {"foo": "bar"}
         code, token = JWTManager.encode_and_compress(claims=claims, secret="super-secret", validity=500,
                                                      compression=False)
         self.assertEqual(code, ValidateCode.VALID)
 
-        code, decoded_token = JWTManager.decode(cookie=token, verify=False, compression=False)
+        code, decoded_token = JWTManager.decode(cookie=token, secret="super-secret", verify=True, compression=False)
 
         self.assertEqual(code, ValidateCode.VALID)
         for key, value in claims.items():
             self.assertIsNotNone(decoded_token.get(key), value)
```

### Comparing `fabric_fss_utils-1.4.0/test/ssh_test.py` & `fabric_fss_utils-1.5.0rc1/test/ssh_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.4.0/test/vouch_encoder_test.py` & `fabric_fss_utils-1.5.0rc1/test/vouch_encoder_test.py`

 * *Files identical despite different names*

