# Comparing `tmp/vortexpy-3.4.4.tar.gz` & `tmp/vortexpy-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vortexpy-3.4.4.tar", last modified: Sat Apr  1 02:00:24 2023, max compression
+gzip compressed data, was "vortexpy-3.4.5.tar", last modified: Thu May 11 05:33:38 2023, max compression
```

## Comparing `vortexpy-3.4.4.tar` & `vortexpy-3.4.5.tar`

### file list

```diff
@@ -1,96 +1,99 @@
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-04-01 02:00:24.370417 vortexpy-3.4.4/
--rw-r--r--   0 jchesney   (501) staff       (20)      450 2023-04-01 02:00:24.370640 vortexpy-3.4.4/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)     4607 2021-09-22 06:19:17.000000 vortexpy-3.4.4/README.md
--rw-r--r--   0 jchesney   (501) staff       (20)       79 2023-04-01 02:00:24.371831 vortexpy-3.4.4/setup.cfg
--rw-r--r--   0 jchesney   (501) staff       (20)     1386 2023-04-01 02:00:22.000000 vortexpy-3.4.4/setup.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-04-01 02:00:24.348421 vortexpy-3.4.4/vortex/
--rw-r--r--   0 jchesney   (501) staff       (20)     1869 2022-06-14 01:05:48.000000 vortexpy-3.4.4/vortex/DataLoaderDelegate.py
--rw-r--r--   0 jchesney   (501) staff       (20)      551 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/DataWrapTuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4476 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/DeferUtil.py
--rw-r--r--   0 jchesney   (501) staff       (20)     9286 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/Jsonable.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3674 2023-02-13 09:01:49.000000 vortexpy-3.4.4/vortex/Payload.py
--rw-r--r--   0 jchesney   (501) staff       (20)     6602 2022-09-10 02:45:31.000000 vortexpy-3.4.4/vortex/PayloadEndpoint.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4911 2023-02-13 09:01:49.000000 vortexpy-3.4.4/vortex/PayloadEnvelope.py
--rw-r--r--   0 jchesney   (501) staff       (20)      319 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/PayloadFilterKeys.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4500 2023-01-11 02:41:19.000000 vortexpy-3.4.4/vortex/PayloadIO.py
--rw-r--r--   0 jchesney   (501) staff       (20)      213 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/PayloadPriority.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5356 2023-01-10 04:54:31.000000 vortexpy-3.4.4/vortex/PayloadResponse.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5830 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/SerialiseUtil.py
--rw-r--r--   0 jchesney   (501) staff       (20)    28869 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/Tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1956 2023-01-10 11:24:51.000000 vortexpy-3.4.4/vortex/TupleAction.py
--rw-r--r--   0 jchesney   (501) staff       (20)      187 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/TupleActionVortex.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1713 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/TupleSelector.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1350 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/VortexABC.py
--rw-r--r--   0 jchesney   (501) staff       (20)     8531 2023-01-07 04:45:16.000000 vortexpy-3.4.4/vortex/VortexClientHttp.py
--rw-r--r--   0 jchesney   (501) staff       (20)    10800 2023-01-07 04:45:16.000000 vortexpy-3.4.4/vortex/VortexClientTcp.py
--rw-r--r--   0 jchesney   (501) staff       (20)    11639 2023-01-08 09:38:46.000000 vortexpy-3.4.4/vortex/VortexClientWebsocketFactory.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2057 2022-09-08 04:32:19.000000 vortexpy-3.4.4/vortex/VortexConnectionABC.py
--rw-r--r--   0 jchesney   (501) staff       (20)    30776 2023-01-12 00:54:49.000000 vortexpy-3.4.4/vortex/VortexFactory.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5620 2022-12-31 04:15:27.000000 vortexpy-3.4.4/vortex/VortexPayloadProtocol.py
--rw-r--r--   0 jchesney   (501) staff       (20)    11557 2023-02-13 22:21:32.000000 vortexpy-3.4.4/vortex/VortexServer.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3758 2023-01-05 06:06:13.000000 vortexpy-3.4.4/vortex/VortexServerConnection.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5834 2023-01-08 09:01:52.000000 vortexpy-3.4.4/vortex/VortexServerHttpResource.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3081 2023-01-08 09:00:29.000000 vortexpy-3.4.4/vortex/VortexServerTcp.py
--rw-rw-rw-   0 jchesney   (501) staff       (20)     7700 2023-01-10 07:21:05.000000 vortexpy-3.4.4/vortex/VortexServerWebsocket.py
--rw-r--r--   0 jchesney   (501) staff       (20)     9717 2023-01-11 12:46:46.000000 vortexpy-3.4.4/vortex/VortexUtil.py
--rw-r--r--   0 jchesney   (501) staff       (20)    10495 2023-01-01 11:44:30.000000 vortexpy-3.4.4/vortex/VortexWritePushProducer.py
--rw-r--r--   0 jchesney   (501) staff       (20)      194 2023-04-01 02:00:22.000000 vortexpy-3.4.4/vortex/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-04-01 02:00:24.351887 vortexpy-3.4.4/vortex/handler/
--rw-r--r--   0 jchesney   (501) staff       (20)     8353 2023-04-01 02:00:03.000000 vortexpy-3.4.4/vortex/handler/TupleActionProcessor.py
--rw-r--r--   0 jchesney   (501) staff       (20)     7290 2023-01-11 11:42:42.000000 vortexpy-3.4.4/vortex/handler/TupleActionProcessorProxy.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2112 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/handler/TupleDataActionClient.py
--rw-r--r--   0 jchesney   (501) staff       (20)     9797 2023-04-01 02:00:03.000000 vortexpy-3.4.4/vortex/handler/TupleDataLoader.py
--rw-r--r--   0 jchesney   (501) staff       (20)     6196 2023-01-10 11:27:53.000000 vortexpy-3.4.4/vortex/handler/TupleDataObservableCache.py
--rw-r--r--   0 jchesney   (501) staff       (20)    12078 2023-01-10 12:12:02.000000 vortexpy-3.4.4/vortex/handler/TupleDataObservableHandler.py
--rw-r--r--   0 jchesney   (501) staff       (20)    11648 2023-01-10 12:12:02.000000 vortexpy-3.4.4/vortex/handler/TupleDataObservableProxyHandler.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5497 2023-01-10 11:27:28.000000 vortexpy-3.4.4/vortex/handler/TupleDataObserverClient.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/handler/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-04-01 02:00:24.356188 vortexpy-3.4.4/vortex/restful/
--rw-r--r--   0 jchesney   (501) staff       (20)     5153 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/restful/GzippedDataHttpClient.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3304 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/restful/GzippedDataHttpClientTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5636 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/restful/GzippedPayloadHttpClient.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3007 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/restful/RestfulHttpClient.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1662 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/restful/RestfulHttpClientTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4958 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/restful/RestfulResource.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3292 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/restful/RestfulResourceTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/restful/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-04-01 02:00:24.356979 vortexpy-3.4.4/vortex/rpc/
--rw-r--r--   0 jchesney   (501) staff       (20)    13497 2022-09-08 03:30:59.000000 vortexpy-3.4.4/vortex/rpc/RPC.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/rpc/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-04-01 02:00:24.357726 vortexpy-3.4.4/vortex/rpc/test/
--rw-r--r--   0 jchesney   (501) staff       (20)      387 2022-09-12 02:58:12.000000 vortexpy-3.4.4/vortex/rpc/test/RPCTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/rpc/test/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-04-01 02:00:24.358866 vortexpy-3.4.4/vortex/sqla_orm/
--rw-r--r--   0 jchesney   (501) staff       (20)    13698 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/sqla_orm/OrmCrudHandler.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1414 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/sqla_orm/TupleProviderForDb.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/sqla_orm/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-04-01 02:00:24.359621 vortexpy-3.4.4/vortex/storage/
--rw-r--r--   0 jchesney   (501) staff       (20)    11237 2022-09-11 13:08:55.000000 vortexpy-3.4.4/vortex/storage/TupleStorageSqlite.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-09-10 22:39:53.000000 vortexpy-3.4.4/vortex/storage/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-04-01 02:00:24.365747 vortexpy-3.4.4/vortex/test/
--rw-r--r--   0 jchesney   (501) staff       (20)     4636 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/PayloadEndpointTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1290 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/PayloadResponseTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4373 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/PayloadTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)      713 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/PerformTestActionTuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2207 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/PolymorphicTupleTypeFieldArgTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1597 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/TestTuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)      611 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/TupleDataForTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1623 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/TuplePerfTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4015 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/TupleRestfulTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3892 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/TupleTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1790 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/VortexClientHttpTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)    19710 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/VortexTcpMemoryLeakPayloadTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2336 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/VortexTcpMemoryLeakRawTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)      548 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/VortexTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-04-01 02:00:24.367028 vortexpy-3.4.4/vortex/test/vortexjs/
--rw-r--r--   0 jchesney   (501) staff       (20)      969 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/vortexjs/TupleActionProcessorTestHandler.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1979 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/vortexjs/TupleDataObservableTestHandler.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1438 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/vortexjs/VortexJSTupleLoaderTestHandler.py
--rw-r--r--   0 jchesney   (501) staff       (20)      311 2022-06-07 01:35:57.000000 vortexpy-3.4.4/vortex/test/vortexjs/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-04-01 02:00:24.368893 vortexpy-3.4.4/vortexpy.egg-info/
--rw-r--r--   0 jchesney   (501) staff       (20)      450 2023-04-01 02:00:24.000000 vortexpy-3.4.4/vortexpy.egg-info/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)     2609 2023-04-01 02:00:24.000000 vortexpy-3.4.4/vortexpy.egg-info/SOURCES.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-04-01 02:00:24.000000 vortexpy-3.4.4/vortexpy.egg-info/dependency_links.txt
--rw-r--r--   0 jchesney   (501) staff       (20)      148 2023-04-01 02:00:24.000000 vortexpy-3.4.4/vortexpy.egg-info/requires.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        7 2023-04-01 02:00:24.000000 vortexpy-3.4.4/vortexpy.egg-info/top_level.txt
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-11 05:33:38.988315 vortexpy-3.4.5/
+-rw-r--r--   0 jchesney   (501) staff       (20)      450 2023-05-11 05:33:38.988491 vortexpy-3.4.5/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)     4607 2021-09-22 06:19:17.000000 vortexpy-3.4.5/README.md
+-rw-r--r--   0 jchesney   (501) staff       (20)       79 2023-05-11 05:33:38.989144 vortexpy-3.4.5/setup.cfg
+-rw-r--r--   0 jchesney   (501) staff       (20)     1386 2023-05-11 05:33:36.000000 vortexpy-3.4.5/setup.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-11 05:33:38.951969 vortexpy-3.4.5/vortex/
+-rw-r--r--   0 jchesney   (501) staff       (20)      551 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/DataWrapTuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4476 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/DeferUtil.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     9286 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/Jsonable.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3674 2023-02-13 09:01:49.000000 vortexpy-3.4.5/vortex/Payload.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     6602 2022-09-10 02:45:31.000000 vortexpy-3.4.5/vortex/PayloadEndpoint.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4911 2023-02-13 09:01:49.000000 vortexpy-3.4.5/vortex/PayloadEnvelope.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      319 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/PayloadFilterKeys.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4500 2023-01-11 02:41:19.000000 vortexpy-3.4.5/vortex/PayloadIO.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      213 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/PayloadPriority.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5356 2023-01-10 04:54:31.000000 vortexpy-3.4.5/vortex/PayloadResponse.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5830 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/SerialiseUtil.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    28869 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/Tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1956 2023-01-10 11:24:51.000000 vortexpy-3.4.5/vortex/TupleAction.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      187 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/TupleActionVortex.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1713 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/TupleSelector.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1350 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/VortexABC.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     8531 2023-01-07 04:45:16.000000 vortexpy-3.4.5/vortex/VortexClientHttp.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    10800 2023-01-07 04:45:16.000000 vortexpy-3.4.5/vortex/VortexClientTcp.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    11639 2023-01-08 09:38:46.000000 vortexpy-3.4.5/vortex/VortexClientWebsocketFactory.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2057 2022-09-08 04:32:19.000000 vortexpy-3.4.5/vortex/VortexConnectionABC.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    30776 2023-01-12 00:54:49.000000 vortexpy-3.4.5/vortex/VortexFactory.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5620 2022-12-31 04:15:27.000000 vortexpy-3.4.5/vortex/VortexPayloadProtocol.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    11557 2023-02-13 22:21:32.000000 vortexpy-3.4.5/vortex/VortexServer.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3758 2023-01-05 06:06:13.000000 vortexpy-3.4.5/vortex/VortexServerConnection.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5834 2023-01-08 09:01:52.000000 vortexpy-3.4.5/vortex/VortexServerHttpResource.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3081 2023-01-08 09:00:29.000000 vortexpy-3.4.5/vortex/VortexServerTcp.py
+-rw-rw-rw-   0 jchesney   (501) staff       (20)     7700 2023-01-10 07:21:05.000000 vortexpy-3.4.5/vortex/VortexServerWebsocket.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     9717 2023-01-11 12:46:46.000000 vortexpy-3.4.5/vortex/VortexUtil.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    10495 2023-01-01 11:44:30.000000 vortexpy-3.4.5/vortex/VortexWritePushProducer.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      194 2023-05-11 05:33:36.000000 vortexpy-3.4.5/vortex/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-11 05:33:38.954115 vortexpy-3.4.5/vortex/data_loader/
+-rw-r--r--   0 jchesney   (501) staff       (20)    10220 2023-04-25 07:58:51.000000 vortexpy-3.4.5/vortex/data_loader/TupleDataLoader.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1953 2023-04-18 12:21:01.000000 vortexpy-3.4.5/vortex/data_loader/TupleDataLoaderDelegate.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      177 2023-04-18 11:21:17.000000 vortexpy-3.4.5/vortex/data_loader/TupleDataLoaderTupleABC.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2023-04-01 05:32:56.000000 vortexpy-3.4.5/vortex/data_loader/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-11 05:33:38.959122 vortexpy-3.4.5/vortex/handler/
+-rw-r--r--   0 jchesney   (501) staff       (20)     8353 2023-04-01 02:00:03.000000 vortexpy-3.4.5/vortex/handler/TupleActionProcessor.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     7290 2023-01-11 11:42:42.000000 vortexpy-3.4.5/vortex/handler/TupleActionProcessorProxy.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2112 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/handler/TupleDataActionClient.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     6196 2023-01-10 11:27:53.000000 vortexpy-3.4.5/vortex/handler/TupleDataObservableCache.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    12078 2023-01-10 12:12:02.000000 vortexpy-3.4.5/vortex/handler/TupleDataObservableHandler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    11648 2023-01-10 12:12:02.000000 vortexpy-3.4.5/vortex/handler/TupleDataObservableProxyHandler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5497 2023-01-10 11:27:28.000000 vortexpy-3.4.5/vortex/handler/TupleDataObserverClient.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/handler/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-11 05:33:38.964157 vortexpy-3.4.5/vortex/restful/
+-rw-r--r--   0 jchesney   (501) staff       (20)     5153 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/restful/GzippedDataHttpClient.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3304 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/restful/GzippedDataHttpClientTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5636 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/restful/GzippedPayloadHttpClient.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3007 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/restful/RestfulHttpClient.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1662 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/restful/RestfulHttpClientTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4958 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/restful/RestfulResource.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3292 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/restful/RestfulResourceTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/restful/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-11 05:33:38.965890 vortexpy-3.4.5/vortex/rpc/
+-rw-r--r--   0 jchesney   (501) staff       (20)    13497 2022-09-08 03:30:59.000000 vortexpy-3.4.5/vortex/rpc/RPC.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/rpc/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-11 05:33:38.967203 vortexpy-3.4.5/vortex/rpc/test/
+-rw-r--r--   0 jchesney   (501) staff       (20)      387 2022-09-12 02:58:12.000000 vortexpy-3.4.5/vortex/rpc/test/RPCTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/rpc/test/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-11 05:33:38.968585 vortexpy-3.4.5/vortex/sqla_orm/
+-rw-r--r--   0 jchesney   (501) staff       (20)    13698 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/sqla_orm/OrmCrudHandler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1414 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/sqla_orm/TupleProviderForDb.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/sqla_orm/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-11 05:33:38.969419 vortexpy-3.4.5/vortex/storage/
+-rw-r--r--   0 jchesney   (501) staff       (20)    11237 2022-09-11 13:08:55.000000 vortexpy-3.4.5/vortex/storage/TupleStorageSqlite.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-09-10 22:39:53.000000 vortexpy-3.4.5/vortex/storage/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-11 05:33:38.983916 vortexpy-3.4.5/vortex/test/
+-rw-r--r--   0 jchesney   (501) staff       (20)     4636 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/PayloadEndpointTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1290 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/PayloadResponseTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4373 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/PayloadTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      713 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/PerformTestActionTuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2207 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/PolymorphicTupleTypeFieldArgTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1597 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/TestTuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      611 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/TupleDataForTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1623 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/TuplePerfTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4015 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/TupleRestfulTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3892 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/TupleTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1790 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/VortexClientHttpTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    19710 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/VortexTcpMemoryLeakPayloadTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2336 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/VortexTcpMemoryLeakRawTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      548 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/VortexTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-11 05:33:38.985714 vortexpy-3.4.5/vortex/test/vortexjs/
+-rw-r--r--   0 jchesney   (501) staff       (20)      969 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/vortexjs/TupleActionProcessorTestHandler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1979 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/vortexjs/TupleDataObservableTestHandler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1438 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/vortexjs/VortexJSTupleLoaderTestHandler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      311 2022-06-07 01:35:57.000000 vortexpy-3.4.5/vortex/test/vortexjs/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-05-11 05:33:38.987932 vortexpy-3.4.5/vortexpy.egg-info/
+-rw-r--r--   0 jchesney   (501) staff       (20)      450 2023-05-11 05:33:38.000000 vortexpy-3.4.5/vortexpy.egg-info/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)     2707 2023-05-11 05:33:38.000000 vortexpy-3.4.5/vortexpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-05-11 05:33:38.000000 vortexpy-3.4.5/vortexpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)      148 2023-05-11 05:33:38.000000 vortexpy-3.4.5/vortexpy.egg-info/requires.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        7 2023-05-11 05:33:38.000000 vortexpy-3.4.5/vortexpy.egg-info/top_level.txt
```

### Comparing `vortexpy-3.4.4/README.md` & `vortexpy-3.4.5/README.md`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/setup.py` & `vortexpy-3.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
 
 from setuptools import setup, find_packages
 
 package_name = "vortexpy"
-package_version = '3.4.4'
+package_version = '3.4.5'
 
 egg_info = "%s.egg-info" % package_name
 if os.path.isdir(egg_info):
     shutil.rmtree(egg_info)
 
 requirements = [
     "SQLAlchemy >= 1.0.14",  # Database abstraction layer
```

