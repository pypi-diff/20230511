# Comparing `tmp/adafruit-circuitpython-gfx-1.1.16.tar.gz` & `tmp/adafruit-circuitpython-gfx-1.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-gfx-1.1.16.tar", last modified: Mon Jan 23 20:44:31 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-gfx-1.1.17.tar", last modified: Tue Mar 21 16:52:10 2023, max compression
```

## Comparing `adafruit-circuitpython-gfx-1.1.16.tar` & `adafruit-circuitpython-gfx-1.1.17.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:44:31.567298 adafruit-circuitpython-gfx-1.1.16/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:44:31.559297 adafruit-circuitpython-gfx-1.1.16/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:44:31.563298 adafruit-circuitpython-gfx-1.1.16/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:44:31.563298 adafruit-circuitpython-gfx-1.1.16/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:44:31.563298 adafruit-circuitpython-gfx-1.1.16/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19269 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/LICENSES/CC-BY-NC-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-01-23 20:44:31.567298 adafruit-circuitpython-gfx-1.1.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:44:31.563298 adafruit-circuitpython-gfx-1.1.16/adafruit_circuitpython_gfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-01-23 20:44:31.000000 adafruit-circuitpython-gfx-1.1.16/adafruit_circuitpython_gfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-01-23 20:44:31.000000 adafruit-circuitpython-gfx-1.1.16/adafruit_circuitpython_gfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 20:44:31.000000 adafruit-circuitpython-gfx-1.1.16/adafruit_circuitpython_gfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-23 20:44:31.000000 adafruit-circuitpython-gfx-1.1.16/adafruit_circuitpython_gfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-23 20:44:31.000000 adafruit-circuitpython-gfx-1.1.16/adafruit_circuitpython_gfx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:44:31.563298 adafruit-circuitpython-gfx-1.1.16/adafruit_gfx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:44:31.563298 adafruit-circuitpython-gfx-1.1.16/adafruit_gfx/fonts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4755 2023-01-23 20:44:24.000000 adafruit-circuitpython-gfx-1.1.16/adafruit_gfx/fonts/gfx_standard_font_01.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19787 2023-01-23 20:44:24.000000 adafruit-circuitpython-gfx-1.1.16/adafruit_gfx/gfx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:44:31.567298 adafruit-circuitpython-gfx-1.1.16/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:44:31.567298 adafruit-circuitpython-gfx-1.1.16/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:44:31.567298 adafruit-circuitpython-gfx-1.1.16/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-01-23 20:44:24.000000 adafruit-circuitpython-gfx-1.1.16/examples/gfx_ili9341_randlines.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2587 2023-01-23 20:44:24.000000 adafruit-circuitpython-gfx-1.1.16/examples/gfx_ili9341_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 20:44:24.000000 adafruit-circuitpython-gfx-1.1.16/examples/gfx_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-01-23 20:44:24.000000 adafruit-circuitpython-gfx-1.1.16/font_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-01-23 20:44:24.000000 adafruit-circuitpython-gfx-1.1.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-23 20:44:17.000000 adafruit-circuitpython-gfx-1.1.16/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 20:44:31.567298 adafruit-circuitpython-gfx-1.1.16/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:52:10.771731 adafruit-circuitpython-gfx-1.1.17/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:52:10.763731 adafruit-circuitpython-gfx-1.1.17/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:52:10.767732 adafruit-circuitpython-gfx-1.1.17/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:52:10.767732 adafruit-circuitpython-gfx-1.1.17/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:52:10.771731 adafruit-circuitpython-gfx-1.1.17/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19269 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/LICENSES/CC-BY-NC-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-21 16:52:10.771731 adafruit-circuitpython-gfx-1.1.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:52:10.771731 adafruit-circuitpython-gfx-1.1.17/adafruit_circuitpython_gfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-21 16:52:10.000000 adafruit-circuitpython-gfx-1.1.17/adafruit_circuitpython_gfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-21 16:52:10.000000 adafruit-circuitpython-gfx-1.1.17/adafruit_circuitpython_gfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 16:52:10.000000 adafruit-circuitpython-gfx-1.1.17/adafruit_circuitpython_gfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-21 16:52:10.000000 adafruit-circuitpython-gfx-1.1.17/adafruit_circuitpython_gfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-21 16:52:10.000000 adafruit-circuitpython-gfx-1.1.17/adafruit_circuitpython_gfx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:52:10.771731 adafruit-circuitpython-gfx-1.1.17/adafruit_gfx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:52:10.771731 adafruit-circuitpython-gfx-1.1.17/adafruit_gfx/fonts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4755 2023-03-21 16:52:03.000000 adafruit-circuitpython-gfx-1.1.17/adafruit_gfx/fonts/gfx_standard_font_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19787 2023-03-21 16:52:03.000000 adafruit-circuitpython-gfx-1.1.17/adafruit_gfx/gfx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:52:10.771731 adafruit-circuitpython-gfx-1.1.17/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:52:10.771731 adafruit-circuitpython-gfx-1.1.17/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:52:10.771731 adafruit-circuitpython-gfx-1.1.17/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-03-21 16:52:03.000000 adafruit-circuitpython-gfx-1.1.17/examples/gfx_ili9341_randlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2587 2023-03-21 16:52:03.000000 adafruit-circuitpython-gfx-1.1.17/examples/gfx_ili9341_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 16:52:03.000000 adafruit-circuitpython-gfx-1.1.17/examples/gfx_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-03-21 16:52:03.000000 adafruit-circuitpython-gfx-1.1.17/font_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-21 16:52:03.000000 adafruit-circuitpython-gfx-1.1.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-21 16:51:51.000000 adafruit-circuitpython-gfx-1.1.17/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 16:52:10.771731 adafruit-circuitpython-gfx-1.1.17/setup.cfg
```

### Comparing `adafruit-circuitpython-gfx-1.1.16/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-gfx-1.1.17/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/.gitignore` & `adafruit-circuitpython-gfx-1.1.17/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/.pre-commit-config.yaml` & `adafruit-circuitpython-gfx-1.1.17/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/.pylintrc` & `adafruit-circuitpython-gfx-1.1.17/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-gfx-1.1.17/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/LICENSE` & `adafruit-circuitpython-gfx-1.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-gfx-1.1.17/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/LICENSES/CC-BY-NC-3.0.txt` & `adafruit-circuitpython-gfx-1.1.17/LICENSES/CC-BY-NC-3.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/LICENSES/MIT.txt` & `adafruit-circuitpython-gfx-1.1.17/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/LICENSES/Unlicense.txt` & `adafruit-circuitpython-gfx-1.1.17/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/PKG-INFO` & `adafruit-circuitpython-gfx-1.1.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-gfx
-Version: 1.1.16
+Version: 1.1.17
 Summary: CircuitPython pixel graphics drawing library
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_GFX
 Keywords: adafruit,gfx,graphics,display,pixel,drawing,hardware,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-gfx-1.1.16/README.rst` & `adafruit-circuitpython-gfx-1.1.17/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/adafruit_circuitpython_gfx.egg-info/PKG-INFO` & `adafruit-circuitpython-gfx-1.1.17/adafruit_circuitpython_gfx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-gfx
