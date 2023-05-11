# Comparing `tmp/stac-fastapi.pgstac-2.4.5.tar.gz` & `tmp/stac-fastapi.pgstac-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.pgstac-2.4.5.tar", last modified: Wed Apr  5 14:03:59 2023, max compression
+gzip compressed data, was "stac-fastapi.pgstac-2.4.6.tar", last modified: Thu May 11 15:16:57 2023, max compression
```

## Comparing `stac-fastapi.pgstac-2.4.5.tar` & `stac-fastapi.pgstac-2.4.6.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:59.265037 stac-fastapi.pgstac-2.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-05 14:03:59.265037 stac-fastapi.pgstac-2.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-05 14:03:59.265037 stac-fastapi.pgstac-2.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:59.261037 stac-fastapi.pgstac-2.4.5/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:59.261037 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:59.265037 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/extensions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/extensions/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:59.265037 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/models/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/models/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:59.265037 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/types/base_item_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/types/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:59.261037 stac-fastapi.pgstac-2.4.5/stac_fastapi.pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-05 14:03:59.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi.pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-05 14:03:59.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi.pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:03:59.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi.pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-05 14:03:59.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi.pgstac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:03:59.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi.pgstac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-05 14:03:59.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi.pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-05 14:03:59.000000 stac-fastapi.pgstac-2.4.5/stac_fastapi.pgstac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:59.261037 stac-fastapi.pgstac-2.4.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:59.265037 stac-fastapi.pgstac-2.4.5/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21437 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/tests/api/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:59.265037 stac-fastapi.pgstac-2.4.5/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/tests/clients/test_postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:59.265037 stac-fastapi.pgstac-2.4.5/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/tests/resources/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/tests/resources/test_conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)    50432 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/tests/resources/test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-05 14:03:26.000000 stac-fastapi.pgstac-2.4.5/tests/resources/test_mgmt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.229380 stac-fastapi.pgstac-2.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-11 15:16:57.229380 stac-fastapi.pgstac-2.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-11 15:16:57.229380 stac-fastapi.pgstac-2.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/extensions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/extensions/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/types/base_item_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.229380 stac-fastapi.pgstac-2.4.6/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21437 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/api/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.229380 stac-fastapi.pgstac-2.4.6/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/clients/test_postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.229380 stac-fastapi.pgstac-2.4.6/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/resources/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/resources/test_conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50432 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/resources/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/resources/test_mgmt.py
```

### Comparing `stac-fastapi.pgstac-2.4.5/PKG-INFO` & `stac-fastapi.pgstac-2.4.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7374 6163  : 2.1.Name: stac
 00000020: 2d66 6173 7461 7069 2e70 6773 7461 630a  -fastapi.pgstac.
-00000030: 5665 7273 696f 6e3a 2032 2e34 2e35 0a53  Version: 2.4.5.S
+00000030: 5665 7273 696f 6e3a 2032 2e34 2e36 0a53  Version: 2.4.6.S
 00000040: 756d 6d61 7279 3a20 416e 2069 6d70 6c65  ummary: An imple
 00000050: 6d65 6e74 6174 696f 6e20 6f66 2053 5441  mentation of STA
 00000060: 4320 4150 4920 6261 7365 6420 6f6e 2074  C API based on t
 00000070: 6865 2046 6173 7441 5049 2066 7261 6d65  he FastAPI frame
 00000080: 776f 726b 2061 6e64 2075 7369 6e67 2074  work and using t
 00000090: 6865 2070 6773 7461 6320 6261 636b 656e  he pgstac backen
 000000a0: 642e 0a48 6f6d 652d 7061 6765 3a20 6874  d..Home-page: ht
@@ -39,260 +39,301 @@
 00000260: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
 00000270: 6172 6b64 6f77 6e0a 5072 6f76 6964 6573  arkdown.Provides
 00000280: 2d45 7874 7261 3a20 6465 760a 5072 6f76  -Extra: dev.Prov
 00000290: 6964 6573 2d45 7874 7261 3a20 646f 6373  ides-Extra: docs
 000002a0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
 000002b0: 2073 6572 7665 720a 5072 6f76 6964 6573   server.Provides
 000002c0: 2d45 7874 7261 3a20 6177 736c 616d 6264  -Extra: awslambd
