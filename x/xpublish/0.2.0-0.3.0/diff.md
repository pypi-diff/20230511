# Comparing `tmp/xpublish-0.2.0.tar.gz` & `tmp/xpublish-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpublish-0.2.0.tar", last modified: Mon Jul 18 19:24:07 2022, max compression
+gzip compressed data, was "xpublish-0.3.0.tar", last modified: Thu May 11 14:29:36 2023, max compression
```

## Comparing `xpublish-0.2.0.tar` & `xpublish-0.3.0.tar`

### file list

```diff
@@ -1,67 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 19:24:07.036990 xpublish-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 19:24:07.024990 xpublish-0.2.0/.binder/
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-18 19:23:56.000000 xpublish-0.2.0/.binder/dask_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-07-18 19:23:56.000000 xpublish-0.2.0/.binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-07-18 19:23:56.000000 xpublish-0.2.0/.binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-07-18 19:23:56.000000 xpublish-0.2.0/.binder/start
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-07-18 19:23:56.000000 xpublish-0.2.0/.binder/test.py
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-07-18 19:23:56.000000 xpublish-0.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 19:24:07.024990 xpublish-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-07-18 19:23:56.000000 xpublish-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 19:24:07.024990 xpublish-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2328 2022-07-18 19:23:56.000000 xpublish-0.2.0/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-07-18 19:23:56.000000 xpublish-0.2.0/.github/workflows/pypipublish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-07-18 19:23:56.000000 xpublish-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-07-18 19:23:56.000000 xpublish-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-07-18 19:23:56.000000 xpublish-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11378 2022-07-18 19:23:56.000000 xpublish-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-07-18 19:24:07.036990 xpublish-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-07-18 19:23:56.000000 xpublish-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-07-18 19:23:56.000000 xpublish-0.2.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-07-18 19:23:56.000000 xpublish-0.2.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 19:24:07.028990 xpublish-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6788 2022-07-18 19:23:56.000000 xpublish-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     6467 2022-07-18 19:23:56.000000 xpublish-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-07-18 19:23:56.000000 xpublish-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 19:24:07.028990 xpublish-0.2.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-07-18 19:23:56.000000 xpublish-0.2.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9034 2022-07-18 19:23:56.000000 xpublish-0.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4288 2022-07-18 19:23:56.000000 xpublish-0.2.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2174 2022-07-18 19:23:56.000000 xpublish-0.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-18 19:23:56.000000 xpublish-0.2.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6977 2022-07-18 19:23:56.000000 xpublish-0.2.0/docs/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 19:24:07.028990 xpublish-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     5644 2022-07-18 19:23:56.000000 xpublish-0.2.0/examples/open_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-07-18 19:23:56.000000 xpublish-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-07-18 19:24:07.036990 xpublish-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-07-18 19:23:56.000000 xpublish-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 19:24:07.032990 xpublish-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 19:23:56.000000 xpublish-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-07-18 19:23:56.000000 xpublish-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3536 2022-07-18 19:23:56.000000 xpublish-0.2.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-07-18 19:23:56.000000 xpublish-0.2.0/tests/test_fsspec_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     8410 2022-07-18 19:23:56.000000 xpublish-0.2.0/tests/test_rest_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4525 2022-07-18 19:23:56.000000 xpublish-0.2.0/tests/test_zarr_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-07-18 19:23:56.000000 xpublish-0.2.0/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 19:24:07.032990 xpublish-0.2.0/xpublish/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-07-18 19:23:56.000000 xpublish-0.2.0/xpublish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2022-07-18 19:23:56.000000 xpublish-0.2.0/xpublish/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     7992 2022-07-18 19:23:56.000000 xpublish-0.2.0/xpublish/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 19:24:07.036990 xpublish-0.2.0/xpublish/routers/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-07-18 19:23:56.000000 xpublish-0.2.0/xpublish/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-07-18 19:23:56.000000 xpublish-0.2.0/xpublish/routers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-07-18 19:23:56.000000 xpublish-0.2.0/xpublish/routers/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2740 2022-07-18 19:23:56.000000 xpublish-0.2.0/xpublish/routers/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 19:24:07.036990 xpublish-0.2.0/xpublish/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 19:23:56.000000 xpublish-0.2.0/xpublish/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3747 2022-07-18 19:23:56.000000 xpublish-0.2.0/xpublish/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-07-18 19:23:56.000000 xpublish-0.2.0/xpublish/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2139 2022-07-18 19:23:56.000000 xpublish-0.2.0/xpublish/utils/info.py
--rw-r--r--   0 runner    (1001) docker     (121)     5823 2022-07-18 19:23:56.000000 xpublish-0.2.0/xpublish/utils/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 19:24:07.036990 xpublish-0.2.0/xpublish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-07-18 19:24:06.000000 xpublish-0.2.0/xpublish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-07-18 19:24:06.000000 xpublish-0.2.0/xpublish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 19:24:06.000000 xpublish-0.2.0/xpublish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 19:24:06.000000 xpublish-0.2.0/xpublish.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-07-18 19:24:06.000000 xpublish-0.2.0/xpublish.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-18 19:24:06.000000 xpublish-0.2.0/xpublish.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.397112 xpublish-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/.binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-11 14:29:19.000000 xpublish-0.3.0/.binder/dask_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-11 14:29:19.000000 xpublish-0.3.0/.binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-11 14:29:19.000000 xpublish-0.3.0/.binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 14:29:19.000000 xpublish-0.3.0/.binder/start
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-11 14:29:19.000000 xpublish-0.3.0/.binder/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 14:29:19.000000 xpublish-0.3.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-11 14:29:19.000000 xpublish-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-11 14:29:19.000000 xpublish-0.3.0/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-11 14:29:19.000000 xpublish-0.3.0/.github/workflows/pypipublish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-11 14:29:19.000000 xpublish-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 14:29:19.000000 xpublish-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-11 14:29:19.000000 xpublish-0.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-05-11 14:29:19.000000 xpublish-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-11 14:29:36.397112 xpublish-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-11 14:29:19.000000 xpublish-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 14:29:19.000000 xpublish-0.3.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 14:29:19.000000 xpublish-0.3.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/docs/source/ecosystem/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/ecosystem/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.389112 xpublish-0.3.0/docs/source/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/docs/source/getting-started/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/dataset-provider-plugin.md
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/dataset-provider-plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/dataset-router-plugin.md
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/dataset-router-plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/dataset-router.md
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/dataset-router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/serving-multiple-datasets.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/tutorial/using-plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/getting-started/why-xpublish.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/docs/source/user-guide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/docs/source/user-guide/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/user-guide/deployment/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/user-guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-05-11 14:29:19.000000 xpublish-0.3.0/docs/source/user-guide/plugins.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-11 14:29:19.000000 xpublish-0.3.0/examples/open_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-11 14:29:19.000000 xpublish-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 14:29:19.000000 xpublish-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:29:36.397112 xpublish-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-11 14:29:19.000000 xpublish-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/test_fsspec_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/test_plugin_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/test_rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/test_zarr_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-11 14:29:19.000000 xpublish-0.3.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/xpublish/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/xpublish/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/xpublish/plugins/included/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/included/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/included/module_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/included/plugin_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/included/zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/plugins/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13303 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/xpublish/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/routers/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.397112 xpublish-0.3.0/xpublish/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/utils/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-11 14:29:19.000000 xpublish-0.3.0/xpublish/utils/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:29:36.393112 xpublish-0.3.0/xpublish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 14:29:36.000000 xpublish-0.3.0/xpublish.egg-info/top_level.txt
```

### Comparing `xpublish-0.2.0/.github/workflows/main.yaml` & `xpublish-0.3.0/.github/workflows/main.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 
 jobs:
   test:
     name: ${{ matrix.python-version }}-build
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.9", "3.10"]
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
-      - uses: actions/cache@v3.0.4
+      - uses: actions/cache@v3.3.1
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}-pip-${{ hashFiles('**/dev-requirements.txt') }}
           restore-keys: |
             ${{ runner.os }}-pip-
       - run: |
           python -m pip install -r dev-requirements.txt
           python -m pip install --no-deps -e .
           python -m pip list
       - name: Running Tests
         run: |
           python -m pytest --cov=./ --cov-report=xml --verbose
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3.1.0
+        uses: codecov/codecov-action@v3.1.3
         if: ${{ matrix.python-version }} == 3.9
         with:
           file: ./coverage.xml
           fail_ci_if_error: false
 
   test-upstream:
     name: ${{ matrix.python-version }}-dev-build
