# Comparing `tmp/tarn-0.4.3.tar.gz` & `tmp/tarn-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.4.3.tar", last modified: Mon May  1 17:00:35 2023, max compression
+gzip compressed data, was "tarn-0.4.4.tar", last modified: Wed May 10 23:42:22 2023, max compression
```

## Comparing `tarn-0.4.3.tar` & `tarn-0.4.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.760567 tarn-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-01 17:00:33.000000 tarn-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-01 17:00:33.000000 tarn-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-01 17:00:35.760567 tarn-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-01 17:00:33.000000 tarn-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-01 17:00:33.000000 tarn-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-01 17:00:33.000000 tarn-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:00:35.760567 tarn-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-01 17:00:33.000000 tarn-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.756569 tarn-0.4.3/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.756569 tarn-0.4.3/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.756569 tarn-0.4.3/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.760567 tarn-0.4.3/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.760567 tarn-0.4.3/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.760567 tarn-0.4.3/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.760567 tarn-0.4.3/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.760567 tarn-0.4.3/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.756569 tarn-0.4.3/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-01 17:00:35.000000 tarn-0.4.3/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-01 17:00:35.000000 tarn-0.4.3/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:00:35.000000 tarn-0.4.3/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-01 17:00:35.000000 tarn-0.4.3/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 17:00:35.000000 tarn-0.4.3/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:42:22.065216 tarn-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-10 23:42:19.000000 tarn-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 23:42:19.000000 tarn-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-10 23:42:22.065216 tarn-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-10 23:42:19.000000 tarn-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-10 23:42:19.000000 tarn-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 23:42:19.000000 tarn-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 23:42:22.069217 tarn-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-10 23:42:19.000000 tarn-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:42:22.061216 tarn-0.4.4/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:42:22.061216 tarn-0.4.4/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:42:22.061216 tarn-0.4.4/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:42:22.065216 tarn-0.4.4/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:42:22.065216 tarn-0.4.4/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:42:22.065216 tarn-0.4.4/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:42:22.065216 tarn-0.4.4/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:42:22.065216 tarn-0.4.4/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-10 23:42:19.000000 tarn-0.4.4/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:42:22.061216 tarn-0.4.4/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-10 23:42:21.000000 tarn-0.4.4/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-10 23:42:22.000000 tarn-0.4.4/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 23:42:21.000000 tarn-0.4.4/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 23:42:21.000000 tarn-0.4.4/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 23:42:21.000000 tarn-0.4.4/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.4.3/LICENSE` & `tarn-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/PKG-INFO` & `tarn-0.4.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.4.3
+Version: 0.4.4
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.3.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.4.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.4.3/README.md` & `tarn-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/pyproject.toml` & `tarn-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/setup.py` & `tarn-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/cache/storage.py` & `tarn-0.4.4/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/compat.py` & `tarn-0.4.4/tarn/compat.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from pathlib import Path
 from typing import Union
 
 try:
     from typing import Protocol
 except ImportError:
     Protocol = object
+try:
+    from gzip import BadGzipFile
+except ImportError:
+    BadGzipFile = OSError
 
 from .interface import PathOrStr
 
 if platform.system() == 'Windows':
     def rmtree(path, ignore_errors=False):
         # source: https://docs.python.org/3.10/library/shutil.html#rmtree-example
         def remove_readonly(func, p, _):