-000002d0: 610a 0a3c 7020 616c 6967 6e3d 2263 656e  a..<p align="cen
-000002e0: 7465 7222 3e0a 2020 3c69 6d67 2073 7263  ter">.  <img src
-000002f0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000300: 2e63 6f6d 2f72 6164 6961 6e74 6561 7274  .com/radianteart
-00000310: 682f 7374 6163 2d73 6974 652f 7261 772f  h/stac-site/raw/
-00000320: 6d61 7374 6572 2f69 6d61 6765 732f 6c6f  master/images/lo
-00000330: 676f 2f73 7461 632d 3033 302d 6c6f 6e67  go/stac-030-long
-00000340: 2e70 6e67 2220 7769 6474 683d 3430 303e  .png" width=400>
-00000350: 0a20 203c 7020 616c 6967 6e3d 2263 656e  .  <p align="cen
-00000360: 7465 7222 3e46 6173 7441 5049 2069 6d70  ter">FastAPI imp
-00000370: 6c65 6d65 6e74 696f 6e20 6f66 2074 6865  lemention of the
-00000380: 2053 5441 4320 4150 4920 7370 6563 2075   STAC API spec u
-00000390: 7369 6e67 203c 6120 6872 6566 3d22 6874  sing <a href="ht
-000003a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000003b0: 2f73 7461 632d 7574 696c 732f 7067 7374  /stac-utils/pgst
-000003c0: 6163 223e 5047 5374 6163 3c2f 613e 3c2f  ac">PGStac</a></
-000003d0: 703e 0a3c 2f70 3e0a 3c70 2061 6c69 676e  p>.</p>.<p align
-000003e0: 3d22 6365 6e74 6572 223e 0a20 203c 6120  ="center">.  <a 
-000003f0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000400: 7468 7562 2e63 6f6d 2f73 7461 632d 7574  thub.com/stac-ut
-00000410: 696c 732f 7374 6163 2d66 6173 7461 7069  ils/stac-fastapi
-00000420: 2f61 6374 696f 6e73 3f71 7565 7279 3d77  /actions?query=w
-00000430: 6f72 6b66 6c6f 7725 3341 6369 6364 2220  orkflow%3Acicd" 
-00000440: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00000450: 0a20 2020 2020 203c 696d 6720 7372 633d  .      <img src=
-00000460: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000470: 636f 6d2f 7374 6163 2d75 7469 6c73 2f73  com/stac-utils/s
-00000480: 7461 632d 6661 7374 6170 692f 776f 726b  tac-fastapi/work
-00000490: 666c 6f77 732f 7374 6163 2d66 6173 7461  flows/stac-fasta
-000004a0: 7069 2f62 6164 6765 2e73 7667 2220 616c  pi/badge.svg" al
-000004b0: 743d 2254 6573 7422 3e0a 2020 3c2f 613e  t="Test">.  </a>
-000004c0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-000004d0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000004e0: 6a65 6374 2f73 7461 632d 6661 7374 6170  ject/stac-fastap
-000004f0: 6922 2074 6172 6765 743d 225f 626c 616e  i" target="_blan
-00000500: 6b22 3e0a 2020 2020 2020 3c69 6d67 2073  k">.      <img s
-00000510: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000520: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000530: 762f 7374 6163 2d66 6173 7461 7069 3f63  v/stac-fastapi?c
-00000540: 6f6c 6f72 3d25 3233 3334 4430 3538 266c  olor=%2334D058&l
-00000550: 6162 656c 3d70 7970 6925 3230 7061 636b  abel=pypi%20pack
-00000560: 6167 6522 2061 6c74 3d22 5061 636b 6167  age" alt="Packag
-00000570: 6520 7665 7273 696f 6e22 3e0a 2020 3c2f  e version">.  </
-00000580: 613e 0a20 203c 6120 6872 6566 3d22 6874  a>.  <a href="ht
-00000590: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000005a0: 2f73 7461 632d 7574 696c 732f 7374 6163  /stac-utils/stac
-000005b0: 2d66 6173 7461 7069 2f62 6c6f 622f 6d61  -fastapi/blob/ma
-000005c0: 696e 2f4c 4943 454e 5345 2220 7461 7267  in/LICENSE" targ
-000005d0: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
-000005e0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-000005f0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000600: 2e69 6f2f 6769 7468 7562 2f6c 6963 656e  .io/github/licen
-00000610: 7365 2f73 7461 632d 7574 696c 732f 7374  se/stac-utils/st
-00000620: 6163 2d66 6173 7461 7069 2e73 7667 2220  ac-fastapi.svg" 
-00000630: 616c 743d 2244 6f77 6e6c 6f61 6473 223e  alt="Downloads">
-00000640: 0a20 203c 2f61 3e0a 3c2f 703e 0a0a 2d2d  .  </a>.</p>..--
-00000650: 2d0a 0a2a 2a44 6f63 756d 656e 7461 7469  -..**Documentati
-00000660: 6f6e 2a2a 3a20 5b68 7474 7073 3a2f 2f73  on**: [https://s
-00000670: 7461 632d 7574 696c 732e 6769 7468 7562  tac-utils.github
-00000680: 2e69 6f2f 7374 6163 2d66 6173 7461 7069  .io/stac-fastapi
-00000690: 2f5d 2868 7474 7073 3a2f 2f73 7461 632d  /](https://stac-
-000006a0: 7574 696c 732e 6769 7468 7562 2e69 6f2f  utils.github.io/
-000006b0: 7374 6163 2d66 6173 7461 7069 2f29 0a0a  stac-fastapi/)..
-000006c0: 2a2a 536f 7572 6365 2043 6f64 652a 2a3a  **Source Code**:
-000006d0: 205b 6874 7470 733a 2f2f 6769 7468 7562   [https://github
-000006e0: 2e63 6f6d 2f73 7461 632d 7574 696c 732f  .com/stac-utils/
-000006f0: 7374 6163 2d66 6173 7461 7069 5d28 6874  stac-fastapi](ht
-00000700: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000710: 2f73 7461 632d 7574 696c 732f 7374 6163  /stac-utils/stac
-00000720: 2d66 6173 7461 7069 290a 0a2d 2d2d 0a0a  -fastapi)..---..
-00000730: 5374 6163 2046 6173 7441 5049 2075 7369  Stac FastAPI usi
-00000740: 6e67 2074 6865 205b 5047 5374 6163 5d28  ng the [PGStac](
-00000750: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000760: 6f6d 2f73 7461 632d 7574 696c 732f 7067  om/stac-utils/pg
-00000770: 7374 6163 2920 6261 636b 656e 642e 0a0a  stac) backend...
-00000780: 5b50 4753 7461 635d 2868 7474 7073 3a2f  [PGStac](https:/
-00000790: 2f67 6974 6875 622e 636f 6d2f 7374 6163  /github.com/stac
-000007a0: 2d75 7469 6c73 2f70 6773 7461 6329 2069  -utils/pgstac) i
-000007b0: 7320 6120 7365 7061 7261 7465 6c79 206d  s a separately m
-000007c0: 616e 6167 6564 2050 6f73 7467 7265 5351  anaged PostgreSQ
-000007d0: 4c20 6461 7461 6261 7365 2074 6861 7420  L database that 
-000007e0: 6973 2064 6573 6967 6e65 6420 666f 7220  is designed for 
-000007f0: 656e 6861 6e63 6564 2070 6572 666f 726d  enhanced perform
-00000800: 616e 6365 2074 6f20 6265 2061 626c 6520  ance to be able 
-00000810: 746f 2073 6361 6c65 2053 7461 6320 4661  to scale Stac Fa
-00000820: 7374 4150 4920 746f 2062 6520 6162 6c65  stAPI to be able
-00000830: 2074 6f20 6566 6669 6369 656e 746c 7920   to efficiently 
-00000840: 6861 6e64 6c65 2068 756e 6472 6564 7320  handle hundreds 
-00000850: 6f66 206d 696c 6c69 6f6e 7320 6f66 2072  of millions of r
-00000860: 6563 6f72 6473 2e20 5b50 4753 7461 635d  ecords. [PGStac]
-00000870: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000880: 636f 6d2f 7374 6163 2d75 7469 6c73 2f70  com/stac-utils/p
-00000890: 6773 7461 6329 2061 7574 6f6d 6174 6963  gstac) automatic
-000008a0: 616c 6c79 2069 6e63 6c75 6465 7320 696e  ally includes in
-000008b0: 6465 7865 7320 6f6e 2049 7465 6d20 6964  dexes on Item id
-000008c0: 2c20 436f 6c6c 6563 7469 6f6e 2069 642c  , Collection id,
-000008d0: 2049 7465 6d20 4765 6f6d 6574 7279 2c20   Item Geometry, 
-000008e0: 4974 656d 2044 6174 6574 696d 652c 2061  Item Datetime, a
-000008f0: 6e64 2061 6e20 496e 6465 7820 666f 7220  nd an Index for 
-00000900: 6571 7561 6c69 7479 2063 6865 636b 7320  equality checks 
-00000910: 6f6e 2061 6e79 206b 6579 2069 6e20 4974  on any key in It
-00000920: 656d 2050 726f 7065 7274 6965 732e 2041  em Properties. A
-00000930: 6464 6974 696f 6e61 6c20 696e 6465 7865  dditional indexe
-00000940: 7320 6d61 7920 6265 2061 6464 6564 2074  s may be added t
-00000950: 6f20 4974 656d 2050 726f 7065 7274 6965  o Item Propertie
-00000960: 7320 746f 2073 7065 6564 2075 7020 7468  s to speed up th
-00000970: 6520 7573 6520 6f66 206f 7264 6572 2c20  e use of order, 
-00000980: 3c2c 203c 3d2c 203e 2c20 616e 6420 3e3d  <, <=, >, and >=
-00000990: 2071 7565 7269 6573 2e0a 0a53 7461 6320   queries...Stac 
-000009a0: 4661 7374 4150 4920 6163 7473 2061 7320  FastAPI acts as 
-000009b0: 7468 6520 4854 5450 2069 6e74 6572 6661  the HTTP interfa
-000009c0: 6365 2076 616c 6964 6174 696e 6720 616e  ce validating an
-000009d0: 7920 7265 7175 6573 7473 2061 6e64 2064  y requests and d
-000009e0: 6174 6120 7468 6174 2069 7320 7365 6e74  ata that is sent
-000009f0: 2074 6f20 7468 6520 5b50 4753 7461 635d   to the [PGStac]
-00000a00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000a10: 636f 6d2f 7374 6163 2d75 7469 6c73 2f70  com/stac-utils/p
-00000a20: 6773 7461 6329 2062 6163 6b65 6e64 2061  gstac) backend a
-00000a30: 6e64 2061 6464 7320 696e 204c 696e 6b20  nd adds in Link 
-00000a40: 6974 656d 7320 6f6e 2064 6174 6120 7265  items on data re
-00000a50: 7475 726e 2072 656c 6174 6976 6520 746f  turn relative to
-00000a60: 2074 6865 2073 6572 7669 6365 2068 6f73   the service hos
-00000a70: 742e 2041 6c6c 206f 7468 6572 2070 726f  t. All other pro
-00000a80: 6365 7373 696e 6720 616e 6420 7365 6172  cessing and sear
-00000a90: 6368 2069 7320 7072 6f76 6964 6564 2064  ch is provided d
-00000aa0: 6972 6563 746c 7920 7573 696e 6720 5047  irectly using PG
-00000ab0: 5374 6163 2070 726f 6365 6475 7261 6c20  Stac procedural 
-00000ac0: 7371 6c20 2f20 706c 7067 7371 6c20 6675  sql / plpgsql fu
-00000ad0: 6e63 7469 6f6e 7320 6f6e 2074 6865 2064  nctions on the d
-00000ae0: 6174 6162 6173 652e 0a0a 5047 5374 6163  atabase...PGStac
-00000af0: 2073 746f 7265 7320 616c 6c20 636f 6c6c   stores all coll
-00000b00: 6563 7469 6f6e 2061 6e64 2069 7465 6d20  ection and item 
-00000b10: 7265 636f 7264 7320 6173 206a 736f 6e62  records as jsonb
-00000b20: 2066 6965 6c64 7320 6578 6163 746c 7920   fields exactly 
-00000b30: 6173 2074 6865 7920 636f 6d65 2069 6e20  as they come in 
-00000b40: 616c 6c6f 7769 6e67 2066 6f72 2061 6e79  allowing for any
-00000b50: 2063 7573 746f 6d20 6669 656c 6473 2074   custom fields t
-00000b60: 6f20 6265 2073 746f 7265 6420 616e 6420  o be stored and 
-00000b70: 7265 7472 6965 7665 6420 7472 616e 7370  retrieved transp
-00000b80: 6172 656e 746c 792e 0a0a 5768 696c 6520  arently...While 
-00000b90: 7468 6520 5374 6163 2053 6f72 7420 4578  the Stac Sort Ex
-00000ba0: 7465 6e73 696f 6e20 6973 2066 756c 6c79  tension is fully
-00000bb0: 2073 7570 706f 7274 6564 2c20 5b50 4753   supported, [PGS
-00000bc0: 7461 635d 2868 7474 7073 3a2f 2f67 6974  tac](https://git
-00000bd0: 6875 622e 636f 6d2f 7374 6163 2d75 7469  hub.com/stac-uti
-00000be0: 6c73 2f70 6773 7461 6329 2069 7320 7061  ls/pgstac) is pa
-00000bf0: 7274 6963 756c 6172 6c79 2065 6e68 616e  rticularly enhan
-00000c00: 6365 6420 746f 2062 6520 6162 6c65 2074  ced to be able t
-00000c10: 6f20 736f 7274 2062 7920 6461 7465 7469  o sort by dateti
-00000c20: 6d65 2028 6569 7468 6572 2061 7363 656e  me (either ascen
-00000c30: 6469 6e67 206f 7220 6465 7363 656e 6469  ding or descendi
-00000c40: 6e67 292e 2053 6f72 7469 6e67 2062 7920  ng). Sorting by 
-00000c50: 616e 7974 6869 6e67 206f 7468 6572 2074  anything other t
-00000c60: 6861 6e20 6461 7465 7469 6d65 2028 7468  han datetime (th
-00000c70: 6520 6465 6661 756c 7420 6966 206e 6f20  e default if no 
-00000c80: 736f 7274 2069 7320 7370 6563 6966 6965  sort is specifie
-00000c90: 6429 206f 6e20 7665 7279 206c 6172 6765  d) on very large
-00000ca0: 2053 7461 6320 7265 706f 7369 746f 7269   Stac repositori
-00000cb0: 6573 2077 6974 686f 7574 2076 6572 7920  es without very 
-00000cc0: 7370 6563 6966 6963 2071 7565 7279 206c  specific query l
-00000cd0: 696d 6974 7320 2869 6520 7365 6c65 6374  imits (ie select
-00000ce0: 696e 6720 6120 7369 6e67 6c65 2064 6179  ing a single day
-00000cf0: 2064 6174 6520 7261 6e67 6529 2077 696c   date range) wil
-00000d00: 6c20 6e6f 7420 6861 7665 2074 6865 2073  l not have the s
-00000d10: 616d 6520 7065 7266 6f72 6d61 6e63 652e  ame performance.
-00000d20: 2046 6f72 206d 6f72 6520 7468 616e 206d   For more than m
-00000d30: 696c 6c69 6f6e 7320 6f66 2072 6563 6f72  illions of recor
-00000d40: 6473 2069 7420 6973 2072 6563 6f6d 6d65  ds it is recomme
-00000d50: 6e64 6564 2074 6f20 6569 7468 6572 2073  nded to either s
-00000d60: 6574 2061 206c 6f77 2063 6f6e 6e65 6374  et a low connect
-00000d70: 696f 6e20 7469 6d65 6f75 7420 6f6e 2050  ion timeout on P
-00000d80: 6f73 7467 7265 5351 4c20 6f72 2074 6f20  ostgreSQL or to 
-00000d90: 6469 7361 626c 6520 7573 6520 6f66 2074  disable use of t
-00000da0: 6865 2053 6f72 7420 4578 7465 6e73 696f  he Sort Extensio
-00000db0: 6e2e 0a0a 6073 7461 632d 6661 7374 6170  n...`stac-fastap
-00000dc0: 6920 7067 7374 6163 6020 7761 7320 696e  i pgstac` was in
-00000dd0: 6974 6961 6c6c 7920 6164 6465 6420 746f  itially added to
-00000de0: 2060 7374 6163 2d66 6173 7461 7069 6020   `stac-fastapi` 
-00000df0: 6279 205b 6465 7665 6c6f 706d 656e 7473  by [developments
-00000e00: 6565 645d 2868 7474 7073 3a2f 2f67 6974  eed](https://git
-00000e10: 6875 622e 636f 6d2f 6465 7665 6c6f 706d  hub.com/developm
-00000e20: 656e 7473 6565 6429 2e0a 0a23 2320 496e  entseed)...## In
-00000e30: 7374 616c 6c61 7469 6f6e 0a0a 6060 6073  stallation..```s
-00000e40: 6865 6c6c 0a67 6974 2063 6c6f 6e65 2068  hell.git clone h
-00000e50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000e60: 6d2f 7374 6163 2d75 7469 6c73 2f73 7461  m/stac-utils/sta
-00000e70: 632d 6661 7374 6170 692e 6769 740a 6364  c-fastapi.git.cd
-00000e80: 2073 7461 632d 6661 7374 6170 690a 7069   stac-fastapi.pi
-00000e90: 7020 696e 7374 616c 6c20 2d65 205c 0a20  p install -e \. 
-00000ea0: 2020 2073 7461 635f 6661 7374 6170 692f     stac_fastapi/
-00000eb0: 6170 695b 6465 765d 205c 0a20 2020 2073  api[dev] \.    s
-00000ec0: 7461 635f 6661 7374 6170 692f 7479 7065  tac_fastapi/type
-00000ed0: 735b 6465 765d 205c 0a20 2020 2073 7461  s[dev] \.    sta
-00000ee0: 635f 6661 7374 6170 692f 6578 7465 6e73  c_fastapi/extens
-00000ef0: 696f 6e73 5b64 6576 5d20 5c0a 2020 2020  ions[dev] \.    
-00000f00: 7374 6163 5f66 6173 7461 7069 2f70 6773  stac_fastapi/pgs
-00000f10: 7461 635b 6465 762c 7365 7276 6572 5d0a  tac[dev,server].
-00000f20: 6060 600a 0a23 2323 2053 6574 7469 6e67  ```..### Setting
-00000f30: 730a 0a54 6f20 636f 6e66 6967 7572 6520  s..To configure 
-00000f40: 5047 5374 6163 2073 7461 632d 6661 7374  PGStac stac-fast
-00000f50: 6170 6920 746f 205b 6879 6472 6174 6520  api to [hydrate 
-00000f60: 7365 6172 6368 2072 6573 756c 7420 6974  search result it
-00000f70: 656d 7320 696e 2074 6865 2041 5049 5d28  ems in the API](
-00000f80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000f90: 6f6d 2f73 7461 632d 7574 696c 732f 7067  om/stac-utils/pg
-00000fa0: 7374 6163 2372 756e 7469 6d65 2d63 6f6e  stac#runtime-con
-00000fb0: 6669 6775 7261 7469 6f6e 7329 2c20 7365  figurations), se
-00000fc0: 7420 7468 6520 6055 5345 5f41 5049 5f48  t the `USE_API_H
-00000fd0: 5944 5241 5445 6020 656e 7669 726f 6e6d  YDRATE` environm
-00000fe0: 656e 7420 7661 7269 6162 6c65 2074 6f20  ent variable to 
-00000ff0: 6074 7275 6560 206f 7220 6578 706c 6963  `true` or explic
-00001000: 6974 6c79 2073 6574 2074 6865 206f 7074  itly set the opt
-00001010: 696f 6e20 696e 2074 6865 2050 4753 7461  ion in the PGSta
-00001020: 6320 5365 7474 696e 6773 206f 626a 6563  c Settings objec
-00001030: 742e 0a0a 2323 2320 4d69 6772 6174 696f  t...### Migratio
-00001040: 6e73 0a0a 5047 5374 6163 2069 7320 616e  ns..PGStac is an
-00001050: 2065 7874 6572 6e61 6c20 7072 6f6a 6563   external projec
-00001060: 7420 616e 6420 7468 6520 6d61 7920 6265  t and the may be
-00001070: 2075 7365 6420 6279 206d 756c 7469 706c   used by multipl
-00001080: 6520 6672 6f6e 7420 656e 6473 2e0a 466f  e front ends..Fo
-00001090: 7220 5374 6163 2046 6173 7441 5049 2064  r Stac FastAPI d
-000010a0: 6576 656c 6f70 6d65 6e74 2c20 6120 646f  evelopment, a do
-000010b0: 636b 6572 2069 6d61 6765 2028 7768 6963  cker image (whic
-000010c0: 6820 6973 2070 756c 6c65 6420 6173 2070  h is pulled as p
-000010d0: 6172 7420 6f66 2074 6865 2064 6f63 6b65  art of the docke
-000010e0: 722d 636f 6d70 6f73 6529 2069 7320 6176  r-compose) is av
-000010f0: 6169 6c61 626c 6520 6174 0a62 6974 6e65  ailable at.bitne
-00001100: 722f 7067 7374 6163 3a5b 7665 7273 696f  r/pgstac:[versio
-00001110: 6e5d 2074 6861 7420 6861 7320 7468 6520  n] that has the 
-00001120: 6675 6c6c 2064 6174 6162 6173 6520 616c  full database al
-00001130: 7265 6164 7920 7365 7420 7570 2066 6f72  ready set up for
-00001140: 2050 4753 7461 632e 0a0a 5468 6572 6520   PGStac...There 
-00001150: 6973 2061 6c73 6f20 6120 7079 7468 6f6e  is also a python
-00001160: 2075 7469 6c69 7479 2061 7320 7061 7274   utility as part
-00001170: 206f 6620 5047 5374 6163 2028 7079 7067   of PGStac (pypg
-00001180: 7374 6163 2920 7468 6174 2069 6e63 6c75  stac) that inclu
-00001190: 6465 7320 6120 6d69 6772 6174 696f 6e20  des a migration 
-000011a0: 7574 696c 6974 792e 2054 6865 2070 6773  utility. The pgs
-000011b0: 7461 630a 7665 7273 696f 6e20 7265 7175  tac.version requ
-000011c0: 6972 6564 2062 7920 7374 6163 2d66 6173  ired by stac-fas
-000011d0: 7461 7069 2f70 6773 7461 6320 6973 2070  tapi/pgstac is p
-000011e0: 696e 6e65 6420 6279 2075 7369 6e67 2074  inned by using t
-000011f0: 6865 2070 696e 6e65 6420 7665 7273 696f  he pinned versio
-00001200: 6e20 6f66 2070 7970 6773 7461 6320 696e  n of pypgstac in
-00001210: 2074 6865 205b 7365 7475 705d 2873 6574   the [setup](set
-00001220: 7570 2e70 7929 2066 696c 652e 0a0a 496e  up.py) file...In
-00001230: 206f 7264 6572 2074 6f20 6d69 6772 6174   order to migrat
-00001240: 6520 6461 7461 6261 7365 2076 6572 7369  e database versi
-00001250: 6f6e 7320 796f 7520 6361 6e20 7573 6520  ons you can use 
-00001260: 7468 6520 6d69 6772 6174 696f 6e20 7574  the migration ut
-00001270: 696c 6974 793a 0a0a 6060 6073 6865 6c6c  ility:..```shell
-00001280: 0a70 7970 6773 7461 6320 6d69 6772 6174  .pypgstac migrat
-00001290: 650a 6060 600a                           e.```.
+000002d0: 610a 4c69 6365 6e73 652d 4669 6c65 3a20  a.License-File: 
+000002e0: 4c49 4345 4e53 450a 0a23 2073 7461 632d  LICENSE..# stac-
+000002f0: 6661 7374 6170 692d 7067 7374 6163 0a0a  fastapi-pgstac..
+00000300: 5b21 5b47 6974 4875 6220 576f 726b 666c  [![GitHub Workfl
+00000310: 6f77 2053 7461 7475 735d 2868 7474 7073  ow Status](https
+00000320: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000330: 6f2f 6769 7468 7562 2f61 6374 696f 6e73  o/github/actions
+00000340: 2f77 6f72 6b66 6c6f 772f 7374 6174 7573  /workflow/status
+00000350: 2f73 7461 632d 7574 696c 732f 7374 6163  /stac-utils/stac
+00000360: 2d66 6173 7461 7069 2d70 6773 7461 632f  -fastapi-pgstac/
+00000370: 6369 6364 2e79 616d 6c3f 7374 796c 653d  cicd.yaml?style=
+00000380: 666f 722d 7468 652d 6261 6467 6529 5d28  for-the-badge)](
+00000390: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000003a0: 6f6d 2f73 7461 632d 7574 696c 732f 7374  om/stac-utils/st
+000003b0: 6163 2d66 6173 7461 7069 2d70 6773 7461  ac-fastapi-pgsta
+000003c0: 632f 6163 7469 6f6e 732f 776f 726b 666c  c/actions/workfl
+000003d0: 6f77 732f 6369 6364 2e79 616d 6c29 0a5b  ows/cicd.yaml).[
+000003e0: 215b 5079 5049 5d28 6874 7470 733a 2f2f  ![PyPI](https://
+000003f0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000400: 7970 692f 762f 7374 6163 2d66 6173 7461  ypi/v/stac-fasta
+00000410: 7069 2e70 6773 7461 633f 7374 796c 653d  pi.pgstac?style=
+00000420: 666f 722d 7468 652d 6261 6467 6529 5d28  for-the-badge)](
+00000430: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000440: 2f70 726f 6a65 6374 2f73 7461 632d 6661  /project/stac-fa
+00000450: 7374 6170 692e 7067 7374 6163 290a 5b21  stapi.pgstac).[!
+00000460: 5b44 6f63 756d 656e 7461 7469 6f6e 5d28  [Documentation](
+00000470: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000480: 6c64 732e 696f 2f67 6974 6875 622f 6163  lds.io/github/ac
+00000490: 7469 6f6e 732f 776f 726b 666c 6f77 2f73  tions/workflow/s
+000004a0: 7461 7475 732f 7374 6163 2d75 7469 6c73  tatus/stac-utils
+000004b0: 2f73 7461 632d 6661 7374 6170 692d 7067  /stac-fastapi-pg
+000004c0: 7374 6163 2f70 6167 6573 2e79 6d6c 3f6c  stac/pages.yml?l
+000004d0: 6162 656c 3d44 6f63 7326 7374 796c 653d  abel=Docs&style=
+000004e0: 666f 722d 7468 652d 6261 6467 6529 5d28  for-the-badge)](
+000004f0: 6874 7470 733a 2f2f 7374 6163 2d75 7469  https://stac-uti
+00000500: 6c73 2e67 6974 6875 622e 696f 2f73 7461  ls.github.io/sta
+00000510: 632d 6661 7374 6170 692d 7067 7374 6163  c-fastapi-pgstac
+00000520: 2f29 0a5b 215b 4c69 6365 6e73 655d 2868  /).[![License](h
+00000530: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000540: 6473 2e69 6f2f 6769 7468 7562 2f6c 6963  ds.io/github/lic
+00000550: 656e 7365 2f73 7461 632d 7574 696c 732f  ense/stac-utils/
+00000560: 7374 6163 2d66 6173 7461 7069 2d70 6773  stac-fastapi-pgs
+00000570: 7461 633f 7374 796c 653d 666f 722d 7468  tac?style=for-th
+00000580: 652d 6261 6467 6529 5d28 6874 7470 733a  e-badge)](https:
+00000590: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7461  //github.com/sta
+000005a0: 632d 7574 696c 732f 7374 6163 2d66 6173  c-utils/stac-fas
+000005b0: 7461 7069 2d70 6773 7461 632f 626c 6f62  tapi-pgstac/blob
+000005c0: 2f6d 6169 6e2f 4c49 4345 4e53 4529 0a0a  /main/LICENSE)..
+000005d0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+000005e0: 223e 0a20 203c 696d 6720 7372 633d 2268  ">.  <img src="h
+000005f0: 7474 7073 3a2f 2f75 7365 722d 696d 6167  ttps://user-imag
+00000600: 6573 2e67 6974 6875 6275 7365 7263 6f6e  es.githubusercon
+00000610: 7465 6e74 2e63 6f6d 2f31 3034 3037 3738  tent.com/1040778
+00000620: 382f 3137 3438 3933 3837 362d 3761 3362  8/174893876-7a3b
+00000630: 3562 3761 2d39 3561 352d 3438 6334 2d39  5b7a-95a5-48c4-9
+00000640: 6666 322d 6363 3430 3866 3162 3661 6639  ff2-cc408f1b6af9
+00000650: 2e70 6e67 2220 7374 796c 653d 2276 6572  .png" style="ver
+00000660: 7469 6361 6c2d 616c 6967 6e3a 206d 6964  tical-align: mid
+00000670: 646c 653b 206d 6178 2d77 6964 7468 3a20  dle; max-width: 
+00000680: 3430 3070 783b 206d 6178 2d68 6569 6768  400px; max-heigh
+00000690: 743a 2031 3030 7078 3b22 2068 6569 6768  t: 100px;" heigh
+000006a0: 743d 3130 3020 2f3e 0a20 203c 696d 6720  t=100 />.  <img 
+000006b0: 7372 633d 2268 7474 7073 3a2f 2f66 6173  src="https://fas
+000006c0: 7461 7069 2e74 6961 6e67 6f6c 6f2e 636f  tapi.tiangolo.co
+000006d0: 6d2f 696d 672f 6c6f 676f 2d6d 6172 6769  m/img/logo-margi
+000006e0: 6e2f 6c6f 676f 2d74 6561 6c2e 706e 6722  n/logo-teal.png"
+000006f0: 2061 6c74 3d22 4661 7374 4150 4922 2073   alt="FastAPI" s
+00000700: 7479 6c65 3d22 7665 7274 6963 616c 2d61  tyle="vertical-a
+00000710: 6c69 676e 3a20 6d69 6464 6c65 3b20 6d61  lign: middle; ma
+00000720: 782d 7769 6474 683a 2034 3030 7078 3b20  x-width: 400px; 
+00000730: 6d61 782d 6865 6967 6874 3a20 3130 3070  max-height: 100p
+00000740: 783b 2220 7769 6474 683d 3230 3020 2f3e  x;" width=200 />
+00000750: 0a3c 2f70 3e0a 0a5b 5067 5354 4143 5d28  .</p>..[PgSTAC](
+00000760: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000770: 6f6d 2f73 7461 632d 7574 696c 732f 7067  om/stac-utils/pg
+00000780: 7374 6163 2920 6261 636b 656e 6420 666f  stac) backend fo
+00000790: 7220 5b73 7461 632d 6661 7374 6170 695d  r [stac-fastapi]
+000007a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000007b0: 636f 6d2f 7374 6163 2d75 7469 6c73 2f73  com/stac-utils/s
+000007c0: 7461 632d 6661 7374 6170 6929 2c20 7468  tac-fastapi), th
+000007d0: 6520 5b46 6173 7441 5049 5d28 6874 7470  e [FastAPI](http
+000007e0: 733a 2f2f 6661 7374 6170 692e 7469 616e  s://fastapi.tian
+000007f0: 676f 6c6f 2e63 6f6d 2f29 2069 6d70 6c65  golo.com/) imple
+00000800: 6d65 6e74 6174 696f 6e20 6f66 2074 6865  mentation of the
+00000810: 205b 5354 4143 2041 5049 2073 7065 635d   [STAC API spec]
+00000820: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000830: 636f 6d2f 7261 6469 616e 7465 6172 7468  com/radiantearth
+00000840: 2f73 7461 632d 6170 692d 7370 6563 290a  /stac-api-spec).
+00000850: 0a23 2320 4f76 6572 7669 6577 0a0a 2a2a  .## Overview..**
+00000860: 7374 6163 2d66 6173 7461 7069 2d70 6773  stac-fastapi-pgs
+00000870: 7461 632a 2a20 6973 2061 6e20 4854 5450  tac** is an HTTP
+00000880: 2069 6e74 6572 6661 6365 2062 7569 6c74   interface built
+00000890: 2069 6e20 4661 7374 4150 492e 0a49 7420   in FastAPI..It 
+000008a0: 7661 6c69 6461 7465 7320 7265 7175 6573  validates reques
+000008b0: 7473 2061 6e64 2064 6174 6120 7365 6e74  ts and data sent
+000008c0: 2074 6f20 6120 5b50 6753 5441 435d 2868   to a [PgSTAC](h
+000008d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000008e0: 6d2f 7374 6163 2d75 7469 6c73 2f70 6773  m/stac-utils/pgs
+000008f0: 7461 6329 2062 6163 6b65 6e64 2c20 616e  tac) backend, an
+00000900: 6420 6164 6473 205b 6c69 6e6b 735d 2868  d adds [links](h
+00000910: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000920: 6d2f 7261 6469 616e 7465 6172 7468 2f73  m/radiantearth/s
+00000930: 7461 632d 7370 6563 2f62 6c6f 622f 6d61  tac-spec/blob/ma
+00000940: 7374 6572 2f69 7465 6d2d 7370 6563 2f69  ster/item-spec/i
+00000950: 7465 6d2d 7370 6563 2e6d 6423 6c69 6e6b  tem-spec.md#link
+00000960: 2d6f 626a 6563 7429 2074 6f20 7468 6520  -object) to the 
+00000970: 7265 7475 726e 6564 2064 6174 612e 0a41  returned data..A
+00000980: 6c6c 206f 7468 6572 2070 726f 6365 7373  ll other process
+00000990: 696e 6720 616e 6420 7365 6172 6368 2069  ing and search i
+000009a0: 7320 7072 6f76 6964 6564 2064 6972 6563  s provided direc
+000009b0: 746c 7920 7573 696e 6720 5067 5354 4143  tly using PgSTAC
+000009c0: 2070 726f 6365 6475 7261 6c20 7371 6c20   procedural sql 
+000009d0: 2f20 706c 7067 7371 6c20 6675 6e63 7469  / plpgsql functi
+000009e0: 6f6e 7320 6f6e 2074 6865 2064 6174 6162  ons on the datab
+000009f0: 6173 652e 0a50 6753 5441 4320 7374 6f72  ase..PgSTAC stor
+00000a00: 6573 2061 6c6c 2063 6f6c 6c65 6374 696f  es all collectio
+00000a10: 6e20 616e 6420 6974 656d 2072 6563 6f72  n and item recor
+00000a20: 6473 2061 7320 6a73 6f6e 6220 6669 656c  ds as jsonb fiel
+00000a30: 6473 2065 7861 6374 6c79 2061 7320 7468  ds exactly as th
+00000a40: 6579 2063 6f6d 6520 696e 2061 6c6c 6f77  ey come in allow
+00000a50: 696e 6720 666f 7220 616e 7920 6375 7374  ing for any cust
+00000a60: 6f6d 2066 6965 6c64 7320 746f 2062 6520  om fields to be 
+00000a70: 7374 6f72 6564 2061 6e64 2072 6574 7269  stored and retri
+00000a80: 6576 6564 2074 7261 6e73 7061 7265 6e74  eved transparent
+00000a90: 6c79 2e0a 0a23 2320 5573 6167 650a 0a50  ly...## Usage..P
+00000aa0: 6753 5441 4320 6973 2061 6e20 6578 7465  gSTAC is an exte
+00000ab0: 726e 616c 2070 726f 6a65 6374 2061 6e64  rnal project and
+00000ac0: 206d 6179 2062 6520 7573 6564 2062 7920   may be used by 
+00000ad0: 6d75 6c74 6970 6c65 2066 726f 6e74 2065  multiple front e
+00000ae0: 6e64 732e 0a46 6f72 2053 7461 6320 4661  nds..For Stac Fa
+00000af0: 7374 4150 4920 6465 7665 6c6f 706d 656e  stAPI developmen
+00000b00: 742c 2061 2044 6f63 6b65 7220 696d 6167  t, a Docker imag
+00000b10: 6520 2877 6869 6368 2069 7320 7075 6c6c  e (which is pull
+00000b20: 6564 2061 7320 7061 7274 206f 6620 7468  ed as part of th
+00000b30: 6520 646f 636b 6572 2d63 6f6d 706f 7365  e docker-compose
+00000b40: 2920 6973 2061 7661 696c 6162 6c65 2076  ) is available v
+00000b50: 6961 2074 6865 205b 4769 7468 7562 2063  ia the [Github c
+00000b60: 6f6e 7461 696e 6572 2072 6567 6973 7472  ontainer registr
+00000b70: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
+00000b80: 622e 636f 6d2f 7374 6163 2d75 7469 6c73  b.com/stac-utils
+00000b90: 2f70 6773 7461 632f 706b 6773 2f63 6f6e  /pgstac/pkgs/con
+00000ba0: 7461 696e 6572 2f70 6773 7461 632f 3831  tainer/pgstac/81
+00000bb0: 3638 3937 3934 3f74 6167 3d6c 6174 6573  689794?tag=lates
+00000bc0: 7429 2e0a 5468 6520 5067 5354 4143 2076  t)..The PgSTAC v
+00000bd0: 6572 7369 6f6e 2072 6571 7569 7265 6420  ersion required 
+00000be0: 6279 202a 2a73 7461 632d 6661 7374 6170  by **stac-fastap
+00000bf0: 692d 7067 7374 6163 2a2a 2069 7320 666f  i-pgstac** is fo
+00000c00: 756e 6420 696e 2074 6865 205b 7365 7475  und in the [setu
+00000c10: 705d 2868 7474 703a 2f2f 6769 7468 7562  p](http://github
+00000c20: 2e63 6f6d 2f73 7461 632d 7574 696c 732f  .com/stac-utils/
+00000c30: 7374 6163 2d66 6173 7461 7069 2d70 6773  stac-fastapi-pgs
+00000c40: 7461 632f 626c 6f62 2f6d 6169 6e2f 7365  tac/blob/main/se
+00000c50: 7475 702e 7079 2920 6669 6c65 2e0a 0a23  tup.py) file...#
+00000c60: 2323 2053 6f72 7469 6e67 0a0a 5768 696c  ## Sorting..Whil
+00000c70: 6520 7468 6520 5354 4143 205b 536f 7274  e the STAC [Sort
+00000c80: 2045 7874 656e 7369 6f6e 5d28 6874 7470   Extension](http
+00000c90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000ca0: 7461 632d 6170 692d 6578 7465 6e73 696f  tac-api-extensio
+00000cb0: 6e73 2f73 6f72 7429 2069 7320 6675 6c6c  ns/sort) is full
+00000cc0: 7920 7375 7070 6f72 7465 642c 205b 5067  y supported, [Pg
+00000cd0: 5354 4143 5d28 6874 7470 733a 2f2f 6769  STAC](https://gi
+00000ce0: 7468 7562 2e63 6f6d 2f73 7461 632d 7574  thub.com/stac-ut
+00000cf0: 696c 732f 7067 7374 6163 2920 6973 2070  ils/pgstac) is p
+00000d00: 6172 7469 6375 6c61 726c 7920 656e 6861  articularly enha
+00000d10: 6e63 6564 2074 6f20 6265 2061 626c 6520  nced to be able 
+00000d20: 746f 2073 6f72 7420 6279 2064 6174 6574  to sort by datet
+00000d30: 696d 6520 2865 6974 6865 7220 6173 6365  ime (either asce
+00000d40: 6e64 696e 6720 6f72 2064 6573 6365 6e64  nding or descend
+00000d50: 696e 6729 2e0a 536f 7274 696e 6720 6279  ing)..Sorting by
+00000d60: 2061 6e79 7468 696e 6720 6f74 6865 7220   anything other 
+00000d70: 7468 616e 2064 6174 6574 696d 6520 2874  than datetime (t
+00000d80: 6865 2064 6566 6175 6c74 2069 6620 6e6f  he default if no
+00000d90: 2073 6f72 7420 6973 2073 7065 6369 6669   sort is specifi
+00000da0: 6564 2920 6f6e 2076 6572 7920 6c61 7267  ed) on very larg
+00000db0: 6520 5354 4143 2072 6570 6f73 6974 6f72  e STAC repositor
+00000dc0: 6965 7320 7769 7468 6f75 7420 7665 7279  ies without very
+00000dd0: 2073 7065 6369 6669 6320 7175 6572 7920   specific query 
+00000de0: 6c69 6d69 7473 2028 6965 2073 656c 6563  limits (ie selec
+00000df0: 7469 6e67 2061 2073 696e 676c 6520 6461  ting a single da
+00000e00: 7920 6461 7465 2072 616e 6765 2920 7769  y date range) wi
+00000e10: 6c6c 206e 6f74 2068 6176 6520 7468 6520  ll not have the 
+00000e20: 7361 6d65 2070 6572 666f 726d 616e 6365  same performance
+00000e30: 2e0a 466f 7220 6d6f 7265 2074 6861 6e20  ..For more than 
+00000e40: 6d69 6c6c 696f 6e73 206f 6620 7265 636f  millions of reco
+00000e50: 7264 7320 6974 2069 7320 7265 636f 6d6d  rds it is recomm
+00000e60: 656e 6465 6420 746f 2065 6974 6865 7220  ended to either 
+00000e70: 7365 7420 6120 6c6f 7720 636f 6e6e 6563  set a low connec
+00000e80: 7469 6f6e 2074 696d 656f 7574 206f 6e20  tion timeout on 
+00000e90: 506f 7374 6772 6553 514c 206f 7220 746f  PostgreSQL or to
+00000ea0: 2064 6973 6162 6c65 2075 7365 206f 6620   disable use of 
+00000eb0: 7468 6520 536f 7274 2045 7874 656e 7369  the Sort Extensi
+00000ec0: 6f6e 2e0a 0a23 2323 2048 7964 7261 7469  on...### Hydrati
+00000ed0: 6f6e 0a0a 546f 2063 6f6e 6669 6775 7265  on..To configure
+00000ee0: 202a 2a73 7461 632d 6661 7374 6170 692d   **stac-fastapi-
+00000ef0: 7067 7374 6163 2a2a 2074 6f20 5b68 7964  pgstac** to [hyd
+00000f00: 7261 7465 2073 6561 7263 6820 7265 7375  rate search resu
+00000f10: 6c74 2069 7465 6d73 2069 6e20 7468 6520  lt items in the 
+00000f20: 4150 495d 2868 7474 7073 3a2f 2f73 7461  API](https://sta
+00000f30: 632d 7574 696c 732e 6769 7468 7562 2e69  c-utils.github.i
+00000f40: 6f2f 7067 7374 6163 2f70 6773 7461 632f  o/pgstac/pgstac/
+00000f50: 2372 756e 7469 6d65 2d63 6f6e 6669 6775  #runtime-configu
+00000f60: 7261 7469 6f6e 7329 2c20 7365 7420 7468  rations), set th
+00000f70: 6520 6055 5345 5f41 5049 5f48 5944 5241  e `USE_API_HYDRA
+00000f80: 5445 6020 656e 7669 726f 6e6d 656e 7420  TE` environment 
+00000f90: 7661 7269 6162 6c65 2074 6f20 6074 7275  variable to `tru
+00000fa0: 6560 206f 7220 6578 706c 6963 6974 6c79  e` or explicitly
+00000fb0: 2073 6574 2074 6865 206f 7074 696f 6e20   set the option 
+00000fc0: 696e 2074 6865 2050 4753 7461 6320 5365  in the PGStac Se
+00000fd0: 7474 696e 6773 206f 626a 6563 742e 0a0a  ttings object...
+00000fe0: 2323 2320 4d69 6772 6174 696f 6e73 0a0a  ### Migrations..
+00000ff0: 5468 6572 6520 6973 2061 2050 7974 686f  There is a Pytho
+00001000: 6e20 7574 696c 6974 7920 6173 2070 6172  n utility as par
+00001010: 7420 6f66 2050 6753 5441 4320 285b 7079  t of PgSTAC ([py
+00001020: 7067 7374 6163 5d28 6874 7470 733a 2f2f  pgstac](https://
+00001030: 7374 6163 2d75 7469 6c73 2e67 6974 6875  stac-utils.githu
+00001040: 622e 696f 2f70 6773 7461 632f 7079 7067  b.io/pgstac/pypg
+00001050: 7374 6163 2f29 2920 7468 6174 2069 6e63  stac/)) that inc
+00001060: 6c75 6465 7320 6120 6d69 6772 6174 696f  ludes a migratio
+00001070: 6e20 7574 696c 6974 792e 0a54 6f20 7573  n utility..To us
+00001080: 653a 0a0a 6060 6073 6865 6c6c 0a70 7970  e:..```shell.pyp
+00001090: 6773 7461 6320 6d69 6772 6174 650a 6060  gstac migrate.``
+000010a0: 600a 0a23 2320 436f 6e74 7269 6275 7469  `..## Contributi
+000010b0: 6e67 0a0a 5365 6520 5b43 4f4e 5452 4942  ng..See [CONTRIB
+000010c0: 5554 494e 475d 2868 7474 7073 3a2f 2f67  UTING](https://g
+000010d0: 6974 6875 622e 636f 6d2f 7374 6163 2d75  ithub.com/stac-u
+000010e0: 7469 6c73 2f73 7461 632d 6661 7374 6170  tils/stac-fastap
+000010f0: 692d 7067 7374 6163 2f62 6c6f 622f 6d61  i-pgstac/blob/ma
+00001100: 696e 2f43 4f4e 5452 4942 5554 494e 472e  in/CONTRIBUTING.
+00001110: 6d64 2920 666f 7220 6465 7461 696c 6564  md) for detailed
+00001120: 2063 6f6e 7472 6962 7574 696f 6e20 696e   contribution in
+00001130: 7374 7275 6374 696f 6e73 2e0a 0a54 6f20  structions...To 
+00001140: 696e 7374 616c 6c3a 0a0a 6060 6073 6865  install:..```she
+00001150: 6c6c 0a67 6974 2063 6c6f 6e65 2068 7474  ll.git clone htt
+00001160: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001170: 7374 6163 2d75 7469 6c73 2f73 7461 632d  stac-utils/stac-
+00001180: 6661 7374 6170 692d 7067 7374 6163 0a63  fastapi-pgstac.c
+00001190: 6420 7374 6163 2d66 6173 7461 7069 2d70  d stac-fastapi-p
+000011a0: 6773 7461 630a 7069 7020 696e 7374 616c  gstac.pip instal
+000011b0: 6c20 2d65 2022 2e5b 6465 762c 7365 7276  l -e ".[dev,serv
+000011c0: 6572 2c64 6f63 735d 220a 6060 600a 0a54  er,docs]".```..T
+000011d0: 6f20 7465 7374 3a0a 0a60 6060 7368 656c  o test:..```shel
+000011e0: 6c0a 6d61 6b65 2074 6573 740a 6060 600a  l.make test.```.
+000011f0: 0a55 7365 2047 6974 6875 6220 5b50 756c  .Use Github [Pul
+00001200: 6c20 5265 7175 6573 7473 5d28 6874 7470  l Requests](http
+00001210: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00001220: 7461 632d 7574 696c 732f 7374 6163 2d66  tac-utils/stac-f
+00001230: 6173 7461 7069 2d70 6773 7461 632f 7075  astapi-pgstac/pu
+00001240: 6c6c 7329 2074 6f20 7072 6f76 6964 6520  lls) to provide 
+00001250: 6e65 7720 6665 6174 7572 6573 206f 7220  new features or 
+00001260: 746f 2072 6571 7565 7374 2072 6576 6965  to request revie
+00001270: 7720 6f66 2064 7261 6674 2063 6f64 652c  w of draft code,
+00001280: 2061 6e64 2075 7365 205b 4973 7375 6573   and use [Issues
+00001290: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000012a0: 2e63 6f6d 2f73 7461 632d 7574 696c 732f  .com/stac-utils/
+000012b0: 7374 6163 2d66 6173 7461 7069 2d70 6773  stac-fastapi-pgs
+000012c0: 7461 632f 6973 7375 6573 2920 746f 2072  tac/issues) to r
+000012d0: 6570 6f72 7420 6275 6773 206f 7220 7265  eport bugs or re
+000012e0: 7175 6573 7420 6e65 7720 6665 6174 7572  quest new featur
+000012f0: 6573 2e0a 0a23 2323 2044 6f63 756d 656e  es...### Documen
+00001300: 7461 7469 6f6e 0a0a 546f 2062 7569 6c64  tation..To build
+00001310: 2074 6865 2064 6f63 733a 0a0a 6060 6073   the docs:..```s
+00001320: 6865 6c6c 0a6d 616b 6520 646f 6373 0a60  hell.make docs.`
+00001330: 6060 0a0a 5468 656e 2c20 7365 7276 6520  ``..Then, serve 
+00001340: 7468 6520 646f 6373 2076 6961 2061 206c  the docs via a l
+00001350: 6f63 616c 2048 5454 5020 7365 7276 6572  ocal HTTP server
+00001360: 3a0a 0a60 6060 7368 656c 6c0a 6d6b 646f  :..```shell.mkdo
+00001370: 6373 2073 6572 7665 0a60 6060 0a0a 2323  cs serve.```..##
+00001380: 2048 6973 746f 7279 0a0a 2a2a 7374 6163   History..**stac
+00001390: 2d66 6173 7461 7069 2d70 6773 7461 632a  -fastapi-pgstac*
+000013a0: 2a20 7761 7320 696e 6974 6961 6c6c 7920  * was initially 
+000013b0: 6164 6465 6420 746f 202a 2a73 7461 632d  added to **stac-
+000013c0: 6661 7374 6170 692a 2a20 6279 205b 6465  fastapi** by [de
+000013d0: 7665 6c6f 706d 656e 7473 6565 645d 2868  velopmentseed](h
+000013e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000013f0: 6d2f 6465 7665 6c6f 706d 656e 7473 6565  m/developmentsee
+00001400: 6429 2e0a 496e 2041 7072 696c 206f 6620  d)..In April of 
+00001410: 3230 3233 2c20 6974 2077 6173 2072 656d  2023, it was rem
+00001420: 6f76 6564 2066 726f 6d20 7468 6520 636f  oved from the co
+00001430: 7265 202a 2a73 7461 632d 6661 7374 6170  re **stac-fastap
+00001440: 692a 2a20 7265 706f 7369 746f 7279 2061  i** repository a
+00001450: 6e64 206d 6f76 6564 2074 6f20 6974 7320  nd moved to its 
+00001460: 6375 7272 656e 7420 6c6f 6361 7469 6f6e  current location
+00001470: 2028 3c68 7474 703a 2f2f 6769 7468 7562   (<http://github
+00001480: 2e63 6f6d 2f73 7461 632d 7574 696c 2f73  .com/stac-util/s
+00001490: 7461 632d 6661 7374 6170 692d 7067 7374  tac-fastapi-pgst
+000014a0: 6163 3e29 2e0a 0a23 2320 4c69 6365 6e73  ac>)...## Licens
+000014b0: 650a 0a5b 4d49 545d 2868 7474 7073 3a2f  e..[MIT](https:/
+000014c0: 2f67 6974 6875 622e 636f 6d2f 7374 6163  /github.com/stac
+000014d0: 2d75 7469 6c73 2f73 7461 632d 6661 7374  -utils/stac-fast
+000014e0: 6170 692d 7067 7374 6163 2f62 6c6f 622f  api-pgstac/blob/
+000014f0: 6d61 696e 2f4c 4943 454e 5345 290a 0a3c  main/LICENSE)..<
+00001500: 212d 2d20 6d61 726b 646f 776e 6c69 6e74  !-- markdownlint
+00001510: 2d64 6973 6162 6c65 2d66 696c 6520 4d44  -disable-file MD
+00001520: 3033 3320 2d2d 3e0a                      033 -->.
```

### Comparing `stac-fastapi.pgstac-2.4.5/setup.py` & `stac-fastapi.pgstac-2.4.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,21 +18,25 @@
     "brotli_asgi",
     "pygeofilter>=0.2",
     "pypgstac==0.7.*",
 ]
 
 extra_reqs = {
     "dev": [
+        "pystac[validation]",
         "pypgstac[psycopg]==0.7.*",
         "pytest",
         "pytest-cov",
         "pytest-asyncio>=0.17",
         "pre-commit",
         "requests",
+        "shapely",
         "httpx",
+        "twine",
+        "wheel",
     ],
     "docs": ["mkdocs", "mkdocs-material", "pdocs"],
     "server": ["uvicorn[standard]==0.19.0"],
     "awslambda": ["mangum"],
 }
 
 
