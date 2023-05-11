# Comparing `tmp/qwc-services-core-1.3.8.tar.gz` & `tmp/qwc-services-core-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qwc-services-core-1.3.8.tar", last modified: Wed Apr 27 11:42:19 2022, max compression
+gzip compressed data, was "qwc-services-core-1.3.9.tar", last modified: Mon Jul 11 07:03:20 2022, max compression
```

## Comparing `qwc-services-core-1.3.8.tar` & `qwc-services-core-1.3.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 mwa       (1027) mwa       (1000)        0 2022-04-27 11:42:19.000000 qwc-services-core-1.3.8/
--rw-rw-r--   0 mwa       (1027) mwa       (1000)      802 2022-04-27 11:29:04.000000 qwc-services-core-1.3.8/README.md
-drwxrwxr-x   0 mwa       (1027) mwa       (1000)        0 2022-04-27 11:42:19.000000 qwc-services-core-1.3.8/qwc_services_core/
--rw-rw-r--   0 mwa       (1027) mwa       (1000)        0 2021-06-23 14:41:46.000000 qwc-services-core-1.3.8/qwc_services_core/__init__.py
--rw-rw-r--   0 mwa       (1027) mwa       (1000)     2164 2022-04-12 13:33:39.000000 qwc-services-core-1.3.8/qwc_services_core/jwt.py
--rw-rw-r--   0 mwa       (1027) mwa       (1000)     3605 2022-04-27 11:05:59.000000 qwc-services-core-1.3.8/qwc_services_core/runtime_config.py
--rw-rw-r--   0 mwa       (1027) mwa       (1000)     2240 2021-06-23 14:41:46.000000 qwc-services-core-1.3.8/qwc_services_core/api.py
--rw-rw-r--   0 mwa       (1027) mwa       (1000)     3198 2021-06-23 14:41:46.000000 qwc-services-core-1.3.8/qwc_services_core/cache.py
--rw-rw-r--   0 mwa       (1027) mwa       (1000)     1540 2021-06-23 14:41:46.000000 qwc-services-core-1.3.8/qwc_services_core/database.py
--rw-rw-r--   0 mwa       (1027) mwa       (1000)      442 2021-06-23 14:41:46.000000 qwc-services-core-1.3.8/qwc_services_core/app.py
--rw-rw-r--   0 mwa       (1027) mwa       (1000)    11331 2021-06-23 14:41:46.000000 qwc-services-core-1.3.8/qwc_services_core/permissions_reader.py
--rw-rw-r--   0 mwa       (1027) mwa       (1000)     6700 2022-04-27 11:23:37.000000 qwc-services-core-1.3.8/qwc_services_core/config_models.py
--rw-rw-r--   0 mwa       (1027) mwa       (1000)     1671 2022-04-12 13:33:39.000000 qwc-services-core-1.3.8/qwc_services_core/auth.py
--rw-rw-r--   0 mwa       (1027) mwa       (1000)     6004 2022-04-25 07:22:32.000000 qwc-services-core-1.3.8/qwc_services_core/tenant_handler.py
--rw-rw-r--   0 mwa       (1027) mwa       (1000)      686 2022-04-27 11:32:11.000000 qwc-services-core-1.3.8/setup.py
-drwxrwxr-x   0 mwa       (1027) mwa       (1000)        0 2022-04-27 11:42:19.000000 qwc-services-core-1.3.8/qwc_services_core.egg-info/
--rw-rw-r--   0 mwa       (1027) mwa       (1000)      517 2022-04-27 11:42:19.000000 qwc-services-core-1.3.8/qwc_services_core.egg-info/SOURCES.txt
--rw-rw-r--   0 mwa       (1027) mwa       (1000)       18 2022-04-27 11:42:19.000000 qwc-services-core-1.3.8/qwc_services_core.egg-info/top_level.txt
--rw-rw-r--   0 mwa       (1027) mwa       (1000)        1 2022-04-27 11:42:19.000000 qwc-services-core-1.3.8/qwc_services_core.egg-info/dependency_links.txt
--rw-rw-r--   0 mwa       (1027) mwa       (1000)      592 2022-04-27 11:42:19.000000 qwc-services-core-1.3.8/qwc_services_core.egg-info/PKG-INFO
--rw-rw-r--   0 mwa       (1027) mwa       (1000)       38 2022-04-27 11:42:19.000000 qwc-services-core-1.3.8/setup.cfg
--rw-rw-r--   0 mwa       (1027) mwa       (1000)      592 2022-04-27 11:42:19.000000 qwc-services-core-1.3.8/PKG-INFO
+drwxrwxr-x   0 sandro    (1000) sandro    (1000)        0 2022-07-11 07:03:20.519030 qwc-services-core-1.3.9/
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     1070 2020-11-04 16:28:43.000000 qwc-services-core-1.3.9/LICENSE
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      534 2022-07-11 07:03:20.519030 qwc-services-core-1.3.9/PKG-INFO
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      802 2022-01-12 17:20:48.000000 qwc-services-core-1.3.9/README.md
+drwxrwxr-x   0 sandro    (1000) sandro    (1000)        0 2022-07-11 07:03:20.518030 qwc-services-core-1.3.9/qwc_services_core/
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)        0 2020-11-04 16:28:43.000000 qwc-services-core-1.3.9/qwc_services_core/__init__.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     2240 2020-11-04 16:28:43.000000 qwc-services-core-1.3.9/qwc_services_core/api.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      442 2020-11-04 16:28:43.000000 qwc-services-core-1.3.9/qwc_services_core/app.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     1671 2021-12-17 11:31:10.000000 qwc-services-core-1.3.9/qwc_services_core/auth.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     3198 2020-11-04 16:28:43.000000 qwc-services-core-1.3.9/qwc_services_core/cache.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     6700 2022-07-01 09:33:49.000000 qwc-services-core-1.3.9/qwc_services_core/config_models.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     1540 2020-11-04 16:28:43.000000 qwc-services-core-1.3.9/qwc_services_core/database.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     2164 2022-04-08 19:56:44.000000 qwc-services-core-1.3.9/qwc_services_core/jwt.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)    11331 2021-12-17 11:31:10.000000 qwc-services-core-1.3.9/qwc_services_core/permissions_reader.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     3605 2022-07-01 09:33:49.000000 qwc-services-core-1.3.9/qwc_services_core/runtime_config.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     5724 2022-07-11 06:49:59.000000 qwc-services-core-1.3.9/qwc_services_core/tenant_handler.py
+drwxrwxr-x   0 sandro    (1000) sandro    (1000)        0 2022-07-11 07:03:20.519030 qwc-services-core-1.3.9/qwc_services_core.egg-info/
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      534 2022-07-11 07:03:19.000000 qwc-services-core-1.3.9/qwc_services_core.egg-info/PKG-INFO
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      525 2022-07-11 07:03:20.000000 qwc-services-core-1.3.9/qwc_services_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)        1 2022-07-11 07:03:20.000000 qwc-services-core-1.3.9/qwc_services_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)       18 2022-07-11 07:03:20.000000 qwc-services-core-1.3.9/qwc_services_core.egg-info/top_level.txt
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)       38 2022-07-11 07:03:20.519030 qwc-services-core-1.3.9/setup.cfg
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      686 2022-07-11 07:02:24.000000 qwc-services-core-1.3.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qwc-services-core-1.3.8/README.md` & `qwc-services-core-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `qwc-services-core-1.3.8/qwc_services_core/jwt.py` & `qwc-services-core-1.3.9/qwc_services_core/jwt.py`

 * *Files identical despite different names*

