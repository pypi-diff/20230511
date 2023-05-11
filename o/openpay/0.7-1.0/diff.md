# Comparing `tmp/openpay0.7.tar.gz` & `tmp/openpay-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpay-0.7.tar", last modified: Thu May 11 18:48:18 2023, max compression
+gzip compressed data, was "openpay-1.0.tar", last modified: Wed May 10 20:14:12 2023, max compression
```

## Comparing `openpay0.7.tar` & `openpay-1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 marcos.vazquez   (502) staff       (20)        0 2023-05-11 18:48:18.338669 openpay-0.7/
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)      211 2023-05-11 18:48:18.338346 openpay-0.7/PKG-INFO
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)    16581 2023-04-28 23:58:01.000000 openpay-0.7/README.md
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)        4 2023-05-11 16:31:49.000000 openpay-0.7/VERSION
-drwxr-xr-x   0 marcos.vazquez   (502) staff       (20)        0 2023-05-11 18:48:18.309845 openpay-0.7/openpay/
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)     2196 2023-05-10 19:52:12.000000 openpay-0.7/openpay/__init__.py
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)     6187 2023-04-18 15:51:40.000000 openpay-0.7/openpay/api.py
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)     1601 2023-04-18 15:51:40.000000 openpay-0.7/openpay/error.py
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)     6997 2023-04-18 15:51:40.000000 openpay-0.7/openpay/http_client.py
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)    25744 2023-04-18 15:51:40.000000 openpay-0.7/openpay/resource.py
-drwxr-xr-x   0 marcos.vazquez   (502) staff       (20)        0 2023-05-11 18:48:18.336987 openpay-0.7/openpay/test/
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)      434 2023-04-18 15:51:40.000000 openpay-0.7/openpay/test/__init__.py
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)     5434 2023-04-18 15:51:40.000000 openpay-0.7/openpay/test/helper.py
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)    21990 2023-04-18 15:51:40.000000 openpay-0.7/openpay/test/test_integration.py
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)    11339 2023-04-18 15:51:40.000000 openpay-0.7/openpay/test/test_resources.py
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)      237 2023-04-18 15:51:40.000000 openpay-0.7/openpay/util.py
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)       15 2023-05-11 18:40:58.000000 openpay-0.7/openpay/version.py
-drwxr-xr-x   0 marcos.vazquez   (502) staff       (20)        0 2023-05-11 18:48:18.326864 openpay-0.7/openpay.egg-info/
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)      211 2023-05-11 18:48:18.000000 openpay-0.7/openpay.egg-info/PKG-INFO
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)      433 2023-05-11 18:48:18.000000 openpay-0.7/openpay.egg-info/SOURCES.txt
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)        1 2023-05-11 18:48:18.000000 openpay-0.7/openpay.egg-info/dependency_links.txt
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)       47 2023-05-11 18:48:18.000000 openpay-0.7/openpay.egg-info/requires.txt
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)        8 2023-05-11 18:48:18.000000 openpay-0.7/openpay.egg-info/top_level.txt
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)       38 2023-05-11 18:48:18.338772 openpay-0.7/setup.cfg
--rw-r--r--   0 marcos.vazquez   (502) staff       (20)     1330 2023-05-11 18:42:38.000000 openpay-0.7/setup.py
+drwxr-xr-x   0 marcos.vazquez   (502) staff       (20)        0 2023-05-10 20:14:12.265625 openpay-1.0/
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)      211 2023-05-10 20:14:12.265194 openpay-1.0/PKG-INFO
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)    16581 2023-04-28 23:58:01.000000 openpay-1.0/README.md
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)        4 2023-05-10 19:15:34.000000 openpay-1.0/VERSION
+drwxr-xr-x   0 marcos.vazquez   (502) staff       (20)        0 2023-05-10 20:14:12.233664 openpay-1.0/openpay/
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)     2196 2023-05-10 19:52:12.000000 openpay-1.0/openpay/__init__.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)     6187 2023-04-18 15:51:40.000000 openpay-1.0/openpay/api.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)     1601 2023-04-18 15:51:40.000000 openpay-1.0/openpay/error.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)     6997 2023-04-18 15:51:40.000000 openpay-1.0/openpay/http_client.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)    25744 2023-04-18 15:51:40.000000 openpay-1.0/openpay/resource.py
+drwxr-xr-x   0 marcos.vazquez   (502) staff       (20)        0 2023-05-10 20:14:12.264248 openpay-1.0/openpay/test/
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)      434 2023-04-18 15:51:40.000000 openpay-1.0/openpay/test/__init__.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)     5434 2023-04-18 15:51:40.000000 openpay-1.0/openpay/test/helper.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)    21990 2023-04-18 15:51:40.000000 openpay-1.0/openpay/test/test_integration.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)    11339 2023-04-18 15:51:40.000000 openpay-1.0/openpay/test/test_resources.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)      237 2023-04-18 15:51:40.000000 openpay-1.0/openpay/util.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)       16 2023-04-18 15:51:40.000000 openpay-1.0/openpay/version.py
+drwxr-xr-x   0 marcos.vazquez   (502) staff       (20)        0 2023-05-10 20:14:12.253673 openpay-1.0/openpay.egg-info/
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)      211 2023-05-10 20:14:12.000000 openpay-1.0/openpay.egg-info/PKG-INFO
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)      433 2023-05-10 20:14:12.000000 openpay-1.0/openpay.egg-info/SOURCES.txt
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)        1 2023-05-10 20:14:12.000000 openpay-1.0/openpay.egg-info/dependency_links.txt
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)       31 2023-05-10 20:14:12.000000 openpay-1.0/openpay.egg-info/requires.txt
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)        8 2023-05-10 20:14:12.000000 openpay-1.0/openpay.egg-info/top_level.txt
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)       38 2023-05-10 20:14:12.265682 openpay-1.0/setup.cfg
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)     1312 2023-04-18 15:51:40.000000 openpay-1.0/setup.py
```

### Comparing `openpay-0.7/README.md` & `openpay-1.0/README.md`

 * *Files identical despite different names*

### Comparing `openpay-0.7/openpay/__init__.py` & `openpay-1.0/openpay/__init__.py`

 * *Files identical despite different names*

### Comparing `openpay-0.7/openpay/api.py` & `openpay-1.0/openpay/api.py`

 * *Files identical despite different names*

### Comparing `openpay-0.7/openpay/error.py` & `openpay-1.0/openpay/error.py`

 * *Files identical despite different names*

### Comparing `openpay-0.7/openpay/http_client.py` & `openpay-1.0/openpay/http_client.py`

 * *Files identical despite different names*

### Comparing `openpay-0.7/openpay/resource.py` & `openpay-1.0/openpay/resource.py`

 * *Files identical despite different names*

### Comparing `openpay-0.7/openpay/test/helper.py` & `openpay-1.0/openpay/test/helper.py`

 * *Files identical despite different names*

### Comparing `openpay-0.7/openpay/test/test_integration.py` & `openpay-1.0/openpay/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `openpay-0.7/openpay/test/test_resources.py` & `openpay-1.0/openpay/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `openpay-0.7/setup.py` & `openpay-1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 path, script = os.path.split(sys.argv[0])
 os.chdir(os.path.abspath(path))
 
 requests = 'requests >= 2.1.0'
 if sys.version_info < (2, 6):
     requests += ', < 2.1.0'
-install_requires = [requests, "future==0.15.2","setuptools<58.0"]
+install_requires = [requests, "future==0.15.2"]
 
 
 # Don't import openpay module here, since deps may not be installed
 sys.path.insert(0, os.path.join(os.path.dirname(__file__), 'openpay'))
 from version import VERSION
 
 # Get simplejson if we don't already have json
```

