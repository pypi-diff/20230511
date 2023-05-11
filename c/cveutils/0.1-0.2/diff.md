# Comparing `tmp/cveutils-0.1.tar.gz` & `tmp/cveutils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cveutils-0.1.tar", last modified: Thu May 11 04:04:57 2023, max compression
+gzip compressed data, was "cveutils-0.2.tar", last modified: Thu May 11 04:27:15 2023, max compression
```

## Comparing `cveutils-0.1.tar` & `cveutils-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:04:57.925330 cveutils-0.1/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      309 2023-05-11 04:04:57.925330 cveutils-0.1/PKG-INFO
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:04:57.913920 cveutils-0.1/cveutils/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)     3231 2023-05-11 04:00:13.000000 cveutils-0.1/cveutils/__init__.py
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:04:57.922320 cveutils-0.1/cveutils.egg-info/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      309 2023-05-11 04:04:57.000000 cveutils-0.1/cveutils.egg-info/PKG-INFO
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      201 2023-05-11 04:04:57.000000 cveutils-0.1/cveutils.egg-info/SOURCES.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        1 2023-05-11 04:04:57.000000 cveutils-0.1/cveutils.egg-info/dependency_links.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        9 2023-05-11 04:04:57.000000 cveutils-0.1/cveutils.egg-info/requires.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)        9 2023-05-11 04:04:57.000000 cveutils-0.1/cveutils.egg-info/top_level.txt
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)       38 2023-05-11 04:04:57.926330 cveutils-0.1/setup.cfg
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      436 2023-05-11 04:04:21.000000 cveutils-0.1/setup.py
-drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:04:57.924331 cveutils-0.1/test/
--rw-r--r--   0 vinicius  (1000) vinicius  (1000)      179 2023-05-11 04:01:48.000000 cveutils-0.1/test/test.py
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:27:15.736610 cveutils-0.2/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      309 2023-05-11 04:27:15.736395 cveutils-0.2/PKG-INFO
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)     1670 2023-05-11 04:22:48.000000 cveutils-0.2/README.md
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:27:15.732921 cveutils-0.2/cveutils.egg-info/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      309 2023-05-11 04:27:15.000000 cveutils-0.2/cveutils.egg-info/PKG-INFO
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      206 2023-05-11 04:27:15.000000 cveutils-0.2/cveutils.egg-info/SOURCES.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        1 2023-05-11 04:27:15.000000 cveutils-0.2/cveutils.egg-info/dependency_links.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        9 2023-05-11 04:27:15.000000 cveutils-0.2/cveutils.egg-info/requires.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        1 2023-05-11 04:27:15.000000 cveutils-0.2/cveutils.egg-info/top_level.txt
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:19:26.000000 cveutils-0.2/pyproject.toml
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)       38 2023-05-11 04:27:15.736610 cveutils-0.2/setup.cfg
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      472 2023-05-11 04:27:12.000000 cveutils-0.2/setup.py
+drwxr-xr-x   0 vinicius  (1000) vinicius  (1000)        0 2023-05-11 04:27:15.735040 cveutils-0.2/tests/
+-rw-r--r--   0 vinicius  (1000) vinicius  (1000)      179 2023-05-11 04:01:48.000000 cveutils-0.2/tests/test.py
```