@@ -49,15 +49,15 @@
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
-      - uses: actions/cache@v3.0.4
+      - uses: actions/cache@v3.3.1
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}-pip-${{ hashFiles('**/dev-requirements.txt') }}
           restore-keys: |
             ${{ runner.os }}-pip-
       - run: |
           python -m pip install -r dev-requirements.txt
```

### Comparing `xpublish-0.2.0/.github/workflows/pypipublish.yaml` & `xpublish-0.3.0/.github/workflows/pypipublish.yaml`

 * *Files identical despite different names*

### Comparing `xpublish-0.2.0/.gitignore` & `xpublish-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xpublish-0.2.0/LICENSE` & `xpublish-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xpublish-0.2.0/PKG-INFO` & `xpublish-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 Metadata-Version: 2.1
 Name: xpublish
-Version: 0.2.0
+Version: 0.3.0
 Summary: Publish Xarray Datasets via a REST API.
-Home-page: https://github.com/xarray-contrib/xpublish
+Home-page: https://github.com/xpublish-community/xpublish
 Maintainer: Joe Hamman
 Maintainer-email: jhamman@ucar.edu
 License: MIT
 Keywords: xarray,zarr,api
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 License-File: LICENSE
 
 Xpublish
 ========
 
 Publish Xarray Datasets via a REST API.
 
-.. image:: https://img.shields.io/github/workflow/status/xarray-contrib/xpublish/CI?logo=github
-   :target: https://github.com/xarray-contrib/xpublish/actions?query=workflow%3ACI
+.. image:: https://github.com/xpublish-community/xpublish/actions/workflows/main.yaml/badge.svg
+   :target: https://github.com/xpublish-community/xpublish/actions/workflows/main.yaml
    :alt: GitHub Workflow Status
 
 .. image:: https://readthedocs.org/projects/xpublish/badge/?version=latest
    :target: https://xpublish.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/xarray-contrib/xpublish/main
    :alt: Binder
 
 .. image:: https://codecov.io/gh/xarray-contrib/xpublish/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/xarray-contrib/xpublish
 
+.. image:: https://results.pre-commit.ci/badge/github/xpublish-community/xpublish/main.svg
+   :target: https://results.pre-commit.ci/latest/github/xpublish-community/xpublish/main
+   :alt: pre-commit.ci status
+
 **Serverside: Publish a Xarray Dataset through a rest API**
 
 .. code-block:: python
 
    ds.rest.serve(host="0.0.0.0", port=9000)
 
 
