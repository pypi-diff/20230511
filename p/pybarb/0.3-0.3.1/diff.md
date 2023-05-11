# Comparing `tmp/pybarb-0.3.tar.gz` & `tmp/pybarb-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybarb-0.3.tar", last modified: Thu Mar 30 17:16:48 2023, max compression
+gzip compressed data, was "pybarb-0.3.1.tar", last modified: Thu May 11 11:27:21 2023, max compression
```

## Comparing `pybarb-0.3.tar` & `pybarb-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-03-30 17:16:48.114100 pybarb-0.3/
--rw-r--r--   0 simon_business   (501) staff       (20)       34 2023-03-22 12:48:08.000000 pybarb-0.3/MANIFEST.in
--rw-r--r--   0 simon_business   (501) staff       (20)      198 2023-03-30 17:16:48.113834 pybarb-0.3/PKG-INFO
--rw-r--r--   0 simon_business   (501) staff       (20)        0 2023-03-22 12:46:57.000000 pybarb-0.3/README.md
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-03-30 17:16:48.113443 pybarb-0.3/pybarb.egg-info/
--rw-r--r--   0 simon_business   (501) staff       (20)      198 2023-03-30 17:16:48.000000 pybarb-0.3/pybarb.egg-info/PKG-INFO
--rw-r--r--   0 simon_business   (501) staff       (20)      179 2023-03-30 17:16:48.000000 pybarb-0.3/pybarb.egg-info/SOURCES.txt
--rw-r--r--   0 simon_business   (501) staff       (20)        1 2023-03-30 17:16:48.000000 pybarb-0.3/pybarb.egg-info/dependency_links.txt
--rw-r--r--   0 simon_business   (501) staff       (20)       25 2023-03-30 17:16:48.000000 pybarb-0.3/pybarb.egg-info/requires.txt
--rw-r--r--   0 simon_business   (501) staff       (20)        1 2023-03-30 17:16:48.000000 pybarb-0.3/pybarb.egg-info/top_level.txt
--rw-r--r--   0 simon_business   (501) staff       (20)       38 2023-03-30 17:16:48.114198 pybarb-0.3/setup.cfg
--rw-r--r--   0 simon_business   (501) staff       (20)      382 2023-03-30 17:16:41.000000 pybarb-0.3/setup.py
+drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-11 11:27:21.607655 pybarb-0.3.1/
+-rw-r--r--   0 simon_business   (501) staff       (20)     1062 2023-04-25 15:18:38.000000 pybarb-0.3.1/LICENCE
+-rw-r--r--   0 simon_business   (501) staff       (20)       34 2023-04-25 15:18:38.000000 pybarb-0.3.1/MANIFEST.in
+-rw-r--r--   0 simon_business   (501) staff       (20)      222 2023-05-11 11:27:21.607430 pybarb-0.3.1/PKG-INFO
+-rw-r--r--   0 simon_business   (501) staff       (20)        0 2023-04-25 15:18:38.000000 pybarb-0.3.1/README.md
+drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-11 11:27:21.607081 pybarb-0.3.1/pybarb.egg-info/
+-rw-r--r--   0 simon_business   (501) staff       (20)      222 2023-05-11 11:27:21.000000 pybarb-0.3.1/pybarb.egg-info/PKG-INFO
+-rw-r--r--   0 simon_business   (501) staff       (20)      187 2023-05-11 11:27:21.000000 pybarb-0.3.1/pybarb.egg-info/SOURCES.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)        1 2023-05-11 11:27:21.000000 pybarb-0.3.1/pybarb.egg-info/dependency_links.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)       25 2023-05-11 11:27:21.000000 pybarb-0.3.1/pybarb.egg-info/requires.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)        1 2023-05-11 11:27:21.000000 pybarb-0.3.1/pybarb.egg-info/top_level.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)       38 2023-05-11 11:27:21.607747 pybarb-0.3.1/setup.cfg
+-rw-r--r--   0 simon_business   (501) staff       (20)      384 2023-05-11 11:27:06.000000 pybarb-0.3.1/setup.py
```

