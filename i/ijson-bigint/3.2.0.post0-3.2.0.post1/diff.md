# Comparing `tmp/ijson-bigint-3.2.0.post0.tar.gz` & `tmp/ijson-bigint-3.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ijson-bigint-3.2.0.post0.tar", last modified: Thu May 11 12:45:56 2023, max compression
+gzip compressed data, was "dist/ijson-bigint-3.2.0.post1.tar", last modified: Thu May 11 15:31:03 2023, max compression
```

## Comparing `ijson-bigint-3.2.0.post0.tar` & `ijson-bigint-3.2.0.post1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:45:56.000000 ijson-bigint-3.2.0.post0/
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25700 2023-05-11 12:45:56.000000 ijson-bigint-3.2.0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:45:56.000000 ijson-bigint-3.2.0.post0/ijson/
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:45:56.000000 ijson-bigint-3.2.0.post0/ijson/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/_yajl2_ctypes_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:45:56.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/async_reading_generator.c
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/async_reading_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/basic_parse.c
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/basic_parse.h
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/basic_parse_async.c
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/basic_parse_async.h
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/basic_parse_basecoro.c
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/basic_parse_basecoro.h
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/coro_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/coro_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/items.c
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/items.h
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/items_async.c
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/items_async.h
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/items_basecoro.c
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/items_basecoro.h
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/kvitems.c
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/kvitems.h
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/kvitems_async.c
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/kvitems_async.h
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/kvitems_basecoro.c
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/kvitems_basecoro.h
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/module.c
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/parse.c
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/parse.h
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/parse_async.c
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/parse_async.h
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/parse_basecoro.c
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/parse_basecoro.h
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/reading_generator.c
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/reading_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/backends/yajl2_cffi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/utils35.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:45:56.000000 ijson-bigint-3.2.0.post0/ijson_bigint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25700 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson_bigint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-11 12:45:56.000000 ijson-bigint-3.2.0.post0/ijson_bigint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson_bigint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/ijson_bigint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:45:56.000000 ijson-bigint-3.2.0.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:45:56.000000 ijson-bigint-3.2.0.post0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/test/_test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/test/_test_async_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/test/_test_async_types_coroutine.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/test/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/test/test_async_types_coroutines.py
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/test/test_coroutines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/test/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/test/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/test/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-11 12:45:55.000000 ijson-bigint-3.2.0.post0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:31:03.000000 ijson-bigint-3.2.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25700 2023-05-11 15:31:03.000000 ijson-bigint-3.2.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:31:03.000000 ijson-bigint-3.2.0.post1/ijson/
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:31:03.000000 ijson-bigint-3.2.0.post1/ijson/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/_yajl2_ctypes_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:31:03.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/async_reading_generator.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/async_reading_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/basic_parse.c
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/basic_parse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/basic_parse_async.c
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/basic_parse_async.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/basic_parse_basecoro.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/basic_parse_basecoro.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/coro_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/coro_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/items.c
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/items.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/items_async.c
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/items_async.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/items_basecoro.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/items_basecoro.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/kvitems.c
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/kvitems.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/kvitems_async.c
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/kvitems_async.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/kvitems_basecoro.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/kvitems_basecoro.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/parse.c
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/parse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/parse_async.c
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/parse_async.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/parse_basecoro.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/parse_basecoro.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/reading_generator.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/reading_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/backends/yajl2_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/utils35.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/ijson/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:31:03.000000 ijson-bigint-3.2.0.post1/ijson_bigint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25700 2023-05-11 15:31:02.000000 ijson-bigint-3.2.0.post1/ijson_bigint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-11 15:31:03.000000 ijson-bigint-3.2.0.post1/ijson_bigint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:31:02.000000 ijson-bigint-3.2.0.post1/ijson_bigint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 15:31:02.000000 ijson-bigint-3.2.0.post1/ijson_bigint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:31:03.000000 ijson-bigint-3.2.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:31:03.000000 ijson-bigint-3.2.0.post1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/test/_test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/test/_test_async_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/test/_test_async_types_coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/test/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/test/test_async_types_coroutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/test/test_coroutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/test/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/test/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/test/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-11 15:30:58.000000 ijson-bigint-3.2.0.post1/tox.ini
```

### Comparing `ijson-bigint-3.2.0.post0/CHANGELOG.md` & `ijson-bigint-3.2.0.post1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/LICENSE.txt` & `ijson-bigint-3.2.0.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/PKG-INFO` & `ijson-bigint-3.2.0.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ijson-bigint
-Version: 3.2.0.post0
+Version: 3.2.0.post1
 Summary: Iterative JSON parser with standard Python iterator interfaces
 Home-page: https://github.com/jbinary/ijson
 Author: Rodrigo Tobar, Ivan Sagalaev, Sergey Dobrov
 Author-email: rtobar@icrar.org, maniac@softwaremaniacs.org
 License: BSD
 Description: .. image:: https://github.com/ICRAR/ijson/actions/workflows/deploy-to-pypi.yml/badge.svg
             :target: https://github.com/ICRAR/ijson/actions/workflows/deploy-to-pypi.yml