@@ -50,15 +54,15 @@
         "License :: OSI Approved :: MIT License",
     ],
     keywords="STAC FastAPI COG",
     author="David Bitner",
     author_email="david@developmentseed.org",
     url="https://github.com/stac-utils/stac-fastapi",
     license="MIT",
-    packages=find_namespace_packages(exclude=["alembic", "tests", "scripts"]),
+    packages=find_namespace_packages(exclude=["tests", "scripts"]),
     zip_safe=False,
     install_requires=install_requires,
     tests_require=extra_reqs["dev"],
     extras_require=extra_reqs,
     entry_points={
         "console_scripts": ["stac-fastapi-pgstac=stac_fastapi.pgstac.app:run"]
     },
```

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/app.py` & `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/app.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 the ENABLED_EXTENSIONS environment variable (e.g. `transactions,sort,query`).
 If the variable is not set, enables all extensions.
 """
 
 import os
 
 from fastapi.responses import ORJSONResponse
-
 from stac_fastapi.api.app import StacApi
 from stac_fastapi.api.models import create_get_request_model, create_post_request_model
 from stac_fastapi.extensions.core import (
     ContextExtension,
     FieldsExtension,
     FilterExtension,
     SortExtension,
     TokenPaginationExtension,
     TransactionExtension,
 )
 from stac_fastapi.extensions.third_party import BulkTransactionExtension
+
 from stac_fastapi.pgstac.config import Settings
 from stac_fastapi.pgstac.core import CoreCrudClient
 from stac_fastapi.pgstac.db import close_db_connection, connect_to_db
 from stac_fastapi.pgstac.extensions import QueryExtension
 from stac_fastapi.pgstac.extensions.filter import FiltersClient
 from stac_fastapi.pgstac.transactions import BulkTransactionsClient, TransactionsClient
 from stac_fastapi.pgstac.types.search import PgstacSearch
```

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/config.py` & `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Postgres API configuration."""
 
 from typing import Type
 from urllib.parse import quote
 
+from stac_fastapi.types.config import ApiSettings
+
 from stac_fastapi.pgstac.types.base_item_cache import (
     BaseItemCache,
     DefaultBaseItemCache,
 )
-from stac_fastapi.types.config import ApiSettings
 
 
 class Settings(ApiSettings):
     """Postgres-specific API settings.
 
     Attributes:
         postgres_user: postgres username.
