# Comparing `tmp/pydantic-kedro-0.3.0.tar.gz` & `tmp/pydantic-kedro-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-kedro-0.3.0.tar", last modified: Wed May 10 21:11:03 2023, max compression
+gzip compressed data, was "pydantic-kedro-0.4.0.tar", last modified: Thu May 11 00:23:30 2023, max compression
```

## Comparing `pydantic-kedro-0.3.0.tar` & `pydantic-kedro-0.4.0.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.232605 pydantic-kedro-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.232605 pydantic-kedro-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.github/workflows/python-testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.232605 pydantic-kedro-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/docs/arbitrary_types.md
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/docs/implementation_details.md
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/docs/reference.md
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/docs/standalone_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.228605 pydantic-kedro-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.232605 pydantic-kedro-0.3.0/src/pydantic_kedro/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-10 21:11:03.000000 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-10 21:11:03.000000 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:11:03.000000 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:10:05.000000 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 21:11:03.000000 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 21:11:03.000000 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/test/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.232605 pydantic-kedro-0.3.0/src/test/catalogs/conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/test/catalogs/conf/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/catalogs/conf/base/catalog.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/test/catalogs/conf/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/catalogs/conf/local/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/catalogs/conf/local/credentials.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/test/catalogs/data/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/catalogs/data/tst1.json
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/catalogs/test_basic_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_docs_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_ds_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_ds_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_ds_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.086284 pydantic-kedro-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.078284 pydantic-kedro-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.078284 pydantic-kedro-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.github/workflows/python-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-11 00:23:30.086284 pydantic-kedro-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.078284 pydantic-kedro-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/docs/arbitrary_types.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/docs/implementation_details.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/docs/reference.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/docs/standalone_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 00:23:30.086284 pydantic-kedro-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.074284 pydantic-kedro-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.082284 pydantic-kedro-0.4.0/src/pydantic_kedro/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/_internals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.082284 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/pydantic_kedro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.082284 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-11 00:23:29.000000 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-11 00:23:30.000000 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:23:29.000000 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:22:28.000000 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 00:23:29.000000 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 00:23:29.000000 pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.082284 pydantic-kedro-0.4.0/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.082284 pydantic-kedro-0.4.0/src/test/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.078284 pydantic-kedro-0.4.0/src/test/catalogs/conf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.082284 pydantic-kedro-0.4.0/src/test/catalogs/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/catalogs/conf/base/catalog.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.086284 pydantic-kedro-0.4.0/src/test/catalogs/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/catalogs/conf/local/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/catalogs/conf/local/credentials.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:23:30.086284 pydantic-kedro-0.4.0/src/test/catalogs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/catalogs/data/tst1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/catalogs/test_basic_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_docs_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_ds_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_ds_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_ds_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 00:22:13.000000 pydantic-kedro-0.4.0/src/test/test_utils.py
```

### Comparing `pydantic-kedro-0.3.0/.github/dependabot.yml` & `pydantic-kedro-0.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/.github/workflows/python-publish.yml` & `pydantic-kedro-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/.github/workflows/python-testing.yml` & `pydantic-kedro-0.4.0/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/.pre-commit-config.yaml` & `pydantic-kedro-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/LICENSE` & `pydantic-kedro-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/PKG-INFO` & `pydantic-kedro-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.3.0
+Version: 0.4.0
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pydantic-kedro-0.3.0/README.md` & `pydantic-kedro-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/docs/arbitrary_types.md` & `pydantic-kedro-0.4.0/docs/arbitrary_types.md`

 * *Files 11% similar despite different names*

```diff
@@ -122,19 +122,43 @@
 ```
 
 Internally, this uses the `ParquetDataSet` to save the dataframe as an
 [Apache Parquet](https://parquet.apache.org/) file within the Zip file,
 as well as reference it from within the JSON file. That means that, unlike
 Pickle, the file isn't "fragile" and will be readable with future versions.
 
-## Known Issues
+## Config Inheritence
 
-1. Currently, the `Config` is not magically inherited by subclasses.
-   That means that you should explicitly inherit `YourType.Config` from `YourType`'s
-   base class if you want to override it. It also means that the `kedro_map`
-   isn't merged for subclasses; you'll need to do this explicitly for now.
-2. Only the top-level model's `Config` is taken into account when serializing
+[Similarly to Pydantic](https://docs.pydantic.dev/latest/usage/model_config/#change-behaviour-globally),
+the `Config` class has a sort of pseudo-inheritence.
+That is, if you define your classes like this:
+
+```python
+class A(BaseModel):
+    class Config:
+        allow_arbitrary_types = True
+        kedro_map = {Foo: FooDataSet}
+
+
+class B(A):
+    class Config:
+        kedro_map = {Bar: BarDataSet}
+
+class C(B):
+    class Config:
+        kedro_map = {Foo: foo_ds_maker}
+        kedro_default = DefaultDataSet
+
+```
+
+Then class `B` will act as if `kedro_map = {Foo: FooDataSet, Bar: BarDataSet}`,
+and class `C` will act as if `kedro_map = {Foo: foo_ds_maker, Bar: BarDataSet}`
+and `kedro_default = DefaultDataSet`
+
+## Considerations
+
+1. Only the top-level model's `Config` is taken into account when serializing
    to a Kedro dataset, ignoring any children's configs.
    This means that all values of a particular type are serialized the same way.
-3. `pydantic` V2 is not supported yet, but V2
+2. `pydantic` V2 is not supported yet, but V2
    [has a different configuration method](https://docs.pydantic.dev/blog/pydantic-v2-alpha/#changes-to-config).
    `pydantic-kedro` might change the configuration method entirely to be more compliant.
```

