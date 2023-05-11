# Comparing `tmp/keyrock-core-2023.5.11.1117.tar.gz` & `tmp/keyrock-core-2023.5.7.1147.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyrock-core-2023.5.11.1117.tar", last modified: Thu May 11 11:17:34 2023, max compression
+gzip compressed data, was "keyrock-core-2023.5.7.1147.tar", last modified: Sun May  7 11:47:31 2023, max compression
```

## Comparing `keyrock-core-2023.5.11.1117.tar` & `keyrock-core-2023.5.7.1147.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:17:34.028392 keyrock-core-2023.5.11.1117/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 11:17:34.028392 keyrock-core-2023.5.11.1117/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:17:34.021058 keyrock-core-2023.5.11.1117/keyrock_core/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:17:34.023809 keyrock-core-2023.5.11.1117/keyrock_core/config_loader/
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/config_loader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5047 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/config_loader/config_loader.py
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/config_loader/test_config_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:17:34.024725 keyrock-core-2023.5.11.1117/keyrock_core/hash_util/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/hash_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/hash_util/hash_util.py
--rw-rw-rw-   0 root         (0) root         (0)     1144 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/hash_util/test_hash_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:17:34.025642 keyrock-core-2023.5.11.1117/keyrock_core/json_util/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/json_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4169 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/json_util/diff.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/json_util/encoders.py
--rw-rw-rw-   0 root         (0) root         (0)     6247 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/json_util/json_util.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/json_util/test_json_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:17:34.028392 keyrock-core-2023.5.11.1117/keyrock_core/sql_util/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/sql_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/sql_util/date_util.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/sql_util/misc_util.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/sql_util/query_util.py
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/keyrock_core/sql_util/test_sql_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 11:17:34.022892 keyrock-core-2023.5.11.1117/keyrock_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 11:17:34.000000 keyrock-core-2023.5.11.1117/keyrock_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      829 2023-05-11 11:17:34.000000 keyrock-core-2023.5.11.1117/keyrock_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 11:17:34.000000 keyrock-core-2023.5.11.1117/keyrock_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-11 11:17:34.000000 keyrock-core-2023.5.11.1117/keyrock_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 11:17:34.000000 keyrock-core-2023.5.11.1117/keyrock_core.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-11 11:17:17.000000 keyrock-core-2023.5.11.1117/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-11 11:17:34.029309 keyrock-core-2023.5.11.1117/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.027128 keyrock-core-2023.5.7.1147/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-07 11:47:31.027128 keyrock-core-2023.5.7.1147/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.018128 keyrock-core-2023.5.7.1147/keyrock_core/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.022128 keyrock-core-2023.5.7.1147/keyrock_core/config_loader/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/config_loader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5047 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/config_loader/config_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/config_loader/test_config_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.023128 keyrock-core-2023.5.7.1147/keyrock_core/hash_util/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/hash_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/hash_util/hash_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/hash_util/test_hash_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.025128 keyrock-core-2023.5.7.1147/keyrock_core/json_util/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/json_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4169 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/json_util/diff.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/json_util/encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)     6247 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/json_util/json_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/json_util/test_json_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.027128 keyrock-core-2023.5.7.1147/keyrock_core/sql_util/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/sql_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/sql_util/date_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      546 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/sql_util/misc_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/sql_util/query_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      960 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/keyrock_core/sql_util/test_sql_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.020128 keyrock-core-2023.5.7.1147/keyrock_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-07 11:47:31.000000 keyrock-core-2023.5.7.1147/keyrock_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      829 2023-05-07 11:47:31.000000 keyrock-core-2023.5.7.1147/keyrock_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 11:47:31.000000 keyrock-core-2023.5.7.1147/keyrock_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-07 11:47:31.000000 keyrock-core-2023.5.7.1147/keyrock_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-07 11:47:31.000000 keyrock-core-2023.5.7.1147/keyrock_core.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-07 11:47:14.000000 keyrock-core-2023.5.7.1147/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-07 11:47:31.028128 keyrock-core-2023.5.7.1147/setup.cfg
```

### Comparing `keyrock-core-2023.5.11.1117/keyrock_core/config_loader/config_loader.py` & `keyrock-core-2023.5.7.1147/keyrock_core/config_loader/config_loader.py`

 * *Files identical despite different names*

### Comparing `keyrock-core-2023.5.11.1117/keyrock_core/config_loader/test_config_loader.py` & `keyrock-core-2023.5.7.1147/keyrock_core/config_loader/test_config_loader.py`

 * *Files identical despite different names*

### Comparing `keyrock-core-2023.5.11.1117/keyrock_core/hash_util/hash_util.py` & `keyrock-core-2023.5.7.1147/keyrock_core/hash_util/hash_util.py`

 * *Files identical despite different names*

### Comparing `keyrock-core-2023.5.11.1117/keyrock_core/hash_util/test_hash_util.py` & `keyrock-core-2023.5.7.1147/keyrock_core/hash_util/test_hash_util.py`

 * *Files identical despite different names*

### Comparing `keyrock-core-2023.5.11.1117/keyrock_core/json_util/diff.py` & `keyrock-core-2023.5.7.1147/keyrock_core/json_util/diff.py`

 * *Files identical despite different names*

### Comparing `keyrock-core-2023.5.11.1117/keyrock_core/json_util/encoders.py` & `keyrock-core-2023.5.7.1147/keyrock_core/json_util/encoders.py`

 * *Files identical despite different names*

### Comparing `keyrock-core-2023.5.11.1117/keyrock_core/json_util/json_util.py` & `keyrock-core-2023.5.7.1147/keyrock_core/json_util/json_util.py`

 * *Files identical despite different names*

### Comparing `keyrock-core-2023.5.11.1117/keyrock_core/json_util/test_json_util.py` & `keyrock-core-2023.5.7.1147/keyrock_core/json_util/test_json_util.py`

 * *Files identical despite different names*

### Comparing `keyrock-core-2023.5.11.1117/keyrock_core/sql_util/misc_util.py` & `keyrock-core-2023.5.7.1147/keyrock_core/sql_util/misc_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 
 logger = logging.getLogger('')
 
 def parse_database_url(url):
     #
     # postgres://[user[:password]@][netloc][:port][/dbname][?param1=value1&...]
     #
-    if url is None:
-        return {}
-
     parsed = urlparse(url)
     result = {
         'type': parsed.scheme,
         'host': parsed.hostname,
         'port': parsed.port,
         'user': parsed.username,
         'pass': parsed.password,
```

### Comparing `keyrock-core-2023.5.11.1117/keyrock_core/sql_util/test_sql_util.py` & `keyrock-core-2023.5.7.1147/keyrock_core/sql_util/test_sql_util.py`

 * *Files identical despite different names*

### Comparing `keyrock-core-2023.5.11.1117/keyrock_core.egg-info/SOURCES.txt` & `keyrock-core-2023.5.7.1147/keyrock_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

