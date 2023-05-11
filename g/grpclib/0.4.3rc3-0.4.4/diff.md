# Comparing `tmp/grpclib-0.4.3rc3.tar.gz` & `tmp/grpclib-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grpclib-0.4.3rc3.tar", last modified: Fri Jun  3 19:22:23 2022, max compression
+gzip compressed data, was "dist/grpclib-0.4.4.tar", last modified: Thu May 11 19:29:29 2023, max compression
```

## Comparing `grpclib-0.4.3rc3.tar` & `grpclib-0.4.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6810 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4599 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib/channelz/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/channelz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/channelz/service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib/channelz/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/channelz/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6401 2022-06-03 19:22:21.000000 grpclib-0.4.3rc3/grpclib/channelz/v1/channelz_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    30387 2022-06-03 19:22:21.000000 grpclib-0.4.3rc3/grpclib/channelz/v1/channelz_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    54996 2022-06-03 19:22:21.000000 grpclib-0.4.3rc3/grpclib/channelz/v1/channelz_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    34946 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4415 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/const.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib/encoding/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/encoding/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/encoding/proto.py
--rw-r--r--   0 runner    (1001) docker     (121)    10504 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib/health/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6318 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/health/check.py
--rw-r--r--   0 runner    (1001) docker     (121)     4660 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/health/service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib/health/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/health/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-06-03 19:22:20.000000 grpclib-0.4.3rc3/grpclib/health/v1/health_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-06-03 19:22:20.000000 grpclib-0.4.3rc3/grpclib/health/v1/health_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2308 2022-06-03 19:22:20.000000 grpclib-0.4.3rc3/grpclib/health/v1/health_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5130 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib/plugin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9053 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/plugin/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    25039 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib/reflection/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/reflection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5952 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/reflection/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)     6886 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/reflection/service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib/reflection/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/reflection/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-06-03 19:22:20.000000 grpclib-0.4.3rc3/grpclib/reflection/v1/reflection_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7107 2022-06-03 19:22:20.000000 grpclib-0.4.3rc3/grpclib/reflection/v1/reflection_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    11832 2022-06-03 19:22:20.000000 grpclib-0.4.3rc3/grpclib/reflection/v1/reflection_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib/reflection/v1alpha/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/reflection/v1alpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-06-03 19:22:21.000000 grpclib-0.4.3rc3/grpclib/reflection/v1alpha/reflection_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7189 2022-06-03 19:22:21.000000 grpclib-0.4.3rc3/grpclib/reflection/v1alpha/reflection_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    11820 2022-06-03 19:22:21.000000 grpclib-0.4.3rc3/grpclib/reflection/v1alpha/reflection_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    26879 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     1761 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     3947 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     6374 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/grpclib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6810 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/grpclib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-06-03 19:22:23.000000 grpclib-0.4.3rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-06-03 19:21:57.000000 grpclib-0.4.3rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-11 19:29:11.000000 grpclib-0.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-11 19:29:29.000000 grpclib-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-11 19:29:11.000000 grpclib-0.4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/channelz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/channelz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/channelz/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/channelz/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/channelz/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-11 19:29:27.000000 grpclib-0.4.4/grpclib/channelz/v1/channelz_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30387 2023-05-11 19:29:27.000000 grpclib-0.4.4/grpclib/channelz/v1/channelz_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54996 2023-05-11 19:29:27.000000 grpclib-0.4.4/grpclib/channelz/v1/channelz_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34946 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/encoding/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/encoding/proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/health/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/health/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/health/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/health/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/health/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/health/v1/health_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/health/v1/health_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/health/v1/health_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/plugin/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25144 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/reflection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/reflection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/reflection/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/reflection/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/reflection/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/reflection/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/reflection/v1/reflection_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/reflection/v1/reflection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/reflection/v1/reflection_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib/reflection/v1alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/reflection/v1alpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/reflection/v1alpha/reflection_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/reflection/v1alpha/reflection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-11 19:29:26.000000 grpclib-0.4.4/grpclib/reflection/v1alpha/reflection_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26879 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-11 19:29:11.000000 grpclib-0.4.4/grpclib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-11 19:29:28.000000 grpclib-0.4.4/grpclib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-11 19:29:29.000000 grpclib-0.4.4/grpclib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:29:28.000000 grpclib-0.4.4/grpclib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 19:29:28.000000 grpclib-0.4.4/grpclib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 19:29:28.000000 grpclib-0.4.4/grpclib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 19:29:28.000000 grpclib-0.4.4/grpclib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-11 19:29:11.000000 grpclib-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-11 19:29:29.000000 grpclib-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-11 19:29:11.000000 grpclib-0.4.4/setup.py
```

### Comparing `grpclib-0.4.3rc3/LICENSE.txt` & `grpclib-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/PKG-INFO` & `grpclib-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: grpclib
-Version: 0.4.3rc3
+Version: 0.4.4
 Summary: Pure-Python gRPC implementation for asyncio
 Home-page: https://github.com/vmagamedov/grpclib
 Author: Vladimir Magamedov
 Author-email: vladimir@magamedov.com
 License: BSD-3-Clause
 Description: Pure-Python gRPC implementation for asyncio
         ===========================================
         