### Comparing `vortexpy-3.4.4/vortex/DataLoaderDelegate.py` & `vortexpy-3.4.5/vortex/data_loader/TupleDataLoaderDelegate.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,20 +4,20 @@
  * This software is open source, the MIT license applies.
  *
  * Website : https://www.synerty.com
  * Support : support@synerty.com
 """
 import abc
 from abc import abstractmethod
-from typing import Union, Dict, Any
+from typing import Union
 
-from twisted.internet.defer import Deferred, inlineCallbacks
+from twisted.internet.defer import Deferred
 
-from vortex.Tuple import Tuple
 from vortex.TupleSelector import TupleSelector
+from vortex.data_loader.TupleDataLoaderTupleABC import TupleDataLoaderTupleABC
 
 
 class TupleDataLoaderDelegateABC(abc.ABC):
     """Tuple Data Loader Delegate ABC
 
     ABC for delegate classes to handle the reading and writing for each forms'
     data. Handlers must be register in
@@ -28,28 +28,32 @@
     def start(self):
         pass
 
     def shutdown(self):
         pass
 
     @abstractmethod
-    def loadData(self, selector: TupleSelector) -> Union[Deferred, Tuple]:
+    def loadData(
+        self, selector: TupleSelector
+    ) -> Union[Deferred, TupleDataLoaderTupleABC]:
         """Load Data
 
         The `loadData` method is called when data needs to be loaded from a
         storage medium. The query is represented by a `TupleSelector` value
         `selector`.
 
         :param selector: The `TupleSelector` for which to load data
         :return: The `Tuple` or a `Deferred` which eventually results in a `Tuple`
         """
         pass
 
     @abstractmethod