```

### Comparing `ijson-bigint-3.2.0.post0/README.rst` & `ijson-bigint-3.2.0.post1/README.rst`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/__init__.py` & `ijson-bigint-3.2.0.post1/ijson/__init__.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/__init__.py` & `ijson-bigint-3.2.0.post1/ijson/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/_yajl2_ctypes_common.py` & `ijson-bigint-3.2.0.post1/ijson/backends/_yajl2_ctypes_common.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/python.py` & `ijson-bigint-3.2.0.post1/ijson/backends/python.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl.py` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2.py` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/async_reading_generator.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/async_reading_generator.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/async_reading_generator.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/async_reading_generator.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/basic_parse.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/basic_parse.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/basic_parse.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/basic_parse.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/basic_parse_async.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/basic_parse_async.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/basic_parse_async.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/basic_parse_async.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/basic_parse_basecoro.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/basic_parse_basecoro.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/basic_parse_basecoro.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/basic_parse_basecoro.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/builder.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/builder.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/common.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/common.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/coro_utils.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/coro_utils.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/coro_utils.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/coro_utils.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/items.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/items.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/items.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/items.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/items_async.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/items_async.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/items_async.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/items_async.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/items_basecoro.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/items_basecoro.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/items_basecoro.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/items_basecoro.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/kvitems.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/kvitems.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/kvitems.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/kvitems.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/kvitems_async.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/kvitems_async.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/kvitems_async.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/kvitems_async.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/kvitems_basecoro.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/kvitems_basecoro.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/kvitems_basecoro.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/kvitems_basecoro.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/module.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/module.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/parse.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/parse.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/parse.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/parse.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/parse_async.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/parse_async.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/parse_async.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/parse_async.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/parse_basecoro.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/parse_basecoro.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/parse_basecoro.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/parse_basecoro.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/reading_generator.c` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/reading_generator.c`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c/reading_generator.h` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c/reading_generator.h`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_c.py` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_c.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/backends/yajl2_cffi.py` & `ijson-bigint-3.2.0.post1/ijson/backends/yajl2_cffi.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/common.py` & `ijson-bigint-3.2.0.post1/ijson/common.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/compat.py` & `ijson-bigint-3.2.0.post1/ijson/compat.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/dump.py` & `ijson-bigint-3.2.0.post1/ijson/dump.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/utils.py` & `ijson-bigint-3.2.0.post1/ijson/utils.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson/utils35.py` & `ijson-bigint-3.2.0.post1/ijson/utils35.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/ijson_bigint.egg-info/PKG-INFO` & `ijson-bigint-3.2.0.post1/ijson_bigint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ijson-bigint
-Version: 3.2.0.post0
+Version: 3.2.0.post1
 Summary: Iterative JSON parser with standard Python iterator interfaces
 Home-page: https://github.com/jbinary/ijson
 Author: Rodrigo Tobar, Ivan Sagalaev, Sergey Dobrov
 Author-email: rtobar@icrar.org, maniac@softwaremaniacs.org
 License: BSD
 Description: .. image:: https://github.com/ICRAR/ijson/actions/workflows/deploy-to-pypi.yml/badge.svg
             :target: https://github.com/ICRAR/ijson/actions/workflows/deploy-to-pypi.yml
```

### Comparing `ijson-bigint-3.2.0.post0/ijson_bigint.egg-info/SOURCES.txt` & `ijson-bigint-3.2.0.post1/ijson_bigint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/setup.py` & `ijson-bigint-3.2.0.post1/setup.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/test/_test_async_common.py` & `ijson-bigint-3.2.0.post1/test/_test_async_common.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/test/_test_async_types_coroutine.py` & `ijson-bigint-3.2.0.post1/test/_test_async_types_coroutine.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/test/test_base.py` & `ijson-bigint-3.2.0.post1/test/test_base.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/test/test_coroutines.py` & `ijson-bigint-3.2.0.post1/test/test_coroutines.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/test/test_dump.py` & `ijson-bigint-3.2.0.post1/test/test_dump.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/test/test_generators.py` & `ijson-bigint-3.2.0.post1/test/test_generators.py`

 * *Files identical despite different names*

### Comparing `ijson-bigint-3.2.0.post0/test/test_misc.py` & `ijson-bigint-3.2.0.post1/test/test_misc.py`

 * *Files identical despite different names*

