# Comparing `tmp/printername-0.0.2.tar.gz` & `tmp/printername-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printername-0.0.2.tar", last modified: Wed Apr 26 07:25:07 2023, max compression
+gzip compressed data, was "printername-0.0.3.tar", last modified: Thu May 11 14:33:02 2023, max compression
```

## Comparing `printername-0.0.2.tar` & `printername-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 07:25:07.327957 printername-0.0.2/
--rw-r--r--   0 vsts      (1001) docker     (123)      232 2023-04-26 07:25:07.327957 printername-0.0.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      985 2023-04-26 07:24:58.000000 printername-0.0.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 07:25:07.327957 printername-0.0.2/printername.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      232 2023-04-26 07:25:07.000000 printername-0.0.2/printername.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      191 2023-04-26 07:25:07.000000 printername-0.0.2/printername.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-26 07:25:07.000000 printername-0.0.2/printername.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-04-26 07:25:07.000000 printername-0.0.2/printername.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-26 07:25:07.327957 printername-0.0.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-04-26 07:24:58.000000 printername-0.0.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 07:25:07.327957 printername-0.0.2/test/
--rw-r--r--   0 vsts      (1001) docker     (123)       36 2023-04-26 07:24:58.000000 printername-0.0.2/test/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       74 2023-04-26 07:24:58.000000 printername-0.0.2/test/printer.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 14:33:02.474143 printername-0.0.3/
+-rw-r--r--   0 vsts      (1001) docker     (123)      232 2023-05-11 14:33:02.474143 printername-0.0.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      985 2023-05-11 14:32:52.000000 printername-0.0.3/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 14:33:02.474143 printername-0.0.3/printername.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      232 2023-05-11 14:33:02.000000 printername-0.0.3/printername.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      191 2023-05-11 14:33:02.000000 printername-0.0.3/printername.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-11 14:33:02.000000 printername-0.0.3/printername.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-11 14:33:02.000000 printername-0.0.3/printername.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-11 14:33:02.474143 printername-0.0.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-11 14:32:52.000000 printername-0.0.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 14:33:02.474143 printername-0.0.3/test/
+-rw-r--r--   0 vsts      (1001) docker     (123)       36 2023-05-11 14:32:52.000000 printername-0.0.3/test/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       74 2023-05-11 14:32:52.000000 printername-0.0.3/test/printer.py
```

### Comparing `printername-0.0.2/README.md` & `printername-0.0.3/README.md`

 * *Files identical despite different names*