-        |project|_ |documentation|_ |version|_ |tag|_ |license|_
+        .. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/7e1631d13476f1e870af0d5605b643fc14471a6d/banner-direct-single.svg
+          :target: https://standforukraine.com
+        
+        |project|_ |documentation|_ |version|_ |tag|_ |downloads|_ |license|_
         
         This project is based on `hyper-h2`_ and **requires Python >= 3.7**.
         
         .. contents::
           :local:
         
         Example
@@ -83,21 +86,21 @@
               asyncio.run(main())
         
         Installation
         ~~~~~~~~~~~~
         
         .. code-block:: console
         
-          $ pip3 install grpclib protobuf
+          $ pip3 install "grpclib[protobuf]"
         
         Bug fixes and new features are frequently published via release candidates:
         
         .. code-block:: console
         
-          $ pip3 install --upgrade --pre grpclib
+          $ pip3 install --upgrade --pre "grpclib[protobuf]"
         
         For the code generation you will also need a ``protoc`` compiler, which can be
         installed with ``protobuf`` system package:
         
         .. code-block:: console
         
           $ brew install protobuf  # example for macOS users
@@ -158,14 +161,16 @@
         .. _license: https://github.com/vmagamedov/grpclib/blob/master/LICENSE.txt
         .. |tag| image:: https://img.shields.io/github/tag/vmagamedov/grpclib.svg?label=latest&color=blue
         .. _tag: https://pypi.org/project/grpclib/#history
         .. |project| image:: https://img.shields.io/badge/vmagamedov%2Fgrpclib-blueviolet.svg?logo=github&color=blue
         .. _project: https://github.com/vmagamedov/grpclib
         .. |documentation| image:: https://img.shields.io/badge/docs-grpclib.rtfd.io-blue.svg
         .. _documentation: https://grpclib.readthedocs.io/en/latest/
+        .. |downloads| image:: https://static.pepy.tech/badge/grpclib/month
+        .. _downloads: https://pepy.tech/project/grpclib
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -174,7 +179,8 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: protobuf
```

### Comparing `grpclib-0.4.3rc3/README.rst` & `grpclib-0.4.4/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Pure-Python gRPC implementation for asyncio
 ===========================================
 
-|project|_ |documentation|_ |version|_ |tag|_ |license|_
+.. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/7e1631d13476f1e870af0d5605b643fc14471a6d/banner-direct-single.svg
+  :target: https://standforukraine.com
+
+|project|_ |documentation|_ |version|_ |tag|_ |downloads|_ |license|_
 
 This project is based on `hyper-h2`_ and **requires Python >= 3.7**.
 
 .. contents::
   :local:
 
 Example
@@ -75,21 +78,21 @@
       asyncio.run(main())
 
 Installation
 ~~~~~~~~~~~~
 
 .. code-block:: console
 
-  $ pip3 install grpclib protobuf
+  $ pip3 install "grpclib[protobuf]"
 
 Bug fixes and new features are frequently published via release candidates:
 
 .. code-block:: console
 
