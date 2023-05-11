# Comparing `tmp/pyclean-2.7.0.tar.gz` & `tmp/pyclean-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclean-2.7.0.tar", last modified: Thu Feb 23 17:14:24 2023, max compression
+gzip compressed data, was "pyclean-2.7.1.tar", last modified: Thu May 11 08:12:20 2023, max compression
```

## Comparing `pyclean-2.7.0.tar` & `pyclean-2.7.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:14:24.858094 pyclean-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-23 17:14:10.000000 pyclean-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-23 17:14:10.000000 pyclean-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-02-23 17:14:24.858094 pyclean-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-02-23 17:14:10.000000 pyclean-2.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:14:24.858094 pyclean-2.7.0/pyclean/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-23 17:14:10.000000 pyclean-2.7.0/pyclean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-23 17:14:10.000000 pyclean-2.7.0/pyclean/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-02-23 17:14:10.000000 pyclean-2.7.0/pyclean/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-02-23 17:14:10.000000 pyclean-2.7.0/pyclean/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-02-23 17:14:10.000000 pyclean-2.7.0/pyclean/modern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-02-23 17:14:10.000000 pyclean-2.7.0/pyclean/py2clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-02-23 17:14:10.000000 pyclean-2.7.0/pyclean/py3clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-02-23 17:14:10.000000 pyclean-2.7.0/pyclean/pypyclean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:14:24.858094 pyclean-2.7.0/pyclean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-02-23 17:14:24.000000 pyclean-2.7.0/pyclean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-02-23 17:14:24.000000 pyclean-2.7.0/pyclean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 17:14:24.000000 pyclean-2.7.0/pyclean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-23 17:14:24.000000 pyclean-2.7.0/pyclean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-23 17:14:24.000000 pyclean-2.7.0/pyclean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-23 17:14:10.000000 pyclean-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 17:14:24.858094 pyclean-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-02-23 17:14:10.000000 pyclean-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:14:24.858094 pyclean-2.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-02-23 17:14:10.000000 pyclean-2.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-02-23 17:14:10.000000 pyclean-2.7.0/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-23 17:14:10.000000 pyclean-2.7.0/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-02-23 17:14:10.000000 pyclean-2.7.0/tests/test_modern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-02-23 17:14:10.000000 pyclean-2.7.0/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-02-23 17:14:10.000000 pyclean-2.7.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:12:20.495812 pyclean-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 08:12:05.000000 pyclean-2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-11 08:12:05.000000 pyclean-2.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-05-11 08:12:20.495812 pyclean-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-05-11 08:12:05.000000 pyclean-2.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:12:20.495812 pyclean-2.7.1/pyclean/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-11 08:12:05.000000 pyclean-2.7.1/pyclean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-11 08:12:05.000000 pyclean-2.7.1/pyclean/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-11 08:12:05.000000 pyclean-2.7.1/pyclean/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-11 08:12:05.000000 pyclean-2.7.1/pyclean/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-11 08:12:05.000000 pyclean-2.7.1/pyclean/modern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-11 08:12:05.000000 pyclean-2.7.1/pyclean/py2clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-11 08:12:05.000000 pyclean-2.7.1/pyclean/py3clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-11 08:12:05.000000 pyclean-2.7.1/pyclean/pypyclean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:12:20.495812 pyclean-2.7.1/pyclean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-05-11 08:12:20.000000 pyclean-2.7.1/pyclean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-11 08:12:20.000000 pyclean-2.7.1/pyclean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:12:20.000000 pyclean-2.7.1/pyclean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-11 08:12:20.000000 pyclean-2.7.1/pyclean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 08:12:20.000000 pyclean-2.7.1/pyclean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-11 08:12:05.000000 pyclean-2.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:12:20.495812 pyclean-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-11 08:12:05.000000 pyclean-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:12:20.495812 pyclean-2.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-11 08:12:05.000000 pyclean-2.7.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-11 08:12:05.000000 pyclean-2.7.1/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-11 08:12:05.000000 pyclean-2.7.1/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-05-11 08:12:05.000000 pyclean-2.7.1/tests/test_modern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-11 08:12:05.000000 pyclean-2.7.1/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-11 08:12:05.000000 pyclean-2.7.1/tests/test_version.py
```

### Comparing `pyclean-2.7.0/LICENSE` & `pyclean-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.0/PKG-INFO` & `pyclean-2.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclean
-Version: 2.7.0
+Version: 2.7.1
 Summary: Pure Python cross-platform pyclean. Clean up your Python bytecode.
 Home-page: https://github.com/bittner/pyclean
 Author: Peter Bittner
 Author-email: django@bittner.it
 Keywords: python,bytecode,cli,tools
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -25,33 +25,36 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 pyclean |latest-version|
 ========================
 
