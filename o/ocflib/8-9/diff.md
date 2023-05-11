# Comparing `tmp/ocflib-8.tar.gz` & `tmp/ocflib-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ocflib-8.tar", last modified: Thu Jan 22 19:07:34 2015, max compression
+gzip compressed data, was "dist/ocflib-9.tar", last modified: Sat Jan 24 00:50:13 2015, max compression
```

## Comparing `ocflib-8.tar` & `ocflib-9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ckuehl   (28460) ocf         (20)        0 2015-01-22 19:07:36.000000 ocflib-8/
--rw-r--r--   0 ckuehl   (28460) ocf         (20)      467 2015-01-22 19:07:34.000000 ocflib-8/setup.py
-drwxr-xr-x   0 ckuehl   (28460) ocf         (20)        0 2015-01-22 19:07:36.000000 ocflib-8/ocflib/
-drwxr-xr-x   0 ckuehl   (28460) ocf         (20)        0 2015-01-22 19:07:36.000000 ocflib-8/ocflib/account/
--rw-r--r--   0 ckuehl   (28460) ocf         (20)      384 2015-01-19 22:48:10.000000 ocflib-8/ocflib/account/ldap.py
--rw-r--r--   0 ckuehl   (28460) ocf         (20)     1481 2015-01-19 23:33:47.000000 ocflib-8/ocflib/account/search.py
--rw-r--r--   0 ckuehl   (28460) ocf         (20)        0 2015-01-17 08:01:24.000000 ocflib-8/ocflib/account/__init__.py
--rw-r--r--   0 ckuehl   (28460) ocf         (20)     4916 2015-01-19 23:38:35.000000 ocflib-8/ocflib/account/manage.py
--rw-r--r--   0 ckuehl   (28460) ocf         (20)     2003 2015-01-19 23:33:19.000000 ocflib-8/ocflib/account/validators.py
--rw-r--r--   0 ckuehl   (28460) ocf         (20)     1154 2015-01-21 23:29:04.000000 ocflib-8/ocflib/account/utils.py
-drwxr-xr-x   0 ckuehl   (28460) ocf         (20)        0 2015-01-22 19:07:36.000000 ocflib-8/ocflib/misc/
--rw-r--r--   0 ckuehl   (28460) ocf         (20)        0 2015-01-17 08:01:24.000000 ocflib-8/ocflib/misc/__init__.py
--rw-r--r--   0 ckuehl   (28460) ocf         (20)      215 2015-01-19 23:44:40.000000 ocflib-8/ocflib/misc/shell.py
--rw-r--r--   0 ckuehl   (28460) ocf         (20)     1054 2015-01-19 23:42:18.000000 ocflib-8/ocflib/misc/validators.py
--rw-r--r--   0 ckuehl   (28460) ocf         (20)     2306 2015-01-21 23:16:04.000000 ocflib-8/ocflib/constants.py
-drwxr-xr-x   0 ckuehl   (28460) ocf         (20)        0 2015-01-22 19:07:36.000000 ocflib-8/ocflib/calnet/
--rw-r--r--   0 ckuehl   (28460) ocf         (20)        0 2015-01-17 08:01:24.000000 ocflib-8/ocflib/calnet/__init__.py
--rw-r--r--   0 ckuehl   (28460) ocf         (20)     1876 2015-01-21 22:57:14.000000 ocflib-8/ocflib/calnet/utils.py
--rw-r--r--   0 ckuehl   (28460) ocf         (20)        0 2015-01-17 08:01:24.000000 ocflib-8/ocflib/__init__.py
--rw-r--r--   0 ckuehl   (28460) ocf         (20)       59 2015-01-22 19:07:36.000000 ocflib-8/setup.cfg
--rw-r--r--   0 ckuehl   (28460) ocf         (20)      263 2015-01-22 19:07:36.000000 ocflib-8/PKG-INFO
-drwxr-xr-x   0 ckuehl   (28460) ocf         (20)        0 2015-01-22 19:07:36.000000 ocflib-8/ocflib.egg-info/
--rw-r--r--   0 ckuehl   (28460) ocf         (20)        7 2015-01-22 19:07:35.000000 ocflib-8/ocflib.egg-info/top_level.txt
--rw-r--r--   0 ckuehl   (28460) ocf         (20)      469 2015-01-22 19:07:36.000000 ocflib-8/ocflib.egg-info/SOURCES.txt
--rw-r--r--   0 ckuehl   (28460) ocf         (20)       51 2015-01-22 19:07:35.000000 ocflib-8/ocflib.egg-info/requires.txt
--rw-r--r--   0 ckuehl   (28460) ocf         (20)        1 2015-01-22 19:07:35.000000 ocflib-8/ocflib.egg-info/dependency_links.txt
--rw-r--r--   0 ckuehl   (28460) ocf         (20)      263 2015-01-22 19:07:35.000000 ocflib-8/ocflib.egg-info/PKG-INFO
+drwxr-xr-x   0 ckuehl   (28460) ocf         (20)        0 2015-01-24 00:50:15.000000 ocflib-9/
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)      467 2015-01-24 00:50:12.000000 ocflib-9/setup.py
+drwxr-xr-x   0 ckuehl   (28460) ocf         (20)        0 2015-01-24 00:50:15.000000 ocflib-9/ocflib/
+drwxr-xr-x   0 ckuehl   (28460) ocf         (20)        0 2015-01-24 00:50:15.000000 ocflib-9/ocflib/account/
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)      384 2015-01-19 22:48:10.000000 ocflib-9/ocflib/account/ldap.py
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)     1481 2015-01-19 23:33:47.000000 ocflib-9/ocflib/account/search.py
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)        0 2015-01-17 08:01:24.000000 ocflib-9/ocflib/account/__init__.py
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)     4916 2015-01-19 23:38:35.000000 ocflib-9/ocflib/account/manage.py
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)     2003 2015-01-19 23:33:19.000000 ocflib-9/ocflib/account/validators.py
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)     1154 2015-01-21 23:29:04.000000 ocflib-9/ocflib/account/utils.py
+drwxr-xr-x   0 ckuehl   (28460) ocf         (20)        0 2015-01-24 00:50:15.000000 ocflib-9/ocflib/misc/
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)        0 2015-01-17 08:01:24.000000 ocflib-9/ocflib/misc/__init__.py
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)      215 2015-01-19 23:44:40.000000 ocflib-9/ocflib/misc/shell.py
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)     1054 2015-01-19 23:42:18.000000 ocflib-9/ocflib/misc/validators.py
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)     2293 2015-01-24 00:49:39.000000 ocflib-9/ocflib/constants.py
+drwxr-xr-x   0 ckuehl   (28460) ocf         (20)        0 2015-01-24 00:50:15.000000 ocflib-9/ocflib/calnet/
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)        0 2015-01-17 08:01:24.000000 ocflib-9/ocflib/calnet/__init__.py
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)     1876 2015-01-21 22:57:14.000000 ocflib-9/ocflib/calnet/utils.py
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)        0 2015-01-17 08:01:24.000000 ocflib-9/ocflib/__init__.py
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)       59 2015-01-24 00:50:15.000000 ocflib-9/setup.cfg
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)      263 2015-01-24 00:50:15.000000 ocflib-9/PKG-INFO
+drwxr-xr-x   0 ckuehl   (28460) ocf         (20)        0 2015-01-24 00:50:15.000000 ocflib-9/ocflib.egg-info/
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)        7 2015-01-24 00:50:14.000000 ocflib-9/ocflib.egg-info/top_level.txt
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)      469 2015-01-24 00:50:15.000000 ocflib-9/ocflib.egg-info/SOURCES.txt
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)       51 2015-01-24 00:50:14.000000 ocflib-9/ocflib.egg-info/requires.txt
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)        1 2015-01-24 00:50:14.000000 ocflib-9/ocflib.egg-info/dependency_links.txt
+-rw-r--r--   0 ckuehl   (28460) ocf         (20)      263 2015-01-24 00:50:14.000000 ocflib-9/ocflib.egg-info/PKG-INFO
```

### Comparing `ocflib-8/ocflib/account/search.py` & `ocflib-9/ocflib/account/search.py`

 * *Files identical despite different names*

### Comparing `ocflib-8/ocflib/account/manage.py` & `ocflib-9/ocflib/account/manage.py`

 * *Files identical despite different names*

### Comparing `ocflib-8/ocflib/account/validators.py` & `ocflib-9/ocflib/account/validators.py`

 * *Files identical despite different names*

### Comparing `ocflib-8/ocflib/account/utils.py` & `ocflib-9/ocflib/account/utils.py`

 * *Files identical despite different names*

### Comparing `ocflib-8/ocflib/misc/validators.py` & `ocflib-9/ocflib/misc/validators.py`

 * *Files identical despite different names*

### Comparing `ocflib-8/ocflib/constants.py` & `ocflib-9/ocflib/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     'dump',
     'dumper',
     'epidemic',
     'games',
     'gm',
     'gnats',
     'groups',
-    'guser',
     'help',
     'hostmaster',
     'irc',
     'jabber',
     'libuuid',
     'list',
     'logjam',
```

### Comparing `ocflib-8/ocflib/calnet/utils.py` & `ocflib-9/ocflib/calnet/utils.py`

 * *Files identical despite different names*