-  $ pip3 install --upgrade --pre grpclib
+  $ pip3 install --upgrade --pre "grpclib[protobuf]"
 
 For the code generation you will also need a ``protoc`` compiler, which can be
 installed with ``protobuf`` system package:
 
 .. code-block:: console
 
   $ brew install protobuf  # example for macOS users
@@ -150,7 +153,9 @@
 .. _license: https://github.com/vmagamedov/grpclib/blob/master/LICENSE.txt
 .. |tag| image:: https://img.shields.io/github/tag/vmagamedov/grpclib.svg?label=latest&color=blue
 .. _tag: https://pypi.org/project/grpclib/#history
 .. |project| image:: https://img.shields.io/badge/vmagamedov%2Fgrpclib-blueviolet.svg?logo=github&color=blue
 .. _project: https://github.com/vmagamedov/grpclib
 .. |documentation| image:: https://img.shields.io/badge/docs-grpclib.rtfd.io-blue.svg
 .. _documentation: https://grpclib.readthedocs.io/en/latest/
+.. |downloads| image:: https://static.pepy.tech/badge/grpclib/month
+.. _downloads: https://pepy.tech/project/grpclib
```

### Comparing `grpclib-0.4.3rc3/grpclib/_typing.py` & `grpclib-0.4.4/grpclib/_typing.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/channelz/service.py` & `grpclib-0.4.4/grpclib/channelz/service.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/channelz/v1/channelz_grpc.py` & `grpclib-0.4.4/grpclib/channelz/v1/channelz_grpc.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/channelz/v1/channelz_pb2.py` & `grpclib-0.4.4/grpclib/channelz/v1/channelz_pb2.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/channelz/v1/channelz_pb2.pyi` & `grpclib-0.4.4/grpclib/channelz/v1/channelz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/client.py` & `grpclib-0.4.4/grpclib/client.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/config.py` & `grpclib-0.4.4/grpclib/config.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/const.py` & `grpclib-0.4.4/grpclib/const.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/encoding/base.py` & `grpclib-0.4.4/grpclib/encoding/base.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/encoding/proto.py` & `grpclib-0.4.4/grpclib/encoding/proto.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/events.py` & `grpclib-0.4.4/grpclib/events.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/exceptions.py` & `grpclib-0.4.4/grpclib/exceptions.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/health/check.py` & `grpclib-0.4.4/grpclib/health/check.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/health/service.py` & `grpclib-0.4.4/grpclib/health/service.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/health/v1/health_grpc.py` & `grpclib-0.4.4/grpclib/health/v1/health_grpc.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/health/v1/health_pb2.py` & `grpclib-0.4.4/grpclib/health/v1/health_pb2.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/health/v1/health_pb2.pyi` & `grpclib-0.4.4/grpclib/health/v1/health_pb2.pyi`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/metadata.py` & `grpclib-0.4.4/grpclib/metadata.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/plugin/main.py` & `grpclib-0.4.4/grpclib/plugin/main.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/protocol.py` & `grpclib-0.4.4/grpclib/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -560,14 +560,16 @@
             del self.processors
 
     def process(self, event: H2Event) -> None:
         try:
             proc = self.processors[event.__class__]
         except KeyError:
             raise NotImplementedError(event)
+        except AttributeError:
+            pass  # connection was closed and self.processors was deleted
         else:
             proc(event)
 
     def process_request_received(self, event: RequestReceived) -> None:
         stream = self.connection.create_stream(stream_id=event.stream_id)
         release_stream = self.register(stream)
         self.handler.accept(stream, event.headers, release_stream)
```

