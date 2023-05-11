# Comparing `tmp/vsv-1.0.1.tar.gz` & `tmp/vsv-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsv-1.0.1.tar", last modified: Thu May 11 09:06:40 2023, max compression
+gzip compressed data, was "vsv-1.0.2.tar", last modified: Thu May 11 09:14:58 2023, max compression
```

## Comparing `vsv-1.0.1.tar` & `vsv-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 09:06:40.347004 vsv-1.0.1/
--rw-rw-rw-   0        0        0     1055 2023-05-11 08:57:14.000000 vsv-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0      166 2023-05-11 09:06:40.347004 vsv-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       49 2023-05-11 08:57:10.000000 vsv-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 09:06:40.347004 vsv-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      269 2023-05-11 09:06:33.000000 vsv-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 09:06:40.331377 vsv-1.0.1/vsv/
--rw-rw-rw-   0        0        0      164 2023-05-11 08:58:23.000000 vsv-1.0.1/vsv/__init__.py
--rw-rw-rw-   0        0        0      249 2023-05-11 08:50:07.000000 vsv-1.0.1/vsv/ddb.py
--rw-rw-rw-   0        0        0      946 2023-05-11 08:45:42.000000 vsv-1.0.1/vsv/dv.py
--rw-rw-rw-   0        0        0      278 2023-05-11 08:36:47.000000 vsv-1.0.1/vsv/idb.py
--rw-rw-rw-   0        0        0      284 2023-05-11 08:50:51.000000 vsv-1.0.1/vsv/qdb.py
--rw-rw-rw-   0        0        0      208 2023-05-11 08:40:36.000000 vsv-1.0.1/vsv/sdb.py
-drwxrwxrwx   0        0        0        0 2023-05-11 09:06:40.347004 vsv-1.0.1/vsv.egg-info/
--rw-rw-rw-   0        0        0      166 2023-05-11 09:06:40.000000 vsv-1.0.1/vsv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-11 09:06:40.000000 vsv-1.0.1/vsv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 09:06:40.000000 vsv-1.0.1/vsv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-11 09:06:40.000000 vsv-1.0.1/vsv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-11 09:06:40.000000 vsv-1.0.1/vsv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 09:14:58.162525 vsv-1.0.2/
+-rw-rw-rw-   0        0        0     1055 2023-05-11 08:57:14.000000 vsv-1.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0      166 2023-05-11 09:14:58.162525 vsv-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2023-05-11 08:57:10.000000 vsv-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 09:14:58.162525 vsv-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      269 2023-05-11 09:14:29.000000 vsv-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:14:58.162525 vsv-1.0.2/vsv/
+-rw-rw-rw-   0        0        0      164 2023-05-11 08:58:23.000000 vsv-1.0.2/vsv/__init__.py
+-rw-rw-rw-   0        0        0      249 2023-05-11 08:50:07.000000 vsv-1.0.2/vsv/ddb.py
+-rw-rw-rw-   0        0        0      946 2023-05-11 08:45:42.000000 vsv-1.0.2/vsv/dv.py
+-rw-rw-rw-   0        0        0      278 2023-05-11 09:14:05.000000 vsv-1.0.2/vsv/idb.py
+-rw-rw-rw-   0        0        0      284 2023-05-11 08:50:51.000000 vsv-1.0.2/vsv/qdb.py
+-rw-rw-rw-   0        0        0      208 2023-05-11 08:40:36.000000 vsv-1.0.2/vsv/sdb.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:14:58.162525 vsv-1.0.2/vsv.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-05-11 09:14:58.000000 vsv-1.0.2/vsv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-11 09:14:58.000000 vsv-1.0.2/vsv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 09:14:58.000000 vsv-1.0.2/vsv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-11 09:14:58.000000 vsv-1.0.2/vsv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-11 09:14:58.000000 vsv-1.0.2/vsv.egg-info/top_level.txt
```

### Comparing `vsv-1.0.1/LICENSE.md` & `vsv-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vsv-1.0.1/vsv/dv.py` & `vsv-1.0.2/vsv/dv.py`

 * *Files identical despite different names*