-    def storeData(self, data: Tuple, selector: TupleSelector) -> Deferred:
+    def storeData(
+        self, data: TupleDataLoaderTupleABC, selector: TupleSelector
+    ) -> Deferred:
         """Store Data
 
         Store the data into the storage medium. The `data` is the `Tuple` which
         needs to be written
 
         :param data: Tuple to write and store
         :param selector: Previous selector used
```

### Comparing `vortexpy-3.4.4/vortex/DataWrapTuple.py` & `vortexpy-3.4.5/vortex/DataWrapTuple.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/DeferUtil.py` & `vortexpy-3.4.5/vortex/DeferUtil.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/Jsonable.py` & `vortexpy-3.4.5/vortex/Jsonable.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/Payload.py` & `vortexpy-3.4.5/vortex/Payload.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/PayloadEndpoint.py` & `vortexpy-3.4.5/vortex/PayloadEndpoint.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/PayloadEnvelope.py` & `vortexpy-3.4.5/vortex/PayloadEnvelope.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/PayloadIO.py` & `vortexpy-3.4.5/vortex/PayloadIO.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/PayloadResponse.py` & `vortexpy-3.4.5/vortex/PayloadResponse.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/SerialiseUtil.py` & `vortexpy-3.4.5/vortex/SerialiseUtil.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/Tuple.py` & `vortexpy-3.4.5/vortex/Tuple.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/TupleAction.py` & `vortexpy-3.4.5/vortex/TupleAction.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/TupleSelector.py` & `vortexpy-3.4.5/vortex/TupleSelector.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexABC.py` & `vortexpy-3.4.5/vortex/VortexABC.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexClientHttp.py` & `vortexpy-3.4.5/vortex/VortexClientHttp.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexClientTcp.py` & `vortexpy-3.4.5/vortex/VortexClientTcp.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexClientWebsocketFactory.py` & `vortexpy-3.4.5/vortex/VortexClientWebsocketFactory.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexConnectionABC.py` & `vortexpy-3.4.5/vortex/VortexConnectionABC.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexFactory.py` & `vortexpy-3.4.5/vortex/VortexFactory.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexPayloadProtocol.py` & `vortexpy-3.4.5/vortex/VortexPayloadProtocol.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexServer.py` & `vortexpy-3.4.5/vortex/VortexServer.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexServerConnection.py` & `vortexpy-3.4.5/vortex/VortexServerConnection.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexServerHttpResource.py` & `vortexpy-3.4.5/vortex/VortexServerHttpResource.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexServerTcp.py` & `vortexpy-3.4.5/vortex/VortexServerTcp.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexServerWebsocket.py` & `vortexpy-3.4.5/vortex/VortexServerWebsocket.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexUtil.py` & `vortexpy-3.4.5/vortex/VortexUtil.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/VortexWritePushProducer.py` & `vortexpy-3.4.5/vortex/VortexWritePushProducer.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/handler/TupleActionProcessor.py` & `vortexpy-3.4.5/vortex/handler/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/handler/TupleActionProcessorProxy.py` & `vortexpy-3.4.5/vortex/handler/TupleActionProcessorProxy.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/handler/TupleDataActionClient.py` & `vortexpy-3.4.5/vortex/handler/TupleDataActionClient.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/handler/TupleDataLoader.py` & `vortexpy-3.4.5/vortex/data_loader/TupleDataLoader.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,34 +3,36 @@
  *
  * This software is open source, the MIT license applies.
  *
  * Website : https://www.synerty.com
  * Support : support@synerty.com
 """
 import logging