-|checks-status| |tests-status| |scrutinizer| |codacy| |python-versions| |python-impl| |license|
+|checks-status| |tests-status| |publish-status| |scrutinizer| |codacy| |python-versions| |python-impl| |license|
 
 Worried about ``.pyc`` files and ``__pycache__`` directories? Fear not!
 PyClean is here to help. Finally the single-command clean up for Python
 bytecode files in your favorite directories. On any platform.
 
 |video|
 
 `Presented at PyConX`_, Firenze 2019.
 
 .. |latest-version| image:: https://img.shields.io/pypi/v/pyclean.svg
    :target: https://pypi.org/project/pyclean
    :alt: Latest version on PyPI
-.. |checks-status| image:: https://img.shields.io/github/actions/workflow/status/bittner/pyclean/check.yml?branch=main&label=Checks&logo=github
+.. |checks-status| image:: https://github.com/bittner/pyclean/actions/workflows/check.yml/badge.svg
    :target: https://github.com/bittner/pyclean/actions/workflows/check.yml
    :alt: GitHub Workflow Status
-.. |tests-status| image:: https://img.shields.io/github/actions/workflow/status/bittner/pyclean/test.yml?branch=main&label=Tests&logo=github
+.. |tests-status| image:: https://github.com/bittner/pyclean/actions/workflows/test.yml/badge.svg
    :target: https://github.com/bittner/pyclean/actions/workflows/test.yml
    :alt: GitHub Workflow Status
+.. |publish-status| image:: https://github.com/bittner/pyclean/actions/workflows/publish.yml/badge.svg
+   :target: https://github.com/bittner/pyclean/actions/workflows/publish.yml
+   :alt: GitHub Workflow Status
 .. |scrutinizer| image:: https://img.shields.io/scrutinizer/build/g/bittner/pyclean/main?logo=scrutinizer&label=%22
    :target: https://scrutinizer-ci.com/g/bittner/pyclean/
    :alt: Scrutinizer
 .. |codacy| image:: https://img.shields.io/codacy/grade/69de1364a09f41b399f95afe901826eb/main.svg?logo=codacy&label=%22
    :target: https://app.codacy.com/gh/bittner/pyclean/dashboard
    :alt: Code health
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/pyclean.svg
```

### Comparing `pyclean-2.7.0/README.rst` & `pyclean-2.7.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 pyclean |latest-version|
 ========================
 
-|checks-status| |tests-status| |scrutinizer| |codacy| |python-versions| |python-impl| |license|
+|checks-status| |tests-status| |publish-status| |scrutinizer| |codacy| |python-versions| |python-impl| |license|
 
 Worried about ``.pyc`` files and ``__pycache__`` directories? Fear not!
 PyClean is here to help. Finally the single-command clean up for Python
 bytecode files in your favorite directories. On any platform.
 
 |video|
 
 `Presented at PyConX`_, Firenze 2019.
 
 .. |latest-version| image:: https://img.shields.io/pypi/v/pyclean.svg
    :target: https://pypi.org/project/pyclean
    :alt: Latest version on PyPI
-.. |checks-status| image:: https://img.shields.io/github/actions/workflow/status/bittner/pyclean/check.yml?branch=main&label=Checks&logo=github
+.. |checks-status| image:: https://github.com/bittner/pyclean/actions/workflows/check.yml/badge.svg
    :target: https://github.com/bittner/pyclean/actions/workflows/check.yml
    :alt: GitHub Workflow Status
-.. |tests-status| image:: https://img.shields.io/github/actions/workflow/status/bittner/pyclean/test.yml?branch=main&label=Tests&logo=github
+.. |tests-status| image:: https://github.com/bittner/pyclean/actions/workflows/test.yml/badge.svg
    :target: https://github.com/bittner/pyclean/actions/workflows/test.yml
    :alt: GitHub Workflow Status