```

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/core.py` & `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,51 +4,48 @@
 from typing import Any, Dict, List, Optional, Union
 from urllib.parse import unquote_plus, urljoin
 
 import attr
 import orjson
 from asyncpg.exceptions import InvalidDatetimeFormatError
 from buildpg import render
-from fastapi import HTTPException
+from fastapi import HTTPException, Request
 from pydantic import ValidationError
 from pygeofilter.backends.cql2_json import to_cql2
 from pygeofilter.parsers.cql2_text import parse as parse_cql2_text
 from pypgstac.hydration import hydrate
+from stac_fastapi.types.core import AsyncBaseCoreClient
+from stac_fastapi.types.errors import InvalidQueryParameter, NotFoundError
+from stac_fastapi.types.requests import get_base_url
+from stac_fastapi.types.stac import Collection, Collections, Item, ItemCollection
 from stac_pydantic.links import Relations
 from stac_pydantic.shared import MimeTypes
-from starlette.requests import Request
 
 from stac_fastapi.pgstac.config import Settings
 from stac_fastapi.pgstac.models.links import (
     CollectionLinks,
     ItemCollectionLinks,
     ItemLinks,
     PagingLinks,
 )
 from stac_fastapi.pgstac.types.search import PgstacSearch
 from stac_fastapi.pgstac.utils import filter_fields
-from stac_fastapi.types.core import AsyncBaseCoreClient
-from stac_fastapi.types.errors import InvalidQueryParameter, NotFoundError
-from stac_fastapi.types.requests import get_base_url
-from stac_fastapi.types.stac import Collection, Collections, Item, ItemCollection
 
 NumType = Union[float, int]
 
 
 @attr.s
 class CoreCrudClient(AsyncBaseCoreClient):
     """Client for core endpoints defined by stac."""
 
-    async def all_collections(self, **kwargs) -> Collections:
+    async def all_collections(self, request: Request, **kwargs) -> Collections:
         """Read all collections from the database."""
-        request: Request = kwargs["request"]
         base_url = get_base_url(request)
-        pool = request.app.state.readpool
 
-        async with pool.acquire() as conn:
+        async with request.app.state.get_connection(request, "r") as conn:
             collections = await conn.fetchval(
                 """
                 SELECT * FROM all_collections();
                 """
             )
         linked_collections: List[Collection] = []
         if collections is not None and len(collections) > 0:
@@ -76,30 +73,30 @@
                 "type": MimeTypes.json,
                 "href": urljoin(base_url, "collections"),
             },
         ]
         collection_list = Collections(collections=linked_collections or [], links=links)
         return collection_list
 
-    async def get_collection(self, collection_id: str, **kwargs) -> Collection:
+    async def get_collection(
+        self, collection_id: str, request: Request, **kwargs
+    ) -> Collection:
         """Get collection by id.
 
         Called with `GET /collections/{collection_id}`.
 
         Args:
             collection_id: ID of the collection.
 
         Returns:
             Collection.
         """
         collection: Optional[Dict[str, Any]]
 
-        request: Request = kwargs["request"]
-        pool = request.app.state.readpool
-        async with pool.acquire() as conn:
+        async with request.app.state.get_connection(request, "r") as conn:
             q, p = render(
                 """
                 SELECT * FROM get_collection(:id::text);
                 """,
                 id=collection_id,
             )
             collection = await conn.fetchval(q, *p)
@@ -121,16 +118,15 @@
             collection: ID of the collection.
 
         Returns:
             Item.
         """
         item: Optional[Dict[str, Any]]
 
-        pool = request.app.state.readpool
-        async with pool.acquire() as conn:
+        async with request.app.state.get_connection(request, "r") as conn:
             q, p = render(
                 """
                 SELECT * FROM collection_base_item(:collection_id::text);
                 """,
                 collection_id=collection_id,
             )
             item = await conn.fetchval(q, *p)
@@ -139,43 +135,41 @@
             raise NotFoundError(f"A base item for {collection_id} does not exist.")
 
         return item
 
     async def _search_base(
         self,
         search_request: PgstacSearch,
-        **kwargs: Any,
+        request: Request,
     ) -> ItemCollection:
         """Cross catalog search (POST).
 
         Called with `POST /search`.
 
         Args:
             search_request: search request parameters.
 
         Returns:
             ItemCollection containing items which match the search criteria.
         """
         items: Dict[str, Any]
 
-        request: Request = kwargs["request"]
         settings: Settings = request.app.state.settings
-        pool = request.app.state.readpool
 
         search_request.conf = search_request.conf or {}
         search_request.conf["nohydrate"] = settings.use_api_hydrate
-        req = search_request.json(exclude_none=True, by_alias=True)
+        search_request_json = search_request.json(exclude_none=True, by_alias=True)
 
         try:
-            async with pool.acquire() as conn:
+            async with request.app.state.get_connection(request, "r") as conn:
                 q, p = render(
                     """
                     SELECT * FROM search(:req::text::jsonb);
                     """,
-                    req=req,
+                    req=search_request_json,
                 )
                 items = await conn.fetchval(q, *p)
         except InvalidDatetimeFormatError:
             raise InvalidQueryParameter(
                 f"Datetime parameter {search_request.datetime} is invalid."
             )
 
@@ -249,14 +243,15 @@
             prev=prev,
         ).get_links()
         return collection
 
     async def item_collection(
         self,
         collection_id: str,
+        request: Request,
         bbox: Optional[List[NumType]] = None,
         datetime: Optional[Union[str, datetime]] = None,
         limit: Optional[int] = None,
         token: str = None,
         **kwargs,
     ) -> ItemCollection:
         """Get all items from a specific collection.
@@ -268,83 +263,86 @@
             limit: number of items to return.
             token: pagination token.
 
         Returns:
             An ItemCollection.
         """
         # If collection does not exist, NotFoundError wil be raised
-        await self.get_collection(collection_id, **kwargs)
+        await self.get_collection(collection_id, request)
 
         base_args = {
             "collections": [collection_id],
             "bbox": bbox,
             "datetime": datetime,
             "limit": limit,
             "token": token,
         }
 
         clean = {}
         for k, v in base_args.items():
             if v is not None and v != []:
                 clean[k] = v
 
-        req = self.post_request_model(
+        search_request = self.post_request_model(
             **clean,
         )
-        item_collection = await self._search_base(req, **kwargs)
+        item_collection = await self._search_base(search_request, request)
         links = await ItemCollectionLinks(
-            collection_id=collection_id, request=kwargs["request"]
+            collection_id=collection_id, request=request
         ).get_links(extra_links=item_collection["links"])
         item_collection["links"] = links
         return item_collection
 
-    async def get_item(self, item_id: str, collection_id: str, **kwargs) -> Item:
+    async def get_item(
+        self, item_id: str, collection_id: str, request: Request, **kwargs
+    ) -> Item:
         """Get item by id.
 
         Called with `GET /collections/{collection_id}/items/{item_id}`.
 
         Args:
             item_id: ID of the item.
             collection_id: ID of the collection the item is in.
 
         Returns:
             Item.
         """
         # If collection does not exist, NotFoundError wil be raised
-        await self.get_collection(collection_id, **kwargs)
+        await self.get_collection(collection_id, request)
 
-        req = self.post_request_model(
+        search_request = self.post_request_model(
             ids=[item_id], collections=[collection_id], limit=1
         )
-        item_collection = await self._search_base(req, **kwargs)
+        item_collection = await self._search_base(search_request, request)
         if not item_collection["features"]:
             raise NotFoundError(
                 f"Item {item_id} in Collection {collection_id} does not exist."
             )
 
         return Item(**item_collection["features"][0])
 
     async def post_search(
-        self, search_request: PgstacSearch, **kwargs
+        self, search_request: PgstacSearch, request: Request, **kwargs
     ) -> ItemCollection:
         """Cross catalog search (POST).
 
         Called with `POST /search`.
 
         Args:
             search_request: search request parameters.
 
         Returns:
             ItemCollection containing items which match the search criteria.
         """
-        item_collection = await self._search_base(search_request, **kwargs)
+        item_collection = await self._search_base(search_request, request)
         return ItemCollection(**item_collection)
 
     async def get_search(
         self,
+        request: Request,
         collections: Optional[List[str]] = None,
         ids: Optional[List[str]] = None,
         bbox: Optional[List[NumType]] = None,
         datetime: Optional[Union[str, datetime]] = None,
         limit: Optional[int] = None,
         query: Optional[str] = None,
         token: Optional[str] = None,
@@ -358,15 +356,14 @@
         """Cross catalog search (GET).
 
         Called with `GET /search`.
 
         Returns:
             ItemCollection containing items which match the search criteria.
         """
-        request = kwargs["request"]
         query_params = str(request.query_params)
 
         # Kludgy fix because using factory does not allow alias for filter-lang
         if filter_lang is None:
             match = re.search(r"filter-lang=([a-z0-9-]+)", query_params, re.IGNORECASE)
             if match:
                 filter_lang = match.group(1)
@@ -428,8 +425,8 @@
         # Do the request
         try:
             search_request = self.post_request_model(**clean)
         except ValidationError as e:
             raise HTTPException(
                 status_code=400, detail=f"Invalid parameters provided {e}"
             )
-        return await self.post_search(search_request, request=kwargs["request"])
+        return await self.post_search(search_request, request=request)
```

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/db.py` & `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/db.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Database connection handling."""
 
 import json
-from contextlib import contextmanager
-from typing import Dict, Generator, Union
+from contextlib import asynccontextmanager, contextmanager
+from typing import AsyncIterator, Callable, Dict, Generator, Literal, Union
 
 import attr
 import orjson
-from asyncpg import exceptions, pool
+from asyncpg import Connection, exceptions
 from buildpg import V, asyncpg, render
-from fastapi import FastAPI
-
+from fastapi import FastAPI, Request
 from stac_fastapi.types.errors import (
     ConflictError,
     DatabaseError,
     ForeignKeyError,
     NotFoundError,
 )
 
@@ -30,63 +29,79 @@
         "jsonb",
         encoder=orjson.dumps,
         decoder=orjson.loads,
         schema="pg_catalog",
     )
 
 
-async def connect_to_db(app: FastAPI) -> None:
-    """Connect to Database."""
+ConnectionGetter = Callable[[Request, Literal["r", "w"]], AsyncIterator[Connection]]
+
+
+async def connect_to_db(app: FastAPI, get_conn: ConnectionGetter = None) -> None:
+    """Create connection pools & connection retriever on application."""
     settings = app.state.settings
     if app.state.settings.testing:
         readpool = writepool = settings.testing_connection_string
     else:
         readpool = settings.reader_connection_string
         writepool = settings.writer_connection_string
     db = DB()
     app.state.readpool = await db.create_pool(readpool, settings)
     app.state.writepool = await db.create_pool(writepool, settings)
+    app.state.get_connection = get_conn if get_conn else get_connection
 
 
 async def close_db_connection(app: FastAPI) -> None:
     """Close connection."""
     await app.state.readpool.close()
     await app.state.writepool.close()
 
 
-async def dbfunc(pool: pool, func: str, arg: Union[str, Dict]):
+@asynccontextmanager
+async def get_connection(
+    request: Request,
+    readwrite: Literal["r", "w"] = "r",
+) -> AsyncIterator[Connection]:
+    """Retrieve connection from database conection pool."""
+    pool = (
+        request.app.state.writepool if readwrite == "w" else request.app.state.readpool
+    )
+    with translate_pgstac_errors():
+        async with pool.acquire() as conn:
+            yield conn
+
+
+async def dbfunc(conn: Connection, func: str, arg: Union[str, Dict]):
     """Wrap PLPGSQL Functions.
 
     Keyword arguments:
     pool -- the asyncpg pool to use to connect to the database
     func -- the name of the PostgreSQL function to call
     arg -- the argument to the PostgreSQL function as either a string
     or a dict that will be converted into jsonb
     """
     with translate_pgstac_errors():
         if isinstance(arg, str):
-            async with pool.acquire() as conn:
-                q, p = render(
-                    """
-                    SELECT * FROM :func(:item::text);
-                    """,
-                    func=V(func),
-                    item=arg,
-                )
-                return await conn.fetchval(q, *p)
+            q, p = render(
+                """
+                SELECT * FROM :func(:item::text);
+                """,
+                func=V(func),
+                item=arg,
+            )
+            return await conn.fetchval(q, *p)
         else:
-            async with pool.acquire() as conn:
-                q, p = render(
-                    """
-                    SELECT * FROM :func(:item::text::jsonb);
-                    """,
-                    func=V(func),
-                    item=json.dumps(arg),
-                )
-                return await conn.fetchval(q, *p)
+            q, p = render(
+                """
+                SELECT * FROM :func(:item::text::jsonb);
+                """,
+                func=V(func),
+                item=json.dumps(arg),
+            )
+            return await conn.fetchval(q, *p)
 
 
 @contextmanager
 def translate_pgstac_errors() -> Generator[None, None, None]:
     """Context manager that translates pgstac errors into FastAPI errors."""
     try:
         yield
```

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/extensions/filter.py` & `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/extensions/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Get Queryables."""
 from typing import Any, Optional
 
 from buildpg import render
 from fastapi import Request
 from fastapi.responses import JSONResponse
