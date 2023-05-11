# Comparing `tmp/esdbclient-1.0a2.tar.gz` & `tmp/esdbclient-1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esdbclient-1.0a2.tar", max compression
+gzip compressed data, was "esdbclient-1.0a3.tar", max compression
```

## Comparing `esdbclient-1.0a2.tar` & `esdbclient-1.0a3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1520 2022-06-23 14:19:18.317032 esdbclient-1.0a2/LICENSE
--rw-r--r--   0        0        0    92729 2023-05-10 19:02:06.187791 esdbclient-1.0a2/README.md
--rw-r--r--   0        0        0      515 2023-05-10 19:02:05.845353 esdbclient-1.0a2/esdbclient/__init__.py
--rw-r--r--   0        0        0    13681 2023-05-10 19:02:05.845906 esdbclient-1.0a2/esdbclient/asyncio_client.py
--rw-r--r--   0        0        0    32692 2023-05-10 19:02:05.846721 esdbclient-1.0a2/esdbclient/client.py
--rw-r--r--   0        0        0    11556 2023-05-10 19:02:05.847236 esdbclient-1.0a2/esdbclient/connection.py
--rw-r--r--   0        0        0     2156 2023-05-10 19:02:05.847689 esdbclient-1.0a2/esdbclient/esdbapibase.py
--rw-r--r--   0        0        0      800 2023-02-12 00:54:11.521056 esdbclient-1.0a2/esdbclient/events.py
--rw-r--r--   0        0        0     3100 2023-05-09 23:15:53.658421 esdbclient-1.0a2/esdbclient/exceptions.py
--rw-r--r--   0        0        0     4912 2023-05-10 19:02:05.848113 esdbclient-1.0a2/esdbclient/gossip.py
--rw-r--r--   0        0        0    23300 2023-05-10 19:02:05.848956 esdbclient-1.0a2/esdbclient/persistent.py
--rw-r--r--   0        0        0    13401 2023-05-09 15:45:39.784205 esdbclient-1.0a2/esdbclient/protos/Grpc/cluster_pb2.py
--rw-r--r--   0        0        0    37958 2023-05-09 15:45:38.350807 esdbclient-1.0a2/esdbclient/protos/Grpc/cluster_pb2.pyi
--rw-r--r--   0        0        0    19336 2023-05-09 15:45:39.761236 esdbclient-1.0a2/esdbclient/protos/Grpc/cluster_pb2_grpc.py
--rw-r--r--   0        0        0     1790 2023-05-09 15:45:39.793881 esdbclient-1.0a2/esdbclient/protos/Grpc/code_pb2.py
--rw-r--r--   0        0        0    13555 2023-05-09 15:45:37.813695 esdbclient-1.0a2/esdbclient/protos/Grpc/code_pb2.pyi
--rw-r--r--   0        0        0      158 2023-05-09 15:45:37.734763 esdbclient-1.0a2/esdbclient/protos/Grpc/code_pb2_grpc.py
--rw-r--r--   0        0        0     2817 2023-05-09 15:45:39.765118 esdbclient-1.0a2/esdbclient/protos/Grpc/gossip_pb2.py
--rw-r--r--   0        0        0     5524 2023-05-09 15:45:37.858863 esdbclient-1.0a2/esdbclient/protos/Grpc/gossip_pb2.pyi
--rw-r--r--   0        0        0     2752 2023-05-09 15:45:39.763073 esdbclient-1.0a2/esdbclient/protos/Grpc/gossip_pb2_grpc.py
--rw-r--r--   0        0        0    22467 2023-05-09 15:45:39.771649 esdbclient-1.0a2/esdbclient/protos/Grpc/persistent_pb2.py
--rw-r--r--   0        0        0    73220 2023-05-09 15:45:38.784305 esdbclient-1.0a2/esdbclient/protos/Grpc/persistent_pb2.pyi
--rw-r--r--   0        0        0    15771 2023-05-09 15:45:39.791304 esdbclient-1.0a2/esdbclient/protos/Grpc/persistent_pb2_grpc.py
--rw-r--r--   0        0        0     3782 2023-05-09 15:45:39.773845 esdbclient-1.0a2/esdbclient/protos/Grpc/shared_pb2.py
--rw-r--r--   0        0        0     9874 2023-05-09 15:45:37.963369 esdbclient-1.0a2/esdbclient/protos/Grpc/shared_pb2.pyi
--rw-r--r--   0        0        0      158 2023-05-09 15:45:37.783977 esdbclient-1.0a2/esdbclient/protos/Grpc/shared_pb2_grpc.py
--rw-r--r--   0        0        0     1686 2023-05-09 15:45:39.755017 esdbclient-1.0a2/esdbclient/protos/Grpc/status_pb2.py
--rw-r--r--   0        0        0     2838 2023-05-09 15:45:37.828819 esdbclient-1.0a2/esdbclient/protos/Grpc/status_pb2.pyi
--rw-r--r--   0        0        0      158 2023-05-09 15:45:37.797991 esdbclient-1.0a2/esdbclient/protos/Grpc/status_pb2_grpc.py
--rw-r--r--   0        0        0    19933 2023-05-09 15:45:39.801455 esdbclient-1.0a2/esdbclient/protos/Grpc/streams_pb2.py
--rw-r--r--   0        0        0    71744 2023-05-09 15:45:38.782146 esdbclient-1.0a2/esdbclient/protos/Grpc/streams_pb2.pyi
--rw-r--r--   0        0        0     9787 2023-05-09 15:45:37.926522 esdbclient-1.0a2/esdbclient/protos/Grpc/streams_pb2_grpc.py
--rw-r--r--   0        0        0        0 2022-06-23 14:19:18.321130 esdbclient-1.0a2/esdbclient/py.typed
--rw-r--r--   0        0        0    43278 2023-05-10 19:02:05.850483 esdbclient-1.0a2/esdbclient/streams.py
--rw-r--r--   0        0        0     2668 2023-05-10 23:33:41.663176 esdbclient-1.0a2/pyproject.toml
--rw-r--r--   0        0        0    96074 1970-01-01 00:00:00.000000 esdbclient-1.0a2/setup.py
--rw-r--r--   0        0        0    94059 1970-01-01 00:00:00.000000 esdbclient-1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1520 2022-06-23 14:19:18.317032 esdbclient-1.0a3/LICENSE
+-rw-r--r--   0        0        0    92729 2023-05-11 00:27:43.607190 esdbclient-1.0a3/README.md
+-rw-r--r--   0        0        0      515 2023-05-10 19:02:05.845353 esdbclient-1.0a3/esdbclient/__init__.py
+-rw-r--r--   0        0        0    13681 2023-05-10 19:02:05.845906 esdbclient-1.0a3/esdbclient/asyncio_client.py
+-rw-r--r--   0        0        0    32692 2023-05-10 19:02:05.846721 esdbclient-1.0a3/esdbclient/client.py
+-rw-r--r--   0        0        0    11556 2023-05-10 19:02:05.847236 esdbclient-1.0a3/esdbclient/connection.py
+-rw-r--r--   0        0        0     2156 2023-05-10 19:02:05.847689 esdbclient-1.0a3/esdbclient/esdbapibase.py
+-rw-r--r--   0        0        0      800 2023-02-12 00:54:11.521056 esdbclient-1.0a3/esdbclient/events.py
+-rw-r--r--   0        0        0     3100 2023-05-09 23:15:53.658421 esdbclient-1.0a3/esdbclient/exceptions.py
+-rw-r--r--   0        0        0     4912 2023-05-10 19:02:05.848113 esdbclient-1.0a3/esdbclient/gossip.py
+-rw-r--r--   0        0        0    23300 2023-05-10 19:02:05.848956 esdbclient-1.0a3/esdbclient/persistent.py
+-rw-r--r--   0        0        0    13401 2023-05-09 15:45:39.784205 esdbclient-1.0a3/esdbclient/protos/Grpc/cluster_pb2.py
+-rw-r--r--   0        0        0    37958 2023-05-09 15:45:38.350807 esdbclient-1.0a3/esdbclient/protos/Grpc/cluster_pb2.pyi
+-rw-r--r--   0        0        0    19336 2023-05-09 15:45:39.761236 esdbclient-1.0a3/esdbclient/protos/Grpc/cluster_pb2_grpc.py
+-rw-r--r--   0        0        0     1790 2023-05-09 15:45:39.793881 esdbclient-1.0a3/esdbclient/protos/Grpc/code_pb2.py
+-rw-r--r--   0        0        0    13555 2023-05-09 15:45:37.813695 esdbclient-1.0a3/esdbclient/protos/Grpc/code_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-09 15:45:37.734763 esdbclient-1.0a3/esdbclient/protos/Grpc/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2817 2023-05-09 15:45:39.765118 esdbclient-1.0a3/esdbclient/protos/Grpc/gossip_pb2.py
+-rw-r--r--   0        0        0     5524 2023-05-09 15:45:37.858863 esdbclient-1.0a3/esdbclient/protos/Grpc/gossip_pb2.pyi
+-rw-r--r--   0        0        0     2752 2023-05-09 15:45:39.763073 esdbclient-1.0a3/esdbclient/protos/Grpc/gossip_pb2_grpc.py
+-rw-r--r--   0        0        0    22467 2023-05-09 15:45:39.771649 esdbclient-1.0a3/esdbclient/protos/Grpc/persistent_pb2.py
+-rw-r--r--   0        0        0    73220 2023-05-09 15:45:38.784305 esdbclient-1.0a3/esdbclient/protos/Grpc/persistent_pb2.pyi
+-rw-r--r--   0        0        0    15771 2023-05-09 15:45:39.791304 esdbclient-1.0a3/esdbclient/protos/Grpc/persistent_pb2_grpc.py
+-rw-r--r--   0        0        0     3782 2023-05-09 15:45:39.773845 esdbclient-1.0a3/esdbclient/protos/Grpc/shared_pb2.py
+-rw-r--r--   0        0        0     9874 2023-05-09 15:45:37.963369 esdbclient-1.0a3/esdbclient/protos/Grpc/shared_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-09 15:45:37.783977 esdbclient-1.0a3/esdbclient/protos/Grpc/shared_pb2_grpc.py
+-rw-r--r--   0        0        0     1686 2023-05-09 15:45:39.755017 esdbclient-1.0a3/esdbclient/protos/Grpc/status_pb2.py
+-rw-r--r--   0        0        0     2838 2023-05-09 15:45:37.828819 esdbclient-1.0a3/esdbclient/protos/Grpc/status_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-09 15:45:37.797991 esdbclient-1.0a3/esdbclient/protos/Grpc/status_pb2_grpc.py
+-rw-r--r--   0        0        0    19933 2023-05-09 15:45:39.801455 esdbclient-1.0a3/esdbclient/protos/Grpc/streams_pb2.py
+-rw-r--r--   0        0        0    71744 2023-05-09 15:45:38.782146 esdbclient-1.0a3/esdbclient/protos/Grpc/streams_pb2.pyi
+-rw-r--r--   0        0        0     9787 2023-05-09 15:45:37.926522 esdbclient-1.0a3/esdbclient/protos/Grpc/streams_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2022-06-23 14:19:18.321130 esdbclient-1.0a3/esdbclient/py.typed
+-rw-r--r--   0        0        0    43278 2023-05-10 19:02:05.850483 esdbclient-1.0a3/esdbclient/streams.py
+-rw-r--r--   0        0        0     2668 2023-05-10 23:34:49.111370 esdbclient-1.0a3/pyproject.toml
+-rw-r--r--   0        0        0    96074 1970-01-01 00:00:00.000000 esdbclient-1.0a3/setup.py
+-rw-r--r--   0        0        0    94059 1970-01-01 00:00:00.000000 esdbclient-1.0a3/PKG-INFO
```

### Comparing `esdbclient-1.0a2/LICENSE` & `esdbclient-1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/README.md` & `esdbclient-1.0a3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5512,20 +5512,20 @@
 00015870: 7375 6273 6372 6962 655f 616c 6c5f 6576  subscribe_all_ev
 00015880: 656e 7473 2829 3a0a 2020 2020 2020 2020  ents():.        
 00015890: 7265 6365 6976 6564 2e61 7070 656e 6428  received.append(
 000158a0: 6576 656e 7429 0a20 2020 2020 2020 2069  event).        i
 000158b0: 6620 6576 656e 742e 6964 203d 3d20 6576  f event.id == ev
 000158c0: 656e 7433 2e69 643a 0a20 2020 2020 2020  ent3.id:.       
 000158d0: 2020 2020 2062 7265 616b 0a20 2020 2061       break.    a
