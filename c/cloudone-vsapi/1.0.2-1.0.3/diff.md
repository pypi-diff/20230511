# Comparing `tmp/cloudone-vsapi-1.0.2.tar.gz` & `tmp/cloudone-vsapi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudone-vsapi-1.0.2.tar", last modified: Wed May 10 18:24:34 2023, max compression
+gzip compressed data, was "cloudone-vsapi-1.0.3.tar", last modified: Thu May 11 05:31:11 2023, max compression
```

## Comparing `cloudone-vsapi-1.0.2.tar` & `cloudone-vsapi-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.902701 cloudone-vsapi-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-10 18:24:34.902701 cloudone-vsapi-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.898701 cloudone-vsapi-1.0.2/amaas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/amaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/amaas/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.898701 cloudone-vsapi-1.0.2/amaas/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/amaas/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.898701 cloudone-vsapi-1.0.2/amaas/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/amaas/grpc/aio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.898701 cloudone-vsapi-1.0.2/amaas/grpc/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/amaas/grpc/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.898701 cloudone-vsapi-1.0.2/amaas/grpc/protos/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-10 18:24:32.000000 cloudone-vsapi-1.0.2/amaas/grpc/protos/scan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-10 18:24:32.000000 cloudone-vsapi-1.0.2/amaas/grpc/protos/scan_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-10 18:24:32.000000 cloudone-vsapi-1.0.2/amaas/grpc/protos/scan_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.902701 cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-10 18:24:34.000000 cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 18:24:34.000000 cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:24:34.000000 cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 18:24:34.000000 cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 18:24:34.000000 cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-10 18:24:34.902701 cloudone-vsapi-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-10 18:24:33.000000 cloudone-vsapi-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.902701 cloudone-vsapi-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.981561 cloudone-vsapi-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-11 05:31:11.981561 cloudone-vsapi-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.977561 cloudone-vsapi-1.0.3/amaas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/amaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/amaas/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.977561 cloudone-vsapi-1.0.3/amaas/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/amaas/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.977561 cloudone-vsapi-1.0.3/amaas/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/amaas/grpc/aio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.977561 cloudone-vsapi-1.0.3/amaas/grpc/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/amaas/grpc/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.977561 cloudone-vsapi-1.0.3/amaas/grpc/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-11 05:31:10.000000 cloudone-vsapi-1.0.3/amaas/grpc/protos/scan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-11 05:31:10.000000 cloudone-vsapi-1.0.3/amaas/grpc/protos/scan_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-11 05:31:10.000000 cloudone-vsapi-1.0.3/amaas/grpc/protos/scan_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.981561 cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-11 05:31:11.000000 cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-11 05:31:11.000000 cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:31:11.000000 cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 05:31:11.000000 cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 05:31:11.000000 cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-11 05:31:11.981561 cloudone-vsapi-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-11 05:31:11.000000 cloudone-vsapi-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.981561 cloudone-vsapi-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/tests/test_simple.py
```

### Comparing `cloudone-vsapi-1.0.2/LICENSE` & `cloudone-vsapi-1.0.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Trend Micro Inc
+Copyright (c) 2023 Trend Micro Inc
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `cloudone-vsapi-1.0.2/PKG-INFO` & `cloudone-vsapi-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudone-vsapi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Trend Micro Cloud One VSAPI SDK for python
 Home-page: https://github.com/trendmicro/cloudone-antimalware-python-sdk
 Author: Trend Micro Cloud One Team
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -127,10 +127,10 @@
 
 
 asyncio.run(scan_files())
 
 ```
 
 ## More Resources
