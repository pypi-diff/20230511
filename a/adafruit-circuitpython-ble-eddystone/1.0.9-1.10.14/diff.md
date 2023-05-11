# Comparing `tmp/adafruit-circuitpython-ble-eddystone-1.0.9.tar.gz` & `tmp/adafruit-circuitpython-ble-eddystone-1.10.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-eddystone-1.0.9.tar", last modified: Tue Jun  7 17:20:27 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-eddystone-1.10.14.tar", last modified: Thu May 11 18:27:29 2023, max compression
```

## Comparing `adafruit-circuitpython-ble-eddystone-1.0.9.tar` & `adafruit-circuitpython-ble-eddystone-1.10.14.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:20:27.025656 adafruit-circuitpython-ble-eddystone-1.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:20:27.021656 adafruit-circuitpython-ble-eddystone-1.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:20:27.021656 adafruit-circuitpython-ble-eddystone-1.0.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:20:27.025656 adafruit-circuitpython-ble-eddystone-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:20:27.025656 adafruit-circuitpython-ble-eddystone-1.0.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-06-07 17:20:27.025656 adafruit-circuitpython-ble-eddystone-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:20:27.025656 adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_ble_eddystone/
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_ble_eddystone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_ble_eddystone/uid.py
--rw-r--r--   0 runner    (1001) docker     (121)     3019 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_ble_eddystone/url.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:20:27.025656 adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_circuitpython_ble_eddystone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-06-07 17:20:26.000000 adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_circuitpython_ble_eddystone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-06-07 17:20:26.000000 adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_circuitpython_ble_eddystone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:20:26.000000 adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_circuitpython_ble_eddystone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-06-07 17:20:26.000000 adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_circuitpython_ble_eddystone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-07 17:20:26.000000 adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_circuitpython_ble_eddystone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:20:27.025656 adafruit-circuitpython-ble-eddystone-1.0.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:20:27.025656 adafruit-circuitpython-ble-eddystone-1.0.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5475 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:20:27.025656 adafruit-circuitpython-ble-eddystone-1.0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/examples/ble_eddystone_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:20:27.025656 adafruit-circuitpython-ble-eddystone-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1939 2022-06-07 17:20:14.000000 adafruit-circuitpython-ble-eddystone-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.020913 adafruit-circuitpython-ble-eddystone-1.10.14/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.020913 adafruit-circuitpython-ble-eddystone-1.10.14/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.020913 adafruit-circuitpython-ble-eddystone-1.10.14/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.020913 adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.020913 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-11 18:27:21.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-11 18:27:21.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-11 18:27:21.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-11 18:27:29.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-11 18:27:29.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:27:29.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 18:27:29.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 18:27:29.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 18:27:21.000000 adafruit-circuitpython-ble-eddystone-1.10.14/examples/ble_eddystone_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-11 18:27:21.000000 adafruit-circuitpython-ble-eddystone-1.10.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/setup.cfg
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-eddystone-1.10.14/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/.gitignore` & `adafruit-circuitpython-ble-eddystone-1.10.14/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-eddystone-1.10.14/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/.pylintrc` & `adafruit-circuitpython-ble-eddystone-1.10.14/.pylintrc`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-eddystone-1.10.14/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/LICENSE` & `adafruit-circuitpython-ble-eddystone-1.10.14/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/PKG-INFO` & `adafruit-circuitpython-ble-eddystone-1.10.14/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: adafruit-circuitpython-ble-eddystone
-Version: 1.0.9
-Summary: CircuitPython BLE library for Google's open "physical web" Eddystone.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
-License: MIT
-Keywords: adafruit blinka circuitpython micropython ble_eddystone eddystone ble
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: System :: Hardware
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble_eddystone/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ble_eddystone/en/latest/
     :alt: Documentation Status
 
@@ -28,14 +9,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython BLE library for Google's open "physical web" Eddystone.
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -62,16 +47,16 @@
     sudo pip3 install adafruit-circuitpython-ble-eddystone
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ble-eddystone
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -110,9 +95,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_ble_eddystone/__init__.py` & `adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import struct
 
 from adafruit_ble.advertising import Advertisement
 from adafruit_ble.advertising.standard import ServiceList, ServiceData
 from adafruit_ble.uuid import StandardUUID
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.10.14"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone.git"
 
 
 class _EddystoneService:
     """Placeholder service. Not implemented."""
 
     # pylint: disable=too-few-public-methods
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_ble_eddystone/uid.py` & `adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/uid.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Static Eddystone UID advertisement. Documented by Google here:
 https://github.com/google/eddystone/tree/master/eddystone-uid
 
 """
 
 from . import EddystoneAdvertisement, EddystoneFrameStruct, EddystoneFrameBytes
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.10.14"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone.git"
 
 
 class EddystoneUID(EddystoneAdvertisement):  # pylint: disable=too-few-public-methods
     """Static Eddystone unique identifier.
 
     :param bytes instance_id: instance component of the id. 10 bytes long
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_ble_eddystone/url.py` & `adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Eddystone URL advertisement. Documented by Google here:
 https://github.com/google/eddystone/tree/master/eddystone-url
 
 """
 
 from . import EddystoneAdvertisement, EddystoneFrameStruct, EddystoneFrameBytes
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.10.14"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone.git"
 
 # These prefixes are replaced with a single one-byte scheme number.
 _URL_SCHEMES = (b"http://www.", b"https://www.", b"http://", b"https://")
 
 # These common domains are replaced with a single non-printing byte.
 # Byte value is 0-6 for these with a '/' suffix.
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_circuitpython_ble_eddystone.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-eddystone-1.10.14/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-eddystone
-Version: 1.0.9
-Summary: CircuitPython BLE library for Google's open "physical web" Eddystone.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Version: 1.10.14
+Summary: CircuitPython BLE library for Google's open 'physical web' Eddystone.
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython ble_eddystone eddystone ble
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone
+Keywords: adafruit,blinka,circuitpython,micropython,ble_eddystone,eddystone,ble
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble_eddystone/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ble_eddystone/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython BLE library for Google's open "physical web" Eddystone.
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -62,16 +65,16 @@
     sudo pip3 install adafruit-circuitpython-ble-eddystone
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ble-eddystone
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -110,9 +113,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/adafruit_circuitpython_ble_eddystone.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
+optional_requirements.txt
+pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_ble_eddystone/__init__.py
 adafruit_ble_eddystone/uid.py
 adafruit_ble_eddystone/url.py
 adafruit_circuitpython_ble_eddystone.egg-info/PKG-INFO
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-eddystone-1.10.14/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/docs/conf.py` & `adafruit-circuitpython-ble-eddystone-1.10.14/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -21,15 +22,15 @@
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
-autodoc_mock_imports = ["bleak"]
+autodoc_mock_imports = ["bleak", "_bleio"]
 
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
 }
 
@@ -39,15 +40,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit BLE_Eddystone Library"
-copyright = "2020 Scott Shawcroft"
+creation_year = "2020"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Scott Shawcroft"
 author = "Scott Shawcroft"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/docs/index.rst` & `adafruit-circuitpython-ble-eddystone-1.10.14/docs/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 .. toctree::
     :caption: Related Products
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.0.9/examples/ble_eddystone_simpletest.py` & `adafruit-circuitpython-ble-eddystone-1.10.14/examples/ble_eddystone_simpletest.py`

 * *Files identical despite different names*