-
 from stac_fastapi.types.core import AsyncBaseFiltersClient
 from stac_fastapi.types.errors import NotFoundError
 
 
 class FiltersClient(AsyncBaseFiltersClient):
     """Defines a pattern for implementing the STAC filter extension."""
```

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/extensions/query.py` & `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/extensions/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 import operator
 from enum import auto
 from types import DynamicClassAttribute
 from typing import Any, Callable, Dict, Optional
 
 from pydantic import BaseModel
-from stac_pydantic.utils import AutoValueEnum
-
 from stac_fastapi.extensions.core.query import QueryExtension as QueryExtensionBase
+from stac_pydantic.utils import AutoValueEnum
 
 
 class Operator(str, AutoValueEnum):
     """Defines the set of operators supported by the API."""
 
     eq = auto()
     ne = auto()
```

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/models/links.py` & `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/models/links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """link helpers."""
 
 from typing import Any, Dict, List, Optional
 from urllib.parse import ParseResult, parse_qs, unquote, urlencode, urljoin, urlparse
 
 import attr
+from stac_fastapi.types.requests import get_base_url
 from stac_pydantic.links import Relations
 from stac_pydantic.shared import MimeTypes
 from starlette.requests import Request
 
-from stac_fastapi.types.requests import get_base_url
-
 # These can be inferred from the item/collection so they aren't included in the database
 # Instead they are dynamically generated when querying the database using the classes defined below
 INFERRED_LINK_RELS = ["self", "item", "parent", "collection", "root"]
 
 
 def filter_links(links: List[Dict]) -> List[Dict]:
     """Remove inferred links."""
```

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/transactions.py` & `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/transactions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 """transactions extension client."""
 
 import logging
 from typing import Optional, Union
 
 import attr
 from buildpg import render
-from fastapi import HTTPException
-from starlette.responses import JSONResponse, Response
-
+from fastapi import HTTPException, Request
 from stac_fastapi.extensions.third_party.bulk_transactions import (
     AsyncBaseBulkTransactionsClient,
     Items,
 )
-from stac_fastapi.pgstac.db import dbfunc, translate_pgstac_errors
-from stac_fastapi.pgstac.models.links import CollectionLinks, ItemLinks
 from stac_fastapi.types import stac as stac_types
 from stac_fastapi.types.core import AsyncBaseTransactionsClient
+from starlette.responses import JSONResponse, Response
+
+from stac_fastapi.pgstac.db import dbfunc
+from stac_fastapi.pgstac.models.links import CollectionLinks, ItemLinks
 
 logger = logging.getLogger("uvicorn")
 logger.setLevel(logging.INFO)
 
 
 @attr.s
 class TransactionsClient(AsyncBaseTransactionsClient):
     """Transactions extension specific CRUD operations."""
 
     async def create_item(
-        self, collection_id: str, item: stac_types.Item, **kwargs
+        self, collection_id: str, item: stac_types.Item, request: Request, **kwargs
     ) -> Optional[Union[stac_types.Item, Response]]:
         """Create item."""
         body_collection_id = item.get("collection")
         if body_collection_id is not None and collection_id != body_collection_id:
             raise HTTPException(
                 status_code=400,
                 detail=f"Collection ID from path parameter ({collection_id}) does not match Collection ID from Item ({body_collection_id})",
             )
         item["collection"] = collection_id
-        request = kwargs["request"]
-        pool = request.app.state.writepool
-        await dbfunc(pool, "create_item", item)
+        async with request.app.state.get_connection(request, "w") as conn:
+            await dbfunc(conn, "create_item", item)
         item["links"] = await ItemLinks(
             collection_id=collection_id,
             item_id=item["id"],
             request=request,
         ).get_links(extra_links=item.get("links"))
         return stac_types.Item(**item)
 
     async def update_item(
-        self, collection_id: str, item_id: str, item: stac_types.Item, **kwargs
+        self,
+        request: Request,
+        collection_id: str,
+        item_id: str,
+        item: stac_types.Item,
+        **kwargs,
     ) -> Optional[Union[stac_types.Item, Response]]:
         """Update item."""
         body_collection_id = item.get("collection")
         if body_collection_id is not None and collection_id != body_collection_id:
             raise HTTPException(
                 status_code=400,
                 detail=f"Collection ID from path parameter ({collection_id}) does not match Collection ID from Item ({body_collection_id})",
@@ -59,81 +63,73 @@
         item["collection"] = collection_id
         body_item_id = item["id"]
         if body_item_id != item_id:
             raise HTTPException(
                 status_code=400,
                 detail=f"Item ID from path parameter ({item_id}) does not match Item ID from Item ({body_item_id})",
             )
-        request = kwargs["request"]
-        pool = request.app.state.writepool
-        await dbfunc(pool, "update_item", item)
+        async with request.app.state.get_connection(request, "w") as conn:
+            await dbfunc(conn, "update_item", item)
         item["links"] = await ItemLinks(
             collection_id=collection_id,
             item_id=item["id"],
             request=request,
         ).get_links(extra_links=item.get("links"))
         return stac_types.Item(**item)
 
     async def create_collection(
-        self, collection: stac_types.Collection, **kwargs
+        self, collection: stac_types.Collection, request: Request, **kwargs
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Create collection."""
-        request = kwargs["request"]
-        pool = request.app.state.writepool
-        await dbfunc(pool, "create_collection", collection)
+        async with request.app.state.get_connection(request, "w") as conn:
+            await dbfunc(conn, "create_collection", collection)
         collection["links"] = await CollectionLinks(
             collection_id=collection["id"], request=request
         ).get_links(extra_links=collection.get("links"))
 
         return stac_types.Collection(**collection)
 
     async def update_collection(
-        self, collection: stac_types.Collection, **kwargs
+        self, collection: stac_types.Collection, request: Request, **kwargs
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Update collection."""
-        request = kwargs["request"]
-        pool = request.app.state.writepool
-        await dbfunc(pool, "update_collection", collection)
+        async with request.app.state.get_connection(request, "w") as conn:
+            await dbfunc(conn, "update_collection", collection)
         collection["links"] = await CollectionLinks(
             collection_id=collection["id"], request=request
         ).get_links(extra_links=collection.get("links"))
         return stac_types.Collection(**collection)
 
     async def delete_item(
-        self, item_id: str, collection_id: str, **kwargs
+        self, item_id: str, collection_id: str, request: Request, **kwargs
     ) -> Optional[Union[stac_types.Item, Response]]:
         """Delete item."""
-        request = kwargs["request"]
-        pool = request.app.state.writepool
-        async with pool.acquire() as conn:
-            q, p = render(
-                "SELECT * FROM delete_item(:item::text, :collection::text);",
-                item=item_id,
-                collection=collection_id,
-            )
-            with translate_pgstac_errors():
-                await conn.fetchval(q, *p)
+        q, p = render(
+            "SELECT * FROM delete_item(:item::text, :collection::text);",
+            item=item_id,
+            collection=collection_id,
+        )
+        async with request.app.state.get_connection(request, "w") as conn:
+            await conn.fetchval(q, *p)
         return JSONResponse({"deleted item": item_id})
 
     async def delete_collection(
-        self, collection_id: str, **kwargs
+        self, collection_id: str, request: Request, **kwargs
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Delete collection."""
-        request = kwargs["request"]
-        pool = request.app.state.writepool
-        await dbfunc(pool, "delete_collection", collection_id)
+        async with request.app.state.get_connection(request, "w") as conn:
+            await dbfunc(conn, "delete_collection", collection_id)
         return JSONResponse({"deleted collection": collection_id})
 
 
 @attr.s
 class BulkTransactionsClient(AsyncBaseBulkTransactionsClient):
     """Postgres bulk transactions."""
 
-    async def bulk_item_insert(self, items: Items, **kwargs) -> str:
+    async def bulk_item_insert(self, items: Items, request: Request, **kwargs) -> str:
         """Bulk item insertion using pgstac."""
-        request = kwargs["request"]
-        pool = request.app.state.writepool
         items = list(items.items.values())
-        await dbfunc(pool, "create_items", items)
+        async with request.app.state.get_connection(request, "w") as conn:
+            await dbfunc(conn, "create_items", items)
 
         return_msg = f"Successfully added {len(items)} items."
         return return_msg
```

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/types/base_item_cache.py` & `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/types/base_item_cache.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/types/search.py` & `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/types/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """stac_fastapi.types.search module."""
 
 from typing import Dict, Optional
 
 from pydantic import validator