-Version: 1.1.16
+Version: 1.1.17
 Summary: CircuitPython pixel graphics drawing library
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_GFX
 Keywords: adafruit,gfx,graphics,display,pixel,drawing,hardware,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-gfx-1.1.16/adafruit_circuitpython_gfx.egg-info/SOURCES.txt` & `adafruit-circuitpython-gfx-1.1.17/adafruit_circuitpython_gfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/adafruit_gfx/fonts/gfx_standard_font_01.py` & `adafruit-circuitpython-gfx-1.1.17/adafruit_gfx/fonts/gfx_standard_font_01.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/adafruit_gfx/gfx.py` & `adafruit-circuitpython-gfx-1.1.17/adafruit_gfx/gfx.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
-__version__ = "1.1.16"
+__version__ = "1.1.17"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_GFX.git"
 
 # pylint: disable=invalid-name
 class GFX:
     # pylint: disable=too-many-instance-attributes
     """Create an instance of the GFX drawing class.
```

### Comparing `adafruit-circuitpython-gfx-1.1.16/docs/_static/favicon.ico` & `adafruit-circuitpython-gfx-1.1.17/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/docs/conf.py` & `adafruit-circuitpython-gfx-1.1.17/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/docs/index.rst` & `adafruit-circuitpython-gfx-1.1.17/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/examples/gfx_ili9341_randlines.py` & `adafruit-circuitpython-gfx-1.1.17/examples/gfx_ili9341_randlines.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/examples/gfx_ili9341_test.py` & `adafruit-circuitpython-gfx-1.1.17/examples/gfx_ili9341_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.16/font_maker.py` & `adafruit-circuitpython-gfx-1.1.17/font_maker.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 # Attribution-NonCommercial 3.0 United States (CC BY-NC 3.0 US)
 # Author: Jonah Yolles-Murphy on Date: 10/12/18
 
 """`TG-Modules.TG-RGB.rgb`
 a dictionary of bytes organised to create basic text, just the templates
 Author(s):Jonah Yolles-Murphy
 imspiration for base letter style from Ben Gelb"""
-__version__ = "1.0"
+
+__version__ = "1.1.17"
+__repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_GFX.git"
 
 
 text_dict = {
     "Height": 7,
     "Width": 5,
     "A": (0b10111111, 0b11000100, 0b11000100, 0b11000100, 0b10111111),
     "B": (0b11111111, 0b11000001, 0b11001001, 0b11001001, 0b10110110),
```

### Comparing `adafruit-circuitpython-gfx-1.1.16/pyproject.toml` & `adafruit-circuitpython-gfx-1.1.17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-gfx"
 description = "CircuitPython pixel graphics drawing library"
-version = "1.1.16"
+version = "1.1.17"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_GFX"}
 keywords = [
     "adafruit",
```

