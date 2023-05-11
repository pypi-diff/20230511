# Comparing `tmp/cloudnetpy_qc-1.9.4.tar.gz` & `tmp/cloudnetpy_qc-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudnetpy_qc-1.9.4.tar", last modified: Mon May  8 12:52:23 2023, max compression
+gzip compressed data, was "cloudnetpy_qc-1.9.5.tar", last modified: Mon May  8 13:43:19 2023, max compression
```

## Comparing `cloudnetpy_qc-1.9.4.tar` & `cloudnetpy_qc-1.9.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:23.068998 cloudnetpy_qc-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 12:52:23.064998 cloudnetpy_qc-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:23.060998 cloudnetpy_qc-1.9.4/cloudnetpy_qc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:23.064998 cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/area-type-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)  4094783 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/cf-standard-name-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/data_quality_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/metadata_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/standardized-region-list.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20904 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30120 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:23.060998 cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 12:52:23.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-08 12:52:23.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:52:23.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 12:52:23.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 12:52:23.000000 cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 12:52:23.068998 cloudnetpy_qc-1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-08 12:52:12.000000 cloudnetpy_qc-1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:43:19.465463 cloudnetpy_qc-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 13:43:19.465463 cloudnetpy_qc-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:43:19.457463 cloudnetpy_qc-1.9.5/cloudnetpy_qc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:43:19.465463 cloudnetpy_qc-1.9.5/cloudnetpy_qc/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc/data/area-type-table.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  4094783 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc/data/cf-standard-name-table.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc/data/data_quality_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc/data/metadata_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc/data/standardized-region-list.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20904 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30120 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:43:19.457463 cloudnetpy_qc-1.9.5/cloudnetpy_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 13:43:19.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-08 13:43:19.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:43:19.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 13:43:19.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 13:43:19.000000 cloudnetpy_qc-1.9.5/cloudnetpy_qc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:43:19.465463 cloudnetpy_qc-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-08 13:42:53.000000 cloudnetpy_qc-1.9.5/setup.py
```

### Comparing `cloudnetpy_qc-1.9.4/LICENSE` & `cloudnetpy_qc-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.4/PKG-INFO` & `cloudnetpy_qc-1.9.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudnetpy_qc
-Version: 1.9.4
+Version: 1.9.5
 Summary: Quality control routines for CloudnetPy products
 Home-page: https://github.com/actris-cloudnet/cloudnetpy-qc
 Author: Finnish Meteorological Institute
 Author-email: actris-cloudnet@fmi.fi
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudnetpy_qc-1.9.4/README.md` & `cloudnetpy_qc-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/area-type-table.xml` & `cloudnetpy_qc-1.9.5/cloudnetpy_qc/data/area-type-table.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/cf-standard-name-table.xml` & `cloudnetpy_qc-1.9.5/cloudnetpy_qc/data/cf-standard-name-table.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/data_quality_config.ini` & `cloudnetpy_qc-1.9.5/cloudnetpy_qc/data/data_quality_config.ini`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.4/cloudnetpy_qc/data/standardized-region-list.xml` & `cloudnetpy_qc-1.9.5/cloudnetpy_qc/data/standardized-region-list.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.4/cloudnetpy_qc/quality.py` & `cloudnetpy_qc-1.9.5/cloudnetpy_qc/quality.py`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.4/cloudnetpy_qc/utils.py` & `cloudnetpy_qc-1.9.5/cloudnetpy_qc/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,10 +67,10 @@
 
 @lru_cache
 def fetch_pid(pid: str) -> dict:
     match = re.fullmatch(PID_FORMAT, pid)
     if match is None:
         raise ValueError("Invalid PID format")
     url = "https://hdl.handle.net/api/handles/" + match[1]
-    res = requests.get(url)
+    res = requests.get(url, timeout=30)
     res.raise_for_status()
     return res.json()
```

### Comparing `cloudnetpy_qc-1.9.4/cloudnetpy_qc/variables.py` & `cloudnetpy_qc-1.9.5/cloudnetpy_qc/variables.py`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/PKG-INFO` & `cloudnetpy_qc-1.9.5/cloudnetpy_qc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudnetpy-qc
-Version: 1.9.4
+Version: 1.9.5
 Summary: Quality control routines for CloudnetPy products
 Home-page: https://github.com/actris-cloudnet/cloudnetpy-qc
 Author: Finnish Meteorological Institute
 Author-email: actris-cloudnet@fmi.fi
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudnetpy_qc-1.9.4/cloudnetpy_qc.egg-info/SOURCES.txt` & `cloudnetpy_qc-1.9.5/cloudnetpy_qc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.4/setup.py` & `cloudnetpy_qc-1.9.5/setup.py`

 * *Files identical despite different names*

