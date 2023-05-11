# Comparing `tmp/types-redis-4.5.5.1.tar.gz` & `tmp/types-redis-4.5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-redis-4.5.5.1.tar", last modified: Wed May 10 15:23:48 2023, max compression
+gzip compressed data, was "types-redis-4.5.5.2.tar", last modified: Thu May 11 18:18:04 2023, max compression
```

## Comparing `types-redis-4.5.5.1.tar` & `types-redis-4.5.5.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:48.734824 types-redis-4.5.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-05-10 15:23:47.000000 types-redis-4.5.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:23:47.000000 types-redis-4.5.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-10 15:23:48.734824 types-redis-4.5.5.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:48.730824 types-redis-4.5.5.1/redis-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-10 15:23:47.000000 types-redis-4.5.5.1/redis-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:48.730824 types-redis-4.5.5.1/redis-stubs/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/asyncio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    47468 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/asyncio/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/asyncio/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/asyncio/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/asyncio/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/asyncio/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/asyncio/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/asyncio/sentinel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/asyncio/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/backoff.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    41578 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/cluster.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:48.730824 types-redis-4.5.5.1/redis-stubs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:48.730824 types-redis-4.5.5.1/redis-stubs/commands/bf/
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/bf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/bf/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/bf/info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    72299 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/core.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:48.734824 types-redis-4.5.5.1/redis-stubs/commands/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/graph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/graph/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/graph/edge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/graph/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/graph/node.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/graph/path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/graph/query_result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/helpers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:48.734824 types-redis-4.5.5.1/redis-stubs/commands/json/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/json/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/json/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/json/decoders.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/json/path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/redismodules.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:48.734824 types-redis-4.5.5.1/redis-stubs/commands/search/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/search/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/search/aggregation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/search/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/search/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/search/result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/sentinel.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:48.734824 types-redis-4.5.5.1/redis-stubs/commands/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/timeseries/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/timeseries/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/timeseries/info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/commands/timeseries/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/crc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/ocsp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/sentinel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/typing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-10 15:19:44.000000 types-redis-4.5.5.1/redis-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:23:48.734824 types-redis-4.5.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-10 15:23:47.000000 types-redis-4.5.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:48.734824 types-redis-4.5.5.1/types_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-10 15:23:48.000000 types-redis-4.5.5.1/types_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-10 15:23:48.000000 types-redis-4.5.5.1/types_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:23:48.000000 types-redis-4.5.5.1/types_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 15:23:48.000000 types-redis-4.5.5.1/types_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 15:23:48.000000 types-redis-4.5.5.1/types_redis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-05-11 18:18:03.000000 types-redis-4.5.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 18:18:03.000000 types-redis-4.5.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.306382 types-redis-4.5.5.2/redis-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 18:18:03.000000 types-redis-4.5.5.2/redis-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.310382 types-redis-4.5.5.2/redis-stubs/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    47468 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/sentinel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/backoff.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    41578 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/cluster.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.310382 types-redis-4.5.5.2/redis-stubs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.310382 types-redis-4.5.5.2/redis-stubs/commands/bf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/bf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/bf/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/bf/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    72299 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.310382 types-redis-4.5.5.2/redis-stubs/commands/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/edge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/node.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/query_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/redis-stubs/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/json/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/json/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/json/decoders.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/json/path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/redismodules.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/redis-stubs/commands/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/search/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/search/aggregation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/search/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/search/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/search/result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/sentinel.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/redis-stubs/commands/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/timeseries/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/timeseries/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/timeseries/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/timeseries/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/crc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/ocsp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/sentinel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/typing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-11 18:18:03.000000 types-redis-4.5.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/types_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-11 18:18:04.000000 types-redis-4.5.5.2/types_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-11 18:18:04.000000 types-redis-4.5.5.2/types_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:18:04.000000 types-redis-4.5.5.2/types_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-11 18:18:04.000000 types-redis-4.5.5.2/types_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 18:18:04.000000 types-redis-4.5.5.2/types_redis.egg-info/top_level.txt
```

### Comparing `types-redis-4.5.5.1/CHANGELOG.md` & `types-redis-4.5.5.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 4.5.5.2 (2023-05-11)
+
+Bump `mypy` to `1.3.0` (#10173)
+
+Co-authored-by: AlexWaygood <alex.waygood@gmail.com>
+
 ## 4.5.5.1 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 4.5.5.0 (2023-05-09)
 
 [redis] Add new methods to `RedisClusterCommands` (#10162)
```

### Comparing `types-redis-4.5.5.1/PKG-INFO` & `types-redis-4.5.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-redis
-Version: 4.5.5.1
+Version: 4.5.5.2
 Summary: Typing stubs for redis
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `redis`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/redis. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `6c54c74a84642faf8ed9834bd1adbc10c1877326`.
```

### Comparing `types-redis-4.5.5.1/redis-stubs/__init__.pyi` & `types-redis-4.5.5.2/redis-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/asyncio/__init__.pyi` & `types-redis-4.5.5.2/redis-stubs/asyncio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/asyncio/client.pyi` & `types-redis-4.5.5.2/redis-stubs/asyncio/client.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/asyncio/cluster.pyi` & `types-redis-4.5.5.2/redis-stubs/asyncio/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/asyncio/connection.pyi` & `types-redis-4.5.5.2/redis-stubs/asyncio/connection.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/asyncio/lock.pyi` & `types-redis-4.5.5.2/redis-stubs/asyncio/lock.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/asyncio/retry.pyi` & `types-redis-4.5.5.2/redis-stubs/asyncio/retry.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/asyncio/sentinel.pyi` & `types-redis-4.5.5.2/redis-stubs/asyncio/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/asyncio/utils.pyi` & `types-redis-4.5.5.2/redis-stubs/asyncio/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/backoff.pyi` & `types-redis-4.5.5.2/redis-stubs/backoff.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/client.pyi` & `types-redis-4.5.5.2/redis-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/cluster.pyi` & `types-redis-4.5.5.2/redis-stubs/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/__init__.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/bf/__init__.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/bf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/bf/commands.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/bf/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/bf/info.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/bf/info.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/cluster.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/core.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/core.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/graph/__init__.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/graph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/graph/commands.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/graph/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/graph/query_result.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/graph/query_result.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/json/__init__.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/json/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/json/commands.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/json/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/search/__init__.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/search/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/search/aggregation.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/search/aggregation.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/search/commands.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/search/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/search/query.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/search/query.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/sentinel.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/timeseries/__init__.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/timeseries/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/timeseries/commands.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/timeseries/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/commands/timeseries/info.pyi` & `types-redis-4.5.5.2/redis-stubs/commands/timeseries/info.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/connection.pyi` & `types-redis-4.5.5.2/redis-stubs/connection.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/exceptions.pyi` & `types-redis-4.5.5.2/redis-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/lock.pyi` & `types-redis-4.5.5.2/redis-stubs/lock.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/ocsp.pyi` & `types-redis-4.5.5.2/redis-stubs/ocsp.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/sentinel.pyi` & `types-redis-4.5.5.2/redis-stubs/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/typing.pyi` & `types-redis-4.5.5.2/redis-stubs/typing.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/redis-stubs/utils.pyi` & `types-redis-4.5.5.2/redis-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.1/setup.py` & `types-redis-4.5.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `redis`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/redis. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `6c54c74a84642faf8ed9834bd1adbc10c1877326`.
 '''.lstrip()
 
 setup(name=name,
-      version="4.5.5.1",
+      version="4.5.5.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md",
```

### Comparing `types-redis-4.5.5.1/types_redis.egg-info/PKG-INFO` & `types-redis-4.5.5.2/types_redis.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-redis
-Version: 4.5.5.1
+Version: 4.5.5.2
 Summary: Typing stubs for redis
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `redis`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/redis. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `6c54c74a84642faf8ed9834bd1adbc10c1877326`.
```

### Comparing `types-redis-4.5.5.1/types_redis.egg-info/SOURCES.txt` & `types-redis-4.5.5.2/types_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