### Comparing `pydantic-kedro-0.3.0/docs/implementation_details.md` & `pydantic-kedro-0.4.0/docs/implementation_details.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/docs/index.md` & `pydantic-kedro-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/docs/standalone_usage.md` & `pydantic-kedro-0.4.0/docs/standalone_usage.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/mkdocs.yml` & `pydantic-kedro-0.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/pyproject.toml` & `pydantic-kedro-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/src/pydantic_kedro/__init__.py` & `pydantic-kedro-0.4.0/src/pydantic_kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/auto.py` & `pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/auto.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/folder.py` & `pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/folder.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,40 +9,48 @@
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 from uuid import uuid4
 
 import fsspec
 from fsspec import AbstractFileSystem
 from fsspec.core import strip_protocol
 from fsspec.implementations.local import LocalFileSystem
-from kedro.extras.datasets.pickle import PickleDataSet
 from kedro.io.core import AbstractDataSet, parse_dataset_definition
 from pydantic import BaseConfig, BaseModel, Extra, Field
 from pydantic.utils import import_string
 
-# __all__ = ["PydanticFolderDataSet"]
+from pydantic_kedro._internals import get_kedro_default, get_kedro_map
+
+__all__ = ["PydanticFolderDataSet"]
 
 
 DATA_PLACEHOLDER = "__DATA_PLACEHOLDER__"
 
 JsonPath = str  # not a "real" JSON Path, but just `.`-separated
-_Bis = Union[bool, int, str, Path, None]
 
 logger = logging.getLogger(__name__)
 
+# Some ridiculous types to support nested configurations
+_Bis = Union[bool, int, str, Path, None]
+_Dis1 = Dict[str, _Bis]
+_Dis2 = Dict[str, Union[_Bis, _Dis1]]
+_Dis3 = Dict[str, Union[_Bis, _Dis1, _Dis2]]
+_Dis4 = Dict[str, Union[_Bis, _Dis1, _Dis2, _Dis3]]
+# basically, Dict[str, Union[_Bis, Dict[str, Union[_Bis, Dict[str, _Bis]]]]], but better :)
+
 
 class KedroDataSetSpec(BaseModel):
     """Kedro dataset specification. This allows arbitrary extra fields, including versions.
 
     Unfortunately, because there's no standard on how to specify "file paths", this will likely fail
     in many cases where it "should" work.
     """
 
     type_: str = Field(alias="type")
     relative_path: str
-    args: Dict[str, Union[_Bis, Dict[str, Dict[str, _Bis]]]] = {}
+    args: _Dis4 = {}
 
     class Config(BaseConfig):
         """Internal Pydantic model configuration."""
 
         allow_population_by_field_name = True
         extra = Extra.allow
         smart_union = True
@@ -248,20 +256,16 @@
         kls = type(data)
         model_class_str = get_import_name(kls)
         model_info: Union[Dict[str, Any], List[Any]] = {}
         catalog: Dict[JsonPath, KedroDataSetSpec] = {}
 
         # These are used to make datasets for various types
         # See the `kls.Config` class - this is inherited
