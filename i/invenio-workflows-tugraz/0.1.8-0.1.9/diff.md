# Comparing `tmp/invenio-workflows-tugraz-0.1.8.tar.gz` & `tmp/invenio-workflows-tugraz-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-workflows-tugraz-0.1.8.tar", last modified: Tue Apr 25 21:13:08 2023, max compression
+gzip compressed data, was "invenio-workflows-tugraz-0.1.9.tar", last modified: Wed May 10 09:58:40 2023, max compression
```

## Comparing `invenio-workflows-tugraz-0.1.8.tar` & `invenio-workflows-tugraz-0.1.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.615503 invenio-workflows-tugraz-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.615503 invenio-workflows-tugraz-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.615503 invenio-workflows-tugraz-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/data/
--rw-r--r--   0 runner    (1001) docker     (123)   939307 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/data/iso6393.json
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/theses.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 21:13:08.000000 invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      437 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:13:08.619503 invenio-workflows-tugraz-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-25 21:13:02.000000 invenio-workflows-tugraz-0.1.8/tests/test_invenio_workflows_tugraz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.744153 invenio-workflows-tugraz-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.736153 invenio-workflows-tugraz-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.740153 invenio-workflows-tugraz-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 09:58:40.744153 invenio-workflows-tugraz-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.740153 invenio-workflows-tugraz-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.740153 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.744153 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   939307 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/data/iso6393.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.744153 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.744153 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/theses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.740153 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      437 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-10 09:58:40.748153 invenio-workflows-tugraz-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.744153 invenio-workflows-tugraz-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/tests/test_invenio_workflows_tugraz.py
```

### Comparing `invenio-workflows-tugraz-0.1.8/.editorconfig` & `invenio-workflows-tugraz-0.1.9/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/.github/workflows/tests.yml` & `invenio-workflows-tugraz-0.1.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/CHANGES.rst` & `invenio-workflows-tugraz-0.1.9/CHANGES.rst`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.1.9 (release 2023-05-10)
+
+- theses: apply marc21 request changes
+
+
 Version v0.1.8 (release 2023-04-25)
 
 - theses: add necessary need to import
 
 
 Version v0.1.7 (release 2023-01-26)
```

### Comparing `invenio-workflows-tugraz-0.1.8/CONTRIBUTING.rst` & `invenio-workflows-tugraz-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/LICENSE` & `invenio-workflows-tugraz-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/MANIFEST.in` & `invenio-workflows-tugraz-0.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/PKG-INFO` & `invenio-workflows-tugraz-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-workflows-tugraz
-Version: 0.1.8
+Version: 0.1.9
 Summary: "This package serves as a place for the workflows of the repository of the TU Graz."
 Home-page: https://github.com/tu-graz-library/invenio-workflows-tugraz
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio workflows TUGraz
 Platform: any
@@ -26,14 +26,19 @@
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.1.9 (release 2023-05-10)
+
+- theses: apply marc21 request changes
+
+
 Version v0.1.8 (release 2023-04-25)
 
 - theses: add necessary need to import
 
 
 Version v0.1.7 (release 2023-01-26)