### Comparing `qwc-services-core-1.3.8/qwc_services_core/runtime_config.py` & `qwc-services-core-1.3.9/qwc_services_core/runtime_config.py`

 * *Files identical despite different names*

### Comparing `qwc-services-core-1.3.8/qwc_services_core/api.py` & `qwc-services-core-1.3.9/qwc_services_core/api.py`

 * *Files identical despite different names*

### Comparing `qwc-services-core-1.3.8/qwc_services_core/cache.py` & `qwc-services-core-1.3.9/qwc_services_core/cache.py`

 * *Files identical despite different names*

### Comparing `qwc-services-core-1.3.8/qwc_services_core/database.py` & `qwc-services-core-1.3.9/qwc_services_core/database.py`

 * *Files identical despite different names*

### Comparing `qwc-services-core-1.3.8/qwc_services_core/permissions_reader.py` & `qwc-services-core-1.3.9/qwc_services_core/permissions_reader.py`

 * *Files identical despite different names*

### Comparing `qwc-services-core-1.3.8/qwc_services_core/config_models.py` & `qwc-services-core-1.3.9/qwc_services_core/config_models.py`

 * *Files identical despite different names*

### Comparing `qwc-services-core-1.3.8/qwc_services_core/auth.py` & `qwc-services-core-1.3.9/qwc_services_core/auth.py`

 * *Files identical despite different names*