-from typing import Type, Dict, Union
-
-from twisted.internet.defer import Deferred, inlineCallbacks
+from typing import Dict
+from typing import Type
+from typing import Union
 
+from twisted.internet.defer import Deferred
+from twisted.internet.defer import inlineCallbacks
 from vortex.DeferUtil import callMethodLater
-from vortex.DataLoaderDelegate import TupleDataLoaderDelegateABC
 from vortex.Payload import Payload
 from vortex.PayloadEnvelope import PayloadEnvelope
-from vortex.Tuple import TupleField, addTupleType, Tuple
+from vortex.Tuple import Tuple
+from vortex.Tuple import TupleField
+from vortex.Tuple import addTupleType
 from vortex.TupleAction import TupleActionABC
 from vortex.TupleActionVortex import TupleActionVortex
 from vortex.TupleSelector import TupleSelector
-from vortex.handler.TupleActionProcessor import (
-    TupleActionProcessorDelegateABC,
-    TupleActionProcessor,
-)
-from vortex.handler.TupleDataObservableHandler import (
-    TupleDataObservableHandler,
-    TuplesProviderABC,
+from vortex.data_loader.TupleDataLoaderDelegate import (
+    TupleDataLoaderDelegateABC,
 )
+from vortex.handler.TupleActionProcessor import TupleActionProcessor
+from vortex.handler.TupleActionProcessor import TupleActionProcessorDelegateABC
+from vortex.handler.TupleDataObservableHandler import TupleDataObservableHandler
+from vortex.handler.TupleDataObservableHandler import TuplesProviderABC
 
 logger = logging.getLogger(__name__)
 
 
 class _DataLoaderDelegateState:
     def __init__(self, delegate):
         self.delegate = delegate
@@ -209,31 +211,33 @@
             selector={
                 "name": tupleAction.selector.name,
                 "selector": tupleAction.selector.selector,
             },
         )
 
         if isinstance(tupleAction, _LockDataTupleAction):
