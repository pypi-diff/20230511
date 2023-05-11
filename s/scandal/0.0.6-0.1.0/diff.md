# Comparing `tmp/scandal-0.0.6.tar.gz` & `tmp/scandal-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scandal-0.0.6.tar", max compression
+gzip compressed data, was "scandal-0.1.0.tar", max compression
```

## Comparing `scandal-0.0.6.tar` & `scandal-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,5 @@
--rw-r--r--   0        0        0       10 2023-05-11 10:26:14.791135 scandal-0.0.6/README.md
--rw-r--r--   0        0        0      693 2023-05-11 10:26:14.791135 scandal-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2467 2023-05-11 10:26:14.791135 scandal-0.0.6/scandal/__init__.py
--rw-r--r--   0        0        0      168 2023-05-11 10:26:14.791135 scandal-0.0.6/scandal/__main__.py
--rw-r--r--   0        0        0     3056 2023-05-11 10:26:14.791135 scandal-0.0.6/scandal/_auth.py
--rw-r--r--   0        0        0      114 2023-05-11 10:26:14.791135 scandal-0.0.6/scandal/_connection.py
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 scandal-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-01-25 19:10:04.641866 scandal-0.1.0/README.md
+-rw-r--r--   0        0        0      267 2023-03-13 15:15:00.725127 scandal-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-25 19:09:43.713227 scandal-0.1.0/scandal/__init__.py
+-rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 scandal-0.1.0/setup.py
+-rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 scandal-0.1.0/PKG-INFO
```