```

### Comparing `tarn-0.4.3/tarn/config.py` & `tarn-0.4.4/tarn/config.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/digest.py` & `tarn-0.4.4/tarn/digest.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/interface.py` & `tarn-0.4.4/tarn/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/local/storage.py` & `tarn-0.4.4/tarn/local/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/location/disk_dict.py` & `tarn-0.4.4/tarn/location/disk_dict.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/location/fanout.py` & `tarn-0.4.4/tarn/location/fanout.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/location/interface.py` & `tarn-0.4.4/tarn/location/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/location/levels.py` & `tarn-0.4.4/tarn/location/levels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/location/nginx.py` & `tarn-0.4.4/tarn/location/nginx.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/location/scp.py` & `tarn-0.4.4/tarn/location/scp.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/pickler/compat.py` & `tarn-0.4.4/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/pickler/interface.py` & `tarn-0.4.4/tarn/pickler/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/pool/hash_key.py` & `tarn-0.4.4/tarn/pool/hash_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/pool/pickle_key.py` & `tarn-0.4.4/tarn/pool/pickle_key.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from contextlib import contextmanager
 from io import BytesIO
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any, NamedTuple, Optional, Sequence, Type, Union
 
 from ..compat import HashAlgorithm
-from ..exceptions import ReadError, StorageCorruption, WriteError
+from ..exceptions import ReadError, StorageCorruption, WriteError, DeserializationError
 from ..interface import Key, PathOrStr
 from ..location import Level, Location
 from ..pickler import PREVIOUS_VERSIONS, dumps
 from ..serializers import Serializer, SerializerError
 from .hash_key import HashKeyStorage, LocationsLike, resolve_location
 
 logger = logging.getLogger(__name__)
@@ -95,15 +95,16 @@
         with self.index.read(digest) as index:
             if index is None:
                 return None, False
 
             with _unpack_mapping(index) as folder:
                 try:
                     return self.serializer.load(folder, self.storage), True
-                except ReadError as e:
+                # either the data is corrupted or missing
+                except (DeserializationError, ReadError) as e:
                     raise StorageCorruption from e
 
                 except SerializerError:
                     raise
                 except Exception as e:
                     raise RuntimeError(f'An error occurred while loading the cache for "{digest.hex()}"') from e
```

### Comparing `tarn-0.4.3/tarn/serializers.py` & `tarn-0.4.4/tarn/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,24 @@
 from functools import partial
 from gzip import GzipFile
 from pathlib import Path
 from typing import Callable, Dict, Union
 
 import numpy as np
 
-from .compat import rmtree
-from .exceptions import ReadError
+from .compat import rmtree, BadGzipFile
+from .exceptions import SerializerError, DeserializationError
 from .pool import HashKeyStorage
 
 __all__ = (
     'Serializer', 'SerializerError', 'ChainSerializer', 'DictSerializer',
     'NumpySerializer', 'JsonSerializer', 'PickleSerializer',
 )
 
 
-class SerializerError(Exception):
-    pass
-
-
 class Serializer(ABC):
     @abstractmethod
     def save(self, value, folder: Path):
         """ Saves the ``value`` to ``folder`` """
 
     @abstractmethod
     def load(self, folder: Path, storage: HashKeyStorage):
@@ -149,16 +145,18 @@
                 with GzipFile(x, 'rb') as file:
                     return np.load(file, allow_pickle=False)
         else:
             raise SerializerError
 
         try:
             return self._load_file(storage, loader, path)
-        except ValueError as e:
-            raise ReadError from e
+        except (ValueError, EOFError) as e:
+            raise DeserializationError from e
+        except BadGzipFile as e:
+            raise SerializerError from e
 
 
 class DictSerializer(Serializer):
     def __init__(self, serializer: Serializer):
         self.keys_filename = 'dict_keys.json'
         self.serializer = serializer
```

### Comparing `tarn-0.4.3/tarn/tools/locker.py` & `tarn-0.4.4/tarn/tools/locker.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/tools/size.py` & `tarn-0.4.4/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/tools/usage.py` & `tarn-0.4.4/tarn/tools/usage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn/utils.py` & `tarn-0.4.4/tarn/utils.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.3/tarn.egg-info/PKG-INFO` & `tarn-0.4.4/tarn.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.4.3
+Version: 0.4.4
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.3.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.4.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.4.3/tarn.egg-info/SOURCES.txt` & `tarn-0.4.4/tarn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