-- [License](LICENSE)
-- [Changelog](CHANGELOG.md)
-- [Notice](NOTICE)
+- [License](https://github.com/trendmicro/cloudone-antimalware-python-sdk/blob/main/LICENSE)
+- [Changelog](https://github.com/trendmicro/cloudone-antimalware-python-sdk/blob/main/CHANGELOG.md)
+- [Notice](https://github.com/trendmicro/cloudone-antimalware-python-sdk/blob/main/NOTICE)
```

### Comparing `cloudone-vsapi-1.0.2/README.md` & `cloudone-vsapi-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -108,10 +108,10 @@
 
 
 asyncio.run(scan_files())
 
 ```
 
 ## More Resources
-- [License](LICENSE)
-- [Changelog](CHANGELOG.md)
-- [Notice](NOTICE)
+- [License](https://github.com/trendmicro/cloudone-antimalware-python-sdk/blob/main/LICENSE)
+- [Changelog](https://github.com/trendmicro/cloudone-antimalware-python-sdk/blob/main/CHANGELOG.md)
+- [Notice](https://github.com/trendmicro/cloudone-antimalware-python-sdk/blob/main/NOTICE)
```

### Comparing `cloudone-vsapi-1.0.2/amaas/grpc/__init__.py` & `cloudone-vsapi-1.0.3/amaas/grpc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,14 @@
         'in-1': 'antimalware.in-1.cloudone.trendmicro.com:443',
         'de-1': 'antimalware.de-1.cloudone.trendmicro.com:443',
         'sg-1': 'antimalware.sg-1.cloudone.trendmicro.com:443',
         'au-1': 'antimalware.au-1.cloudone.trendmicro.com:443',
         'jp-1': 'antimalware.jp-1.cloudone.trendmicro.com:443',
         'gb-1': 'antimalware.gb-1.cloudone.trendmicro.com:443',
         'ca-1': 'antimalware.ca-1.cloudone.trendmicro.com:443',
-        'trend-us-1': 'antimalware.trend-us-1.cloudone.trendmicro.com:443'
     }
 
     host = mapping[region]
     return init(host, api_key, enable_tls, ca_cert)
 
 
 def quit(handle):
```

### Comparing `cloudone-vsapi-1.0.2/amaas/grpc/aio/__init__.py` & `cloudone-vsapi-1.0.3/amaas/grpc/aio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         'in-1': 'antimalware.in-1.cloudone.trendmicro.com:443',
         'de-1': 'antimalware.de-1.cloudone.trendmicro.com:443',
         'sg-1': 'antimalware.sg-1.cloudone.trendmicro.com:443',
         'au-1': 'antimalware.au-1.cloudone.trendmicro.com:443',
         'jp-1': 'antimalware.jp-1.cloudone.trendmicro.com:443',
         'gb-1': 'antimalware.gb-1.cloudone.trendmicro.com:443',
         'ca-1': 'antimalware.ca-1.cloudone.trendmicro.com:443',
-        'trend-us-1': 'antimalware.trend-us-1.cloudone.trendmicro.com:443'
     }
 
     host = mapping[region]
     return init(host, api_key, enable_tls, ca_cert)
 
 
 async def quit(handle):
```

### Comparing `cloudone-vsapi-1.0.2/amaas/grpc/protos/scan_pb2.py` & `cloudone-vsapi-1.0.3/amaas/grpc/protos/scan_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.2/amaas/grpc/protos/scan_pb2.pyi` & `cloudone-vsapi-1.0.3/amaas/grpc/protos/scan_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.2/amaas/grpc/protos/scan_pb2_grpc.py` & `cloudone-vsapi-1.0.3/amaas/grpc/protos/scan_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/PKG-INFO` & `cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudone-vsapi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Trend Micro Cloud One VSAPI SDK for python
 Home-page: https://github.com/trendmicro/cloudone-antimalware-python-sdk
 Author: Trend Micro Cloud One Team
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -127,10 +127,10 @@
 
 
 asyncio.run(scan_files())
 
 ```
 
 ## More Resources
-- [License](LICENSE)
-- [Changelog](CHANGELOG.md)
-- [Notice](NOTICE)
+- [License](https://github.com/trendmicro/cloudone-antimalware-python-sdk/blob/main/LICENSE)
+- [Changelog](https://github.com/trendmicro/cloudone-antimalware-python-sdk/blob/main/CHANGELOG.md)
+- [Notice](https://github.com/trendmicro/cloudone-antimalware-python-sdk/blob/main/NOTICE)
```

### Comparing `cloudone-vsapi-1.0.2/setup.py` & `cloudone-vsapi-1.0.3/setup.py`

 * *Files identical despite different names*

