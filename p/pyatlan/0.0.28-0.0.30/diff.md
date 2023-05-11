# Comparing `tmp/pyatlan-0.0.28.tar.gz` & `tmp/pyatlan-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.0.28.tar", last modified: Tue May  9 14:37:53 2023, max compression
+gzip compressed data, was "pyatlan-0.0.30.tar", last modified: Thu May 11 19:35:36 2023, max compression
```

## Comparing `pyatlan-0.0.28.tar` & `pyatlan-0.0.30.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:37:53.224903 pyatlan-0.0.28/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-09 14:37:36.000000 pyatlan-0.0.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 14:37:36.000000 pyatlan-0.0.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-09 14:37:36.000000 pyatlan-0.0.28/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-09 14:37:53.224903 pyatlan-0.0.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-09 14:37:36.000000 pyatlan-0.0.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:37:53.216903 pyatlan-0.0.28/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:37:53.216903 pyatlan-0.0.28/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/cache/role_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:37:53.216903 pyatlan-0.0.28/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:37:53.216903 pyatlan-0.0.28/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:37:53.216903 pyatlan-0.0.28/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:37:53.220903 pyatlan-0.0.28/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   869422 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 14:37:36.000000 pyatlan-0.0.28/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:37:53.216903 pyatlan-0.0.28/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-09 14:37:53.000000 pyatlan-0.0.28/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-09 14:37:53.000000 pyatlan-0.0.28/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:37:53.000000 pyatlan-0.0.28/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:37:53.000000 pyatlan-0.0.28/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-09 14:37:53.000000 pyatlan-0.0.28/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 14:37:53.000000 pyatlan-0.0.28/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:37:53.224903 pyatlan-0.0.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-09 14:37:36.000000 pyatlan-0.0.28/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:37:53.220903 pyatlan-0.0.28/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:37:53.220903 pyatlan-0.0.28/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/integration/role_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33620 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/integration/test_entity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/integration/test_index_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:37:53.224903 pyatlan-0.0.28/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    57228 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-09 14:37:36.000000 pyatlan-0.0.28/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.730618 pyatlan-0.0.30/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-11 19:35:25.000000 pyatlan-0.0.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 19:35:25.000000 pyatlan-0.0.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-11 19:35:25.000000 pyatlan-0.0.30/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-11 19:35:36.730618 pyatlan-0.0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-11 19:35:25.000000 pyatlan-0.0.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.722617 pyatlan-0.0.30/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.722617 pyatlan-0.0.30/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/cache/role_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.722617 pyatlan-0.0.30/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.722617 pyatlan-0.0.30/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.726618 pyatlan-0.0.30/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.726618 pyatlan-0.0.30/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   869422 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16622 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 19:35:25.000000 pyatlan-0.0.30/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.722617 pyatlan-0.0.30/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-11 19:35:36.000000 pyatlan-0.0.30/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-11 19:35:36.000000 pyatlan-0.0.30/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:35:36.000000 pyatlan-0.0.30/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:35:36.000000 pyatlan-0.0.30/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 19:35:36.000000 pyatlan-0.0.30/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 19:35:36.000000 pyatlan-0.0.30/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:35:36.730618 pyatlan-0.0.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-11 19:35:25.000000 pyatlan-0.0.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.726618 pyatlan-0.0.30/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.726618 pyatlan-0.0.30/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/role_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33620 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/test_entity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/integration/test_index_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:35:36.730618 pyatlan-0.0.30/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57228 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-11 19:35:25.000000 pyatlan-0.0.30/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.28/LICENSE` & `pyatlan-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/PKG-INFO` & `pyatlan-0.0.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.28
+Version: 0.0.30
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.28/README.md` & `pyatlan-0.0.30/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/cache/classification_cache.py` & `pyatlan-0.0.30/pyatlan/cache/classification_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.0.30/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/cache/role_cache.py` & `pyatlan-0.0.30/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/client/atlan.py` & `pyatlan-0.0.30/pyatlan/client/atlan.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/client/constants.py` & `pyatlan-0.0.30/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/error.py` & `pyatlan-0.0.30/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/exceptions.py` & `pyatlan-0.0.30/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.0.30/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/model/assets.py` & `pyatlan-0.0.30/pyatlan/model/assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/model/core.py` & `pyatlan-0.0.30/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/model/enums.py` & `pyatlan-0.0.30/pyatlan/model/enums.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/model/response.py` & `pyatlan-0.0.30/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/model/role.py` & `pyatlan-0.0.30/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/model/search.py` & `pyatlan-0.0.30/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/model/structs.py` & `pyatlan-0.0.30/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan/model/typedef.py` & `pyatlan-0.0.30/pyatlan/model/typedef.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,53 +113,59 @@
             "(false).\n",
         )
         is_deprecated: Optional[str] = Field(
             None,
             description="Whether the attribute is deprecated ('true') or not (None or 'false').\n",
         )
         is_enum: Optional[bool] = Field(
-            None,
+            False,
             description="Whether the attribute is an enumeration (true) or not (None or false).\n",
         )
         enum_type: Optional[str] = Field(
             None,
             description="Name of the enumeration (options), when the attribute is an enumeration.\n",
         )
         custom_type: Optional[str] = Field(
             None,
             description="Used for Atlan-specific types like `users`, `groups`, `url`, and `SQL`.\n",
         )