-            if tupleAction.lock:
-                if tupleAction.selector in self._lockingUuidByTs:
-                    raise Exception("Data already locked")
-
-                self._lockingUuidByTs[
-                    tupleAction.selector
-                ] = tupleActionVortex.uuid
-            else:
-                if tupleAction.selector not in self._lockingUuidByTs:
-                    raise Exception("Data not locked")
-
-                lockingUuid = self._lockingUuidByTs[tupleAction.selector]
+            # FIXME - This doesn't work
+            # if tupleAction.lock:
+            #     if tupleAction.selector in self._lockingUuidByTs:
+            #         raise Exception("Data already locked")
+            #
+            #     self._lockingUuidByTs[
+            #         tupleAction.selector
+            #     ] = tupleActionVortex.uuid
+            # else:
+            #     if tupleAction.selector not in self._lockingUuidByTs:
+            #         raise Exception("Data not locked")
+            #
+            #     lockingUuid = self._lockingUuidByTs[tupleAction.selector]
+            #
+            #     if lockingUuid != tupleActionVortex.uuid:
+            #         raise Exception("Only the locker can unlock the data")
+            #
+            #     self._lockingUuidByTs.pop(tupleAction.selector)
 
-                if lockingUuid != tupleActionVortex.uuid:
-                    raise Exception("Only the locker can unlock the data")
-
-                self._lockingUuidByTs.pop(tupleAction.selector)
             self.__notifyOfTupleUpdate(lockingTs)
             return
 
         if (
             tupleAction.data.tupleType()
             not in self._registeredDataDelegateByDataType
         ):
