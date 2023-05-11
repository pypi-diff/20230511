# Comparing `tmp/py-evm-0.7.0a1.tar.gz` & `tmp/py-evm-0.7.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-evm-0.7.0a1.tar", last modified: Mon Apr 10 16:50:19 2023, max compression
+gzip compressed data, was "py-evm-0.7.0a2.tar", last modified: Thu May 11 21:31:06 2023, max compression
```

## Comparing `py-evm-0.7.0a1.tar` & `py-evm-0.7.0a2.tar`

### file list

```diff
@@ -1,337 +1,337 @@
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.798251 py-evm-0.7.0a1/
--rw-r--r--   0 eve        (501) staff       (20)     1087 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/LICENSE
--rw-r--r--   0 eve        (501) staff       (20)      137 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/MANIFEST.in
--rw-r--r--   0 eve        (501) staff       (20)     2673 2023-04-10 16:50:19.798089 py-evm-0.7.0a1/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     1854 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/README.md
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.767113 py-evm-0.7.0a1/eth/
--rw-r--r--   0 eve        (501) staff       (20)      368 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.769086 py-evm-0.7.0a1/eth/_utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      734 2022-12-07 18:37:56.000000 py-evm-0.7.0a1/eth/_utils/address.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.769501 py-evm-0.7.0a1/eth/_utils/blake2/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 18:37:56.000000 py-evm-0.7.0a1/eth/_utils/blake2/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1791 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/_utils/blake2/coders.py
--rwxr-xr-x   0 eve        (501) staff       (20)     5784 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/blake2/compression.py
--rw-r--r--   0 eve        (501) staff       (20)      972 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/bn128.py
--rw-r--r--   0 eve        (501) staff       (20)     3900 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/datatypes.py
--rw-r--r--   0 eve        (501) staff       (20)     1001 2022-12-07 18:37:56.000000 py-evm-0.7.0a1/eth/_utils/db.py
--rw-r--r--   0 eve        (501) staff       (20)       40 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/empty.py
--rw-r--r--   0 eve        (501) staff       (20)     8214 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/env.py
--rw-r--r--   0 eve        (501) staff       (20)      613 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/generator.py
--rw-r--r--   0 eve        (501) staff       (20)     5061 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/_utils/headers.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 18:37:56.000000 py-evm-0.7.0a1/eth/_utils/logging.py
--rw-r--r--   0 eve        (501) staff       (20)     1532 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/module_loading.py
--rw-r--r--   0 eve        (501) staff       (20)     2801 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/numeric.py
--rw-r--r--   0 eve        (501) staff       (20)      338 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/padding.py
--rw-r--r--   0 eve        (501) staff       (20)     3338 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/eth/_utils/rlp.py
--rw-r--r--   0 eve        (501) staff       (20)     1739 2022-12-07 18:37:56.000000 py-evm-0.7.0a1/eth/_utils/spoof.py
--rw-r--r--   0 eve        (501) staff       (20)     1352 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/state.py
--rw-r--r--   0 eve        (501) staff       (20)     3409 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/_utils/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)      376 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/_utils/version.py
--rw-r--r--   0 eve        (501) staff       (20)      346 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_warnings.py
--rw-r--r--   0 eve        (501) staff       (20)   118518 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/abc.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.769802 py-evm-0.7.0a1/eth/chains/
--rw-r--r--   0 eve        (501) staff       (20)      223 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/chains/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    26256 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/chains/base.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.770110 py-evm-0.7.0a1/eth/chains/goerli/
--rw-r--r--   0 eve        (501) staff       (20)     1277 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/chains/goerli/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      262 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/chains/goerli/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     2599 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/chains/header.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.770339 py-evm-0.7.0a1/eth/chains/mainnet/
--rw-r--r--   0 eve        (501) staff       (20)     4517 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/chains/mainnet/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1191 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/chains/mainnet/constants.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.770548 py-evm-0.7.0a1/eth/chains/ropsten/
--rw-r--r--   0 eve        (501) staff       (20)     2105 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/chains/ropsten/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      839 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/chains/ropsten/constants.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.770648 py-evm-0.7.0a1/eth/chains/tester/
--rw-r--r--   0 eve        (501) staff       (20)     5965 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/chains/tester/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.771225 py-evm-0.7.0a1/eth/consensus/
--rw-r--r--   0 eve        (501) staff       (20)      313 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      956 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/applier.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.772023 py-evm-0.7.0a1/eth/consensus/clique/
--rw-r--r--   0 eve        (501) staff       (20)      270 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/clique/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5106 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/consensus/clique/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)     5468 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/clique/clique.py
--rw-r--r--   0 eve        (501) staff       (20)      477 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/clique/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     3380 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/clique/datatypes.py
--rw-r--r--   0 eve        (501) staff       (20)     2929 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/consensus/clique/encoding.py
--rw-r--r--   0 eve        (501) staff       (20)      149 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/clique/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)    11037 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/clique/snapshot_manager.py
--rw-r--r--   0 eve        (501) staff       (20)      188 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/context.py
--rw-r--r--   0 eve        (501) staff       (20)      732 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/noproof.py
--rw-r--r--   0 eve        (501) staff       (20)      834 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/consensus/pos.py
--rw-r--r--   0 eve        (501) staff       (20)     4037 2022-08-17 18:04:11.000000 py-evm-0.7.0a1/eth/consensus/pow.py
--rw-r--r--   0 eve        (501) staff       (20)     3853 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/constants.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.773815 py-evm-0.7.0a1/eth/db/
--rw-r--r--   0 eve        (501) staff       (20)      746 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3434 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/accesslog.py
--rw-r--r--   0 eve        (501) staff       (20)    24116 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/db/account.py
--rw-r--r--   0 eve        (501) staff       (20)     4172 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/atomic.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.774173 py-evm-0.7.0a1/eth/db/backends/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/backends/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2494 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/backends/base.py
--rw-r--r--   0 eve        (501) staff       (20)     4410 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/backends/level.py
--rw-r--r--   0 eve        (501) staff       (20)      890 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/backends/memory.py
--rw-r--r--   0 eve        (501) staff       (20)     2811 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/batch.py
--rw-r--r--   0 eve        (501) staff       (20)      943 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/cache.py
--rw-r--r--   0 eve        (501) staff       (20)    19392 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/db/chain.py
--rw-r--r--   0 eve        (501) staff       (20)     5524 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/chain_gaps.py
--rw-r--r--   0 eve        (501) staff       (20)     7303 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/diff.py
--rw-r--r--   0 eve        (501) staff       (20)      488 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/db/hash_trie.py
--rw-r--r--   0 eve        (501) staff       (20)    24092 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/db/header.py
--rw-r--r--   0 eve        (501) staff       (20)    16683 2021-03-10 18:54:42.000000 py-evm-0.7.0a1/eth/db/journal.py
--rw-r--r--   0 eve        (501) staff       (20)     1291 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/keymap.py
--rw-r--r--   0 eve        (501) staff       (20)     1345 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/db/schema.py
--rw-r--r--   0 eve        (501) staff       (20)    16275 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/slow_journal.py
--rw-r--r--   0 eve        (501) staff       (20)    16229 2021-03-04 23:10:51.000000 py-evm-0.7.0a1/eth/db/storage.py
--rw-r--r--   0 eve        (501) staff       (20)     1363 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/db/trie.py
--rw-r--r--   0 eve        (501) staff       (20)     1667 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/witness.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.774399 py-evm-0.7.0a1/eth/estimators/
--rw-r--r--   0 eve        (501) staff       (20)      522 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/estimators/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3285 2021-08-19 20:42:40.000000 py-evm-0.7.0a1/eth/estimators/gas.py
--rw-r--r--   0 eve        (501) staff       (20)     4076 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/eth/exceptions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.775590 py-evm-0.7.0a1/eth/precompiles/
--rw-r--r--   0 eve        (501) staff       (20)      398 2021-02-26 19:54:17.000000 py-evm-0.7.0a1/eth/precompiles/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      919 2021-09-03 20:35:50.000000 py-evm-0.7.0a1/eth/precompiles/blake2.py
--rw-r--r--   0 eve        (501) staff       (20)     1487 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/precompiles/ecadd.py
--rw-r--r--   0 eve        (501) staff       (20)     1375 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/precompiles/ecmul.py
--rw-r--r--   0 eve        (501) staff       (20)     3261 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/precompiles/ecpairing.py
--rw-r--r--   0 eve        (501) staff       (20)     1511 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/eth/precompiles/ecrecover.py
--rw-r--r--   0 eve        (501) staff       (20)      478 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/precompiles/identity.py
--rw-r--r--   0 eve        (501) staff       (20)     4026 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/precompiles/modexp.py
--rw-r--r--   0 eve        (501) staff       (20)      676 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/precompiles/ripemd160.py
--rw-r--r--   0 eve        (501) staff       (20)      548 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/precompiles/sha256.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/py.typed
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.776441 py-evm-0.7.0a1/eth/rlp/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/rlp/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1032 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/rlp/accounts.py
--rw-r--r--   0 eve        (501) staff       (20)      904 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/rlp/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     5587 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/rlp/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      669 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/rlp/logs.py
--rw-r--r--   0 eve        (501) staff       (20)     1312 2021-03-10 18:54:47.000000 py-evm-0.7.0a1/eth/rlp/receipts.py
--rw-r--r--   0 eve        (501) staff       (20)      370 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/rlp/sedes.py
--rw-r--r--   0 eve        (501) staff       (20)     3595 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/rlp/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.776722 py-evm-0.7.0a1/eth/tools/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.777921 py-evm-0.7.0a1/eth/tools/_utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      637 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/tools/_utils/deprecation.py
--rw-r--r--   0 eve        (501) staff       (20)      181 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/_utils/git.py
--rw-r--r--   0 eve        (501) staff       (20)      532 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/tools/_utils/hashing.py
--rw-r--r--   0 eve        (501) staff       (20)     1486 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/_utils/mappings.py
--rw-r--r--   0 eve        (501) staff       (20)    17880 2022-08-31 18:17:44.000000 py-evm-0.7.0a1/eth/tools/_utils/normalization.py
--rw-r--r--   0 eve        (501) staff       (20)     4314 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/_utils/slow_code_stream.py
--rw-r--r--   0 eve        (501) staff       (20)      886 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/_utils/vyper.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.778044 py-evm-0.7.0a1/eth/tools/builder/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/builder/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.778269 py-evm-0.7.0a1/eth/tools/builder/chain/
--rw-r--r--   0 eve        (501) staff       (20)     2936 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/tools/builder/chain/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    15213 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/tools/builder/chain/builders.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.778684 py-evm-0.7.0a1/eth/tools/db/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/db/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5130 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/db/atomic.py
--rw-r--r--   0 eve        (501) staff       (20)     2260 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/db/base.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.779239 py-evm-0.7.0a1/eth/tools/fixtures/
--rw-r--r--   0 eve        (501) staff       (20)      615 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/tools/fixtures/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      878 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/_utils.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.780043 py-evm-0.7.0a1/eth/tools/fixtures/fillers/
--rw-r--r--   0 eve        (501) staff       (20)      282 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2461 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)    12490 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/common.py
--rw-r--r--   0 eve        (501) staff       (20)     3108 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/formatters.py
--rw-r--r--   0 eve        (501) staff       (20)     1305 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/main.py
--rw-r--r--   0 eve        (501) staff       (20)     2617 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1747 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/vm.py
--rw-r--r--   0 eve        (501) staff       (20)     2136 2021-11-05 22:07:56.000000 py-evm-0.7.0a1/eth/tools/fixtures/generation.py
--rw-r--r--   0 eve        (501) staff       (20)     9639 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/tools/fixtures/helpers.py
--rw-r--r--   0 eve        (501) staff       (20)     3140 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/tools/fixtures/loading.py
--rw-r--r--   0 eve        (501) staff       (20)      759 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/mining.py
--rw-r--r--   0 eve        (501) staff       (20)      449 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/tools/rlp.py
--rw-r--r--   0 eve        (501) staff       (20)     3085 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/typing.py
--rw-r--r--   0 eve        (501) staff       (20)     8876 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.782010 py-evm-0.7.0a1/eth/vm/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    26822 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/base.py
--rw-r--r--   0 eve        (501) staff       (20)      615 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/chain_context.py
--rw-r--r--   0 eve        (501) staff       (20)     4247 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/code_stream.py
--rw-r--r--   0 eve        (501) staff       (20)    18099 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/computation.py
--rw-r--r--   0 eve        (501) staff       (20)     2086 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/execution_context.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.782120 py-evm-0.7.0a1/eth/vm/forks/
--rw-r--r--   0 eve        (501) staff       (20)      899 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.782822 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/
--rw-r--r--   0 eve        (501) staff       (20)      856 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      951 2022-06-23 20:10:28.000000 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      267 2021-12-15 20:27:15.000000 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/computation.py
--rw-r--r--   0 eve        (501) staff       (20)     1088 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      463 2021-12-15 20:27:15.000000 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1132 2021-12-15 20:27:15.000000 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.783925 py-evm-0.7.0a1/eth/vm/forks/berlin/
--rw-r--r--   0 eve        (501) staff       (20)      760 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      760 2021-03-10 18:54:47.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     2402 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      327 2021-08-30 21:22:29.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      381 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     6462 2021-09-10 18:06:54.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/logic.py
--rw-r--r--   0 eve        (501) staff       (20)     2888 2021-03-17 17:52:03.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)     4521 2021-08-30 17:37:29.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/receipts.py
--rw-r--r--   0 eve        (501) staff       (20)     1192 2021-03-17 17:52:03.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/state.py
--rw-r--r--   0 eve        (501) staff       (20)    15608 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.785022 py-evm-0.7.0a1/eth/vm/forks/byzantium/
--rw-r--r--   0 eve        (501) staff       (20)     3585 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      483 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      965 2021-02-26 17:26:20.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      226 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     3434 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     3499 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      204 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1442 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.786005 py-evm-0.7.0a1/eth/vm/forks/constantinople/
--rw-r--r--   0 eve        (501) staff       (20)     1108 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      482 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      809 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      321 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      401 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     1569 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      211 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/state.py
--rw-r--r--   0 eve        (501) staff       (20)      325 2021-03-17 17:52:03.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/storage.py
--rw-r--r--   0 eve        (501) staff       (20)     1446 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.787002 py-evm-0.7.0a1/eth/vm/forks/frontier/
--rw-r--r--   0 eve        (501) staff       (20)     3820 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3318 2021-08-19 20:42:40.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     3696 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/computation.py
--rw-r--r--   0 eve        (501) staff       (20)       96 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     3546 2021-08-19 20:42:40.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/headers.py
--rw-r--r--   0 eve        (501) staff       (20)    20208 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)     7722 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/state.py
--rw-r--r--   0 eve        (501) staff       (20)      131 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/transaction_context.py
--rw-r--r--   0 eve        (501) staff       (20)     6040 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)     1698 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.787544 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/
--rw-r--r--   0 eve        (501) staff       (20)      855 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1017 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      297 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/computation.py
--rw-r--r--   0 eve        (501) staff       (20)     1132 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      496 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1168 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.788390 py-evm-0.7.0a1/eth/vm/forks/homestead/
--rw-r--r--   0 eve        (501) staff       (20)     1210 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      463 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     2261 2021-03-05 23:32:34.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/computation.py
--rw-r--r--   0 eve        (501) staff       (20)       61 2021-09-03 20:35:50.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     9661 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      603 2021-03-05 23:31:28.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      613 2021-03-05 23:32:34.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/state.py
--rw-r--r--   0 eve        (501) staff       (20)     2292 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)      548 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.789417 py-evm-0.7.0a1/eth/vm/forks/istanbul/
--rw-r--r--   0 eve        (501) staff       (20)      805 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      467 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     1466 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      316 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      385 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     1637 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      196 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/state.py
--rw-r--r--   0 eve        (501) staff       (20)      883 2021-09-02 18:17:22.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/storage.py
--rw-r--r--   0 eve        (501) staff       (20)     2000 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.790511 py-evm-0.7.0a1/eth/vm/forks/london/
--rw-r--r--   0 eve        (501) staff       (20)     2286 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/london/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5835 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/london/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      772 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/london/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      470 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/london/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     5587 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/london/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      860 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/london/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      620 2021-08-30 17:37:29.000000 py-evm-0.7.0a1/eth/vm/forks/london/receipts.py
--rw-r--r--   0 eve        (501) staff       (20)     4940 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/london/state.py
--rw-r--r--   0 eve        (501) staff       (20)      527 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/london/storage.py
--rw-r--r--   0 eve        (501) staff       (20)     9548 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/london/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)      845 2021-08-19 20:42:40.000000 py-evm-0.7.0a1/eth/vm/forks/london/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.791208 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/
--rw-r--r--   0 eve        (501) staff       (20)      830 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      470 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      562 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      438 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      137 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      199 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1423 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.791879 py-evm-0.7.0a1/eth/vm/forks/paris/
--rw-r--r--   0 eve        (501) staff       (20)     2088 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/paris/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1014 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/paris/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      375 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/paris/computation.py
--rw-r--r--   0 eve        (501) staff       (20)     2234 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/paris/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      649 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/paris/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      619 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/paris/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1119 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/paris/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.792661 py-evm-0.7.0a1/eth/vm/forks/petersburg/
--rw-r--r--   0 eve        (501) staff       (20)     1024 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      470 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      556 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      102 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      381 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     1378 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      199 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1422 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.793716 py-evm-0.7.0a1/eth/vm/forks/shanghai/
--rw-r--r--   0 eve        (501) staff       (20)      667 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     8631 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     1595 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      187 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      784 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      820 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/logic.py
--rw-r--r--   0 eve        (501) staff       (20)     1474 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      717 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1097 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)     1461 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/withdrawals.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.794726 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/
--rw-r--r--   0 eve        (501) staff       (20)      429 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2124 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)      481 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     3234 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      169 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     1180 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)     1486 2021-09-03 22:22:38.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/state.py
--rw-r--r--   0 eve        (501) staff       (20)     2950 2021-03-10 18:54:47.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.795297 py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/
--rw-r--r--   0 eve        (501) staff       (20)      469 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      396 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      225 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     2067 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      209 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/state.py
--rw-r--r--   0 eve        (501) staff       (20)     2637 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/gas_meter.py
--rw-r--r--   0 eve        (501) staff       (20)      531 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/header.py
--rw-r--r--   0 eve        (501) staff       (20)     3414 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/interrupt.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.797136 py-evm-0.7.0a1/eth/vm/logic/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     4819 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/arithmetic.py
--rw-r--r--   0 eve        (501) staff       (20)     1066 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/logic/block.py
--rw-r--r--   0 eve        (501) staff       (20)    14298 2021-03-17 17:52:03.000000 py-evm-0.7.0a1/eth/vm/logic/call.py
--rw-r--r--   0 eve        (501) staff       (20)     2831 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/comparison.py
--rw-r--r--   0 eve        (501) staff       (20)     6448 2021-03-17 17:52:03.000000 py-evm-0.7.0a1/eth/vm/logic/context.py
--rw-r--r--   0 eve        (501) staff       (20)      948 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/duplication.py
--rw-r--r--   0 eve        (501) staff       (20)     1518 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/flow.py
--rw-r--r--   0 eve        (501) staff       (20)      480 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/invalid.py
--rw-r--r--   0 eve        (501) staff       (20)     1342 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/logging.py
--rw-r--r--   0 eve        (501) staff       (20)     1109 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/memory.py
--rw-r--r--   0 eve        (501) staff       (20)      626 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/sha3.py
--rw-r--r--   0 eve        (501) staff       (20)     2181 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/logic/stack.py
--rw-r--r--   0 eve        (501) staff       (20)     3921 2021-09-10 18:08:36.000000 py-evm-0.7.0a1/eth/vm/logic/storage.py
--rw-r--r--   0 eve        (501) staff       (20)      978 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/swap.py
--rw-r--r--   0 eve        (501) staff       (20)     9441 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/eth/vm/logic/system.py
--rw-r--r--   0 eve        (501) staff       (20)     2122 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/memory.py
--rw-r--r--   0 eve        (501) staff       (20)     3177 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/message.py
--rw-r--r--   0 eve        (501) staff       (20)     2785 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/mnemonics.py
--rw-r--r--   0 eve        (501) staff       (20)     1895 2021-08-30 21:41:40.000000 py-evm-0.7.0a1/eth/vm/opcode.py
--rw-r--r--   0 eve        (501) staff       (20)     2430 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/opcode_values.py
--rw-r--r--   0 eve        (501) staff       (20)      385 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/spoof.py
--rw-r--r--   0 eve        (501) staff       (20)     7675 2021-03-17 17:52:03.000000 py-evm-0.7.0a1/eth/vm/stack.py
--rw-r--r--   0 eve        (501) staff       (20)    10402 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/state.py
--rw-r--r--   0 eve        (501) staff       (20)      857 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/transaction_context.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.797881 py-evm-0.7.0a1/py_evm.egg-info/
--rw-r--r--   0 eve        (501) staff       (20)     2673 2023-04-10 16:50:19.000000 py-evm-0.7.0a1/py_evm.egg-info/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     8485 2023-04-10 16:50:19.000000 py-evm-0.7.0a1/py_evm.egg-info/SOURCES.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-04-10 16:50:19.000000 py-evm-0.7.0a1/py_evm.egg-info/dependency_links.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2021-02-24 18:15:32.000000 py-evm-0.7.0a1/py_evm.egg-info/not-zip-safe
--rw-r--r--   0 eve        (501) staff       (20)     2057 2023-04-10 16:50:19.000000 py-evm-0.7.0a1/py_evm.egg-info/requires.txt
--rw-r--r--   0 eve        (501) staff       (20)        4 2023-04-10 16:50:19.000000 py-evm-0.7.0a1/py_evm.egg-info/top_level.txt
--rw-r--r--   0 eve        (501) staff       (20)     1108 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/pyproject.toml
--rw-r--r--   0 eve        (501) staff       (20)       38 2023-04-10 16:50:19.798298 py-evm-0.7.0a1/setup.cfg
--rw-r--r--   0 eve        (501) staff       (20)     3674 2023-04-10 16:50:15.000000 py-evm-0.7.0a1/setup.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.470517 py-evm-0.7.0a2/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1095 2023-04-28 21:58:38.000000 py-evm-0.7.0a2/LICENSE
+-rw-r--r--   0 fselmo     (501) staff       (20)      141 2023-04-28 21:58:38.000000 py-evm-0.7.0a2/MANIFEST.in
+-rw-r--r--   0 fselmo     (501) staff       (20)     2976 2023-05-11 21:31:06.469745 py-evm-0.7.0a2/PKG-INFO
+-rw-r--r--   0 fselmo     (501) staff       (20)     2157 2023-04-28 21:58:38.000000 py-evm-0.7.0a2/README.md
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.132414 py-evm-0.7.0a2/eth/
+-rw-r--r--   0 fselmo     (501) staff       (20)      368 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.142130 py-evm-0.7.0a2/eth/_utils/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/_utils/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      687 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/address.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.144715 py-evm-0.7.0a2/eth/_utils/blake2/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/_utils/blake2/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1841 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/blake2/coders.py
+-rwxr-xr-x   0 fselmo     (501) staff       (20)     5793 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/blake2/compression.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      980 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/bn128.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3924 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/datatypes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1013 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/db.py
+-rw-r--r--   0 fselmo     (501) staff       (20)       40 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/_utils/empty.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8124 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/env.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      612 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/generator.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5024 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/_utils/logging.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1540 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/module_loading.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2671 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/numeric.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      337 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/padding.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3284 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/rlp.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1749 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/spoof.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1343 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3379 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/transactions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      385 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/version.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      364 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_warnings.py
+-rw-r--r--   0 fselmo     (501) staff       (20)   117125 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/abc.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.146869 py-evm-0.7.0a2/eth/chains/
+-rw-r--r--   0 fselmo     (501) staff       (20)      223 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/chains/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    25965 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/base.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.148085 py-evm-0.7.0a2/eth/chains/goerli/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1305 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/goerli/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      270 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/goerli/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2554 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/header.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.149533 py-evm-0.7.0a2/eth/chains/mainnet/
+-rw-r--r--   0 fselmo     (501) staff       (20)     4409 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/mainnet/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1199 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/mainnet/constants.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.150947 py-evm-0.7.0a2/eth/chains/ropsten/
+-rw-r--r--   0 fselmo     (501) staff       (20)     2131 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/ropsten/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      847 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/ropsten/constants.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.151666 py-evm-0.7.0a2/eth/chains/tester/
+-rw-r--r--   0 fselmo     (501) staff       (20)     5919 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/tester/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.155213 py-evm-0.7.0a2/eth/consensus/
+-rw-r--r--   0 fselmo     (501) staff       (20)      313 2022-06-06 17:44:51.000000 py-evm-0.7.0a2/eth/consensus/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      968 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/applier.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.159710 py-evm-0.7.0a2/eth/consensus/clique/
+-rw-r--r--   0 fselmo     (501) staff       (20)      271 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5208 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/_utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5383 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/clique.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      486 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3368 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/datatypes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2949 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/encoding.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      158 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/exceptions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    11157 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/snapshot_manager.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      187 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/context.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      683 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/noproof.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      819 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/pos.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4024 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/pow.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3921 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/constants.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.172356 py-evm-0.7.0a2/eth/db/
+-rw-r--r--   0 fselmo     (501) staff       (20)      730 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3460 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/accesslog.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    24391 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/account.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4277 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/atomic.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.174356 py-evm-0.7.0a2/eth/db/backends/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/db/backends/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2513 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/backends/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4496 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/backends/level.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      890 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/db/backends/memory.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2874 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/batch.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      971 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/cache.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    19178 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/chain.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5873 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/chain_gaps.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     7394 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/diff.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      506 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/hash_trie.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    24129 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/header.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    17008 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/journal.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1306 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/keymap.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1354 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/schema.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    16562 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/slow_journal.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    16442 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/storage.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1393 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/trie.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1660 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/witness.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.175706 py-evm-0.7.0a2/eth/estimators/
+-rw-r--r--   0 fselmo     (501) staff       (20)      514 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/estimators/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3427 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/estimators/gas.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4115 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/exceptions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.181870 py-evm-0.7.0a2/eth/precompiles/
+-rw-r--r--   0 fselmo     (501) staff       (20)      398 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/precompiles/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      962 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/blake2.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1502 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/ecadd.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1390 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/ecmul.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3257 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/ecpairing.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1512 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/ecrecover.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      472 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/identity.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3934 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/modexp.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      670 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/ripemd160.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      541 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/sha256.py
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/py.typed
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.189931 py-evm-0.7.0a2/eth/rlp/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/rlp/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1022 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/accounts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      904 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5417 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      603 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/logs.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1285 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/receipts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      387 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/sedes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3611 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.192185 py-evm-0.7.0a2/eth/tools/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/tools/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.199164 py-evm-0.7.0a2/eth/tools/_utils/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/tools/_utils/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      636 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/deprecation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      190 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/git.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      556 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/hashing.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1564 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/mappings.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    18084 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/normalization.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4410 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/slow_code_stream.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      903 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/vyper.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.200084 py-evm-0.7.0a2/eth/tools/builder/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/tools/builder/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.203230 py-evm-0.7.0a2/eth/tools/builder/chain/
+-rw-r--r--   0 fselmo     (501) staff       (20)     2936 2023-04-17 23:21:54.000000 py-evm-0.7.0a2/eth/tools/builder/chain/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    15254 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/builder/chain/builders.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.205942 py-evm-0.7.0a2/eth/tools/db/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/tools/db/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5184 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/db/atomic.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2269 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/db/base.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.211823 py-evm-0.7.0a2/eth/tools/fixtures/
+-rw-r--r--   0 fselmo     (501) staff       (20)      615 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/tools/fixtures/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      887 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/_utils.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.221591 py-evm-0.7.0a2/eth/tools/fixtures/fillers/
+-rw-r--r--   0 fselmo     (501) staff       (20)      282 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2456 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/_utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    12732 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/common.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3461 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/formatters.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1307 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2758 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1737 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/vm.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2079 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/generation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9361 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/helpers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3068 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/loading.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      791 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/mining.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      476 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/rlp.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2693 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/typing.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8548 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/validation.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.243609 py-evm-0.7.0a2/eth/vm/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    26238 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      632 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/chain_context.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4408 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/code_stream.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    19222 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2124 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/execution_context.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.244467 py-evm-0.7.0a2/eth/vm/forks/
+-rw-r--r--   0 fselmo     (501) staff       (20)      899 2023-05-04 19:22:49.000000 py-evm-0.7.0a2/eth/vm/forks/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.253170 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/
+-rw-r--r--   0 fselmo     (501) staff       (20)      856 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      993 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      287 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1084 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      523 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1134 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.270170 py-evm-0.7.0a2/eth/vm/forks/berlin/
+-rw-r--r--   0 fselmo     (501) staff       (20)      772 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      784 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2441 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      327 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      374 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6417 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/logic.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2922 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4606 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/receipts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1187 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    15375 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.296825 py-evm-0.7.0a2/eth/vm/forks/byzantium/
+-rw-r--r--   0 fselmo     (501) staff       (20)     3584 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      485 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1016 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      235 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3368 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3526 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      222 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1231 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.328039 py-evm-0.7.0a2/eth/vm/forks/constantinople/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1106 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      484 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      757 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      329 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      406 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1574 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      221 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      334 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/storage.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1235 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.354068 py-evm-0.7.0a2/eth/vm/forks/frontier/
+-rw-r--r--   0 fselmo     (501) staff       (20)     3732 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3412 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3715 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)       96 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3529 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    20228 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     7686 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      140 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/transaction_context.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5849 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/transactions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1603 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/validation.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.360109 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/
+-rw-r--r--   0 fselmo     (501) staff       (20)      855 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1068 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      317 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1119 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      556 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1170 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.369439 py-evm-0.7.0a2/eth/vm/forks/homestead/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1250 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      466 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2289 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)       61 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9656 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      637 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      640 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2197 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/transactions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      518 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/validation.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.378364 py-evm-0.7.0a2/eth/vm/forks/istanbul/
+-rw-r--r--   0 fselmo     (501) staff       (20)      817 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      469 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1421 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      316 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      384 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1664 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      206 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      909 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/storage.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1798 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.390946 py-evm-0.7.0a2/eth/vm/forks/london/
+-rw-r--r--   0 fselmo     (501) staff       (20)     2260 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5828 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      810 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      470 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5618 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      895 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      629 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/receipts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4881 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      544 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/storage.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9466 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/transactions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      855 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/validation.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.399860 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/
+-rw-r--r--   0 fselmo     (501) staff       (20)      842 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      472 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      537 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      443 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      137 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      209 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1212 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.406971 py-evm-0.7.0a2/eth/vm/forks/paris/
+-rw-r--r--   0 fselmo     (501) staff       (20)     2117 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1039 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      379 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2284 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      686 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      666 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1121 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.416338 py-evm-0.7.0a2/eth/vm/forks/petersburg/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1036 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      472 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      531 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      110 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      386 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1399 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      209 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1211 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.428399 py-evm-0.7.0a2/eth/vm/forks/shanghai/
+-rw-r--r--   0 fselmo     (501) staff       (20)      667 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9048 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1655 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      196 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      824 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/headers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      821 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/logic.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1531 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      751 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1099 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/transactions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1515 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/withdrawals.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.438268 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/
+-rw-r--r--   0 fselmo     (501) staff       (20)      429 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2145 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/_utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      484 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3322 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      169 2023-04-17 23:21:54.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1221 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1465 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2866 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.446334 py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/
+-rw-r--r--   0 fselmo     (501) staff       (20)      469 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      428 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/computation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      225 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2106 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/opcodes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      227 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2626 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/gas_meter.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      540 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/header.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3425 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/interrupt.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.463876 py-evm-0.7.0a2/eth/vm/logic/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/logic/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4805 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/arithmetic.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1113 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/block.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    13394 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/call.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2824 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/comparison.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6418 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/context.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      944 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/duplication.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1508 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/flow.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      507 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/invalid.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1355 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/logging.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1102 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/memory.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      640 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/sha3.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2176 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/stack.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3939 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/storage.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      974 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/swap.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9518 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/system.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2134 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/memory.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3214 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/message.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2785 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/mnemonics.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1864 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/opcode.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2432 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/opcode_values.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      416 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/spoof.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     7713 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/stack.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    10406 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/state.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      875 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/transaction_context.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.468847 py-evm-0.7.0a2/py_evm.egg-info/
+-rw-r--r--   0 fselmo     (501) staff       (20)     2976 2023-05-11 21:31:02.000000 py-evm-0.7.0a2/py_evm.egg-info/PKG-INFO
+-rw-r--r--   0 fselmo     (501) staff       (20)     8485 2023-05-11 21:31:06.000000 py-evm-0.7.0a2/py_evm.egg-info/SOURCES.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-05-11 21:31:02.000000 py-evm-0.7.0a2/py_evm.egg-info/dependency_links.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        1 2021-11-19 17:48:51.000000 py-evm-0.7.0a2/py_evm.egg-info/not-zip-safe
+-rw-r--r--   0 fselmo     (501) staff       (20)     2141 2023-05-11 21:31:02.000000 py-evm-0.7.0a2/py_evm.egg-info/requires.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        4 2023-05-11 21:31:02.000000 py-evm-0.7.0a2/py_evm.egg-info/top_level.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)     1116 2023-04-28 21:58:38.000000 py-evm-0.7.0a2/pyproject.toml
+-rw-r--r--   0 fselmo     (501) staff       (20)       38 2023-05-11 21:31:06.470806 py-evm-0.7.0a2/setup.cfg
+-rw-r--r--   0 fselmo     (501) staff       (20)     3724 2023-05-11 21:30:18.000000 py-evm-0.7.0a2/setup.py
```

### Comparing `py-evm-0.7.0a1/LICENSE` & `py-evm-0.7.0a2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright 2017-2019 Ethereum Foundation
+Copyright (c) 2017-2023 The Ethereum Foundation
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `py-evm-0.7.0a1/PKG-INFO` & `py-evm-0.7.0a2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-evm
-Version: 0.7.0a1
+Version: 0.7.0a2
 Summary: Python implementation of the Ethereum Virtual Machine
 Home-page: https://github.com/ethereum/py-evm
 Author: Ethereum Foundation
 Author-email: piper@pipermerriam.com
 License: MIT
 Keywords: ethereum blockchain evm
 Classifier: Development Status :: 3 - Alpha
@@ -23,15 +23,18 @@
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE
 
 # Python Implementation of the Ethereum protocol
 
 [![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
-[![Documentation Status](https://readthedocs.org/projects/py-evm/badge/?version=latest)](https://py-evm.readthedocs.io/en/latest/?badge=latest)
+[![Build Status](https://circleci.com/gh/ethereum/py-evm.svg?style=shield)](https://circleci.com/gh/ethereum/py-evm)
+[![PyPI version](https://badge.fury.io/py/py-evm.svg)](https://badge.fury.io/py/py-evm)
+[![Python versions](https://img.shields.io/pypi/pyversions/py-evm.svg)](https://pypi.python.org/pypi/py-evm)
+[![Docs build](https://readthedocs.org/projects/py-evm/badge/?version=latest)](http://py-evm.readthedocs.io/en/latest/?badge=latest)
 
 
 ## Py-EVM
 
 Py-EVM is an implementation of the Ethereum protocol in Python. It contains the low level
 primitives for the existing Ethereum 1.0 chain as well as emerging support for the upcoming
 Ethereum 2.0 / Serenity spec.
```

### Comparing `py-evm-0.7.0a1/README.md` & `py-evm-0.7.0a2/py_evm.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,40 @@
+Metadata-Version: 2.1
+Name: py-evm
+Version: 0.7.0a2
+Summary: Python implementation of the Ethereum Virtual Machine
+Home-page: https://github.com/ethereum/py-evm
+Author: Ethereum Foundation
+Author-email: piper@pipermerriam.com
+License: MIT
+Keywords: ethereum blockchain evm
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+Provides-Extra: eth
+Provides-Extra: eth-extra
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: benchmark
+Provides-Extra: doc
+Provides-Extra: dev
+License-File: LICENSE
+
 # Python Implementation of the Ethereum protocol
 
 [![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
-[![Documentation Status](https://readthedocs.org/projects/py-evm/badge/?version=latest)](https://py-evm.readthedocs.io/en/latest/?badge=latest)
+[![Build Status](https://circleci.com/gh/ethereum/py-evm.svg?style=shield)](https://circleci.com/gh/ethereum/py-evm)
+[![PyPI version](https://badge.fury.io/py/py-evm.svg)](https://badge.fury.io/py/py-evm)
+[![Python versions](https://img.shields.io/pypi/pyversions/py-evm.svg)](https://pypi.python.org/pypi/py-evm)
+[![Docs build](https://readthedocs.org/projects/py-evm/badge/?version=latest)](http://py-evm.readthedocs.io/en/latest/?badge=latest)
 
 
 ## Py-EVM
 
 Py-EVM is an implementation of the Ethereum protocol in Python. It contains the low level
 primitives for the existing Ethereum 1.0 chain as well as emerging support for the upcoming
 Ethereum 2.0 / Serenity spec.
```

### Comparing `py-evm-0.7.0a1/eth/_utils/address.py` & `py-evm-0.7.0a2/eth/_utils/address.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+from eth_hash.auto import (
+    keccak,
+)
+from eth_typing import (
+    Address,
+)
 import rlp
 
-from eth_hash.auto import keccak
-from eth_typing import Address
-
 from eth._utils.numeric import (
     int_to_bytes32,
 )
 
 
 def force_bytes_to_address(value: bytes) -> Address:
     trimmed_value = value[-20:]
-    padded_value = trimmed_value.rjust(20, b'\x00')
+    padded_value = trimmed_value.rjust(20, b"\x00")
     return Address(padded_value)
 
 
 def generate_contract_address(address: Address, nonce: int) -> Address:
     return force_bytes_to_address(keccak(rlp.encode([address, nonce])))
 
 
-def generate_safe_contract_address(address: Address,
-                                   salt: int,
-                                   call_data: bytes) -> Address:
+def generate_safe_contract_address(
+    address: Address, salt: int, call_data: bytes
+) -> Address:
     return force_bytes_to_address(
-        keccak(b'\xff' + address + int_to_bytes32(salt) + keccak(call_data))
+        keccak(b"\xff" + address + int_to_bytes32(salt) + keccak(call_data))
     )
```

### Comparing `py-evm-0.7.0a1/eth/_utils/blake2/coders.py` & `py-evm-0.7.0a2/eth/_utils/blake2/coders.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 from typing import (
-    cast,
     Iterable,
     Tuple,
+    cast,
 )
 
 from eth_utils import (
+    ValidationError,
     to_int,
     to_tuple,
-    ValidationError,
 )
 
 from .compression import (
     TMessageBlock,
 )
 
-TMessage = Tuple[int, int, int, int, int, int, int, int, int, int, int, int, int, int, int, int]
+TMessage = Tuple[
+    int, int, int, int, int, int, int, int, int, int, int, int, int, int, int, int
+]
 TFCompressArgs = Tuple[int, TMessageBlock, TMessage, Tuple[int, int], bool]
 
 
 def extract_blake2b_parameters(input_bytes: bytes) -> TFCompressArgs:
     num_bytes = len(input_bytes)
     if num_bytes != 213:
         raise ValidationError(
-            f"input length for Blake2 F precompile should be exactly 213 bytes, got: {num_bytes}"
+            "input length for Blake2 F precompile should be exactly 213 bytes, got: "
+            f"{num_bytes}"
         )
 
     rounds = to_int(input_bytes[:4])
 
     h_state = cast(TMessageBlock, _get_64_bit_little_endian_words(input_bytes[4:68]))
 
     message = cast(TMessage, _get_64_bit_little_endian_words(input_bytes[68:196]))
 
-    t_offset_counters = cast(Tuple[int, int], _get_64_bit_little_endian_words(input_bytes[196:212]))
+    t_offset_counters = cast(
+        Tuple[int, int], _get_64_bit_little_endian_words(input_bytes[196:212])
+    )
 
     final_block_int = to_int(input_bytes[212])
     if final_block_int == 0:
         final_block_flag = False
     elif final_block_int == 1:
         final_block_flag = True
     else:
         raise ValidationError(
-            f"incorrect final block indicator flag, needed 0 or 1, got: {final_block_int}"
+            "incorrect final block indicator flag, needed 0 or 1, got: "
+            f"{final_block_int}"
         )
 
     return rounds, h_state, message, t_offset_counters, final_block_flag
 
 
 @to_tuple
 def _get_64_bit_little_endian_words(compact_bytes: bytes) -> Iterable[int]:
```

### Comparing `py-evm-0.7.0a1/eth/_utils/blake2/compression.py` & `py-evm-0.7.0a2/eth/_utils/blake2/compression.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
         (the ISC license, a minor tweak of the BSD license)
 
 """
 
 
 class Blake2:
-    """ Blake2 is a base class for Blake2b and Blake2s """
+    """Blake2 is a base class for Blake2b and Blake2s"""
 
     # for more than 10 rounds, the schedule wraps around to the beginning
     sigma_schedule = (
         (0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15),
         (14, 10, 4, 8, 9, 15, 13, 6, 1, 12, 0, 2, 11, 7, 5, 3),
         (11, 8, 12, 0, 5, 2, 15, 13, 10, 14, 3, 6, 7, 1, 9, 4),
         (7, 9, 3, 1, 13, 12, 11, 14, 2, 6, 5, 10, 4, 0, 15, 8),
@@ -43,41 +43,45 @@
         (13, 11, 7, 14, 12, 1, 3, 9, 5, 0, 15, 4, 8, 6, 2, 10),
         (6, 15, 14, 9, 11, 3, 0, 8, 12, 2, 13, 7, 1, 4, 10, 5),
         (10, 2, 8, 4, 7, 6, 1, 5, 15, 11, 9, 14, 3, 12, 13, 0),
     )
 
 
 class Blake2b(Blake2):
-
     WORDBITS = 64
-    MASKBITS = 2 ** WORDBITS - 1
-    WORDFMT = 'Q'
+    MASKBITS = 2**WORDBITS - 1
+    WORDFMT = "Q"
 
     IV = (
-        0x6a09e667f3bcc908, 0xbb67ae8584caa73b,
-        0x3c6ef372fe94f82b, 0xa54ff53a5f1d36f1,
-        0x510e527fade682d1, 0x9b05688c2b3e6c1f,
-        0x1f83d9abfb41bd6b, 0x5be0cd19137e2179
+        0x6A09E667F3BCC908,
+        0xBB67AE8584CAA73B,
+        0x3C6EF372FE94F82B,
+        0xA54FF53A5F1D36F1,
+        0x510E527FADE682D1,
+        0x9B05688C2B3E6C1F,
+        0x1F83D9ABFB41BD6B,
+        0x5BE0CD19137E2179,
     )
 
     ROT1 = 32
     ROT2 = 24
     ROT3 = 16
     ROT4 = 63
 
 
 TMessageBlock = Tuple[int, int, int, int, int, int, int, int]
 
 
 def blake2b_compress(
-        num_rounds: int,
-        h_starting_state: TMessageBlock,
-        block: bytes,
-        t_offset_counters: Tuple[int, int],
-        final_block_flag: bool) -> bytes:
+    num_rounds: int,
+    h_starting_state: TMessageBlock,
+    block: bytes,
+    t_offset_counters: Tuple[int, int],
+    final_block_flag: bool,
+) -> bytes:
     """
     'F Compression' from section 3.2 of RFC 7693:
     https://tools.ietf.org/html/rfc7693#section-3.2
     """
 
     # Dereference these for [very small] speed improvement.
     # Perhaps more than anything, this makes the code
@@ -94,18 +98,18 @@
     WB_ROT3 = WORDBITS - ROT3
     WB_ROT4 = WORDBITS - ROT4
 
     sigma_schedule = Blake2b.sigma_schedule
     sigma_schedule_len = len(sigma_schedule)
 
     # convert block (bytes) into 16 LE words
-    m = struct.unpack_from('<16%s' % Blake2b.WORDFMT, bytes(block))
+    m = struct.unpack_from("<16%s" % Blake2b.WORDFMT, bytes(block))
 
     v = [0] * 16
-    v[0: 8] = h_starting_state
+    v[0:8] = h_starting_state
     v[8:12] = IV[:4]
     v[12] = t_offset_counters[0] ^ IV[4]
     v[13] = t_offset_counters[1] ^ IV[5]
 
     if final_block_flag:
         v[14] = Blake2b.MASKBITS ^ IV[6]
     else:
@@ -173,8 +177,8 @@
         msri21 = m[sr[13]]
         G(2, 7, 8, 13)
         msri2 = m[sr[14]]
         msri21 = m[sr[15]]
         G(3, 4, 9, 14)
 
     result_message_words = (h_starting_state[i] ^ v[i] ^ v[i + 8] for i in range(8))
-    return struct.pack(f'<8{Blake2b.WORDFMT}', *result_message_words)
+    return struct.pack(f"<8{Blake2b.WORDFMT}", *result_message_words)
```

### Comparing `py-evm-0.7.0a1/eth/_utils/bn128.py` & `py-evm-0.7.0a2/eth/_utils/bn128.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from typing import (
+    Tuple,
+)
+
+from eth_utils import (
+    ValidationError,
+)
 from py_ecc import (
     optimized_bn128 as bn128,
 )
 from py_ecc.optimized_bn128 import (
-    FQP,
     FQ2,
+    FQP,
 )
 
-from eth_utils import (
-    ValidationError,
-)
-
-from typing import Tuple
-
 
 def validate_point(x: int, y: int) -> Tuple[bn128.FQ, bn128.FQ, bn128.FQ]:
     FQ = bn128.FQ
 
     if x >= bn128.field_modulus:
         raise ValidationError("Point x value is greater than field modulus")
     elif y >= bn128.field_modulus:
```

### Comparing `py-evm-0.7.0a1/eth/_utils/datatypes.py` & `py-evm-0.7.0a2/eth/_utils/datatypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-from eth_utils.toolz import (
-    assoc,
-    groupby,
+from typing import (
+    Any,
+    Dict,
+    Iterator,
+    List,
+    Tuple,
+    Type,
+    TypeVar,
 )
 
 from eth_utils import (
     to_dict,
     to_set,
 )
+from eth_utils.toolz import (
+    assoc,
+    groupby,
+)
 
-
-from typing import Any, Dict, Tuple, Type, TypeVar, Iterator, List
-
-from eth.abc import ConfigurableAPI
+from eth.abc import (
+    ConfigurableAPI,
+)
 
 
 def _is_local_prop(prop: str) -> bool:
-    return len(prop.split('.')) == 1
+    return len(prop.split(".")) == 1
 
 
 def _extract_top_level_key(prop: str) -> str:
-    left, _, _ = prop.partition('.')
+    left, _, _ = prop.partition(".")
     return left
 
 
 def _extract_tail_key(prop: str) -> str:
-    _, _, right = prop.partition('.')
+    _, _, right = prop.partition(".")
     return right
 
 
 @to_dict
 def _get_local_overrides(overrides: Dict[str, Any]) -> Iterator[Tuple[str, Any]]:
     for prop, value in overrides.items():
         if _is_local_prop(prop):
@@ -40,55 +48,57 @@
     for prop, value in overrides.items():
         if not _is_local_prop(prop):
             yield prop, value
 
 
 @to_dict
 def _get_sub_overrides_by_prop(
-        overrides: Dict[str, Any]) -> Iterator[Tuple[str, Dict[str, List[str]]]]:
+    overrides: Dict[str, Any]
+) -> Iterator[Tuple[str, Dict[str, List[str]]]]:
     # we only want the overrides that are not top level.
     sub_overrides = _get_sub_overrides(overrides)
     key_groups = groupby(_extract_top_level_key, sub_overrides.keys())
     for top_level_key, props in key_groups.items():
-        yield top_level_key, {_extract_tail_key(prop): overrides[prop] for prop in props}
+        yield top_level_key, {
+            _extract_tail_key(prop): overrides[prop] for prop in props
+        }
 
 
 @to_set
 def _get_top_level_keys(overrides: Dict[str, Any]) -> Iterator[str]:
     for prop in overrides:
         yield _extract_top_level_key(prop)
 
+
 # Dynamic subclassing is not supported by mypy
 # https://github.com/python/mypy/wiki/Unsupported-Python-Features
 # Most of the cases where we silence mypy boil down to cases where
 # dynamic subclasses where generated through this method
 
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class Configurable(ConfigurableAPI):
     """
     Base class for simple inline subclassing
     """
-    @classmethod
-    def configure(cls: Type[T],
-                  __name__: str = None,
-                  **overrides: Any) -> Type[T]:
 
+    @classmethod
+    def configure(cls: Type[T], __name__: str = None, **overrides: Any) -> Type[T]:
         if __name__ is None:
             __name__ = cls.__name__
 
         top_level_keys = _get_top_level_keys(overrides)
 
         # overrides that are *local* to this class.
         local_overrides = _get_local_overrides(overrides)
 
         for key in top_level_keys:
-            if key == '__name__':
+            if key == "__name__":
                 continue
             elif not hasattr(cls, key):
                 raise TypeError(
                     f"The {cls.__name__}.configure cannot set attributes that are not "
                     f"already present on the base class. The attribute `{key}` was "
                     f"not found on the base class `{cls}`"
                 )
```

### Comparing `py-evm-0.7.0a1/eth/_utils/db.py` & `py-evm-0.7.0a2/eth/_utils/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,26 @@
     StateAPI,
 )
 from eth.typing import (
     AccountState,
 )
 
 
-def get_parent_header(block_header: BlockHeaderAPI, db: ChainDatabaseAPI) -> BlockHeaderAPI:
+def get_parent_header(
+    block_header: BlockHeaderAPI, db: ChainDatabaseAPI
+) -> BlockHeaderAPI:
     """
     Returns the header for the parent block.
     """
     return db.get_block_header_by_hash(block_header.parent_hash)
 
 
-def get_block_header_by_hash(block_hash: Hash32, db: ChainDatabaseAPI) -> BlockHeaderAPI:
+def get_block_header_by_hash(
+    block_hash: Hash32, db: ChainDatabaseAPI
+) -> BlockHeaderAPI:
     """
     Returns the header for the parent block.
     """
     return db.get_block_header_by_hash(block_hash)
 
 
 def apply_state_dict(state: StateAPI, state_dict: AccountState) -> None:
```

### Comparing `py-evm-0.7.0a1/eth/_utils/env.py` & `py-evm-0.7.0a2/eth/_utils/env.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 """
-This module is copied from https://github.com/simpleenergy/env-excavator, which is helpful for
-extracting environment variables.
+This module is copied from https://github.com/simpleenergy/env-excavator,
+which is helpful for extracting environment variables.
 """
 
 import os
-
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Type,
     TypeVar,
     Union,
 )
 
-
 # No set literals because we support Python 2.6.
 TRUE_VALUES = {
     True,
-    'True',
-    'true',
+    "True",
+    "true",
 }
 
 
 class empty:
     """
     We use this sentinel object, instead of None, as None is a plausible value
     for a default in real Python code.
     """
+
     pass
 
 
 def get_env_value(name: str, required: bool = False, default: Any = empty) -> str:
     """
     Core function for extracting the environment variable.
 
@@ -44,23 +43,23 @@
     """
     if required and default is not empty:
         raise ValueError("Using `default` with `required=True` is invalid")
     elif required:
         try:
             value = os.environ[name]
         except KeyError:
-            raise KeyError(
-                f"Must set environment variable {name}"
-            )
+            raise KeyError(f"Must set environment variable {name}")
     else:
         value = os.environ.get(name, default)
     return value
 
 
-def env_int(name: str, required: bool = False, default: Union[Type[empty], int] = empty) -> int:
+def env_int(
+    name: str, required: bool = False, default: Union[Type[empty], int] = empty
+) -> int:
     """Pulls an environment variable out of the environment and casts it to an
     integer. If the name is not present in the environment and no default is
     specified then a ``ValueError`` will be raised. Similarly, if the
     environment value is not castable to an integer, a ``ValueError`` will be
     raised.
 
     :param name: The name of the environment variable be pulled
@@ -80,17 +79,17 @@
         raise ValueError(
             "`env_int` requires either a default value to be specified, or for "
             "the variable to be present in the environment"
         )
     return int(value)
 
 
-def env_float(name: str,
-              required: bool = False,
-              default: Union[Type[empty], float] = empty) -> float:
+def env_float(
+    name: str, required: bool = False, default: Union[Type[empty], float] = empty
+) -> float:
     """Pulls an environment variable out of the environment and casts it to an
     float. If the name is not present in the environment and no default is
     specified then a ``ValueError`` will be raised. Similarly, if the
     environment value is not castable to an float, a ``ValueError`` will be
     raised.
 
     :param name: The name of the environment variable be pulled
@@ -110,18 +109,20 @@
         raise ValueError(
             "`env_float` requires either a default value to be specified, or for "
             "the variable to be present in the environment"
         )
     return float(value)
 
 
-def env_bool(name: str,
-             truthy_values: Iterable[Any] = TRUE_VALUES,
-             required: bool = False,
-             default: Union[Type[empty], bool] = empty) -> bool:
+def env_bool(
+    name: str,
+    truthy_values: Iterable[Any] = TRUE_VALUES,
+    required: bool = False,
+    default: Union[Type[empty], bool] = empty,
+) -> bool:
     """Pulls an environment variable out of the environment returning it as a
     boolean. The strings ``'True'`` and ``'true'`` are the default *truthy*
     values. If not present in the environment and no default is specified,
     ``None`` is returned.
 
     :param name: The name of the environment variable be pulled
     :type name: str
@@ -141,15 +142,17 @@
     """
     value = get_env_value(name, required=required, default=default)
     if value is empty:
         return None
     return value in TRUE_VALUES
 
 
-def env_string(name: str, required: bool = False, default: Union[Type[empty], str] = empty) -> str:
+def env_string(
+    name: str, required: bool = False, default: Union[Type[empty], str] = empty
+) -> str:
     """Pulls an environment variable out of the environment returning it as a
     string. If not present in the environment and no default is specified, an
     empty string is returned.
 
     :param name: The name of the environment variable be pulled
     :type name: str
 
@@ -160,22 +163,24 @@
     :param default: The value to return if the environment variable is not
     present. (Providing a default alongside setting ``required=True`` will raise
     a ``ValueError``)
     :type default: bool
     """
     value = get_env_value(name, default=default, required=required)
     if value is empty:
-        value = ''
+        value = ""
     return value
 
 
-def env_list(name: str,
-             separator: str = ',',
-             required: bool = False,
-             default: Union[Type[empty], List[Any]] = empty) -> List[Any]:
+def env_list(
+    name: str,
+    separator: str = ",",
+    required: bool = False,
+    default: Union[Type[empty], List[Any]] = empty,
+) -> List[Any]:
     """Pulls an environment variable out of the environment, splitting it on a
     separator, and returning it as a list. Extra whitespace on the list values
     is stripped. List values that evaluate as falsy are removed. If not present
     and no default specified, an empty list is returned.
 
     :param name: The name of the environment variable be pulled
     :type name: str
@@ -195,21 +200,23 @@
     value = get_env_value(name, required=required, default=default)
     if value is empty:
         return []
     # wrapped in list to force evaluation in python 3
     return list(filter(bool, [v.strip() for v in value.split(separator)]))
 
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
-def get(name: str,
-        required: bool = False,
-        default: Union[Type[empty], T] = empty,
-        type: Type[T] = None) -> T:
+def get(
+    name: str,
+    required: bool = False,
+    default: Union[Type[empty], T] = empty,
+    type: Type[T] = None,
+) -> T:
     """Generic getter for environment variables. Handles defaults,
     required-ness, and what type to expect.
 
     :param name: The name of the environment variable be pulled
     :type name: str
 
     :param required: Whether the environment variable is required. If ``True``
@@ -221,25 +228,21 @@
     a ``ValueError``)
     :type default: bool
 
     :param type: The type of variable expected.
     :param type: str or type
     """
     fns: Dict[Union[str, Type[Any]], Callable[..., Any]] = {
-        'int': env_int,
+        "int": env_int,
         int: env_int,
-
         # 'float': env_float,
         # float: env_float,
-
-        'bool': env_bool,
+        "bool": env_bool,
         bool: env_bool,
-
-        'string': env_string,
+        "string": env_string,
         str: env_string,
-
-        'list': env_list,
+        "list": env_list,
         list: env_list,
     }
 
     fn = fns.get(type, env_string)
     return fn(name, default=default, required=required)
```

### Comparing `py-evm-0.7.0a1/eth/_utils/generator.py` & `py-evm-0.7.0a2/eth/_utils/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
     Generic,
     Iterable,
     Iterator,
     List,
     TypeVar,
 )
 
-
-TItem = TypeVar('TItem')
+TItem = TypeVar("TItem")
 
 
 class CachedIterable(Generic[TItem], Iterable[TItem]):
     def __init__(self, iterable: Iterable[TItem]) -> None:
         self._cached_results: List[TItem] = []
         self._iterator = iter(iterable)
```

### Comparing `py-evm-0.7.0a1/eth/_utils/headers.py` & `py-evm-0.7.0a2/eth/_utils/headers.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,27 @@
     Tuple,
 )
 
 from eth_typing import (
     Address,
 )
 
-from eth.abc import BlockHeaderAPI
+from eth.abc import (
+    BlockHeaderAPI,
+)
 from eth.constants import (
     BLANK_ROOT_HASH,
-    GENESIS_BLOCK_NUMBER,
-    GENESIS_PARENT_HASH,
-    GAS_LIMIT_EMA_DENOMINATOR,
     GAS_LIMIT_ADJUSTMENT_FACTOR,
+    GAS_LIMIT_EMA_DENOMINATOR,
     GAS_LIMIT_MAXIMUM,
     GAS_LIMIT_MINIMUM,
-    GAS_LIMIT_USAGE_ADJUSTMENT_NUMERATOR,
     GAS_LIMIT_USAGE_ADJUSTMENT_DENOMINATOR,
+    GAS_LIMIT_USAGE_ADJUSTMENT_NUMERATOR,
+    GENESIS_BLOCK_NUMBER,
+    GENESIS_PARENT_HASH,
     ZERO_ADDRESS,
 )
 from eth.typing import (
     BlockNumber,
     HeaderParams,
 )
 
@@ -50,69 +52,69 @@
         return max(
             parent.timestamp + 1,
             eth_now(),
         )
 
 
 def fill_header_params_from_parent(
-        parent: BlockHeaderAPI,
-        gas_limit: int,
-        difficulty: int,
-        timestamp: int,
-        coinbase: Address = ZERO_ADDRESS,
-        nonce: bytes = None,
-        extra_data: bytes = None,
-        transaction_root: bytes = None,
-        state_root: bytes = None,
-        mix_hash: bytes = None,
-        receipt_root: bytes = None) -> Dict[str, HeaderParams]:
-
+    parent: BlockHeaderAPI,
+    gas_limit: int,
+    difficulty: int,
+    timestamp: int,
+    coinbase: Address = ZERO_ADDRESS,
+    nonce: bytes = None,
+    extra_data: bytes = None,
+    transaction_root: bytes = None,
+    state_root: bytes = None,
+    mix_hash: bytes = None,
+    receipt_root: bytes = None,
+) -> Dict[str, HeaderParams]:
     if parent is None:
         parent_hash = GENESIS_PARENT_HASH
         block_number = GENESIS_BLOCK_NUMBER
         if state_root is None:
             state_root = BLANK_ROOT_HASH
     else:
         parent_hash = parent.hash
         block_number = BlockNumber(parent.block_number + 1)
 
         if state_root is None:
             state_root = parent.state_root
 
     header_kwargs: Dict[str, HeaderParams] = {
-        'parent_hash': parent_hash,
-        'coinbase': coinbase,
-        'state_root': state_root,
-        'gas_limit': gas_limit,
-        'difficulty': difficulty,
-        'block_number': block_number,
-        'timestamp': timestamp,
+        "parent_hash": parent_hash,
+        "coinbase": coinbase,
+        "state_root": state_root,
+        "gas_limit": gas_limit,
+        "difficulty": difficulty,
+        "block_number": block_number,
+        "timestamp": timestamp,
     }
     if nonce is not None:
-        header_kwargs['nonce'] = nonce
+        header_kwargs["nonce"] = nonce
     if extra_data is not None:
-        header_kwargs['extra_data'] = extra_data
+        header_kwargs["extra_data"] = extra_data
     if transaction_root is not None:
-        header_kwargs['transaction_root'] = transaction_root
+        header_kwargs["transaction_root"] = transaction_root
     if receipt_root is not None:
-        header_kwargs['receipt_root'] = receipt_root
+        header_kwargs["receipt_root"] = receipt_root
     if mix_hash is not None:
-        header_kwargs['mix_hash'] = mix_hash
+        header_kwargs["mix_hash"] = mix_hash
 
     return header_kwargs
 
 
 def compute_gas_limit_bounds(previous_limit: int) -> Tuple[int, int]:
     """
     Compute the boundaries for the block gas limit based on the parent block.
     """
     boundary_range = previous_limit // GAS_LIMIT_ADJUSTMENT_FACTOR
 
     # the boundary range is the exclusive limit, therefore the inclusive bounds are
-    # (boundary_range - 1) and (boundary_range + 1) for upper and lower bounds, respectively
+    # (boundary_range - 1) and (boundary_range + 1) for upper and lower bounds, respectively  # noqa: E501
     upper_bound_inclusive = min(GAS_LIMIT_MAXIMUM, previous_limit + boundary_range - 1)
     lower_bound_inclusive = max(GAS_LIMIT_MINIMUM, previous_limit - boundary_range + 1)
     return lower_bound_inclusive, upper_bound_inclusive
 
 
 def compute_gas_limit(parent_header: BlockHeaderAPI, genesis_gas_limit: int) -> int:
     """
@@ -141,27 +143,25 @@
     if parent_header is None:
         return genesis_gas_limit
 
     decay = parent_header.gas_limit // GAS_LIMIT_EMA_DENOMINATOR
 
     if parent_header.gas_used:
         usage_increase = (
-            parent_header.gas_used * GAS_LIMIT_USAGE_ADJUSTMENT_NUMERATOR
-        ) // (
-            GAS_LIMIT_USAGE_ADJUSTMENT_DENOMINATOR
-        ) // (
-            GAS_LIMIT_EMA_DENOMINATOR
+            (parent_header.gas_used * GAS_LIMIT_USAGE_ADJUSTMENT_NUMERATOR)
+            // (GAS_LIMIT_USAGE_ADJUSTMENT_DENOMINATOR)
+            // (GAS_LIMIT_EMA_DENOMINATOR)
         )
     else:
         usage_increase = 0
 
     gas_limit = max(
         GAS_LIMIT_MINIMUM,
         # + 1 because the decay is an exclusive limit we have to remain inside of
-        (parent_header.gas_limit - decay + 1) + usage_increase
+        (parent_header.gas_limit - decay + 1) + usage_increase,
     )
 
     if gas_limit < GAS_LIMIT_MINIMUM:
         return GAS_LIMIT_MINIMUM
     elif gas_limit < genesis_gas_limit:
         # - 1 because the decay is an exclusive limit we have to remain inside of
         return parent_header.gas_limit + decay - 1
```

### Comparing `py-evm-0.7.0a1/eth/_utils/module_loading.py` & `py-evm-0.7.0a2/eth/_utils/module_loading.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from importlib import (
+    import_module,
+)
 import operator
-from importlib import import_module
-
 from types import (
     ModuleType,
 )
 from typing import (
     Tuple,
 )
 
@@ -12,35 +13,35 @@
 def import_string(dotted_path: str) -> ModuleType:
     """
     Source: django.utils.module_loading
     Import a dotted module path and return the attribute/class designated by the
     last name in the path. Raise ImportError if the import failed.
     """
     try:
-        module_path, class_name = dotted_path.rsplit('.', 1)
+        module_path, class_name = dotted_path.rsplit(".", 1)
     except ValueError:
         msg = f"{dotted_path} doesn't look like a module path"
         raise ImportError(msg)
 
     module = import_module(module_path)
 
     try:
         return getattr(module, class_name)
     except AttributeError:
         msg = f'Module "{module_path}" does not define a "{class_name}" attribute/class'
         raise ImportError(msg)
 
 
 def split_at_longest_importable_path(dotted_path: str) -> Tuple[str, str]:
-    num_path_parts = len(dotted_path.split('.'))
+    num_path_parts = len(dotted_path.split("."))
 
     for i in range(1, num_path_parts):
-        path_parts = dotted_path.rsplit('.', i)
+        path_parts = dotted_path.rsplit(".", i)
         import_part = path_parts[0]
-        remainder = '.'.join(path_parts[1:])
+        remainder = ".".join(path_parts[1:])
 
         try:
             module = import_module(import_part)
         except ImportError:
             continue
 
         try:
@@ -48,8 +49,8 @@
         except AttributeError:
             raise ImportError(
                 f"Unable to derive appropriate import path for {dotted_path}"
             )
         else:
             return import_part, remainder
     else:
-        return '', dotted_path
+        return "", dotted_path
```

### Comparing `py-evm-0.7.0a1/eth/_utils/numeric.py` & `py-evm-0.7.0a2/eth/_utils/numeric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 import decimal
 import functools
 import itertools
 from typing import (
     Union,
 )
 
-from eth_utils.toolz import (
-    curry,
-)
 from eth_typing import (
     Hash32,
 )
+from eth_utils.toolz import (
+    curry,
+)
 
 from eth.constants import (
     UINT_255_MAX,
-    UINT_256_MAX,
     UINT_256_CEILING,
+    UINT_256_MAX,
 )
 
 
 def int_to_bytes32(value: Union[int, bool]) -> Hash32:
     if not isinstance(value, int) or isinstance(value, bool):
-        raise ValueError(
-            f"Value must be an integer: Got: {type(value)}"
-        )
+        raise ValueError(f"Value must be an integer: Got: {type(value)}")
     if value < 0:
-        raise ValueError(
-            f"Value cannot be negative: Got: {value}"
-        )
+        raise ValueError(f"Value cannot be negative: Got: {value}")
     if value > UINT_256_MAX:
-        raise ValueError(
-            f"Value exeeds maximum UINT256 size.  Got: {value}"
-        )
-    value_bytes = value.to_bytes(32, 'big')
+        raise ValueError(f"Value exeeds maximum UINT256 size.  Got: {value}")
+    value_bytes = value.to_bytes(32, "big")
     return Hash32(value_bytes)
 
 
 def ceilXX(value: int, ceiling: int) -> int:
     remainder = value % ceiling
     if remainder == 0:
         return value
@@ -77,17 +71,15 @@
             return bit_length
         value >>= 1
 
     raise Exception("Invariant: unreachable code path")
 
 
 @curry
-def clamp(inclusive_lower_bound: int,
-          inclusive_upper_bound: int,
-          value: int) -> int:
+def clamp(inclusive_lower_bound: int, inclusive_upper_bound: int, value: int) -> int:
     """
     Bound the given ``value`` between ``inclusive_lower_bound`` and
     ``inclusive_upper_bound``.
     """
     if value <= inclusive_lower_bound:
         return inclusive_lower_bound
     elif value >= inclusive_upper_bound:
@@ -101,18 +93,14 @@
     Return the integer square root of ``value``.
 
     Uses Python's decimal module to compute the square root of ``value`` with
     a precision of 128-bits. The value 128 is chosen since the largest square
     root of a 256-bit integer is a 128-bit integer.
     """
     if not isinstance(value, int) or isinstance(value, bool):
-        raise ValueError(
-            f"Value must be an integer: Got: {type(value)}"
-        )
+        raise ValueError(f"Value must be an integer: Got: {type(value)}")
     if value < 0:
-        raise ValueError(
-            f"Value cannot be negative: Got: {value}"
-        )
+        raise ValueError(f"Value cannot be negative: Got: {value}")
 
     with decimal.localcontext() as ctx:
         ctx.prec = 128
         return int(decimal.Decimal(value).sqrt())
```

### Comparing `py-evm-0.7.0a1/eth/_utils/rlp.py` & `py-evm-0.7.0a2/eth/_utils/rlp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-import rlp
 from typing import (
     Iterable,
     Optional,
     Tuple,
 )
 
-from eth_utils.toolz import (
-    curry,
-)
-
 from eth_utils import (
-    to_tuple,
     ValidationError,
+    to_tuple,
+)
+from eth_utils.toolz import (
+    curry,
 )
+import rlp
 
 from eth.rlp.blocks import (
     BaseBlock,
 )
 
 
 @to_tuple
-def diff_rlp_object(left: BaseBlock,
-                    right: BaseBlock) -> Optional[Iterable[Tuple[str, str, str]]]:
+def diff_rlp_object(
+    left: BaseBlock, right: BaseBlock
+) -> Optional[Iterable[Tuple[str, str, str]]]:
     if left != right:
         rlp_type = type(left)
 
         for field_name, field_type in rlp_type._meta.fields:
             left_value = getattr(left, field_name)
             right_value = getattr(right, field_name)
-            if isinstance(field_type, type) and issubclass(field_type, rlp.Serializable):
+            if isinstance(field_type, type) and issubclass(
+                field_type, rlp.Serializable
+            ):
                 sub_diff = diff_rlp_object(left_value, right_value)
                 for sub_field_name, sub_left_value, sub_right_value in sub_diff:
                     yield (
                         f"{field_name}.{sub_field_name}",
                         sub_left_value,
                         sub_right_value,
                     )
@@ -50,18 +52,16 @@
                     right_value,
                 )
             else:
                 continue
 
 
 def _humanized_diff_elements(
-        diff: Iterable[Tuple[str, str, str]],
-        obj_a_name: str,
-        obj_b_name: str) -> Iterable[str]:
-
+    diff: Iterable[Tuple[str, str, str]], obj_a_name: str, obj_b_name: str
+) -> Iterable[str]:
     longest_obj_name = max(len(obj_a_name), len(obj_b_name))
 
     for field_name, a_val, b_val in diff:
         if isinstance(a_val, int) and isinstance(b_val, int):
             element_diff = b_val - a_val
             if element_diff > 0:
                 element_diff_display = f" (+{element_diff})"
@@ -69,30 +69,29 @@
                 element_diff_display = f" ({element_diff})"
         else:
             element_diff_display = ""
 
         yield (
             f"{field_name}:\n"
             f"    ({obj_a_name.ljust(longest_obj_name, ' ')}) : {a_val}\n"
-            f"    ({obj_b_name.ljust(longest_obj_name, ' ')}) : {b_val}{element_diff_display}"
+            f"    ({obj_b_name.ljust(longest_obj_name, ' ')}) : {b_val}{element_diff_display}"  # noqa: E501
         )
 
 
 @curry
-def validate_rlp_equal(obj_a: BaseBlock,
-                       obj_b: BaseBlock,
-                       obj_a_name: str = None,
-                       obj_b_name: str = None) -> None:
+def validate_rlp_equal(
+    obj_a: BaseBlock, obj_b: BaseBlock, obj_a_name: str = None, obj_b_name: str = None
+) -> None:
     if obj_a == obj_b:
         return
 
     if obj_a_name is None:
-        obj_a_name = obj_a.__class__.__name__ + '_a'
+        obj_a_name = obj_a.__class__.__name__ + "_a"
     if obj_b_name is None:
-        obj_b_name = obj_b.__class__.__name__ + '_b'
+        obj_b_name = obj_b.__class__.__name__ + "_b"
 
     diff = diff_rlp_object(obj_a, obj_b)
     if len(diff) == 0:
         raise TypeError(
             f"{obj_a_name} ({obj_a!r}) != "
             f"{obj_b_name} ({obj_b!r}) but got an empty diff"
         )
```

### Comparing `py-evm-0.7.0a1/eth/_utils/spoof.py` & `py-evm-0.7.0a2/eth/_utils/spoof.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,51 +4,52 @@
     Union,
 )
 
 from eth_utils.toolz import (
     merge,
 )
 
-from eth.constants import (
-    DEFAULT_SPOOF_Y_PARITY,
-    DEFAULT_SPOOF_R,
-    DEFAULT_SPOOF_S,
-)
-
 from eth.abc import (
     SignedTransactionAPI,
     UnsignedTransactionAPI,
 )
+from eth.constants import (
+    DEFAULT_SPOOF_R,
+    DEFAULT_SPOOF_S,
+    DEFAULT_SPOOF_Y_PARITY,
+)
 
 SPOOF_ATTRIBUTES_DEFAULTS = {
-    'y_parity': DEFAULT_SPOOF_Y_PARITY,
-    'r': DEFAULT_SPOOF_R,
-    's': DEFAULT_SPOOF_S
+    "y_parity": DEFAULT_SPOOF_Y_PARITY,
+    "r": DEFAULT_SPOOF_R,
+    "s": DEFAULT_SPOOF_S,
 }
 
-T = TypeVar('T', bound='SpoofAttributes')
+T = TypeVar("T", bound="SpoofAttributes")
 
 
 class SpoofAttributes:
     def __init__(
-            self,
-            spoof_target: Union[SignedTransactionAPI, UnsignedTransactionAPI],
-            **overrides: Any) -> None:
+        self,
+        spoof_target: Union[SignedTransactionAPI, UnsignedTransactionAPI],
+        **overrides: Any
+    ) -> None:
         self.spoof_target = spoof_target
         self.overrides = overrides
 
-        if 'from_' in overrides:
-            if hasattr(spoof_target, 'sender'):
+        if "from_" in overrides:
+            if hasattr(spoof_target, "sender"):
                 raise TypeError(
-                    "A from_ parameter can only be supplied when the spoof target",
-                    "does not have a sender attribute.  SpoofTransaction will not attempt",
-                    "to override the sender of a signed transaction.")
+                    "A from_ parameter can only be supplied when the spoof target "
+                    "does not have a sender attribute.  SpoofTransaction will not "
+                    "attempt to override the sender of a signed transaction."
+                )
 
-            overrides['sender'] = overrides['from_']
-            overrides['get_sender'] = lambda: overrides['from_']
+            overrides["sender"] = overrides["from_"]
+            overrides["get_sender"] = lambda: overrides["from_"]
             for attr, value in SPOOF_ATTRIBUTES_DEFAULTS.items():
                 if not hasattr(spoof_target, attr):
                     overrides[attr] = value
 
     def __getattr__(self, attr: str) -> Any:
         if attr in self.overrides:
             return self.overrides[attr]
```

### Comparing `py-evm-0.7.0a1/eth/_utils/state.py` & `py-evm-0.7.0a2/eth/_utils/state.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,40 +2,39 @@
     to_tuple,
 )
 
 from eth.typing import (
     AccountDiff,
     AccountState,
 )
-from eth.vm.state import BaseState
+from eth.vm.state import (
+    BaseState,
+)
 
 
 @to_tuple
-def diff_state(
-        expected_state: AccountState,
-        state: BaseState) -> AccountDiff:
-
+def diff_state(expected_state: AccountState, state: BaseState) -> AccountDiff:
     for account, account_data in sorted(expected_state.items()):
-        expected_balance = account_data['balance']
-        expected_nonce = account_data['nonce']
-        expected_code = account_data['code']
+        expected_balance = account_data["balance"]
+        expected_nonce = account_data["nonce"]
+        expected_code = account_data["code"]
 
         actual_nonce = state.get_nonce(account)
         actual_code = state.get_code(account)
         actual_balance = state.get_balance(account)
 
         if actual_nonce != expected_nonce:
-            yield (account, 'nonce', actual_nonce, expected_nonce)
+            yield (account, "nonce", actual_nonce, expected_nonce)
         if actual_code != expected_code:
-            yield (account, 'code', actual_code, expected_code)
+            yield (account, "code", actual_code, expected_code)
         if actual_balance != expected_balance:
-            yield (account, 'balance', actual_balance, expected_balance)
+            yield (account, "balance", actual_balance, expected_balance)
 
-        for slot, expected_storage_value in sorted(account_data['storage'].items()):
+        for slot, expected_storage_value in sorted(account_data["storage"].items()):
             actual_storage_value = state.get_storage(account, slot)
             if actual_storage_value != expected_storage_value:
                 yield (
                     account,
-                    f'storage[{slot}]',
+                    f"storage[{slot}]",
                     actual_storage_value,
                     expected_storage_value,
                 )
```

### Comparing `py-evm-0.7.0a1/eth/_utils/transactions.py` & `py-evm-0.7.0a2/eth/_utils/transactions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-from typing import NamedTuple
-
-import rlp
+from typing import (
+    NamedTuple,
+)
 
-from eth_keys import keys
-from eth_keys import datatypes
+from eth_keys import (
+    datatypes,
+    keys,
+)
 from eth_keys.exceptions import (
     BadSignature,
 )
-
 from eth_utils import (
-    int_to_big_endian,
     ValidationError,
+    int_to_big_endian,
 )
+import rlp
 
+from eth._utils.numeric import (
+    is_even,
+)
 from eth.abc import (
     SignedTransactionAPI,
     UnsignedTransactionAPI,
 )
 from eth.constants import (
     CREATE_CONTRACT_ADDRESS,
 )
+from eth.rlp.transactions import (
+    BaseTransaction,
+)
 from eth.typing import (
-    Address,
     VRS,
+    Address,
 )
-from eth._utils.numeric import (
-    is_even,
-)
-
-from eth.rlp.transactions import BaseTransaction
-
 
 EIP155_CHAIN_ID_OFFSET = 35
 # Add this offset to y_parity to get "v" for legacy transactions, from Frontier
 V_OFFSET = 27
 
 
 def is_eip_155_signed_transaction(transaction: BaseTransaction) -> bool:
@@ -50,24 +52,27 @@
 def extract_signature_v(v: int) -> int:
     if is_even(v):
         return V_OFFSET + 1
     else:
         return V_OFFSET
 
 
-def create_transaction_signature(unsigned_txn: UnsignedTransactionAPI,
-                                 private_key: datatypes.PrivateKey,
-                                 chain_id: int = None) -> VRS:
-
+def create_transaction_signature(
+    unsigned_txn: UnsignedTransactionAPI,
+    private_key: datatypes.PrivateKey,
+    chain_id: int = None,
+) -> VRS:
     transaction_parts = rlp.decode(rlp.encode(unsigned_txn))
 
     if chain_id:
-        transaction_parts_for_signature = (
-            transaction_parts + [int_to_big_endian(chain_id), b'', b'']
-        )
+        transaction_parts_for_signature = transaction_parts + [
+            int_to_big_endian(chain_id),
+            b"",
+            b"",
+        ]
     else:
         transaction_parts_for_signature = transaction_parts
 
     message = rlp.encode(transaction_parts_for_signature)
     signature = private_key.sign_msg(message)
 
     canonical_v, r, s = signature.vrs
@@ -106,18 +111,18 @@
     gas_tx: int
     gas_txcreate: int
     gas_txdatazero: int
     gas_txdatanonzero: int
 
 
 def calculate_intrinsic_gas(
-        gas_schedule: IntrinsicGasSchedule,
-        transaction: SignedTransactionAPI,
+    gas_schedule: IntrinsicGasSchedule,
+    transaction: SignedTransactionAPI,
 ) -> int:
-    num_zero_bytes = transaction.data.count(b'\x00')
+    num_zero_bytes = transaction.data.count(b"\x00")
     num_non_zero_bytes = len(transaction.data) - num_zero_bytes
     if transaction.to == CREATE_CONTRACT_ADDRESS:
         create_cost = gas_schedule.gas_txcreate
     else:
         create_cost = 0
     return (
         gas_schedule.gas_tx
```

### Comparing `py-evm-0.7.0a1/eth/abc.py` & `py-evm-0.7.0a2/eth/abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 from abc import (
     ABC,
-    abstractmethod
+    abstractmethod,
 )
 from typing import (
     Any,
     Callable,
     ClassVar,
     ContextManager,
     Dict,
     FrozenSet,
+    Hashable,
     Iterable,
     Iterator,
     List,
     MutableMapping,
     NamedTuple,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
-    Hashable,
 )
 
-from eth_bloom import BloomFilter
-
+from eth_bloom import (
+    BloomFilter,
+)
+from eth_keys.datatypes import (
+    PrivateKey,
+)
 from eth_typing import (
     Address,
     BlockNumber,
     Hash32,
 )
-
-from eth_utils import ExtendedDebugLogger
-
-from eth_keys.datatypes import PrivateKey
+from eth_utils import (
+    ExtendedDebugLogger,
+)
 
 from eth.constants import (
     BLANK_ROOT_HASH,
 )
-
-from eth.exceptions import VMError
+from eth.exceptions import (
+    VMError,
+)
 from eth.typing import (
+    AccountState,
     BytesOrView,
     ChainGaps,
-    JournalDBCheckpoint,
-    AccountState,
     HeaderParams,
+    JournalDBCheckpoint,
     VMConfiguration,
 )
 
-
-T = TypeVar('T')
+T = TypeVar("T")
 
 # A decoded RLP object of unknown interpretation, with a maximum "depth" of 1.
 DecodedZeroOrOneLayerRLP = Union[bytes, List[bytes]]
 
 
 class MiningHeaderAPI(ABC):
     """
-    A class to define a block header without ``mix_hash`` and ``nonce`` which can act as a
-    temporary representation during mining before the block header is sealed.
+    A class to define a block header without ``mix_hash`` and ``nonce`` which can act as
+    a temporary representation during mining before the block header is sealed.
     """
+
     parent_hash: Hash32
     uncles_hash: Hash32
     coinbase: Address
     state_root: Hash32
     transaction_root: Hash32
     receipt_root: Hash32
     bloom: int
@@ -150,54 +154,56 @@
 
     The header may be one of several definitions, like a London (EIP-1559) or
     pre-London header.
     """
 
     @classmethod
     @abstractmethod
-    def deserialize(cls, encoded: List[bytes]) -> 'BlockHeaderAPI':
+    def deserialize(cls, encoded: List[bytes]) -> "BlockHeaderAPI":
         """
         Extract a header from an encoded RLP object.
 
         This method is used by rlp.decode(..., sedes=TransactionBuilderAPI).
         """
         ...
 
     @classmethod
     @abstractmethod
-    def serialize(cls, obj: 'BlockHeaderAPI') -> List[bytes]:
+    def serialize(cls, obj: "BlockHeaderAPI") -> List[bytes]:
         """
         Encode a header to a series of bytes used by RLP.
 
         This method is used by rlp.encode(obj).
         """
         ...
 
 
 class BlockHeaderAPI(MiningHeaderAPI, BlockHeaderSedesAPI):
     """
-    A class derived from :class:`~eth.abc.MiningHeaderAPI` to define a block header after it is
-    sealed.
+    A class derived from :class:`~eth.abc.MiningHeaderAPI` to define a block header
+    after it is sealed.
     """
+
     mix_hash: Hash32
     nonce: bytes
 
     # We can remove this API and inherit from rlp.Serializable when it becomes typesafe
     @abstractmethod
-    def copy(self, *args: Any, **kwargs: Any) -> 'BlockHeaderAPI':
+    def copy(self, *args: Any, **kwargs: Any) -> "BlockHeaderAPI":
         """
         Return a copy of the header, optionally overwriting any of its properties.
         """
         ...
 
 
 class LogAPI(ABC):
     """
     A class to define a written log.
     """
+
     address: Address
     topics: Sequence[int]
     data: bytes
 
     @property
     @abstractmethod
     def bloomables(self) -> Tuple[bytes, ...]:
@@ -231,20 +237,20 @@
 
     @property
     @abstractmethod
     def bloom_filter(self) -> BloomFilter:
         ...
 
     # We can remove this API and inherit from rlp.Serializable when it becomes typesafe
-    def copy(self, *args: Any, **kwargs: Any) -> 'ReceiptAPI':
+    def copy(self, *args: Any, **kwargs: Any) -> "ReceiptAPI":
         """
         Return a copy of the receipt, optionally overwriting any of its properties.
         """
-        # This method isn't marked abstract because derived classes implement it by deriving from
-        # rlp.Serializable but mypy won't recognize it as implemented.
+        # This method isn't marked abstract because derived classes implement it by
+        # deriving from rlp.Serializable but mypy won't recognize it as implemented.
         ...
 
     @abstractmethod
     def encode(self) -> bytes:
         """
         This encodes a receipt, no matter if it's: a legacy receipt, a
         typed receipt, or the payload of a typed receipt. See more
@@ -291,25 +297,25 @@
 
     Some VMs support multiple distinct transaction types. In that case, the
     builder is responsible for dispatching on the different types.
     """
 
     @classmethod
     @abstractmethod
-    def deserialize(cls, encoded: DecodedZeroOrOneLayerRLP) -> 'ReceiptAPI':
+    def deserialize(cls, encoded: DecodedZeroOrOneLayerRLP) -> "ReceiptAPI":
         """
         Extract a receipt from an encoded RLP object.
 
         This method is used by rlp.decode(..., sedes=ReceiptBuilderAPI).
         """
         ...
 
     @classmethod
     @abstractmethod
-    def serialize(cls, obj: 'ReceiptAPI') -> DecodedZeroOrOneLayerRLP:
+    def serialize(cls, obj: "ReceiptAPI") -> DecodedZeroOrOneLayerRLP:
         """
         Encode a receipt to a series of bytes used by RLP.
 
         In the case of legacy receipt, it will actually be a list of
         bytes. That doesn't show up here, because pyrlp doesn't export type
         annotations.
 
@@ -318,14 +324,15 @@
         ...
 
 
 class BaseTransactionAPI(ABC):
     """
     A class to define all common methods of a transaction.
     """
+
     @abstractmethod
     def validate(self) -> None:
         """
         Hook called during instantiation to ensure that all transaction
         parameters pass validation rules.
         """
         ...
@@ -337,21 +344,21 @@
         Convenience property for the return value of `get_intrinsic_gas`
         """
         ...
 
     @abstractmethod
     def get_intrinsic_gas(self) -> int:
         """
-        Return the intrinsic gas for the transaction which is defined as the amount of gas that
-        is needed before any code runs.
+        Return the intrinsic gas for the transaction which is defined as the amount of
+        gas that is needed before any code runs.
         """
         ...
 
     @abstractmethod
-    def gas_used_by(self, computation: 'ComputationAPI') -> int:
+    def gas_used_by(self, computation: "ComputationAPI") -> int:
         """
         Return the gas used by the given computation. In Frontier,
         for example, this is sum of the intrinsic cost and the gas used
         during computation.
         """
         ...
 
@@ -372,14 +379,15 @@
         ...
 
 
 class TransactionFieldsAPI(ABC):
     """
     A class to define all common transaction fields.
     """
+
     @property
     @abstractmethod
     def nonce(self) -> int:
         ...
 
     @property
     @abstractmethod
@@ -463,26 +471,27 @@
 
 
 class UnsignedTransactionAPI(BaseTransactionAPI):
 
     """
     A class representing a transaction before it is signed.
     """
+
     nonce: int
     gas_price: int
     gas: int
     to: Address
     value: int
     data: bytes
 
     #
     # API that must be implemented by all Transaction subclasses.
     #
     @abstractmethod
-    def as_signed_transaction(self, private_key: PrivateKey) -> 'SignedTransactionAPI':
+    def as_signed_transaction(self, private_key: PrivateKey) -> "SignedTransactionAPI":
         """
         Return a version of this transaction which has been signed using the
         provided `private_key`
         """
         ...
 
 
@@ -492,15 +501,15 @@
 
     Some VMs support multiple distinct transaction types. In that case, the
     decoder is responsible for dispatching on the different types.
     """
 
     @classmethod
     @abstractmethod
-    def decode(cls, encoded: bytes) -> 'SignedTransactionAPI':
+    def decode(cls, encoded: bytes) -> "SignedTransactionAPI":
         """
         This decodes a transaction that is encoded to either a typed
         transaction or a legacy transaction, or even the payload of one of the
         transaction types. It assumes that typed transactions are *not*
         rlp-encoded first.
 
         If dealing with an object that is rlp encoded first, then use this instead:
@@ -530,78 +539,81 @@
 
     Some VMs support multiple distinct transaction types. In that case, the
     builder is responsible for dispatching on the different types.
     """
 
     @classmethod
     @abstractmethod
-    def deserialize(cls, encoded: DecodedZeroOrOneLayerRLP) -> 'SignedTransactionAPI':
+    def deserialize(cls, encoded: DecodedZeroOrOneLayerRLP) -> "SignedTransactionAPI":
         """
         Extract a transaction from an encoded RLP object.
 
         This method is used by rlp.decode(..., sedes=TransactionBuilderAPI).
         """
         ...
 
     @classmethod
     @abstractmethod
-    def serialize(cls, obj: 'SignedTransactionAPI') -> DecodedZeroOrOneLayerRLP:
+    def serialize(cls, obj: "SignedTransactionAPI") -> DecodedZeroOrOneLayerRLP:
         """
         Encode a transaction to a series of bytes used by RLP.
 
         In the case of legacy transactions, it will actually be a list of
         bytes. That doesn't show up here, because pyrlp doesn't export type
         annotations.
 
         This method is used by rlp.encode(obj).
         """
         ...
 
     @classmethod
     @abstractmethod
-    def create_unsigned_transaction(cls,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> UnsignedTransactionAPI:
+    def create_unsigned_transaction(
+        cls,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+    ) -> UnsignedTransactionAPI:
         """
         Create an unsigned transaction.
         """
         ...
 
     @classmethod
     @abstractmethod
     def new_transaction(
-            cls,
-            nonce: int,
-            gas_price: int,
-            gas: int,
-            to: Address,
-            value: int,
-            data: bytes,
-            v: int,
-            r: int,
-            s: int) -> 'SignedTransactionAPI':
+        cls,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+        v: int,
+        r: int,
+        s: int,
+    ) -> "SignedTransactionAPI":
         """
         Create a signed transaction.
         """
         ...
 
 
 class SignedTransactionAPI(BaseTransactionAPI, TransactionFieldsAPI):
-
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         ...
 
     """
     A class representing a transaction that was signed with a private key.
     """
+
     @property
     @abstractmethod
     def sender(self) -> Address:
         """
         Convenience and performance property for the return value of `get_sender`
         """
         ...
@@ -673,31 +685,33 @@
 
     #
     # Conversion to and creation of unsigned transactions.
     #
     @abstractmethod
     def get_message_for_signing(self) -> bytes:
         """
-        Return the bytestring that should be signed in order to create a signed transaction.
+        Return the bytestring that should be signed in order to create a signed
+        transaction.
         """
         ...
 
     # We can remove this API and inherit from rlp.Serializable when it becomes typesafe
     def as_dict(self) -> Dict[Hashable, Any]:
         """
         Return a dictionary representation of the transaction.
         """
         ...
 
     @abstractmethod
     def make_receipt(
-            self,
-            status: bytes,
-            gas_used: int,
-            log_entries: Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...]) -> ReceiptAPI:
+        self,
+        status: bytes,
+        gas_used: int,
+        log_entries: Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...],
+    ) -> ReceiptAPI:
         """
         Build a receipt for this transaction.
 
         Transactions have this responsibility because there are different types
         of transactions, which have different types of receipts. (See
         access-list transactions, which change the receipt encoding)
 
@@ -780,14 +794,15 @@
         ...
 
 
 class BlockAPI(ABC):
     """
     A class to define a block.
     """
+
     header: BlockHeaderAPI
     transactions: Tuple[SignedTransactionAPI, ...]
     uncles: Tuple[BlockHeaderAPI, ...]
     withdrawals: Tuple[WithdrawalAPI, ...]
 
     transaction_builder: Type[TransactionBuilderAPI] = None
     receipt_builder: Type[ReceiptBuilderAPI] = None
@@ -816,22 +831,24 @@
         """
         Return the receipt builder for the block.
         """
         ...
 
     @classmethod
     @abstractmethod
-    def from_header(cls, header: BlockHeaderAPI, chaindb: 'ChainDatabaseAPI') -> 'BlockAPI':
+    def from_header(
+        cls, header: BlockHeaderAPI, chaindb: "ChainDatabaseAPI"
+    ) -> "BlockAPI":
         """
         Instantiate a block from the given ``header`` and the ``chaindb``.
         """
         ...
 
     @abstractmethod
-    def get_receipts(self, chaindb: 'ChainDatabaseAPI') -> Tuple[ReceiptAPI, ...]:
+    def get_receipts(self, chaindb: "ChainDatabaseAPI") -> Tuple[ReceiptAPI, ...]:
         """
         Fetch the receipts for this block from the given ``chaindb``.
         """
         ...
 
     @property
     @abstractmethod
@@ -855,20 +872,20 @@
         """
         Return ``True`` if this block represents the genesis block of the chain,
         otherwise ``False``.
         """
         ...
 
     # We can remove this API and inherit from rlp.Serializable when it becomes typesafe
-    def copy(self, *args: Any, **kwargs: Any) -> 'BlockAPI':
+    def copy(self, *args: Any, **kwargs: Any) -> "BlockAPI":
         """
         Return a copy of the block, optionally overwriting any of its properties.
         """
-        # This method isn't marked abstract because derived classes implement it by deriving from
-        # rlp.Serializable but mypy won't recognize it as implemented.
+        # This method isn't marked abstract because derived classes implement it by
+        # deriving from rlp.Serializable but mypy won't recognize it as implemented.
         ...
 
 
 class MetaWitnessAPI(ABC):
     @property
     @abstractmethod
     def hashes(self) -> FrozenSet[Hash32]:
@@ -898,48 +915,53 @@
 
 
 class BlockAndMetaWitness(NamedTuple):
     """
     After evaluating a block using the VirtualMachine, this information
     becomes available.
     """
+
     block: BlockAPI
     meta_witness: MetaWitnessAPI
 
 
 class BlockPersistResult(NamedTuple):
     """
     After persisting a block into the active chain, this information
     becomes available.
     """
+
     imported_block: BlockAPI
     new_canonical_blocks: Tuple[BlockAPI, ...]
     old_canonical_blocks: Tuple[BlockAPI, ...]
 
 
 class BlockImportResult(NamedTuple):
     """
     After importing and persisting a block into the active chain, this information
     becomes available.
     """
+
     imported_block: BlockAPI
     new_canonical_blocks: Tuple[BlockAPI, ...]
     old_canonical_blocks: Tuple[BlockAPI, ...]
     meta_witness: MetaWitnessAPI
 
 
 class SchemaAPI(ABC):
     """
     A class representing a database schema that maps values to lookup keys.
     """
+
     @staticmethod
     @abstractmethod
     def make_header_chain_gaps_lookup_key() -> bytes:
         """
-        Return the lookup key to retrieve the header chain integrity info from the database.
+        Return the lookup key to retrieve the header chain integrity info from the
+        database.
         """
         ...
 
     @staticmethod
     @abstractmethod
     def make_canonical_head_hash_lookup_key() -> bytes:
         """
@@ -980,14 +1002,15 @@
         ...
 
 
 class DatabaseAPI(MutableMapping[bytes, bytes], ABC):
     """
     A class representing a database.
     """
+
     @abstractmethod
     def set(self, key: bytes, value: bytes) -> None:
         """
         Assign the ``value`` to the ``key``.
         """
         ...
 
@@ -1010,54 +1033,60 @@
     """
     The readable/writeable object returned by an atomic database when we start building
     a batch of writes to commit.
 
     Reads to this database will observe writes written during batching,
     but the writes will not actually persist until this object is committed.
     """
+
     pass
 
 
 class AtomicDatabaseAPI(DatabaseAPI):
     """
     Like ``BatchDB``, but immediately write out changes if they are
     not in an ``atomic_batch()`` context.
     """
+
     @abstractmethod
     def atomic_batch(self) -> ContextManager[AtomicWriteBatchAPI]:
         """
-        Return a :class:`~typing.ContextManager` to write an atomic batch to the database.
+        Return a :class:`~typing.ContextManager` to write an atomic batch to the
+        database.
         """
         ...
 
 
 class HeaderDatabaseAPI(ABC):
     """
     A class representing a database for block headers.
     """
+
     db: AtomicDatabaseAPI
 
     @abstractmethod
     def __init__(self, db: AtomicDatabaseAPI) -> None:
         """
         Instantiate the database from an :class:`~eth.abc.AtomicDatabaseAPI`.
         """
         ...
 
     @abstractmethod
     def get_header_chain_gaps(self) -> ChainGaps:
         """
-        Return information about gaps in the chain of headers. This consists of an ordered sequence
-        of block ranges describing the integrity of the chain. Each block range describes a missing
-        segment in the chain and each range is defined with inclusive boundaries, meaning the first
-        value describes the first missing block of that segment and the second value describes the
-        last missing block of the segment.
-
-        In addition to the sequences of block ranges a block number is included that indicates the
-        number of the first header that is known to be missing at the very tip of the chain.
+        Return information about gaps in the chain of headers. This consists of an
+        ordered sequence of block ranges describing the integrity of the chain. Each
+        block range describes a missing segment in the chain and each range is defined
+        with inclusive boundaries, meaning the first value describes the first missing
+        block of that segment and the second value describes the last missing block
+        of the segment.
+
+        In addition to the sequences of block ranges a block number is included that
+        indicates the number of the first header that is known to be missing at the
+        very tip of the chain.
         """
 
     #
     # Canonical Chain API
     #
     @abstractmethod
     def get_canonical_block_hash(self, block_number: BlockNumber) -> Hash32:
@@ -1066,15 +1095,17 @@
 
         Raise ``BlockNotFound`` if there's no block header with the given number in the
         canonical chain.
         """
         ...
 
     @abstractmethod
-    def get_canonical_block_header_by_number(self, block_number: BlockNumber) -> BlockHeaderAPI:
+    def get_canonical_block_header_by_number(
+        self, block_number: BlockNumber
+    ) -> BlockHeaderAPI:
         """
         Return the block header with the given number in the canonical chain.
 
         Raise ``HeaderNotFound`` if there's no block header with the given number in the
         canonical chain.
         """
         ...
@@ -1089,127 +1120,133 @@
     #
     # Header API
     #
     @abstractmethod
     def get_block_header_by_hash(self, block_hash: Hash32) -> BlockHeaderAPI:
         """
         Return the block header for the given ``block_hash``.
-        Raise ``HeaderNotFound`` if no header with the given ``block_hash`` exists in the database.
+        Raise ``HeaderNotFound`` if no header with the given ``block_hash`` exists
+        in the database.
         """
         ...
 
     @abstractmethod
     def get_score(self, block_hash: Hash32) -> int:
         """
         Return the score for the given ``block_hash``.
         """
         ...
 
     @abstractmethod
     def header_exists(self, block_hash: Hash32) -> bool:
         """
-        Return ``True`` if the ``block_hash`` exists in the database, otherwise ``False``.
+        Return ``True`` if the ``block_hash`` exists in the database,
+        otherwise ``False``.
         """
         ...
 
     @abstractmethod
     def persist_checkpoint_header(self, header: BlockHeaderAPI, score: int) -> None:
         """
-        Persist a checkpoint header with a trusted score. Persisting the checkpoint header
-        automatically sets it as the new canonical head.
+        Persist a checkpoint header with a trusted score. Persisting the checkpoint
+        header automatically sets it as the new canonical head.
         """
         ...
 
     @abstractmethod
-    def persist_header(self,
-                       header: BlockHeaderAPI
-                       ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
+    def persist_header(
+        self, header: BlockHeaderAPI
+    ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
         """
         Persist the ``header`` in the database.
         Return two iterable of headers, the first containing the new canonical header,
         the second containing the old canonical headers
         """
         ...
 
     @abstractmethod
-    def persist_header_chain(self,
-                             headers: Sequence[BlockHeaderAPI],
-                             genesis_parent_hash: Hash32 = None,
-                             ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
+    def persist_header_chain(
+        self,
+        headers: Sequence[BlockHeaderAPI],
+        genesis_parent_hash: Hash32 = None,
+    ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
         """
         Persist a chain of headers in the database.
         Return two iterable of headers, the first containing the new canonical headers,
         the second containing the old canonical headers
 
-        :param genesis_parent_hash: *optional* parent hash of the block that is treated as genesis.
-            Providing a ``genesis_parent_hash`` allows storage of headers that aren't (yet)
-            connected back to the true genesis header.
+        :param genesis_parent_hash: *optional* parent hash of the block that is treated
+            as genesis. Providing a ``genesis_parent_hash`` allows storage of headers
+            that aren't (yet) connected back to the true genesis header.
 
         """
         ...
 
 
 class ChainDatabaseAPI(HeaderDatabaseAPI):
     """
     A class representing a database for chain data. This class is derived from
     :class:`~eth.abc.HeaderDatabaseAPI`.
     """
+
     #
     # Header API
     #
     @abstractmethod
     def get_block_uncles(self, uncles_hash: Hash32) -> Tuple[BlockHeaderAPI, ...]:
         """
         Return an iterable of uncle headers specified by the given ``uncles_hash``
         """
         ...
 
     #
     # Block API
     #
     @abstractmethod
-    def persist_block(self,
-                      block: BlockAPI,
-                      genesis_parent_hash: Hash32 = None,
-                      ) -> Tuple[Tuple[Hash32, ...], Tuple[Hash32, ...]]:
+    def persist_block(
+        self,
+        block: BlockAPI,
+        genesis_parent_hash: Hash32 = None,
+    ) -> Tuple[Tuple[Hash32, ...], Tuple[Hash32, ...]]:
         """
         Persist the given block's header and uncles.
 
         :param block: the block that gets persisted
         :param genesis_parent_hash: *optional* parent hash of the header that is treated
-            as genesis. Providing a ``genesis_parent_hash`` allows storage of blocks that
-            aren't (yet) connected back to the true genesis header.
+            as genesis. Providing a ``genesis_parent_hash`` allows storage of blocks
+            that aren't (yet) connected back to the true genesis header.
 
         .. warning::
             This API assumes all block transactions have been persisted already. Use
-            :meth:`eth.abc.ChainDatabaseAPI.persist_unexecuted_block` to persist blocks that were
-            not executed.
+            :meth:`eth.abc.ChainDatabaseAPI.persist_unexecuted_block` to persist blocks
+            that were not executed.
         """
         ...
 
     @abstractmethod
-    def persist_unexecuted_block(self,
-                                 block: BlockAPI,
-                                 receipts: Tuple[ReceiptAPI, ...],
-                                 genesis_parent_hash: Hash32 = None
-                                 ) -> Tuple[Tuple[Hash32, ...], Tuple[Hash32, ...]]:
+    def persist_unexecuted_block(
+        self,
+        block: BlockAPI,
+        receipts: Tuple[ReceiptAPI, ...],
+        genesis_parent_hash: Hash32 = None,
+    ) -> Tuple[Tuple[Hash32, ...], Tuple[Hash32, ...]]:
         """
         Persist the given block's header, uncles, transactions, and receipts. Does
         **not** validate if state transitions are valid.
 
         :param block: the block that gets persisted
         :param receipts: the receipts for the given block
         :param genesis_parent_hash: *optional* parent hash of the header that is treated
-            as genesis. Providing a ``genesis_parent_hash`` allows storage of blocks that
-            aren't (yet) connected back to the true genesis header.
+            as genesis. Providing a ``genesis_parent_hash`` allows storage of blocks
+            that aren't (yet) connected back to the true genesis header.
 
-        This API should be used to persist blocks that the EVM does not execute but which it
-        stores to make them available. It ensures to persist receipts and transactions which
-        :meth:`eth.abc.ChainDatabaseAPI.persist_block` in contrast assumes to be persisted
-        separately.
+        This API should be used to persist blocks that the EVM does not execute but
+        which it stores to make them available. It ensures to persist receipts and
+        transactions which :meth:`eth.abc.ChainDatabaseAPI.persist_block` in contrast
+        assumes to be persisted separately.
         """
 
     @abstractmethod
     def persist_uncles(self, uncles: Tuple[BlockHeaderAPI]) -> Hash32:
         """
         Persist the list of uncles to the database.
 
@@ -1217,90 +1254,102 @@
         """
         ...
 
     #
     # Transaction API
     #
     @abstractmethod
-    def add_receipt(self,
-                    block_header: BlockHeaderAPI,
-                    index_key: int, receipt: ReceiptAPI) -> Hash32:
+    def add_receipt(
+        self, block_header: BlockHeaderAPI, index_key: int, receipt: ReceiptAPI
+    ) -> Hash32:
         """
         Add the given receipt to the provided block header.
 
         Return the updated `receipts_root` for updated block header.
         """
         ...
 
     @abstractmethod
-    def add_transaction(self,
-                        block_header: BlockHeaderAPI,
-                        index_key: int, transaction: SignedTransactionAPI) -> Hash32:
+    def add_transaction(
+        self,
+        block_header: BlockHeaderAPI,
+        index_key: int,
+        transaction: SignedTransactionAPI,
+    ) -> Hash32:
         """
         Add the given transaction to the provided block header.
 
         Return the updated `transactions_root` for updated block header.
         """
         ...
 
     @abstractmethod
     def get_block_transactions(
-            self,
-            block_header: BlockHeaderAPI,
-            transaction_decoder: Type[TransactionDecoderAPI]) -> Tuple[SignedTransactionAPI, ...]:
+        self,
+        block_header: BlockHeaderAPI,
+        transaction_decoder: Type[TransactionDecoderAPI],
+    ) -> Tuple[SignedTransactionAPI, ...]:
         """
         Return an iterable of transactions for the block speficied by the
         given block header.
         """
         ...
 
     @abstractmethod
-    def get_block_transaction_hashes(self, block_header: BlockHeaderAPI) -> Tuple[Hash32, ...]:
+    def get_block_transaction_hashes(
+        self, block_header: BlockHeaderAPI
+    ) -> Tuple[Hash32, ...]:
         """
-        Return a tuple cointaining the hashes of the transactions of the given ``block_header``.
+        Return a tuple cointaining the hashes of the transactions of the
+        given ``block_header``.
         """
         ...
 
     @abstractmethod
-    def get_receipt_by_index(self,
-                             block_number: BlockNumber,
-                             receipt_index: int,
-                             receipt_decoder: Type[ReceiptDecoderAPI]) -> ReceiptAPI:
+    def get_receipt_by_index(
+        self,
+        block_number: BlockNumber,
+        receipt_index: int,
+        receipt_decoder: Type[ReceiptDecoderAPI],
+    ) -> ReceiptAPI:
         """
         Return the receipt of the transaction at specified index
         for the block header obtained by the specified block number
         """
         ...
 
     @abstractmethod
-    def get_receipts(self,
-                     header: BlockHeaderAPI,
-                     receipt_decoder: Type[ReceiptDecoderAPI]) -> Tuple[ReceiptAPI, ...]:
+    def get_receipts(
+        self, header: BlockHeaderAPI, receipt_decoder: Type[ReceiptDecoderAPI]
+    ) -> Tuple[ReceiptAPI, ...]:
         """
         Return a tuple of receipts for the block specified by the given
         block header.
         """
         ...
 
     @abstractmethod
     def get_transaction_by_index(
-            self,
-            block_number: BlockNumber,
-            transaction_index: int,
-            transaction_decoder: Type[TransactionDecoderAPI]) -> SignedTransactionAPI:
+        self,
+        block_number: BlockNumber,
+        transaction_index: int,
+        transaction_decoder: Type[TransactionDecoderAPI],
+    ) -> SignedTransactionAPI:
         """
         Return the transaction at the specified `transaction_index` from the
         block specified by `block_number` from the canonical chain.
 
         Raise ``TransactionNotFound`` if no block with that ``block_number`` exists.
         """
         ...
 
     @abstractmethod
-    def get_transaction_index(self, transaction_hash: Hash32) -> Tuple[BlockNumber, int]:
+    def get_transaction_index(
+        self, transaction_hash: Hash32
+    ) -> Tuple[BlockNumber, int]:
         """
         Return a 2-tuple of (block_number, transaction_index) indicating which
         block the given transaction can be found in and at what index in the
         block transactions.
 
         Raise ``TransactionNotFound`` if the transaction_hash is not found in the
         canonical chain.
@@ -1331,15 +1380,16 @@
         Return ``True`` if the given key exists in the database.
         """
         ...
 
     @abstractmethod
     def get(self, key: bytes) -> bytes:
         """
-        Return the value for the given key or a KeyError if it doesn't exist in the database.
+        Return the value for the given key or a KeyError if it doesn't exist in the
+        database.
         """
         ...
 
     @abstractmethod
     def persist_trie_data_dict(self, trie_data_dict: Dict[Hash32, bytes]) -> None:
         """
         Store raw trie data to db from a dict
@@ -1347,14 +1397,16 @@
         ...
 
 
 class GasMeterAPI(ABC):
     """
     A class to define a gas meter.
     """
+
+    start_gas: int
     gas_refunded: int
     gas_remaining: int
 
     #
     # Write API
     #
     @abstractmethod
@@ -1379,40 +1431,40 @@
         ...
 
 
 class MessageAPI(ABC):
     """
     A message for VM computation.
     """
+
     code: bytes
     _code_address: Address
     create_address: Address
     data: BytesOrView
     depth: int
     gas: int
     is_static: bool
     sender: Address
     should_transfer_value: bool
     _storage_address: Address
     to: Address
     value: int
 
     __slots__ = [
-        'code',
-        '_code_address',
-        'create_address',
-        'data',
-        'depth',
-        'gas',
-        'is_static',
-        'sender',
-        'should_transfer_value',
-        '_storage_address'
-        'to',
-        'value',
+        "code",
+        "_code_address",
+        "create_address",
+        "data",
+        "depth",
+        "gas",
+        "is_static",
+        "sender",
+        "should_transfer_value",
+        "_storage_address" "to",
+        "value",
     ]
 
     @property
     @abstractmethod
     def code_address(self) -> Address:
         ...
 
@@ -1432,53 +1484,57 @@
         ...
 
 
 class OpcodeAPI(ABC):
     """
     A class representing an opcode.
     """
+
     mnemonic: str
 
     @abstractmethod
-    def __call__(self, computation: 'ComputationAPI') -> None:
+    def __call__(self, computation: "ComputationAPI") -> None:
         """
         Execute the logic of the opcode.
         """
         ...
 
     @classmethod
     @abstractmethod
-    def as_opcode(cls: Type[T],
-                  logic_fn: Callable[['ComputationAPI'], None],
-                  mnemonic: str,
-                  gas_cost: int) -> T:
+    def as_opcode(
+        cls: Type[T],
+        logic_fn: Callable[["ComputationAPI"], None],
+        mnemonic: str,
+        gas_cost: int,
+    ) -> T:
         """
         Class factory method for turning vanilla functions into Opcodes.
         """
         ...
 
     @abstractmethod
-    def __copy__(self) -> 'OpcodeAPI':
+    def __copy__(self) -> "OpcodeAPI":
         """
         Return a copy of the opcode.
         """
         ...
 
     @abstractmethod
-    def __deepcopy__(self, memo: Any) -> 'OpcodeAPI':
+    def __deepcopy__(self, memo: Any) -> "OpcodeAPI":
         """
         Return a deep copy of the opcode.
         """
         ...
 
 
 class ChainContextAPI(ABC):
     """
     Immutable chain context information that remains constant over the VM execution.
     """
+
     @abstractmethod
     def __init__(self, chain_id: Optional[int]) -> None:
         """
         Initialize the chain context with the given ``chain_id``.
         """
         ...
 
@@ -1489,20 +1545,23 @@
         Return the chain id of the chain context.
         """
         ...
 
 
 class TransactionContextAPI(ABC):
     """
-    Immutable transaction context information that remains constant over the VM execution.
+    Immutable transaction context information that remains constant over the
+    VM execution.
     """
+
     @abstractmethod
     def __init__(self, gas_price: int, origin: Address) -> None:
         """
-        Initialize the transaction context from the given ``gas_price`` and ``origin`` address.
+        Initialize the transaction context from the given ``gas_price`` and
+        ``origin`` address.
         """
         ...
 
     @abstractmethod
     def get_next_log_counter(self) -> int:
         """
         Increment and return the log counter.
@@ -1526,14 +1585,15 @@
         ...
 
 
 class MemoryAPI(ABC):
     """
     A class representing the memory of the :class:`~eth.abc.VirtualMachineAPI`.
     """
+
     @abstractmethod
     def extend(self, start_position: int, size: int) -> None:
         """
         Extend the memory from the given ``start_position`` to the provided ``size``.
         """
         ...
 
@@ -1566,14 +1626,15 @@
         ...
 
 
 class StackAPI(ABC):
     """
     A class representing the stack of the :class:`~eth.abc.VirtualMachineAPI`.
     """
+
     @abstractmethod
     def push_int(self, value: int) -> None:
         """
         Push an integer item onto the stack.
         """
         ...
 
@@ -1666,14 +1727,15 @@
         ...
 
 
 class CodeStreamAPI(ABC):
     """
     A class representing a stream of EVM code.
     """
+
     program_counter: int
 
     @abstractmethod
     def read(self, size: int) -> bytes:
         """
         Read and return the code from the current position of the cursor up to ``size``.
         """
@@ -1704,15 +1766,15 @@
     def peek(self) -> int:
         """
         Return the ordinal value of the byte at the current program counter.
         """
         ...
 
     @abstractmethod
-    def seek(self, program_counter: int) -> ContextManager['CodeStreamAPI']:
+    def seek(self, program_counter: int) -> ContextManager["CodeStreamAPI"]:
         """
         Return a :class:`~typing.ContextManager` with the program counter
         set to ``program_counter``.
         """
         ...
 
     @abstractmethod
@@ -1723,52 +1785,54 @@
         ...
 
 
 class StackManipulationAPI(ABC):
     @abstractmethod
     def stack_pop_ints(self, num_items: int) -> Tuple[int, ...]:
         """
-        Pop the last ``num_items`` from the stack, returning a tuple of their ordinal values.
+        Pop the last ``num_items`` from the stack,
+        returning a tuple of their ordinal values.
         """
         ...
 
     @abstractmethod
     def stack_pop_bytes(self, num_items: int) -> Tuple[bytes, ...]:
         """
         Pop the last ``num_items`` from the stack, returning a tuple of bytes.
         """
         ...
 
     @abstractmethod
     def stack_pop_any(self, num_items: int) -> Tuple[Union[int, bytes], ...]:
         """
-        Pop the last ``num_items`` from the stack, returning a tuple with potentially mixed values
-        of bytes or ordinal values of bytes.
+        Pop the last ``num_items`` from the stack, returning a tuple with potentially
+        mixed values of bytes or ordinal values of bytes.
         """
         ...
 
     @abstractmethod
     def stack_pop1_int(self) -> int:
         """
-        Pop one item from the stack and return the ordinal value of the represented bytes.
+        Pop one item from the stack and return the ordinal value
+        of the represented bytes.
         """
         ...
 
     @abstractmethod
     def stack_pop1_bytes(self) -> bytes:
         """
         Pop one item from the stack and return the value as ``bytes``.
         """
         ...
 
     @abstractmethod
     def stack_pop1_any(self) -> Union[int, bytes]:
         """
-        Pop one item from the stack and return the value either as byte or the ordinal value of
-        a byte.
+        Pop one item from the stack and return the value either as byte or the ordinal
+        value of a byte.
         """
         ...
 
     @abstractmethod
     def stack_push_int(self, value: int) -> None:
         """
         Push ``value`` on the stack which must be a 256 bit integer.
@@ -1781,16 +1845,18 @@
         Push ``value`` on the stack which must be a 32 byte string.
         """
         ...
 
 
 class ExecutionContextAPI(ABC):
     """
-    A class representing context information that remains constant over the execution of a block.
+    A class representing context information that remains constant over the
+    execution of a block.
     """
+
     @property
     @abstractmethod
     def coinbase(self) -> Address:
         """
         Return the coinbase address of the block.
         """
         ...
@@ -1856,49 +1922,73 @@
     def base_fee_per_gas(self) -> Optional[int]:
         """
         Return the base fee per gas of the block
         """
         ...
 
 
-class ComputationAPI(ContextManager['ComputationAPI'], StackManipulationAPI):
+class ComputationAPI(
+    ContextManager["ComputationAPI"],
+    StackManipulationAPI,
+):
     """
-    The base class for all execution computations.
+    The base abstract class for all execution computations.
     """
-    msg: MessageAPI
+
     logger: ExtendedDebugLogger
+
+    state: "StateAPI"
+    msg: MessageAPI
+    transaction_context: TransactionContextAPI
     code: CodeStreamAPI
-    opcodes: Dict[int, OpcodeAPI] = None
-    state: 'StateAPI'
-    return_data: bytes
+    children: List["ComputationAPI"]
+    return_data: bytes = b""
+    accounts_to_delete: Dict[Address, Address]
+
+    _memory: MemoryAPI
+    _stack: StackAPI
+    _gas_meter: GasMeterAPI
+    _error: VMError
+    _output: bytes = b""
+    _log_entries: List[Tuple[int, Address, Tuple[int, ...], bytes]]
+
+    # VM configuration
+    opcodes: Dict[int, OpcodeAPI]
+    _precompiles: Dict[Address, Callable[["ComputationAPI"], "ComputationAPI"]]
 
     @abstractmethod
-    def __init__(self,
-                 state: 'StateAPI',
-                 message: MessageAPI,
-                 transaction_context: TransactionContextAPI) -> None:
+    def __init__(
+        self,
+        state: "StateAPI",
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI,
+    ) -> None:
         """
         Instantiate the computation.
         """
         ...
 
-    #
-    # Convenience
-    #
+    @abstractmethod
+    def _configure_gas_meter(self) -> GasMeterAPI:
+        """
+        Configure the gas meter for the computation at class initialization.
+        """
+        ...
+
+    # -- convenience -- #
     @property
     @abstractmethod
     def is_origin_computation(self) -> bool:
         """
-        Return ``True`` if this computation is the outermost computation at ``depth == 0``.
+        Return ``True`` if this computation is the outermost computation at
+        ``depth == 0``.
         """
         ...
 
-    #
-    # Error handling
-    #
+    # -- error handling -- #
     @property
     @abstractmethod
     def is_success(self) -> bool:
         """
         Return ``True`` if the computation did not result in an error.
         """
         ...
@@ -1959,54 +2049,52 @@
     @abstractmethod
     def should_erase_return_data(self) -> bool:
         """
         Return ``True`` if the return data should be zerod out due to an error.
         """
         ...
 
-    #
-    # Memory Management
-    #
+    # -- memory management -- #
     @abstractmethod
     def extend_memory(self, start_position: int, size: int) -> None:
         """
         Extend the size of the memory to be at minimum ``start_position + size``
         bytes in length.  Raise `eth.exceptions.OutOfGas` if there is not enough
         gas to pay for extending the memory.
         """
         ...
 
     @abstractmethod
     def memory_write(self, start_position: int, size: int, value: bytes) -> None:
         """
-        Write ``value`` to memory at ``start_position``. Require that ``len(value) == size``.
+        Write ``value`` to memory at ``start_position``. Require that
+        ``len(value) == size``.
         """
         ...
 
     @abstractmethod
     def memory_read(self, start_position: int, size: int) -> memoryview:
         """
-        Read and return a view of ``size`` bytes from memory starting at ``start_position``.
+        Read and return a view of ``size`` bytes from memory starting at
+        ``start_position``.
         """
         ...
 
     @abstractmethod
     def memory_read_bytes(self, start_position: int, size: int) -> bytes:
         """
         Read and return ``size`` bytes from memory starting at ``start_position``.
         """
         ...
 
-    #
-    # Gas Consumption
-    #
+    # -- gas consumption -- #
     @abstractmethod
     def get_gas_meter(self) -> GasMeterAPI:
         """
-        Return the :class:`~eth.abc.GasMeterAPI` of the computation.
+        Return the gas meter for the computation.
         """
         ...
 
     @abstractmethod
     def consume_gas(self, amount: int, reason: str) -> None:
         """
         Consume ``amount`` of gas from the remaining gas.
@@ -2025,54 +2113,43 @@
     def refund_gas(self, amount: int) -> None:
         """
         Add ``amount`` of gas to the pool of gas marked to be refunded.
         """
         ...
 
     @abstractmethod
-    def get_gas_refund(self) -> int:
-        """
-        Return the number of refunded gas.
-        """
-        ...
-
-    @abstractmethod
     def get_gas_used(self) -> int:
         """
         Return the number of used gas.
         """
         ...
 
     @abstractmethod
     def get_gas_remaining(self) -> int:
         """
         Return the number of remaining gas.
         """
         ...
 
-    #
-    # Stack management
-    #
+    # -- stack management -- #
     @abstractmethod
     def stack_swap(self, position: int) -> None:
         """
         Swap the item on the top of the stack with the item at ``position``.
         """
         ...
 
     @abstractmethod
     def stack_dup(self, position: int) -> None:
         """
         Duplicate the stack item at ``position`` and pushes it onto the stack.
         """
         ...
 
-    #
-    # Computation result
-    #
+    # -- computation result -- #
     @property
     @abstractmethod
     def output(self) -> bytes:
         """
         Get the return value of the computation.
         """
         ...
@@ -2083,180 +2160,199 @@
         Set the return value of the computation.
         """
         # See: https://github.com/python/mypy/issues/4165
         # Since we can't also decorate this with abstract method we want to be
         # sure that the setter doesn't actually get used as a noop.
         raise NotImplementedError
 
-    #
-    # Runtime operations
-    #
+    # -- opcode API -- #
+    @property
+    @abstractmethod
+    def precompiles(self) -> Dict[Address, Callable[["ComputationAPI"], None]]:
+        """
+        Return a dictionary where the keys are the addresses of precompiles and the
+        values are the precompile functions.
+        """
+        ...
+
+    @classmethod
+    @abstractmethod
+    def get_precompiles(cls) -> Dict[Address, Callable[["ComputationAPI"], None]]:
+        """
+        Return a dictionary where the keys are the addresses of precompiles and the
+        values are the precompile functions.
+        """
+        ...
+
+    @abstractmethod
+    def get_opcode_fn(self, opcode: int) -> OpcodeAPI:
+        """
+        Return the function for the given ``opcode``.
+        """
+        ...
+
+    # -- runtime operations -- #
     @abstractmethod
-    def prepare_child_message(self,
-                              gas: int,
-                              to: Address,
-                              value: int,
-                              data: BytesOrView,
-                              code: bytes,
-                              **kwargs: Any) -> MessageAPI:
+    def prepare_child_message(
+        self,
+        gas: int,
+        to: Address,
+        value: int,
+        data: BytesOrView,
+        code: bytes,
+        **kwargs: Any,
+    ) -> MessageAPI:
         """
         Helper method for creating a child computation.
         """
         ...
 
     @abstractmethod
-    def apply_child_computation(self, child_msg: MessageAPI) -> 'ComputationAPI':
+    def apply_child_computation(
+        self,
+        child_msg: MessageAPI,
+    ) -> "ComputationAPI":
         """
         Apply the vm message ``child_msg`` as a child computation.
         """
         ...
 
     @abstractmethod
-    def generate_child_computation(self, child_msg: MessageAPI) -> 'ComputationAPI':
+    def generate_child_computation(
+        self,
+        child_msg: MessageAPI,
+    ) -> "ComputationAPI":
         """
         Generate a child computation from the given ``child_msg``.
         """
         ...
 
     @abstractmethod
-    def add_child_computation(self, child_computation: 'ComputationAPI') -> None:
+    def add_child_computation(
+        self,
+        child_computation: "ComputationAPI",
+    ) -> None:
         """
         Add the given ``child_computation``.
         """
         ...
 
-    #
-    # Account management
-    #
+    # -- gas consumption -- #
+    @abstractmethod
+    def get_gas_refund(self) -> int:
+        """
+        Return the number of refunded gas.
+        """
+        ...
+
+    # -- account management -- #
     @abstractmethod
     def register_account_for_deletion(self, beneficiary: Address) -> None:
         """
         Register the address of ``beneficiary`` for deletion.
         """
         ...
 
     @abstractmethod
     def get_accounts_for_deletion(self) -> Tuple[Tuple[Address, Address], ...]:
         """
         Return a tuple of addresses that are registered for deletion.
         """
         ...
 
-    #
-    # EVM logging
-    #
+    # -- EVM logging -- #
     @abstractmethod
-    def add_log_entry(self, account: Address, topics: Tuple[int, ...], data: bytes) -> None:
+    def add_log_entry(
+        self, account: Address, topics: Tuple[int, ...], data: bytes
+    ) -> None:
         """
         Add a log entry.
         """
         ...
 
     @abstractmethod
-    def get_raw_log_entries(self) -> Tuple[Tuple[int, bytes, Tuple[int, ...], bytes], ...]:
+    def get_raw_log_entries(
+        self,
+    ) -> Tuple[Tuple[int, bytes, Tuple[int, ...], bytes], ...]:
         """
         Return a tuple of raw log entries.
         """
         ...
 
     @abstractmethod
     def get_log_entries(self) -> Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...]:
         """
         Return the log entries for this computation and its children.
 
-        They are sorted in the same order they were emitted during the transaction processing, and
-        include the sequential counter as the first element of the tuple representing every entry.
+        They are sorted in the same order they were emitted during the transaction
+        processing, and include the sequential counter as the first element of the
+        tuple representing every entry.
         """
         ...
 
-    #
-    # State Transition
-    #
+    # -- state transition -- #
     @classmethod
     @abstractmethod
     def apply_message(
-            cls,
-            state: 'StateAPI',
-            message: MessageAPI,
-            transaction_context: TransactionContextAPI) -> 'ComputationAPI':
+        cls,
+        state: "StateAPI",
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI,
+    ) -> "ComputationAPI":
         """
         Execute a VM message. This is where the VM-specific call logic exists.
         """
         ...
 
     @classmethod
     @abstractmethod
     def apply_create_message(
-            cls,
-            state: 'StateAPI',
-            message: MessageAPI,
-            transaction_context: TransactionContextAPI) -> 'ComputationAPI':
+        cls,
+        state: "StateAPI",
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI,
+    ) -> "ComputationAPI":
         """
         Execute a VM message to create a new contract. This is where the VM-specific
         create logic exists.
         """
         ...
 
     @classmethod
     @abstractmethod
-    def apply_computation(cls,
-                          state: 'StateAPI',
-                          message: MessageAPI,
-                          transaction_context: TransactionContextAPI) -> 'ComputationAPI':
+    def apply_computation(
+        cls,
+        state: "StateAPI",
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI,
+    ) -> "ComputationAPI":
         """
         Execute the logic within the message: Either run the precompile, or
         step through each opcode.  Generally, the only VM-specific logic is for
         each opcode as it executes.
 
-        This should rarely be called directly, because it will skip over other important
-        VM-specific logic that happens before or after the execution.
+        This should rarely be called directly, because it will skip over other
+        important VM-specific logic that happens before or after the execution.
 
         Instead, prefer :meth:`~apply_message` or :meth:`~apply_create_message`.
         """
         ...
 
-    #
-    # Opcode API
-    #
-    @property
-    @abstractmethod
-    def precompiles(self) -> Dict[Address, Callable[['ComputationAPI'], None]]:
-        """
-        Return a dictionary where the keys are the addresses of precompiles and the values are
-        the precompile functions.
-        """
-        ...
-
-    @classmethod
-    @abstractmethod
-    def get_precompiles(cls) -> Dict[Address, Callable[['ComputationAPI'], None]]:
-        """
-        Return a dictionary where the keys are the addresses of precompiles and the values are
-        the precompile functions.
-        """
-        ...
-
-    @abstractmethod
-    def get_opcode_fn(self, opcode: int) -> OpcodeAPI:
-        """
-        Return the function for the given ``opcode``.
-        """
-        ...
-
 
 class AccountStorageDatabaseAPI(ABC):
     """
     Storage cache and write batch for a single account. Changes are not
     merklized until :meth:`make_storage_root` is called.
     """
+
     @abstractmethod
     def get(self, slot: int, from_journal: bool = True) -> int:
         """
-        Return the value at ``slot``. Lookups take the journal into consideration unless
-        ``from_journal`` is explicitly set to ``False``.
+        Return the value at ``slot``. Lookups take the journal into consideration
+        unless ``from_journal`` is explicitly set to ``False``.
         """
         ...
 
     @abstractmethod
     def set(self, slot: int, value: int) -> None:
         """
         Write ``value`` into ``slot``.
@@ -2339,26 +2435,30 @@
         ...
 
 
 class AccountAPI(ABC):
     """
     A class representing an Ethereum account.
     """
+
     nonce: int
     balance: int
     storage_root: Hash32
     code_hash: Hash32
 
 
 class AccountDatabaseAPI(ABC):
     """
     A class representing a database for accounts.
     """
+
     @abstractmethod
-    def __init__(self, db: AtomicDatabaseAPI, state_root: Hash32 = BLANK_ROOT_HASH) -> None:
+    def __init__(
+        self, db: AtomicDatabaseAPI, state_root: Hash32 = BLANK_ROOT_HASH
+    ) -> None:
         """
         Initialize the account database.
         """
         ...
 
     @property
     @abstractmethod
@@ -2385,15 +2485,17 @@
         """
         ...
 
     #
     # Storage
     #
     @abstractmethod
-    def get_storage(self, address: Address, slot: int, from_journal: bool = True) -> int:
+    def get_storage(
+        self, address: Address, slot: int, from_journal: bool = True
+    ) -> int:
         """
         Return the value stored at ``slot`` for the given ``address``. Take the journal
         into consideration unless ``from_journal`` is set to ``False``.
         """
         ...
 
     @abstractmethod
@@ -2597,21 +2699,22 @@
         ...
 
     @abstractmethod
     def make_state_root(self) -> Hash32:
         """
         Generate the state root with all the current changes in AccountDB
 
-        Current changes include every pending change to storage, as well as all account changes.
-        After generating all the required tries, the final account state root is returned.
-
-        This is an expensive operation, so should be called as little as possible. For example,
-        pre-Byzantium, this is called after every transaction, because we need the state root
-        in each receipt. Byzantium+, we only need state roots at the end of the block,
-        so we *only* call it right before persistance.
+        Current changes include every pending change to storage, as well as all account
+        changes. After generating all the required tries, the final account state root
+        is returned.
+
+        This is an expensive operation, so should be called as little as possible.
+        For example, pre-Byzantium, this is called after every transaction, because we
+        need the state root in each receipt. Byzantium+, we only need state roots at
+        the end of the block, so we *only* call it right before persistance.
 
         :return: the new state root
         """
         ...
 
     @abstractmethod
     def persist(self) -> MetaWitnessAPI:
@@ -2625,23 +2728,24 @@
         ...
 
 
 class TransactionExecutorAPI(ABC):
     """
     A class providing APIs to execute transactions on VM state.
     """
+
     @abstractmethod
-    def __init__(self, vm_state: 'StateAPI') -> None:
+    def __init__(self, vm_state: "StateAPI") -> None:
         """
         Initialize the executor from the given ``vm_state``.
         """
         ...
 
     @abstractmethod
-    def __call__(self, transaction: SignedTransactionAPI) -> 'ComputationAPI':
+    def __call__(self, transaction: SignedTransactionAPI) -> "ComputationAPI":
         """
         Execute the ``transaction`` and return a :class:`eth.abc.ComputationAPI`.
         """
         ...
 
     @abstractmethod
     def validate_transaction(self, transaction: SignedTransactionAPI) -> None:
@@ -2655,43 +2759,42 @@
     def build_evm_message(self, transaction: SignedTransactionAPI) -> MessageAPI:
         """
         Build and return a :class:`~eth.abc.MessageAPI` from the given ``transaction``.
         """
         ...
 
     @abstractmethod
-    def build_computation(self,
-                          message: MessageAPI,
-                          transaction: SignedTransactionAPI) -> 'ComputationAPI':
+    def build_computation(
+        self, message: MessageAPI, transaction: SignedTransactionAPI
+    ) -> "ComputationAPI":
         """
         Apply the ``message`` to the VM and use the given ``transaction`` to
         retrieve the context from.
         """
 
         ...
 
     @abstractmethod
-    def finalize_computation(self,
-                             transaction: SignedTransactionAPI,
-                             computation: 'ComputationAPI') -> 'ComputationAPI':
+    def finalize_computation(
+        self, transaction: SignedTransactionAPI, computation: "ComputationAPI"
+    ) -> "ComputationAPI":
         """
         Finalize the ``transaction``.
         """
         ...
 
 
 class ConfigurableAPI(ABC):
     """
     A class providing inline subclassing.
     """
+
     @classmethod
     @abstractmethod
-    def configure(cls: Type[T],
-                  __name__: str = None,
-                  **overrides: Any) -> Type[T]:
+    def configure(cls: Type[T], __name__: str = None, **overrides: Any) -> Type[T]:
         ...
 
 
 class StateAPI(ConfigurableAPI):
     """
     The base class that encapsulates all of the various moving parts related to
     the state of the VM during execution.
@@ -2703,30 +2806,32 @@
         Each :class:`~eth.abc.StateAPI` class must be configured with:
 
         - ``computation_class``: The :class:`~eth.abc.ComputationAPI` class for
           vm execution.
         - ``transaction_context_class``: The :class:`~eth.abc.TransactionContextAPI`
           class for vm execution.
     """
+
     #
     # Set from __init__
     #
     execution_context: ExecutionContextAPI
 
     computation_class: Type[ComputationAPI]
     transaction_context_class: Type[TransactionContextAPI]
     account_db_class: Type[AccountDatabaseAPI]
     transaction_executor_class: Type[TransactionExecutorAPI] = None
 
     @abstractmethod
     def __init__(
-            self,
-            db: AtomicDatabaseAPI,
-            execution_context: ExecutionContextAPI,
-            state_root: bytes) -> None:
+        self,
+        db: AtomicDatabaseAPI,
+        execution_context: ExecutionContextAPI,
+        state_root: bytes,
+    ) -> None:
         """
         Initialize the state.
         """
         ...
 
     @property
     @abstractmethod
@@ -2843,15 +2948,17 @@
     def make_state_root(self) -> Hash32:
         """
         Create and return the state root.
         """
         ...
 
     @abstractmethod
-    def get_storage(self, address: Address, slot: int, from_journal: bool = True) -> int:
+    def get_storage(
+        self, address: Address, slot: int, from_journal: bool = True
+    ) -> int:
         """
         Return the storage at ``slot`` for ``address``.
         """
         ...
 
     @abstractmethod
     def set_storage(self, address: Address, slot: int, value: int) -> None:
@@ -3065,39 +3172,42 @@
         """
         ...
 
     #
     # Computation
     #
     @abstractmethod
-    def get_computation(self,
-                        message: MessageAPI,
-                        transaction_context: TransactionContextAPI) -> ComputationAPI:
+    def get_computation(
+        self, message: MessageAPI, transaction_context: TransactionContextAPI
+    ) -> ComputationAPI:
         """
         Return a computation instance for the given `message` and `transaction_context`
         """
         ...
 
     #
     # Transaction context
     #
     @classmethod
     @abstractmethod
     def get_transaction_context_class(cls) -> Type[TransactionContextAPI]:
         """
-        Return the :class:`~eth.vm.transaction_context.BaseTransactionContext` class that the
-        state class uses.
+        Return the :class:`~eth.vm.transaction_context.BaseTransactionContext` class
+        that the state class uses.
         """
         ...
 
     #
     # Execution
     #
     @abstractmethod
-    def apply_transaction(self, transaction: SignedTransactionAPI) -> ComputationAPI:
+    def apply_transaction(
+        self,
+        transaction: SignedTransactionAPI,
+    ) -> ComputationAPI:
         """
         Apply transaction to the vm state
 
         :param transaction: the transaction to apply
         :return: the computation
         """
         ...
@@ -3106,39 +3216,42 @@
     def get_transaction_executor(self) -> TransactionExecutorAPI:
         """
         Return the transaction executor.
         """
         ...
 
     @abstractmethod
-    def costless_execute_transaction(self,
-                                     transaction: SignedTransactionAPI) -> ComputationAPI:
+    def costless_execute_transaction(
+        self,
+        transaction: SignedTransactionAPI,
+    ) -> ComputationAPI:
         """
         Execute the given ``transaction`` with a gas price of ``0``.
         """
         ...
 
     @abstractmethod
     def override_transaction_context(self, gas_price: int) -> ContextManager[None]:
         """
-        Return a :class:`~typing.ContextManager` that overwrites the current transaction context,
-        applying the given ``gas_price``.
+        Return a :class:`~typing.ContextManager` that overwrites the current
+        transaction context, applying the given ``gas_price``.
         """
         ...
 
     @abstractmethod
     def validate_transaction(self, transaction: SignedTransactionAPI) -> None:
         """
         Validate the given ``transaction``.
         """
         ...
 
     @abstractmethod
-    def get_transaction_context(self,
-                                transaction: SignedTransactionAPI) -> TransactionContextAPI:
+    def get_transaction_context(
+        self, transaction: SignedTransactionAPI
+    ) -> TransactionContextAPI:
         """
         Return the :class:`~eth.abc.TransactionContextAPI` for the given ``transaction``
         """
         ...
 
     #
     # Withdrawals
@@ -3162,16 +3275,17 @@
         Initialize the context with a database.
         """
         ...
 
 
 class ConsensusAPI(ABC):
     """
-    A class encapsulating the consensus scheme to allow chains to run under different kind of
-    EVM-compatible consensus mechanisms such as the Clique Proof of Authority scheme.
+    A class encapsulating the consensus scheme to allow chains to run
+    under different kind of EVM-compatible consensus mechanisms such
+    as the Clique Proof of Authority scheme.
     """
 
     @abstractmethod
     def __init__(self, context: ConsensusContextAPI) -> None:
         """
         Initialize the consensus api.
         """
@@ -3181,20 +3295,20 @@
     def validate_seal(self, header: BlockHeaderAPI) -> None:
         """
         Validate the seal on the given header, even if its parent is missing.
         """
         ...
 
     @abstractmethod
-    def validate_seal_extension(self,
-                                header: BlockHeaderAPI,
-                                parents: Iterable[BlockHeaderAPI]) -> None:
+    def validate_seal_extension(
+        self, header: BlockHeaderAPI, parents: Iterable[BlockHeaderAPI]
+    ) -> None:
         """
-        Validate the seal on the given header when all parents must be present. Parent headers
-        that are not yet in the database must be passed as ``parents``.
+        Validate the seal on the given header when all parents must be present.
+        Parent headers that are not yet in the database must be passed as ``parents``.
         """
         ...
 
     @classmethod
     @abstractmethod
     def get_fee_recipient(cls, header: BlockHeaderAPI) -> Address:
         """
@@ -3208,30 +3322,35 @@
     The :class:`~eth.abc.VirtualMachineAPI` class represents the Chain rules for a
     specific protocol definition such as the Frontier or Homestead network.
 
       .. note::
 
         Each :class:`~eth.abc.VirtualMachineAPI` class must be configured with:
 
-        - ``block_class``: The :class:`~eth.abc.BlockAPI` class for blocks in this VM ruleset.
-        - ``_state_class``: The :class:`~eth.abc.StateAPI` class used by this VM for execution.
+        - ``block_class``: The :class:`~eth.abc.BlockAPI` class for blocks in this
+            VM ruleset.
+        - ``_state_class``: The :class:`~eth.abc.StateAPI` class used by this
+            VM for execution.
+
     """
 
     fork: str
     chaindb: ChainDatabaseAPI
     extra_data_max_bytes: ClassVar[int]
     consensus_class: Type[ConsensusAPI]
     consensus_context: ConsensusContextAPI
 
     @abstractmethod
-    def __init__(self,
-                 header: BlockHeaderAPI,
-                 chaindb: ChainDatabaseAPI,
-                 chain_context: ChainContextAPI,
-                 consensus_context: ConsensusContextAPI) -> None:
+    def __init__(
+        self,
+        header: BlockHeaderAPI,
+        chaindb: ChainDatabaseAPI,
+        chain_context: ChainContextAPI,
+        consensus_context: ConsensusContextAPI,
+    ) -> None:
         """
         Initialize the virtual machine.
         """
         ...
 
     @property
     @abstractmethod
@@ -3239,25 +3358,27 @@
         """
         Return the current state.
         """
         ...
 
     @classmethod
     @abstractmethod
-    def build_state(cls,
-                    db: AtomicDatabaseAPI,
-                    header: BlockHeaderAPI,
-                    chain_context: ChainContextAPI,
-                    previous_hashes: Iterable[Hash32] = (),
-                    ) -> StateAPI:
+    def build_state(
+        cls,
+        db: AtomicDatabaseAPI,
+        header: BlockHeaderAPI,
+        chain_context: ChainContextAPI,
+        previous_hashes: Iterable[Hash32] = (),
+    ) -> StateAPI:
         """
         You probably want `VM().state` instead of this.
 
-        Occasionally, you want to build custom state against a particular header and DB,
-        even if you don't have the VM initialized. This is a convenience method to do that.
+        Occasionally, you want to build custom state against a particular
+        header and DB, even if you don't have the VM initialized.
+        This is a convenience method to do that.
         """
         ...
 
     @abstractmethod
     def get_header(self) -> BlockHeaderAPI:
         """
         Return the current header.
@@ -3272,67 +3393,73 @@
         ...
 
     #
     # Hooks
     #
 
     def transaction_applied_hook(
-            self,
-            transaction_index: int,
-            transactions: Sequence[SignedTransactionAPI],
-            base_header: BlockHeaderAPI,
-            partial_header: BlockHeaderAPI,
-            computation: ComputationAPI,
-            receipt: ReceiptAPI) -> None:
+        self,
+        transaction_index: int,
+        transactions: Sequence[SignedTransactionAPI],
+        base_header: BlockHeaderAPI,
+        partial_header: BlockHeaderAPI,
+        computation: ComputationAPI,
+        receipt: ReceiptAPI,
+    ) -> None:
         """
         A hook for a subclass to use as a way to note that a transaction was applied.
         This only gets triggered as part of `apply_all_transactions`, which is called
         by `block_import`.
         """
         pass
 
     #
     # Execution
     #
     @abstractmethod
-    def apply_transaction(self,
-                          header: BlockHeaderAPI,
-                          transaction: SignedTransactionAPI
-                          ) -> Tuple[ReceiptAPI, ComputationAPI]:
+    def apply_transaction(
+        self, header: BlockHeaderAPI, transaction: SignedTransactionAPI
+    ) -> Tuple[ReceiptAPI, ComputationAPI]:
         """
         Apply the transaction to the current block. This is a wrapper around
-        :func:`~eth.vm.state.State.apply_transaction` with some extra orchestration logic.
+        :func:`~eth.vm.state.State.apply_transaction` with some extra
+        orchestration logic.
 
         :param header: header of the block before application
         :param transaction: to apply
         """
         ...
 
     @staticmethod
     @abstractmethod
-    def create_execution_context(header: BlockHeaderAPI,
-                                 prev_hashes: Iterable[Hash32],
-                                 chain_context: ChainContextAPI) -> ExecutionContextAPI:
-        """
-        Create and return the :class:`~eth.abc.ExecutionContextAPI`` for the given ``header``,
-        iterable of block hashes that precede the block and the ``chain_context``.
+    def create_execution_context(
+        header: BlockHeaderAPI,
+        prev_hashes: Iterable[Hash32],
+        chain_context: ChainContextAPI,
+    ) -> ExecutionContextAPI:
+        """
+        Create and return the :class:`~eth.abc.ExecutionContextAPI`` for the given
+        ``header``, iterable of block hashes that precede the block and
+        the ``chain_context``.
         """
         ...
 
     @abstractmethod
-    def execute_bytecode(self,
-                         origin: Address,
-                         gas_price: int,
-                         gas: int,
-                         to: Address,
-                         sender: Address,
-                         value: int,
-                         data: bytes,
-                         code: bytes,
-                         code_address: Address = None) -> ComputationAPI:
+    def execute_bytecode(
+        self,
+        origin: Address,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        sender: Address,
+        value: int,
+        data: bytes,
+        code: bytes,
+        code_address: Address = None,
+    ) -> ComputationAPI:
         """
         Execute raw bytecode in the context of the current state of
         the virtual machine. Note that this skips over some of the logic
         that would normally happen during a call. Watch out for:
 
             - value (ether) is *not* transferred
             - state is *not* rolled back in case of an error
@@ -3343,43 +3470,45 @@
         between :meth:`ComputationAPI.apply_computation` and
         :meth:`ComputationAPI.apply_message`. (depending on the VM fork)
         """
         ...
 
     @abstractmethod
     def apply_all_transactions(
-        self,
-        transactions: Sequence[SignedTransactionAPI],
-        base_header: BlockHeaderAPI
+        self, transactions: Sequence[SignedTransactionAPI], base_header: BlockHeaderAPI
     ) -> Tuple[BlockHeaderAPI, Tuple[ReceiptAPI, ...], Tuple[ComputationAPI, ...]]:
         """
         Determine the results of applying all transactions to the base header.
         This does *not* update the current block or header of the VM.
 
         :param transactions: an iterable of all transactions to apply
         :param base_header: the starting header to apply transactions to
-        :return: the final header, the receipts of each transaction, and the computations
+        :return: the final header, the receipts of each transaction, and the
+            computations
+
         """
         ...
 
     def apply_all_withdrawals(self, withdrawals: Sequence[WithdrawalAPI]) -> None:
         """
         Updates the state by applying all withdrawals.
         This does *not* update the current block or header of the VM.
 
         :param withdrawals: an iterable of all withdrawals to apply
         """
         ...
 
     @abstractmethod
-    def make_receipt(self,
-                     base_header: BlockHeaderAPI,
-                     transaction: SignedTransactionAPI,
-                     computation: ComputationAPI,
-                     state: StateAPI) -> ReceiptAPI:
+    def make_receipt(
+        self,
+        base_header: BlockHeaderAPI,
+        transaction: SignedTransactionAPI,
+        computation: ComputationAPI,
+        state: StateAPI,
+    ) -> ReceiptAPI:
         """
         Generate the receipt resulting from applying the transaction.
 
         :param base_header: the header of the block before the transaction was applied.
         :param transaction: the transaction used to generate the receipt
         :param computation: the result of running the transaction computation
         :param state: the resulting state, after executing the computation
@@ -3395,15 +3524,17 @@
     def import_block(self, block: BlockAPI) -> BlockAndMetaWitness:
         """
         Import the given block to the chain.
         """
         ...
 
     @abstractmethod
-    def mine_block(self, block: BlockAPI, *args: Any, **kwargs: Any) -> BlockAndMetaWitness:
+    def mine_block(
+        self, block: BlockAPI, *args: Any, **kwargs: Any
+    ) -> BlockAndMetaWitness:
         """
         Mine the given block. Proxies to self.pack_block method.
         """
         ...
 
     @abstractmethod
     def set_block_transactions_and_withdrawals(
@@ -3448,21 +3579,22 @@
         """
         ...
 
     #
     # Headers
     #
     @abstractmethod
-    def add_receipt_to_header(self,
-                              old_header: BlockHeaderAPI,
-                              receipt: ReceiptAPI) -> BlockHeaderAPI:
-        """
-        Apply the receipt to the old header, and return the resulting header. This may have
-        storage-related side-effects. For example, pre-Byzantium, the state root hash
-        is included in the receipt, and so must be stored into the database.
+    def add_receipt_to_header(
+        self, old_header: BlockHeaderAPI, receipt: ReceiptAPI
+    ) -> BlockHeaderAPI:
+        """
+        Apply the receipt to the old header, and return the resulting header.
+        This may have storage-related side-effects. For example, pre-Byzantium,
+        the state root hash is included in the receipt, and so must be stored
+        into the database.
         """
         ...
 
     @classmethod
     @abstractmethod
     def compute_difficulty(cls, parent_header: BlockHeaderAPI, timestamp: int) -> int:
         """
@@ -3480,31 +3612,31 @@
         used to set fields like the gas limit or timestamp to value different
         than their computed defaults.
         """
         ...
 
     @classmethod
     @abstractmethod
-    def create_header_from_parent(cls,
-                                  parent_header: BlockHeaderAPI,
-                                  **header_params: Any) -> BlockHeaderAPI:
+    def create_header_from_parent(
+        cls, parent_header: BlockHeaderAPI, **header_params: Any
+    ) -> BlockHeaderAPI:
         """
         Creates and initializes a new block header from the provided
         `parent_header`.
         """
         ...
 
     #
     # Blocks
     #
     @classmethod
     @abstractmethod
-    def generate_block_from_parent_header_and_coinbase(cls,
-                                                       parent_header: BlockHeaderAPI,
-                                                       coinbase: Address) -> BlockAPI:
+    def generate_block_from_parent_header_and_coinbase(
+        cls, parent_header: BlockHeaderAPI, coinbase: Address
+    ) -> BlockAPI:
         """
         Generate block from parent header and coinbase.
         """
         ...
 
     @classmethod
     @abstractmethod
@@ -3546,17 +3678,17 @@
           .. note::
             This is an abstract method that must be implemented in subclasses
         """
         ...
 
     @classmethod
     @abstractmethod
-    def get_prev_hashes(cls,
-                        last_block_hash: Hash32,
-                        chaindb: ChainDatabaseAPI) -> Optional[Iterable[Hash32]]:
+    def get_prev_hashes(
+        cls, last_block_hash: Hash32, chaindb: ChainDatabaseAPI
+    ) -> Optional[Iterable[Hash32]]:
         """
         Return an iterable of block hashes that precede the block with the given
         ``last_block_hash``.
         """
         ...
 
     @property
@@ -3586,22 +3718,24 @@
         """
         Proxy for instantiating a signed transaction for this VM.
         """
         ...
 
     @classmethod
     @abstractmethod
-    def create_unsigned_transaction(cls,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> UnsignedTransactionAPI:
+    def create_unsigned_transaction(
+        cls,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+    ) -> UnsignedTransactionAPI:
         """
         Proxy for instantiating an unsigned transaction for this VM.
         """
         ...
 
     @classmethod
     @abstractmethod
@@ -3635,26 +3769,26 @@
         """
         Validate the the given block.
         """
         ...
 
     @classmethod
     @abstractmethod
-    def validate_header(self,
-                        header: BlockHeaderAPI,
-                        parent_header: BlockHeaderAPI) -> None:
+    def validate_header(
+        self, header: BlockHeaderAPI, parent_header: BlockHeaderAPI
+    ) -> None:
         """
         :raise eth.exceptions.ValidationError: if the header is not valid
         """
         ...
 
     @abstractmethod
-    def validate_transaction_against_header(self,
-                                            base_header: BlockHeaderAPI,
-                                            transaction: SignedTransactionAPI) -> None:
+    def validate_transaction_against_header(
+        self, base_header: BlockHeaderAPI, transaction: SignedTransactionAPI
+    ) -> None:
         """
         Validate that the given transaction is valid to apply to the given header.
 
         :param base_header: header before applying the transaction
         :param transaction: the transaction to validate
 
         :raises: ValidationError if the transaction is not valid to apply
@@ -3665,30 +3799,28 @@
     def validate_seal(self, header: BlockHeaderAPI) -> None:
         """
         Validate the seal on the given header.
         """
         ...
 
     @abstractmethod
-    def validate_seal_extension(self,
-                                header: BlockHeaderAPI,
-                                parents: Iterable[BlockHeaderAPI]) -> None:
+    def validate_seal_extension(
+        self, header: BlockHeaderAPI, parents: Iterable[BlockHeaderAPI]
+    ) -> None:
         """
-        Validate the seal on the given header when all parents must be present. Parent headers
-        that are not yet in the database must be passed as ``parents``.
+        Validate the seal on the given header when all parents must be present. Parent
+        headers that are not yet in the database must be passed as ``parents``.
         """
         ...
 
     @classmethod
     @abstractmethod
-    def validate_uncle(cls,
-                       block: BlockAPI,
-                       uncle: BlockHeaderAPI,
-                       uncle_parent: BlockHeaderAPI
-                       ) -> None:
+    def validate_uncle(
+        cls, block: BlockAPI, uncle: BlockHeaderAPI, uncle_parent: BlockHeaderAPI
+    ) -> None:
         """
         Validate the given uncle in the context of the given block.
         """
         ...
 
     #
     # State
@@ -3700,57 +3832,61 @@
         Return the class that this VM uses for states.
         """
         ...
 
     @abstractmethod
     def in_costless_state(self) -> ContextManager[StateAPI]:
         """
-        Return a :class:`~typing.ContextManager` with the current state wrapped in a temporary
-        block. In this state, the ability to pay gas costs is ignored.
+        Return a :class:`~typing.ContextManager` with the current state wrapped in a
+        temporary block. In this state, the ability to pay gas costs is ignored.
         """
         ...
 
 
 class VirtualMachineModifierAPI(ABC):
     """
-    Amend a set of VMs for a chain. This allows modifying a chain for different consensus schemes.
+    Amend a set of VMs for a chain. This allows modifying a chain for different
+    consensus schemes.
     """
 
     @abstractmethod
     def amend_vm_configuration(self, vm_config: VMConfiguration) -> VMConfiguration:
         """
-        Amend the ``vm_config`` by configuring the VM classes, and hence returning a modified
-        set of VM classes.
+        Amend the ``vm_config`` by configuring the VM classes, and hence returning
+        a modified set of VM classes.
         """
         ...
 
 
 class HeaderChainAPI(ABC):
     """
     Like :class:`eth.abc.ChainAPI` but does only support headers, not entire blocks.
     """
+
     header: BlockHeaderAPI
     chain_id: int
     vm_configuration: Tuple[Tuple[BlockNumber, Type[VirtualMachineAPI]], ...]
 
     @abstractmethod
-    def __init__(self, base_db: AtomicDatabaseAPI, header: BlockHeaderAPI = None) -> None:
+    def __init__(
+        self, base_db: AtomicDatabaseAPI, header: BlockHeaderAPI = None
+    ) -> None:
         """
         Initialize the header chain.
         """
         ...
 
     #
     # Chain Initialization API
     #
     @classmethod
     @abstractmethod
-    def from_genesis_header(cls,
-                            base_db: AtomicDatabaseAPI,
-                            genesis_header: BlockHeaderAPI) -> 'HeaderChainAPI':
+    def from_genesis_header(
+        cls, base_db: AtomicDatabaseAPI, genesis_header: BlockHeaderAPI
+    ) -> "HeaderChainAPI":
         """
         Initialize the chain from the genesis header.
         """
         ...
 
     #
     # Helpers
@@ -3768,15 +3904,17 @@
     #
     def get_canonical_block_hash(self, block_number: BlockNumber) -> Hash32:
         """
         Direct passthrough to `headerdb`
         """
 
     @abstractmethod
-    def get_canonical_block_header_by_number(self, block_number: BlockNumber) -> BlockHeaderAPI:
+    def get_canonical_block_header_by_number(
+        self, block_number: BlockNumber
+    ) -> BlockHeaderAPI:
         """
         Direct passthrough to `headerdb`
         """
         ...
 
     @abstractmethod
     def get_canonical_head(self) -> BlockHeaderAPI:
@@ -3799,17 +3937,18 @@
     def header_exists(self, block_hash: Hash32) -> bool:
         """
         Direct passthrough to `headerdb`
         """
         ...
 
     @abstractmethod
-    def import_header(self,
-                      header: BlockHeaderAPI,
-                      ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
+    def import_header(
+        self,
+        header: BlockHeaderAPI,
+    ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
         """
         Direct passthrough to `headerdb`
 
         Also updates the local `header` property to be the latest canonical head.
 
         Returns an iterable of headers representing the headers that are newly
         part of the canonical chain.
@@ -3828,14 +3967,15 @@
 class ChainAPI(ConfigurableAPI):
     """
     A Chain is a combination of one or more VM classes. Each VM is associated
     with a range of blocks. The Chain class acts as a wrapper around these other
     VM classes, delegating operations to the appropriate VM depending on the
     current block number.
     """
+
     vm_configuration: Tuple[Tuple[BlockNumber, Type[VirtualMachineAPI]], ...]
     chain_id: int
     chaindb: ChainDatabaseAPI
     consensus_context_class: Type[ConsensusContextAPI]
 
     #
     # Helpers
@@ -3849,28 +3989,30 @@
         ...
 
     #
     # Chain API
     #
     @classmethod
     @abstractmethod
-    def from_genesis(cls,
-                     base_db: AtomicDatabaseAPI,
-                     genesis_params: Dict[str, HeaderParams],
-                     genesis_state: AccountState = None) -> 'ChainAPI':
+    def from_genesis(
+        cls,
+        base_db: AtomicDatabaseAPI,
+        genesis_params: Dict[str, HeaderParams],
+        genesis_state: AccountState = None,
+    ) -> "ChainAPI":
         """
         Initialize the Chain from a genesis state.
         """
         ...
 
     @classmethod
     @abstractmethod
-    def from_genesis_header(cls,
-                            base_db: AtomicDatabaseAPI,
-                            genesis_header: BlockHeaderAPI) -> 'ChainAPI':
+    def from_genesis_header(
+        cls, base_db: AtomicDatabaseAPI, genesis_header: BlockHeaderAPI
+    ) -> "ChainAPI":
         """
         Initialize the chain from the genesis header.
         """
         ...
 
     #
     # VM API
@@ -3887,27 +4029,29 @@
     def get_vm(self, header: BlockHeaderAPI = None) -> VirtualMachineAPI:
         """
         Return the VM instance for the given ``header``.
         """
         ...
 
     @classmethod
-    def get_vm_class_for_block_number(cls, block_number: BlockNumber) -> Type[VirtualMachineAPI]:
+    def get_vm_class_for_block_number(
+        cls, block_number: BlockNumber
+    ) -> Type[VirtualMachineAPI]:
         """
         Return the VM class for the given ``block_number``
         """
         ...
 
     #
     # Header API
     #
     @abstractmethod
-    def create_header_from_parent(self,
-                                  parent_header: BlockHeaderAPI,
-                                  **header_params: HeaderParams) -> BlockHeaderAPI:
+    def create_header_from_parent(
+        self, parent_header: BlockHeaderAPI, **header_params: HeaderParams
+    ) -> BlockHeaderAPI:
         """
         Passthrough helper to the VM class of the block descending from the
         given header.
         """
         ...
 
     @abstractmethod
@@ -3915,29 +4059,32 @@
         """
         Return the requested block header as specified by ``block_hash``.
         Raise ``BlockNotFound`` if no block header with the given hash exists in the db.
         """
         ...
 
     @abstractmethod
-    def get_canonical_block_header_by_number(self, block_number: BlockNumber) -> BlockHeaderAPI:
+    def get_canonical_block_header_by_number(
+        self, block_number: BlockNumber
+    ) -> BlockHeaderAPI:
         """
         Return the block header with the given number in the canonical chain.
 
         Raise ``HeaderNotFound`` if there's no block header with the given number in the
         canonical chain.
         """
         ...
 
     @abstractmethod
     def get_canonical_head(self) -> BlockHeaderAPI:
         """
         Return the block header at the canonical chain head.
 
-        Raise ``CanonicalHeadNotFound`` if there's no head defined for the canonical chain.
+        Raise ``CanonicalHeadNotFound`` if there's no head defined for the
+        canonical chain.
         """
         ...
 
     @abstractmethod
     def get_score(self, block_hash: Hash32) -> int:
         """
         Return the difficulty score of the block with the given ``block_hash``.
@@ -3983,16 +4130,16 @@
         ...
 
     @abstractmethod
     def get_canonical_block_by_number(self, block_number: BlockNumber) -> BlockAPI:
         """
         Return the block with the given ``block_number`` in the canonical chain.
 
-        Raise ``BlockNotFound`` if no block with the given ``block_number`` exists in the
-        canonical chain.
+        Raise ``BlockNotFound`` if no block with the given ``block_number`` exists
+        in the canonical chain.
         """
         ...
 
     @abstractmethod
     def get_canonical_block_hash(self, block_number: BlockNumber) -> Hash32:
         """
         Return the block hash with the given ``block_number`` in the canonical chain.
@@ -4000,18 +4147,18 @@
         Raise ``BlockNotFound`` if there's no block with the given number in the
         canonical chain.
         """
         ...
 
     @abstractmethod
     def build_block_with_transactions_and_withdrawals(
-            self,
-            transactions: Tuple[SignedTransactionAPI, ...],
-            parent_header: BlockHeaderAPI = None,
-            withdrawals: Tuple[WithdrawalAPI, ...] = None,
+        self,
+        transactions: Tuple[SignedTransactionAPI, ...],
+        parent_header: BlockHeaderAPI = None,
+        withdrawals: Tuple[WithdrawalAPI, ...] = None,
     ) -> Tuple[BlockAPI, Tuple[ReceiptAPI, ...], Tuple[ComputationAPI, ...]]:
         """
         Generate a block with the provided transactions. This does *not* import
         that block into your chain. If you want this new block in your chain,
         run :meth:`~import_block` with the result block from this method.
 
         :param transactions: an iterable of transactions to insert into the block
@@ -4028,113 +4175,121 @@
     def create_transaction(self, *args: Any, **kwargs: Any) -> SignedTransactionAPI:
         """
         Passthrough helper to the current VM class.
         """
         ...
 
     @abstractmethod
-    def create_unsigned_transaction(cls,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> UnsignedTransactionAPI:
+    def create_unsigned_transaction(
+        cls,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+    ) -> UnsignedTransactionAPI:
         """
         Passthrough helper to the current VM class.
         """
         ...
 
     @abstractmethod
-    def get_canonical_transaction_index(self, transaction_hash: Hash32) -> Tuple[BlockNumber, int]:
+    def get_canonical_transaction_index(
+        self, transaction_hash: Hash32
+    ) -> Tuple[BlockNumber, int]:
         """
         Return a 2-tuple of (block_number, transaction_index) indicating which
         block the given transaction can be found in and at what index in the
         block transactions.
 
         Raise ``TransactionNotFound`` if the transaction does not exist in the canoncial
         chain.
         """
 
     @abstractmethod
-    def get_canonical_transaction(self, transaction_hash: Hash32) -> SignedTransactionAPI:
+    def get_canonical_transaction(
+        self, transaction_hash: Hash32
+    ) -> SignedTransactionAPI:
         """
         Return the requested transaction as specified by the ``transaction_hash``
         from the canonical chain.
 
         Raise ``TransactionNotFound`` if no transaction with the specified hash is
         found in the canonical chain.
         """
         ...
 
     @abstractmethod
-    def get_canonical_transaction_by_index(self,
-                                           block_number: BlockNumber,
-                                           index: int) -> SignedTransactionAPI:
+    def get_canonical_transaction_by_index(
+        self, block_number: BlockNumber, index: int
+    ) -> SignedTransactionAPI:
         """
         Return the requested transaction as specified by the ``block_number``
         and ``index`` from the canonical chain.
 
-        Raise ``TransactionNotFound`` if no transaction exists at ``index`` at ``block_number`` in
-        the canonical chain.
+        Raise ``TransactionNotFound`` if no transaction exists at ``index`` at
+        ``block_number`` in the canonical chain.
         """
         ...
 
     @abstractmethod
     def get_transaction_receipt(self, transaction_hash: Hash32) -> ReceiptAPI:
         """
-        Return the requested receipt for the transaction as specified by the ``transaction_hash``.
+        Return the requested receipt for the transaction as specified
+        by the ``transaction_hash``.
 
-        Raise ``ReceiptNotFound`` if not receipt for the specified ``transaction_hash`` is found
-        in the canonical chain.
+        Raise ``ReceiptNotFound`` if no receipt for the specified
+        ``transaction_hash`` is found in the canonical chain.
         """
         ...
 
     @abstractmethod
-    def get_transaction_receipt_by_index(self, block_number: BlockNumber, index: int) -> ReceiptAPI:
+    def get_transaction_receipt_by_index(
+        self, block_number: BlockNumber, index: int
+    ) -> ReceiptAPI:
         """
-        Return the requested receipt for the transaction as specified by the ``block_number``
-        and ``index``.
+        Return the requested receipt for the transaction as specified by the
+        ``block_number`` and ``index``.
 
-        Raise ``ReceiptNotFound`` if not receipt for the specified ``block_number`` and ``index`` is
-        found in the canonical chain.
+        Raise ``ReceiptNotFound`` if no receipt for the specified ``block_number``
+        and ``index`` is found in the canonical chain.
         """
         ...
 
     #
     # Execution API
     #
     @abstractmethod
     def get_transaction_result(
-            self,
-            transaction: SignedTransactionAPI,
-            at_header: BlockHeaderAPI) -> bytes:
+        self, transaction: SignedTransactionAPI, at_header: BlockHeaderAPI
+    ) -> bytes:
         """
         Return the result of running the given transaction.
         This is referred to as a `call()` in web3.
         """
         ...
 
     @abstractmethod
     def estimate_gas(
-            self,
-            transaction: SignedTransactionAPI,
-            at_header: BlockHeaderAPI = None) -> int:
+        self, transaction: SignedTransactionAPI, at_header: BlockHeaderAPI = None
+    ) -> int:
         """
         Return an estimation of the amount of gas the given ``transaction`` will
         use if executed on top of the block specified by ``at_header``.
         """
         ...
 
     @abstractmethod
-    def import_block(self,
-                     block: BlockAPI,
-                     perform_validation: bool = True,
-                     ) -> BlockImportResult:
+    def import_block(
+        self,
+        block: BlockAPI,
+        perform_validation: bool = True,
+    ) -> BlockImportResult:
         """
         Import the given ``block`` and return a 3-tuple
 
         - the imported block
         - a tuple of blocks which are now part of the canonical chain.
         - a tuple of blocks which were canonical and now are no longer canonical.
         """
@@ -4175,47 +4330,53 @@
         """
         Validate the uncles for the given ``block``.
         """
         ...
 
     @abstractmethod
     def validate_chain(
-            self,
-            root: BlockHeaderAPI,
-            descendants: Tuple[BlockHeaderAPI, ...],
-            seal_check_random_sample_rate: int = 1) -> None:
-        """
-        Validate that all of the descendents are valid, given that the root header is valid.
-
-        By default, check the seal validity (Proof-of-Work on Ethereum 1.x mainnet) of all headers.
-        This can be expensive. Instead, check a random sample of seals using
-        seal_check_random_sample_rate.
+        self,
+        root: BlockHeaderAPI,
+        descendants: Tuple[BlockHeaderAPI, ...],
+        seal_check_random_sample_rate: int = 1,
+    ) -> None:
+        """
+        Validate that all of the descendents are valid, given that the
+        root header is valid.
+
+        By default, check the seal validity (Proof-of-Work on Ethereum 1.x mainnet)
+        of all headers. This can be expensive. Instead, check a random sample of seals
+        using seal_check_random_sample_rate.
         """
         ...
 
     @abstractmethod
     def validate_chain_extension(self, headers: Tuple[BlockHeaderAPI, ...]) -> None:
         """
-        Validate a chain of headers under the assumption that the entire chain of headers is
-        present. Headers that are not already in the database must exist in ``headers``. Calling
-        this API is not a replacement for calling :meth:`~eth.abc.ChainAPI.validate_chain`, it is
-        an additional API to call at a different stage of header processing to enable consensus
-        schemes where the consensus can not be verified out of order.
+        Validate a chain of headers under the assumption that the entire chain of
+        headers is present. Headers that are not already in the database must exist in
+        ``headers``. Calling this API is not a replacement for calling
+        :meth:`~eth.abc.ChainAPI.validate_chain`, it is an additional API to call at a
+        different stage of header processing to enable consensus schemes where the
+        consensus can not be verified out of order.
         """
         ...
 
 
 class MiningChainAPI(ChainAPI):
     """
     Like :class:`~eth.abc.ChainAPI` but with APIs to create blocks incrementally.
     """
+
     header: BlockHeaderAPI
 
     @abstractmethod
-    def __init__(self, base_db: AtomicDatabaseAPI, header: BlockHeaderAPI = None) -> None:
+    def __init__(
+        self, base_db: AtomicDatabaseAPI, header: BlockHeaderAPI = None
+    ) -> None:
         """
         Initialize the chain.
         """
         ...
 
     @abstractmethod
     def set_header_timestamp(self, timestamp: int) -> None:
@@ -4225,34 +4386,34 @@
         This is mostly useful for testing, as the timestamp will be chosen
         automatically if this method is not called.
         """
         ...
 
     @abstractmethod
     def mine_all(
-            self,
-            transactions: Sequence[SignedTransactionAPI],
-            *args: Any,
-            parent_header: BlockHeaderAPI = None,
-            **kwargs: Any,
+        self,
+        transactions: Sequence[SignedTransactionAPI],
+        *args: Any,
+        parent_header: BlockHeaderAPI = None,
+        **kwargs: Any,
     ) -> Tuple[BlockImportResult, Tuple[ReceiptAPI, ...], Tuple[ComputationAPI, ...]]:
         """
         Build a block with the given transactions, and mine it.
 
         Optionally, supply the parent block header to mine on top of.
 
         This is much faster than individually running :meth:`apply_transaction`
         and then :meth:`mine_block`.
         """
         ...
 
     @abstractmethod
-    def apply_transaction(self,
-                          transaction: SignedTransactionAPI
-                          ) -> Tuple[BlockAPI, ReceiptAPI, ComputationAPI]:
+    def apply_transaction(
+        self, transaction: SignedTransactionAPI
+    ) -> Tuple[BlockAPI, ReceiptAPI, ComputationAPI]:
         """
         Apply the transaction to the current tip block.
 
         WARNING: ReceiptAPI and Transaction trie generation is computationally
         heavy and incurs significant performance overhead.
         """
         ...
```

### Comparing `py-evm-0.7.0a1/eth/chains/base.py` & `py-evm-0.7.0a2/eth/chains/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,133 +1,136 @@
+import logging
 import operator
 import random
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     Sequence,
     Tuple,
     Type,
 )
 
-import logging
-
 from eth_typing import (
     Address,
     BlockNumber,
     Hash32,
 )
 from eth_utils import (
     encode_hex,
 )
 from eth_utils.toolz import (
     concatv,
     sliding_window,
 )
 
-from eth._utils.db import (
-    apply_state_dict,
-)
 from eth._utils.datatypes import (
     Configurable,
 )
+from eth._utils.db import (
+    apply_state_dict,
+)
 from eth._utils.rlp import (
     validate_imported_block_unchanged,
 )
+from eth._warnings import (
+    catch_and_ignore_import_warning,
+)
 from eth.abc import (
-    BlockAPI,
-    BlockAndMetaWitness,
-    MiningChainAPI,
     AtomicDatabaseAPI,
+    BlockAndMetaWitness,
+    BlockAPI,
     BlockHeaderAPI,
     BlockImportResult,
     BlockPersistResult,
     ChainAPI,
     ChainDatabaseAPI,
+    ComputationAPI,
     ConsensusContextAPI,
-    VirtualMachineAPI,
+    MiningChainAPI,
     ReceiptAPI,
-    ComputationAPI,
-    StateAPI,
     SignedTransactionAPI,
+    StateAPI,
     UnsignedTransactionAPI,
+    VirtualMachineAPI,
     WithdrawalAPI,
 )
 from eth.consensus import (
     ConsensusContext,
 )
 from eth.constants import (
     EMPTY_UNCLE_HASH,
     MAX_UNCLE_DEPTH,
 )
-
 from eth.db.chain import (
     ChainDB,
 )
 from eth.db.header import (
     HeaderDB,
 )
-
 from eth.estimators import (
     get_gas_estimator,
 )
 from eth.exceptions import (
     HeaderNotFound,
     TransactionNotFound,
     VMNotFound,
 )
-
 from eth.rlp.headers import (
     BlockHeader,
 )
-
 from eth.typing import (
     AccountState,
     HeaderParams,
     StaticMethod,
 )
-
 from eth.validation import (
     validate_block_number,
     validate_uint256,
-    validate_word,
     validate_vm_configuration,
+    validate_word,
+)
+from eth.vm.chain_context import (
+    ChainContext,
 )
-from eth.vm.chain_context import ChainContext
 
-from eth._warnings import catch_and_ignore_import_warning
 with catch_and_ignore_import_warning():
     from eth_utils import (
-        to_set,
         ValidationError,
+        to_set,
     )
     from eth_utils.toolz import (
         assoc,
         compose,
         groupby,
         iterate,
         take,
     )
 
 
 class BaseChain(Configurable, ChainAPI):
     """
     The base class for all Chain objects
     """
+
     chaindb: ChainDatabaseAPI = None
     chaindb_class: Type[ChainDatabaseAPI] = None
     consensus_context_class: Type[ConsensusContextAPI] = None
     vm_configuration: Tuple[Tuple[BlockNumber, Type[VirtualMachineAPI]], ...] = None
     chain_id: int = None
 
     @classmethod
-    def get_vm_class_for_block_number(cls, block_number: BlockNumber) -> Type[VirtualMachineAPI]:
+    def get_vm_class_for_block_number(
+        cls, block_number: BlockNumber
+    ) -> Type[VirtualMachineAPI]:
         if cls.vm_configuration is None:
-            raise AttributeError("Chain classes must define the VMs in vm_configuration")
+            raise AttributeError(
+                "Chain classes must define the VMs in vm_configuration"
+            )
 
         validate_block_number(block_number)
         for start_block, vm_class in reversed(cls.vm_configuration):
             if block_number >= start_block:
                 return vm_class
         else:
             raise VMNotFound(f"No vm available for block #{block_number}")
@@ -136,34 +139,35 @@
     def get_vm_class(cls, header: BlockHeaderAPI) -> Type[VirtualMachineAPI]:
         return cls.get_vm_class_for_block_number(header.block_number)
 
     #
     # Validation API
     #
     def validate_chain(
-            self,
-            root: BlockHeaderAPI,
-            descendants: Tuple[BlockHeaderAPI, ...],
-            seal_check_random_sample_rate: int = 1) -> None:
-
+        self,
+        root: BlockHeaderAPI,
+        descendants: Tuple[BlockHeaderAPI, ...],
+        seal_check_random_sample_rate: int = 1,
+    ) -> None:
         all_indices = range(len(descendants))
         if seal_check_random_sample_rate == 1:
             indices_to_check_seal = set(all_indices)
         elif seal_check_random_sample_rate == 0:
             indices_to_check_seal = set()
         else:
             sample_size = len(all_indices) // seal_check_random_sample_rate
             indices_to_check_seal = set(random.sample(all_indices, sample_size))
 
         header_pairs = sliding_window(2, concatv([root], descendants))
 
         for index, (parent, child) in enumerate(header_pairs):
             if child.parent_hash != parent.hash:
                 raise ValidationError(
-                    f"Invalid header chain; {child} has parent {encode_hex(child.parent_hash)},"
+                    f"Invalid header chain; {child} has parent"
+                    f" {encode_hex(child.parent_hash)},"
                     f" but expected {encode_hex(parent.hash)}"
                 )
             vm = self.get_vm(child)
             try:
                 vm.validate_header(child, parent)
             except ValidationError as exc:
                 raise ValidationError(
@@ -188,15 +192,16 @@
 
     chaindb_class: Type[ChainDatabaseAPI] = ChainDB
     consensus_context_class: Type[ConsensusContextAPI] = ConsensusContext
 
     def __init__(self, base_db: AtomicDatabaseAPI) -> None:
         if not self.vm_configuration:
             raise ValueError(
-                "The Chain class cannot be instantiated with an empty `vm_configuration`"
+                "The Chain class cannot be instantiated with "
+                "an empty `vm_configuration`"
             )
         else:
             validate_vm_configuration(self.vm_configuration)
 
         self.chaindb = self.get_chaindb_class()(base_db)
         self.consensus_context = self.consensus_context_class(self.chaindb.db)
         self.headerdb = HeaderDB(base_db)
@@ -212,51 +217,53 @@
             raise AttributeError("`chaindb_class` not set")
         return cls.chaindb_class
 
     #
     # Chain API
     #
     @classmethod
-    def from_genesis(cls,
-                     base_db: AtomicDatabaseAPI,
-                     genesis_params: Dict[str, HeaderParams],
-                     genesis_state: AccountState = None) -> 'BaseChain':
+    def from_genesis(
+        cls,
+        base_db: AtomicDatabaseAPI,
+        genesis_params: Dict[str, HeaderParams],
+        genesis_state: AccountState = None,
+    ) -> "BaseChain":
         genesis_vm_class = cls.get_vm_class_for_block_number(BlockNumber(0))
 
         pre_genesis_header = BlockHeader(difficulty=0, block_number=-1, gas_limit=0)
         chain_context = ChainContext(cls.chain_id)
         state = genesis_vm_class.build_state(base_db, pre_genesis_header, chain_context)
 
         if genesis_state is None:
             genesis_state = {}
 
         # mutation
         apply_state_dict(state, genesis_state)
         state.persist()
 
-        if 'state_root' not in genesis_params:
+        if "state_root" not in genesis_params:
             # If the genesis state_root was not specified, use the value
             # computed from the initialized state database.
-            genesis_params = assoc(genesis_params, 'state_root', state.state_root)
-        elif genesis_params['state_root'] != state.state_root:
+            genesis_params = assoc(genesis_params, "state_root", state.state_root)
+        elif genesis_params["state_root"] != state.state_root:
             # If the genesis state_root was specified, validate that it matches
             # the computed state from the initialized state database.
             raise ValidationError(
                 "The provided genesis state root does not match the computed "
                 f"genesis state root.  Got {state.state_root!r}.  "
                 f"Expected {genesis_params['state_root']!r}"
             )
 
         genesis_header = genesis_vm_class.create_genesis_header(**genesis_params)
         return cls.from_genesis_header(base_db, genesis_header)
 
     @classmethod
-    def from_genesis_header(cls,
-                            base_db: AtomicDatabaseAPI,
-                            genesis_header: BlockHeaderAPI) -> 'BaseChain':
+    def from_genesis_header(
+        cls, base_db: AtomicDatabaseAPI, genesis_header: BlockHeaderAPI
+    ) -> "BaseChain":
         chaindb = cls.get_chaindb_class()(base_db)
         chaindb.persist_header(genesis_header)
         return cls(base_db)
 
     #
     # VM API
     #
@@ -265,32 +272,34 @@
         vm_class = self.get_vm_class_for_block_number(header.block_number)
         chain_context = ChainContext(self.chain_id)
 
         return vm_class(
             header=header,
             chaindb=self.chaindb,
             chain_context=chain_context,
-            consensus_context=self.consensus_context
+            consensus_context=self.consensus_context,
         )
 
     #
     # Header API
     #
-    def create_header_from_parent(self,
-                                  parent_header: BlockHeaderAPI,
-                                  **header_params: HeaderParams) -> BlockHeaderAPI:
+    def create_header_from_parent(
+        self, parent_header: BlockHeaderAPI, **header_params: HeaderParams
+    ) -> BlockHeaderAPI:
         return self.get_vm_class_for_block_number(
             block_number=BlockNumber(parent_header.block_number + 1),
         ).create_header_from_parent(parent_header, **header_params)
 
     def get_block_header_by_hash(self, block_hash: Hash32) -> BlockHeaderAPI:
         validate_word(block_hash, title="Block Hash")
         return self.chaindb.get_block_header_by_hash(block_hash)
 
-    def get_canonical_block_header_by_number(self, block_number: BlockNumber) -> BlockHeaderAPI:
+    def get_canonical_block_header_by_number(
+        self, block_number: BlockNumber
+    ) -> BlockHeaderAPI:
         return self.chaindb.get_canonical_block_header_by_number(block_number)
 
     def get_canonical_head(self) -> BlockHeaderAPI:
         return self.chaindb.get_canonical_head()
 
     def get_score(self, block_hash: Hash32) -> int:
         return self.headerdb.get_score(block_hash)
@@ -313,19 +322,22 @@
         ancestor_count = min(header.block_number, limit)
 
         # We construct a temporary block object
         vm_class = self.get_vm_class_for_block_number(header.block_number)
         block_class = vm_class.get_block_class()
         block = block_class(header=header, uncles=[], transactions=[])
 
-        ancestor_generator = iterate(compose(
-            self.get_block_by_hash,
-            operator.attrgetter('parent_hash'),
-            operator.attrgetter('header'),
-        ), block)
+        ancestor_generator = iterate(
+            compose(
+                self.get_block_by_hash,
+                operator.attrgetter("parent_hash"),
+                operator.attrgetter("header"),
+            ),
+            block,
+        )
         # we peel off the first element from the iterator which will be the
         # temporary block object we constructed.
         next(ancestor_generator)
 
         return tuple(take(ancestor_count, ancestor_generator))
 
     def get_block(self) -> BlockAPI:
@@ -338,24 +350,26 @@
 
     def get_block_by_header(self, block_header: BlockHeaderAPI) -> BlockAPI:
         vm = self.get_vm(block_header)
         return vm.get_block()
 
     def get_canonical_block_by_number(self, block_number: BlockNumber) -> BlockAPI:
         validate_uint256(block_number, title="Block Number")
-        return self.get_block_by_hash(self.chaindb.get_canonical_block_hash(block_number))
+        return self.get_block_by_hash(
+            self.chaindb.get_canonical_block_hash(block_number)
+        )
 
     def get_canonical_block_hash(self, block_number: BlockNumber) -> Hash32:
         return self.chaindb.get_canonical_block_hash(block_number)
 
     def build_block_with_transactions_and_withdrawals(
-            self,
-            transactions: Sequence[SignedTransactionAPI],
-            parent_header: BlockHeaderAPI = None,
-            withdrawals: Sequence[WithdrawalAPI] = None,
+        self,
+        transactions: Sequence[SignedTransactionAPI],
+        parent_header: BlockHeaderAPI = None,
+        withdrawals: Sequence[WithdrawalAPI] = None,
     ) -> Tuple[BlockAPI, Tuple[ReceiptAPI, ...], Tuple[ComputationAPI, ...]]:
         base_header = self.ensure_header(parent_header)
         vm = self.get_vm(base_header)
 
         new_header, receipts, computations = vm.apply_all_transactions(
             transactions,
             base_header,
@@ -373,165 +387,166 @@
         )
 
         return new_block, receipts, computations
 
     #
     # Transaction API
     #
-    def get_canonical_transaction_index(self, transaction_hash: Hash32) -> Tuple[BlockNumber, int]:
+    def get_canonical_transaction_index(
+        self, transaction_hash: Hash32
+    ) -> Tuple[BlockNumber, int]:
         return self.chaindb.get_transaction_index(transaction_hash)
 
-    def get_canonical_transaction(self, transaction_hash: Hash32) -> SignedTransactionAPI:
+    def get_canonical_transaction(
+        self, transaction_hash: Hash32
+    ) -> SignedTransactionAPI:
         (block_num, index) = self.chaindb.get_transaction_index(transaction_hash)
 
         transaction = self.get_canonical_transaction_by_index(block_num, index)
 
         if transaction.hash == transaction_hash:
             return transaction
         else:
             raise TransactionNotFound(
                 f"Found transaction {encode_hex(transaction.hash)} "
-                f"instead of {encode_hex(transaction_hash)} in block {block_num} at {index}"
+                f"instead of {encode_hex(transaction_hash)} in block "
+                f"{block_num} at {index}"
             )
 
-    def get_canonical_transaction_by_index(self,
-                                           block_number: BlockNumber,
-                                           index: int) -> SignedTransactionAPI:
-
+    def get_canonical_transaction_by_index(
+        self, block_number: BlockNumber, index: int
+    ) -> SignedTransactionAPI:
         VM_class = self.get_vm_class_for_block_number(block_number)
 
         return self.chaindb.get_transaction_by_index(
             block_number,
             index,
             VM_class.get_transaction_builder(),
         )
 
     def create_transaction(self, *args: Any, **kwargs: Any) -> SignedTransactionAPI:
         return self.get_vm().create_transaction(*args, **kwargs)
 
-    def create_unsigned_transaction(self,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> UnsignedTransactionAPI:
+    def create_unsigned_transaction(
+        self,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+    ) -> UnsignedTransactionAPI:
         return self.get_vm().create_unsigned_transaction(
             nonce=nonce,
             gas_price=gas_price,
             gas=gas,
             to=to,
             value=value,
             data=data,
         )
 
     def get_transaction_receipt(self, transaction_hash: Hash32) -> ReceiptAPI:
-        transaction_block_number, transaction_index = self.chaindb.get_transaction_index(
+        (
+            transaction_block_number,
+            transaction_index,
+        ) = self.chaindb.get_transaction_index(
             transaction_hash,
         )
-        return self.get_transaction_receipt_by_index(transaction_block_number, transaction_index)
-
-    def get_transaction_receipt_by_index(self,
-                                         block_number: BlockNumber,
-                                         index: int) -> ReceiptAPI:
+        return self.get_transaction_receipt_by_index(
+            transaction_block_number, transaction_index
+        )
 
+    def get_transaction_receipt_by_index(
+        self, block_number: BlockNumber, index: int
+    ) -> ReceiptAPI:
         vm = self.get_vm_class_for_block_number(block_number)
 
         receipt = self.chaindb.get_receipt_by_index(
             block_number,
             index,
             vm.get_receipt_builder(),
         )
 
         return receipt
 
     #
     # Execution API
     #
     def get_transaction_result(
-            self,
-            transaction: SignedTransactionAPI,
-            at_header: BlockHeaderAPI) -> bytes:
-
+        self, transaction: SignedTransactionAPI, at_header: BlockHeaderAPI
+    ) -> bytes:
         with self.get_vm(at_header).in_costless_state() as state:
             computation = state.costless_execute_transaction(transaction)
 
         computation.raise_if_error()
         return computation.output
 
     def estimate_gas(
-            self,
-            transaction: SignedTransactionAPI,
-            at_header: BlockHeaderAPI = None) -> int:
+        self, transaction: SignedTransactionAPI, at_header: BlockHeaderAPI = None
+    ) -> int:
         if at_header is None:
             at_header = self.get_canonical_head()
         with self.get_vm(at_header).in_costless_state() as state:
             return self.gas_estimator(state, transaction)
 
-    def import_block(self,
-                     block: BlockAPI,
-                     perform_validation: bool = True
-                     ) -> BlockImportResult:
-
+    def import_block(
+        self, block: BlockAPI, perform_validation: bool = True
+    ) -> BlockImportResult:
         try:
             parent_header = self.get_block_header_by_hash(block.header.parent_hash)
         except HeaderNotFound:
             raise ValidationError(
                 f"Attempt to import block #{block.number}.  "
                 f"Cannot import block {block.hash!r} before importing "
                 f"its parent block at {block.header.parent_hash!r}"
             )
 
         base_header_for_import = self.create_header_from_parent(parent_header)
-        # Make a copy of the empty header, adding in the expected amount of gas used. This
-        #   allows for richer logging in the VM.
+        # Make a copy of the empty header, adding in the expected amount of gas used.
+        #   This allows for richer logging in the VM.
         annotated_header = base_header_for_import.copy(gas_used=block.header.gas_used)
         block_result = self.get_vm(annotated_header).import_block(block)
         imported_block = block_result.block
 
         # Validate the imported block.
         if perform_validation:
             try:
                 validate_imported_block_unchanged(imported_block, block)
             except ValidationError:
-                self.logger.warning("Proposed %s doesn't follow EVM rules, rejecting...", block)
+                self.logger.warning(
+                    "Proposed %s doesn't follow EVM rules, rejecting...", block
+                )
                 raise
 
         persist_result = self.persist_block(imported_block, perform_validation)
         return BlockImportResult(*persist_result, block_result.meta_witness)
 
     def persist_block(
-            self,
-            block: BlockAPI,
-            perform_validation: bool = True) -> BlockPersistResult:
-
+        self, block: BlockAPI, perform_validation: bool = True
+    ) -> BlockPersistResult:
         if perform_validation:
             self.validate_block(block)
 
         (
             new_canonical_hashes,
             old_canonical_hashes,
         ) = self.chaindb.persist_block(block)
 
         self.logger.debug(
-            'Persisted block: number %s | hash %s',
+            "Persisted block: number %s | hash %s",
             block.number,
             encode_hex(block.hash),
         )
 
         new_canonical_blocks = tuple(
-            self.get_block_by_hash(header_hash)
-            for header_hash
-            in new_canonical_hashes
+            self.get_block_by_hash(header_hash) for header_hash in new_canonical_hashes
         )
         old_canonical_blocks = tuple(
-            self.get_block_by_hash(header_hash)
-            for header_hash
-            in old_canonical_hashes
+            self.get_block_by_hash(header_hash) for header_hash in old_canonical_hashes
         )
 
         return BlockPersistResult(
             imported_block=block,
             new_canonical_blocks=new_canonical_blocks,
             old_canonical_blocks=old_canonical_blocks,
         )
@@ -558,61 +573,64 @@
         vm.validate_seal(header)
 
     def validate_uncles(self, block: BlockAPI) -> None:
         has_uncles = len(block.uncles) > 0
         should_have_uncles = block.header.uncles_hash != EMPTY_UNCLE_HASH
 
         if not has_uncles and not should_have_uncles:
-            # optimization to avoid loading ancestors from DB, since the block has no uncles
+            # optimization to avoid loading ancestors from DB,
+            # since the block has no uncles
             return
         elif has_uncles and not should_have_uncles:
-            raise ValidationError("Block has uncles but header suggests uncles should be empty")
+            raise ValidationError(
+                "Block has uncles but header suggests uncles should be empty"
+            )
         elif should_have_uncles and not has_uncles:
-            raise ValidationError("Header suggests block should have uncles but block has none")
+            raise ValidationError(
+                "Header suggests block should have uncles but block has none"
+            )
 
         # Check for duplicates
-        uncle_groups = groupby(operator.attrgetter('hash'), block.uncles)
-        duplicate_uncles = tuple(sorted(
-            hash for hash, twins in uncle_groups.items() if len(twins) > 1
-        ))
+        uncle_groups = groupby(operator.attrgetter("hash"), block.uncles)
+        duplicate_uncles = tuple(
+            sorted(hash for hash, twins in uncle_groups.items() if len(twins) > 1)
+        )
         if duplicate_uncles:
             raise ValidationError(
                 "Block contains duplicate uncles:\n"
                 f" - {' - '.join(duplicate_uncles)}"
             )
 
         recent_ancestors = tuple(
             ancestor
-            for ancestor
-            in self.get_ancestors(MAX_UNCLE_DEPTH + 1, header=block.header)
+            for ancestor in self.get_ancestors(MAX_UNCLE_DEPTH + 1, header=block.header)
         )
         recent_ancestor_hashes = {ancestor.hash for ancestor in recent_ancestors}
         recent_uncle_hashes = _extract_uncle_hashes(recent_ancestors)
 
         for uncle in block.uncles:
             if uncle.hash == block.hash:
                 raise ValidationError("Uncle has same hash as block")
 
             # ensure the uncle has not already been included.
             if uncle.hash in recent_uncle_hashes:
-                raise ValidationError(
-                    f"Duplicate uncle: {encode_hex(uncle.hash)}"
-                )
+                raise ValidationError(f"Duplicate uncle: {encode_hex(uncle.hash)}")
 
             # ensure that the uncle is not one of the canonical chain blocks.
             if uncle.hash in recent_ancestor_hashes:
                 raise ValidationError(
                     f"Uncle {encode_hex(uncle.hash)} cannot be an ancestor "
                     f"of {encode_hex(block.hash)}"
                 )
 
             # ensure that the uncle was built off of one of the canonical chain
             # blocks.
             if uncle.parent_hash not in recent_ancestor_hashes or (
-               uncle.parent_hash == block.header.parent_hash):
+                uncle.parent_hash == block.header.parent_hash
+            ):
                 raise ValidationError(
                     f"Uncle's parent {encode_hex(uncle.parent_hash)} "
                     f"is not an ancestor of {encode_hex(block.hash)}"
                 )
 
             # Now perform VM level validation of the uncle
             self.validate_seal(uncle)
@@ -634,83 +652,87 @@
         for uncle in block.uncles:
             yield uncle.hash
 
 
 class MiningChain(Chain, MiningChainAPI):
     header: BlockHeaderAPI = None
 
-    def __init__(self, base_db: AtomicDatabaseAPI, header: BlockHeaderAPI = None) -> None:
+    def __init__(
+        self, base_db: AtomicDatabaseAPI, header: BlockHeaderAPI = None
+    ) -> None:
         super().__init__(base_db)
         self.header = self.ensure_header(header)
 
     def apply_transaction(
         self,
         transaction: SignedTransactionAPI,
     ) -> Tuple[BlockAPI, ReceiptAPI, ComputationAPI]:
         vm = self.get_vm(self.header)
         base_block = vm.get_block()
 
         receipt, computation = vm.apply_transaction(base_block.header, transaction)
         header_with_receipt = vm.add_receipt_to_header(base_block.header, receipt)
 
-        # since we are building the block locally, we have to persist all the incremental state
+        # since we are building the block locally,
+        # we have to persist all the incremental state
         vm.state.persist()
-        new_header: BlockHeaderAPI = header_with_receipt.copy(state_root=vm.state.state_root)
+        new_header: BlockHeaderAPI = header_with_receipt.copy(
+            state_root=vm.state.state_root
+        )
 
-        transactions = base_block.transactions + (transaction, )
-        receipts = base_block.get_receipts(self.chaindb) + (receipt, )
+        transactions = base_block.transactions + (transaction,)
+        receipts = base_block.get_receipts(self.chaindb) + (receipt,)
 
         new_block = vm.set_block_transactions_and_withdrawals(
             base_block,
             new_header,
             transactions,
             receipts,
         )
 
         self.header = new_block.header
 
         return new_block, receipt, computation
 
-    def import_block(self,
-                     block: BlockAPI,
-                     perform_validation: bool = True
-                     ) -> BlockImportResult:
-        result = super().import_block(
-            block, perform_validation)
+    def import_block(
+        self, block: BlockAPI, perform_validation: bool = True
+    ) -> BlockImportResult:
+        result = super().import_block(block, perform_validation)
 
         self.header = self.ensure_header()
         return result
 
     def set_header_timestamp(self, timestamp: int) -> None:
         self.header = self.header.copy(timestamp=timestamp)
 
     @staticmethod
     def _custom_header(base_header: BlockHeaderAPI, **kwargs: Any) -> BlockHeaderAPI:
-        header_fields = {'coinbase'}
+        header_fields = {"coinbase"}
         header_params = {k: v for k, v in kwargs.items() if k in header_fields}
         return base_header.copy(**header_params)
 
     def mine_all(
-            self,
-            transactions: Sequence[SignedTransactionAPI],
-            *args: Any,
-            parent_header: BlockHeaderAPI = None,
-            withdrawals: Sequence[WithdrawalAPI] = None,
-            **kwargs: Any,
+        self,
+        transactions: Sequence[SignedTransactionAPI],
+        *args: Any,
+        parent_header: BlockHeaderAPI = None,
+        withdrawals: Sequence[WithdrawalAPI] = None,
+        **kwargs: Any,
     ) -> Tuple[BlockImportResult, Tuple[ReceiptAPI, ...], Tuple[ComputationAPI, ...]]:
-
         if parent_header is None:
             base_header = self.header
         else:
             base_header = self.create_header_from_parent(parent_header)
 
         custom_header = self._custom_header(base_header, **kwargs)
         vm = self.get_vm(custom_header)
 
-        new_header, receipts, computations = vm.apply_all_transactions(transactions, base_header)
+        new_header, receipts, computations = vm.apply_all_transactions(
+            transactions, base_header
+        )
 
         if withdrawals:
             vm.apply_all_withdrawals(withdrawals)
 
         filled_block = vm.set_block_transactions_and_withdrawals(
             vm.get_block(),
             new_header,
```

### Comparing `py-evm-0.7.0a1/eth/chains/goerli/__init__.py` & `py-evm-0.7.0a2/eth/chains/goerli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,19 +23,23 @@
 
 
 GOERLI_GENESIS_HEADER = BlockHeader(
     block_number=0,
     bloom=0,
     coinbase=constants.ZERO_ADDRESS,
     difficulty=1,
-    extra_data=decode_hex('0x22466c6578692069732061207468696e6722202d204166726900000000000000e0a2bd4258d2768837baa26a28fe71dc079f84c70000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000'),  # noqa: E501
+    extra_data=decode_hex(
+        "0x22466c6578692069732061207468696e6722202d204166726900000000000000e0a2bd4258d2768837baa26a28fe71dc079f84c70000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000"  # noqa: E501
+    ),
     gas_limit=10485760,
     gas_used=0,
     mix_hash=constants.ZERO_HASH32,
-    nonce=decode_hex('0x0000000000000000'),
+    nonce=decode_hex("0x0000000000000000"),
     parent_hash=constants.GENESIS_PARENT_HASH,
     receipt_root=constants.BLANK_ROOT_HASH,
-    state_root=decode_hex('0x5d6cded585e73c4e322c30c2f782a336316f17dd85a4863b9d838d2d4b8b3008'),
+    state_root=decode_hex(
+        "0x5d6cded585e73c4e322c30c2f782a336316f17dd85a4863b9d838d2d4b8b3008"
+    ),
     timestamp=1548854791,
     transaction_root=constants.BLANK_ROOT_HASH,
     uncles_hash=constants.EMPTY_UNCLE_HASH,
 )
```

### Comparing `py-evm-0.7.0a1/eth/chains/header.py` & `py-evm-0.7.0a2/eth/chains/header.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 from typing import (
-    cast,
     Tuple,
     Type,
+    cast,
 )
 
 from eth_typing import (
     BlockNumber,
     Hash32,
 )
 
+from eth._utils.datatypes import (
+    Configurable,
+)
 from eth.abc import (
     AtomicDatabaseAPI,
     BlockHeaderAPI,
     HeaderChainAPI,
     HeaderDatabaseAPI,
 )
 from eth.db.backends.base import (
     BaseAtomicDB,
 )
 from eth.db.header import (
     HeaderDB,
 )
-from eth._utils.datatypes import (
-    Configurable,
-)
 
 
 class HeaderChain(Configurable, HeaderChainAPI):
     _base_db: AtomicDatabaseAPI = None
     _headerdb: HeaderDatabaseAPI = None
 
     _headerdb_class: Type[HeaderDatabaseAPI] = HeaderDB
 
-    def __init__(self, base_db: AtomicDatabaseAPI, header: BlockHeaderAPI = None) -> None:
+    def __init__(
+        self, base_db: AtomicDatabaseAPI, header: BlockHeaderAPI = None
+    ) -> None:
         self.base_db = base_db
         self.headerdb = self.get_headerdb_class()(base_db)
 
         if header is None:
             self.header = self.get_canonical_head()
         else:
             self.header = header
 
     #
     # Chain Initialization API
     #
     @classmethod
-    def from_genesis_header(cls,
-                            base_db: AtomicDatabaseAPI,
-                            genesis_header: BlockHeaderAPI) -> HeaderChainAPI:
+    def from_genesis_header(
+        cls, base_db: AtomicDatabaseAPI, genesis_header: BlockHeaderAPI
+    ) -> HeaderChainAPI:
         headerdb = cls.get_headerdb_class()(cast(BaseAtomicDB, base_db))
         headerdb.persist_header(genesis_header)
         return cls(base_db, genesis_header)
 
     #
     # Helpers
     #
@@ -63,28 +65,30 @@
 
     #
     # Canonical Chain API
     #
     def get_canonical_block_hash(self, block_number: BlockNumber) -> Hash32:
         return self.headerdb.get_canonical_block_hash(block_number)
 
-    def get_canonical_block_header_by_number(self, block_number: BlockNumber) -> BlockHeaderAPI:
+    def get_canonical_block_header_by_number(
+        self, block_number: BlockNumber
+    ) -> BlockHeaderAPI:
         return self.headerdb.get_canonical_block_header_by_number(block_number)
 
     def get_canonical_head(self) -> BlockHeaderAPI:
         return self.headerdb.get_canonical_head()
 
     #
     # Header API
     #
     def get_block_header_by_hash(self, block_hash: Hash32) -> BlockHeaderAPI:
         return self.headerdb.get_block_header_by_hash(block_hash)
 
     def header_exists(self, block_hash: Hash32) -> bool:
         return self.headerdb.header_exists(block_hash)
 
-    def import_header(self,
-                      header: BlockHeaderAPI
-                      ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
+    def import_header(
+        self, header: BlockHeaderAPI
+    ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
         new_canonical_headers = self.headerdb.persist_header(header)
         self.header = self.get_canonical_head()
         return new_canonical_headers
```

### Comparing `py-evm-0.7.0a1/eth/chains/mainnet/__init__.py` & `py-evm-0.7.0a2/eth/chains/mainnet/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,18 +51,17 @@
     PetersburgVM,
     ShanghaiVM,
     SpuriousDragonVM,
     TangerineWhistleVM,
 )
 
 
-def validate_header_is_on_intended_dao_fork(support_dao_fork: bool,
-                                            dao_fork_at: BlockNumber,
-                                            header: BlockHeaderAPI) -> None:
-
+def validate_header_is_on_intended_dao_fork(
+    support_dao_fork: bool, dao_fork_at: BlockNumber, header: BlockHeaderAPI
+) -> None:
     # The special extra_data is set on the ten headers starting at the fork
     extra_data_block_nums = range(dao_fork_at, dao_fork_at + 10)
 
     if header.block_number in extra_data_block_nums:
         if support_dao_fork and header.extra_data != DAO_FORK_MAINNET_EXTRA_DATA:
             raise ValidationError(
                 f"Block {header!r} must have extra data "
@@ -73,26 +72,26 @@
             raise ValidationError(
                 f"Block {header!r} must not have extra data "
                 f"{encode_hex(DAO_FORK_MAINNET_EXTRA_DATA)} when declining the DAO fork"
             )
 
 
 class MainnetDAOValidatorVM(HomesteadVM):
-    """Only on mainnet, TheDAO fork is accompanied by special extra data. Validate those headers"""
+    """
+    Only on mainnet, TheDAO fork is accompanied by special extra data.
+    Validate those headers
+    """
 
     @classmethod
-    def validate_header(cls,
-                        header: BlockHeaderAPI,
-                        previous_header: BlockHeaderAPI) -> None:
-
+    def validate_header(
+        cls, header: BlockHeaderAPI, previous_header: BlockHeaderAPI
+    ) -> None:
         super().validate_header(header, previous_header)
         validate_header_is_on_intended_dao_fork(
-            cls.support_dao_fork,
-            cls.get_dao_fork_block_number(),
-            header
+            cls.support_dao_fork, cls.get_dao_fork_block_number(), header
         )
 
 
 class MainnetHomesteadVM(MainnetDAOValidatorVM):
     _dao_fork_block_number = DAO_FORK_MAINNET_BLOCK
 
 
@@ -133,32 +132,35 @@
 MAINNET_VMS = MINING_MAINNET_VMS + POS_MAINNET_VMS
 MAINNET_VM_CONFIGURATION = tuple(zip(MAINNET_FORK_BLOCKS, MAINNET_VMS))
 
 
 class BaseMainnetChain:
     chain_id = MAINNET_CHAIN_ID
     vm_configuration: Tuple[
-        Tuple[BlockNumber, Type[VirtualMachineAPI]],
-        ...
+        Tuple[BlockNumber, Type[VirtualMachineAPI]], ...
     ] = MAINNET_VM_CONFIGURATION
 
 
 class MainnetChain(BaseMainnetChain, Chain):
     pass
 
 
 MAINNET_GENESIS_HEADER = BlockHeader(
     difficulty=eth_constants.GENESIS_DIFFICULTY,
-    extra_data=decode_hex("0x11bbe8db4e347b4e8c937c1c8370e4b5ed33adb3db69cbdb7a38e1e50b1b82fa"),
+    extra_data=decode_hex(
+        "0x11bbe8db4e347b4e8c937c1c8370e4b5ed33adb3db69cbdb7a38e1e50b1b82fa"
+    ),
     gas_limit=eth_constants.GENESIS_GAS_LIMIT,
     gas_used=0,
     bloom=0,
     mix_hash=eth_constants.ZERO_HASH32,
     nonce=eth_constants.GENESIS_NONCE,
     block_number=0,
     parent_hash=eth_constants.ZERO_HASH32,
     receipt_root=eth_constants.BLANK_ROOT_HASH,
     uncles_hash=eth_constants.EMPTY_UNCLE_HASH,
-    state_root=decode_hex("0xd7f8974fb5ac78d9ac099b9ad5018bedc2ce0a72dad1827a1709da30580f0544"),
+    state_root=decode_hex(
+        "0xd7f8974fb5ac78d9ac099b9ad5018bedc2ce0a72dad1827a1709da30580f0544"
+    ),
     timestamp=0,
     transaction_root=eth_constants.BLANK_ROOT_HASH,
 )
```

### Comparing `py-evm-0.7.0a1/eth/chains/mainnet/constants.py` & `py-evm-0.7.0a2/eth/chains/mainnet/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from eth_typing import BlockNumber
-
+from eth_typing import (
+    BlockNumber,
+)
 
 # https://github.com/ethereum/EIPs/blob/master/EIPS/eip-155.md
 MAINNET_CHAIN_ID = 1
 
 # Fork Blocks listed in ascending order
 
 
@@ -14,15 +15,15 @@
 
 
 #
 # DAO Block
 #
 DAO_FORK_MAINNET_BLOCK = BlockNumber(1920000)
 
-DAO_FORK_MAINNET_EXTRA_DATA = b'dao-hard-fork'
+DAO_FORK_MAINNET_EXTRA_DATA = b"dao-hard-fork"
 
 
 #
 # Tangerine Whistle Block
 #
 TANGERINE_WHISTLE_MAINNET_BLOCK = BlockNumber(2463000)
```

### Comparing `py-evm-0.7.0a1/eth/chains/ropsten/__init__.py` & `py-evm-0.7.0a2/eth/chains/ropsten/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,47 +27,51 @@
     PetersburgVM,
     SpuriousDragonVM,
     TangerineWhistleVM,
 )
 
 
 ROPSTEN_VM_CONFIGURATION = (
-    # Note: Frontier and Homestead are excluded since this chain starts at Tangerine Whistle.
+    # Note: Frontier and Homestead are excluded since this chain
+    # starts at Tangerine Whistle.
     (TANGERINE_WHISTLE_ROPSTEN_BLOCK, TangerineWhistleVM),
     (SPURIOUS_DRAGON_ROPSTEN_BLOCK, SpuriousDragonVM),
     (BYZANTIUM_ROPSTEN_BLOCK, ByzantiumVM),
     (CONSTANTINOPLE_ROPSTEN_BLOCK, ConstantinopleVM),
     (PETERSBURG_ROPSTEN_BLOCK, PetersburgVM),
     (ISTANBUL_ROPSTEN_BLOCK, IstanbulVM),
     (MUIR_GLACIER_ROPSTEN_BLOCK, MuirGlacierVM),
     (BERLIN_ROPSTEN_BLOCK, BerlinVM),
 )
 
 
 class BaseRopstenChain:
     vm_configuration: Tuple[
-        Tuple[BlockNumber, Type[VirtualMachineAPI]],
-        ...
+        Tuple[BlockNumber, Type[VirtualMachineAPI]], ...
     ] = ROPSTEN_VM_CONFIGURATION
     chain_id: int = ROPSTEN_CHAIN_ID
 
 
 class RopstenChain(BaseRopstenChain, Chain):
     pass
 
 
 ROPSTEN_GENESIS_HEADER = BlockHeader(
     difficulty=1048576,
-    extra_data=decode_hex("0x3535353535353535353535353535353535353535353535353535353535353535"),
+    extra_data=decode_hex(
+        "0x3535353535353535353535353535353535353535353535353535353535353535"
+    ),
     gas_limit=16777216,
     gas_used=0,
     bloom=0,
     mix_hash=constants.ZERO_HASH32,
     nonce=constants.GENESIS_NONCE,
     block_number=constants.GENESIS_BLOCK_NUMBER,
     parent_hash=constants.ZERO_HASH32,
     receipt_root=constants.BLANK_ROOT_HASH,
     uncles_hash=constants.EMPTY_UNCLE_HASH,
-    state_root=decode_hex("0x217b0bbcfb72e2d57e28f33cb361b9983513177755dc3f33ce3e7022ed62b77b"),
+    state_root=decode_hex(
+        "0x217b0bbcfb72e2d57e28f33cb361b9983513177755dc3f33ce3e7022ed62b77b"
+    ),
     timestamp=0,
     transaction_root=constants.BLANK_ROOT_HASH,
 )
```

### Comparing `py-evm-0.7.0a1/eth/chains/ropsten/constants.py` & `py-evm-0.7.0a2/eth/chains/ropsten/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from eth_typing import BlockNumber
-
+from eth_typing import (
+    BlockNumber,
+)
 
 # https://github.com/ethereum/EIPs/blob/master/EIPS/eip-155.md
 ROPSTEN_CHAIN_ID = 3
 
 # Fork Blocks listed in ascending order
 
 #
```

### Comparing `py-evm-0.7.0a1/eth/chains/tester/__init__.py` & `py-evm-0.7.0a2/eth/chains/tester/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,40 +31,39 @@
     validate_gte,
 )
 from eth.vm.forks.homestead import HomesteadVM
 
 
 class MaintainGasLimitMixin:
     @classmethod
-    def create_header_from_parent(cls,
-                                  parent_header: BlockHeaderAPI,
-                                  **header_params: Any) -> 'MaintainGasLimitMixin':
+    def create_header_from_parent(
+        cls, parent_header: BlockHeaderAPI, **header_params: Any
+    ) -> "MaintainGasLimitMixin":
         """
         Call the parent class method maintaining the same gas_limit as the
         previous block.
         """
         return super().create_header_from_parent(  # type: ignore
-            parent_header,
-            **assoc(header_params, 'gas_limit', parent_header.gas_limit)
+            parent_header, **assoc(header_params, "gas_limit", parent_header.gas_limit)
         )
 
 
 MAINNET_VMS = collections.OrderedDict(
     (vm_class.fork, type(vm_class.__name__, (MaintainGasLimitMixin, vm_class), {}))
-    for _, vm_class
-    in MainnetChain.vm_configuration
+    for _, vm_class in MainnetChain.vm_configuration
 )
 
 ForkStartBlocks = Sequence[Tuple[BlockNumber, Union[str, Type[VirtualMachineAPI]]]]
 VMStartBlock = Tuple[BlockNumber, Type[VirtualMachineAPI]]
 
 
 @to_tuple
-def _generate_vm_configuration(*fork_start_blocks: ForkStartBlocks,
-                               dao_start_block: Union[int, bool] = None) -> Generator[VMStartBlock, None, None]:  # noqa: E501
+def _generate_vm_configuration(
+    *fork_start_blocks: ForkStartBlocks, dao_start_block: Union[int, bool] = None
+) -> Generator[VMStartBlock, None, None]:
     """
     fork_start_blocks should be 2-tuples of (start_block, fork_name_or_vm_class)
 
     dao_start_block determines whether the Homestead fork will support the DAO
     fork and if so, at what block.
 
         - dao_start_block = None: perform the DAO fork at the same block as the
@@ -77,38 +76,33 @@
     if not fork_start_blocks:
         yield (GENESIS_BLOCK_NUMBER, last(MAINNET_VMS.values()))
         return
 
     # Validate that there are no fork names which are not represented in the
     # mainnet chain.
     fork_names = {
-        fork_name for
-        _, fork_name
-        in fork_start_blocks
-        if isinstance(fork_name, str)
+        fork_name for _, fork_name in fork_start_blocks if isinstance(fork_name, str)
     }
-    unknown_forks = sorted(fork_names.difference(
-        MAINNET_VMS.keys()
-    ))
+    unknown_forks = sorted(fork_names.difference(MAINNET_VMS.keys()))
     if unknown_forks:
         raise ValidationError(f"Configuration contains unknown forks: {unknown_forks}")
 
     # Validate that *if* an explicit value was passed in for dao_start_block
     # that the Homestead fork rules are part of the VM configuration.
-    if dao_start_block is not None and 'homestead' not in fork_names:
+    if dao_start_block is not None and "homestead" not in fork_names:
         raise ValidationError(
             "The `dao_start_block` parameter is only valid for the 'homestead' "
             "fork rules.  The 'homestead' VM was not included in the provided "
             "fork configuration"
         )
 
     # If no VM is set to start at block 0, default to the frontier VM
     start_blocks = {start_block for start_block, _ in fork_start_blocks}
     if 0 not in start_blocks:
-        yield GENESIS_BLOCK_NUMBER, MAINNET_VMS['frontier']
+        yield GENESIS_BLOCK_NUMBER, MAINNET_VMS["frontier"]
 
     ordered_fork_start_blocks = sorted(fork_start_blocks, key=operator.itemgetter(0))
 
     # Iterate over the parameters, generating a tuple of 2-tuples in the form:
     # (start_block, vm_class)
     for start_block, fork in ordered_fork_start_blocks:
         if isinstance(fork, type) and issubclass(fork, VirtualMachineAPI):
@@ -118,26 +112,34 @@
         else:
             raise Exception("Invariant: unreachable code path")
 
         if issubclass(vm_class, HomesteadVM):
             if dao_start_block is False:
                 yield (start_block, vm_class.configure(support_dao_fork=False))
             elif dao_start_block is None:
-                yield (start_block, vm_class.configure(_dao_fork_block_number=start_block))
+                yield (
+                    start_block,
+                    vm_class.configure(_dao_fork_block_number=start_block),
+                )
             elif isinstance(dao_start_block, int):
                 validate_gte(dao_start_block, start_block)
-                yield (start_block, vm_class.configure(_dao_fork_block_number=dao_start_block))
+                yield (
+                    start_block,
+                    vm_class.configure(_dao_fork_block_number=dao_start_block),
+                )
             else:
                 raise Exception("Invariant: unreachable code path")
         else:
             yield (start_block, vm_class)
 
 
 class BaseMainnetTesterChain(Chain):
-    vm_configuration: Tuple[Tuple[BlockNumber, Type[VirtualMachineAPI]], ...] = _generate_vm_configuration()  # noqa: E501
+    vm_configuration: Tuple[
+        Tuple[BlockNumber, Type[VirtualMachineAPI]], ...
+    ] = _generate_vm_configuration()
 
 
 class MainnetTesterChain(BaseMainnetTesterChain):
     """
     This class is intended to be used for in-memory test chains.  It
     explicitely bypasses the proof of work validation to allow for instant
     block mining.
@@ -148,17 +150,19 @@
 
     def validate_seal(self, header: BlockHeaderAPI) -> None:
         """
         We don't validate the proof of work seal on the tester chain.
         """
         pass
 
-    def configure_forks(self,
-                        *fork_start_blocks: ForkStartBlocks,
-                        dao_start_block: Union[int, bool] = None) -> None:
+    def configure_forks(
+        self,
+        *fork_start_blocks: ForkStartBlocks,
+        dao_start_block: Union[int, bool] = None,
+    ) -> None:
         """
         On demand configuration of fork rules.  This is a foot gun that if used
         incorrectly could cause weird VM errors.
 
         It should generally only be used on a genesis chain (head block == 0).
         Modifying the fork rules, especially if the modification effects
         existing blocks could result in a broken chain.
```

### Comparing `py-evm-0.7.0a1/eth/consensus/applier.py` & `py-evm-0.7.0a2/eth/consensus/applier.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,25 @@
 from eth.typing import (
     VMFork,
 )
 
 
 class ConsensusApplier(VirtualMachineModifierAPI):
     """
-    This class is used to apply simple types of consensus engines to a series of virtual machines.
+    This class is used to apply simple types of consensus engines to a series of
+    virtual machines.
 
     Note that this *must not* be used for Clique, which has its own modifier
     """
 
     def __init__(self, consensus_class: Type[ConsensusAPI]) -> None:
         self._consensus_class = consensus_class
 
     @to_tuple
     def amend_vm_configuration(self, config: VMConfiguration) -> Iterable[VMFork]:
         """
-        Amend the given ``VMConfiguration`` to operate under the rules of the pre-defined consensus
+        Amend the given ``VMConfiguration`` to operate
+        under the rules of the pre-defined consensus
         """
         for pair in config:
             block_number, vm = pair
             yield block_number, vm.configure(consensus_class=self._consensus_class)
```

### Comparing `py-evm-0.7.0a1/eth/consensus/clique/_utils.py` & `py-evm-0.7.0a2/eth/consensus/clique/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from typing import (
     Iterable,
 )
 
-from eth_keys import keys
-from eth_keys.datatypes import PrivateKey
+from eth_keys import (
+    keys,
+)
+from eth_keys.datatypes import (
+    PrivateKey,
+)
 from eth_typing import (
     Address,
     Hash32,
 )
 from eth_utils import (
+    ValidationError,
     encode_hex,
     to_tuple,
-    ValidationError,
 )
 
-from eth._utils.headers import eth_now
+from eth._utils.headers import (
+    eth_now,
+)
 from eth.abc import (
     BlockHeaderAPI,
 )
 from eth.constants import (
     EMPTY_UNCLE_HASH,
     ZERO_ADDRESS,
     ZERO_HASH32,
@@ -45,35 +51,38 @@
 
     signers_length = len(header.extra_data) - VANITY_LENGTH - SIGNATURE_LENGTH
 
     if signers_length % COMMON_ADDRESS_LENGTH != 0:
         raise ValidationError("Checkpoint header must contain list of signers")
 
     signer_count = int(
-        (len(header.extra_data) - VANITY_LENGTH - SIGNATURE_LENGTH) / COMMON_ADDRESS_LENGTH
+        (len(header.extra_data) - VANITY_LENGTH - SIGNATURE_LENGTH)
+        / COMMON_ADDRESS_LENGTH
     )
 
     for i in range(signer_count):
         yield Address(
-            header.extra_data[VANITY_LENGTH + i * COMMON_ADDRESS_LENGTH:][:COMMON_ADDRESS_LENGTH]
+            header.extra_data[VANITY_LENGTH + i * COMMON_ADDRESS_LENGTH :][
+                :COMMON_ADDRESS_LENGTH
+            ]
         )
 
 
 def get_signature_hash(header: BlockHeaderAPI) -> Hash32:
     """
     Return the hash that is signed by the block producer. It is defined as the hash of
     the ``header`` except that the last 65 bytes of the ``extra_data`` (the signature)
     are removed before calculating the hash.
     """
 
     if len(header.extra_data) < SIGNATURE_LENGTH:
         raise ValueError("header.extra_data too short to contain signature")
 
     signature_header: BlockHeaderAPI = header.copy(
-        extra_data=header.extra_data[:len(header.extra_data) - SIGNATURE_LENGTH]
+        extra_data=header.extra_data[: len(header.extra_data) - SIGNATURE_LENGTH]
     )
     return signature_header.hash
 
 
 def get_block_signer(header: BlockHeaderAPI) -> Address:
     """
     Return the address of the signer of the ``header``.
@@ -81,15 +90,17 @@
 
     signature_hash = get_signature_hash(header)
 
     signature_bytes = header.extra_data[-SIGNATURE_LENGTH:]
 
     signature = keys.Signature(signature_bytes=signature_bytes)
 
-    return signature.recover_public_key_from_msg_hash(signature_hash).to_canonical_address()
+    return signature.recover_public_key_from_msg_hash(
+        signature_hash
+    ).to_canonical_address()
 
 
 def is_in_turn(signer: Address, snapshot: Snapshot, header: BlockHeaderAPI) -> bool:
     """
     Return ``True`` if the block was produced *in turn*, otherwise return ``False``.
     """
     sorted_signers = snapshot.get_sorted_signers()
@@ -98,39 +109,40 @@
         offset = sorted_signers.index(signer)
     except ValueError:
         return False
     else:
         return header.block_number % len(sorted_signers) == offset
 
 
-def sign_block_header(header: BlockHeaderAPI, private_key: PrivateKey) -> BlockHeaderAPI:
+def sign_block_header(
+    header: BlockHeaderAPI, private_key: PrivateKey
+) -> BlockHeaderAPI:
     signature_hash = get_signature_hash(header)
     signature = private_key.sign_msg_hash(signature_hash)
     signers = get_signers_at_checkpoint(header)
 
-    signed_extra_data = b''.join((
-        header.extra_data[:VANITY_LENGTH],
-        b''.join(signers),
-        signature.to_bytes(),
-    ))
-
-    return header.copy(
-        extra_data=signed_extra_data
+    signed_extra_data = b"".join(
+        (
+            header.extra_data[:VANITY_LENGTH],
+            b"".join(signers),
+            signature.to_bytes(),
+        )
     )
 
+    return header.copy(extra_data=signed_extra_data)
+
 
 def is_checkpoint(block_number: int, epoch_length: int) -> bool:
     """
     Return ``True`` if the given ``block_number`` is a checkpoint, otherwise ``False``.
     """
     return block_number % epoch_length == 0
 
 
 def validate_header_integrity(header: BlockHeaderAPI, epoch_length: int) -> None:
-
     if header.timestamp > eth_now():
         raise ValidationError(f"Invalid future timestamp: {header.timestamp}")
 
     at_checkpoint = is_checkpoint(header.block_number, epoch_length)
 
     if at_checkpoint and header.coinbase != ZERO_ADDRESS:
         raise ValidationError(
```

### Comparing `py-evm-0.7.0a1/eth/consensus/clique/clique.py` & `py-evm-0.7.0a2/eth/consensus/clique/clique.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,138 +1,145 @@
 import logging
 from typing import (
     Iterable,
     Sequence,
 )
 
-from eth.abc import (
-    AtomicDatabaseAPI,
-    BlockHeaderAPI,
-    VirtualMachineAPI,
-    VirtualMachineModifierAPI,
-)
-from eth.db.chain import ChainDB
-
 from eth_typing import (
     Address,
 )
 from eth_utils import (
+    ValidationError,
     encode_hex,
     to_tuple,
-    ValidationError,
 )
 
 from eth.abc import (
+    AtomicDatabaseAPI,
+    BlockHeaderAPI,
     ConsensusAPI,
     ConsensusContextAPI,
+    VirtualMachineAPI,
+    VirtualMachineModifierAPI,
+)
+from eth.db.chain import (
+    ChainDB,
 )
 from eth.typing import (
     HeaderParams,
     VMConfiguration,
     VMFork,
 )
 
+from ._utils import (
+    get_block_signer,
+    is_in_turn,
+    validate_header_integrity,
+)
 from .constants import (
     EPOCH_LENGTH,
 )
 from .datatypes import (
     Snapshot,
 )
-from .snapshot_manager import SnapshotManager
-from ._utils import (
-    get_block_signer,
-    is_in_turn,
-    validate_header_integrity,
+from .snapshot_manager import (
+    SnapshotManager,
 )
 
 
-def configure_header(vm: VirtualMachineAPI, **header_params: HeaderParams) -> BlockHeaderAPI:
+def configure_header(
+    vm: VirtualMachineAPI, **header_params: HeaderParams
+) -> BlockHeaderAPI:
     with vm.get_header().build_changeset(**header_params) as changeset:
-        # We do this because the default `configure_header` tries to compute the difficulty
-        # which we can not do at this point. We take the `difficulty` as provided and rely
-        # on the `validate_seal` call that will happen as the last step when blocks are
-        # imported.
+        # We do this because the default `configure_header` tries to compute the
+        # difficulty which we can not do at this point. We take the `difficulty` as
+        # provided and rely on the `validate_seal` call that will happen as the last
+        # step when blocks are imported.
         header = changeset.commit()
     return header
 
 
-def _construct_turn_error_message(expected_difficulty: int,
-                                  header: BlockHeaderAPI,
-                                  signer: Address,
-                                  signers: Sequence[Address]) -> str:
-
+def _construct_turn_error_message(
+    expected_difficulty: int,
+    header: BlockHeaderAPI,
+    signer: Address,
+    signers: Sequence[Address],
+) -> str:
     return (
         f"Expected difficulty of {header} to be {expected_difficulty} "
         f"but was {header.difficulty}.\n"
         f"Header signer: {encode_hex(signer)}. Valid signers: {signers}"
     )
 
 
 class CliqueConsensusContext(ConsensusContextAPI):
-
     epoch_length = EPOCH_LENGTH
 
     def __init__(self, db: AtomicDatabaseAPI):
         self.db = db
         self.snapshot_manager = SnapshotManager(ChainDB(db), self.epoch_length)
 
 
 class CliqueConsensus(ConsensusAPI):
     """
-    This class is the entry point to operate a chain under the rules of Clique consensus which
-    is defined in EIP-225: https://eips.ethereum.org/EIPS/eip-225
+    This class is the entry point to operate a chain under the rules of Clique consensus
+    which is defined in EIP-225: https://eips.ethereum.org/EIPS/eip-225
     """
 
-    logger = logging.getLogger('eth.consensus.clique.CliqueConsensus')
+    logger = logging.getLogger("eth.consensus.clique.CliqueConsensus")
 
     def __init__(self, context: CliqueConsensusContext) -> None:
         if context is None:
             raise ValueError("Can not instantiate without `context`")
         self._epoch_length = context.epoch_length
         self._snapshot_manager = context.snapshot_manager
 
     @classmethod
     def get_fee_recipient(cls, header: BlockHeaderAPI) -> Address:
         """
-        If the ``header`` has a signer, return the signer, otherwise return the ``coinbase``
-        of the passed header.
+        If the ``header`` has a signer, return the signer, otherwise return the
+        ``coinbase`` of the passed header.
         """
         try:
             return get_block_signer(header)
         except ValueError:
             return header.coinbase
 
     def get_snapshot(self, header: BlockHeaderAPI) -> Snapshot:
         """
         Retrieve the ``Snapshot`` for the given ``header``.
         """
-        return self._snapshot_manager.get_or_create_snapshot(header.block_number, header.hash)
+        return self._snapshot_manager.get_or_create_snapshot(
+            header.block_number, header.hash
+        )
 
     def validate_seal(self, header: BlockHeaderAPI) -> None:
         """
-        Only validate the integrity of the header, use `validate_seal_extension` to validate
-        the consensus relevant seal of the header.
+        Only validate the integrity of the header, use `validate_seal_extension`
+        to validate the consensus relevant seal of the header.
         """
         validate_header_integrity(header, self._epoch_length)
 
-    def validate_seal_extension(self,
-                                header: BlockHeaderAPI,
-                                parents: Iterable[BlockHeaderAPI]) -> None:
+    def validate_seal_extension(
+        self, header: BlockHeaderAPI, parents: Iterable[BlockHeaderAPI]
+    ) -> None:
         """
-        Validate the seal of the given ``header`` according to the Clique consensus rules.
+        Validate the seal of the given ``header`` according
+        to the Clique consensus rules.
         """
 
         if header.block_number == 0:
             return
 
         validate_header_integrity(header, self._epoch_length)
 
         signer = get_block_signer(header)
         snapshot = self._snapshot_manager.get_or_create_snapshot(
-            header.block_number - 1, header.parent_hash, parents)
+            header.block_number - 1, header.parent_hash, parents
+        )
         in_turn = is_in_turn(signer, snapshot, header)
 
         authorized_signers = snapshot.get_sorted_signers()
 
         if in_turn and header.difficulty != 2:
             raise ValidationError(
                 _construct_turn_error_message(2, header, signer, authorized_signers)
@@ -149,21 +156,23 @@
                 f"Failed to validate {header}."
                 f"Signer {encode_hex(signer)} not in {authorized_signers}"
             )
 
 
 class CliqueApplier(VirtualMachineModifierAPI):
     """
-    This class is used to apply a clique consensus engine to a series of virtual machines
+    This class is used to apply a clique consensus engine
+    to a series of virtual machines
     """
 
     @to_tuple
     def amend_vm_configuration(self, config: VMConfiguration) -> Iterable[VMFork]:
         """
-        Amend the given ``VMConfiguration`` to operate under the rules of Clique consensus.
+        Amend the given ``VMConfiguration`` to operate
+        under the rules of Clique consensus.
         """
         for pair in config:
             block_number, vm = pair
             vm_class = vm.configure(
                 extra_data_max_bytes=65535,
                 consensus_class=CliqueConsensus,
                 configure_header=configure_header,
```

### Comparing `py-evm-0.7.0a1/eth/consensus/clique/datatypes.py` & `py-evm-0.7.0a2/eth/consensus/clique/datatypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from enum import (
-    Enum
+    Enum,
 )
 from typing import (
     Dict,
     FrozenSet,
     List,
     NamedTuple,
     Sequence,
 )
 
 from eth_typing import (
     Address,
-    Hash32
+    Hash32,
 )
 from eth_utils import (
     ValidationError,
 )
 
 from .constants import (
     NONCE_AUTH,
-    NONCE_DROP
+    NONCE_DROP,
 )
 
 
 class VoteAction(Enum):
     """
     The action that is being voted on (nominate or kick).
     """
 
-    # Using the byte representation rather than auto() makes serialization more convenient
+    # Using the byte representation rather than auto()
+    # makes serialization more convenient
     NOMINATE = NONCE_AUTH
     KICK = NONCE_DROP
 
-    def validate_for(self,
-                     signers: Sequence[Address],
-                     subject: Address) -> None:
+    def validate_for(self, signers: Sequence[Address], subject: Address) -> None:
         """
-        Check if a vote action is semantically valid, meaning it is either voting against
-        an existing member or voting in favor of an address that is not yet a member.
+        Check if a vote action is semantically valid, meaning it is either voting
+        against an existing member or voting in favor of an address that is not
+        yet a member.
         """
         signer_exists = subject in signers
         signer_is_kicked = signer_exists and self is VoteAction.KICK
         signer_is_nominated = not signer_exists and self is VoteAction.NOMINATE
 
         if not signer_is_kicked and not signer_is_nominated:
             raise ValidationError(
@@ -50,76 +50,81 @@
             )
 
 
 class Tally(NamedTuple):
     """
     Represent a tally to track votes on new members getting signed in or out.
     """
+
     action: VoteAction
     votes: int = 0
 
-    def upvote(self) -> 'Tally':
+    def upvote(self) -> "Tally":
         return Tally(self.action, self.votes + 1)
 
-    def downvote(self) -> 'Tally':
+    def downvote(self) -> "Tally":
         return Tally(self.action, self.votes - 1)
 
 
 class Vote(NamedTuple):
     """
     Represent a vote (nominate/kick) from a signer regarding a subject.
     """
+
     signer: Address
     block_number: int
     subject: Address
     action: VoteAction
 
 
 class Snapshot(NamedTuple):
     """
     Represent the current state of the consensus at a given time. This
     includes all current signers, all current votes as well at all tallies.
     """
+
     signers: FrozenSet[Address]
     block_hash: Hash32
     votes: FrozenSet[Vote]
-    # Unfortunatly there's no FrozenDict but at least Address and Tally are both immutable
+    # Unfortunately there's no FrozenDict but at least Address and Tally
+    # are both immutable
     tallies: Dict[Address, Tally]
 
-    def get_mutable_clone(self, block_hash: Hash32) -> 'MutableSnapshot':
+    def get_mutable_clone(self, block_hash: Hash32) -> "MutableSnapshot":
         """
-        Return a ``MutableSnapshot`` snapshot clone that can be used as a work in progress
-        representation of the snapshot.
+        Return a ``MutableSnapshot`` snapshot clone that can be used as a work in
+        progress representation of the snapshot.
         """
         return MutableSnapshot(
             signers=list(self.signers),
             block_hash=block_hash,
             votes=list(self.votes),
-            tallies=self.tallies.copy()
+            tallies=self.tallies.copy(),
         )
 
     def get_sorted_signers(self) -> List[Address]:
         """
         Return the sorted list of signers.
         """
         return sorted(self.signers)
 
 
 class MutableSnapshot(NamedTuple):
     """
     Like ``Snapshot`` but mutable as a work in progress representation.
     """
+
     signers: List[Address]
     block_hash: Hash32
     votes: List[Vote]
     tallies: Dict[Address, Tally]
 
     def get_immutable_clone(self) -> Snapshot:
         """
         Return a ``Snapshot``, an immutable clone of the mutable snapshot.
         """
         return Snapshot(
             signers=frozenset(self.signers),
             block_hash=self.block_hash,
             votes=frozenset(self.votes),
-            tallies=self.tallies.copy()
+            tallies=self.tallies.copy(),
         )
```

### Comparing `py-evm-0.7.0a1/eth/consensus/clique/encoding.py` & `py-evm-0.7.0a2/eth/consensus/clique/encoding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import rlp
 from typing import (
     Tuple,
 )
 
 from eth_typing import (
     Address,
 )
+import rlp
 
-from eth.rlp.sedes import (
-    uint256,
-)
 from eth.consensus.clique.datatypes import (
     Snapshot,
     Tally,
     Vote,
     VoteAction,
 )
+from eth.rlp.sedes import (
+    uint256,
+)
 
 ADDRESS_TALLY_SEDES = rlp.sedes.List((rlp.sedes.binary, rlp.sedes.binary))
 VOTE_SEDES = rlp.sedes.List(
     (
         rlp.sedes.binary,
         uint256,
         rlp.sedes.binary,
@@ -41,15 +41,18 @@
     return rlp.encode(
         [pair[0], encode_tally(pair[1])],
         sedes=ADDRESS_TALLY_SEDES,
     )
 
 
 def decode_address_tally_pair(pair: bytes) -> Tuple[Address, Tally]:
-    address, tally_bytes, = rlp.decode(
+    (
+        address,
+        tally_bytes,
+    ) = rlp.decode(
         pair,
         sedes=ADDRESS_TALLY_SEDES,
     )
 
     tally = decode_tally(tally_bytes)
 
     return address, tally
@@ -72,15 +75,17 @@
         vote,
         sedes=VOTE_SEDES,
     )
     return Vote(
         signer=signer,
         block_number=block_number,
         subject=subject,
-        action=VoteAction.NOMINATE if action == VoteAction.NOMINATE.value else VoteAction.KICK
+        action=VoteAction.NOMINATE
+        if action == VoteAction.NOMINATE.value
+        else VoteAction.KICK,
     )
 
 
 def encode_snapshot(snapshot: Snapshot) -> bytes:
     return rlp.encode(
         [
             snapshot.block_hash,
@@ -104,15 +109,15 @@
     votes = [decode_vote(vote) for vote in votes_rlp]
     tallies = dict(decode_address_tally_pair(pair) for pair in tallies_rlp)
 
     return Snapshot(
         signers=frozenset(signers),
         block_hash=block_hash,
         votes=frozenset(votes),
-        tallies=tallies
+        tallies=tallies,
     )
 
 
 def encode_tally(tally: Tally) -> bytes:
     return rlp.encode(
         [tally.action.value, tally.votes],
         sedes=TALLY_SEDES,
@@ -121,11 +126,8 @@
 
 def decode_tally(tally: bytes) -> Tally:
     action_binary, votes = rlp.decode(
         tally,
         sedes=TALLY_SEDES,
     )
 
-    return Tally(
-        action=VoteAction(action_binary),
-        votes=votes
-    )
+    return Tally(action=VoteAction(action_binary), votes=votes)
```

### Comparing `py-evm-0.7.0a1/eth/consensus/clique/snapshot_manager.py` & `py-evm-0.7.0a2/eth/consensus/clique/snapshot_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-import lru
-from typing import Iterable
-
-from eth.abc import (
-    BlockHeaderAPI,
-    ChainDatabaseAPI,
-)
-from eth.exceptions import (
-    HeaderNotFound,
+from typing import (
+    Iterable,
 )
 
 from eth_typing import (
     Address,
     Hash32,
 )
 from eth_utils import (
+    ValidationError,
     encode_hex,
     get_extended_debug_logger,
-    ValidationError,
 )
+import lru
 
-from .encoding import (
-    decode_snapshot,
-    encode_snapshot,
+from eth.abc import (
+    BlockHeaderAPI,
+    ChainDatabaseAPI,
 )
-from .exceptions import (
-    SnapshotNotFound,
+from eth.exceptions import (
+    HeaderNotFound,
+)
+
+from ._utils import (
+    get_block_signer,
+    get_signers_at_checkpoint,
+    is_checkpoint,
 )
 from .constants import (
     IN_MEMORY_SNAPSHOTS,
     NONCE_AUTH,
     NONCE_DROP,
 )
 from .datatypes import (
     MutableSnapshot,
     Snapshot,
     Tally,
     Vote,
     VoteAction,
 )
-
-from ._utils import (
-    get_signers_at_checkpoint,
-    get_block_signer,
-    is_checkpoint,
+from .encoding import (
+    decode_snapshot,
+    encode_snapshot,
+)
+from .exceptions import (
+    SnapshotNotFound,
 )
 
 
 def make_snapshot_lookup_key(block_hash: Hash32) -> bytes:
-    return b'block-hash-to-snapshot:%s' % block_hash
+    return b"block-hash-to-snapshot:%s" % block_hash
 
 
 class SnapshotManager:
     """
-    The ``SnapshotManager`` is responsible for managing the snapshots that hold the current
-    state of the consensus engine. It creates new snapshots by applying headers on top of
-    existing snapshots. It comes with APIs to create, persist and retrieve snapshots.
+    The ``SnapshotManager`` is responsible for managing the snapshots that hold the
+    current state of the consensus engine. It creates new snapshots by applying headers
+    on top of existing snapshots. It comes with APIs to create,
+    persist and retrieve snapshots.
     """
 
-    logger = get_extended_debug_logger('eth.consensus.clique.snapshot_manager.SnapshotManager')
+    logger = get_extended_debug_logger(
+        "eth.consensus.clique.snapshot_manager.SnapshotManager"
+    )
 
-    def __init__(self,
-                 chain_db: ChainDatabaseAPI,
-                 epoch_length: int) -> None:
+    def __init__(self, chain_db: ChainDatabaseAPI, epoch_length: int) -> None:
         self._chain_db = chain_db
         self._epoch_length = epoch_length
         self._snapshots = lru.LRU(IN_MEMORY_SNAPSHOTS)
 
-    def _lookup_header(self,
-                       block_hash: Hash32,
-                       parents: Iterable[BlockHeaderAPI]) -> BlockHeaderAPI:
-
+    def _lookup_header(
+        self, block_hash: Hash32, parents: Iterable[BlockHeaderAPI]
+    ) -> BlockHeaderAPI:
         for parent in parents:
             if parent.hash == block_hash:
                 return parent
         try:
             return self._chain_db.get_block_header_by_hash(block_hash)
         except HeaderNotFound:
             raise ValidationError("Unknown ancestor %s", encode_hex(block_hash))
 
-    def _create_snapshot_from_checkpoint_header(self, header: BlockHeaderAPI) -> Snapshot:
+    def _create_snapshot_from_checkpoint_header(
+        self, header: BlockHeaderAPI
+    ) -> Snapshot:
         signers = get_signers_at_checkpoint(header)
         self.logger.debug2("Created snapshot from checkpoint at %s", header)
 
         snapshot = MutableSnapshot(
-            signers=list(signers),
-            block_hash=header.hash,
-            votes=[],
-            tallies={}
+            signers=list(signers), block_hash=header.hash, votes=[], tallies={}
         )
         return self.add_snapshot(snapshot)
 
     def apply(self, current_snapshot: Snapshot, header: BlockHeaderAPI) -> Snapshot:
         """
         Apply the given header on top of the current snapshot to create a new snapshot.
         """
@@ -112,15 +112,15 @@
             action = VoteAction(header.nonce)
 
             if self.cast_vote(snapshot, header.coinbase, action):
                 vote = Vote(
                     signer=signer,
                     block_number=header.block_number,
                     subject=header.coinbase,
-                    action=action
+                    action=action,
                 )
                 snapshot.votes.append(vote)
 
                 tally = snapshot.tallies[header.coinbase]
                 if tally.votes > len(snapshot.signers) / 2:
                     if tally.action is VoteAction.NOMINATE:
                         snapshot.signers.append(header.coinbase)
@@ -132,86 +132,98 @@
 
                     for vote in snapshot.votes.copy():
                         # Discard any pending votes *from* the added or removed member
                         if vote.signer == header.coinbase:
                             if self.retract_vote(snapshot, vote.subject, vote.action):
                                 snapshot.votes.remove(vote)
 
-                        # Discard any pending votes *regarding* the added or removed member
-                        # No need to uncast, the whole tally is going to be removed anyway.
+                        # Discard any pending votes *regarding* the added or
+                        # removed member. No need to uncast, the whole tally is going
+                        # to be removed anyway.
                         if vote.subject == header.coinbase:
                             snapshot.votes.remove(vote)
 
                     snapshot.tallies.pop(header.coinbase)
 
         self.add_snapshot(snapshot)
 
         return snapshot.get_immutable_clone()
 
-    def get_or_create_snapshot(self,
-                               block_number: int,
-                               block_hash: Hash32,
-                               parents: Iterable[BlockHeaderAPI] = ()) -> Snapshot:
+    def get_or_create_snapshot(
+        self,
+        block_number: int,
+        block_hash: Hash32,
+        parents: Iterable[BlockHeaderAPI] = (),
+    ) -> Snapshot:
         """
-        Return a snapshot either by creating or retrieving it or raise a ``ValidationError``
-        if the header does not have a known ancestor.
+        Return a snapshot either by creating or retrieving it or raise a
+        ``ValidationError`` if the header does not have a known ancestor.
         """
         try:
             snapshot = self.get_snapshot(block_number, block_hash)
         except SnapshotNotFound:
             return self.create_snapshot_for(block_hash, parents)
         else:
             return snapshot
 
-    def create_snapshot_for(self,
-                            block_hash: Hash32,
-                            cached_parents: Iterable[BlockHeaderAPI]) -> Snapshot:
+    def create_snapshot_for(
+        self, block_hash: Hash32, cached_parents: Iterable[BlockHeaderAPI]
+    ) -> Snapshot:
         """
         Create a ``Snapshot`` for the given ``block_hash``. This involves traversing
         backwards through the chain of headers to find a suitable base snapshot either
         from memory, on disk or by creating it on the fly from a checkpoint header.
         After we've found a suitable base snapshot, apply all headers from after the
-        base snapshot up to the header of ``block_hash`` to create the requested snapshot.
+        base snapshot up to the header of ``block_hash`` to create the requested
+        snapshot.
         """
         current_header = header = self._lookup_header(block_hash, cached_parents)
 
         if is_checkpoint(header.block_number, self._epoch_length):
             return self._create_snapshot_from_checkpoint_header(current_header)
 
         parents = []
         while True:
             try:
                 new_snapshot = self.get_snapshot(
-                    current_header.block_number, current_header.parent_hash)
+                    current_header.block_number, current_header.parent_hash
+                )
             except SnapshotNotFound:
-                current_header = self._lookup_header(current_header.parent_hash, cached_parents)
+                current_header = self._lookup_header(
+                    current_header.parent_hash, cached_parents
+                )
 
                 if is_checkpoint(current_header.block_number, self._epoch_length):
-                    new_snapshot = self._create_snapshot_from_checkpoint_header(current_header)
+                    new_snapshot = self._create_snapshot_from_checkpoint_header(
+                        current_header
+                    )
                     break
                 else:
                     parents.append(current_header)
             else:
                 break
 
         for parent in reversed(parents):
             new_snapshot = self.apply(new_snapshot, parent)
 
         new_snapshot = self.apply(new_snapshot, header)
 
         if is_checkpoint(header.block_number, self._epoch_length):
-            self.logger.debug2("Persisting checkpoint snapshot at %s", header.block_number)
+            self.logger.debug2(
+                "Persisting checkpoint snapshot at %s", header.block_number
+            )
             self.persist_snapshot(new_snapshot)
 
         return new_snapshot
 
     def get_snapshot(self, block_number: int, block_hash: Hash32) -> Snapshot:
         """
-        Return a ``Snapshot`` if it exists in memory, on-disk or can be computed directly from
-        a header that serves as a checkpoint. Otherwise raise a ``SnapshotNotFound`` error.
+        Return a ``Snapshot`` if it exists in memory, on-disk or can be computed
+        directly from a header that serves as a checkpoint.
+        Otherwise raise a ``SnapshotNotFound`` error.
         """
 
         # We first try to find the snapshot in memory
         if block_hash in self._snapshots:
             return self._snapshots[block_hash]
 
         if is_checkpoint(block_number, self._epoch_length):
@@ -221,28 +233,33 @@
             except SnapshotNotFound:
                 pass
 
             try:
                 # Otherwise, we can retrieve it on the fly
                 header = self._chain_db.get_block_header_by_hash(block_hash)
             except HeaderNotFound:
-                raise SnapshotNotFound(f"Can not get snapshot for {block_hash!r} at {block_number}")
+                raise SnapshotNotFound(
+                    f"Can not get snapshot for {block_hash!r} at {block_number}"
+                )
             else:
                 if header.block_number != block_number:
                     raise SnapshotNotFound(
                         f"Can not get snapshot for {block_hash!r} at {block_number}"
                     )
                 else:
                     return self._create_snapshot_from_checkpoint_header(header)
 
-        raise SnapshotNotFound(f"Can not get snapshot for {block_hash!r} at {block_number}")
+        raise SnapshotNotFound(
+            f"Can not get snapshot for {block_hash!r} at {block_number}"
+        )
 
     def add_snapshot(self, mutable_snapshot: MutableSnapshot) -> Snapshot:
         """
-        Retrieve a ``Snapshot`` from the given ``mutable_snapshot`` and add it to the local cache.
+        Retrieve a ``Snapshot`` from the given ``mutable_snapshot``
+        and add it to the local cache.
         """
         snapshot = mutable_snapshot.get_immutable_clone()
         self._snapshots[snapshot.block_hash] = snapshot
         return snapshot
 
     def persist_snapshot(self, snapshot: Snapshot) -> None:
         """
@@ -250,42 +267,47 @@
         """
         key = make_snapshot_lookup_key(snapshot.block_hash)
         with self._chain_db.db.atomic_batch() as db:
             db[key] = encode_snapshot(snapshot)
 
     def get_snapshot_from_db(self, block_hash: Hash32) -> Snapshot:
         """
-        Retrieve a snapshot from the database. Raise ``SnapshotNotFound`` if it does not exist.
+        Retrieve a snapshot from the database.
+        Raise ``SnapshotNotFound`` if it does not exist.
         """
         key = make_snapshot_lookup_key(block_hash)
         try:
             encoded_key = self._chain_db.db[key]
         except KeyError as e:
             raise SnapshotNotFound(
                 f"Can not get on-disk snapshot for {block_hash!r}"
             ) from e
         else:
             return decode_snapshot(encoded_key)
 
-    def cast_vote(self, snapshot: MutableSnapshot, subject: Address, action: VoteAction) -> bool:
+    def cast_vote(
+        self, snapshot: MutableSnapshot, subject: Address, action: VoteAction
+    ) -> bool:
         """
         Cast a vote on a ``MutableSnapshot``.
         """
         try:
             action.validate_for(snapshot.signers, subject)
         except ValidationError:
             return False
 
         if subject not in snapshot.tallies:
             snapshot.tallies[subject] = Tally(action)
 
         snapshot.tallies[subject] = snapshot.tallies[subject].upvote()
         return True
 
-    def retract_vote(self, snapshot: MutableSnapshot, subject: Address, action: VoteAction) -> bool:
+    def retract_vote(
+        self, snapshot: MutableSnapshot, subject: Address, action: VoteAction
+    ) -> bool:
         """
         Retract a vote on a ``MutableSnapshot``.
         """
         if subject not in snapshot.tallies:
             # Dangling votes are simply dropped
             return True
```

### Comparing `py-evm-0.7.0a1/eth/consensus/noproof.py` & `py-evm-0.7.0a2/eth/consensus/pos.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from typing import (
     Iterable,
 )
+
 from eth.abc import (
     AtomicDatabaseAPI,
     BlockHeaderAPI,
     ConsensusAPI,
 )
 from eth.typing import (
     Address,
 )
 
 
-class NoProofConsensus(ConsensusAPI):
+class PosConsensus(ConsensusAPI):
     """
-    Modify a set of VMs to accept blocks without any validation.
+    Proof of Stake (PoS) consensus is not achieved in the execution layer (EL).
+    This consensus class basically implements the same rules as ``NoProofConsensus``
+    but with a more proper distinction.
     """
 
     def __init__(self, base_db: AtomicDatabaseAPI) -> None:
         pass
 
     def validate_seal(self, header: BlockHeaderAPI) -> None:
         pass
 
-    def validate_seal_extension(self,
-                                header: BlockHeaderAPI,
-                                parents: Iterable[BlockHeaderAPI]) -> None:
+    def validate_seal_extension(
+        self, header: BlockHeaderAPI, parents: Iterable[BlockHeaderAPI]
+    ) -> None:
         pass
 
     @classmethod
     def get_fee_recipient(cls, header: BlockHeaderAPI) -> Address:
         return header.coinbase
```

### Comparing `py-evm-0.7.0a1/eth/consensus/pos.py` & `py-evm-0.7.0a2/eth/consensus/noproof.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from typing import (
     Iterable,
 )
+
 from eth.abc import (
     AtomicDatabaseAPI,
     BlockHeaderAPI,
     ConsensusAPI,
 )
 from eth.typing import (
     Address,
 )
 
 
-class PosConsensus(ConsensusAPI):
+class NoProofConsensus(ConsensusAPI):
     """
-    Proof of Stake (PoS) consensus is not achieved in the execution layer (EL).
-    This consensus class basically implements the same rules as ``NoProofConsensus``
-    but with a more proper distinction.
+    Modify a set of VMs to accept blocks without any validation.
     """
 
     def __init__(self, base_db: AtomicDatabaseAPI) -> None:
         pass
 
     def validate_seal(self, header: BlockHeaderAPI) -> None:
         pass
 
     def validate_seal_extension(
-        self,
-        header: BlockHeaderAPI,
-        parents: Iterable[BlockHeaderAPI]
+        self, header: BlockHeaderAPI, parents: Iterable[BlockHeaderAPI]
     ) -> None:
         pass
 
     @classmethod
     def get_fee_recipient(cls, header: BlockHeaderAPI) -> Address:
         return header.coinbase
```

### Comparing `py-evm-0.7.0a1/eth/consensus/pow.py` & `py-evm-0.7.0a2/eth/consensus/pow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-from collections import OrderedDict
+from collections import (
+    OrderedDict,
+)
 from typing import (
     Iterable,
     Tuple,
 )
 
+from eth_hash.auto import (
+    keccak,
+)
 from eth_typing import (
     Address,
     Hash32,
 )
-
 from eth_utils import (
-    big_endian_to_int,
     ValidationError,
+    big_endian_to_int,
     encode_hex,
 )
-
-from eth_hash.auto import keccak
-
 from pyethash import (
     EPOCH_LENGTH,
     hashimoto_light,
     mkcache_bytes,
 )
 
-
 from eth.abc import (
     AtomicDatabaseAPI,
     BlockHeaderAPI,
     ConsensusAPI,
 )
 from eth.validation import (
     validate_length,
     validate_lte,
 )
 
-
 # Type annotation here is to ensure we don't accidentally use strings instead of bytes.
-cache_by_epoch: 'OrderedDict[int, bytearray]' = OrderedDict()
+cache_by_epoch: "OrderedDict[int, bytearray]" = OrderedDict()
 CACHE_MAX_ITEMS = 10
 
 
 def get_cache(block_number: int) -> bytes:
     epoch_index = block_number // EPOCH_LENGTH
 
     # doing explicit caching, because functools.lru_cache is 70% slower in the tests
@@ -59,48 +58,53 @@
     # Limit memory usage for cache
     if len(cache_by_epoch) > CACHE_MAX_ITEMS:
         cache_by_epoch.popitem(last=False)  # remove last recently accessed
 
     return c
 
 
-def check_pow(block_number: int,
-              mining_hash: Hash32,
-              mix_hash: Hash32,
-              nonce: bytes,
-              difficulty: int) -> None:
+def check_pow(
+    block_number: int,
+    mining_hash: Hash32,
+    mix_hash: Hash32,
+    nonce: bytes,
+    difficulty: int,
+) -> None:
     validate_length(mix_hash, 32, title="Mix Hash")
     validate_length(mining_hash, 32, title="Mining Hash")
     validate_length(nonce, 8, title="POW Nonce")
     cache = get_cache(block_number)
     mining_output = hashimoto_light(
-        block_number, cache, mining_hash, big_endian_to_int(nonce))
-    if mining_output[b'mix digest'] != mix_hash:
+        block_number, cache, mining_hash, big_endian_to_int(nonce)
+    )
+    if mining_output[b"mix digest"] != mix_hash:
         raise ValidationError(
             f"mix hash mismatch; expected: {encode_hex(mining_output[b'mix digest'])} "
             f"!= actual: {encode_hex(mix_hash)}. "
             f"Mix hash calculated from block #{block_number}, "
             f"mine hash {encode_hex(mining_hash)}, nonce {encode_hex(nonce)}"
             f", difficulty {difficulty}, cache hash {encode_hex(keccak(cache))}"
         )
-    result = big_endian_to_int(mining_output[b'result'])
+    result = big_endian_to_int(mining_output[b"result"])
     validate_lte(result, 2**256 // difficulty, title="POW Difficulty")
 
 
 MAX_TEST_MINE_ATTEMPTS = 1000
 
 
-def mine_pow_nonce(block_number: int, mining_hash: Hash32, difficulty: int) -> Tuple[bytes, bytes]:
+def mine_pow_nonce(
+    block_number: int, mining_hash: Hash32, difficulty: int
+) -> Tuple[bytes, bytes]:
     cache = get_cache(block_number)
     for nonce in range(MAX_TEST_MINE_ATTEMPTS):
         mining_output = hashimoto_light(block_number, cache, mining_hash, nonce)
-        result = big_endian_to_int(mining_output[b'result'])
+        result = big_endian_to_int(mining_output[b"result"])
         result_cap = 2**256 // difficulty
         if result <= result_cap:
-            return nonce.to_bytes(8, 'big'), mining_output[b'mix digest']
+            return nonce.to_bytes(8, "big"), mining_output[b"mix digest"]
 
     raise Exception("Too many attempts at POW mining, giving up")
 
 
 class PowConsensus(ConsensusAPI):
     """
     Modify a set of VMs to validate blocks via Proof of Work (POW)
@@ -110,20 +114,24 @@
         pass
 
     def validate_seal(self, header: BlockHeaderAPI) -> None:
         """
         Validate the seal on the given header by checking the proof of work.
         """
         check_pow(
-            header.block_number, header.mining_hash,
-            header.mix_hash, header.nonce, header.difficulty)
+            header.block_number,
+            header.mining_hash,
+            header.mix_hash,
+            header.nonce,
+            header.difficulty,
+        )
 
-    def validate_seal_extension(self,
-                                header: BlockHeaderAPI,
-                                parents: Iterable[BlockHeaderAPI]) -> None:
+    def validate_seal_extension(
+        self, header: BlockHeaderAPI, parents: Iterable[BlockHeaderAPI]
+    ) -> None:
         pass
 
     @classmethod
     def get_fee_recipient(cls, header: BlockHeaderAPI) -> Address:
         """
         Return the ``coinbase`` of the passed ``header`` as the receipient for any
         rewards for the block.
```

### Comparing `py-evm-0.7.0a1/eth/constants.py` & `py-evm-0.7.0a2/eth/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,46 @@
+from typing import (
+    List,
+    Optional,
+)
+
 from eth_typing import (
     Address,
     BlockNumber,
     Hash32,
 )
-from typing import (
-    List,
-    Optional,
+
+from eth._warnings import (
+    catch_and_ignore_import_warning,
 )
 
-from eth._warnings import catch_and_ignore_import_warning
 with catch_and_ignore_import_warning():
-    from eth_utils import denoms
+    from eth_utils import (
+        denoms,
+    )
 
 
-ANY = 'any'
-UINT256 = 'uint256'
-BYTES = 'bytes'
+ANY = "any"
+UINT256 = "uint256"
+BYTES = "bytes"
 
 UINT_256_MAX = 2**256 - 1
 UINT_256_CEILING = 2**256
 UINT_255_MAX = 2**255 - 1
 UINT_255_CEILING = 2**255
 UINT_255_NEGATIVE_ONE = -1 + UINT_256_CEILING
 UINT_64_MAX = 2**64 - 1
-NULL_BYTE = b'\x00'
+NULL_BYTE = b"\x00"
 EMPTY_WORD = NULL_BYTE * 32
 
 UINT_160_CEILING = 2**160
 
-CREATE_CONTRACT_ADDRESS = Address(b'')
-ZERO_ADDRESS = Address(20 * b'\x00')
-ZERO_HASH32 = Hash32(32 * b'\x00')
+CREATE_CONTRACT_ADDRESS = Address(b"")
+ZERO_ADDRESS = Address(20 * b"\x00")
+ZERO_HASH32 = Hash32(32 * b"\x00")
 
 
 #
 # Stack Limit
 #
 STACK_DEPTH_LIMIT = 1024
 
@@ -107,15 +113,15 @@
 
 #
 # Gas Limit
 #
 GAS_LIMIT_EMA_DENOMINATOR = 1024
 GAS_LIMIT_ADJUSTMENT_FACTOR = 1024
 GAS_LIMIT_MINIMUM = 5000
-GAS_LIMIT_MAXIMUM = 2 ** 63 - 1
+GAS_LIMIT_MAXIMUM = 2**63 - 1
 
 GAS_LIMIT_USAGE_ADJUSTMENT_NUMERATOR = 3
 GAS_LIMIT_USAGE_ADJUSTMENT_DENOMINATOR = 2
 
 
 #
 # Difficulty
@@ -135,48 +141,60 @@
 MAX_UNCLE_DEPTH = 6
 MAX_UNCLES = 2
 
 #
 # SECPK1N
 #
 SECPK1_P = 2**256 - 2**32 - 977
-SECPK1_N = 115792089237316195423570985008687907852837564279074904382605163141518161494337
+SECPK1_N = (
+    115792089237316195423570985008687907852837564279074904382605163141518161494337
+)
 SECPK1_A = 0
 SECPK1_B = 7
-SECPK1_Gx = 55066263022277343669578718895168534326250603453777594175500187360389116729240
-SECPK1_Gy = 32670510020758816978083085130507043184471273380659243275938904335757337482424
+SECPK1_Gx = (
+    55066263022277343669578718895168534326250603453777594175500187360389116729240
+)
+SECPK1_Gy = (
+    32670510020758816978083085130507043184471273380659243275938904335757337482424
+)
 SECPK1_G = (SECPK1_Gx, SECPK1_Gy)
 
 
 #
 # Block and Header
 #
 # keccak(rlp.encode([]))
-EMPTY_UNCLE_HASH = Hash32(b'\x1d\xccM\xe8\xde\xc7]z\xab\x85\xb5g\xb6\xcc\xd4\x1a\xd3\x12E\x1b\x94\x8at\x13\xf0\xa1B\xfd@\xd4\x93G')  # noqa: E501
+EMPTY_UNCLE_HASH = Hash32(
+    b"\x1d\xccM\xe8\xde\xc7]z\xab\x85\xb5g\xb6\xcc\xd4\x1a\xd3\x12E\x1b\x94\x8at\x13\xf0\xa1B\xfd@\xd4\x93G"  # noqa: E501
+)
 
 
 #
 # Genesis Data
 #
 GENESIS_BLOCK_NUMBER = BlockNumber(0)
 GENESIS_DIFFICULTY = 17179869184
 GENESIS_GAS_LIMIT = 5000
 GENESIS_PARENT_HASH = ZERO_HASH32
 GENESIS_COINBASE = ZERO_ADDRESS
-GENESIS_NONCE = b'\x00\x00\x00\x00\x00\x00\x00B'  # 0x42 encoded as big-endian-integer
+GENESIS_NONCE = b"\x00\x00\x00\x00\x00\x00\x00B"  # 0x42 encoded as big-endian-integer
 GENESIS_MIX_HASH = ZERO_HASH32
-GENESIS_EXTRA_DATA = b''
+GENESIS_EXTRA_DATA = b""
 GENESIS_BLOOM = 0
 GENESIS_GAS_USED = 0
 
 #
 # Sha3 Keccak
 #
-EMPTY_SHA3 = Hash32(b"\xc5\xd2F\x01\x86\xf7#<\x92~}\xb2\xdc\xc7\x03\xc0\xe5\x00\xb6S\xca\x82';\x7b\xfa\xd8\x04]\x85\xa4p")  # noqa: E501
-BLANK_ROOT_HASH = Hash32(b'V\xe8\x1f\x17\x1b\xccU\xa6\xff\x83E\xe6\x92\xc0\xf8n\x5bH\xe0\x1b\x99l\xad\xc0\x01b/\xb5\xe3c\xb4!')  # noqa: E501
+EMPTY_SHA3 = Hash32(
+    b"\xc5\xd2F\x01\x86\xf7#<\x92~}\xb2\xdc\xc7\x03\xc0\xe5\x00\xb6S\xca\x82';\x7b\xfa\xd8\x04]\x85\xa4p"  # noqa: E501
+)
+BLANK_ROOT_HASH = Hash32(
+    b"V\xe8\x1f\x17\x1b\xccU\xa6\xff\x83E\xe6\x92\xc0\xf8n\x5bH\xe0\x1b\x99l\xad\xc0\x01b/\xb5\xe3c\xb4!"  # noqa: E501
+)
 
 
 GAS_MOD_EXP_QUADRATIC_DENOMINATOR = 20
 
 #
 # BLOCKHASH opcode maximum depth
 #
```

### Comparing `py-evm-0.7.0a1/eth/db/__init__.py` & `py-evm-0.7.0a2/eth/db/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import os
-from typing import (
-    Any,
-    Type,
-    cast
-)
+from typing import Any, Type, cast
 
 from eth_utils import import_string
 
 from eth.abc import AtomicDatabaseAPI
 
 
-DEFAULT_DB_BACKEND = 'eth.db.atomic.AtomicDB'
+DEFAULT_DB_BACKEND = "eth.db.atomic.AtomicDB"
 
 
 def get_db_backend_class(import_path: str = None) -> Type[AtomicDatabaseAPI]:
     if import_path is None:
         import_path = os.environ.get(
-            'CHAIN_DB_BACKEND_CLASS',
+            "CHAIN_DB_BACKEND_CLASS",
             DEFAULT_DB_BACKEND,
         )
     return cast(Type[AtomicDatabaseAPI], import_string(import_path))
 
 
 def get_db_backend(import_path: str = None, **init_kwargs: Any) -> AtomicDatabaseAPI:
     backend_class = get_db_backend_class(import_path)
```

### Comparing `py-evm-0.7.0a1/eth/db/accesslog.py` & `py-evm-0.7.0a2/eth/db/accesslog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-from contextlib import contextmanager
+from contextlib import (
+    contextmanager,
+)
 import logging
 from typing import (
-    Iterator,
     FrozenSet,
+    Iterator,
     Set,
 )
 
 from eth.abc import (
-    AtomicWriteBatchAPI,
     AtomicDatabaseAPI,
+    AtomicWriteBatchAPI,
     DatabaseAPI,
 )
-from eth.db.backends.base import (
-    BaseDB,
-)
 from eth.db.atomic import (
     BaseAtomicDB,
 )
+from eth.db.backends.base import (
+    BaseDB,
+)
 
 
 class KeyAccessLoggerDB(BaseDB):
     """
-    Wraps around a database, and tracks all the keys that were read since initialization.
+    Wraps around a database and tracks all the keys that were read since initialization.
     """
 
     logger = logging.getLogger("eth.db.KeyAccessLoggerDB")
 
     def __init__(self, wrapped_db: DatabaseAPI, log_missing_keys: bool = True) -> None:
         """
         :param log_missing_keys: True if a key is added to :attr:`keys_read` even if the
@@ -62,19 +64,23 @@
         if does_exist or self._log_missing_keys:
             self._keys_read.add(key)
         return does_exist
 
 
 class KeyAccessLoggerAtomicDB(BaseAtomicDB):
     """
-    Wraps around an atomic database, and tracks all the keys that were read since initialization.
+    Wraps around an atomic database and tracks all the keys
+    that were read since initialization.
     """
+
     logger = logging.getLogger("eth.db.KeyAccessLoggerAtomicDB")
 
-    def __init__(self, wrapped_db: AtomicDatabaseAPI, log_missing_keys: bool = True) -> None:
+    def __init__(
+        self, wrapped_db: AtomicDatabaseAPI, log_missing_keys: bool = True
+    ) -> None:
         """
         :param log_missing_keys: True if a key is added to :attr:`keys_read` even if the
             key/value does not exist in the database.
         """
         self.wrapped_db = wrapped_db
         self._keys_read: Set[bytes] = set()
         self._log_missing_keys = log_missing_keys
```

### Comparing `py-evm-0.7.0a1/eth/db/account.py` & `py-evm-0.7.0a2/eth/db/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-from lru import LRU
 from typing import (
-    cast,
     Dict,
     Iterable,
     Set,
     Tuple,
+    cast,
 )
 
-from eth_hash.auto import keccak
+from eth_hash.auto import (
+    keccak,
+)
 from eth_typing import (
     Address,
-    Hash32
+    Hash32,
 )
-
 from eth_utils import (
+    ValidationError,
     encode_hex,
     get_extended_debug_logger,
     int_to_big_endian,
     to_checksum_address,
     to_dict,
     to_tuple,
-    ValidationError,
+)
+from lru import (
+    LRU,
 )
 import rlp
 from trie import (
     HexaryTrie,
     exceptions as trie_exceptions,
 )
 
@@ -39,70 +42,74 @@
     BLANK_ROOT_HASH,
     EMPTY_SHA3,
 )
 from eth.db.accesslog import (
     KeyAccessLoggerAtomicDB,
     KeyAccessLoggerDB,
 )
+from eth.db.backends.memory import (
+    MemoryDB,
+)
 from eth.db.batch import (
     BatchDB,
 )
 from eth.db.cache import (
     CacheDB,
 )
 from eth.db.diff import (
     DBDiff,
 )
 from eth.db.journal import (
     JournalDB,
 )
-from eth.db.backends.memory import (
-    MemoryDB,
-)
 from eth.db.storage import (
     AccountStorageDB,
 )
 from eth.db.witness import (
     AccountQueryTracker,
     MetaWitness,
 )
-from eth.typing import (
-    JournalDBCheckpoint,
-)
-from eth.vm.interrupt import (
-    MissingAccountTrieNode,
-    MissingBytecode,
-)
 from eth.rlp.accounts import (
     Account,
 )
+from eth.typing import (
+    JournalDBCheckpoint,
+)
 from eth.validation import (
+    validate_canonical_address,
     validate_is_bytes,
     validate_uint256,
-    validate_canonical_address,
+)
+from eth.vm.interrupt import (
+    MissingAccountTrieNode,
+    MissingBytecode,
 )
 
-from .hash_trie import HashTrie
+from .hash_trie import (
+    HashTrie,
+)
 
-IS_PRESENT_VALUE = b''
+IS_PRESENT_VALUE = b""
 
 
 class AccountDB(AccountDatabaseAPI):
-    logger = get_extended_debug_logger('eth.db.account.AccountDB')
+    logger = get_extended_debug_logger("eth.db.account.AccountDB")
 
-    def __init__(self, db: AtomicDatabaseAPI, state_root: Hash32 = BLANK_ROOT_HASH) -> None:
+    def __init__(
+        self, db: AtomicDatabaseAPI, state_root: Hash32 = BLANK_ROOT_HASH
+    ) -> None:
         r"""
         Internal implementation details (subject to rapid change):
         Database entries go through several pipes, like so...
 
         .. code::
 
-            db > _batchdb ---------------------------> _journaldb ----------------> code lookups
+            db > _batchdb ------------------------> _journaldb -----------> code lookups
              \
-              -> _batchtrie -> _trie -> _trie_cache -> _journaltrie --------------> account lookups
+              -> _batchtrie -> _trie -> _trie_cache -> _journaltrie ---> account lookups
 
         Journaling sequesters writes at the _journal* attrs ^, until persist is called.
 
         _batchtrie enables us to prune all trie changes while building
         state,  without deleting old trie roots.
 
         _batchdb and _batchtrie together enable us to make the state root,
@@ -137,15 +144,16 @@
         self._journaltrie = JournalDB(self._trie_cache)
         self._account_cache = LRU(2048)
         self._account_stores: Dict[Address, AccountStorageDatabaseAPI] = {}
         self._dirty_accounts: Set[Address] = set()
         self._root_hash_at_last_persist = state_root
         self._accessed_accounts: Set[Address] = set()
         self._accessed_bytecodes: Set[Address] = set()
-        # Track whether an account or slot have been accessed during a given transaction:
+        # Track whether an account or slot have been accessed
+        # during a given transaction:
         self._reset_access_counters()
 
     @property
     def state_root(self) -> Hash32:
         return self._trie.root_hash
 
     @state_root.setter
@@ -156,15 +164,17 @@
 
     def has_root(self, state_root: bytes) -> bool:
         return state_root in self._batchtrie
 
     #
     # Storage
     #
-    def get_storage(self, address: Address, slot: int, from_journal: bool = True) -> int:
+    def get_storage(
+        self, address: Address, slot: int, from_journal: bool = True
+    ) -> int:
         validate_canonical_address(address, title="Storage Address")
         validate_uint256(slot, title="Storage Slot")
 
         account_store = self._get_address_store(address)
         return account_store.get(slot, from_journal)
 
     def set_storage(self, address: Address, slot: int, value: int) -> None:
@@ -211,15 +221,17 @@
             store = self._account_stores[address]
         else:
             storage_root = self._get_storage_root(address)
             store = AccountStorageDB(self._raw_store_db, storage_root, address)
             self._account_stores[address] = store
         return store
 
-    def _dirty_account_stores(self) -> Iterable[Tuple[Address, AccountStorageDatabaseAPI]]:
+    def _dirty_account_stores(
+        self,
+    ) -> Iterable[Tuple[Address, AccountStorageDatabaseAPI]]:
         for address in self._dirty_accounts:
             store = self._account_stores[address]
             yield address, store
 
     @to_tuple
     def _get_changed_roots(self) -> Iterable[Tuple[Address, Hash32]]:
         # list all the accounts that were changed, and their new storage roots
@@ -231,22 +243,24 @@
         account = self._get_account(address)
         return account.storage_root
 
     def _set_storage_root(self, address: Address, new_storage_root: Hash32) -> None:
         account = self._get_account(address)
         self._set_account(address, account.copy(storage_root=new_storage_root))
 
-    def _validate_flushed_storage(self, address: Address, store: AccountStorageDatabaseAPI) -> None:
+    def _validate_flushed_storage(
+        self, address: Address, store: AccountStorageDatabaseAPI
+    ) -> None:
         if store.has_changed_root:
             actual_storage_root = self._get_storage_root(address)
             expected_storage_root = store.get_changed_root()
             if expected_storage_root != actual_storage_root:
                 raise ValidationError(
-                    "Storage root was not saved to account before trying to persist roots. "
-                    f"Account {address!r} had storage {actual_storage_root!r}, "
+                    "Storage root was not saved to account before trying to persist "
+                    f"roots. Account {address!r} had storage {actual_storage_root!r}, "
                     f"but should be {expected_storage_root!r}."
                 )
 
     #
     # Balance
     #
     def get_balance(self, address: Address) -> int:
@@ -286,15 +300,15 @@
     # Code
     #
     def get_code(self, address: Address) -> bytes:
         validate_canonical_address(address, title="Storage Address")
 
         code_hash = self.get_code_hash(address)
         if code_hash == EMPTY_SHA3:
-            return b''
+            return b""
         else:
             try:
                 return self._journaldb[code_hash]
             except KeyError:
                 raise MissingBytecode(code_hash) from KeyError
             finally:
                 if code_hash in self._get_accessed_node_hashes():
@@ -329,25 +343,26 @@
         return self.get_nonce(address) != 0 or self.get_code_hash(address) != EMPTY_SHA3
 
     def delete_account(self, address: Address) -> None:
         validate_canonical_address(address, title="Storage Address")
 
         # We must wipe the storage first, because if it's the first time we load it,
         #   then we want to load it with the original storage root hash, not the
-        #   empty one. (in case of a later revert, we don't want to poison the storage cache)
+        #   empty one. (in case of a later revert, we don't want to poison the
+        #   storage cache)
         self._wipe_storage(address)
 
         if address in self._account_cache:
             del self._account_cache[address]
         del self._journaltrie[address]
 
     def account_exists(self, address: Address) -> bool:
         validate_canonical_address(address, title="Storage Address")
         account_rlp = self._get_encoded_account(address, from_journal=True)
-        return account_rlp != b''
+        return account_rlp != b""
 
     def touch_account(self, address: Address) -> None:
         validate_canonical_address(address, title="Storage Address")
 
         account = self._get_account(address)
         self._set_account(address, account)
 
@@ -363,25 +378,27 @@
     def mark_address_warm(self, address: Address) -> None:
         if address not in self._journal_accessed_state:
             self._journal_accessed_state[address] = IS_PRESENT_VALUE
 
     #
     # Internal
     #
-    def _get_encoded_account(self, address: Address, from_journal: bool = True) -> bytes:
+    def _get_encoded_account(
+        self, address: Address, from_journal: bool = True
+    ) -> bytes:
         self._accessed_accounts.add(address)
         lookup_trie = self._journaltrie if from_journal else self._trie_cache
 
         try:
             return lookup_trie[address]
         except trie_exceptions.MissingTrieNode as exc:
             raise MissingAccountTrieNode(*exc.args) from exc
         except KeyError:
             # In case the account is deleted in the JournalDB
-            return b''
+            return b""
 
     def _get_account(self, address: Address, from_journal: bool = True) -> Account:
         if from_journal and address in self._account_cache:
             return self._account_cache[address]
 
         rlp_account = self._get_encoded_account(address, from_journal)
 
@@ -397,15 +414,16 @@
         self._account_cache[address] = account
         rlp_account = rlp.encode(account, sedes=Account)
         self._journaltrie[address] = rlp_account
 
     def _reset_access_counters(self) -> None:
         # Account accesses and storage accesses recorded in the same journal
         # Accounts just use the address as the key (and an empty value as a flag)
-        # Storage use a concatenation of address and slot converted to bytes (and empty value)
+        # Storage use a concatenation of address and slot converted to bytes
+        # (and empty value)
         self._journal_accessed_state = JournalDB(MemoryDB())
 
     #
     # Record and discard API
     #
     def record(self) -> JournalDBCheckpoint:
         checkpoint = self._journaldb.record()
@@ -449,16 +467,16 @@
                 )
                 self._set_storage_root(address, storage_root)
 
         self._journaldb.persist()
 
         diff = self._journaltrie.diff()
         if diff.deleted_keys() or diff.pending_items():
-            # In addition to squashing (which is redundant here), this context manager causes
-            # an atomic commit of the changes, so exceptions will revert the trie
+            # In addition to squashing (which is redundant here), this context manager
+            # causes an atomic commit of the changes, so exceptions will revert the trie
             with self._trie.squash_changes() as memory_trie:
                 self._apply_account_diff_without_proof(diff, memory_trie)
 
         self._journaltrie.reset()
         self._trie_cache.reset_cache()
 
         return self.state_root
@@ -511,30 +529,35 @@
 
     def _get_accessed_node_hashes(self) -> Set[Hash32]:
         return cast(Set[Hash32], self._raw_store_db.keys_read)
 
     @to_dict
     def _get_access_list(self) -> Iterable[Tuple[Address, AccountQueryTracker]]:
         """
-        Get the list of addresses that were accessed, whether the bytecode was accessed, and
-        which storage slots were accessed.
+        Get the list of addresses that were accessed, whether the bytecode was accessed,
+        and which storage slots were accessed.
         """
         for address in self._accessed_accounts:
             did_access_bytecode = address in self._accessed_bytecodes
             if address in self._account_stores:
-                accessed_storage_slots = self._account_stores[address].get_accessed_slots()
+                accessed_storage_slots = self._account_stores[
+                    address
+                ].get_accessed_slots()
             else:
                 accessed_storage_slots = frozenset()
-            yield address, AccountQueryTracker(did_access_bytecode, accessed_storage_slots)
+            yield address, AccountQueryTracker(
+                did_access_bytecode, accessed_storage_slots
+            )
 
     def _get_meta_witness(self) -> MetaWitness:
         """
         Get a variety of metadata about the state witness needed to execute the block.
 
-        This creates a copy, so that underlying changes do not affect the returned MetaWitness.
+        This creates a copy, so that underlying changes do not affect the returned
+        MetaWitness.
         """
         return MetaWitness(self._get_accessed_node_hashes(), self._get_access_list())
 
     def _validate_generated_root(self) -> None:
         db_diff = self._journaldb.diff()
         if db_diff:
             raise ValidationError(
@@ -551,36 +574,40 @@
         if not self.logger.show_debug2:
             return
 
         diff = self._journaltrie.diff()
         for address in sorted(diff.pending_keys()):
             account = self._get_account(Address(address))
             self.logger.debug2(
-                "Pending Account %s: balance %d, nonce %d, storage root %s, code hash %s",
+                "Pending Account %s: balance %d, nonce %d, storage root %s, code hash %s",  # noqa: E501
                 to_checksum_address(address),
                 account.balance,
                 account.nonce,
                 encode_hex(account.storage_root),
                 encode_hex(account.code_hash),
             )
         for deleted_address in sorted(diff.deleted_keys()):
-            # Check if the account was accessed before accessing/logging info about the address
+            # Check if the account was accessed before accessing/logging
+            # info about the address
             was_account_accessed = deleted_address in self._accessed_accounts
             cast_deleted_address = Address(deleted_address)
             self.logger.debug2(
                 "Deleted Account %s, empty? %s, exists? %s",
                 to_checksum_address(deleted_address),
                 self.account_is_empty(cast_deleted_address),
                 self.account_exists(cast_deleted_address),
             )
-            # If the account was not accessed previous to the log, (re)mark it as not accessed
+            # If the account was not accessed previous to the log,
+            # (re)mark it as not accessed
             if not was_account_accessed:
                 self._accessed_accounts.remove(cast_deleted_address)
 
-    def _apply_account_diff_without_proof(self, diff: DBDiff, trie: DatabaseAPI) -> None:
+    def _apply_account_diff_without_proof(
+        self, diff: DBDiff, trie: DatabaseAPI
+    ) -> None:
         """
         Apply diff of trie updates, when original nodes might be missing.
         Note that doing this naively will raise exceptions about missing nodes
         from *intermediate* trie roots. This captures exceptions and uses the previous
         trie root hash that will be recognized by other nodes.
         """
         # It's fairly common that when an account is deleted, we need to retrieve nodes
@@ -606,16 +633,18 @@
         #
         # Setup:
         #   - Root node is a branch, with 0 pointing to a leaf
         #   - The complete leaf key is (0, 1, 2), so (1, 2) is in the leaf node
         #   - We know the leaf node hash but not the leaf node body
         # Refactor that triggers missing node:
         #   - Add value with key (0, 3, 4)
-        #   - We need to replace the current leaf node with a branch that points leaves at 1 and 3
-        #   - The leaf for key (0, 1, 2) now contains only the (2) part, so needs to be rebuilt
+        #   - We need to replace the current leaf node with a branch that points leaves
+        #       at 1 and 3
+        #   - The leaf for key (0, 1, 2) now contains only the (2) part, so needs to
+        #       be rebuilt
         #   - We need the full body of the old (1, 2) leaf node, to rebuild
 
         for key, val in diff.pending_items():
             try:
                 trie[key] = val
             except trie_exceptions.MissingTrieNode as exc:
                 self.logger.debug(
```

### Comparing `py-evm-0.7.0a1/eth/db/atomic.py` & `py-evm-0.7.0a2/eth/db/atomic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-from contextlib import contextmanager
+from contextlib import (
+    contextmanager,
+)
 import logging
 from typing import (
     Iterator,
 )
 
 from eth_utils import (
     ValidationError,
 )
 
 from eth.abc import (
     AtomicWriteBatchAPI,
     DatabaseAPI,
 )
-
+from eth.db.backends.base import (
+    BaseAtomicDB,
+    BaseDB,
+)
+from eth.db.backends.memory import (
+    MemoryDB,
+)
 from eth.db.diff import (
     DBDiff,
     DBDiffTracker,
     DiffMissingError,
 )
-from eth.db.backends.base import BaseAtomicDB, BaseDB
-from eth.db.backends.memory import MemoryDB
 
 
 class AtomicDB(BaseAtomicDB):
     logger = logging.getLogger("eth.db.AtomicDB")
 
     wrapped_db: DatabaseAPI = None
     _track_diff: DBDiffTracker = None
@@ -50,17 +56,18 @@
     def atomic_batch(self) -> Iterator[AtomicWriteBatchAPI]:
         with AtomicDBWriteBatch._commit_unless_raises(self) as readable_batch:
             yield readable_batch
 
 
 class AtomicDBWriteBatch(BaseDB, AtomicWriteBatchAPI):
     """
-    This is returned by a BaseAtomicDB during an atomic_batch, to provide a temporary view
-    of the database, before commit.
+    This is returned by a BaseAtomicDB during an atomic_batch, to provide a temporary
+    view of the database, before commit.
     """
+
     logger = logging.getLogger("eth.db.AtomicDBWriteBatch")
 
     _write_target_db: DatabaseAPI = None
     _track_diff: DBDiffTracker = None
 
     def __init__(self, write_target_db: DatabaseAPI) -> None:
         self._write_target_db = write_target_db
@@ -84,45 +91,51 @@
         if self._track_diff is None:
             raise ValidationError("Cannot set data from a write batch, out of context")
 
         self._track_diff[key] = value
 
     def __delitem__(self, key: bytes) -> None:
         if self._track_diff is None:
-            raise ValidationError("Cannot delete data from a write batch, out of context")
+            raise ValidationError(
+                "Cannot delete data from a write batch, out of context"
+            )
 
         if key not in self:
             raise KeyError(key)
         del self._track_diff[key]
 
     def _diff(self) -> DBDiff:
         return self._track_diff.diff()
 
     def _commit(self) -> None:
         self._diff().apply_to(self._write_target_db, apply_deletes=True)
 
     def _exists(self, key: bytes) -> bool:
         if self._track_diff is None:
-            raise ValidationError("Cannot test data existance from a write batch, out of context")
+            raise ValidationError(
+                "Cannot test data existance from a write batch, out of context"
+            )
 
         try:
             self[key]
         except KeyError:
             return False
         else:
             return True
 
     @classmethod
     @contextmanager
-    def _commit_unless_raises(cls, write_target_db: DatabaseAPI) -> Iterator[AtomicWriteBatchAPI]:
+    def _commit_unless_raises(
+        cls, write_target_db: DatabaseAPI
+    ) -> Iterator[AtomicWriteBatchAPI]:
         """
         Commit all writes inside the context, unless an exception was raised.
 
-        Although this is technically an external API, it (and this whole class) is only intended
-        to be used by AtomicDB.
+        Although this is technically an external API, it (and this whole class) is only
+        intended to be used by AtomicDB.
         """
         readable_write_batch: AtomicDBWriteBatch = cls(write_target_db)
         try:
             yield readable_write_batch
         except Exception:
             cls.logger.exception(
                 "Unexpected error in atomic db write, dropped partial writes: %r",
```

### Comparing `py-evm-0.7.0a1/eth/db/backends/base.py` & `py-evm-0.7.0a2/eth/db/backends/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,59 +19,63 @@
 
     All subclasses must implement these methods:
     __init__, __getitem__, __setitem__, __delitem__
 
     Subclasses may optionally implement an _exists method
     that is type-checked for key and value.
     """
+
     def set(self, key: bytes, value: bytes) -> None:
         self[key] = value
 
     def exists(self, key: bytes) -> bool:
         return self.__contains__(key)
 
-    def __contains__(self, key: bytes) -> bool:     # type: ignore # Breaks LSP
-        if hasattr(self, '_exists'):
+    def __contains__(self, key: bytes) -> bool:  # type: ignore # Breaks LSP
+        if hasattr(self, "_exists"):
             # Classes which inherit this class would have `_exists` attr
-            return self._exists(key)    # type: ignore
+            return self._exists(key)  # type: ignore
         else:
             return super().__contains__(key)
 
     def delete(self, key: bytes) -> None:
         try:
             del self[key]
         except KeyError:
             pass
 
     def __iter__(self) -> Iterator[bytes]:
         raise NotImplementedError("By default, DB classes cannot be iterated.")
 
     def __len__(self) -> int:
-        raise NotImplementedError("By default, DB classes cannot return the total number of keys.")
+        raise NotImplementedError(
+            "By default, DB classes cannot return the total number of keys."
+        )
 
 
 class BaseAtomicDB(BaseDB, AtomicDatabaseAPI):
     """
-    This is an abstract key/value lookup that permits batching of updates, such that the batch of
-    changes are atomically saved. They are either all saved, or none are.
+    This is an abstract key/value lookup that permits batching of updates, such that the
+    batch of changes are atomically saved. They are either all saved, or none are.
 
     Writes to the database are immediately saved, unless they are explicitly batched
     in a context, like this:
 
     ::
 
         atomic_db = AtomicDB()
         with atomic_db.atomic_batch() as db:
             # changes are not immediately saved to the db, inside this context
             db[key] = val
 
-            # changes are still locally visible even though they are not yet committed to the db
-            assert db[key] == val
+            # changes are still locally visible even though they are not yet committed
+            to the db assert db[key] == val
 
             if some_bad_condition:
                 raise Exception("something went wrong, erase all the pending changes")
 
             db[key2] = val2
-            # when exiting the context, the values are saved either key and key2 will both be saved,
-            # or neither will
+            # when exiting the context, the values are saved either key and key2 will
+            # both be saved, or neither will
     """
+
     pass
```

### Comparing `py-evm-0.7.0a1/eth/db/backends/level.py` & `py-evm-0.7.0a2/eth/db/backends/level.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,65 @@
-from contextlib import contextmanager
+from contextlib import (
+    contextmanager,
+)
 import logging
-from pathlib import Path
+from pathlib import (
+    Path,
+)
 from typing import (
-    Iterator,
     TYPE_CHECKING,
+    Iterator,
 )
 
-from eth_utils import ValidationError
+from eth_utils import (
+    ValidationError,
+)
 
+from eth._warnings import (
+    catch_and_ignore_import_warning,
+)
 from eth.abc import (
     AtomicWriteBatchAPI,
     DatabaseAPI,
 )
 from eth.db.diff import (
     DBDiffTracker,
     DiffMissingError,
 )
+
 from .base import (
     BaseAtomicDB,
     BaseDB,
 )
 
-from eth._warnings import catch_and_ignore_import_warning
-
 if TYPE_CHECKING:
     with catch_and_ignore_import_warning():
         import plyvel  # noqa: F401
 
 
 class LevelDB(BaseAtomicDB):
     logger = logging.getLogger("eth.db.backends.LevelDB")
 
     # Creates db as a class variable to avoid level db lock error
-    def __init__(self,
-                 db_path: Path = None,
-                 max_open_files: int = None) -> None:
+    def __init__(self, db_path: Path = None, max_open_files: int = None) -> None:
         if not db_path:
             raise TypeError("Please specifiy a valid path for your database.")
         try:
             with catch_and_ignore_import_warning():
                 import plyvel  # noqa: F811
         except ImportError:
             raise ImportError(
                 "LevelDB requires the plyvel library which is not available for import."
             )
         self.db_path = db_path
         self.db = plyvel.DB(
             str(db_path),
             create_if_missing=True,
             error_if_exists=False,
-            max_open_files=max_open_files
+            max_open_files=max_open_files,
         )
 
     def __getitem__(self, key: bytes) -> bytes:
         v = self.db.get(key)
         if v is None:
             raise KeyError(key)
         return v
@@ -81,17 +87,20 @@
 
 class LevelDBWriteBatch(BaseDB, AtomicWriteBatchAPI):
     """
     A native leveldb write batch does not permit reads on the in-progress data.
     This class fills that gap, by tracking the in-progress diff, and adding
     a read interface.
     """
+
     logger = logging.getLogger("eth.db.backends.LevelDBWriteBatch")
 
-    def __init__(self, original_read_db: DatabaseAPI, write_batch: 'plyvel.WriteBatch') -> None:
+    def __init__(
+        self, original_read_db: DatabaseAPI, write_batch: "plyvel.WriteBatch"
+    ) -> None:
         self._original_read_db = original_read_db
         self._write_batch = write_batch
         # keep track of the temporary changes made
         self._track_diff = DBDiffTracker()
 
     def __getitem__(self, key: bytes) -> bytes:
         if self._track_diff is None:
@@ -112,31 +121,36 @@
             raise ValidationError("Cannot set data from a write batch, out of context")
 
         self._write_batch.put(key, value)
         self._track_diff[key] = value
 
     def _exists(self, key: bytes) -> bool:
         if self._track_diff is None:
-            raise ValidationError("Cannot test data existance from a write batch, out of context")
+            raise ValidationError(
+                "Cannot test data existance from a write batch, out of context"
+            )
 
         try:
             self._track_diff[key]
         except DiffMissingError as missing:
             if missing.is_deleted:
                 return False
             else:
                 return key in self._original_read_db
         else:
             return True
 
     def __delitem__(self, key: bytes) -> None:
         if self._track_diff is None:
-            raise ValidationError("Cannot delete data from a write batch, out of context")
+            raise ValidationError(
+                "Cannot delete data from a write batch, out of context"
+            )
 
         self._write_batch.delete(key)
         del self._track_diff[key]
 
     def decommission(self) -> None:
         """
-        Prevent any further actions to be taken on this write batch, called after leaving context
+        Prevent any further actions to be taken on this write batch,
+        called after leaving context
         """
         self._track_diff = None
```

### Comparing `py-evm-0.7.0a1/eth/db/backends/memory.py` & `py-evm-0.7.0a2/eth/db/backends/memory.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a1/eth/db/batch.py` & `py-evm-0.7.0a2/eth/db/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 import logging
 
 from eth_utils import (
     ValidationError,
 )
 
-from eth.abc import DatabaseAPI
+from eth.abc import (
+    DatabaseAPI,
+)
+from eth.db.backends.base import (
+    BaseDB,
+)
 from eth.db.diff import (
     DBDiff,
     DBDiffTracker,
     DiffMissingError,
 )
-from eth.db.backends.base import BaseDB
 
 
 class BatchDB(BaseDB):
     """
     A wrapper of basic DB objects with uncommitted DB changes stored in local cache,
     which represents as a dictionary of database keys and values.
-    This class should be usable as a context manager, the changes either all fail or all succeed.
-    Upon exiting the context, it writes all of the key value pairs from the cache into
-    the underlying database. If any error occurred before committing phase,
+    This class should be usable as a context manager, the changes either all fail or all
+    succeed. Upon exiting the context, it writes all of the key value pairs from the
+    cache into the underlying database. If any error occurred before committing phase,
     we would not apply commits at all.
     """
+
     logger = logging.getLogger("eth.db.BatchDB")
 
     wrapped_db: DatabaseAPI = None
     _track_diff: DBDiffTracker = None
 
-    def __init__(self, wrapped_db: DatabaseAPI, read_through_deletes: bool = False) -> None:
+    def __init__(
+        self, wrapped_db: DatabaseAPI, read_through_deletes: bool = False
+    ) -> None:
         self.wrapped_db = wrapped_db
         self._track_diff = DBDiffTracker()
         self._read_through_deletes = read_through_deletes
 
-    def __enter__(self) -> 'BatchDB':
+    def __enter__(self) -> "BatchDB":
         return self
 
     def __exit__(self, exc_type: None, exc_value: None, traceback: None) -> None:
         # commit all the changes from local cache to underlying db
         if exc_type is None:
             self.commit()
         else:
@@ -47,15 +54,17 @@
         self._track_diff = DBDiffTracker()
 
     def commit(self, apply_deletes: bool = True) -> None:
         self.commit_to(self.wrapped_db, apply_deletes)
 
     def commit_to(self, target_db: DatabaseAPI, apply_deletes: bool = True) -> None:
         if apply_deletes and self._read_through_deletes:
-            raise ValidationError("BatchDB should never apply deletes when reading through deletes")
+            raise ValidationError(
+                "BatchDB should never apply deletes when reading through deletes"
+            )
         diff = self.diff()
         diff.apply_to(target_db, apply_deletes)
         self.clear()
 
     def _exists(self, key: bytes) -> bool:
         try:
             self[key]
```

### Comparing `py-evm-0.7.0a1/eth/db/cache.py` & `py-evm-0.7.0a2/eth/db/cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-from lru import LRU
+from lru import (
+    LRU,
+)
 
-from eth.abc import DatabaseAPI
-from eth.db.backends.base import BaseDB
+from eth.abc import (
+    DatabaseAPI,
+)
+from eth.db.backends.base import (
+    BaseDB,
+)
 
 
 class CacheDB(BaseDB):
     """
     Set and get decoded RLP objects, where the underlying db stores
     encoded objects.
     """
+
     def __init__(self, db: DatabaseAPI, cache_size: int = 2048) -> None:
         self._db = db
         self._cache_size = cache_size
         self.reset_cache()
 
     def reset_cache(self) -> None:
         self._cached_values = LRU(self._cache_size)
```

### Comparing `py-evm-0.7.0a1/eth/db/chain.py` & `py-evm-0.7.0a2/eth/db/chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,90 +1,105 @@
 import functools
 import itertools
-
 from typing import (
     Dict,
     Iterable,
     Sequence,
     Tuple,
     Type,
     cast,
 )
 
-from eth.vm.forks.shanghai.withdrawals import (
-    Withdrawal,
+from eth_hash.auto import (
+    keccak,
 )
 from eth_typing import (
     BlockNumber,
-    Hash32
+    Hash32,
 )
 from eth_utils import (
     encode_hex,
 )
-
-from eth_hash.auto import keccak
 from trie.exceptions import (
     MissingTrieNode,
 )
 
+from eth._warnings import (
+    catch_and_ignore_import_warning,
+)
 from eth.abc import (
+    AtomicDatabaseAPI,
     BlockAPI,
     BlockHeaderAPI,
     ChainDatabaseAPI,
     DatabaseAPI,
-    AtomicDatabaseAPI,
     ReceiptAPI,
     ReceiptDecoderAPI,
     SignedTransactionAPI,
     TransactionDecoderAPI,
     WithdrawalAPI,
 )
 from eth.constants import (
     EMPTY_UNCLE_HASH,
     GENESIS_PARENT_HASH,
 )
 from eth.db.chain_gaps import (
-    fill_gap,
+    GENESIS_CHAIN_GAPS,
     GapChange,
     GapInfo,
-    GENESIS_CHAIN_GAPS,
+    fill_gap,
     is_block_number_in_gap,
     reopen_gap,
 )
-from eth.db.trie import make_trie_root_and_nodes
+from eth.db.header import (
+    HeaderDB,
+)
+from eth.db.schema import (
+    SchemaV1,
+)
+from eth.db.trie import (
+    make_trie_root_and_nodes,
+)
 from eth.exceptions import (
     HeaderNotFound,
     ReceiptNotFound,
     TransactionNotFound,
 )
-from eth.db.header import HeaderDB
-from eth.db.schema import SchemaV1
-from eth.rlp.sedes import chain_gaps
-from eth.typing import ChainGaps
+from eth.rlp.sedes import (
+    chain_gaps,
+)
+from eth.typing import (
+    ChainGaps,
+)
 from eth.validation import (
     validate_word,
 )
-from eth.vm.header import HeaderSedes
-from eth._warnings import catch_and_ignore_import_warning
+from eth.vm.forks.shanghai.withdrawals import (
+    Withdrawal,
+)
+from eth.vm.header import (
+    HeaderSedes,
+)
+
 with catch_and_ignore_import_warning():
+    from eth_utils import (
+        ValidationError,
+        to_tuple,
+    )
     import rlp
     from trie import (
         HexaryTrie,
     )
-    from eth_utils import (
-        to_tuple,
-        ValidationError,
-    )
 
 
 class BlockDataKey(rlp.Serializable):
     # used for transactions and withdrawals
     fields = [
-        ('block_number', rlp.sedes.big_endian_int),
-        ('index', rlp.sedes.big_endian_int),
+        ("block_number", rlp.sedes.big_endian_int),
+        ("index", rlp.sedes.big_endian_int),
     ]
 
 
 class ChainDB(HeaderDB, ChainDatabaseAPI):
     def __init__(self, db: AtomicDatabaseAPI) -> None:
         self.db = db
 
@@ -98,82 +113,80 @@
         except KeyError:
             return GENESIS_CHAIN_GAPS
         else:
             return rlp.decode(encoded_gaps, sedes=chain_gaps)
 
     @classmethod
     def _update_chain_gaps(
-            cls,
-            db: DatabaseAPI,
-            persisted_block: BlockAPI,
-            base_gaps: ChainGaps = None
+        cls, db: DatabaseAPI, persisted_block: BlockAPI, base_gaps: ChainGaps = None
     ) -> GapInfo:
-
         # If we make many updates in a row, we can avoid reloading the integrity info by
         # continuously caching it and providing it as a parameter to this API
         if base_gaps is None:
             base_gaps = cls._get_chain_gaps(db)
 
         gap_change, gaps = fill_gap(persisted_block.number, base_gaps)
         if gap_change is not GapChange.NoChange:
             db.set(
                 SchemaV1.make_chain_gaps_lookup_key(),
-                rlp.encode(gaps, sedes=chain_gaps)
+                rlp.encode(gaps, sedes=chain_gaps),
             )
 
         return gap_change, gaps
 
     @classmethod
     def _update_header_chain_gaps(
-            cls,
-            db: DatabaseAPI,
-            persisting_header: BlockHeaderAPI,
-            base_gaps: ChainGaps = None
+        cls,
+        db: DatabaseAPI,
+        persisting_header: BlockHeaderAPI,
+        base_gaps: ChainGaps = None,
     ) -> GapInfo:
-        # The only reason we overwrite this here is to be able to detect when the HeaderDB
-        # de-canonicalizes an uncle that should cause us to re-open a block gap.
-        gap_change, gaps = super()._update_header_chain_gaps(db, persisting_header, base_gaps)
+        # The only reason we overwrite this here is to be able to detect when the
+        # HeaderDB de-canonicalizes an uncle that should cause us to
+        # re-open a block gap.
+        gap_change, gaps = super()._update_header_chain_gaps(
+            db, persisting_header, base_gaps
+        )
 
         if gap_change is not GapChange.NoChange or persisting_header.block_number == 0:
             return gap_change, gaps
 
         # We have written a header for which block number we've already had a header.
         # This might be a sign of a de-canonicalized uncle.
         current_gaps = cls._get_chain_gaps(db)
         if not is_block_number_in_gap(persisting_header.block_number, current_gaps):
-            # ChainDB believes we have that block. If the header has changed, we need to re-open
-            # a gap for the corresponding block.
+            # ChainDB believes we have that block. If the header has changed, we need to
+            # re-open a gap for the corresponding block.
             old_canonical_header = cls._get_canonical_block_header_by_number(
-                db,
-                persisting_header.block_number
+                db, persisting_header.block_number
             )
             if old_canonical_header != persisting_header:
                 updated_gaps = reopen_gap(persisting_header.block_number, current_gaps)
                 db.set(
                     SchemaV1.make_chain_gaps_lookup_key(),
-                    rlp.encode(updated_gaps, sedes=chain_gaps)
+                    rlp.encode(updated_gaps, sedes=chain_gaps),
                 )
 
         return gap_change, gaps
 
     #
     # Header API
     #
     def get_block_uncles(self, uncles_hash: Hash32) -> Tuple[BlockHeaderAPI, ...]:
         validate_word(uncles_hash, title="Uncles Hash")
         if uncles_hash == EMPTY_UNCLE_HASH:
             return ()
         try:
             encoded_uncles = self.db[uncles_hash]
         except KeyError as exc:
-            raise HeaderNotFound(
-                f"No uncles found for hash {uncles_hash!r}"
-            ) from exc
+            raise HeaderNotFound(f"No uncles found for hash {uncles_hash!r}") from exc
         else:
-            return tuple(rlp.decode(encoded_uncles, sedes=rlp.sedes.CountableList(HeaderSedes)))
+            return tuple(
+                rlp.decode(encoded_uncles, sedes=rlp.sedes.CountableList(HeaderSedes))
+            )
 
     @classmethod
     def _decanonicalize_old_headers(
         cls,
         db: DatabaseAPI,
         numbers_to_decanonicalize: Sequence[BlockNumber],
     ) -> Tuple[BlockHeaderAPI, ...]:
@@ -186,41 +199,44 @@
             except HeaderNotFound:
                 # no old block, and no more possible
                 break
             else:
                 old_header = cls._get_block_header_by_hash(db, old_hash)
                 old_canonical_headers.append(old_header)
                 try:
-                    transaction_hashes = cls._get_block_transaction_hashes(db, old_header)
+                    transaction_hashes = cls._get_block_transaction_hashes(
+                        db, old_header
+                    )
                     for transaction_hash in transaction_hashes:
-                        cls._remove_transaction_from_canonical_chain(db, transaction_hash)
+                        cls._remove_transaction_from_canonical_chain(
+                            db, transaction_hash
+                        )
                 except MissingTrieNode:
                     # If the transactions were never stored for the (now) non-canonical
                     # chain, then you don't need to remove them from the canonical chain
                     # lookup.
                     pass
 
         return tuple(old_canonical_headers)
 
     #
     # Block API
     #
-    def persist_block(self,
-                      block: BlockAPI,
-                      genesis_parent_hash: Hash32 = GENESIS_PARENT_HASH
-                      ) -> Tuple[Tuple[Hash32, ...], Tuple[Hash32, ...]]:
+    def persist_block(
+        self, block: BlockAPI, genesis_parent_hash: Hash32 = GENESIS_PARENT_HASH
+    ) -> Tuple[Tuple[Hash32, ...], Tuple[Hash32, ...]]:
         with self.db.atomic_batch() as db:
             return self._persist_block(db, block, genesis_parent_hash)
 
-    def persist_unexecuted_block(self,
-                                 block: BlockAPI,
-                                 receipts: Tuple[ReceiptAPI, ...],
-                                 genesis_parent_hash: Hash32 = GENESIS_PARENT_HASH
-                                 ) -> Tuple[Tuple[Hash32, ...], Tuple[Hash32, ...]]:
-
+    def persist_unexecuted_block(
+        self,
+        block: BlockAPI,
+        receipts: Tuple[ReceiptAPI, ...],
+        genesis_parent_hash: Hash32 = GENESIS_PARENT_HASH,
+    ) -> Tuple[Tuple[Hash32, ...], Tuple[Hash32, ...]]:
         tx_root_hash, tx_kv_nodes = make_trie_root_and_nodes(block.transactions)
 
         if tx_root_hash != block.header.transaction_root:
             raise ValidationError(
                 f"Block's transaction_root ({block.header.transaction_root!r}) "
                 f"does not match expected value: {tx_root_hash!r}"
             )
@@ -237,36 +253,34 @@
             self._persist_trie_data_dict(db, receipt_kv_nodes)
             self._persist_trie_data_dict(db, tx_kv_nodes)
 
             return self._persist_block(db, block, genesis_parent_hash)
 
     @classmethod
     def _persist_block(
-            cls,
-            db: DatabaseAPI,
-            block: BlockAPI,
-            genesis_parent_hash: Hash32) -> Tuple[Tuple[Hash32, ...], Tuple[Hash32, ...]]:
-        header_chain = (block.header, )
+        cls, db: DatabaseAPI, block: BlockAPI, genesis_parent_hash: Hash32
+    ) -> Tuple[Tuple[Hash32, ...], Tuple[Hash32, ...]]:
+        header_chain = (block.header,)
         new_canonical_headers, old_canonical_headers = cls._persist_header_chain(
-            db,
-            header_chain,
-            genesis_parent_hash
+            db, header_chain, genesis_parent_hash
         )
 
         for header in new_canonical_headers:
             if header.hash == block.hash:
-                # Most of the time this is called to persist a block whose parent is the current
-                # head, so we optimize for that and read the tx hashes from the block itself. This
-                # is specially important during a fast sync.
+                # Most of the time this is called to persist a block whose parent is the
+                # current head, so we optimize for that and read the tx hashes from the
+                # block itself. This is specially important during a fast sync.
                 tx_hashes = tuple(tx.hash for tx in block.transactions)
             else:
                 tx_hashes = cls._get_block_transaction_hashes(db, header)
 
             for index, transaction_hash in enumerate(tx_hashes):
-                cls._add_transaction_to_canonical_chain(db, transaction_hash, header, index)
+                cls._add_transaction_to_canonical_chain(
+                    db, transaction_hash, header, index
+                )
 
             # post-shanghai, look for withdrawals
             if hasattr(block, "withdrawals") and block.withdrawals not in (None, ()):
                 withdrawal_hashes = tuple(
                     withdrawal.hash for withdrawal in block.withdrawals
                 )
                 for index, withdrawal_hash in enumerate(withdrawal_hashes):
@@ -280,32 +294,28 @@
         if block.uncles:
             uncles_hash = cls._persist_uncles(db, block.uncles)
         else:
             uncles_hash = EMPTY_UNCLE_HASH
         if uncles_hash != block.header.uncles_hash:
             raise ValidationError(
                 "Block's uncles_hash (%s) does not match actual uncles' hash (%s)",
-                block.header.uncles_hash, uncles_hash)
+                block.header.uncles_hash,
+                uncles_hash,
+            )
         new_canonical_hashes = tuple(header.hash for header in new_canonical_headers)
-        old_canonical_hashes = tuple(
-            header.hash for header in old_canonical_headers)
+        old_canonical_hashes = tuple(header.hash for header in old_canonical_headers)
 
         cls._update_chain_gaps(db, block)
         return new_canonical_hashes, old_canonical_hashes
 
-    def persist_uncles(
-            self,
-            uncles: Tuple[BlockHeaderAPI]) -> Hash32:
+    def persist_uncles(self, uncles: Tuple[BlockHeaderAPI]) -> Hash32:
         return self._persist_uncles(self.db, uncles)
 
     @staticmethod
-    def _persist_uncles(
-            db: DatabaseAPI,
-            uncles: Tuple[BlockHeaderAPI, ...]) -> Hash32:
-
+    def _persist_uncles(db: DatabaseAPI, uncles: Tuple[BlockHeaderAPI, ...]) -> Hash32:
         uncles_hash = keccak(rlp.encode(uncles))
         db.set(
             uncles_hash,
             rlp.encode(uncles, sedes=rlp.sedes.CountableList(HeaderSedes)),
         )
         return cast(Hash32, uncles_hash)
 
@@ -322,157 +332,176 @@
         useful for retrieving encoded transactions or withdrawals from the
         transaction_root or withdrawals_root of a block.
         """
         item_db = HexaryTrie(db, root_hash=block_root_hash)
         for item_idx in itertools.count():
             item_key = rlp.encode(item_idx)
             encoded = item_db[item_key]
-            if encoded != b'':
+            if encoded != b"":
                 yield encoded
             else:
                 break
 
     #
     # Transaction API
     #
-    def add_receipt(self,
-                    block_header: BlockHeaderAPI,
-                    index_key: int, receipt: ReceiptAPI) -> Hash32:
+    def add_receipt(
+        self, block_header: BlockHeaderAPI, index_key: int, receipt: ReceiptAPI
+    ) -> Hash32:
         receipt_db = HexaryTrie(db=self.db, root_hash=block_header.receipt_root)
         receipt_db[index_key] = receipt.encode()
         return receipt_db.root_hash
 
-    def add_transaction(self,
-                        block_header: BlockHeaderAPI,
-                        index_key: int,
-                        transaction: SignedTransactionAPI) -> Hash32:
+    def add_transaction(
+        self,
+        block_header: BlockHeaderAPI,
+        index_key: int,
+        transaction: SignedTransactionAPI,
+    ) -> Hash32:
         transaction_db = HexaryTrie(self.db, root_hash=block_header.transaction_root)
         transaction_db[index_key] = transaction.encode()
         return transaction_db.root_hash
 
     def get_block_transactions(
-            self,
-            header: BlockHeaderAPI,
-            transaction_decoder: Type[TransactionDecoderAPI]) -> Tuple[SignedTransactionAPI, ...]:
-        return self._get_block_transactions(header.transaction_root, transaction_decoder)
+        self, header: BlockHeaderAPI, transaction_decoder: Type[TransactionDecoderAPI]
+    ) -> Tuple[SignedTransactionAPI, ...]:
+        return self._get_block_transactions(
+            header.transaction_root, transaction_decoder
+        )
 
-    def get_block_transaction_hashes(self, block_header: BlockHeaderAPI) -> Tuple[Hash32, ...]:
+    def get_block_transaction_hashes(
+        self, block_header: BlockHeaderAPI
+    ) -> Tuple[Hash32, ...]:
         """
         Returns an iterable of the transaction hashes from the block specified
         by the given block header.
         """
         return self._get_block_transaction_hashes(self.db, block_header)
 
     @classmethod
     @to_tuple
     def _get_block_transaction_hashes(
-            cls,
-            db: DatabaseAPI,
-            block_header: BlockHeaderAPI) -> Iterable[Hash32]:
+        cls, db: DatabaseAPI, block_header: BlockHeaderAPI
+    ) -> Iterable[Hash32]:
         all_encoded_transactions = cls._get_block_data_from_root_hash(
             db,
             block_header.transaction_root,
         )
         for encoded_transaction in all_encoded_transactions:
             yield cast(Hash32, keccak(encoded_transaction))
 
     @to_tuple
-    def get_receipts(self,
-                     header: BlockHeaderAPI,
-                     receipt_decoder: Type[ReceiptDecoderAPI]) -> Iterable[ReceiptAPI]:
+    def get_receipts(
+        self, header: BlockHeaderAPI, receipt_decoder: Type[ReceiptDecoderAPI]
+    ) -> Iterable[ReceiptAPI]:
         receipt_db = HexaryTrie(db=self.db, root_hash=header.receipt_root)
         for receipt_idx in itertools.count():
             receipt_key = rlp.encode(receipt_idx)
             receipt_data = receipt_db[receipt_key]
-            if receipt_data != b'':
+            if receipt_data != b"":
                 yield receipt_decoder.decode(receipt_data)
             else:
                 break
 
     def get_transaction_by_index(
-            self,
-            block_number: BlockNumber,
-            transaction_index: int,
-            transaction_decoder: Type[TransactionDecoderAPI]) -> SignedTransactionAPI:
+        self,
+        block_number: BlockNumber,
+        transaction_index: int,
+        transaction_decoder: Type[TransactionDecoderAPI],
+    ) -> SignedTransactionAPI:
         try:
             block_header = self.get_canonical_block_header_by_number(block_number)
         except HeaderNotFound:
-            raise TransactionNotFound(f"Block {block_number} is not in the canonical chain")
+            raise TransactionNotFound(
+                f"Block {block_number} is not in the canonical chain"
+            )
         transaction_db = HexaryTrie(self.db, root_hash=block_header.transaction_root)
         encoded_index = rlp.encode(transaction_index)
         encoded_transaction = transaction_db[encoded_index]
-        if encoded_transaction != b'':
+        if encoded_transaction != b"":
             return transaction_decoder.decode(encoded_transaction)
         else:
             raise TransactionNotFound(
-                f"No transaction is at index {transaction_index} of block {block_number}"
+                f"No transaction is at index {transaction_index} "
+                f"of block {block_number}"
             )
 
-    def get_transaction_index(self, transaction_hash: Hash32) -> Tuple[BlockNumber, int]:
+    def get_transaction_index(
+        self, transaction_hash: Hash32
+    ) -> Tuple[BlockNumber, int]:
         key = SchemaV1.make_transaction_hash_to_block_lookup_key(transaction_hash)
         try:
             encoded_key = self.db[key]
         except KeyError:
             raise TransactionNotFound(
-                f"Transaction {encode_hex(transaction_hash)} not found in canonical chain"
+                f"Transaction {encode_hex(transaction_hash)} "
+                "not found in canonical chain"
             )
 
         transaction_key = rlp.decode(encoded_key, sedes=BlockDataKey)
         return (transaction_key.block_number, transaction_key.index)
 
-    def get_receipt_by_index(self,
-                             block_number: BlockNumber,
-                             receipt_index: int,
-                             receipt_decoder: Type[ReceiptDecoderAPI],
-                             ) -> ReceiptAPI:
+    def get_receipt_by_index(
+        self,
+        block_number: BlockNumber,
+        receipt_index: int,
+        receipt_decoder: Type[ReceiptDecoderAPI],
+    ) -> ReceiptAPI:
         try:
             block_header = self.get_canonical_block_header_by_number(block_number)
         except HeaderNotFound:
             raise ReceiptNotFound(f"Block {block_number} is not in the canonical chain")
 
         receipt_db = HexaryTrie(db=self.db, root_hash=block_header.receipt_root)
         receipt_key = rlp.encode(receipt_index)
         receipt_data = receipt_db[receipt_key]
-        if receipt_data != b'':
+        if receipt_data != b"":
             return receipt_decoder.decode(receipt_data)
         else:
             raise ReceiptNotFound(
                 f"Receipt with index {receipt_index} not found in block"
             )
 
     @functools.lru_cache(maxsize=32)
     @to_tuple
     def _get_block_transactions(
-            self,
-            transaction_root: Hash32,
-            transaction_decoder: Type[TransactionDecoderAPI]) -> Iterable[SignedTransactionAPI]:
+        self, transaction_root: Hash32, transaction_decoder: Type[TransactionDecoderAPI]
+    ) -> Iterable[SignedTransactionAPI]:
         """
         Memoizable version of `get_block_transactions`
         """
-        for encoded_transaction in self._get_block_data_from_root_hash(self.db, transaction_root):
+        for encoded_transaction in self._get_block_data_from_root_hash(
+            self.db, transaction_root
+        ):
             yield transaction_decoder.decode(encoded_transaction)
 
     @staticmethod
-    def _remove_transaction_from_canonical_chain(db: DatabaseAPI, transaction_hash: Hash32) -> None:
+    def _remove_transaction_from_canonical_chain(
+        db: DatabaseAPI, transaction_hash: Hash32
+    ) -> None:
         """
         Removes the transaction specified by the given hash from the canonical
         chain.
         """
         db.delete(SchemaV1.make_transaction_hash_to_block_lookup_key(transaction_hash))
 
     @staticmethod
-    def _add_transaction_to_canonical_chain(db: DatabaseAPI,
-                                            transaction_hash: Hash32,
-                                            block_header: BlockHeaderAPI,
-                                            index: int) -> None:
+    def _add_transaction_to_canonical_chain(
+        db: DatabaseAPI,
+        transaction_hash: Hash32,
+        block_header: BlockHeaderAPI,
+        index: int,
+    ) -> None:
         """
         :param bytes transaction_hash: the hash of the transaction to add the lookup for
-        :param block_header: The header of the block with the txn that is in the canonical chain
+        :param block_header: The header of the block with the txn that is in the
+            canonical chain
         :param int index: the position of the transaction in the block
-        - add lookup from transaction hash to the block number and index that the body is stored at
+        - add lookup from transaction hash to the block number and index that the body
+            is stored at
         - remove transaction hash to body lookup in the pending pool
         """
         transaction_key = BlockDataKey(block_header.block_number, index)
         db.set(
             SchemaV1.make_transaction_hash_to_block_lookup_key(transaction_hash),
             rlp.encode(transaction_key),
         )
@@ -502,15 +531,15 @@
             yield rlp.decode(encoded_withdrawal, sedes=Withdrawal)
 
     @staticmethod
     def _add_withdrawal_to_canonical_chain(
         db: DatabaseAPI,
         withdrawal_hash: Hash32,
         block_header: BlockHeaderAPI,
-        index: int
+        index: int,
     ) -> None:
         withdrawal_key = BlockDataKey(block_header.block_number, index)
         db.set(
             SchemaV1.make_withdrawal_hash_to_block_lookup_key(withdrawal_hash),
             rlp.encode(withdrawal_key),
         )
 
@@ -524,10 +553,12 @@
         return self.db[key]
 
     def persist_trie_data_dict(self, trie_data_dict: Dict[Hash32, bytes]) -> None:
         with self.db.atomic_batch() as db:
             self._persist_trie_data_dict(db, trie_data_dict)
 
     @classmethod
-    def _persist_trie_data_dict(cls, db: DatabaseAPI, trie_data_dict: Dict[Hash32, bytes]) -> None:
+    def _persist_trie_data_dict(
+        cls, db: DatabaseAPI, trie_data_dict: Dict[Hash32, bytes]
+    ) -> None:
         for key, value in trie_data_dict.items():
             db[key] = value
```

### Comparing `py-evm-0.7.0a1/eth/db/chain_gaps.py` & `py-evm-0.7.0a2/eth/db/chain_gaps.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 import enum
-from typing import Iterable, Tuple
+from typing import (
+    Iterable,
+    Tuple,
+)
 
-from eth_typing import BlockNumber
+from eth_typing import (
+    BlockNumber,
+)
 from eth_utils import (
     ValidationError,
     to_tuple,
 )
 
-from eth.exceptions import GapTrackingCorrupted
-from eth.typing import BlockRange, ChainGaps
+from eth.exceptions import (
+    GapTrackingCorrupted,
+)
+from eth.typing import (
+    BlockRange,
+    ChainGaps,
+)
 
 
 class GapChange(enum.Enum):
     NoChange = enum.auto()
     NewGap = enum.auto()
     GapFill = enum.auto()
     GapSplit = enum.auto()
@@ -29,15 +39,17 @@
 )
 GENESIS_CHAIN_GAPS = ((), BlockNumber(1))
 
 GapInfo = Tuple[GapChange, ChainGaps]
 
 
 @to_tuple
-def _join_overlapping_gaps(unjoined_gaps: Tuple[BlockRange, ...]) -> Iterable[BlockRange]:
+def _join_overlapping_gaps(
+    unjoined_gaps: Tuple[BlockRange, ...]
+) -> Iterable[BlockRange]:
     """
     After introducing a new gap, join any that overlap.
     Input must already be sorted.
     """
     unyielded_low = None
     unyielded_high = None
     for low, high in unjoined_gaps:
@@ -62,15 +74,15 @@
     Add a new gap, for a header that was decanonicalized.
     """
     current_gaps, tip_child = base_gaps
 
     if tip_child <= decanonicalized:
         return base_gaps
 
-    new_raw_gaps = current_gaps + ((decanonicalized, decanonicalized), )
+    new_raw_gaps = current_gaps + ((decanonicalized, decanonicalized),)
 
     # join overlapping gaps
     joined_gaps = _join_overlapping_gaps(sorted(new_raw_gaps))
 
     # is the last gap overlapping with the tip child? if so, merge it
     if joined_gaps[-1][1] + 1 >= tip_child:
         return joined_gaps[:-1], joined_gaps[-1][0]
@@ -104,21 +116,23 @@
         # This is adding a consecutive header at the very tail
         new_gaps = (current_gaps, BlockNumber(newly_persisted + 1))
         gap_change = GapChange.TailWrite
     elif newly_persisted > tip_child:
         # We are creating a gap in the chain
         gap_end = BlockNumber(newly_persisted - 1)
         new_gaps = (
-            current_gaps + ((tip_child, gap_end),), BlockNumber(newly_persisted + 1)
+            current_gaps + ((tip_child, gap_end),),
+            BlockNumber(newly_persisted + 1),
         )
         gap_change = GapChange.NewGap
     elif newly_persisted < tip_child:
         # We are patching a gap which may either shrink an existing gap or divide it
         matching_gaps = [
-            (index, pair) for index, pair in enumerate(current_gaps)
+            (index, pair)
+            for index, pair in enumerate(current_gaps)
             if newly_persisted >= pair[0] and newly_persisted <= pair[1]
         ]
 
         if len(matching_gaps) > 1:
             first_match, second_match, *_ = matching_gaps
             raise GapTrackingCorrupted(
                 "Corrupted chain gap tracking",
@@ -132,30 +146,43 @@
         elif len(matching_gaps) == 1:
             gap_index, gap = matching_gaps[0]
             if newly_persisted == gap[0] and newly_persisted == gap[1]:
                 updated_center: Tuple[BlockRange, ...] = ()
                 gap_change = GapChange.GapFill
             elif newly_persisted == gap[0]:
                 # we are shrinking the gap at the start
-                updated_center = ((BlockNumber(gap[0] + 1), gap[1],),)
+                updated_center = (
+                    (
+                        BlockNumber(gap[0] + 1),
+                        gap[1],
+                    ),
+                )
                 gap_change = GapChange.GapLeftShrink
             elif newly_persisted == gap[1]:
                 # we are shrinking the gap at the tail
-                updated_center = ((gap[0], BlockNumber(gap[1] - 1),),)
+                updated_center = (
+                    (
+                        gap[0],
+                        BlockNumber(gap[1] - 1),
+                    ),
+                )
                 gap_change = GapChange.GapRightShrink
             elif gap[0] < newly_persisted < gap[1]:
                 # we are dividing the gap
                 first_new_gap = (gap[0], BlockNumber(newly_persisted - 1))
                 second_new_gap = (BlockNumber(newly_persisted + 1), gap[1])
-                updated_center = (first_new_gap, second_new_gap,)
+                updated_center = (
+                    first_new_gap,
+                    second_new_gap,
+                )
                 gap_change = GapChange.GapSplit
             else:
                 raise Exception("Invariant")
 
             before_gap = current_gaps[:gap_index]
-            after_gap = current_gaps[gap_index + 1:]
+            after_gap = current_gaps[gap_index + 1 :]
             new_gaps = (before_gap + updated_center + after_gap, tip_child)
 
     else:
         raise Exception("Invariant")
 
     return gap_change, new_gaps
```

### Comparing `py-evm-0.7.0a1/eth/db/diff.py` & `py-evm-0.7.0a2/eth/db/diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from collections.abc import (
     Mapping,
     MutableMapping,
 )
 from typing import (
-    cast,
+    TYPE_CHECKING,
     Dict,
     Iterable,
-    Union,
     Tuple,
-    TYPE_CHECKING,
+    Union,
+    cast,
 )
 
 from eth_utils import (
     encode_hex,
     to_tuple,
 )
 
-from eth.abc import DatabaseAPI
-from eth.vm.interrupt import EVMMissingData
+from eth.abc import (
+    DatabaseAPI,
+)
+from eth.vm.interrupt import (
+    EVMMissingData,
+)
 
 if TYPE_CHECKING:
-    ABC_Mutable_Mapping = MutableMapping[bytes, Union[bytes, 'MissingReason']]
-    ABC_Mapping = Mapping[bytes, Union[bytes, 'MissingReason']]
+    ABC_Mutable_Mapping = MutableMapping[bytes, Union[bytes, "MissingReason"]]
+    ABC_Mapping = Mapping[bytes, Union[bytes, "MissingReason"]]
 else:
     ABC_Mutable_Mapping = MutableMapping
     ABC_Mapping = Mapping
 
 
 class MissingReason(str):
     pass
@@ -39,14 +43,15 @@
     """
     Raised when trying to access a missing key/value pair in a :class:`DBDiff`
     or :class:`DBDiffTracker`.
 
     Use :attr:`is_deleted` to check if the value is missing because it was
     deleted, or simply because it was never updated.
     """
+
     def __init__(self, missing_key: bytes, reason: MissingReason) -> None:
         self.reason = reason
         super().__init__(missing_key, reason)
 
     @property
     def is_deleted(self) -> bool:
         return self.reason == DELETED
@@ -61,88 +66,95 @@
     - the key was deleted at some point
 
     When getting a value, a special subtype of KeyError is raised on failure.
     The exception, :class:`DiffMissingError`, can be used to check if the value
     was deleted, or never present, using :meth:`DiffMissingError.is_deleted`.
 
     When it's time to take the tracked changes and write them to your database,
-    get the :class:`DBDiff` with :meth:`DBDiffTracker.diff` and use the attached methods.
+    get the :class:`DBDiff` with :meth:`DBDiffTracker.diff` and use the attached
+    methods.
     """
+
     def __init__(self) -> None:
         self._changes: Dict[bytes, Union[bytes, MissingReason]] = {}
 
     def __contains__(self, key: bytes) -> bool:  # type: ignore # Breaks LSP
         result = self._changes.get(key, NEVER_INSERTED)
         return result not in (DELETED, NEVER_INSERTED)
 
     def __getitem__(self, key: bytes) -> bytes:
         result = self._changes.get(key, NEVER_INSERTED)
         if result in (DELETED, NEVER_INSERTED):
-            raise DiffMissingError(key, result)  # type: ignore # ignore over cast for perf reasons
+            raise DiffMissingError(key, result)  # type: ignore # ignore over cast for perf reasons  # noqa: E501
         else:
             return result  # type: ignore # ignore over cast for perf reasons
 
     def __setitem__(self, key: bytes, value: Union[bytes, MissingReason]) -> None:
         self._changes[key] = value
 
     def __delitem__(self, key: bytes) -> None:
         # The diff does not have access to any underlying db,
         # so it cannot check if the key exists before deleting.
         self._changes[key] = DELETED
 
     def __iter__(self) -> None:
         raise NotImplementedError(
-            "Cannot iterate through changes, use diff().apply_to(db) to update a database"
+            "Cannot iterate through changes, use diff().apply_to(db) "
+            "to update a database"
         )
 
     def __len__(self) -> int:
         return len(self._changes)
 
-    def diff(self) -> 'DBDiff':
+    def diff(self) -> "DBDiff":
         return DBDiff(dict(self._changes))
 
 
 class DBDiff(ABC_Mapping):
     """
     DBDiff is a read-only view of the updates/inserts and deletes
     generated when tracking changes with :class:`DBDiffTracker`.
 
     The primary usage is to apply these changes to your underlying
     database with :meth:`apply_to`.
     """
+
     _changes: Dict[bytes, Union[bytes, MissingReason]] = None
 
-    def __init__(self, changes: Dict[bytes, Union[bytes, MissingReason]] = None) -> None:
+    def __init__(
+        self, changes: Dict[bytes, Union[bytes, MissingReason]] = None
+    ) -> None:
         if changes is None:
             self._changes = {}
         else:
             self._changes = changes
 
     def __getitem__(self, key: bytes) -> bytes:
         result = self._changes.get(key, NEVER_INSERTED)
         if result in (DELETED, NEVER_INSERTED):
-            raise DiffMissingError(key, result)  # type: ignore # ignore over cast for perf reasons
+            raise DiffMissingError(key, result)  # type: ignore # ignore over cast for perf reasons  # noqa: E501
         else:
             return result  # type: ignore # ignore over cast for perf reasons
 
     def __iter__(self) -> None:
         raise NotImplementedError(
             "Cannot iterate through changes, use apply_to(db) to update a database. "
-            "Also, pending_keys(), deleted_keys(), and pending_items() might be of interest."
+            "Also, pending_keys(), deleted_keys(), and pending_items() might be of "
+            "interest."
         )
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, DBDiff):
             return False
         else:
             return self._changes == other._changes
 
     def __repr__(self) -> str:
         deleted = [
-            f'key={encode_hex(key)}'
+            f"key={encode_hex(key)}"
             for key, val in self._changes.items()
             if val is DELETED
         ]
         updated = [
             f"key={encode_hex(key)} to val={encode_hex(cast(bytes, val))}"
             for key, val in self._changes.items()
             if val is not DELETED
@@ -175,19 +187,19 @@
     def pending_items(self) -> Iterable[Tuple[bytes, bytes]]:
         """
         A tuple of (key, value) pairs for every key that has been updated.
         Like :meth:`pending_keys()`, this does not return any deleted keys.
         """
         for key, value in self._changes.items():
             if value is not DELETED:
-                yield key, value  # type: ignore # value can only be DELETED or actual new value
+                yield key, value  # type: ignore # value can only be DELETED or actual new value  # noqa: E501
 
-    def apply_to(self,
-                 db: Union[DatabaseAPI, ABC_Mutable_Mapping],
-                 apply_deletes: bool = True) -> None:
+    def apply_to(
+        self, db: Union[DatabaseAPI, ABC_Mutable_Mapping], apply_deletes: bool = True
+    ) -> None:
         """
         Apply the changes in this diff to the given database.
         You may choose to opt out of deleting any underlying keys.
 
         :param apply_deletes: whether the pending deletes should be
             applied to the database
         """
@@ -202,15 +214,15 @@
                         pass
                 else:
                     pass
             else:
                 db[key] = value  # type: ignore # ignore over cast for perf reasons
 
     @classmethod
-    def join(cls, diffs: Iterable['DBDiff']) -> 'DBDiff':
+    def join(cls, diffs: Iterable["DBDiff"]) -> "DBDiff":
         """
         Join several DBDiff objects into a single DBDiff object.
 
         In case of a conflict, changes in diffs that come later
         in ``diffs`` will overwrite changes from earlier changes.
         """
         tracker = DBDiffTracker()
```

### Comparing `py-evm-0.7.0a1/eth/db/header.py` & `py-evm-0.7.0a2/eth/db/header.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 import functools
 from typing import (
-    cast,
     Iterable,
     Sequence,
     Tuple,
+    cast,
 )
 
-import rlp
-
-from eth_utils.toolz import (
-    concat,
-    first,
-    sliding_window,
+from eth_typing import (
+    BlockNumber,
+    Hash32,
 )
-
 from eth_utils import (
+    ValidationError,
     encode_hex,
     to_tuple,
-    ValidationError,
 )
-
-from eth_typing import (
-    Hash32,
-    BlockNumber,
+from eth_utils.toolz import (
+    concat,
+    first,
+    sliding_window,
 )
+import rlp
 
 from eth.abc import (
     AtomicDatabaseAPI,
     BlockHeaderAPI,
     DatabaseAPI,
     HeaderDatabaseAPI,
 )
 from eth.constants import (
     GENESIS_PARENT_HASH,
 )
 from eth.db.chain_gaps import (
-    GapChange,
-    GapInfo,
     GAP_WRITES,
     GENESIS_CHAIN_GAPS,
+    GapChange,
+    GapInfo,
     fill_gap,
     reopen_gap,
 )
+from eth.db.schema import (
+    SchemaV1,
+)
 from eth.exceptions import (
     CanonicalHeadNotFound,
     CheckpointsMustBeCanonical,
     HeaderNotFound,
     ParentNotFound,
 )
-from eth.db.schema import SchemaV1
-from eth.rlp.sedes import chain_gaps
-from eth.typing import ChainGaps
+from eth.rlp.sedes import (
+    chain_gaps,
+)
+from eth.typing import (
+    ChainGaps,
+)
 from eth.validation import (
     validate_block_number,
     validate_word,
 )
-from eth.vm.header import HeaderSedes
+from eth.vm.header import (
+    HeaderSedes,
+)
 
 
 class HeaderDB(HeaderDatabaseAPI):
     def __init__(self, db: AtomicDatabaseAPI) -> None:
         self.db = db
 
     def get_header_chain_gaps(self) -> ChainGaps:
@@ -72,31 +77,30 @@
         except KeyError:
             return GENESIS_CHAIN_GAPS
         else:
             return rlp.decode(encoded_gaps, sedes=chain_gaps)
 
     @classmethod
     def _update_header_chain_gaps(
-            cls,
-            db: DatabaseAPI,
-            persisted_header: BlockHeaderAPI,
-            base_gaps: ChainGaps = None
+        cls,
+        db: DatabaseAPI,
+        persisted_header: BlockHeaderAPI,
+        base_gaps: ChainGaps = None,
     ) -> GapInfo:
-
         # If we make many updates in a row, we can avoid reloading the integrity info by
         # continuously caching it and providing it as a parameter to this API
         if base_gaps is None:
             base_gaps = cls._get_header_chain_gaps(db)
 
         gap_change, gaps = fill_gap(persisted_header.block_number, base_gaps)
 
         if gap_change is not GapChange.NoChange:
             db.set(
                 SchemaV1.make_header_chain_gaps_lookup_key(),
-                rlp.encode(gaps, sedes=chain_gaps)
+                rlp.encode(gaps, sedes=chain_gaps),
             )
 
         return gap_change, gaps
 
     #
     # Canonical Chain API
     #
@@ -113,22 +117,23 @@
         except KeyError:
             raise HeaderNotFound(
                 f"No canonical header for block number #{block_number}"
             )
         else:
             return rlp.decode(encoded_key, sedes=rlp.sedes.binary)
 
-    def get_canonical_block_header_by_number(self, block_number: BlockNumber) -> BlockHeaderAPI:
+    def get_canonical_block_header_by_number(
+        self, block_number: BlockNumber
+    ) -> BlockHeaderAPI:
         return self._get_canonical_block_header_by_number(self.db, block_number)
 
     @classmethod
     def _get_canonical_block_header_by_number(
-            cls,
-            db: DatabaseAPI,
-            block_number: BlockNumber) -> BlockHeaderAPI:
+        cls, db: DatabaseAPI, block_number: BlockNumber
+    ) -> BlockHeaderAPI:
         validate_block_number(block_number)
         canonical_block_hash = cls._get_canonical_block_hash(db, block_number)
         return cls._get_block_header_by_hash(db, canonical_block_hash)
 
     def get_canonical_head(self) -> BlockHeaderAPI:
         return self._get_canonical_head(self.db)
 
@@ -147,15 +152,17 @@
     #
     # Header API
     #
     def get_block_header_by_hash(self, block_hash: Hash32) -> BlockHeaderAPI:
         return self._get_block_header_by_hash(self.db, block_hash)
 
     @staticmethod
-    def _get_block_header_by_hash(db: DatabaseAPI, block_hash: Hash32) -> BlockHeaderAPI:
+    def _get_block_header_by_hash(
+        db: DatabaseAPI, block_hash: Hash32
+    ) -> BlockHeaderAPI:
         """
         Returns the requested block header as specified by block hash.
 
         Raises BlockNotFound if it is not present in the db.
         """
         validate_word(block_hash, title="Block Hash")
         try:
@@ -179,128 +186,128 @@
         return self._header_exists(self.db, block_hash)
 
     @staticmethod
     def _header_exists(db: DatabaseAPI, block_hash: Hash32) -> bool:
         validate_word(block_hash, title="Block Hash")
         return block_hash in db
 
-    def persist_header(self,
-                       header: BlockHeaderAPI
-                       ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
+    def persist_header(
+        self, header: BlockHeaderAPI
+    ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
         return self.persist_header_chain((header,))
 
-    def persist_header_chain(self,
-                             headers: Iterable[BlockHeaderAPI],
-                             genesis_parent_hash: Hash32 = GENESIS_PARENT_HASH
-                             ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
+    def persist_header_chain(
+        self,
+        headers: Iterable[BlockHeaderAPI],
+        genesis_parent_hash: Hash32 = GENESIS_PARENT_HASH,
+    ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
         with self.db.atomic_batch() as db:
             return self._persist_header_chain(db, headers, genesis_parent_hash)
 
     def persist_checkpoint_header(self, header: BlockHeaderAPI, score: int) -> None:
         with self.db.atomic_batch() as db:
             return self._persist_checkpoint_header(db, header, score)
 
     @classmethod
     def _set_hash_scores_to_db(
-            cls,
-            db: DatabaseAPI,
-            header: BlockHeaderAPI,
-            score: int
+        cls, db: DatabaseAPI, header: BlockHeaderAPI, score: int
     ) -> int:
         difficulty = header.difficulty
         new_score = (
             # In PoS, difficulty = 0 and score values do not need to work the same way
-            score + difficulty if difficulty != 0 else score + header.block_number
+            score + difficulty
+            if difficulty != 0
+            else score + header.block_number
         )
 
         db.set(
             SchemaV1.make_block_hash_to_score_lookup_key(header.hash),
             rlp.encode(new_score, sedes=rlp.sedes.big_endian_int),
         )
 
         return new_score
 
     @classmethod
     def _persist_checkpoint_header(
-            cls,
-            db: DatabaseAPI,
-            header: BlockHeaderAPI,
-            score: int
+        cls, db: DatabaseAPI, header: BlockHeaderAPI, score: int
     ) -> None:
         db.set(
             header.hash,
             rlp.encode(header),
         )
 
         # Add new checkpoint header
         previous_checkpoints = cls._get_checkpoints(db)
         new_checkpoints = previous_checkpoints + (header.hash,)
         db.set(
             SchemaV1.make_checkpoint_headers_key(),
-            b''.join(new_checkpoints),
+            b"".join(new_checkpoints),
         )
 
         difficulty = header.difficulty
         previous_score = (
             # In PoS, difficulty = 0 and score values do not need to work the same way
-            score - difficulty if difficulty != 0 else score - header.block_number
+            score - difficulty
+            if difficulty != 0
+            else score - header.block_number
         )
         cls._set_hash_scores_to_db(db, header, previous_score)
         cls._set_as_canonical_chain_head(db, header, GENESIS_PARENT_HASH)
         _, gaps = cls._update_header_chain_gaps(db, header)
 
-        # check if the parent block number exists, and is not a match for checkpoint.parent_hash
+        # check if the parent block number exists, and is not a match
+        # for checkpoint.parent_hash
         parent_block_num = BlockNumber(header.block_number - 1)
         try:
             parent_hash = cls._get_canonical_block_hash(db, parent_block_num)
         except HeaderNotFound:
             # no parent to check
             pass
         else:
-            # User is asserting that the checkpoint must be canonical, so if the parent doesn't
-            # match, then the parent must not be canonical, and should be de-canonicalized.
+            # User is asserting that the checkpoint must be canonical, so if the parent
+            # doesn't match, then the parent must not be canonical,
+            # and should be de-canonicalized.
             if parent_hash != header.parent_hash:
                 # does the correct header exist in the database?
                 try:
                     true_parent = cls._get_block_header_by_hash(db, header.parent_hash)
                 except HeaderNotFound:
                     # True parent unavailable, just delete the now non-canonical one
                     cls._decanonicalize_single(db, parent_block_num, gaps)
                 else:
                     # True parent should have already been canonicalized during
                     #   _set_as_canonical_chain_head()
                     raise ValidationError(
-                        f"Why was a non-matching parent header {parent_hash!r} left as canonical "
-                        f"after _set_as_canonical_chain_head() and {true_parent} is available?"
+                        f"Why was a non-matching parent header {parent_hash!r} left as "
+                        "canonical after _set_as_canonical_chain_head() and "
+                        f"{true_parent} is available?"
                     )
 
         cls._decanonicalize_descendant_orphans(db, header, new_checkpoints)
 
     @classmethod
     def _decanonicalize_descendant_orphans(
-            cls,
-            db: DatabaseAPI,
-            header: BlockHeaderAPI,
-            checkpoints: Tuple[Hash32, ...]) -> None:
-
-        # Determine if any children need to be de-canonicalized because they are not children of
-        #   the new chain head
+        cls, db: DatabaseAPI, header: BlockHeaderAPI, checkpoints: Tuple[Hash32, ...]
+    ) -> None:
+        # Determine if any children need to be de-canonicalized because they are not
+        # children of the new chain head
         new_gaps = starting_gaps = cls._get_header_chain_gaps(db)
 
         child_number = BlockNumber(header.block_number + 1)
         try:
             child = cls._get_canonical_block_header_by_number(db, child_number)
         except HeaderNotFound:
             # There is no canonical block here
             next_invalid_child = None
         else:
             if child.parent_hash != header.hash:
                 if child.hash in checkpoints:
                     raise CheckpointsMustBeCanonical(
-                        f"Trying to decanonicalize {child} while making {header} the chain tip"
+                        f"Trying to decanonicalize {child} while making "
+                        f"{header} the chain tip"
                     )
                 else:
                     next_invalid_child = child
             else:
                 next_invalid_child = None
 
         while next_invalid_child:
@@ -308,62 +315,60 @@
             db.delete(SchemaV1.make_block_number_to_hash_lookup_key(child_number))
             new_gaps = reopen_gap(child_number, new_gaps)
 
             # find next child
             child_number = BlockNumber(child_number + 1)
             try:
                 # All contiguous children must now be made invalid
-                next_invalid_child = cls._get_canonical_block_header_by_number(db, child_number)
+                next_invalid_child = cls._get_canonical_block_header_by_number(
+                    db, child_number
+                )
             except HeaderNotFound:
                 # Found the end of this streak of canonical blocks
                 break
             else:
                 if next_invalid_child.hash in checkpoints:
                     raise CheckpointsMustBeCanonical(
-                        f"Trying to decanonicalize {next_invalid_child} while making {header} the"
-                        " chain tip"
+                        f"Trying to decanonicalize {next_invalid_child} while making "
+                        f"{header} the chain tip"
                     )
 
         if new_gaps != starting_gaps:
             db.set(
                 SchemaV1.make_header_chain_gaps_lookup_key(),
-                rlp.encode(new_gaps, sedes=chain_gaps)
+                rlp.encode(new_gaps, sedes=chain_gaps),
             )
 
     @classmethod
     def _decanonicalize_single(
-            cls,
-            db: DatabaseAPI,
-            block_num: BlockNumber,
-            base_gaps: ChainGaps) -> ChainGaps:
+        cls, db: DatabaseAPI, block_num: BlockNumber, base_gaps: ChainGaps
+    ) -> ChainGaps:
         """
         A single block number was found to no longer be canonical. At doc-time,
         this only happens because it does not link up with a checkpoint header.
         So de-canonicalize this block number and insert a gap in the tracked
         chain gaps.
         """
 
-        db.delete(
-            SchemaV1.make_block_number_to_hash_lookup_key(block_num)
-        )
+        db.delete(SchemaV1.make_block_number_to_hash_lookup_key(block_num))
 
         new_gaps = reopen_gap(block_num, base_gaps)
         if new_gaps != base_gaps:
             db.set(
                 SchemaV1.make_header_chain_gaps_lookup_key(),
-                rlp.encode(new_gaps, sedes=chain_gaps)
+                rlp.encode(new_gaps, sedes=chain_gaps),
             )
         return new_gaps
 
     @classmethod
     def _persist_header_chain(
-            cls,
-            db: DatabaseAPI,
-            headers: Iterable[BlockHeaderAPI],
-            genesis_parent_hash: Hash32,
+        cls,
+        db: DatabaseAPI,
+        headers: Iterable[BlockHeaderAPI],
+        genesis_parent_hash: Hash32,
     ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
         headers_iterator = iter(headers)
 
         try:
             first_header = first(headers_iterator)
         except StopIteration:
             return (), ()
@@ -385,15 +390,17 @@
             curr_chain_head.hash,
             rlp.encode(curr_chain_head),
         )
         score = cls._set_hash_scores_to_db(db, curr_chain_head, score)
 
         base_gaps = cls._get_header_chain_gaps(db)
         gap_info = cls._update_header_chain_gaps(db, curr_chain_head, base_gaps)
-        gaps = cls._handle_gap_change(db, gap_info, curr_chain_head, genesis_parent_hash)
+        gaps = cls._handle_gap_change(
+            db, gap_info, curr_chain_head, genesis_parent_hash
+        )
 
         orig_headers_seq = concat([(first_header,), headers_iterator])
         for parent, child in sliding_window(2, orig_headers_seq):
             if parent.hash != child.parent_hash:
                 raise ValidationError(
                     f"Non-contiguous chain. Expected {encode_hex(child.hash)} "
                     f"to have {encode_hex(parent.hash)} as parent "
@@ -404,116 +411,134 @@
             db.set(
                 curr_chain_head.hash,
                 rlp.encode(curr_chain_head),
             )
 
             score = cls._set_hash_scores_to_db(db, curr_chain_head, score)
             gap_info = cls._update_header_chain_gaps(db, curr_chain_head, gaps)
-            gaps = cls._handle_gap_change(db, gap_info, curr_chain_head, genesis_parent_hash)
+            gaps = cls._handle_gap_change(
+                db, gap_info, curr_chain_head, genesis_parent_hash
+            )
         try:
             previous_canonical_head = cls._get_canonical_head_hash(db)
             head_score = cls._get_score(db, previous_canonical_head)
         except CanonicalHeadNotFound:
-            return cls._set_as_canonical_chain_head(db, curr_chain_head, genesis_parent_hash)
+            return cls._set_as_canonical_chain_head(
+                db, curr_chain_head, genesis_parent_hash
+            )
 
         if score > head_score:
-            return cls._set_as_canonical_chain_head(db, curr_chain_head, genesis_parent_hash)
+            return cls._set_as_canonical_chain_head(
+                db, curr_chain_head, genesis_parent_hash
+            )
 
         return (), ()
 
     @classmethod
-    def _handle_gap_change(cls,
-                           db: DatabaseAPI,
-                           gap_info: GapInfo,
-                           header: BlockHeaderAPI,
-                           genesis_parent_hash: Hash32) -> ChainGaps:
-
+    def _handle_gap_change(
+        cls,
+        db: DatabaseAPI,
+        gap_info: GapInfo,
+        header: BlockHeaderAPI,
+        genesis_parent_hash: Hash32,
+    ) -> ChainGaps:
         gap_change, gaps = gap_info
         if gap_change not in GAP_WRITES:
             return gaps
 
         # Check if this change will link up the chain to the right
         if gap_change in (GapChange.GapFill, GapChange.GapRightShrink):
             next_child_number = BlockNumber(header.block_number + 1)
-            expected_child = cls._get_canonical_block_header_by_number(db, next_child_number)
+            expected_child = cls._get_canonical_block_header_by_number(
+                db, next_child_number
+            )
             if header.hash != expected_child.parent_hash:
-                # Must not join a canonical chain that is not linked from parent to child
-                # If the child is a checkpoint, reject this fill as an uncle.
+                # Must not join a canonical chain that is not linked from parent to
+                # child. If the child is a checkpoint, reject this fill as an uncle.
                 checkpoints = cls._get_checkpoints(db)
                 if expected_child.hash in checkpoints:
                     raise CheckpointsMustBeCanonical(
-                        f"Cannot make {header} canonical, because it is not the parent of"
-                        f" declared checkpoint: {expected_child}"
+                        f"Cannot make {header} canonical, because it is not the parent "
+                        f"of declared checkpoint: {expected_child}"
                     )
                 else:
-                    # If the child is *not* a checkpoint, then re-open a gap in the chain
-                    gaps = cls._decanonicalize_single(db, expected_child.block_number, gaps)
+                    # If the child is *not* a checkpoint,
+                    # then re-open a gap in the chain
+                    gaps = cls._decanonicalize_single(
+                        db, expected_child.block_number, gaps
+                    )
 
         # We implicitly assert that persisted headers are canonical here.
-        # This assertion is made when persisting headers that are known to be part of a gap
-        # in the canonical chain.
-        # What if this assertion is later found to be false? At gap fill time, we can detect if the
-        # chains don't link (and raise a ValidationError). Also, when a true canonical header is
-        # added eventually, we need to canonicalize all the true headers.
+        # This assertion is made when persisting headers that are known to be part of a
+        # gap in the canonical chain.
+        # What if this assertion is later found to be false? At gap fill time, we can
+        # detect if the chains don't link (and raise a ValidationError). Also, when a
+        # true canonical header is added eventually, we need to canonicalize all the
+        # true headers.
         cls._canonicalize_header(db, header, genesis_parent_hash)
         return gaps
 
     @classmethod
     def _canonicalize_header(
         cls,
         db: DatabaseAPI,
         header: BlockHeaderAPI,
         genesis_parent_hash: Hash32,
     ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
         """
-        Force this header to be canonical, and adjust its ancestors/descendants as necessary
+        Force this header to be canonical,
+        and adjust its ancestors/descendants as necessary
 
         :raises CheckpointsMustBeCanonical: if trying to set a head that would
             de-canonicalize a checkpoint
         """
         new_canonical_headers = cast(
             Tuple[BlockHeaderAPI, ...],
-            tuple(reversed(cls._find_new_ancestors(db, header, genesis_parent_hash)))
+            tuple(reversed(cls._find_new_ancestors(db, header, genesis_parent_hash))),
         )
         old_canonical_headers = cls._find_headers_to_decanonicalize(
             db,
             [h.block_number for h in new_canonical_headers],
         )
 
         # Reject if this would make a checkpoint non-canonical
         checkpoints = cls._get_checkpoints(db)
-        attempted_checkpoint_overrides = {old for old in old_canonical_headers
-                                          if old.hash in checkpoints}
+        attempted_checkpoint_overrides = {
+            old for old in old_canonical_headers if old.hash in checkpoints
+        }
         if len(attempted_checkpoint_overrides):
             raise CheckpointsMustBeCanonical(
-                f"Tried to switch chain away from checkpoint(s) {attempted_checkpoint_overrides!r}"
-                f" by inserting new canonical headers {new_canonical_headers}"
+                "Tried to switch chain away from checkpoint(s) "
+                f"{attempted_checkpoint_overrides!r} by inserting new canonical "
+                f"headers {new_canonical_headers}"
             )
 
         for ancestor in new_canonical_headers:
             cls._add_block_number_to_hash_lookup(db, ancestor)
 
         if len(new_canonical_headers):
-            cls._decanonicalize_descendant_orphans(db, new_canonical_headers[-1], checkpoints)
+            cls._decanonicalize_descendant_orphans(
+                db, new_canonical_headers[-1], checkpoints
+            )
 
         return new_canonical_headers, old_canonical_headers
 
     @classmethod
     def _set_as_canonical_chain_head(
         cls,
         db: DatabaseAPI,
         header: BlockHeaderAPI,
         genesis_parent_hash: Hash32,
     ) -> Tuple[Tuple[BlockHeaderAPI, ...], Tuple[BlockHeaderAPI, ...]]:
         """
         Sets the canonical chain HEAD to the block header as specified by the
         given block hash.
 
-        :return: a tuple of the headers that are newly in the canonical chain, and the headers that
-            are no longer in the canonical chain
+        :return: a tuple of the headers that are newly in the canonical chain, and the
+            headers that are no longer in the canonical chain
         :raises CheckpointsMustBeCanonical: if trying to set a head that would
             de-canonicalize a checkpoint
         """
         try:
             current_canonical_head = cls._get_canonical_head_hash(db)
         except CanonicalHeadNotFound:
             current_canonical_head = None
@@ -541,40 +566,37 @@
     @classmethod
     def _get_checkpoints(cls, db: DatabaseAPI) -> Tuple[Hash32, ...]:
         concatenated_checkpoints = db.get(SchemaV1.make_checkpoint_headers_key())
         if concatenated_checkpoints is None:
             return ()
         else:
             return tuple(
-                Hash32(concatenated_checkpoints[index:index + 32])
+                Hash32(concatenated_checkpoints[index : index + 32])
                 for index in range(0, len(concatenated_checkpoints), 32)
             )
 
     @classmethod
     @to_tuple
     def _find_headers_to_decanonicalize(
-        cls,
-        db: DatabaseAPI,
-        numbers_to_decanonicalize: Sequence[BlockNumber]
+        cls, db: DatabaseAPI, numbers_to_decanonicalize: Sequence[BlockNumber]
     ) -> Iterable[BlockHeaderAPI]:
         for block_number in numbers_to_decanonicalize:
             try:
                 old_canonical_hash = cls._get_canonical_block_hash(db, block_number)
             except HeaderNotFound:
                 # no old_canonical block, but due to checkpointing, more may be possible
                 continue
             else:
                 yield cls._get_block_header_by_hash(db, old_canonical_hash)
 
     @classmethod
     @to_tuple
-    def _find_new_ancestors(cls,
-                            db: DatabaseAPI,
-                            header: BlockHeaderAPI,
-                            genesis_parent_hash: Hash32) -> Iterable[BlockHeaderAPI]:
+    def _find_new_ancestors(
+        cls, db: DatabaseAPI, header: BlockHeaderAPI, genesis_parent_hash: Hash32
+    ) -> Iterable[BlockHeaderAPI]:
         """
         Returns the chain leading up from the given header until (but not including)
         the first ancestor it has in common with our canonical chain.
 
         If D is the canonical head in the following chain, and F is the new header,
         then this function returns (F, E).
 
@@ -603,32 +625,34 @@
                 try:
                     h = cls._get_block_header_by_hash(db, h.parent_hash)
                 except HeaderNotFound:
                     # We must have hit a checkpoint parent, return early
                     break
 
     @staticmethod
-    def _add_block_number_to_hash_lookup(db: DatabaseAPI, header: BlockHeaderAPI) -> None:
+    def _add_block_number_to_hash_lookup(
+        db: DatabaseAPI, header: BlockHeaderAPI
+    ) -> None:
         """
         Sets a record in the database to allow looking up this header by its
         block number.
         """
         block_number_to_hash_key = SchemaV1.make_block_number_to_hash_lookup_key(
             header.block_number
         )
         db.set(
             block_number_to_hash_key,
             rlp.encode(header.hash, sedes=rlp.sedes.binary),
         )
 
 
-# When performing a chain sync (either fast or regular modes), we'll very often need to look
-# up recent block headers to validate the chain, and decoding their RLP representation is
-# relatively expensive so we cache that here, but use a small cache because we *should* only
-# be looking up recent blocks.
+# When performing a chain sync (either fast or regular modes), we'll very often need to
+# look up recent block headers to validate the chain, and decoding their RLP
+# representation is relatively expensive so we cache that here, but use a small cache
+# because we *should* only be looking up recent blocks.
 @functools.lru_cache(128)
 def _decode_block_header(header_rlp: bytes) -> BlockHeaderAPI:
     # Use a deserialization class that can handle any type of header.
     # This feels a little hack-y, but we don't know the shape of the header
     # at this point. It could be a pre-London header, or a post-London
     # header, which includes the base fee. So we use a class that knows how to
     # decode both.
```

### Comparing `py-evm-0.7.0a1/eth/db/journal.py` & `py-evm-0.7.0a2/eth/db/journal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 import collections
 from itertools import (
     count,
 )
-from typing import Callable, cast, Dict, List, Set, Union
+from typing import (
+    Callable,
+    Dict,
+    List,
+    Set,
+    Union,
+    cast,
+)
 
+from eth_utils import (
+    ValidationError,
+)
 from eth_utils.toolz import (
     first,
     nth,
 )
-from eth_utils import (
-    ValidationError,
-)
 
-from eth.abc import DatabaseAPI
-from eth.typing import JournalDBCheckpoint
+from eth.abc import (
+    DatabaseAPI,
+)
+from eth.typing import (
+    JournalDBCheckpoint,
+)
 
-from .backends.base import BaseDB
-from .diff import DBDiff, DBDiffTracker
+from .backends.base import (
+    BaseDB,
+)
+from .diff import (
+    DBDiff,
+    DBDiffTracker,
+)
 
 
 class DeletedEntry:
     pass
 
 
 # Track two different kinds of deletion:
@@ -40,55 +56,62 @@
 
 get_next_checkpoint = cast(Callable[[], JournalDBCheckpoint], count().__next__)
 
 
 class Journal(BaseDB):
     """
     A Journal provides a mechanism to track a series of changes to a dict, by inserting
-    checkpoints, and committing to them or rolling back to them, and ultimitely persisting
-    the final changes.
+    checkpoints, and committing to them or rolling back to them, and ultimitely
+    persisting the final changes.
 
     Internally, it keeps an ordered list of reversion changesets, used to roll back
-    on demand. This is optimized for the most common path: lots of checkpoints and commits,
-    and not many discards.
+    on demand. This is optimized for the most common path: lots of checkpoints and
+    commits, and not many discards.
 
-    Checkpoints are referenced by an internally-generated integer. This is *not* threadsafe.
+    Checkpoints are referenced by an internally-generated integer.
+    This is *not* threadsafe.
     """
+
     __slots__ = [
-        '_journal_data',
-        '_clears_at',
-        '_current_values',
-        '_ignore_wrapped_db',
-        '_checkpoint_stack',
+        "_journal_data",
+        "_clears_at",
+        "_current_values",
+        "_ignore_wrapped_db",
+        "_checkpoint_stack",
     ]
 
     #
-    # This is a high-use class, where we sometimes prefere optimization over readability.
-    # It's most important to optimize for record, commit, and persist, which ard the most commonly
-    # used methods.
+    # This is a high-use class, where we sometimes prefer optimization over
+    # readability. It's most important to optimize for record, commit, and persist,
+    # which are the most commonly used methods.
     #
 
     def __init__(self) -> None:
-        # If the journal was persisted right now, these would be the current changes to push:
+        # If the journal was persisted right now,
+        # these would be the current changes to push:
         self._current_values: ChangesetDict = {}
 
         # contains a mapping from all of the int checkpoints
-        # to a dictionary of key:value pairs that are used to rewind from the current values
-        # to the given checkpoint
-        self._journal_data: collections.OrderedDict[JournalDBCheckpoint, ChangesetDict] = collections.OrderedDict()  # noqa E501
-
-        # Clears are special operations that enforce that the underlying database and current
-        # changes are completely emptied out. Clears are also committable & discardable.
+        # to a dictionary of key:value pairs that are used to rewind from the current
+        # values to the given checkpoint
+        self._journal_data: collections.OrderedDict[
+            JournalDBCheckpoint, ChangesetDict
+        ] = collections.OrderedDict()
+
+        # Clears are special operations that enforce that the underlying database and
+        # current changes are completely emptied out. Clears are also committable &
+        # discardable.
         self._clears_at: Set[JournalDBCheckpoint] = set()
 
         # If a clear was called, then any missing keys should be treated as missing
         self._ignore_wrapped_db = False
 
-        # To speed up commits, we leave in old recorded checkpoints in self._journal_data, even
-        # on commit. Instead of dropping them, we keep a separate list of active checkpoints.
+        # To speed up commits, we leave in old recorded checkpoints in
+        # self._journal_data, even on commit. Instead of dropping them, we keep a
+        # separate list of active checkpoints.
         self._checkpoint_stack: List[JournalDBCheckpoint] = []
 
     @property
     def root_checkpoint(self) -> JournalDBCheckpoint:
         """
         Returns the starting checkpoint
         """
@@ -102,35 +125,37 @@
         return len(self._checkpoint_stack) < 2
 
     @property
     def last_checkpoint(self) -> JournalDBCheckpoint:
         """
         Returns the latest checkpoint
         """
-        # last() was iterating through all values, so first(reversed()) gives a 12.5x speedup
-        # Interestingly, an attempt to cache this value caused a slowdown.
+        # last() was iterating through all values, so first(reversed()) gives a 12.5x
+        # speedup Interestingly, an attempt to cache this value caused a slowdown.
         return first(reversed(self._journal_data.keys()))
 
     def has_checkpoint(self, checkpoint: JournalDBCheckpoint) -> bool:
-        # another option would be to enforce monotonically-increasing checkpoints, so we can do:
+        # another option would be to enforce monotonically-increasing checkpoints,
+        # so we can do:
         # checkpoint_idx = bisect_left(self._checkpoint_stack, checkpoint)
         # (then validate against length and value at index)
         return checkpoint in self._checkpoint_stack
 
     def record_checkpoint(
-            self,
-            custom_checkpoint: JournalDBCheckpoint = None) -> JournalDBCheckpoint:
+        self, custom_checkpoint: JournalDBCheckpoint = None
+    ) -> JournalDBCheckpoint:
         """
         Creates a new checkpoint. Checkpoints are a sequential int chosen by Journal
         to prevent collisions.
         """
         if custom_checkpoint is not None:
             if custom_checkpoint in self._journal_data:
                 raise ValidationError(
-                    f"Tried to record with an existing checkpoint: {custom_checkpoint!r}"
+                    "Tried to record with an existing checkpoint: "
+                    f"{custom_checkpoint!r}"
                 )
             else:
                 checkpoint = custom_checkpoint
         else:
             checkpoint = get_next_checkpoint()
 
         self._journal_data[checkpoint] = {}
@@ -149,40 +174,43 @@
         # This might be optimized further by iterating the other direction and
         # ignoring any follow-up rollbacks on the same variable.
         for _ in range(len(self._journal_data)):
             checkpoint_id, rollback_data = self._journal_data.popitem()
 
             for old_key, old_value in rollback_data.items():
                 if old_value is REVERT_TO_WRAPPED:
-                    # The current value may not exist, if it was a delete followed by a clear,
-                    # so pop it off, or ignore if it is already missing
+                    # The current value may not exist, if it was a delete followed by a
+                    # clear, so pop it off, or ignore if it is already missing
                     self._current_values.pop(old_key, None)
                 elif old_value is DELETE_WRAPPED:
                     self._current_values[old_key] = old_value
                 elif type(old_value) is bytes:
                     self._current_values[old_key] = old_value
                 else:
-                    raise ValidationError(f"Unexpected value, must be bytes: {old_value!r}")
+                    raise ValidationError(
+                        f"Unexpected value, must be bytes: {old_value!r}"
+                    )
 
             if checkpoint_id in self._clears_at:
                 self._clears_at.remove(checkpoint_id)
                 self._ignore_wrapped_db = False
 
             if checkpoint_id == through_checkpoint_id:
                 break
 
         if self._clears_at:
-            # if there is still a clear in older locations, then reinitiate the clear flag
+            # if there is still a clear in older locations,
+            # then reinitiate the clear flag
             self._ignore_wrapped_db = True
 
     def clear(self) -> None:
         """
-        Treat as if the *underlying* database will also be cleared by some other mechanism.
-        We build a special empty reversion changeset just for marking that all previous data should
-        be ignored.
+        Treat as if the *underlying* database will also be cleared by some other
+        mechanism. We build a special empty reversion changeset just for marking that
+        all previous data should be ignored.
         """
         checkpoint = get_next_checkpoint()
         self._journal_data[checkpoint] = self._current_values
         self._current_values = {}
         self._ignore_wrapped_db = True
         self._clears_at.add(checkpoint)
 
@@ -192,33 +220,38 @@
                 return True
             elif at_checkpoint == reversion_changeset_id:
                 return False
         raise ValidationError(f"Checkpoint {at_checkpoint} is not in the journal")
 
     def commit_checkpoint(self, commit_to: JournalDBCheckpoint) -> ChangesetDict:
         """
-        Collapses all changes since the given checkpoint. Can no longer discard to any of
-        the checkpoints that followed the given checkpoint.
+        Collapses all changes since the given checkpoint. Can no longer discard to any
+        of the checkpoints that followed the given checkpoint.
         """
-        # Another option would be to enforce monotonically-increasing changeset ids, so we can do:
+        # Another option would be to enforce monotonically-increasing changeset ids,
+        # so we can do:
         # checkpoint_idx = bisect_left(self._checkpoint_stack, commit_to)
         # (then validate against length and value at index)
-        for positions_before_last, checkpoint in enumerate(reversed(self._checkpoint_stack)):
+        for positions_before_last, checkpoint in enumerate(
+            reversed(self._checkpoint_stack)
+        ):
             if checkpoint == commit_to:
                 checkpoint_idx = -1 - positions_before_last
                 break
         else:
             raise ValidationError(f"No checkpoint {commit_to} was found")
 
         if checkpoint_idx == -1 * len(self._checkpoint_stack):
             raise ValidationError(
-                "Should not commit root changeset with commit_changeset, use pop_all() instead"
+                "Should not commit root changeset with commit_changeset, "
+                "use pop_all() instead"
             )
 
-        # delete committed checkpoints from the stack (but keep rollbacks for future discards)
+        # delete committed checkpoints from the stack
+        # (but keep rollbacks for future discards)
         del self._checkpoint_stack[checkpoint_idx:]
 
         return self._current_values
 
     def pop_all(self) -> ChangesetDict:
         final_changes = self._current_values
         self._journal_data.clear()
@@ -235,40 +268,43 @@
 
         checkpoint_after_root = nth(1, self._checkpoint_stack)
         self.commit_checkpoint(checkpoint_after_root)
 
     #
     # Database API
     #
-    def __getitem__(self, key: bytes) -> ChangesetValue:    # type: ignore # Breaks LSP
+    def __getitem__(self, key: bytes) -> ChangesetValue:  # type: ignore # Breaks LSP
         """
         For key lookups we need to iterate through the changesets in reverse
         order, returning from the first one in which the key is present.
         """
-        # the default result (the value if not in the local values) depends on whether there
-        # was a clear
+        # the default result (the value if not in the local values) depends on whether
+        # there was a clear
         if self._ignore_wrapped_db:
             default_result = REVERT_TO_WRAPPED
         else:
             default_result = None  # indicate that caller should check wrapped database
         return self._current_values.get(key, default_result)
 
     def __setitem__(self, key: bytes, value: bytes) -> None:
-        # if the value has not been changed since wrapping, then simply revert to original value
+        # if the value has not been changed since wrapping,
+        # then simply revert to original value
         revert_changeset = self._journal_data[self.last_checkpoint]
         if key not in revert_changeset:
             revert_changeset[key] = self._current_values.get(key, REVERT_TO_WRAPPED)
         self._current_values[key] = value
 
     def _exists(self, key: bytes) -> bool:
         val = self.get(key)
         return val is not None and val not in (REVERT_TO_WRAPPED, DELETE_WRAPPED)
 
     def __delitem__(self, key: bytes) -> None:
-        raise NotImplementedError("You must delete with one of delete_local or delete_wrapped")
+        raise NotImplementedError(
+            "You must delete with one of delete_local or delete_wrapped"
+        )
 
     def delete_wrapped(self, key: bytes) -> None:
         revert_changeset = self._journal_data[self.last_checkpoint]
         if key not in revert_changeset:
             revert_changeset[key] = self._current_values.get(key, REVERT_TO_WRAPPED)
         self._current_values[key] = DELETE_WRAPPED
 
@@ -302,39 +338,40 @@
     checkpoint.
     Commiting a checkpoint simply removes the option of reverting back to it
     later.
 
     Nothing is written to the underlying db until `persist()` is called.
 
     The added memory footprint for a JournalDB is one key/value stored per
-    database key which is changed, at each checkpoint.  Subsequent changes to the same key
-    between two checkpoints will not increase the journal size, since we
+    database key which is changed, at each checkpoint.  Subsequent changes to the same
+    key between two checkpoints will not increase the journal size, since we
     do not permit reverting to a place that has no checkpoint.
     """
-    __slots__ = ['_wrapped_db', '_journal', 'record', 'commit']
+
+    __slots__ = ["_wrapped_db", "_journal", "record", "commit"]
 
     def __init__(self, wrapped_db: DatabaseAPI) -> None:
         self._wrapped_db = wrapped_db
         self._journal = Journal()
         self.record = self._journal.record_checkpoint
         self.commit = self._journal.commit_checkpoint
         self.reset()
 
     def __getitem__(self, key: bytes) -> bytes:
-
         val = self._journal[key]
         if val is DELETE_WRAPPED:
             raise KeyError(
                 key,
                 "item is deleted in JournalDB, and will be deleted from the wrapped DB",
             )
         elif val is REVERT_TO_WRAPPED:
             raise KeyError(
                 key,
-                "item is deleted in JournalDB, and is presumed gone from the wrapped DB",
+                "item is deleted in JournalDB, "
+                "and is presumed gone from the wrapped DB",
             )
         elif val is None:
             return self._wrapped_db[key]
         else:
             # mypy doesn't allow custom type guards yet so we need to cast here
             # even though we know it can only be `bytes` at this point.
             return cast(bytes, val)
@@ -353,54 +390,55 @@
         elif val is None:
             return key in self._wrapped_db
         else:
             return True
 
     def clear(self) -> None:
         """
-        Remove all keys. Immediately after a clear, *all* getitem requests will return a KeyError.
-        That includes the changes pending persist and any data in the underlying database.
+        Remove all keys. Immediately after a clear, *all* getitem requests will return a
+        KeyError. That includes the changes pending persist and any data in the
+        underlying database.
 
         (This action is journaled, like all other actions)
 
         clear will *not* persist the emptying of all keys in the underlying DB.
         It only prevents any updates (or deletes!) before it from being persisted.
 
-        Any caller that wants to use clear must also make sure that the underlying database
-        reflects their desired end state (maybe emptied, maybe not).
+        Any caller that wants to use clear must also make sure that the underlying
+        database reflects their desired end state (maybe emptied, maybe not).
         """
         self._journal.clear()
 
     def has_clear(self) -> bool:
         return self._journal.has_clear(self._journal.root_checkpoint)
 
     def __delitem__(self, key: bytes) -> None:
         if key in self._wrapped_db:
             self._journal.delete_wrapped(key)
         else:
             if key in self._journal:
                 self._journal.delete_local(key)
             else:
-                raise KeyError(key, "key could not be deleted in JournalDB, because it was missing")
+                raise KeyError(
+                    key, "key could not be deleted in JournalDB, because it was missing"
+                )
 
     #
     # Snapshot API
     #
     def has_checkpoint(self, checkpoint: JournalDBCheckpoint) -> bool:
         return self._journal.has_checkpoint(checkpoint)
 
     def discard(self, checkpoint: JournalDBCheckpoint) -> None:
         """
         Throws away all journaled data starting at the given checkpoint
         """
         self._journal.discard(checkpoint)
 
-    def _reapply_checkpoint_to_journal(
-            self,
-            journal_data: ChangesetDict) -> None:
+    def _reapply_checkpoint_to_journal(self, journal_data: ChangesetDict) -> None:
         for key, value in journal_data.items():
             if value is DELETE_WRAPPED:
                 self._journal.delete_wrapped(key)
             elif value is REVERT_TO_WRAPPED:
                 self._journal.delete_local(key)
             else:
                 self._journal[key] = cast(bytes, value)
```

### Comparing `py-evm-0.7.0a1/eth/db/keymap.py` & `py-evm-0.7.0a2/eth/db/keymap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from abc import (
     abstractmethod,
 )
-
 from typing import (
     Any,
 )
 
-from eth.abc import DatabaseAPI
-from eth.db.backends.base import BaseDB
+from eth.abc import (
+    DatabaseAPI,
+)
+from eth.db.backends.base import (
+    BaseDB,
+)
 
 
 class KeyMapDB(BaseDB):
     """
     Modify keys when accessing the database, according to the
     abstract keymap function set in the subclass.
     """
+
     def __init__(self, db: DatabaseAPI) -> None:
         self._db = db
 
     @staticmethod
     @abstractmethod
     def keymap(key: bytes) -> bytes:
         raise NotImplementedError
@@ -31,19 +35,19 @@
         mapped_key = self.keymap(key)
         self._db[mapped_key] = val
 
     def __delitem__(self, key: bytes) -> None:
         mapped_key = self.keymap(key)
         del self._db[mapped_key]
 
-    def __contains__(self, key: bytes) -> bool:     # type: ignore # Breaks LSP
+    def __contains__(self, key: bytes) -> bool:  # type: ignore # Breaks LSP
         mapped_key = self.keymap(key)
         return mapped_key in self._db
 
     def __getattr__(self, attr: Any) -> Any:
         return getattr(self._db, attr)
 
     def __setattr__(self, attr: Any, val: Any) -> None:
-        if attr in ('_db', 'keymap'):
+        if attr in ("_db", "keymap"):
             super().__setattr__(attr, val)
         else:
             setattr(self._db, attr, val)
```

### Comparing `py-evm-0.7.0a1/eth/db/schema.py` & `py-evm-0.7.0a2/eth/db/schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 from eth_typing import (
     BlockNumber,
     Hash32,
 )
 
-from eth.abc import SchemaAPI
+from eth.abc import (
+    SchemaAPI,
+)
 
 
 class SchemaV1(SchemaAPI):
     @staticmethod
     def make_canonical_head_hash_lookup_key() -> bytes:
-        return b'v1:canonical_head_hash'
+        return b"v1:canonical_head_hash"
 
     @staticmethod
     def make_block_number_to_hash_lookup_key(block_number: BlockNumber) -> bytes:
-        number_to_hash_key = b'block-number-to-hash:%d' % block_number
+        number_to_hash_key = b"block-number-to-hash:%d" % block_number
         return number_to_hash_key
 
     @staticmethod
     def make_block_hash_to_score_lookup_key(block_hash: Hash32) -> bytes:
-        return b'block-hash-to-score:%s' % block_hash
+        return b"block-hash-to-score:%s" % block_hash
 
     @staticmethod
     def make_header_chain_gaps_lookup_key() -> bytes:
-        return b'v1:header_chain_gaps'
+        return b"v1:header_chain_gaps"
 
     @staticmethod
     def make_chain_gaps_lookup_key() -> bytes:
-        return b'v1:chain_gaps'
+        return b"v1:chain_gaps"
 
     @staticmethod
     def make_checkpoint_headers_key() -> bytes:
         """
         Checkpoint header hashes stored as concatenated 32 byte values
         """
-        return b'v1:checkpoint-header-hashes-list'
+        return b"v1:checkpoint-header-hashes-list"
 
     @staticmethod
     def make_transaction_hash_to_block_lookup_key(transaction_hash: Hash32) -> bytes:
-        return b'transaction-hash-to-block:%s' % transaction_hash
+        return b"transaction-hash-to-block:%s" % transaction_hash
 
     @staticmethod
     def make_withdrawal_hash_to_block_lookup_key(withdrawal_hash: Hash32) -> bytes:
-        return b'withdrawal-hash-to-block:%s' % withdrawal_hash
+        return b"withdrawal-hash-to-block:%s" % withdrawal_hash
```

### Comparing `py-evm-0.7.0a1/eth/db/slow_journal.py` & `py-evm-0.7.0a2/eth/db/slow_journal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 import collections
-from typing import cast, Dict, Set, Union
+from typing import (
+    Dict,
+    Set,
+    Union,
+    cast,
+)
 import uuid
 
+from eth_utils import (
+    ValidationError,
+)
 from eth_utils.toolz import (
     first,
     merge,
     nth,
 )
-from eth_utils import (
-    ValidationError,
-)
 
-from eth.abc import DatabaseAPI
-from eth.db.backends.base import BaseDB
-from eth.db.diff import DBDiff, DBDiffTracker
+from eth.abc import (
+    DatabaseAPI,
+)
+from eth.db.backends.base import (
+    BaseDB,
+)
+from eth.db.diff import (
+    DBDiff,
+    DBDiffTracker,
+)
 
 
 class DeletedEntry:
     pass
 
 
 # Track two different kinds of deletion:
@@ -42,15 +54,17 @@
     Changesets are referenced by a random uuid4.
     """
 
     def __init__(self) -> None:
         # contains a mapping from all of the `uuid4` changeset_ids
         # to a dictionary of key:value pairs with the recorded changes
         # that belong to the changeset
-        self.journal_data: collections.OrderedDict[uuid.UUID, Dict[bytes, Union[bytes, DeletedEntry]]] = collections.OrderedDict()  # noqa E501
+        self.journal_data: collections.OrderedDict[
+            uuid.UUID, Dict[bytes, Union[bytes, DeletedEntry]]
+        ] = collections.OrderedDict()
         self._clears_at: Set[uuid.UUID] = set()
 
     @property
     def root_changeset_id(self) -> uuid.UUID:
         """
         Returns the id of the root changeset
         """
@@ -64,15 +78,16 @@
         return len(self.journal_data) < 2
 
     @property
     def latest_id(self) -> uuid.UUID:
         """
         Returns the id of the latest changeset
         """
-        # last() was iterating through all values, so first(reversed()) gives a 12.5x speedup
+        # last() was iterating through all values, so first(reversed()) gives
+        # a 12.5x speedup
         return first(reversed(self.journal_data.keys()))
 
     @property
     def latest(self) -> Dict[bytes, Union[bytes, DeletedEntry]]:
         """
         Returns the dictionary of db keys and values for the latest changeset.
         """
@@ -95,94 +110,102 @@
         """
         Creates a new changeset. Changesets are referenced by a random uuid4
         to prevent collisions between multiple changesets.
         """
         if custom_changeset_id is not None:
             if custom_changeset_id in self.journal_data:
                 raise ValidationError(
-                    f"Tried to record with an existing changeset id: {custom_changeset_id!r}"
+                    "Tried to record with an existing "
+                    f"changeset id: {custom_changeset_id!r}"
                 )
             else:
                 changeset_id = custom_changeset_id
         else:
             changeset_id = uuid.uuid4()
 
         self.journal_data[changeset_id] = {}
         return changeset_id
 
-    def pop_changeset(self, changeset_id: uuid.UUID) -> Dict[bytes, Union[bytes, DeletedEntry]]:
+    def pop_changeset(
+        self, changeset_id: uuid.UUID
+    ) -> Dict[bytes, Union[bytes, DeletedEntry]]:
         """
         Returns all changes from the given changeset.  This includes all of
         the changes from any subsequent changeset, giving precedence to
         later changesets.
         """
         if changeset_id not in self.journal_data:
             raise KeyError(changeset_id, "Unknown changeset in JournalDB")
 
         all_ids = tuple(self.journal_data.keys())
         changeset_idx = all_ids.index(changeset_id)
         changesets_to_pop = all_ids[changeset_idx:]
-        popped_clears = tuple(idx for idx in changesets_to_pop if idx in self._clears_at)
+        popped_clears = tuple(
+            idx for idx in changesets_to_pop if idx in self._clears_at
+        )
         if popped_clears:
             last_clear_idx = changesets_to_pop.index(popped_clears[-1])
             changesets_to_drop = changesets_to_pop[:last_clear_idx]
             changesets_to_merge = changesets_to_pop[last_clear_idx:]
         else:
             changesets_to_drop = ()
             changesets_to_merge = changesets_to_pop
 
         # we pull all of the changesets *after* the changeset we are
         # reverting to and collapse them to a single set of keys (giving
         # precedence to later changesets)
-        changeset_data = merge(*(
-            self.journal_data.pop(c_id)
-            for c_id
-            in changesets_to_merge
-        ))
+        changeset_data = merge(
+            *(self.journal_data.pop(c_id) for c_id in changesets_to_merge)
+        )
 
-        # drop the changes on the floor if they came before a clear that is being committed
+        # drop the changes on the floor if they came before a clear that is
+        # being committed
         for changeset_id in changesets_to_drop:
             self.journal_data.pop(changeset_id)
 
         self._clears_at.difference_update(popped_clears)
         return changeset_data
 
     def clear(self) -> None:
         """
-        Treat as if the *underlying* database will also be cleared by some other mechanism.
-        We build a special empty changeset just for marking that all previous data should
-        be ignored.
+        Treat as if the *underlying* database will also be cleared by some other
+        mechanism. We build a special empty changeset just for marking that all
+        previous data should be ignored.
         """
         # these internal records are used as a way to tell the difference between
         # changes that came before and after the clear
         self.record_changeset()
         self._clears_at.add(self.latest_id)
         self.record_changeset()
 
     def has_clear(self, check_changeset_id: uuid.UUID) -> bool:
         for changeset_id in reversed(self.journal_data.keys()):
             if changeset_id in self._clears_at:
                 return True
             elif check_changeset_id == changeset_id:
                 return False
-        raise ValidationError("Changeset ID %s is not in the journal" % check_changeset_id)
-
-    def commit_changeset(self, changeset_id: uuid.UUID) -> Dict[bytes, Union[bytes, DeletedEntry]]:
+        raise ValidationError(
+            "Changeset ID %s is not in the journal" % check_changeset_id
+        )
+
+    def commit_changeset(
+        self, changeset_id: uuid.UUID
+    ) -> Dict[bytes, Union[bytes, DeletedEntry]]:
         """
         Collapses all changes for the given changeset into the previous
         changesets if it exists.
         """
         does_clear = self.has_clear(changeset_id)
         changeset_data = self.pop_changeset(changeset_id)
         if not self.is_empty():
             # we only have to assign changeset data into the latest changeset if
             # there is one.
             if does_clear:
-                # if there was a clear and more changesets underneath then clear the latest
-                # changeset, and replace with a new clear changeset
+                # if there was a clear and more changesets underneath then clear the
+                # latest changeset, and replace with a new clear changeset
                 self.latest = {}
                 self._clears_at.add(self.latest_id)
                 self.record_changeset()
                 self.latest = changeset_data
             else:
                 # otherwise, merge in all the current data
                 self.latest = merge(
@@ -197,15 +220,15 @@
 
         changeset_id_after_root = nth(1, self.journal_data.keys())
         self.commit_changeset(changeset_id_after_root)
 
     #
     # Database API
     #
-    def __getitem__(self, key: bytes) -> Union[bytes, DeletedEntry]:    # type: ignore # Breaks LSP
+    def __getitem__(self, key: bytes) -> Union[bytes, DeletedEntry]:  # type: ignore # Breaks LSP  # noqa: E501
         """
         For key lookups we need to iterate through the changesets in reverse
         order, returning from the first one in which the key is present.
         """
         # Ignored from mypy because of https://github.com/python/typeshed/issues/2078
         for changeset_id, changeset_data in reversed(self.journal_data.items()):
             if changeset_id in self._clears_at:
@@ -221,29 +244,32 @@
         self.latest[key] = value
 
     def _exists(self, key: bytes) -> bool:
         val = self.get(key)
         return val is not None and val not in (ERASE_CREATED_ENTRY, DELETED_ENTRY)
 
     def __delitem__(self, key: bytes) -> None:
-        raise NotImplementedError("You must delete with one of delete_local or delete_wrapped")
+        raise NotImplementedError(
+            "You must delete with one of delete_local or delete_wrapped"
+        )
 
     def delete_wrapped(self, key: bytes) -> None:
         self.latest[key] = DELETED_ENTRY
 
     def delete_local(self, key: bytes) -> None:
         self.latest[key] = ERASE_CREATED_ENTRY
 
     def diff(self) -> DBDiff:
         tracker = DBDiffTracker()
         visited_keys: Set[bytes] = set()
 
         # Iterate in reverse, so you can skip over any keys from old checkpoints.
-        # This is required so that when a key is created and then deleted in the journal,
-        #   we don't add the delete to the diff. (We simply omit the change altogether)
+        # This is required so that when a key is created and then deleted in the
+        #   journal, we don't add the delete to the diff.
+        #   (We simply omit the change altogether)
         for changeset_id, changeset in reversed(self.journal_data.items()):
             if changeset_id in self._clears_at:
                 break
 
             for key, value in changeset.items():
                 if key in visited_keys:
                     # this old change has already been tracked
@@ -275,33 +301,34 @@
     Nothing is written to the underlying db until `persist()` is called.
 
     The added memory footprint for a JournalDB is one key/value stored per
     database key which is changed.  Subsequent changes to the same key within
     the same changeset will not increase the journal size since we only need
     to track latest value for any given key within any given changeset.
     """
+
     wrapped_db = None
     journal: Journal = None
 
     def __init__(self, wrapped_db: DatabaseAPI) -> None:
         self.wrapped_db = wrapped_db
         self.reset()
 
     def __getitem__(self, key: bytes) -> bytes:
-
         val = self.journal[key]
         if val is DELETED_ENTRY:
             raise KeyError(
                 key,
                 "item is deleted in JournalDB, and will be deleted from the wrapped DB",
             )
         elif val is ERASE_CREATED_ENTRY:
             raise KeyError(
                 key,
-                "item is deleted in JournalDB, and is presumed gone from the wrapped DB",
+                "item is deleted in JournalDB, and is presumed gone "
+                "from the wrapped DB",
             )
         elif val is None:
             return self.wrapped_db[key]
         else:
             # mypy doesn't allow custom type guards yet so we need to cast here
             # even though we know it can only be `bytes` at this point.
             return cast(bytes, val)
@@ -320,48 +347,53 @@
         elif val is None:
             return key in self.wrapped_db
         else:
             return True
 
     def clear(self) -> None:
         """
-        Remove all keys. Immediately after a clear, *all* getitem requests will return a KeyError.
-        That includes the changes pending persist and any data in the underlying database.
+        Remove all keys. Immediately after a clear, *all* getitem requests will
+        return a KeyError. That includes the changes pending persist and any data
+        in the underlying database.
 
         (This action is journaled, like all other actions)
 
         clear will *not* persist the emptying of all keys in the underlying DB.
         It only prevents any updates (or deletes!) before it from being persisted.
 
-        Any caller that wants to use clear must also make sure that the underlying database
-        reflects their desired end state (maybe emptied, maybe not).
+        Any caller that wants to use clear must also make sure that the underlying
+        database reflects their desired end state (maybe emptied, maybe not).
         """
         self.journal.clear()
 
     def has_clear(self) -> bool:
         return self.journal.has_clear(self.journal.root_changeset_id)
 
     def __delitem__(self, key: bytes) -> None:
         if key in self.wrapped_db:
             self.journal.delete_wrapped(key)
         else:
             if key in self.journal:
                 self.journal.delete_local(key)
             else:
-                raise KeyError(key, "key could not be deleted in JournalDB, because it was missing")
+                raise KeyError(
+                    key, "key could not be deleted in JournalDB, because it was missing"
+                )
 
     #
     # Snapshot API
     #
     def _validate_changeset(self, changeset_id: uuid.UUID) -> None:
         """
         Checks to be sure the changeset is known by the journal
         """
         if not self.journal.has_changeset(changeset_id):
-            raise ValidationError(f"Changeset not found in journal: {str(changeset_id)}")
+            raise ValidationError(
+                f"Changeset not found in journal: {str(changeset_id)}"
+            )
 
     def has_changeset(self, changeset_id: uuid.UUID) -> bool:
         return self.journal.has_changeset(changeset_id)
 
     def record(self, custom_changeset_id: uuid.UUID = None) -> uuid.UUID:
         """
         Starts a new recording and returns an id for the associated changeset
@@ -380,23 +412,24 @@
         Commits a given changeset. This merges the given changeset and all
         subsequent changesets into the previous changeset giving precidence
         to later changesets in case of any conflicting keys.
         """
         self._validate_changeset(changeset_id)
         if changeset_id == self.journal.root_changeset_id:
             raise ValidationError(
-                "Tried to commit the root changeset. Callers should not keep references "
-                "to the root changeset. Maybe you meant to use persist()?"
+                "Tried to commit the root changeset. Callers should not keep references"
+                " to the root changeset. Maybe you meant to use persist()?"
             )
         self.journal.commit_changeset(changeset_id)
 
     def _reapply_changeset_to_journal(
-            self,
-            changeset_id: uuid.UUID,
-            journal_data: Dict[bytes, Union[bytes, DeletedEntry]]) -> None:
+        self,
+        changeset_id: uuid.UUID,
+        journal_data: Dict[bytes, Union[bytes, DeletedEntry]],
+    ) -> None:
         self.record(changeset_id)
         for key, value in journal_data.items():
             if value is DELETED_ENTRY:
                 self.journal.delete_wrapped(key)
             elif value is ERASE_CREATED_ENTRY:
                 self.journal.delete_local(key)
             else:
```

### Comparing `py-evm-0.7.0a1/eth/db/storage.py` & `py-evm-0.7.0a2/eth/db/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import (
     FrozenSet,
     List,
     NamedTuple,
     Set,
 )
 
-from eth_hash.auto import keccak
+from eth_hash.auto import (
+    keccak,
+)
 from eth_typing import (
     Address,
     Hash32,
 )
 from eth_utils import (
     ValidationError,
     encode_hex,
@@ -46,50 +48,53 @@
 )
 from eth.db.cache import (
     CacheDB,
 )
 from eth.db.journal import (
     JournalDB,
 )
-from eth.vm.interrupt import (
-    MissingStorageTrieNode,
-)
 from eth.typing import (
     JournalDBCheckpoint,
 )
+from eth.vm.interrupt import (
+    MissingStorageTrieNode,
+)
 
 
 class PendingWrites(NamedTuple):
     """
     A set of variables captured just before account storage deletion.
     The variables are used to revive storage if the EVM reverts to a point
     prior to deletion.
     """
+
     write_trie: HexaryTrie  # The write trie at the time of deletion
     trie_nodes_batch: BatchDB  # A batch of all trie nodes written to the trie
     starting_root_hash: Hash32  # The starting root hash
 
 
 class StorageLookup(BaseDB):
     """
-    This lookup converts lookups of storage slot integers into the appropriate trie lookup.
-    Similarly, it persists changes to the appropriate trie at write time.
+    This lookup converts lookups of storage slot integers into the appropriate trie
+    lookup. Similarly, it persists changes to the appropriate trie at write time.
 
     StorageLookup also tracks the state roots changed since the last persist.
     """
+
     logger = get_extended_debug_logger("eth.db.storage.StorageLookup")
 
     # The trie that is modified in-place, used to calculate storage root on-demand
     _write_trie: HexaryTrie
 
     # These are the new trie nodes, waiting to be committed to disk
     _trie_nodes_batch: BatchDB
 
     # When deleting an account, push the pending write info onto this stack.
-    # This stack can get as big as the number of transactions per block: one for each delete.
+    # This stack can get as big as the number of transactions per block: one for
+    # each delete.
     _historical_write_tries: List[PendingWrites]
 
     def __init__(self, db: DatabaseAPI, storage_root: Hash32, address: Address) -> None:
         self._db = db
 
         # Set the starting root hash, to be used for on-disk storage read lookups
         self._initialize_to_root_hash(storage_root)
@@ -98,15 +103,17 @@
 
     def _get_write_trie(self) -> HexaryTrie:
         if self._trie_nodes_batch is None:
             self._trie_nodes_batch = BatchDB(self._db, read_through_deletes=True)
 
         if self._write_trie is None:
             batch_db = self._trie_nodes_batch
-            self._write_trie = HexaryTrie(batch_db, root_hash=self._starting_root_hash, prune=True)
+            self._write_trie = HexaryTrie(
+                batch_db, root_hash=self._starting_root_hash, prune=True
+            )
 
         return self._write_trie
 
     def _get_read_trie(self) -> HexaryTrie:
         if self._write_trie is not None:
             return self._write_trie
         else:
@@ -162,35 +169,38 @@
     def has_changed_root(self) -> bool:
         return self._write_trie is not None
 
     def get_changed_root(self) -> Hash32:
         if self._write_trie is not None:
             return self._write_trie.root_hash
         else:
-            raise ValidationError("Asked for changed root when no writes have been made")
+            raise ValidationError(
+                "Asked for changed root when no writes have been made"
+            )
 
     def _initialize_to_root_hash(self, root_hash: Hash32) -> None:
         self._starting_root_hash = root_hash
         self._write_trie = None
         self._trie_nodes_batch = None
 
         # Reset the historical writes, which can't be reverted after committing
         self._historical_write_tries = []
 
     def commit_to(self, db: DatabaseAPI) -> None:
         """
         Trying to commit changes when nothing has been written will raise a
         ValidationError
         """
-        self.logger.debug2('persist storage root to data store')
+        self.logger.debug2("persist storage root to data store")
         if self._trie_nodes_batch is None:
             raise ValidationError(
-                "It is invalid to commit an account's storage if it has no pending changes. "
-                "Always check storage_lookup.has_changed_root before attempting to commit. "
-                f"Write tries on stack = {len(self._historical_write_tries)}; Root hash = "
+                "It is invalid to commit an account's storage if it has no pending "
+                "changes. Always check storage_lookup.has_changed_root before "
+                "attempting to commit. Write tries on stack = "
+                f"{len(self._historical_write_tries)}; Root hash = "
                 f"{encode_hex(self._starting_root_hash)}"
             )
         self._trie_nodes_batch.commit_to(db, apply_deletes=False)
 
         # Mark the trie as having been all written out to the database.
         # It removes the 'dirty' flag and clears out any pending writes.
         self._initialize_to_root_hash(self._write_trie.root_hash)
@@ -201,19 +211,21 @@
         case of a revert.
 
         :return: index for reviving the previous trie
         """
         write_trie = self._get_write_trie()
 
         # Write the previous trie into a historical stack
-        self._historical_write_tries.append(PendingWrites(
-            write_trie,
-            self._trie_nodes_batch,
-            self._starting_root_hash,
-        ))
+        self._historical_write_tries.append(
+            PendingWrites(
+                write_trie,
+                self._trie_nodes_batch,
+                self._starting_root_hash,
+            )
+        )
 
         new_idx = len(self._historical_write_tries)
         self._starting_root_hash = BLANK_ROOT_HASH
         self._write_trie = None
         self._trie_nodes_batch = None
 
         return new_idx
@@ -225,94 +237,97 @@
         to the trie in place *before* the call.
 
         :param trie_index: index for reviving the previous trie
         """
 
         if trie_index >= len(self._historical_write_tries):
             raise ValidationError(
-                f"Trying to roll back a delete to index {trie_index}, but there are only"
-                f" {len(self._historical_write_tries)} indices available."
+                f"Trying to roll back a delete to index {trie_index}, but there are "
+                f"only {len(self._historical_write_tries)} indices available."
             )
 
         (
             self._write_trie,
             self._trie_nodes_batch,
             self._starting_root_hash,
         ) = self._historical_write_tries[trie_index]
 
         # Cannot roll forward after a rollback, so remove created/ignored tries.
         # This also deletes the trie that you just reverted to. It will be re-added
         # to the stack when the next new_trie() is called.
         del self._historical_write_tries[trie_index:]
 
 
-CLEAR_COUNT_KEY_NAME = b'clear-count'
+CLEAR_COUNT_KEY_NAME = b"clear-count"
 
 
 class AccountStorageDB(AccountStorageDatabaseAPI):
     logger = get_extended_debug_logger("eth.db.storage.AccountStorageDB")
 
-    def __init__(self, db: AtomicDatabaseAPI, storage_root: Hash32, address: Address) -> None:
+    def __init__(
+        self, db: AtomicDatabaseAPI, storage_root: Hash32, address: Address
+    ) -> None:
         """
         Database entries go through several pipes, like so...
 
         .. code::
 
-            db -> _storage_lookup -> _storage_cache -> _locked_changes -> _journal_storage
+          db -> _storage_lookup -> _storage_cache -> _locked_changes -> _journal_storage
 
         db is the raw database, we can assume it hits disk when written to.
         Keys are stored as node hashes and rlp-encoded node values.
 
         _storage_lookup is itself a pair of databases: (BatchDB -> HexaryTrie),
         writes to storage lookup *are* immeditaely applied to a trie, generating
         the appropriate trie nodes and and root hash (via the HexaryTrie). The
-        writes are *not* persisted to db, until _storage_lookup is explicitly instructed to,
-        via :meth:`StorageLookup.commit_to`
+        writes are *not* persisted to db, until _storage_lookup is explicitly instructed
+        to, via :meth:`StorageLookup.commit_to`
 
         _storage_cache is a cache tied to the state root of the trie. It
         is important that this cache is checked *after* looking for
         the key in _journal_storage, because the cache is only invalidated
         after a state root change. Otherwise, you will see data since the last
         storage root was calculated.
 
         _locked_changes is a batch database that includes only those values that are
         un-revertable in the EVM. Currently, that means changes that completed in a
         previous transaction.
 
-        Journaling batches writes at the _journal_storage layer, until persist is called.
-        It manages all the checkpointing and rollbacks that happen during EVM execution.
+        Journaling batches writes at the _journal_storage layer, until persist is
+        called. It manages all the checkpointing and rollbacks that happen during
+        EVM execution.
 
         In both _storage_cache and _journal_storage, Keys are set/retrieved as the
         big_endian encoding of the slot integer, and the rlp-encoded value.
         """
         self._address = address
         self._storage_lookup = StorageLookup(db, storage_root, address)
         self._storage_cache = CacheDB(self._storage_lookup)
         self._locked_changes = JournalDB(self._storage_cache)
         self._journal_storage = JournalDB(self._locked_changes)
         self._accessed_slots: Set[int] = set()
 
         # Track how many times we have cleared the storage. This is journaled
         # in lockstep with other storage changes. That way, we can detect if a revert
-        # causes use to revert past the previous storage deletion. The clear count is used
-        # as an index to find the base trie from before the revert.
+        # causes use to revert past the previous storage deletion. The clear count is
+        # used as an index to find the base trie from before the revert.
         self._clear_count = JournalDB(MemoryDB({CLEAR_COUNT_KEY_NAME: to_bytes(0)}))
 
     def get(self, slot: int, from_journal: bool = True) -> int:
         self._accessed_slots.add(slot)
         key = int_to_big_endian(slot)
         lookup_db = self._journal_storage if from_journal else self._locked_changes
         try:
             encoded_value = lookup_db[key]
         except MissingStorageTrieNode:
             raise
         except KeyError:
             return 0
 
-        if encoded_value == b'':
+        if encoded_value == b"":
             return 0
         else:
             return rlp.decode(encoded_value, sedes=rlp.sedes.big_endian_int)
 
     def set(self, slot: int, value: int) -> None:
         key = int_to_big_endian(slot)
         if value:
@@ -320,15 +335,15 @@
         else:
             try:
                 current_val = self._journal_storage[key]
             except KeyError:
                 # deleting an empty key has no effect
                 return
             else:
-                if current_val != b'':
+                if current_val != b"":
                     # only try to delete the value if it's present
                     del self._journal_storage[key]
 
     def delete(self) -> None:
         self.logger.debug2(
             "Deleting all storage in account 0x%s",
             self._address.hex(),
@@ -343,26 +358,27 @@
         # This can happen multiple times in one block, via CREATE2.
         old_clear_count = to_int(self._clear_count[CLEAR_COUNT_KEY_NAME])
 
         # Gut check that we have incremented correctly
         if new_clear_count != old_clear_count + 1:
             raise ValidationError(
                 f"Must increase clear count by one on each delete. Instead, went from"
-                f" {old_clear_count} -> {new_clear_count} in account 0x{self._address.hex()}"
+                f" {old_clear_count} -> {new_clear_count} in account"
+                f" 0x{self._address.hex()}"
             )
 
         # Save the new count, ie~ the index used for a future revert.
         self._clear_count[CLEAR_COUNT_KEY_NAME] = to_bytes(new_clear_count)
 
     def record(self, checkpoint: JournalDBCheckpoint) -> None:
         self._journal_storage.record(checkpoint)
         self._clear_count.record(checkpoint)
 
     def discard(self, checkpoint: JournalDBCheckpoint) -> None:
-        self.logger.debug2('discard checkpoint %r', checkpoint)
+        self.logger.debug2("discard checkpoint %r", checkpoint)
         latest_clear_count = to_int(self._clear_count[CLEAR_COUNT_KEY_NAME])
 
         if self._journal_storage.has_checkpoint(checkpoint):
             self._journal_storage.discard(checkpoint)
             self._clear_count.discard(checkpoint)
         else:
             # if the checkpoint comes before this account started tracking,
@@ -383,15 +399,16 @@
             pass
         else:
             # Although CREATE2 permits multiple creates and deletes in a single block,
             #   you can still only revert across a single delete. That's because delete
             #   is only triggered at the end of the transaction.
             raise ValidationError(
                 f"This revert has changed the clear count in an invalid way, from"
-                f" {latest_clear_count} to {reverted_clear_count}, in 0x{self._address.hex()}"
+                f" {latest_clear_count} to {reverted_clear_count}, in"
+                f" 0x{self._address.hex()}"
             )
 
     def commit(self, checkpoint: JournalDBCheckpoint) -> None:
         if self._journal_storage.has_checkpoint(checkpoint):
             self._journal_storage.commit(checkpoint)
             self._clear_count.commit(checkpoint)
         else:
@@ -412,15 +429,16 @@
     def _validate_flushed(self) -> None:
         """
         Will raise an exception if there are some changes made since the last persist.
         """
         journal_diff = self._journal_storage.diff()
         if len(journal_diff) > 0:
             raise ValidationError(
-                f"StorageDB had a dirty journal when it needed to be clean: {journal_diff!r}"
+                "StorageDB had a dirty journal when it needed to be "
+                f"clean: {journal_diff!r}"
             )
 
     def get_accessed_slots(self) -> FrozenSet[int]:
         return frozenset(self._accessed_slots)
 
     @property
     def has_changed_root(self) -> bool:
```

### Comparing `py-evm-0.7.0a1/eth/db/trie.py` & `py-evm-0.7.0a2/eth/db/trie.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import functools
-from typing import Dict, Sequence, Tuple, Union
+from typing import (
+    Dict,
+    Sequence,
+    Tuple,
+    Union,
+)
 
+from eth_typing import (
+    Hash32,
+)
 import rlp
 from trie import (
     HexaryTrie,
 )
 
-from eth_typing import Hash32
-
 from eth.abc import (
     ReceiptAPI,
     SignedTransactionAPI,
     WithdrawalAPI,
 )
 from eth.constants import (
     BLANK_ROOT_HASH,
@@ -23,18 +29,18 @@
 TrieRootAndData = Tuple[Hash32, Dict[Hash32, bytes]]
 
 
 def make_trie_root_and_nodes(items: BlockRootData) -> TrieRootAndData:
     return _make_trie_root_and_nodes(tuple(item.encode() for item in items))
 
 
-# This cache is expected to be useful when importing blocks as we call this once when importing
-# and again when validating the imported block. But it should also help for post-Byzantium blocks
-# as it's common for them to have duplicate receipt_roots. Given that, it probably makes sense to
-# use a relatively small cache size here.
+# This cache is expected to be useful when importing blocks as we call this once when'
+# importing and again when validating the imported block. But it should also help for
+# post-Byzantium blocks as it's common for them to have duplicate receipt_roots.
+# Given that, it probably makes sense to use a relatively small cache size here.
 @functools.lru_cache(128)
 def _make_trie_root_and_nodes(items: Tuple[bytes, ...]) -> TrieRootAndData:
     kv_store: Dict[Hash32, bytes] = {}
     trie = HexaryTrie(kv_store, BLANK_ROOT_HASH)
     with trie.squash_changes() as memory_trie:
         for index, item in enumerate(items):
             index_key = rlp.encode(index, sedes=rlp.sedes.big_endian_int)
```

### Comparing `py-evm-0.7.0a1/eth/db/witness.py` & `py-evm-0.7.0a2/eth/db/witness.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 class AccountQueryTracker(NamedTuple):
     did_query_bytecode: bool
     slots_queried: FrozenSet[int]
 
 
 class MetaWitness(MetaWitnessAPI):
     def __init__(
-            self,
-            witness_hashes: Set[Hash32],
-            accounts_metadata_queried: Dict[Address, AccountQueryTracker]) -> None:
-
+        self,
+        witness_hashes: Set[Hash32],
+        accounts_metadata_queried: Dict[Address, AccountQueryTracker],
+    ) -> None:
         self._trie_node_hashes = frozenset(witness_hashes)
         self._accounts_metadata_queried = accounts_metadata_queried
 
     @property
     def hashes(self) -> FrozenSet[Hash32]:
         return self._trie_node_hashes
```

### Comparing `py-evm-0.7.0a1/eth/estimators/__init__.py` & `py-evm-0.7.0a2/eth/estimators/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,13 @@
 from eth._utils.module_loading import (
     import_string,
 )
 
 
 def get_gas_estimator() -> Callable[[StateAPI, SignedTransactionAPI], int]:
     import_path = os.environ.get(
-        'GAS_ESTIMATOR_BACKEND_FUNC',
-        'eth.estimators.gas.binary_gas_search_intrinsic_tolerance',
+        "GAS_ESTIMATOR_BACKEND_FUNC",
+        "eth.estimators.gas.binary_gas_search_intrinsic_tolerance",
     )
     return cast(
-        Callable[[StateAPI, SignedTransactionAPI], int],
-        import_string(import_path)
+        Callable[[StateAPI, SignedTransactionAPI], int], import_string(import_path)
     )
```

### Comparing `py-evm-0.7.0a1/eth/estimators/gas.py` & `py-evm-0.7.0a2/eth/estimators/gas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,92 +1,114 @@
-from typing import cast, Optional
-
-from eth_utils.toolz import curry
+from typing import (
+    Optional,
+    cast,
+)
 
-from eth.exceptions import VMError
+from eth_utils.toolz import (
+    curry,
+)
 
 from eth.abc import (
     SignedTransactionAPI,
     StateAPI,
 )
-from eth.vm.spoof import SpoofTransaction
-
+from eth.exceptions import (
+    VMError,
+)
+from eth.vm.spoof import (
+    SpoofTransaction,
+)
 
-def _get_computation_error(state: StateAPI, transaction: SignedTransactionAPI) -> Optional[VMError]:
 
+def _get_computation_error(
+    state: StateAPI, transaction: SignedTransactionAPI
+) -> Optional[VMError]:
     snapshot = state.snapshot()
 
     try:
         computation = state.apply_transaction(transaction)
         if computation.is_error:
             return computation.error
         else:
             return None
 
     finally:
         state.revert(snapshot)
 
 
 @curry
-def binary_gas_search(state: StateAPI,
-                      transaction: SignedTransactionAPI,
-                      tolerance: int = 1) -> int:
+def binary_gas_search(
+    state: StateAPI, transaction: SignedTransactionAPI, tolerance: int = 1
+) -> int:
     """
     Run the transaction with various gas limits, progressively
     approaching the minimum needed to succeed without an OutOfGas exception.
 
     The starting range of possible estimates is:
     [transaction.intrinsic_gas, state.gas_limit].
-    After the first OutOfGas exception, the range is: (largest_limit_out_of_gas, state.gas_limit].
-    After the first run not out of gas, the range is: (largest_limit_out_of_gas, smallest_success].
+    After the first OutOfGas exception, the range is:
+        (largest_limit_out_of_gas, state.gas_limit].
+    After the first run not out of gas, the range is:
+        (largest_limit_out_of_gas, smallest_success].
 
     :param int tolerance: When the range of estimates is less than tolerance,
         return the top of the range.
     :returns int: The smallest confirmed gas to not throw an OutOfGas exception,
         subject to tolerance. If OutOfGas is thrown at block limit, return block limit.
-    :raises VMError: if the computation fails even when given the block gas_limit to complete
+    :raises VMError: if the computation fails even when given the block gas_limit to
+        complete
     """
-    if not hasattr(transaction, 'sender'):
+    if not hasattr(transaction, "sender"):
         raise TypeError(
             "Transaction is missing attribute sender.",
             "If sending an unsigned transaction, use SpoofTransaction and provide the",
-            "sender using the 'from' parameter")
+            "sender using the 'from' parameter",
+        )
 
-    minimum_transaction = cast(SignedTransactionAPI, SpoofTransaction(
-        transaction,
-        gas=transaction.intrinsic_gas,
-        gas_price=0,
-    ))
+    minimum_transaction = cast(
+        SignedTransactionAPI,
+        SpoofTransaction(
+            transaction,
+            gas=transaction.intrinsic_gas,
+            gas_price=0,
+        ),
+    )
 
     if _get_computation_error(state, minimum_transaction) is None:
         return transaction.intrinsic_gas
 
-    maximum_transaction = cast(SignedTransactionAPI, SpoofTransaction(
-        transaction,
-        gas=state.gas_limit,
-        gas_price=0,
-    ))
+    maximum_transaction = cast(
+        SignedTransactionAPI,
+        SpoofTransaction(
+            transaction,
+            gas=state.gas_limit,
+            gas_price=0,
+        ),
+    )
     error = _get_computation_error(state, maximum_transaction)
     if error is not None:
         raise error
 
     minimum_viable = state.gas_limit
     maximum_out_of_gas = transaction.intrinsic_gas
     while minimum_viable - maximum_out_of_gas > tolerance:
         midpoint = (minimum_viable + maximum_out_of_gas) // 2
-        test_transaction = cast(SignedTransactionAPI, SpoofTransaction(transaction, gas=midpoint))
+        test_transaction = cast(
+            SignedTransactionAPI, SpoofTransaction(transaction, gas=midpoint)
+        )
         if _get_computation_error(state, test_transaction) is None:
             minimum_viable = midpoint
         else:
             maximum_out_of_gas = midpoint
 
     return minimum_viable
 
 
 # Estimate in increments of intrinsic gas usage
 binary_gas_search_intrinsic_tolerance = binary_gas_search(tolerance=21000)
 
-# Estimate in increments of 1000 gas, takes roughly 5 more executions than intrinsic to estimate
+# Estimate in increments of 1000 gas, takes roughly 5 more executions than
+# intrinsic to estimate
 binary_gas_search_1000_tolerance = binary_gas_search(tolerance=1000)
 
 # Estimate to the exact gas, takes roughly 15 more executions than intrinsic to estimate
 binary_gas_search_exact = binary_gas_search(tolerance=1)
```

### Comparing `py-evm-0.7.0a1/eth/exceptions.py` & `py-evm-0.7.0a2/eth/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-from eth_typing import Hash32
+from eth_typing import (
+    Hash32,
+)
 
 
 class PyEVMError(Exception):
     """
     Base class for all py-evm errors.
     """
+
     pass
 
 
 class VMNotFound(PyEVMError):
     """
     Raised when no VM is available for the provided block number.
     """
+
     pass
 
 
 class StateRootNotFound(PyEVMError):
     """
     Raised when the requested state root is not present in our DB.
     """
+
     @property
     def missing_state_root(self) -> Hash32:
         return self.args[0]
 
 
 class HeaderNotFound(PyEVMError):
     """
@@ -32,174 +37,198 @@
 
 class BlockNotFound(PyEVMError):
     """
     Raised when the block with the given number/hash does not exist.
     This will happen, for example, if the transactions or uncles are not
     saved in the database.
     """
+
     pass
 
 
 class TransactionNotFound(PyEVMError):
     """
     Raised when the transaction with the given hash or block index does not exist.
     """
+
     pass
 
 
 class UnrecognizedTransactionType(PyEVMError):
     """
     Raised when an encoded transaction is using a first byte that is valid, but
     unrecognized. According to EIP 2718, the byte may be in the range [0, 0x7f].
     As of the Berlin hard fork, all of those versions are undefined, except for
     0x01 in EIP 2930.
     """
+
     @property
     def type_int(self) -> int:
         return self.args[0]
 
 
 class ReceiptNotFound(PyEVMError):
     """
     Raised when the Receipt with the given receipt index does not exist.
     """
+
     pass
 
 
 class ParentNotFound(HeaderNotFound):
     """
     Raised when the parent of a given block does not exist.
     """
+
     pass
 
 
 class CanonicalHeadNotFound(PyEVMError):
     """
     Raised when the chain has no canonical head.
     """
+
     pass
 
 
 class GapTrackingCorrupted(PyEVMError):
     """
-    Raised when the tracking of chain gaps appears to be corrupted (e.g. overlapping gaps)
+    Raised when the tracking of chain gaps appears to be corrupted
+    (e.g. overlapping gaps)
     """
+
     pass
 
 
 class CheckpointsMustBeCanonical(PyEVMError):
     """
     Raised when a persisted header attempts to de-canonicalize a checkpoint
     """
+
     pass
 
 
 class Halt(PyEVMError):
     """
     Raised when an opcode function halts vm execution.
     """
+
     pass
 
 
 class VMError(PyEVMError):
     """
     Base class for errors raised during VM execution.
     """
+
     burns_gas = True
     erases_return_data = True
 
 
 class OutOfGas(VMError):
     """
     Raised when a VM execution has run out of gas.
     """
+
     pass
 
 
 class InsufficientStack(VMError):
     """
     Raised when the stack is empty.
     """
+
     pass
 
 
 class FullStack(VMError):
     """
     Raised when the stack is full.
     """
+
     pass
 
 
 class InvalidJumpDestination(VMError):
     """
     Raised when the jump destination for a JUMPDEST operation is invalid.
     """
+
     pass
 
 
 class InvalidInstruction(VMError):
     """
     Raised when an opcode is invalid.
     """
+
     pass
 
 
 class InsufficientFunds(VMError):
     """
     Raised when an account has insufficient funds to transfer the
     requested value.
     """
+
     pass
 
 
 class StackDepthLimit(VMError):
     """
     Raised when the call stack has exceeded it's maximum allowed depth.
     """
+
     pass
 
 
 class ContractCreationCollision(VMError):
     """
     Raised when there was an address collision during contract creation.
     """
+
     pass
 
 
 class IncorrectContractCreationAddress(VMError):
     """
     Raised when the address provided by transaction does not
     match the calculated contract creation address.
     """
+
     pass
 
 
 class Revert(VMError):
     """
     Raised when the REVERT opcode occured
     """
+
     burns_gas = False
     erases_return_data = False
 
 
 class WriteProtection(VMError):
     """
     Raised when an attempt to modify the state database is made while
     operating inside of a STATICCALL context.
     """
+
     pass
 
 
 class OutOfBoundsRead(VMError):
     """
     Raised when an attempt was made to read data beyond the
     boundaries of the buffer (such as with RETURNDATACOPY)
     """
+
     pass
 
 
 class ReservedBytesInCode(VMError):
     """
     Raised when bytes for the code to be deployed are reserved
     for a particular reason.
     """
+
     pass
```

### Comparing `py-evm-0.7.0a1/eth/precompiles/blake2.py` & `py-evm-0.7.0a2/eth/precompiles/blake2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 from eth_utils import (
     ValidationError,
 )
 
-from eth._utils.blake2.coders import extract_blake2b_parameters
+from eth._utils.blake2.coders import (
+    extract_blake2b_parameters,
+)
+from eth.abc import (
+    ComputationAPI,
+)
 from eth.exceptions import (
     VMError,
 )
-from eth.vm.computation import (
-    BaseComputation,
-)
 
 try:
-    from blake2b import compress as blake2b_compress
+    from blake2b import (
+        compress as blake2b_compress,
+    )
 except ImportError:
-    from eth._utils.blake2.compression import blake2b_compress
+    from eth._utils.blake2.compression import (
+        blake2b_compress,
+    )
 
 GAS_COST_PER_ROUND = 1
 
 
-def blake2b_fcompress(computation: BaseComputation) -> BaseComputation:
+def blake2b_fcompress(computation: ComputationAPI) -> ComputationAPI:
     try:
         parameters = extract_blake2b_parameters(computation.msg.data_as_bytes)
     except ValidationError as exc:
         raise VMError(f"Blake2b input parameter validation failure: {exc}") from exc
 
     num_rounds = parameters[0]
     gas_cost = GAS_COST_PER_ROUND * num_rounds
 
-    computation.consume_gas(gas_cost, reason=f"Blake2b Compress Precompile w/ {num_rounds} rounds")
+    computation.consume_gas(
+        gas_cost, reason=f"Blake2b Compress Precompile w/ {num_rounds} rounds"
+    )
 
     computation.output = blake2b_compress(*parameters)
     return computation
```

### Comparing `py-evm-0.7.0a1/eth/precompiles/ecadd.py` & `py-evm-0.7.0a2/eth/precompiles/ecadd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,59 @@
-from typing import Tuple
-
-from py_ecc import (
-    optimized_bn128 as bn128,
+from typing import (
+    Tuple,
 )
 
 from eth_utils import (
     ValidationError,
     big_endian_to_int,
     int_to_big_endian,
 )
 from eth_utils.toolz import (
     curry,
 )
+from py_ecc import (
+    optimized_bn128 as bn128,
+)
 
-from eth import constants
-
-from eth.exceptions import (
-    VMError,
+from eth import (
+    constants,
 )
 from eth._utils.bn128 import (
     validate_point,
 )
 from eth._utils.padding import (
     pad32,
     pad32r,
 )
-
-from eth.vm.computation import (
-    BaseComputation,
+from eth.abc import (
+    ComputationAPI,
+)
+from eth.exceptions import (
+    VMError,
 )
 
 
 @curry
 def ecadd(
-        computation: BaseComputation,
-        gas_cost: int = constants.GAS_ECADD) -> BaseComputation:
-
-    computation.consume_gas(gas_cost, reason='ECADD Precompile')
+    computation: ComputationAPI, gas_cost: int = constants.GAS_ECADD
+) -> ComputationAPI:
+    computation.consume_gas(gas_cost, reason="ECADD Precompile")
 
     try:
         result = _ecadd(computation.msg.data_as_bytes)
     except ValidationError:
         raise VMError("Invalid ECADD parameters")
 
     result_x, result_y = result
-    result_bytes = b''.join((
-        pad32(int_to_big_endian(result_x.n)),
-        pad32(int_to_big_endian(result_y.n)),
-    ))
+    result_bytes = b"".join(
+        (
+            pad32(int_to_big_endian(result_x.n)),
+            pad32(int_to_big_endian(result_y.n)),
+        )
+    )
     computation.output = result_bytes
     return computation
 
 
 def _ecadd(data: bytes) -> Tuple[bn128.FQ, bn128.FQ]:
     x1_bytes = pad32r(data[:32])
     y1_bytes = pad32r(data[32:64])
```

### Comparing `py-evm-0.7.0a1/eth/precompiles/ecmul.py` & `py-evm-0.7.0a2/eth/precompiles/ecmul.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,59 @@
-from typing import Tuple
-
-from py_ecc import (
-    optimized_bn128 as bn128,
+from typing import (
+    Tuple,
 )
 
 from eth_utils import (
+    ValidationError,
     big_endian_to_int,
     int_to_big_endian,
-    ValidationError,
 )
 from eth_utils.toolz import (
     curry,
 )
+from py_ecc import (
+    optimized_bn128 as bn128,
+)
 
-from eth import constants
-
-from eth.exceptions import (
-    VMError,
+from eth import (
+    constants,
 )
 from eth._utils.bn128 import (
     validate_point,
 )
 from eth._utils.padding import (
     pad32,
     pad32r,
 )
-
-from eth.vm.computation import (
-    BaseComputation,
+from eth.abc import (
+    ComputationAPI,
+)
+from eth.exceptions import (
+    VMError,
 )
 
 
 @curry
 def ecmul(
-        computation: BaseComputation,
-        gas_cost: int = constants.GAS_ECMUL) -> BaseComputation:
-
-    computation.consume_gas(gas_cost, reason='ECMUL Precompile')
+    computation: ComputationAPI, gas_cost: int = constants.GAS_ECMUL
+) -> ComputationAPI:
+    computation.consume_gas(gas_cost, reason="ECMUL Precompile")
 
     try:
         result = _ecmull(computation.msg.data_as_bytes)
     except ValidationError:
         raise VMError("Invalid ECMUL parameters")
 
     result_x, result_y = result
-    result_bytes = b''.join((
-        pad32(int_to_big_endian(result_x.n)),
-        pad32(int_to_big_endian(result_y.n)),
-    ))
+    result_bytes = b"".join(
+        (
+            pad32(int_to_big_endian(result_x.n)),
+            pad32(int_to_big_endian(result_y.n)),
+        )
+    )
     computation.output = result_bytes
     return computation
 
 
 def _ecmull(data: bytes) -> Tuple[bn128.FQ, bn128.FQ]:
     x_bytes = pad32r(data[:32])
     y_bytes = pad32r(data[32:64])
```

### Comparing `py-evm-0.7.0a1/eth/precompiles/ecpairing.py` & `py-evm-0.7.0a2/eth/precompiles/ecpairing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,84 +1,82 @@
-from typing import Tuple
+from typing import (
+    Tuple,
+)
 
 from eth_utils import (
-    big_endian_to_int,
     ValidationError,
+    big_endian_to_int,
 )
 from eth_utils.toolz import (
     curry,
     pipe,
 )
 from py_ecc import (
     optimized_bn128 as bn128,
 )
 
-from eth import constants
-
-from eth.exceptions import (
-    VMError,
-)
-
-from eth.typing import (
-    BytesOrView,
+from eth import (
+    constants,
 )
-
 from eth._utils.bn128 import (
-    validate_point,
     FQP_point_to_FQ2_point,
+    validate_point,
 )
 from eth._utils.padding import (
     pad32,
 )
-
-from eth.vm.computation import (
-    BaseComputation,
+from eth.abc import (
+    ComputationAPI,
+)
+from eth.exceptions import (
+    VMError,
+)
+from eth.typing import (
+    BytesOrView,
 )
-
 
 ZERO = bn128.Z2
 EXPONENT = bn128.FQ12.one()
 
 
 @curry
 def ecpairing(
-        computation: BaseComputation,
-        gas_cost_base: int = constants.GAS_ECPAIRING_BASE,
-        gas_cost_per_point: int = constants.GAS_ECPAIRING_PER_POINT) -> BaseComputation:
-
+    computation: ComputationAPI,
+    gas_cost_base: int = constants.GAS_ECPAIRING_BASE,
+    gas_cost_per_point: int = constants.GAS_ECPAIRING_PER_POINT,
+) -> ComputationAPI:
     if len(computation.msg.data) % 192:
         # data length must be an exact multiple of 192
         raise VMError("Invalid ECPAIRING parameters")
 
     num_points = len(computation.msg.data) // 192
     gas_fee = gas_cost_base + num_points * gas_cost_per_point
 
-    computation.consume_gas(gas_fee, reason='ECPAIRING Precompile')
+    computation.consume_gas(gas_fee, reason="ECPAIRING Precompile")
 
     try:
         result = _ecpairing(computation.msg.data)
     except ValidationError:
         raise VMError("Invalid ECPAIRING parameters")
 
     if result is True:
-        computation.output = pad32(b'\x01')
+        computation.output = pad32(b"\x01")
     elif result is False:
-        computation.output = pad32(b'\x00')
+        computation.output = pad32(b"\x00")
     else:
         raise Exception("Invariant: unreachable code path")
     return computation
 
 
 def _ecpairing(data: BytesOrView) -> bool:
     exponent = bn128.FQ12.one()
 
     processing_pipeline = (
-        _process_point(data[start_idx:start_idx + 192])
-        for start_idx
-        in range(0, len(data), 192)
+        _process_point(data[start_idx : start_idx + 192])
+        for start_idx in range(0, len(data), 192)
     )
     exponent = pipe(bn128.FQ12.one(), *processing_pipeline)
 
     result = bn128.final_exponentiate(exponent) == bn128.FQ12.one()
     return result
 
 
@@ -99,15 +97,17 @@
         p2 = (fq2_x, fq2_y, bn128.FQ2.one())
         if not bn128.is_on_curve(p2, bn128.b2):
             raise ValidationError("point is not on curve")
 
     if bn128.multiply(p2, bn128.curve_order)[-1] != bn128.FQ2.zero():
         raise ValidationError("TODO: what case is this?????")
 
-    return exponent * bn128.pairing(FQP_point_to_FQ2_point(p2), p1, final_exponentiate=False)
+    return exponent * bn128.pairing(
+        FQP_point_to_FQ2_point(p2), p1, final_exponentiate=False
+    )
 
 
 def _extract_point(data_slice: bytes) -> Tuple[int, int, int, int, int, int]:
     x1_bytes = data_slice[:32]
     y1_bytes = data_slice[32:64]
     x2_i_bytes = data_slice[64:96]
     x2_r_bytes = data_slice[96:128]
```

### Comparing `py-evm-0.7.0a1/eth/precompiles/ecrecover.py` & `py-evm-0.7.0a2/eth/precompiles/ecrecover.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from eth_keys import keys
+from eth_keys import (
+    keys,
+)
 from eth_keys.exceptions import (
     BadSignature,
 )
-
 from eth_utils import (
-    big_endian_to_int,
     ValidationError,
+    big_endian_to_int,
 )
 
-from eth import constants
-
+from eth import (
+    constants,
+)
 from eth._utils.padding import (
     pad32,
     pad32r,
 )
-
+from eth.abc import (
+    ComputationAPI,
+)
 from eth.validation import (
-    validate_lt_secpk1n,
     validate_gte,
+    validate_lt_secpk1n,
     validate_lte,
 )
-from eth.vm.computation import (
-    BaseComputation,
-)
 
 
-def ecrecover(computation: BaseComputation) -> BaseComputation:
+def ecrecover(computation: ComputationAPI) -> ComputationAPI:
     computation.consume_gas(constants.GAS_ECRECOVER, reason="ECRecover Precompile")
     data = computation.msg.data_as_bytes
     raw_message_hash = data[:32]
     message_hash = pad32r(raw_message_hash)
 
     v_bytes = pad32r(data[32:64])
     v = big_endian_to_int(v_bytes)
```

### Comparing `py-evm-0.7.0a1/eth/precompiles/modexp.py` & `py-evm-0.7.0a2/eth/precompiles/modexp.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,55 +7,51 @@
     big_endian_to_int,
     int_to_big_endian,
 )
 from eth_utils.toolz import (
     curry,
 )
 
-from eth import constants
-
+from eth import (
+    constants,
+)
 from eth._utils.numeric import (
     get_highest_bit_index,
 )
 from eth._utils.padding import (
     pad32r,
-    zpad_right,
     zpad_left,
+    zpad_right,
 )
-
-from eth.vm.computation import (
-    BaseComputation,
+from eth.abc import (
+    ComputationAPI,
 )
 
 
-def _compute_adjusted_exponent_length(exponent_length: int,
-                                      first_32_exponent_bytes: bytes) -> int:
+def _compute_adjusted_exponent_length(
+    exponent_length: int, first_32_exponent_bytes: bytes
+) -> int:
     exponent = big_endian_to_int(first_32_exponent_bytes)
 
     if exponent_length <= 32 and exponent == 0:
         return 0
     elif exponent_length <= 32:
         return get_highest_bit_index(exponent)
     else:
         first_32_bytes_as_int = big_endian_to_int(first_32_exponent_bytes)
-        return (
-            8 * (exponent_length - 32)
-            + get_highest_bit_index(first_32_bytes_as_int)
-        )
+        return 8 * (exponent_length - 32) + get_highest_bit_index(first_32_bytes_as_int)
 
 
 def _compute_complexity(length: int) -> int:
     if length <= 64:
-        return length ** 2
+        return length**2
     elif length <= 1024:
-        return (
-            length ** 2 // 4 + 96 * length - 3072
-        )
+        return length**2 // 4 + 96 * length - 3072
     else:
-        return length ** 2 // 16 + 480 * length - 199680
+        return length**2 // 16 + 480 * length - 199680
 
 
 def extract_lengths(data: bytes) -> Tuple[int, int, int]:
     # extract argument lengths
     base_length_bytes = pad32r(data[:32])
     base_length = big_endian_to_int(base_length_bytes)
 
@@ -68,15 +64,15 @@
     return base_length, exponent_length, modulus_length
 
 
 def _compute_modexp_gas_fee_eip_198(data: bytes) -> int:
     base_length, exponent_length, modulus_length = extract_lengths(data)
 
     first_32_exponent_bytes = zpad_right(
-        data[96 + base_length:96 + base_length + exponent_length],
+        data[96 + base_length : 96 + base_length + exponent_length],
         to_size=min(exponent_length, 32),
     )[:32]
     adjusted_exponent_length = _compute_adjusted_exponent_length(
         exponent_length,
         first_32_exponent_bytes,
     )
     complexity = _compute_complexity(max(modulus_length, base_length))
@@ -123,31 +119,32 @@
     result = pow(base, exponent, modulus)
 
     return result
 
 
 @curry
 def modexp(
-    computation: BaseComputation,
-    gas_calculator: Callable[[bytes], int] = _compute_modexp_gas_fee_eip_198
-) -> BaseComputation:
+    computation: ComputationAPI,
+    gas_calculator: Callable[[bytes], int] = _compute_modexp_gas_fee_eip_198,
+) -> ComputationAPI:
     """
     https://github.com/ethereum/EIPs/pull/198
     """
     data = computation.msg.data_as_bytes
 
     gas_fee = gas_calculator(data)
-    computation.consume_gas(gas_fee, reason='MODEXP Precompile')
+    computation.consume_gas(gas_fee, reason="MODEXP Precompile")
 
     result = _modexp(data)
 
     _, _, modulus_length = extract_lengths(data)
 
     # Modulo 0 is undefined, return zero
     # https://math.stackexchange.com/questions/516251/why-is-n-mod-0-undefined
-    result_bytes = b'' if modulus_length == 0 else zpad_left(
-        int_to_big_endian(result),
-        to_size=modulus_length
+    result_bytes = (
+        b""
+        if modulus_length == 0
+        else zpad_left(int_to_big_endian(result), to_size=modulus_length)
     )
 
     computation.output = result_bytes
     return computation
```

### Comparing `py-evm-0.7.0a1/eth/precompiles/ripemd160.py` & `py-evm-0.7.0a2/eth/precompiles/ripemd160.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import hashlib
 
-from eth import constants
-
+from eth import (
+    constants,
+)
 from eth._utils.numeric import (
     ceil32,
 )
 from eth._utils.padding import (
     pad32,
 )
-from eth.vm.computation import (
-    BaseComputation,
+from eth.abc import (
+    ComputationAPI,
 )
 
 
-def ripemd160(computation: BaseComputation) -> BaseComputation:
+def ripemd160(computation: ComputationAPI) -> ComputationAPI:
     word_count = ceil32(len(computation.msg.data)) // 32
     gas_fee = constants.GAS_RIPEMD160 + word_count * constants.GAS_RIPEMD160WORD
 
     computation.consume_gas(gas_fee, reason="RIPEMD160 Precompile")
 
     # TODO: this only works if openssl is installed.
-    hash = hashlib.new('ripemd160', computation.msg.data).digest()
+    hash = hashlib.new("ripemd160", computation.msg.data).digest()
     padded_hash = pad32(hash)
     computation.output = padded_hash
     return computation
```

### Comparing `py-evm-0.7.0a1/eth/precompiles/sha256.py` & `py-evm-0.7.0a2/eth/precompiles/sha256.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import hashlib
 
-from eth import constants
-
+from eth import (
+    constants,
+)
 from eth._utils.numeric import (
     ceil32,
 )
-
-from eth.vm.computation import (
-    BaseComputation,
+from eth.abc import (
+    ComputationAPI,
 )
 
 
-def sha256(computation: BaseComputation) -> BaseComputation:
+def sha256(computation: ComputationAPI) -> ComputationAPI:
     word_count = ceil32(len(computation.msg.data)) // 32
     gas_fee = constants.GAS_SHA256 + word_count * constants.GAS_SHA256WORD
 
     computation.consume_gas(gas_fee, reason="SHA256 Precompile")
     input_bytes = computation.msg.data
     hash = hashlib.sha256(input_bytes).digest()
     computation.output = hash
```

### Comparing `py-evm-0.7.0a1/eth/rlp/accounts.py` & `py-evm-0.7.0a2/eth/rlp/accounts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,50 @@
+from typing import (
+    Any,
+)
+
 import rlp
 from rlp.sedes import (
     big_endian_int,
 )
 
-from eth.abc import AccountAPI
+from eth.abc import (
+    AccountAPI,
+)
 from eth.constants import (
-    EMPTY_SHA3,
     BLANK_ROOT_HASH,
+    EMPTY_SHA3,
 )
 
 from .sedes import (
-    trie_root,
     hash32,
+    trie_root,
 )
 
-from typing import Any
-
 
 class Account(rlp.Serializable, AccountAPI):
     """
     RLP object for accounts.
     """
+
     fields = [
-        ('nonce', big_endian_int),
-        ('balance', big_endian_int),
-        ('storage_root', trie_root),
-        ('code_hash', hash32)
+        ("nonce", big_endian_int),
+        ("balance", big_endian_int),
+        ("storage_root", trie_root),
+        ("code_hash", hash32),
     ]
 
-    def __init__(self,
-                 nonce: int = 0,
-                 balance: int = 0,
-                 storage_root: bytes = BLANK_ROOT_HASH,
-                 code_hash: bytes = EMPTY_SHA3,
-                 **kwargs: Any) -> None:
+    def __init__(
+        self,
+        nonce: int = 0,
+        balance: int = 0,
+        storage_root: bytes = BLANK_ROOT_HASH,
+        code_hash: bytes = EMPTY_SHA3,
+        **kwargs: Any,
+    ) -> None:
         super().__init__(nonce, balance, storage_root, code_hash, **kwargs)
 
     def __repr__(self) -> str:
         return (
             f"Account(nonce={self.nonce}, balance={self.balance}, "
             f"storage_root=0x{self.storage_root.hex()}, "
             f"code_hash=0x{self.code_hash.hex()})"
```

### Comparing `py-evm-0.7.0a1/eth/rlp/blocks.py` & `py-evm-0.7.0a2/eth/rlp/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,12 +26,12 @@
         return cls.transaction_builder
 
     @property
     def is_genesis(self) -> bool:
         return self.header.is_genesis
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__}(#{str(self)})>'
+        return f"<{self.__class__.__name__}(#{str(self)})>"
 
     def __str__(self) -> str:
         clipped_hash = humanize_hash(self.hash)
         return f"Block #{self.number}-0x{clipped_hash}"
```

### Comparing `py-evm-0.7.0a1/eth/rlp/headers.py` & `py-evm-0.7.0a2/eth/rlp/headers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,139 +1,147 @@
 from typing import (
     Optional,
     cast,
     overload,
 )
 
-import rlp
-from rlp.sedes import (
-    big_endian_int,
-    Binary,
-    binary,
+from eth_hash.auto import (
+    keccak,
 )
-
 from eth_typing import (
     Address,
     BlockNumber,
     Hash32,
 )
-
-from eth_hash.auto import keccak
-
 from eth_utils import (
     encode_hex,
 )
+import rlp
+from rlp.sedes import (
+    Binary,
+    big_endian_int,
+    binary,
+)
 
 from eth._utils.headers import (
     new_timestamp_from_parent,
 )
 from eth.abc import (
     BlockHeaderAPI,
     MiningHeaderAPI,
 )
 from eth.constants import (
-    ZERO_ADDRESS,
-    ZERO_HASH32,
+    BLANK_ROOT_HASH,
     EMPTY_UNCLE_HASH,
     GENESIS_NONCE,
     GENESIS_PARENT_HASH,
-    BLANK_ROOT_HASH,
+    ZERO_ADDRESS,
+    ZERO_HASH32,
+)
+from eth.typing import (
+    HeaderParams,
 )
-from eth.typing import HeaderParams
 
 from .sedes import (
     address,
     hash32,
-    uint256,
     trie_root,
+    uint256,
 )
 
 
 class MiningHeader(rlp.Serializable, MiningHeaderAPI):
     fields = [
-        ('parent_hash', hash32),
-        ('uncles_hash', hash32),
-        ('coinbase', address),
-        ('state_root', trie_root),
-        ('transaction_root', trie_root),
-        ('receipt_root', trie_root),
-        ('bloom', uint256),
-        ('difficulty', big_endian_int),
-        ('block_number', big_endian_int),
-        ('gas_limit', big_endian_int),
-        ('gas_used', big_endian_int),
-        ('timestamp', big_endian_int),
-        ('extra_data', binary),
+        ("parent_hash", hash32),
+        ("uncles_hash", hash32),
+        ("coinbase", address),
+        ("state_root", trie_root),
+        ("transaction_root", trie_root),
+        ("receipt_root", trie_root),
+        ("bloom", uint256),
+        ("difficulty", big_endian_int),
+        ("block_number", big_endian_int),
+        ("gas_limit", big_endian_int),
+        ("gas_used", big_endian_int),
+        ("timestamp", big_endian_int),
+        ("extra_data", binary),
     ]
 
 
 class BlockHeader(rlp.Serializable, BlockHeaderAPI):
     fields = [
-        ('parent_hash', hash32),
-        ('uncles_hash', hash32),
-        ('coinbase', address),
-        ('state_root', trie_root),
-        ('transaction_root', trie_root),
-        ('receipt_root', trie_root),
-        ('bloom', uint256),
-        ('difficulty', big_endian_int),
-        ('block_number', big_endian_int),
-        ('gas_limit', big_endian_int),
-        ('gas_used', big_endian_int),
-        ('timestamp', big_endian_int),
-        ('extra_data', binary),
-        ('mix_hash', binary),
-        ('nonce', Binary(8, allow_empty=True))
+        ("parent_hash", hash32),
+        ("uncles_hash", hash32),
+        ("coinbase", address),
+        ("state_root", trie_root),
+        ("transaction_root", trie_root),
+        ("receipt_root", trie_root),
+        ("bloom", uint256),
+        ("difficulty", big_endian_int),
+        ("block_number", big_endian_int),
+        ("gas_limit", big_endian_int),
+        ("gas_used", big_endian_int),
+        ("timestamp", big_endian_int),
+        ("extra_data", binary),
+        ("mix_hash", binary),
+        ("nonce", Binary(8, allow_empty=True)),
     ]
 
     @overload
     def __init__(self, **kwargs: HeaderParams) -> None:
         ...
 
     @overload  # noqa: F811
-    def __init__(self,
-                 difficulty: int,
-                 block_number: BlockNumber,
-                 gas_limit: int,
-                 timestamp: int = None,
-                 coinbase: Address = ZERO_ADDRESS,
-                 parent_hash: Hash32 = ZERO_HASH32,
-                 uncles_hash: Hash32 = EMPTY_UNCLE_HASH,
-                 state_root: Hash32 = BLANK_ROOT_HASH,
-                 transaction_root: Hash32 = BLANK_ROOT_HASH,
-                 receipt_root: Hash32 = BLANK_ROOT_HASH,
-                 bloom: int = 0,
-                 gas_used: int = 0,
-                 extra_data: bytes = b'',
-                 mix_hash: Hash32 = ZERO_HASH32,
-                 nonce: bytes = GENESIS_NONCE) -> None:
+    def __init__(
+        self,
+        difficulty: int,
+        block_number: BlockNumber,
+        gas_limit: int,
+        timestamp: int = None,
+        coinbase: Address = ZERO_ADDRESS,
+        parent_hash: Hash32 = ZERO_HASH32,
+        uncles_hash: Hash32 = EMPTY_UNCLE_HASH,
+        state_root: Hash32 = BLANK_ROOT_HASH,
+        transaction_root: Hash32 = BLANK_ROOT_HASH,
+        receipt_root: Hash32 = BLANK_ROOT_HASH,
+        bloom: int = 0,
+        gas_used: int = 0,
+        extra_data: bytes = b"",
+        mix_hash: Hash32 = ZERO_HASH32,
+        nonce: bytes = GENESIS_NONCE,
+    ) -> None:
         ...
 
-    def __init__(self,              # type: ignore  # noqa: F811
-                 difficulty: int,
-                 block_number: BlockNumber,
-                 gas_limit: int,
-                 timestamp: int = None,
-                 coinbase: Address = ZERO_ADDRESS,
-                 parent_hash: Hash32 = ZERO_HASH32,
-                 uncles_hash: Hash32 = EMPTY_UNCLE_HASH,
-                 state_root: Hash32 = BLANK_ROOT_HASH,
-                 transaction_root: Hash32 = BLANK_ROOT_HASH,
-                 receipt_root: Hash32 = BLANK_ROOT_HASH,
-                 bloom: int = 0,
-                 gas_used: int = 0,
-                 extra_data: bytes = b'',
-                 mix_hash: Hash32 = ZERO_HASH32,
-                 nonce: bytes = GENESIS_NONCE) -> None:
+    def __init__(  # type: ignore  # noqa: F811
+        self,
+        difficulty: int,
+        block_number: BlockNumber,
+        gas_limit: int,
+        timestamp: int = None,
+        coinbase: Address = ZERO_ADDRESS,
+        parent_hash: Hash32 = ZERO_HASH32,
+        uncles_hash: Hash32 = EMPTY_UNCLE_HASH,
+        state_root: Hash32 = BLANK_ROOT_HASH,
+        transaction_root: Hash32 = BLANK_ROOT_HASH,
+        receipt_root: Hash32 = BLANK_ROOT_HASH,
+        bloom: int = 0,
+        gas_used: int = 0,
+        extra_data: bytes = b"",
+        mix_hash: Hash32 = ZERO_HASH32,
+        nonce: bytes = GENESIS_NONCE,
+    ) -> None:
         if timestamp is None:
             if parent_hash == ZERO_HASH32:
                 timestamp = new_timestamp_from_parent(None)
             else:
-                # without access to the parent header, we cannot select a new timestamp correctly
-                raise ValueError("Must set timestamp explicitly if this is not a genesis header")
+                # without access to the parent header,
+                # we cannot select a new timestamp correctly
+                raise ValueError(
+                    "Must set timestamp explicitly if this is not a genesis header"
+                )
 
         super().__init__(
             parent_hash=parent_hash,
             uncles_hash=uncles_hash,
             coinbase=coinbase,
             state_root=state_root,
             transaction_root=transaction_root,
@@ -146,15 +154,15 @@
             timestamp=timestamp,
             extra_data=extra_data,
             mix_hash=mix_hash,
             nonce=nonce,
         )
 
     def __str__(self) -> str:
-        return f'<BlockHeader #{self.block_number} {encode_hex(self.hash)[2:10]}>'
+        return f"<BlockHeader #{self.block_number} {encode_hex(self.hash)[2:10]}>"
 
     _hash = None
 
     @property
     def hash(self) -> Hash32:
         if self._hash is None:
             self._hash = keccak(rlp.encode(self))
@@ -168,16 +176,17 @@
     @property
     def hex_hash(self) -> str:
         return encode_hex(self.hash)
 
     @property
     def is_genesis(self) -> bool:
         # if removing the block_number == 0 test, consider the validation consequences.
-        # validate_header stops trying to check the current header against a parent header.
-        # Can someone trick us into following a high difficulty header with genesis parent hash?
+        # validate_header stops trying to check the current header against a parent
+        # header. Can someone trick us into following a high difficulty header with
+        # genesis parent hash?
         return self.parent_hash == GENESIS_PARENT_HASH and self.block_number == 0
 
     @property
     def base_fee_per_gas(self) -> int:
         raise AttributeError("Base fee per gas not available until London fork")
 
     @property
```

### Comparing `py-evm-0.7.0a1/eth/rlp/logs.py` & `py-evm-0.7.0a2/eth/rlp/logs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,29 @@
-from rlp.sedes import (
-    CountableList,
-    binary,
-)
-
 from typing import (
     Tuple,
 )
 
 import rlp
+from rlp.sedes import (
+    CountableList,
+    binary,
+)
 
-from eth.abc import LogAPI
+from eth.abc import (
+    LogAPI,
+)
 
 from .sedes import (
     address,
     uint32,
 )
 
 
 class Log(rlp.Serializable, LogAPI):
-    fields = [
-        ('address', address),
-        ('topics', CountableList(uint32)),
-        ('data', binary)
-    ]
+    fields = [("address", address), ("topics", CountableList(uint32)), ("data", binary)]
 
     def __init__(self, address: bytes, topics: Tuple[int, ...], data: bytes) -> None:
         super().__init__(address, topics, data)
 
     @property
     def bloomables(self) -> Tuple[bytes, ...]:
-        return (
-            self.address,
-        ) + tuple(
-            uint32.serialize(topic) for topic in self.topics
-        )
+        return (self.address,) + tuple(uint32.serialize(topic) for topic in self.topics)
```

### Comparing `py-evm-0.7.0a1/eth/rlp/receipts.py` & `py-evm-0.7.0a2/eth/rlp/receipts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import itertools
-from typing import Iterable
+from typing import (
+    Iterable,
+)
 
-from eth_bloom import BloomFilter
+from eth_bloom import (
+    BloomFilter,
+)
 import rlp
 from rlp.sedes import (
-    big_endian_int,
     CountableList,
+    big_endian_int,
     binary,
 )
 
 from eth.abc import (
     ReceiptAPI,
     ReceiptBuilderAPI,
 )
 
-from .logs import Log
+from .logs import (
+    Log,
+)
 from .sedes import (
     uint256,
 )
 
 
 class Receipt(rlp.Serializable, ReceiptAPI, ReceiptBuilderAPI):
     type_id = None
 
     fields = [
-        ('state_root', binary),
-        ('gas_used', big_endian_int),
-        ('bloom', uint256),
-        ('logs', CountableList(Log))
+        ("state_root", binary),
+        ("gas_used", big_endian_int),
+        ("bloom", uint256),
+        ("logs", CountableList(Log)),
     ]
 
-    def __init__(self,
-                 state_root: bytes,
-                 gas_used: int,
-                 logs: Iterable[Log],
-                 bloom: int = None) -> None:
-
+    def __init__(
+        self, state_root: bytes, gas_used: int, logs: Iterable[Log], bloom: int = None
+    ) -> None:
         if bloom is None:
             bloomables = itertools.chain.from_iterable(log.bloomables for log in logs)
             bloom = int(BloomFilter.from_iterable(bloomables))
 
         super().__init__(
             state_root=state_root,
             gas_used=gas_used,
```

### Comparing `py-evm-0.7.0a1/eth/rlp/transactions.py` & `py-evm-0.7.0a2/eth/rlp/transactions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 from typing import (
     Optional,
     Sequence,
     Tuple,
     cast,
 )
 
-from cached_property import cached_property
-import rlp
-from rlp.sedes import (
-    big_endian_int,
-    binary,
+from cached_property import (
+    cached_property,
+)
+from eth_hash.auto import (
+    keccak,
 )
-
 from eth_typing import (
     Address,
     Hash32,
 )
-
-from eth_hash.auto import keccak
 from eth_utils import (
     ValidationError,
 )
+import rlp
+from rlp.sedes import (
+    big_endian_int,
+    binary,
+)
 
 from eth.abc import (
     BaseTransactionAPI,
     ComputationAPI,
     LegacyTransactionFieldsAPI,
     SignedTransactionAPI,
     TransactionBuilderAPI,
     TransactionFieldsAPI,
     UnsignedTransactionAPI,
 )
 
-from .sedes import address
+from .sedes import (
+    address,
+)
 
 
 class BaseTransactionMethods(BaseTransactionAPI):
-
     def validate(self) -> None:
         pass
 
     @property
     def intrinsic_gas(self) -> int:
         return self.get_intrinsic_gas()
 
@@ -53,23 +56,23 @@
 
     @property
     def access_list(self) -> Sequence[Tuple[Address, Sequence[int]]]:
         return []
 
 
 BASE_TRANSACTION_FIELDS = [
-    ('nonce', big_endian_int),
-    ('gas_price', big_endian_int),
-    ('gas', big_endian_int),
-    ('to', address),
-    ('value', big_endian_int),
-    ('data', binary),
-    ('v', big_endian_int),
-    ('r', big_endian_int),
-    ('s', big_endian_int),
+    ("nonce", big_endian_int),
+    ("gas_price", big_endian_int),
+    ("gas", big_endian_int),
+    ("to", address),
+    ("value", big_endian_int),
+    ("data", binary),
+    ("v", big_endian_int),
+    ("r", big_endian_int),
+    ("s", big_endian_int),
 ]
 
 
 class BaseTransactionFields(rlp.Serializable, TransactionFieldsAPI):
     fields = BASE_TRANSACTION_FIELDS
 
     @property
@@ -102,18 +105,19 @@
         except ValidationError:
             return False
         else:
             return True
 
 
 class BaseTransaction(
-        LegacyTransactionFieldsAPI,
-        BaseTransactionFields,
-        SignedTransactionMethods,
-        TransactionBuilderAPI):
+    LegacyTransactionFieldsAPI,
+    BaseTransactionFields,
+    SignedTransactionMethods,
+    TransactionBuilderAPI,
+):
     # "Legacy" transactions implemented by BaseTransaction are a combination of
     # the transaction codec (TransactionBuilderAPI) *and* the transaction
     # object (SignedTransactionAPI). In a multi-transaction-type world, that
     # becomes less desirable, and that responsibility splits up. See Berlin
     # transactions, for example.
 
     # Note that it includes at least one legacy field (v) that is not
@@ -129,16 +133,18 @@
     def decode(cls, encoded: bytes) -> SignedTransactionAPI:
         return rlp.decode(encoded, sedes=cls)
 
     def encode(self) -> bytes:
         return rlp.encode(self)
 
 
-class BaseUnsignedTransaction(BaseTransactionMethods, rlp.Serializable, UnsignedTransactionAPI):
+class BaseUnsignedTransaction(
+    BaseTransactionMethods, rlp.Serializable, UnsignedTransactionAPI
+):
     fields = [
-        ('nonce', big_endian_int),
-        ('gas_price', big_endian_int),
-        ('gas', big_endian_int),
-        ('to', address),
-        ('value', big_endian_int),
-        ('data', binary),
+        ("nonce", big_endian_int),
+        ("gas_price", big_endian_int),
+        ("gas", big_endian_int),
+        ("to", address),
+        ("value", big_endian_int),
+        ("data", binary),
     ]
```

### Comparing `py-evm-0.7.0a1/eth/tools/_utils/deprecation.py` & `py-evm-0.7.0a2/eth/tools/_utils/deprecation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import functools
-import warnings
 from typing import (
     Any,
     Callable,
     TypeVar,
     cast,
 )
-
+import warnings
 
 TFunc = TypeVar("TFunc", bound=Callable[..., Any])
 
 
 def deprecate_method(func: TFunc, message: str = None) -> TFunc:
     @functools.wraps(func)
     def deprecated_func(*args: Any, **kwargs: Any) -> Any:
```

### Comparing `py-evm-0.7.0a1/eth/tools/_utils/hashing.py` & `py-evm-0.7.0a2/eth/tools/_utils/hashing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from typing import (
     Iterable,
     Tuple,
     cast,
 )
 
-from eth_hash.auto import keccak
+from eth_hash.auto import (
+    keccak,
+)
 from eth_typing import (
     Hash32,
 )
 import rlp
 
-from eth.rlp.logs import Log
+from eth.rlp.logs import (
+    Log,
+)
 
 
-def hash_log_entries(log_entries: Iterable[Tuple[bytes, Tuple[int, ...], bytes]]) -> Hash32:
+def hash_log_entries(
+    log_entries: Iterable[Tuple[bytes, Tuple[int, ...], bytes]]
+) -> Hash32:
     """
     Helper function for computing the RLP hash of the logs from transaction
     execution.
     """
     logs = [Log(*entry) for entry in log_entries]
     encoded_logs = rlp.encode(logs)
     logs_hash = keccak(encoded_logs)
```

### Comparing `py-evm-0.7.0a1/eth/tools/_utils/mappings.py` & `py-evm-0.7.0a2/eth/tools/_utils/mappings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-from collections.abc import Mapping
+from collections.abc import (
+    Mapping,
+)
 import itertools
-
 from typing import (
     Any,
     Dict,
     Sequence,
 )
 
-from eth_utils.toolz import merge_with
+from eth_utils.toolz import (
+    merge_with,
+)
 
 
 def merge_if_dicts(values: Sequence[Dict[Any, Any]]) -> Any:
     if all(isinstance(item, Mapping) for item in values):
         return merge_with(merge_if_dicts, *values)
     else:
         return values[-1]
 
 
 def deep_merge(*dicts: Dict[Any, Any]) -> Dict[Any, Any]:
     return merge_with(merge_if_dicts, *dicts)
 
 
 def is_cleanly_mergable(*dicts: Dict[Any, Any]) -> bool:
-    """Check that nothing will be overwritten when dictionaries are merged using `deep_merge`.
+    """
+    Check that nothing will be overwritten when
+    dictionaries are merged using `deep_merge`.
 
     Examples:
 
         >>> is_cleanly_mergable({"a": 1}, {"b": 2}, {"c": 3})
         True
         >>> is_cleanly_mergable({"a": 1}, {"b": 2}, {"a": 0, c": 3})
         False
@@ -39,11 +44,15 @@
     if len(dicts) <= 1:
         return True
     elif len(dicts) == 2:
         if not all(isinstance(d, Mapping) for d in dicts):
             return False
         else:
             shared_keys = set(dicts[0].keys()) & set(dicts[1].keys())
-            return all(is_cleanly_mergable(dicts[0][key], dicts[1][key]) for key in shared_keys)
+            return all(
+                is_cleanly_mergable(dicts[0][key], dicts[1][key]) for key in shared_keys
+            )
     else:
         dict_combinations = itertools.combinations(dicts, 2)
-        return all(is_cleanly_mergable(*combination) for combination in dict_combinations)
+        return all(
+            is_cleanly_mergable(*combination) for combination in dict_combinations
+        )
```

### Comparing `py-evm-0.7.0a1/eth/tools/_utils/normalization.py` & `py-evm-0.7.0a2/eth/tools/_utils/normalization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 import binascii
 import functools
 from typing import (
     Any,
     AnyStr,
     Callable,
-    cast,
     Dict,
     Iterable,
     List,
     Mapping,
     Sequence,
     Tuple,
     Union,
+    cast,
 )
 
-from mypy_extensions import (
-    TypedDict,
-)
-
-from eth_utils.toolz import (
-    assoc_in,
-    compose,
-    concat,
-    curry,
-    identity,
-    merge,
-)
-from eth_utils.toolz import curried
-
 from eth_typing import (
     Address,
     HexStr,
 )
-
 from eth_utils.curried import (
+    ValidationError,
     apply_formatter_if,
     apply_formatter_to_array,
     apply_formatters_to_dict,
     big_endian_to_int,
     decode_hex,
     hexstr_if_str,
     is_0x_prefixed,
@@ -45,26 +31,35 @@
     is_hex,
     is_integer,
     is_string,
     is_text,
     to_bytes,
     to_canonical_address,
     to_dict,
-    ValidationError,
+)
+from eth_utils.toolz import (
+    assoc_in,
+    compose,
+    concat,
+    curried,
+    curry,
+    identity,
+    merge,
+)
+from mypy_extensions import (
+    TypedDict,
 )
 
 from eth.constants import (
     CREATE_CONTRACT_ADDRESS,
 )
-
 from eth.tools._utils.mappings import (
     deep_merge,
     is_cleanly_mergable,
 )
-
 from eth.typing import (
     AccountState,
     GeneralState,
     IntConvertible,
     Normalizer,
     TransactionDict,
     TransactionNormalizer,
@@ -99,15 +94,15 @@
 
 def normalize_bytes(value: Union[bytes, str]) -> bytes:
     if is_bytes(value):
         return cast(bytes, value)
     elif is_text(value) and is_hex(value):
         return decode_hex(cast(str, value))
     elif is_text(value):
-        return b''
+        return b""
     else:
         raise TypeError("Value must be either a string or bytes object")
 
 
 @functools.lru_cache(maxsize=1024)
 def to_int(value: str) -> int:
     """
@@ -133,18 +128,19 @@
 
 robust_decode_hex = hexstr_if_str(to_bytes)
 
 
 #
 # Containers
 #
-def dict_normalizer(formatters: Dict[Any, Callable[..., Any]],
-                    required: Iterable[Any] = None,
-                    optional: Iterable[Any] = None) -> Normalizer:
-
+def dict_normalizer(
+    formatters: Dict[Any, Callable[..., Any]],
+    required: Iterable[Any] = None,
+    optional: Iterable[Any] = None,
+) -> Normalizer:
     all_keys = set(formatters.keys())
 
     if required is None and optional is None:
         required_set_form = all_keys
     elif required is not None and optional is not None:
         raise ValueError("Both required and optional keys specified")
     elif required is not None:
@@ -163,15 +159,14 @@
 
         return apply_formatters_to_dict(formatters, d)
 
     return normalizer
 
 
 def dict_options_normalizer(normalizers: Iterable[Normalizer]) -> Normalizer:
-
     def normalize(d: Dict[Any, Any]) -> Dict[str, Any]:
         first_exception = None
         for normalizer in normalizers:
             try:
                 normalized = normalizer(d)
             except KeyError as e:
                 if not first_exception:
@@ -186,18 +181,18 @@
 
 #
 # Composition
 #
 def state_definition_to_dict(state_definition: GeneralState) -> AccountState:
     """Convert a state definition to the canonical dict form.
 
-    State can either be defined in the canonical form, or as a list of sub states that are then
-    merged to one. Sub states can either be given as dictionaries themselves, or as tuples where
-    the last element is the value and all others the keys for this value in the nested state
-    dictionary. Example:
+    State can either be defined in the canonical form, or as a list of sub states that
+    are then merged to one. Sub states can either be given as dictionaries themselves,
+    or as tuples where the last element is the value and all others the keys for this
+    value in the nested state dictionary. Example:
 
     ```
         [
             ("0xaabb", "balance", 3),
             ("0xaabb", "storage", {
                 4: 5,
             }),
@@ -208,384 +203,425 @@
         ]
     ```
     """
     if isinstance(state_definition, Mapping):
         state_dict = state_definition
     elif isinstance(state_definition, Iterable):
         state_dicts = [
-            assoc_in(
-                {},
-                state_item[:-1],
-                state_item[-1]
-            ) if not isinstance(state_item, Mapping) else state_item
-            for state_item
-            in state_definition
+            assoc_in({}, state_item[:-1], state_item[-1])
+            if not isinstance(state_item, Mapping)
+            else state_item
+            for state_item in state_definition
         ]
         if not is_cleanly_mergable(*state_dicts):
             raise ValidationError("Some state item is defined multiple times")
         state_dict = deep_merge(*state_dicts)
     else:
         assert TypeError("State definition must either be a mapping or a sequence")
 
     seen_keys = set(concat(d.keys() for d in state_dict.values()))
     bad_keys = seen_keys - {"balance", "nonce", "storage", "code"}
     if bad_keys:
         raise ValidationError(
-            f"State definition contains the following invalid account fields: {', '.join(bad_keys)}"
+            "State definition contains the following invalid "
+            f"account fields: {', '.join(bad_keys)}"
         )
 
     return state_dict
 
 
 normalize_storage = compose(
     curried.keymap(normalize_int),
     curried.valmap(normalize_int),
 )
 
 
 normalize_state = compose(
     curried.keymap(to_canonical_address),
-    curried.valmap(dict_normalizer({
-        "balance": normalize_int,
-        "code": normalize_bytes,
-        "nonce": normalize_int,
-        "storage": normalize_storage
-    }, required=[])),
+    curried.valmap(
+        dict_normalizer(
+            {
+                "balance": normalize_int,
+                "code": normalize_bytes,
+                "nonce": normalize_int,
+                "storage": normalize_storage,
+            },
+            required=[],
+        )
+    ),
     apply_formatter_if(
         lambda s: isinstance(s, Iterable) and not isinstance(s, Mapping),
-        state_definition_to_dict
+        state_definition_to_dict,
     ),
 )
 
 
-normalize_main_transaction = dict_normalizer({
-    "data": normalize_bytes,
-    "gasLimit": normalize_int,
-    "gasPrice": normalize_int,
-    "nonce": normalize_int,
-    "secretKey": normalize_bytes,
-    "to": normalize_to_address,
-    "value": normalize_int,
-})
-
-
-normalize_transaction = cast(TransactionNormalizer, dict_options_normalizer([
-    normalize_main_transaction,
-]))
-
-
-normalize_main_transaction_group = dict_normalizer({
-    "data": apply_formatter_to_array(normalize_bytes),
-    "gasLimit": apply_formatter_to_array(normalize_int),
-    "gasPrice": normalize_int,
-    "nonce": normalize_int,
-    "secretKey": normalize_bytes,
-    "to": normalize_to_address,
-    "value": apply_formatter_to_array(normalize_int),
-})
-
-
-normalize_transaction_group = cast(TransactionNormalizer, dict_options_normalizer([
-    normalize_main_transaction_group,
-]))
-
-
-normalize_execution = dict_normalizer({
-    "address": to_canonical_address,
-    "origin": to_canonical_address,
-    "caller": to_canonical_address,
-    "value": normalize_int,
-    "data": normalize_bytes,
-    "gasPrice": normalize_int,
-    "gas": normalize_int,
-})
+normalize_main_transaction = dict_normalizer(
+    {
+        "data": normalize_bytes,
+        "gasLimit": normalize_int,
+        "gasPrice": normalize_int,
+        "nonce": normalize_int,
+        "secretKey": normalize_bytes,
+        "to": normalize_to_address,
+        "value": normalize_int,
+    }
+)
+
+
+normalize_transaction = cast(
+    TransactionNormalizer,
+    dict_options_normalizer(
+        [
+            normalize_main_transaction,
+        ]
+    ),
+)
+
+
+normalize_main_transaction_group = dict_normalizer(
+    {
+        "data": apply_formatter_to_array(normalize_bytes),
+        "gasLimit": apply_formatter_to_array(normalize_int),
+        "gasPrice": normalize_int,
+        "nonce": normalize_int,
+        "secretKey": normalize_bytes,
+        "to": normalize_to_address,
+        "value": apply_formatter_to_array(normalize_int),
+    }
+)
+
+
+normalize_transaction_group = cast(
+    TransactionNormalizer,
+    dict_options_normalizer(
+        [
+            normalize_main_transaction_group,
+        ]
+    ),
+)
+
+
+normalize_execution = dict_normalizer(
+    {
+        "address": to_canonical_address,
+        "origin": to_canonical_address,
+        "caller": to_canonical_address,
+        "value": normalize_int,
+        "data": normalize_bytes,
+        "gasPrice": normalize_int,
+        "gas": normalize_int,
+    }
+)
 
 
 normalize_networks = identity
 
 
-normalize_call_create_item = dict_normalizer({
-    "data": normalize_bytes,
-    "destination": to_canonical_address,
-    "gasLimit": normalize_int,
-    "value": normalize_int,
-})
+normalize_call_create_item = dict_normalizer(
+    {
+        "data": normalize_bytes,
+        "destination": to_canonical_address,
+        "gasLimit": normalize_int,
+        "value": normalize_int,
+    }
+)
 normalize_call_creates: Callable[[Iterable[Any]], Iterable[Any]]
 normalize_call_creates = apply_formatter_to_array(normalize_call_create_item)
 
-normalize_log_item = dict_normalizer({
-    "address": to_canonical_address,
-    "topics": apply_formatter_to_array(normalize_int),
-    "data": normalize_bytes,
-})
+normalize_log_item = dict_normalizer(
+    {
+        "address": to_canonical_address,
+        "topics": apply_formatter_to_array(normalize_int),
+        "data": normalize_bytes,
+    }
+)
 normalize_logs: Callable[[Iterable[Any]], Iterable[Any]]
 normalize_logs = apply_formatter_to_array(normalize_log_item)
 
 
-normalize_main_environment = dict_normalizer({
-    "currentCoinbase": to_canonical_address,
-    "previousHash": normalize_bytes,
-    "currentNumber": normalize_int,
-    "currentDifficulty": normalize_int,
-    "currentGasLimit": normalize_int,
-    "currentTimestamp": normalize_int,
-}, optional=["previousHash"])
+normalize_main_environment = dict_normalizer(
+    {
+        "currentCoinbase": to_canonical_address,
+        "previousHash": normalize_bytes,
+        "currentNumber": normalize_int,
+        "currentDifficulty": normalize_int,
+        "currentGasLimit": normalize_int,
+        "currentTimestamp": normalize_int,
+    },
+    optional=["previousHash"],
+)
 
 
-normalize_environment = dict_options_normalizer([
-    normalize_main_environment,
-])
+normalize_environment = dict_options_normalizer(
+    [
+        normalize_main_environment,
+    ]
+)
 
 
 #
 # Fixture Normalizers
 #
-def normalize_unsigned_transaction(transaction: TransactionDict,
-                                   indexes: Dict[str, Any]) -> TransactionDict:
-
+def normalize_unsigned_transaction(
+    transaction: TransactionDict, indexes: Dict[str, Any]
+) -> TransactionDict:
     normalized = normalize_transaction_group(transaction)
-    return merge(normalized, {
-        # Dynamic key access not yet allowed with TypedDict
-        # https://github.com/python/mypy/issues/5359
-        transaction_key: normalized[transaction_key][indexes[index_key]]  # type: ignore
-        for transaction_key, index_key in [
-            ("gasLimit", "gas"),
-            ("value", "value"),
-            ("data", "data"),
-        ]
-        if index_key in indexes
-    })
-
-
-FixtureAccountDetails = TypedDict('FixtureAccountDetails',
-                                  {'balance': HexStr,
-                                   'nonce': HexStr,
-                                   'code': HexStr,
-                                   'storage': Dict[HexStr, HexStr]
-                                   })
+    return merge(
+        normalized,
+        {
+            # Dynamic key access not yet allowed with TypedDict
+            # https://github.com/python/mypy/issues/5359
+            transaction_key: normalized[transaction_key][indexes[index_key]]  # type: ignore  # noqa: E501
+            for transaction_key, index_key in [
+                ("gasLimit", "gas"),
+                ("value", "value"),
+                ("data", "data"),
+            ]
+            if index_key in indexes
+        },
+    )
+
+
+FixtureAccountDetails = TypedDict(
+    "FixtureAccountDetails",
+    {
+        "balance": HexStr,
+        "nonce": HexStr,
+        "code": HexStr,
+        "storage": Dict[HexStr, HexStr],
+    },
+)
 FixtureAccountState = Dict[Address, FixtureAccountDetails]
 
 
 def normalize_account_state(account_state: FixtureAccountState) -> AccountState:
     return {
         to_canonical_address(address): {
-            'balance': to_int(state['balance']),
-            'code': decode_hex(state['code']),
-            'nonce': to_int(state['nonce']),
-            'storage': {
+            "balance": to_int(state["balance"]),
+            "code": decode_hex(state["code"]),
+            "nonce": to_int(state["nonce"]),
+            "storage": {
                 to_int(slot): big_endian_to_int(decode_hex(value))
-                for slot, value in state['storage'].items()
+                for slot, value in state["storage"].items()
             },
-        } for address, state in account_state.items()
+        }
+        for address, state in account_state.items()
     }
 
 
 def normalize_post_state(postate: FixtureAccountState) -> AccountState:
     # poststate might not be present in some fixtures
     # https://github.com/ethereum/tests/issues/637#issuecomment-534072897
     if postate is None:
         return {}
     else:
         return normalize_account_state(postate)
 
 
 @to_dict
-def normalize_post_state_hash(post_state: Dict[str, Any]) -> Iterable[Tuple[str, bytes]]:
-    yield 'hash', decode_hex(post_state['hash'])
-    if 'logs' in post_state:
-        yield 'logs', decode_hex(post_state['logs'])
+def normalize_post_state_hash(
+    post_state: Dict[str, Any]
+) -> Iterable[Tuple[str, bytes]]:
+    yield "hash", decode_hex(post_state["hash"])
+    if "logs" in post_state:
+        yield "logs", decode_hex(post_state["logs"])
 
 
 @curry
-def normalize_statetest_fixture(fixture: Dict[str, Any],
-                                fork: str,
-                                post_state_index: int) -> Dict[str, Any]:
-
-    post_state = fixture['post'][fork][post_state_index]
+def normalize_statetest_fixture(
+    fixture: Dict[str, Any], fork: str, post_state_index: int
+) -> Dict[str, Any]:
+    post_state = fixture["post"][fork][post_state_index]
 
     normalized_fixture = {
-        'env': normalize_environment(fixture['env']),
-        'pre': normalize_account_state(fixture['pre']),
-        'post': normalize_post_state_hash(post_state),
-        'transaction': normalize_unsigned_transaction(
-            fixture['transaction'],
-            post_state['indexes'],
+        "env": normalize_environment(fixture["env"]),
+        "pre": normalize_account_state(fixture["pre"]),
+        "post": normalize_post_state_hash(post_state),
+        "transaction": normalize_unsigned_transaction(
+            fixture["transaction"],
+            post_state["indexes"],
         ),
     }
 
     return normalized_fixture
 
 
 def normalize_exec(exec_params: Dict[str, Any]) -> Dict[str, Any]:
     return {
-        'origin': to_canonical_address(exec_params['origin']),
-        'address': to_canonical_address(exec_params['address']),
-        'caller': to_canonical_address(exec_params['caller']),
-        'value': to_int(exec_params['value']),
-        'data': decode_hex(exec_params['data']),
-        'gas': to_int(exec_params['gas']),
-        'gasPrice': to_int(exec_params['gasPrice']),
+        "origin": to_canonical_address(exec_params["origin"]),
+        "address": to_canonical_address(exec_params["address"]),
+        "caller": to_canonical_address(exec_params["caller"]),
+        "value": to_int(exec_params["value"]),
+        "data": decode_hex(exec_params["data"]),
+        "gas": to_int(exec_params["gas"]),
+        "gasPrice": to_int(exec_params["gasPrice"]),
     }
 
 
-def normalize_callcreates(callcreates: Sequence[Dict[str, Any]]) -> List[Dict[str, Any]]:
+def normalize_callcreates(
+    callcreates: Sequence[Dict[str, Any]]
+) -> List[Dict[str, Any]]:
     return [
         {
-            'data': decode_hex(created_call['data']),
-            'destination': (
-                to_canonical_address(created_call['destination'])
-                if created_call['destination']
+            "data": decode_hex(created_call["data"]),
+            "destination": (
+                to_canonical_address(created_call["destination"])
+                if created_call["destination"]
                 else CREATE_CONTRACT_ADDRESS
             ),
-            'gasLimit': to_int(created_call['gasLimit']),
-            'value': to_int(created_call['value']),
-        } for created_call in callcreates
+            "gasLimit": to_int(created_call["gasLimit"]),
+            "value": to_int(created_call["value"]),
+        }
+        for created_call in callcreates
     ]
 
 
 @to_dict
 def normalize_vmtest_fixture(fixture: Dict[str, Any]) -> Iterable[Tuple[str, Any]]:
-    yield 'env', normalize_environment(fixture['env'])
-    yield 'exec', normalize_exec(fixture['exec'])
-    yield 'pre', normalize_account_state(fixture['pre'])
+    yield "env", normalize_environment(fixture["env"])
+    yield "exec", normalize_exec(fixture["exec"])
+    yield "pre", normalize_account_state(fixture["pre"])
 
-    if 'post' in fixture:
-        yield 'post', normalize_account_state(fixture['post'])
+    if "post" in fixture:
+        yield "post", normalize_account_state(fixture["post"])
 
-    if 'callcreates' in fixture:
-        yield 'callcreates', normalize_callcreates(fixture['callcreates'])
+    if "callcreates" in fixture:
+        yield "callcreates", normalize_callcreates(fixture["callcreates"])
 
-    if 'gas' in fixture:
-        yield 'gas', to_int(fixture['gas'])
+    if "gas" in fixture:
+        yield "gas", to_int(fixture["gas"])
 
-    if 'out' in fixture:
-        yield 'out', decode_hex(fixture['out'])
+    if "out" in fixture:
+        yield "out", decode_hex(fixture["out"])
 
-    if 'logs' in fixture:
-        yield 'logs', decode_hex(fixture['logs'])
+    if "logs" in fixture:
+        yield "logs", decode_hex(fixture["logs"])
 
 
 def normalize_signed_transaction(transaction: Dict[str, Any]) -> Dict[str, Any]:
     normalized_universal_transaction = {
-        'data': robust_decode_hex(transaction['data']),
-        'gasLimit': to_int(transaction['gasLimit']),
-        'nonce': to_int(transaction['nonce']),
-        'r': to_int(transaction['r']),
-        's': to_int(transaction['s']),
-        'v': to_int(transaction['v']),
-        'to': decode_hex(transaction['to']),
-        'value': to_int(transaction['value']),
+        "data": robust_decode_hex(transaction["data"]),
+        "gasLimit": to_int(transaction["gasLimit"]),
+        "nonce": to_int(transaction["nonce"]),
+        "r": to_int(transaction["r"]),
+        "s": to_int(transaction["s"]),
+        "v": to_int(transaction["v"]),
+        "to": decode_hex(transaction["to"]),
+        "value": to_int(transaction["value"]),
     }
-    if 'type' in transaction:
-        type_id = to_int(transaction['type'])
+    if "type" in transaction:
+        type_id = to_int(transaction["type"])
         if type_id == 1:
             custom_fields = {
-                'type': type_id,
-                'gasPrice': to_int(transaction['gasPrice']),
-                'chainId': to_int(transaction['chainId']),
+                "type": type_id,
+                "gasPrice": to_int(transaction["gasPrice"]),
+                "chainId": to_int(transaction["chainId"]),
             }
         elif type_id == 2:
             custom_fields = {
-                'type': type_id,
-                'chainId': to_int(transaction['chainId']),
-                'maxFeePerGas': to_int(transaction['maxFeePerGas']),
-                'maxPriorityFeePerGas': to_int(transaction['maxPriorityFeePerGas']),
+                "type": type_id,
+                "chainId": to_int(transaction["chainId"]),
+                "maxFeePerGas": to_int(transaction["maxFeePerGas"]),
+                "maxPriorityFeePerGas": to_int(transaction["maxPriorityFeePerGas"]),
             }
         else:
             raise ValidationError(f"Did not recognize transaction type {type_id}")
     else:
         custom_fields = {
-            'gasPrice': to_int(transaction['gasPrice']),
+            "gasPrice": to_int(transaction["gasPrice"]),
         }
 
     return merge(normalized_universal_transaction, custom_fields)
 
 
 @curry
-def normalize_transactiontest_fixture(fixture: Dict[str, Any], fork: str) -> Dict[str, Any]:
-
+def normalize_transactiontest_fixture(
+    fixture: Dict[str, Any], fork: str
+) -> Dict[str, Any]:
     normalized_fixture = {}
 
-    fork_data = fixture['result'][fork]
+    fork_data = fixture["result"][fork]
 
     try:
-        normalized_fixture['txbytes'] = decode_hex(fixture['txbytes'])
+        normalized_fixture["txbytes"] = decode_hex(fixture["txbytes"])
     except binascii.Error:
-        normalized_fixture['rlpHex'] = fixture['txbytes']
+        normalized_fixture["rlpHex"] = fixture["txbytes"]
 
     if "sender" in fork_data:
-        normalized_fixture['sender'] = fork_data['sender']
+        normalized_fixture["sender"] = fork_data["sender"]
 
     if "hash" in fork_data:
-        normalized_fixture['hash'] = fork_data['hash']
+        normalized_fixture["hash"] = fork_data["hash"]
 
     return normalized_fixture
 
 
 def normalize_block_header(header: Dict[str, Any]) -> Dict[str, Any]:
     normalized_header = {
-        'bloom': big_endian_to_int(decode_hex(header['bloom'])),
-        'coinbase': to_canonical_address(header['coinbase']),
-        'difficulty': to_int(header['difficulty']),
-        'extraData': decode_hex(header['extraData']),
-        'gasLimit': to_int(header['gasLimit']),
-        'gasUsed': to_int(header['gasUsed']),
-        'hash': decode_hex(header['hash']),
-        'mixHash': decode_hex(header['mixHash']),
-        'nonce': decode_hex(header['nonce']),
-        'number': to_int(header['number']),
-        'parentHash': decode_hex(header['parentHash']),
-        'receiptTrie': decode_hex(header['receiptTrie']),
-        'stateRoot': decode_hex(header['stateRoot']),
-        'timestamp': to_int(header['timestamp']),
-        'transactionsTrie': decode_hex(header['transactionsTrie']),
-        'uncleHash': decode_hex(header['uncleHash']),
-    }
-    if 'blocknumber' in header:
-        normalized_header['blocknumber'] = to_int(header['blocknumber'])
-    if 'baseFeePerGas' in header:
-        normalized_header['baseFeePerGas'] = to_int(header['baseFeePerGas'])
-    if 'chainname' in header:
-        normalized_header['chainname'] = header['chainname']
-    if 'chainnetwork' in header:
-        normalized_header['chainnetwork'] = header['chainnetwork']
+        "bloom": big_endian_to_int(decode_hex(header["bloom"])),
+        "coinbase": to_canonical_address(header["coinbase"]),
+        "difficulty": to_int(header["difficulty"]),
+        "extraData": decode_hex(header["extraData"]),
+        "gasLimit": to_int(header["gasLimit"]),
+        "gasUsed": to_int(header["gasUsed"]),
+        "hash": decode_hex(header["hash"]),
+        "mixHash": decode_hex(header["mixHash"]),
+        "nonce": decode_hex(header["nonce"]),
+        "number": to_int(header["number"]),
+        "parentHash": decode_hex(header["parentHash"]),
+        "receiptTrie": decode_hex(header["receiptTrie"]),
+        "stateRoot": decode_hex(header["stateRoot"]),
+        "timestamp": to_int(header["timestamp"]),
+        "transactionsTrie": decode_hex(header["transactionsTrie"]),
+        "uncleHash": decode_hex(header["uncleHash"]),
+    }
+    if "blocknumber" in header:
+        normalized_header["blocknumber"] = to_int(header["blocknumber"])
+    if "baseFeePerGas" in header:
+        normalized_header["baseFeePerGas"] = to_int(header["baseFeePerGas"])
+    if "chainname" in header:
+        normalized_header["chainname"] = header["chainname"]
+    if "chainnetwork" in header:
+        normalized_header["chainnetwork"] = header["chainnetwork"]
     return normalized_header
 
 
 def normalize_block(block: Dict[str, Any]) -> Dict[str, Any]:
     normalized_block: Dict[str, Any] = {}
 
     try:
-        normalized_block['rlp'] = decode_hex(block['rlp'])
+        normalized_block["rlp"] = decode_hex(block["rlp"])
     except ValueError as err:
-        normalized_block['rlp_error'] = err
+        normalized_block["rlp_error"] = err
 
-    if 'blockHeader' in block:
-        normalized_block['blockHeader'] = normalize_block_header(block['blockHeader'])
-    if 'transactions' in block:
-        normalized_block['transactions'] = [
+    if "blockHeader" in block:
+        normalized_block["blockHeader"] = normalize_block_header(block["blockHeader"])
+    if "transactions" in block:
+        normalized_block["transactions"] = [
             normalize_signed_transaction(transaction)
-            for transaction
-            in block['transactions']
+            for transaction in block["transactions"]
         ]
-    if 'expectException' in block:
-        normalized_block['expectException'] = block['expectException']
+    if "expectException" in block:
+        normalized_block["expectException"] = block["expectException"]
     return normalized_block
 
 
 def normalize_blockchain_fixtures(fixture: Dict[str, Any]) -> Dict[str, Any]:
     normalized_fixture = {
-        'blocks': [normalize_block(block_fixture) for block_fixture in fixture['blocks']],
-        'genesisBlockHeader': normalize_block_header(fixture['genesisBlockHeader']),
-        'lastblockhash': decode_hex(fixture['lastblockhash']),
-        'pre': normalize_account_state(fixture['pre']),
-        'postState': normalize_post_state(fixture.get('postState')),
-        'network': fixture['network'],
+        "blocks": [
+            normalize_block(block_fixture) for block_fixture in fixture["blocks"]
+        ],
+        "genesisBlockHeader": normalize_block_header(fixture["genesisBlockHeader"]),
+        "lastblockhash": decode_hex(fixture["lastblockhash"]),
+        "pre": normalize_account_state(fixture["pre"]),
+        "postState": normalize_post_state(fixture.get("postState")),
+        "network": fixture["network"],
     }
 
-    if 'sealEngine' in fixture:
-        normalized_fixture['sealEngine'] = fixture['sealEngine']
+    if "sealEngine" in fixture:
+        normalized_fixture["sealEngine"] = fixture["sealEngine"]
 
-    if 'genesisRLP' in fixture:
-        normalized_fixture['genesisRLP'] = decode_hex(fixture['genesisRLP'])
+    if "genesisRLP" in fixture:
+        normalized_fixture["genesisRLP"] = decode_hex(fixture["genesisRLP"])
 
     return normalized_fixture
```

### Comparing `py-evm-0.7.0a1/eth/tools/_utils/slow_code_stream.py` & `py-evm-0.7.0a2/eth/tools/_utils/slow_code_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import contextlib
 import io
 import logging
 from typing import (
     Iterator,
-    Set
+    Set,
 )
 
 from eth.validation import (
     validate_is_bytes,
 )
-from eth.vm import opcode_values
+from eth.vm import (
+    opcode_values,
+)
 
 PUSH1, PUSH32, STOP = opcode_values.PUSH1, opcode_values.PUSH32, opcode_values.STOP
 
 
 class SlowCodeStream:
     """
     A known working version of code stream that is kept around for testing,
     despite not being optimized.
     """
+
     stream = None
     _length_cache = None
     _raw_code_bytes = None
     invalid_positions: Set[int] = None
     valid_positions: Set[int] = None
 
-    logger = logging.getLogger('eth.vm.SlowCodeStream')
+    logger = logging.getLogger("eth.vm.SlowCodeStream")
 
     def __init__(self, code_bytes: bytes) -> None:
         validate_is_bytes(code_bytes, title="SlowCodeStream bytes")
         stream = io.BytesIO(code_bytes)
         self.stream = stream
         self._bound_stream_read = stream.read
         self._raw_code_bytes = code_bytes
@@ -75,23 +78,25 @@
         return self.stream.tell()
 
     @program_counter.setter
     def program_counter(self, value: int) -> None:
         self.stream.seek(min(value, len(self)))
 
     @contextlib.contextmanager
-    def seek(self, pc: int) -> Iterator['SlowCodeStream']:
+    def seek(self, pc: int) -> Iterator["SlowCodeStream"]:
         anchor_pc = self.program_counter
         self.program_counter = pc
         try:
             yield self
         finally:
             self.program_counter = anchor_pc
 
-    def _potentially_disqualifying_opcode_positions(self, position: int) -> Iterator[int]:
+    def _potentially_disqualifying_opcode_positions(
+        self, position: int
+    ) -> Iterator[int]:
         # Look at the last 32 positions (from 1 byte back to 32 bytes back).
         # Don't attempt to look at negative positions.
         deepest_lookback = min(32, position)
         # iterate in reverse, because PUSH32 is more common than others
         for bytes_back in range(deepest_lookback, 0, -1):
             earlier_position = position - bytes_back
             opcode = self._raw_code_bytes[earlier_position]
@@ -105,20 +110,22 @@
             return False
         elif position in self.invalid_positions:
             return False
         elif position in self.valid_positions:
             return True
         else:
             # An opcode is not valid, iff it is the "data" following a PUSH_
-            # So we look at the previous 32 bytes (PUSH32 being the largest) to see if there
-            # is a PUSH_ before the opcode in this position.
-            for disqualifier in self._potentially_disqualifying_opcode_positions(position):
-                # Now that we found a PUSH_ before this position, we check if *that* PUSH is valid
+            # So we look at the previous 32 bytes (PUSH32 being the largest) to see if
+            # there is a PUSH_ before the opcode in this position.
+            for disqualifier in self._potentially_disqualifying_opcode_positions(
+                position
+            ):
+                # Now that we found a PUSH_ before this position, we check if *that* PUSH is valid  # noqa: E501
                 if self.is_valid_opcode(disqualifier):
                     # If the PUSH_ valid, then the current position is invalid
                     self.invalid_positions.add(position)
                     return False
-                # Otherwise, keep looking for other potentially disqualifying PUSH_ codes
+                # Otherwise, keep looking for other potentially disqualifying PUSH_ codes  # noqa: E501
 
-            # We didn't find any valid PUSH_ opcodes in the 32 bytes before position; it's valid
+            # We didn't find any valid PUSH_ opcodes in the 32 bytes before position;it's valid  # noqa: E501
             self.valid_positions.add(position)
             return True
```

### Comparing `py-evm-0.7.0a1/eth/tools/_utils/vyper.py` & `py-evm-0.7.0a2/eth/tools/_utils/vyper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import functools
-
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Tuple,
 )
 
 try:
     from vyper.compile_lll import (
-        compile_to_assembly,
         assembly_to_evm,
+        compile_to_assembly,
+    )
+    from vyper.parser.parser_utils import (
+        LLLnode,
     )
-    from vyper.parser.parser_utils import LLLnode
 except ImportError:
     vyper_available = False
 else:
     vyper_available = True
 
 
 def require_vyper(fn: Callable[..., Any]) -> Callable[..., Any]:
     @functools.wraps(fn)
     def inner(*args: Any, **kwargs: Any) -> Any:
         if vyper_available:
             return fn(*args, **kwargs)
         else:
             raise ImportError("The `{0}` function requires the vyper compiler.")
+
     return inner
 
 
 @require_vyper
 def compile_vyper_lll(vyper_code: List[Any]) -> Tuple[bytes, Dict[str, Any]]:
     lll_node = LLLnode.from_list(vyper_code)
     assembly = compile_to_assembly(lll_node)
```

### Comparing `py-evm-0.7.0a1/eth/tools/builder/chain/__init__.py` & `py-evm-0.7.0a2/eth/tools/builder/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a1/eth/tools/builder/chain/builders.py` & `py-evm-0.7.0a2/eth/tools/builder/chain/builders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,87 +1,95 @@
 import functools
 import time
 from typing import (
-    cast,
     Any,
     Callable,
     Dict,
     Iterable,
     Tuple,
     Type,
     Union,
-)
-
-from eth_utils.toolz import (
-    curry,
-    merge,
-    pipe,
+    cast,
 )
 
 from eth_typing import (
     Address,
     BlockNumber,
     Hash32,
 )
-
 from eth_utils import (
+    ValidationError,
     to_dict,
     to_tuple,
-    ValidationError,
+)
+from eth_utils.toolz import (
+    curry,
+    merge,
+    pipe,
 )
 
-from eth import constants
+from eth import (
+    constants,
+)
 from eth.abc import (
     AtomicDatabaseAPI,
     BlockAPI,
     ChainAPI,
     MiningChainAPI,
     VirtualMachineAPI,
 )
-from eth.consensus.applier import ConsensusApplier
-from eth.consensus.noproof import NoProofConsensus
-from eth.db.atomic import AtomicDB
+from eth.consensus.applier import (
+    ConsensusApplier,
+)
+from eth.consensus.noproof import (
+    NoProofConsensus,
+)
+from eth.db.atomic import (
+    AtomicDB,
+)
 from eth.db.backends.memory import (
     MemoryDB,
 )
 from eth.rlp.headers import (
     HeaderParams,
 )
-from eth.tools.mining import POWMiningMixin
 from eth.tools._utils.mappings import (
     deep_merge,
 )
 from eth.tools._utils.normalization import (
     normalize_state,
 )
+from eth.tools.mining import (
+    POWMiningMixin,
+)
 from eth.typing import (
     AccountState,
     GeneralState,
-    VMFork,
     VMConfiguration,
+    VMFork,
 )
 from eth.validation import (
     validate_vm_configuration,
 )
 from eth.vm.forks import (
-    FrontierVM,
-    HomesteadVM,
-    TangerineWhistleVM,
-    SpuriousDragonVM,
+    ArrowGlacierVM,
+    BerlinVM,
     ByzantiumVM,
     ConstantinopleVM,
-    PetersburgVM,
+    FrontierVM,
+    GrayGlacierVM,
+    HomesteadVM,
     IstanbulVM,
-    MuirGlacierVM,
-    BerlinVM,
     LondonVM,
-    ArrowGlacierVM,
-    GrayGlacierVM,
+    MuirGlacierVM,
     ParisVM,
+    PetersburgVM,
     ShanghaiVM,
+    SpuriousDragonVM,
+    TangerineWhistleVM,
 )
 
 
 def build(obj: Any, *applicators: Callable[..., Any]) -> Any:
     """
     Run the provided object through the series of applicator functions.
 
@@ -111,17 +119,19 @@
     """
     Set the ``chain_id`` for the chain class.
     """
     return chain_class.configure(chain_id=chain_id)
 
 
 @curry
-def fork_at(vm_class: Type[VirtualMachineAPI],
-            at_block: Union[int, BlockNumber],
-            chain_class: Type[ChainAPI]) -> Type[ChainAPI]:
+def fork_at(
+    vm_class: Type[VirtualMachineAPI],
+    at_block: Union[int, BlockNumber],
+    chain_class: Type[ChainAPI],
+) -> Type[ChainAPI]:
     """
     Adds the ``vm_class`` to the chain's ``vm_configuration``.
 
     .. code-block:: python
 
         from eth.chains.base import MiningChain
         from eth.tools.builder.chain import build, fork_at
@@ -148,15 +158,15 @@
     * :func:`~eth.tools.builder.chain.petersburg_at`
     * :func:`~eth.tools.builder.chain.istanbul_at`
     * :func:`~eth.tools.builder.chain.muir_glacier_at`
     * :func:`~eth.tools.builder.chain.berlin_at`
     * :func:`~eth.tools.builder.chain.london_at`
     * :func:`~eth.tools.builder.chain.arrow_glacier_at`
     * :func:`~eth.tools.builder.chain.gray_glacier_at`
-    * :func:`~eth.tools.builder.chain.latest_mainnet_at` - whatever the latest mainnet VM is
+    * :func:`~eth.tools.builder.chain.latest_mainnet_at` - whatever latest mainnet VM is
     """
     if chain_class.vm_configuration is not None:
         base_configuration = chain_class.vm_configuration
     else:
         base_configuration = ()
 
     vm_configuration = base_configuration + ((BlockNumber(at_block), vm_class),)
@@ -199,29 +209,31 @@
         raise ValidationError("No HomesteadVM found in vm_configuration.")
 
     vm_configuration = _set_vm_dao_support_false(chain_class.vm_configuration)
     return chain_class.configure(vm_configuration=vm_configuration)
 
 
 @to_tuple
-def _set_vm_dao_fork_block_number(dao_fork_block_number: BlockNumber,
-                                  vm_configuration: VMConfiguration) -> Iterable[VMFork]:
+def _set_vm_dao_fork_block_number(
+    dao_fork_block_number: BlockNumber, vm_configuration: VMConfiguration
+) -> Iterable[VMFork]:
     for fork_block, vm_class in vm_configuration:
         if _is_homestead(vm_class):
             yield fork_block, vm_class.configure(
                 support_dao_fork=True,
                 _dao_fork_block_number=dao_fork_block_number,
             )
         else:
             yield fork_block, vm_class
 
 
 @curry
-def dao_fork_at(dao_fork_block_number: BlockNumber,
-                chain_class: Type[ChainAPI]) -> Type[ChainAPI]:
+def dao_fork_at(
+    dao_fork_block_number: BlockNumber, chain_class: Type[ChainAPI]
+) -> Type[ChainAPI]:
     """
     Set the block number on which the DAO fork will happen.  Requires that a
     version of the :class:`~eth.vm.forks.homestead.HomesteadVM` is present in
     the chain's ``vm_configuration``
 
     """
     homstead_vms_found = any(
@@ -255,47 +267,50 @@
 
 latest_mainnet_at = shanghai_at
 
 GENESIS_DEFAULTS = cast(
     Tuple[Tuple[str, Union[BlockNumber, int, None, bytes, Address, Hash32]], ...],
     # values that will automatically be default are commented out
     (
-        ('difficulty', 1),
-        ('extra_data', constants.GENESIS_EXTRA_DATA),
-        ('gas_limit', constants.GENESIS_GAS_LIMIT),
+        ("difficulty", 1),
+        ("extra_data", constants.GENESIS_EXTRA_DATA),
+        ("gas_limit", constants.GENESIS_GAS_LIMIT),
         # ('gas_used', 0),
         # ('bloom', 0),
-        ('mix_hash', constants.ZERO_HASH32),
-        ('nonce', constants.GENESIS_NONCE),
+        ("mix_hash", constants.ZERO_HASH32),
+        ("nonce", constants.GENESIS_NONCE),
         # ('block_number', constants.GENESIS_BLOCK_NUMBER),
         # ('parent_hash', constants.GENESIS_PARENT_HASH),
-        ('receipt_root', constants.BLANK_ROOT_HASH),
+        ("receipt_root", constants.BLANK_ROOT_HASH),
         # ('uncles_hash', constants.EMPTY_UNCLE_HASH),
-        ('state_root', constants.BLANK_ROOT_HASH),
-        ('transaction_root', constants.BLANK_ROOT_HASH),
-    )
+        ("state_root", constants.BLANK_ROOT_HASH),
+        ("transaction_root", constants.BLANK_ROOT_HASH),
+    ),
 )
 
 
 @to_dict
-def _get_default_genesis_params(genesis_state: AccountState,
-                                ) -> Iterable[Tuple[str, Union[BlockNumber, int, None, bytes, Address, Hash32]]]:  # noqa: E501
+def _get_default_genesis_params(
+    genesis_state: AccountState,
+) -> Iterable[Tuple[str, Union[BlockNumber, int, None, bytes, Address, Hash32]]]:
     for key, value in GENESIS_DEFAULTS:
-        if key == 'state_root' and genesis_state:
+        if key == "state_root" and genesis_state:
             # leave out the `state_root` if a genesis state was specified
             pass
         else:
             yield key, value
-    yield 'timestamp', int(time.time())  # populate the timestamp value at runtime
+    yield "timestamp", int(time.time())  # populate the timestamp value at runtime
 
 
 @to_tuple
 def _mix_in_pow_mining(vm_configuration: VMConfiguration) -> Iterable[VMFork]:
     for fork_block, vm_class in vm_configuration:
-        vm_class_with_pow_mining = type(vm_class.__name__, (POWMiningMixin, vm_class), {})
+        vm_class_with_pow_mining = type(
+            vm_class.__name__, (POWMiningMixin, vm_class), {}
+        )
         yield fork_block, vm_class_with_pow_mining
 
 
 @curry
 def enable_pow_mining(chain_class: Type[ChainAPI]) -> Type[ChainAPI]:
     """
     Inject on demand generation of the proof of work mining seal on newly
@@ -326,29 +341,34 @@
 
 
 #
 # Initializers (initialization of chain state and chain class instantiation)
 #
 def _fill_and_normalize_state(simple_state: GeneralState) -> AccountState:
     base_state = normalize_state(simple_state)
-    defaults = {address: {
-        "balance": 0,
-        "nonce": 0,
-        "code": b"",
-        "storage": {},
-    } for address in base_state.keys()}
+    defaults = {
+        address: {
+            "balance": 0,
+            "nonce": 0,
+            "code": b"",
+            "storage": {},
+        }
+        for address in base_state.keys()
+    }
     state = deep_merge(defaults, base_state)
     return state
 
 
 @curry
-def genesis(chain_class: ChainAPI,
-            db: AtomicDatabaseAPI = None,
-            params: Dict[str, HeaderParams] = None,
-            state: GeneralState = None) -> ChainAPI:
+def genesis(
+    chain_class: ChainAPI,
+    db: AtomicDatabaseAPI = None,
+    params: Dict[str, HeaderParams] = None,
+    state: GeneralState = None,
+) -> ChainAPI:
     """
     Initialize the given chain class with the given genesis header parameters
     and chain state.
     """
     if state is None:
         genesis_state: AccountState = {}
     else:
@@ -377,29 +397,29 @@
     """
     Mine a new block on the chain.  Header parameters for the new block can be
     overridden using keyword arguments.
 
     """
 
     if not isinstance(chain, MiningChainAPI):
-        raise ValidationError('`mine_block` may only be used on MiningChain instances')
+        raise ValidationError("`mine_block` may only be used on MiningChain instances")
 
-    transactions = kwargs.pop('transactions', ())
+    transactions = kwargs.pop("transactions", ())
 
     chain.mine_all(transactions, **kwargs)
     return chain
 
 
 @curry
 def mine_blocks(num_blocks: int, chain: MiningChainAPI) -> MiningChainAPI:
     """
     Variadic argument version of :func:`~eth.tools.builder.chain.mine_block`
     """
     if not isinstance(chain, MiningChainAPI):
-        raise ValidationError('`mine_block` may only be used on MiningChain instances')
+        raise ValidationError("`mine_block` may only be used on MiningChain instances")
     for _ in range(num_blocks):
         chain.mine_block()
     return chain
 
 
 @curry
 def import_block(block: BlockAPI, chain: ChainAPI) -> ChainAPI:
@@ -410,14 +430,15 @@
     return chain
 
 
 def import_blocks(*blocks: BlockAPI) -> Callable[[ChainAPI], ChainAPI]:
     """
     Variadic argument version of :func:`~eth.tools.builder.chain.import_block`
     """
+
     @functools.wraps(import_blocks)
     def _import_blocks(chain: ChainAPI) -> ChainAPI:
         for block in blocks:
             chain.import_block(block)
         return chain
 
     return _import_blocks
@@ -434,21 +455,25 @@
     base_db = chain.chaindb.db
     if not isinstance(base_db, AtomicDB):
         raise ValidationError(f"Unsupported database type: {type(base_db)}")
 
     if isinstance(base_db.wrapped_db, MemoryDB):
         db = AtomicDB(MemoryDB(base_db.wrapped_db.kv_store.copy()))
     else:
-        raise ValidationError(f"Unsupported wrapped database: {type(base_db.wrapped_db)}")
+        raise ValidationError(
+            f"Unsupported wrapped database: {type(base_db.wrapped_db)}"
+        )
 
     chain_copy = type(chain)(db, chain.header)
     return chain_copy
 
 
-def chain_split(*splits: Iterable[Callable[..., Any]]) -> Callable[[ChainAPI], Iterable[ChainAPI]]:   # noqa: E501
+def chain_split(
+    *splits: Iterable[Callable[..., Any]]
+) -> Callable[[ChainAPI], Iterable[ChainAPI]]:
     """
     Construct and execute multiple concurrent forks of the chain.
 
     Any number of forks may be executed.  For each fork, provide an iterable of
     commands.
 
     Returns the resulting chain objects for each fork.
@@ -461,15 +486,17 @@
             chain_split(
                 (mine_block(extra_data=b'chain-a'), mine_block()),
                 (mine_block(extra_data=b'chain-b'), mine_block(), mine_block()),
             ),
         )
     """
     if not splits:
-        raise ValidationError("Cannot use `chain_split` without providing at least one split")
+        raise ValidationError(
+            "Cannot use `chain_split` without providing at least one split"
+        )
 
     @functools.wraps(chain_split)
     @to_tuple
     def _chain_split(chain: ChainAPI) -> Iterable[ChainAPI]:
         for split_fns in splits:
             result = build(
                 chain,
@@ -477,15 +504,17 @@
             )
             yield result
 
     return _chain_split
 
 
 @curry
-def at_block_number(block_number: Union[int, BlockNumber], chain: MiningChainAPI) -> MiningChainAPI:
+def at_block_number(
+    block_number: Union[int, BlockNumber], chain: MiningChainAPI
+) -> MiningChainAPI:
     """
     Rewind the chain back to the given block number.  Calls to things like
     ``get_canonical_head`` will still return the canonical head of the chain,
     however, you can use ``mine_block`` to mine fork chains.
     """
     if not isinstance(chain, MiningChainAPI):
         raise ValidationError("`at_block_number` may only be used with 'MiningChain")
```

### Comparing `py-evm-0.7.0a1/eth/tools/db/atomic.py` & `py-evm-0.7.0a2/eth/tools/db/atomic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,158 +1,175 @@
 import pytest
 
-from eth_utils import ValidationError
-
-from eth.abc import AtomicDatabaseAPI
+from eth_utils import (
+    ValidationError,
+)
+
+from eth.abc import (
+    AtomicDatabaseAPI,
+)
 
 
 class AtomicDatabaseBatchAPITestSuite:
     def test_atomic_batch_set_and_get(self, atomic_db: AtomicDatabaseAPI) -> None:
         with atomic_db.atomic_batch() as batch:
-            batch.set(b'1', b'2')
-            assert batch.get(b'1') == b'2'
+            batch.set(b"1", b"2")
+            assert batch.get(b"1") == b"2"
 
-        assert atomic_db.get(b'1') == b'2'
+        assert atomic_db.get(b"1") == b"2"
 
-    def test_atomic_db_cannot_recursively_batch(self, atomic_db: AtomicDatabaseAPI) -> None:
+    def test_atomic_db_cannot_recursively_batch(
+        self, atomic_db: AtomicDatabaseAPI
+    ) -> None:
         with atomic_db.atomic_batch() as batch:
-            assert not hasattr(batch, 'atomic_batch')
+            assert not hasattr(batch, "atomic_batch")
 
-    def test_atomic_db_with_set_and_delete_batch(self, atomic_db: AtomicDatabaseAPI) -> None:
-        atomic_db[b'key-1'] = b'origin'
+    def test_atomic_db_with_set_and_delete_batch(
+        self, atomic_db: AtomicDatabaseAPI
+    ) -> None:
+        atomic_db[b"key-1"] = b"origin"
 
         with atomic_db.atomic_batch() as batch:
-            batch.delete(b'key-1')
+            batch.delete(b"key-1")
 
-            assert b'key-1' not in batch
+            assert b"key-1" not in batch
             with pytest.raises(KeyError):
-                assert batch[b'key-1']
+                assert batch[b"key-1"]
 
         with pytest.raises(KeyError):
-            atomic_db[b'key-1']
+            atomic_db[b"key-1"]
 
-    def test_atomic_db_unbatched_sets_are_immediate(self, atomic_db: AtomicDatabaseAPI) -> None:
-        atomic_db[b'1'] = b'A'
+    def test_atomic_db_unbatched_sets_are_immediate(
+        self, atomic_db: AtomicDatabaseAPI
+    ) -> None:
+        atomic_db[b"1"] = b"A"
 
         with atomic_db.atomic_batch() as batch:
             # Unbatched changes are immediate, and show up in batch reads
-            atomic_db[b'1'] = b'B'
-            assert batch[b'1'] == b'B'
+            atomic_db[b"1"] = b"B"
+            assert batch[b"1"] == b"B"
 
-            batch[b'1'] = b'C1'
+            batch[b"1"] = b"C1"
 
             # It doesn't matter what changes happen underlying, all reads now
             # show the write applied to the batch db handle
-            atomic_db[b'1'] = b'C2'
-            assert batch[b'1'] == b'C1'
+            atomic_db[b"1"] = b"C2"
+            assert batch[b"1"] == b"C1"
 
         # the batch write should overwrite any intermediate changes
-        assert atomic_db[b'1'] == b'C1'
+        assert atomic_db[b"1"] == b"C1"
 
-    def test_atomic_db_unbatched_deletes_are_immediate(self, atomic_db: AtomicDatabaseAPI) -> None:
-        atomic_db[b'1'] = b'A'
+    def test_atomic_db_unbatched_deletes_are_immediate(
+        self, atomic_db: AtomicDatabaseAPI
+    ) -> None:
+        atomic_db[b"1"] = b"A"
 
         with atomic_db.atomic_batch() as batch:
-            assert b'1' in batch
+            assert b"1" in batch
 
             # Unbatched changes are immediate, and show up in batch reads
-            del atomic_db[b'1']
+            del atomic_db[b"1"]
 
-            assert b'1' not in batch
+            assert b"1" not in batch
 
-            batch[b'1'] = b'C1'
+            batch[b"1"] = b"C1"
 
             # It doesn't matter what changes happen underlying, all reads now
             # show the write applied to the batch db handle
-            atomic_db[b'1'] = b'C2'
-            assert batch[b'1'] == b'C1'
+            atomic_db[b"1"] = b"C2"
+            assert batch[b"1"] == b"C1"
 
         # the batch write should overwrite any intermediate changes
-        assert atomic_db[b'1'] == b'C1'
+        assert atomic_db[b"1"] == b"C1"
 
-    def test_atomic_db_cannot_use_batch_after_context(self, atomic_db: AtomicDatabaseAPI) -> None:
-        atomic_db[b'1'] = b'A'
+    def test_atomic_db_cannot_use_batch_after_context(
+        self, atomic_db: AtomicDatabaseAPI
+    ) -> None:
+        atomic_db[b"1"] = b"A"
 
         with atomic_db.atomic_batch() as batch:
-            batch[b'1'] = b'B'
+            batch[b"1"] = b"B"
 
         # set
         with pytest.raises(ValidationError):
-            batch[b'1'] = b'C'
+            batch[b"1"] = b"C"
 
         with pytest.raises(ValidationError):
-            batch.set(b'1', b'C')
+            batch.set(b"1", b"C")
 
         # get
         with pytest.raises(ValidationError):
-            batch[b'1']
+            batch[b"1"]
 
         with pytest.raises(ValidationError):
-            batch.get(b'1')
+            batch.get(b"1")
 
         # exists
         with pytest.raises(ValidationError):
-            b'1' in batch
+            b"1" in batch
 
         with pytest.raises(ValidationError):
-            batch.exists(b'1')
+            batch.exists(b"1")
 
         # delete
         with pytest.raises(ValidationError):
-            del batch[b'1']
+            del batch[b"1"]
 
         with pytest.raises(ValidationError):
-            batch.delete(b'1')
+            batch.delete(b"1")
 
         # none of the invalid changes above should change the original db
-        assert atomic_db[b'1'] == b'B'
+        assert atomic_db[b"1"] == b"B"
 
-    def test_atomic_db_with_reverted_delete_batch(self, atomic_db: AtomicDatabaseAPI) -> None:
+    def test_atomic_db_with_reverted_delete_batch(
+        self, atomic_db: AtomicDatabaseAPI
+    ) -> None:
         class CustomException(Exception):
             pass
 
-        atomic_db[b'key-1'] = b'origin'
+        atomic_db[b"key-1"] = b"origin"
 
         with pytest.raises(CustomException):
             with atomic_db.atomic_batch() as batch:
-                batch.delete(b'key-1')
+                batch.delete(b"key-1")
 
-                assert b'key-1' not in batch
+                assert b"key-1" not in batch
                 with pytest.raises(KeyError):
-                    assert batch[b'key-1']
+                    assert batch[b"key-1"]
 
-                raise CustomException('pretend something went wrong')
+                raise CustomException("pretend something went wrong")
 
-        assert atomic_db[b'key-1'] == b'origin'
+        assert atomic_db[b"key-1"] == b"origin"
 
-    def test_atomic_db_temporary_state_dropped_across_batches(self,
-                                                              atomic_db: AtomicDatabaseAPI) -> None:
+    def test_atomic_db_temporary_state_dropped_across_batches(
+        self, atomic_db: AtomicDatabaseAPI
+    ) -> None:
         class CustomException(Exception):
             pass
 
-        atomic_db[b'key-1'] = b'origin'
+        atomic_db[b"key-1"] = b"origin"
 
         with pytest.raises(CustomException):
             with atomic_db.atomic_batch() as batch:
-                batch.delete(b'key-1')
-                batch.set(b'key-2', b'val-2')
-                raise CustomException('pretend something went wrong')
+                batch.delete(b"key-1")
+                batch.set(b"key-2", b"val-2")
+                raise CustomException("pretend something went wrong")
 
         with atomic_db.atomic_batch() as batch:
-            assert batch[b'key-1'] == b'origin'
-            assert b'key-2' not in batch
+            assert batch[b"key-1"] == b"origin"
+            assert b"key-2" not in batch
 
     def test_atomic_db_with_exception_batch(self, atomic_db: AtomicDatabaseAPI) -> None:
-        atomic_db.set(b'key-1', b'value-1')
+        atomic_db.set(b"key-1", b"value-1")
 
         try:
             with atomic_db.atomic_batch() as batch:
-                batch.set(b'key-1', b'new-value-1')
-                batch.set(b'key-2', b'value-2')
+                batch.set(b"key-1", b"new-value-1")
+                batch.set(b"key-2", b"value-2")
                 raise Exception
         except Exception:
             pass
 
-        assert atomic_db.get(b'key-1') == b'value-1'
+        assert atomic_db.get(b"key-1") == b"value-1"
 
         with pytest.raises(KeyError):
-            atomic_db[b'key-2']
+            atomic_db[b"key-2"]
```

### Comparing `py-evm-0.7.0a1/eth/tools/db/base.py` & `py-evm-0.7.0a2/eth/tools/db/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 import pytest
 
-from eth.abc import DatabaseAPI
+from eth.abc import (
+    DatabaseAPI,
+)
 
 
 class DatabaseAPITestSuite:
     def test_database_api_get(self, db: DatabaseAPI) -> None:
-        db[b'key-1'] = b'value-1'
-        assert db.get(b'key-1') == b'value-1'
+        db[b"key-1"] = b"value-1"
+        assert db.get(b"key-1") == b"value-1"
 
     def test_database_api_item_getter(self, db: DatabaseAPI) -> None:
-        db[b'key-1'] = b'value-1'
-        assert db[b'key-1'] == b'value-1'
+        db[b"key-1"] = b"value-1"
+        assert db[b"key-1"] == b"value-1"
 
     def test_database_api_get_missing_key(self, db: DatabaseAPI) -> None:
-        assert b'key-1' not in db
-        assert db.get(b'key-1') is None
+        assert b"key-1" not in db
+        assert db.get(b"key-1") is None
 
     def test_database_api_item_getter_missing_key(self, db: DatabaseAPI) -> None:
-        assert b'key-1' not in db
+        assert b"key-1" not in db
         with pytest.raises(KeyError):
-            db[b'key-1']
+            db[b"key-1"]
 
     def test_database_api_set(self, db: DatabaseAPI) -> None:
-        db[b'key-1'] = b'value-1'
-        assert db[b'key-1'] == b'value-1'
-        db[b'key-1'] = b'value-2'
-        assert db[b'key-1'] == b'value-2'
+        db[b"key-1"] = b"value-1"
+        assert db[b"key-1"] == b"value-1"
+        db[b"key-1"] = b"value-2"
+        assert db[b"key-1"] == b"value-2"
 
     def test_database_api_item_setter(self, db: DatabaseAPI) -> None:
-        db.set(b'key-1', b'value-1')
-        assert db[b'key-1'] == b'value-1'
-        db.set(b'key-1', b'value-2')
-        assert db[b'key-1'] == b'value-2'
+        db.set(b"key-1", b"value-1")
+        assert db[b"key-1"] == b"value-1"
+        db.set(b"key-1", b"value-2")
+        assert db[b"key-1"] == b"value-2"
 
     def test_database_api_exists(self, db: DatabaseAPI) -> None:
-        assert db.exists(b'key-1') is False
+        assert db.exists(b"key-1") is False
 
-        db[b'key-1'] = b'value-1'
+        db[b"key-1"] = b"value-1"
 
-        assert db.exists(b'key-1') is True
+        assert db.exists(b"key-1") is True
 
     def test_database_api_contains_checking(self, db: DatabaseAPI) -> None:
-        assert b'key-1' not in db
+        assert b"key-1" not in db
 
-        db[b'key-1'] = b'value-1'
+        db[b"key-1"] = b"value-1"
 
-        assert b'key-1' in db
+        assert b"key-1" in db
 
     def test_database_api_delete(self, db: DatabaseAPI) -> None:
-        db[b'key-1'] = b'value-1'
+        db[b"key-1"] = b"value-1"
 
-        assert b'key-1' in db
+        assert b"key-1" in db
 
-        db.delete(b'key-1')
+        db.delete(b"key-1")
 
-        assert not db.exists(b'key-1')
-        assert b'key-1' not in db
+        assert not db.exists(b"key-1")
+        assert b"key-1" not in db
 
     def test_database_api_item_delete(self, db: DatabaseAPI) -> None:
-        db[b'key-1'] = b'value-1'
+        db[b"key-1"] = b"value-1"
 
-        assert b'key-1' in db
+        assert b"key-1" in db
 
-        del db[b'key-1']
+        del db[b"key-1"]
 
-        assert b'key-1' not in db
+        assert b"key-1" not in db
 
     def test_database_api_delete_missing_key(self, db: DatabaseAPI) -> None:
-        assert b'key-1' not in db
-        db.delete(b'key-1')
+        assert b"key-1" not in db
+        db.delete(b"key-1")
 
     def test_database_api_item_delete_missing_key(self, db: DatabaseAPI) -> None:
-        assert b'key-1' not in db
+        assert b"key-1" not in db
         with pytest.raises(KeyError):
-            del db[b'key-1']
+            del db[b"key-1"]
```

### Comparing `py-evm-0.7.0a1/eth/tools/fixtures/__init__.py` & `py-evm-0.7.0a2/eth/tools/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a1/eth/tools/fixtures/_utils.py` & `py-evm-0.7.0a2/eth/tools/fixtures/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import fnmatch
 import functools
 import os
-
 from typing import (
     Any,
     Callable,
     Iterable,
 )
 
-from eth_utils import to_tuple
+from eth_utils import (
+    to_tuple,
+)
 
 
 @to_tuple
 def recursive_find_files(base_dir: str, pattern: str) -> Iterable[str]:
     for dirpath, _, filenames in os.walk(base_dir):
         for filename in filenames:
             if fnmatch.fnmatch(filename, pattern):
@@ -22,13 +23,14 @@
 def require_pytest(fn: Callable[..., Any]) -> Callable[..., Any]:
     @functools.wraps(fn)
     def inner(*args: Any, **kwargs: Any) -> Callable[..., Any]:
         try:
             import pytest  # noqa: F401
         except ImportError:
             raise ImportError(
-                'pytest is required to use the fixture_tests.  Please ensure '
-                'it is installed.'
+                "pytest is required to use the fixture_tests.  Please ensure "
+                "it is installed."
             )
         else:
             return fn(*args, **kwargs)
+
     return inner
```

### Comparing `py-evm-0.7.0a1/eth/tools/fixtures/fillers/_utils.py` & `py-evm-0.7.0a2/eth/tools/fixtures/fillers/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,61 +4,67 @@
     Any,
     Dict,
     List,
     Tuple,
     Type,
 )
 
-from eth_keys import keys
+from eth_keys import (
+    keys,
+)
 from eth_typing import (
     Address,
 )
 from eth_utils import (
     int_to_big_endian,
 )
 
 from eth._utils.db import (
     apply_state_dict,
 )
 from eth._utils.padding import (
     pad32,
 )
-from eth.constants import BLANK_ROOT_HASH
-from eth.db.atomic import AtomicDB
+from eth.constants import (
+    BLANK_ROOT_HASH,
+)
+from eth.db.atomic import (
+    AtomicDB,
+)
 from eth.typing import (
     AccountState,
     TransactionDict,
 )
 from eth.vm.state import (
     BaseState,
 )
 
 
 def wrap_in_list(item: Any) -> List[Any]:
     return [item]
 
 
-def add_transaction_to_group(group: Dict[str, Any],
-                             transaction: TransactionDict) -> Tuple[Dict[str, Any], Dict[str, int]]:
-
+def add_transaction_to_group(
+    group: Dict[str, Any], transaction: TransactionDict
+) -> Tuple[Dict[str, Any], Dict[str, int]]:
     for key in ["gasPrice", "nonce", "secretKey", "to"]:
-        if key in transaction and transaction[key] != group[key]:   # type: ignore # https://github.com/python/mypy/issues/5359 # noqa: 501
+        if key in transaction and transaction[key] != group[key]:  # type: ignore # https://github.com/python/mypy/issues/5359 # noqa: 501
             raise ValueError(f"Can't add transaction as it differs in {key}")
 
     new_group = copy.deepcopy(group)
     indexes = {}
     for key, index_key in [("data", "data"), ("gasLimit", "gas"), ("value", "value")]:
         if key in group:
             if key not in transaction:
                 if len(new_group[key]) != 1:
                     raise ValueError(f"Can't add transaction as {key} is ambiguous")
                 index = 0
             else:
-                if transaction[key] not in new_group[key]:      # type: ignore # https://github.com/python/mypy/issues/5359 # noqa: 501
-                    new_group[key].append(transaction[key])     # type: ignore # https://github.com/python/mypy/issues/5359 # noqa: 501
+                if transaction[key] not in new_group[key]:  # type: ignore # https://github.com/python/mypy/issues/5359 # noqa: 501
+                    new_group[key].append(transaction[key])  # type: ignore # https://github.com/python/mypy/issues/5359 # noqa: 501
                 index = new_group[key].index(transaction[key])  # type: ignore # https://github.com/python/mypy/issues/5359 # noqa: 501
             indexes[index_key] = index
         else:
             assert key not in transaction
     return new_group, indexes
```

### Comparing `py-evm-0.7.0a1/eth/tools/fixtures/fillers/common.py` & `py-evm-0.7.0a2/eth/tools/fixtures/fillers/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,60 +6,61 @@
     wraps,
 )
 from typing import (
     Any,
     Callable,
     Dict,
 )
+
+from eth_utils import (
+    apply_formatters_to_dict,
+    decode_hex,
+    to_canonical_address,
+)
 from eth_utils.toolz import (
     assoc,
     assoc_in,
     curry,
     merge,
 )
-from eth_utils import (
-    apply_formatters_to_dict,
-    decode_hex,
-    to_canonical_address,
-)
 
-from eth.tools.fixtures.helpers import (
-    get_test_name,
+from eth.tools._utils.mappings import (
+    deep_merge,
 )
 from eth.tools._utils.normalization import (
     normalize_environment,
     normalize_execution,
+    normalize_networks,
     normalize_state,
     normalize_transaction,
-    normalize_networks,
-)
-from eth.tools._utils.mappings import (
-    deep_merge,
 )
 from eth.tools._utils.vyper import (
     compile_vyper_lll,
 )
-
+from eth.tools.fixtures.helpers import (
+    get_test_name,
+)
 from eth.typing import (
     GeneralState,
     TransactionDict,
 )
 
 from ._utils import (
     add_transaction_to_group,
     wrap_in_list,
 )
 
-
 #
 # Defaults
 #
 
 DEFAULT_MAIN_ENVIRONMENT = {
-    "currentCoinbase": to_canonical_address("0x2adc25665018aa1fe0e6bc666dac8fc2697ff9ba"),
+    "currentCoinbase": to_canonical_address(
+        "0x2adc25665018aa1fe0e6bc666dac8fc2697ff9ba"
+    ),
     "currentDifficulty": 131072,
     "currentGasLimit": 1000000,
     "currentNumber": 1,
     "currentTimestamp": 1000,
     "previousHash": decode_hex(
         "0x5e20a0453cecd065ea59c37ac63e079ee08998b6045136a8ce6635c7912ec0b6"
     ),
@@ -67,59 +68,68 @@
 
 
 DEFAULT_MAIN_TRANSACTION: TransactionDict = {
     "data": b"",
     "gasLimit": 100000,
     "gasPrice": 0,
     "nonce": 0,
-    "secretKey": decode_hex("0x45a915e4d060149eb4365960e6a7a45f334393093061116b197e3240065ff2d8"),
+    "secretKey": decode_hex(
+        "0x45a915e4d060149eb4365960e6a7a45f334393093061116b197e3240065ff2d8"
+    ),
     "to": to_canonical_address("0x0f572e5295c57f15886f9b263e2f6d2d6c7b5ec6"),
-    "value": 0
+    "value": 0,
 }
 
 
 def get_default_transaction(networks: Any) -> TransactionDict:
     return DEFAULT_MAIN_TRANSACTION
 
 
 DEFAULT_EXECUTION = {
     "address": to_canonical_address("0x0f572e5295c57f15886f9b263e2f6d2d6c7b5ec6"),
     "origin": to_canonical_address("0xcd1722f2947def4cf144679da39c4c32bdc35681"),
     "caller": to_canonical_address("0xcd1722f2947def4cf144679da39c4c32bdc35681"),
     "value": 1000000000000000000,
     "data": b"",
     "gasPrice": 1,
-    "gas": 100000
+    "gas": 100000,
 }
 
 
 Test = namedtuple("Test", ["filler", "fill_kwargs"])
 # make `None` default for fill_kwargs
 Test.__new__.__defaults__ = (None,)  # type: ignore
 
 
 #
 # Filler Generation
 #
 
-def setup_filler(name: str, environment: Dict[Any, Any] = None) -> Dict[str, Dict[str, Any]]:
+
+def setup_filler(
+    name: str, environment: Dict[Any, Any] = None
+) -> Dict[str, Dict[str, Any]]:
     environment = normalize_environment(environment or {})
-    return {name: {
-        "env": environment,
-        "pre": {},
-    }}
+    return {
+        name: {
+            "env": environment,
+            "pre": {},
+        }
+    }
 
 
-def setup_main_filler(name: str, environment: Dict[Any, Any] = None) -> Dict[str, Dict[str, Any]]:
+def setup_main_filler(
+    name: str, environment: Dict[Any, Any] = None
+) -> Dict[str, Dict[str, Any]]:
     """
     Kick off the filler generation process by creating the general filler scaffold with
     a test name and general information about the testing environment.
 
-    For tests for the main chain, the `environment` parameter is expected to be a dictionary with
-    some or all of the following keys:
+    For tests for the main chain, the `environment` parameter is expected to be a
+    dictionary with some or all of the following keys:
 
     +------------------------+---------------------------------+
     | key                    | description                     |
     +========================+=================================+
     | ``"currentCoinbase"``  | the coinbase address            |
     +------------------------+---------------------------------+
     | ``"currentNumber"``    | the block number                |
@@ -137,131 +147,148 @@
 
 
 def pre_state(*raw_state: GeneralState, filler: Dict[str, Any]) -> None:
     """
     Specify the state prior to the test execution. Multiple invocations don't override
     the state but extend it instead.
 
-    In general, the elements of `state_definitions` are nested dictionaries of the following form:
+    In general, the elements of `state_definitions` are nested dictionaries of the
+    following form:
 
     .. code-block:: python
 
         {
             address: {
                 "nonce": <account nonce>,
                 "balance": <account balance>,
                 "code": <account code>,
                 "storage": {
                     <storage slot>: <storage value>
                 }
             }
         }
 
-    To avoid unnecessary nesting especially if only few fields per account are specified, the
-    following and similar formats are possible as well:
+    To avoid unnecessary nesting especially if only few fields per account are
+    specified, the following and similar formats are possible as well:
 
     .. code-block:: python
 
         (address, "balance", <account balance>)
         (address, "storage", <storage slot>, <storage value>)
         (address, "storage", {<storage slot>: <storage value>})
         (address, {"balance", <account balance>})
     """
+
     @wraps(pre_state)
     def _pre_state(filler: Dict[str, Any]) -> Dict[str, Any]:
         test_name = get_test_name(filler)
 
         old_pre_state = filler[test_name].get("pre_state", {})
         pre_state = normalize_state(raw_state)
-        defaults = {address: {
-            "balance": 0,
-            "nonce": 0,
-            "code": b"",
-            "storage": {},
-        } for address in pre_state}
+        defaults = {
+            address: {
+                "balance": 0,
+                "nonce": 0,
+                "code": b"",
+                "storage": {},
+            }
+            for address in pre_state
+        }
         new_pre_state = deep_merge(defaults, old_pre_state, pre_state)
 
         return assoc_in(filler, [test_name, "pre"], new_pre_state)
 
 
-def _expect(post_state: Dict[str, Any],
-            networks: Any,
-            transaction: TransactionDict,
-            filler: Dict[str, Any]) -> Dict[str, Any]:
-
+def _expect(
+    post_state: Dict[str, Any],
+    networks: Any,
+    transaction: TransactionDict,
+    filler: Dict[str, Any],
+) -> Dict[str, Any]:
     test_name = get_test_name(filler)
     test = filler[test_name]
     test_update: Dict[str, Dict[Any, Any]] = {test_name: {}}
 
     pre_state = test.get("pre", {})
     post_state = normalize_state(post_state or {})
-    defaults = {address: {
-        "balance": 0,
-        "nonce": 0,
-        "code": b"",
-        "storage": {},
-    } for address in post_state}
+    defaults = {
+        address: {
+            "balance": 0,
+            "nonce": 0,
+            "code": b"",
+            "storage": {},
+        }
+        for address in post_state
+    }
     result = deep_merge(defaults, pre_state, normalize_state(post_state))
     new_expect = {"result": result}
 
     if transaction is not None:
         transaction = normalize_transaction(
             merge(get_default_transaction(networks), transaction)
         )
         if "transaction" not in test:
-            transaction_group = apply_formatters_to_dict({
-                "data": wrap_in_list,
-                "gasLimit": wrap_in_list,
-                "value": wrap_in_list,
-            }, transaction)
+            transaction_group = apply_formatters_to_dict(
+                {
+                    "data": wrap_in_list,
+                    "gasLimit": wrap_in_list,
+                    "value": wrap_in_list,
+                },
+                transaction,
+            )
             indexes = {
                 index_key: 0
                 for transaction_key, index_key in [
                     ("gasLimit", "gas"),
                     ("value", "value"),
                     ("data", "data"),
                 ]
                 if transaction_key in transaction_group
             }
         else:
             transaction_group, indexes = add_transaction_to_group(
                 test["transaction"], transaction
             )
         new_expect = assoc(new_expect, "indexes", indexes)
-        test_update = assoc_in(test_update, [test_name, "transaction"], transaction_group)
+        test_update = assoc_in(
+            test_update, [test_name, "transaction"], transaction_group
+        )
 
     if networks is not None:
         networks = normalize_networks(networks)
         new_expect = assoc(new_expect, "networks", networks)
 
     existing_expects = test.get("expect", [])
     expect = existing_expects + [new_expect]
     test_update = assoc_in(test_update, [test_name, "expect"], expect)
 
     return deep_merge(filler, test_update)
 
 
-def expect(post_state: Dict[str, Any] = None,
-           networks: Any = None,
-           transaction: TransactionDict = None) -> Callable[..., Dict[str, Any]]:
-
+def expect(
+    post_state: Dict[str, Any] = None,
+    networks: Any = None,
+    transaction: TransactionDict = None,
+) -> Callable[..., Dict[str, Any]]:
     """
     Specify the expected result for the test.
 
-    For state tests, multiple expectations can be given, differing in the transaction data, gas
-    limit, and value, in the applicable networks, and as a result also in the post state. VM tests
-    support only a single expectation with no specified network and no transaction (here, its role
-    is played by :func:`~eth.tools.fixtures.fillers.execution`).
+    For state tests, multiple expectations can be given, differing in the transaction
+    data, gas limit, and value, in the applicable networks, and as a result also in the
+    post state. VM tests support only a single expectation with no specified network and
+    no transaction.
+    (here, its role is played by :func:`~eth.tools.fixtures.fillers.execution`).
 
     * ``post_state`` is a list of state definition in the same form as expected
       by :func:`~eth.tools.fixtures.fillers.pre_state`. State items that are
       not set explicitly default to their pre state.
 
-    * ``networks`` defines the forks under which the expectation is applicable. It should be a
-        sublist of the following identifiers (also available in `ALL_FORKS`):
+    * ``networks`` defines the forks under which the expectation is applicable. It
+        should be a sublist of the following identifiers
+        (also available in `ALL_FORKS`):
 
       * ``"Frontier"``
       * ``"Homestead"``
       * ``"EIP150"``
       * ``"EIP158"``
       * ``"Byzantium"``
 
@@ -277,26 +304,26 @@
       | ``"gasPrice"`` | the gas price,                |
       +----------------+-------------------------------+
       | ``"nonce"``    | the transaction nonce,        |
       +----------------+-------------------------------+
       | ``"value"``    | the transaction value         |
       +----------------+-------------------------------+
 
-    In addition, one should specify either the signature itself (via keys ``"v"``, ``"r"``,
-    and ``"s"``) or a private key used for signing (via ``"secretKey"``).
+    In addition, one should specify either the signature itself (via keys ``"v"``,
+    ``"r"``, and ``"s"``) or a private key used for signing (via ``"secretKey"``).
     """
     return partial(_expect, post_state, networks, transaction)
 
 
 @curry
 def execution(execution: Dict[str, Any], filler: Dict[str, Any]) -> Dict[str, Any]:
     """
     For VM tests, specify the code that is being run as well as the current state of
-    the EVM. State tests don't support this object. The parameter is a dictionary specifying some
-    or all of the following keys:
+    the EVM. State tests don't support this object. The parameter is a dictionary
+    specifying some or all of the following keys:
 
     +--------------------+------------------------------------------------------------+
     |  key               | description                                                |
     +====================+============================================================+
     | ``"address"``      | the address of the account executing the code              |
     +--------------------+------------------------------------------------------------+
     | ``"caller"``       | the caller address                                         |
@@ -334,9 +361,9 @@
     test_name = get_test_name(filler)
     return deep_merge(
         filler,
         {
             test_name: {
                 "exec": execution,
             }
-        }
+        },
     )
```

### Comparing `py-evm-0.7.0a1/eth/tools/fixtures/fillers/formatters.py` & `py-evm-0.7.0a2/eth/tools/fixtures/fillers/formatters.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,111 +8,129 @@
     apply_formatter_to_array,
     apply_formatters_to_dict,
     apply_formatters_to_sequence,
     encode_hex,
     to_checksum_address,
     to_hex,
 )
+from eth_utils.toolz import (
+    curried,
+)
 
-from eth_utils.toolz import curried
-
-
-environment_formatter = apply_formatters_to_dict({
-    "currentCoinbase": to_checksum_address,
-    "previousHash": encode_hex,
-    "currentNumber": to_hex,
-    "currentDifficulty": to_hex,
-    "currentGasLimit": to_hex,
-    "currentTimestamp": to_hex,
-})
+environment_formatter = apply_formatters_to_dict(
+    {
+        "currentCoinbase": to_checksum_address,
+        "previousHash": encode_hex,
+        "currentNumber": to_hex,
+        "currentDifficulty": to_hex,
+        "currentGasLimit": to_hex,
+        "currentTimestamp": to_hex,
+    }
+)
 
 
 storage_item_formatter: Callable[[List[Any]], List[Any]]
 storage_item_formatter = apply_formatters_to_sequence([to_hex, to_hex])
 storage_formatter = curried.itemmap(storage_item_formatter)
 
 
-account_state_formatter = apply_formatters_to_dict({
-    "balance": to_hex,
-    "nonce": to_hex,
-    "code": encode_hex,
-    "storage": storage_formatter,
-})
+account_state_formatter = apply_formatters_to_dict(
+    {
+        "balance": to_hex,
+        "nonce": to_hex,
+        "code": encode_hex,
+        "storage": storage_formatter,
+    }
+)
 
 
 state_item_formatter: Callable[[List[Any]], List[Any]]
-state_item_formatter = apply_formatters_to_sequence([to_checksum_address, account_state_formatter])
+state_item_formatter = apply_formatters_to_sequence(
+    [to_checksum_address, account_state_formatter]
+)
 state_formatter = curried.itemmap(state_item_formatter)
 
 
-transaction_group_formatter = apply_formatters_to_dict({
-    # all transaction types
-    "to": to_checksum_address,
-    "data": apply_formatter_to_array(encode_hex),
-    "gasLimit": apply_formatter_to_array(to_hex),
-    "gasPrice": to_hex,
-    "nonce": to_hex,
-    "secretKey": encode_hex,
-    "value": apply_formatter_to_array(to_hex),
-})
-
-
-execution_formatter = apply_formatters_to_dict({
-    "address": to_checksum_address,
-    "origin": to_checksum_address,
-    "caller": to_checksum_address,
-    "code": encode_hex,
-    "value": to_hex,
-    "data": encode_hex,
-    "gasPrice": to_hex,
-    "gas": to_hex,
-})
-
-
-expect_element_formatter = apply_formatters_to_dict({
-    "result": state_formatter
-})
+transaction_group_formatter = apply_formatters_to_dict(
+    {
+        # all transaction types
+        "to": to_checksum_address,
+        "data": apply_formatter_to_array(encode_hex),
+        "gasLimit": apply_formatter_to_array(to_hex),
+        "gasPrice": to_hex,
+        "nonce": to_hex,
+        "secretKey": encode_hex,
+        "value": apply_formatter_to_array(to_hex),
+    }
+)
+
+
+execution_formatter = apply_formatters_to_dict(
+    {
+        "address": to_checksum_address,
+        "origin": to_checksum_address,
+        "caller": to_checksum_address,
+        "code": encode_hex,
+        "value": to_hex,
+        "data": encode_hex,
+        "gasPrice": to_hex,
+        "gas": to_hex,
+    }
+)
+
+
+expect_element_formatter = apply_formatters_to_dict({"result": state_formatter})
 expect_formatter: Callable[[List[Any]], List[Any]]
 expect_formatter = apply_formatter_to_array(expect_element_formatter)
 
 
-test_formatter = apply_formatters_to_dict({
-    "env": environment_formatter,
-    "pre": state_formatter,
-    "transaction": transaction_group_formatter,
-    "expect": expect_formatter,
-    "exec": execution_formatter,
-})
+test_formatter = apply_formatters_to_dict(
+    {
+        "env": environment_formatter,
+        "pre": state_formatter,
+        "transaction": transaction_group_formatter,
+        "expect": expect_formatter,
+        "exec": execution_formatter,
+    }
+)
 filler_formatter = curried.valmap(test_formatter)
 
 
-state_post_formatter = apply_formatters_to_dict({
-    "hash": encode_hex
-})
-
-
-filled_state_test_formatter = curried.valmap(apply_formatters_to_dict({
-    "env": environment_formatter,
-    "pre": state_formatter,
-    "transaction": transaction_group_formatter,
-    "post": state_post_formatter,
-}))
-
-call_create_item_formatter = apply_formatters_to_dict({
-    "data": encode_hex,
-    "destination": to_checksum_address,
-    "gasLimit": to_hex,
-    "value": to_hex,
-})
+state_post_formatter = apply_formatters_to_dict({"hash": encode_hex})
+
+
+filled_state_test_formatter = curried.valmap(
+    apply_formatters_to_dict(
+        {
+            "env": environment_formatter,
+            "pre": state_formatter,
+            "transaction": transaction_group_formatter,
+            "post": state_post_formatter,
+        }
+    )
+)
+
+call_create_item_formatter = apply_formatters_to_dict(
+    {
+        "data": encode_hex,
+        "destination": to_checksum_address,
+        "gasLimit": to_hex,
+        "value": to_hex,
+    }
+)
 call_creates_formatter: Callable[[List[Any]], List[Any]]
 call_creates_formatter = apply_formatter_to_array(call_create_item_formatter)
 
-filled_vm_test_formatter = curried.valmap(apply_formatters_to_dict({
-    "env": environment_formatter,
-    "pre": state_formatter,
-    "exec": execution_formatter,
-    "post": state_formatter,
-    "callcreates": call_creates_formatter,
-    "logs": encode_hex,
-    "gas": to_hex,
-    "output": encode_hex,
-}))
+filled_vm_test_formatter = curried.valmap(
+    apply_formatters_to_dict(
+        {
+            "env": environment_formatter,
+            "pre": state_formatter,
+            "exec": execution_formatter,
+            "post": state_formatter,
+            "callcreates": call_creates_formatter,
+            "logs": encode_hex,
+            "gas": to_hex,
+            "output": encode_hex,
+        }
+    )
+)
```

### Comparing `py-evm-0.7.0a1/eth/tools/fixtures/fillers/main.py` & `py-evm-0.7.0a2/eth/tools/fixtures/fillers/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,53 +4,59 @@
 )
 
 from eth_utils.toolz import (
     assoc_in,
     merge,
 )
 
+from eth.tools._utils.git import (
+    get_version_from_git,
+)
 from eth.tools.fixtures.helpers import (
     get_test_name,
 )
-from eth.tools._utils.git import get_version_from_git
 
 from .formatters import (
     filled_state_test_formatter,
     filled_vm_test_formatter,
 )
-from .state import fill_state_test
-from .vm import fill_vm_test
-
+from .state import (
+    fill_state_test,
+)
+from .vm import (
+    fill_vm_test,
+)
 
 FILLED_WITH_TEMPLATE = "py-evm-{version}"
 
 
 #
 # Primary test filler
 #
-def fill_test(filler: Dict[str, Any],
-              info: Dict[str, Any] = None,
-              apply_formatter: bool = True,
-              **kwargs: Any) -> Dict[str, Any]:
-
+def fill_test(
+    filler: Dict[str, Any],
+    info: Dict[str, Any] = None,
+    apply_formatter: bool = True,
+    **kwargs: Any
+) -> Dict[str, Any]:
     test_name = get_test_name(filler)
     test = filler[test_name]
 
     if "transaction" in test:
         filled = fill_state_test(filler)
         formatter = filled_state_test_formatter
     elif "exec" in test:
         filled = fill_vm_test(filler, **kwargs)
         formatter = filled_vm_test_formatter
     else:
         raise ValueError("Given filler does not appear to be for VM or state test")
 
     info = merge(
         {"filledwith": FILLED_WITH_TEMPLATE.format(version=get_version_from_git())},
-        info if info else {}
+        info if info else {},
     )
     filled = assoc_in(filled, [test_name, "_info"], info)
 
     if apply_formatter:
         return formatter(filled)
     else:
         return filled
```

### Comparing `py-evm-0.7.0a1/eth/tools/fixtures/fillers/state.py` & `py-evm-0.7.0a2/eth/tools/fixtures/fillers/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,61 @@
-from collections import defaultdict
+from collections import (
+    defaultdict,
+)
 from typing import (
     Any,
     Dict,
     List,
 )
 
-from eth_utils import encode_hex
+from eth_utils import (
+    encode_hex,
+)
 
-from eth.tools.fixtures.helpers import (
-    get_test_name,
+from eth.tools._utils.mappings import (
+    deep_merge,
 )
 from eth.tools._utils.normalization import (
     normalize_environment,
     normalize_networks,
     normalize_state,
     normalize_transaction_group,
 )
-from eth.tools._utils.mappings import deep_merge
-from eth.vm.forks.byzantium.state import ByzantiumState
-from eth.vm.forks.constantinople.state import ConstantinopleState
-from eth.vm.forks.frontier.state import FrontierState
-from eth.vm.forks.homestead.state import HomesteadState
-from eth.vm.forks.istanbul.state import IstanbulState
-from eth.vm.forks.petersburg.state import PetersburgState
-from eth.vm.forks.spurious_dragon.state import SpuriousDragonState
-from eth.vm.forks.tangerine_whistle.state import TangerineWhistleState
+from eth.tools.fixtures.helpers import (
+    get_test_name,
+)
+from eth.vm.forks.byzantium.state import (
+    ByzantiumState,
+)
+from eth.vm.forks.constantinople.state import (
+    ConstantinopleState,
+)
+from eth.vm.forks.frontier.state import (
+    FrontierState,
+)
+from eth.vm.forks.homestead.state import (
+    HomesteadState,
+)
+from eth.vm.forks.istanbul.state import (
+    IstanbulState,
+)
+from eth.vm.forks.petersburg.state import (
+    PetersburgState,
+)
+from eth.vm.forks.spurious_dragon.state import (
+    SpuriousDragonState,
+)
+from eth.vm.forks.tangerine_whistle.state import (
+    TangerineWhistleState,
+)
 
 from ._utils import (
     calc_state_root,
 )
 
-
 ALL_NETWORKS = [
     "Frontier",
     "Homestead",
     "EIP150",
     "EIP158",
     "Byzantium",
     "Constantinople",
@@ -73,20 +94,22 @@
         indexes = expect["indexes"]
         networks = normalize_networks(expect["networks"])
         result = normalize_state(expect["result"])
         post_state = deep_merge(pre_state, result)
         for network in networks:
             state_class = STATE_CLASSES[network]
             post_state_root = calc_state_root(post_state, state_class)
-            post[network].append({
-                "hash": encode_hex(post_state_root),
-                "indexes": indexes,
-            })
+            post[network].append(
+                {
+                    "hash": encode_hex(post_state_root),
+                    "indexes": indexes,
+                }
+            )
 
     return {
         test_name: {
             "env": environment,
             "pre": pre_state,
             "transaction": transaction_group,
-            "post": post
+            "post": post,
         }
     }
```

### Comparing `py-evm-0.7.0a1/eth/tools/fixtures/fillers/vm.py` & `py-evm-0.7.0a2/eth/tools/fixtures/fillers/vm.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,39 +2,43 @@
     Any,
     Dict,
     Iterable,
     Tuple,
     Union,
 )
 
-from eth.tools.fixtures.helpers import (
-    get_test_name,
+from eth.tools._utils.hashing import (
+    hash_log_entries,
+)
+from eth.tools._utils.mappings import (
+    deep_merge,
 )
 from eth.tools._utils.normalization import (
     normalize_bytes,
     normalize_call_creates,
     normalize_environment,
     normalize_execution,
     normalize_int,
     normalize_logs,
     normalize_state,
 )
-from eth.tools._utils.hashing import hash_log_entries
-from eth.tools._utils.mappings import deep_merge
+from eth.tools.fixtures.helpers import (
+    get_test_name,
+)
 
 
 def fill_vm_test(
-        filler: Dict[str, Any],
-        *,
-        call_creates: Any = None,
-        gas_price: Union[int, str] = None,
-        gas_remaining: Union[int, str] = 0,
-        logs: Iterable[Tuple[bytes, Tuple[int, ...], bytes]] = None,
-        output: bytes = b"") -> Dict[str, Dict[str, Any]]:
-
+    filler: Dict[str, Any],
+    *,
+    call_creates: Any = None,
+    gas_price: Union[int, str] = None,
+    gas_remaining: Union[int, str] = 0,
+    logs: Iterable[Tuple[bytes, Tuple[int, ...], bytes]] = None,
+    output: bytes = b""
+) -> Dict[str, Dict[str, Any]]:
     test_name = get_test_name(filler)
     test = filler[test_name]
 
     environment = normalize_environment(test["env"])
     pre_state = normalize_state(test["pre"])
     execution = normalize_execution(test["exec"])
```

### Comparing `py-evm-0.7.0a1/eth/tools/fixtures/generation.py` & `py-evm-0.7.0a2/eth/tools/fixtures/generation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import hashlib
-
 from typing import (
     Any,
     Callable,
     Iterable,
 )
 
 from eth_utils.toolz import (
@@ -32,39 +31,42 @@
 
 def get_fixtures_file_hash(all_fixture_paths: Iterable[str]) -> str:
     """
     Returns the MD5 hash of the fixture files.  Used for cache busting.
     """
     hasher = hashlib.md5()
     for fixture_path in sorted(all_fixture_paths):
-        with open(fixture_path, 'rb') as fixture_file:
+        with open(fixture_path, "rb") as fixture_file:
             hasher.update(fixture_file.read())
     return hasher.hexdigest()
 
 
 @curry
-def generate_fixture_tests(metafunc: Any,
-                           base_fixture_path: str,
-                           filter_fn: Callable[..., Any] = identity,
-                           preprocess_fn: Callable[..., Any] = identity) -> None:
+def generate_fixture_tests(
+    metafunc: Any,
+    base_fixture_path: str,
+    filter_fn: Callable[..., Any] = identity,
+    preprocess_fn: Callable[..., Any] = identity,
+) -> None:
     """
     Helper function for use with `pytest_generate_tests` which will use the
     pytest caching facilities to reduce the load time for fixture tests.
 
     - `metafunc` is the parameter from `pytest_generate_tests`
     - `base_fixture_path` is the base path that fixture files will be collected from.
-    - `filter_fn` handles ignoring or marking the various fixtures.  See `filter_fixtures`.
+    - `filter_fn` handles ignoring or marking the various fixtures.
+       See `filter_fixtures`.
     - `preprocess_fn` handles any preprocessing that should be done on the raw
        fixtures (such as expanding the statetest fixtures to be multiple tests for
        each fork.
     """
-    if 'fixture_data' in metafunc.fixturenames:
+    if "fixture_data" in metafunc.fixturenames:
         all_fixtures = find_fixtures(base_fixture_path)
 
         if not all_fixtures:
             raise AssertionError(
                 f"Suspiciously found zero fixtures: {base_fixture_path}"
             )
 
         filtered_fixtures = filter_fn(preprocess_fn(all_fixtures))
 
-        metafunc.parametrize('fixture_data', filtered_fixtures, ids=idfn)
+        metafunc.parametrize("fixture_data", filtered_fixtures, ids=idfn)
```

### Comparing `py-evm-0.7.0a1/eth/tools/fixtures/helpers.py` & `py-evm-0.7.0a2/eth/tools/fixtures/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,191 +1,168 @@
 import os
-
-import rlp
-
 from typing import (
-    cast,
     Any,
     Dict,
     Iterable,
     Tuple,
     Type,
+    cast,
 )
 
+from eth_utils import (
+    to_normalized_address,
+)
 from eth_utils.toolz import (
     assoc,
     first,
 )
+import rlp
 
-from eth_utils import (
-    to_normalized_address,
+from eth import (
+    MainnetChain,
+    constants,
+)
+from eth._utils.state import (
+    diff_state,
 )
-
-from eth import MainnetChain
 from eth.abc import (
     BlockAPI,
     ChainAPI,
     StateAPI,
     VirtualMachineAPI,
 )
-from eth import constants
-from eth.db.atomic import AtomicDB
 from eth.chains.mainnet import (
     MainnetDAOValidatorVM,
 )
+from eth.db.atomic import (
+    AtomicDB,
+)
 from eth.tools.builder.chain import (
     disable_pow_check,
 )
 from eth.typing import (
     AccountState,
 )
-from eth._utils.state import (
-    diff_state,
-)
 from eth.vm.forks import (
-    PetersburgVM,
-    ConstantinopleVM,
+    BerlinVM,
     ByzantiumVM,
-    TangerineWhistleVM,
+    ConstantinopleVM,
     FrontierVM,
+    GrayGlacierVM,
     HomesteadVM as BaseHomesteadVM,
-    SpuriousDragonVM,
     IstanbulVM,
-    BerlinVM,
     LondonVM,
-    GrayGlacierVM,
     ParisVM,
+    PetersburgVM,
     ShanghaiVM,
+    SpuriousDragonVM,
+    TangerineWhistleVM,
 )
 
 
 #
 # State Setup
 #
 def setup_state(desired_state: AccountState, state: StateAPI) -> None:
     for account, account_data in desired_state.items():
-        for slot, value in account_data['storage'].items():
+        for slot, value in account_data["storage"].items():
             state.set_storage(account, slot, value)
 
-        nonce = account_data['nonce']
-        code = account_data['code']
-        balance = account_data['balance']
+        nonce = account_data["nonce"]
+        code = account_data["code"]
+        balance = account_data["balance"]
 
         state.set_nonce(account, nonce)
         state.set_code(account, code)
         state.set_balance(account, balance)
     state.persist()
 
 
 def verify_state(expected_state: AccountState, state: StateAPI) -> None:
     diff = diff_state(expected_state, state)
     new_line = "\n"
     if diff:
         error_messages = []
         for account, field, actual_value, expected_value in diff:
-            if field == 'balance':
+            if field == "balance":
                 error_messages.append(
                     f"{to_normalized_address(account)}(balance) | "
                     f"Actual: {actual_value!r} | Expected: {expected_value!r} | "
                     f"Delta: {cast(int, actual_value) - cast(int, expected_value)}"
                 )
             else:
                 error_messages.append(
                     f"{to_normalized_address(account)}({field}) | "
                     f"Actual: {actual_value!r} | Expected: {expected_value!r}"
                 )
         raise AssertionError(
-            f"State DB did not match expected state on {len(error_messages)} values:{new_line}"
-            f"{f'{new_line} - '.join(error_messages)}"
+            f"State DB did not match expected state on {len(error_messages)} "
+            f"values:{new_line} {f'{new_line} - '.join(error_messages)}"
         )
 
 
-def chain_vm_configuration(fixture: Dict[str, Any]) -> Iterable[Tuple[int, Type[VirtualMachineAPI]]]:  # noqa: E501
-    network = fixture['network']
+def chain_vm_configuration(
+    fixture: Dict[str, Any]
+) -> Iterable[Tuple[int, Type[VirtualMachineAPI]]]:
+    network = fixture["network"]
 
-    if network == 'Frontier':
-        return (
-            (0, FrontierVM),
-        )
-    elif network == 'Homestead':
+    if network == "Frontier":
+        return ((0, FrontierVM),)
+    elif network == "Homestead":
         HomesteadVM = BaseHomesteadVM.configure(support_dao_fork=False)
-        return (
-            (0, HomesteadVM),
-        )
-    elif network == 'EIP150':
-        return (
-            (0, TangerineWhistleVM),
-        )
-    elif network == 'EIP158':
-        return (
-            (0, SpuriousDragonVM),
-        )
-    elif network == 'Byzantium':
-        return (
-            (0, ByzantiumVM),
-        )
-    elif network == 'Constantinople':
-        return (
-            (0, ConstantinopleVM),
-        )
-    elif network == 'ConstantinopleFix':
-        return (
-            (0, PetersburgVM),
-        )
-    elif network == 'Istanbul':
-        return (
-            (0, IstanbulVM),
-        )
-    elif network == 'Berlin':
-        return (
-            (0, BerlinVM),
-        )
-    elif network == 'London':
-        return (
-            (0, LondonVM),
-        )
-    elif network == 'Merge':
-        return (
-            (0, ParisVM),
-        )
+        return ((0, HomesteadVM),)
+    elif network == "EIP150":
+        return ((0, TangerineWhistleVM),)
+    elif network == "EIP158":
+        return ((0, SpuriousDragonVM),)
+    elif network == "Byzantium":
+        return ((0, ByzantiumVM),)
+    elif network == "Constantinople":
+        return ((0, ConstantinopleVM),)
+    elif network == "ConstantinopleFix":
+        return ((0, PetersburgVM),)
+    elif network == "Istanbul":
+        return ((0, IstanbulVM),)
+    elif network == "Berlin":
+        return ((0, BerlinVM),)
+    elif network == "London":
+        return ((0, LondonVM),)
+    elif network == "Merge":
+        return ((0, ParisVM),)
     elif network == "Shanghai":
-        return (
-            (0, ShanghaiVM),
-        )
-    elif network == 'FrontierToHomesteadAt5':
+        return ((0, ShanghaiVM),)
+    elif network == "FrontierToHomesteadAt5":
         HomesteadVM = BaseHomesteadVM.configure(support_dao_fork=False)
         return (
             (0, FrontierVM),
             (5, HomesteadVM),
         )
-    elif network == 'HomesteadToEIP150At5':
+    elif network == "HomesteadToEIP150At5":
         HomesteadVM = BaseHomesteadVM.configure(support_dao_fork=False)
         return (
             (0, HomesteadVM),
             (5, TangerineWhistleVM),
         )
-    elif network == 'HomesteadToDaoAt5':
+    elif network == "HomesteadToDaoAt5":
         HomesteadVM = MainnetDAOValidatorVM.configure(
             support_dao_fork=True,
             _dao_fork_block_number=5,
         )
-        return (
-            (0, HomesteadVM),
-        )
-    elif network == 'EIP158ToByzantiumAt5':
+        return ((0, HomesteadVM),)
+    elif network == "EIP158ToByzantiumAt5":
         return (
             (0, SpuriousDragonVM),
             (5, ByzantiumVM),
         )
-    elif network == 'ByzantiumToConstantinopleFixAt5':
+    elif network == "ByzantiumToConstantinopleFixAt5":
         return (
             (0, ByzantiumVM),
             (5, PetersburgVM),
         )
-    elif network == 'BerlinToLondonAt5':
+    elif network == "BerlinToLondonAt5":
         return (
             (0, BerlinVM),
             (5, LondonVM),
         )
     elif network == "ArrowGlacierToMergeAtDiffC0000":
         # Transition expected at 6 for all tests written thus far
         return (
@@ -207,34 +184,34 @@
 
 
 def genesis_fields_from_fixture(fixture: Dict[str, Any]) -> Dict[str, Any]:
     """
     Convert all genesis fields in a fixture to a dictionary of header fields and values.
     """
 
-    header_fields = fixture['genesisBlockHeader']
+    header_fields = fixture["genesisBlockHeader"]
     base_fields = {
-        'parent_hash': header_fields['parentHash'],
-        'uncles_hash': header_fields['uncleHash'],
-        'coinbase': header_fields['coinbase'],
-        'state_root': header_fields['stateRoot'],
-        'transaction_root': header_fields['transactionsTrie'],
-        'receipt_root': header_fields['receiptTrie'],
-        'bloom': header_fields['bloom'],
-        'difficulty': header_fields['difficulty'],
-        'block_number': header_fields['number'],
-        'gas_limit': header_fields['gasLimit'],
-        'gas_used': header_fields['gasUsed'],
-        'timestamp': header_fields['timestamp'],
-        'extra_data': header_fields['extraData'],
-        'mix_hash': header_fields['mixHash'],
-        'nonce': header_fields['nonce'],
+        "parent_hash": header_fields["parentHash"],
+        "uncles_hash": header_fields["uncleHash"],
+        "coinbase": header_fields["coinbase"],
+        "state_root": header_fields["stateRoot"],
+        "transaction_root": header_fields["transactionsTrie"],
+        "receipt_root": header_fields["receiptTrie"],
+        "bloom": header_fields["bloom"],
+        "difficulty": header_fields["difficulty"],
+        "block_number": header_fields["number"],
+        "gas_limit": header_fields["gasLimit"],
+        "gas_used": header_fields["gasUsed"],
+        "timestamp": header_fields["timestamp"],
+        "extra_data": header_fields["extraData"],
+        "mix_hash": header_fields["mixHash"],
+        "nonce": header_fields["nonce"],
     }
-    if 'baseFeePerGas' in header_fields:
-        return assoc(base_fields, 'base_fee_per_gas', header_fields['baseFeePerGas'])
+    if "baseFeePerGas" in header_fields:
+        return assoc(base_fields, "base_fee_per_gas", header_fields["baseFeePerGas"])
     else:
         return base_fields
 
 
 def genesis_params_from_fixture(fixture: Dict[str, Any]) -> Dict[str, Any]:
     """
     Convert a genesis fixture into a dict of the configurable header fields and values.
@@ -244,79 +221,82 @@
     """
 
     params = genesis_fields_from_fixture(fixture)
 
     # Confirm that (currently) non-configurable defaults are set correctly,
     #   then remove them because they cannot be configured on the header.
     defaults = (
-        ('parent_hash', constants.GENESIS_PARENT_HASH),
-        ('uncles_hash', constants.EMPTY_UNCLE_HASH),
-        ('bloom', constants.GENESIS_BLOOM),
-        ('block_number', constants.GENESIS_BLOCK_NUMBER),
-        ('gas_used', constants.GENESIS_GAS_USED),
+        ("parent_hash", constants.GENESIS_PARENT_HASH),
+        ("uncles_hash", constants.EMPTY_UNCLE_HASH),
+        ("bloom", constants.GENESIS_BLOOM),
+        ("block_number", constants.GENESIS_BLOCK_NUMBER),
+        ("gas_used", constants.GENESIS_GAS_USED),
     )
 
     for key, default_val in defaults:
         supplied_val = params.pop(key)
         if supplied_val != default_val:
-            raise ValueError(f"Unexpected genesis {key}: {supplied_val}, expected: {default_val}")
+            raise ValueError(
+                f"Unexpected genesis {key}: {supplied_val}, expected: {default_val}"
+            )
 
     return params
 
 
-def new_chain_from_fixture(fixture: Dict[str, Any],
-                           chain_cls: Type[ChainAPI] = MainnetChain) -> ChainAPI:
+def new_chain_from_fixture(
+    fixture: Dict[str, Any], chain_cls: Type[ChainAPI] = MainnetChain
+) -> ChainAPI:
     base_db = AtomicDB()
 
     vm_config = chain_vm_configuration(fixture)
 
     ChainFromFixture = chain_cls.configure(
-        'ChainFromFixture',
+        "ChainFromFixture",
         vm_configuration=vm_config,
     )
 
-    if 'sealEngine' in fixture and fixture['sealEngine'] == 'NoProof':
+    if "sealEngine" in fixture and fixture["sealEngine"] == "NoProof":
         ChainFromFixture = disable_pow_check(ChainFromFixture)
 
     return ChainFromFixture.from_genesis(
         base_db,
         genesis_params=genesis_params_from_fixture(fixture),
-        genesis_state=fixture['pre'],
+        genesis_state=fixture["pre"],
     )
 
 
 def apply_fixture_block_to_chain(
-        block_fixture: Dict[str, Any],
-        chain: ChainAPI,
-        perform_validation: bool = True
+    block_fixture: Dict[str, Any], chain: ChainAPI, perform_validation: bool = True
 ) -> Tuple[BlockAPI, BlockAPI, bytes]:
     """
     :return: (provided_block, imported_block, rlp_encoded_imported_block)
     """
     # The block to import may be in a different block-class-range than the
     # chain's current one, so we use the block number specified in the
     # fixture to look up the correct block class.
-    if 'blockHeader' in block_fixture:
-        block_number = block_fixture['blockHeader']['number']
-        block_class = chain.get_vm_class_for_block_number(block_number).get_block_class()
+    if "blockHeader" in block_fixture:
+        block_number = block_fixture["blockHeader"]["number"]
+        block_class = chain.get_vm_class_for_block_number(
+            block_number
+        ).get_block_class()
     else:
         block_class = chain.get_vm().get_block_class()
 
-    block = rlp.decode(block_fixture['rlp'], sedes=block_class)
+    block = rlp.decode(block_fixture["rlp"], sedes=block_class)
 
     import_result = chain.import_block(block, perform_validation=perform_validation)
     imported_block = import_result.imported_block
 
     rlp_encoded_imported_block = rlp.encode(imported_block, sedes=block_class)
 
     return (block, imported_block, rlp_encoded_imported_block)
 
 
 def should_run_slow_tests() -> bool:
-    if os.environ.get('TRAVIS_EVENT_TYPE') == 'cron':
+    if os.environ.get("TRAVIS_EVENT_TYPE") == "cron":
         return True
     return False
 
 
 def get_test_name(filler: Dict[str, Any]) -> str:
     assert len(filler) == 1
     return first(filler)
```

### Comparing `py-evm-0.7.0a1/eth/tools/fixtures/loading.py` & `py-evm-0.7.0a2/eth/tools/fixtures/loading.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import functools
 import json
 import os
-
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     Tuple,
 )
 
+from eth_utils import (
+    to_tuple,
+)
 from eth_utils.toolz import (
     curry,
     identity,
 )
 
-from eth_utils import to_tuple
-
 from ._utils import (
     recursive_find_files,
     require_pytest,
 )
 
 
 #
@@ -56,37 +56,39 @@
     Loads a fixture file, caching the most recent files it loaded.
     """
     with open(fixture_path) as fixture_file:
         file_fixtures = json.load(fixture_file)
     return file_fixtures
 
 
-def load_fixture(fixture_path: str,
-                 fixture_key: str,
-                 normalize_fn: Callable[..., Any] = identity) -> Dict[str, Any]:
+def load_fixture(
+    fixture_path: str, fixture_key: str, normalize_fn: Callable[..., Any] = identity
+) -> Dict[str, Any]:
     """
     Loads a specific fixture from a fixture file, optionally passing it through
     a normalization function.
     """
     file_fixtures = load_json_fixture(fixture_path)
     fixture = normalize_fn(file_fixtures[fixture_key])
     return fixture
 
 
 @require_pytest
 @curry
-def filter_fixtures(all_fixtures: Iterable[Any],
-                    fixtures_base_dir: str,
-                    mark_fn: Callable[[str, str], bool] = None,
-                    ignore_fn: Callable[..., bool] = None) -> Any:
+def filter_fixtures(
+    all_fixtures: Iterable[Any],
+    fixtures_base_dir: str,
+    mark_fn: Callable[[str, str], bool] = None,
+    ignore_fn: Callable[..., bool] = None,
+) -> Any:
     """
     Helper function for filtering test fixtures.
 
-    - `fixtures_base_dir` should be the base directory that the fixtures were collected from.
-    - `mark_fn` should be a function which either returns `None` or a `pytest.mark` object.
+    - `fixtures_base_dir` should be the base dir that the fixtures were collected from.
+    - `mark_fn` should be a func which either returns `None` or a `pytest.mark` object.
     - `ignore_fn` should be a function which returns `True` for any fixture
        which should be ignored.
     """
     import pytest  # noqa: F401
 
     for fixture_data in all_fixtures:
         fixture_path = fixture_data[0]
```

### Comparing `py-evm-0.7.0a1/eth/tools/mining.py` & `py-evm-0.7.0a2/eth/tools/mining.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from eth.abc import (
-    BlockAPI,
     BlockAndMetaWitness,
+    BlockAPI,
     VirtualMachineAPI,
 )
 from eth.consensus import (
     pow,
 )
 
 
 class POWMiningMixin(VirtualMachineAPI):
     """
     A VM that does POW mining as well. Should be used only in tests, when we
     need to programatically populate a ChainDB.
     """
+
     def finalize_block(self, block: BlockAPI) -> BlockAndMetaWitness:
         block_result = super().finalize_block(block)
         block = block_result.block
 
         nonce, mix_hash = pow.mine_pow_nonce(
-            block.number, block.header.mining_hash, block.header.difficulty)
+            block.number, block.header.mining_hash, block.header.difficulty
+        )
 
-        mined_block = block.copy(header=block.header.copy(nonce=nonce, mix_hash=mix_hash))
+        mined_block = block.copy(
+            header=block.header.copy(nonce=nonce, mix_hash=mix_hash)
+        )
 
         return BlockAndMetaWitness(mined_block, block_result.meta_witness)
```

### Comparing `py-evm-0.7.0a1/eth/typing.py` & `py-evm-0.7.0a2/eth/typing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Generic,
     Iterable,
     List,
-    Optional,
     NewType,
+    Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
-    TYPE_CHECKING,
     Union,
 )
 
 from eth_typing import (
     Address,
     BlockNumber,
     Hash32,
@@ -30,22 +30,20 @@
         BlockHeaderAPI,
         SignedTransactionAPI,
         VirtualMachineAPI,
         WithdrawalAPI,
     )
 
 
-JournalDBCheckpoint = NewType('JournalDBCheckpoint', int)
+JournalDBCheckpoint = NewType("JournalDBCheckpoint", int)
 
-AccountDetails = TypedDict('AccountDetails',
-                           {'balance': int,
-                            'nonce': int,
-                            'code': bytes,
-                            'storage': Dict[int, int]
-                            })
+AccountDetails = TypedDict(
+    "AccountDetails",
+    {"balance": int, "nonce": int, "code": bytes, "storage": Dict[int, int]},
+)
 AccountState = Dict[Address, AccountDetails]
 AccountDiff = Iterable[Tuple[Address, str, Union[int, bytes], Union[int, bytes]]]
 
 
 class Block(TypedDict, total=False):
     header: "BlockHeaderAPI"
     transactions: Sequence["SignedTransactionAPI"]
@@ -59,60 +57,67 @@
     # series of gaps before the chain head
     Tuple[BlockRange, ...],
     # the first missing block number at the tip of the chain
     BlockNumber,
 ]
 
 GeneralState = Union[
-    AccountState,
-    List[Tuple[Address, Dict[str, Union[int, bytes, Dict[int, int]]]]]
+    AccountState, List[Tuple[Address, Dict[str, Union[int, bytes, Dict[int, int]]]]]
 ]
 
 GenesisDict = Dict[str, Union[int, BlockNumber, bytes, Hash32]]
 
 BytesOrView = Union[bytes, memoryview]
 
 Normalizer = Callable[[Dict[Any, Any]], Dict[str, Any]]
 
-RawAccountDetails = TypedDict('RawAccountDetails',
-                              {'balance': HexStr,
-                               'nonce': HexStr,
-                               'code': HexStr,
-                               'storage': Dict[HexStr, HexStr]
-                               })
-
-TransactionDict = TypedDict('TransactionDict',
-                            {'nonce': int,
-                             'gasLimit': int,
-                             'gasPrice': int,
-                             'to': Address,
-                             'value': int,
-                             'data': bytes,
-                             'secretKey': bytes,
-                             })
+RawAccountDetails = TypedDict(
+    "RawAccountDetails",
+    {
+        "balance": HexStr,
+        "nonce": HexStr,
+        "code": HexStr,
+        "storage": Dict[HexStr, HexStr],
+    },
+)
+
+TransactionDict = TypedDict(
+    "TransactionDict",
+    {
+        "nonce": int,
+        "gasLimit": int,
+        "gasPrice": int,
+        "to": Address,
+        "value": int,
+        "data": bytes,
+        "secretKey": bytes,
+    },
+)
 
 TransactionNormalizer = Callable[[TransactionDict], TransactionDict]
 
-VMFork = Tuple[BlockNumber, Type['VirtualMachineAPI']]
+VMFork = Tuple[BlockNumber, Type["VirtualMachineAPI"]]
 
 VMConfiguration = Sequence[VMFork]
 
 VRS = NewType("VRS", Tuple[int, int, int])
 
 IntConvertible = Union[int, bytes, HexStr, str]
 
 
-TFunc = TypeVar('TFunc')
+TFunc = TypeVar("TFunc")
 
 
 class StaticMethod(Generic[TFunc]):
     """
     A property class purely to convince mypy to let us assign a function to an
-    instance variable. See more at: https://github.com/python/mypy/issues/708#issuecomment-405812141
+    instance variable.
+    See more at: https://github.com/python/mypy/issues/708#issuecomment-405812141
     """
+
     def __get__(self, oself: Any, owner: Any) -> TFunc:
         return self._func
 
     def __set__(self, oself: Any, value: TFunc) -> None:
         self._func = value
```

### Comparing `py-evm-0.7.0a1/eth/validation.py` & `py-evm-0.7.0a2/eth/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,80 +1,75 @@
 import functools
-
 from typing import (
     Any,
-    cast,
     Dict,
     Iterable,
     Sequence,
     Tuple,
     Type,
     Union,
+    cast,
 )
 
 from eth_typing import (
     Address,
     Hash32,
 )
-
 from eth_utils import (
-    is_list_like,
     ValidationError,
+    is_list_like,
+)
+from eth_utils.toolz import (
+    dicttoolz,
+    functoolz,
+    itertoolz,
 )
-from eth_utils.toolz import dicttoolz
-
-from eth_utils.toolz import functoolz
-
-from eth_utils.toolz import itertoolz
 
 from eth._utils.headers import (
     compute_gas_limit_bounds,
 )
-from eth.abc import VirtualMachineAPI
+from eth.abc import (
+    VirtualMachineAPI,
+)
 from eth.constants import (
     SECPK1_N,
-    UINT_256_MAX,
     UINT_64_MAX,
+    UINT_256_MAX,
 )
-
 from eth.typing import (
     BytesOrView,
 )
 
 
 def validate_is_bytes(value: bytes, title: str = "Value") -> None:
     if not isinstance(value, bytes):
-        raise ValidationError(
-            f"{title} must be a byte string.  Got: {type(value)}"
-        )
+        raise ValidationError(f"{title} must be a byte string.  Got: {type(value)}")
 
 
 def validate_is_bytes_or_view(value: BytesOrView, title: str = "Value") -> None:
     if isinstance(value, (bytes, memoryview)):
         return
-    raise ValidationError(
-        f"{title} must be bytes or memoryview. Got {type(value)}"
-    )
+    raise ValidationError(f"{title} must be bytes or memoryview. Got {type(value)}")
 
 
 def validate_is_integer(value: Union[int, bool], title: str = "Value") -> None:
     if not isinstance(value, int) or isinstance(value, bool):
-        raise ValidationError(
-            f"{title} must be a an integer.  Got: {type(value)}"
-        )
+        raise ValidationError(f"{title} must be a an integer.  Got: {type(value)}")
 
 
 def validate_length(value: Sequence[Any], length: int, title: str = "Value") -> None:
     if not len(value) == length:
         raise ValidationError(
             f"{title} must be of length {length}.  Got {value} of length {len(value)}"
         )
 
 
-def validate_length_lte(value: Sequence[Any], maximum_length: int, title: str = "Value") -> None:
+def validate_length_lte(
+    value: Sequence[Any], maximum_length: int, title: str = "Value"
+) -> None:
     if len(value) > maximum_length:
         raise ValidationError(
             f"{title} must be of length less than or equal to {maximum_length}.  "
             f"Got {value} of length {len(value)}"
         )
 
 
@@ -84,96 +79,73 @@
             f"{title} {value} is not greater than or equal to {minimum}"
         )
     validate_is_integer(value)
 
 
 def validate_gt(value: int, minimum: int, title: str = "Value") -> None:
     if value <= minimum:
-        raise ValidationError(
-            f"{title} {value} is not greater than {minimum}"
-        )
+        raise ValidationError(f"{title} {value} is not greater than {minimum}")
     validate_is_integer(value, title=title)
 
 
 def validate_lte(value: int, maximum: int, title: str = "Value") -> None:
     if value > maximum:
-        raise ValidationError(
-            f"{title} {value} is not less than or equal to {maximum}"
-        )
+        raise ValidationError(f"{title} {value} is not less than or equal to {maximum}")
     validate_is_integer(value, title=title)
 
 
 def validate_lt(value: int, maximum: int, title: str = "Value") -> None:
     if value >= maximum:
-        raise ValidationError(
-            f"{title} {value} is not less than {maximum}"
-        )
+        raise ValidationError(f"{title} {value} is not less than {maximum}")
     validate_is_integer(value, title=title)
 
 
 def validate_canonical_address(value: Address, title: str = "Value") -> None:
     if not isinstance(value, bytes) or not len(value) == 20:
-        raise ValidationError(
-            f"{title} {value!r} is not a valid canonical address"
-        )
+        raise ValidationError(f"{title} {value!r} is not a valid canonical address")
 
 
 def validate_multiple_of(value: int, multiple_of: int, title: str = "Value") -> None:
     if not value % multiple_of == 0:
-        raise ValidationError(
-            f"{title} {value} is not a multiple of {multiple_of}"
-        )
+        raise ValidationError(f"{title} {value} is not a multiple of {multiple_of}")
 
 
 def validate_is_boolean(value: bool, title: str = "Value") -> None:
     if not isinstance(value, bool):
-        raise ValidationError(
-            f"{title} must be an boolean.  Got type: {type(value)}"
-        )
+        raise ValidationError(f"{title} must be an boolean.  Got type: {type(value)}")
 
 
 def validate_word(value: Hash32, title: str = "Value") -> None:
     if not isinstance(value, bytes):
         raise ValidationError(
             f"{title} is not a valid word. Must be of bytes type: Got: {type(value)}"
         )
     elif not len(value) == 32:
         raise ValidationError(
-            f"{title} is not a valid word. Must be 32 bytes in length: Got: {len(value)}"
+            f"{title} is not a valid word. Must be 32 bytes in length: "
+            f"Got: {len(value)}"
         )
 
 
 def validate_uint64(value: int, title: str = "Value") -> None:
     if not isinstance(value, int) or isinstance(value, bool):
-        raise ValidationError(
-            f"{title} must be an integer: Got: {type(value)}"
-        )
+        raise ValidationError(f"{title} must be an integer: Got: {type(value)}")
     if value < 0:
-        raise ValidationError(
-            f"{title} cannot be negative: Got: {value}"
-        )
+        raise ValidationError(f"{title} cannot be negative: Got: {value}")
     if value > UINT_64_MAX:
-        raise ValidationError(
-            f"{title} exceeds maximum uint64 size.  Got: {value}"
-        )
+        raise ValidationError(f"{title} exceeds maximum uint64 size.  Got: {value}")
 
 
 def validate_uint256(value: int, title: str = "Value") -> None:
     if not isinstance(value, int) or isinstance(value, bool):
-        raise ValidationError(
-            f"{title} must be an integer: Got: {type(value)}"
-        )
+        raise ValidationError(f"{title} must be an integer: Got: {type(value)}")
     if value < 0:
-        raise ValidationError(
-            f"{title} cannot be negative: Got: {value}"
-        )
+        raise ValidationError(f"{title} cannot be negative: Got: {value}")
     if value > UINT_256_MAX:
-        raise ValidationError(
-            f"{title} exceeds maximum uint256 size.  Got: {value}"
-        )
+        raise ValidationError(f"{title} exceeds maximum uint256 size.  Got: {value}")
 
 
 def validate_stack_int(value: int) -> None:
     if 0 <= value <= UINT_256_MAX:
         return
     raise ValidationError(
         "Invalid Stack Item: Must be a 256 bit integer. Got {value!r}"
@@ -193,15 +165,14 @@
 
 
 def validate_unique(values: Iterable[Any], title: str = "Value") -> None:
     if not itertoolz.isdistinct(values):
         duplicates = functoolz.pipe(
             values,
             itertoolz.frequencies,  # get the frequencies
-
             # filter to ones that occure > 1
             functoolz.partial(dicttoolz.valfilter, lambda v: v > 1),
             sorted,  # sort them
             tuple,  # cast them to an immutiable form
         )
         raise ValidationError(
             f"{title} does not contain unique items.  Duplicates: "
@@ -216,21 +187,26 @@
     for entry in access_list:
         validate_is_list_like(entry, "Transaction.access_list entry")
         if len(entry) != 2:
             raise ValidationError(
                 "Transaction.access_list entry does not have 2 values. "
                 "Needs address value and storage key list."
             )
-        validate_canonical_address(cast(Address, entry[0]), "Transaction.access_list entry address")
+        validate_canonical_address(
+            cast(Address, entry[0]), "Transaction.access_list entry address"
+        )
         validate_is_list_like(entry[1], "Transaction.access_list entry storage keys")
         for k in entry[1]:
             validate_is_integer(k, "Transaction.access_list entry storage key")
 
 
-def validate_is_list_like(obj: Sequence[Any], title: str = "Value",) -> None:
+def validate_is_list_like(
+    obj: Sequence[Any],
+    title: str = "Value",
+) -> None:
     if not is_list_like(obj):
         raise ValidationError(f"{title} is not list like: {repr(obj)}")
 
 
 def validate_block_number(block_number: int, title: str = "Block Number") -> None:
     validate_is_integer(block_number, title)
     validate_gte(block_number, 0, title)
@@ -239,21 +215,20 @@
 def validate_vm_block_numbers(vm_block_numbers: Iterable[int]) -> None:
     validate_unique(vm_block_numbers, title="Block Number set")
 
     for block_number in vm_block_numbers:
         validate_block_number(block_number)
 
 
-def validate_vm_configuration(vm_configuration: Tuple[Tuple[int, Type[VirtualMachineAPI]], ...],
-                              ) -> None:
-    validate_vm_block_numbers(tuple(
-        block_number
-        for block_number, _
-        in vm_configuration
-    ))
+def validate_vm_configuration(
+    vm_configuration: Tuple[Tuple[int, Type[VirtualMachineAPI]], ...],
+) -> None:
+    validate_vm_block_numbers(
+        tuple(block_number for block_number, _ in vm_configuration)
+    )
 
 
 def validate_gas_limit(gas_limit: int, parent_gas_limit: int) -> None:
     low_bound, high_bound = compute_gas_limit_bounds(parent_gas_limit)
     if gas_limit < low_bound:
         raise ValidationError(
             f"The gas limit {gas_limit} is too low. It must be at least {low_bound}"
@@ -261,29 +236,30 @@
     elif gas_limit > high_bound:
         raise ValidationError(
             f"The gas limit {gas_limit} is too high. It must be at most {high_bound}"
         )
 
 
 ALLOWED_HEADER_FIELDS = {
-    'coinbase',
-    'difficulty',
-    'gas_limit',
-    'timestamp',
-    'extra_data',
-    'mix_hash',
-    'nonce',
-    'uncles_hash',
-    'transaction_root',
-    'receipt_root',
-    'withdrawals_root',
+    "coinbase",
+    "difficulty",
+    "gas_limit",
+    "timestamp",
+    "extra_data",
+    "mix_hash",
+    "nonce",
+    "uncles_hash",
+    "transaction_root",
+    "receipt_root",
+    "withdrawals_root",
 }
 
 
 def validate_header_params_for_configuration(header_params: Dict[str, Any]) -> None:
     extra_fields = set(header_params.keys()).difference(ALLOWED_HEADER_FIELDS)
     if extra_fields:
         raise ValidationError(
             "The `configure_header` method may only be used with the fields "
             f"({', '.join(tuple(sorted(ALLOWED_HEADER_FIELDS)))}). "
-            f"The provided fields ({', '.join(tuple(sorted(extra_fields)))}) are not supported"
+            f"The provided fields ({', '.join(tuple(sorted(extra_fields)))}) "
+            "are not supported"
         )
```

### Comparing `py-evm-0.7.0a1/eth/vm/base.py` & `py-evm-0.7.0a2/eth/vm/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,30 +12,41 @@
     Sequence,
     Set,
     Tuple,
     Type,
     Union,
 )
 
-from cached_property import cached_property
-from eth_hash.auto import keccak
+from cached_property import (
+    cached_property,
+)
+from eth_hash.auto import (
+    keccak,
+)
 from eth_typing import (
     Address,
     Hash32,
 )
 from eth_utils import (
     ValidationError,
     encode_hex,
 )
 import rlp
 
+from eth._utils.datatypes import (
+    Configurable,
+)
+from eth._utils.db import (
+    get_block_header_by_hash,
+    get_parent_header,
+)
 from eth.abc import (
     AtomicDatabaseAPI,
-    BlockAPI,
     BlockAndMetaWitness,
+    BlockAPI,
     BlockHeaderAPI,
     ChainContextAPI,
     ChainDatabaseAPI,
     ComputationAPI,
     ConsensusAPI,
     ConsensusContextAPI,
     ExecutionContextAPI,
@@ -52,34 +63,29 @@
     PowConsensus,
 )
 from eth.constants import (
     GENESIS_PARENT_HASH,
     MAX_PREV_HEADER_DEPTH,
     MAX_UNCLES,
 )
-from eth.db.trie import make_trie_root_and_nodes
+from eth.db.trie import (
+    make_trie_root_and_nodes,
+)
 from eth.exceptions import (
     HeaderNotFound,
 )
 from eth.rlp.headers import (
     BlockHeader,
 )
 from eth.rlp.sedes import (
     uint32,
 )
-from eth._utils.datatypes import (
-    Configurable,
-)
-from eth._utils.db import (
-    get_parent_header,
-    get_block_header_by_hash,
-)
 from eth.validation import (
-    validate_length_lte,
     validate_gas_limit,
+    validate_length_lte,
 )
 from eth.vm.execution_context import (
     ExecutionContext,
 )
 from eth.vm.interrupt import (
     EVMMissingData,
 )
@@ -100,22 +106,22 @@
     fork: str = None
     chaindb: ChainDatabaseAPI = None
     _state_class: Type[StateAPI] = None
 
     _state = None
     _block = None
 
-    cls_logger = logging.getLogger('eth.vm.base.VM')
+    cls_logger = logging.getLogger("eth.vm.base.VM")
 
     def __init__(
         self,
         header: BlockHeaderAPI,
         chaindb: ChainDatabaseAPI,
         chain_context: ChainContextAPI,
-        consensus_context: ConsensusContextAPI
+        consensus_context: ConsensusContextAPI,
     ) -> None:
         self.chaindb = chaindb
         self.chain_context = chain_context
         self.consensus_context = consensus_context
         self._initial_header = header
 
     def get_header(self) -> BlockHeaderAPI:
@@ -123,54 +129,60 @@
             return self._initial_header
         else:
             return self._block.header
 
     def get_block(self) -> BlockAPI:
         if self._block is None:
             block_class = self.get_block_class()
-            self._block = block_class.from_header(header=self._initial_header, chaindb=self.chaindb)
+            self._block = block_class.from_header(
+                header=self._initial_header, chaindb=self.chaindb
+            )
         return self._block
 
     @property
     def state(self) -> StateAPI:
         if self._state is None:
-            self._state = self.build_state(self.chaindb.db,
-                                           self.get_header(),
-                                           self.chain_context,
-                                           self.previous_hashes)
+            self._state = self.build_state(
+                self.chaindb.db,
+                self.get_header(),
+                self.chain_context,
+                self.previous_hashes,
+            )
         return self._state
 
     @classmethod
-    def build_state(cls,
-                    db: AtomicDatabaseAPI,
-                    header: BlockHeaderAPI,
-                    chain_context: ChainContextAPI,
-                    previous_hashes: Iterable[Hash32] = (),
-                    ) -> StateAPI:
-        execution_context = cls.create_execution_context(header, previous_hashes, chain_context)
+    def build_state(
+        cls,
+        db: AtomicDatabaseAPI,
+        header: BlockHeaderAPI,
+        chain_context: ChainContextAPI,
+        previous_hashes: Iterable[Hash32] = (),
+    ) -> StateAPI:
+        execution_context = cls.create_execution_context(
+            header, previous_hashes, chain_context
+        )
         return cls.get_state_class()(db, execution_context, header.state_root)
 
     @cached_property
     def _consensus(self) -> ConsensusAPI:
         return self.consensus_class(self.consensus_context)
 
     #
     # Logging
     #
     @property
     def logger(self) -> logging.Logger:
-        return logging.getLogger(f'eth.vm.base.VM.{self.__class__.__name__}')
+        return logging.getLogger(f"eth.vm.base.VM.{self.__class__.__name__}")
 
     #
     # Execution
     #
-    def apply_transaction(self,
-                          header: BlockHeaderAPI,
-                          transaction: SignedTransactionAPI
-                          ) -> Tuple[ReceiptAPI, ComputationAPI]:
+    def apply_transaction(
+        self, header: BlockHeaderAPI, transaction: SignedTransactionAPI
+    ) -> Tuple[ReceiptAPI, ComputationAPI]:
         self.validate_transaction_against_header(header, transaction)
 
         # Mark current state as un-revertable, since new transaction is starting...
         self.state.lock_changes()
 
         computation = self.state.apply_transaction(transaction)
         receipt = self.make_receipt(header, transaction, computation, self.state)
@@ -179,15 +191,15 @@
         return receipt, computation
 
     @classmethod
     def create_execution_context(
         cls,
         header: BlockHeaderAPI,
         prev_hashes: Iterable[Hash32],
-        chain_context: ChainContextAPI
+        chain_context: ChainContextAPI,
     ) -> ExecutionContextAPI:
         fee_recipient = cls.consensus_class.get_fee_recipient(header)
         try:
             base_fee = header.base_fee_per_gas
         except AttributeError:
             return ExecutionContext(
                 coinbase=fee_recipient,
@@ -208,25 +220,26 @@
                 mix_hash=header.mix_hash,
                 gas_limit=header.gas_limit,
                 prev_hashes=prev_hashes,
                 chain_id=chain_context.chain_id,
                 base_fee_per_gas=base_fee,
             )
 
-    def execute_bytecode(self,
-                         origin: Address,
-                         gas_price: int,
-                         gas: int,
-                         to: Address,
-                         sender: Address,
-                         value: int,
-                         data: bytes,
-                         code: bytes,
-                         code_address: Address = None,
-                         ) -> ComputationAPI:
+    def execute_bytecode(
+        self,
+        origin: Address,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        sender: Address,
+        value: int,
+        data: bytes,
+        code: bytes,
+        code_address: Address = None,
+    ) -> ComputationAPI:
         if origin is None:
             origin = sender
 
         # Construct a message
         message = Message(
             gas=gas,
             to=to,
@@ -247,22 +260,20 @@
         return self.state.computation_class.apply_computation(
             self.state,
             message,
             transaction_context,
         )
 
     def apply_all_transactions(
-        self,
-        transactions: Sequence[SignedTransactionAPI],
-        base_header: BlockHeaderAPI
+        self, transactions: Sequence[SignedTransactionAPI], base_header: BlockHeaderAPI
     ) -> Tuple[BlockHeaderAPI, Tuple[ReceiptAPI, ...], Tuple[ComputationAPI, ...]]:
         vm_header = self.get_header()
         if base_header.block_number != vm_header.block_number:
             raise ValidationError(
-                f"This VM instance must only work on block #{self.get_header().block_number}, "
+                f"This VM instance must only work on block #{self.get_header().block_number}, "  # noqa: E501
                 f"but the target header has block #{base_header.block_number}"
             )
 
         receipts = []
         computations = []
         previous_header = base_header
         result_header = base_header
@@ -361,18 +372,22 @@
         )
 
         # Zero out the gas_used before applying transactions. Each applied transaction
         # will increase the gas used in the final new_header.
         header = self.get_header().copy(gas_used=0)
 
         # we need to re-initialize the `state` to update the execution context.
-        self._state = self.get_state_class()(self.chaindb.db, execution_context, header.state_root)
+        self._state = self.get_state_class()(
+            self.chaindb.db, execution_context, header.state_root
+        )
 
         # run all of the transactions.
-        new_header, receipts, _ = self.apply_all_transactions(block.transactions, header)
+        new_header, receipts, _ = self.apply_all_transactions(
+            block.transactions, header
+        )
 
         withdrawals = block.withdrawals if hasattr(block, "withdrawals") else None
 
         if withdrawals:
             # post-shanghai blocks
             self.apply_all_withdrawals(block.withdrawals)
 
@@ -382,15 +397,17 @@
             block.transactions,
             receipts,
             withdrawals=withdrawals,
         )
 
         return self.mine_block(filled_block)
 
-    def mine_block(self, block: BlockAPI, *args: Any, **kwargs: Any) -> BlockAndMetaWitness:
+    def mine_block(
+        self, block: BlockAPI, *args: Any, **kwargs: Any
+    ) -> BlockAndMetaWitness:
         packed_block = self.pack_block(block, *args, **kwargs)
         block_result = self.finalize_block(packed_block)
 
         # Perform validation
         self.validate_block(block_result.block)
 
         return block_result
@@ -399,15 +416,14 @@
         self,
         base_block: BlockAPI,
         new_header: BlockHeaderAPI,
         transactions: Sequence[SignedTransactionAPI],
         receipts: Sequence[ReceiptAPI],
         withdrawals: Sequence[WithdrawalAPI] = None,
     ) -> BlockAPI:
-
         tx_root_hash, tx_kv_nodes = make_trie_root_and_nodes(transactions)
         self.chaindb.persist_trie_data_dict(tx_kv_nodes)
 
         receipt_root_hash, receipt_kv_nodes = make_trie_root_and_nodes(receipts)
         self.chaindb.persist_trie_data_dict(receipt_kv_nodes)
 
         block_fields: "Block" = {"transactions": transactions}
@@ -469,58 +485,60 @@
             else:
                 self.state.commit(snapshot)
 
         # We need to call `persist` here since the state db batches
         # all writes until we tell it to write to the underlying db
         meta_witness = self.state.persist()
 
-        final_block = block.copy(header=block.header.copy(state_root=self.state.state_root))
+        final_block = block.copy(
+            header=block.header.copy(state_root=self.state.state_root)
+        )
 
         self.logger.debug(
-            "%s reads %d unique node hashes, %d addresses, %d bytecodes, and %d storage slots",
+            "%s reads %d unique node hashes, %d addresses, %d bytecodes, and %d storage slots",  # noqa: E501
             final_block,
             len(meta_witness.hashes),
             len(meta_witness.accounts_queried),
             len(meta_witness.account_bytecodes_queried),
             meta_witness.total_slots_queried,
         )
 
         return BlockAndMetaWitness(final_block, meta_witness)
 
     def pack_block(self, block: BlockAPI, *args: Any, **kwargs: Any) -> BlockAPI:
-        if 'uncles' in kwargs:
-            uncles = kwargs.pop('uncles')
-            kwargs.setdefault('uncles_hash', keccak(rlp.encode(uncles)))
+        if "uncles" in kwargs:
+            uncles = kwargs.pop("uncles")
+            kwargs.setdefault("uncles_hash", keccak(rlp.encode(uncles)))
         else:
             uncles = block.uncles
 
         provided_fields = set(kwargs.keys())
         known_fields = set(BlockHeader._meta.field_names)
         unknown_fields = provided_fields.difference(known_fields)
 
         if unknown_fields:
             raise AttributeError(
                 f"Unable to set the field(s) {', '.join(known_fields)} "
                 "on the `BlockHeader` class. "
-                f"Received the following unexpected fields: {', '.join(unknown_fields)}."
+                f"Received the following unexpected fields: {', '.join(unknown_fields)}."  # noqa: E501
             )
 
         header: BlockHeaderAPI = block.header.copy(**kwargs)
 
         packed_block = block.copy(uncles=uncles, header=header)
 
         return packed_block
 
     #
     # Blocks
     #
     @classmethod
-    def generate_block_from_parent_header_and_coinbase(cls,
-                                                       parent_header: BlockHeaderAPI,
-                                                       coinbase: Address) -> BlockAPI:
+    def generate_block_from_parent_header_and_coinbase(
+        cls, parent_header: BlockHeaderAPI, coinbase: Address
+    ) -> BlockAPI:
         block_header = cls.create_header_from_parent(parent_header, coinbase=coinbase)
         block = cls.get_block_class()(
             block_header,
             transactions=[],
             uncles=[],
         )
         return block
@@ -534,17 +552,17 @@
     def get_block_class(cls) -> Type[BlockAPI]:
         if cls.block_class is None:
             raise AttributeError("No `block_class` has been set for this VM")
         else:
             return cls.block_class
 
     @classmethod
-    def get_prev_hashes(cls,
-                        last_block_hash: Hash32,
-                        chaindb: ChainDatabaseAPI) -> Optional[Iterable[Hash32]]:
+    def get_prev_hashes(
+        cls, last_block_hash: Hash32, chaindb: ChainDatabaseAPI
+    ) -> Optional[Iterable[Hash32]]:
         if last_block_hash == GENESIS_PARENT_HASH:
             return
 
         block_header = get_block_header_by_hash(last_block_hash, chaindb)
 
         for _ in range(MAX_PREV_HEADER_DEPTH):
             yield block_header.hash
@@ -560,29 +578,26 @@
     #
     # Transactions
     #
     def create_transaction(self, *args: Any, **kwargs: Any) -> SignedTransactionAPI:
         return self.get_transaction_builder().new_transaction(*args, **kwargs)
 
     @classmethod
-    def create_unsigned_transaction(cls,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> UnsignedTransactionAPI:
+    def create_unsigned_transaction(
+        cls,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+    ) -> UnsignedTransactionAPI:
         return cls.get_transaction_builder().create_unsigned_transaction(
-            nonce=nonce,
-            gas_price=gas_price,
-            gas=gas,
-            to=to,
-            value=value,
-            data=data
+            nonce=nonce, gas_price=gas_price, gas=gas, to=to, value=value, data=data
         )
 
     @classmethod
     def get_transaction_builder(cls) -> Type[TransactionBuilderAPI]:
         return cls.get_block_class().get_transaction_builder()
 
     @classmethod
@@ -609,29 +624,29 @@
         for log_idx, log in enumerate(receipt.logs):
             for topic_idx, topic in enumerate(log.topics):
                 if topic in already_checked:
                     continue
                 elif uint32.serialize(topic) not in receipt.bloom_filter:
                     raise ValidationError(
                         f"The topic at position {topic_idx} from the log entry at "
-                        f"position {log_idx} is not present in the provided bloom filter."
+                        f"position {log_idx} is not present in the provided bloom filter."  # noqa: E501
                     )
                 already_checked.add(topic)
 
     def validate_block(self, block: BlockAPI) -> None:
         if not isinstance(block, self.get_block_class()):
             raise ValidationError(
-                f"This vm ({self!r}) is not equipped to validate a block of type {block!r}"
+                f"This vm ({self!r}) is not equipped to validate a block of type {block!r}"  # noqa: E501
             )
 
         if block.is_genesis:
             validate_length_lte(
                 block.header.extra_data,
                 self.extra_data_max_bytes,
-                title="BlockHeader.extra_data"
+                title="BlockHeader.extra_data",
             )
         else:
             parent_header = get_parent_header(block.header, self.chaindb)
             self.validate_header(block.header, parent_header)
 
         tx_root_hash, _ = make_trie_root_and_nodes(block.transactions)
         if tx_root_hash != block.header.transaction_root:
@@ -660,72 +675,74 @@
                 "`uncles_hash` and block `uncles` do not match.\n"
                 f" - num_uncles       : {len(block.uncles)}\n"
                 f" - block uncle_hash : {local_uncle_hash!r}\n"
                 f" - header uncle_hash: {block.header.uncles_hash!r}"
             )
 
     @classmethod
-    def validate_header(cls,
-                        header: BlockHeaderAPI,
-                        parent_header: BlockHeaderAPI) -> None:
-
+    def validate_header(
+        cls, header: BlockHeaderAPI, parent_header: BlockHeaderAPI
+    ) -> None:
         if parent_header is None:
-            # to validate genesis header, check if it equals canonical header at block number 0
-            raise ValidationError("Must have access to parent header to validate current header")
+            # to validate genesis header, check if it equals canonical header
+            # at block number 0
+            raise ValidationError(
+                "Must have access to parent header to validate current header"
+            )
         else:
             validate_length_lte(
-                header.extra_data, cls.extra_data_max_bytes, title="BlockHeader.extra_data")
+                header.extra_data,
+                cls.extra_data_max_bytes,
+                title="BlockHeader.extra_data",
+            )
 
             cls.validate_gas(header, parent_header)
 
             if header.block_number != parent_header.block_number + 1:
                 raise ValidationError(
                     "Blocks must be numbered consecutively. "
                     f"Block number #{header.block_number} "
                     f"has parent #{parent_header.block_number}"
                 )
 
             # timestamp
             if header.timestamp <= parent_header.timestamp:
                 raise ValidationError(
                     "timestamp must be strictly later than parent, "
-                    f"but is {parent_header.timestamp - header.timestamp} seconds before.\n"
+                    f"but is {parent_header.timestamp - header.timestamp} seconds before.\n"  # noqa: E501
                     f"- child  : {header.timestamp}\n"
                     f"- parent : {parent_header.timestamp}. "
                 )
 
     @classmethod
     def validate_gas(
-            cls,
-            header: BlockHeaderAPI,
-            parent_header: BlockHeaderAPI) -> None:
+        cls, header: BlockHeaderAPI, parent_header: BlockHeaderAPI
+    ) -> None:
         validate_gas_limit(header.gas_limit, parent_header.gas_limit)
 
     def validate_seal(self, header: BlockHeaderAPI) -> None:
         try:
             self._consensus.validate_seal(header)
         except ValidationError as exc:
             self.cls_logger.debug(
                 "Failed to validate seal on header: %r. Error: %s",
                 header.as_dict(),
                 exc,
             )
             raise
 
-    def validate_seal_extension(self,
-                                header: BlockHeaderAPI,
-                                parents: Iterable[BlockHeaderAPI]) -> None:
+    def validate_seal_extension(
+        self, header: BlockHeaderAPI, parents: Iterable[BlockHeaderAPI]
+    ) -> None:
         self._consensus.validate_seal_extension(header, parents)
 
     @classmethod
-    def validate_uncle(cls,
-                       block: BlockAPI,
-                       uncle: BlockHeaderAPI,
-                       uncle_parent: BlockHeaderAPI) -> None:
-
+    def validate_uncle(
+        cls, block: BlockAPI, uncle: BlockHeaderAPI, uncle_parent: BlockHeaderAPI
+    ) -> None:
         if uncle.block_number >= block.number:
             raise ValidationError(
                 f"Uncle number ({uncle.block_number}) is higher than "
                 f"block number ({block.number})"
             )
         if uncle.block_number != uncle_parent.block_number + 1:
             raise ValidationError(
@@ -740,15 +757,17 @@
         if uncle.gas_used > uncle.gas_limit:
             raise ValidationError(
                 f"Uncle's gas usage ({uncle.gas_used}) is above "
                 f"the limit ({uncle.gas_limit})"
             )
 
         uncle_parent_gas_limit = uncle_parent.gas_limit
-        if not hasattr(uncle_parent, 'base_fee_per_gas') and hasattr(uncle, 'base_fee_per_gas'):
+        if not hasattr(uncle_parent, "base_fee_per_gas") and hasattr(
+            uncle, "base_fee_per_gas"
+        ):
             # if Berlin -> London transition, double the parent limit for validation
             uncle_parent_gas_limit *= 2
 
         validate_gas_limit(uncle.gas_limit, uncle_parent_gas_limit)
 
     #
     # State
@@ -760,23 +779,24 @@
 
         return cls._state_class
 
     @contextlib.contextmanager
     def in_costless_state(self) -> Iterator[StateAPI]:
         header = self.get_header()
 
-        temp_block = self.generate_block_from_parent_header_and_coinbase(header, header.coinbase)
+        temp_block = self.generate_block_from_parent_header_and_coinbase(
+            header, header.coinbase
+        )
         prev_hashes = itertools.chain((header.hash,), self.previous_hashes)
 
-        if hasattr(temp_block.header, 'base_fee_per_gas'):
+        if hasattr(temp_block.header, "base_fee_per_gas"):
             free_header = temp_block.header.copy(base_fee_per_gas=0)
         else:
             free_header = temp_block.header
 
-        state = self.build_state(self.chaindb.db,
-                                 free_header,
-                                 self.chain_context,
-                                 prev_hashes)
+        state = self.build_state(
+            self.chaindb.db, free_header, self.chain_context, prev_hashes
+        )
 
         snapshot = state.snapshot()
         yield state
         state.revert(snapshot)
```

### Comparing `py-evm-0.7.0a1/eth/vm/chain_context.py` & `py-evm-0.7.0a2/eth/vm/chain_context.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from typing import Optional
+from typing import (
+    Optional,
+)
 
-from eth.abc import ChainContextAPI
+from eth.abc import (
+    ChainContextAPI,
+)
 from eth.validation import (
     validate_uint256,
 )
 
 
 class ChainContext(ChainContextAPI):
-    __slots__ = ['_chain_id']
+    __slots__ = ["_chain_id"]
 
     def __init__(self, chain_id: Optional[int]) -> None:
-
         if chain_id is None:
             chain_id = 0  # Default value (invalid for public networks)
         # Due to EIP-155's definition of Chain ID,
         # the number that needs to be RLP encoded is `CHAINID * 2 + 36`
         validate_uint256(chain_id)
         self._chain_id = chain_id
```

### Comparing `py-evm-0.7.0a1/eth/vm/code_stream.py` & `py-evm-0.7.0a2/eth/vm/code_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 import contextlib
 import logging
 from typing import (
     Iterator,
-    Set
+    Set,
 )
 
-from eth.abc import CodeStreamAPI
+from eth.abc import (
+    CodeStreamAPI,
+)
 from eth.validation import (
     validate_is_bytes,
 )
 from eth.vm.opcode_values import (
     PUSH1,
     PUSH32,
     STOP,
 )
 
 
 class CodeStream(CodeStreamAPI):
-    __slots__ = ['_length_cache', '_raw_code_bytes', 'invalid_positions', 'valid_positions', 'pc']
+    __slots__ = [
+        "_length_cache",
+        "_raw_code_bytes",
+        "invalid_positions",
+        "valid_positions",
+        "pc",
+    ]
 
-    logger = logging.getLogger('eth.vm.CodeStream')
+    logger = logging.getLogger("eth.vm.CodeStream")
 
     def __init__(self, code_bytes: bytes) -> None:
         validate_is_bytes(code_bytes, title="CodeStream bytes")
-        # in order to avoid method overhead when setting/accessing pc, we no longer fence
-        # the pc (Program Counter) into 0 <= pc <= len(code_bytes). We now let it float free.
+        # in order to avoid method overhead when setting/accessing pc, we no longer
+        # fence the pc (Program Counter) into 0 <= pc <= len(code_bytes).
+        # We now let it float free.
         # NOTE: Setting pc to a negative value has undefined behavior.
         self.program_counter = 0
         self._raw_code_bytes = code_bytes
         self._length_cache = len(code_bytes)
         self.invalid_positions: Set[int] = set()
         self.valid_positions: Set[int] = set()
 
@@ -60,23 +69,25 @@
         pc = self.program_counter
         if pc < self._length_cache:
             return self._raw_code_bytes[pc]
         else:
             return STOP
 
     @contextlib.contextmanager
-    def seek(self, program_counter: int) -> Iterator['CodeStream']:
+    def seek(self, program_counter: int) -> Iterator["CodeStream"]:
         anchor_pc = self.program_counter
         self.program_counter = program_counter
         try:
             yield self
         finally:
             self.program_counter = anchor_pc
 
-    def _potentially_disqualifying_opcode_positions(self, position: int) -> Iterator[int]:
+    def _potentially_disqualifying_opcode_positions(
+        self, position: int
+    ) -> Iterator[int]:
         # Look at the last 32 positions (from 1 byte back to 32 bytes back).
         # Don't attempt to look at negative positions.
         deepest_lookback = min(32, position)
         # iterate in reverse, because PUSH32 is more common than others
         for bytes_back in range(deepest_lookback, 0, -1):
             earlier_position = position - bytes_back
             opcode = self._raw_code_bytes[earlier_position]
@@ -90,20 +101,25 @@
             return False
         elif position in self.invalid_positions:
             return False
         elif position in self.valid_positions:
             return True
         else:
             # An opcode is not valid, iff it is the "data" following a PUSH_
-            # So we look at the previous 32 bytes (PUSH32 being the largest) to see if there
-            # is a PUSH_ before the opcode in this position.
-            for disqualifier in self._potentially_disqualifying_opcode_positions(position):
-                # Now that we found a PUSH_ before this position, we check if *that* PUSH is valid
+            # So we look at the previous 32 bytes (PUSH32 being the largest) to see if
+            # there is a PUSH_ before the opcode in this position.
+            for disqualifier in self._potentially_disqualifying_opcode_positions(
+                position
+            ):
+                # Now that we found a PUSH_ before this position,
+                # we check if *that* PUSH is valid
                 if self.is_valid_opcode(disqualifier):
                     # If the PUSH_ valid, then the current position is invalid
                     self.invalid_positions.add(position)
                     return False
-                # Otherwise, keep looking for other potentially disqualifying PUSH_ codes
+                # Otherwise, keep looking for other potentially
+                # disqualifying PUSH_ codes
 
-            # We didn't find any valid PUSH_ opcodes in the 32 bytes before position; it's valid
+            # We didn't find any valid PUSH_ opcodes in the 32 bytes
+            # before position; it's valid
             self.valid_positions.add(position)
             return True
```

### Comparing `py-evm-0.7.0a1/eth/vm/computation.py` & `py-evm-0.7.0a2/eth/vm/computation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 import itertools
-from types import TracebackType
+from types import (
+    TracebackType,
+)
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Tuple,
     Type,
     Union,
     cast,
 )
 
-from cached_property import cached_property
+from cached_property import (
+    cached_property,
+)
 from eth_typing import (
     Address,
 )
 from eth_utils import (
     encode_hex,
     get_extended_debug_logger,
 )
 
+from eth._utils.datatypes import (
+    Configurable,
+)
+from eth._utils.numeric import (
+    ceil32,
+)
 from eth.abc import (
-    MemoryAPI,
-    StackAPI,
+    CodeStreamAPI,
+    ComputationAPI,
     GasMeterAPI,
+    MemoryAPI,
     MessageAPI,
     OpcodeAPI,
-    CodeStreamAPI,
-    ComputationAPI,
+    StackAPI,
     StateAPI,
     TransactionContextAPI,
 )
 from eth.constants import (
     GAS_MEMORY,
     GAS_MEMORY_QUADRATIC_DENOMINATOR,
 )
 from eth.exceptions import (
     Halt,
     VMError,
 )
 from eth.typing import (
     BytesOrView,
 )
-from eth._utils.datatypes import (
-    Configurable,
-)
-from eth._utils.numeric import (
-    ceil32,
-)
 from eth.validation import (
     validate_canonical_address,
     validate_is_bytes,
     validate_uint256,
 )
 from eth.vm.code_stream import (
     CodeStream,
@@ -81,89 +85,291 @@
     """
     raise Exception("This method is never intended to be executed")
 
 
 def memory_gas_cost(size_in_bytes: int) -> int:
     size_in_words = ceil32(size_in_bytes) // 32
     linear_cost = size_in_words * GAS_MEMORY
-    quadratic_cost = size_in_words ** 2 // GAS_MEMORY_QUADRATIC_DENOMINATOR
+    quadratic_cost = size_in_words**2 // GAS_MEMORY_QUADRATIC_DENOMINATOR
 
     total_cost = linear_cost + quadratic_cost
     return total_cost
 
 
-class BaseComputation(Configurable, ComputationAPI):
+class BaseComputation(ComputationAPI, Configurable):
     """
     The base class for all execution computations.
 
       .. note::
 
         Each :class:`~eth.vm.computation.BaseComputation` class must be configured with:
 
-        ``opcodes``: A mapping from the opcode integer value to the logic function for the opcode.
+        ``opcodes``:        A mapping from the opcode integer value to the logic
+                            function for the opcode.
 
-        ``_precompiles``: A mapping of contract address to the precompile function for execution
-        of precompiled contracts.
+        ``_precompiles``:   A mapping of contract address to the precompile function
+                            for execution of precompiled contracts.
     """
+
+    logger = get_extended_debug_logger("eth.vm.computation.BaseComputation")
+
     state: StateAPI = None
     msg: MessageAPI = None
     transaction_context: TransactionContextAPI = None
+    code: CodeStreamAPI = None
+    children: List[ComputationAPI] = None
+    return_data: bytes = b""
+    accounts_to_delete: Dict[Address, Address] = None
 
     _memory: MemoryAPI = None
     _stack: StackAPI = None
     _gas_meter: GasMeterAPI = None
-
-    code: CodeStreamAPI = None
-
-    children: List[ComputationAPI] = None
-
-    _output: bytes = b''
-    return_data: bytes = b''
     _error: VMError = None
-
-    # TODO: use a NamedTuple for log entries
+    _output: bytes = b""
     _log_entries: List[Tuple[int, Address, Tuple[int, ...], bytes]] = None
-    accounts_to_delete: Dict[Address, Address] = None
 
     # VM configuration
     opcodes: Dict[int, OpcodeAPI] = None
     _precompiles: Dict[Address, Callable[[ComputationAPI], ComputationAPI]] = None
 
-    logger = get_extended_debug_logger('eth.vm.computation.Computation')
-
-    def __init__(self,
-                 state: StateAPI,
-                 message: MessageAPI,
-                 transaction_context: TransactionContextAPI) -> None:
-
+    def __init__(
+        self,
+        state: StateAPI,
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI,
+    ) -> None:
         self.state = state
         self.msg = message
         self.transaction_context = transaction_context
+        self.code = CodeStream(message.code)
 
-        self._memory = Memory()
-        self._stack = Stack()
-        self._gas_meter = self.get_gas_meter()
+        self._gas_meter = self._configure_gas_meter()
 
         self.children = []
         self.accounts_to_delete = {}
+        self._stack = Stack()
+        self._memory = Memory()
         self._log_entries = []
 
-        code = message.code
-        self.code = CodeStream(code)
+    def _configure_gas_meter(self) -> GasMeter:
+        return GasMeter(self.msg.gas)
+
+    # -- class methods -- #
+    @classmethod
+    def apply_message(
+        cls,
+        state: StateAPI,
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI,
+    ) -> ComputationAPI:
+        raise NotImplementedError("Must be implemented by subclasses")
+
+    @classmethod
+    def apply_create_message(
+        cls,
+        state: StateAPI,
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI,
+    ) -> ComputationAPI:
+        raise NotImplementedError("Must be implemented by subclasses")
 
-    #
-    # Convenience
-    #
+    # -- convenience -- #
     @property
     def is_origin_computation(self) -> bool:
         return self.msg.sender == self.transaction_context.origin
 
-    #
-    # Error handling
-    #
+    # -- runtime operations -- #
+    def prepare_child_message(
+        self,
+        gas: int,
+        to: Address,
+        value: int,
+        data: BytesOrView,
+        code: bytes,
+        **kwargs: Any,
+    ) -> MessageAPI:
+        kwargs.setdefault("sender", self.msg.storage_address)
+
+        child_message = Message(
+            gas=gas,
+            to=to,
+            value=value,
+            data=data,
+            code=code,
+            depth=self.msg.depth + 1,
+            **kwargs,
+        )
+        return child_message
+
+    def apply_child_computation(
+        self,
+        child_msg: MessageAPI,
+    ) -> ComputationAPI:
+        child_computation = self.generate_child_computation(child_msg)
+        self.add_child_computation(child_computation)
+        return child_computation
+
+    def generate_child_computation(
+        self,
+        child_msg: MessageAPI,
+    ) -> ComputationAPI:
+        if child_msg.is_create:
+            child_computation = self.apply_create_message(
+                self.state,
+                child_msg,
+                self.transaction_context,
+            )
+        else:
+            child_computation = self.apply_message(
+                self.state,
+                child_msg,
+                self.transaction_context,
+            )
+        return child_computation
+
+    def add_child_computation(
+        self,
+        child_computation: ComputationAPI,
+    ) -> None:
+        if child_computation.is_error:
+            if child_computation.msg.is_create:
+                self.return_data = child_computation.output
+            elif child_computation.should_burn_gas:
+                self.return_data = b""
+            else:
+                self.return_data = child_computation.output
+        else:
+            if child_computation.msg.is_create:
+                self.return_data = b""
+            else:
+                self.return_data = child_computation.output
+        self.children.append(child_computation)
+
+    # -- gas consumption -- #
+    def get_gas_refund(self) -> int:
+        if self.is_error:
+            return 0
+        else:
+            return self._gas_meter.gas_refunded + sum(
+                c.get_gas_refund() for c in self.children
+            )
+
+    # -- account management -- #
+    def register_account_for_deletion(self, beneficiary: Address) -> None:
+        # SELFDESTRUCT
+
+        validate_canonical_address(
+            beneficiary,
+            title="Self destruct beneficiary address",
+        )
+
+        if self.msg.storage_address in self.accounts_to_delete:
+            raise ValueError(
+                "Invariant.  Should be impossible for an account to be "
+                "registered for deletion multiple times"
+            )
+        self.accounts_to_delete[self.msg.storage_address] = beneficiary
+
+    def get_accounts_for_deletion(self) -> Tuple[Tuple[Address, Address], ...]:
+        # SELFDESTRUCT
+
+        if self.is_error:
+            return ()
+        else:
+            return tuple(
+                dict(
+                    itertools.chain(
+                        self.accounts_to_delete.items(),
+                        *(child.get_accounts_for_deletion() for child in self.children),
+                    )
+                ).items()
+            )
+
+    # -- EVM logging -- #
+    def add_log_entry(
+        self,
+        account: Address,
+        topics: Tuple[int, ...],
+        data: bytes,
+    ) -> None:
+        validate_canonical_address(account, title="Log entry address")
+        for topic in topics:
+            validate_uint256(topic, title="Log entry topic")
+        validate_is_bytes(data, title="Log entry data")
+        self._log_entries.append(
+            (self.transaction_context.get_next_log_counter(), account, topics, data)
+        )
+
+    def get_raw_log_entries(
+        self,
+    ) -> Tuple[Tuple[int, bytes, Tuple[int, ...], bytes], ...]:
+        if self.is_error:
+            return ()
+        else:
+            return tuple(
+                sorted(
+                    itertools.chain(
+                        self._log_entries,
+                        *(child.get_raw_log_entries() for child in self.children),
+                    )
+                )
+            )
+
+    def get_log_entries(self) -> Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...]:
+        return tuple(log[1:] for log in self.get_raw_log_entries())
+
+    # -- state transition -- #
+    @classmethod
+    def apply_computation(
+        cls,
+        state: StateAPI,
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI,
+    ) -> ComputationAPI:
+        with cls(state, message, transaction_context) as computation:
+            if message.is_create and computation.is_origin_computation:
+                # If computation is from a create transaction, consume initcode gas if
+                # >= Shanghai. CREATE and CREATE2 are handled in the opcode
+                # implementations.
+                cls.consume_initcode_gas_cost(computation)
+
+            # Early exit on pre-compiles
+            precompile = computation.precompiles.get(message.code_address, NO_RESULT)
+            if precompile is not NO_RESULT:
+                precompile(computation)
+                return computation
+
+            show_debug2 = computation.logger.show_debug2
+
+            opcode_lookup = computation.opcodes
+            for opcode in computation.code:
+                try:
+                    opcode_fn = opcode_lookup[opcode]
+                except KeyError:
+                    opcode_fn = InvalidOpcode(opcode)
+
+                if show_debug2:
+                    # We dig into some internals for debug logs
+                    base_comp = cast(BaseComputation, computation)
+                    computation.logger.debug2(
+                        "OPCODE: 0x%x (%s) | pc: %s | stack: %s",
+                        opcode,
+                        opcode_fn.mnemonic,
+                        max(0, computation.code.program_counter - 1),
+                        base_comp._stack,
+                    )
+
+                try:
+                    opcode_fn(computation=computation)
+                except Halt:
+                    break
+
+        return computation
+
+    # -- error handling -- #
     @property
     def is_success(self) -> bool:
         return self._error is None
 
     @property
     def is_error(self) -> bool:
         return not self.is_success
@@ -192,17 +398,15 @@
     def should_return_gas(self) -> bool:
         return not self.should_burn_gas
 
     @property
     def should_erase_return_data(self) -> bool:
         return self.is_error and self._error.erases_return_data
 
-    #
-    # Memory Management
-    #
+    # -- memory management -- #
     def extend_memory(self, start_position: int, size: int) -> None:
         validate_uint256(start_position, title="Memory start position")
         validate_uint256(size, title="Memory size")
 
         before_size = ceil32(len(self._memory))
         after_size = ceil32(start_position + size)
 
@@ -219,61 +423,55 @@
             )
 
         if size:
             if before_cost < after_cost:
                 gas_fee = after_cost - before_cost
                 self._gas_meter.consume_gas(
                     gas_fee,
-                    reason=" ".join((
-                        "Expanding memory",
-                        str(before_size),
-                        "->",
-                        str(after_size),
-                    ))
+                    reason=" ".join(
+                        (
+                            "Expanding memory",
+                            str(before_size),
+                            "->",
+                            str(after_size),
+                        )
+                    ),
                 )
 
             self._memory.extend(start_position, size)
 
     def memory_write(self, start_position: int, size: int, value: bytes) -> None:
         return self._memory.write(start_position, size, value)
 
     def memory_read(self, start_position: int, size: int) -> memoryview:
         return self._memory.read(start_position, size)
 
     def memory_read_bytes(self, start_position: int, size: int) -> bytes:
         return self._memory.read_bytes(start_position, size)
 
-    #
-    # Gas Consumption
-    #
+    # -- gas consumption -- #
     def get_gas_meter(self) -> GasMeterAPI:
-        return GasMeter(self.msg.gas)
+        return self._gas_meter
 
     def consume_gas(self, amount: int, reason: str) -> None:
         return self._gas_meter.consume_gas(amount, reason)
 
     def return_gas(self, amount: int) -> None:
         return self._gas_meter.return_gas(amount)
 
     def refund_gas(self, amount: int) -> None:
         return self._gas_meter.refund_gas(amount)
 
-    def get_gas_refund(self) -> int:
-        if self.is_error:
-            return 0
-        else:
-            return self._gas_meter.gas_refunded + sum(c.get_gas_refund() for c in self.children)
-
     def get_gas_used(self) -> int:
         if self.should_burn_gas:
-            return self.msg.gas
+            return self._gas_meter.start_gas
         else:
             return max(
                 0,
-                self.msg.gas - self._gas_meter.gas_remaining,
+                self._gas_meter.start_gas - self._gas_meter.gas_remaining,
             )
 
     def get_gas_remaining(self) -> int:
         if self.should_burn_gas:
             return 0
         else:
             return self._gas_meter.gas_remaining
@@ -282,17 +480,15 @@
     def consume_initcode_gas_cost(cls, computation: ComputationAPI) -> None:
         # this method does not become relevant until the Shanghai hard fork
         """
         Before starting the computation, consume initcode gas cost.
         """
         pass
 
-    #
-    # Stack management
-    #
+    # -- stack management -- #
     def stack_swap(self, position: int) -> None:
         return self._stack.swap(position)
 
     def stack_dup(self, position: int) -> None:
         return self._stack.dup(position)
 
     # Stack manipulation is performance-sensitive code.
@@ -326,270 +522,117 @@
     def stack_push_int(self) -> Callable[[int], None]:
         return self._stack.push_int
 
     @cached_property
     def stack_push_bytes(self) -> Callable[[bytes], None]:
         return self._stack.push_bytes
 
-    #
-    # Computation result
-    #
+    # -- computation result -- #
     @property
     def output(self) -> bytes:
         if self.should_erase_return_data:
-            return b''
+            return b""
         else:
             return self._output
 
     @output.setter
     def output(self, value: bytes) -> None:
         validate_is_bytes(value)
         self._output = value
 
-    #
-    # Runtime operations
-    #
-    def prepare_child_message(self,
-                              gas: int,
-                              to: Address,
-                              value: int,
-                              data: BytesOrView,
-                              code: bytes,
-                              **kwargs: Any) -> MessageAPI:
-        kwargs.setdefault('sender', self.msg.storage_address)
-
-        child_message = Message(
-            gas=gas,
-            to=to,
-            value=value,
-            data=data,
-            code=code,
-            depth=self.msg.depth + 1,
-            **kwargs
-        )
-        return child_message
-
-    def apply_child_computation(self, child_msg: MessageAPI) -> ComputationAPI:
-        child_computation = self.generate_child_computation(child_msg)
-        self.add_child_computation(child_computation)
-        return child_computation
-
-    def generate_child_computation(self, child_msg: MessageAPI) -> ComputationAPI:
-        if child_msg.is_create:
-            child_computation = self.apply_create_message(
-                self.state,
-                child_msg,
-                self.transaction_context,
-            )
-        else:
-            child_computation = self.apply_message(
-                self.state,
-                child_msg,
-                self.transaction_context,
-            )
-        return child_computation
-
-    def add_child_computation(self, child_computation: ComputationAPI) -> None:
-        if child_computation.is_error:
-            if child_computation.msg.is_create:
-                self.return_data = child_computation.output
-            elif child_computation.should_burn_gas:
-                self.return_data = b''
-            else:
-                self.return_data = child_computation.output
-        else:
-            if child_computation.msg.is_create:
-                self.return_data = b''
-            else:
-                self.return_data = child_computation.output
-        self.children.append(child_computation)
-
-    #
-    # Account management
-    #
-    def register_account_for_deletion(self, beneficiary: Address) -> None:
-        validate_canonical_address(beneficiary, title="Self destruct beneficiary address")
-
-        if self.msg.storage_address in self.accounts_to_delete:
-            raise ValueError(
-                "Invariant.  Should be impossible for an account to be "
-                "registered for deletion multiple times"
-            )
-        self.accounts_to_delete[self.msg.storage_address] = beneficiary
-
-    def get_accounts_for_deletion(self) -> Tuple[Tuple[Address, Address], ...]:
-        if self.is_error:
-            return ()
+    # -- opcode API -- #
+    @property
+    def precompiles(self) -> Dict[Address, Callable[[ComputationAPI], Any]]:
+        if self._precompiles is None:
+            return {}
         else:
-            return tuple(dict(itertools.chain(
-                self.accounts_to_delete.items(),
-                *(child.get_accounts_for_deletion() for child in self.children)
-            )).items())
-
-    #
-    # EVM logging
-    #
-    def add_log_entry(self, account: Address, topics: Tuple[int, ...], data: bytes) -> None:
-        validate_canonical_address(account, title="Log entry address")
-        for topic in topics:
-            validate_uint256(topic, title="Log entry topic")
-        validate_is_bytes(data, title="Log entry data")
-        self._log_entries.append(
-            (self.transaction_context.get_next_log_counter(), account, topics, data))
+            return self._precompiles
 
-    def get_raw_log_entries(self) -> Tuple[Tuple[int, bytes, Tuple[int, ...], bytes], ...]:
-        if self.is_error:
-            return ()
+    @classmethod
+    def get_precompiles(cls) -> Dict[Address, Callable[[ComputationAPI], Any]]:
+        if cls._precompiles is None:
+            return {}
         else:
-            return tuple(sorted(itertools.chain(
-                self._log_entries,
-                *(child.get_raw_log_entries() for child in self.children)
-            )))
+            return cls._precompiles
 
-    def get_log_entries(self) -> Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...]:
-        return tuple(log[1:] for log in self.get_raw_log_entries())
+    def get_opcode_fn(self, opcode: int) -> OpcodeAPI:
+        try:
+            return self.opcodes[opcode]
+        except KeyError:
+            return InvalidOpcode(opcode)
 
-    #
-    # Context Manager API
-    #
+    # -- context manager API -- #
     def __enter__(self) -> ComputationAPI:
         if self.logger.show_debug2:
             self.logger.debug2(
                 (
-                    "COMPUTATION STARTING: gas: %s | from: %s | to: %s | value: %s "
-                    "| depth %s | static: %s"
+                    "MESSAGE COMPUTATION STARTING: "
+                    "from: %s | to: %s | value: %s | depth %s | static: %s | gas: %s"
                 ),
-                self.msg.gas,
                 encode_hex(self.msg.sender),
                 encode_hex(self.msg.to),
                 self.msg.value,
                 self.msg.depth,
                 "y" if self.msg.is_static else "n",
+                self.msg.gas,
             )
-
         return self
 
-    def __exit__(self,
-                 exc_type: Optional[Type[BaseException]],
-                 exc_value: Optional[BaseException],
-                 traceback: Optional[TracebackType]) -> Union[None, bool]:
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_value: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> Union[None, bool]:
         if exc_value and isinstance(exc_value, VMError):
             if self.logger.show_debug2:
                 self.logger.debug2(
                     (
-                        "COMPUTATION ERROR: gas: %s | from: %s | to: %s | value: %s | "
+                        "COMPUTATION ERROR: "
+                        "gas: %s | from: %s | to: %s | value: %s | "
                         "depth: %s | static: %s | error: %s"
                     ),
                     self.msg.gas,
                     encode_hex(self.msg.sender),
                     encode_hex(self.msg.to),
                     self.msg.value,
                     self.msg.depth,
                     "y" if self.msg.is_static else "n",
                     exc_value,
                 )
+
             self._error = exc_value
             if self.should_burn_gas:
                 self.consume_gas(
                     self._gas_meter.gas_remaining,
-                    reason=" ".join((
-                        "Zeroing gas due to VM Exception:",
-                        str(exc_value),
-                    )),
+                    reason=" ".join(
+                        (
+                            "Zeroing gas due to VM Exception:",
+                            str(exc_value),
+                        )
+                    ),
                 )
 
-            # When we raise an exception that erases return data, erase the return data.
+            # when we raise an exception that erases return data, erase the return data
             if self.should_erase_return_data:
-                self.return_data = b''
+                self.return_data = b""
 
             # suppress VM exceptions
             return True
+
         elif exc_type is None and self.logger.show_debug2:
             self.logger.debug2(
                 (
-                    "COMPUTATION SUCCESS: from: %s | to: %s | value: %s | "
-                    "depth: %s | static: %s | gas-used: %s | gas-remaining: %s"
+                    "COMPUTATION SUCCESS: "
+                    "from: %s | to: %s | value: %s | depth: %s | static: %s "
+                    "| gas-used: %s | gas-remaining: %s"
                 ),
                 encode_hex(self.msg.sender),
                 encode_hex(self.msg.to),
                 self.msg.value,
                 self.msg.depth,
                 "y" if self.msg.is_static else "n",
                 self.get_gas_used(),
                 self._gas_meter.gas_remaining,
             )
 
         return None
-
-    #
-    # State Transition
-    #
-    @classmethod
-    def apply_computation(
-        cls,
-        state: StateAPI,
-        message: MessageAPI,
-        transaction_context: TransactionContextAPI
-    ) -> ComputationAPI:
-
-        with cls(state, message, transaction_context) as computation:
-            if message.is_create and computation.is_origin_computation:
-                # If computation is from a create transaction, consume initcode gas if
-                # >= Shanghai. CREATE and CREATE2 are handled in the opcode
-                # implementations.
-                cls.consume_initcode_gas_cost(computation)
-
-            # Early exit on pre-compiles
-            precompile = computation.precompiles.get(message.code_address, NO_RESULT)
-            if precompile is not NO_RESULT:
-                precompile(computation)
-                return computation
-
-            show_debug2 = computation.logger.show_debug2
-
-            opcode_lookup = computation.opcodes
-            for opcode in computation.code:
-                try:
-                    opcode_fn = opcode_lookup[opcode]
-                except KeyError:
-                    opcode_fn = InvalidOpcode(opcode)
-
-                if show_debug2:
-                    # We dig into some internals for debug logs
-                    base_comp = cast(BaseComputation, computation)
-                    computation.logger.debug2(
-                        "OPCODE: 0x%x (%s) | pc: %s | stack: %s",
-                        opcode,
-                        opcode_fn.mnemonic,
-                        max(0, computation.code.program_counter - 1),
-                        base_comp._stack,
-                    )
-
-                try:
-                    opcode_fn(computation=computation)
-                except Halt:
-                    break
-
-        return computation
-
-    #
-    # Opcode API
-    #
-    @property
-    def precompiles(self) -> Dict[Address, Callable[[ComputationAPI], Any]]:
-        if self._precompiles is None:
-            return {}
-        else:
-            return self._precompiles
-
-    @classmethod
-    def get_precompiles(cls) -> Dict[Address, Callable[[ComputationAPI], Any]]:
-        if cls._precompiles is None:
-            return {}
-        else:
-            return cls._precompiles
-
-    def get_opcode_fn(self, opcode: int) -> OpcodeAPI:
-        try:
-            return self.opcodes[opcode]
-        except KeyError:
-            return InvalidOpcode(opcode)
```

### Comparing `py-evm-0.7.0a1/eth/vm/execution_context.py` & `py-evm-0.7.0a2/eth/vm/execution_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 
 from eth_typing import (
     Address,
     BlockNumber,
     Hash32,
 )
 
-from eth.abc import ExecutionContextAPI
-from eth._utils.generator import CachedIterable
+from eth._utils.generator import (
+    CachedIterable,
+)
+from eth.abc import (
+    ExecutionContextAPI,
+)
 
 
 class ExecutionContext(ExecutionContextAPI):
     _coinbase = None
     _timestamp = None
     _number = None
     _difficulty = None
@@ -30,15 +34,15 @@
         timestamp: int,
         block_number: BlockNumber,
         difficulty: int,
         mix_hash: Hash32,
         gas_limit: int,
         prev_hashes: Iterable[Hash32],
         chain_id: int,
-        base_fee_per_gas: Optional[int] = None
+        base_fee_per_gas: Optional[int] = None,
     ) -> None:
         self._coinbase = coinbase
         self._timestamp = timestamp
         self._block_number = block_number
         self._difficulty = difficulty
         self._mix_hash = mix_hash
         self._gas_limit = gas_limit
@@ -78,11 +82,12 @@
     def chain_id(self) -> int:
         return self._chain_id
 
     @property
     def base_fee_per_gas(self) -> int:
         if self._base_fee_per_gas is None:
             raise AttributeError(
-                f"This header at Block #{self.block_number} does not have a base gas fee"
+                f"This header at Block #{self.block_number} "
+                "does not have a base gas fee"
             )
         else:
             return self._base_fee_per_gas
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 )
 from .state import ArrowGlacierState
 from .. import LondonVM
 
 
 class ArrowGlacierVM(LondonVM):
     # fork name
-    fork = 'arrow-glacier'
+    fork = "arrow-glacier"
 
     # classes
     block_class: Type[BaseBlock] = ArrowGlacierBlock
     _state_class: Type[BaseState] = ArrowGlacierState
 
     # Methods
     create_header_from_parent = staticmethod(  # type: ignore
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/blocks.py` & `py-evm-0.7.0a2/eth/vm/forks/gray_glacier/blocks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-from abc import ABC
-from typing import Type
+from abc import (
+    ABC,
+)
+from typing import (
+    Type,
+)
 
-from eth.abc import TransactionBuilderAPI
 from eth_utils import (
     encode_hex,
 )
-
 from rlp.sedes import (
     CountableList,
 )
 
-from .transactions import (
-    ArrowGlacierTransactionBuilder,
+from eth.abc import (
+    TransactionBuilderAPI,
 )
-from ..london import (
-    LondonBlock,
+
+from ..arrow_glacier import (
+    ArrowGlacierBlock,
+)
+from ..arrow_glacier.blocks import (
+    ArrowGlacierBlockHeader,
+    ArrowGlacierMiningHeader,
 )
 from ..london.blocks import (
     LondonBackwardsHeader,
-    LondonBlockHeader,
-    LondonMiningHeader,
+)
+from .transactions import (
+    GrayGlacierTransactionBuilder,
 )
 
 
-class ArrowGlacierMiningHeader(LondonMiningHeader, ABC):
+class GrayGlacierMiningHeader(ArrowGlacierMiningHeader, ABC):
     pass
 
 
-class ArrowGlacierBlockHeader(LondonBlockHeader, ABC):
+class GrayGlacierBlockHeader(ArrowGlacierBlockHeader, ABC):
     def __str__(self) -> str:
-        return f'<ArrowGlacierBlockHeader #{self.block_number} {encode_hex(self.hash)[2:10]}>'
+        return f"<GrayGlacierBlockHeader #{self.block_number} {encode_hex(self.hash)[2:10]}>"  # noqa: E501
 
 
-class ArrowGlacierBlock(LondonBlock):
-    transaction_builder: Type[TransactionBuilderAPI] = ArrowGlacierTransactionBuilder
+class GrayGlacierBlock(ArrowGlacierBlock):
+    transaction_builder: Type[TransactionBuilderAPI] = GrayGlacierTransactionBuilder
     fields = [
-        ('header', ArrowGlacierBlockHeader),
-        ('transactions', CountableList(transaction_builder)),
-        ('uncles', CountableList(LondonBackwardsHeader))
+        ("header", GrayGlacierBlockHeader),
+        ("transactions", CountableList(transaction_builder)),
+        ("uncles", CountableList(LondonBackwardsHeader)),
     ]
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/headers.py` & `py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/headers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,43 @@
-from typing import Any, Callable, Optional
-
-from toolz import curry
+from typing import (
+    Any,
+    Callable,
+    Optional,
+)
 
-from eth.abc import BlockHeaderAPI
-from .blocks import (
-    ArrowGlacierBlockHeader,
+from toolz import (
+    curry,
 )
-from eth.vm.forks.london.headers import (
-    create_london_header_from_parent,
+
+from eth.abc import (
+    BlockHeaderAPI,
 )
 from eth.vm.forks.byzantium.headers import (
     compute_difficulty,
-)
-from eth.vm.forks.byzantium.headers import (
     configure_header,
 )
+from eth.vm.forks.london.headers import (
+    create_london_header_from_parent,
+)
+
+from .blocks import (
+    ArrowGlacierBlockHeader,
+)
 
 compute_arrow_glacier_difficulty = compute_difficulty(10_700_000)
-configure_arrow_glacier_header = configure_header(difficulty_fn=compute_arrow_glacier_difficulty)
+configure_arrow_glacier_header = configure_header(
+    difficulty_fn=compute_arrow_glacier_difficulty
+)
 
 
 @curry
 def create_arrow_glacier_header_from_parent(
     difficulty_fn: Callable[[BlockHeaderAPI, int], int],
     parent_header: Optional[BlockHeaderAPI],
-    **header_params: Any
+    **header_params: Any,
 ) -> BlockHeaderAPI:
     london_validated_header = create_london_header_from_parent(
         difficulty_fn, parent_header, **header_params
     )
 
     # extract header params validated up to london (previous VM) and plug
     # into `ArrowGlacierBlockHeader` class
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/transactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-from abc import ABC
+from abc import (
+    ABC,
+)
 
-from eth_keys.datatypes import PrivateKey
+from eth_keys.datatypes import (
+    PrivateKey,
+)
 
 from eth._utils.transactions import (
     create_transaction_signature,
 )
 from eth.vm.forks.london.transactions import (
     LondonLegacyTransaction,
     LondonTransactionBuilder,
@@ -14,17 +18,15 @@
 
 class ArrowGlacierLegacyTransaction(LondonLegacyTransaction, ABC):
     pass
 
 
 class ArrowGlacierUnsignedLegacyTransaction(LondonUnsignedLegacyTransaction):
     def as_signed_transaction(
-        self,
-        private_key: PrivateKey,
-        chain_id: int = None
+        self, private_key: PrivateKey, chain_id: int = None
     ) -> ArrowGlacierLegacyTransaction:
         v, r, s = create_transaction_signature(self, private_key, chain_id=chain_id)
         return ArrowGlacierLegacyTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/berlin/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/berlin/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     create_berlin_header_from_parent,
 )
 from .state import BerlinState
 
 
 class BerlinVM(MuirGlacierVM):
     # fork name
-    fork = 'berlin'
+    fork = "berlin"
 
     # classes
     block_class: Type[BaseBlock] = BerlinBlock
     _state_class: Type[BaseState] = BerlinState
 
     # Methods
-    create_header_from_parent = staticmethod(create_berlin_header_from_parent)  # type: ignore
-    compute_difficulty = staticmethod(compute_berlin_difficulty)    # type: ignore
+    create_header_from_parent = staticmethod(create_berlin_header_from_parent)  # type: ignore  # noqa: E501
+    compute_difficulty = staticmethod(compute_berlin_difficulty)  # type: ignore
     configure_header = configure_berlin_header
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/berlin/blocks.py` & `py-evm-0.7.0a2/eth/vm/forks/berlin/blocks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Type
+from typing import (
+    Type,
+)
 
 from rlp.sedes import (
     CountableList,
 )
 
 from eth.abc import (
     ReceiptBuilderAPI,
@@ -20,14 +22,14 @@
 )
 from .transactions import (
     BerlinTransactionBuilder,
 )
 
 
 class BerlinBlock(MuirGlacierBlock):
-    transaction_builder: Type[TransactionBuilderAPI] = BerlinTransactionBuilder  # type: ignore
+    transaction_builder: Type[TransactionBuilderAPI] = BerlinTransactionBuilder  # type: ignore  # noqa: E501
     receipt_builder: Type[ReceiptBuilderAPI] = BerlinReceiptBuilder  # type: ignore
     fields = [
-        ('header', BlockHeader),
-        ('transactions', CountableList(transaction_builder)),
-        ('uncles', CountableList(BlockHeader))
+        ("header", BlockHeader),
+        ("transactions", CountableList(transaction_builder)),
+        ("uncles", CountableList(BlockHeader)),
     ]
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/berlin/computation.py` & `py-evm-0.7.0a2/eth/vm/forks/berlin/computation.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,47 +3,49 @@
 from eth_utils import (
     big_endian_to_int,
 )
 from eth_utils.toolz import (
     merge,
 )
 
-from eth.precompiles.modexp import (
-    extract_lengths,
-    modexp,
-)
 from eth._utils.address import (
     force_bytes_to_address,
 )
 from eth._utils.numeric import (
     get_highest_bit_index,
 )
 from eth._utils.padding import (
     zpad_right,
 )
-
-from eth.vm.forks.berlin import constants
-
-from eth.vm.forks.muir_glacier.computation import (
-    MUIR_GLACIER_PRECOMPILES
+from eth.precompiles.modexp import (
+    extract_lengths,
+    modexp,
+)
+from eth.vm.forks.berlin import (
+    constants,
 )
 from eth.vm.forks.muir_glacier.computation import (
+    MUIR_GLACIER_PRECOMPILES,
     MuirGlacierComputation,
 )
 
-from .opcodes import BERLIN_OPCODES
+from .opcodes import (
+    BERLIN_OPCODES,
+)
 
 
 def _calculate_multiplication_complexity(base_length: int, modulus_length: int) -> int:
     max_length = max(base_length, modulus_length)
     words = math.ceil(max_length / 8)
     return words**2
 
 
-def _calculate_iteration_count(exponent_length: int, first_32_exponent_bytes: bytes) -> int:
+def _calculate_iteration_count(
+    exponent_length: int, first_32_exponent_bytes: bytes
+) -> int:
     first_32_exponent = big_endian_to_int(first_32_exponent_bytes)
 
     highest_bit_index = get_highest_bit_index(first_32_exponent)
 
     if exponent_length <= 32:
         iteration_count = highest_bit_index
     else:
@@ -63,27 +65,37 @@
         to_size=min(exponent_length, 32),
     )[:32]
     iteration_count = _calculate_iteration_count(
         exponent_length,
         first_32_exponent_bytes,
     )
 
-    multiplication_complexity = _calculate_multiplication_complexity(base_length, modulus_length)
-    return max(200,
-               multiplication_complexity * iteration_count
-               // constants.GAS_MOD_EXP_QUADRATIC_DENOMINATOR_EIP_2565)
+    multiplication_complexity = _calculate_multiplication_complexity(
+        base_length, modulus_length
+    )
+    return max(
+        200,
+        multiplication_complexity
+        * iteration_count
+        // constants.GAS_MOD_EXP_QUADRATIC_DENOMINATOR_EIP_2565,
+    )
 
 
 BERLIN_PRECOMPILES = merge(
     MUIR_GLACIER_PRECOMPILES,
-    {force_bytes_to_address(b'\x05'): modexp(gas_calculator=_compute_modexp_gas_fee_eip_2565)},
+    {
+        force_bytes_to_address(b"\x05"): modexp(
+            gas_calculator=_compute_modexp_gas_fee_eip_2565
+        )
+    },
 )
 
 
 class BerlinComputation(MuirGlacierComputation):
     """
-    A class for all execution computations in the ``Berlin`` fork.
+    A class for all execution *message* computations in the ``Berlin`` fork.
     Inherits from :class:`~eth.vm.forks.muir_glacier.MuirGlacierComputation`
     """
+
     # Override
     opcodes = BERLIN_OPCODES
     _precompiles = BERLIN_PRECOMPILES
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/berlin/logic.py` & `py-evm-0.7.0a2/eth/vm/forks/berlin/logic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 from eth_typing import (
     Address,
 )
-from eth_utils.toolz import curry
+from eth_utils.toolz import (
+    curry,
+)
 
-from eth import constants
+from eth import (
+    constants,
+)
 from eth._utils.address import (
     force_bytes_to_address,
 )
 from eth.abc import (
     ComputationAPI,
 )
-from eth.vm import mnemonics
+from eth.vm import (
+    mnemonics,
+)
 from eth.vm.forks.istanbul.storage import (
     GAS_SCHEDULE_EIP2200,
     sstore_eip2200_generic,
 )
 from eth.vm.logic.call import (
     CallByzantium,
     CallCodeEIP150,
     DelegateCallEIP150,
     StaticCall,
 )
 from eth.vm.logic.context import (
     consume_extcodecopy_word_cost,
-    push_balance_of_address,
     extcodecopy_execute,
+    push_balance_of_address,
 )
 from eth.vm.logic.storage import (
     NetSStoreGasSchedule,
 )
 from eth.vm.logic.system import (
     Create2,
     CreateByzantium,
     CreateOpcodeStackData,
     selfdestruct_eip161_on_address,
 )
 
-from . import constants as berlin_constants
+from . import (
+    constants as berlin_constants,
+)
 
 
 def _mark_address_warm(computation: ComputationAPI, address: Address) -> bool:
     """
     Mark the given address as warm if it was not previously.
 
     :return was_cold: True if the account was not previously accessed
@@ -58,17 +66,16 @@
     if was_cold:
         return berlin_constants.COLD_ACCOUNT_ACCESS_COST
     else:
         return berlin_constants.WARM_STORAGE_READ_COST
 
 
 def _consume_gas_for_account_load(
-        computation: ComputationAPI,
-        address: Address,
-        reason: str) -> None:
+    computation: ComputationAPI, address: Address, reason: str
+) -> None:
     was_cold = _mark_address_warm(computation, address)
     gas_cost = _account_load_cost(was_cold)
     computation.consume_gas(gas_cost, reason=reason)
 
 
 def _mark_storage_warm(computation: ComputationAPI, slot: int) -> bool:
     """
@@ -138,29 +145,38 @@
 GAS_SCHEDULE_EIP2929 = GAS_SCHEDULE_EIP2200._replace(
     sload_gas=berlin_constants.WARM_STORAGE_READ_COST,
     sstore_reset_gas=5000 - berlin_constants.COLD_SLOAD_COST,
 )
 
 
 @curry
-def sstore_eip2929_generic(gas_schedule: NetSStoreGasSchedule, computation: ComputationAPI) -> int:
+def sstore_eip2929_generic(
+    gas_schedule: NetSStoreGasSchedule,
+    computation: ComputationAPI,
+) -> int:
     slot = sstore_eip2200_generic(gas_schedule, computation)
 
     if _mark_storage_warm(computation, slot):
         gas_cost = berlin_constants.COLD_SLOAD_COST
-        computation.consume_gas(gas_cost, reason=f"Implicit SLOAD during {mnemonics.SSTORE}")
+        computation.consume_gas(
+            gas_cost, reason=f"Implicit SLOAD during {mnemonics.SSTORE}"
+        )
 
     return slot
 
 
 sstore_eip2929 = sstore_eip2929_generic(GAS_SCHEDULE_EIP2929)
 
 
 class LoadFeeByCacheWarmth:
-    def get_account_load_fee(self, computation: ComputationAPI, code_address: Address) -> int:
+    def get_account_load_fee(
+        self,
+        computation: ComputationAPI,
+        code_address: Address,
+    ) -> int:
         was_cold = _mark_address_warm(computation, code_address)
         return _account_load_cost(was_cold)
 
 
 class CallEIP2929(LoadFeeByCacheWarmth, CallByzantium):
     pass
 
@@ -187,24 +203,28 @@
             reason=f"Implicit account load during {mnemonics.SELFDESTRUCT}",
         )
 
     selfdestruct_eip161_on_address(computation, beneficiary)
 
 
 class CreateEIP2929(CreateByzantium):
-    def generate_contract_address(self,
-                                  stack_data: CreateOpcodeStackData,
-                                  call_data: bytes,
-                                  computation: ComputationAPI) -> Address:
+    def generate_contract_address(
+        self,
+        stack_data: CreateOpcodeStackData,
+        call_data: bytes,
+        computation: ComputationAPI,
+    ) -> Address:
         address = super().generate_contract_address(stack_data, call_data, computation)
         computation.state.mark_address_warm(address)
         return address
 
 
 class Create2EIP2929(Create2):
-    def generate_contract_address(self,
-                                  stack_data: CreateOpcodeStackData,
-                                  call_data: bytes,
-                                  computation: ComputationAPI) -> Address:
+    def generate_contract_address(
+        self,
+        stack_data: CreateOpcodeStackData,
+        call_data: bytes,
+        computation: ComputationAPI,
+    ) -> Address:
         address = super().generate_contract_address(stack_data, call_data, computation)
         computation.state.mark_address_warm(address)
         return address
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/berlin/opcodes.py` & `py-evm-0.7.0a2/eth/vm/forks/berlin/opcodes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import copy
-from typing import Dict
+from typing import (
+    Dict,
+)
 
-from eth_utils.toolz import merge
+from eth_utils.toolz import (
+    merge,
+)
 
+from eth import (
+    constants,
+)
 from eth.vm import (
     mnemonics,
     opcode_values,
 )
-from eth.vm.opcode import (
-    Opcode,
-    as_opcode,
-)
-from eth import constants
-
-from eth.vm.forks.tangerine_whistle.constants import (
-    GAS_SELFDESTRUCT_EIP150,
-)
 from eth.vm.forks.byzantium.opcodes import (
     ensure_no_static,
 )
 from eth.vm.forks.muir_glacier.opcodes import (
     MUIR_GLACIER_OPCODES,
 )
+from eth.vm.forks.tangerine_whistle.constants import (
+    GAS_SELFDESTRUCT_EIP150,
+)
+from eth.vm.opcode import (
+    Opcode,
+    as_opcode,
+)
 
-from . import logic
-
+from . import (
+    logic,
+)
 
 UPDATED_OPCODES: Dict[int, Opcode] = {
     opcode_values.BALANCE: as_opcode(
         gas_cost=constants.GAS_NULL,
         logic_fn=logic.balance_eip2929,
         mnemonic=mnemonics.BALANCE,
     ),
@@ -55,40 +61,40 @@
     opcode_values.SSTORE: as_opcode(
         logic_fn=ensure_no_static(logic.sstore_eip2929),
         mnemonic=mnemonics.SSTORE,
         gas_cost=constants.GAS_NULL,
     ),
     # System opcodes
     opcode_values.CREATE: logic.CreateEIP2929.configure(
-        __name__='opcode:CREATE',
+        __name__="opcode:CREATE",
         mnemonic=mnemonics.CREATE,
         gas_cost=constants.GAS_CREATE,
     )(),
     opcode_values.CALL: logic.CallEIP2929.configure(
-        __name__='opcode:CALL',
+        __name__="opcode:CALL",
         mnemonic=mnemonics.CALL,
         gas_cost=constants.GAS_NULL,
     )(),
     opcode_values.CALLCODE: logic.CallCodeEIP2929.configure(
-        __name__='opcode:CALLCODE',
+        __name__="opcode:CALLCODE",
         mnemonic=mnemonics.CALLCODE,
         gas_cost=constants.GAS_NULL,
     )(),
     opcode_values.DELEGATECALL: logic.DelegateCallEIP2929.configure(
-        __name__='opcode:DELEGATECALL',
+        __name__="opcode:DELEGATECALL",
         mnemonic=mnemonics.DELEGATECALL,
         gas_cost=constants.GAS_NULL,
     )(),
     opcode_values.CREATE2: logic.Create2EIP2929.configure(
-        __name__='opcode:CREATE2',
+        __name__="opcode:CREATE2",
         mnemonic=mnemonics.CREATE2,
         gas_cost=constants.GAS_CREATE,
     )(),
     opcode_values.STATICCALL: logic.StaticCallEIP2929.configure(
-        __name__='opcode:STATICCALL',
+        __name__="opcode:STATICCALL",
         mnemonic=mnemonics.STATICCALL,
         gas_cost=constants.GAS_NULL,
     )(),
     opcode_values.SELFDESTRUCT: as_opcode(
         logic_fn=ensure_no_static(logic.selfdestruct_eip2929),
         mnemonic=mnemonics.SELFDESTRUCT,
         gas_cost=GAS_SELFDESTRUCT_EIP150,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/berlin/receipts.py` & `py-evm-0.7.0a2/eth/vm/forks/berlin/receipts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import (
     Any,
     Sequence,
     Type,
 )
 
-from cached_property import cached_property
-from eth_bloom import BloomFilter
+from cached_property import (
+    cached_property,
+)
+from eth_bloom import (
+    BloomFilter,
+)
 from eth_utils import (
     ValidationError,
     to_bytes,
     to_int,
 )
 import rlp
 from rlp.sedes import (
@@ -19,23 +23,26 @@
 from eth.abc import (
     DecodedZeroOrOneLayerRLP,
     LogAPI,
     ReceiptAPI,
     ReceiptBuilderAPI,
     ReceiptDecoderAPI,
 )
-from eth.exceptions import UnrecognizedTransactionType
-from eth.rlp.receipts import Receipt
+from eth.exceptions import (
+    UnrecognizedTransactionType,
+)
+from eth.rlp.receipts import (
+    Receipt,
+)
 
 from .constants import (
     ACCESS_LIST_TRANSACTION_TYPE,
     VALID_TRANSACTION_TYPES,
 )
 
-
 TYPED_RECEIPT_BODY_CODECS = {
     # Note that the body of a "type 1" receipt uses exactly the same codec as a
     # legacy receipt, so we can simply reuse all the logic.
     ACCESS_LIST_TRANSACTION_TYPE: Receipt,
 }
 
 
@@ -49,15 +56,16 @@
         self.type_id = type_id
         self._inner = proxy_target
 
         # Doing validation here means we don't have to validate on every encode()
         payload_codec = self.get_payload_codec(type_id)
         if not isinstance(proxy_target, payload_codec):
             raise ValidationError(
-                f"Cannot embed target {proxy_target!r} which doesn't match type ID {type_id}"
+                f"Cannot embed target {proxy_target!r} "
+                f"which doesn't match type ID {type_id}"
             )
 
     @classmethod
     def decode(cls, encoded: bytes) -> ReceiptAPI:
         type_id = to_int(encoded[0])
         payload = encoded[1:]
 
@@ -71,24 +79,26 @@
     @classmethod
     def get_payload_codec(cls, type_id: int) -> Type[ReceiptDecoderAPI]:
         if type_id in cls.codecs:
             return cls.codecs[type_id]
         elif type_id in VALID_TRANSACTION_TYPES:
             raise UnrecognizedTransactionType(type_id, "Unknown receipt type")
         else:
-            raise ValidationError(f"Cannot build typed receipt with {hex(type_id)} >= 0x80")
+            raise ValidationError(
+                f"Cannot build typed receipt with {hex(type_id)} >= 0x80"
+            )
 
     @classmethod
     def deserialize(cls, encoded_unchecked: DecodedZeroOrOneLayerRLP) -> ReceiptAPI:
         # binary checks a few basics, like the length of the bytes
         encoded = cls.rlp_type.deserialize(encoded_unchecked)
         return cls.decode(encoded)
 
     @classmethod
-    def serialize(cls, obj: 'TypedReceipt') -> DecodedZeroOrOneLayerRLP:
+    def serialize(cls, obj: "TypedReceipt") -> DecodedZeroOrOneLayerRLP:
         encoded = obj.encode()
         return cls.rlp_type.serialize(encoded)
 
     @cached_property
     def _type_byte(self) -> bytes:
         return to_bytes(self.type_id)
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/berlin/state.py` & `py-evm-0.7.0a2/eth/vm/forks/berlin/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-from typing import Type
+from typing import (
+    Type,
+)
 
 from eth.abc import (
     ComputationAPI,
     MessageAPI,
     SignedTransactionAPI,
     TransactionExecutorAPI,
 )
 from eth.vm.forks.muir_glacier.state import (
-    MuirGlacierState
+    MuirGlacierState,
 )
 from eth.vm.forks.spurious_dragon.state import (
     SpuriousDragonTransactionExecutor,
 )
 
-from .computation import BerlinComputation
+from .computation import (
+    BerlinComputation,
+)
 
 
 class BerlinTransactionExecutor(SpuriousDragonTransactionExecutor):
     def build_computation(
-            self,
-            message: MessageAPI,
-            transaction: SignedTransactionAPI) -> ComputationAPI:
-
+        self, message: MessageAPI, transaction: SignedTransactionAPI
+    ) -> ComputationAPI:
         self.vm_state.mark_address_warm(transaction.sender)
 
         # Mark recipient as accessed, or the new contract being created
         self.vm_state.mark_address_warm(message.storage_address)
 
         for address, slots in transaction.access_list:
             self.vm_state.mark_address_warm(address)
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/berlin/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/berlin/transactions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from typing import (
     Any,
     Dict,
     Sequence,
     Tuple,
     Type,
-    cast,
     Union,
+    cast,
 )
 
-from cached_property import cached_property
-from eth_keys.datatypes import PrivateKey
-from eth_hash.auto import keccak
+from cached_property import (
+    cached_property,
+)
+from eth_hash.auto import (
+    keccak,
+)
+from eth_keys.datatypes import (
+    PrivateKey,
+)
 from eth_typing import (
     Address,
     Hash32,
 )
 from eth_utils import (
     ValidationError,
     to_bytes,
@@ -25,49 +31,60 @@
     BigEndianInt,
     Binary,
     CountableList,
     big_endian_int,
     binary,
 )
 
+from eth._utils.transactions import (
+    calculate_intrinsic_gas,
+    create_transaction_signature,
+    extract_transaction_sender,
+    validate_transaction_signature,
+)
 from eth.abc import (
     DecodedZeroOrOneLayerRLP,
     ReceiptAPI,
     SignedTransactionAPI,
     TransactionBuilderAPI,
     TransactionDecoderAPI,
     UnsignedTransactionAPI,
 )
-from eth.constants import CREATE_CONTRACT_ADDRESS
-from eth.exceptions import UnrecognizedTransactionType
-from eth.rlp.logs import Log
-from eth.rlp.receipts import Receipt
-from eth.rlp.sedes import address
-from eth.rlp.transactions import SignedTransactionMethods
+from eth.constants import (
+    CREATE_CONTRACT_ADDRESS,
+)
+from eth.exceptions import (
+    UnrecognizedTransactionType,
+)
+from eth.rlp.logs import (
+    Log,
+)
+from eth.rlp.receipts import (
+    Receipt,
+)
+from eth.rlp.sedes import (
+    address,
+)
+from eth.rlp.transactions import (
+    SignedTransactionMethods,
+)
 from eth.validation import (
     validate_canonical_address,
     validate_is_bytes,
     validate_is_transaction_access_list,
     validate_uint256,
 )
 from eth.vm.forks.istanbul.transactions import (
     ISTANBUL_TX_GAS_SCHEDULE,
 )
 from eth.vm.forks.muir_glacier.transactions import (
     MuirGlacierTransaction,
     MuirGlacierUnsignedTransaction,
 )
 
-from eth._utils.transactions import (
-    calculate_intrinsic_gas,
-    create_transaction_signature,
-    extract_transaction_sender,
-    validate_transaction_signature,
-)
-
 from .constants import (
     ACCESS_LIST_ADDRESS_COST_EIP_2930,
     ACCESS_LIST_STORAGE_KEY_COST_EIP_2930,
     ACCESS_LIST_TRANSACTION_TYPE,
     VALID_TRANSACTION_TYPES,
 )
 from .receipts import (
@@ -76,17 +93,17 @@
 
 
 class BerlinLegacyTransaction(MuirGlacierTransaction):
     pass
 
 
 class BerlinUnsignedLegacyTransaction(MuirGlacierUnsignedTransaction):
-    def as_signed_transaction(self,
-                              private_key: PrivateKey,
-                              chain_id: int = None) -> BerlinLegacyTransaction:
+    def as_signed_transaction(
+        self, private_key: PrivateKey, chain_id: int = None
+    ) -> BerlinLegacyTransaction:
         v, r, s = create_transaction_signature(self, private_key, chain_id=chain_id)
         return BerlinLegacyTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
             value=self.value,
@@ -95,41 +112,41 @@
             r=r,
             s=s,
         )
 
 
 class AccountAccesses(rlp.Serializable):
     fields = [
-        ('account', address),
-        ('storage_keys', CountableList(BigEndianInt(32))),
+        ("account", address),
+        ("storage_keys", CountableList(BigEndianInt(32))),
     ]
 
 
 class UnsignedAccessListTransaction(rlp.Serializable):
     _type_id = ACCESS_LIST_TRANSACTION_TYPE
     fields = [
-        ('chain_id', big_endian_int),
-        ('nonce', big_endian_int),
-        ('gas_price', big_endian_int),
-        ('gas', big_endian_int),
-        ('to', address),
-        ('value', big_endian_int),
-        ('data', binary),
-        ('access_list', CountableList(AccountAccesses)),
+        ("chain_id", big_endian_int),
+        ("nonce", big_endian_int),
+        ("gas_price", big_endian_int),
+        ("gas", big_endian_int),
+        ("to", address),
+        ("value", big_endian_int),
+        ("data", binary),
+        ("access_list", CountableList(AccountAccesses)),
     ]
 
     @cached_property
     def _type_byte(self) -> bytes:
         return to_bytes(self._type_id)
 
     def get_message_for_signing(self) -> bytes:
         payload = rlp.encode(self)
         return self._type_byte + payload
 
-    def as_signed_transaction(self, private_key: PrivateKey) -> 'TypedTransaction':
+    def as_signed_transaction(self, private_key: PrivateKey) -> "TypedTransaction":
         message = self.get_message_for_signing()
         signature = private_key.sign_msg(message)
         y_parity, r, s = signature.vrs
 
         signed_transaction = AccessListTransaction(
             self.chain_id,
             self.nonce,
@@ -137,15 +154,15 @@
             self.gas,
             self.to,
             self.value,
             self.data,
             self.access_list,
             y_parity,
             r,
-            s
+            s,
         )
         return TypedTransaction(self._type_id, signed_transaction)
 
     def validate(self) -> None:
         validate_uint256(self.chain_id, title="Transaction.chain_id")
         validate_uint256(self.nonce, title="Transaction.nonce")
         validate_uint256(self.gas_price, title="Transaction.gas_price")
@@ -169,28 +186,30 @@
         return self.gas_price
 
     @property
     def max_fee_per_gas(self) -> int:
         return self.gas_price
 
 
-class AccessListTransaction(rlp.Serializable, SignedTransactionMethods, SignedTransactionAPI):
+class AccessListTransaction(
+    rlp.Serializable, SignedTransactionMethods, SignedTransactionAPI
+):
     _type_id = ACCESS_LIST_TRANSACTION_TYPE
     fields = [
-        ('chain_id', big_endian_int),
-        ('nonce', big_endian_int),
-        ('gas_price', big_endian_int),
-        ('gas', big_endian_int),
-        ('to', address),
-        ('value', big_endian_int),
-        ('data', binary),
-        ('access_list', CountableList(AccountAccesses)),
-        ('y_parity', big_endian_int),
-        ('r', big_endian_int),
-        ('s', big_endian_int),
+        ("chain_id", big_endian_int),
+        ("nonce", big_endian_int),
+        ("gas_price", big_endian_int),
+        ("gas", big_endian_int),
+        ("to", address),
+        ("value", big_endian_int),
+        ("data", binary),
+        ("access_list", CountableList(AccountAccesses)),
+        ("y_parity", big_endian_int),
+        ("r", big_endian_int),
+        ("s", big_endian_int),
     ]
 
     def get_sender(self) -> Address:
         return extract_transaction_sender(self)
 
     def get_message_for_signing(self) -> bytes:
         unsigned = UnsignedAccessListTransaction(
@@ -220,24 +239,20 @@
     def get_intrinsic_gas(self) -> int:
         return _get_access_list_txn_intrinsic_gas(self)
 
     def encode(self) -> bytes:
         return rlp.encode(self)
 
     def make_receipt(
-            self,
-            status: bytes,
-            gas_used: int,
-            log_entries: Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...]) -> ReceiptAPI:
-
-        logs = [
-            Log(address, topics, data)
-            for address, topics, data
-            in log_entries
-        ]
+        self,
+        status: bytes,
+        gas_used: int,
+        log_entries: Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...],
+    ) -> ReceiptAPI:
+        logs = [Log(address, topics, data) for address, topics, data in log_entries]
         # TypedTransaction is responsible for wrapping this into a TypedReceipt
         return Receipt(
             state_root=status,
             gas_used=gas_used,
             logs=logs,
         )
 
@@ -253,15 +268,17 @@
 
 class AccessListPayloadDecoder(TransactionDecoderAPI):
     @classmethod
     def decode(cls, payload: bytes) -> SignedTransactionAPI:
         return rlp.decode(payload, sedes=AccessListTransaction)
 
 
-class TypedTransaction(SignedTransactionMethods, SignedTransactionAPI, TransactionDecoderAPI):
+class TypedTransaction(
+    SignedTransactionMethods, SignedTransactionAPI, TransactionDecoderAPI
+):
     rlp_type = Binary(min_length=1)  # must have at least one byte for the type
     _inner: SignedTransactionAPI
 
     decoders: Dict[int, Type[TransactionDecoderAPI]] = {
         ACCESS_LIST_TRANSACTION_TYPE: AccessListPayloadDecoder,
     }
     receipt_builder = BerlinReceiptBuilder
@@ -273,35 +290,39 @@
     @classmethod
     def get_payload_codec(cls, type_id: int) -> Type[TransactionDecoderAPI]:
         if type_id in cls.decoders:
             return cls.decoders[type_id]
         elif type_id in VALID_TRANSACTION_TYPES:
             raise UnrecognizedTransactionType(type_id, "Unknown transaction type")
         else:
-            raise ValidationError(f"Cannot build typed transaction with {hex(type_id)} >= 0x80")
+            raise ValidationError(
+                f"Cannot build typed transaction with {hex(type_id)} >= 0x80"
+            )
 
     def encode(self) -> bytes:
         return self._type_byte + self._inner.encode()
 
     @classmethod
     def decode(cls, encoded: bytes) -> SignedTransactionAPI:
         type_id = to_int(encoded[0])
         payload = encoded[1:]
 
         payload_codec = cls.get_payload_codec(type_id)
         inner_transaction = payload_codec.decode(payload)
         return cls(type_id, inner_transaction)
 
     @classmethod
-    def serialize(cls, obj: 'TypedTransaction') -> DecodedZeroOrOneLayerRLP:
+    def serialize(cls, obj: "TypedTransaction") -> DecodedZeroOrOneLayerRLP:
         encoded = obj.encode()
         return cls.rlp_type.serialize(encoded)
 
     @classmethod
-    def deserialize(cls, encoded_unchecked: DecodedZeroOrOneLayerRLP) -> SignedTransactionAPI:
+    def deserialize(
+        cls, encoded_unchecked: DecodedZeroOrOneLayerRLP
+    ) -> SignedTransactionAPI:
         # binary checks a few basics, like the length of the bytes
         encoded = cls.rlp_type.deserialize(encoded_unchecked)
         return cls.decode(encoded)
 
     @cached_property
     def _type_byte(self) -> bytes:
         return to_bytes(self.type_id)
@@ -370,30 +391,30 @@
     @cached_property
     def hash(self) -> Hash32:
         return cast(Hash32, keccak(self.encode()))
 
     def get_intrinsic_gas(self) -> int:
         return self._inner.get_intrinsic_gas()
 
-    def copy(self, **overrides: Any) -> 'TypedTransaction':
+    def copy(self, **overrides: Any) -> "TypedTransaction":
         inner_copy = self._inner.copy(**overrides)
         return type(self)(self.type_id, inner_copy)
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, TypedTransaction):
             return False
         else:
             return self.type_id == other.type_id and self._inner == other._inner
 
     def make_receipt(
-            self,
-            status: bytes,
-            gas_used: int,
-            log_entries: Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...]) -> ReceiptAPI:
-
+        self,
+        status: bytes,
+        gas_used: int,
+        log_entries: Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...],
+    ) -> ReceiptAPI:
         inner_receipt = self._inner.make_receipt(status, gas_used, log_entries)
 
         return self.receipt_builder.typed_receipt_class(self.type_id, inner_receipt)
 
     def __hash__(self) -> int:
         return hash((self.type_id, self._inner))
 
@@ -401,22 +422,25 @@
 class BerlinTransactionBuilder(TransactionBuilderAPI):
     """
     Responsible for serializing transactions of ambiguous type.
 
     It dispatches to either the legacy transaction type or the new typed
     transaction, depending on the nature of the encoded/decoded transaction.
     """
+
     legacy_signed = BerlinLegacyTransaction
     legacy_unsigned = BerlinUnsignedLegacyTransaction
     typed_transaction = TypedTransaction
 
     @classmethod
     def decode(cls, encoded: bytes) -> SignedTransactionAPI:
         if len(encoded) == 0:
-            raise ValidationError("Encoded transaction was empty, which makes it invalid")
+            raise ValidationError(
+                "Encoded transaction was empty, which makes it invalid"
+            )
 
         type_id = to_int(encoded[0])
         if type_id in VALID_TRANSACTION_TYPES:
             return cls.typed_transaction.decode(encoded)
         else:
             return rlp.decode(encoded, sedes=cls.legacy_signed)
 
@@ -431,75 +455,80 @@
     def serialize(cls, obj: SignedTransactionAPI) -> DecodedZeroOrOneLayerRLP:
         if isinstance(obj, cls.typed_transaction):
             return cls.typed_transaction.serialize(obj)
         else:
             return cls.legacy_signed.serialize(obj)
 
     @classmethod
-    def create_unsigned_transaction(cls,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> UnsignedTransactionAPI:
+    def create_unsigned_transaction(
+        cls,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+    ) -> UnsignedTransactionAPI:
         return cls.legacy_unsigned(nonce, gas_price, gas, to, value, data)
 
     @classmethod
     def new_transaction(
-            cls,
-            nonce: int,
-            gas_price: int,
-            gas: int,
-            to: Address,
-            value: int,
-            data: bytes,
-            v: int,
-            r: int,
-            s: int) -> SignedTransactionAPI:
+        cls,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+        v: int,
+        r: int,
+        s: int,
+    ) -> SignedTransactionAPI:
         return cls.legacy_signed(nonce, gas_price, gas, to, value, data, v, r, s)
 
     @classmethod
     def new_unsigned_access_list_transaction(
-            cls,
-            chain_id: int,
-            nonce: int,
-            gas_price: int,
-            gas: int,
-            to: Address,
-            value: int,
-            data: bytes,
-            access_list: Sequence[Tuple[Address, Sequence[int]]]) -> TypedTransaction:
+        cls,
+        chain_id: int,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+        access_list: Sequence[Tuple[Address, Sequence[int]]],
+    ) -> TypedTransaction:
         transaction = UnsignedAccessListTransaction(
             chain_id,
             nonce,
             gas_price,
             gas,
             to,
             value,
             data,
             access_list,
         )
         return transaction
 
     @classmethod
     def new_access_list_transaction(
-            cls,
-            chain_id: int,
-            nonce: int,
-            gas_price: int,
-            gas: int,
-            to: Address,
-            value: int,
-            data: bytes,
-            access_list: Sequence[Tuple[Address, Sequence[int]]],
-            y_parity: int,
-            r: int,
-            s: int) -> TypedTransaction:
+        cls,
+        chain_id: int,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+        access_list: Sequence[Tuple[Address, Sequence[int]]],
+        y_parity: int,
+        r: int,
+        s: int,
+    ) -> TypedTransaction:
         transaction = AccessListTransaction(
             chain_id,
             nonce,
             gas_price,
             gas,
             to,
             value,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/byzantium/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/byzantium/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,37 +40,39 @@
     configure_byzantium_header,
     compute_byzantium_difficulty,
 )
 from .state import ByzantiumState
 
 
 @curry
-def get_uncle_reward(block_reward: int, block_number: int, uncle: BlockHeaderAPI) -> int:
+def get_uncle_reward(
+    block_reward: int, block_number: int, uncle: BlockHeaderAPI
+) -> int:
     block_number_delta = block_number - uncle.block_number
     validate_lte(block_number_delta, MAX_UNCLE_DEPTH)
     return (8 - block_number_delta) * block_reward // 8
 
 
 EIP658_STATUS_CODES = {
     EIP658_TRANSACTION_STATUS_CODE_SUCCESS,
     EIP658_TRANSACTION_STATUS_CODE_FAILURE,
 }
 
 
 class ByzantiumVM(SpuriousDragonVM):
     # fork name
-    fork = 'byzantium'
+    fork = "byzantium"
 
     # classes
     block_class: Type[BlockAPI] = ByzantiumBlock
     _state_class: Type[StateAPI] = ByzantiumState
 
     # Methods
-    create_header_from_parent = staticmethod(create_byzantium_header_from_parent)   # type: ignore
-    compute_difficulty = staticmethod(compute_byzantium_difficulty)     # type: ignore
+    create_header_from_parent = staticmethod(create_byzantium_header_from_parent)  # type: ignore  # noqa: E501
+    compute_difficulty = staticmethod(compute_byzantium_difficulty)  # type: ignore
     configure_header = configure_byzantium_header
     # Separated into two steps due to mypy bug of staticmethod.
     # https://github.com/python/mypy/issues/5530
     get_uncle_reward = get_uncle_reward(EIP649_BLOCK_REWARD)
     get_uncle_reward = staticmethod(get_uncle_reward)
 
     @classmethod
@@ -84,34 +86,38 @@
                 f"{encode_hex(receipt.state_root)}"
             )
 
     @staticmethod
     def get_block_reward() -> int:
         return EIP649_BLOCK_REWARD
 
-    def add_receipt_to_header(self,
-                              old_header: BlockHeaderAPI,
-                              receipt: ReceiptAPI) -> BlockHeaderAPI:
-        # Skip merkelizing the account data and persisting it to disk on every transaction.
-        # Starting in Byzantium, this is no longer necessary, because the state root isn't
-        # in the receipt anymore.
+    def add_receipt_to_header(
+        self, old_header: BlockHeaderAPI, receipt: ReceiptAPI
+    ) -> BlockHeaderAPI:
+        # Skip merkelizing the account data and persisting it to disk on every
+        # transaction. Starting in Byzantium, this is no longer necessary,
+        # because the state root isn't in the receipt anymore.
         return old_header.copy(
             bloom=int(BloomFilter(old_header.bloom) | receipt.bloom),
             gas_used=receipt.gas_used,
         )
 
     @classmethod
     def make_receipt(
-            cls,
-            base_header: BlockHeaderAPI,
-            transaction: SignedTransactionAPI,
-            computation: ComputationAPI,
-            state: StateAPI) -> ReceiptAPI:
-
-        gas_used = base_header.gas_used + cls.finalize_gas_used(transaction, computation)
+        cls,
+        base_header: BlockHeaderAPI,
+        transaction: SignedTransactionAPI,
+        computation: ComputationAPI,
+        state: StateAPI,
+    ) -> ReceiptAPI:
+        gas_used = base_header.gas_used + cls.finalize_gas_used(
+            transaction, computation
+        )
 
         if computation.is_error:
             status_code = EIP658_TRANSACTION_STATUS_CODE_FAILURE
         else:
             status_code = EIP658_TRANSACTION_STATUS_CODE_SUCCESS
 
-        return transaction.make_receipt(status_code, gas_used, computation.get_log_entries())
+        return transaction.make_receipt(
+            status_code, gas_used, computation.get_log_entries()
+        )
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/byzantium/computation.py` & `py-evm-0.7.0a2/eth/vm/forks/byzantium/computation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 from eth_utils.toolz import (
     merge,
 )
 
-from eth import precompiles
+from eth import (
+    precompiles,
+)
 from eth._utils.address import (
     force_bytes_to_address,
 )
-from eth.vm.forks.frontier.computation import FRONTIER_PRECOMPILES
-from eth.vm.forks.spurious_dragon.computation import SpuriousDragonComputation
+from eth.vm.forks.frontier.computation import (
+    FRONTIER_PRECOMPILES,
+)
+from eth.vm.forks.spurious_dragon.computation import (
+    SpuriousDragonComputation,
+)
 
-from .opcodes import BYZANTIUM_OPCODES
+from .opcodes import (
+    BYZANTIUM_OPCODES,
+)
 
 BYZANTIUM_PRECOMPILES = merge(
     FRONTIER_PRECOMPILES,
     {
-        force_bytes_to_address(b'\x05'): precompiles.modexp,
-        force_bytes_to_address(b'\x06'): precompiles.ecadd,
-        force_bytes_to_address(b'\x07'): precompiles.ecmul,
-        force_bytes_to_address(b'\x08'): precompiles.ecpairing,
+        force_bytes_to_address(b"\x05"): precompiles.modexp,
+        force_bytes_to_address(b"\x06"): precompiles.ecadd,
+        force_bytes_to_address(b"\x07"): precompiles.ecmul,
+        force_bytes_to_address(b"\x08"): precompiles.ecpairing,
     },
 )
 
 
 class ByzantiumComputation(SpuriousDragonComputation):
     """
-    A class for all execution computations in the ``Byzantium`` fork.
-    Inherits from :class:`~eth.vm.forks.spurious_dragon.computation.SpuriousDragonComputation`
+    A class for all execution *message* computations in the ``Byzantium`` fork.
+    Inherits from
+    :class:`~eth.vm.forks.spurious_dragon.computation.SpuriousDragonComputation`
     """
+
     # Override
     opcodes = BYZANTIUM_OPCODES
     _precompiles = BYZANTIUM_PRECOMPILES
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/byzantium/headers.py` & `py-evm-0.7.0a2/eth/vm/forks/byzantium/headers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 from typing import (
     Any,
     Callable,
 )
+
 from eth_utils.toolz import (
     curry,
 )
 
+from eth._utils.db import (
+    get_parent_header,
+)
+from eth._utils.headers import (
+    new_timestamp_from_parent,
+)
 from eth.abc import (
     BlockHeaderAPI,
     VirtualMachineAPI,
 )
 from eth.constants import (
-    EMPTY_UNCLE_HASH,
+    BOMB_EXPONENTIAL_FREE_PERIODS,
+    BOMB_EXPONENTIAL_PERIOD,
     DIFFICULTY_ADJUSTMENT_DENOMINATOR,
     DIFFICULTY_MINIMUM,
-    BOMB_EXPONENTIAL_PERIOD,
-    BOMB_EXPONENTIAL_FREE_PERIODS,
-)
-from eth._utils.db import (
-    get_parent_header,
-)
-from eth._utils.headers import (
-    new_timestamp_from_parent,
+    EMPTY_UNCLE_HASH,
 )
 from eth.validation import (
     validate_gt,
     validate_header_params_for_configuration,
 )
 from eth.vm.forks.frontier.headers import (
     create_frontier_header_from_parent,
 )
 
 from .constants import (
-    BYZANTIUM_DIFFICULTY_ADJUSTMENT_CUTOFF
+    BYZANTIUM_DIFFICULTY_ADJUSTMENT_CUTOFF,
 )
 
 
 @curry
 def compute_difficulty(
-        bomb_delay: int,
-        parent_header: BlockHeaderAPI,
-        timestamp: int) -> int:
+    bomb_delay: int, parent_header: BlockHeaderAPI, timestamp: int
+) -> int:
     """
     https://github.com/ethereum/EIPs/issues/100
     """
     parent_timestamp = parent_header.timestamp
     validate_gt(timestamp, parent_timestamp, title="Header.timestamp")
 
     parent_difficulty = parent_header.difficulty
@@ -54,69 +54,71 @@
     adj_factor = max(
         (
             (2 if has_uncles else 1)
             - ((timestamp - parent_timestamp) // BYZANTIUM_DIFFICULTY_ADJUSTMENT_CUTOFF)
         ),
         -99,
     )
-    difficulty = max(
-        parent_difficulty + offset * adj_factor,
-        DIFFICULTY_MINIMUM
-    )
+    difficulty = max(parent_difficulty + offset * adj_factor, DIFFICULTY_MINIMUM)
     num_bomb_periods = (
         max(
             0,
             parent_header.block_number + 1 - bomb_delay,
-        ) // BOMB_EXPONENTIAL_PERIOD
+        )
+        // BOMB_EXPONENTIAL_PERIOD
     ) - BOMB_EXPONENTIAL_FREE_PERIODS
 
     if num_bomb_periods >= 0:
         return max(difficulty + 2**num_bomb_periods, DIFFICULTY_MINIMUM)
     else:
         return difficulty
 
 
 @curry
-def create_header_from_parent(difficulty_fn: Callable[[BlockHeaderAPI, int], int],
-                              parent_header: BlockHeaderAPI,
-                              **header_params: Any) -> BlockHeaderAPI:
-
-    if 'timestamp' not in header_params:
-        header_params['timestamp'] = new_timestamp_from_parent(parent_header)
+def create_header_from_parent(
+    difficulty_fn: Callable[[BlockHeaderAPI, int], int],
+    parent_header: BlockHeaderAPI,
+    **header_params: Any,
+) -> BlockHeaderAPI:
+    if "timestamp" not in header_params:
+        header_params["timestamp"] = new_timestamp_from_parent(parent_header)
 
-    if 'difficulty' not in header_params:
-        header_params['difficulty'] = difficulty_fn(
+    if "difficulty" not in header_params:
+        header_params["difficulty"] = difficulty_fn(
             parent_header,
-            header_params['timestamp'],
+            header_params["timestamp"],
         )
     return create_frontier_header_from_parent(parent_header, **header_params)
 
 
 @curry
 def configure_header(
     vm: VirtualMachineAPI,
     difficulty_fn: Callable[[BlockHeaderAPI, int], int] = None,
     **header_params: Any,
 ) -> BlockHeaderAPI:
     validate_header_params_for_configuration(header_params)
 
     with vm.get_header().build_changeset(**header_params) as changeset:
         if (
-            'timestamp' in header_params
+            "timestamp" in header_params
             and changeset.block_number > 0
-
             # post-POS does not use difficulty_fn
             and difficulty_fn is not None
         ):
             parent_header = get_parent_header(changeset.build_rlp(), vm.chaindb)
             changeset.difficulty = difficulty_fn(
                 parent_header,
-                header_params['timestamp'],
+                header_params["timestamp"],
             )
 
         header = changeset.commit()
     return header
 
 
 compute_byzantium_difficulty = compute_difficulty(3000000)
-create_byzantium_header_from_parent = create_header_from_parent(compute_byzantium_difficulty)
-configure_byzantium_header = configure_header(difficulty_fn=compute_byzantium_difficulty)
+create_byzantium_header_from_parent = create_header_from_parent(
+    compute_byzantium_difficulty
+)
+configure_byzantium_header = configure_header(
+    difficulty_fn=compute_byzantium_difficulty
+)
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/byzantium/opcodes.py` & `py-evm-0.7.0a2/eth/vm/forks/byzantium/opcodes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 import copy
 import functools
-from typing import Dict
-
-from eth_utils.toolz import merge
-
 from typing import (
     Any,
     Callable,
+    Dict,
 )
 
-from eth import constants
+from eth_utils.toolz import (
+    merge,
+)
 
-from eth.abc import OpcodeAPI
+from eth import (
+    constants,
+)
+from eth.abc import (
+    ComputationAPI,
+    OpcodeAPI,
+)
 from eth.exceptions import (
     WriteProtection,
 )
-from eth.vm import mnemonics
-from eth.vm import opcode_values
-from eth.vm.computation import BaseComputation
+from eth.vm import (
+    mnemonics,
+    opcode_values,
+)
+from eth.vm.forks.spurious_dragon.opcodes import (
+    SPURIOUS_DRAGON_OPCODES,
+)
 from eth.vm.forks.tangerine_whistle.constants import (
     GAS_CALL_EIP150,
-    GAS_SELFDESTRUCT_EIP150
+    GAS_SELFDESTRUCT_EIP150,
 )
 from eth.vm.logic import (
     call,
     context,
     logging,
     storage,
     system,
 )
-from eth.vm.opcode import as_opcode
-
-from eth.vm.forks.spurious_dragon.opcodes import SPURIOUS_DRAGON_OPCODES
+from eth.vm.opcode import (
+    as_opcode,
+)
 
 
 def ensure_no_static(opcode_fn: Callable[..., Any]) -> Callable[..., Any]:
     @functools.wraps(opcode_fn)
-    def inner(computation: BaseComputation) -> Callable[..., Any]:
+    def inner(computation: ComputationAPI) -> Callable[..., Any]:
         if computation.msg.is_static:
-            raise WriteProtection("Cannot modify state while inside of a STATICCALL context")
+            raise WriteProtection(
+                "Cannot modify state while inside of a STATICCALL context"
+            )
         return opcode_fn(computation)
+
     return inner
 
 
 UPDATED_OPCODES = {
     opcode_values.REVERT: as_opcode(
         logic_fn=system.revert,
         mnemonic=mnemonics.REVERT,
@@ -62,20 +74,20 @@
         mnemonic=mnemonics.RETURNDATACOPY,
         gas_cost=constants.GAS_VERYLOW,
     ),
     #
     # Call
     #
     opcode_values.STATICCALL: call.StaticCall.configure(
-        __name__='opcode:STATICCALL',
+        __name__="opcode:STATICCALL",
         mnemonic=mnemonics.STATICCALL,
         gas_cost=GAS_CALL_EIP150,
     )(),
     opcode_values.CALL: call.CallByzantium.configure(
-        __name__='opcode:CALL',
+        __name__="opcode:CALL",
         mnemonic=mnemonics.CALL,
         gas_cost=GAS_CALL_EIP150,
     )(),
     #
     # Logging
     #
     opcode_values.LOG0: as_opcode(
@@ -103,15 +115,15 @@
         mnemonic=mnemonics.LOG4,
         gas_cost=constants.GAS_LOG,
     ),
     #
     # Create
     #
     opcode_values.CREATE: system.CreateByzantium.configure(
-        __name__='opcode:CREATE',
+        __name__="opcode:CREATE",
         mnemonic=mnemonics.CREATE,
         gas_cost=constants.GAS_CREATE,
     )(),
     #
     # Storage
     #
     opcode_values.SSTORE: as_opcode(
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/byzantium/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/muir_glacier/transactions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-from eth_keys.datatypes import PrivateKey
-from eth_typing import Address
+from eth_keys.datatypes import (
+    PrivateKey,
+)
+from eth_typing import (
+    Address,
+)
 
 from eth._utils.transactions import (
     create_transaction_signature,
 )
-
-from eth.vm.forks.spurious_dragon.transactions import (
-    SpuriousDragonTransaction,
-    SpuriousDragonUnsignedTransaction,
+from eth.vm.forks.istanbul.transactions import (
+    IstanbulTransaction,
+    IstanbulUnsignedTransaction,
 )
 
 
-class ByzantiumTransaction(SpuriousDragonTransaction):
+class MuirGlacierTransaction(IstanbulTransaction):
     @classmethod
-    def create_unsigned_transaction(cls,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> 'ByzantiumUnsignedTransaction':
-        return ByzantiumUnsignedTransaction(nonce, gas_price, gas, to, value, data)
-
-
-class ByzantiumUnsignedTransaction(SpuriousDragonUnsignedTransaction):
-    def as_signed_transaction(self,
-                              private_key: PrivateKey,
-                              chain_id: int = None) -> ByzantiumTransaction:
+    def create_unsigned_transaction(
+        cls,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes
+    ) -> "MuirGlacierUnsignedTransaction":
+        return MuirGlacierUnsignedTransaction(nonce, gas_price, gas, to, value, data)
+
+
+class MuirGlacierUnsignedTransaction(IstanbulUnsignedTransaction):
+    def as_signed_transaction(
+        self, private_key: PrivateKey, chain_id: int = None
+    ) -> MuirGlacierTransaction:
         v, r, s = create_transaction_signature(self, private_key, chain_id=chain_id)
-        return ByzantiumTransaction(
+        return MuirGlacierTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
             value=self.value,
             data=self.data,
             v=v,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/constantinople/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/constantinople/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     create_constantinople_header_from_parent,
 )
 from .state import ConstantinopleState
 
 
 class ConstantinopleVM(ByzantiumVM):
     # fork name
-    fork = 'constantinople'
+    fork = "constantinople"
 
     # classes
     block_class: Type[BaseBlock] = ConstantinopleBlock
     _state_class: Type[BaseState] = ConstantinopleState
 
     # Methods
     create_header_from_parent = staticmethod(create_constantinople_header_from_parent)  # type: ignore  # noqa: E501
-    compute_difficulty = staticmethod(compute_constantinople_difficulty)    # type: ignore
+    compute_difficulty = staticmethod(compute_constantinople_difficulty)  # type: ignore
     configure_header = configure_constantinople_header
     get_uncle_reward = staticmethod(get_uncle_reward(EIP1234_BLOCK_REWARD))
 
     @staticmethod
     def get_block_reward() -> int:
         return EIP1234_BLOCK_REWARD
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/constantinople/opcodes.py` & `py-evm-0.7.0a2/eth/vm/forks/constantinople/opcodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import copy
+
 from eth_utils.toolz import (
-    merge
+    merge,
 )
 
 from eth import (
-    constants
+    constants,
 )
 from eth.vm import (
     mnemonics,
     opcode_values,
 )
 from eth.vm.forks.byzantium.opcodes import (
     BYZANTIUM_OPCODES,
-    ensure_no_static
+    ensure_no_static,
 )
 from eth.vm.forks.constantinople.constants import (
-    GAS_EXTCODEHASH_EIP1052
+    GAS_EXTCODEHASH_EIP1052,
 )
 from eth.vm.forks.constantinople.storage import (
     sstore_eip1283,
 )
 from eth.vm.logic import (
     arithmetic,
     context,
     system,
 )
 from eth.vm.opcode import (
-    as_opcode
+    as_opcode,
 )
 
-
 UPDATED_OPCODES = {
     opcode_values.SHL: as_opcode(
         logic_fn=arithmetic.shl,
         mnemonic=mnemonics.SHL,
         gas_cost=constants.GAS_VERYLOW,
     ),
     opcode_values.SHR: as_opcode(
@@ -48,15 +48,15 @@
     ),
     opcode_values.EXTCODEHASH: as_opcode(
         logic_fn=context.extcodehash,
         mnemonic=mnemonics.EXTCODEHASH,
         gas_cost=GAS_EXTCODEHASH_EIP1052,
     ),
     opcode_values.CREATE2: system.Create2.configure(
-        __name__='opcode:CREATE2',
+        __name__="opcode:CREATE2",
         mnemonic=mnemonics.CREATE2,
         gas_cost=constants.GAS_CREATE,
     )(),
     opcode_values.SSTORE: as_opcode(
         logic_fn=ensure_no_static(sstore_eip1283),
         mnemonic=mnemonics.SSTORE,
         gas_cost=constants.GAS_NULL,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/constantinople/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/constantinople/transactions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-from eth_keys.datatypes import PrivateKey
-from eth_typing import Address
-
-from eth.vm.forks.byzantium.transactions import (
-    ByzantiumTransaction,
-    ByzantiumUnsignedTransaction,
+from eth_keys.datatypes import (
+    PrivateKey,
+)
+from eth_typing import (
+    Address,
 )
 
 from eth._utils.transactions import (
     create_transaction_signature,
 )
+from eth.vm.forks.byzantium.transactions import (
+    ByzantiumTransaction,
+    ByzantiumUnsignedTransaction,
+)
 
 
 class ConstantinopleTransaction(ByzantiumTransaction):
     @classmethod
-    def create_unsigned_transaction(cls,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> 'ConstantinopleUnsignedTransaction':
+    def create_unsigned_transaction(
+        cls,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes
+    ) -> "ConstantinopleUnsignedTransaction":
         return ConstantinopleUnsignedTransaction(nonce, gas_price, gas, to, value, data)
 
 
 class ConstantinopleUnsignedTransaction(ByzantiumUnsignedTransaction):
-    def as_signed_transaction(self,
-                              private_key: PrivateKey,
-                              chain_id: int = None) -> ConstantinopleTransaction:
+    def as_signed_transaction(
+        self, private_key: PrivateKey, chain_id: int = None
+    ) -> ConstantinopleTransaction:
         v, r, s = create_transaction_signature(self, private_key, chain_id=chain_id)
         return ConstantinopleTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
             value=self.value,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/frontier/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/frontier/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,98 +31,100 @@
     create_frontier_header_from_parent,
     compute_frontier_difficulty,
     configure_frontier_header,
 )
 from .validation import validate_frontier_transaction_against_header
 
 
-def make_frontier_receipt(computation: ComputationAPI,
-                          new_cumulative_gas_used: int) -> ReceiptAPI:
+def make_frontier_receipt(
+    computation: ComputationAPI, new_cumulative_gas_used: int
+) -> ReceiptAPI:
     # Reusable for other forks
-    # This skips setting the state root (set to 0 instead). The logic for making a state root
-    # lives in the FrontierVM, so that state merkelization at each receipt is skipped at Byzantium+.
+    # This skips setting the state root (set to 0 instead). The logic for making a
+    # state root lives in the FrontierVM, so that state merkelization at each receipt
+    # is skipped at Byzantium+.
 
     logs = [
         Log(address, topics, data)
-        for address, topics, data
-        in computation.get_log_entries()
+        for address, topics, data in computation.get_log_entries()
     ]
 
     receipt = Receipt(
         state_root=ZERO_HASH32,
         gas_used=new_cumulative_gas_used,
         logs=logs,
     )
 
     return receipt
 
 
 class FrontierVM(VM):
     # fork name
-    fork: str = 'frontier'
+    fork: str = "frontier"
 
     # classes
     block_class: Type[BlockAPI] = FrontierBlock
     _state_class: Type[StateAPI] = FrontierState
 
     # methods
-    create_header_from_parent = staticmethod(create_frontier_header_from_parent)    # type: ignore
-    compute_difficulty = staticmethod(compute_frontier_difficulty)      # type: ignore
+    create_header_from_parent = staticmethod(create_frontier_header_from_parent)  # type: ignore  # noqa: E501
+    compute_difficulty = staticmethod(compute_frontier_difficulty)  # type: ignore
     configure_header = configure_frontier_header
     validate_transaction_against_header = validate_frontier_transaction_against_header
 
     @staticmethod
     def get_block_reward() -> int:
         return BLOCK_REWARD
 
     @staticmethod
     def get_uncle_reward(block_number: int, uncle: BlockHeaderAPI) -> int:
-        return BLOCK_REWARD * (
-            UNCLE_DEPTH_PENALTY_FACTOR + uncle.block_number - block_number
-        ) // UNCLE_DEPTH_PENALTY_FACTOR
+        return (
+            BLOCK_REWARD
+            * (UNCLE_DEPTH_PENALTY_FACTOR + uncle.block_number - block_number)
+            // UNCLE_DEPTH_PENALTY_FACTOR
+        )
 
     @classmethod
     def get_nephew_reward(cls) -> int:
         return cls.get_block_reward() // 32
 
-    def add_receipt_to_header(self,
-                              old_header: BlockHeaderAPI,
-                              receipt: ReceiptAPI) -> BlockHeaderAPI:
+    def add_receipt_to_header(
+        self, old_header: BlockHeaderAPI, receipt: ReceiptAPI
+    ) -> BlockHeaderAPI:
         return old_header.copy(
             bloom=int(BloomFilter(old_header.bloom) | receipt.bloom),
             gas_used=receipt.gas_used,
             state_root=self.state.make_state_root(),
         )
 
     @classmethod
     def calculate_net_gas_refund(cls, consumed_gas: int, gross_refund: int) -> int:
         max_refund = consumed_gas // MAX_REFUND_QUOTIENT
         return min(max_refund, gross_refund)
 
     @classmethod
-    def finalize_gas_used(cls,
-                          transaction: SignedTransactionAPI,
-                          computation: ComputationAPI) -> int:
-
+    def finalize_gas_used(
+        cls, transaction: SignedTransactionAPI, computation: ComputationAPI
+    ) -> int:
         gas_remaining = computation.get_gas_remaining()
         consumed_gas = transaction.gas - gas_remaining
 
         gross_refund = computation.get_gas_refund()
         net_refund = cls.calculate_net_gas_refund(consumed_gas, gross_refund)
 
         return consumed_gas - net_refund
 
     @classmethod
     def make_receipt(
-            cls,
-            base_header: BlockHeaderAPI,
-            transaction: SignedTransactionAPI,
-            computation: ComputationAPI,
-            state: StateAPI) -> ReceiptAPI:
-
-        gas_used = base_header.gas_used + cls.finalize_gas_used(transaction, computation)
+        cls,
+        base_header: BlockHeaderAPI,
+        transaction: SignedTransactionAPI,
+        computation: ComputationAPI,
+        state: StateAPI,
+    ) -> ReceiptAPI:
+        gas_used = base_header.gas_used + cls.finalize_gas_used(
+            transaction, computation
+        )
 
         receipt_without_state_root = make_frontier_receipt(computation, gas_used)
 
-        return receipt_without_state_root.copy(
-            state_root=state.make_state_root()
-        )
+        return receipt_without_state_root.copy(state_root=state.make_state_root())
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/frontier/blocks.py` & `py-evm-0.7.0a2/eth/vm/forks/frontier/blocks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from typing import (
     Sequence,
     Tuple,
     Type,
 )
 
-from rlp.sedes import (
-    CountableList,
-)
-
 from eth_bloom import (
     BloomFilter,
 )
-
 from eth_typing import (
     BlockNumber,
     Hash32,
 )
-
+from rlp.sedes import (
+    CountableList,
+)
 from trie.exceptions import (
     MissingTrieNode,
 )
 
 from eth.abc import (
     BlockHeaderAPI,
     ChainDatabaseAPI,
@@ -51,25 +48,27 @@
 )
 
 
 class FrontierBlock(BaseBlock):
     transaction_builder = FrontierTransaction
     receipt_builder = Receipt
     fields = [
-        ('header', BlockHeader),
-        ('transactions', CountableList(transaction_builder)),
-        ('uncles', CountableList(BlockHeader))
+        ("header", BlockHeader),
+        ("transactions", CountableList(transaction_builder)),
+        ("uncles", CountableList(BlockHeader)),
     ]
 
     bloom_filter = None
 
-    def __init__(self,
-                 header: BlockHeaderAPI,
-                 transactions: Sequence[SignedTransactionAPI] = None,
-                 uncles: Sequence[BlockHeaderAPI] = None) -> None:
+    def __init__(
+        self,
+        header: BlockHeaderAPI,
+        transactions: Sequence[SignedTransactionAPI] = None,
+        uncles: Sequence[BlockHeaderAPI] = None,
+    ) -> None:
         if transactions is None:
             transactions = []
         if uncles is None:
             uncles = []
 
         self.bloom_filter = BloomFilter(header.bloom)
 
@@ -108,31 +107,39 @@
     def get_receipts(self, chaindb: ChainDatabaseAPI) -> Tuple[ReceiptAPI, ...]:
         return chaindb.get_receipts(self.header, self.get_receipt_builder())
 
     #
     # Header API
     #
     @classmethod
-    def from_header(cls, header: BlockHeaderAPI, chaindb: ChainDatabaseAPI) -> "FrontierBlock":
+    def from_header(
+        cls, header: BlockHeaderAPI, chaindb: ChainDatabaseAPI
+    ) -> "FrontierBlock":
         """
         Returns the block denoted by the given block header.
 
-        :raise eth.exceptions.BlockNotFound: if transactions or uncle headers are missing
+        :raise eth.exceptions.BlockNotFound: if transactions or uncle headers missing
         """
         if header.uncles_hash == EMPTY_UNCLE_HASH:
             uncles: Tuple[BlockHeaderAPI, ...] = ()
         else:
             try:
                 uncles = chaindb.get_block_uncles(header.uncles_hash)
             except HeaderNotFound as exc:
-                raise BlockNotFound(f"Uncles not found in database for {header}: {exc}") from exc
+                raise BlockNotFound(
+                    f"Uncles not found in database for {header}: {exc}"
+                ) from exc
 
         try:
-            transactions = chaindb.get_block_transactions(header, cls.get_transaction_builder())
+            transactions = chaindb.get_block_transactions(
+                header, cls.get_transaction_builder()
+            )
         except MissingTrieNode as exc:
-            raise BlockNotFound(f"Transactions not found in database for {header}: {exc}") from exc
+            raise BlockNotFound(
+                f"Transactions not found in database for {header}: {exc}"
+            ) from exc
 
         return cls(
             header=header,
             transactions=transactions,
             uncles=uncles,
         )
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/frontier/computation.py` & `py-evm-0.7.0a2/eth/vm/forks/frontier/computation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,68 @@
-from eth import precompiles
-
-from eth_hash.auto import keccak
+from eth_hash.auto import (
+    keccak,
+)
 from eth_utils import (
     encode_hex,
 )
 
-from eth.constants import (
-    GAS_CODEDEPOSIT,
-    STACK_DEPTH_LIMIT,
+from eth import (
+    precompiles,
 )
-
 from eth._utils.address import (
     force_bytes_to_address,
 )
 from eth.abc import (
     ComputationAPI,
     MessageAPI,
     StateAPI,
     TransactionContextAPI,
 )
+from eth.constants import (
+    GAS_CODEDEPOSIT,
+    STACK_DEPTH_LIMIT,
+)
 from eth.exceptions import (
-    OutOfGas,
     InsufficientFunds,
+    OutOfGas,
     StackDepthLimit,
 )
 from eth.vm.computation import (
     BaseComputation,
 )
 
-from .opcodes import FRONTIER_OPCODES
-
+from .opcodes import (
+    FRONTIER_OPCODES,
+)
 
 FRONTIER_PRECOMPILES = {
-    force_bytes_to_address(b'\x01'): precompiles.ecrecover,
-    force_bytes_to_address(b'\x02'): precompiles.sha256,
-    force_bytes_to_address(b'\x03'): precompiles.ripemd160,
-    force_bytes_to_address(b'\x04'): precompiles.identity,
+    force_bytes_to_address(b"\x01"): precompiles.ecrecover,
+    force_bytes_to_address(b"\x02"): precompiles.sha256,
+    force_bytes_to_address(b"\x03"): precompiles.ripemd160,
+    force_bytes_to_address(b"\x04"): precompiles.identity,
 }
 
 
 class FrontierComputation(BaseComputation):
     """
-    A class for all execution computations in the ``Frontier`` fork.
+    A class for all execution message computations in the ``Frontier`` fork.
     Inherits from :class:`~eth.vm.computation.BaseComputation`
     """
+
     # Override
     opcodes = FRONTIER_OPCODES
-    _precompiles = FRONTIER_PRECOMPILES     # type: ignore # https://github.com/python/mypy/issues/708 # noqa: E501
+    _precompiles = FRONTIER_PRECOMPILES  # type: ignore # https://github.com/python/mypy/issues/708 # noqa: E501
 
     @classmethod
     def apply_message(
         cls,
         state: StateAPI,
         message: MessageAPI,
         transaction_context: TransactionContextAPI,
     ) -> ComputationAPI:
-
         snapshot = state.snapshot()
 
         if message.depth > STACK_DEPTH_LIMIT:
             raise StackDepthLimit("Stack depth limit reached")
 
         if message.should_transfer_value and message.value:
             sender_balance = state.get_balance(message.sender)
@@ -92,19 +95,19 @@
         else:
             state.commit(snapshot)
 
         return computation
 
     @classmethod
     def apply_create_message(
-            cls,
-            state: StateAPI,
-            message: MessageAPI,
-            transaction_context: TransactionContextAPI) -> ComputationAPI:
-
+        cls,
+        state: StateAPI,
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI,
+    ) -> ComputationAPI:
         computation = cls.apply_message(state, message, transaction_context)
 
         if computation.is_error:
             return computation
         else:
             contract_code = computation.output
 
@@ -112,17 +115,17 @@
                 contract_code_gas_fee = len(contract_code) * GAS_CODEDEPOSIT
                 try:
                     computation.consume_gas(
                         contract_code_gas_fee,
                         reason="Write contract code for CREATE",
                     )
                 except OutOfGas:
-                    computation.output = b''
+                    computation.output = b""
                 else:
                     cls.logger.debug2(
                         "SETTING CODE: %s -> length: %s | hash: %s",
                         encode_hex(message.storage_address),
                         len(contract_code),
-                        encode_hex(keccak(contract_code))
+                        encode_hex(keccak(contract_code)),
                     )
                     state.set_code(message.storage_address, contract_code)
             return computation
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/frontier/headers.py` & `py-evm-0.7.0a2/eth/vm/forks/frontier/headers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 from typing import (
-    Any,
     TYPE_CHECKING,
+    Any,
 )
 
-from eth.abc import BlockHeaderAPI
-from eth.validation import (
-    validate_gt,
-    validate_header_params_for_configuration,
-)
-
-from eth.constants import (
-    GENESIS_GAS_LIMIT,
-    DIFFICULTY_ADJUSTMENT_DENOMINATOR,
-    DIFFICULTY_MINIMUM,
-    BOMB_EXPONENTIAL_PERIOD,
-    BOMB_EXPONENTIAL_FREE_PERIODS,
-)
 from eth._utils.db import (
     get_parent_header,
 )
 from eth._utils.headers import (
     compute_gas_limit,
     fill_header_params_from_parent,
     new_timestamp_from_parent,
 )
-from eth.rlp.headers import BlockHeader
+from eth.abc import (
+    BlockHeaderAPI,
+)
+from eth.constants import (
+    BOMB_EXPONENTIAL_FREE_PERIODS,
+    BOMB_EXPONENTIAL_PERIOD,
+    DIFFICULTY_ADJUSTMENT_DENOMINATOR,
+    DIFFICULTY_MINIMUM,
+    GENESIS_GAS_LIMIT,
+)
+from eth.rlp.headers import (
+    BlockHeader,
+)
+from eth.validation import (
+    validate_gt,
+    validate_header_params_for_configuration,
+)
 
 from .constants import (
-    FRONTIER_DIFFICULTY_ADJUSTMENT_CUTOFF
+    FRONTIER_DIFFICULTY_ADJUSTMENT_CUTOFF,
 )
 
 if TYPE_CHECKING:
-    from eth.vm.forks.frontier import FrontierVM    # noqa: F401
+    from eth.vm.forks.frontier import FrontierVM  # noqa: F401
 
 
 def compute_frontier_difficulty(parent_header: BlockHeaderAPI, timestamp: int) -> int:
     """
     Computes the difficulty for a frontier block based on the parent block.
     """
     validate_gt(timestamp, parent_header.timestamp, title="Header timestamp")
@@ -70,42 +73,43 @@
         )
     else:
         difficulty = base_difficulty
 
     return difficulty
 
 
-def create_frontier_header_from_parent(parent_header: BlockHeaderAPI,
-                                       **header_params: Any) -> BlockHeader:
-    if 'timestamp' not in header_params:
-        header_params['timestamp'] = new_timestamp_from_parent(parent_header)
-
-    if 'difficulty' not in header_params:
-        # Use setdefault to ensure the new header has the same timestamp we use to calculate its
-        # difficulty.
-        header_params['difficulty'] = compute_frontier_difficulty(
+def create_frontier_header_from_parent(
+    parent_header: BlockHeaderAPI, **header_params: Any
+) -> BlockHeader:
+    if "timestamp" not in header_params:
+        header_params["timestamp"] = new_timestamp_from_parent(parent_header)
+
+    if "difficulty" not in header_params:
+        # Use setdefault to ensure the new header has the same timestamp we use to
+        # calculate its difficulty.
+        header_params["difficulty"] = compute_frontier_difficulty(
             parent_header,
-            header_params['timestamp'],
+            header_params["timestamp"],
         )
-    if 'gas_limit' not in header_params:
-        header_params['gas_limit'] = compute_gas_limit(
+    if "gas_limit" not in header_params:
+        header_params["gas_limit"] = compute_gas_limit(
             parent_header,
             genesis_gas_limit=GENESIS_GAS_LIMIT,
         )
 
     all_fields = fill_header_params_from_parent(parent_header, **header_params)
     return BlockHeader(**all_fields)
 
 
 def configure_frontier_header(vm: "FrontierVM", **header_params: Any) -> BlockHeader:
     validate_header_params_for_configuration(header_params)
 
     with vm.get_header().build_changeset(**header_params) as changeset:
-        if 'timestamp' in header_params and vm.get_header().block_number > 0:
+        if "timestamp" in header_params and vm.get_header().block_number > 0:
             parent_header = get_parent_header(changeset.build_rlp(), vm.chaindb)
             changeset.difficulty = compute_frontier_difficulty(
                 parent_header,
-                header_params['timestamp'],
+                header_params["timestamp"],
             )
 
         header = changeset.commit()
     return header
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/frontier/opcodes.py` & `py-evm-0.7.0a2/eth/vm/forks/frontier/opcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-from typing import Dict
-
-from eth import constants
+from typing import (
+    Dict,
+)
 
-from eth.abc import OpcodeAPI
-from eth.vm import mnemonics
-from eth.vm import opcode_values
+from eth import (
+    constants,
+)
+from eth.abc import (
+    OpcodeAPI,
+)
+from eth.vm import (
+    mnemonics,
+    opcode_values,
+)
 from eth.vm.logic import (
     arithmetic,
     block,
     call,
     comparison,
     context,
     duplication,
@@ -21,15 +28,14 @@
     swap,
     system,
 )
 from eth.vm.opcode import (
     as_opcode,
 )
 
-
 FRONTIER_OPCODES: Dict[int, OpcodeAPI] = {
     #
     # Arithmetic
     #
     opcode_values.STOP: as_opcode(
         logic_fn=flow.stop,
         mnemonic=mnemonics.STOP,
@@ -677,25 +683,25 @@
         mnemonic=mnemonics.LOG4,
         gas_cost=constants.GAS_LOG,
     ),
     #
     # System
     #
     opcode_values.CREATE: system.Create.configure(
-        __name__='opcode:CREATE',
+        __name__="opcode:CREATE",
         mnemonic=mnemonics.CREATE,
         gas_cost=constants.GAS_CREATE,
     )(),
     opcode_values.CALL: call.Call.configure(
-        __name__='opcode:CALL',
+        __name__="opcode:CALL",
         mnemonic=mnemonics.CALL,
         gas_cost=constants.GAS_CALL,
     )(),
     opcode_values.CALLCODE: call.CallCode.configure(
-        __name__='opcode:CALLCODE',
+        __name__="opcode:CALLCODE",
         mnemonic=mnemonics.CALLCODE,
         gas_cost=constants.GAS_CALL,
     )(),
     opcode_values.RETURN: as_opcode(
         logic_fn=system.return_op,
         mnemonic=mnemonics.RETURN,
         gas_cost=constants.GAS_ZERO,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/frontier/state.py` & `py-evm-0.7.0a2/eth/vm/forks/frontier/state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,74 @@
-from typing import Type
+from typing import (
+    Type,
+)
 
-from eth_hash.auto import keccak
+from eth_hash.auto import (
+    keccak,
+)
 from eth_utils import (
     encode_hex,
 )
 
+from eth._utils.address import (
+    generate_contract_address,
+)
 from eth.abc import (
     AccountDatabaseAPI,
     ComputationAPI,
-    SignedTransactionAPI,
     MessageAPI,
+    SignedTransactionAPI,
     TransactionContextAPI,
     TransactionExecutorAPI,
 )
-from eth.constants import CREATE_CONTRACT_ADDRESS
+from eth.constants import (
+    CREATE_CONTRACT_ADDRESS,
+)
 from eth.db.account import (
     AccountDB,
 )
 from eth.exceptions import (
     ContractCreationCollision,
 )
-
-from eth._utils.address import (
-    generate_contract_address,
-)
-
 from eth.vm.message import (
     Message,
 )
 from eth.vm.state import (
     BaseState,
     BaseTransactionExecutor,
 )
 
-
-from .computation import FrontierComputation
+from .computation import (
+    FrontierComputation,
+)
 from .constants import (
-    REFUND_SELFDESTRUCT,
     MAX_REFUND_QUOTIENT,
+    REFUND_SELFDESTRUCT,
 )
 from .transaction_context import (
-    FrontierTransactionContext
+    FrontierTransactionContext,
+)
+from .validation import (
+    validate_frontier_transaction,
 )
-from .validation import validate_frontier_transaction
 
 
 class FrontierTransactionExecutor(BaseTransactionExecutor):
     def validate_transaction(self, transaction: SignedTransactionAPI) -> None:
-
         # Validate the transaction
         transaction.validate()
         self.vm_state.validate_transaction(transaction)
 
     def build_evm_message(self, transaction: SignedTransactionAPI) -> MessageAPI:
         # Use vm_state.get_gas_price instead of transaction_context.gas_price so
         #   that we can run get_transaction_result (aka~ eth_call) and estimate_gas.
         #   Both work better if the GASPRICE opcode returns the original real price,
-        #   but the sender's balance doesn't actually deduct the gas. This get_gas_price()
-        #   will return 0 for eth_call, but transaction_context.gas_price will return
+        #   but the sender's balance doesn't actually deduct the gas. This
+        #   get_gas_price() will return 0 for eth_call, but
+        #   transaction_context.gas_price will return
         #   the same value as the GASPRICE opcode.
         gas_fee = transaction.gas * self.vm_state.get_gas_price(transaction)
 
         # Buy Gas
         self.vm_state.delta_balance(transaction.sender, -1 * gas_fee)
 
         # Increment Nonce
@@ -71,15 +78,15 @@
         message_gas = transaction.gas - transaction.intrinsic_gas
 
         if transaction.to == CREATE_CONTRACT_ADDRESS:
             contract_address = generate_contract_address(
                 transaction.sender,
                 self.vm_state.get_nonce(transaction.sender) - 1,
             )
-            data = b''
+            data = b""
             code = transaction.data
         else:
             contract_address = None
             data = transaction.data
             code = self.vm_state.get_code(transaction.to)
 
         self.vm_state.logger.debug2(
@@ -105,27 +112,27 @@
             value=transaction.value,
             data=data,
             code=code,
             create_address=contract_address,
         )
         return message
 
-    def build_computation(self,
-                          message: MessageAPI,
-                          transaction: SignedTransactionAPI) -> ComputationAPI:
+    def build_computation(
+        self, message: MessageAPI, transaction: SignedTransactionAPI
+    ) -> ComputationAPI:
         transaction_context = self.vm_state.get_transaction_context(transaction)
         if message.is_create:
-            is_collision = self.vm_state.has_code_or_nonce(
-                message.storage_address
-            )
+            is_collision = self.vm_state.has_code_or_nonce(message.storage_address)
 
             if is_collision:
                 # The address of the newly created contract has *somehow* collided
                 # with an existing contract address.
-                computation = self.vm_state.get_computation(message, transaction_context)
+                computation = self.vm_state.get_computation(
+                    message, transaction_context
+                )
                 computation.error = ContractCreationCollision(
                     f"Address collision while creating contract: "
                     f"{encode_hex(message.storage_address)}"
                 )
                 self.vm_state.logger.debug2(
                     "Address collision while creating contract: %s",
                     encode_hex(message.storage_address),
@@ -142,42 +149,38 @@
                 message,
                 transaction_context,
             )
 
         return computation
 
     @classmethod
-    def calculate_gas_refund(cls,
-                             computation: ComputationAPI,
-                             gas_used: int) -> int:
+    def calculate_gas_refund(cls, computation: ComputationAPI, gas_used: int) -> int:
         # Self Destruct Refunds
         num_deletions = len(computation.get_accounts_for_deletion())
         if num_deletions:
             computation.refund_gas(REFUND_SELFDESTRUCT * num_deletions)
 
         # Gas Refunds
         gas_refunded = computation.get_gas_refund()
 
         return min(gas_refunded, gas_used // MAX_REFUND_QUOTIENT)
 
     def finalize_computation(
-        self,
-        transaction: SignedTransactionAPI,
-        computation: ComputationAPI
+        self, transaction: SignedTransactionAPI, computation: ComputationAPI
     ) -> ComputationAPI:
         transaction_context = self.vm_state.get_transaction_context(transaction)
 
         gas_remaining = computation.get_gas_remaining()
         gas_used = transaction.gas - gas_remaining
         gas_refund = self.calculate_gas_refund(computation, gas_used)
         gas_refund_amount = (gas_refund + gas_remaining) * transaction_context.gas_price
 
         if gas_refund_amount:
             self.vm_state.logger.debug2(
-                'TRANSACTION REFUND: %s -> %s',
+                "TRANSACTION REFUND: %s -> %s",
                 gas_refund_amount,
                 encode_hex(computation.msg.sender),
             )
             self.vm_state.delta_balance(computation.msg.sender, gas_refund_amount)
 
         # Beneficiary Fees
         gas_used = transaction.gas - gas_remaining - gas_refund
@@ -185,33 +188,35 @@
 
         # EIP-161:
         # Even if the txn fee is zero, the coinbase is still touched here. Post-merge,
         # with no block reward, in the cases where the txn fee is also zero, the
         # coinbase may end up zeroed after the computation and thus should be marked
         # for deletion since it was touched.
         self.vm_state.logger.debug2(
-            'TRANSACTION FEE: %s -> %s',
+            "TRANSACTION FEE: %s -> %s",
             transaction_fee,
             encode_hex(self.vm_state.coinbase),
         )
         self.vm_state.delta_balance(self.vm_state.coinbase, transaction_fee)
 
         # Process Self Destructs
         for account, _ in computation.get_accounts_for_deletion():
-            self.vm_state.logger.debug2('DELETING ACCOUNT: %s', encode_hex(account))
+            self.vm_state.logger.debug2("DELETING ACCOUNT: %s", encode_hex(account))
             self.vm_state.delete_account(account)
 
         return computation
 
 
 class FrontierState(BaseState):
     computation_class: Type[ComputationAPI] = FrontierComputation
     transaction_context_class: Type[TransactionContextAPI] = FrontierTransactionContext
     account_db_class: Type[AccountDatabaseAPI] = AccountDB
-    transaction_executor_class: Type[TransactionExecutorAPI] = FrontierTransactionExecutor
+    transaction_executor_class: Type[
+        TransactionExecutorAPI
+    ] = FrontierTransactionExecutor
 
     def apply_transaction(self, transaction: SignedTransactionAPI) -> ComputationAPI:
         executor = self.get_transaction_executor()
         return executor(transaction)
 
     def validate_transaction(self, transaction: SignedTransactionAPI) -> None:
         validate_frontier_transaction(self, transaction)
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/frontier/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/frontier/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,68 +1,72 @@
-from functools import partial
+from functools import (
+    partial,
+)
 from typing import (
     Tuple,
 )
 
-from eth_keys.datatypes import PrivateKey
+from eth_keys.datatypes import (
+    PrivateKey,
+)
 from eth_typing import (
     Address,
 )
 import rlp
 
+from eth._utils.transactions import (
+    V_OFFSET,
+    IntrinsicGasSchedule,
+    calculate_intrinsic_gas,
+    create_transaction_signature,
+    extract_transaction_sender,
+    validate_transaction_signature,
+)
 from eth.abc import (
     ReceiptAPI,
     SignedTransactionAPI,
 )
 from eth.constants import (
     CREATE_CONTRACT_ADDRESS,
     GAS_TX,
-    GAS_TXDATAZERO,
     GAS_TXDATANONZERO,
+    GAS_TXDATAZERO,
 )
-from eth.validation import (
-    validate_uint256,
-    validate_is_integer,
-    validate_is_bytes,
-    validate_lt_secpk1n,
-    validate_lte,
-    validate_gte,
-    validate_canonical_address,
+from eth.rlp.logs import (
+    Log,
+)
+from eth.rlp.receipts import (
+    Receipt,
 )
-
-from eth.rlp.logs import Log
-from eth.rlp.receipts import Receipt
 from eth.rlp.transactions import (
     BaseTransaction,
     BaseUnsignedTransaction,
 )
-
-from eth._utils.transactions import (
-    V_OFFSET,
-    create_transaction_signature,
-    extract_transaction_sender,
-    validate_transaction_signature,
-    IntrinsicGasSchedule,
-    calculate_intrinsic_gas,
+from eth.validation import (
+    validate_canonical_address,
+    validate_gte,
+    validate_is_bytes,
+    validate_is_integer,
+    validate_lt_secpk1n,
+    validate_lte,
+    validate_uint256,
 )
 
-
 FRONTIER_TX_GAS_SCHEDULE = IntrinsicGasSchedule(
     gas_tx=GAS_TX,
     gas_txcreate=0,
     gas_txdatazero=GAS_TXDATAZERO,
     gas_txdatanonzero=GAS_TXDATANONZERO,
 )
 
 
 frontier_get_intrinsic_gas = partial(calculate_intrinsic_gas, FRONTIER_TX_GAS_SCHEDULE)
 
 
 class FrontierTransaction(BaseTransaction):
-
     @property
     def y_parity(self) -> int:
         return self.v - V_OFFSET
 
     @property
     def v_min(self) -> int:
         return V_OFFSET
@@ -100,61 +104,63 @@
     def get_sender(self) -> Address:
         return extract_transaction_sender(self)
 
     def get_intrinsic_gas(self) -> int:
         return frontier_get_intrinsic_gas(self)
 
     def get_message_for_signing(self) -> bytes:
-        return rlp.encode(FrontierUnsignedTransaction(
-            nonce=self.nonce,
-            gas_price=self.gas_price,
-            gas=self.gas,
-            to=self.to,
-            value=self.value,
-            data=self.data,
-        ))
+        return rlp.encode(
+            FrontierUnsignedTransaction(
+                nonce=self.nonce,
+                gas_price=self.gas_price,
+                gas=self.gas,
+                to=self.to,
+                value=self.value,
+                data=self.data,
+            )
+        )
 
     @classmethod
-    def create_unsigned_transaction(cls,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> 'FrontierUnsignedTransaction':
+    def create_unsigned_transaction(
+        cls,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes
+    ) -> "FrontierUnsignedTransaction":
         return FrontierUnsignedTransaction(nonce, gas_price, gas, to, value, data)
 
     @classmethod
     def new_transaction(
-            cls,
-            nonce: int,
-            gas_price: int,
-            gas: int,
-            to: Address,
-            value: int,
-            data: bytes,
-            v: int,
-            r: int,
-            s: int) -> SignedTransactionAPI:
+        cls,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+        v: int,
+        r: int,
+        s: int,
+    ) -> SignedTransactionAPI:
         return cls(nonce, gas_price, gas, to, value, data, v, r, s)
 
     def make_receipt(
-            self,
-            status: bytes,
-            gas_used: int,
-            log_entries: Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...]) -> ReceiptAPI:
+        self,
+        status: bytes,
+        gas_used: int,
+        log_entries: Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...],
+    ) -> ReceiptAPI:
         # 'status' is a misnomer in Frontier. Until Byzantium, it is the
         # intermediate state root.
 
-        logs = [
-            Log(address, topics, data)
-            for address, topics, data
-            in log_entries
-        ]
+        logs = [Log(address, topics, data) for address, topics, data in log_entries]
 
         return Receipt(
             state_root=status,
             gas_used=gas_used,
             logs=logs,
         )
 
@@ -165,15 +171,14 @@
 
     @property
     def max_fee_per_gas(self) -> int:
         return self.gas_price
 
 
 class FrontierUnsignedTransaction(BaseUnsignedTransaction):
-
     def validate(self) -> None:
         validate_uint256(self.nonce, title="Transaction.nonce")
         validate_is_integer(self.gas_price, title="Transaction.gas_price")
         validate_uint256(self.gas, title="Transaction.gas")
         if self.to != CREATE_CONTRACT_ADDRESS:
             validate_canonical_address(self.to, title="Transaction.to")
         validate_uint256(self.value, title="Transaction.value")
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/frontier/validation.py` & `py-evm-0.7.0a2/eth/vm/forks/frontier/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,17 @@
     BlockHeaderAPI,
     SignedTransactionAPI,
     StateAPI,
     VirtualMachineAPI,
 )
 
 
-def validate_frontier_transaction(state: StateAPI,
-                                  transaction: SignedTransactionAPI) -> None:
+def validate_frontier_transaction(
+    state: StateAPI, transaction: SignedTransactionAPI
+) -> None:
     max_gas_cost = transaction.gas * state.get_gas_price(transaction)
     sender_balance = state.get_balance(transaction.sender)
 
     if sender_balance < max_gas_cost:
         raise ValidationError(
             f"Sender {transaction.sender!r} cannot afford txn gas "
             f"{max_gas_cost} with account balance {sender_balance}"
@@ -28,20 +29,23 @@
             f"Sender does not have enough balance to cover transaction value and gas "
             f" (has {sender_balance}, needs {total_cost})"
         )
 
     sender_nonce = state.get_nonce(transaction.sender)
     if sender_nonce != transaction.nonce:
         raise ValidationError(
-            f"Invalid transaction nonce: Expected {sender_nonce}, but got {transaction.nonce}"
+            f"Invalid transaction nonce: Expected {sender_nonce}, "
+            f"but got {transaction.nonce}"
         )
 
 
-def validate_frontier_transaction_against_header(_vm: VirtualMachineAPI,
-                                                 base_header: BlockHeaderAPI,
-                                                 transaction: SignedTransactionAPI) -> None:
+def validate_frontier_transaction_against_header(
+    _vm: VirtualMachineAPI,
+    base_header: BlockHeaderAPI,
+    transaction: SignedTransactionAPI,
+) -> None:
     if base_header.gas_used + transaction.gas > base_header.gas_limit:
         raise ValidationError(
             f"Transaction exceeds gas limit: using {transaction.gas}, "
             f"bringing total to {base_header.gas_used + transaction.gas}, "
             f"but limit is {base_header.gas_limit}"
         )
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/gray_glacier/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/gray_glacier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 )
 from .state import GrayGlacierState
 from .. import ArrowGlacierVM
 
 
 class GrayGlacierVM(ArrowGlacierVM):
     # fork name
-    fork = 'gray-glacier'
+    fork = "gray-glacier"
 
     # classes
     block_class: Type[BaseBlock] = GrayGlacierBlock
     _state_class: Type[BaseState] = GrayGlacierState
 
     # Methods
     create_header_from_parent = staticmethod(  # type: ignore
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/gray_glacier/blocks.py` & `py-evm-0.7.0a2/eth/vm/forks/paris/blocks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,48 @@
-from abc import ABC
-from typing import Type
+from abc import (
+    ABC,
+)
+from typing import (
+    Type,
+)
 
-from eth.abc import TransactionBuilderAPI
 from eth_utils import (
     encode_hex,
 )
-
 from rlp.sedes import (
     CountableList,
 )
 
-from .transactions import (
-    GrayGlacierTransactionBuilder,
+from eth.abc import (
+    TransactionBuilderAPI,
 )
-from ..arrow_glacier import (
-    ArrowGlacierBlock,
+from eth.vm.forks.gray_glacier.blocks import (
+    GrayGlacierBlock,
+    GrayGlacierBlockHeader,
+    GrayGlacierMiningHeader,
 )
-from ..arrow_glacier.blocks import (
-    ArrowGlacierBlockHeader,
-    ArrowGlacierMiningHeader,
+
+from ..london.blocks import (
+    LondonBackwardsHeader,
+)
+from .transactions import (
+    ParisTransactionBuilder,
 )
-from ..london.blocks import LondonBackwardsHeader
 
 
-class GrayGlacierMiningHeader(ArrowGlacierMiningHeader, ABC):
+class ParisMiningHeader(GrayGlacierMiningHeader, ABC):
     pass
 
 
-class GrayGlacierBlockHeader(ArrowGlacierBlockHeader, ABC):
+class ParisBlockHeader(GrayGlacierBlockHeader, ABC):
     def __str__(self) -> str:
-        return f'<GrayGlacierBlockHeader #{self.block_number} {encode_hex(self.hash)[2:10]}>'
+        return f"<ParisBlockHeader #{self.block_number} {encode_hex(self.hash)[2:10]}>"
 
 
-class GrayGlacierBlock(ArrowGlacierBlock):
-    transaction_builder: Type[TransactionBuilderAPI] = GrayGlacierTransactionBuilder
+class ParisBlock(GrayGlacierBlock):
+    transaction_builder: Type[TransactionBuilderAPI] = ParisTransactionBuilder
     fields = [
-        ('header', GrayGlacierBlockHeader),
-        ('transactions', CountableList(transaction_builder)),
-        ('uncles', CountableList(LondonBackwardsHeader))
+        ("header", ParisBlockHeader),
+        ("transactions", CountableList(transaction_builder)),
+        # no uncles in pos, max_length=0
+        ("uncles", CountableList(LondonBackwardsHeader, max_length=0)),
     ]
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/gray_glacier/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/gray_glacier/transactions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-from abc import ABC
+from abc import (
+    ABC,
+)
 
-from eth_keys.datatypes import PrivateKey
+from eth_keys.datatypes import (
+    PrivateKey,
+)
 
 from eth._utils.transactions import (
     create_transaction_signature,
 )
 from eth.vm.forks.arrow_glacier.transactions import (
     ArrowGlacierLegacyTransaction,
     ArrowGlacierTransactionBuilder,
@@ -14,17 +18,15 @@
 
 class GrayGlacierLegacyTransaction(ArrowGlacierLegacyTransaction, ABC):
     pass
 
 
 class GrayGlacierUnsignedLegacyTransaction(ArrowGlacierUnsignedLegacyTransaction):
     def as_signed_transaction(
-        self,
-        private_key: PrivateKey,
-        chain_id: int = None
+        self, private_key: PrivateKey, chain_id: int = None
     ) -> GrayGlacierLegacyTransaction:
         v, r, s = create_transaction_signature(self, private_key, chain_id=chain_id)
         return GrayGlacierLegacyTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/homestead/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/homestead/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 class MetaHomesteadVM(FrontierVM):
     support_dao_fork = True
     _dao_fork_block_number: Optional[BlockNumber] = None
 
     @classmethod
     def get_dao_fork_block_number(cls) -> BlockNumber:
         if cls._dao_fork_block_number is None:
-            raise TypeError("HomesteadVM must be configured with a valid `_dao_fork_block_number`")
+            raise TypeError(
+                "HomesteadVM must be configured with a valid `_dao_fork_block_number`"
+            )
         return cls._dao_fork_block_number
 
 
 class HomesteadVM(MetaHomesteadVM):
     # fork name
-    fork: str = 'homestead'
+    fork: str = "homestead"
 
     # classes
     block_class: Type[BlockAPI] = HomesteadBlock
     _state_class: Type[StateAPI] = HomesteadState
 
     # method overrides
-    create_header_from_parent = staticmethod(create_homestead_header_from_parent)   # type: ignore
-    compute_difficulty = staticmethod(compute_homestead_difficulty)     # type: ignore
+    create_header_from_parent = staticmethod(create_homestead_header_from_parent)  # type: ignore  # noqa: E501
+    compute_difficulty = staticmethod(compute_homestead_difficulty)  # type: ignore
     configure_header = configure_homestead_header
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/homestead/computation.py` & `py-evm-0.7.0a2/eth/vm/forks/homestead/computation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,51 @@
-from eth_hash.auto import keccak
-
-from eth import constants
-from eth.exceptions import (
-    OutOfGas,
+from eth_hash.auto import (
+    keccak,
 )
 from eth_utils import (
     encode_hex,
 )
 
+from eth import (
+    constants,
+)
 from eth.abc import (
     ComputationAPI,
     MessageAPI,
     StateAPI,
     TransactionContextAPI,
 )
+from eth.exceptions import (
+    OutOfGas,
+)
 from eth.vm.forks.frontier.computation import (
     FrontierComputation,
 )
 
-from .opcodes import HOMESTEAD_OPCODES
+from .opcodes import (
+    HOMESTEAD_OPCODES,
+)
 
 
 class HomesteadComputation(FrontierComputation):
     """
-    A class for all execution computations in the ``Frontier`` fork.
+    A class for all execution *message* computations in the ``Frontier`` fork.
     Inherits from :class:`~eth.vm.forks.frontier.computation.FrontierComputation`
     """
+
     # Override
     opcodes = HOMESTEAD_OPCODES
 
     @classmethod
     def apply_create_message(
-            cls,
-            state: StateAPI,
-            message: MessageAPI,
-            transaction_context: TransactionContextAPI) -> ComputationAPI:
+        cls,
+        state: StateAPI,
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI,
+    ) -> ComputationAPI:
         snapshot = state.snapshot()
 
         computation = cls.apply_message(state, message, transaction_context)
 
         if computation.is_error:
             state.revert(snapshot)
             return computation
@@ -59,15 +66,15 @@
                     state.revert(snapshot)
                 else:
                     if cls.logger:
                         cls.logger.debug2(
                             "SETTING CODE: %s -> length: %s | hash: %s",
                             encode_hex(message.storage_address),
                             len(contract_code),
-                            encode_hex(keccak(contract_code))
+                            encode_hex(keccak(contract_code)),
                         )
 
                     state.set_code(message.storage_address, contract_code)
                     state.commit(snapshot)
             else:
                 state.commit(snapshot)
             return computation
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/homestead/headers.py` & `py-evm-0.7.0a2/eth/vm/forks/homestead/headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,101 +1,106 @@
 from typing import (
-    Any,
     TYPE_CHECKING,
+    Any,
 )
 
 from eth_typing import (
     Address,
 )
 from eth_utils import (
     decode_hex,
 )
 
-from eth.abc import BlockHeaderAPI
+from eth._utils.db import (
+    get_parent_header,
+)
+from eth.abc import (
+    BlockHeaderAPI,
+)
 from eth.constants import (
+    BOMB_EXPONENTIAL_FREE_PERIODS,
+    BOMB_EXPONENTIAL_PERIOD,
     DIFFICULTY_ADJUSTMENT_DENOMINATOR,
     DIFFICULTY_MINIMUM,
-    BOMB_EXPONENTIAL_PERIOD,
-    BOMB_EXPONENTIAL_FREE_PERIODS,
 )
-from eth.rlp.headers import BlockHeader
-from eth._utils.db import (
-    get_parent_header,
+from eth.rlp.headers import (
+    BlockHeader,
 )
 from eth.validation import (
     validate_gt,
     validate_header_params_for_configuration,
 )
 from eth.vm.forks.frontier.headers import (
     create_frontier_header_from_parent,
 )
 
 from .constants import (
-    HOMESTEAD_DIFFICULTY_ADJUSTMENT_CUTOFF
+    HOMESTEAD_DIFFICULTY_ADJUSTMENT_CUTOFF,
 )
 
 if TYPE_CHECKING:
-    from eth.vm.forks.homestead import HomesteadVM      # noqa: F401
+    from eth.vm.forks.homestead import HomesteadVM  # noqa: F401
 
 
 def compute_homestead_difficulty(parent_header: BlockHeaderAPI, timestamp: int) -> int:
     """
     Computes the difficulty for a homestead block based on the parent block.
     """
     parent_tstamp = parent_header.timestamp
     validate_gt(timestamp, parent_tstamp, title="Header.timestamp")
     offset = parent_header.difficulty // DIFFICULTY_ADJUSTMENT_DENOMINATOR
     sign = max(
         1 - (timestamp - parent_tstamp) // HOMESTEAD_DIFFICULTY_ADJUSTMENT_CUTOFF,
         -99,
     )
-    difficulty = max(
-        parent_header.difficulty + offset * sign,
-        DIFFICULTY_MINIMUM
-    )
+    difficulty = max(parent_header.difficulty + offset * sign, DIFFICULTY_MINIMUM)
     num_bomb_periods = (
         (parent_header.block_number + 1) // BOMB_EXPONENTIAL_PERIOD
     ) - BOMB_EXPONENTIAL_FREE_PERIODS
 
     if num_bomb_periods >= 0:
         return max(difficulty + 2**num_bomb_periods, DIFFICULTY_MINIMUM)
     else:
         return difficulty
 
 
-def create_homestead_header_from_parent(parent_header: BlockHeaderAPI,
-                                        **header_params: Any) -> BlockHeader:
-    if 'difficulty' not in header_params:
-        # Use setdefault to ensure the new header has the same timestamp we use to calculate its
-        # difficulty.
-        header_params.setdefault('timestamp', parent_header.timestamp + 1)
-        header_params['difficulty'] = compute_homestead_difficulty(
+def create_homestead_header_from_parent(
+    parent_header: BlockHeaderAPI, **header_params: Any
+) -> BlockHeader:
+    if "difficulty" not in header_params:
+        # Use setdefault to ensure the new header has the same timestamp we use to
+        # calculate its difficulty.
+        header_params.setdefault("timestamp", parent_header.timestamp + 1)
+        header_params["difficulty"] = compute_homestead_difficulty(
             parent_header,
-            header_params['timestamp'],
+            header_params["timestamp"],
         )
     return create_frontier_header_from_parent(parent_header, **header_params)
 
 
 def configure_homestead_header(vm: "HomesteadVM", **header_params: Any) -> BlockHeader:
     validate_header_params_for_configuration(header_params)
 
     with vm.get_header().build_changeset(**header_params) as changeset:
-        if 'timestamp' in header_params and changeset.block_number > 0:
+        if "timestamp" in header_params and changeset.block_number > 0:
             parent_header = get_parent_header(changeset.build_rlp(), vm.chaindb)
             changeset.difficulty = compute_homestead_difficulty(
                 parent_header,
-                header_params['timestamp'],
+                header_params["timestamp"],
             )
 
         # In geth the modification of the state in the DAO fork block is performed
         # before any transactions are applied, so doing it here is the closest we
         # get to that. Another alternative would be to do it in Block.mine(), but
         # there we'd need to manually instantiate the State and update
         # header.state_root after we're done.
-        if vm.support_dao_fork and changeset.block_number == vm.get_dao_fork_block_number():
+        if (
+            vm.support_dao_fork
+            and changeset.block_number == vm.get_dao_fork_block_number()
+        ):
             state = vm.state
 
             for hex_account in dao_drain_list:
                 address = Address(decode_hex(hex_account))
                 balance = state.get_balance(address)
                 state.delta_balance(dao_refund_contract, balance)
                 state.set_balance(address, 0)
@@ -106,15 +111,15 @@
             # Update state_root manually
             changeset.state_root = state.state_root
 
         header = changeset.commit()
     return header
 
 
-dao_refund_contract = Address(decode_hex('0xbf4ed7b27f1d666546e30d74d50d173d20bca754'))
+dao_refund_contract = Address(decode_hex("0xbf4ed7b27f1d666546e30d74d50d173d20bca754"))
 dao_drain_list = [
     "0xd4fe7bc31cedb7bfb8a345f31e668033056b2728",
     "0xb3fb0e5aba0e20e5c49d252dfd30e102b171a425",
     "0x2c19c7f9ae8b751e37aeb2d93a699722395ae18f",
     "0xecd135fa4f61a655311e86238c92adcd779555d2",
     "0x1975bd06d486162d5dc297798dfc41edd5d160a7",
     "0xa3acf3a1e16b1d7c315e23510fdd7847b48234f6",
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/homestead/state.py` & `py-evm-0.7.0a2/eth/vm/forks/homestead/state.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-from typing import Type
+from typing import (
+    Type,
+)
 
 from eth.abc import (
     ComputationAPI,
     SignedTransactionAPI,
 )
 from eth.vm.forks.frontier.state import (
     FrontierState,
     FrontierTransactionExecutor,
 )
 
-from .computation import HomesteadComputation
-from .validation import validate_homestead_transaction
+from .computation import (
+    HomesteadComputation,
+)
+from .validation import (
+    validate_homestead_transaction,
+)
 
 
 class HomesteadState(FrontierState):
     computation_class: Type[ComputationAPI] = HomesteadComputation
 
     def validate_transaction(self, transaction: SignedTransactionAPI) -> None:
         validate_homestead_transaction(self, transaction)
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/homestead/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/homestead/transactions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,76 @@
-from functools import partial
+from functools import (
+    partial,
+)
 
+from eth_keys.datatypes import (
+    PrivateKey,
+)
+from eth_typing import (
+    Address,
+)
 import rlp
 
-from eth_keys.datatypes import PrivateKey
-
-from eth_typing import Address
-
-from eth.constants import GAS_TXCREATE
-
+from eth._utils.transactions import (
+    calculate_intrinsic_gas,
+    create_transaction_signature,
+)
+from eth.constants import (
+    GAS_TXCREATE,
+)
 from eth.validation import (
     validate_lt_secpk1n2,
 )
-
 from eth.vm.forks.frontier.transactions import (
+    FRONTIER_TX_GAS_SCHEDULE,
     FrontierTransaction,
     FrontierUnsignedTransaction,
-    FRONTIER_TX_GAS_SCHEDULE,
-)
-
-from eth._utils.transactions import (
-    create_transaction_signature,
-    calculate_intrinsic_gas,
 )
 
 HOMESTEAD_TX_GAS_SCHEDULE = FRONTIER_TX_GAS_SCHEDULE._replace(
     gas_txcreate=GAS_TXCREATE,
 )
 
 
-homestead_get_intrinsic_gas = partial(calculate_intrinsic_gas, HOMESTEAD_TX_GAS_SCHEDULE)
+homestead_get_intrinsic_gas = partial(
+    calculate_intrinsic_gas, HOMESTEAD_TX_GAS_SCHEDULE
+)
 
 
 class HomesteadTransaction(FrontierTransaction):
     def validate(self) -> None:
         super().validate()
         validate_lt_secpk1n2(self.s, title="Transaction.s")
 
     def get_intrinsic_gas(self) -> int:
         return homestead_get_intrinsic_gas(self)
 
     def get_message_for_signing(self) -> bytes:
-        return rlp.encode(HomesteadUnsignedTransaction(
-            nonce=self.nonce,
-            gas_price=self.gas_price,
-            gas=self.gas,
-            to=self.to,
-            value=self.value,
-            data=self.data,
-        ))
+        return rlp.encode(
+            HomesteadUnsignedTransaction(
+                nonce=self.nonce,
+                gas_price=self.gas_price,
+                gas=self.gas,
+                to=self.to,
+                value=self.value,
+                data=self.data,
+            )
+        )
 
     @classmethod
-    def create_unsigned_transaction(cls,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> 'HomesteadUnsignedTransaction':
+    def create_unsigned_transaction(
+        cls,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes
+    ) -> "HomesteadUnsignedTransaction":
         return HomesteadUnsignedTransaction(nonce, gas_price, gas, to, value, data)
 
 
 class HomesteadUnsignedTransaction(FrontierUnsignedTransaction):
     def as_signed_transaction(self, private_key: PrivateKey) -> HomesteadTransaction:
         v, r, s = create_transaction_signature(self, private_key)
         return HomesteadTransaction(
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/homestead/validation.py` & `py-evm-0.7.0a2/eth/vm/forks/homestead/validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from eth_utils import (
     ValidationError,
 )
 
-from eth.constants import (
-    SECPK1_N,
-)
-
 from eth.abc import (
     SignedTransactionAPI,
     StateAPI,
 )
+from eth.constants import (
+    SECPK1_N,
+)
 from eth.vm.forks.frontier.validation import (
     validate_frontier_transaction,
 )
 
 
-def validate_homestead_transaction(state: StateAPI,
-                                   transaction: SignedTransactionAPI) -> None:
+def validate_homestead_transaction(
+    state: StateAPI, transaction: SignedTransactionAPI
+) -> None:
     if transaction.s > SECPK1_N // 2 or transaction.s == 0:
         raise ValidationError("Invalid signature S value")
 
     validate_frontier_transaction(state, transaction)
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/istanbul/computation.py` & `py-evm-0.7.0a2/eth/vm/forks/istanbul/computation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 from eth_utils.toolz import (
     merge,
 )
 
-from eth import precompiles
+from eth import (
+    precompiles,
+)
 from eth._utils.address import (
     force_bytes_to_address,
 )
 from eth.vm.forks.petersburg.computation import (
-    PETERSBURG_PRECOMPILES
-)
-from eth.vm.forks.petersburg.computation import (
+    PETERSBURG_PRECOMPILES,
     PetersburgComputation,
 )
 from eth.vm.gas_meter import (
-    allow_negative_refund_strategy,
     GasMeter,
+    allow_negative_refund_strategy,
 )
 
 from .constants import (
     GAS_ECADD,
     GAS_ECMUL,
     GAS_ECPAIRING_BASE,
     GAS_ECPAIRING_PER_POINT,
 )
-from .opcodes import ISTANBUL_OPCODES
+from .opcodes import (
+    ISTANBUL_OPCODES,
+)
 
 ISTANBUL_PRECOMPILES = merge(
     PETERSBURG_PRECOMPILES,
     {
-        force_bytes_to_address(b'\x06'): precompiles.ecadd(gas_cost=GAS_ECADD),
-        force_bytes_to_address(b'\x07'): precompiles.ecmul(gas_cost=GAS_ECMUL),
-        force_bytes_to_address(b'\x08'): precompiles.ecpairing(
+        force_bytes_to_address(b"\x06"): precompiles.ecadd(gas_cost=GAS_ECADD),
+        force_bytes_to_address(b"\x07"): precompiles.ecmul(gas_cost=GAS_ECMUL),
+        force_bytes_to_address(b"\x08"): precompiles.ecpairing(
             gas_cost_base=GAS_ECPAIRING_BASE,
             gas_cost_per_point=GAS_ECPAIRING_PER_POINT,
         ),
-        force_bytes_to_address(b'\x09'): precompiles.blake2b_fcompress,
+        force_bytes_to_address(b"\x09"): precompiles.blake2b_fcompress,
     },
 )
 
 
 class IstanbulComputation(PetersburgComputation):
     """
-    A class for all execution computations in the ``Istanbul`` fork.
-    Inherits from :class:`~eth.vm.forks.constantinople.petersburg.PetersburgComputation`
+    A class for all execution *message* computations in the ``Istanbul`` fork.
+    Inherits from
+    :class:`~eth.vm.forks.constantinople.petersburg.PetersburgComputation`
     """
+
     # Override
     opcodes = ISTANBUL_OPCODES
     _precompiles = ISTANBUL_PRECOMPILES
 
-    def get_gas_meter(self) -> GasMeter:
-        return GasMeter(
-            self.msg.gas,
-            allow_negative_refund_strategy
-        )
+    def _configure_gas_meter(self) -> GasMeter:
+        return GasMeter(self.msg.gas, allow_negative_refund_strategy)
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/istanbul/opcodes.py` & `py-evm-0.7.0a2/eth/vm/forks/istanbul/opcodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 import copy
 
-from eth_utils.toolz import merge
+from eth_utils.toolz import (
+    merge,
+)
 
-from eth import constants
+from eth import (
+    constants,
+)
 from eth.vm import (
     mnemonics,
     opcode_values,
 )
 from eth.vm.forks.byzantium.opcodes import (
-    ensure_no_static
-)
-from eth.vm.forks.petersburg.opcodes import (
-    PETERSBURG_OPCODES,
+    ensure_no_static,
 )
 from eth.vm.forks.istanbul.constants import (
     GAS_BALANCE_EIP1884,
-    GAS_SLOAD_EIP1884,
     GAS_EXTCODEHASH_EIP1884,
+    GAS_SLOAD_EIP1884,
+)
+from eth.vm.forks.petersburg.opcodes import (
+    PETERSBURG_OPCODES,
 )
 from eth.vm.logic import (
     context,
     storage,
 )
-from eth.vm.opcode import as_opcode
+from eth.vm.opcode import (
+    as_opcode,
+)
+
 from .storage import (
     sstore_eip2200,
 )
 
-
 UPDATED_OPCODES = {
     # New opcodes
     opcode_values.CHAINID: as_opcode(
         logic_fn=context.chain_id,
         mnemonic=mnemonics.CHAINID,
         gas_cost=constants.GAS_BASE,
     ),
     opcode_values.SELFBALANCE: as_opcode(
         logic_fn=context.selfbalance,
         mnemonic=mnemonics.SELFBALANCE,
         gas_cost=constants.GAS_LOW,
     ),
-
     # Repriced opcodes
     opcode_values.SSTORE: as_opcode(
         logic_fn=ensure_no_static(sstore_eip2200),
         mnemonic=mnemonics.SSTORE,
         gas_cost=constants.GAS_NULL,
     ),
     opcode_values.BALANCE: as_opcode(
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/istanbul/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/petersburg/transactions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,47 @@
-from functools import partial
-
-from eth_keys.datatypes import PrivateKey
-from eth_typing import Address
-
-from eth.vm.forks.petersburg.transactions import (
-    PetersburgTransaction,
-    PetersburgUnsignedTransaction,
+from eth_keys.datatypes import (
+    PrivateKey,
+)
+from eth_typing import (
+    Address,
 )
 
 from eth._utils.transactions import (
     create_transaction_signature,
-    calculate_intrinsic_gas,
-)
-from eth.vm.forks.homestead.transactions import (
-    HOMESTEAD_TX_GAS_SCHEDULE,
 )
-
-from .constants import (
-    GAS_TXDATANONZERO_EIP2028,
-)
-
-ISTANBUL_TX_GAS_SCHEDULE = HOMESTEAD_TX_GAS_SCHEDULE._replace(
-    gas_txdatanonzero=GAS_TXDATANONZERO_EIP2028,
+from eth.vm.forks.byzantium.transactions import (
+    ByzantiumTransaction,
+    ByzantiumUnsignedTransaction,
 )
 
 
-istanbul_get_intrinsic_gas = partial(calculate_intrinsic_gas, ISTANBUL_TX_GAS_SCHEDULE)
-
-
-class IstanbulTransaction(PetersburgTransaction):
+class PetersburgTransaction(ByzantiumTransaction):
     @classmethod
-    def create_unsigned_transaction(cls,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> 'IstanbulUnsignedTransaction':
-        return IstanbulUnsignedTransaction(nonce, gas_price, gas, to, value, data)
-
-    def get_intrinsic_gas(self) -> int:
-        return istanbul_get_intrinsic_gas(self)
-
-
-class IstanbulUnsignedTransaction(PetersburgUnsignedTransaction):
-    def as_signed_transaction(self,
-                              private_key: PrivateKey,
-                              chain_id: int = None) -> IstanbulTransaction:
+    def create_unsigned_transaction(
+        cls,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes
+    ) -> "PetersburgUnsignedTransaction":
+        return PetersburgUnsignedTransaction(nonce, gas_price, gas, to, value, data)
+
+
+class PetersburgUnsignedTransaction(ByzantiumUnsignedTransaction):
+    def as_signed_transaction(
+        self, private_key: PrivateKey, chain_id: int = None
+    ) -> PetersburgTransaction:
         v, r, s = create_transaction_signature(self, private_key, chain_id=chain_id)
-        return IstanbulTransaction(
+        return PetersburgTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
             value=self.value,
             data=self.data,
             v=v,
             r=r,
             s=s,
         )
-
-    def get_intrinsic_gas(self) -> int:
-        return istanbul_get_intrinsic_gas(self)
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/london/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/london/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,34 +22,32 @@
     create_london_header_from_parent,
 )
 from .state import LondonState
 
 
 class LondonVM(BerlinVM):
     # fork name
-    fork = 'london'
+    fork = "london"
 
     # classes
     block_class: Type[BaseBlock] = LondonBlock
     _state_class: Type[BaseState] = LondonState
 
     # Methods
     create_header_from_parent = staticmethod(  # type: ignore
         create_london_header_from_parent(compute_london_difficulty)
     )
-    compute_difficulty = staticmethod(compute_london_difficulty)    # type: ignore
+    compute_difficulty = staticmethod(compute_london_difficulty)  # type: ignore
     configure_header = configure_london_header
 
     @classmethod
     def validate_gas(
-            cls,
-            header: BlockHeaderAPI,
-            parent_header: BlockHeaderAPI) -> None:
-
-        if hasattr(parent_header, 'base_fee_per_gas'):
+        cls, header: BlockHeaderAPI, parent_header: BlockHeaderAPI
+    ) -> None:
+        if hasattr(parent_header, "base_fee_per_gas"):
             # Follow normal gas limit rules if the previous block had a base fee
             parent_gas_limit = parent_header.gas_limit
         else:
             # On the fork block, double the gas limit.
             # That way, the gas target (which is half the London limit) equals the
             # previous (pre-London) gas limit.
             parent_gas_limit = parent_header.gas_limit * ELASTICITY_MULTIPLIER
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/london/blocks.py` & `py-evm-0.7.0a2/eth/vm/forks/london/blocks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 from typing import (
     List,
     Optional,
     Type,
     cast,
 )
 
-from eth_hash.auto import keccak
+from eth_hash.auto import (
+    keccak,
+)
 from eth_typing import (
     BlockNumber,
 )
 from eth_typing.evm import (
     Address,
-    Hash32
+    Hash32,
 )
 from eth_utils import (
     encode_hex,
 )
 import rlp
 from rlp.sedes import (
     Binary,
     CountableList,
     big_endian_int,
-    binary
+    binary,
 )
 
 from eth._utils.headers import (
     new_timestamp_from_parent,
 )
 from eth.abc import (
     BlockHeaderAPI,
     BlockHeaderSedesAPI,
     MiningHeaderAPI,
     ReceiptBuilderAPI,
     TransactionBuilderAPI,
 )
 from eth.constants import (
-    ZERO_ADDRESS,
-    ZERO_HASH32,
+    BLANK_ROOT_HASH,
     EMPTY_UNCLE_HASH,
     GENESIS_NONCE,
     GENESIS_PARENT_HASH,
-    BLANK_ROOT_HASH,
+    ZERO_ADDRESS,
+    ZERO_HASH32,
 )
 from eth.rlp.headers import (
     BlockHeader,
 )
 from eth.rlp.sedes import (
     address,
     hash32,
@@ -59,64 +61,73 @@
     LondonReceiptBuilder,
 )
 from .transactions import (
     LondonTransactionBuilder,
 )
 
 UNMINED_LONDON_HEADER_FIELDS = [
-    ('parent_hash', hash32),
-    ('uncles_hash', hash32),
-    ('coinbase', address),
-    ('state_root', trie_root),
-    ('transaction_root', trie_root),
-    ('receipt_root', trie_root),
-    ('bloom', uint256),
-    ('difficulty', big_endian_int),
-    ('block_number', big_endian_int),
-    ('gas_limit', big_endian_int),
-    ('gas_used', big_endian_int),
-    ('timestamp', big_endian_int),
-    ('extra_data', binary),
-    ('base_fee_per_gas', big_endian_int),
+    ("parent_hash", hash32),
+    ("uncles_hash", hash32),
+    ("coinbase", address),
+    ("state_root", trie_root),
+    ("transaction_root", trie_root),
+    ("receipt_root", trie_root),
+    ("bloom", uint256),
+    ("difficulty", big_endian_int),
+    ("block_number", big_endian_int),
+    ("gas_limit", big_endian_int),
+    ("gas_used", big_endian_int),
+    ("timestamp", big_endian_int),
+    ("extra_data", binary),
+    ("base_fee_per_gas", big_endian_int),
 ]
 
 
 class LondonMiningHeader(rlp.Serializable, MiningHeaderAPI):
     fields = UNMINED_LONDON_HEADER_FIELDS
 
 
 class LondonBlockHeader(rlp.Serializable, BlockHeaderAPI):
-    fields = UNMINED_LONDON_HEADER_FIELDS[:-1] + [
-        ('mix_hash', binary),
-        ('nonce', Binary(8, allow_empty=True)),
-    ] + UNMINED_LONDON_HEADER_FIELDS[-1:]
-
-    def __init__(self,
-                 difficulty: int,
-                 block_number: BlockNumber,
-                 gas_limit: int,
-                 timestamp: int = None,
-                 coinbase: Address = ZERO_ADDRESS,
-                 parent_hash: Hash32 = ZERO_HASH32,
-                 uncles_hash: Hash32 = EMPTY_UNCLE_HASH,
-                 state_root: Hash32 = BLANK_ROOT_HASH,
-                 transaction_root: Hash32 = BLANK_ROOT_HASH,
-                 receipt_root: Hash32 = BLANK_ROOT_HASH,
-                 bloom: int = 0,
-                 gas_used: int = 0,
-                 extra_data: bytes = b'',
-                 mix_hash: Hash32 = ZERO_HASH32,
-                 nonce: bytes = GENESIS_NONCE,
-                 base_fee_per_gas: int = 0) -> None:
+    fields = (
+        UNMINED_LONDON_HEADER_FIELDS[:-1]
+        + [
+            ("mix_hash", binary),
+            ("nonce", Binary(8, allow_empty=True)),
+        ]
+        + UNMINED_LONDON_HEADER_FIELDS[-1:]
+    )
+
+    def __init__(
+        self,
+        difficulty: int,
+        block_number: BlockNumber,
+        gas_limit: int,
+        timestamp: int = None,
+        coinbase: Address = ZERO_ADDRESS,
+        parent_hash: Hash32 = ZERO_HASH32,
+        uncles_hash: Hash32 = EMPTY_UNCLE_HASH,
+        state_root: Hash32 = BLANK_ROOT_HASH,
+        transaction_root: Hash32 = BLANK_ROOT_HASH,
+        receipt_root: Hash32 = BLANK_ROOT_HASH,
+        bloom: int = 0,
+        gas_used: int = 0,
+        extra_data: bytes = b"",
+        mix_hash: Hash32 = ZERO_HASH32,
+        nonce: bytes = GENESIS_NONCE,
+        base_fee_per_gas: int = 0,
+    ) -> None:
         if timestamp is None:
             if parent_hash == ZERO_HASH32:
                 timestamp = new_timestamp_from_parent(None)
             else:
-                # without access to the parent header, we cannot select a new timestamp correctly
-                raise ValueError("Must set timestamp explicitly if this is not a genesis header")
+                # without access to the parent header,
+                # we cannot select a new timestamp correctly
+                raise ValueError(
+                    "Must set timestamp explicitly if this is not a genesis header"
+                )
         super().__init__(
             parent_hash=parent_hash,
             uncles_hash=uncles_hash,
             coinbase=coinbase,
             state_root=state_root,
             transaction_root=transaction_root,
             receipt_root=receipt_root,
@@ -129,15 +140,15 @@
             extra_data=extra_data,
             mix_hash=mix_hash,
             nonce=nonce,
             base_fee_per_gas=base_fee_per_gas,
         )
 
     def __str__(self) -> str:
-        return f'<LondonBlockHeader #{self.block_number} {encode_hex(self.hash)[2:10]}>'
+        return f"<LondonBlockHeader #{self.block_number} {encode_hex(self.hash)[2:10]}>"
 
     _hash = None
 
     @property
     def hash(self) -> Hash32:
         if self._hash is None:
             self._hash = keccak(rlp.encode(self))
@@ -152,16 +163,17 @@
     @property
     def hex_hash(self) -> str:
         return encode_hex(self.hash)
 
     @property
     def is_genesis(self) -> bool:
         # if removing the block_number == 0 test, consider the validation consequences.
-        # validate_header stops trying to check the current header against a parent header.
-        # Can someone trick us into following a high difficulty header with genesis parent hash?
+        # validate_header stops trying to check the current header against
+        # a parent header. Can someone trick us into following a high difficulty header
+        # with genesis parent hash?
         return self.parent_hash == GENESIS_PARENT_HASH and self.block_number == 0
 
     @property
     def withdrawals_root(self) -> Optional[Hash32]:
         raise AttributeError("Withdrawals root not available until Shanghai fork")
 
 
@@ -190,11 +202,11 @@
             )
 
 
 class LondonBlock(BerlinBlock):
     transaction_builder: Type[TransactionBuilderAPI] = LondonTransactionBuilder
     receipt_builder: Type[ReceiptBuilderAPI] = LondonReceiptBuilder
     fields = [
-        ('header', LondonBlockHeader),
-        ('transactions', CountableList(transaction_builder)),
-        ('uncles', CountableList(LondonBackwardsHeader))
+        ("header", LondonBlockHeader),
+        ("transactions", CountableList(transaction_builder)),
+        ("uncles", CountableList(LondonBackwardsHeader)),
     ]
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/london/computation.py` & `py-evm-0.7.0a2/eth/vm/forks/london/computation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-from eth.exceptions import ReservedBytesInCode
+from eth.exceptions import (
+    ReservedBytesInCode,
+)
 from eth.vm.forks.berlin.computation import (
     BerlinComputation,
 )
 
-from .opcodes import LONDON_OPCODES
-from ..london.constants import EIP3541_RESERVED_STARTING_BYTE
+from ..london.constants import (
+    EIP3541_RESERVED_STARTING_BYTE,
+)
+from .opcodes import (
+    LONDON_OPCODES,
+)
 
 
 class LondonComputation(BerlinComputation):
     """
-    A class for all execution computations in the ``London`` fork.
+    A class for all execution *message* computations in the ``London`` fork.
     Inherits from :class:`~eth.vm.forks.berlin.BerlinComputation`
     """
+
     opcodes = LONDON_OPCODES
 
     @classmethod
     def validate_contract_code(cls, contract_code: bytes) -> None:
         super().validate_contract_code(contract_code)
 
         if contract_code[:1] == EIP3541_RESERVED_STARTING_BYTE:
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/london/headers.py` & `py-evm-0.7.0a2/eth/vm/forks/london/headers.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,36 +4,43 @@
     List,
     Optional,
 )
 
 from eth_utils import (
     ValidationError,
 )
-from toolz.functoolz import curry
+from toolz.functoolz import (
+    curry,
+)
 
 from eth._utils.headers import (
     compute_gas_limit,
     fill_header_params_from_parent,
     new_timestamp_from_parent,
 )
 from eth.abc import (
     BlockHeaderAPI,
     BlockHeaderSedesAPI,
 )
-from eth.constants import GENESIS_GAS_LIMIT
-from eth.rlp.headers import BlockHeader
+from eth.constants import (
+    GENESIS_GAS_LIMIT,
+)
+from eth.rlp.headers import (
+    BlockHeader,
+)
 from eth.vm.forks.berlin.headers import (
     configure_header,
 )
 from eth.vm.forks.muir_glacier.headers import (
     compute_difficulty,
 )
 
-
-from .blocks import LondonBlockHeader
+from .blocks import (
+    LondonBlockHeader,
+)
 from .constants import (
     BASE_FEE_MAX_CHANGE_DENOMINATOR,
     ELASTICITY_MULTIPLIER,
     INITIAL_BASE_FEE,
 )
 
 
@@ -64,69 +71,68 @@
         )
         return parent_base_fee_per_gas + base_fee_per_gas_delta
 
     else:
         gas_used_delta = parent_gas_target - parent_gas_used
         underburnt_wei = parent_base_fee_per_gas * gas_used_delta
         base_fee_per_gas_delta = (
-            underburnt_wei
-            // parent_gas_target
-            // BASE_FEE_MAX_CHANGE_DENOMINATOR
+            underburnt_wei // parent_gas_target // BASE_FEE_MAX_CHANGE_DENOMINATOR
         )
         return max(parent_base_fee_per_gas - base_fee_per_gas_delta, 0)
 
 
 @curry
 def create_london_header_from_parent(
     difficulty_fn: Callable[[BlockHeaderAPI, int], int],
     parent_header: Optional[BlockHeaderAPI],
-    **header_params: Any
+    **header_params: Any,
 ) -> BlockHeaderAPI:
-    if 'gas_limit' not in header_params:
-        if parent_header is not None and not hasattr(parent_header, 'base_fee_per_gas'):
+    if "gas_limit" not in header_params:
+        if parent_header is not None and not hasattr(parent_header, "base_fee_per_gas"):
             # If the previous block was not a London block,
             #   double the gas limit, so the new target is the old gas limit
-            header_params['gas_limit'] = parent_header.gas_limit * ELASTICITY_MULTIPLIER
+            header_params["gas_limit"] = parent_header.gas_limit * ELASTICITY_MULTIPLIER
         else:
             # frontier rules
-            header_params['gas_limit'] = compute_gas_limit(
+            header_params["gas_limit"] = compute_gas_limit(
                 parent_header,
                 genesis_gas_limit=GENESIS_GAS_LIMIT,
             )
 
     # byzantium
-    if 'timestamp' not in header_params:
-        header_params['timestamp'] = new_timestamp_from_parent(parent_header)
+    if "timestamp" not in header_params:
+        header_params["timestamp"] = new_timestamp_from_parent(parent_header)
 
-    if 'difficulty' not in header_params:
+    if "difficulty" not in header_params:
         if parent_header is None:
             raise ValueError(
                 "Must set difficulty when creating a new genesis header (no parent)."
-                " Consider 1 for easy mining or eth.constants.GENESIS_DIFFICULTY for consistency."
+                " Consider 1 for easy mining or eth.constants.GENESIS_DIFFICULTY for"
+                " consistency."
             )
         else:
-            header_params['difficulty'] = difficulty_fn(
+            header_params["difficulty"] = difficulty_fn(
                 parent_header,
-                header_params['timestamp'],
+                header_params["timestamp"],
             )
 
     # The general fill function doesn't recognize this custom field, so remove it
-    configured_fee_per_gas = header_params.pop('base_fee_per_gas', None)
+    configured_fee_per_gas = header_params.pop("base_fee_per_gas", None)
 
     all_fields = fill_header_params_from_parent(parent_header, **header_params)
 
     calculated_fee_per_gas = calculate_expected_base_fee_per_gas(parent_header)
     if configured_fee_per_gas is None:
-        all_fields['base_fee_per_gas'] = calculated_fee_per_gas
+        all_fields["base_fee_per_gas"] = calculated_fee_per_gas
     else:
         # Must not configure an invalid base fee. So verify that either:
         #   1. This is the genesis header, or
         #   2. The configured value matches the calculated value from the parent
         if parent_header is None or configured_fee_per_gas == calculated_fee_per_gas:
-            all_fields['base_fee_per_gas'] = configured_fee_per_gas
+            all_fields["base_fee_per_gas"] = configured_fee_per_gas
         else:
             raise ValidationError(
                 f"Cannot select an invalid base_fee_per_gas of:"
                 f" {configured_fee_per_gas}, expected: {calculated_fee_per_gas}"
             )
 
     new_header = LondonBlockHeader(**all_fields)  # type:ignore
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/london/opcodes.py` & `py-evm-0.7.0a2/eth/vm/forks/london/opcodes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 import copy
-from typing import Dict
+from typing import (
+    Dict,
+)
 
-from eth_utils.toolz import merge
+from eth_utils.toolz import (
+    merge,
+)
 
-from eth.vm.logic import (
-    block,
+from eth import (
+    constants,
 )
 from eth.vm import (
     mnemonics,
     opcode_values,
 )
-from eth.vm.opcode import (
-    Opcode,
-    as_opcode,
-)
-from eth import constants
-
 from eth.vm.forks.berlin.opcodes import (
     BERLIN_OPCODES,
 )
 from eth.vm.forks.byzantium.opcodes import (
     ensure_no_static,
 )
+from eth.vm.logic import (
+    block,
+)
+from eth.vm.opcode import (
+    Opcode,
+    as_opcode,
+)
 
-from . import storage
+from . import (
+    storage,
+)
 
 UPDATED_OPCODES: Dict[int, Opcode] = {
     opcode_values.BASEFEE: as_opcode(
         gas_cost=constants.GAS_BASE,
         logic_fn=block.basefee,
         mnemonic=mnemonics.BASEFEE,
     ),
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/london/receipts.py` & `py-evm-0.7.0a2/eth/vm/forks/london/receipts.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,25 @@
     Dict,
     Type,
 )
 
 from eth.rlp.receipts import (
     Receipt,
 )
+from eth.vm.forks.berlin.constants import (
+    ACCESS_LIST_TRANSACTION_TYPE,
+)
 from eth.vm.forks.berlin.receipts import (
     BerlinReceiptBuilder,
     TypedReceipt as BerlinTypedReceipt,
 )
-from eth.vm.forks.berlin.constants import (
-    ACCESS_LIST_TRANSACTION_TYPE,
-)
 
-from .constants import DYNAMIC_FEE_TRANSACTION_TYPE
+from .constants import (
+    DYNAMIC_FEE_TRANSACTION_TYPE,
+)
 
 
 class LondonTypedReceipt(BerlinTypedReceipt):
     codecs: Dict[int, Type[Receipt]] = {
         ACCESS_LIST_TRANSACTION_TYPE: Receipt,
         DYNAMIC_FEE_TRANSACTION_TYPE: Receipt,
     }
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/london/state.py` & `py-evm-0.7.0a2/eth/vm/forks/london/state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,60 @@
-from typing import Type
+from typing import (
+    Type,
+)
 
-from eth_hash.auto import keccak
+from eth_hash.auto import (
+    keccak,
+)
 from eth_utils import (
     encode_hex,
 )
 
+from eth._utils.address import (
+    generate_contract_address,
+)
 from eth.abc import (
     ComputationAPI,
     MessageAPI,
     SignedTransactionAPI,
     StateAPI,
     TransactionContextAPI,
     TransactionExecutorAPI,
 )
 from eth.constants import (
     CREATE_CONTRACT_ADDRESS,
 )
-from eth.vm.message import (
-    Message,
-)
 from eth.vm.forks.berlin.state import (
     BerlinState,
     BerlinTransactionExecutor,
 )
-from eth._utils.address import (
-    generate_contract_address,
+from eth.vm.message import (
+    Message,
 )
 
-from .computation import LondonComputation
-from .validation import validate_london_normalized_transaction
-from .constants import EIP3529_MAX_REFUND_QUOTIENT
+from .computation import (
+    LondonComputation,
+)
+from .constants import (
+    EIP3529_MAX_REFUND_QUOTIENT,
+)
+from .validation import (
+    validate_london_normalized_transaction,
+)
 
 
 class LondonTransactionExecutor(BerlinTransactionExecutor):
     def build_evm_message(self, transaction: SignedTransactionAPI) -> MessageAPI:
         # Use vm_state.get_gas_price instead of transaction_context.gas_price so
         #   that we can run get_transaction_result (aka~ eth_call) and estimate_gas.
         #   Both work better if the GASPRICE opcode returns the original real price,
-        #   but the sender's balance doesn't actually deduct the gas. This get_gas_price()
-        #   will return 0 for eth_call, but transaction_context.gas_price will return
-        #   the same value as the GASPRICE opcode.
+        #   but the sender's balance doesn't actually deduct the gas. This
+        #   get_gas_price() will return 0 for eth_call, but
+        #   transaction_context.gas_price will return the same value as the
+        #   GASPRICE opcode.
         gas_fee = transaction.gas * self.vm_state.get_gas_price(transaction)
 
         # Buy Gas
         self.vm_state.delta_balance(transaction.sender, -1 * gas_fee)
 
         # Increment Nonce
         self.vm_state.increment_nonce(transaction.sender)
@@ -52,25 +63,23 @@
         message_gas = transaction.gas - transaction.intrinsic_gas
 
         if transaction.to == CREATE_CONTRACT_ADDRESS:
             contract_address = generate_contract_address(
                 transaction.sender,
                 self.vm_state.get_nonce(transaction.sender) - 1,
             )
-            data = b''
+            data = b""
             code = transaction.data
         else:
             contract_address = None
             data = transaction.data
             code = self.vm_state.get_code(transaction.to)
 
         self.vm_state.logger.debug2(
-            (
-                "TRANSACTION: %r; sender: %s | to: %s | data-hash: %s"
-            ),
+            ("TRANSACTION: %r; sender: %s | to: %s | data-hash: %s"),
             transaction,
             encode_hex(transaction.sender),
             encode_hex(transaction.to),
             encode_hex(keccak(transaction.data)),
         )
 
         message = Message(
@@ -81,17 +90,15 @@
             data=data,
             code=code,
             create_address=contract_address,
         )
         return message
 
     @classmethod
-    def calculate_gas_refund(cls,
-                             computation: ComputationAPI,
-                             gas_used: int) -> int:
+    def calculate_gas_refund(cls, computation: ComputationAPI, gas_used: int) -> int:
         # Self destruct refunds were added in Frontier
         # London removes them in EIP-3529
         gas_refunded = computation.get_gas_refund()
 
         return min(gas_refunded, gas_used // EIP3529_MAX_REFUND_QUOTIENT)
 
 
@@ -104,45 +111,44 @@
             transaction.max_fee_per_gas - self.execution_context.base_fee_per_gas,
             transaction.max_priority_fee_per_gas,
         )
 
     def get_gas_price(self, transaction: SignedTransactionAPI) -> int:
         return min(
             transaction.max_fee_per_gas,
-            transaction.max_priority_fee_per_gas + self.execution_context.base_fee_per_gas,
+            transaction.max_priority_fee_per_gas
+            + self.execution_context.base_fee_per_gas,
         )
 
-    def validate_transaction(
-        self,
-        transaction: SignedTransactionAPI
-    ) -> None:
+    def validate_transaction(self, transaction: SignedTransactionAPI) -> None:
         validate_london_normalized_transaction(
             state=self,
             transaction=transaction,
         )
 
-    def get_transaction_context(self: StateAPI,
-                                transaction: SignedTransactionAPI) -> TransactionContextAPI:
+    def get_transaction_context(
+        self: StateAPI, transaction: SignedTransactionAPI
+    ) -> TransactionContextAPI:
         """
         London-specific transaction context creation,
         where gas_price includes the block base fee
         """
         effective_gas_price = min(
-            transaction.max_priority_fee_per_gas + self.execution_context.base_fee_per_gas,
+            transaction.max_priority_fee_per_gas
+            + self.execution_context.base_fee_per_gas,
             transaction.max_fee_per_gas,
         )
         # See how this reduces in a pre-1559 transaction:
         # 1. effective_gas_price = min(
         #     transaction.gas_price + self.execution_context.base_fee_per_gas,
         #     transaction.gas_price,
         # )
         # base_fee_per_gas is non-negative, so:
         # 2. effective_gas_price = transaction.gas_price
 
         return self.get_transaction_context_class()(
-            gas_price=effective_gas_price,
-            origin=transaction.sender
+            gas_price=effective_gas_price, origin=transaction.sender
         )
 
     @property
     def base_fee(self: StateAPI) -> int:
         return self.execution_context.base_fee_per_gas
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/london/storage.py` & `py-evm-0.7.0a2/eth/vm/forks/london/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from eth_utils.toolz import partial
+from eth_utils.toolz import (
+    partial,
+)
 
-from eth.vm.forks.berlin import constants as berlin_constants
+from eth.vm.forks.berlin import (
+    constants as berlin_constants,
+)
 from eth.vm.forks.berlin.logic import (
     GAS_SCHEDULE_EIP2929,
     sstore_eip2929_generic,
 )
 
-
 SSTORE_CLEARS_SCHEDULE_EIP_3529 = (
     GAS_SCHEDULE_EIP2929.sstore_reset_gas
     + berlin_constants.ACCESS_LIST_STORAGE_KEY_COST_EIP_2930
 )
 
 
 GAS_SCHEDULE_EIP3529 = GAS_SCHEDULE_EIP2929._replace(
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/london/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/london/transactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-from cached_property import cached_property
 from typing import (
     Dict,
     Sequence,
     Tuple,
     Type,
     Union,
 )
 
-from eth_keys.datatypes import PrivateKey
+from cached_property import (
+    cached_property,
+)
+from eth_keys.datatypes import (
+    PrivateKey,
+)
 from eth_typing import (
     Address,
     Hash32,
 )
 from eth_utils import (
     to_bytes,
 )
@@ -29,19 +33,29 @@
     validate_transaction_signature,
 )
 from eth.abc import (
     ReceiptAPI,
     SignedTransactionAPI,
     TransactionDecoderAPI,
 )
-from eth.constants import CREATE_CONTRACT_ADDRESS
-from eth.rlp.logs import Log
-from eth.rlp.receipts import Receipt
-from eth.rlp.transactions import SignedTransactionMethods
-from eth.rlp.sedes import address
+from eth.constants import (
+    CREATE_CONTRACT_ADDRESS,
+)
+from eth.rlp.logs import (
+    Log,
+)
+from eth.rlp.receipts import (
+    Receipt,
+)
+from eth.rlp.sedes import (
+    address,
+)
+from eth.rlp.transactions import (
+    SignedTransactionMethods,
+)
 from eth.validation import (
     validate_canonical_address,
     validate_is_bytes,
     validate_is_transaction_access_list,
     validate_uint256,
 )
 from eth.vm.forks.berlin.constants import (
@@ -57,26 +71,30 @@
     BerlinUnsignedLegacyTransaction,
     TypedTransaction,
 )
 from eth.vm.forks.istanbul.transactions import (
     ISTANBUL_TX_GAS_SCHEDULE,
 )
 
-from .constants import DYNAMIC_FEE_TRANSACTION_TYPE
-from .receipts import LondonReceiptBuilder
+from .constants import (
+    DYNAMIC_FEE_TRANSACTION_TYPE,
+)
+from .receipts import (
+    LondonReceiptBuilder,
+)
 
 
 class LondonLegacyTransaction(BerlinLegacyTransaction):
     pass
 
 
 class LondonUnsignedLegacyTransaction(BerlinUnsignedLegacyTransaction):
-    def as_signed_transaction(self,
-                              private_key: PrivateKey,
-                              chain_id: int = None) -> LondonLegacyTransaction:
+    def as_signed_transaction(
+        self, private_key: PrivateKey, chain_id: int = None
+    ) -> LondonLegacyTransaction:
         v, r, s = create_transaction_signature(self, private_key, chain_id=chain_id)
         return LondonLegacyTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
             value=self.value,
@@ -86,34 +104,34 @@
             s=s,
         )
 
 
 class UnsignedDynamicFeeTransaction(rlp.Serializable):
     _type_id = DYNAMIC_FEE_TRANSACTION_TYPE
     fields = [
-        ('chain_id', big_endian_int),
-        ('nonce', big_endian_int),
-        ('max_priority_fee_per_gas', big_endian_int),
-        ('max_fee_per_gas', big_endian_int),
-        ('gas', big_endian_int),
-        ('to', address),
-        ('value', big_endian_int),
-        ('data', binary),
-        ('access_list', CountableList(AccountAccesses)),
+        ("chain_id", big_endian_int),
+        ("nonce", big_endian_int),
+        ("max_priority_fee_per_gas", big_endian_int),
+        ("max_fee_per_gas", big_endian_int),
+        ("gas", big_endian_int),
+        ("to", address),
+        ("value", big_endian_int),
+        ("data", binary),
+        ("access_list", CountableList(AccountAccesses)),
     ]
 
     @cached_property
     def _type_byte(self) -> bytes:
         return to_bytes(self._type_id)
 
     def get_message_for_signing(self) -> bytes:
         payload = rlp.encode(self)
         return self._type_byte + payload
 
-    def as_signed_transaction(self, private_key: PrivateKey) -> 'TypedTransaction':
+    def as_signed_transaction(self, private_key: PrivateKey) -> "TypedTransaction":
         message = self.get_message_for_signing()
         signature = private_key.sign_msg(message)
         y_parity, r, s = signature.vrs
 
         signed_transaction = DynamicFeeTransaction(
             self.chain_id,
             self.nonce,
@@ -122,15 +140,15 @@
             self.gas,
             self.to,
             self.value,
             self.data,
             self.access_list,
             y_parity,
             r,
-            s
+            s,
         )
         return LondonTypedTransaction(self._type_id, signed_transaction)
 
     def validate(self) -> None:
         validate_uint256(self.chain_id, title="Transaction.chain_id")
         validate_uint256(self.nonce, title="Transaction.nonce")
         validate_uint256(self.max_fee_per_gas, title="Transaction.max_fee_per_gas")
@@ -148,35 +166,38 @@
         return _get_dynamic_fee_txn_intrinsic_gas(self)
 
     @property
     def intrinsic_gas(self) -> int:
         return self.get_intrinsic_gas()
 
 
-class DynamicFeeTransaction(rlp.Serializable, SignedTransactionMethods, SignedTransactionAPI):
+class DynamicFeeTransaction(
+    rlp.Serializable, SignedTransactionMethods, SignedTransactionAPI
+):
     _type_id = DYNAMIC_FEE_TRANSACTION_TYPE
     fields = [
-        ('chain_id', big_endian_int),
-        ('nonce', big_endian_int),
-        ('max_priority_fee_per_gas', big_endian_int),
-        ('max_fee_per_gas', big_endian_int),
-        ('gas', big_endian_int),
-        ('to', address),
-        ('value', big_endian_int),
-        ('data', binary),
-        ('access_list', CountableList(AccountAccesses)),
-        ('y_parity', big_endian_int),
-        ('r', big_endian_int),
-        ('s', big_endian_int),
+        ("chain_id", big_endian_int),
+        ("nonce", big_endian_int),
+        ("max_priority_fee_per_gas", big_endian_int),
+        ("max_fee_per_gas", big_endian_int),
+        ("gas", big_endian_int),
+        ("to", address),
+        ("value", big_endian_int),
+        ("data", binary),
+        ("access_list", CountableList(AccountAccesses)),
+        ("y_parity", big_endian_int),
+        ("r", big_endian_int),
+        ("s", big_endian_int),
     ]
 
     @property
     def gas_price(self) -> None:
         raise AttributeError(
-            "Gas price is no longer available. See max_priority_fee_per_gas or max_fee_per_gas"
+            "Gas price is no longer available."
+            "See max_priority_fee_per_gas or max_fee_per_gas"
         )
 
     def get_sender(self) -> Address:
         return extract_transaction_sender(self)
 
     def get_message_for_signing(self) -> bytes:
         unsigned = UnsignedDynamicFeeTransaction(
@@ -207,24 +228,20 @@
     def get_intrinsic_gas(self) -> int:
         return _get_dynamic_fee_txn_intrinsic_gas(self)
 
     def encode(self) -> bytes:
         return rlp.encode(self)
 
     def make_receipt(
-            self,
-            status: bytes,
-            gas_used: int,
-            log_entries: Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...]) -> ReceiptAPI:
-
-        logs = [
-            Log(address, topics, data)
-            for address, topics, data
-            in log_entries
-        ]
+        self,
+        status: bytes,
+        gas_used: int,
+        log_entries: Tuple[Tuple[bytes, Tuple[int, ...], bytes], ...],
+    ) -> ReceiptAPI:
+        logs = [Log(address, topics, data) for address, topics, data in log_entries]
         # TypedTransaction is responsible for wrapping this into a TypedReceipt
         return Receipt(
             state_root=status,
             gas_used=gas_used,
             logs=logs,
         )
 
@@ -246,24 +263,25 @@
 class LondonTransactionBuilder(BerlinTransactionBuilder):
     legacy_signed = LondonLegacyTransaction
     legacy_unsigned = LondonUnsignedLegacyTransaction
     typed_transaction = LondonTypedTransaction
 
     @classmethod
     def new_unsigned_dynamic_fee_transaction(
-            cls,
-            chain_id: int,
-            nonce: int,
-            max_priority_fee_per_gas: int,
-            max_fee_per_gas: int,
-            gas: int,
-            to: Address,
-            value: int,
-            data: bytes,
-            access_list: Sequence[Tuple[Address, Sequence[int]]],) -> LondonTypedTransaction:
+        cls,
+        chain_id: int,
+        nonce: int,
+        max_priority_fee_per_gas: int,
+        max_fee_per_gas: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+        access_list: Sequence[Tuple[Address, Sequence[int]]],
+    ) -> LondonTypedTransaction:
         transaction = UnsignedDynamicFeeTransaction(
             chain_id,
             nonce,
             max_priority_fee_per_gas,
             max_fee_per_gas,
             gas,
             to,
@@ -271,27 +289,28 @@
             data,
             access_list,
         )
         return transaction
 
     @classmethod
     def new_dynamic_fee_transaction(
-            cls,
-            chain_id: int,
-            nonce: int,
-            max_priority_fee_per_gas: int,
-            max_fee_per_gas: int,
-            gas: int,
-            to: Address,
-            value: int,
-            data: bytes,
-            access_list: Sequence[Tuple[Address, Sequence[int]]],
-            y_parity: int,
-            r: int,
-            s: int) -> LondonTypedTransaction:
+        cls,
+        chain_id: int,
+        nonce: int,
+        max_priority_fee_per_gas: int,
+        max_fee_per_gas: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes,
+        access_list: Sequence[Tuple[Address, Sequence[int]]],
+        y_parity: int,
+        r: int,
+        s: int,
+    ) -> LondonTypedTransaction:
         transaction = DynamicFeeTransaction(
             chain_id,
             nonce,
             max_priority_fee_per_gas,
             max_fee_per_gas,
             gas,
             to,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/london/validation.py` & `py-evm-0.7.0a2/eth/vm/forks/london/validation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from eth_utils.exceptions import ValidationError
+from eth_utils.exceptions import (
+    ValidationError,
+)
 
 from eth.abc import (
     SignedTransactionAPI,
-    StateAPI
+    StateAPI,
 )
 from eth.vm.forks.homestead.validation import (
     validate_homestead_transaction,
 )
 
 
 def validate_london_normalized_transaction(
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/muir_glacier/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/muir_glacier/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     create_muir_glacier_header_from_parent,
 )
 from .state import MuirGlacierState
 
 
 class MuirGlacierVM(IstanbulVM):
     # fork name
-    fork = 'muir-glacier'
+    fork = "muir-glacier"
 
     # classes
     block_class: Type[BaseBlock] = MuirGlacierBlock
     _state_class: Type[BaseState] = MuirGlacierState
 
     # Methods
-    create_header_from_parent = staticmethod(create_muir_glacier_header_from_parent)  # type: ignore
-    compute_difficulty = staticmethod(compute_muir_glacier_difficulty)    # type: ignore
+    create_header_from_parent = staticmethod(create_muir_glacier_header_from_parent)  # type: ignore  # noqa: E501
+    compute_difficulty = staticmethod(compute_muir_glacier_difficulty)  # type: ignore
     configure_header = configure_muir_glacier_header
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/paris/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/paris/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     create_paris_header_from_parent,
 )
 from .state import ParisState
 
 
 class ParisVM(GrayGlacierVM):
     # fork name
-    fork = 'paris'
+    fork = "paris"
 
     # classes
     block_class: Type[BaseBlock] = ParisBlock
     _state_class: Type[BaseState] = ParisState
     consensus_class: Type[ConsensusAPI] = PosConsensus
 
     # Methods
@@ -49,29 +49,30 @@
 
     def _assign_block_rewards(self, block: BlockAPI) -> None:
         # No block reward or uncles / uncle rewards in PoS
         pass
 
     @classmethod
     def validate_header(
-        cls,
-        header: BlockHeaderAPI,
-        parent_header: BlockHeaderAPI
+        cls, header: BlockHeaderAPI, parent_header: BlockHeaderAPI
     ) -> None:
         super().validate_header(header, parent_header)
 
         difficulty, nonce, uncles_hash = (
-            header.difficulty, header.nonce, header.uncles_hash
+            header.difficulty,
+            header.nonce,
+            header.uncles_hash,
         )
 
         if difficulty != POST_MERGE_DIFFICULTY:
             raise ValidationError(
                 f"Difficulty must be {POST_MERGE_DIFFICULTY}, got {difficulty}."
             )
         if nonce != POST_MERGE_NONCE:
             raise ValidationError(
                 f"Nonce must be {POST_MERGE_NONCE !r}, got {nonce !r}."
             )
         if uncles_hash != POST_MERGE_OMMERS_HASH:
             raise ValidationError(
-                f"Uncles hash must be {POST_MERGE_OMMERS_HASH !r}, got {uncles_hash !r}."
+                f"Uncles hash must be {POST_MERGE_OMMERS_HASH !r}, "
+                f"got {uncles_hash !r}."
             )
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/paris/headers.py` & `py-evm-0.7.0a2/eth/vm/forks/paris/headers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,38 @@
-from typing import Any, Optional
+from typing import (
+    Any,
+    Optional,
+)
 
-from toolz import curry
+from eth_utils import (
+    ValidationError,
+)
+from toolz import (
+    curry,
+)
 
-from eth.abc import BlockHeaderAPI
+from eth.abc import (
+    BlockHeaderAPI,
+)
 from eth.constants import (
     POST_MERGE_DIFFICULTY,
     POST_MERGE_MIX_HASH,
     POST_MERGE_NONCE,
 )
+from eth.vm.forks.byzantium.headers import (
+    configure_header,
+)
 from eth.vm.forks.gray_glacier.headers import (
     compute_gray_glacier_difficulty,
     create_gray_glacier_header_from_parent,
 )
-from eth.vm.forks.byzantium.headers import (
-    configure_header,
+
+from .blocks import (
+    ParisBlockHeader,
 )
-from eth_utils import ValidationError
-from .blocks import ParisBlockHeader
 
 
 def _validate_and_return_paris_header_param(
     header_param: str,
     actual: Any,
     constant_value: Any,
 ) -> Any:
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/paris/opcodes.py` & `py-evm-0.7.0a2/eth/vm/forks/paris/opcodes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 import copy
-from typing import Dict
+from typing import (
+    Dict,
+)
 
-from eth.vm.opcode import as_opcode
-from eth_utils.toolz import merge
+from eth_utils.toolz import (
+    merge,
+)
 
-from eth import constants
-from eth.abc import OpcodeAPI
-from eth.vm import mnemonics
-from eth.vm import opcode_values
+from eth import (
+    constants,
+)
+from eth.abc import (
+    OpcodeAPI,
+)
+from eth.vm import (
+    mnemonics,
+    opcode_values,
+)
+from eth.vm.forks.london.opcodes import (
+    LONDON_OPCODES,
+)
 from eth.vm.logic import (
     block,
 )
-
-from eth.vm.forks.london.opcodes import LONDON_OPCODES
-
+from eth.vm.opcode import (
+    as_opcode,
+)
 
 NEW_OPCODES = {
     # EIP-4399: supplant DIFFICULTY with PREVRANDAO
     opcode_values.PREVRANDAO: as_opcode(
         logic_fn=block.mixhash,
         mnemonic=mnemonics.PREVRANDAO,
         gas_cost=constants.GAS_BASE,
     ),
 }
 
-PARIS_OPCODES: Dict[int, OpcodeAPI] = merge(
-    copy.deepcopy(LONDON_OPCODES),
-    NEW_OPCODES
-)
+PARIS_OPCODES: Dict[int, OpcodeAPI] = merge(copy.deepcopy(LONDON_OPCODES), NEW_OPCODES)
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/paris/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/paris/transactions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-from abc import ABC
+from abc import (
+    ABC,
+)
 
-from eth_keys.datatypes import PrivateKey
+from eth_keys.datatypes import (
+    PrivateKey,
+)
 
 from eth._utils.transactions import (
     create_transaction_signature,
 )
 from eth.vm.forks.gray_glacier.transactions import (
     GrayGlacierLegacyTransaction,
     GrayGlacierTransactionBuilder,
@@ -14,17 +18,15 @@
 
 class ParisLegacyTransaction(GrayGlacierLegacyTransaction, ABC):
     pass
 
 
 class ParisUnsignedLegacyTransaction(GrayGlacierUnsignedLegacyTransaction):
     def as_signed_transaction(
-        self,
-        private_key: PrivateKey,
-        chain_id: int = None
+        self, private_key: PrivateKey, chain_id: int = None
     ) -> ParisLegacyTransaction:
         v, r, s = create_transaction_signature(self, private_key, chain_id=chain_id)
         return ParisLegacyTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/petersburg/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/petersburg/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,22 +19,22 @@
     create_petersburg_header_from_parent,
 )
 from .state import PetersburgState
 
 
 class PetersburgVM(ByzantiumVM):
     # fork name
-    fork = 'petersburg'
+    fork = "petersburg"
 
     # classes
     block_class: Type[BlockAPI] = PetersburgBlock
     _state_class: Type[StateAPI] = PetersburgState
 
     # Methods
-    create_header_from_parent = staticmethod(create_petersburg_header_from_parent)  # type: ignore
-    compute_difficulty = staticmethod(compute_petersburg_difficulty)    # type: ignore
+    create_header_from_parent = staticmethod(create_petersburg_header_from_parent)  # type: ignore  # noqa: E501
+    compute_difficulty = staticmethod(compute_petersburg_difficulty)  # type: ignore
     configure_header = configure_petersburg_header
     get_uncle_reward = staticmethod(get_uncle_reward(EIP1234_BLOCK_REWARD))
 
     @staticmethod
     def get_block_reward() -> int:
         return EIP1234_BLOCK_REWARD
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/petersburg/computation.py` & `py-evm-0.7.0a2/eth/vm/forks/petersburg/computation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from eth.vm.forks.byzantium.computation import (
-    BYZANTIUM_PRECOMPILES
-)
-from eth.vm.forks.byzantium.computation import (
-    ByzantiumComputation
+    BYZANTIUM_PRECOMPILES,
+    ByzantiumComputation,
 )
 
-from .opcodes import PETERSBURG_OPCODES
+from .opcodes import (
+    PETERSBURG_OPCODES,
+)
 
 PETERSBURG_PRECOMPILES = BYZANTIUM_PRECOMPILES
 
 
 class PetersburgComputation(ByzantiumComputation):
     """
-    A class for all execution computations in the ``Petersburg`` fork.
-    Inherits from :class:`~eth.vm.forks.byzantium.computation.ByzantiumComputation`
+    A class for all execution *message* computations in the ``Petersburg`` fork.
+    Inherits from
+    :class:`~eth.vm.forks.byzantium.computation.ByzantiumComputation`
     """
+
     # Override
     opcodes = PETERSBURG_OPCODES
     _precompiles = PETERSBURG_PRECOMPILES
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/petersburg/opcodes.py` & `py-evm-0.7.0a2/eth/vm/forks/shanghai/opcodes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 import copy
-from typing import Dict
+from typing import (
+    Dict,
+)
 
 from eth_utils.toolz import (
-    merge
+    merge,
 )
 
 from eth import (
-    constants
+    constants,
+)
+from eth.abc import (
+    OpcodeAPI,
+)
+from eth.tools._utils.deprecation import (
+    deprecate_method,
 )
-from eth.abc import OpcodeAPI
 from eth.vm import (
     mnemonics,
     opcode_values,
 )
-from eth.vm.forks.byzantium.opcodes import (
-    BYZANTIUM_OPCODES,
-)
-from eth.vm.forks.petersburg.constants import (
-    GAS_EXTCODEHASH_EIP1052
+from eth.vm.forks.paris.opcodes import (
+    PARIS_OPCODES,
 )
 from eth.vm.logic import (
-    arithmetic,
-    context,
-    system,
+    stack,
 )
 from eth.vm.opcode import (
-    as_opcode
+    as_opcode,
 )
 
+from .logic import (
+    Create2EIP3860,
+    CreateEIP3860,
+)
 
-UPDATED_OPCODES = {
-    opcode_values.SHL: as_opcode(
-        logic_fn=arithmetic.shl,
-        mnemonic=mnemonics.SHL,
-        gas_cost=constants.GAS_VERYLOW,
-    ),
-    opcode_values.SHR: as_opcode(
-        logic_fn=arithmetic.shr,
-        mnemonic=mnemonics.SHR,
-        gas_cost=constants.GAS_VERYLOW,
-    ),
-    opcode_values.SAR: as_opcode(
-        logic_fn=arithmetic.sar,
-        mnemonic=mnemonics.SAR,
-        gas_cost=constants.GAS_VERYLOW,
-    ),
-    opcode_values.EXTCODEHASH: as_opcode(
-        logic_fn=context.extcodehash,
-        mnemonic=mnemonics.EXTCODEHASH,
-        gas_cost=GAS_EXTCODEHASH_EIP1052,
-    ),
-    opcode_values.CREATE2: system.Create2.configure(
-        __name__='opcode:CREATE2',
+UPDATED_OPCODES: Dict[int, OpcodeAPI] = {
+    opcode_values.CREATE: CreateEIP3860.configure(
+        __name__="CreateEIP3860",
+        mnemonic=mnemonics.CREATE,
+        gas_cost=constants.GAS_CREATE,
+    )(),
+    opcode_values.CREATE2: Create2EIP3860.configure(
+        __name__="Create2EIP3860",
         mnemonic=mnemonics.CREATE2,
         gas_cost=constants.GAS_CREATE,
     )(),
+    opcode_values.SELFDESTRUCT: deprecate_method(
+        PARIS_OPCODES[opcode_values.SELFDESTRUCT],
+        message=(
+            f"{mnemonics.SELFDESTRUCT} opcode present in computation. This opcode is "
+            "deprecated and a breaking change to its functionality is likely to come "
+            "in the future."
+        ),
+    ),
+}
+
+NEW_OPCODES: Dict[int, OpcodeAPI] = {
+    opcode_values.PUSH0: as_opcode(
+        logic_fn=stack.push0,
+        mnemonic=mnemonics.PUSH0,
+        gas_cost=constants.GAS_BASE,
+    ),
 }
 
-PETERSBURG_OPCODES: Dict[int, OpcodeAPI] = merge(
-    copy.deepcopy(BYZANTIUM_OPCODES),
+SHANGHAI_OPCODES: Dict[int, OpcodeAPI] = merge(
+    copy.deepcopy(PARIS_OPCODES),
     UPDATED_OPCODES,
+    NEW_OPCODES,
 )
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/petersburg/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/byzantium/transactions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-from eth_keys.datatypes import PrivateKey
-from eth_typing import Address
-
-from eth.vm.forks.byzantium.transactions import (
-    ByzantiumTransaction,
-    ByzantiumUnsignedTransaction,
+from eth_keys.datatypes import (
+    PrivateKey,
+)
+from eth_typing import (
+    Address,
 )
 
 from eth._utils.transactions import (
     create_transaction_signature,
 )
+from eth.vm.forks.spurious_dragon.transactions import (
+    SpuriousDragonTransaction,
+    SpuriousDragonUnsignedTransaction,
+)
 
 
-class PetersburgTransaction(ByzantiumTransaction):
+class ByzantiumTransaction(SpuriousDragonTransaction):
     @classmethod
-    def create_unsigned_transaction(cls,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> 'PetersburgUnsignedTransaction':
-        return PetersburgUnsignedTransaction(nonce, gas_price, gas, to, value, data)
-
-
-class PetersburgUnsignedTransaction(ByzantiumUnsignedTransaction):
-    def as_signed_transaction(self,
-                              private_key: PrivateKey,
-                              chain_id: int = None) -> PetersburgTransaction:
+    def create_unsigned_transaction(
+        cls,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes
+    ) -> "ByzantiumUnsignedTransaction":
+        return ByzantiumUnsignedTransaction(nonce, gas_price, gas, to, value, data)
+
+
+class ByzantiumUnsignedTransaction(SpuriousDragonUnsignedTransaction):
+    def as_signed_transaction(
+        self, private_key: PrivateKey, chain_id: int = None
+    ) -> ByzantiumTransaction:
         v, r, s = create_transaction_signature(self, private_key, chain_id=chain_id)
-        return PetersburgTransaction(
+        return ByzantiumTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
             value=self.value,
             data=self.data,
             v=v,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/shanghai/__init__.py` & `py-evm-0.7.0a2/eth/vm/forks/shanghai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     create_shanghai_header_from_parent,
 )
 from .state import ShanghaiState
 
 
 class ShanghaiVM(ParisVM):
     # fork name
-    fork = 'shanghai'
+    fork = "shanghai"
 
     # classes
     block_class: Type[BaseBlock] = ShanghaiBlock
     _state_class: Type[BaseState] = ShanghaiState
 
     # Methods
     create_header_from_parent = staticmethod(  # type: ignore
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/shanghai/blocks.py` & `py-evm-0.7.0a2/eth/vm/forks/shanghai/blocks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,127 @@
-from abc import ABC
-from typing import List, Sequence, Tuple, Type, cast
-
+from abc import (
+    ABC,
+)
+from typing import (
+    List,
+    Sequence,
+    Tuple,
+    Type,
+    cast,
+)
+
+from eth_bloom import (
+    BloomFilter,
+)
+from eth_typing import (
+    Address,
+    BlockNumber,
+    Hash32,
+)
+from eth_utils import (
+    encode_hex,
+    keccak,
+)
 import rlp
-from eth.exceptions import BlockNotFound, HeaderNotFound
-from eth.rlp.blocks import BaseBlock
-from eth.rlp.headers import BlockHeader
-from eth.rlp.sedes import address, hash32, trie_root, uint256
-from eth_bloom import BloomFilter
-from eth_typing import Address, BlockNumber, Hash32
+from rlp.sedes import (
+    Binary,
+    CountableList,
+    big_endian_int,
+    binary,
+)
+from trie.exceptions import (
+    MissingTrieNode,
+)
 
-from eth._utils.headers import new_timestamp_from_parent
+from eth._utils.headers import (
+    new_timestamp_from_parent,
+)
 from eth.abc import (
-    BlockHeaderAPI, BlockHeaderSedesAPI, ChainDatabaseAPI, MiningHeaderAPI,
-    ReceiptAPI, ReceiptBuilderAPI, SignedTransactionAPI, TransactionBuilderAPI,
+    BlockHeaderAPI,
+    BlockHeaderSedesAPI,
+    ChainDatabaseAPI,
+    MiningHeaderAPI,
+    ReceiptAPI,
+    ReceiptBuilderAPI,
+    SignedTransactionAPI,
+    TransactionBuilderAPI,
     WithdrawalAPI,
 )
 from eth.constants import (
-    ZERO_ADDRESS,
-    ZERO_HASH32,
+    BLANK_ROOT_HASH,
     EMPTY_UNCLE_HASH,
     GENESIS_NONCE,
     GENESIS_PARENT_HASH,
-    BLANK_ROOT_HASH,
+    ZERO_ADDRESS,
+    ZERO_HASH32,
 )
-
-from eth_utils import (
-    encode_hex, keccak,
+from eth.exceptions import (
+    BlockNotFound,
+    HeaderNotFound,
+)
+from eth.rlp.blocks import (
+    BaseBlock,
+)
+from eth.rlp.headers import (
+    BlockHeader,
+)
+from eth.rlp.sedes import (
+    address,
+    hash32,
+    trie_root,
+    uint256,
 )
 
-from rlp.sedes import (
-    Binary, CountableList, big_endian_int, binary,
+from ..london.blocks import (
+    LondonBlockHeader,
+)
+from ..london.receipts import (
+    LondonReceiptBuilder,
 )
-from trie.exceptions import MissingTrieNode
-
 from .transactions import (
     ShanghaiTransactionBuilder,
 )
-from .withdrawals import Withdrawal
-from ..london.blocks import (
-    LondonBlockHeader,
+from .withdrawals import (
+    Withdrawal,
 )
 
-
 UNMINED_SHANGHAI_HEADER_FIELDS = [
-    ('parent_hash', hash32),
-    ('uncles_hash', hash32),
-    ('coinbase', address),
-    ('state_root', trie_root),
-    ('transaction_root', trie_root),
-    ('receipt_root', trie_root),
-    ('bloom', uint256),
-    ('difficulty', big_endian_int),
-    ('block_number', big_endian_int),
-    ('gas_limit', big_endian_int),
-    ('gas_used', big_endian_int),
-    ('timestamp', big_endian_int),
-    ('extra_data', binary),
-    ('base_fee_per_gas', big_endian_int),
-    ('withdrawals_root', trie_root),
+    ("parent_hash", hash32),
+    ("uncles_hash", hash32),
+    ("coinbase", address),
+    ("state_root", trie_root),
+    ("transaction_root", trie_root),
+    ("receipt_root", trie_root),
+    ("bloom", uint256),
+    ("difficulty", big_endian_int),
+    ("block_number", big_endian_int),
+    ("gas_limit", big_endian_int),
+    ("gas_used", big_endian_int),
+    ("timestamp", big_endian_int),
+    ("extra_data", binary),
+    ("base_fee_per_gas", big_endian_int),
+    ("withdrawals_root", trie_root),
 ]
 
 
 class ShanghaiMiningHeader(rlp.Serializable, MiningHeaderAPI, ABC):
     fields = UNMINED_SHANGHAI_HEADER_FIELDS
 
 
 class ShanghaiBlockHeader(rlp.Serializable, BlockHeaderAPI, ABC):
     # `mix_hash` and `nonce` were fields before `base_fee_per_gas` and
     # `withdrawals_root` and, thus, appear in the block header before them.
-    fields = UNMINED_SHANGHAI_HEADER_FIELDS[:13] + [
-        ('mix_hash', binary),
-        ('nonce', Binary(8, allow_empty=True)),
-    ] + UNMINED_SHANGHAI_HEADER_FIELDS[13:]
+    fields = (
+        UNMINED_SHANGHAI_HEADER_FIELDS[:13]
+        + [
+            ("mix_hash", binary),
+            ("nonce", Binary(8, allow_empty=True)),
+        ]
+        + UNMINED_SHANGHAI_HEADER_FIELDS[13:]
+    )
 
     def __init__(
         self,
         difficulty: int,
         block_number: BlockNumber,
         gas_limit: int,
         timestamp: int = None,
@@ -83,15 +129,15 @@
         parent_hash: Hash32 = ZERO_HASH32,
         uncles_hash: Hash32 = EMPTY_UNCLE_HASH,
         state_root: Hash32 = BLANK_ROOT_HASH,
         transaction_root: Hash32 = BLANK_ROOT_HASH,
         receipt_root: Hash32 = BLANK_ROOT_HASH,
         bloom: int = 0,
         gas_used: int = 0,
-        extra_data: bytes = b'',
+        extra_data: bytes = b"",
         mix_hash: Hash32 = ZERO_HASH32,
         nonce: bytes = GENESIS_NONCE,
         base_fee_per_gas: int = 0,
         withdrawals_root: Hash32 = BLANK_ROOT_HASH,
     ) -> None:
         if timestamp is None:
             if parent_hash == ZERO_HASH32:
@@ -121,16 +167,16 @@
             nonce=nonce,
             base_fee_per_gas=base_fee_per_gas,
             withdrawals_root=withdrawals_root,
         )
 
     def __str__(self) -> str:
         return (
-            f'<ShanghaiBlockHeader '
-            f'#{self.block_number} {encode_hex(self.hash)[2:10]}>'
+            f"<ShanghaiBlockHeader "
+            f"#{self.block_number} {encode_hex(self.hash)[2:10]}>"
         )
 
     _hash = None
 
     @property
     def hash(self) -> Hash32:
         if self._hash is None:
@@ -178,19 +224,21 @@
             )
 
 
 class ShanghaiBlock(BaseBlock):
     # re-defined from `BaseBlock`, as `FrontierBlock` was, to include withdrawals
 
     transaction_builder: Type[TransactionBuilderAPI] = ShanghaiTransactionBuilder
+    # London was the last fork where the receipt builder was updated
+    receipt_builder: Type[ReceiptBuilderAPI] = LondonReceiptBuilder
     fields = [
-        ('header', ShanghaiBlockHeader),
-        ('transactions', CountableList(transaction_builder)),
-        ('uncles', CountableList(ShanghaiBackwardsHeader, max_length=0)),
-        ('withdrawals', CountableList(Withdrawal)),
+        ("header", ShanghaiBlockHeader),
+        ("transactions", CountableList(transaction_builder)),
+        ("uncles", CountableList(ShanghaiBackwardsHeader, max_length=0)),
+        ("withdrawals", CountableList(Withdrawal)),
     ]
 
     bloom_filter = None
 
     def __init__(
         self,
         header: BlockHeaderAPI,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/shanghai/computation.py` & `py-evm-0.7.0a2/eth/vm/forks/shanghai/computation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,37 @@
-from eth._utils.numeric import ceil32
-from eth.abc import ComputationAPI, MessageAPI, StateAPI, TransactionContextAPI
+from eth._utils.numeric import (
+    ceil32,
+)
+from eth.abc import (
+    ComputationAPI,
+    MessageAPI,
+    StateAPI,
+    TransactionContextAPI,
+)
+from eth.exceptions import (
+    OutOfGas,
+)
+from eth.vm.forks.paris.computation import (
+    ParisComputation,
+)
+
 from .constants import (
     INITCODE_WORD_COST,
     MAX_INITCODE_SIZE,
 )
-from .opcodes import SHANGHAI_OPCODES
-from eth.exceptions import (
-    OutOfGas,
+from .opcodes import (
+    SHANGHAI_OPCODES,
 )
-from eth.vm.forks.paris.computation import ParisComputation
 
 
 class ShanghaiComputation(ParisComputation):
     """
-    A class for all execution computations in the ``Shanghai`` hard fork
+    A class for all execution *message* computations in the ``Shanghai`` hard fork
     """
+
     opcodes = SHANGHAI_OPCODES
 
     def __init__(
         self,
         state: StateAPI,
         message: MessageAPI,
         transaction_context: TransactionContextAPI,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/shanghai/headers.py` & `py-evm-0.7.0a2/eth/vm/forks/shanghai/headers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,36 @@
-from typing import Any, Optional
+from typing import (
+    Any,
+    Optional,
+)
 
-from toolz import curry
+from toolz import (
+    curry,
+)
 
-from eth.abc import BlockHeaderAPI
-from eth.vm.forks.paris.headers import (
-    create_paris_header_from_parent,
+from eth.abc import (
+    BlockHeaderAPI,
 )
 from eth.vm.forks.byzantium.headers import (
     configure_header,
 )
-from .blocks import ShanghaiBlockHeader
+from eth.vm.forks.paris.headers import (
+    create_paris_header_from_parent,
+)
+
+from .blocks import (
+    ShanghaiBlockHeader,
+)
 
 
 @curry
 def create_shanghai_header_from_parent(
     parent_header: Optional[BlockHeaderAPI],
     **header_params: Any,
 ) -> BlockHeaderAPI:
-
     paris_validated_header = create_paris_header_from_parent(
         parent_header, **header_params
     )
 
     # extract params validated up to paris (previous VM)
     # and plug into a `ShanghaiBlockHeader` class
     all_fields = paris_validated_header.as_dict()
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/shanghai/logic.py` & `py-evm-0.7.0a2/eth/vm/forks/shanghai/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from .constants import (
-    INITCODE_WORD_COST,
-)
 from eth._utils.numeric import (
     ceil32,
 )
 from eth.vm.forks.berlin.logic import (
-    CreateEIP2929,
     Create2EIP2929,
+    CreateEIP2929,
 )
 from eth.vm.logic.system import (
     CreateOpcodeStackData,
 )
 
+from .constants import (
+    INITCODE_WORD_COST,
+)
+
 
 class CreateEIP3860(CreateEIP2929):
     def get_gas_cost(self, data: CreateOpcodeStackData) -> int:
         eip2929_gas_cost = super().get_gas_cost(data)
         eip3860_gas_cost = INITCODE_WORD_COST * ceil32(data.memory_length) // 32
         return eip2929_gas_cost + eip3860_gas_cost
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/shanghai/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/shanghai/transactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-from abc import ABC
+from abc import (
+    ABC,
+)
 
-from eth_keys.datatypes import PrivateKey
+from eth_keys.datatypes import (
+    PrivateKey,
+)
 
 from eth._utils.transactions import (
     create_transaction_signature,
 )
 from eth.vm.forks.paris.transactions import (
     ParisLegacyTransaction,
     ParisTransactionBuilder,
@@ -14,17 +18,15 @@
 
 class ShanghaiLegacyTransaction(ParisLegacyTransaction, ABC):
     pass
 
 
 class ShanghaiUnsignedLegacyTransaction(ParisUnsignedLegacyTransaction):
     def as_signed_transaction(
-        self,
-        private_key: PrivateKey,
-        chain_id: int = None
+        self, private_key: PrivateKey, chain_id: int = None
     ) -> ShanghaiLegacyTransaction:
         v, r, s = create_transaction_signature(self, private_key, chain_id=chain_id)
         return ShanghaiLegacyTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/shanghai/withdrawals.py` & `py-evm-0.7.0a2/eth/vm/forks/shanghai/withdrawals.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,44 @@
-from cached_property import cached_property
-from typing import cast
+from typing import (
+    cast,
+)
 
-from eth.abc import WithdrawalAPI
-from eth.validation import (
-    validate_canonical_address,
-    validate_uint64,
+from cached_property import (
+    cached_property,
 )
 from eth_typing import (
     Address,
     Hash32,
 )
-
+from eth_utils import (
+    keccak,
+)
 import rlp
-from eth.rlp.sedes import address
-from eth_utils import keccak
-from rlp.sedes import big_endian_int
+from rlp.sedes import (
+    big_endian_int,
+)
+
+from eth.abc import (
+    WithdrawalAPI,
+)
+from eth.rlp.sedes import (
+    address,
+)
+from eth.validation import (
+    validate_canonical_address,
+    validate_uint64,
+)
 
 
 class Withdrawal(rlp.Serializable):
     fields = [
-        ('index', big_endian_int),
-        ('validator_index', big_endian_int),
-        ('address', address),
-        ('amount', big_endian_int),
+        ("index", big_endian_int),
+        ("validator_index", big_endian_int),
+        ("address", address),
+        ("amount", big_endian_int),
     ]
 
     def __init__(
         self,
         index: int = 0,
         validator_index: int = 0,
         address: Address = None,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/_utils.py` & `py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-from typing import Iterable
-
-from eth_typing import Address
-
-from eth_utils import to_set
+from typing import (
+    Iterable,
+)
 
-from eth import constants
+from eth_typing import (
+    Address,
+)
+from eth_utils import (
+    to_set,
+)
 
+from eth import (
+    constants,
+)
 from eth._utils.address import (
     force_bytes_to_address,
 )
+from eth.abc import (
+    ComputationAPI,
+)
 
-from eth.vm.computation import BaseComputation
-
-
-THREE = force_bytes_to_address(b'\x03')
+THREE = force_bytes_to_address(b"\x03")
 
 
 @to_set
 def collect_touched_accounts(
-    computation: BaseComputation,
-    ancestor_had_error: bool = False
+    computation: ComputationAPI, ancestor_had_error: bool = False
 ) -> Iterable[Address]:
     """
     Collect all of the accounts that *may* need to be deleted based on
     `EIP-161 <https://eips.ethereum.org/EIPS/eip-161>`_.
 
     Checking whether they *do* need to be deleted happens in the caller.
 
@@ -55,9 +60,9 @@
                 yield computation.msg.to
         else:
             yield computation.msg.to
 
     # recurse into nested computations (even errored ones, since looking for RIPEMD160)
     for child in computation.children:
         yield from collect_touched_accounts(
-            child,
-            ancestor_had_error=(computation.is_error or ancestor_had_error))
+            child, ancestor_had_error=(computation.is_error or ancestor_had_error)
+        )
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/computation.py` & `py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/computation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,56 @@
-from eth_hash.auto import keccak
-
+from eth_hash.auto import (
+    keccak,
+)
 from eth_utils import (
     encode_hex,
 )
 
-from eth import constants
+from eth import (
+    constants,
+)
 from eth.abc import (
     ComputationAPI,
     MessageAPI,
     StateAPI,
     TransactionContextAPI,
 )
 from eth.exceptions import (
     OutOfGas,
     VMError,
 )
 from eth.vm.forks.homestead.computation import (
     HomesteadComputation,
 )
 
-from ..spurious_dragon.constants import EIP170_CODE_SIZE_LIMIT
-from .opcodes import SPURIOUS_DRAGON_OPCODES
+from ..spurious_dragon.constants import (
+    EIP170_CODE_SIZE_LIMIT,
+)
+from .opcodes import (
+    SPURIOUS_DRAGON_OPCODES,
+)
 
 
 class SpuriousDragonComputation(HomesteadComputation):
     """
-    A class for all execution computations in the ``SpuriousDragon`` fork.
-    Inherits from :class:`~eth.vm.forks.homestead.computation.HomesteadComputation`
+    A class for all execution *message* computations in the ``SpuriousDragon`` fork.
+    Inherits from
+    :class:`~eth.vm.forks.homestead.computation.HomesteadComputation`
     """
+
     # Override
     opcodes = SPURIOUS_DRAGON_OPCODES
 
     @classmethod
     def apply_create_message(
-            cls,
-            state: StateAPI,
-            message: MessageAPI,
-            transaction_context: TransactionContextAPI) -> ComputationAPI:
-
+        cls,
+        state: StateAPI,
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI,
+    ) -> ComputationAPI:
         snapshot = state.snapshot()
 
         # EIP161 nonce incrementation
         state.increment_nonce(message.storage_address)
 
         cls.validate_create_message(message)
 
@@ -53,15 +62,17 @@
         else:
             contract_code = computation.output
 
             if contract_code:
                 try:
                     cls.validate_contract_code(contract_code)
 
-                    contract_code_gas_cost = len(contract_code) * constants.GAS_CODEDEPOSIT
+                    contract_code_gas_cost = (
+                        len(contract_code) * constants.GAS_CODEDEPOSIT
+                    )
                     computation.consume_gas(
                         contract_code_gas_cost,
                         reason="Write contract code for CREATE",
                     )
                 except VMError as err:
                     # Different from Frontier: reverts state on gas failure while
                     # writing contract code.
@@ -70,15 +81,15 @@
                     cls.logger.debug2(f"VMError setting contract code: {err}")
                 else:
                     if cls.logger:
                         cls.logger.debug2(
                             "SETTING CODE: %s -> length: %s | hash: %s",
                             encode_hex(message.storage_address),
                             len(contract_code),
-                            encode_hex(keccak(contract_code))
+                            encode_hex(keccak(contract_code)),
                         )
 
                     state.set_code(message.storage_address, contract_code)
                     state.commit(snapshot)
             else:
                 state.commit(snapshot)
             return computation
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/opcodes.py` & `py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/opcodes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 import copy
-from typing import Dict
+from typing import (
+    Dict,
+)
 
-from eth_utils.toolz import merge
+from eth_utils.toolz import (
+    merge,
+)
 
-from eth.abc import OpcodeAPI
+from eth.abc import (
+    OpcodeAPI,
+)
+from eth.vm import (
+    mnemonics,
+    opcode_values,
+)
 from eth.vm.forks.tangerine_whistle.constants import (
+    GAS_CALL_EIP150,
     GAS_SELFDESTRUCT_EIP150,
-    GAS_CALL_EIP150
 )
-from eth.vm import mnemonics
-from eth.vm import opcode_values
-from eth.vm.forks.tangerine_whistle.opcodes import TANGERINE_WHISTLE_OPCODES
+from eth.vm.forks.tangerine_whistle.opcodes import (
+    TANGERINE_WHISTLE_OPCODES,
+)
 from eth.vm.logic import (
     arithmetic,
-    system,
     call,
+    system,
+)
+from eth.vm.opcode import (
+    as_opcode,
 )
-from eth.vm.opcode import as_opcode
 
 from .constants import (
     GAS_EXP_EIP160,
-    GAS_EXPBYTE_EIP160
+    GAS_EXPBYTE_EIP160,
 )
 
-
 UPDATED_OPCODES = {
     opcode_values.EXP: as_opcode(
         logic_fn=arithmetic.exp(gas_per_byte=GAS_EXPBYTE_EIP160),
         mnemonic=mnemonics.EXP,
         gas_cost=GAS_EXP_EIP160,
     ),
     opcode_values.SELFDESTRUCT: as_opcode(
         logic_fn=system.selfdestruct_eip161,
         mnemonic=mnemonics.SELFDESTRUCT,
         gas_cost=GAS_SELFDESTRUCT_EIP150,
     ),
     opcode_values.CALL: call.CallEIP161.configure(
-        __name__='opcode:CALL',
+        __name__="opcode:CALL",
         mnemonic=mnemonics.CALL,
         gas_cost=GAS_CALL_EIP150,
     )(),
 }
 
 
 SPURIOUS_DRAGON_OPCODES: Dict[int, OpcodeAPI] = merge(
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/state.py` & `py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/state.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Type
+from typing import (
+    Type,
+)
 
 from eth_utils import (
     encode_hex,
 )
 
 from eth.abc import (
     ComputationAPI,
@@ -10,40 +12,45 @@
     TransactionExecutorAPI,
 )
 from eth.vm.forks.homestead.state import (
     HomesteadState,
     HomesteadTransactionExecutor,
 )
 
-from .computation import SpuriousDragonComputation
-from ._utils import collect_touched_accounts
+from ._utils import (
+    collect_touched_accounts,
+)
+from .computation import (
+    SpuriousDragonComputation,
+)
 
 
 class SpuriousDragonTransactionExecutor(HomesteadTransactionExecutor):
-    def finalize_computation(self,
-                             transaction: SignedTransactionAPI,
-                             computation: ComputationAPI) -> ComputationAPI:
+    def finalize_computation(
+        self, transaction: SignedTransactionAPI, computation: ComputationAPI
+    ) -> ComputationAPI:
         computation = super().finalize_computation(transaction, computation)
 
         #
         # EIP161 state clearing
         #
         touched_accounts = collect_touched_accounts(computation)
 
         for account in touched_accounts:
-            should_delete = (
-                self.vm_state.account_exists(account)
-                and self.vm_state.account_is_empty(account)
-            )
+            should_delete = self.vm_state.account_exists(
+                account
+            ) and self.vm_state.account_is_empty(account)
             if should_delete:
                 self.vm_state.logger.debug2(
                     "CLEARING EMPTY ACCOUNT: %s",
                     encode_hex(account),
                 )
                 self.vm_state.delete_account(account)
 
         return computation
 
 
 class SpuriousDragonState(HomesteadState):
     computation_class: Type[ComputationAPI] = SpuriousDragonComputation
-    transaction_executor_class: Type[TransactionExecutorAPI] = SpuriousDragonTransactionExecutor
+    transaction_executor_class: Type[
+        TransactionExecutorAPI
+    ] = SpuriousDragonTransactionExecutor
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/transactions.py` & `py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/transactions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,76 @@
-from typing import Optional
-
-from eth_keys.datatypes import PrivateKey
+from typing import (
+    Optional,
+)
 
+from eth_keys.datatypes import (
+    PrivateKey,
+)
 from eth_typing import (
     Address,
 )
-
 from eth_utils import (
     int_to_big_endian,
 )
-
 import rlp
 
-from eth.vm.forks.homestead.transactions import (
-    HomesteadTransaction,
-    HomesteadUnsignedTransaction,
+from eth._utils.numeric import (
+    is_even,
 )
-
-from eth._utils.numeric import is_even
 from eth._utils.transactions import (
     create_transaction_signature,
     extract_chain_id,
     is_eip_155_signed_transaction,
 )
+from eth.vm.forks.homestead.transactions import (
+    HomesteadTransaction,
+    HomesteadUnsignedTransaction,
+)
 
 
 class SpuriousDragonTransaction(HomesteadTransaction):
     @property
     def y_parity(self) -> int:
         if is_eip_155_signed_transaction(self):
             return int(is_even(self.v))
         else:
             return super().y_parity
 
     def get_message_for_signing(self) -> bytes:
         if is_eip_155_signed_transaction(self):
             txn_parts = rlp.decode(rlp.encode(self))
-            txn_parts_for_signing = txn_parts[:-3] + [int_to_big_endian(self.chain_id), b'', b'']
+            txn_parts_for_signing = txn_parts[:-3] + [
+                int_to_big_endian(self.chain_id),
+                b"",
+                b"",
+            ]
             return rlp.encode(txn_parts_for_signing)
         else:
-            return rlp.encode(SpuriousDragonUnsignedTransaction(
-                nonce=self.nonce,
-                gas_price=self.gas_price,
-                gas=self.gas,
-                to=self.to,
-                value=self.value,
-                data=self.data,
-            ))
+            return rlp.encode(
+                SpuriousDragonUnsignedTransaction(
+                    nonce=self.nonce,
+                    gas_price=self.gas_price,
+                    gas=self.gas,
+                    to=self.to,
+                    value=self.value,
+                    data=self.data,
+                )
+            )
 
     @classmethod
-    def create_unsigned_transaction(cls,
-                                    *,
-                                    nonce: int,
-                                    gas_price: int,
-                                    gas: int,
-                                    to: Address,
-                                    value: int,
-                                    data: bytes) -> 'SpuriousDragonUnsignedTransaction':
+    def create_unsigned_transaction(
+        cls,
+        *,
+        nonce: int,
+        gas_price: int,
+        gas: int,
+        to: Address,
+        value: int,
+        data: bytes
+    ) -> "SpuriousDragonUnsignedTransaction":
         return SpuriousDragonUnsignedTransaction(nonce, gas_price, gas, to, value, data)
 
     @property
     def chain_id(self) -> Optional[int]:
         if is_eip_155_signed_transaction(self):
             return extract_chain_id(self.v)
         else:
@@ -78,17 +88,17 @@
         if is_eip_155_signed_transaction(self):
             return 36 + (2 * self.chain_id)
         else:
             return 28
 
 
 class SpuriousDragonUnsignedTransaction(HomesteadUnsignedTransaction):
-    def as_signed_transaction(self,
-                              private_key: PrivateKey,
-                              chain_id: int = None) -> SpuriousDragonTransaction:
+    def as_signed_transaction(
+        self, private_key: PrivateKey, chain_id: int = None
+    ) -> SpuriousDragonTransaction:
         v, r, s = create_transaction_signature(self, private_key, chain_id=chain_id)
         return SpuriousDragonTransaction(
             nonce=self.nonce,
             gas_price=self.gas_price,
             gas=self.gas,
             to=self.to,
             value=self.value,
```

### Comparing `py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/opcodes.py` & `py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/opcodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 import copy
 
-from eth_utils.toolz import merge
+from eth_utils.toolz import (
+    merge,
+)
 
-from eth.vm.forks.tangerine_whistle import constants
-from eth.constants import GAS_CREATE
-from eth.vm import opcode_values
-from eth.vm import mnemonics
-from eth.vm.forks.homestead.opcodes import HOMESTEAD_OPCODES
+from eth.constants import (
+    GAS_CREATE,
+)
+from eth.vm import (
+    mnemonics,
+    opcode_values,
+)
+from eth.vm.forks.homestead.opcodes import (
+    HOMESTEAD_OPCODES,
+)
+from eth.vm.forks.tangerine_whistle import (
+    constants,
+)
 from eth.vm.logic import (
     call,
     context,
     storage,
     system,
 )
-from eth.vm.opcode import as_opcode
-
+from eth.vm.opcode import (
+    as_opcode,
+)
 
 UPDATED_OPCODES = {
     opcode_values.EXTCODESIZE: as_opcode(
         logic_fn=context.extcodesize,
         mnemonic=mnemonics.EXTCODESIZE,
         gas_cost=constants.GAS_EXTCODE_EIP150,
     ),
@@ -39,30 +50,30 @@
     ),
     opcode_values.SELFDESTRUCT: as_opcode(
         logic_fn=system.selfdestruct_eip150,
         mnemonic=mnemonics.SELFDESTRUCT,
         gas_cost=constants.GAS_SELFDESTRUCT_EIP150,
     ),
     opcode_values.CREATE: system.CreateEIP150.configure(
-        __name__='opcode:CREATE',
+        __name__="opcode:CREATE",
         mnemonic=mnemonics.CREATE,
         gas_cost=GAS_CREATE,
     )(),
     opcode_values.CALL: call.CallEIP150.configure(
-        __name__='opcode:CALL',
+        __name__="opcode:CALL",
         mnemonic=mnemonics.CALL,
         gas_cost=constants.GAS_CALL_EIP150,
     )(),
     opcode_values.CALLCODE: call.CallCodeEIP150.configure(
-        __name__='opcode:CALLCODE',
+        __name__="opcode:CALLCODE",
         mnemonic=mnemonics.CALLCODE,
         gas_cost=constants.GAS_CALL_EIP150,
     )(),
     opcode_values.DELEGATECALL: call.DelegateCallEIP150.configure(
-        __name__='opcode:DELEGATECALL',
+        __name__="opcode:DELEGATECALL",
         mnemonic=mnemonics.DELEGATECALL,
         gas_cost=constants.GAS_CALL_EIP150,
     )(),
 }
 
 
 TANGERINE_WHISTLE_OPCODES = merge(
```

### Comparing `py-evm-0.7.0a1/eth/vm/gas_meter.py` & `py-evm-0.7.0a2/eth/vm/gas_meter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import (
     Callable,
 )
+
 from eth_utils import (
     ValidationError,
     get_extended_debug_logger,
 )
 
-from eth.abc import GasMeterAPI
+from eth.abc import (
+    GasMeterAPI,
+)
 from eth.exceptions import (
     OutOfGas,
 )
 from eth.validation import (
     validate_uint256,
 )
 
@@ -26,25 +29,24 @@
     return gas_refunded_total + amount
 
 
 RefundStrategy = Callable[[int, int], int]
 
 
 class GasMeter(GasMeterAPI):
-
     start_gas: int = None
 
     gas_refunded: int = None
     gas_remaining: int = None
 
-    logger = get_extended_debug_logger('eth.gas.GasMeter')
+    logger = get_extended_debug_logger("eth.gas.GasMeter")
 
-    def __init__(self,
-                 start_gas: int,
-                 refund_strategy: RefundStrategy = default_refund_strategy) -> None:
+    def __init__(
+        self, start_gas: int, refund_strategy: RefundStrategy = default_refund_strategy
+    ) -> None:
         validate_uint256(start_gas, title="Start Gas")
 
         self.refund_strategy = refund_strategy
         self.start_gas = start_gas
 
         self.gas_remaining = self.start_gas
         self.gas_refunded = 0
@@ -63,38 +65,38 @@
                 f"- Reason: {reason}"
             )
 
         self.gas_remaining -= amount
 
         if self.logger.show_debug2:
             self.logger.debug2(
-                'GAS CONSUMPTION: %s - %s -> %s (%s)',
+                "GAS CONSUMPTION: %s - %s -> %s (%s)",
                 self.gas_remaining + amount,
                 amount,
                 self.gas_remaining,
                 reason,
             )
 
     def return_gas(self, amount: int) -> None:
         if amount < 0:
             raise ValidationError("Gas return amount must be positive")
 
         self.gas_remaining += amount
 
         if self.logger.show_debug2:
             self.logger.debug2(
-                'GAS RETURNED: %s + %s -> %s',
+                "GAS RETURNED: %s + %s -> %s",
                 self.gas_remaining - amount,
                 amount,
                 self.gas_remaining,
             )
 
     def refund_gas(self, amount: int) -> None:
         self.gas_refunded = self.refund_strategy(self.gas_refunded, amount)
 
         if self.logger.show_debug2:
             self.logger.debug2(
-                'GAS REFUND: %s + %s -> %s',
+                "GAS REFUND: %s + %s -> %s",
                 self.gas_refunded - amount,
                 amount,
                 self.gas_refunded,
             )
```

### Comparing `py-evm-0.7.0a1/eth/vm/interrupt.py` & `py-evm-0.7.0a2/eth/vm/interrupt.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     pass
 
 
 class MissingAccountTrieNode(EVMMissingData, MissingTrieNode):
     """
     Raised when a main state trie node is missing from the DB, to get an account RLP
     """
+
     @property
     def state_root_hash(self) -> Hash32:
         return self.root_hash
 
     @property
     def address_hash(self) -> Hash32:
         return self.requested_key
@@ -51,22 +52,24 @@
         )
 
 
 class MissingStorageTrieNode(EVMMissingData, MissingTrieNode):
     """
     Raised when a storage trie node is missing from the DB
     """
+
     def __init__(
-            self,
-            missing_node_hash: Hash32,
-            storage_root_hash: Hash32,
-            requested_key: Hash32,
-            prefix: Optional[Nibbles],
-            account_address: Address,
-            *args: bytes) -> None:
+        self,
+        missing_node_hash: Hash32,
+        storage_root_hash: Hash32,
+        requested_key: Hash32,
+        prefix: Optional[Nibbles],
+        account_address: Address,
+        *args: bytes,
+    ) -> None:
         if not isinstance(account_address, bytes):
             raise TypeError(f"Account address must be bytes, was: {account_address!r}")
 
         super().__init__(
             missing_node_hash,
             storage_root_hash,
             requested_key,
@@ -98,17 +101,20 @@
         )
 
 
 class MissingBytecode(EVMMissingData):
     """
     Raised when the bytecode is missing from the database for a known bytecode hash.
     """
+
     def __init__(self, missing_code_hash: Hash32) -> None:
         if not isinstance(missing_code_hash, bytes):
-            raise TypeError(f"Missing code hash must be bytes, was: {missing_code_hash!r}")
+            raise TypeError(
+                f"Missing code hash must be bytes, was: {missing_code_hash!r}"
+            )
 
         super().__init__(missing_code_hash)
 
     @property
     def missing_code_hash(self) -> Hash32:
         return self.args[0]
```

### Comparing `py-evm-0.7.0a1/eth/vm/logic/arithmetic.py` & `py-evm-0.7.0a2/eth/vm/logic/arithmetic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,75 @@
 from eth_utils.toolz import (
     curry,
 )
 
-from eth import constants
-
+from eth import (
+    constants,
+)
 from eth._utils.numeric import (
-    unsigned_to_signed,
-    signed_to_unsigned,
     ceil8,
+    signed_to_unsigned,
+    unsigned_to_signed,
+)
+from eth.abc import (
+    ComputationAPI,
 )
-
-from eth.vm.computation import BaseComputation
 
 
-def add(computation: BaseComputation) -> None:
+def add(computation: ComputationAPI) -> None:
     """
     Addition
     """
     left, right = computation.stack_pop_ints(2)
 
     result = (left + right) & constants.UINT_256_MAX
 
     computation.stack_push_int(result)
 
 
-def addmod(computation: BaseComputation) -> None:
+def addmod(computation: ComputationAPI) -> None:
     """
     Modulo Addition
     """
     left, right, mod = computation.stack_pop_ints(3)
 
     if mod == 0:
         result = 0
     else:
         result = (left + right) % mod
 
     computation.stack_push_int(result)
 
 
-def sub(computation: BaseComputation) -> None:
+def sub(computation: ComputationAPI) -> None:
     """
     Subtraction
     """
     left, right = computation.stack_pop_ints(2)
 
     result = (left - right) & constants.UINT_256_MAX
 
     computation.stack_push_int(result)
 
 
-def mod(computation: BaseComputation) -> None:
+def mod(computation: ComputationAPI) -> None:
     """
     Modulo
     """
     value, mod = computation.stack_pop_ints(2)
 
     if mod == 0:
         result = 0
     else:
         result = value % mod
 
     computation.stack_push_int(result)
 
 
-def smod(computation: BaseComputation) -> None:
+def smod(computation: ComputationAPI) -> None:
     """
     Signed Modulo
     """
     value, mod = map(
         unsigned_to_signed,
         computation.stack_pop_ints(2),
     )
@@ -78,73 +80,73 @@
         result = 0
     else:
         result = (abs(value) % abs(mod) * pos_or_neg) & constants.UINT_256_MAX
 
     computation.stack_push_int(signed_to_unsigned(result))
 
 
-def mul(computation: BaseComputation) -> None:
+def mul(computation: ComputationAPI) -> None:
     """
     Multiplication
     """
     left, right = computation.stack_pop_ints(2)
 
     result = (left * right) & constants.UINT_256_MAX
 
     computation.stack_push_int(result)
 
 
-def mulmod(computation: BaseComputation) -> None:
+def mulmod(computation: ComputationAPI) -> None:
     """
     Modulo Multiplication
     """
     left, right, mod = computation.stack_pop_ints(3)
 
     if mod == 0:
         result = 0
     else:
         result = (left * right) % mod
     computation.stack_push_int(result)
 
 
-def div(computation: BaseComputation) -> None:
+def div(computation: ComputationAPI) -> None:
     """
     Division
     """
     numerator, denominator = computation.stack_pop_ints(2)
 
     if denominator == 0:
         result = 0
     else:
         result = (numerator // denominator) & constants.UINT_256_MAX
 
     computation.stack_push_int(result)
 
 
-def sdiv(computation: BaseComputation) -> None:
+def sdiv(computation: ComputationAPI) -> None:
     """
     Signed Division
     """
     numerator, denominator = map(
         unsigned_to_signed,
         computation.stack_pop_ints(2),
     )
 
     pos_or_neg = -1 if numerator * denominator < 0 else 1
 
     if denominator == 0:
         result = 0
     else:
-        result = (pos_or_neg * (abs(numerator) // abs(denominator)))
+        result = pos_or_neg * (abs(numerator) // abs(denominator))
 
     computation.stack_push_int(signed_to_unsigned(result))
 
 
 @curry
-def exp(computation: BaseComputation, gas_per_byte: int) -> None:
+def exp(computation: ComputationAPI, gas_per_byte: int) -> None:
     """
     Exponentiation
     """
     base, exponent = computation.stack_pop_ints(2)
 
     bit_size = exponent.bit_length()
     byte_size = ceil8(bit_size) // 8
@@ -160,62 +162,62 @@
         gas_per_byte * byte_size,
         reason="EXP: exponent bytes",
     )
 
     computation.stack_push_int(result)
 
 
-def signextend(computation: BaseComputation) -> None:
+def signextend(computation: ComputationAPI) -> None:
     """
     Signed Extend
     """
     bits, value = computation.stack_pop_ints(2)
 
     if bits <= 31:
         testbit = bits * 8 + 7
-        sign_bit = (1 << testbit)
+        sign_bit = 1 << testbit
         if value & sign_bit:
             result = value | (constants.UINT_256_CEILING - sign_bit)
         else:
             result = value & (sign_bit - 1)
     else:
         result = value
 
     computation.stack_push_int(result)
 
 
-def shl(computation: BaseComputation) -> None:
+def shl(computation: ComputationAPI) -> None:
     """
     Bitwise left shift
     """
     shift_length, value = computation.stack_pop_ints(2)
 
     if shift_length >= 256:
         result = 0
     else:
         result = (value << shift_length) & constants.UINT_256_MAX
 
     computation.stack_push_int(result)
 
 
-def shr(computation: BaseComputation) -> None:
+def shr(computation: ComputationAPI) -> None:
     """
     Bitwise right shift
     """
     shift_length, value = computation.stack_pop_ints(2)
 
     if shift_length >= 256:
         result = 0
     else:
         result = (value >> shift_length) & constants.UINT_256_MAX
 
     computation.stack_push_int(result)
 
 
-def sar(computation: BaseComputation) -> None:
+def sar(computation: ComputationAPI) -> None:
     """
     Arithmetic bitwise right shift
     """
     shift_length, value = computation.stack_pop_ints(2)
     value = unsigned_to_signed(value)
 
     if shift_length >= 256:
```

### Comparing `py-evm-0.7.0a1/eth/vm/logic/call.py` & `py-evm-0.7.0a2/eth/vm/logic/call.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,63 @@
 from abc import (
     ABC,
-    abstractmethod
+    abstractmethod,
 )
-
 from typing import (
     Tuple,
 )
 
-from eth import constants
-
 from eth_typing import (
     Address,
 )
 
+from eth import (
+    constants,
+)
+from eth._utils.address import (
+    force_bytes_to_address,
+)
 from eth.abc import (
     ComputationAPI,
 )
 from eth.exceptions import (
     OutOfGas,
     WriteProtection,
 )
 from eth.vm.opcode import (
     Opcode,
 )
 
-from eth._utils.address import (
-    force_bytes_to_address,
-)
-
-
 CallParams = Tuple[int, int, Address, Address, Address, int, int, int, int, bool, bool]
 
 
 class BaseCall(Opcode, ABC):
     @abstractmethod
-    def compute_msg_extra_gas(self,
-                              computation: ComputationAPI,
-                              gas: int,
-                              to: Address,
-                              value: int) -> int:
+    def compute_msg_extra_gas(
+        self, computation: ComputationAPI, gas: int, to: Address, value: int
+    ) -> int:
         raise NotImplementedError("Must be implemented by subclasses")
 
     @abstractmethod
     def get_call_params(self, computation: ComputationAPI) -> CallParams:
         raise NotImplementedError("Must be implemented by subclasses")
 
-    def compute_msg_gas(self,
-                        computation: ComputationAPI,
-                        gas: int,
-                        to: Address,
-                        value: int) -> Tuple[int, int]:
+    def compute_msg_gas(
+        self, computation: ComputationAPI, gas: int, to: Address, value: int
+    ) -> Tuple[int, int]:
         extra_gas = self.compute_msg_extra_gas(computation, gas, to, value)
         total_fee = gas + extra_gas
         child_msg_gas = gas + (constants.GAS_CALLSTIPEND if value else 0)
         return child_msg_gas, total_fee
 
-    def get_account_load_fee(self, computation: ComputationAPI, code_address: Address) -> int:
+    def get_account_load_fee(
+        self,
+        computation: ComputationAPI,
+        code_address: Address,
+    ) -> int:
         """
         Return the gas cost for implicitly loading the account needed to access
         the bytecode.
         """
         return 0
 
     def __call__(self, computation: ComputationAPI) -> None:
@@ -81,54 +79,58 @@
             should_transfer_value,
             is_static,
         ) = self.get_call_params(computation)
 
         computation.extend_memory(memory_input_start_position, memory_input_size)
         computation.extend_memory(memory_output_start_position, memory_output_size)
 
-        call_data = computation.memory_read(memory_input_start_position, memory_input_size)
+        call_data = computation.memory_read(
+            memory_input_start_position, memory_input_size
+        )
 
         #
         # Message gas allocation and fees
         #
         if code_address:
             code_source = code_address
         else:
             code_source = to
         load_account_fee = self.get_account_load_fee(computation, code_source)
         if load_account_fee > 0:
             computation.consume_gas(
                 load_account_fee,
-                reason=f"{self.mnemonic} charges implicit account load for reading code",
+                reason=f"{self.mnemonic} charges implicit account load for reading code",  # noqa: E501
             )
             if self.logger.show_debug2:
                 self.logger.debug2(
                     "%s is charged %d for invoking code at account 0x%s",
                     self.mnemonic,
                     load_account_fee,
                     code_source.hex(),
                 )
 
         # This must be computed *after* the load account fee is charged, so
         # that the 63/64ths rule is applied against the reduced remaining gas.
-        child_msg_gas, child_msg_gas_fee = self.compute_msg_gas(computation, gas, to, value)
+        child_msg_gas, child_msg_gas_fee = self.compute_msg_gas(
+            computation, gas, to, value
+        )
         computation.consume_gas(child_msg_gas_fee, reason=self.mnemonic)
 
         # Pre-call checks
-        sender_balance = computation.state.get_balance(
-            computation.msg.storage_address
-        )
+        sender_balance = computation.state.get_balance(computation.msg.storage_address)
 
         insufficient_funds = should_transfer_value and sender_balance < value
         stack_too_deep = computation.msg.depth + 1 > constants.STACK_DEPTH_LIMIT
 
         if insufficient_funds or stack_too_deep:
-            computation.return_data = b''
+            computation.return_data = b""
             if insufficient_funds:
-                err_message = f"Insufficient Funds: have: {sender_balance} | need: {value}"
+                err_message = (
+                    f"Insufficient Funds: have: {sender_balance} | need: {value}"
+                )
             elif stack_too_deep:
                 err_message = "Stack Limit Reached"
             else:
                 raise Exception("Invariant: Unreachable code path")
 
             self.logger.debug2(
                 "%s failure: %s",
@@ -140,54 +142,54 @@
         else:
             if code_address:
                 code = computation.state.get_code(code_address)
             else:
                 code = computation.state.get_code(to)
 
             child_msg_kwargs = {
-                'gas': child_msg_gas,
-                'value': value,
-                'to': to,
-                'data': call_data,
-                'code': code,
-                'code_address': code_address,
-                'should_transfer_value': should_transfer_value,
-                'is_static': is_static,
+                "gas": child_msg_gas,
+                "value": value,
+                "to": to,
+                "data": call_data,
+                "code": code,
+                "code_address": code_address,
+                "should_transfer_value": should_transfer_value,
+                "is_static": is_static,
             }
             if sender is not None:
-                child_msg_kwargs['sender'] = sender
+                child_msg_kwargs["sender"] = sender
 
             # TODO: after upgrade to py3.6, use a TypedDict and try again
-            child_msg = computation.prepare_child_message(**child_msg_kwargs)  # type: ignore
+            child_msg = computation.prepare_child_message(**child_msg_kwargs)  # type: ignore  # noqa: E501
 
             child_computation = computation.apply_child_computation(child_msg)
 
             if child_computation.is_error:
                 computation.stack_push_int(0)
             else:
                 computation.stack_push_int(1)
 
             if not child_computation.should_erase_return_data:
-                actual_output_size = min(memory_output_size, len(child_computation.output))
+                actual_output_size = min(
+                    memory_output_size, len(child_computation.output)
+                )
                 computation.memory_write(
                     memory_output_start_position,
                     actual_output_size,
                     child_computation.output[:actual_output_size],
                 )
 
             if child_computation.should_return_gas:
                 computation.return_gas(child_computation.get_gas_remaining())
 
 
 class Call(BaseCall):
-    def compute_msg_extra_gas(self,
-                              computation: ComputationAPI,
-                              gas: int,
-                              to: Address,
-                              value: int) -> int:
+    def compute_msg_extra_gas(
+        self, computation: ComputationAPI, gas: int, to: Address, value: int
+    ) -> int:
         account_exists = computation.state.account_exists(to)
 
         transfer_gas_fee = constants.GAS_CALLVALUE if value else 0
         create_gas_fee = constants.GAS_NEWACCOUNT if not account_exists else 0
         return transfer_gas_fee + create_gas_fee
 
     def get_call_params(self, computation: ComputationAPI) -> CallParams:
@@ -214,19 +216,17 @@
             memory_output_size,
             True,  # should_transfer_value,
             computation.msg.is_static,
         )
 
 
 class CallCode(BaseCall):
-    def compute_msg_extra_gas(self,
-                              computation: ComputationAPI,
-                              gas: int,
-                              to: Address,
-                              value: int) -> int:
+    def compute_msg_extra_gas(
+        self, computation: ComputationAPI, gas: int, to: Address, value: int
+    ) -> int:
         return constants.GAS_CALLVALUE if value else 0
 
     def get_call_params(self, computation: ComputationAPI) -> CallParams:
         gas = computation.stack_pop1_int()
         code_address = force_bytes_to_address(computation.stack_pop1_bytes())
 
         (
@@ -252,26 +252,22 @@
             memory_output_size,
             True,  # should_transfer_value,
             computation.msg.is_static,
         )
 
 
 class DelegateCall(BaseCall):
-    def compute_msg_gas(self,
-                        computation: ComputationAPI,
-                        gas: int,
-                        to: Address,
-                        value: int) -> Tuple[int, int]:
+    def compute_msg_gas(
+        self, computation: ComputationAPI, gas: int, to: Address, value: int
+    ) -> Tuple[int, int]:
         return gas, gas
 
-    def compute_msg_extra_gas(self,
-                              computation: ComputationAPI,
-                              gas: int,
-                              to: Address,
-                              value: int) -> int:
+    def compute_msg_extra_gas(
+        self, computation: ComputationAPI, gas: int, to: Address, value: int
+    ) -> int:
         return 0
 
     def get_call_params(self, computation: ComputationAPI) -> CallParams:
         gas = computation.stack_pop1_int()
         code_address = force_bytes_to_address(computation.stack_pop1_bytes())
 
         (
@@ -300,105 +296,96 @@
         )
 
 
 #
 # EIP150
 #
 class CallEIP150(Call):
-    def compute_msg_gas(self,
-                        computation: ComputationAPI,
-                        gas: int,
-                        to: Address,
-                        value: int) -> Tuple[int, int]:
+    def compute_msg_gas(
+        self, computation: ComputationAPI, gas: int, to: Address, value: int
+    ) -> Tuple[int, int]:
         extra_gas = self.compute_msg_extra_gas(computation, gas, to, value)
         return compute_eip150_msg_gas(
             computation=computation,
             gas=gas,
             extra_gas=extra_gas,
             value=value,
             mnemonic=self.mnemonic,
-            callstipend=constants.GAS_CALLSTIPEND
+            callstipend=constants.GAS_CALLSTIPEND,
         )
 
 
 class CallCodeEIP150(CallCode):
-    def compute_msg_gas(self,
-                        computation: ComputationAPI,
-                        gas: int,
-                        to: Address,
-                        value: int) -> Tuple[int, int]:
+    def compute_msg_gas(
+        self, computation: ComputationAPI, gas: int, to: Address, value: int
+    ) -> Tuple[int, int]:
         extra_gas = self.compute_msg_extra_gas(computation, gas, to, value)
         return compute_eip150_msg_gas(
             computation=computation,
             gas=gas,
             extra_gas=extra_gas,
             value=value,
             mnemonic=self.mnemonic,
-            callstipend=constants.GAS_CALLSTIPEND
+            callstipend=constants.GAS_CALLSTIPEND,
         )
 
 
 class DelegateCallEIP150(DelegateCall):
-    def compute_msg_gas(self,
-                        computation: ComputationAPI,
-                        gas: int,
-                        to: Address,
-                        value: int) -> Tuple[int, int]:
+    def compute_msg_gas(
+        self, computation: ComputationAPI, gas: int, to: Address, value: int
+    ) -> Tuple[int, int]:
         extra_gas = self.compute_msg_extra_gas(computation, gas, to, value)
         callstipend = 0
         return compute_eip150_msg_gas(
             computation=computation,
             gas=gas,
             extra_gas=extra_gas,
             value=value,
             mnemonic=self.mnemonic,
-            callstipend=callstipend
+            callstipend=callstipend,
         )
 
 
 def max_child_gas_eip150(gas: int) -> int:
     return gas - (gas // 64)
 
 
-def compute_eip150_msg_gas(*,
-                           computation: ComputationAPI,
-                           gas: int,
-                           extra_gas: int,
-                           value: int,
-                           mnemonic: str,
-                           callstipend: int) -> Tuple[int, int]:
+def compute_eip150_msg_gas(
+    *,
+    computation: ComputationAPI,
+    gas: int,
+    extra_gas: int,
+    value: int,
+    mnemonic: str,
+    callstipend: int,
+) -> Tuple[int, int]:
     if computation.get_gas_remaining() < extra_gas:
         # It feels wrong to raise an OutOfGas exception outside of GasMeter,
         # but I don't see an easy way around it.
         raise OutOfGas(
             f"Out of gas: Needed {extra_gas}"
             f" - Remaining {computation.get_gas_remaining()}"
             f" - Reason: {mnemonic}"
         )
-    gas = min(
-        gas,
-        max_child_gas_eip150(computation.get_gas_remaining() - extra_gas))
+    gas = min(gas, max_child_gas_eip150(computation.get_gas_remaining() - extra_gas))
     total_fee = gas + extra_gas
     child_msg_gas = gas + (callstipend if value else 0)
     return child_msg_gas, total_fee
 
 
 #
 # EIP161
 #
 class CallEIP161(CallEIP150):
-    def compute_msg_extra_gas(self,
-                              computation: ComputationAPI,
-                              gas: int,
-                              to: Address,
-                              value: int) -> int:
-        account_is_dead = (
-            not computation.state.account_exists(to)
-            or computation.state.account_is_empty(to)
-        )
+    def compute_msg_extra_gas(
+        self, computation: ComputationAPI, gas: int, to: Address, value: int
+    ) -> int:
+        account_is_dead = not computation.state.account_exists(
+            to
+        ) or computation.state.account_is_empty(to)
 
         transfer_gas_fee = constants.GAS_CALLVALUE if value else 0
         create_gas_fee = constants.GAS_NEWACCOUNT if (account_is_dead and value) else 0
         return transfer_gas_fee + create_gas_fee
 
 
 #
@@ -432,9 +419,11 @@
 
 
 class CallByzantium(CallEIP161):
     def get_call_params(self, computation: ComputationAPI) -> CallParams:
         call_params = super().get_call_params(computation)
         value = call_params[1]
         if computation.msg.is_static and value != 0:
-            raise WriteProtection("Cannot modify state while inside of a STATICCALL context")
+            raise WriteProtection(
+                "Cannot modify state while inside of a STATICCALL context"
+            )
         return call_params
```

### Comparing `py-evm-0.7.0a1/eth/vm/logic/comparison.py` & `py-evm-0.7.0a2/eth/vm/logic/comparison.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-from eth import constants
-
+from eth import (
+    constants,
+)
 from eth._utils.numeric import (
     signed_to_unsigned,
     unsigned_to_signed,
 )
-
-from eth.vm.computation import BaseComputation
+from eth.abc import (
+    ComputationAPI,
+)
 
 
-def lt(computation: BaseComputation) -> None:
+def lt(computation: ComputationAPI) -> None:
     """
     Lesser Comparison
     """
     left, right = computation.stack_pop_ints(2)
 
     if left < right:
         result = 1
     else:
         result = 0
 
     computation.stack_push_int(result)
 
 
-def gt(computation: BaseComputation) -> None:
+def gt(computation: ComputationAPI) -> None:
     """
     Greater Comparison
     """
     left, right = computation.stack_pop_ints(2)
 
     if left > right:
         result = 1
     else:
         result = 0
 
     computation.stack_push_int(result)
 
 
-def slt(computation: BaseComputation) -> None:
+def slt(computation: ComputationAPI) -> None:
     """
     Signed Lesser Comparison
     """
     left, right = map(
         unsigned_to_signed,
         computation.stack_pop_ints(2),
     )
@@ -49,15 +51,15 @@
         result = 1
     else:
         result = 0
 
     computation.stack_push_int(signed_to_unsigned(result))
 
 
-def sgt(computation: BaseComputation) -> None:
+def sgt(computation: ComputationAPI) -> None:
     """
     Signed Greater Comparison
     """
     left, right = map(
         unsigned_to_signed,
         computation.stack_pop_ints(2),
     )
@@ -66,87 +68,87 @@
         result = 1
     else:
         result = 0
 
     computation.stack_push_int(signed_to_unsigned(result))
 
 
-def eq(computation: BaseComputation) -> None:
+def eq(computation: ComputationAPI) -> None:
     """
     Equality
     """
     left, right = computation.stack_pop_ints(2)
 
     if left == right:
         result = 1
     else:
         result = 0
 
     computation.stack_push_int(result)
 
 
-def iszero(computation: BaseComputation) -> None:
+def iszero(computation: ComputationAPI) -> None:
     """
     Not
     """
     value = computation.stack_pop1_int()
 
     if value == 0:
         result = 1
     else:
         result = 0
 
     computation.stack_push_int(result)
 
 
-def and_op(computation: BaseComputation) -> None:
+def and_op(computation: ComputationAPI) -> None:
     """
     Bitwise And
     """
     left, right = computation.stack_pop_ints(2)
 
     result = left & right
 
     computation.stack_push_int(result)
 
 
-def or_op(computation: BaseComputation) -> None:
+def or_op(computation: ComputationAPI) -> None:
     """
     Bitwise Or
     """
     left, right = computation.stack_pop_ints(2)
 
     result = left | right
 
     computation.stack_push_int(result)
 
 
-def xor(computation: BaseComputation) -> None:
+def xor(computation: ComputationAPI) -> None:
     """
     Bitwise XOr
     """
     left, right = computation.stack_pop_ints(2)
 
     result = left ^ right
 
     computation.stack_push_int(result)
 
 
-def not_op(computation: BaseComputation) -> None:
+def not_op(computation: ComputationAPI) -> None:
     """
     Not
     """
     value = computation.stack_pop1_int()
 
     result = constants.UINT_256_MAX - value
 
     computation.stack_push_int(result)
 
 
-def byte_op(computation: BaseComputation) -> None:
+def byte_op(computation: ComputationAPI) -> None:
     """
     Bitwise And
     """
     position, value = computation.stack_pop_ints(2)
 
     if position >= 32:
         result = 0
```

### Comparing `py-evm-0.7.0a1/eth/vm/logic/context.py` & `py-evm-0.7.0a2/eth/vm/logic/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-from typing import Tuple
+from typing import (
+    Tuple,
+)
 
 from eth_typing import (
     Address,
 )
 
-from eth import constants
-
-from eth.abc import (
-    ComputationAPI,
+from eth import (
+    constants,
 )
-from eth.exceptions import (
-    OutOfBoundsRead,
-)
-
 from eth._utils.address import (
     force_bytes_to_address,
 )
 from eth._utils.numeric import (
     ceil32,
 )
-
-from eth.vm.computation import BaseComputation
+from eth.abc import (
+    ComputationAPI,
+)
+from eth.exceptions import (
+    OutOfBoundsRead,
+)
 
 
-def balance(computation: BaseComputation) -> None:
+def balance(computation: ComputationAPI) -> None:
     addr = force_bytes_to_address(computation.stack_pop1_bytes())
     push_balance_of_address(addr, computation)
 
 
-def selfbalance(computation: BaseComputation) -> None:
+def selfbalance(computation: ComputationAPI) -> None:
     push_balance_of_address(computation.msg.storage_address, computation)
 
 
 def push_balance_of_address(address: Address, computation: ComputationAPI) -> None:
     balance = computation.state.get_balance(address)
     computation.stack_push_int(balance)
 
 
-def origin(computation: BaseComputation) -> None:
+def origin(computation: ComputationAPI) -> None:
     computation.stack_push_bytes(computation.transaction_context.origin)
 
 
-def address(computation: BaseComputation) -> None:
+def address(computation: ComputationAPI) -> None:
     computation.stack_push_bytes(computation.msg.storage_address)
 
 
-def caller(computation: BaseComputation) -> None:
+def caller(computation: ComputationAPI) -> None:
     computation.stack_push_bytes(computation.msg.sender)
 
 
-def callvalue(computation: BaseComputation) -> None:
+def callvalue(computation: ComputationAPI) -> None:
     computation.stack_push_int(computation.msg.value)
 
 
-def calldataload(computation: BaseComputation) -> None:
+def calldataload(computation: ComputationAPI) -> None:
     """
     Load call data into memory.
     """
     start_position = computation.stack_pop1_int()
 
-    value = computation.msg.data_as_bytes[start_position:start_position + 32]
-    padded_value = value.ljust(32, b'\x00')
-    normalized_value = padded_value.lstrip(b'\x00')
+    value = computation.msg.data_as_bytes[start_position : start_position + 32]
+    padded_value = value.ljust(32, b"\x00")
+    normalized_value = padded_value.lstrip(b"\x00")
 
     computation.stack_push_bytes(normalized_value)
 
 
-def calldatasize(computation: BaseComputation) -> None:
+def calldatasize(computation: ComputationAPI) -> None:
     size = len(computation.msg.data)
     computation.stack_push_int(size)
 
 
-def calldatacopy(computation: BaseComputation) -> None:
+def calldatacopy(computation: ComputationAPI) -> None:
     (
         mem_start_position,
         calldata_start_position,
         size,
     ) = computation.stack_pop_ints(3)
 
     computation.extend_memory(mem_start_position, size)
 
     word_count = ceil32(size) // 32
     copy_gas_cost = word_count * constants.GAS_COPY
 
     computation.consume_gas(copy_gas_cost, reason="CALLDATACOPY fee")
 
     value = computation.msg.data_as_bytes[
-        calldata_start_position: calldata_start_position + size
+        calldata_start_position : calldata_start_position + size
     ]
-    padded_value = value.ljust(size, b'\x00')
+    padded_value = value.ljust(size, b"\x00")
 
     computation.memory_write(mem_start_position, size, padded_value)
 
 
-def chain_id(computation: BaseComputation) -> None:
+def chain_id(computation: ComputationAPI) -> None:
     computation.stack_push_int(computation.state.execution_context.chain_id)
 
 
-def codesize(computation: BaseComputation) -> None:
+def codesize(computation: ComputationAPI) -> None:
     size = len(computation.code)
     computation.stack_push_int(size)
 
 
-def codecopy(computation: BaseComputation) -> None:
+def codecopy(computation: ComputationAPI) -> None:
     (
         mem_start_position,
         code_start_position,
         size,
     ) = computation.stack_pop_ints(3)
 
     computation.extend_memory(mem_start_position, size)
@@ -118,24 +118,24 @@
         copy_gas_cost,
         reason="CODECOPY: word gas cost",
     )
 
     with computation.code.seek(code_start_position):
         code_bytes = computation.code.read(size)
 
-    padded_code_bytes = code_bytes.ljust(size, b'\x00')
+    padded_code_bytes = code_bytes.ljust(size, b"\x00")
 
     computation.memory_write(mem_start_position, size, padded_code_bytes)
 
 
-def gasprice(computation: BaseComputation) -> None:
+def gasprice(computation: ComputationAPI) -> None:
     computation.stack_push_int(computation.transaction_context.gas_price)
 
 
-def extcodesize(computation: BaseComputation) -> None:
+def extcodesize(computation: ComputationAPI) -> None:
     account = force_bytes_to_address(computation.stack_pop1_bytes())
     code_size = len(computation.state.get_code(account))
 
     computation.stack_push_int(code_size)
 
 
 def extcodecopy_execute(computation: ComputationAPI) -> Tuple[Address, int]:
@@ -151,56 +151,56 @@
         size,
     ) = computation.stack_pop_ints(3)
 
     computation.extend_memory(mem_start_position, size)
 
     code = computation.state.get_code(account)
 
-    code_bytes = code[code_start_position:code_start_position + size]
-    padded_code_bytes = code_bytes.ljust(size, b'\x00')
+    code_bytes = code[code_start_position : code_start_position + size]
+    padded_code_bytes = code_bytes.ljust(size, b"\x00")
 
     computation.memory_write(mem_start_position, size, padded_code_bytes)
 
     return account, size
 
 
 def consume_extcodecopy_word_cost(computation: ComputationAPI, size: int) -> None:
     word_count = ceil32(size) // 32
     copy_gas_cost = constants.GAS_COPY * word_count
     computation.consume_gas(
         copy_gas_cost,
-        reason='EXTCODECOPY: word gas cost',
+        reason="EXTCODECOPY: word gas cost",
     )
 
 
-def extcodecopy(computation: BaseComputation) -> None:
+def extcodecopy(computation: ComputationAPI) -> None:
     _address, size = extcodecopy_execute(computation)
     consume_extcodecopy_word_cost(computation, size)
 
 
-def extcodehash(computation: BaseComputation) -> None:
+def extcodehash(computation: ComputationAPI) -> None:
     """
     Return the code hash for a given address.
     EIP: https://github.com/ethereum/EIPs/blob/master/EIPS/eip-1052.md
     """
     account = force_bytes_to_address(computation.stack_pop1_bytes())
     state = computation.state
 
     if state.account_is_empty(account):
         computation.stack_push_bytes(constants.NULL_BYTE)
     else:
         computation.stack_push_bytes(state.get_code_hash(account))
 
 
-def returndatasize(computation: BaseComputation) -> None:
+def returndatasize(computation: ComputationAPI) -> None:
     size = len(computation.return_data)
     computation.stack_push_int(size)
 
 
-def returndatacopy(computation: BaseComputation) -> None:
+def returndatacopy(computation: ComputationAPI) -> None:
     (
         mem_start_position,
         returndata_start_position,
         size,
     ) = computation.stack_pop_ints(3)
 
     if returndata_start_position + size > len(computation.return_data):
@@ -214,10 +214,12 @@
     computation.extend_memory(mem_start_position, size)
 
     word_count = ceil32(size) // 32
     copy_gas_cost = word_count * constants.GAS_COPY
 
     computation.consume_gas(copy_gas_cost, reason="RETURNDATACOPY fee")
 
-    value = computation.return_data[returndata_start_position: returndata_start_position + size]
+    value = computation.return_data[
+        returndata_start_position : returndata_start_position + size
+    ]
 
     computation.memory_write(mem_start_position, size, value)
```

### Comparing `py-evm-0.7.0a1/eth/vm/logic/duplication.py` & `py-evm-0.7.0a2/eth/vm/logic/duplication.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import functools
 
-from eth.vm.computation import BaseComputation
+from eth.abc import (
+    ComputationAPI,
+)
 
 
-def dup_XX(computation: BaseComputation, position: int) -> None:
+def dup_XX(computation: ComputationAPI, position: int) -> None:
     """
     Stack item duplication.
     """
     computation.stack_dup(position)
 
 
 dup1 = functools.partial(dup_XX, position=1)
```

### Comparing `py-evm-0.7.0a1/eth/vm/logic/flow.py` & `py-evm-0.7.0a2/eth/vm/logic/flow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,60 @@
+from eth.abc import (
+    ComputationAPI,
+)
 from eth.exceptions import (
-    InvalidJumpDestination,
-    InvalidInstruction,
     Halt,
+    InvalidInstruction,
+    InvalidJumpDestination,
 )
-
-from eth.vm.computation import BaseComputation
 from eth.vm.opcode_values import (
     JUMPDEST,
 )
 
 
-def stop(computation: BaseComputation) -> None:
-    raise Halt('STOP')
+def stop(computation: ComputationAPI) -> None:
+    raise Halt("STOP")
 
 
-def jump(computation: BaseComputation) -> None:
+def jump(computation: ComputationAPI) -> None:
     jump_dest = computation.stack_pop1_int()
 
     computation.code.program_counter = jump_dest
 
     next_opcode = computation.code.peek()
 
     if next_opcode != JUMPDEST:
         raise InvalidJumpDestination("Invalid Jump Destination")
 
     if not computation.code.is_valid_opcode(jump_dest):
         raise InvalidInstruction("Jump resulted in invalid instruction")
 
 
-def jumpi(computation: BaseComputation) -> None:
+def jumpi(computation: ComputationAPI) -> None:
     jump_dest, check_value = computation.stack_pop_ints(2)
 
     if check_value:
         computation.code.program_counter = jump_dest
 
         next_opcode = computation.code.peek()
 
         if next_opcode != JUMPDEST:
             raise InvalidJumpDestination("Invalid Jump Destination")
 
         if not computation.code.is_valid_opcode(jump_dest):
             raise InvalidInstruction("Jump resulted in invalid instruction")
 
 
-def jumpdest(computation: BaseComputation) -> None:
+def jumpdest(computation: ComputationAPI) -> None:
     pass
 
 
-def program_counter(computation: BaseComputation) -> None:
+def program_counter(computation: ComputationAPI) -> None:
     pc = max(computation.code.program_counter - 1, 0)
 
     computation.stack_push_int(pc)
 
 
-def gas(computation: BaseComputation) -> None:
+def gas(computation: ComputationAPI) -> None:
     gas_remaining = computation.get_gas_remaining()
 
     computation.stack_push_int(gas_remaining)
```

### Comparing `py-evm-0.7.0a1/eth/vm/logic/logging.py` & `py-evm-0.7.0a2/eth/vm/logic/logging.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import functools
-from typing import Tuple
-from eth import constants
+from typing import (
+    Tuple,
+)
+
+from eth import (
+    constants,
+)
+from eth.abc import (
+    ComputationAPI,
+)
 
-from eth.vm.computation import BaseComputation
 
-
-def log_XX(computation: BaseComputation, topic_count: int) -> None:
+def log_XX(computation: ComputationAPI, topic_count: int) -> None:
     if topic_count < 0 or topic_count > 4:
         raise TypeError("Invalid log topic size.  Must be 0, 1, 2, 3, or 4")
 
     mem_start_position, size = computation.stack_pop_ints(2)
 
     if not topic_count:
         topics: Tuple[int, ...] = ()
     elif topic_count > 1:
         topics = computation.stack_pop_ints(topic_count)
     else:
-        topics = (computation.stack_pop1_int(), )
+        topics = (computation.stack_pop1_int(),)
 
     data_gas_cost = constants.GAS_LOGDATA * size
     topic_gas_cost = constants.GAS_LOGTOPIC * topic_count
     total_gas_cost = data_gas_cost + topic_gas_cost
 
     computation.consume_gas(
         total_gas_cost,
```

### Comparing `py-evm-0.7.0a1/eth/vm/logic/sha3.py` & `py-evm-0.7.0a2/eth/vm/logic/sha3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-from eth_hash.auto import keccak
+from eth_hash.auto import (
+    keccak,
+)
 
-from eth import constants
+from eth import (
+    constants,
+)
 from eth._utils.numeric import (
     ceil32,
 )
-from eth.vm.computation import BaseComputation
+from eth.abc import (
+    ComputationAPI,
+)
 
 
-def sha3(computation: BaseComputation) -> None:
+def sha3(computation: ComputationAPI) -> None:
     start_position, size = computation.stack_pop_ints(2)
 
     computation.extend_memory(start_position, size)
 
     sha3_bytes = computation.memory_read_bytes(start_position, size)
     word_count = ceil32(len(sha3_bytes)) // 32
```

### Comparing `py-evm-0.7.0a1/eth/vm/logic/stack.py` & `py-evm-0.7.0a2/eth/vm/logic/stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import functools
 
-from eth.vm.computation import BaseComputation
+from eth.abc import (
+    ComputationAPI,
+)
 
 
-def pop(computation: BaseComputation) -> None:
+def pop(computation: ComputationAPI) -> None:
     computation.stack_pop1_any()
 
 
-def push_XX(computation: BaseComputation, size: int) -> None:
+def push_XX(computation: ComputationAPI, size: int) -> None:
     raw_value = computation.code.read(size)
 
     # This is a performance-sensitive area.
     # Calling raw_value.ljust() when size == len(raw_value) is more expensive than
     # calling len(raw_value) and raw_len is typically the correct size already,
     # so this saves a bit of time:
     raw_len = len(raw_value)
     if raw_len == size:
         computation.stack_push_bytes(raw_value)
     else:
-        padded_value = raw_value.ljust(size, b'\x00')
+        padded_value = raw_value.ljust(size, b"\x00")
         computation.stack_push_bytes(padded_value)
 
 
 push0 = functools.partial(push_XX, size=0)
 push1 = functools.partial(push_XX, size=1)
 push2 = functools.partial(push_XX, size=2)
 push3 = functools.partial(push_XX, size=3)
```

### Comparing `py-evm-0.7.0a1/eth/vm/logic/storage.py` & `py-evm-0.7.0a2/eth/vm/logic/storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-from typing import NamedTuple
+from typing import (
+    NamedTuple,
+)
 
 from eth_utils import (
     encode_hex,
 )
-from eth import constants
 
-from eth.vm.computation import BaseComputation
+from eth import (
+    constants,
+)
+from eth.abc import (
+    ComputationAPI,
+)
 
 
-def sstore(computation: BaseComputation) -> None:
+def sstore(computation: ComputationAPI) -> None:
     slot, value = computation.stack_pop_ints(2)
 
     current_value = computation.state.get_storage(
         address=computation.msg.storage_address,
         slot=slot,
     )
 
@@ -32,31 +38,32 @@
         gas_cost = constants.GAS_SSET
     elif is_going_to_be_empty:
         gas_cost = constants.GAS_SRESET
     else:
         gas_cost = constants.GAS_SRESET
 
     computation.consume_gas(
-        gas_cost, reason=(
+        gas_cost,
+        reason=(
             f"SSTORE: {encode_hex(computation.msg.storage_address)}"
             f"[{slot}] -> {value} ({current_value})"
-        )
+        ),
     )
 
     if gas_refund:
         computation.refund_gas(gas_refund)
 
     computation.state.set_storage(
         address=computation.msg.storage_address,
         slot=slot,
         value=value,
     )
 
 
-def sload(computation: BaseComputation) -> None:
+def sload(computation: ComputationAPI) -> None:
     slot = computation.stack_pop1_int()
 
     value = computation.state.get_storage(
         address=computation.msg.storage_address,
         slot=slot,
     )
     computation.stack_push_int(value)
@@ -72,29 +79,27 @@
     # a change to a value when the value was previously unchanged, aka clean, reset
     sstore_reset_gas: int
 
     # the refund for removing a value, aka: clear_refund
     sstore_clears_schedule: int
 
 
-def net_sstore(gas_schedule: NetSStoreGasSchedule, computation: BaseComputation) -> int:
+def net_sstore(gas_schedule: NetSStoreGasSchedule, computation: ComputationAPI) -> int:
     """
     :return slot: where the new value was stored
     """
     slot, value = computation.stack_pop_ints(2)
 
     current_value = computation.state.get_storage(
         address=computation.msg.storage_address,
         slot=slot,
     )
 
     original_value = computation.state.get_storage(
-        address=computation.msg.storage_address,
-        slot=slot,
-        from_journal=False
+        address=computation.msg.storage_address, slot=slot, from_journal=False
     )
 
     gas_refund = 0
 
     if current_value == value:
         gas_cost = gas_schedule.sload_gas
     else:
@@ -113,24 +118,25 @@
                 if current_value == 0:
                     gas_refund -= gas_schedule.sstore_clears_schedule
                 if value == 0:
                     gas_refund += gas_schedule.sstore_clears_schedule
 
             if original_value == value:
                 if original_value == 0:
-                    gas_refund += (gas_schedule.sstore_set_gas - gas_schedule.sload_gas)
+                    gas_refund += gas_schedule.sstore_set_gas - gas_schedule.sload_gas
                 else:
-                    gas_refund += (gas_schedule.sstore_reset_gas - gas_schedule.sload_gas)
+                    gas_refund += gas_schedule.sstore_reset_gas - gas_schedule.sload_gas
 
     computation.consume_gas(
         gas_cost,
         reason=(
             f"SSTORE: {encode_hex(computation.msg.storage_address)}"
-            f"[{slot}] -> {value} (current: {current_value} / original: {original_value})"
-        )
+            f"[{slot}] -> {value} (current: {current_value} / "
+            f"original: {original_value})"
+        ),
     )
 
     if gas_refund:
         computation.refund_gas(gas_refund)
 
     computation.state.set_storage(
         address=computation.msg.storage_address,
```

### Comparing `py-evm-0.7.0a1/eth/vm/logic/swap.py` & `py-evm-0.7.0a2/eth/vm/logic/swap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import functools
 
-from eth.vm.computation import BaseComputation
+from eth.abc import (
+    ComputationAPI,
+)
 
 
-def swap_XX(computation: BaseComputation, position: int) -> None:
+def swap_XX(computation: ComputationAPI, position: int) -> None:
     """
     Stack item swapping
     """
     computation.stack_swap(position)
 
 
 swap1 = functools.partial(swap_XX, position=1)
```

### Comparing `py-evm-0.7.0a1/eth/vm/logic/system.py` & `py-evm-0.7.0a2/eth/vm/logic/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 from eth_typing import (
     Address,
 )
 from eth_utils import (
     encode_hex,
 )
-from eth import constants
-from eth.exceptions import (
-    Halt,
-    Revert,
-    WriteProtection,
-)
 
+from eth import (
+    constants,
+)
 from eth._utils.address import (
     force_bytes_to_address,
     generate_contract_address,
     generate_safe_contract_address,
 )
 from eth._utils.numeric import (
     ceil32,
 )
 from eth.abc import (
     ComputationAPI,
     MessageAPI,
 )
-from eth.vm import mnemonics
-from eth.vm.opcode import Opcode
+from eth.exceptions import (
+    Halt,
+    Revert,
+    WriteProtection,
+)
+from eth.vm import (
+    mnemonics,
+)
+from eth.vm.opcode import (
+    Opcode,
+)
 
-from .call import max_child_gas_eip150
+from .call import (
+    max_child_gas_eip150,
+)
 
 
 def return_op(computation: ComputationAPI) -> None:
     start_position, size = computation.stack_pop_ints(2)
 
     computation.extend_memory(start_position, size)
 
     computation.output = computation.memory_read_bytes(start_position, size)
-    raise Halt('RETURN')
+    raise Halt("RETURN")
 
 
 def revert(computation: ComputationAPI) -> None:
     start_position, size = computation.stack_pop_ints(2)
 
     computation.extend_memory(start_position, size)
 
@@ -58,19 +66,21 @@
         computation.consume_gas(
             constants.GAS_SELFDESTRUCT_NEWACCOUNT,
             reason=mnemonics.SELFDESTRUCT,
         )
     _selfdestruct(computation, beneficiary)
 
 
-def selfdestruct_eip161_on_address(computation: ComputationAPI, beneficiary: Address) -> None:
-    is_dead = (
-        not computation.state.account_exists(beneficiary)
-        or computation.state.account_is_empty(beneficiary)
-    )
+def selfdestruct_eip161_on_address(
+    computation: ComputationAPI,
+    beneficiary: Address,
+) -> None:
+    is_dead = not computation.state.account_exists(
+        beneficiary
+    ) or computation.state.account_is_empty(beneficiary)
     if is_dead and computation.state.get_balance(computation.msg.storage_address):
         computation.consume_gas(
             constants.GAS_SELFDESTRUCT_NEWACCOUNT,
             reason=mnemonics.SELFDESTRUCT,
         )
     _selfdestruct(computation, beneficiary)
 
@@ -96,44 +106,40 @@
         encode_hex(computation.msg.storage_address),
         local_balance,
         encode_hex(beneficiary),
     )
 
     # 3rd: Register the account to be deleted
     computation.register_account_for_deletion(beneficiary)
-    raise Halt('SELFDESTRUCT')
+    raise Halt("SELFDESTRUCT")
 
 
 class CreateOpcodeStackData:
-
-    def __init__(self,
-                 endowment: int,
-                 memory_start: int,
-                 memory_length: int,
-                 salt: int = None) -> None:
-
+    def __init__(
+        self, endowment: int, memory_start: int, memory_length: int, salt: int = None
+    ) -> None:
         self.endowment = endowment
         self.memory_start = memory_start
         self.memory_length = memory_length
         self.salt = salt
 
 
 class Create(Opcode):
-
     def max_child_gas_modifier(self, gas: int) -> int:
         return gas
 
     def get_gas_cost(self, data: CreateOpcodeStackData) -> int:
         return self.gas_cost
 
-    def generate_contract_address(self,
-                                  stack_data: CreateOpcodeStackData,
-                                  call_data: bytes,
-                                  computation: ComputationAPI) -> Address:
-
+    def generate_contract_address(
+        self,
+        stack_data: CreateOpcodeStackData,
+        call_data: bytes,
+        computation: ComputationAPI,
+    ) -> Address:
         creation_nonce = computation.state.get_nonce(computation.msg.storage_address)
         computation.state.increment_nonce(computation.msg.storage_address)
 
         contract_address = generate_contract_address(
             computation.msg.storage_address,
             creation_nonce,
         )
@@ -142,75 +148,85 @@
 
     def get_stack_data(self, computation: ComputationAPI) -> CreateOpcodeStackData:
         endowment, memory_start, memory_length = computation.stack_pop_ints(3)
 
         return CreateOpcodeStackData(endowment, memory_start, memory_length)
 
     def __call__(self, computation: ComputationAPI) -> None:
-
         stack_data = self.get_stack_data(computation)
 
         gas_cost = self.get_gas_cost(stack_data)
         computation.consume_gas(gas_cost, reason=self.mnemonic)
 
         computation.extend_memory(stack_data.memory_start, stack_data.memory_length)
 
-        storage_address_balance = computation.state.get_balance(computation.msg.storage_address)
+        storage_address_balance = computation.state.get_balance(
+            computation.msg.storage_address
+        )
 
         insufficient_funds = storage_address_balance < stack_data.endowment
         stack_too_deep = computation.msg.depth + 1 > constants.STACK_DEPTH_LIMIT
 
         if insufficient_funds or stack_too_deep:
             computation.stack_push_int(0)
-            computation.return_data = b''
+            computation.return_data = b""
             if insufficient_funds:
                 self.logger.debug2(
                     "%s failure: %s",
                     self.mnemonic,
-                    f"Insufficient Funds: {storage_address_balance} < {stack_data.endowment}"
+                    f"Insufficient Funds: {storage_address_balance} < "
+                    f"{stack_data.endowment}",
                 )
             elif stack_too_deep:
-                self.logger.debug2("%s failure: %s", self.mnemonic, "Stack limit reached")
+                self.logger.debug2(
+                    "%s failure: %s", self.mnemonic, "Stack limit reached"
+                )
             else:
-                raise RuntimeError("Invariant: error must be insufficient funds or stack too deep")
+                raise RuntimeError(
+                    "Invariant: error must be insufficient funds or stack too deep"
+                )
             return
 
         call_data = computation.memory_read_bytes(
             stack_data.memory_start, stack_data.memory_length
         )
 
-        create_msg_gas = self.max_child_gas_modifier(
-            computation.get_gas_remaining()
-        )
+        create_msg_gas = self.max_child_gas_modifier(computation.get_gas_remaining())
         computation.consume_gas(create_msg_gas, reason=self.mnemonic)
 
-        contract_address = self.generate_contract_address(stack_data, call_data, computation)
+        contract_address = self.generate_contract_address(
+            stack_data, call_data, computation
+        )
 
         is_collision = computation.state.has_code_or_nonce(contract_address)
 
         if is_collision:
             computation.stack_push_int(0)
-            computation.return_data = b''
+            computation.return_data = b""
             self.logger.debug2(
                 "Address collision while creating contract: %s",
                 encode_hex(contract_address),
             )
             return
 
         child_msg = computation.prepare_child_message(
             gas=create_msg_gas,
             to=constants.CREATE_CONTRACT_ADDRESS,
             value=stack_data.endowment,
-            data=b'',
+            data=b"",
             code=call_data,
             create_address=contract_address,
         )
         self.apply_create_message(computation, child_msg)
 
-    def apply_create_message(self, computation: ComputationAPI, child_msg: MessageAPI) -> None:
+    def apply_create_message(
+        self,
+        computation: ComputationAPI,
+        child_msg: MessageAPI,
+    ) -> None:
         child_computation = computation.apply_child_computation(child_msg)
 
         if child_computation.is_error:
             computation.stack_push_int(0)
         else:
             computation.stack_push_bytes(child_msg.storage_address)
 
@@ -221,41 +237,48 @@
     def max_child_gas_modifier(self, gas: int) -> int:
         return max_child_gas_eip150(gas)
 
 
 class CreateByzantium(CreateEIP150):
     def __call__(self, computation: ComputationAPI) -> None:
         if computation.msg.is_static:
-            raise WriteProtection("Cannot modify state while inside of a STATICCALL context")
+            raise WriteProtection(
+                "Cannot modify state while inside of a STATICCALL context"
+            )
         return super().__call__(computation)
 
 
 class Create2(CreateByzantium):
-
     def get_stack_data(self, computation: ComputationAPI) -> CreateOpcodeStackData:
         endowment, memory_start, memory_length, salt = computation.stack_pop_ints(4)
 
         return CreateOpcodeStackData(endowment, memory_start, memory_length, salt)
 
     def get_gas_cost(self, data: CreateOpcodeStackData) -> int:
-        return constants.GAS_CREATE + constants.GAS_SHA3WORD * ceil32(data.memory_length) // 32
-
-    def generate_contract_address(self,
-                                  stack_data: CreateOpcodeStackData,
-                                  call_data: bytes,
-                                  computation: ComputationAPI) -> Address:
+        return (
+            constants.GAS_CREATE
+            + constants.GAS_SHA3WORD * ceil32(data.memory_length) // 32
+        )
 
+    def generate_contract_address(
+        self,
+        stack_data: CreateOpcodeStackData,
+        call_data: bytes,
+        computation: ComputationAPI,
+    ) -> Address:
         computation.state.increment_nonce(computation.msg.storage_address)
         return generate_safe_contract_address(
-            computation.msg.storage_address,
-            stack_data.salt,
-            call_data
+            computation.msg.storage_address, stack_data.salt, call_data
         )
 
-    def apply_create_message(self, computation: ComputationAPI, child_msg: MessageAPI) -> None:
+    def apply_create_message(
+        self,
+        computation: ComputationAPI,
+        child_msg: MessageAPI,
+    ) -> None:
         # We need to ensure that creation operates on empty storage **and**
         # that if the initialization code fails that we revert the account back
         # to its original state root.
         snapshot = computation.state.snapshot()
 
         computation.state.delete_storage(child_msg.storage_address)
```

### Comparing `py-evm-0.7.0a1/eth/vm/memory.py` & `py-evm-0.7.0a2/eth/vm/memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import itertools
 import logging
 
+from eth._utils.numeric import (
+    ceil32,
+)
+from eth.abc import (
+    MemoryAPI,
+)
 from eth.validation import (
     validate_is_bytes,
     validate_length,
     validate_lte,
     validate_uint256,
 )
 
-from eth._utils.numeric import (
-    ceil32,
-)
-from eth.abc import MemoryAPI
-
 
 class Memory(MemoryAPI):
-    __slots__ = ['_bytes']
-    logger = logging.getLogger('eth.vm.memory.Memory')
+    __slots__ = ["_bytes"]
+    logger = logging.getLogger("eth.vm.memory.Memory")
 
     def __init__(self) -> None:
         self._bytes = bytearray()
 
     def extend(self, start_position: int, size: int) -> None:
         if size == 0:
             return
@@ -33,16 +34,16 @@
         try:
             self._bytes.extend(itertools.repeat(0, size_to_extend))
         except BufferError:
             # we can't extend the buffer (which might involve relocating it) if a
             # memoryview (which stores a pointer into the buffer) has been created by
             # read() and not released. Callers of read() will never try to write to the
             # buffer so we're not missing anything by making a new buffer and forgetting
-            # about the old one. We're keeping too much memory around but this is still a
-            # net savings over having read() return a new bytes() object every time.
+            # about the old one. We're keeping too much memory around but this is still
+            # a net savings over having read() return a new bytes() object every time.
             self._bytes = self._bytes + bytearray(size_to_extend)
 
     def __len__(self) -> int:
         return len(self._bytes)
 
     def write(self, start_position: int, size: int, value: bytes) -> None:
         if size:
@@ -52,11 +53,11 @@
             validate_length(value, length=size)
             validate_lte(start_position + size, maximum=len(self))
 
             for idx, v in enumerate(value):
                 self._bytes[start_position + idx] = v
 
     def read(self, start_position: int, size: int) -> memoryview:
-        return memoryview(self._bytes)[start_position:start_position + size]
+        return memoryview(self._bytes)[start_position : start_position + size]
 
     def read_bytes(self, start_position: int, size: int) -> bytes:
-        return bytes(self._bytes[start_position:start_position + size])
+        return bytes(self._bytes[start_position : start_position + size])
```

### Comparing `py-evm-0.7.0a1/eth/vm/message.py` & `py-evm-0.7.0a2/eth/vm/message.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,65 @@
 import logging
 
-from eth_typing import Address
+from eth_typing import (
+    Address,
+)
 
-from eth.abc import MessageAPI
+from eth.abc import (
+    MessageAPI,
+)
 from eth.constants import (
     CREATE_CONTRACT_ADDRESS,
 )
 from eth.typing import (
     BytesOrView,
 )
 from eth.validation import (
     validate_canonical_address,
+    validate_gte,
+    validate_is_boolean,
     validate_is_bytes,
     validate_is_bytes_or_view,
     validate_is_integer,
-    validate_gte,
     validate_uint256,
-    validate_is_boolean,
 )
 
 
 class Message(MessageAPI):
     __slots__ = [
-        'to', 'sender', 'value', 'data', 'depth', 'gas', 'code', '_code_address',
-        'create_address', 'should_transfer_value', 'is_static', '_storage_address'
+        "to",
+        "sender",
+        "value",
+        "data",
+        "depth",
+        "gas",
+        "code",
+        "_code_address",
+        "create_address",
+        "should_transfer_value",
+        "is_static",
+        "_storage_address",
     ]
 
-    logger = logging.getLogger('eth.vm.message.Message')
+    logger = logging.getLogger("eth.vm.message.Message")
 
-    def __init__(self,
-                 gas: int,
-                 to: Address,
-                 sender: Address,
-                 value: int,
-                 data: BytesOrView,
-                 code: bytes,
-                 depth: int = 0,
-                 create_address: Address = None,
-                 code_address: Address = None,
-                 should_transfer_value: bool = True,
-                 is_static: bool = False) -> None:
+    def __init__(
+        self,
+        gas: int,
+        to: Address,
+        sender: Address,
+        value: int,
+        data: BytesOrView,
+        code: bytes,
+        depth: int = 0,
+        create_address: Address = None,
+        code_address: Address = None,
+        should_transfer_value: bool = True,
+        is_static: bool = False,
+    ) -> None:
         validate_uint256(gas, title="Message.gas")
         self.gas: int = gas
 
         if to != CREATE_CONTRACT_ADDRESS:
             validate_canonical_address(to, title="Message.to")
         self.to = to
 
@@ -67,15 +83,17 @@
             validate_canonical_address(create_address, title="Message.storage_address")
         self.storage_address = create_address
 
         if code_address is not None:
             validate_canonical_address(code_address, title="Message.code_address")
         self.code_address = code_address
 
-        validate_is_boolean(should_transfer_value, title="Message.should_transfer_value")
+        validate_is_boolean(
+            should_transfer_value, title="Message.should_transfer_value"
+        )
         self.should_transfer_value = should_transfer_value
 
         validate_is_boolean(is_static, title="Message.is_static")
         self.is_static = is_static
 
     @property
     def code_address(self) -> Address:
```

### Comparing `py-evm-0.7.0a1/eth/vm/opcode.py` & `py-evm-0.7.0a2/eth/vm/opcode.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 import functools
-
 from typing import (
     Any,
     Callable,
     Type,
     TypeVar,
 )
 
 from eth_utils import (
     ExtendedDebugLogger,
     get_extended_debug_logger,
 )
 
-from eth._utils.datatypes import Configurable
+from eth._utils.datatypes import (
+    Configurable,
+)
 from eth.abc import (
     ComputationAPI,
     OpcodeAPI,
 )
 
-
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class Opcode(Configurable, OpcodeAPI):
     mnemonic: str = None
     gas_cost: int = None
 
     def __init__(self) -> None:
         if self.mnemonic is None:
             raise TypeError(f"Opcode class {type(self)} missing opcode mnemonic")
         if self.gas_cost is None:
             raise TypeError(f"Opcode class {type(self)} missing opcode gas_cost")
 
     @property
     def logger(self) -> ExtendedDebugLogger:
-        return get_extended_debug_logger(f'eth.vm.logic.{self.mnemonic}')
+        return get_extended_debug_logger(f"eth.vm.logic.{self.mnemonic}")
 
     @classmethod
-    def as_opcode(cls: Type[T],
-                  logic_fn: Callable[..., Any],
-                  mnemonic: str,
-                  gas_cost: int) -> T:
+    def as_opcode(
+        cls: Type[T], logic_fn: Callable[..., Any], mnemonic: str, gas_cost: int
+    ) -> T:
         if gas_cost:
+
             @functools.wraps(logic_fn)
             def wrapped_logic_fn(computation: ComputationAPI) -> Any:
                 """
                 Wrapper function for the logic function which consumes the base
                 opcode gas cost prior to execution.
                 """
                 computation.consume_gas(
                     gas_cost,
                     mnemonic,
                 )
                 return logic_fn(computation)
+
         else:
             wrapped_logic_fn = logic_fn
 
         props = {
-            '__call__': staticmethod(wrapped_logic_fn),
-            'mnemonic': mnemonic,
-            'gas_cost': gas_cost,
+            "__call__": staticmethod(wrapped_logic_fn),
+            "mnemonic": mnemonic,
+            "gas_cost": gas_cost,
         }
         opcode_cls = type(f"opcode:{mnemonic}", (cls,), props)
         return opcode_cls()
 
-    def __copy__(self) -> 'Opcode':
+    def __copy__(self) -> "Opcode":
         return type(self)()
 
-    def __deepcopy__(self, memo: Any) -> 'Opcode':
+    def __deepcopy__(self, memo: Any) -> "Opcode":
         return type(self)()
 
 
 as_opcode = Opcode.as_opcode
```

### Comparing `py-evm-0.7.0a1/eth/vm/opcode_values.py` & `py-evm-0.7.0a2/eth/vm/opcode_values.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 SUB = 0x03
 DIV = 0x04
 SDIV = 0x05
 MOD = 0x06
 SMOD = 0x07
 ADDMOD = 0x08
 MULMOD = 0x09
-EXP = 0x0a
-SIGNEXTEND = 0x0b
+EXP = 0x0A
+SIGNEXTEND = 0x0B
 
 
 #
 # Comparison and Bitwise Logic
 #
 LT = 0x10
 GT = 0x11
@@ -24,18 +24,18 @@
 SGT = 0x13
 EQ = 0x14
 ISZERO = 0x15
 AND = 0x16
 OR = 0x17
 XOR = 0x18
 NOT = 0x19
-BYTE = 0x1a
-SHL = 0x1b
-SHR = 0x1c
-SAR = 0x1d
+BYTE = 0x1A
+SHL = 0x1B
+SHR = 0x1C
+SAR = 0x1D
 
 
 #
 # Sha3
 #
 SHA3 = 0x20
 
@@ -49,22 +49,23 @@
 CALLER = 0x33
 CALLVALUE = 0x34
 CALLDATALOAD = 0x35
 CALLDATASIZE = 0x36
 CALLDATACOPY = 0x37
 CODESIZE = 0x38
 CODECOPY = 0x39
-GASPRICE = 0x3a
-EXTCODESIZE = 0x3b
-EXTCODECOPY = 0x3c
-RETURNDATASIZE = 0x3d
-RETURNDATACOPY = 0x3e
-EXTCODEHASH = 0x3f
+GASPRICE = 0x3A
+EXTCODESIZE = 0x3B
+EXTCODECOPY = 0x3C
+RETURNDATASIZE = 0x3D
+RETURNDATACOPY = 0x3E
+EXTCODEHASH = 0x3F
 
-# These opcodes seem to belong in the environment block, but we are out of opcode space in 0x3*
+# These opcodes seem to belong in the environment block,
+# but we are out of opcode space in 0x3*
 CHAINID = 0x46
 SELFBALANCE = 0x47
 BASEFEE = 0x48
 
 #
 # Block Information
 #
@@ -87,54 +88,54 @@
 MSTORE8 = 0x53
 SLOAD = 0x54
 SSTORE = 0x55
 JUMP = 0x56
 JUMPI = 0x57
 PC = 0x58
 MSIZE = 0x59
-GAS = 0x5a
-JUMPDEST = 0x5b
+GAS = 0x5A
+JUMPDEST = 0x5B
 
 
 #
 # Push Operations
 #
-PUSH0 = 0x5f
+PUSH0 = 0x5F
 PUSH1 = 0x60
 PUSH2 = 0x61
 PUSH3 = 0x62
 PUSH4 = 0x63
 PUSH5 = 0x64
 PUSH6 = 0x65
 PUSH7 = 0x66
 PUSH8 = 0x67
 PUSH9 = 0x68
 PUSH10 = 0x69
-PUSH11 = 0x6a
-PUSH12 = 0x6b
-PUSH13 = 0x6c
-PUSH14 = 0x6d
-PUSH15 = 0x6e
-PUSH16 = 0x6f
+PUSH11 = 0x6A
+PUSH12 = 0x6B
+PUSH13 = 0x6C
+PUSH14 = 0x6D
+PUSH15 = 0x6E
+PUSH16 = 0x6F
 PUSH17 = 0x70
 PUSH18 = 0x71
 PUSH19 = 0x72
 PUSH20 = 0x73
 PUSH21 = 0x74
 PUSH22 = 0x75
 PUSH23 = 0x76
 PUSH24 = 0x77
 PUSH25 = 0x78
 PUSH26 = 0x79
-PUSH27 = 0x7a
-PUSH28 = 0x7b
-PUSH29 = 0x7c
-PUSH30 = 0x7d
-PUSH31 = 0x7e
-PUSH32 = 0x7f
+PUSH27 = 0x7A
+PUSH28 = 0x7B
+PUSH29 = 0x7C
+PUSH30 = 0x7D
+PUSH31 = 0x7E
+PUSH32 = 0x7F
 
 
 #
 # Duplicate Operations
 #
 DUP1 = 0x80
 DUP2 = 0x81
@@ -142,20 +143,20 @@
 DUP4 = 0x83
 DUP5 = 0x84
 DUP6 = 0x85
 DUP7 = 0x86
 DUP8 = 0x87
 DUP9 = 0x88
 DUP10 = 0x89
-DUP11 = 0x8a
-DUP12 = 0x8b
-DUP13 = 0x8c
-DUP14 = 0x8d
-DUP15 = 0x8e
-DUP16 = 0x8f
+DUP11 = 0x8A
+DUP12 = 0x8B
+DUP13 = 0x8C
+DUP14 = 0x8D
+DUP15 = 0x8E
+DUP16 = 0x8F
 
 
 #
 # Exchange Operations
 #
 SWAP1 = 0x90
 SWAP2 = 0x91
@@ -163,37 +164,37 @@
 SWAP4 = 0x93
 SWAP5 = 0x94
 SWAP6 = 0x95
 SWAP7 = 0x96
 SWAP8 = 0x97
 SWAP9 = 0x98
 SWAP10 = 0x99
-SWAP11 = 0x9a
-SWAP12 = 0x9b
-SWAP13 = 0x9c
-SWAP14 = 0x9d
-SWAP15 = 0x9e
-SWAP16 = 0x9f
+SWAP11 = 0x9A
+SWAP12 = 0x9B
+SWAP13 = 0x9C
+SWAP14 = 0x9D
+SWAP15 = 0x9E
+SWAP16 = 0x9F
 
 
 #
 # Logging
 #
-LOG0 = 0xa0
-LOG1 = 0xa1
-LOG2 = 0xa2
-LOG3 = 0xa3
-LOG4 = 0xa4
+LOG0 = 0xA0
+LOG1 = 0xA1
+LOG2 = 0xA2
+LOG3 = 0xA3
+LOG4 = 0xA4
 
 
 #
 # System
 #
-CREATE = 0xf0
-CALL = 0xf1
-CALLCODE = 0xf2
-RETURN = 0xf3
-DELEGATECALL = 0xf4
-CREATE2 = 0xf5
-STATICCALL = 0xfa
-REVERT = 0xfd
-SELFDESTRUCT = 0xff
+CREATE = 0xF0
+CALL = 0xF1
+CALLCODE = 0xF2
+RETURN = 0xF3
+DELEGATECALL = 0xF4
+CREATE2 = 0xF5
+STATICCALL = 0xFA
+REVERT = 0xFD
+SELFDESTRUCT = 0xFF
```

### Comparing `py-evm-0.7.0a1/eth/vm/stack.py` & `py-evm-0.7.0a2/eth/vm/stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,74 +1,76 @@
 import logging
 from typing import (
     Iterable,
     List,
     Tuple,
-    Union
+    Union,
 )
 
 from eth_utils import (
     ValidationError,
     big_endian_to_int,
     int_to_big_endian,
 )
+
+from eth.abc import (
+    StackAPI,
+)
 from eth.exceptions import (
-    InsufficientStack,
     FullStack,
+    InsufficientStack,
 )
 from eth.validation import (
     validate_stack_bytes,
     validate_stack_int,
 )
 
-from eth.abc import StackAPI
-
 
 def _busted_type(item_type: type, value: Union[int, bytes]) -> ValidationError:
     return ValidationError(
-        "Stack must always be bytes or int, "
-        f"got {item_type!r} type, val {value!r}"
+        f"Stack must always be bytes or int, got {item_type!r} type, val {value!r}"
     )
 
 
 class Stack(StackAPI):
     """
     VM Stack
     """
-    __slots__ = ['values', '_append', '_pop_typed', '__len__']
-    logger = logging.getLogger('eth.vm.stack.Stack')
+
+    __slots__ = ["values", "_append", "_pop_typed", "__len__"]
+    logger = logging.getLogger("eth.vm.stack.Stack")
 
     #
-    # Performance Note: Operations that push to the stack have the data in some natural form:
-    #   integer or bytes. Whatever operation is pulling from the stack, also has its preferred
-    #   representation to work with. Typically, those two representations line up (pushed & pulled)
-    #   so we save a notable amount of conversion time by storing heterogenous data on the stack,
-    #   and converting only when necessary.
+    # Performance Note: Operations that push to the stack have the data in some natural
+    #   form: integer or bytes. Whatever operation is pulling from the stack, also has
+    #   its preferred representation to work with. Typically, those two representations
+    #   line up (pushed & pulled) so we save a notable amount of conversion time by
+    #   storing heterogenous data on the stack, and converting only when necessary.
     #
 
     def __init__(self) -> None:
         values: List[Tuple[type, Union[int, bytes]]] = []
         self.values = values
         # caching optimizations to avoid an attribute lookup on self.values
         # This doesn't use `cached_property`, because it doesn't play nice with slots
         self._append = values.append
         self._pop_typed = values.pop
         self.__len__ = values.__len__
 
     def push_int(self, value: int) -> None:
         if len(self.values) > 1023:
-            raise FullStack('Stack limit reached')
+            raise FullStack("Stack limit reached")
 
         validate_stack_int(value)
 
         self._append((int, value))
 
     def push_bytes(self, value: bytes) -> None:
         if len(self.values) > 1023:
-            raise FullStack('Stack limit reached')
+            raise FullStack("Stack limit reached")
 
         validate_stack_bytes(value)
 
         self._append((bytes, value))
 
     def pop1_bytes(self) -> bytes:
         #
@@ -198,26 +200,28 @@
         try:
             self.values[-1], self.values[idx] = self.values[idx], self.values[-1]
         except IndexError:
             raise InsufficientStack(f"Insufficient stack items for SWAP{position}")
 
     def dup(self, position: int) -> None:
         if len(self.values) > 1023:
-            raise FullStack('Stack limit reached')
+            raise FullStack("Stack limit reached")
 
         peek_index = -1 * position
         try:
             self._append(self.values[peek_index])
         except IndexError:
             raise InsufficientStack(f"Insufficient stack items for DUP{position}")
 
     def _stack_items_str(self) -> Iterable[str]:
         for item_type, val in self.values:
             if isinstance(val, int):
                 yield hex(val)
             elif isinstance(val, bytes):
                 yield "0x" + val.hex()
             else:
-                raise RuntimeError(f"Stack items can only be int or bytes, not {val!r}:{item_type}")
+                raise RuntimeError(
+                    f"Stack items can only be int or bytes, not {val!r}:{item_type}"
+                )
 
     def __str__(self) -> str:
         return str(list(self._stack_items_str()))
```

### Comparing `py-evm-0.7.0a1/eth/vm/state.py` & `py-evm-0.7.0a2/eth/vm/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,64 +11,69 @@
     BlockNumber,
     Hash32,
 )
 from eth_utils import (
     ExtendedDebugLogger,
     get_extended_debug_logger,
 )
-from eth_utils.toolz import nth
+from eth_utils.toolz import (
+    nth,
+)
 
+from eth._utils.datatypes import (
+    Configurable,
+)
 from eth.abc import (
     AccountDatabaseAPI,
     AtomicDatabaseAPI,
     ComputationAPI,
     ExecutionContextAPI,
     MessageAPI,
+    MetaWitnessAPI,
     SignedTransactionAPI,
     StateAPI,
     TransactionContextAPI,
     TransactionExecutorAPI,
-    MetaWitnessAPI,
     WithdrawalAPI,
 )
 from eth.constants import (
     MAX_PREV_HEADER_DEPTH,
 )
-from eth.typing import JournalDBCheckpoint
-from eth._utils.datatypes import (
-    Configurable,
+from eth.typing import (
+    JournalDBCheckpoint,
 )
 
 
 class BaseState(Configurable, StateAPI):
     #
     # Set from __init__
     #
-    __slots__ = ['_db', 'execution_context', '_account_db']
+    __slots__ = ["_db", "execution_context", "_account_db"]
 
     computation_class: Type[ComputationAPI] = None
     transaction_context_class: Type[TransactionContextAPI] = None
     account_db_class: Type[AccountDatabaseAPI] = None
     transaction_executor_class: Type[TransactionExecutorAPI] = None
 
     def __init__(
-            self,
-            db: AtomicDatabaseAPI,
-            execution_context: ExecutionContextAPI,
-            state_root: Hash32) -> None:
+        self,
+        db: AtomicDatabaseAPI,
+        execution_context: ExecutionContextAPI,
+        state_root: Hash32,
+    ) -> None:
         self._db = db
         self.execution_context = execution_context
         self._account_db = self.get_account_db_class()(db, state_root)
 
     #
     # Logging
     #
     @property
     def logger(self) -> ExtendedDebugLogger:
-        return get_extended_debug_logger(f'eth.vm.state.{self.__class__.__name__}')
+        return get_extended_debug_logger(f"eth.vm.state.{self.__class__.__name__}")
 
     #
     # Block Object Properties (in opcodes)
     #
 
     @property
     def coinbase(self) -> Address:
@@ -92,15 +97,17 @@
 
     @property
     def gas_limit(self) -> int:
         return self.execution_context.gas_limit
 
     @property
     def base_fee(self) -> int:
-        raise NotImplementedError("Basefee opcode is not implemented prior to London hard fork")
+        raise NotImplementedError(
+            "Basefee opcode is not implemented prior to London hard fork"
+        )
 
     def get_tip(self, transaction: SignedTransactionAPI) -> int:
         return transaction.gas_price
 
     def get_gas_price(self, transaction: SignedTransactionAPI) -> int:
         return transaction.gas_price
 
@@ -116,15 +123,17 @@
     @property
     def state_root(self) -> Hash32:
         return self._account_db.state_root
 
     def make_state_root(self) -> Hash32:
         return self._account_db.make_state_root()
 
-    def get_storage(self, address: Address, slot: int, from_journal: bool = True) -> int:
+    def get_storage(
+        self, address: Address, slot: int, from_journal: bool = True
+    ) -> int:
         return self._account_db.get_storage(address, slot, from_journal)
 
     def set_storage(self, address: Address, slot: int, value: int) -> None:
         return self._account_db.set_storage(address, slot, value)
 
     def delete_storage(self, address: Address) -> None:
         self._account_db.delete_storage(address)
@@ -225,72 +234,78 @@
         ancestor_depth = self.block_number - block_number - 1
         is_ancestor_depth_out_of_range = (
             ancestor_depth >= MAX_PREV_HEADER_DEPTH
             or ancestor_depth < 0
             or block_number < 0
         )
         if is_ancestor_depth_out_of_range:
-            return Hash32(b'')
+            return Hash32(b"")
 
         try:
             return nth(ancestor_depth, self.execution_context.prev_hashes)
         except StopIteration:
             # Ancestor with specified depth not present
-            return Hash32(b'')
+            return Hash32(b"")
 
     #
     # Computation
     #
-    def get_computation(self,
-                        message: MessageAPI,
-                        transaction_context: TransactionContextAPI) -> ComputationAPI:
+    def get_computation(
+        self, message: MessageAPI, transaction_context: TransactionContextAPI
+    ) -> ComputationAPI:
         if self.computation_class is None:
             raise AttributeError("No `computation_class` has been set for this State")
         else:
             computation = self.computation_class(self, message, transaction_context)
         return computation
 
     #
     # Transaction context
     #
     @classmethod
     def get_transaction_context_class(cls) -> Type[TransactionContextAPI]:
         if cls.transaction_context_class is None:
-            raise AttributeError("No `transaction_context_class` has been set for this State")
+            raise AttributeError(
+                "No `transaction_context_class` has been set for this State"
+            )
         return cls.transaction_context_class
 
     #
     # Execution
     #
     def get_transaction_executor(self) -> TransactionExecutorAPI:
         return self.transaction_executor_class(self)
 
-    def costless_execute_transaction(self,
-                                     transaction: SignedTransactionAPI) -> ComputationAPI:
+    def costless_execute_transaction(
+        self, transaction: SignedTransactionAPI
+    ) -> ComputationAPI:
         with self.override_transaction_context(gas_price=transaction.gas_price):
             free_transaction = transaction.copy(gas_price=0)
             return self.apply_transaction(free_transaction)
 
     @contextlib.contextmanager
     def override_transaction_context(self, gas_price: int) -> Iterator[None]:
         original_context = self.get_transaction_context
 
-        def get_custom_transaction_context(transaction: SignedTransactionAPI) -> TransactionContextAPI:   # noqa: E501
+        def get_custom_transaction_context(
+            transaction: SignedTransactionAPI,
+        ) -> TransactionContextAPI:
             custom_transaction = transaction.copy(gas_price=gas_price)
             return original_context(custom_transaction)
 
         # mypy doesn't like assigning to an existing method
         self.get_transaction_context = get_custom_transaction_context  # type: ignore
         try:
             yield
         finally:
-            self.get_transaction_context = original_context     # type: ignore # Remove ignore if https://github.com/python/mypy/issues/708 is fixed. # noqa: E501
+            self.get_transaction_context = original_context  # type: ignore # Remove ignore if https://github.com/python/mypy/issues/708 is fixed. # noqa: E501
 
-    def get_transaction_context(self,
-                                transaction: SignedTransactionAPI) -> TransactionContextAPI:
+    def get_transaction_context(
+        self, transaction: SignedTransactionAPI
+    ) -> TransactionContextAPI:
         return self.get_transaction_context_class()(
             gas_price=transaction.gas_price,
             origin=transaction.sender,
         )
 
     #
     # Withdrawals
```

### Comparing `py-evm-0.7.0a1/eth/vm/transaction_context.py` & `py-evm-0.7.0a2/eth/vm/transaction_context.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import itertools
 
-from eth_typing import Address
+from eth_typing import (
+    Address,
+)
 
-from eth.abc import TransactionContextAPI
+from eth.abc import (
+    TransactionContextAPI,
+)
 from eth.validation import (
     validate_canonical_address,
     validate_uint256,
 )
 
 
 class BaseTransactionContext(TransactionContextAPI):
-    __slots__ = ['_gas_price', '_origin', '_log_counter']
+    __slots__ = ["_gas_price", "_origin", "_log_counter"]
 
     def __init__(self, gas_price: int, origin: Address) -> None:
         validate_uint256(gas_price, title="TransactionContext.gas_price")
         self._gas_price = gas_price
         validate_canonical_address(origin, title="TransactionContext.origin")
         self._origin = origin
         self._log_counter = itertools.count()
```

### Comparing `py-evm-0.7.0a1/py_evm.egg-info/SOURCES.txt` & `py-evm-0.7.0a2/py_evm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a1/py_evm.egg-info/requires.txt` & `py-evm-0.7.0a2/py_evm.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -47,15 +47,18 @@
 Sphinx<2,>=1.5.5
 jinja2<3.1.0,>=3.0.0
 sphinx_rtd_theme>=0.1.9
 sphinxcontrib-asyncio<0.4,>=0.2.0
 towncrier<22,>=21
 flake8==3.8.2
 flake8-bugbear==20.1.4
+isort>=5.10.1
 mypy==0.910
+pydocstyle>=6.0.0
+black>=23
 types-setuptools
 
 [dev:python_version < "3.8"]
 importlib-metadata<5.0
 
 [doc]
 py-evm>=0.2.0-a.14
@@ -89,15 +92,18 @@
 
 [eth-extra:implementation_name == "pypy"]
 eth-hash[pycryptodome]
 
 [lint]
 flake8==3.8.2
 flake8-bugbear==20.1.4
+isort>=5.10.1
 mypy==0.910
+pydocstyle>=6.0.0
+black>=23
 types-setuptools
 
 [lint:python_version < "3.8"]
 importlib-metadata<5.0
 
 [test]
 factory-boy==2.11.1
```

### Comparing `py-evm-0.7.0a1/pyproject.toml` & `py-evm-0.7.0a2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.towncrier]
 # Read https://github.com/ethereum/py-evm/newsfragments/README.md for instructions
 package = "eth"
 filename = "docs/release_notes.rst"
 directory = "newsfragments"
 underlines = ["-", "~", "^"]
-title_format = "py-evm {version} ({project_date})"
+title_format = "py-evm v{version} ({project_date})"
 issue_format = "`#{issue} <https://github.com/ethereum/py-evm/issues/{issue}>`__"
 
 [[tool.towncrier.type]]
 directory = "feature"
 name = "Features"
 showcontent = true
 
@@ -30,15 +30,15 @@
 [[tool.towncrier.type]]
 directory = "removal"
 name = "Deprecations and Removals"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "internal"
-name = "Internal Changes - For Contributors"
+name = "Internal Changes - For py-evm Contributors"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "misc"
 name = "Miscellaneous changes"
 showcontent = false
```

### Comparing `py-evm-0.7.0a1/setup.py` & `py-evm-0.7.0a2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 
 deps = {
-    'eth': [
+    "eth": [
         "cached-property>=1.5.1,<2",
         "eth-bloom>=1.0.3",
         "eth-keys>=0.4.0,<0.5.0",
         "eth-typing>=3.3.0,<4.0.0",
         "eth-utils>=2.0.0,<3.0.0",
         "lru-dict>=1.1.6",
         "mypy_extensions>=0.4.1,<1.0.0",
@@ -17,106 +17,102 @@
         "rlp>=3,<4",
         "trie>=2.0.0,<3",
     ],
     # The eth-extra sections is for libraries that the evm does not
     # explicitly need to function and hence should not depend on.
     # Installing these libraries may make the evm perform better than
     # using the default fallbacks though.
-    'eth-extra': [
+    "eth-extra": [
         "blake2b-py>=0.1.4,<0.2",
         "coincurve>=13.0.0,<14.0.0",
         "eth-hash[pysha3];implementation_name=='cpython'",
         "eth-hash[pycryptodome];implementation_name=='pypy'",
         "plyvel>=1.2.0,<2",
     ],
-    'test': [
+    "test": [
         "factory-boy==2.11.1",
         "hypothesis>=5,<6",
         "pexpect>=4.6, <5",
         "pytest>=6.2.4,<7",
         "pytest-asyncio>=0.10.0,<0.11",
         "pytest-cov==2.5.1",
         "pytest-timeout>=1.4.2,<2",
         "pytest-watch>=4.1.0,<5",
         "pytest-xdist==2.3.0",
         "importlib-metadata<5.0;python_version<'3.8'",
     ],
-    'lint': [
+    "lint": [
         "flake8==3.8.2",
         "flake8-bugbear==20.1.4",
+        "isort>=5.10.1",
         "mypy==0.910",
+        "pydocstyle>=6.0.0",
+        "black>=23",
         "types-setuptools",
         "importlib-metadata<5.0;python_version<'3.8'",
     ],
-    'benchmark': [
+    "benchmark": [
         "termcolor>=1.1.0,<2.0.0",
         "web3>=4.1.0,<5.0.0",
     ],
-    'doc': [
+    "doc": [
         "py-evm>=0.2.0-a.14",
         # We need to have pysha for autodoc to be able to extract API docs
         "pysha3>=1.0.0,<2.0.0",
         "Sphinx>=1.5.5,<2",
         "jinja2>=3.0.0,<3.1.0",  # jinja2<3.0 or >=3.1.0 cause doc build failures.
         "sphinx_rtd_theme>=0.1.9",
         "sphinxcontrib-asyncio>=0.2.0,<0.4",
         "towncrier>=21,<22",
     ],
-    'dev': [
+    "dev": [
         "bumpversion>=0.5.3,<1",
         "wheel",
         "setuptools>=36.2.0",
-
         # Fixing this dependency due to: requests 2.20.1 has requirement
         # idna<2.8,>=2.5, but you'll have idna 2.8 which is incompatible.
         "idna==2.7",
         # idna 2.7 is not supported by requests 2.18
         "requests>=2.20,<3",
         "tox==2.7.0",
         "twine",
     ],
 }
 
 
-deps['dev'] = (
-    deps['dev'] +
-    deps['eth'] +
-    deps['test'] +
-    deps['doc'] +
-    deps['lint']
-)
+deps["dev"] = deps["dev"] + deps["eth"] + deps["test"] + deps["doc"] + deps["lint"]
 
 
-install_requires = deps['eth']
+install_requires = deps["eth"]
 
-with open('README.md') as readme_file:
+with open("README.md") as readme_file:
     long_description = readme_file.read()
 
 setup(
-    name='py-evm',
+    name="py-evm",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version='0.7.0-alpha.1',
-    description='Python implementation of the Ethereum Virtual Machine',
+    version="0.7.0-alpha.2",
+    description="Python implementation of the Ethereum Virtual Machine",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    author='Ethereum Foundation',
-    author_email='piper@pipermerriam.com',
-    url='https://github.com/ethereum/py-evm',
+    long_description_content_type="text/markdown",
+    author="Ethereum Foundation",
+    author_email="piper@pipermerriam.com",
+    url="https://github.com/ethereum/py-evm",
     include_package_data=True,
-    py_modules=['eth'],
+    py_modules=["eth"],
     install_requires=install_requires,
     extras_require=deps,
-    license='MIT',
+    license="MIT",
     zip_safe=False,
-    keywords='ethereum blockchain evm',
+    keywords="ethereum blockchain evm",
     packages=find_packages(exclude=["tests", "tests.*"]),
-    package_data={'eth': ['py.typed']},
+    package_data={"eth": ["py.typed"]},
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
 )
```

