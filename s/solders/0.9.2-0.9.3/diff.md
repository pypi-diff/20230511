# Comparing `tmp/solders-0.9.2.tar.gz` & `tmp/solders-0.9.3.tar.gz`

## Comparing `solders-0.9.2.tar` & `solders-0.9.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 solders-0.9.2/Cargo.toml
--rw-r--r--   0     1001      121    11357 2022-10-14 22:44:47.000000 solders-0.9.2/LICENSE
--rw-r--r--   0     1001      121     1946 2022-10-14 22:44:47.000000 solders-0.9.2/README.md
--rw-r--r--   0     1001      121     1344 2022-10-14 22:44:47.000000 solders-0.9.2/pyproject.toml
--rw-r--r--   0     1001      121     6877 2022-10-14 22:44:47.000000 solders-0.9.2/src/account.rs
--rw-r--r--   0     1001      121     4539 2022-10-14 22:44:47.000000 solders-0.9.2/src/account_decoder.rs
--rw-r--r--   0     1001      121     2174 2022-10-14 22:44:47.000000 solders-0.9.2/src/address_lookup_table_account.rs
--rw-r--r--   0     1001      121     5978 2022-10-14 22:44:47.000000 solders-0.9.2/src/commitment_config.rs
--rw-r--r--   0     1001      121     3738 2022-10-14 22:44:47.000000 solders-0.9.2/src/epoch_schedule.rs
--rw-r--r--   0     1001      121     4219 2022-10-14 22:44:47.000000 solders-0.9.2/src/hash.rs
--rw-r--r--   0     1001      121    12605 2022-10-14 22:44:47.000000 solders-0.9.2/src/instruction.rs
--rw-r--r--   0     1001      121     8179 2022-10-14 22:44:47.000000 solders-0.9.2/src/keypair.rs
--rw-r--r--   0     1001      121    14806 2022-10-14 22:44:47.000000 solders-0.9.2/src/lib.rs
--rw-r--r--   0     1001      121    33817 2022-10-14 22:44:47.000000 solders-0.9.2/src/message.rs
--rw-r--r--   0     1001      121     3641 2022-10-14 22:44:47.000000 solders-0.9.2/src/null_signer.rs
--rw-r--r--   0     1001      121     3304 2022-10-14 22:44:47.000000 solders-0.9.2/src/presigner.rs
--rw-r--r--   0     1001      121     9420 2022-10-14 22:44:47.000000 solders-0.9.2/src/pubkey.rs
--rw-r--r--   0     1001      121    45314 2022-10-14 22:44:47.000000 solders-0.9.2/src/rpc/config.rs
--rw-r--r--   0     1001      121    12780 2022-10-14 22:44:47.000000 solders-0.9.2/src/rpc/errors.rs
--rw-r--r--   0     1001      121     4500 2022-10-14 22:44:47.000000 solders-0.9.2/src/rpc/filter.rs
--rw-r--r--   0     1001      121     1208 2022-10-14 22:44:47.000000 solders-0.9.2/src/rpc/mod.rs
--rw-r--r--   0     1001      121    98962 2022-10-14 22:44:47.000000 solders-0.9.2/src/rpc/requests.rs
--rw-r--r--   0     1001      121   106527 2022-10-14 22:44:47.000000 solders-0.9.2/src/rpc/responses.rs
--rw-r--r--   0     1001      121    11061 2022-10-14 22:44:47.000000 solders-0.9.2/src/rpc/tmp_config.rs
--rw-r--r--   0     1001      121     8838 2022-10-14 22:44:47.000000 solders-0.9.2/src/rpc/tmp_filter.rs
--rw-r--r--   0     1001      121    13286 2022-10-14 22:44:47.000000 solders-0.9.2/src/rpc/tmp_response.rs
--rw-r--r--   0     1001      121     4860 2022-10-14 22:44:47.000000 solders-0.9.2/src/signature.rs
--rw-r--r--   0     1001      121     2174 2022-10-14 22:44:47.000000 solders-0.9.2/src/signer.rs
--rw-r--r--   0     1001      121    20432 2022-10-14 22:44:47.000000 solders-0.9.2/src/system_program.rs
--rw-r--r--   0     1001      121      840 2022-10-14 22:44:47.000000 solders-0.9.2/src/sysvar.rs
--rw-r--r--   0     1001      121     2933 2022-10-14 22:44:47.000000 solders-0.9.2/src/tmp_account_decoder.rs
--rw-r--r--   0     1001      121    11583 2022-10-14 22:44:47.000000 solders-0.9.2/src/tmp_transaction_status.rs
--rw-r--r--   0     1001      121    29418 2022-10-14 22:44:47.000000 solders-0.9.2/src/transaction.rs
--rw-r--r--   0     1001      121    69005 2022-10-14 22:44:47.000000 solders-0.9.2/src/transaction_status.rs
--rw-r--r--   0     1001      121    46242 2022-10-14 22:44:47.000000 solders-0.9.2/Cargo.lock
--rw-r--r--   0     1001      121     2274 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/instruction.pyi
--rw-r--r--   0     1001      121     1021 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/commitment_config.pyi
--rw-r--r--   0     1001      121      272 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/_sysvar.pyi
--rw-r--r--   0     1001      121      715 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/address_lookup_table_account.pyi
--rw-r--r--   0     1001      121        0 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/py.typed
--rw-r--r--   0     1001      121     2375 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/_system_program.pyi
--rw-r--r--   0     1001      121      138 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/errors.pyi
--rw-r--r--   0     1001      121     1785 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/account.pyi
--rw-r--r--   0     1001      121    25733 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/transaction_status.pyi
--rw-r--r--   0     1001      121     5913 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/message.pyi
--rw-r--r--   0     1001      121     1388 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/epoch_schedule.pyi
--rw-r--r--   0     1001      121     1133 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/keypair.pyi
--rw-r--r--   0     1001      121     1673 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/sysvar.py
--rw-r--r--   0     1001      121     4592 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/transaction.pyi
--rw-r--r--   0     1001      121      754 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/hash.pyi
--rw-r--r--   0     1001      121      566 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/presigner.pyi
--rw-r--r--   0     1001      121      757 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/__init__.py
--rw-r--r--   0     1001      121      874 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/signature.pyi
--rw-r--r--   0     1001      121    19266 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/rpc/config.pyi
--rw-r--r--   0     1001      121    15660 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/rpc/errors.pyi
--rw-r--r--   0     1001      121    76037 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/rpc/responses.pyi
--rw-r--r--   0     1001      121      880 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/rpc/filter.pyi
--rw-r--r--   0     1001      121        0 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/rpc/__init__.pyi
--rw-r--r--   0     1001      121    47665 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/rpc/requests.pyi
--rw-r--r--   0     1001      121      791 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/null_signer.pyi
--rw-r--r--   0     1001      121    18736 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/system_program.py
--rw-r--r--   0     1001      121     1171 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/pubkey.pyi
--rw-r--r--   0     1001      121     2027 2022-10-14 22:44:47.000000 solders-0.9.2/python/solders/account_decoder.pyi
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 solders-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 solders-0.9.3/Cargo.toml
+-rw-r--r--   0     1001      121    11357 2022-10-15 00:32:00.000000 solders-0.9.3/LICENSE
+-rw-r--r--   0     1001      121     1946 2022-10-15 00:32:00.000000 solders-0.9.3/README.md
+-rw-r--r--   0     1001      121     1344 2022-10-15 00:32:00.000000 solders-0.9.3/pyproject.toml
+-rw-r--r--   0     1001      121     6877 2022-10-15 00:32:00.000000 solders-0.9.3/src/account.rs
+-rw-r--r--   0     1001      121     4539 2022-10-15 00:32:00.000000 solders-0.9.3/src/account_decoder.rs
+-rw-r--r--   0     1001      121     2174 2022-10-15 00:32:00.000000 solders-0.9.3/src/address_lookup_table_account.rs
+-rw-r--r--   0     1001      121     5978 2022-10-15 00:32:00.000000 solders-0.9.3/src/commitment_config.rs
+-rw-r--r--   0     1001      121     3738 2022-10-15 00:32:00.000000 solders-0.9.3/src/epoch_schedule.rs
+-rw-r--r--   0     1001      121     4219 2022-10-15 00:32:00.000000 solders-0.9.3/src/hash.rs
+-rw-r--r--   0     1001      121    12605 2022-10-15 00:32:00.000000 solders-0.9.3/src/instruction.rs
+-rw-r--r--   0     1001      121     8179 2022-10-15 00:32:00.000000 solders-0.9.3/src/keypair.rs
+-rw-r--r--   0     1001      121    14806 2022-10-15 00:32:00.000000 solders-0.9.3/src/lib.rs
+-rw-r--r--   0     1001      121    33817 2022-10-15 00:32:00.000000 solders-0.9.3/src/message.rs
+-rw-r--r--   0     1001      121     3641 2022-10-15 00:32:00.000000 solders-0.9.3/src/null_signer.rs
+-rw-r--r--   0     1001      121     3304 2022-10-15 00:32:00.000000 solders-0.9.3/src/presigner.rs
+-rw-r--r--   0     1001      121     9420 2022-10-15 00:32:00.000000 solders-0.9.3/src/pubkey.rs
+-rw-r--r--   0     1001      121    45314 2022-10-15 00:32:00.000000 solders-0.9.3/src/rpc/config.rs
+-rw-r--r--   0     1001      121    12780 2022-10-15 00:32:00.000000 solders-0.9.3/src/rpc/errors.rs
+-rw-r--r--   0     1001      121     4500 2022-10-15 00:32:00.000000 solders-0.9.3/src/rpc/filter.rs
+-rw-r--r--   0     1001      121     1208 2022-10-15 00:32:00.000000 solders-0.9.3/src/rpc/mod.rs
+-rw-r--r--   0     1001      121    98962 2022-10-15 00:32:00.000000 solders-0.9.3/src/rpc/requests.rs
+-rw-r--r--   0     1001      121   106527 2022-10-15 00:32:00.000000 solders-0.9.3/src/rpc/responses.rs
+-rw-r--r--   0     1001      121    11061 2022-10-15 00:32:00.000000 solders-0.9.3/src/rpc/tmp_config.rs
+-rw-r--r--   0     1001      121     8838 2022-10-15 00:32:00.000000 solders-0.9.3/src/rpc/tmp_filter.rs
+-rw-r--r--   0     1001      121    13286 2022-10-15 00:32:00.000000 solders-0.9.3/src/rpc/tmp_response.rs
+-rw-r--r--   0     1001      121     4860 2022-10-15 00:32:00.000000 solders-0.9.3/src/signature.rs
+-rw-r--r--   0     1001      121     2174 2022-10-15 00:32:00.000000 solders-0.9.3/src/signer.rs
+-rw-r--r--   0     1001      121    20432 2022-10-15 00:32:00.000000 solders-0.9.3/src/system_program.rs
+-rw-r--r--   0     1001      121      840 2022-10-15 00:32:00.000000 solders-0.9.3/src/sysvar.rs
+-rw-r--r--   0     1001      121     2933 2022-10-15 00:32:00.000000 solders-0.9.3/src/tmp_account_decoder.rs
+-rw-r--r--   0     1001      121    11583 2022-10-15 00:32:00.000000 solders-0.9.3/src/tmp_transaction_status.rs
+-rw-r--r--   0     1001      121    29418 2022-10-15 00:32:00.000000 solders-0.9.3/src/transaction.rs
+-rw-r--r--   0     1001      121    69766 2022-10-15 00:32:00.000000 solders-0.9.3/src/transaction_status.rs
+-rw-r--r--   0     1001      121    46242 2022-10-15 00:32:00.000000 solders-0.9.3/Cargo.lock
+-rw-r--r--   0     1001      121     2274 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/instruction.pyi
+-rw-r--r--   0     1001      121     1021 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/commitment_config.pyi
+-rw-r--r--   0     1001      121      272 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/_sysvar.pyi
+-rw-r--r--   0     1001      121      715 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/address_lookup_table_account.pyi
+-rw-r--r--   0     1001      121        0 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/py.typed
+-rw-r--r--   0     1001      121     2375 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/_system_program.pyi
+-rw-r--r--   0     1001      121      138 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/errors.pyi
+-rw-r--r--   0     1001      121     1785 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/account.pyi
+-rw-r--r--   0     1001      121    25733 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/transaction_status.pyi
+-rw-r--r--   0     1001      121     5913 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/message.pyi
+-rw-r--r--   0     1001      121     1388 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/epoch_schedule.pyi
+-rw-r--r--   0     1001      121     1133 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/keypair.pyi
+-rw-r--r--   0     1001      121     1673 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/sysvar.py
+-rw-r--r--   0     1001      121     4592 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/transaction.pyi
+-rw-r--r--   0     1001      121      754 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/hash.pyi
+-rw-r--r--   0     1001      121      566 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/presigner.pyi
+-rw-r--r--   0     1001      121      757 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/__init__.py
+-rw-r--r--   0     1001      121      874 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/signature.pyi
+-rw-r--r--   0     1001      121    19266 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/rpc/config.pyi
+-rw-r--r--   0     1001      121    15660 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/rpc/errors.pyi
+-rw-r--r--   0     1001      121    76037 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/rpc/responses.pyi
+-rw-r--r--   0     1001      121      880 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/rpc/filter.pyi
+-rw-r--r--   0     1001      121        0 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/rpc/__init__.pyi
+-rw-r--r--   0     1001      121    47665 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/rpc/requests.pyi
+-rw-r--r--   0     1001      121      791 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/null_signer.pyi
+-rw-r--r--   0     1001      121    18736 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/system_program.py
+-rw-r--r--   0     1001      121     1171 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/pubkey.pyi
+-rw-r--r--   0     1001      121     2027 2022-10-15 00:32:00.000000 solders-0.9.3/python/solders/account_decoder.pyi
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 solders-0.9.3/PKG-INFO
```

### Comparing `solders-0.9.2/Cargo.toml` & `solders-0.9.3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "solders"
-version = "0.9.2"
+version = "0.9.3"
 edition = "2021"
 include = ["/src", "/LICENSE", "/pyproject.toml"]
 description = "Python binding to the Solana Rust SDK"
 license = "MIT"
 repository = "https://github.com/kevinheavey/solders"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `solders-0.9.2/LICENSE` & `solders-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/README.md` & `solders-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/pyproject.toml` & `solders-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solders"
-version = "0.9.2"
+version = "0.9.3"
 description = "Python bindings for Solana Rust tools"
 authors = ["kevinheavey <kevinheavey123@gmail.com>"]
 license = "Apache"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
@@ -25,15 +25,15 @@
 [build-system]
 requires = ["maturin>=0.13.2,<0.14"]
 build-backend = "maturin"
 
 
 [project]
 name = "solders"
-version = "0.9.2"
+version = "0.9.3"
 description = "Python binding to the Solana Rust SDK"
 authors = [ {name = "kevinheavey", email = "kevinheavey123@gmail.com"} ]
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `solders-0.9.2/src/account.rs` & `solders-0.9.3/src/account.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/account_decoder.rs` & `solders-0.9.3/src/account_decoder.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/address_lookup_table_account.rs` & `solders-0.9.3/src/address_lookup_table_account.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/commitment_config.rs` & `solders-0.9.3/src/commitment_config.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/epoch_schedule.rs` & `solders-0.9.3/src/epoch_schedule.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/hash.rs` & `solders-0.9.3/src/hash.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/instruction.rs` & `solders-0.9.3/src/instruction.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/keypair.rs` & `solders-0.9.3/src/keypair.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/lib.rs` & `solders-0.9.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/message.rs` & `solders-0.9.3/src/message.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/null_signer.rs` & `solders-0.9.3/src/null_signer.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/presigner.rs` & `solders-0.9.3/src/presigner.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/pubkey.rs` & `solders-0.9.3/src/pubkey.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/rpc/config.rs` & `solders-0.9.3/src/rpc/config.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/rpc/errors.rs` & `solders-0.9.3/src/rpc/errors.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/rpc/filter.rs` & `solders-0.9.3/src/rpc/filter.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/rpc/mod.rs` & `solders-0.9.3/src/rpc/mod.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/rpc/requests.rs` & `solders-0.9.3/src/rpc/requests.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/rpc/responses.rs` & `solders-0.9.3/src/rpc/responses.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/rpc/tmp_config.rs` & `solders-0.9.3/src/rpc/tmp_config.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/rpc/tmp_filter.rs` & `solders-0.9.3/src/rpc/tmp_filter.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/rpc/tmp_response.rs` & `solders-0.9.3/src/rpc/tmp_response.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/signature.rs` & `solders-0.9.3/src/signature.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/signer.rs` & `solders-0.9.3/src/signer.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/system_program.rs` & `solders-0.9.3/src/system_program.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/sysvar.rs` & `solders-0.9.3/src/sysvar.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/tmp_account_decoder.rs` & `solders-0.9.3/src/tmp_account_decoder.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/tmp_transaction_status.rs` & `solders-0.9.3/src/tmp_transaction_status.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/transaction.rs` & `solders-0.9.3/src/transaction.rs`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/src/transaction_status.rs` & `solders-0.9.3/src/transaction_status.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1425,36 +1425,58 @@
     InvalidAddressLookupTableIndex,
     InvalidRentPayingAccount,
     WouldExceedMaxVoteCostLimit,
     WouldExceedAccountDataTotalLimit,
 }
 
 #[derive(FromPyObject, Clone, PartialEq, Eq, Serialize, Deserialize, Debug)]
-pub enum TransactionErrorType {
-    Fieldless(TransactionErrorFieldless),
+pub enum TransactionErrorTypeTagged {
     InstructionError(TransactionErrorInstructionError),
     DuplicateInstruction(TransactionErrorDuplicateInstruction),
     InsufficientFundsForRent(TransactionErrorInsufficientFundsForRent),
 }
 
+impl IntoPy<PyObject> for TransactionErrorTypeTagged {
+    fn into_py(self, py: Python<'_>) -> PyObject {
+        match self {
+            Self::InstructionError(e) => e.into_py(py),
+            Self::DuplicateInstruction(d) => d.into_py(py),
+            Self::InsufficientFundsForRent(i) => i.into_py(py),
+        }
+    }
+}
+
+#[derive(FromPyObject, Clone, PartialEq, Eq, Serialize, Deserialize, Debug)]
+#[serde(untagged)]
+pub enum TransactionErrorType {
+    Fieldless(TransactionErrorFieldless),
+    Tagged(TransactionErrorTypeTagged),
+}
+
 impl Default for TransactionErrorType {
     fn default() -> Self {
         Self::Fieldless(TransactionErrorFieldless::AccountInUse)
     }
 }
 
 impl From<TransactionErrorType> for TransactionErrorOriginal {
     fn from(w: TransactionErrorType) -> Self {
         match w {
-            TransactionErrorType::InstructionError(e) => {
-                Self::InstructionError(e.0 .0, e.0 .1.into())
-            }
-            TransactionErrorType::DuplicateInstruction(e) => Self::DuplicateInstruction(e.0),
-            TransactionErrorType::InsufficientFundsForRent(e) => Self::InsufficientFundsForRent {
-                account_index: e.account_index,
+            TransactionErrorType::Tagged(t) => match t {
+                TransactionErrorTypeTagged::InstructionError(e) => {
+                    Self::InstructionError(e.0 .0, e.0 .1.into())
+                }
+                TransactionErrorTypeTagged::DuplicateInstruction(e) => {
+                    Self::DuplicateInstruction(e.0)
+                }
+                TransactionErrorTypeTagged::InsufficientFundsForRent(e) => {
+                    Self::InsufficientFundsForRent {
+                        account_index: e.account_index,
+                    }
+                }
             },
             TransactionErrorType::Fieldless(f) => match f {
                 TransactionErrorFieldless::AccountInUse => Self::AccountInUse,
                 TransactionErrorFieldless::AccountLoadedTwice => Self::AccountLoadedTwice,
                 TransactionErrorFieldless::AccountNotFound => Self::AccountNotFound,
                 TransactionErrorFieldless::ProgramAccountNotFound => Self::ProgramAccountNotFound,
                 TransactionErrorFieldless::InsufficientFundsForFee => Self::InsufficientFundsForFee,
@@ -1511,23 +1533,27 @@
     }
 }
 
 impl From<TransactionErrorOriginal> for TransactionErrorType {
     fn from(w: TransactionErrorOriginal) -> Self {
         match w {
             TransactionErrorOriginal::InstructionError(index, err) => {
-                Self::InstructionError(TransactionErrorInstructionError((index, err.into())))
+                Self::Tagged(TransactionErrorTypeTagged::InstructionError(
+                    TransactionErrorInstructionError((index, err.into())),
+                ))
             }
             TransactionErrorOriginal::DuplicateInstruction(index) => {
-                Self::DuplicateInstruction(TransactionErrorDuplicateInstruction(index))
+                Self::Tagged(TransactionErrorTypeTagged::DuplicateInstruction(
+                    TransactionErrorDuplicateInstruction(index),
+                ))
             }
             TransactionErrorOriginal::InsufficientFundsForRent { account_index } => {
-                Self::InsufficientFundsForRent(TransactionErrorInsufficientFundsForRent {
-                    account_index,
-                })
+                Self::Tagged(TransactionErrorTypeTagged::InsufficientFundsForRent(
+                    TransactionErrorInsufficientFundsForRent { account_index },
+                ))
             }
             TransactionErrorOriginal::AccountInUse => {
                 Self::Fieldless(TransactionErrorFieldless::AccountInUse)
             }
             TransactionErrorOriginal::AccountLoadedTwice => {
                 Self::Fieldless(TransactionErrorFieldless::AccountLoadedTwice)
             }
@@ -1616,17 +1642,15 @@
     }
 }
 
 impl IntoPy<PyObject> for TransactionErrorType {
     fn into_py(self, py: Python<'_>) -> PyObject {
         match self {
             Self::Fieldless(f) => f.into_py(py),
-            Self::InstructionError(e) => e.into_py(py),
-            Self::DuplicateInstruction(d) => d.into_py(py),
-            Self::InsufficientFundsForRent(i) => i.into_py(py),
+            Self::Tagged(t) => t.into_py(py),
         }
     }
 }
 
 #[derive(Clone, Debug, PartialEq, Eq, Serialize, Deserialize, From, Into)]
 #[pyclass(module = "solders.transaction_status", subclass)]
 pub struct Reward(RewardOriginal);
```