### Comparing `qwc-services-core-1.3.8/qwc_services_core/tenant_handler.py` & `qwc-services-core-1.3.9/qwc_services_core/tenant_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,37 +114,28 @@
 
 
 class TenantPrefixMiddleware:
     """WSGI middleware injecting tenant header in path"""
 
     def __init__(self, app, _header=None, _ignore_default=None):
         self.app = app
-        tenant_header = os.environ.get('TENANT_HEADER')
-        if tenant_header:
-            self.header = 'HTTP_' + tenant_header.upper()
-        else:
-            self.header = None
+        self.tenant_handler = TenantHandlerBase()
         self.service_prefix = os.environ.get(
             'QWC_SERVICE_PREFIX', '/').rstrip('/') + '/'
 
-    def request_tenant(self, environ):
-        if self.header:
-            return environ.get(self.header)
-        else:
-            return None
-
     def __call__(self, environ, start_response):
         # environ in request http://localhost:9090/base/pages/test.html?arg=1
         # /base is mountpoint (e.g. via WSGIScriptAlias)
         # 'REQUEST_URI': '/base/pages/test.html?arg=1'
         # 'SCRIPT_NAME': '/base'
         # 'PATH_INFO': '/pages/test.html'
         # 'QUERY_STRING': 'arg=1'
         # see also https://www.python.org/dev/peps/pep-3333/#environ-variables
-        tenant = self.request_tenant(environ)
+        tenant = self.tenant_handler.tenant()
+
         if tenant:
             prefix = self.service_prefix + tenant
             environ['SCRIPT_NAME'] = prefix + environ.get(
                 'SCRIPT_NAME', '')
         return self.app(environ, start_response)
```

### Comparing `qwc-services-core-1.3.8/setup.py` & `qwc-services-core-1.3.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 QWC Services Core
 =================
 Shared modules for QWC services.
 """
 
 setuptools.setup(
     name="qwc-services-core",
-    version="1.3.8",
+    version="1.3.9",
     author="Sourcepole AG",
     author_email="info@sourcepole.ch",
     description="Shared modules for QWC services",
     long_description=desc,
     long_description_content_type="text/x-rst",
     url="https://github.com/qwc-services/qwc-services-core",
     packages=setuptools.find_packages(),
```

### Comparing `qwc-services-core-1.3.8/qwc_services_core.egg-info/SOURCES.txt` & `qwc-services-core-1.3.9/qwc_services_core.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 qwc_services_core/__init__.py
 qwc_services_core/api.py
 qwc_services_core/app.py
 qwc_services_core/auth.py
 qwc_services_core/cache.py
```