### Comparing `grpclib-0.4.3rc3/grpclib/reflection/_deprecated.py` & `grpclib-0.4.4/grpclib/reflection/_deprecated.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/reflection/service.py` & `grpclib-0.4.4/grpclib/reflection/service.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/reflection/v1/reflection_grpc.py` & `grpclib-0.4.4/grpclib/reflection/v1/reflection_grpc.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/reflection/v1/reflection_pb2.py` & `grpclib-0.4.4/grpclib/reflection/v1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/reflection/v1/reflection_pb2.pyi` & `grpclib-0.4.4/grpclib/reflection/v1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/reflection/v1alpha/reflection_grpc.py` & `grpclib-0.4.4/grpclib/reflection/v1alpha/reflection_grpc.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/reflection/v1alpha/reflection_pb2.py` & `grpclib-0.4.4/grpclib/reflection/v1alpha/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/reflection/v1alpha/reflection_pb2.pyi` & `grpclib-0.4.4/grpclib/reflection/v1alpha/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/server.py` & `grpclib-0.4.4/grpclib/server.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/stream.py` & `grpclib-0.4.4/grpclib/stream.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/testing.py` & `grpclib-0.4.4/grpclib/testing.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib/utils.py` & `grpclib-0.4.4/grpclib/utils.py`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/grpclib.egg-info/PKG-INFO` & `grpclib-0.4.4/grpclib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: grpclib
-Version: 0.4.3rc3
+Version: 0.4.4
 Summary: Pure-Python gRPC implementation for asyncio
 Home-page: https://github.com/vmagamedov/grpclib
 Author: Vladimir Magamedov
 Author-email: vladimir@magamedov.com
 License: BSD-3-Clause
 Description: Pure-Python gRPC implementation for asyncio
         ===========================================
         
-        |project|_ |documentation|_ |version|_ |tag|_ |license|_
+        .. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/7e1631d13476f1e870af0d5605b643fc14471a6d/banner-direct-single.svg
+          :target: https://standforukraine.com
+        
+        |project|_ |documentation|_ |version|_ |tag|_ |downloads|_ |license|_
         
         This project is based on `hyper-h2`_ and **requires Python >= 3.7**.
         
         .. contents::
           :local:
         
         Example
@@ -83,21 +86,21 @@
               asyncio.run(main())
         
         Installation
         ~~~~~~~~~~~~
         
         .. code-block:: console
         
-          $ pip3 install grpclib protobuf
+          $ pip3 install "grpclib[protobuf]"
         
         Bug fixes and new features are frequently published via release candidates:
         
         .. code-block:: console
         
-          $ pip3 install --upgrade --pre grpclib
+          $ pip3 install --upgrade --pre "grpclib[protobuf]"
         
         For the code generation you will also need a ``protoc`` compiler, which can be
         installed with ``protobuf`` system package:
         
         .. code-block:: console
         
           $ brew install protobuf  # example for macOS users
@@ -158,14 +161,16 @@
         .. _license: https://github.com/vmagamedov/grpclib/blob/master/LICENSE.txt
         .. |tag| image:: https://img.shields.io/github/tag/vmagamedov/grpclib.svg?label=latest&color=blue
         .. _tag: https://pypi.org/project/grpclib/#history
         .. |project| image:: https://img.shields.io/badge/vmagamedov%2Fgrpclib-blueviolet.svg?logo=github&color=blue
         .. _project: https://github.com/vmagamedov/grpclib
         .. |documentation| image:: https://img.shields.io/badge/docs-grpclib.rtfd.io-blue.svg
         .. _documentation: https://grpclib.readthedocs.io/en/latest/
+        .. |downloads| image:: https://static.pepy.tech/badge/grpclib/month
+        .. _downloads: https://pepy.tech/project/grpclib
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -174,7 +179,8 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: protobuf
```

### Comparing `grpclib-0.4.3rc3/grpclib.egg-info/SOURCES.txt` & `grpclib-0.4.4/grpclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpclib-0.4.3rc3/setup.cfg` & `grpclib-0.4.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	h2<5,>=3.1.0
 	multidict
 
+[options.extras_require]
+protobuf = 
+	protobuf>=3.15.0
+
 [options.entry_points]
 console_scripts = 
 	protoc-gen-python_grpc=grpclib.plugin.main:main
 	protoc-gen-grpclib_python=grpclib.plugin.main:main
 
 [options.package_data]
 * = *.pyi
@@ -42,15 +46,15 @@
 
 [tool:pytest]
 addopts = -q --tb=native
 testpaths = tests
 asyncio_mode = auto
 filterwarnings = 
 	error
-	ignore::DeprecationWarning:google.*
+	ignore:.*pkg_resources.*:DeprecationWarning
 	ignore::ResourceWarning
 
 [coverage:run]
 source = grpclib
 omit = 
 	grpclib/plugin/main.py
 	*_pb2.py
```