@@ -252,16 +256,19 @@
                 != self._lockingUuidByTs[tupleAction.selector]
             ):
                 raise Exception("Data is locked")
 
         data = None
         if tupleAction.action == STORE_ACTION:
             data = yield entry.delegate.storeData(
-                tupleAction.data, tupleAction.selector.selector
+                tupleAction.data, tupleAction.selector
             )
+            if data is None:
+                data = yield entry.delegate.loadData(tupleAction.selector)
+
             entry.liveValueByTs[tupleAction.selector] = None
 
             # Unlock the form if it is locked
             if tupleAction.selector in self._lockingUuidByTs:
                 self._lockingUuidByTs.pop(tupleAction.selector)
                 self.__notifyOfTupleUpdate(lockingTs)
 
@@ -272,15 +279,15 @@
 
             # Unlock the form if it is locked
             if tupleAction.selector in self._lockingUuidByTs:
                 self._lockingUuidByTs.pop(tupleAction.selector)
                 self.__notifyOfTupleUpdate(lockingTs)
 
         elif tupleAction.action == DELETE_ACTION:
-            yield entry.delegate.deleteData(tupleAction.selector.selector)
+            yield entry.delegate.deleteData(tupleAction.selector)
             entry.liveValueByTs[tupleAction.selector] = None
 
             # Unlock the form if it is locked
             if tupleAction.selector in self._lockingUuidByTs:
                 self._lockingUuidByTs.pop(tupleAction.selector)
                 self.__notifyOfTupleUpdate(lockingTs)
