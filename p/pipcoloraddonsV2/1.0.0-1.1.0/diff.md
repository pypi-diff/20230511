# Comparing `tmp/pipcoloraddonsV2-1.0.0.tar.gz` & `tmp/pipcoloraddonsV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcoloraddonsV2-1.0.0.tar", last modified: Thu May 11 10:30:11 2023, max compression
+gzip compressed data, was "pipcoloraddonsV2-1.1.0.tar", last modified: Thu May 11 10:32:21 2023, max compression
```

## Comparing `pipcoloraddonsV2-1.0.0.tar` & `pipcoloraddonsV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:30:11.331672 pipcoloraddonsV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-11 10:30:11.331672 pipcoloraddonsV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:30:11.331672 pipcoloraddonsV2-1.0.0/pipcoloraddonsV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 10:30:11.000000 pipcoloraddonsV2-1.0.0/pipcoloraddonsV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:30:11.331672 pipcoloraddonsV2-1.0.0/pipcoloraddonsV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-11 10:30:11.000000 pipcoloraddonsV2-1.0.0/pipcoloraddonsV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-11 10:30:11.000000 pipcoloraddonsV2-1.0.0/pipcoloraddonsV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 10:30:11.000000 pipcoloraddonsV2-1.0.0/pipcoloraddonsV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-11 10:30:11.000000 pipcoloraddonsV2-1.0.0/pipcoloraddonsV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 10:30:11.331672 pipcoloraddonsV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      562 2023-05-11 10:30:11.000000 pipcoloraddonsV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:32:21.958059 pipcoloraddonsV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-11 10:32:21.954059 pipcoloraddonsV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:32:21.954059 pipcoloraddonsV2-1.1.0/pipcoloraddonsV2/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-11 10:32:21.000000 pipcoloraddonsV2-1.1.0/pipcoloraddonsV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:32:21.954059 pipcoloraddonsV2-1.1.0/pipcoloraddonsV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-11 10:32:21.000000 pipcoloraddonsV2-1.1.0/pipcoloraddonsV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-11 10:32:21.000000 pipcoloraddonsV2-1.1.0/pipcoloraddonsV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 10:32:21.000000 pipcoloraddonsV2-1.1.0/pipcoloraddonsV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-11 10:32:21.000000 pipcoloraddonsV2-1.1.0/pipcoloraddonsV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 10:32:21.958059 pipcoloraddonsV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      562 2023-05-11 10:32:21.000000 pipcoloraddonsV2-1.1.0/setup.py
```

### Comparing `pipcoloraddonsV2-1.0.0/setup.py` & `pipcoloraddonsV2-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipcoloraddonsV2",
     version=VERSION,
```

