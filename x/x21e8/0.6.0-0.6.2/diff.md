# Comparing `tmp/x21e8-0.6.0.tar.gz` & `tmp/x21e8-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x21e8-0.6.0.tar", max compression
+gzip compressed data, was "x21e8-0.6.2.tar", max compression
```

## Comparing `x21e8-0.6.0.tar` & `x21e8-0.6.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     5030 2023-04-18 08:19:31.622657 x21e8-0.6.0/README.md
--rw-r--r--   0        0        0      740 2023-04-18 08:19:31.626656 x21e8-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/application/__init__.py
--rw-r--r--   0        0        0     6082 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/application/liquid.py
--rw-r--r--   0        0        0        1 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/application/notarize.py
--rw-r--r--   0        0        0     2409 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/application/planetmint.py
--rw-r--r--   0        0        0      398 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/application/rddl.py
--rw-r--r--   0        0        0     1743 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/application/token.py
--rw-r--r--   0        0        0      765 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/config.py
--rw-r--r--   0        0        0     1001 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/main.py
--rw-r--r--   0        0        0        0 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/models/__init__.py
--rw-r--r--   0        0        0      182 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/models/issuing_request.py
--rw-r--r--   0        0        0      188 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/models/nft_asset.py
--rw-r--r--   0        0        0      354 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/models/token_related_accounts.py
--rw-r--r--   0        0        0      494 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/models/transfer.py
--rw-r--r--   0        0        0        0 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/network/__init__.py
--rw-r--r--   0        0        0     2220 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/network/liquid/__init__.py
--rwxr-xr-x   0        0        0    97346 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/network/liquid/util.py
--rw-r--r--   0        0        0     1693 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/routers/assets.py
--rw-r--r--   0        0        0      375 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/routers/config.py
--rw-r--r--   0        0        0     1108 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/routers/data.py
--rw-r--r--   0        0        0     3892 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/routers/machine.py
--rw-r--r--   0        0        0      925 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/routers/seed.py
--rw-r--r--   0        0        0      630 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/routers/utils.py
--rw-r--r--   0        0        0      619 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/routers/wallet.py
--rw-r--r--   0        0        0        0 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/utils/__init__.py
--rw-r--r--   0        0        0      256 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/utils/cointype.py
--rw-r--r--   0        0        0     1035 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/utils/encryption.py
--rw-r--r--   0        0        0     1723 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/utils/storage.py
--rw-r--r--   0        0        0        0 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/wallet/__init__.py
--rw-r--r--   0        0        0      628 2023-04-18 08:19:31.626656 x21e8-0.6.0/x21e8/wallet/base_wallet.py
--rw-r--r--   0        0        0        0 2023-04-18 08:19:31.630656 x21e8-0.6.0/x21e8/wallet/planetmint/__init__.py
--rw-r--r--   0        0        0     2771 2023-04-18 08:19:31.630656 x21e8-0.6.0/x21e8/wallet/planetmint/keymanagement.py
--rw-r--r--   0        0        0     3231 2023-04-18 08:19:31.630656 x21e8-0.6.0/x21e8/wallet/planetmint/keystore.py
--rw-r--r--   0        0        0      720 2023-04-18 08:19:31.630656 x21e8-0.6.0/x21e8/wallet/seed.py
--rw-r--r--   0        0        0     4367 2023-04-18 08:19:31.630656 x21e8-0.6.0/x21e8/wallet/sw_wallet.py
--rw-r--r--   0        0        0     6039 1970-01-01 00:00:00.000000 x21e8-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     5030 2023-05-11 09:08:12.378145 x21e8-0.6.2/README.md
+-rw-r--r--   0        0        0      717 2023-05-11 09:08:12.386145 x21e8-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/application/__init__.py
+-rw-r--r--   0        0        0     6082 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/application/liquid.py
+-rw-r--r--   0        0        0        1 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/application/notarize.py
+-rw-r--r--   0        0        0     2409 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/application/planetmint.py
+-rw-r--r--   0        0        0      398 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/application/rddl.py
+-rw-r--r--   0        0        0     1743 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/application/token.py
+-rw-r--r--   0        0        0      765 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/config.py
+-rw-r--r--   0        0        0     1001 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/main.py
+-rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/models/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/models/issuing_request.py
+-rw-r--r--   0        0        0      188 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/models/nft_asset.py
+-rw-r--r--   0        0        0      354 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/models/token_related_accounts.py
+-rw-r--r--   0        0        0      494 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/models/transfer.py
+-rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/network/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/network/liquid/__init__.py
+-rwxr-xr-x   0        0        0    97346 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/network/liquid/util.py
+-rw-r--r--   0        0        0     1693 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/assets.py
+-rw-r--r--   0        0        0      375 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/config.py
+-rw-r--r--   0        0        0     1108 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/data.py
+-rw-r--r--   0        0        0     3892 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/machine.py
+-rw-r--r--   0        0        0      925 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/seed.py
+-rw-r--r--   0        0        0      630 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/utils.py
+-rw-r--r--   0        0        0      619 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/wallet.py
+-rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/utils/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/utils/cointype.py
+-rw-r--r--   0        0        0     1035 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/utils/encryption.py
+-rw-r--r--   0        0        0     2328 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/utils/storage.py
+-rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/__init__.py
+-rw-r--r--   0        0        0      628 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/base_wallet.py
+-rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/planetmint/__init__.py
+-rw-r--r--   0        0        0     2771 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/planetmint/keymanagement.py
+-rw-r--r--   0        0        0     3231 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/planetmint/keystore.py
+-rw-r--r--   0        0        0      720 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/seed.py
+-rw-r--r--   0        0        0     4367 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/sw_wallet.py
+-rw-r--r--   0        0        0     6001 1970-01-01 00:00:00.000000 x21e8-0.6.2/PKG-INFO
```

### Comparing `x21e8-0.6.0/README.md` & `x21e8-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/pyproject.toml` & `x21e8-0.6.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "x21e8"
-version = "0.6.0"
+version = "0.6.2"
 description = "x"
 authors = ["Firat Berk Cakar <firat@riddleandcode.com>", "Jürgen Eckel <juergen@riddleandcode.com"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 TrezorCryptoTestRc = "*" 
-wallycore = "0.8.6"
 mnemonic = "^0.20"
 fastapi = "^0.85.0"
 bitcoin-utils = "^0.5.6"
 w3storage = "^0.0.1"
 requests = ">2.20.0"
 mypy = "^0.982"
 python-decouple = "^3.6"
 pysha3 = "^1.0.2"
 python-rapidjson = ">1.0.0"
 python-rapidjson-schema = "0.1.1"
-planetmint-ipld = "^0.0.3"
+multiformats = "^0.2.1"
 uvicorn = "^0.19.0"
 planetmint-driver = "0.18.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 black = "^23.3.0"
```

### Comparing `x21e8-0.6.0/x21e8/application/liquid.py` & `x21e8-0.6.2/x21e8/application/liquid.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/application/planetmint.py` & `x21e8-0.6.2/x21e8/application/planetmint.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/application/token.py` & `x21e8-0.6.2/x21e8/application/token.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/config.py` & `x21e8-0.6.2/x21e8/config.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/main.py` & `x21e8-0.6.2/x21e8/main.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/network/liquid/__init__.py` & `x21e8-0.6.2/x21e8/network/liquid/__init__.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/network/liquid/util.py` & `x21e8-0.6.2/x21e8/network/liquid/util.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/routers/assets.py` & `x21e8-0.6.2/x21e8/routers/assets.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/routers/data.py` & `x21e8-0.6.2/x21e8/routers/data.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/routers/machine.py` & `x21e8-0.6.2/x21e8/routers/machine.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/routers/seed.py` & `x21e8-0.6.2/x21e8/routers/seed.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/routers/utils.py` & `x21e8-0.6.2/x21e8/routers/utils.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/routers/wallet.py` & `x21e8-0.6.2/x21e8/routers/wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/utils/encryption.py` & `x21e8-0.6.2/x21e8/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/utils/storage.py` & `x21e8-0.6.2/x21e8/utils/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,31 @@
+import json
 import urllib3
 import w3storage
 from urllib.request import urlopen
-from ipld import marshal, unmarshal, multihash
+from multiformats import CID, multihash
 
 from x21e8.config import WEB3STORAGE_TOKEN, CID_RESOLVER
 from x21e8.utils.encryption import encrypt_bytes, decrypt_2_bytes
 
+ENCODING = "utf-8"
+
 w3s = w3storage.API(token=WEB3STORAGE_TOKEN)
 
 
+def marshal(asset: dict):
+    # one line json without whitespaces as bytes
+    return bytes(json.dumps(asset, separators=(",", ":")), ENCODING)
+
+
+def unmarshal(marshalled_asset: bytes):
+    # unmarshal to dict
+    return json.loads(marshalled_asset.decode(ENCODING))
+
+
 def get_ipfs_link(cid: str):
     return "https://" + cid + ".ipfs.w3s.link"
 
 
 def register_cid_url(cid: str, url: str):
     http = urllib3.PoolManager()
     cid_resp = http.request(
@@ -46,11 +59,21 @@
 def store_asset(asset: dict, encrypt_data: bool = False):
     marshalled_asset = local_marshal(asset, encrypt_data)
     asset_cid = w3s.post_upload(marshalled_asset)
     register_cid_url(asset_cid, get_ipfs_link(asset_cid))
     return asset_cid
 
 
+def get_hashed_marshalled(marshalled_asset: bytes):
+    hashed_marshalled = CID.decode(multihash.digest(marshalled_asset, "sha2-256"))
+    return hashed_marshalled
+
+
+def get_cid_v1(hashed_marshalled: CID):
+    cid = hashed_marshalled.set(base="base32", version=1, codec="raw")
+    return cid
+
+
 def multi_hash(asset: dict, encrypt_data: bool = False):
     marshalled_asset = local_marshal(asset, encrypt_data)
-    hashed_marshalled = multihash(marshalled_asset)
-    return hashed_marshalled
+    hashed_marshalled = get_hashed_marshalled(marshalled_asset)
+    return str(hashed_marshalled)
```

### Comparing `x21e8-0.6.0/x21e8/wallet/base_wallet.py` & `x21e8-0.6.2/x21e8/wallet/base_wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/wallet/planetmint/keymanagement.py` & `x21e8-0.6.2/x21e8/wallet/planetmint/keymanagement.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/wallet/planetmint/keystore.py` & `x21e8-0.6.2/x21e8/wallet/planetmint/keystore.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/wallet/seed.py` & `x21e8-0.6.2/x21e8/wallet/seed.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/x21e8/wallet/sw_wallet.py` & `x21e8-0.6.2/x21e8/wallet/sw_wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.0/PKG-INFO` & `x21e8-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: x21e8
-Version: 0.6.0
+Version: 0.6.2
 Summary: x
 Author: Firat Berk Cakar
 Author-email: firat@riddleandcode.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: TrezorCryptoTestRc
 Requires-Dist: bitcoin-utils (>=0.5.6,<0.6.0)
 Requires-Dist: fastapi (>=0.85.0,<0.86.0)
 Requires-Dist: mnemonic (>=0.20,<0.21)
+Requires-Dist: multiformats (>=0.2.1,<0.3.0)
 Requires-Dist: mypy (>=0.982,<0.983)
 Requires-Dist: planetmint-driver (==0.18.2)
-Requires-Dist: planetmint-ipld (>=0.0.3,<0.0.4)
 Requires-Dist: pysha3 (>=1.0.2,<2.0.0)
 Requires-Dist: python-decouple (>=3.6,<4.0)
 Requires-Dist: python-rapidjson (>1.0.0)
 Requires-Dist: python-rapidjson-schema (==0.1.1)
 Requires-Dist: requests (>2.20.0)
 Requires-Dist: uvicorn (>=0.19.0,<0.20.0)
 Requires-Dist: w3storage (>=0.0.1,<0.0.2)
-Requires-Dist: wallycore (==0.8.6)
 Description-Content-Type: text/markdown
 
 # 0x21e8 RDDL Interaction Service
 
 The 0x21e8 service is usually installed and executed on RDDL compatible hardware wallets (HW-03). The service utilizes the hardware wallet and enables the HW-03 devices to interact with the RDDL network (Planetmint and liquid). 
 
 Besides the pure wallet functionality it works as the core service to launch any RDDL specific use cases:
```

