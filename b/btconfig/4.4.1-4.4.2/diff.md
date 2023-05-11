# Comparing `tmp/btconfig-4.4.1.tar.gz` & `tmp/btconfig-4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btconfig-4.4.1.tar", last modified: Thu May 11 11:54:53 2023, max compression
+gzip compressed data, was "btconfig-4.4.2.tar", last modified: Thu May 11 11:57:32 2023, max compression
```

## Comparing `btconfig-4.4.1.tar` & `btconfig-4.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:54:53.279791 btconfig-4.4.1/
--rw-r--r--   0 etejeda    (501) staff       (20)     1311 2023-01-09 20:02:16.000000 btconfig-4.4.1/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-01-09 20:02:16.000000 btconfig-4.4.1/AUTHORS.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-01-09 20:02:16.000000 btconfig-4.4.1/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)      344 2023-01-09 20:02:16.000000 btconfig-4.4.1/MANIFEST.in
--rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-05-11 11:54:53.280046 btconfig-4.4.1/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     3132 2023-05-11 11:53:49.000000 btconfig-4.4.1/README.md
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:54:53.274939 btconfig-4.4.1/btconfig/
--rw-r--r--   0 etejeda    (501) staff       (20)     1279 2023-05-11 11:53:08.000000 btconfig-4.4.1/btconfig/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3790 2023-05-11 11:53:07.000000 btconfig-4.4.1/btconfig/configloader.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3217 2023-05-11 11:53:07.000000 btconfig-4.4.1/btconfig/configutils.py
--rw-r--r--   0 etejeda    (501) staff       (20)      813 2023-01-09 20:02:16.000000 btconfig-4.4.1/btconfig/logger.py
--rw-r--r--   0 etejeda    (501) staff       (20)     4576 2023-05-11 11:53:09.000000 btconfig-4.4.1/btconfig/superconf.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:54:53.276502 btconfig-4.4.1/btconfig.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-05-11 11:54:53.000000 btconfig-4.4.1/btconfig.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      604 2023-05-11 11:54:53.000000 btconfig-4.4.1/btconfig.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:54:53.000000 btconfig-4.4.1/btconfig.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:54:53.000000 btconfig-4.4.1/btconfig.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)       78 2023-05-11 11:54:53.000000 btconfig-4.4.1/btconfig.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        9 2023-05-11 11:54:53.000000 btconfig-4.4.1/btconfig.egg-info/top_level.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:54:53.279348 btconfig-4.4.1/examples/
--rw-r--r--   0 etejeda    (501) staff       (20)     3045 2023-05-11 11:53:23.000000 btconfig-4.4.1/examples/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)      157 2023-05-11 11:53:25.000000 btconfig-4.4.1/examples/example1.py
--rw-r--r--   0 etejeda    (501) staff       (20)      170 2023-05-11 11:53:22.000000 btconfig-4.4.1/examples/example2.py
--rw-r--r--   0 etejeda    (501) staff       (20)      160 2023-05-11 11:53:23.000000 btconfig-4.4.1/examples/example3.py
--rw-r--r--   0 etejeda    (501) staff       (20)      189 2023-05-11 11:53:24.000000 btconfig-4.4.1/examples/example4.py
--rw-r--r--   0 etejeda    (501) staff       (20)       54 2023-01-09 20:02:16.000000 btconfig-4.4.1/examples/myconfig1.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      234 2023-01-09 20:02:16.000000 btconfig-4.4.1/examples/myconfig2.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      435 2023-01-09 20:02:16.000000 btconfig-4.4.1/examples/myconfig3.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      208 2023-01-09 20:02:16.000000 btconfig-4.4.1/examples/myconfig4.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-01-09 20:02:16.000000 btconfig-4.4.1/requirements.txt
--rw-r--r--   0 etejeda    (501) staff       (20)     1074 2023-05-11 11:54:53.281051 btconfig-4.4.1/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-01-09 20:02:16.000000 btconfig-4.4.1/setup.py
--rw-r--r--   0 etejeda    (501) staff       (20)      248 2023-05-11 11:54:41.000000 btconfig-4.4.1/test.py
--rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-01-09 20:02:16.000000 btconfig-4.4.1/tox.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:57:32.923688 btconfig-4.4.2/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1311 2023-01-09 20:02:16.000000 btconfig-4.4.2/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-01-09 20:02:16.000000 btconfig-4.4.2/AUTHORS.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-01-09 20:02:16.000000 btconfig-4.4.2/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)      344 2023-01-09 20:02:16.000000 btconfig-4.4.2/MANIFEST.in
+-rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-05-11 11:57:32.923898 btconfig-4.4.2/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     3132 2023-05-11 11:53:49.000000 btconfig-4.4.2/README.md
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:57:32.918048 btconfig-4.4.2/btconfig/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1267 2023-05-11 11:55:36.000000 btconfig-4.4.2/btconfig/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3790 2023-05-11 11:53:07.000000 btconfig-4.4.2/btconfig/configloader.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3217 2023-05-11 11:53:07.000000 btconfig-4.4.2/btconfig/configutils.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      813 2023-01-09 20:02:16.000000 btconfig-4.4.2/btconfig/logger.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     4576 2023-05-11 11:53:09.000000 btconfig-4.4.2/btconfig/superconf.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:57:32.919885 btconfig-4.4.2/btconfig.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-05-11 11:57:32.000000 btconfig-4.4.2/btconfig.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      604 2023-05-11 11:57:32.000000 btconfig-4.4.2/btconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:57:32.000000 btconfig-4.4.2/btconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:54:53.000000 btconfig-4.4.2/btconfig.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)       78 2023-05-11 11:57:32.000000 btconfig-4.4.2/btconfig.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        9 2023-05-11 11:57:32.000000 btconfig-4.4.2/btconfig.egg-info/top_level.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:57:32.923300 btconfig-4.4.2/examples/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3045 2023-05-11 11:53:23.000000 btconfig-4.4.2/examples/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)      157 2023-05-11 11:53:25.000000 btconfig-4.4.2/examples/example1.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      170 2023-05-11 11:53:22.000000 btconfig-4.4.2/examples/example2.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      160 2023-05-11 11:53:23.000000 btconfig-4.4.2/examples/example3.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      189 2023-05-11 11:53:24.000000 btconfig-4.4.2/examples/example4.py
+-rw-r--r--   0 etejeda    (501) staff       (20)       54 2023-01-09 20:02:16.000000 btconfig-4.4.2/examples/myconfig1.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      234 2023-01-09 20:02:16.000000 btconfig-4.4.2/examples/myconfig2.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      435 2023-01-09 20:02:16.000000 btconfig-4.4.2/examples/myconfig3.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      208 2023-01-09 20:02:16.000000 btconfig-4.4.2/examples/myconfig4.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-01-09 20:02:16.000000 btconfig-4.4.2/requirements.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)     1074 2023-05-11 11:57:32.924714 btconfig-4.4.2/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-01-09 20:02:16.000000 btconfig-4.4.2/setup.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      248 2023-05-11 11:54:41.000000 btconfig-4.4.2/test.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-01-09 20:02:16.000000 btconfig-4.4.2/tox.ini
```

### Comparing `btconfig-4.4.1/.gitignore` & `btconfig-4.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.1/LICENSE` & `btconfig-4.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.1/PKG-INFO` & `btconfig-4.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btconfig
-Version: 4.4.1
+Version: 4.4.2
 Summary: Module for reading configuration files
 Home-page: https://github.com/berttejeda/bert.config
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btconfig-4.4.1/README.md` & `btconfig-4.4.2/README.md`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.1/btconfig/__init__.py` & `btconfig-4.4.2/btconfig/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from btconfig.logger import Logger
 import os
 from btconfig.superconf import SuperDuperConfig
-from bertdotwebadapter import WebAdapter
+from btweb import WebAdapter
 
 # Setup Logging
 logger = Logger(is_main_logger=True).init_logger(__name__)
 
 class Config(SuperDuperConfig):
 
   def __init__(self, **kwargs):
```

### Comparing `btconfig-4.4.1/btconfig/configloader.py` & `btconfig-4.4.2/btconfig/configloader.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.1/btconfig/configutils.py` & `btconfig-4.4.2/btconfig/configutils.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.1/btconfig/logger.py` & `btconfig-4.4.2/btconfig/logger.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.1/btconfig/superconf.py` & `btconfig-4.4.2/btconfig/superconf.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.1/btconfig.egg-info/PKG-INFO` & `btconfig-4.4.2/btconfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btconfig
-Version: 4.4.1
+Version: 4.4.2
 Summary: Module for reading configuration files
 Home-page: https://github.com/berttejeda/bert.config
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btconfig-4.4.1/btconfig.egg-info/SOURCES.txt` & `btconfig-4.4.2/btconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.1/examples/README.md` & `btconfig-4.4.2/examples/README.md`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.1/setup.cfg` & `btconfig-4.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = btconfig
 author = Engelbert Tejeda
 author_email = berttejeda@gmail.com
 description = Module for reading configuration files
-version = 4.4.1
+version = 4.4.2
 url = https://github.com/berttejeda/bert.config
 keywords = 
 	yaml
 	configuration
 	config
 	file
 	python
```

