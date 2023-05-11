# Comparing `tmp/printername-0.0.4.tar.gz` & `tmp/printername-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printername-0.0.4.tar", last modified: Thu May 11 14:38:25 2023, max compression
+gzip compressed data, was "printername-0.0.5.tar", last modified: Thu May 11 14:42:42 2023, max compression
```

## Comparing `printername-0.0.4.tar` & `printername-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 14:38:25.546279 printername-0.0.4/
--rw-r--r--   0 vsts      (1001) docker     (123)      232 2023-05-11 14:38:25.546279 printername-0.0.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      985 2023-05-11 14:38:15.000000 printername-0.0.4/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 14:38:25.546279 printername-0.0.4/printername.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      232 2023-05-11 14:38:25.000000 printername-0.0.4/printername.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      191 2023-05-11 14:38:25.000000 printername-0.0.4/printername.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-11 14:38:25.000000 printername-0.0.4/printername.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-11 14:38:25.000000 printername-0.0.4/printername.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-11 14:38:25.546279 printername-0.0.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-11 14:38:15.000000 printername-0.0.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 14:38:25.546279 printername-0.0.4/test/
--rw-r--r--   0 vsts      (1001) docker     (123)       36 2023-05-11 14:38:15.000000 printername-0.0.4/test/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       74 2023-05-11 14:38:15.000000 printername-0.0.4/test/printer.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 14:42:42.234209 printername-0.0.5/
+-rw-r--r--   0 vsts      (1001) docker     (123)      232 2023-05-11 14:42:42.230209 printername-0.0.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      985 2023-05-11 14:42:38.000000 printername-0.0.5/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 14:42:42.230209 printername-0.0.5/printername.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      232 2023-05-11 14:42:42.000000 printername-0.0.5/printername.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      191 2023-05-11 14:42:42.000000 printername-0.0.5/printername.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-11 14:42:42.000000 printername-0.0.5/printername.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-11 14:42:42.000000 printername-0.0.5/printername.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-11 14:42:42.234209 printername-0.0.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-11 14:42:38.000000 printername-0.0.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 14:42:42.230209 printername-0.0.5/test/
+-rw-r--r--   0 vsts      (1001) docker     (123)       36 2023-05-11 14:42:38.000000 printername-0.0.5/test/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       74 2023-05-11 14:42:38.000000 printername-0.0.5/test/printer.py
```

### Comparing `printername-0.0.4/README.md` & `printername-0.0.5/README.md`

 * *Files identical despite different names*

