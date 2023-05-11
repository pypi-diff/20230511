# Comparing `tmp/sierras-0.1.2.tar.gz` & `tmp/sierras-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sierras-0.1.2.tar", last modified: Fri Nov  4 19:22:27 2022, max compression
+gzip compressed data, was "sierras-0.2.0.tar", last modified: Wed May 10 17:52:04 2023, max compression
```

## Comparing `sierras-0.1.2.tar` & `sierras-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 19:22:27.548471 sierras-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-11-04 19:22:20.000000 sierras-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-11-04 19:22:20.000000 sierras-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-11-04 19:22:27.548471 sierras-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-11-04 19:22:20.000000 sierras-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 19:22:27.548471 sierras-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-11-04 19:22:20.000000 sierras-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 19:22:27.544471 sierras-0.1.2/sierras/
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-11-04 19:22:20.000000 sierras-0.1.2/sierras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10100 2022-11-04 19:22:20.000000 sierras-0.1.2/sierras/arrhenius.py
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-11-04 19:22:20.000000 sierras-0.1.2/sierras/get_diffusion_coefficient.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 19:22:27.548471 sierras-0.1.2/sierras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-11-04 19:22:27.000000 sierras-0.1.2/sierras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 19:22:27.000000 sierras-0.1.2/sierras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 19:22:27.000000 sierras-0.1.2/sierras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-04 19:22:27.000000 sierras-0.1.2/sierras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-04 19:22:27.000000 sierras-0.1.2/sierras.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:52:04.586007 sierras-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-10 17:51:49.000000 sierras-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-10 17:51:49.000000 sierras-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-10 17:52:04.586007 sierras-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-10 17:51:49.000000 sierras-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-10 17:51:49.000000 sierras-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 17:52:04.586007 sierras-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:52:04.586007 sierras-0.2.0/sierras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-10 17:52:04.000000 sierras-0.2.0/sierras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-10 17:52:04.000000 sierras-0.2.0/sierras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 17:52:04.000000 sierras-0.2.0/sierras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 17:52:04.000000 sierras-0.2.0/sierras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 17:52:04.000000 sierras-0.2.0/sierras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-10 17:51:49.000000 sierras-0.2.0/sierras.py
```

### Comparing `sierras-0.1.2/LICENSE` & `sierras-0.2.0/LICENSE`

 * *Files identical despite different names*