@@ -56,18 +58,18 @@
 .. code-block:: python
 
    import xarray as xr
    import zarr
    from fsspec.implementations.http import HTTPFileSystem
 
    fs = HTTPFileSystem()
-   http_map = fs.get_mapper('http://0.0.0.0:9000')
+   http_map = fs.get_mapper("http://0.0.0.0:9000")
 
    # open as a zarr group
-   zg = zarr.open_consolidated(http_map, mode='r')
+   zg = zarr.open_consolidated(http_map, mode="r")
 
    # or open as another Xarray Dataset
    ds = xr.open_zarr(http_map, consolidated=True)
 
 
 Why?
 ^^^^
@@ -90,9 +92,7 @@
 REST-like API with builtin and/or user-defined endpoints.
 
 For example, Xpublish provides by default a minimal Zarr compatible REST-like
 API with the following endpoints:
 
 * ``.zmetadata``: returns Zarr-formatted metadata keys as json strings.
 * ``var/0.0.0``: returns a variable data chunk as a binary string.
-
-
```

### Comparing `xpublish-0.2.0/README.rst` & `xpublish-0.3.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Xpublish
 ========
 
 Publish Xarray Datasets via a REST API.
 
-.. image:: https://img.shields.io/github/workflow/status/xarray-contrib/xpublish/CI?logo=github
-   :target: https://github.com/xarray-contrib/xpublish/actions?query=workflow%3ACI
+.. image:: https://github.com/xpublish-community/xpublish/actions/workflows/main.yaml/badge.svg
+   :target: https://github.com/xpublish-community/xpublish/actions/workflows/main.yaml
    :alt: GitHub Workflow Status
 
 .. image:: https://readthedocs.org/projects/xpublish/badge/?version=latest
    :target: https://xpublish.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/xarray-contrib/xpublish/main
    :alt: Binder
 
 .. image:: https://codecov.io/gh/xarray-contrib/xpublish/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/xarray-contrib/xpublish
 
+.. image:: https://results.pre-commit.ci/badge/github/xpublish-community/xpublish/main.svg
+   :target: https://results.pre-commit.ci/latest/github/xpublish-community/xpublish/main
+   :alt: pre-commit.ci status
+
 **Serverside: Publish a Xarray Dataset through a rest API**
 
 .. code-block:: python
 
    ds.rest.serve(host="0.0.0.0", port=9000)
 
 
@@ -33,18 +37,18 @@
 .. code-block:: python
 
    import xarray as xr
    import zarr
    from fsspec.implementations.http import HTTPFileSystem
 
    fs = HTTPFileSystem()
-   http_map = fs.get_mapper('http://0.0.0.0:9000')
+   http_map = fs.get_mapper("http://0.0.0.0:9000")
 
    # open as a zarr group
-   zg = zarr.open_consolidated(http_map, mode='r')
+   zg = zarr.open_consolidated(http_map, mode="r")
 
    # or open as another Xarray Dataset
    ds = xr.open_zarr(http_map, consolidated=True)
 
 
 Why?
 ^^^^
```

### Comparing `xpublish-0.2.0/docs/Makefile` & `xpublish-0.3.0/docs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -171,7 +171,10 @@
 	@echo
 	@echo "Build finished. The XML files are in $(BUILDDIR)/xml."
 
 pseudoxml:
 	$(SPHINXBUILD) -b pseudoxml $(ALLSPHINXOPTS) $(BUILDDIR)/pseudoxml
 	@echo
 	@echo "Build finished. The pseudo-XML files are in $(BUILDDIR)/pseudoxml."
+
+live:
+	sphinx-autobuild -b dirhtml  source/ _build/dirhtml/
```

### Comparing `xpublish-0.2.0/docs/make.bat` & `xpublish-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xpublish-0.2.0/docs/source/conf.py` & `xpublish-0.3.0/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,20 +39,27 @@
     'sphinx.ext.autodoc',
     'sphinx.ext.viewcode',
     'sphinx.ext.autosummary',
     'sphinx.ext.doctest',
     'sphinx.ext.intersphinx',
     'sphinx.ext.extlinks',
     'sphinx.ext.napoleon',
+    'sphinxcontrib.autodoc_pydantic',
     'sphinx_autosummary_accessors',
+    'sphinx_autodoc_typehints',
+    'sphinx_design',
+    'myst_parser',
 ]
 
+myst_enable_extensions = []
+myst_heading_anchors = 6
+
 extlinks = {
-    'issue': ('https://github.com/xarray-contrib/xpublish/issues/%s', 'GH#'),
-    'pr': ('https://github.com/xarray-contrib/xpublish/pull/%s', 'GH#'),
+    'issue': ('https://github.com/xpublish-community/xpublish/issues/%s', 'GH#'),
+    'pr': ('https://github.com/xpublish-community/xpublish/pull/%s', 'GH#'),
 }
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates', sphinx_autosummary_accessors.templates_path]
 
 # Generate the API documentation when building
 autosummary_generate = True
 