-000158e0: 7373 6572 7420 7265 636f 7264 6564 5b2d  ssert recorded[-
+000158e0: 7373 6572 7420 7265 6365 6976 6564 5b2d  ssert received[-
 000158f0: 335d 2e69 6420 3d3d 2065 7665 6e74 312e  3].id == event1.
 00015900: 6964 0a20 2020 2061 7373 6572 7420 7265  id.    assert re
-00015910: 636f 7264 6564 5b2d 325d 2e69 6420 3d3d  corded[-2].id ==
+00015910: 6365 6976 6564 5b2d 325d 2e69 6420 3d3d  ceived[-2].id ==
 00015920: 2065 7665 6e74 322e 6964 0a20 2020 2061   event2.id.    a
-00015930: 7373 6572 7420 7265 636f 7264 6564 5b2d  ssert recorded[-
+00015930: 7373 6572 7420 7265 6365 6976 6564 5b2d  ssert received[-
 00015940: 315d 2e69 6420 3d3d 2065 7665 6e74 332e  1].id == event3.
 00015950: 6964 0a0a 0a20 2020 2023 2043 6c6f 7365  id...    # Close
 00015960: 2074 6865 2063 6c69 656e 742e 0a20 2020   the client..   
 00015970: 2061 7761 6974 2063 6c69 656e 742e 636c   await client.cl
 00015980: 6f73 6528 290a 0a0a 2320 5275 6e20 7468  ose()...# Run th
 00015990: 6520 6465 6d6f 2e0a 6173 796e 6369 6f2e  e demo..asyncio.
 000159a0: 6765 745f 6576 656e 745f 6c6f 6f70 2829  get_event_loop()
```

### Comparing `esdbclient-1.0a2/esdbclient/__init__.py` & `esdbclient-1.0a3/esdbclient/__init__.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/asyncio_client.py` & `esdbclient-1.0a3/esdbclient/asyncio_client.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/client.py` & `esdbclient-1.0a3/esdbclient/client.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/connection.py` & `esdbclient-1.0a3/esdbclient/connection.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/esdbapibase.py` & `esdbclient-1.0a3/esdbclient/esdbapibase.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/events.py` & `esdbclient-1.0a3/esdbclient/events.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/exceptions.py` & `esdbclient-1.0a3/esdbclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/gossip.py` & `esdbclient-1.0a3/esdbclient/gossip.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/persistent.py` & `esdbclient-1.0a3/esdbclient/persistent.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/cluster_pb2.py` & `esdbclient-1.0a3/esdbclient/protos/Grpc/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/cluster_pb2.pyi` & `esdbclient-1.0a3/esdbclient/protos/Grpc/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/cluster_pb2_grpc.py` & `esdbclient-1.0a3/esdbclient/protos/Grpc/cluster_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/code_pb2.py` & `esdbclient-1.0a3/esdbclient/protos/Grpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/code_pb2.pyi` & `esdbclient-1.0a3/esdbclient/protos/Grpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/gossip_pb2.py` & `esdbclient-1.0a3/esdbclient/protos/Grpc/gossip_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/gossip_pb2.pyi` & `esdbclient-1.0a3/esdbclient/protos/Grpc/gossip_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/gossip_pb2_grpc.py` & `esdbclient-1.0a3/esdbclient/protos/Grpc/gossip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/persistent_pb2.py` & `esdbclient-1.0a3/esdbclient/protos/Grpc/persistent_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/persistent_pb2.pyi` & `esdbclient-1.0a3/esdbclient/protos/Grpc/persistent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/persistent_pb2_grpc.py` & `esdbclient-1.0a3/esdbclient/protos/Grpc/persistent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/shared_pb2.py` & `esdbclient-1.0a3/esdbclient/protos/Grpc/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/shared_pb2.pyi` & `esdbclient-1.0a3/esdbclient/protos/Grpc/shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/status_pb2.py` & `esdbclient-1.0a3/esdbclient/protos/Grpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/status_pb2.pyi` & `esdbclient-1.0a3/esdbclient/protos/Grpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/streams_pb2.py` & `esdbclient-1.0a3/esdbclient/protos/Grpc/streams_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/streams_pb2.pyi` & `esdbclient-1.0a3/esdbclient/protos/Grpc/streams_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/protos/Grpc/streams_pb2_grpc.py` & `esdbclient-1.0a3/esdbclient/protos/Grpc/streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/esdbclient/streams.py` & `esdbclient-1.0a3/esdbclient/streams.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a2/pyproject.toml` & `esdbclient-1.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esdbclient"
-version = "1.0a2"
+version = "1.0a3"
 description = "Python gRPC Client for EventStoreDB"
 authors = [
     "John Bywater <john.bywater@appropriatesoftware.net>",
 ]
 license = "BSD 3-Clause"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `esdbclient-1.0a2/setup.py` & `esdbclient-1.0a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 000000d0: 2e35 322e 2a27 2c0a 2027 7072 6f74 6f62  .52.*',. 'protob
 000000e0: 7566 3e3d 332e 3131 2e30 272c 0a20 2774  uf>=3.11.0',. 't
 000000f0: 7970 696e 675f 6578 7465 6e73 696f 6e73  yping_extensions
 00000100: 275d 0a0a 7365 7475 705f 6b77 6172 6773  ']..setup_kwargs
 00000110: 203d 207b 0a20 2020 2027 6e61 6d65 273a   = {.    'name':
 00000120: 2027 6573 6462 636c 6965 6e74 272c 0a20   'esdbclient',. 
 00000130: 2020 2027 7665 7273 696f 6e27 3a20 2731     'version': '1
-00000140: 2e30 6132 272c 0a20 2020 2027 6465 7363  .0a2',.    'desc
+00000140: 2e30 6133 272c 0a20 2020 2027 6465 7363  .0a3',.    'desc
 00000150: 7269 7074 696f 6e27 3a20 2750 7974 686f  ription': 'Pytho
 00000160: 6e20 6752 5043 2043 6c69 656e 7420 666f  n gRPC Client fo
 00000170: 7220 4576 656e 7453 746f 7265 4442 272c  r EventStoreDB',
 00000180: 0a20 2020 2027 6c6f 6e67 5f64 6573 6372  .    'long_descr
 00000190: 6970 7469 6f6e 273a 2027 6672 6f6d 2065  iption': 'from e
 000001a0: 7364 6263 6c69 656e 7420 696d 706f 7274  sdbclient import
 000001b0: 2041 7379 6e63 696f 4553 4442 436c 6965   AsyncioESDBClie
@@ -5689,20 +5689,20 @@
 00016380: 7269 6265 5f61 6c6c 5f65 7665 6e74 7328  ribe_all_events(
 00016390: 293a 5c6e 2020 2020 2020 2020 7265 6365  ):\n        rece
 000163a0: 6976 6564 2e61 7070 656e 6428 6576 656e  ived.append(even
 000163b0: 7429 5c6e 2020 2020 2020 2020 6966 2065  t)\n        if e
 000163c0: 7665 6e74 2e69 6420 3d3d 2065 7665 6e74  vent.id == event
 000163d0: 332e 6964 3a5c 6e20 2020 2020 2020 2020  3.id:\n         
 000163e0: 2020 2062 7265 616b 5c6e 2020 2020 6173     break\n    as
-000163f0: 7365 7274 2072 6563 6f72 6465 645b 2d33  sert recorded[-3
+000163f0: 7365 7274 2072 6563 6569 7665 645b 2d33  sert received[-3
 00016400: 5d2e 6964 203d 3d20 6576 656e 7431 2e69  ].id == event1.i
 00016410: 645c 6e20 2020 2061 7373 6572 7420 7265  d\n    assert re
-00016420: 636f 7264 6564 5b2d 325d 2e69 6420 3d3d  corded[-2].id ==
+00016420: 6365 6976 6564 5b2d 325d 2e69 6420 3d3d  ceived[-2].id ==
 00016430: 2065 7665 6e74 322e 6964 5c6e 2020 2020   event2.id\n    
-00016440: 6173 7365 7274 2072 6563 6f72 6465 645b  assert recorded[
+00016440: 6173 7365 7274 2072 6563 6569 7665 645b  assert received[
 00016450: 2d31 5d2e 6964 203d 3d20 6576 656e 7433  -1].id == event3
 00016460: 2e69 645c 6e5c 6e5c 6e20 2020 2023 2043  .id\n\n\n    # C
 00016470: 6c6f 7365 2074 6865 2063 6c69 656e 742e  lose the client.
 00016480: 5c6e 2020 2020 6177 6169 7420 636c 6965  \n    await clie
 00016490: 6e74 2e63 6c6f 7365 2829 5c6e 5c6e 5c6e  nt.close()\n\n\n
 000164a0: 2320 5275 6e20 7468 6520 6465 6d6f 2e5c  # Run the demo.\
 000164b0: 6e61 7379 6e63 696f 2e67 6574 5f65 7665  nasyncio.get_eve
```

### Comparing `esdbclient-1.0a2/PKG-INFO` & `esdbclient-1.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6573 6462  : 2.1.Name: esdb
 00000020: 636c 6965 6e74 0a56 6572 7369 6f6e 3a20  client.Version: 
-00000030: 312e 3061 320a 5375 6d6d 6172 793a 2050  1.0a2.Summary: P
+00000030: 312e 3061 330a 5375 6d6d 6172 793a 2050  1.0a3.Summary: P
 00000040: 7974 686f 6e20 6752 5043 2043 6c69 656e  ython gRPC Clien
 00000050: 7420 666f 7220 4576 656e 7453 746f 7265  t for EventStore
 00000060: 4442 0a48 6f6d 652d 7061 6765 3a20 6874  DB.Home-page: ht
 00000070: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000080: 2f70 7965 7665 6e74 736f 7572 6369 6e67  /pyeventsourcing
 00000090: 2f65 7364 6263 6c69 656e 740a 4c69 6365  /esdbclient.Lice
 000000a0: 6e73 653a 2042 5344 2033 2d43 6c61 7573  nse: BSD 3-Claus
@@ -5595,20 +5595,20 @@
 00015da0: 2e73 7562 7363 7269 6265 5f61 6c6c 5f65  .subscribe_all_e
 00015db0: 7665 6e74 7328 293a 0a20 2020 2020 2020  vents():.       
 00015dc0: 2072 6563 6569 7665 642e 6170 7065 6e64   received.append
 00015dd0: 2865 7665 6e74 290a 2020 2020 2020 2020  (event).        
 00015de0: 6966 2065 7665 6e74 2e69 6420 3d3d 2065  if event.id == e
 00015df0: 7665 6e74 332e 6964 3a0a 2020 2020 2020  vent3.id:.      
 00015e00: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-00015e10: 6173 7365 7274 2072 6563 6f72 6465 645b  assert recorded[
+00015e10: 6173 7365 7274 2072 6563 6569 7665 645b  assert received[
 00015e20: 2d33 5d2e 6964 203d 3d20 6576 656e 7431  -3].id == event1
 00015e30: 2e69 640a 2020 2020 6173 7365 7274 2072  .id.    assert r
-00015e40: 6563 6f72 6465 645b 2d32 5d2e 6964 203d  ecorded[-2].id =
+00015e40: 6563 6569 7665 645b 2d32 5d2e 6964 203d  eceived[-2].id =
 00015e50: 3d20 6576 656e 7432 2e69 640a 2020 2020  = event2.id.    
-00015e60: 6173 7365 7274 2072 6563 6f72 6465 645b  assert recorded[
+00015e60: 6173 7365 7274 2072 6563 6569 7665 645b  assert received[
 00015e70: 2d31 5d2e 6964 203d 3d20 6576 656e 7433  -1].id == event3
 00015e80: 2e69 640a 0a0a 2020 2020 2320 436c 6f73  .id...    # Clos
 00015e90: 6520 7468 6520 636c 6965 6e74 2e0a 2020  e the client..  
 00015ea0: 2020 6177 6169 7420 636c 6965 6e74 2e63    await client.c
 00015eb0: 6c6f 7365 2829 0a0a 0a23 2052 756e 2074  lose()...# Run t
 00015ec0: 6865 2064 656d 6f2e 0a61 7379 6e63 696f  he demo..asyncio
 00015ed0: 2e67 6574 5f65 7665 6e74 5f6c 6f6f 7028  .get_event_loop(
```

