# Comparing `tmp/tera-toolbox-0.0.4.tar.gz` & `tmp/tera-toolbox-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tera-toolbox-0.0.4.tar", last modified: Fri May  5 22:01:53 2023, max compression
+gzip compressed data, was "tera-toolbox-0.0.5.tar", last modified: Thu May 11 21:01:33 2023, max compression
```

## Comparing `tera-toolbox-0.0.4.tar` & `tera-toolbox-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 22:01:53.139336 tera-toolbox-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-05 22:01:53.139336 tera-toolbox-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-05 22:01:42.000000 tera-toolbox-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 22:01:53.139336 tera-toolbox-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-05 22:01:42.000000 tera-toolbox-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 22:01:53.139336 tera-toolbox-0.0.4/tera_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-05 22:01:53.000000 tera-toolbox-0.0.4/tera_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      290 2023-05-05 22:01:53.000000 tera-toolbox-0.0.4/tera_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 22:01:53.000000 tera-toolbox-0.0.4/tera_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-05 22:01:53.000000 tera-toolbox-0.0.4/tera_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-05 22:01:53.000000 tera-toolbox-0.0.4/tera_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 22:01:53.139336 tera-toolbox-0.0.4/toolbox/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-05 22:01:42.000000 tera-toolbox-0.0.4/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-05-05 22:01:42.000000 tera-toolbox-0.0.4/toolbox/data.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-05 22:01:42.000000 tera-toolbox-0.0.4/toolbox/stats.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-05-05 22:01:42.000000 tera-toolbox-0.0.4/toolbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-05 22:01:42.000000 tera-toolbox-0.0.4/toolbox/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 21:01:33.285327 tera-toolbox-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-11 21:01:33.285327 tera-toolbox-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 21:01:33.285327 tera-toolbox-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 21:01:33.285327 tera-toolbox-0.0.5/tera_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-11 21:01:33.000000 tera-toolbox-0.0.5/tera_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-05-11 21:01:33.000000 tera-toolbox-0.0.5/tera_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 21:01:33.000000 tera-toolbox-0.0.5/tera_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-11 21:01:33.000000 tera-toolbox-0.0.5/tera_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-11 21:01:33.000000 tera-toolbox-0.0.5/tera_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 21:01:33.285327 tera-toolbox-0.0.5/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/toolbox/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/toolbox/stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/toolbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-11 21:01:23.000000 tera-toolbox-0.0.5/toolbox/version.py
```

### Comparing `tera-toolbox-0.0.4/setup.py` & `tera-toolbox-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `tera-toolbox-0.0.4/toolbox/utils.py` & `tera-toolbox-0.0.5/toolbox/utils.py`

 * *Files identical despite different names*