@@ -116,29 +123,46 @@
 # If true, keep warnings as "system message" paragraphs in the built documents.
 # keep_warnings = False
 
 
 # -- Intersphinx links ---------------------------------------------------------
 
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/3.6/', None),
+    'python': ('https://docs.python.org/3.11/', None),
     'xarray': ('https://xarray.pydata.org/en/stable/', None),
     # sadly, there is no intersphinx for fastapi docs
 }
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'sphinx_rtd_theme'
+html_theme = 'pydata_sphinx_theme'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-# html_theme_options = {}
+html_theme_options = {
+    'icon_links': [
+        {
+            'name': 'GitHub',
+            'url': 'https://github.com/xpublish-community/xpublish',  # required
+            'icon': 'fa-brands fa-square-github',
+            'type': 'fontawesome',
+        }
+    ],
+    'use_edit_page_button': True,
+}
+
+html_context = {
+    'github_user': 'xpublish-community',
+    'github_repo': 'xpublish',
+    'github_version': 'main',
+    'doc_path': 'docs/source/',
+}
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
```

### Comparing `xpublish-0.2.0/docs/source/contributing.rst` & `xpublish-0.3.0/docs/source/contributing.rst`

 * *Files 26% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 Feature requests and feedback
 -----------------------------
 
 Do you like Xpublish? Share some love on Twitter or in your blog posts!
 
 We'd also like to hear about your propositions and suggestions.  Feel free to
-`submit them as issues <https://github.com/xarray-contrib/xpublish>`_ and:
+`submit them as issues <https://github.com/xpublish-community/xpublish>`_ and:
 
 * Explain in detail how they should work.
 * Keep the scope as narrow as possible.  This will make it easier to implement.
 
 .. _reportbugs:
 
 Report bugs
 -----------
 
-Report bugs for Xpublish in the `issue tracker <https://github.com/xarray-contrib/xpublish>`_.
+Report bugs for Xpublish in the `issue tracker <https://github.com/xpublish-community/xpublish>`_.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting,
   specifically the Python interpreter version, installed libraries, and Xpublish
   version.
@@ -41,15 +41,15 @@
 fix the bug itself.
 
 .. _fixbugs:
 
 Fix bugs
 --------
 
-Look through the `GitHub issues for bugs <https://github.com/xarray-contrib/xpublish/labels/type:%20bug>`_.
+Look through the `GitHub issues for bugs <https://github.com/xpublish-community/xpublish/labels/type:%20bug>`_.
 
 Talk to developers to find out how you can fix specific bugs.
 
 Write documentation
 -------------------
 
 xpublish could always use more documentation. What exactly is needed?
@@ -57,71 +57,72 @@
 * More complementary documentation.  Have you perhaps found something unclear?
 * Docstrings.  There can never be too many of them.
 * Blog posts, articles and such -- they're all very appreciated.
 
 You can also edit documentation files directly in the GitHub web interface,
 without using a local copy. This can be convenient for small fixes.
 
-To build the documentation locally, you first need to install the following
-tools:
-
-- `Sphinx <https://github.com/sphinx-doc/sphinx>`__
-- `sphinx_rtd_theme <https://github.com/readthedocs/sphinx_rtd_theme>`__
-- `sphinx-autosummary-accessors <https://github.com/xarray-contrib/sphinx-autosummary-accessors>`__
+To build the documentation locally, you first need to have a local development environment setup
+by following the the steps in `Preparing Pull Requests <#pull-requests>`__ through the **Install
+dependencies into a new conda environment** step.
 
 You can then build the documentation with the following commands::
 
+    $ conda activate xpublish-dev
     $ cd docs
+    $ pip install -r requirements.txt
     $ make html
 
 The built documentation should be available in the ``docs/_build/`` folder.
 
 .. _`pull requests`:
 .. _pull-requests:
 
 Preparing Pull Requests
 -----------------------
 
 #. Fork the
-   `xpublish GitHub repository <https://github.com/xarray-contrib/xpublish>`__.  It's
+   `xpublish GitHub repository <https://github.com/xpublish-community/xpublish>`__.  It's
    fine to use ``xpublish`` as your fork repository name because it will live
    under your user.
 
 #. Clone your fork locally using `git <https://git-scm.com/>`_ and create a branch::
 
     $ git clone git@github.com:YOUR_GITHUB_USERNAME/xpublish.git
     $ cd xpublish
 
-    # now, to fix a bug or add feature create your own branch off "master":
+    # now, to fix a bug or add feature create your own branch off "main":
 
-    $ git checkout -b your-bugfix-feature-branch-name master
+    $ git checkout -b your-bugfix-feature-branch-name main
 
 #. Install `pre-commit <https://pre-commit.com>`_ and its hook on the Xpublish repo::
 
      $ pip install --user pre-commit
      $ pre-commit install
 
    Afterwards ``pre-commit`` will run whenever you commit.
 
    https://pre-commit.com/ is a framework for managing and maintaining multi-language pre-commit hooks
    to ensure code-style and code formatting is consistent.
 
 #. Install dependencies into a new conda environment::
 
-    $ conda env update -f ci/environment-dev-3.7.yml
+    $ conda create -n xpublish-dev
+    $ conda activate xpublish-dev
+    $ pip install -r dev-requirements.txt
+    $ pip install --no-deps -e .
 
 #. Run all the tests
 
    Now running tests is as simple as issuing this command::
 
     $ conda activate xpublish-dev
-    $ pytest --junitxml=test-reports/junit.xml --cov=./ --verbose
-
+    $ pytest
 
-   This command will run tests via the "pytest" tool against Python 3.7.
+   This command will run tests via the "pytest" tool.
 
 #. You can now edit your local working copy and run the tests again as necessary. Please follow PEP-8 for naming.
 
    When committing, ``pre-commit`` will re-format the files if necessary.
 
 #. Commit and push once your tests pass and you are happy with your change(s)::
 
@@ -129,9 +130,9 @@
     $ git push -u
 
 #. Finally, submit a pull request through the GitHub website using this data::
 
     head-fork: YOUR_GITHUB_USERNAME/xpublish
     compare: your-branch-name
 
