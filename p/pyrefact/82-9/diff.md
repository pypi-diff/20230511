# Comparing `tmp/pyrefact-82.tar.gz` & `tmp/pyrefact-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrefact-82.tar", last modified: Thu May 11 17:27:43 2023, max compression
+gzip compressed data, was "pyrefact-9.tar", last modified: Wed Nov  2 20:30:27 2022, max compression
```

## Comparing `pyrefact-82.tar` & `pyrefact-9.tar`

### file list

```diff
@@ -1,32 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:27:43.874118 pyrefact-82/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-11 17:27:27.000000 pyrefact-82/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-11 17:27:43.874118 pyrefact-82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-11 17:27:27.000000 pyrefact-82/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-11 17:27:27.000000 pyrefact-82/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:27:43.874118 pyrefact-82/pyrefact/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26865 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/abstractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)   124872 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/logs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12888 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/object_oriented.py
--rw-r--r--   0 runner    (1001) docker     (123)    40172 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/performance_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/performance_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-05-11 17:27:27.000000 pyrefact-82/pyrefact/symbolic_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:27:43.874118 pyrefact-82/pyrefact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-11 17:27:43.000000 pyrefact-82/pyrefact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-11 17:27:43.000000 pyrefact-82/pyrefact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 17:27:43.000000 pyrefact-82/pyrefact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 17:27:43.000000 pyrefact-82/pyrefact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-11 17:27:43.000000 pyrefact-82/pyrefact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 17:27:43.000000 pyrefact-82/pyrefact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 17:27:43.874118 pyrefact-82/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:27:43.874118 pyrefact-82/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-11 17:27:27.000000 pyrefact-82/tests/testing_infra.py
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.405663 pyrefact-9/
+-rw-r--r--   0 olle       (501) staff       (20)     1069 2022-10-20 08:55:02.000000 pyrefact-9/LICENSE
+-rw-r--r--   0 olle       (501) staff       (20)      228 2022-11-02 20:30:27.405542 pyrefact-9/PKG-INFO
+-rw-r--r--   0 olle       (501) staff       (20)     1262 2022-11-02 18:36:20.000000 pyrefact-9/README.md
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.404795 pyrefact-9/pyrefact/
+-rw-r--r--   0 olle       (501) staff       (20)        0 2022-10-23 21:51:04.000000 pyrefact-9/pyrefact/__init__.py
+-rwxr-xr-x   0 olle       (501) staff       (20)      120 2022-10-20 18:11:25.000000 pyrefact-9/pyrefact/__main__.py
+-rw-r--r--   0 olle       (501) staff       (20)     2148 2022-11-02 19:54:47.000000 pyrefact-9/pyrefact/completion.py
+-rw-r--r--   0 olle       (501) staff       (20)     1065 2022-10-30 20:04:01.000000 pyrefact-9/pyrefact/constants.py
+-rw-r--r--   0 olle       (501) staff       (20)    31081 2022-11-02 20:24:19.000000 pyrefact-9/pyrefact/fixes.py
+-rwxr-xr-x   0 olle       (501) staff       (20)     3867 2022-11-02 12:50:20.000000 pyrefact-9/pyrefact/main.py
+-rw-r--r--   0 olle       (501) staff       (20)    12892 2022-11-02 19:54:47.000000 pyrefact-9/pyrefact/parsing.py
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.405383 pyrefact-9/pyrefact.egg-info/
+-rw-r--r--   0 olle       (501) staff       (20)      228 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/PKG-INFO
+-rw-r--r--   0 olle       (501) staff       (20)      327 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/SOURCES.txt
+-rw-r--r--   0 olle       (501) staff       (20)        1 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/dependency_links.txt
+-rw-r--r--   0 olle       (501) staff       (20)       40 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/requires.txt
+-rw-r--r--   0 olle       (501) staff       (20)        9 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/top_level.txt
+-rw-r--r--   0 olle       (501) staff       (20)       38 2022-11-02 20:30:27.405698 pyrefact-9/setup.cfg
+-rw-r--r--   0 olle       (501) staff       (20)      468 2022-11-02 20:30:04.000000 pyrefact-9/setup.py
```

### Comparing `pyrefact-82/LICENSE` & `pyrefact-9/LICENSE`

 * *Files identical despite different names*