```

### Comparing `invenio-workflows-tugraz-0.1.8/babel.ini` & `invenio-workflows-tugraz-0.1.9/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/docs/Makefile` & `invenio-workflows-tugraz-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/docs/conf.py` & `invenio-workflows-tugraz-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/docs/index.rst` & `invenio-workflows-tugraz-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/docs/make.bat` & `invenio-workflows-tugraz-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/config.py` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/config.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/data/iso6393.json` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/data/iso6393.json`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/ext.py` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/convert.py` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/convert.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/utils.py` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/openaccess/workflow.py` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/workflow.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/__init__.py` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/convert.py` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # invenio-workflows-tugraz is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Convert from CampusOnline to Marc21."""
 
+from datetime import datetime
 from re import split
 from xml.etree.ElementTree import Element
 
 from invenio_records_marc21.services.record.metadata import Marc21Metadata, QName
 
 
 def construct_name(name):
@@ -66,52 +67,52 @@
 
     def __init__(self, record: Marc21Metadata):
         """Constructor."""
         super().__init__()
         self.author_name = "N/A"
         self.state = ""
         self.metaclass_name = ""
-        self.data_elements = ""
 
+        record.emplace_leader("07878nam a2200421 c 4500")
         record.emplace_controlfield("007", "cr#|||||||||||")
+        record.emplace_controlfield("008", "230501s########   #a###om####000#0#eng c")
         record.emplace_datafield(
             "040...", subfs={"a": "AT-UBTUG", "b": "ger", "d": "AT-UBTUG", "e": "rda"}
         )
         record.emplace_datafield("044...", subfs={"c": "XA-AT"})
-        record.emplace_datafield("264..1.", subfs={"a": "Graz", "c": "JAHR"})
+        record.emplace_datafield("264..1.", subfs={"a": "Graz", "c": "DATUM"})
         record.emplace_datafield(
             "300...", subfs={"a": "1 Online-Ressource ( Seiten )", "b": "ill"}
         )
         record.emplace_datafield("336...", subfs={"b": "txt"})
         record.emplace_datafield("337...", subfs={"b": "c"})
         record.emplace_datafield("338...", subfs={"b": "cr"})
         record.emplace_datafield("347...", subfs={"a": "Textdatei", "b": "PDF"})
         record.emplace_datafield(
-            "506.0..", subfs={"f": "Unrestricted online access", "2": "star"}
+            "506.0..", subfs={"2": "star", "f": "Unrestricted online access"}
         )
         record.emplace_datafield("546...", subfs={"a": "Zusammenfassung in"})
         record.emplace_datafield(
-            "655...",
+            "655..7.",
             subfs={
                 "a": "Hochschulschrift",
                 "0": "(DE-588)4113937-9",
-                "d": "gnd-content",
+                "2": "gnd-content",
             },
         )
+        # TODO: find out what in 008 should be
 
     def visit(self, node, record: Marc21Metadata):
         """Override visit."""
         super().visit(node, record)
-        # TODO: find out what in 008 should be
-        record.emplace_controlfield("008", self.data_elements)
 
     def visit_ID(self, node, record: Marc21Metadata):
         """Visit ID."""
         record.emplace_datafield(
-            "995...", subfs={"i": "TUGRAZonline", "d": node.text, "9": "local"}
+            "995...", subfs={"i": "TUGRAZonline", "a": node.text, "9": "local"}
         )
 
     def visit_PAG(self, node, record: Marc21Metadata):
         """Visit PAG."""
 
     def visit_CO(self, node: Element, record: Marc21Metadata):
         """Visit CO."""
@@ -132,14 +133,18 @@
         """Visit PUBLIC."""
 
     def visit_STATUS(self, node: Element, record: Marc21Metadata):
         """Visit status."""
 
     def visit_STATUSD(self, node: Element, record: Marc21Metadata):
         """Visit Status date."""
+        try:
+            self.year = datetime.strptime(node.text, "%Y-%M-%D %H:%M:%S").year
+        except ValueError:
+            self.year = "JAHR"
 
     def visit_ORG(self, node: Element, record: Marc21Metadata):
         """Visit ."""
 
     def visit_ORGP(self, node: Element, record: Marc21Metadata):
         """Visit ."""
         orgp = node.text.split("&gt;")
@@ -161,15 +166,15 @@
         """Visit ."""
         if self.state == "metaobj":
             self.typ = node.text
             return
 
         record.emplace_datafield(
             "502...",
-            subfs={"b": node.text, "c": "Technische Universität Graz", "d": "JAHR"},
+            subfs={"b": node.text, "c": "Technische Universität Graz", "d": self.year},
         )
 
     def visit_ZUGKB(self, node: Element, record: Marc21Metadata):
         """Visit ."""
 
     def visit_ZUG(self, node: Element, record: Marc21Metadata):
         """Visit ."""
@@ -181,19 +186,23 @@
         """Visit ."""
         text = node.text
         self.spvon = text.split(" ")[0] if text else ""
 
     def visit_SPBIS(self, node: Element, record: Marc21Metadata):
         """Visit ."""
         text = node.text
+        in_format = "%Y-%M-%D %H:%M:%S"
+        out_format = "%D-%M-%Y"
+        spvon = datetime.strptime(self.spvon, in_format).strftime(out_format)
+        spbis = datetime.strptime(text.split(" ")[0], in_format).strftime(out_format)
 
         if text:
             record.emplace_datafield(
                 "971.7..",
-                subfs={"a": "gesperrt", "b": self.spvon, "c": text.split(" ")[0]},
+                subfs={"a": "gesperrt", "b": spvon, "c": spbis},
             )
 
     def visit_SPBGR(self, node: Element, record: Marc21Metadata):
         """Visit ."""
 
     def visit_OLANG(self, node: Element, record: Marc21Metadata):
         """Visit ."""
@@ -228,20 +237,27 @@
             self.author_name = construct_name(self.name)
             record.emplace_datafield(
                 "100.1..", subfs={"a": self.author_name, "4": "aut"}
             )
 
         if self.metaclass_name == "SUPERVISOR":
             types = {
+                "BTEXT": "0",
                 "BTTUG": "0",
                 "MBTUG": "2",
+                "MBEXT": "2",
                 "1BUTUG": "1",
+                "2BUTUG": "1",
+                "3BUTUG": "1",
+                "4BUTUG": "1",
+                "5BUTUG": "1",
+                "6BUTUG": "1",
             }
             ind1 = types.get(self.typ, "")
-            record.emplace_datafield(f"971.{ind1}.0.a", value=construct_name(self.name))
+            record.emplace_datafield(f"971.{ind1}..a", value=construct_name(self.name))
 
         self.state = ""
 
     def visit_FN(self, node: Element, record: Marc21Metadata):
         """Visit ."""
         self.name["fn"] = node.text
 
@@ -270,15 +286,16 @@
     def visit_INTERN(self, node: Element, record: Marc21Metadata):
         """Visit ."""
 
     def visit_TIT(self, node: Element, record: Marc21Metadata):
         """Visit ."""
         if self.state == "metaobj" and self.language == self.object_language:
             record.emplace_datafield(
-                "245.1.0.", subfs={"a": node.text, "c": self.author_name}
+                "245.1.0.",
+                subfs={"a": node.text, "c": f"{self.name.fn} {self.name.ln}"},
             )
 
         if self.state == "metaobj" and self.language != self.object_language:
             record.emplace_datafield(
                 "246.1..", subfs={"i": "TUGRAZonline", "a": node.text}
             )
```

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/decorators.py` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/theses.py` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/theses.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz/theses/views.py` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/views.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/PKG-INFO` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-workflows-tugraz
-Version: 0.1.8
+Version: 0.1.9
 Summary: "This package serves as a place for the workflows of the repository of the TU Graz."
 Home-page: https://github.com/tu-graz-library/invenio-workflows-tugraz
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio workflows TUGraz
 Platform: any
@@ -26,14 +26,19 @@
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.1.9 (release 2023-05-10)
+
+- theses: apply marc21 request changes
+
+
 Version v0.1.8 (release 2023-04-25)
 
 - theses: add necessary need to import
 
 
 Version v0.1.7 (release 2023-01-26)
```

### Comparing `invenio-workflows-tugraz-0.1.8/invenio_workflows_tugraz.egg-info/SOURCES.txt` & `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/setup.cfg` & `invenio-workflows-tugraz-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/tests/conftest.py` & `invenio-workflows-tugraz-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.8/tests/test_invenio_workflows_tugraz.py` & `invenio-workflows-tugraz-0.1.9/tests/test_invenio_workflows_tugraz.py`

 * *Files identical despite different names*

