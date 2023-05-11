# Comparing `tmp/pyrc-test-python-package-0.0.4.tar.gz` & `tmp/pyrc-test-python-package-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrc-test-python-package-0.0.4.tar", last modified: Thu May 11 16:19:14 2023, max compression
+gzip compressed data, was "pyrc-test-python-package-0.0.5.tar", last modified: Thu May 11 16:47:43 2023, max compression
```

## Comparing `pyrc-test-python-package-0.0.4.tar` & `pyrc-test-python-package-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 16:19:14.983995 pyrc-test-python-package-0.0.4/
--rw-rw-rw-   0        0        0      184 2023-05-11 16:19:14.983995 pyrc-test-python-package-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-11 16:19:14.983995 pyrc-test-python-package-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      414 2023-05-11 16:19:12.000000 pyrc-test-python-package-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:19:14.968482 pyrc-test-python-package-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 16:19:14.972482 pyrc-test-python-package-0.0.4/src/pyrc_test_python_package/
--rw-rw-rw-   0        0        0       65 2023-05-11 16:08:59.000000 pyrc-test-python-package-0.0.4/src/pyrc_test_python_package/__init__.py
--rw-rw-rw-   0        0        0      166 2023-05-11 11:42:32.000000 pyrc-test-python-package-0.0.4/src/pyrc_test_python_package/test_module.py
--rw-rw-rw-   0        0        0       88 2023-05-11 11:42:32.000000 pyrc-test-python-package-0.0.4/src/pyrc_test_python_package/test_module_common.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:19:14.982995 pyrc-test-python-package-0.0.4/src/pyrc_test_python_package.egg-info/
--rw-rw-rw-   0        0        0      184 2023-05-11 16:19:14.000000 pyrc-test-python-package-0.0.4/src/pyrc_test_python_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-05-11 16:19:14.000000 pyrc-test-python-package-0.0.4/src/pyrc_test_python_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 16:19:14.000000 pyrc-test-python-package-0.0.4/src/pyrc_test_python_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-11 16:19:14.000000 pyrc-test-python-package-0.0.4/src/pyrc_test_python_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 16:47:43.492917 pyrc-test-python-package-0.0.5/
+-rw-rw-rw-   0        0        0      184 2023-05-11 16:47:43.492917 pyrc-test-python-package-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-11 16:47:43.492917 pyrc-test-python-package-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      368 2023-05-11 16:47:27.000000 pyrc-test-python-package-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:47:43.470869 pyrc-test-python-package-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 16:47:43.474877 pyrc-test-python-package-0.0.5/src/pyrc_test_python_package/
+-rw-rw-rw-   0        0        0       65 2023-05-11 16:08:59.000000 pyrc-test-python-package-0.0.5/src/pyrc_test_python_package/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-05-11 11:42:32.000000 pyrc-test-python-package-0.0.5/src/pyrc_test_python_package/test_module.py
+-rw-rw-rw-   0        0        0       88 2023-05-11 11:42:32.000000 pyrc-test-python-package-0.0.5/src/pyrc_test_python_package/test_module_common.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:47:43.491915 pyrc-test-python-package-0.0.5/src/pyrc_test_python_package.egg-info/
+-rw-rw-rw-   0        0        0      184 2023-05-11 16:47:43.000000 pyrc-test-python-package-0.0.5/src/pyrc_test_python_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-05-11 16:47:43.000000 pyrc-test-python-package-0.0.5/src/pyrc_test_python_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 16:47:43.000000 pyrc-test-python-package-0.0.5/src/pyrc_test_python_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-11 16:47:43.000000 pyrc-test-python-package-0.0.5/src/pyrc_test_python_package.egg-info/top_level.txt
```

