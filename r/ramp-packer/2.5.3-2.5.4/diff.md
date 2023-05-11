# Comparing `tmp/ramp_packer-2.5.3.tar.gz` & `tmp/ramp_packer-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramp_packer-2.5.3.tar", max compression
+gzip compressed data, was "ramp_packer-2.5.4.tar", max compression
```

## Comparing `ramp_packer-2.5.3.tar` & `ramp_packer-2.5.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1310 2023-03-21 11:17:23.842096 ramp_packer-2.5.3/LICENSE
--rw-r--r--   0        0        0        0 2023-03-21 11:17:23.842096 ramp_packer-2.5.3/RAMP/__init__.py
--rw-r--r--   0        0        0     4138 2023-03-21 11:17:23.846096 ramp_packer-2.5.3/RAMP/commands_discovery.py
--rw-r--r--   0        0        0      920 2023-03-21 11:17:23.846096 ramp_packer-2.5.3/RAMP/common.py
--rw-r--r--   0        0        0      310 2023-03-21 11:17:23.846096 ramp_packer-2.5.3/RAMP/config.py
--rw-r--r--   0        0        0     3196 2023-03-21 11:17:23.846096 ramp_packer-2.5.3/RAMP/disposableredis/__init__.py
--rw-r--r--   0        0        0     3598 2023-03-21 11:17:23.846096 ramp_packer-2.5.3/RAMP/module_metadata.py
--rw-r--r--   0        0        0     7156 2023-03-21 11:17:23.846096 ramp_packer-2.5.3/RAMP/packer.py
--rwxr-xr-x   0        0        0     4891 2023-03-21 11:17:23.846096 ramp_packer-2.5.3/RAMP/ramp.py
--rw-r--r--   0        0        0     6885 2023-03-21 11:17:23.846096 ramp_packer-2.5.3/RAMP/unpacker.py
--rw-r--r--   0        0        0      127 2023-03-21 11:17:23.846096 ramp_packer-2.5.3/RAMP/version.py
--rw-r--r--   0        0        0     4962 2023-03-21 11:17:23.846096 ramp_packer-2.5.3/README.md
--rw-r--r--   0        0        0     1018 2023-03-21 11:17:24.646093 ramp_packer-2.5.3/pyproject.toml
--rw-r--r--   0        0        0     6164 1970-01-01 00:00:00.000000 ramp_packer-2.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1310 2023-05-11 06:34:17.535764 ramp_packer-2.5.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-11 06:34:17.535764 ramp_packer-2.5.4/RAMP/__init__.py
+-rw-r--r--   0        0        0     4138 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/commands_discovery.py
+-rw-r--r--   0        0        0      920 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/common.py
+-rw-r--r--   0        0        0      310 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/config.py
+-rw-r--r--   0        0        0     3196 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/disposableredis/__init__.py
+-rw-r--r--   0        0        0     3598 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/module_metadata.py
+-rw-r--r--   0        0        0     7156 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/packer.py
+-rwxr-xr-x   0        0        0     4891 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/ramp.py
+-rw-r--r--   0        0        0     6885 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/unpacker.py
+-rw-r--r--   0        0        0      127 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/RAMP/version.py
+-rw-r--r--   0        0        0     4962 2023-05-11 06:34:17.539764 ramp_packer-2.5.4/README.md
+-rw-r--r--   0        0        0     1020 2023-05-11 06:34:18.427787 ramp_packer-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0     6157 1970-01-01 00:00:00.000000 ramp_packer-2.5.4/PKG-INFO
```

### Comparing `ramp_packer-2.5.3/LICENSE` & `ramp_packer-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.3/RAMP/commands_discovery.py` & `ramp_packer-2.5.4/RAMP/commands_discovery.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.3/RAMP/common.py` & `ramp_packer-2.5.4/RAMP/common.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.3/RAMP/disposableredis/__init__.py` & `ramp_packer-2.5.4/RAMP/disposableredis/__init__.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.3/RAMP/module_metadata.py` & `ramp_packer-2.5.4/RAMP/module_metadata.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.3/RAMP/packer.py` & `ramp_packer-2.5.4/RAMP/packer.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.3/RAMP/ramp.py` & `ramp_packer-2.5.4/RAMP/ramp.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.3/RAMP/unpacker.py` & `ramp_packer-2.5.4/RAMP/unpacker.py`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.3/README.md` & `ramp_packer-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `ramp_packer-2.5.3/pyproject.toml` & `ramp_packer-2.5.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ramp-packer"
-version = "2.5.3"
+version = "2.5.4"
 description = "Packs for Redis modules into a distributable format"
 authors = [ "Redis OSS <oss@redis.com>" ]
 license = "BSD-2-Clause"
 readme = "README.md"
 classifiers = [
   "Topic :: Database",
   "Programming Language :: Python",
@@ -24,15 +24,15 @@
   [tool.poetry.scripts]
   ramp = "RAMP.ramp:ramp"
 
   [tool.poetry.dependencies]
   python = ">= 3.7,<4"
   click = "^8"
   semantic-version = "^2.8.5"
-  redis = "^4.1.0"
+  redis = ">= 4.1.0"
   PyYAML = "^6.0"
   distro = "^1.8"
 
   [tool.poetry.dev-dependencies]
   coverage = "^5.4"
 
 [build-system]
```

### Comparing `ramp_packer-2.5.3/PKG-INFO` & `ramp_packer-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramp-packer
-Version: 2.5.3
+Version: 2.5.4
 Summary: Packs for Redis modules into a distributable format
 License: BSD-2-Clause
 Author: Redis OSS
 Author-email: oss@redis.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8,<9)
 Requires-Dist: distro (>=1.8,<2.0)
-Requires-Dist: redis (>=4.1.0,<5.0.0)
+Requires-Dist: redis (>=4.1.0)
 Requires-Dist: semantic-version (>=2.8.5,<3.0.0)
 Description-Content-Type: text/markdown
 
 [![license](https://img.shields.io/github/license/RedisLabsModules/RAMP.svg)](https://github.com/RedisLabsModules/RAMP)
 [![CI](https://github.com/redislabsmodules/ramp/workflows/CI/badge.svg?branch=master)](https://github.com/redislabsmodules/ramp/actions?query=workflow%3ACI+branch%3Amaster)
 [![GitHub issues](https://img.shields.io/github/release/RedisLabsModules/RAMP.svg)](https://github.com/RedisLabsModules/RAMP/releases/latest)
 [![Codecov](https://codecov.io/gh/RedisLabsModules/RAMP/branch/master/graph/badge.svg)](https://codecov.io/gh/RedisLabsModules/RAMP)
```

