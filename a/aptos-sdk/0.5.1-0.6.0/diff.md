# Comparing `tmp/aptos_sdk-0.5.1.tar.gz` & `tmp/aptos_sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aptos_sdk-0.5.1.tar", last modified: Mon Jan  2 17:37:09 2023, max compression
+gzip compressed data, was "aptos_sdk-0.6.0.tar", max compression
```

## Comparing `aptos_sdk-0.5.1.tar` & `aptos_sdk-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,13 @@
-drwxr-xr-x   0 davidiw   (1000) davidiw   (1000)        0 2023-01-02 17:37:09.336048 aptos_sdk-0.5.1/
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)     2914 2023-01-02 17:37:09.336048 aptos_sdk-0.5.1/PKG-INFO
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)     2529 2022-12-19 20:18:36.000000 aptos_sdk-0.5.1/README.md
-drwxr-xr-x   0 davidiw   (1000) davidiw   (1000)        0 2023-01-02 17:37:09.336048 aptos_sdk-0.5.1/aptos_sdk/
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)       60 2022-10-03 20:57:09.000000 aptos_sdk-0.5.1/aptos_sdk/__init__.py
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)     3005 2022-12-19 20:18:36.000000 aptos_sdk-0.5.1/aptos_sdk/account.py
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)     1544 2022-12-19 20:18:36.000000 aptos_sdk-0.5.1/aptos_sdk/account_address.py
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)     5611 2022-12-19 20:18:36.000000 aptos_sdk-0.5.1/aptos_sdk/authenticator.py
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)    10437 2023-01-02 01:28:52.000000 aptos_sdk-0.5.1/aptos_sdk/bcs.py
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)    23358 2023-01-02 01:28:52.000000 aptos_sdk-0.5.1/aptos_sdk/client.py
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)     4400 2023-01-02 01:28:52.000000 aptos_sdk-0.5.1/aptos_sdk/ed25519.py
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)    26572 2023-01-02 01:28:52.000000 aptos_sdk-0.5.1/aptos_sdk/transactions.py
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)     8981 2023-01-02 01:28:52.000000 aptos_sdk-0.5.1/aptos_sdk/type_tag.py
-drwxr-xr-x   0 davidiw   (1000) davidiw   (1000)        0 2023-01-02 17:37:09.336048 aptos_sdk-0.5.1/aptos_sdk.egg-info/
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)     2914 2023-01-02 17:37:09.000000 aptos_sdk-0.5.1/aptos_sdk.egg-info/PKG-INFO
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)      402 2023-01-02 17:37:09.000000 aptos_sdk-0.5.1/aptos_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)        1 2023-01-02 17:37:09.000000 aptos_sdk-0.5.1/aptos_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)       13 2023-01-02 17:37:09.000000 aptos_sdk-0.5.1/aptos_sdk.egg-info/requires.txt
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)       10 2023-01-02 17:37:09.000000 aptos_sdk-0.5.1/aptos_sdk.egg-info/top_level.txt
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)      532 2023-01-02 17:35:43.000000 aptos_sdk-0.5.1/pyproject.toml
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)       38 2023-01-02 17:37:09.336048 aptos_sdk-0.5.1/setup.cfg
--rw-r--r--   0 davidiw   (1000) davidiw   (1000)      691 2023-01-02 17:35:37.000000 aptos_sdk-0.5.1/setup.py
+-rw-r--r--   0        0        0       70 2023-03-25 17:54:29.320812 aptos_sdk-0.6.0/aptos_sdk/__init__.py
+-rw-r--r--   0        0        0     5651 2023-03-31 16:40:44.468580 aptos_sdk-0.6.0/aptos_sdk/account.py
+-rw-r--r--   0        0        0     5873 2023-05-10 13:54:28.475480 aptos_sdk-0.6.0/aptos_sdk/account_address.py
+-rw-r--r--   0        0        0    18891 2023-05-10 13:54:28.476911 aptos_sdk-0.6.0/aptos_sdk/aptos_token_client.py
+-rw-r--r--   0        0        0    26404 2023-05-10 13:54:28.477184 aptos_sdk-0.6.0/aptos_sdk/async_client.py
+-rw-r--r--   0        0        0     5811 2023-03-31 16:40:44.469044 aptos_sdk-0.6.0/aptos_sdk/authenticator.py
+-rw-r--r--   0        0        0    10447 2023-03-25 17:54:29.321178 aptos_sdk-0.6.0/aptos_sdk/bcs.py
+-rw-r--r--   0        0        0    24234 2023-05-10 13:54:28.477387 aptos_sdk-0.6.0/aptos_sdk/client.py
+-rw-r--r--   0        0        0    12056 2023-03-31 16:40:44.469357 aptos_sdk-0.6.0/aptos_sdk/ed25519.py
+-rw-r--r--   0        0        0    26552 2023-05-10 13:54:28.477553 aptos_sdk-0.6.0/aptos_sdk/transactions.py
+-rw-r--r--   0        0        0     8991 2023-03-25 17:54:29.321627 aptos_sdk-0.6.0/aptos_sdk/type_tag.py
+-rw-r--r--   0        0        0      530 2023-04-03 11:14:59.629687 aptos_sdk-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 aptos_sdk-0.6.0/PKG-INFO
```

### Comparing `aptos_sdk-0.5.1/aptos_sdk/authenticator.py` & `aptos_sdk-0.6.0/aptos_sdk/authenticator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Aptos
+# Copyright © Aptos Foundation
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import typing
 from typing import List
 
