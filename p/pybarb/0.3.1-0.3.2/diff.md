# Comparing `tmp/pybarb-0.3.1.tar.gz` & `tmp/pybarb-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybarb-0.3.1.tar", last modified: Thu May 11 11:27:21 2023, max compression
+gzip compressed data, was "pybarb-0.3.2.tar", last modified: Thu May 11 11:39:43 2023, max compression
```

## Comparing `pybarb-0.3.1.tar` & `pybarb-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-11 11:27:21.607655 pybarb-0.3.1/
--rw-r--r--   0 simon_business   (501) staff       (20)     1062 2023-04-25 15:18:38.000000 pybarb-0.3.1/LICENCE
--rw-r--r--   0 simon_business   (501) staff       (20)       34 2023-04-25 15:18:38.000000 pybarb-0.3.1/MANIFEST.in
--rw-r--r--   0 simon_business   (501) staff       (20)      222 2023-05-11 11:27:21.607430 pybarb-0.3.1/PKG-INFO
--rw-r--r--   0 simon_business   (501) staff       (20)        0 2023-04-25 15:18:38.000000 pybarb-0.3.1/README.md
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-11 11:27:21.607081 pybarb-0.3.1/pybarb.egg-info/
--rw-r--r--   0 simon_business   (501) staff       (20)      222 2023-05-11 11:27:21.000000 pybarb-0.3.1/pybarb.egg-info/PKG-INFO
--rw-r--r--   0 simon_business   (501) staff       (20)      187 2023-05-11 11:27:21.000000 pybarb-0.3.1/pybarb.egg-info/SOURCES.txt
--rw-r--r--   0 simon_business   (501) staff       (20)        1 2023-05-11 11:27:21.000000 pybarb-0.3.1/pybarb.egg-info/dependency_links.txt
--rw-r--r--   0 simon_business   (501) staff       (20)       25 2023-05-11 11:27:21.000000 pybarb-0.3.1/pybarb.egg-info/requires.txt
--rw-r--r--   0 simon_business   (501) staff       (20)        1 2023-05-11 11:27:21.000000 pybarb-0.3.1/pybarb.egg-info/top_level.txt
--rw-r--r--   0 simon_business   (501) staff       (20)       38 2023-05-11 11:27:21.607747 pybarb-0.3.1/setup.cfg
--rw-r--r--   0 simon_business   (501) staff       (20)      384 2023-05-11 11:27:06.000000 pybarb-0.3.1/setup.py
+drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-11 11:39:43.215998 pybarb-0.3.2/
+-rw-r--r--   0 simon_business   (501) staff       (20)      200 2023-05-11 11:39:43.215762 pybarb-0.3.2/PKG-INFO
+-rw-r--r--   0 simon_business   (501) staff       (20)     2744 2023-04-25 15:40:48.000000 pybarb-0.3.2/README.md
+drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-11 11:39:43.213938 pybarb-0.3.2/pybarb/
+-rw-r--r--   0 simon_business   (501) staff       (20)        0 2023-04-25 15:18:38.000000 pybarb-0.3.2/pybarb/__init__.py
+-rw-r--r--   0 simon_business   (501) staff       (20)    23770 2023-04-25 15:18:38.000000 pybarb-0.3.2/pybarb/pybarb.py
+drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-11 11:39:43.215429 pybarb-0.3.2/pybarb.egg-info/
+-rw-r--r--   0 simon_business   (501) staff       (20)      200 2023-05-11 11:39:43.000000 pybarb-0.3.2/pybarb.egg-info/PKG-INFO
+-rw-r--r--   0 simon_business   (501) staff       (20)      203 2023-05-11 11:39:43.000000 pybarb-0.3.2/pybarb.egg-info/SOURCES.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)        1 2023-05-11 11:39:43.000000 pybarb-0.3.2/pybarb.egg-info/dependency_links.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)       25 2023-05-11 11:39:43.000000 pybarb-0.3.2/pybarb.egg-info/requires.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)        7 2023-05-11 11:39:43.000000 pybarb-0.3.2/pybarb.egg-info/top_level.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)       38 2023-05-11 11:39:43.216086 pybarb-0.3.2/setup.cfg
+-rw-r--r--   0 simon_business   (501) staff       (20)      384 2023-05-11 11:39:31.000000 pybarb-0.3.2/setup.py
```