-        kedro_map: Dict[Type, Callable[[str], AbstractDataSet]] = getattr(
-            kls.__config__, "kedro_map", {}
-        )
-        kedro_default: Callable[[str], AbstractDataSet] = getattr(
-            kls.__config__, "kedro_default", PickleDataSet
-        )
+        kedro_map: Dict[Type, Callable[[str], AbstractDataSet]] = get_kedro_map(kls)
+        kedro_default: Callable[[str], AbstractDataSet] = get_kedro_default(kls)
 
         def make_ds_for(obj: Any, path: str) -> AbstractDataSet:
             for k, v in kedro_map.items():
                 if isinstance(obj, k):
                     return v(path)
             warnings.warn(
                 f"No dataset defined for {get_import_name(type(obj))} in `Config.kedro_map`;"
```

### Comparing `pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/json.py` & `pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/yaml.py` & `pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/yaml.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/zip.py` & `pydantic-kedro-0.4.0/src/pydantic_kedro/datasets/zip.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/src/pydantic_kedro/utils.py` & `pydantic-kedro-0.4.0/src/pydantic_kedro/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     Parameters
     ----------
     model : BaseModel
         Pydantic model to save. This can be 'pure' (JSON-safe) or 'arbitrary'.
     uri : str
         The path or URI to save the model to.
     format : {"auto", "zip", "folder", "yaml", "json"}
-        The dataset format to use. "auto" will use [PydanticAutoDataSet][].
+        The dataset format to use.
+        "auto" will use [PydanticAutoDataSet][pydantic_kedro.PydanticAutoDataSet].
     """
     if not isinstance(model, BaseModel):
         raise TypeError(f"Expected Pydantic model, but got {model!r}")
     ds: AbstractDataSet
     if format == "auto":
         ds = PydanticAutoDataSet(uri)
     elif format == "zip":
```

### Comparing `pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/PKG-INFO` & `pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.3.0
+Version: 0.4.0
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/SOURCES.txt` & `pydantic-kedro-0.4.0/src/pydantic_kedro.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 .github/workflows/python-testing.yml
 docs/arbitrary_types.md
 docs/implementation_details.md
 docs/index.md
 docs/reference.md
 docs/standalone_usage.md
 src/pydantic_kedro/__init__.py
+src/pydantic_kedro/_internals.py
 src/pydantic_kedro/models.py
 src/pydantic_kedro/py.typed
 src/pydantic_kedro/utils.py
 src/pydantic_kedro/version.py
 src/pydantic_kedro.egg-info/PKG-INFO
 src/pydantic_kedro.egg-info/SOURCES.txt
 src/pydantic_kedro.egg-info/dependency_links.txt
@@ -35,13 +36,14 @@
 src/pydantic_kedro/datasets/zip.py
 src/test/test_auto.py
 src/test/test_docs_standalone.py
 src/test/test_ds_extended.py
 src/test/test_ds_pandas.py
 src/test/test_ds_simple.py
 src/test/test_import.py
+src/test/test_inheritance.py
 src/test/test_utils.py
 src/test/catalogs/test_basic_catalog.py
 src/test/catalogs/conf/base/catalog.yml
 src/test/catalogs/conf/local/.gitkeep
 src/test/catalogs/conf/local/credentials.yml
 src/test/catalogs/data/tst1.json
```

### Comparing `pydantic-kedro-0.3.0/src/test/catalogs/test_basic_catalog.py` & `pydantic-kedro-0.4.0/src/test/catalogs/test_basic_catalog.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/src/test/test_auto.py` & `pydantic-kedro-0.4.0/src/test/test_auto.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/src/test/test_docs_standalone.py` & `pydantic-kedro-0.4.0/src/test/test_docs_standalone.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/src/test/test_ds_extended.py` & `pydantic-kedro-0.4.0/src/test/test_ds_extended.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.3.0/src/test/test_ds_pandas.py` & `pydantic-kedro-0.4.0/src/test/test_ds_pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pydantic_kedro import (
     ArbModel,
     PydanticAutoDataSet,
     PydanticFolderDataSet,
     PydanticZipDataSet,
 )
 
-Kls = Union[PydanticFolderDataSet, PydanticZipDataSet]
+Kls = Union[PydanticAutoDataSet, PydanticFolderDataSet, PydanticZipDataSet]
 
 dfx = pd.DataFrame([[1, 2, 3]], columns=["a", "b", "c"])
 
 
 class _PdModel(ArbModel):
     """Pandas model, configured to use Parquet."""
```

### Comparing `pydantic-kedro-0.3.0/src/test/test_ds_simple.py` & `pydantic-kedro-0.4.0/src/test/test_ds_simple.py`

 * *Files identical despite different names*