@@ -142,19 +142,24 @@
     def serialize(self, serializer: Serializer):
         serializer.struct(self.sender)
         serializer.sequence([x[0] for x in self.secondary_signers], Serializer.struct)
         serializer.sequence([x[1] for x in self.secondary_signers], Serializer.struct)
 
 
 class MultiEd25519Authenticator:
-    def __init__(self):
-        raise NotImplementedError
+    public_key: ed25519.MultiPublicKey
+    signature: ed25519.MultiSignature
+
+    def __init__(self, public_key, signature):
+        self.public_key = public_key
+        self.signature = signature
 
     def verify(self, data: bytes) -> bool:
         raise NotImplementedError
 
     @staticmethod
     def deserialize(deserializer: Deserializer) -> MultiEd25519Authenticator:
         raise NotImplementedError
 
     def serialize(self, serializer: Serializer):
-        raise NotImplementedError
+        serializer.struct(self.public_key)
+        serializer.struct(self.signature)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aptos_sdk-0.5.1/aptos_sdk/bcs.py` & `aptos_sdk-0.6.0/aptos_sdk/bcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Aptos
+# Copyright © Aptos Foundation
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This is a simple BCS serializer and deserializer. Learn more at https://github.com/diem/bcs
 """
 
 from __future__ import annotations
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aptos_sdk-0.5.1/aptos_sdk/client.py` & `aptos_sdk-0.6.0/aptos_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-# Copyright (c) Aptos
+# Copyright © Aptos Foundation
 # SPDX-License-Identifier: Apache-2.0
 
 import time
 from typing import Any, Dict, List
 
 import httpx
 
 from . import ed25519
 from .account import Account
 from .account_address import AccountAddress
-from .authenticator import (Authenticator, Ed25519Authenticator,
-                            MultiAgentAuthenticator)
+from .authenticator import Authenticator, Ed25519Authenticator, MultiAgentAuthenticator
 from .bcs import Serializer
-from .transactions import (EntryFunction, MultiAgentRawTransaction,
-                           RawTransaction, SignedTransaction,
-                           TransactionArgument, TransactionPayload)
+from .transactions import (
+    EntryFunction,
+    MultiAgentRawTransaction,
+    RawTransaction,
+    SignedTransaction,
+    TransactionArgument,
+    TransactionPayload,
+)
 from .type_tag import StructTag, TypeTag
 
 U64_MAX = 18446744073709551615
 
 
 class ClientConfig:
     """Common configuration for clients, particularly for submitting transactions"""
@@ -46,50 +50,82 @@
     def close(self):
         self.client.close()
 
     #
     # Account accessors
     #
 
-    def account(self, account_address: AccountAddress) -> Dict[str, str]:
+    def account(
+        self, account_address: AccountAddress, ledger_version: int = None
+    ) -> Dict[str, str]:
         """Returns the sequence number and authentication key for an account"""
 
-        response = self.client.get(f"{self.base_url}/accounts/{account_address}")
+        if not ledger_version:
+            request = f"{self.base_url}/accounts/{account_address}"
+        else:
+            request = f"{self.base_url}/accounts/{account_address}?ledger_version={ledger_version}"
+
+        response = self.client.get(request)
         if response.status_code >= 400:
             raise ApiError(f"{response.text} - {account_address}", response.status_code)
         return response.json()
 
-    def account_balance(self, account_address: AccountAddress) -> int:
+    def account_balance(
+        self, account_address: AccountAddress, ledger_version: int = None
+    ) -> int:
         """Returns the test coin balance associated with the account"""
         resource = self.account_resource(
-            account_address, "0x1::coin::CoinStore<0x1::aptos_coin::AptosCoin>"
+            account_address,
+            "0x1::coin::CoinStore<0x1::aptos_coin::AptosCoin>",
+            ledger_version,
         )
         return resource["data"]["coin"]["value"]
 
-    def account_sequence_number(self, account_address: AccountAddress) -> int:
-        account_res = self.account(account_address)
+    def account_sequence_number(
+        self, account_address: AccountAddress, ledger_version: int = None
+    ) -> int:
+        account_res = self.account(account_address, ledger_version)
         return int(account_res["sequence_number"])
 
     def account_resource(
-        self, account_address: AccountAddress, resource_type: str
+        self,
+        account_address: AccountAddress,
+        resource_type: str,
+        ledger_version: int = None,
     ) -> Dict[str, Any]:
-        response = self.client.get(
-            f"{self.base_url}/accounts/{account_address}/resource/{resource_type}"
-        )
+        if not ledger_version:
+            request = (
+                f"{self.base_url}/accounts/{account_address}/resource/{resource_type}"
+            )
+        else:
+            request = f"{self.base_url}/accounts/{account_address}/resource/{resource_type}?ledger_version={ledger_version}"
+
+        response = self.client.get(request)
         if response.status_code == 404:
             raise ResourceNotFound(resource_type, resource_type)
         if response.status_code >= 400:
             raise ApiError(f"{response.text} - {account_address}", response.status_code)
         return response.json()
 
     def get_table_item(
-        self, handle: str, key_type: str, value_type: str, key: Any
+        self,
+        handle: str,
+        key_type: str,
+        value_type: str,
+        key: Any,
+        ledger_version: int = None,
     ) -> Any:
+        if not ledger_version:
+            request = f"{self.base_url}/tables/{handle}/item"
+        else:
+            request = (
+                f"{self.base_url}/tables/{handle}/item?ledger_version={ledger_version}"
+            )
         response = self.client.post(
-            f"{self.base_url}/tables/{handle}/item",
+            request,
             json={
                 "key_type": key_type,
                 "value_type": value_type,
                 "key": key,
             },
         )
         if response.status_code >= 400:
@@ -327,15 +363,15 @@
 
     def transfer(self, sender: Account, recipient: AccountAddress, amount: int) -> str:
         """Transfer a given coin amount from a given Account to the recipient's account address.
         Returns the sequence number of the transaction used to transfer."""
 
         payload = {
             "type": "entry_function_payload",
-            "function": "0x1::coin::transfer",
+            "function": "0x1::aptos_account::transfer_coins",
             "type_arguments": ["0x1::aptos_coin::AptosCoin"],
             "arguments": [
                 f"{recipient}",
                 str(amount),
             ],
         }
         return self.submit_transaction(sender, payload)
@@ -346,16 +382,16 @@
     ) -> str:
         transaction_arguments = [
             TransactionArgument(recipient, Serializer.struct),
             TransactionArgument(amount, Serializer.u64),
         ]
 
         payload = EntryFunction.natural(
-            "0x1::coin",
-            "transfer",
+            "0x1::aptos_account",
+            "transfer_coins",
             [TypeTag(StructTag.from_str("0x1::aptos_coin::AptosCoin"))],
             transaction_arguments,
         )
 
         signed_transaction = self.create_bcs_signed_transaction(
             sender, TransactionPayload(payload)
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aptos_sdk-0.5.1/aptos_sdk/transactions.py` & `aptos_sdk-0.6.0/aptos_sdk/transactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Aptos
+# Copyright © Aptos Foundation
 # SPDX-License-Identifier: Apache-2.0
 
 """
 This translates Aptos transactions to and from BCS for signing and submitting to the REST API.
 """
 
 from __future__ import annotations
@@ -10,16 +10,15 @@
 import hashlib
 import typing
 import unittest
 from typing import List
 
 from . import ed25519
 from .account_address import AccountAddress
-from .authenticator import (Authenticator, Ed25519Authenticator,
-                            MultiAgentAuthenticator)
+from .authenticator import Authenticator, Ed25519Authenticator, MultiAgentAuthenticator
 from .bcs import Deserializer, Serializer
 from .type_tag import StructTag, TypeTag
 
 
 class RawTransaction:
     # Sender's address
     sender: AccountAddress
@@ -65,15 +64,15 @@
             and self.max_gas_amount == other.max_gas_amount
             and self.gas_unit_price == other.gas_unit_price
             and self.expiration_timestamps_secs == other.expiration_timestamps_secs
             and self.chain_id == other.chain_id
         )
 
     def __str__(self):
-        return f"""RawTranasction:
+        return f"""RawTransaction:
     sender: {self.sender}
     sequence_number: {self.sequence_number}
     payload: {self.payload}
     max_gas_amount: {self.max_gas_amount}
     gas_unit_price: {self.gas_unit_price}
     expiration_timestamps_secs: {self.expiration_timestamps_secs}
     chain_id: {self.chain_id}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aptos_sdk-0.5.1/aptos_sdk/type_tag.py` & `aptos_sdk-0.6.0/aptos_sdk/type_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Aptos
+# Copyright © Aptos Foundation
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import typing
 from typing import List
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