-
 from stac_fastapi.types.search import BaseSearchPostRequest
 
 
 class PgstacSearch(BaseSearchPostRequest):
     """Search model.
 
     Overrides the validation for datetime from the base request model.
```

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi/pgstac/utils.py` & `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/utils.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi.pgstac.egg-info/PKG-INFO` & `stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7374 6163  : 2.1.Name: stac
 00000020: 2d66 6173 7461 7069 2e70 6773 7461 630a  -fastapi.pgstac.
-00000030: 5665 7273 696f 6e3a 2032 2e34 2e35 0a53  Version: 2.4.5.S
+00000030: 5665 7273 696f 6e3a 2032 2e34 2e36 0a53  Version: 2.4.6.S
 00000040: 756d 6d61 7279 3a20 416e 2069 6d70 6c65  ummary: An imple
 00000050: 6d65 6e74 6174 696f 6e20 6f66 2053 5441  mentation of STA
 00000060: 4320 4150 4920 6261 7365 6420 6f6e 2074  C API based on t
 00000070: 6865 2046 6173 7441 5049 2066 7261 6d65  he FastAPI frame
 00000080: 776f 726b 2061 6e64 2075 7369 6e67 2074  work and using t
 00000090: 6865 2070 6773 7461 6320 6261 636b 656e  he pgstac backen
 000000a0: 642e 0a48 6f6d 652d 7061 6765 3a20 6874  d..Home-page: ht
@@ -39,260 +39,301 @@
 00000260: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
 00000270: 6172 6b64 6f77 6e0a 5072 6f76 6964 6573  arkdown.Provides
 00000280: 2d45 7874 7261 3a20 6465 760a 5072 6f76  -Extra: dev.Prov
 00000290: 6964 6573 2d45 7874 7261 3a20 646f 6373  ides-Extra: docs
 000002a0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
 000002b0: 2073 6572 7665 720a 5072 6f76 6964 6573   server.Provides
 000002c0: 2d45 7874 7261 3a20 6177 736c 616d 6264  -Extra: awslambd
-000002d0: 610a 0a3c 7020 616c 6967 6e3d 2263 656e  a..<p align="cen
-000002e0: 7465 7222 3e0a 2020 3c69 6d67 2073 7263  ter">.  <img src
-000002f0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000300: 2e63 6f6d 2f72 6164 6961 6e74 6561 7274  .com/radianteart
-00000310: 682f 7374 6163 2d73 6974 652f 7261 772f  h/stac-site/raw/
-00000320: 6d61 7374 6572 2f69 6d61 6765 732f 6c6f  master/images/lo
-00000330: 676f 2f73 7461 632d 3033 302d 6c6f 6e67  go/stac-030-long
-00000340: 2e70 6e67 2220 7769 6474 683d 3430 303e  .png" width=400>
-00000350: 0a20 203c 7020 616c 6967 6e3d 2263 656e  .  <p align="cen
-00000360: 7465 7222 3e46 6173 7441 5049 2069 6d70  ter">FastAPI imp
-00000370: 6c65 6d65 6e74 696f 6e20 6f66 2074 6865  lemention of the
-00000380: 2053 5441 4320 4150 4920 7370 6563 2075   STAC API spec u
-00000390: 7369 6e67 203c 6120 6872 6566 3d22 6874  sing <a href="ht
-000003a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000003b0: 2f73 7461 632d 7574 696c 732f 7067 7374  /stac-utils/pgst
-000003c0: 6163 223e 5047 5374 6163 3c2f 613e 3c2f  ac">PGStac</a></
-000003d0: 703e 0a3c 2f70 3e0a 3c70 2061 6c69 676e  p>.</p>.<p align
-000003e0: 3d22 6365 6e74 6572 223e 0a20 203c 6120  ="center">.  <a 
-000003f0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000400: 7468 7562 2e63 6f6d 2f73 7461 632d 7574  thub.com/stac-ut
-00000410: 696c 732f 7374 6163 2d66 6173 7461 7069  ils/stac-fastapi
-00000420: 2f61 6374 696f 6e73 3f71 7565 7279 3d77  /actions?query=w
-00000430: 6f72 6b66 6c6f 7725 3341 6369 6364 2220  orkflow%3Acicd" 
-00000440: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00000450: 0a20 2020 2020 203c 696d 6720 7372 633d  .      <img src=
-00000460: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000470: 636f 6d2f 7374 6163 2d75 7469 6c73 2f73  com/stac-utils/s
-00000480: 7461 632d 6661 7374 6170 692f 776f 726b  tac-fastapi/work
-00000490: 666c 6f77 732f 7374 6163 2d66 6173 7461  flows/stac-fasta
-000004a0: 7069 2f62 6164 6765 2e73 7667 2220 616c  pi/badge.svg" al
-000004b0: 743d 2254 6573 7422 3e0a 2020 3c2f 613e  t="Test">.  </a>
-000004c0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-000004d0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000004e0: 6a65 6374 2f73 7461 632d 6661 7374 6170  ject/stac-fastap
-000004f0: 6922 2074 6172 6765 743d 225f 626c 616e  i" target="_blan
-00000500: 6b22 3e0a 2020 2020 2020 3c69 6d67 2073  k">.      <img s
-00000510: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000520: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000530: 762f 7374 6163 2d66 6173 7461 7069 3f63  v/stac-fastapi?c
-00000540: 6f6c 6f72 3d25 3233 3334 4430 3538 266c  olor=%2334D058&l
-00000550: 6162 656c 3d70 7970 6925 3230 7061 636b  abel=pypi%20pack
-00000560: 6167 6522 2061 6c74 3d22 5061 636b 6167  age" alt="Packag
-00000570: 6520 7665 7273 696f 6e22 3e0a 2020 3c2f  e version">.  </
-00000580: 613e 0a20 203c 6120 6872 6566 3d22 6874  a>.  <a href="ht
-00000590: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000005a0: 2f73 7461 632d 7574 696c 732f 7374 6163  /stac-utils/stac
-000005b0: 2d66 6173 7461 7069 2f62 6c6f 622f 6d61  -fastapi/blob/ma
-000005c0: 696e 2f4c 4943 454e 5345 2220 7461 7267  in/LICENSE" targ
-000005d0: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
-000005e0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-000005f0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000600: 2e69 6f2f 6769 7468 7562 2f6c 6963 656e  .io/github/licen
-00000610: 7365 2f73 7461 632d 7574 696c 732f 7374  se/stac-utils/st
-00000620: 6163 2d66 6173 7461 7069 2e73 7667 2220  ac-fastapi.svg" 
-00000630: 616c 743d 2244 6f77 6e6c 6f61 6473 223e  alt="Downloads">
-00000640: 0a20 203c 2f61 3e0a 3c2f 703e 0a0a 2d2d  .  </a>.</p>..--
-00000650: 2d0a 0a2a 2a44 6f63 756d 656e 7461 7469  -..**Documentati
-00000660: 6f6e 2a2a 3a20 5b68 7474 7073 3a2f 2f73  on**: [https://s
-00000670: 7461 632d 7574 696c 732e 6769 7468 7562  tac-utils.github
-00000680: 2e69 6f2f 7374 6163 2d66 6173 7461 7069  .io/stac-fastapi
-00000690: 2f5d 2868 7474 7073 3a2f 2f73 7461 632d  /](https://stac-
-000006a0: 7574 696c 732e 6769 7468 7562 2e69 6f2f  utils.github.io/
-000006b0: 7374 6163 2d66 6173 7461 7069 2f29 0a0a  stac-fastapi/)..
-000006c0: 2a2a 536f 7572 6365 2043 6f64 652a 2a3a  **Source Code**:
-000006d0: 205b 6874 7470 733a 2f2f 6769 7468 7562   [https://github
-000006e0: 2e63 6f6d 2f73 7461 632d 7574 696c 732f  .com/stac-utils/
-000006f0: 7374 6163 2d66 6173 7461 7069 5d28 6874  stac-fastapi](ht
-00000700: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000710: 2f73 7461 632d 7574 696c 732f 7374 6163  /stac-utils/stac
-00000720: 2d66 6173 7461 7069 290a 0a2d 2d2d 0a0a  -fastapi)..---..
-00000730: 5374 6163 2046 6173 7441 5049 2075 7369  Stac FastAPI usi
-00000740: 6e67 2074 6865 205b 5047 5374 6163 5d28  ng the [PGStac](
-00000750: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000760: 6f6d 2f73 7461 632d 7574 696c 732f 7067  om/stac-utils/pg
-00000770: 7374 6163 2920 6261 636b 656e 642e 0a0a  stac) backend...
-00000780: 5b50 4753 7461 635d 2868 7474 7073 3a2f  [PGStac](https:/
-00000790: 2f67 6974 6875 622e 636f 6d2f 7374 6163  /github.com/stac
-000007a0: 2d75 7469 6c73 2f70 6773 7461 6329 2069  -utils/pgstac) i
-000007b0: 7320 6120 7365 7061 7261 7465 6c79 206d  s a separately m
-000007c0: 616e 6167 6564 2050 6f73 7467 7265 5351  anaged PostgreSQ
-000007d0: 4c20 6461 7461 6261 7365 2074 6861 7420  L database that 
-000007e0: 6973 2064 6573 6967 6e65 6420 666f 7220  is designed for 
-000007f0: 656e 6861 6e63 6564 2070 6572 666f 726d  enhanced perform
-00000800: 616e 6365 2074 6f20 6265 2061 626c 6520  ance to be able 
-00000810: 746f 2073 6361 6c65 2053 7461 6320 4661  to scale Stac Fa
-00000820: 7374 4150 4920 746f 2062 6520 6162 6c65  stAPI to be able
-00000830: 2074 6f20 6566 6669 6369 656e 746c 7920   to efficiently 
-00000840: 6861 6e64 6c65 2068 756e 6472 6564 7320  handle hundreds 
-00000850: 6f66 206d 696c 6c69 6f6e 7320 6f66 2072  of millions of r
-00000860: 6563 6f72 6473 2e20 5b50 4753 7461 635d  ecords. [PGStac]
-00000870: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000880: 636f 6d2f 7374 6163 2d75 7469 6c73 2f70  com/stac-utils/p
-00000890: 6773 7461 6329 2061 7574 6f6d 6174 6963  gstac) automatic
-000008a0: 616c 6c79 2069 6e63 6c75 6465 7320 696e  ally includes in
-000008b0: 6465 7865 7320 6f6e 2049 7465 6d20 6964  dexes on Item id
-000008c0: 2c20 436f 6c6c 6563 7469 6f6e 2069 642c  , Collection id,
-000008d0: 2049 7465 6d20 4765 6f6d 6574 7279 2c20   Item Geometry, 
-000008e0: 4974 656d 2044 6174 6574 696d 652c 2061  Item Datetime, a
-000008f0: 6e64 2061 6e20 496e 6465 7820 666f 7220  nd an Index for 
-00000900: 6571 7561 6c69 7479 2063 6865 636b 7320  equality checks 
-00000910: 6f6e 2061 6e79 206b 6579 2069 6e20 4974  on any key in It
-00000920: 656d 2050 726f 7065 7274 6965 732e 2041  em Properties. A
-00000930: 6464 6974 696f 6e61 6c20 696e 6465 7865  dditional indexe
-00000940: 7320 6d61 7920 6265 2061 6464 6564 2074  s may be added t
-00000950: 6f20 4974 656d 2050 726f 7065 7274 6965  o Item Propertie
-00000960: 7320 746f 2073 7065 6564 2075 7020 7468  s to speed up th
-00000970: 6520 7573 6520 6f66 206f 7264 6572 2c20  e use of order, 
-00000980: 3c2c 203c 3d2c 203e 2c20 616e 6420 3e3d  <, <=, >, and >=
-00000990: 2071 7565 7269 6573 2e0a 0a53 7461 6320   queries...Stac 
-000009a0: 4661 7374 4150 4920 6163 7473 2061 7320  FastAPI acts as 
-000009b0: 7468 6520 4854 5450 2069 6e74 6572 6661  the HTTP interfa
-000009c0: 6365 2076 616c 6964 6174 696e 6720 616e  ce validating an
-000009d0: 7920 7265 7175 6573 7473 2061 6e64 2064  y requests and d
-000009e0: 6174 6120 7468 6174 2069 7320 7365 6e74  ata that is sent
-000009f0: 2074 6f20 7468 6520 5b50 4753 7461 635d   to the [PGStac]
-00000a00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000a10: 636f 6d2f 7374 6163 2d75 7469 6c73 2f70  com/stac-utils/p
-00000a20: 6773 7461 6329 2062 6163 6b65 6e64 2061  gstac) backend a
-00000a30: 6e64 2061 6464 7320 696e 204c 696e 6b20  nd adds in Link 
-00000a40: 6974 656d 7320 6f6e 2064 6174 6120 7265  items on data re
-00000a50: 7475 726e 2072 656c 6174 6976 6520 746f  turn relative to
-00000a60: 2074 6865 2073 6572 7669 6365 2068 6f73   the service hos
-00000a70: 742e 2041 6c6c 206f 7468 6572 2070 726f  t. All other pro
-00000a80: 6365 7373 696e 6720 616e 6420 7365 6172  cessing and sear
-00000a90: 6368 2069 7320 7072 6f76 6964 6564 2064  ch is provided d
-00000aa0: 6972 6563 746c 7920 7573 696e 6720 5047  irectly using PG
-00000ab0: 5374 6163 2070 726f 6365 6475 7261 6c20  Stac procedural 
-00000ac0: 7371 6c20 2f20 706c 7067 7371 6c20 6675  sql / plpgsql fu
-00000ad0: 6e63 7469 6f6e 7320 6f6e 2074 6865 2064  nctions on the d
-00000ae0: 6174 6162 6173 652e 0a0a 5047 5374 6163  atabase...PGStac
-00000af0: 2073 746f 7265 7320 616c 6c20 636f 6c6c   stores all coll
-00000b00: 6563 7469 6f6e 2061 6e64 2069 7465 6d20  ection and item 
-00000b10: 7265 636f 7264 7320 6173 206a 736f 6e62  records as jsonb
-00000b20: 2066 6965 6c64 7320 6578 6163 746c 7920   fields exactly 
-00000b30: 6173 2074 6865 7920 636f 6d65 2069 6e20  as they come in 
-00000b40: 616c 6c6f 7769 6e67 2066 6f72 2061 6e79  allowing for any
-00000b50: 2063 7573 746f 6d20 6669 656c 6473 2074   custom fields t
-00000b60: 6f20 6265 2073 746f 7265 6420 616e 6420  o be stored and 
-00000b70: 7265 7472 6965 7665 6420 7472 616e 7370  retrieved transp
-00000b80: 6172 656e 746c 792e 0a0a 5768 696c 6520  arently...While 
-00000b90: 7468 6520 5374 6163 2053 6f72 7420 4578  the Stac Sort Ex
-00000ba0: 7465 6e73 696f 6e20 6973 2066 756c 6c79  tension is fully
-00000bb0: 2073 7570 706f 7274 6564 2c20 5b50 4753   supported, [PGS
-00000bc0: 7461 635d 2868 7474 7073 3a2f 2f67 6974  tac](https://git
-00000bd0: 6875 622e 636f 6d2f 7374 6163 2d75 7469  hub.com/stac-uti
-00000be0: 6c73 2f70 6773 7461 6329 2069 7320 7061  ls/pgstac) is pa
-00000bf0: 7274 6963 756c 6172 6c79 2065 6e68 616e  rticularly enhan
-00000c00: 6365 6420 746f 2062 6520 6162 6c65 2074  ced to be able t
-00000c10: 6f20 736f 7274 2062 7920 6461 7465 7469  o sort by dateti
-00000c20: 6d65 2028 6569 7468 6572 2061 7363 656e  me (either ascen
-00000c30: 6469 6e67 206f 7220 6465 7363 656e 6469  ding or descendi
-00000c40: 6e67 292e 2053 6f72 7469 6e67 2062 7920  ng). Sorting by 
-00000c50: 616e 7974 6869 6e67 206f 7468 6572 2074  anything other t
-00000c60: 6861 6e20 6461 7465 7469 6d65 2028 7468  han datetime (th
-00000c70: 6520 6465 6661 756c 7420 6966 206e 6f20  e default if no 
-00000c80: 736f 7274 2069 7320 7370 6563 6966 6965  sort is specifie
-00000c90: 6429 206f 6e20 7665 7279 206c 6172 6765  d) on very large
-00000ca0: 2053 7461 6320 7265 706f 7369 746f 7269   Stac repositori
-00000cb0: 6573 2077 6974 686f 7574 2076 6572 7920  es without very 
-00000cc0: 7370 6563 6966 6963 2071 7565 7279 206c  specific query l
-00000cd0: 696d 6974 7320 2869 6520 7365 6c65 6374  imits (ie select
-00000ce0: 696e 6720 6120 7369 6e67 6c65 2064 6179  ing a single day
-00000cf0: 2064 6174 6520 7261 6e67 6529 2077 696c   date range) wil
-00000d00: 6c20 6e6f 7420 6861 7665 2074 6865 2073  l not have the s
-00000d10: 616d 6520 7065 7266 6f72 6d61 6e63 652e  ame performance.
-00000d20: 2046 6f72 206d 6f72 6520 7468 616e 206d   For more than m
-00000d30: 696c 6c69 6f6e 7320 6f66 2072 6563 6f72  illions of recor
-00000d40: 6473 2069 7420 6973 2072 6563 6f6d 6d65  ds it is recomme
-00000d50: 6e64 6564 2074 6f20 6569 7468 6572 2073  nded to either s
-00000d60: 6574 2061 206c 6f77 2063 6f6e 6e65 6374  et a low connect
-00000d70: 696f 6e20 7469 6d65 6f75 7420 6f6e 2050  ion timeout on P
-00000d80: 6f73 7467 7265 5351 4c20 6f72 2074 6f20  ostgreSQL or to 
-00000d90: 6469 7361 626c 6520 7573 6520 6f66 2074  disable use of t
-00000da0: 6865 2053 6f72 7420 4578 7465 6e73 696f  he Sort Extensio
-00000db0: 6e2e 0a0a 6073 7461 632d 6661 7374 6170  n...`stac-fastap
-00000dc0: 6920 7067 7374 6163 6020 7761 7320 696e  i pgstac` was in
-00000dd0: 6974 6961 6c6c 7920 6164 6465 6420 746f  itially added to
-00000de0: 2060 7374 6163 2d66 6173 7461 7069 6020   `stac-fastapi` 
-00000df0: 6279 205b 6465 7665 6c6f 706d 656e 7473  by [developments
-00000e00: 6565 645d 2868 7474 7073 3a2f 2f67 6974  eed](https://git
-00000e10: 6875 622e 636f 6d2f 6465 7665 6c6f 706d  hub.com/developm
-00000e20: 656e 7473 6565 6429 2e0a 0a23 2320 496e  entseed)...## In
-00000e30: 7374 616c 6c61 7469 6f6e 0a0a 6060 6073  stallation..```s
-00000e40: 6865 6c6c 0a67 6974 2063 6c6f 6e65 2068  hell.git clone h
-00000e50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000e60: 6d2f 7374 6163 2d75 7469 6c73 2f73 7461  m/stac-utils/sta
-00000e70: 632d 6661 7374 6170 692e 6769 740a 6364  c-fastapi.git.cd
-00000e80: 2073 7461 632d 6661 7374 6170 690a 7069   stac-fastapi.pi
-00000e90: 7020 696e 7374 616c 6c20 2d65 205c 0a20  p install -e \. 
-00000ea0: 2020 2073 7461 635f 6661 7374 6170 692f     stac_fastapi/
-00000eb0: 6170 695b 6465 765d 205c 0a20 2020 2073  api[dev] \.    s
-00000ec0: 7461 635f 6661 7374 6170 692f 7479 7065  tac_fastapi/type
-00000ed0: 735b 6465 765d 205c 0a20 2020 2073 7461  s[dev] \.    sta
-00000ee0: 635f 6661 7374 6170 692f 6578 7465 6e73  c_fastapi/extens
-00000ef0: 696f 6e73 5b64 6576 5d20 5c0a 2020 2020  ions[dev] \.    
-00000f00: 7374 6163 5f66 6173 7461 7069 2f70 6773  stac_fastapi/pgs
-00000f10: 7461 635b 6465 762c 7365 7276 6572 5d0a  tac[dev,server].
-00000f20: 6060 600a 0a23 2323 2053 6574 7469 6e67  ```..### Setting
-00000f30: 730a 0a54 6f20 636f 6e66 6967 7572 6520  s..To configure 
-00000f40: 5047 5374 6163 2073 7461 632d 6661 7374  PGStac stac-fast
-00000f50: 6170 6920 746f 205b 6879 6472 6174 6520  api to [hydrate 
-00000f60: 7365 6172 6368 2072 6573 756c 7420 6974  search result it
-00000f70: 656d 7320 696e 2074 6865 2041 5049 5d28  ems in the API](
-00000f80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000f90: 6f6d 2f73 7461 632d 7574 696c 732f 7067  om/stac-utils/pg
-00000fa0: 7374 6163 2372 756e 7469 6d65 2d63 6f6e  stac#runtime-con
-00000fb0: 6669 6775 7261 7469 6f6e 7329 2c20 7365  figurations), se
-00000fc0: 7420 7468 6520 6055 5345 5f41 5049 5f48  t the `USE_API_H
-00000fd0: 5944 5241 5445 6020 656e 7669 726f 6e6d  YDRATE` environm
-00000fe0: 656e 7420 7661 7269 6162 6c65 2074 6f20  ent variable to 
-00000ff0: 6074 7275 6560 206f 7220 6578 706c 6963  `true` or explic
-00001000: 6974 6c79 2073 6574 2074 6865 206f 7074  itly set the opt
-00001010: 696f 6e20 696e 2074 6865 2050 4753 7461  ion in the PGSta
-00001020: 6320 5365 7474 696e 6773 206f 626a 6563  c Settings objec
-00001030: 742e 0a0a 2323 2320 4d69 6772 6174 696f  t...### Migratio
-00001040: 6e73 0a0a 5047 5374 6163 2069 7320 616e  ns..PGStac is an
-00001050: 2065 7874 6572 6e61 6c20 7072 6f6a 6563   external projec
-00001060: 7420 616e 6420 7468 6520 6d61 7920 6265  t and the may be
-00001070: 2075 7365 6420 6279 206d 756c 7469 706c   used by multipl
-00001080: 6520 6672 6f6e 7420 656e 6473 2e0a 466f  e front ends..Fo
-00001090: 7220 5374 6163 2046 6173 7441 5049 2064  r Stac FastAPI d
-000010a0: 6576 656c 6f70 6d65 6e74 2c20 6120 646f  evelopment, a do
-000010b0: 636b 6572 2069 6d61 6765 2028 7768 6963  cker image (whic
-000010c0: 6820 6973 2070 756c 6c65 6420 6173 2070  h is pulled as p
-000010d0: 6172 7420 6f66 2074 6865 2064 6f63 6b65  art of the docke
-000010e0: 722d 636f 6d70 6f73 6529 2069 7320 6176  r-compose) is av
-000010f0: 6169 6c61 626c 6520 6174 0a62 6974 6e65  ailable at.bitne
-00001100: 722f 7067 7374 6163 3a5b 7665 7273 696f  r/pgstac:[versio
-00001110: 6e5d 2074 6861 7420 6861 7320 7468 6520  n] that has the 
-00001120: 6675 6c6c 2064 6174 6162 6173 6520 616c  full database al
-00001130: 7265 6164 7920 7365 7420 7570 2066 6f72  ready set up for
-00001140: 2050 4753 7461 632e 0a0a 5468 6572 6520   PGStac...There 
-00001150: 6973 2061 6c73 6f20 6120 7079 7468 6f6e  is also a python
-00001160: 2075 7469 6c69 7479 2061 7320 7061 7274   utility as part
-00001170: 206f 6620 5047 5374 6163 2028 7079 7067   of PGStac (pypg
-00001180: 7374 6163 2920 7468 6174 2069 6e63 6c75  stac) that inclu
-00001190: 6465 7320 6120 6d69 6772 6174 696f 6e20  des a migration 
-000011a0: 7574 696c 6974 792e 2054 6865 2070 6773  utility. The pgs
-000011b0: 7461 630a 7665 7273 696f 6e20 7265 7175  tac.version requ
-000011c0: 6972 6564 2062 7920 7374 6163 2d66 6173  ired by stac-fas
-000011d0: 7461 7069 2f70 6773 7461 6320 6973 2070  tapi/pgstac is p
-000011e0: 696e 6e65 6420 6279 2075 7369 6e67 2074  inned by using t
-000011f0: 6865 2070 696e 6e65 6420 7665 7273 696f  he pinned versio
-00001200: 6e20 6f66 2070 7970 6773 7461 6320 696e  n of pypgstac in
-00001210: 2074 6865 205b 7365 7475 705d 2873 6574   the [setup](set
-00001220: 7570 2e70 7929 2066 696c 652e 0a0a 496e  up.py) file...In
-00001230: 206f 7264 6572 2074 6f20 6d69 6772 6174   order to migrat
-00001240: 6520 6461 7461 6261 7365 2076 6572 7369  e database versi
-00001250: 6f6e 7320 796f 7520 6361 6e20 7573 6520  ons you can use 
-00001260: 7468 6520 6d69 6772 6174 696f 6e20 7574  the migration ut
-00001270: 696c 6974 793a 0a0a 6060 6073 6865 6c6c  ility:..```shell
-00001280: 0a70 7970 6773 7461 6320 6d69 6772 6174  .pypgstac migrat
-00001290: 650a 6060 600a                           e.```.
+000002d0: 610a 4c69 6365 6e73 652d 4669 6c65 3a20  a.License-File: 
+000002e0: 4c49 4345 4e53 450a 0a23 2073 7461 632d  LICENSE..# stac-
+000002f0: 6661 7374 6170 692d 7067 7374 6163 0a0a  fastapi-pgstac..
+00000300: 5b21 5b47 6974 4875 6220 576f 726b 666c  [![GitHub Workfl
+00000310: 6f77 2053 7461 7475 735d 2868 7474 7073  ow Status](https
+00000320: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000330: 6f2f 6769 7468 7562 2f61 6374 696f 6e73  o/github/actions
+00000340: 2f77 6f72 6b66 6c6f 772f 7374 6174 7573  /workflow/status
+00000350: 2f73 7461 632d 7574 696c 732f 7374 6163  /stac-utils/stac
+00000360: 2d66 6173 7461 7069 2d70 6773 7461 632f  -fastapi-pgstac/
+00000370: 6369 6364 2e79 616d 6c3f 7374 796c 653d  cicd.yaml?style=
+00000380: 666f 722d 7468 652d 6261 6467 6529 5d28  for-the-badge)](
+00000390: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000003a0: 6f6d 2f73 7461 632d 7574 696c 732f 7374  om/stac-utils/st
+000003b0: 6163 2d66 6173 7461 7069 2d70 6773 7461  ac-fastapi-pgsta
+000003c0: 632f 6163 7469 6f6e 732f 776f 726b 666c  c/actions/workfl
+000003d0: 6f77 732f 6369 6364 2e79 616d 6c29 0a5b  ows/cicd.yaml).[
+000003e0: 215b 5079 5049 5d28 6874 7470 733a 2f2f  ![PyPI](https://
+000003f0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000400: 7970 692f 762f 7374 6163 2d66 6173 7461  ypi/v/stac-fasta
+00000410: 7069 2e70 6773 7461 633f 7374 796c 653d  pi.pgstac?style=
+00000420: 666f 722d 7468 652d 6261 6467 6529 5d28  for-the-badge)](
+00000430: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000440: 2f70 726f 6a65 6374 2f73 7461 632d 6661  /project/stac-fa
+00000450: 7374 6170 692e 7067 7374 6163 290a 5b21  stapi.pgstac).[!
+00000460: 5b44 6f63 756d 656e 7461 7469 6f6e 5d28  [Documentation](
+00000470: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000480: 6c64 732e 696f 2f67 6974 6875 622f 6163  lds.io/github/ac
+00000490: 7469 6f6e 732f 776f 726b 666c 6f77 2f73  tions/workflow/s
+000004a0: 7461 7475 732f 7374 6163 2d75 7469 6c73  tatus/stac-utils
+000004b0: 2f73 7461 632d 6661 7374 6170 692d 7067  /stac-fastapi-pg
+000004c0: 7374 6163 2f70 6167 6573 2e79 6d6c 3f6c  stac/pages.yml?l
+000004d0: 6162 656c 3d44 6f63 7326 7374 796c 653d  abel=Docs&style=
+000004e0: 666f 722d 7468 652d 6261 6467 6529 5d28  for-the-badge)](
+000004f0: 6874 7470 733a 2f2f 7374 6163 2d75 7469  https://stac-uti
+00000500: 6c73 2e67 6974 6875 622e 696f 2f73 7461  ls.github.io/sta
+00000510: 632d 6661 7374 6170 692d 7067 7374 6163  c-fastapi-pgstac
+00000520: 2f29 0a5b 215b 4c69 6365 6e73 655d 2868  /).[![License](h
+00000530: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000540: 6473 2e69 6f2f 6769 7468 7562 2f6c 6963  ds.io/github/lic
+00000550: 656e 7365 2f73 7461 632d 7574 696c 732f  ense/stac-utils/
+00000560: 7374 6163 2d66 6173 7461 7069 2d70 6773  stac-fastapi-pgs
+00000570: 7461 633f 7374 796c 653d 666f 722d 7468  tac?style=for-th
+00000580: 652d 6261 6467 6529 5d28 6874 7470 733a  e-badge)](https:
+00000590: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7461  //github.com/sta
+000005a0: 632d 7574 696c 732f 7374 6163 2d66 6173  c-utils/stac-fas
+000005b0: 7461 7069 2d70 6773 7461 632f 626c 6f62  tapi-pgstac/blob
+000005c0: 2f6d 6169 6e2f 4c49 4345 4e53 4529 0a0a  /main/LICENSE)..
+000005d0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+000005e0: 223e 0a20 203c 696d 6720 7372 633d 2268  ">.  <img src="h
+000005f0: 7474 7073 3a2f 2f75 7365 722d 696d 6167  ttps://user-imag
+00000600: 6573 2e67 6974 6875 6275 7365 7263 6f6e  es.githubusercon
+00000610: 7465 6e74 2e63 6f6d 2f31 3034 3037 3738  tent.com/1040778
+00000620: 382f 3137 3438 3933 3837 362d 3761 3362  8/174893876-7a3b
+00000630: 3562 3761 2d39 3561 352d 3438 6334 2d39  5b7a-95a5-48c4-9
+00000640: 6666 322d 6363 3430 3866 3162 3661 6639  ff2-cc408f1b6af9
+00000650: 2e70 6e67 2220 7374 796c 653d 2276 6572  .png" style="ver
+00000660: 7469 6361 6c2d 616c 6967 6e3a 206d 6964  tical-align: mid
+00000670: 646c 653b 206d 6178 2d77 6964 7468 3a20  dle; max-width: 
+00000680: 3430 3070 783b 206d 6178 2d68 6569 6768  400px; max-heigh
+00000690: 743a 2031 3030 7078 3b22 2068 6569 6768  t: 100px;" heigh
+000006a0: 743d 3130 3020 2f3e 0a20 203c 696d 6720  t=100 />.  <img 
+000006b0: 7372 633d 2268 7474 7073 3a2f 2f66 6173  src="https://fas
+000006c0: 7461 7069 2e74 6961 6e67 6f6c 6f2e 636f  tapi.tiangolo.co
+000006d0: 6d2f 696d 672f 6c6f 676f 2d6d 6172 6769  m/img/logo-margi
+000006e0: 6e2f 6c6f 676f 2d74 6561 6c2e 706e 6722  n/logo-teal.png"
+000006f0: 2061 6c74 3d22 4661 7374 4150 4922 2073   alt="FastAPI" s
+00000700: 7479 6c65 3d22 7665 7274 6963 616c 2d61  tyle="vertical-a
+00000710: 6c69 676e 3a20 6d69 6464 6c65 3b20 6d61  lign: middle; ma
+00000720: 782d 7769 6474 683a 2034 3030 7078 3b20  x-width: 400px; 
+00000730: 6d61 782d 6865 6967 6874 3a20 3130 3070  max-height: 100p
+00000740: 783b 2220 7769 6474 683d 3230 3020 2f3e  x;" width=200 />
+00000750: 0a3c 2f70 3e0a 0a5b 5067 5354 4143 5d28  .</p>..[PgSTAC](
+00000760: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000770: 6f6d 2f73 7461 632d 7574 696c 732f 7067  om/stac-utils/pg
+00000780: 7374 6163 2920 6261 636b 656e 6420 666f  stac) backend fo
+00000790: 7220 5b73 7461 632d 6661 7374 6170 695d  r [stac-fastapi]
+000007a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000007b0: 636f 6d2f 7374 6163 2d75 7469 6c73 2f73  com/stac-utils/s
+000007c0: 7461 632d 6661 7374 6170 6929 2c20 7468  tac-fastapi), th
+000007d0: 6520 5b46 6173 7441 5049 5d28 6874 7470  e [FastAPI](http
+000007e0: 733a 2f2f 6661 7374 6170 692e 7469 616e  s://fastapi.tian
+000007f0: 676f 6c6f 2e63 6f6d 2f29 2069 6d70 6c65  golo.com/) imple
+00000800: 6d65 6e74 6174 696f 6e20 6f66 2074 6865  mentation of the
+00000810: 205b 5354 4143 2041 5049 2073 7065 635d   [STAC API spec]
+00000820: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000830: 636f 6d2f 7261 6469 616e 7465 6172 7468  com/radiantearth
+00000840: 2f73 7461 632d 6170 692d 7370 6563 290a  /stac-api-spec).
+00000850: 0a23 2320 4f76 6572 7669 6577 0a0a 2a2a  .## Overview..**
+00000860: 7374 6163 2d66 6173 7461 7069 2d70 6773  stac-fastapi-pgs
+00000870: 7461 632a 2a20 6973 2061 6e20 4854 5450  tac** is an HTTP
+00000880: 2069 6e74 6572 6661 6365 2062 7569 6c74   interface built
+00000890: 2069 6e20 4661 7374 4150 492e 0a49 7420   in FastAPI..It 
+000008a0: 7661 6c69 6461 7465 7320 7265 7175 6573  validates reques
+000008b0: 7473 2061 6e64 2064 6174 6120 7365 6e74  ts and data sent
+000008c0: 2074 6f20 6120 5b50 6753 5441 435d 2868   to a [PgSTAC](h
+000008d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000008e0: 6d2f 7374 6163 2d75 7469 6c73 2f70 6773  m/stac-utils/pgs
+000008f0: 7461 6329 2062 6163 6b65 6e64 2c20 616e  tac) backend, an
+00000900: 6420 6164 6473 205b 6c69 6e6b 735d 2868  d adds [links](h
+00000910: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000920: 6d2f 7261 6469 616e 7465 6172 7468 2f73  m/radiantearth/s
+00000930: 7461 632d 7370 6563 2f62 6c6f 622f 6d61  tac-spec/blob/ma
+00000940: 7374 6572 2f69 7465 6d2d 7370 6563 2f69  ster/item-spec/i
+00000950: 7465 6d2d 7370 6563 2e6d 6423 6c69 6e6b  tem-spec.md#link
+00000960: 2d6f 626a 6563 7429 2074 6f20 7468 6520  -object) to the 
+00000970: 7265 7475 726e 6564 2064 6174 612e 0a41  returned data..A
+00000980: 6c6c 206f 7468 6572 2070 726f 6365 7373  ll other process
+00000990: 696e 6720 616e 6420 7365 6172 6368 2069  ing and search i
+000009a0: 7320 7072 6f76 6964 6564 2064 6972 6563  s provided direc
+000009b0: 746c 7920 7573 696e 6720 5067 5354 4143  tly using PgSTAC
+000009c0: 2070 726f 6365 6475 7261 6c20 7371 6c20   procedural sql 
+000009d0: 2f20 706c 7067 7371 6c20 6675 6e63 7469  / plpgsql functi
+000009e0: 6f6e 7320 6f6e 2074 6865 2064 6174 6162  ons on the datab
+000009f0: 6173 652e 0a50 6753 5441 4320 7374 6f72  ase..PgSTAC stor
+00000a00: 6573 2061 6c6c 2063 6f6c 6c65 6374 696f  es all collectio
+00000a10: 6e20 616e 6420 6974 656d 2072 6563 6f72  n and item recor
+00000a20: 6473 2061 7320 6a73 6f6e 6220 6669 656c  ds as jsonb fiel
+00000a30: 6473 2065 7861 6374 6c79 2061 7320 7468  ds exactly as th
+00000a40: 6579 2063 6f6d 6520 696e 2061 6c6c 6f77  ey come in allow
+00000a50: 696e 6720 666f 7220 616e 7920 6375 7374  ing for any cust
+00000a60: 6f6d 2066 6965 6c64 7320 746f 2062 6520  om fields to be 
+00000a70: 7374 6f72 6564 2061 6e64 2072 6574 7269  stored and retri
+00000a80: 6576 6564 2074 7261 6e73 7061 7265 6e74  eved transparent
+00000a90: 6c79 2e0a 0a23 2320 5573 6167 650a 0a50  ly...## Usage..P
+00000aa0: 6753 5441 4320 6973 2061 6e20 6578 7465  gSTAC is an exte
+00000ab0: 726e 616c 2070 726f 6a65 6374 2061 6e64  rnal project and
+00000ac0: 206d 6179 2062 6520 7573 6564 2062 7920   may be used by 
+00000ad0: 6d75 6c74 6970 6c65 2066 726f 6e74 2065  multiple front e
+00000ae0: 6e64 732e 0a46 6f72 2053 7461 6320 4661  nds..For Stac Fa
+00000af0: 7374 4150 4920 6465 7665 6c6f 706d 656e  stAPI developmen
+00000b00: 742c 2061 2044 6f63 6b65 7220 696d 6167  t, a Docker imag
+00000b10: 6520 2877 6869 6368 2069 7320 7075 6c6c  e (which is pull
+00000b20: 6564 2061 7320 7061 7274 206f 6620 7468  ed as part of th
+00000b30: 6520 646f 636b 6572 2d63 6f6d 706f 7365  e docker-compose
+00000b40: 2920 6973 2061 7661 696c 6162 6c65 2076  ) is available v
+00000b50: 6961 2074 6865 205b 4769 7468 7562 2063  ia the [Github c
+00000b60: 6f6e 7461 696e 6572 2072 6567 6973 7472  ontainer registr
+00000b70: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
+00000b80: 622e 636f 6d2f 7374 6163 2d75 7469 6c73  b.com/stac-utils
+00000b90: 2f70 6773 7461 632f 706b 6773 2f63 6f6e  /pgstac/pkgs/con
+00000ba0: 7461 696e 6572 2f70 6773 7461 632f 3831  tainer/pgstac/81
+00000bb0: 3638 3937 3934 3f74 6167 3d6c 6174 6573  689794?tag=lates
+00000bc0: 7429 2e0a 5468 6520 5067 5354 4143 2076  t)..The PgSTAC v
+00000bd0: 6572 7369 6f6e 2072 6571 7569 7265 6420  ersion required 
+00000be0: 6279 202a 2a73 7461 632d 6661 7374 6170  by **stac-fastap
+00000bf0: 692d 7067 7374 6163 2a2a 2069 7320 666f  i-pgstac** is fo
+00000c00: 756e 6420 696e 2074 6865 205b 7365 7475  und in the [setu
+00000c10: 705d 2868 7474 703a 2f2f 6769 7468 7562  p](http://github
+00000c20: 2e63 6f6d 2f73 7461 632d 7574 696c 732f  .com/stac-utils/
+00000c30: 7374 6163 2d66 6173 7461 7069 2d70 6773  stac-fastapi-pgs
+00000c40: 7461 632f 626c 6f62 2f6d 6169 6e2f 7365  tac/blob/main/se
+00000c50: 7475 702e 7079 2920 6669 6c65 2e0a 0a23  tup.py) file...#
+00000c60: 2323 2053 6f72 7469 6e67 0a0a 5768 696c  ## Sorting..Whil
+00000c70: 6520 7468 6520 5354 4143 205b 536f 7274  e the STAC [Sort
+00000c80: 2045 7874 656e 7369 6f6e 5d28 6874 7470   Extension](http
+00000c90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000ca0: 7461 632d 6170 692d 6578 7465 6e73 696f  tac-api-extensio
+00000cb0: 6e73 2f73 6f72 7429 2069 7320 6675 6c6c  ns/sort) is full
+00000cc0: 7920 7375 7070 6f72 7465 642c 205b 5067  y supported, [Pg
+00000cd0: 5354 4143 5d28 6874 7470 733a 2f2f 6769  STAC](https://gi
+00000ce0: 7468 7562 2e63 6f6d 2f73 7461 632d 7574  thub.com/stac-ut
+00000cf0: 696c 732f 7067 7374 6163 2920 6973 2070  ils/pgstac) is p
+00000d00: 6172 7469 6375 6c61 726c 7920 656e 6861  articularly enha
+00000d10: 6e63 6564 2074 6f20 6265 2061 626c 6520  nced to be able 
+00000d20: 746f 2073 6f72 7420 6279 2064 6174 6574  to sort by datet
+00000d30: 696d 6520 2865 6974 6865 7220 6173 6365  ime (either asce
+00000d40: 6e64 696e 6720 6f72 2064 6573 6365 6e64  nding or descend
+00000d50: 696e 6729 2e0a 536f 7274 696e 6720 6279  ing)..Sorting by
+00000d60: 2061 6e79 7468 696e 6720 6f74 6865 7220   anything other 
+00000d70: 7468 616e 2064 6174 6574 696d 6520 2874  than datetime (t
+00000d80: 6865 2064 6566 6175 6c74 2069 6620 6e6f  he default if no
+00000d90: 2073 6f72 7420 6973 2073 7065 6369 6669   sort is specifi
+00000da0: 6564 2920 6f6e 2076 6572 7920 6c61 7267  ed) on very larg
+00000db0: 6520 5354 4143 2072 6570 6f73 6974 6f72  e STAC repositor
+00000dc0: 6965 7320 7769 7468 6f75 7420 7665 7279  ies without very
+00000dd0: 2073 7065 6369 6669 6320 7175 6572 7920   specific query 
+00000de0: 6c69 6d69 7473 2028 6965 2073 656c 6563  limits (ie selec
+00000df0: 7469 6e67 2061 2073 696e 676c 6520 6461  ting a single da
+00000e00: 7920 6461 7465 2072 616e 6765 2920 7769  y date range) wi
+00000e10: 6c6c 206e 6f74 2068 6176 6520 7468 6520  ll not have the 
+00000e20: 7361 6d65 2070 6572 666f 726d 616e 6365  same performance
+00000e30: 2e0a 466f 7220 6d6f 7265 2074 6861 6e20  ..For more than 
+00000e40: 6d69 6c6c 696f 6e73 206f 6620 7265 636f  millions of reco
+00000e50: 7264 7320 6974 2069 7320 7265 636f 6d6d  rds it is recomm
+00000e60: 656e 6465 6420 746f 2065 6974 6865 7220  ended to either 
+00000e70: 7365 7420 6120 6c6f 7720 636f 6e6e 6563  set a low connec
+00000e80: 7469 6f6e 2074 696d 656f 7574 206f 6e20  tion timeout on 
+00000e90: 506f 7374 6772 6553 514c 206f 7220 746f  PostgreSQL or to
+00000ea0: 2064 6973 6162 6c65 2075 7365 206f 6620   disable use of 
+00000eb0: 7468 6520 536f 7274 2045 7874 656e 7369  the Sort Extensi
+00000ec0: 6f6e 2e0a 0a23 2323 2048 7964 7261 7469  on...### Hydrati
+00000ed0: 6f6e 0a0a 546f 2063 6f6e 6669 6775 7265  on..To configure
+00000ee0: 202a 2a73 7461 632d 6661 7374 6170 692d   **stac-fastapi-
+00000ef0: 7067 7374 6163 2a2a 2074 6f20 5b68 7964  pgstac** to [hyd
+00000f00: 7261 7465 2073 6561 7263 6820 7265 7375  rate search resu
+00000f10: 6c74 2069 7465 6d73 2069 6e20 7468 6520  lt items in the 
+00000f20: 4150 495d 2868 7474 7073 3a2f 2f73 7461  API](https://sta
+00000f30: 632d 7574 696c 732e 6769 7468 7562 2e69  c-utils.github.i
+00000f40: 6f2f 7067 7374 6163 2f70 6773 7461 632f  o/pgstac/pgstac/
+00000f50: 2372 756e 7469 6d65 2d63 6f6e 6669 6775  #runtime-configu
+00000f60: 7261 7469 6f6e 7329 2c20 7365 7420 7468  rations), set th
+00000f70: 6520 6055 5345 5f41 5049 5f48 5944 5241  e `USE_API_HYDRA
+00000f80: 5445 6020 656e 7669 726f 6e6d 656e 7420  TE` environment 
+00000f90: 7661 7269 6162 6c65 2074 6f20 6074 7275  variable to `tru
+00000fa0: 6560 206f 7220 6578 706c 6963 6974 6c79  e` or explicitly
+00000fb0: 2073 6574 2074 6865 206f 7074 696f 6e20   set the option 
+00000fc0: 696e 2074 6865 2050 4753 7461 6320 5365  in the PGStac Se
+00000fd0: 7474 696e 6773 206f 626a 6563 742e 0a0a  ttings object...
+00000fe0: 2323 2320 4d69 6772 6174 696f 6e73 0a0a  ### Migrations..
+00000ff0: 5468 6572 6520 6973 2061 2050 7974 686f  There is a Pytho
+00001000: 6e20 7574 696c 6974 7920 6173 2070 6172  n utility as par
+00001010: 7420 6f66 2050 6753 5441 4320 285b 7079  t of PgSTAC ([py
+00001020: 7067 7374 6163 5d28 6874 7470 733a 2f2f  pgstac](https://
+00001030: 7374 6163 2d75 7469 6c73 2e67 6974 6875  stac-utils.githu
+00001040: 622e 696f 2f70 6773 7461 632f 7079 7067  b.io/pgstac/pypg
+00001050: 7374 6163 2f29 2920 7468 6174 2069 6e63  stac/)) that inc
+00001060: 6c75 6465 7320 6120 6d69 6772 6174 696f  ludes a migratio
+00001070: 6e20 7574 696c 6974 792e 0a54 6f20 7573  n utility..To us
+00001080: 653a 0a0a 6060 6073 6865 6c6c 0a70 7970  e:..```shell.pyp
+00001090: 6773 7461 6320 6d69 6772 6174 650a 6060  gstac migrate.``
+000010a0: 600a 0a23 2320 436f 6e74 7269 6275 7469  `..## Contributi
+000010b0: 6e67 0a0a 5365 6520 5b43 4f4e 5452 4942  ng..See [CONTRIB
+000010c0: 5554 494e 475d 2868 7474 7073 3a2f 2f67  UTING](https://g
+000010d0: 6974 6875 622e 636f 6d2f 7374 6163 2d75  ithub.com/stac-u
+000010e0: 7469 6c73 2f73 7461 632d 6661 7374 6170  tils/stac-fastap
+000010f0: 692d 7067 7374 6163 2f62 6c6f 622f 6d61  i-pgstac/blob/ma
+00001100: 696e 2f43 4f4e 5452 4942 5554 494e 472e  in/CONTRIBUTING.
+00001110: 6d64 2920 666f 7220 6465 7461 696c 6564  md) for detailed
+00001120: 2063 6f6e 7472 6962 7574 696f 6e20 696e   contribution in
+00001130: 7374 7275 6374 696f 6e73 2e0a 0a54 6f20  structions...To 
+00001140: 696e 7374 616c 6c3a 0a0a 6060 6073 6865  install:..```she
+00001150: 6c6c 0a67 6974 2063 6c6f 6e65 2068 7474  ll.git clone htt
+00001160: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001170: 7374 6163 2d75 7469 6c73 2f73 7461 632d  stac-utils/stac-
+00001180: 6661 7374 6170 692d 7067 7374 6163 0a63  fastapi-pgstac.c
+00001190: 6420 7374 6163 2d66 6173 7461 7069 2d70  d stac-fastapi-p
+000011a0: 6773 7461 630a 7069 7020 696e 7374 616c  gstac.pip instal
+000011b0: 6c20 2d65 2022 2e5b 6465 762c 7365 7276  l -e ".[dev,serv
+000011c0: 6572 2c64 6f63 735d 220a 6060 600a 0a54  er,docs]".```..T
+000011d0: 6f20 7465 7374 3a0a 0a60 6060 7368 656c  o test:..```shel
+000011e0: 6c0a 6d61 6b65 2074 6573 740a 6060 600a  l.make test.```.
+000011f0: 0a55 7365 2047 6974 6875 6220 5b50 756c  .Use Github [Pul
+00001200: 6c20 5265 7175 6573 7473 5d28 6874 7470  l Requests](http
+00001210: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00001220: 7461 632d 7574 696c 732f 7374 6163 2d66  tac-utils/stac-f
+00001230: 6173 7461 7069 2d70 6773 7461 632f 7075  astapi-pgstac/pu
+00001240: 6c6c 7329 2074 6f20 7072 6f76 6964 6520  lls) to provide 
+00001250: 6e65 7720 6665 6174 7572 6573 206f 7220  new features or 
+00001260: 746f 2072 6571 7565 7374 2072 6576 6965  to request revie
+00001270: 7720 6f66 2064 7261 6674 2063 6f64 652c  w of draft code,
+00001280: 2061 6e64 2075 7365 205b 4973 7375 6573   and use [Issues
+00001290: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000012a0: 2e63 6f6d 2f73 7461 632d 7574 696c 732f  .com/stac-utils/
+000012b0: 7374 6163 2d66 6173 7461 7069 2d70 6773  stac-fastapi-pgs
+000012c0: 7461 632f 6973 7375 6573 2920 746f 2072  tac/issues) to r
+000012d0: 6570 6f72 7420 6275 6773 206f 7220 7265  eport bugs or re
+000012e0: 7175 6573 7420 6e65 7720 6665 6174 7572  quest new featur
+000012f0: 6573 2e0a 0a23 2323 2044 6f63 756d 656e  es...### Documen
+00001300: 7461 7469 6f6e 0a0a 546f 2062 7569 6c64  tation..To build
+00001310: 2074 6865 2064 6f63 733a 0a0a 6060 6073   the docs:..```s
+00001320: 6865 6c6c 0a6d 616b 6520 646f 6373 0a60  hell.make docs.`
+00001330: 6060 0a0a 5468 656e 2c20 7365 7276 6520  ``..Then, serve 
+00001340: 7468 6520 646f 6373 2076 6961 2061 206c  the docs via a l
+00001350: 6f63 616c 2048 5454 5020 7365 7276 6572  ocal HTTP server
+00001360: 3a0a 0a60 6060 7368 656c 6c0a 6d6b 646f  :..```shell.mkdo
+00001370: 6373 2073 6572 7665 0a60 6060 0a0a 2323  cs serve.```..##
+00001380: 2048 6973 746f 7279 0a0a 2a2a 7374 6163   History..**stac
+00001390: 2d66 6173 7461 7069 2d70 6773 7461 632a  -fastapi-pgstac*
+000013a0: 2a20 7761 7320 696e 6974 6961 6c6c 7920  * was initially 
+000013b0: 6164 6465 6420 746f 202a 2a73 7461 632d  added to **stac-
+000013c0: 6661 7374 6170 692a 2a20 6279 205b 6465  fastapi** by [de
+000013d0: 7665 6c6f 706d 656e 7473 6565 645d 2868  velopmentseed](h
+000013e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000013f0: 6d2f 6465 7665 6c6f 706d 656e 7473 6565  m/developmentsee
+00001400: 6429 2e0a 496e 2041 7072 696c 206f 6620  d)..In April of 
+00001410: 3230 3233 2c20 6974 2077 6173 2072 656d  2023, it was rem
+00001420: 6f76 6564 2066 726f 6d20 7468 6520 636f  oved from the co
+00001430: 7265 202a 2a73 7461 632d 6661 7374 6170  re **stac-fastap
+00001440: 692a 2a20 7265 706f 7369 746f 7279 2061  i** repository a
+00001450: 6e64 206d 6f76 6564 2074 6f20 6974 7320  nd moved to its 
+00001460: 6375 7272 656e 7420 6c6f 6361 7469 6f6e  current location
+00001470: 2028 3c68 7474 703a 2f2f 6769 7468 7562   (<http://github
+00001480: 2e63 6f6d 2f73 7461 632d 7574 696c 2f73  .com/stac-util/s
+00001490: 7461 632d 6661 7374 6170 692d 7067 7374  tac-fastapi-pgst
+000014a0: 6163 3e29 2e0a 0a23 2320 4c69 6365 6e73  ac>)...## Licens
+000014b0: 650a 0a5b 4d49 545d 2868 7474 7073 3a2f  e..[MIT](https:/
+000014c0: 2f67 6974 6875 622e 636f 6d2f 7374 6163  /github.com/stac
+000014d0: 2d75 7469 6c73 2f73 7461 632d 6661 7374  -utils/stac-fast
+000014e0: 6170 692d 7067 7374 6163 2f62 6c6f 622f  api-pgstac/blob/
+000014f0: 6d61 696e 2f4c 4943 454e 5345 290a 0a3c  main/LICENSE)..<
+00001500: 212d 2d20 6d61 726b 646f 776e 6c69 6e74  !-- markdownlint
+00001510: 2d64 6973 6162 6c65 2d66 696c 6520 4d44  -disable-file MD
+00001520: 3033 3320 2d2d 3e0a                      033 -->.
```

### Comparing `stac-fastapi.pgstac-2.4.5/stac_fastapi.pgstac.egg-info/SOURCES.txt` & `stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 stac_fastapi.pgstac.egg-info/PKG-INFO
 stac_fastapi.pgstac.egg-info/SOURCES.txt
 stac_fastapi.pgstac.egg-info/dependency_links.txt
 stac_fastapi.pgstac.egg-info/entry_points.txt
 stac_fastapi.pgstac.egg-info/not-zip-safe
```

### Comparing `stac-fastapi.pgstac-2.4.5/tests/api/test_api.py` & `stac-fastapi.pgstac-2.4.6/tests/api/test_api.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.5/tests/clients/test_postgres.py` & `stac-fastapi.pgstac-2.4.6/tests/clients/test_postgres.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+import logging
 import uuid
+from contextlib import asynccontextmanager
 from copy import deepcopy
-from typing import Callable
+from typing import Callable, Literal
 
+import pytest
+from fastapi import Request
 from stac_pydantic import Collection, Item
 
+from stac_fastapi.pgstac.db import close_db_connection, connect_to_db, get_connection
+
 # from tests.conftest import MockStarletteRequest
+logger = logging.getLogger(__name__)
 
 
 async def test_create_collection(app_client, load_test_data: Callable):
     in_json = load_test_data("test_collection.json")
     in_coll = Collection.parse_obj(in_json)
     resp = await app_client.post(
         "/collections",
@@ -166,7 +173,40 @@
 #         postgres_transactions.create_item(item, request=MockStarletteRequest)
 
 #     fc = postgres_core.item_collection(coll.id, request=MockStarletteRequest)
 #     assert len(fc.features) == 5
 
 #     for item in fc.features:
 #         assert item.collection == coll.id
+
+
+@asynccontextmanager
+async def custom_get_connection(
+    request: Request,
+    readwrite: Literal["r", "w"],
+):
+    """An example of customizing the connection getter"""
+    async with get_connection(request, readwrite) as conn:
+        await conn.execute("SELECT set_config('api.test', 'added-config', false)")
+        yield conn
+
+
+class TestDbConnect:
+    @pytest.fixture
+    async def app(self, api_client):
+        """
+        app fixture override to setup app with a customized db connection getter
+        """
+        logger.debug("Customizing app setup")
+        await connect_to_db(api_client.app, custom_get_connection)
+        yield api_client.app
+        await close_db_connection(api_client.app)
+
+    async def test_db_setup(self, api_client, app_client):
+        @api_client.app.get(f"{api_client.router.prefix}/db-test")
+        async def example_view(request: Request):
+            async with request.app.state.get_connection(request, "r") as conn:
+                return await conn.fetchval("SELECT current_setting('api.test', true)")
+
+        response = await app_client.get("/db-test")
+        assert response.status_code == 200
+        assert response.json() == "added-config"
```

### Comparing `stac-fastapi.pgstac-2.4.5/tests/resources/test_collection.py` & `stac-fastapi.pgstac-2.4.6/tests/resources/test_collection.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.5/tests/resources/test_conformance.py` & `stac-fastapi.pgstac-2.4.6/tests/resources/test_conformance.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.5/tests/resources/test_item.py` & `stac-fastapi.pgstac-2.4.6/tests/resources/test_item.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from urllib.parse import parse_qs, urljoin, urlparse
 
 import pystac
 import pytest
 from httpx import AsyncClient
 from pystac.utils import datetime_to_str
 from shapely.geometry import Polygon
+from stac_fastapi.types.rfc3339 import rfc3339_str_to_datetime
 from stac_pydantic import Collection, Item
 from starlette.requests import Request
 
 from stac_fastapi.pgstac.models.links import CollectionLinks
-from stac_fastapi.types.rfc3339 import rfc3339_str_to_datetime
 
 
 async def test_create_collection(app_client, load_test_data: Callable):
     in_json = load_test_data("test_collection.json")
     in_coll = Collection.parse_obj(in_json)
     resp = await app_client.post(
         "/collections",
```