### Comparing `solders-0.9.2/Cargo.lock` & `solders-0.9.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1460,15 +1460,15 @@
  "quote",
  "rustversion",
  "syn",
 ]
 
 [[package]]
 name = "solders"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "base64 0.13.0",
  "bincode",
  "borsh",
  "bs58",
  "camelpaste",
  "derive_more",
```

### Comparing `solders-0.9.2/python/solders/instruction.pyi` & `solders-0.9.3/python/solders/instruction.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/commitment_config.pyi` & `solders-0.9.3/python/solders/commitment_config.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/address_lookup_table_account.pyi` & `solders-0.9.3/python/solders/address_lookup_table_account.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/_system_program.pyi` & `solders-0.9.3/python/solders/_system_program.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/account.pyi` & `solders-0.9.3/python/solders/account.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/transaction_status.pyi` & `solders-0.9.3/python/solders/transaction_status.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/message.pyi` & `solders-0.9.3/python/solders/message.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/epoch_schedule.pyi` & `solders-0.9.3/python/solders/epoch_schedule.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/keypair.pyi` & `solders-0.9.3/python/solders/keypair.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/sysvar.py` & `solders-0.9.3/python/solders/sysvar.py`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/transaction.pyi` & `solders-0.9.3/python/solders/transaction.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/hash.pyi` & `solders-0.9.3/python/solders/hash.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/presigner.pyi` & `solders-0.9.3/python/solders/presigner.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/__init__.py` & `solders-0.9.3/python/solders/__init__.py`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/signature.pyi` & `solders-0.9.3/python/solders/signature.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/rpc/config.pyi` & `solders-0.9.3/python/solders/rpc/config.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/rpc/errors.pyi` & `solders-0.9.3/python/solders/rpc/errors.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/rpc/responses.pyi` & `solders-0.9.3/python/solders/rpc/responses.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/rpc/filter.pyi` & `solders-0.9.3/python/solders/rpc/filter.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/rpc/requests.pyi` & `solders-0.9.3/python/solders/rpc/requests.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/null_signer.pyi` & `solders-0.9.3/python/solders/null_signer.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/system_program.py` & `solders-0.9.3/python/solders/system_program.py`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/pubkey.pyi` & `solders-0.9.3/python/solders/pubkey.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/python/solders/account_decoder.pyi` & `solders-0.9.3/python/solders/account_decoder.pyi`

 * *Files identical despite different names*

### Comparing `solders-0.9.2/PKG-INFO` & `solders-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: solders
-Version: 0.9.2
+Version: 0.9.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: typing-extensions >=4.2.0
 License-File: LICENSE
 Summary: Python binding to the Solana Rust SDK
 Author-email: kevinheavey <kevinheavey123@gmail.com>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/kevinheavey/solders
 Project-URL: documentation, https://kevinheavey.github.io/solders/
-Project-URL: changelog, https://github.com/kevinheavey/solders/blob/main/CHANGELOG.md
+Project-URL: repository, https://github.com/kevinheavey/solders
 Project-URL: homepage, https://github.com/kevinheavey/solders
+Project-URL: changelog, https://github.com/kevinheavey/solders/blob/main/CHANGELOG.md
 
 <div align="center">
     <img src="https://raw.githubusercontent.com/kevinheavey/solders/main/docs/logo.jpeg" width="50%" height="50%">
 </div>
 
 ---
```

