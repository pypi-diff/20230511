# Comparing `tmp/hakai_api-1.4.0.tar.gz` & `tmp/hakai_api-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hakai_api-1.4.0.tar", last modified: Tue May  2 23:44:24 2023, max compression
+gzip compressed data, was "hakai_api-1.4.1.tar", last modified: Wed May 10 16:36:23 2023, max compression
```

## Comparing `hakai_api-1.4.0.tar` & `hakai_api-1.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:44:24.940628 hakai_api-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-02 23:44:24.940628 hakai_api-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-02 23:44:11.000000 hakai_api-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:44:24.936628 hakai_api-1.4.0/hakai_api/
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-02 23:44:11.000000 hakai_api-1.4.0/hakai_api/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-02 23:44:11.000000 hakai_api-1.4.0/hakai_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:44:24.936628 hakai_api-1.4.0/hakai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-02 23:44:24.000000 hakai_api-1.4.0/hakai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 23:44:24.000000 hakai_api-1.4.0/hakai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 23:44:24.000000 hakai_api-1.4.0/hakai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-02 23:44:24.000000 hakai_api-1.4.0/hakai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 23:44:24.000000 hakai_api-1.4.0/hakai_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 23:44:24.940628 hakai_api-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 23:44:11.000000 hakai_api-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:36:23.969516 hakai_api-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-10 16:36:23.969516 hakai_api-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-10 16:36:11.000000 hakai_api-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:36:23.969516 hakai_api-1.4.1/hakai_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-10 16:36:11.000000 hakai_api-1.4.1/hakai_api/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 16:36:11.000000 hakai_api-1.4.1/hakai_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:36:23.969516 hakai_api-1.4.1/hakai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-10 16:36:23.000000 hakai_api-1.4.1/hakai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-10 16:36:23.000000 hakai_api-1.4.1/hakai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:36:23.000000 hakai_api-1.4.1/hakai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 16:36:23.000000 hakai_api-1.4.1/hakai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 16:36:23.000000 hakai_api-1.4.1/hakai_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:36:23.969516 hakai_api-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-10 16:36:11.000000 hakai_api-1.4.1/setup.py
```

### Comparing `hakai_api-1.4.0/PKG-INFO` & `hakai_api-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakai_api
-Version: 1.4.0
+Version: 1.4.1
 Summary: Get Hakai database resources using http calls
 Home-page: https://github.com/HakaiInstitute/hakai-api-client-python
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `hakai_api-1.4.0/README.md` & `hakai_api-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `hakai_api-1.4.0/hakai_api/Client.py` & `hakai_api-1.4.1/hakai_api/Client.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,17 +101,17 @@
             now = int(
                 (
                         mktime(datetime.now().timetuple())
                         + datetime.now().microsecond / 1000000.0
                 )
             )  # utc timestamp
 
-            if now > expires_at:
-                os.remove(cls._credentials_file)
-                return False
+        if now > expires_at:
+            cls.reset_credentials()
+            return False
 
         return True
 
     @classmethod
     def _get_credentials_from_file(cls) -> Dict:
         """Get user credentials from a cached file."""
         with open(cls._credentials_file, "rb") as infile:
```

### Comparing `hakai_api-1.4.0/hakai_api.egg-info/PKG-INFO` & `hakai_api-1.4.1/hakai_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakai-api
-Version: 1.4.0
+Version: 1.4.1
 Summary: Get Hakai database resources using http calls
 Home-page: https://github.com/HakaiInstitute/hakai-api-client-python
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `hakai_api-1.4.0/setup.py` & `hakai_api-1.4.1/setup.py`

 * *Files identical despite different names*