```

### Comparing `vortexpy-3.4.4/vortex/handler/TupleDataObservableCache.py` & `vortexpy-3.4.5/vortex/handler/TupleDataObservableCache.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/handler/TupleDataObservableHandler.py` & `vortexpy-3.4.5/vortex/handler/TupleDataObservableHandler.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/handler/TupleDataObservableProxyHandler.py` & `vortexpy-3.4.5/vortex/handler/TupleDataObservableProxyHandler.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/handler/TupleDataObserverClient.py` & `vortexpy-3.4.5/vortex/handler/TupleDataObserverClient.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/restful/GzippedDataHttpClient.py` & `vortexpy-3.4.5/vortex/restful/GzippedDataHttpClient.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/restful/GzippedDataHttpClientTest.py` & `vortexpy-3.4.5/vortex/restful/GzippedDataHttpClientTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/restful/GzippedPayloadHttpClient.py` & `vortexpy-3.4.5/vortex/restful/GzippedPayloadHttpClient.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/restful/RestfulHttpClient.py` & `vortexpy-3.4.5/vortex/restful/RestfulHttpClient.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/restful/RestfulHttpClientTest.py` & `vortexpy-3.4.5/vortex/restful/RestfulHttpClientTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/restful/RestfulResource.py` & `vortexpy-3.4.5/vortex/restful/RestfulResource.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/restful/RestfulResourceTest.py` & `vortexpy-3.4.5/vortex/restful/RestfulResourceTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/rpc/RPC.py` & `vortexpy-3.4.5/vortex/rpc/RPC.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/sqla_orm/OrmCrudHandler.py` & `vortexpy-3.4.5/vortex/sqla_orm/OrmCrudHandler.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/sqla_orm/TupleProviderForDb.py` & `vortexpy-3.4.5/vortex/sqla_orm/TupleProviderForDb.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/storage/TupleStorageSqlite.py` & `vortexpy-3.4.5/vortex/storage/TupleStorageSqlite.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/PayloadEndpointTest.py` & `vortexpy-3.4.5/vortex/test/PayloadEndpointTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/PayloadResponseTest.py` & `vortexpy-3.4.5/vortex/test/PayloadResponseTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/PayloadTest.py` & `vortexpy-3.4.5/vortex/test/PayloadTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/PerformTestActionTuple.py` & `vortexpy-3.4.5/vortex/test/PerformTestActionTuple.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/PolymorphicTupleTypeFieldArgTest.py` & `vortexpy-3.4.5/vortex/test/PolymorphicTupleTypeFieldArgTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/TestTuple.py` & `vortexpy-3.4.5/vortex/test/TestTuple.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/TupleDataForTest.py` & `vortexpy-3.4.5/vortex/test/TupleDataForTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/TuplePerfTest.py` & `vortexpy-3.4.5/vortex/test/TuplePerfTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/TupleRestfulTest.py` & `vortexpy-3.4.5/vortex/test/TupleRestfulTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/TupleTest.py` & `vortexpy-3.4.5/vortex/test/TupleTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/VortexClientHttpTest.py` & `vortexpy-3.4.5/vortex/test/VortexClientHttpTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/VortexTcpMemoryLeakPayloadTest.py` & `vortexpy-3.4.5/vortex/test/VortexTcpMemoryLeakPayloadTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/VortexTcpMemoryLeakRawTest.py` & `vortexpy-3.4.5/vortex/test/VortexTcpMemoryLeakRawTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/VortexTest.py` & `vortexpy-3.4.5/vortex/test/VortexTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/vortexjs/TupleActionProcessorTestHandler.py` & `vortexpy-3.4.5/vortex/test/vortexjs/TupleActionProcessorTestHandler.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/vortexjs/TupleDataObservableTestHandler.py` & `vortexpy-3.4.5/vortex/test/vortexjs/TupleDataObservableTestHandler.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortex/test/vortexjs/VortexJSTupleLoaderTestHandler.py` & `vortexpy-3.4.5/vortex/test/vortexjs/VortexJSTupleLoaderTestHandler.py`

 * *Files identical despite different names*

### Comparing `vortexpy-3.4.4/vortexpy.egg-info/SOURCES.txt` & `vortexpy-3.4.5/vortexpy.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.md
 setup.cfg
 setup.py
