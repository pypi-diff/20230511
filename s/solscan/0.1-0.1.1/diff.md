# Comparing `tmp/solscan-0.1.tar.gz` & `tmp/solscan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solscan-0.1.tar", last modified: Thu May 11 06:23:20 2023, max compression
+gzip compressed data, was "solscan-0.1.1.tar", last modified: Thu May 11 06:44:40 2023, max compression
```

## Comparing `solscan-0.1.tar` & `solscan-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 06:23:20.718789 solscan-0.1/
--rw-r--r--   0 manosriram   (501) staff       (20)      240 2023-05-11 06:23:20.718667 solscan-0.1/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      638 2023-05-05 09:07:33.000000 solscan-0.1/README.md
--rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-11 06:23:20.718821 solscan-0.1/setup.cfg
--rw-r--r--   0 manosriram   (501) staff       (20)      727 2023-05-09 11:32:11.000000 solscan-0.1/setup.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 06:23:20.717903 solscan-0.1/solscan/
--rw-r--r--   0 manosriram   (501) staff       (20)     3505 2023-05-11 06:09:17.000000 solscan-0.1/solscan/__init__.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1602 2023-05-11 06:09:28.000000 solscan-0.1/solscan/config.py
--rw-r--r--   0 manosriram   (501) staff       (20)       57 2023-05-11 05:17:41.000000 solscan-0.1/solscan/constants.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1345 2023-05-11 06:09:40.000000 solscan-0.1/solscan/exceptions.py
--rw-r--r--   0 manosriram   (501) staff       (20)      905 2023-05-11 06:10:56.000000 solscan-0.1/solscan/lang.py
--rw-r--r--   0 manosriram   (501) staff       (20)     2925 2023-05-11 06:11:04.000000 solscan-0.1/solscan/scan.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 06:23:20.718520 solscan-0.1/solscan.egg-info/
--rw-r--r--   0 manosriram   (501) staff       (20)      240 2023-05-11 06:23:20.000000 solscan-0.1/solscan.egg-info/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      319 2023-05-11 06:23:20.000000 solscan-0.1/solscan.egg-info/SOURCES.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-05-11 06:23:20.000000 solscan-0.1/solscan.egg-info/dependency_links.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       53 2023-05-11 06:23:20.000000 solscan-0.1/solscan.egg-info/entry_points.txt
--rw-r--r--   0 manosriram   (501) staff       (20)      138 2023-05-11 06:23:20.000000 solscan-0.1/solscan.egg-info/requires.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        8 2023-05-11 06:23:20.000000 solscan-0.1/solscan.egg-info/top_level.txt
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 06:44:40.604719 solscan-0.1.1/
+-rw-r--r--   0 manosriram   (501) staff       (20)      242 2023-05-11 06:44:40.604597 solscan-0.1.1/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      798 2023-05-11 06:27:08.000000 solscan-0.1.1/README.md
+-rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-05-11 06:44:40.604758 solscan-0.1.1/setup.cfg
+-rw-r--r--   0 manosriram   (501) staff       (20)     1120 2023-05-11 06:44:34.000000 solscan-0.1.1/setup.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 06:44:40.603715 solscan-0.1.1/solscan/
+-rw-r--r--   0 manosriram   (501) staff       (20)     3489 2023-05-11 06:31:48.000000 solscan-0.1.1/solscan/__init__.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1784 2023-05-11 06:40:08.000000 solscan-0.1.1/solscan/config.py
+-rw-r--r--   0 manosriram   (501) staff       (20)       57 2023-05-11 05:17:41.000000 solscan-0.1.1/solscan/constants.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1337 2023-05-11 06:31:57.000000 solscan-0.1.1/solscan/exceptions.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      897 2023-05-11 06:31:59.000000 solscan-0.1.1/solscan/lang.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     2901 2023-05-11 06:32:06.000000 solscan-0.1.1/solscan/scan.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-05-11 06:44:40.604428 solscan-0.1.1/solscan.egg-info/
+-rw-r--r--   0 manosriram   (501) staff       (20)      242 2023-05-11 06:44:40.000000 solscan-0.1.1/solscan.egg-info/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      319 2023-05-11 06:44:40.000000 solscan-0.1.1/solscan.egg-info/SOURCES.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-05-11 06:44:40.000000 solscan-0.1.1/solscan.egg-info/dependency_links.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       53 2023-05-11 06:44:40.000000 solscan-0.1.1/solscan.egg-info/entry_points.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)      375 2023-05-11 06:44:40.000000 solscan-0.1.1/solscan.egg-info/requires.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        8 2023-05-11 06:44:40.000000 solscan-0.1.1/solscan.egg-info/top_level.txt
```

### Comparing `solscan-0.1/solscan/__init__.py` & `solscan-0.1.1/solscan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 
-from solscan.config import Config
-from solscan.scan import Scan
+from config import Config
+from scan import Scan
 
 """
     each command is mapped to @config.command()
     commands can be grouped. a group can be created by mapping the method to @config.group()
 """
 
 # base group. under which all other subcommands go.
```

### Comparing `solscan-0.1/solscan/config.py` & `solscan-0.1.1/solscan/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from pathlib import Path
 from ruamel.yaml import YAML
 import click
 
-from solscan.exceptions import TokenNotFound
+from exceptions import TokenNotFound
 
 SOLSCAN_ENV_PATH = f"{str(Path.home())}/solscan.yml"
 
 class Config:
     @staticmethod
     def load_yaml():
-        with open(SOLSCAN_ENV_PATH, 'r') as f:
-            yaml = YAML()
-            generated = yaml.load_all(f)
-            result = {}
-            for x in generated:
-                result = x
-            
-            return result
+        try:
+            with open(SOLSCAN_ENV_PATH, 'r') as f:
+                yaml = YAML()
+                generated = yaml.load_all(f)
+                result = {}
+                for x in generated:
+                    result = x
+                
+                return result
+        except IOError:
+            _ = open(SOLSCAN_ENV_PATH, 'w')
+            return {"version": "0.1", "token": None, "error_language": None}
 
     @staticmethod
     def get_config_value(key):
         return Config.load_yaml().get(key, None)
 
     @staticmethod
     def get_config_path():
```

### Comparing `solscan-0.1/solscan/exceptions.py` & `solscan-0.1.1/solscan/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from loguru import logger
 
-from solscan.lang import ErrorLanguageMapper
+from lang import ErrorLanguageMapper
 
 class TokenNotFound(Exception):
     @staticmethod
     def get_err_code():
         err_code = "ERR_1002"
         return err_code
```

### Comparing `solscan-0.1/solscan/lang.py` & `solscan-0.1.1/solscan/lang.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from deep_translator import GoogleTranslator
-import solscan.config as config
+import config as config
 
 """
     translates error message to specified language in constants.py (ERROR_LANGUAGE_CODE var).
     both the key and value is translated and returned.
     default language is English.
 """
 class ErrorLanguageMapper:
```

### Comparing `solscan-0.1/solscan/scan.py` & `solscan-0.1.1/solscan/scan.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from solscan.config import Config
+from config import Config
 
 import requests
 import click
 from loguru import logger
 
-from solscan.exceptions import ScanFailed, HostNotReachable
-from solscan.constants import HOST
+from exceptions import ScanFailed, HostNotReachable
+from constants import HOST
 
 class Scan:
 
     @property
     def project_scan_host_url(self):
         return f"{HOST}/api-project-scan/"
```

