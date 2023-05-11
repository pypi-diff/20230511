# Comparing `tmp/pyrc-test-python-package-0.0.2.tar.gz` & `tmp/pyrc-test-python-package-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrc-test-python-package-0.0.2.tar", last modified: Thu May 11 15:49:46 2023, max compression
+gzip compressed data, was "pyrc-test-python-package-0.0.3.tar", last modified: Thu May 11 16:10:12 2023, max compression
```

## Comparing `pyrc-test-python-package-0.0.2.tar` & `pyrc-test-python-package-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:49:46.291292 pyrc-test-python-package-0.0.2/
--rw-rw-rw-   0        0        0      184 2023-05-11 15:49:46.290788 pyrc-test-python-package-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-11 15:49:46.291292 pyrc-test-python-package-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      368 2023-05-11 15:49:41.000000 pyrc-test-python-package-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:49:46.271264 pyrc-test-python-package-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:49:46.278273 pyrc-test-python-package-0.0.2/src/pyrc_test_python_package/
--rw-rw-rw-   0        0        0        0 2023-05-11 11:29:19.000000 pyrc-test-python-package-0.0.2/src/pyrc_test_python_package/__init__.py
--rw-rw-rw-   0        0        0      166 2023-05-11 11:42:32.000000 pyrc-test-python-package-0.0.2/src/pyrc_test_python_package/test_module.py
--rw-rw-rw-   0        0        0       88 2023-05-11 11:42:32.000000 pyrc-test-python-package-0.0.2/src/pyrc_test_python_package/test_module_common.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:49:46.289793 pyrc-test-python-package-0.0.2/src/pyrc_test_python_package.egg-info/
--rw-rw-rw-   0        0        0      184 2023-05-11 15:49:46.000000 pyrc-test-python-package-0.0.2/src/pyrc_test_python_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-05-11 15:49:46.000000 pyrc-test-python-package-0.0.2/src/pyrc_test_python_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:49:46.000000 pyrc-test-python-package-0.0.2/src/pyrc_test_python_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-11 15:49:46.000000 pyrc-test-python-package-0.0.2/src/pyrc_test_python_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 16:10:12.785322 pyrc-test-python-package-0.0.3/
+-rw-rw-rw-   0        0        0      184 2023-05-11 16:10:12.784322 pyrc-test-python-package-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-11 16:10:12.785322 pyrc-test-python-package-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      368 2023-05-11 16:09:59.000000 pyrc-test-python-package-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:10:12.766323 pyrc-test-python-package-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 16:10:12.770323 pyrc-test-python-package-0.0.3/src/pyrc_test_python_package/
+-rw-rw-rw-   0        0        0       65 2023-05-11 16:08:59.000000 pyrc-test-python-package-0.0.3/src/pyrc_test_python_package/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-05-11 11:42:32.000000 pyrc-test-python-package-0.0.3/src/pyrc_test_python_package/test_module.py
+-rw-rw-rw-   0        0        0       88 2023-05-11 11:42:32.000000 pyrc-test-python-package-0.0.3/src/pyrc_test_python_package/test_module_common.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:10:12.783322 pyrc-test-python-package-0.0.3/src/pyrc_test_python_package.egg-info/
+-rw-rw-rw-   0        0        0      184 2023-05-11 16:10:12.000000 pyrc-test-python-package-0.0.3/src/pyrc_test_python_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-05-11 16:10:12.000000 pyrc-test-python-package-0.0.3/src/pyrc_test_python_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 16:10:12.000000 pyrc-test-python-package-0.0.3/src/pyrc_test_python_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-11 16:10:12.000000 pyrc-test-python-package-0.0.3/src/pyrc_test_python_package.egg-info/top_level.txt
```

