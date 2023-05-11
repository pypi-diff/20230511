# Comparing `tmp/cveutils-0.2.tar.gz` & `tmp/cveutils-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cveutils-0.2.tar", last modified: Thu May 11 04:27:15 2023, max compression
+gzip compressed data, was "cveutils-0.3.tar", last modified: Thu May 11 04:33:52 2023, max compression
```

## Comparing `cveutils-0.2.tar` & `cveutils-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:27:15.736610 cveutils-0.2/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      309 2023-05-11 04:27:15.736395 cveutils-0.2/PKG-INFO
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)     1670 2023-05-11 04:22:48.000000 cveutils-0.2/README.md
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:27:15.732921 cveutils-0.2/cveutils.egg-info/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      309 2023-05-11 04:27:15.000000 cveutils-0.2/cveutils.egg-info/PKG-INFO
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      206 2023-05-11 04:27:15.000000 cveutils-0.2/cveutils.egg-info/SOURCES.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        1 2023-05-11 04:27:15.000000 cveutils-0.2/cveutils.egg-info/dependency_links.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        9 2023-05-11 04:27:15.000000 cveutils-0.2/cveutils.egg-info/requires.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        1 2023-05-11 04:27:15.000000 cveutils-0.2/cveutils.egg-info/top_level.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:19:26.000000 cveutils-0.2/pyproject.toml
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)       38 2023-05-11 04:27:15.736610 cveutils-0.2/setup.cfg
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      472 2023-05-11 04:27:12.000000 cveutils-0.2/setup.py
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:27:15.735040 cveutils-0.2/tests/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      179 2023-05-11 04:01:48.000000 cveutils-0.2/tests/test.py
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:33:52.313009 cveutils-0.3/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     2020 2023-05-11 04:33:52.312350 cveutils-0.3/PKG-INFO
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     1670 2023-05-11 04:22:48.000000 cveutils-0.3/README.md
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:33:52.309350 cveutils-0.3/cveutils.egg-info/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     2020 2023-05-11 04:33:52.000000 cveutils-0.3/cveutils.egg-info/PKG-INFO
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      206 2023-05-11 04:33:52.000000 cveutils-0.3/cveutils.egg-info/SOURCES.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        1 2023-05-11 04:33:52.000000 cveutils-0.3/cveutils.egg-info/dependency_links.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        9 2023-05-11 04:33:52.000000 cveutils-0.3/cveutils.egg-info/requires.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        1 2023-05-11 04:33:52.000000 cveutils-0.3/cveutils.egg-info/top_level.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:19:26.000000 cveutils-0.3/pyproject.toml
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)       38 2023-05-11 04:33:52.313009 cveutils-0.3/setup.cfg
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      673 2023-05-11 04:33:38.000000 cveutils-0.3/setup.py
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:33:52.311349 cveutils-0.3/tests/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      179 2023-05-11 04:01:48.000000 cveutils-0.3/tests/test.py
```

### Comparing `cveutils-0.2/README.md` & `cveutils-0.3/README.md`

 * *Files identical despite different names*