-    base-fork: xarray-contrib/xpublish
-    base: master
+    base-fork: xpublish-community/xpublish
+    base: main
```

### Comparing `xpublish-0.2.0/examples/open_dataset.ipynb` & `xpublish-0.3.0/examples/open_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `xpublish-0.2.0/setup.py` & `xpublish-0.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,32 +18,39 @@
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Intended Audience :: Science/Research',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Topic :: Scientific/Engineering',
 ]
 
 setup(
     name='xpublish',
     description='Publish Xarray Datasets via a REST API.',
     long_description=long_description,
     python_requires='>=3.8',
     maintainer='Joe Hamman',
     maintainer_email='jhamman@ucar.edu',
     classifiers=CLASSIFIERS,
-    url='https://github.com/xarray-contrib/xpublish',
+    url='https://github.com/xpublish-community/xpublish',
     packages=find_packages(exclude=('tests',)),
     package_dir={'xpublish': 'xpublish'},
     include_package_data=True,
     install_requires=install_requires,
     license='MIT',
     zip_safe=False,
     keywords=['xarray', 'zarr', 'api'],
     use_scm_version={'version_scheme': 'post-release', 'local_scheme': 'dirty-tag'},
     setup_requires=['setuptools_scm>=3.4', 'setuptools>=42'],
+    entry_points={
+        'xpublish.plugin': [
+            'dataset_info = xpublish.plugins.included.dataset_info:DatasetInfoPlugin',
+            'zarr = xpublish.plugins.included.zarr:ZarrPlugin',
+            'module_version = xpublish.plugins.included.module_version:ModuleVersionPlugin',
+            'plugin_info = xpublish.plugins.included.plugin_info:PluginInfoPlugin',
+        ]
+    },
 )
```

### Comparing `xpublish-0.2.0/tests/test_core.py` & `xpublish-0.3.0/tests/test_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,25 @@
     ds = xr.Dataset({'foo': (['x', 'y', 'z'], data1), 'bar': (['x', 'y', 'z'], data2)})
     zmeta = create_zmetadata(ds)
 
     assert zmeta['metadata']['foo/.zarray']['chunks'] == expected
     assert zmeta['metadata']['bar/.zarray']['chunks'] == list(data2.shape)
 
 
+def test_single_dataset_raise(airtemp_ds):
+    """A single dataset should throw a TypeError if it's passed to
+    xpublish.Rest rather than xpublish.SingleDatasetRest.
+    """
+    with pytest.raises(TypeError) as excinfo:
+        xpublish.Rest(airtemp_ds)
+    excinfo.match(
+        'xpublish.Rest no longer directly handles single datasets. Please use xpublish.SingleDatasetRest instead'
+    )
+
+
 def test_invalid_dask_chunks_raise():
     data1 = dask.array.zeros((10, 20, 30), chunks=(4, 10, 1))
     data2 = dask.array.zeros((10, 20, 30), chunks=(4, 5, 1))
     data = dask.array.concatenate([data1, data2])
     ds = xr.Dataset({'foo': (['x', 'y', 'z'], data)})
 
     with pytest.raises(ValueError) as excinfo:
```

### Comparing `xpublish-0.2.0/tests/utils.py` & `xpublish-0.3.0/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
 class TestMapper(TestClient, BaseStore):
     """
     A simple subclass to support getitem syntax on Starlette TestClient Objects
     """
 
     def __getitem__(self, key):
-        response = self.get(key)
+        zarr_key = f'/zarr/{key}'
+        response = self.get(zarr_key)
         if response.status_code != 200:
-            raise KeyError('{} not found. status_code = {}'.format(key, response.status_code))
+            raise KeyError('{} not found. status_code = {}'.format(zarr_key, response.status_code))
         return response.content
 
     def __delitem__(self, key):
         return NotImplemented
 
     def __iter__(self):
         return NotImplemented
@@ -41,14 +42,15 @@
     calendar='standard',
     units='days since 1980-01-01',
     use_cftime=True,
     decode_times=True,
     nlats=1,
     nlons=1,
     var_const=None,
+    use_xy_dim=False,
 ):
     """Utility function for creating test data"""
 
     if use_cftime:
         end = xr.coding.cftime_offsets.to_cftime_datetime(end, calendar=calendar)
         dates = xr.cftime_range(start=start, end=end, freq=freq, calendar=calendar)
 
@@ -87,15 +89,20 @@
         time_bounds = xr.DataArray(
             encoded_time_bounds, name='time_bounds', dims=('time', 'd2'), coords={'time': times}
         )
 
     lats = np.linspace(start=-90, stop=90, num=nlats, dtype='float32')
     lons = np.linspace(start=-180, stop=180, num=nlons, dtype='float32')
 
-    shape = (times.size, lats.size, lons.size)
+    if use_xy_dim:
+        lats, lons = np.meshgrid(lats, lons)
+        shape = (times.size, *lats.shape)
+    else:
+        shape = (times.size, lats.size, lons.size)
+
     num = reduce(mul, shape)
 
     if var_const is None:
         annual_cycle = np.sin(2 * np.pi * (decoded_times.dt.dayofyear.values / 365.25 - 0.28))
         base = 10 + 15 * annual_cycle.reshape(-1, 1)
         tmin_values = base + 3 * np.random.randn(annual_cycle.size, nlats * nlons)
         tmax_values = base + 10 + 3 * np.random.randn(annual_cycle.size, nlats * nlons)
