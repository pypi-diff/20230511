# Comparing `tmp/pyneoncli-0.0.5a0.tar.gz` & `tmp/pyneoncli-0.0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneoncli-0.0.5a0.tar", max compression
+gzip compressed data, was "pyneoncli-0.0.7a0.tar", max compression
```

## Comparing `pyneoncli-0.0.5a0.tar` & `pyneoncli-0.0.7a0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-05-08 12:47:09.933275 pyneoncli-0.0.5a0/LICENSE
--rw-r--r--   0        0        0      299 2023-05-08 18:06:57.594209 pyneoncli-0.0.5a0/README.md
--rw-r--r--   0        0        0        0 2023-05-08 12:47:09.933740 pyneoncli-0.0.5a0/pyneoncli/__init__.py
--rw-r--r--   0        0        0     2077 2023-05-08 18:46:07.690127 pyneoncli-0.0.5a0/pyneoncli/cli_main.py
--rw-r--r--   0        0        0     1706 2023-05-08 19:20:33.722648 pyneoncli-0.0.5a0/pyneoncli/neon_api.py
--rw-r--r--   0        0        0      566 2023-05-08 19:22:23.156232 pyneoncli-0.0.5a0/pyproject.toml
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 pyneoncli-0.0.5a0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 12:47:09.933275 pyneoncli-0.0.7a0/LICENSE
+-rw-r--r--   0        0        0      995 2023-05-11 08:21:00.206759 pyneoncli-0.0.7a0/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 12:47:09.933740 pyneoncli-0.0.7a0/pyneoncli/__init__.py
+-rw-r--r--   0        0        0     4802 2023-05-11 08:17:48.738409 pyneoncli-0.0.7a0/pyneoncli/cli_main.py
+-rw-r--r--   0        0        0     5128 2023-05-11 07:55:41.053879 pyneoncli-0.0.7a0/pyneoncli/neon_api.py
+-rw-r--r--   0        0        0       22 2023-05-11 08:21:20.019916 pyneoncli-0.0.7a0/pyneoncli/version.py
+-rw-r--r--   0        0        0      566 2023-05-11 08:21:26.451662 pyneoncli-0.0.7a0/pyproject.toml
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 pyneoncli-0.0.7a0/PKG-INFO
```

### Comparing `pyneoncli-0.0.5a0/LICENSE` & `pyneoncli-0.0.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.0.5a0/pyproject.toml` & `pyneoncli-0.0.7a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "pyneoncli"
-version = "0.0.5a"
+version = "0.0.7a"
 description = "A Python CLI for the Neon API"
 authors = ["Joe Drumgoole <Joe.Drumgoole@neon.tech>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

