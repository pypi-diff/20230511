# Comparing `tmp/rgwadmin-2.4.1.tar.gz` & `tmp/rgwadmin-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgwadmin-2.4.1.tar", last modified: Fri Apr 14 14:23:51 2023, max compression
+gzip compressed data, was "rgwadmin-2.4.2.tar", last modified: Thu May 11 14:16:20 2023, max compression
```

## Comparing `rgwadmin-2.4.1.tar` & `rgwadmin-2.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.152035 rgwadmin-2.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    26443 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3359 2023-04-14 14:23:51.151035 rgwadmin-2.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.133035 rgwadmin-2.4.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.135034 rgwadmin-2.4.1/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/api.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.138035 rgwadmin-2.4.1/docs/source/apipages/
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/apipages/exceptions.rst
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/apipages/rgw.rst
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/apipages/user.rst
--rw-rw-rw-   0 root         (0) root         (0)     5460 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.139035 rgwadmin-2.4.1/docs/source/rgwadmin/
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/rgwadmin/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)    14356 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/docs/source/rgwadmin/user-guide.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.144035 rgwadmin-2.4.1/rgwadmin/
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/rgwadmin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2633 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/rgwadmin/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/rgwadmin/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    21420 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/rgwadmin/rgw.py
--rw-rw-rw-   0 root         (0) root         (0)     9589 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/rgwadmin/user.py
--rw-rw-rw-   0 root         (0) root         (0)     1042 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/rgwadmin/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.148035 rgwadmin-2.4.1/rgwadmin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3359 2023-04-14 14:23:51.000000 rgwadmin-2.4.1/rgwadmin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      695 2023-04-14 14:23:51.000000 rgwadmin-2.4.1/rgwadmin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 14:23:51.000000 rgwadmin-2.4.1/rgwadmin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 14:23:51.000000 rgwadmin-2.4.1/rgwadmin.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-14 14:23:51.000000 rgwadmin-2.4.1/rgwadmin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-14 14:23:51.000000 rgwadmin-2.4.1/rgwadmin.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 14:23:51.152035 rgwadmin-2.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1444 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:23:51.151035 rgwadmin-2.4.1/test/
--rwxrwxrwx   0 root         (0) root         (0)     2683 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/test/test_metadata.py
--rwxrwxrwx   0 root         (0) root         (0)     6327 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/test/test_rgw.py
--rwxrwxrwx   0 root         (0) root         (0)     1461 2023-04-14 14:23:42.000000 rgwadmin-2.4.1/test/test_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.251102 rgwadmin-2.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)    26443 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3359 2023-05-11 14:16:20.251102 rgwadmin-2.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.242102 rgwadmin-2.4.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.243101 rgwadmin-2.4.2/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/api.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.245102 rgwadmin-2.4.2/docs/source/apipages/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/apipages/exceptions.rst
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/apipages/rgw.rst
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/apipages/user.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5460 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.245102 rgwadmin-2.4.2/docs/source/rgwadmin/
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/rgwadmin/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14356 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/docs/source/rgwadmin/user-guide.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.247102 rgwadmin-2.4.2/rgwadmin/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/rgwadmin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/rgwadmin/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/rgwadmin/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    21585 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/rgwadmin/rgw.py
+-rw-rw-rw-   0 root         (0) root         (0)     9589 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/rgwadmin/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/rgwadmin/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.249101 rgwadmin-2.4.2/rgwadmin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3359 2023-05-11 14:16:20.000000 rgwadmin-2.4.2/rgwadmin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      695 2023-05-11 14:16:20.000000 rgwadmin-2.4.2/rgwadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 14:16:20.000000 rgwadmin-2.4.2/rgwadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 14:16:20.000000 rgwadmin-2.4.2/rgwadmin.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-11 14:16:20.000000 rgwadmin-2.4.2/rgwadmin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-11 14:16:20.000000 rgwadmin-2.4.2/rgwadmin.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 14:16:20.251102 rgwadmin-2.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:16:20.251102 rgwadmin-2.4.2/test/
+-rwxrwxrwx   0 root         (0) root         (0)     2683 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/test/test_metadata.py
+-rwxrwxrwx   0 root         (0) root         (0)     6327 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/test/test_rgw.py
+-rwxrwxrwx   0 root         (0) root         (0)     1461 2023-05-11 14:16:11.000000 rgwadmin-2.4.2/test/test_user.py
```

### Comparing `rgwadmin-2.4.1/LICENSE` & `rgwadmin-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/PKG-INFO` & `rgwadmin-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgwadmin
-Version: 2.4.1
+Version: 2.4.2
 Summary: Python Rados Gateway Admin API
 Home-page: https://github.com/UMIACS/rgwadmin
 Author: Derek Yarnell
 Author-email: derek@umiacs.umd.edu
 Maintainer: UMIACS Staff
 Maintainer-email: github@umiacs.umd.edu
 License: LGPL v2.1
```

### Comparing `rgwadmin-2.4.1/README.md` & `rgwadmin-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/docs/Makefile` & `rgwadmin-2.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/docs/make.bat` & `rgwadmin-2.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/docs/source/conf.py` & `rgwadmin-2.4.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/docs/source/rgwadmin/user-guide.rst` & `rgwadmin-2.4.2/docs/source/rgwadmin/user-guide.rst`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/rgwadmin/exceptions.py` & `rgwadmin-2.4.2/rgwadmin/exceptions.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/rgwadmin/rgw.py` & `rgwadmin-2.4.2/rgwadmin/rgw.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,20 @@
                       InternalError]:
                 if code == e.__name__:
                     raise e(j)
             raise RGWAdminException(code, raw=j)
 
     def request(self, method, request, headers: Optional[Dict] = None, data=None):
         url = '%s%s' % (self.get_base_url(), request)
+        # add host request header
+        if headers:
+            headers['host'] = self._server
+        else:
+            headers = {'host': self._server}
+        
         log.debug('URL: %s' % url)
         log.debug('Access Key: %s' % self._access_key)
         log.debug('Verify: %s  CA Bundle: %s' % (self._verify,
                                                  self._ca_bundle))
         try:
             if self._session:
                 # use connection pool
```

### Comparing `rgwadmin-2.4.1/rgwadmin/user.py` & `rgwadmin-2.4.2/rgwadmin/user.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/rgwadmin/utils.py` & `rgwadmin-2.4.2/rgwadmin/utils.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/rgwadmin.egg-info/PKG-INFO` & `rgwadmin-2.4.2/rgwadmin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgwadmin
-Version: 2.4.1
+Version: 2.4.2
 Summary: Python Rados Gateway Admin API
 Home-page: https://github.com/UMIACS/rgwadmin
 Author: Derek Yarnell
 Author-email: derek@umiacs.umd.edu
 Maintainer: UMIACS Staff
 Maintainer-email: github@umiacs.umd.edu
 License: LGPL v2.1
```

### Comparing `rgwadmin-2.4.1/rgwadmin.egg-info/SOURCES.txt` & `rgwadmin-2.4.2/rgwadmin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/setup.py` & `rgwadmin-2.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/test/test_metadata.py` & `rgwadmin-2.4.2/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/test/test_rgw.py` & `rgwadmin-2.4.2/test/test_rgw.py`

 * *Files identical despite different names*

### Comparing `rgwadmin-2.4.1/test/test_user.py` & `rgwadmin-2.4.2/test/test_user.py`

 * *Files identical despite different names*