-vortex/DataLoaderDelegate.py
 vortex/DataWrapTuple.py
 vortex/DeferUtil.py
 vortex/Jsonable.py
 vortex/Payload.py
 vortex/PayloadEndpoint.py
 vortex/PayloadEnvelope.py
 vortex/PayloadFilterKeys.py
@@ -28,18 +27,21 @@
 vortex/VortexServerConnection.py
 vortex/VortexServerHttpResource.py
 vortex/VortexServerTcp.py
 vortex/VortexServerWebsocket.py
 vortex/VortexUtil.py
 vortex/VortexWritePushProducer.py
 vortex/__init__.py
+vortex/data_loader/TupleDataLoader.py
+vortex/data_loader/TupleDataLoaderDelegate.py
+vortex/data_loader/TupleDataLoaderTupleABC.py
+vortex/data_loader/__init__.py
 vortex/handler/TupleActionProcessor.py
 vortex/handler/TupleActionProcessorProxy.py
 vortex/handler/TupleDataActionClient.py
-vortex/handler/TupleDataLoader.py
 vortex/handler/TupleDataObservableCache.py
 vortex/handler/TupleDataObservableHandler.py
 vortex/handler/TupleDataObservableProxyHandler.py
 vortex/handler/TupleDataObserverClient.py
 vortex/handler/__init__.py
 vortex/restful/GzippedDataHttpClient.py
 vortex/restful/GzippedDataHttpClientTest.py
```