@@ -109,22 +116,30 @@
     else:
         tmin_values = np.arange(1, num + 1).reshape(shape)
         tmax_values = np.arange(1, num + 1).reshape(shape)
 
     ds = xr.Dataset(
         {
             'tmin': xr.DataArray(
-                tmin_values.astype('float32'), dims=('time', 'lat', 'lon'), name='tmin'
+                tmin_values.astype('float32'),
+                dims=('time', 'lat', 'lon') if not use_xy_dim else ('time', 'y', 'x'),
+                name='tmin',
             ),
             'tmax': xr.DataArray(
-                tmax_values.astype('float32'), dims=('time', 'lat', 'lon'), name='tmax'
+                tmax_values.astype('float32'),
+                dims=('time', 'lat', 'lon') if not use_xy_dim else ('time', 'y', 'x'),
+                name='tmax',
             ),
             'time_bounds': time_bounds,
         },
-        {'time': times, 'lat': lats, 'lon': lons},
+        coords={
+            'time': times,
+            'lat': ('lat' if not use_xy_dim else ['y', 'x'], lats),
+            'lon': ('lon' if not use_xy_dim else ['y', 'x'], lons),
+        },
     )
 
     ds.tmin.encoding['_FillValue'] = np.float32(-9999999)
     ds.tmax.encoding['_FillValue'] = np.float32(-9999999)
     ds.time.attrs['bounds'] = 'time_bounds'
     ds.time.encoding['units'] = units
     ds.time.encoding['calendar'] = calendar
```

### Comparing `xpublish-0.2.0/xpublish/dependencies.py` & `xpublish-0.3.0/xpublish/dependencies.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,73 @@
 """
 Helper functions to use a FastAPI dependencies.
 """
+from typing import TYPE_CHECKING, Dict, List
+
 import cachey
+import pluggy
 import xarray as xr
 from fastapi import Depends
 
 from .utils.api import DATASET_ID_ATTR_KEY
 from .utils.zarr import create_zmetadata, create_zvariables, zarr_metadata_key
 
+if TYPE_CHECKING:
+    from .plugins import Plugin  # pragma: no cover
+
 
-def get_dataset_ids():
+def get_dataset_ids() -> List[str]:
     """FastAPI dependency for getting the list of ids (string keys)
     of the collection of datasets being served.
 
     Use this callable as dependency in any FastAPI path operation
     function where you need access to those ids.
 
     This dummy dependency will be overridden when creating the FastAPI
     application.
 
+    Returns:
+        A list of unique keys for datasets
+
     """
     return []  # pragma: no cover
 
 
-def get_dataset(dataset_id: str):
+def get_dataset(dataset_id: str) -> xr.Dataset:
     """FastAPI dependency for accessing the published xarray dataset object.
 
     Use this callable as dependency in any FastAPI path operation
     function where you need access to the xarray Dataset being served.
 
     This dummy dependency will be overridden when creating the FastAPI
     application.
 
+    Parameters:
+        dataset_id:
+            Unique path-safe key identifying dataset
+
+    Returns:
+        Requested Xarray dataset
+
     """
-    return None  # pragma: no cover
+    return xr.Dataset()  # pragma: no cover
 
 
-def get_cache():
+def get_cache() -> cachey.Cache:
     """FastAPI dependency for accessing the application's cache.
 
     Use this callable as dependency in any FastAPI path operation
     function where you need access to the cache provided with the
     application.
 
     This dummy dependency will be overridden when creating the FastAPI
     application.
 
     """
-    return None  # pragma: no cover
+    return cachey.Cache(available_bytes=1e6)  # pragma: no cover
 
 
 def get_zvariables(
     dataset: xr.Dataset = Depends(get_dataset), cache: cachey.Cache = Depends(get_cache)
 ):
     """FastAPI dependency that returns a dictionary of zarr encoded variables."""
 
@@ -80,7 +96,21 @@
     if zmeta is None:
         zmeta = create_zmetadata(dataset)
 
         # we want to permanently cache this: set high cost value
         cache.put(cache_key, zmeta, 99999)
 
     return zmeta
+
+
+def get_plugins() -> Dict[str, 'Plugin']:
+    """FastAPI dependency that returns the a dictionary of loaded plugins
+
+    Returns:
+        Dictionary of names to initialized plugins.
+    """
+
+    return {}  # pragma: no cover
+
+
+def get_plugin_manager() -> pluggy.PluginManager:
+    """Return the active plugin manager"""
```

### Comparing `xpublish-0.2.0/xpublish/routers/common.py` & `xpublish-0.3.0/xpublish/plugins/included/module_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 """
-Dataset-independent API routes.
-
+Version information router
 """
 import importlib
 import sys
+from typing import List
 
-from fastapi import APIRouter, Depends
+from fastapi import APIRouter
 
-from ..dependencies import get_dataset_ids
-from ..utils.info import get_sys_info, netcdf_and_hdf5_versions
+from ...utils.info import get_sys_info, netcdf_and_hdf5_versions
+from .. import Plugin, hookimpl
 
-common_router = APIRouter()
 
+class ModuleVersionPlugin(Plugin):
+    name = 'module_version'
+
+    app_router_prefix: str = ''
+    app_router_tags: List[str] = []
+
+    @hookimpl
+    def app_router(self):
+        router = APIRouter(prefix=self.app_router_prefix, tags=self.app_router_tags)
+
+        @router.get('/versions')
+        def get_versions():
+            versions = dict(get_sys_info() + netcdf_and_hdf5_versions())
+            modules = [
+                'xarray',
+                'zarr',
+                'numcodecs',
+                'fastapi',
+                'starlette',
+                'pandas',
+                'numpy',
+                'dask',
+                'distributed',
+                'uvicorn',
+            ]
+            for modname in modules:
+                try:
+                    if modname in sys.modules:
+                        mod = sys.modules[modname]
+                    else:  # pragma: no cover
+                        mod = importlib.import_module(modname)
+                    versions[modname] = getattr(mod, '__version__', None)
+                except ImportError:  # pragma: no cover
+                    pass
+            return versions
 