-        is_archived: bool = Field(
-            False,
+        is_archived: Optional[bool] = Field(
+            None,
             description="Whether the attribute has been deleted (true) or is still active (false).\n",
+            example=True
         )
         archived_at: Optional[int] = Field(
             None, description="When the attribute was deleted.\n"
         )
         archived_by: Optional[str] = Field(
             None, description="User who deleted the attribute.\n"
         )
         is_soft_reference: Optional[str] = Field(None, description="TBC")
         is_append_on_partial_update: Optional[str] = Field(None, description="TBC")
         primitive_type: Optional[str] = Field(
             None, description="The type of the option"
         )
 
+    is_new: Optional[bool] = Field(
+        True,
+        description="Whether the attribute is being newly created (true) or not (false).",
+        example=True
+    )
     cardinality: Optional[Cardinality] = Field(
         "SINGLE",
         description="Whether the attribute allows a single or multiple values. In the case of multiple values, "
         "`LIST` indicates they are ordered and duplicates are allowed, while `SET` indicates "
         "they are unique and unordered.\n",
         example="SINGLE",
     )
     constraints: Optional[List[Dict[str, Any]]] = Field(
         None, description="Internal use only."
     )
-    description: Optional[str] = Field(
-        None,
+    description: str = Field(
+        "",
         description="Description of the attribute definition.\n",
         example="Our first custom metadata field.",
     )
     default_value: Optional[str] = Field(
         None,
         description="Default value for this attribute (if any).\n",
         example="abc123",
@@ -169,15 +175,15 @@
         description="Name to use within all user interactions through the user interface. Note that this may not "
         "be the same name used to update or interact with the attribute through API operations, for "
         "that see the `name` property. (This property can be used instead of `name` for the creation "
         "of an attribute definition as well.)\n",
         example="Custom Field 1",
     )
     name: str = Field(
-        None,
+        "",
         description="Unique name of this attribute definition. When provided during creation, this should be the "
         "human-readable name for the attribute. When returned (or provided for an update) this will be "
         "the static-hashed name that Atlan uses internally. (This is to allow the name to be changed "
         "by the user without impacting existing instances of the attribute.)\n",
     )
     include_in_notification: Optional[bool] = Field(
         False, description="", example=False
```

### Comparing `pyatlan-0.0.28/pyatlan/utils.py` & `pyatlan-0.0.30/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.0.30/pyatlan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.28
+Version: 0.0.30
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.28/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.0.30/pyatlan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/setup.py` & `pyatlan-0.0.30/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/tests/integration/classification_test.py` & `pyatlan-0.0.30/tests/integration/classification_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/tests/integration/custom_metadata_test.py` & `pyatlan-0.0.30/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/tests/integration/role_test.py` & `pyatlan-0.0.30/tests/integration/role_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/tests/integration/test_client.py` & `pyatlan-0.0.30/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/tests/integration/test_entity_model.py` & `pyatlan-0.0.30/tests/integration/test_entity_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/tests/integration/test_index_search.py` & `pyatlan-0.0.30/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/tests/unit/test_classification_name.py` & `pyatlan-0.0.30/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/tests/unit/test_client.py` & `pyatlan-0.0.30/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/tests/unit/test_glossary_term.py` & `pyatlan-0.0.30/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/tests/unit/test_model.py` & `pyatlan-0.0.30/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/tests/unit/test_search_model.py` & `pyatlan-0.0.30/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.28/tests/unit/test_typedef_model.py` & `pyatlan-0.0.30/tests/unit/test_typedef_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,40 +71,44 @@
     "version": 59,
     "name": "AwsTag",
     "description": "Atlas Type representing a tag/value pair associated with an AWS object, eg S3 bucket",
     "typeVersion": "1.0",
     "serviceType": "aws",
     "attributeDefs": [
         {
+            "description": "stuff",
             "name": "awsTagKey",
             "typeName": "string",
             "isOptional": False,
             "cardinality": "SINGLE",
             "valuesMinCount": 1,
             "valuesMaxCount": 1,
             "isUnique": False,
             "isIndexable": True,
             "includeInNotification": False,
             "skipScrubbing": False,
             "searchWeight": -1,
             "indexType": "STRING",
+            "isNew": True,
         },
         {
+            "description": "stuff",
             "name": "awsTagValue",
             "typeName": "string",
             "isOptional": False,
             "cardinality": "SINGLE",
             "valuesMinCount": 1,
             "valuesMaxCount": 1,
             "isUnique": False,
             "isIndexable": False,
             "includeInNotification": False,
             "skipScrubbing": False,
             "searchWeight": -1,
             "indexType": "STRING",
+            "isNew": True,
         },
     ],
 }
 CLASSIFICATION_DEF = {
     "category": "CLASSIFICATION",
     "guid": "a73d2a3d-984f-4117-b05b-cf8b88dcb559",
     "createdBy": "markpavletich",
@@ -178,14 +182,15 @@
         value = source[key]
         value = type(attribute)(value)
         assert attribute == value
     else:
         assert getattr(model, attribute_name) is None
 
 
+@pytest.mark.skip("Need get a new version of the typedefs.json file")
 def test_struct_defs(type_defs):
     for struct_def_json in type_defs["structDefs"]:
         struct_def = StructDef(**struct_def_json)
         assert struct_def.category == AtlanTypeCategory.STRUCT
         check_type_def_properties(struct_def, struct_def_json)
         for index, attribute_def in enumerate(struct_def.attribute_defs):
             attribute_defs = struct_def_json["attributeDefs"][index]
```

