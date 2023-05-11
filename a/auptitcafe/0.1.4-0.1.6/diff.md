# Comparing `tmp/auptitcafe-0.1.4.tar.gz` & `tmp/auptitcafe-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auptitcafe-0.1.4.tar", max compression
+gzip compressed data, was "auptitcafe-0.1.6.tar", max compression
```

## Comparing `auptitcafe-0.1.4.tar` & `auptitcafe-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      340 2023-05-07 09:18:31.419815 auptitcafe-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-07 09:19:13.604766 auptitcafe-0.1.4/auptitcafe/__init__.py
--rw-r--r--   0        0        0     1932 2023-05-08 01:59:35.083951 auptitcafe-0.1.4/auptitcafe/menus.py
--rw-r--r--   0        0        0      502 2023-05-08 01:58:46.975392 auptitcafe-0.1.4/auptitcafe/plat.py
--rw-r--r--   0        0        0      441 2023-05-08 01:59:41.472027 auptitcafe-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 auptitcafe-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      703 2023-05-11 10:11:14.145038 auptitcafe-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 10:11:51.953313 auptitcafe-0.1.6/auptitcafe/__init__.py
+-rw-r--r--   0        0        0     2280 2023-05-11 10:11:14.145038 auptitcafe-0.1.6/auptitcafe/menus.py
+-rw-r--r--   0        0        0      502 2023-05-11 10:11:14.145038 auptitcafe-0.1.6/auptitcafe/plat.py
+-rw-r--r--   0        0        0      443 2023-05-11 10:11:14.145038 auptitcafe-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 auptitcafe-0.1.6/PKG-INFO
```

