# Comparing `tmp/aiida-hyperqueue-0.1.0.tar.gz` & `tmp/aiida-hyperqueue-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-hyperqueue-0.1.0.tar", last modified: Thu May 11 00:06:46 2023, max compression
+gzip compressed data, was "aiida-hyperqueue-0.1.1.tar", last modified: Thu May 11 01:17:51 2023, max compression
```

## Comparing `aiida-hyperqueue-0.1.0.tar` & `aiida-hyperqueue-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0     2085 2023-05-10 23:55:19.091753 aiida-hyperqueue-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      115 2021-12-12 19:46:22.178074 aiida-hyperqueue-0.1.0/.gitignore
--rw-r--r--   0        0        0      728 2023-05-10 23:55:18.011757 aiida-hyperqueue-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      119 2021-12-10 08:37:45.469825 aiida-hyperqueue-0.1.0/.readthedocs.yml
--rw-r--r--   0        0        0     1072 2021-12-10 08:37:45.469825 aiida-hyperqueue-0.1.0/LICENSE
--rw-r--r--   0        0        0     1023 2023-05-10 23:57:56.619083 aiida-hyperqueue-0.1.0/README.md
--rw-r--r--   0        0        0      119 2022-03-14 13:13:40.066239 aiida-hyperqueue-0.1.0/aiida_hyperqueue/__init__.py
--rw-r--r--   0        0        0     4396 2023-05-10 22:53:05.119596 aiida-hyperqueue-0.1.0/aiida_hyperqueue/cli.py
--rw-r--r--   0        0        0    10759 2023-05-10 22:08:16.531050 aiida-hyperqueue-0.1.0/aiida_hyperqueue/scheduler.py
--rw-r--r--   0        0        0        7 2021-12-10 08:37:45.509825 aiida-hyperqueue-0.1.0/docs/.gitignore
--rwxr-xr-x   0        0        0     1541 2021-12-10 08:37:45.505825 aiida-hyperqueue-0.1.0/docs/Makefile
--rwxr-xr-x   0        0        0     5462 2023-05-10 23:05:50.460339 aiida-hyperqueue-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0     2785 2021-12-15 00:03:59.317511 aiida-hyperqueue-0.1.0/docs/source/developer_guide/index.md
--rw-r--r--   0        0        0     6116 2023-05-10 21:16:05.532499 aiida-hyperqueue-0.1.0/docs/source/get_started.md
--rw-r--r--   0        0        0    76300 2021-12-10 08:37:45.521825 aiida-hyperqueue-0.1.0/docs/source/img/AiiDA_transparent_logo.png
--rw-r--r--   0        0        0     1837 2021-12-15 00:45:56.634347 aiida-hyperqueue-0.1.0/docs/source/index.md
--rw-r--r--   0        0        0     1733 2023-05-10 23:55:20.239748 aiida-hyperqueue-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      239 2022-03-14 13:13:40.190239 aiida-hyperqueue-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      363 2022-03-14 13:13:40.198238 aiida-hyperqueue-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0      485 2022-03-14 13:13:40.198238 aiida-hyperqueue-0.1.0/tests/test_scheduler.py
--rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 aiida-hyperqueue-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1321 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2085 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1611 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/.github/workflows/validate_release_tag.py
+-rw-r--r--   0        0        0      115 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/.gitignore
+-rw-r--r--   0        0        0      728 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      119 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/.readthedocs.yml
+-rw-r--r--   0        0        0      195 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1014 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/README.md
+-rw-r--r--   0        0        0      119 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/aiida_hyperqueue/__init__.py
+-rw-r--r--   0        0        0     4396 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/aiida_hyperqueue/cli.py
+-rw-r--r--   0        0        0    10759 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/aiida_hyperqueue/scheduler.py
+-rw-r--r--   0        0        0        7 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/docs/.gitignore
+-rwxr-xr-x   0        0        0     1541 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/docs/Makefile
+-rwxr-xr-x   0        0        0     5462 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0     2785 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/docs/source/developer_guide/index.md
+-rw-r--r--   0        0        0     6116 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/docs/source/get_started.md
+-rw-r--r--   0        0        0    76300 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/docs/source/img/AiiDA_transparent_logo.png
+-rw-r--r--   0        0        0     1837 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/docs/source/index.md
+-rw-r--r--   0        0        0     1737 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      239 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      363 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0      485 2023-05-11 01:17:44.940708 aiida-hyperqueue-0.1.1/tests/test_scheduler.py
+-rw-r--r--   0        0        0     2284 1970-01-01 00:00:00.000000 aiida-hyperqueue-0.1.1/PKG-INFO
```

### Comparing `aiida-hyperqueue-0.1.0/.github/workflows/ci.yml` & `aiida-hyperqueue-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida-hyperqueue-0.1.0/.pre-commit-config.yaml` & `aiida-hyperqueue-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida-hyperqueue-0.1.0/LICENSE` & `aiida-hyperqueue-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida-hyperqueue-0.1.0/README.md` & `aiida-hyperqueue-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![Build Status](https://github.com/aiidateam/aiida-hyperqueue/workflows/ci/badge.svg?branch=main)](https://github.com/aiidateam/aiida-hyperqueue/actions)
 [![Docs status](https://readthedocs.org/projects/aiida-hyperqueue/badge)](http://aiida-hyperqueue.readthedocs.io/)
-<!-- [![PyPI version](https://badge.fury.io/py/aiida-hyperqueue.svg)](https://badge.fury.io/py/aiida-hyperqueue) -->
+[![PyPI version](https://badge.fury.io/py/aiida-hyperqueue.svg)](https://badge.fury.io/py/aiida-hyperqueue)
 
 # AiiDA HyperQueue plugin
 
 AiiDA plugin for the [HyperQueue](https://github.com/It4innovations/hyperqueue) metascheduler.
 
 | ❗️ This package is still in the early stages of development and we will most likely break the API regularly in new 0.X versions. Be sure to pin the version when installing this package in scripts.|
 |---|
```

### Comparing `aiida-hyperqueue-0.1.0/aiida_hyperqueue/cli.py` & `aiida-hyperqueue-0.1.1/aiida_hyperqueue/cli.py`

 * *Files identical despite different names*

### Comparing `aiida-hyperqueue-0.1.0/aiida_hyperqueue/scheduler.py` & `aiida-hyperqueue-0.1.1/aiida_hyperqueue/scheduler.py`

 * *Files identical despite different names*

### Comparing `aiida-hyperqueue-0.1.0/docs/Makefile` & `aiida-hyperqueue-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida-hyperqueue-0.1.0/docs/source/conf.py` & `aiida-hyperqueue-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aiida-hyperqueue-0.1.0/docs/source/developer_guide/index.md` & `aiida-hyperqueue-0.1.1/docs/source/developer_guide/index.md`

 * *Files identical despite different names*

### Comparing `aiida-hyperqueue-0.1.0/docs/source/get_started.md` & `aiida-hyperqueue-0.1.1/docs/source/get_started.md`

 * *Files identical despite different names*

### Comparing `aiida-hyperqueue-0.1.0/docs/source/img/AiiDA_transparent_logo.png` & `aiida-hyperqueue-0.1.1/docs/source/img/AiiDA_transparent_logo.png`

 * *Files identical despite different names*

### Comparing `aiida-hyperqueue-0.1.0/docs/source/index.md` & `aiida-hyperqueue-0.1.1/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `aiida-hyperqueue-0.1.0/pyproject.toml` & `aiida-hyperqueue-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["flit_core>=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "aiida-hyperqueue"
-version = "0.1.0"
+dynamic = ['version']
+description = "AiiDA plugin for the HyperQueue metascheduler"
 authors = [
   {name = "Marnik Bercx"}
 ]
-description = "AiiDA plugin for the HyperQueue metascheduler"
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Framework :: AiiDA",
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `aiida-hyperqueue-0.1.0/PKG-INFO` & `aiida-hyperqueue-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-hyperqueue
-Version: 0.1.0
+Version: 0.1.1
 Summary: AiiDA plugin for the HyperQueue metascheduler
 Author: Marnik Bercx
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Framework :: AiiDA
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -28,15 +28,15 @@
 Project-URL: Source, https://github.com/aiidateam/aiida-hyperqueue
 Provides-Extra: docs
 Provides-Extra: pre-commit
 Provides-Extra: tests
 
 [![Build Status](https://github.com/aiidateam/aiida-hyperqueue/workflows/ci/badge.svg?branch=main)](https://github.com/aiidateam/aiida-hyperqueue/actions)
 [![Docs status](https://readthedocs.org/projects/aiida-hyperqueue/badge)](http://aiida-hyperqueue.readthedocs.io/)
-<!-- [![PyPI version](https://badge.fury.io/py/aiida-hyperqueue.svg)](https://badge.fury.io/py/aiida-hyperqueue) -->
+[![PyPI version](https://badge.fury.io/py/aiida-hyperqueue.svg)](https://badge.fury.io/py/aiida-hyperqueue)
 
 # AiiDA HyperQueue plugin
 
 AiiDA plugin for the [HyperQueue](https://github.com/It4innovations/hyperqueue) metascheduler.
 
 | ❗️ This package is still in the early stages of development and we will most likely break the API regularly in new 0.X versions. Be sure to pin the version when installing this package in scripts.|
 |---|
```