+.. |publish-status| image:: https://github.com/bittner/pyclean/actions/workflows/publish.yml/badge.svg
+   :target: https://github.com/bittner/pyclean/actions/workflows/publish.yml
+   :alt: GitHub Workflow Status
 .. |scrutinizer| image:: https://img.shields.io/scrutinizer/build/g/bittner/pyclean/main?logo=scrutinizer&label=%22
    :target: https://scrutinizer-ci.com/g/bittner/pyclean/
    :alt: Scrutinizer
 .. |codacy| image:: https://img.shields.io/codacy/grade/69de1364a09f41b399f95afe901826eb/main.svg?logo=codacy&label=%22
    :target: https://app.codacy.com/gh/bittner/pyclean/dashboard
    :alt: Code health
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/pyclean.svg
```

### Comparing `pyclean-2.7.0/pyclean/cli.py` & `pyclean-2.7.1/pyclean/cli.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.0/pyclean/compat.py` & `pyclean-2.7.1/pyclean/compat.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.0/pyclean/modern.py` & `pyclean-2.7.1/pyclean/modern.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,19 @@
         'htmlcov/',
     ],
     'jupyter': [
         '.ipynb_checkpoints/**/*',
         '.ipynb_checkpoints/',
     ],
     'package': [
+        'build/bdist.*/**/*',
+        'build/bdist.*/',
+        'build/lib/**/*',
+        'build/lib/',
+        'build/',
         'dist/**/*',
         'dist/',
         'sdist/**/*',
         'sdist/',
         '*.egg-info/**/*',
         '*.egg-info/',
     ],
```

### Comparing `pyclean-2.7.0/pyclean/py2clean.py` & `pyclean-2.7.1/pyclean/py2clean.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.0/pyclean/py3clean.py` & `pyclean-2.7.1/pyclean/py3clean.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.0/pyclean/pypyclean.py` & `pyclean-2.7.1/pyclean/pypyclean.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.0/pyclean.egg-info/PKG-INFO` & `pyclean-2.7.1/pyclean.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclean
-Version: 2.7.0
+Version: 2.7.1
 Summary: Pure Python cross-platform pyclean. Clean up your Python bytecode.
 Home-page: https://github.com/bittner/pyclean
 Author: Peter Bittner
 Author-email: django@bittner.it
 Keywords: python,bytecode,cli,tools
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -25,33 +25,36 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 pyclean |latest-version|
 ========================
 
-|checks-status| |tests-status| |scrutinizer| |codacy| |python-versions| |python-impl| |license|
+|checks-status| |tests-status| |publish-status| |scrutinizer| |codacy| |python-versions| |python-impl| |license|
 
 Worried about ``.pyc`` files and ``__pycache__`` directories? Fear not!
 PyClean is here to help. Finally the single-command clean up for Python
 bytecode files in your favorite directories. On any platform.
 
 |video|
 
 `Presented at PyConX`_, Firenze 2019.
 
 .. |latest-version| image:: https://img.shields.io/pypi/v/pyclean.svg
    :target: https://pypi.org/project/pyclean
    :alt: Latest version on PyPI
-.. |checks-status| image:: https://img.shields.io/github/actions/workflow/status/bittner/pyclean/check.yml?branch=main&label=Checks&logo=github
+.. |checks-status| image:: https://github.com/bittner/pyclean/actions/workflows/check.yml/badge.svg
    :target: https://github.com/bittner/pyclean/actions/workflows/check.yml
    :alt: GitHub Workflow Status
-.. |tests-status| image:: https://img.shields.io/github/actions/workflow/status/bittner/pyclean/test.yml?branch=main&label=Tests&logo=github
+.. |tests-status| image:: https://github.com/bittner/pyclean/actions/workflows/test.yml/badge.svg
    :target: https://github.com/bittner/pyclean/actions/workflows/test.yml
    :alt: GitHub Workflow Status
+.. |publish-status| image:: https://github.com/bittner/pyclean/actions/workflows/publish.yml/badge.svg
+   :target: https://github.com/bittner/pyclean/actions/workflows/publish.yml
+   :alt: GitHub Workflow Status
 .. |scrutinizer| image:: https://img.shields.io/scrutinizer/build/g/bittner/pyclean/main?logo=scrutinizer&label=%22
    :target: https://scrutinizer-ci.com/g/bittner/pyclean/
    :alt: Scrutinizer
 .. |codacy| image:: https://img.shields.io/codacy/grade/69de1364a09f41b399f95afe901826eb/main.svg?logo=codacy&label=%22
    :target: https://app.codacy.com/gh/bittner/pyclean/dashboard
    :alt: Code health
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/pyclean.svg
```

### Comparing `pyclean-2.7.0/pyproject.toml` & `pyclean-2.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.0/setup.py` & `pyclean-2.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.0/tests/test_cli.py` & `pyclean-2.7.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.0/tests/test_compat.py` & `pyclean-2.7.1/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.0/tests/test_modern.py` & `pyclean-2.7.1/tests/test_modern.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.0/tests/test_package.py` & `pyclean-2.7.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `pyclean-2.7.0/tests/test_version.py` & `pyclean-2.7.1/tests/test_version.py`

 * *Files identical despite different names*