-@common_router.get('/versions')
-def get_versions():
-    versions = dict(get_sys_info() + netcdf_and_hdf5_versions())
-    modules = [
-        'xarray',
-        'zarr',
-        'numcodecs',
-        'fastapi',
-        'starlette',
-        'pandas',
-        'numpy',
-        'dask',
-        'distributed',
-        'uvicorn',
-    ]
-    for modname in modules:
-        try:
-            if modname in sys.modules:
-                mod = sys.modules[modname]
-            else:  # pragma: no cover
-                mod = importlib.import_module(modname)
-            versions[modname] = getattr(mod, '__version__', None)
-        except ImportError:  # pragma: no cover
-            pass
-    return versions
-
-
-dataset_collection_router = APIRouter()
-
-
-@dataset_collection_router.get('/datasets')
-def get_dataset_collection_keys(ids: list = Depends(get_dataset_ids)):
-    return ids
+        return router
```

### Comparing `xpublish-0.2.0/xpublish/utils/api.py` & `xpublish-0.3.0/xpublish/utils/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import json
 from collections.abc import Mapping
-from typing import Dict, List, Tuple
+from typing import Any, Dict, List, Tuple
 
 import xarray as xr
 from fastapi import APIRouter
 from fastapi.openapi.utils import get_openapi
+from starlette.responses import JSONResponse as StarletteJSONResponse  # type: ignore
 
 DATASET_ID_ATTR_KEY = '_xpublish_id'
 
 
 def normalize_datasets(datasets) -> Dict[str, xr.Dataset]:
     """Normalize the given collection of datasets.
 
@@ -19,15 +21,15 @@
 
     """
     error_msg = 'Can only publish a xarray.Dataset object or a mapping of Dataset objects'
 
     if isinstance(datasets, xr.Dataset):
         return {}
     elif isinstance(datasets, Mapping):
-        if not all([isinstance(obj, xr.Dataset) for obj in datasets.values()]):
+        if not all(isinstance(obj, xr.Dataset) for obj in datasets.values()):
             raise TypeError(error_msg)
         return {str(k): ds.assign_attrs({DATASET_ID_ATTR_KEY: k}) for k, ds in datasets.items()}
     else:
         raise TypeError(error_msg)
 
 
 def normalize_app_routers(routers: list, prefix: str) -> List[Tuple[APIRouter, Dict]]:
@@ -51,15 +53,14 @@
                 'instance or a (APIRouter, {...}) tuple.'
             )
 
     return new_routers
 
 
 def check_route_conflicts(routers):
-
     paths = []
 
     for router, kws in routers:
         prefix = kws.get('prefix', '')
         paths += [prefix + r.path for r in router.routes]
 
     seen = set()
@@ -89,26 +90,25 @@
 
     """
 
     def __init__(self, app):
         self._app = app
 
     def openapi(self):
-
         if self._app.openapi_schema:
             return self._app.openapi_schema
 
-        kwargs = dict(
-            title=self._app.title,
-            version=self._app.version,
-            description=self._app.description,
-            routes=self._app.routes,
-            tags=self._app.openapi_tags,
-            servers=self._app.servers,
-        )
+        kwargs = {
+            'title': self._app.title,
+            'version': self._app.version,
+            'description': self._app.description,
+            'routes': self._app.routes,
+            'tags': self._app.openapi_tags,
+            'servers': self._app.servers,
+        }
 
         openapi_schema = get_openapi(**kwargs)
 
         for path in openapi_schema.get('paths', {}).values():
             for http_method in path.values():
                 params = http_method.get('parameters')
 
@@ -116,7 +116,22 @@
                     for i, p in enumerate(params):
                         if p.get('name') == 'dataset_id':
                             params.pop(i)
 
         self._app.openapi_schema = openapi_schema
 
         return self._app.openapi_schema
+
+
+class JSONResponse(StarletteJSONResponse):
+    def __init__(self, *args, **kwargs):
+        self._render_kwargs = {
+            'ensure_ascii': True,
+            'allow_nan': True,
+            'indent': None,
+            'separators': (',', ':'),
+        }
+        self._render_kwargs.update(kwargs.pop('render_kwargs', {}))
+        super().__init__(*args, **kwargs)
+
+    def render(self, content: Any) -> bytes:
+        return json.dumps(content, **self._render_kwargs).encode('utf-8')
```

### Comparing `xpublish-0.2.0/xpublish/utils/info.py` & `xpublish-0.3.0/xpublish/utils/info.py`

 * *Files identical despite different names*

### Comparing `xpublish-0.2.0/xpublish/utils/zarr.py` & `xpublish-0.3.0/xpublish/utils/zarr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import logging
 
-import dask
+import dask.array
 import numpy as np
 import xarray as xr
 from numcodecs.compat import ensure_ndarray
 from xarray.backends.zarr import (
     DIMENSION_KEY,
     encode_zarr_attr_value,
     encode_zarr_variable,
@@ -47,14 +47,26 @@
     # We don't want `_FillValue` in `.zattrs`
     # It should go in `fill_value` section of `.zarray`
     _ = zattrs.pop('_FillValue', None)
 
     return zattrs
 
 
+def _extract_dataarray_coords(da, zattrs):
+    '''helper function to extract coords from DataArray into a directionary'''
+    if da.coords:
+        # Coordinates are only encoded if there are non-dimension coordinates
+        nondim_coords = set(da.coords) - set(da.dims)
+
+        if len(nondim_coords) > 0 and da.name not in nondim_coords:
+            coords = ' '.join(sorted(nondim_coords))
+            zattrs['coordinates'] = encode_zarr_attr_value(coords)
+    return zattrs
+
+
 def _extract_fill_value(da, dtype):
     """helper function to extract fill value from DataArray."""
     fill_value = da.attrs.pop('_FillValue', None)
     return encode_fill_value(fill_value, dtype)
 
 
 def _extract_zarray(da, encoding, dtype):
@@ -100,18 +112,21 @@
 def create_zmetadata(dataset):
     """Helper function to create a consolidated zmetadata dictionary."""
 
     zmeta = {'zarr_consolidated_format': zarr_consolidated_format, 'metadata': {}}
     zmeta['metadata'][group_meta_key] = {'zarr_format': zarr_format}
     zmeta['metadata'][attrs_key] = _extract_dataset_zattrs(dataset)
 
-    for key, da in dataset.variables.items():
-        encoded_da = encode_zarr_variable(da, name=key)
-        encoding = extract_zarr_variable_encoding(da)
-        zmeta['metadata'][f'{key}/{attrs_key}'] = _extract_dataarray_zattrs(encoded_da)
+    for key, dvar in dataset.variables.items():
+        da = dataset[key]
+        encoded_da = encode_zarr_variable(dvar, name=key)
+        encoding = extract_zarr_variable_encoding(dvar)
+        zattrs = _extract_dataarray_zattrs(encoded_da)
+        zattrs = _extract_dataarray_coords(da, zattrs)
+        zmeta['metadata'][f'{key}/{attrs_key}'] = zattrs
         zmeta['metadata'][f'{key}/{array_meta_key}'] = _extract_zarray(
             encoded_da, encoding, encoded_da.dtype
         )
 
     return zmeta
 
 
@@ -159,15 +174,15 @@
 
     If this is an incomplete edge chunk, pad the returned array to match out_shape.
     """
     ikeys = tuple(map(int, chunk_id.split('.')))
     if isinstance(da, dask_array_type):
         chunk_data = da.blocks[ikeys]
     else:
-        if ikeys != ((0,) * da.ndim):
+        if da.ndim > 0 and ikeys != ((0,) * da.ndim):
             raise ValueError(
                 'Invalid chunk_id for numpy array: %s. Should have been: %s'
                 % (chunk_id, ((0,) * da.ndim))
             )
         chunk_data = np.asarray(da)
 
     logger.debug('checking chunk output size, %s == %s' % (chunk_data.shape, out_shape))
```

### Comparing `xpublish-0.2.0/xpublish.egg-info/PKG-INFO` & `xpublish-0.3.0/xpublish.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 Metadata-Version: 2.1
 Name: xpublish
-Version: 0.2.0
+Version: 0.3.0
 Summary: Publish Xarray Datasets via a REST API.
-Home-page: https://github.com/xarray-contrib/xpublish
+Home-page: https://github.com/xpublish-community/xpublish
 Maintainer: Joe Hamman
 Maintainer-email: jhamman@ucar.edu
 License: MIT
 Keywords: xarray,zarr,api
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 License-File: LICENSE
 
 Xpublish
 ========
 
 Publish Xarray Datasets via a REST API.
 
-.. image:: https://img.shields.io/github/workflow/status/xarray-contrib/xpublish/CI?logo=github
-   :target: https://github.com/xarray-contrib/xpublish/actions?query=workflow%3ACI
+.. image:: https://github.com/xpublish-community/xpublish/actions/workflows/main.yaml/badge.svg
+   :target: https://github.com/xpublish-community/xpublish/actions/workflows/main.yaml
    :alt: GitHub Workflow Status
 
 .. image:: https://readthedocs.org/projects/xpublish/badge/?version=latest
    :target: https://xpublish.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/xarray-contrib/xpublish/main
    :alt: Binder
 
 .. image:: https://codecov.io/gh/xarray-contrib/xpublish/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/xarray-contrib/xpublish
 
+.. image:: https://results.pre-commit.ci/badge/github/xpublish-community/xpublish/main.svg
+   :target: https://results.pre-commit.ci/latest/github/xpublish-community/xpublish/main
+   :alt: pre-commit.ci status
+
 **Serverside: Publish a Xarray Dataset through a rest API**
 
 .. code-block:: python
 
    ds.rest.serve(host="0.0.0.0", port=9000)
 
 
@@ -56,18 +58,18 @@
 .. code-block:: python
 
    import xarray as xr
    import zarr
    from fsspec.implementations.http import HTTPFileSystem
 
    fs = HTTPFileSystem()
-   http_map = fs.get_mapper('http://0.0.0.0:9000')
+   http_map = fs.get_mapper("http://0.0.0.0:9000")
 
    # open as a zarr group
-   zg = zarr.open_consolidated(http_map, mode='r')
+   zg = zarr.open_consolidated(http_map, mode="r")
 
    # or open as another Xarray Dataset
    ds = xr.open_zarr(http_map, consolidated=True)
 
 
 Why?
 ^^^^
@@ -90,9 +92,7 @@
 REST-like API with builtin and/or user-defined endpoints.
 
 For example, Xpublish provides by default a minimal Zarr compatible REST-like
 API with the following endpoints:
 
 * ``.zmetadata``: returns Zarr-formatted metadata keys as json strings.
 * ``var/0.0.0``: returns a variable data chunk as a binary string.
-
-
```

