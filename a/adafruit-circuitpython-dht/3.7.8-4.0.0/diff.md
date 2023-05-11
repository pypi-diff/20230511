# Comparing `tmp/adafruit-circuitpython-dht-3.7.8.tar.gz` & `tmp/adafruit-circuitpython-dht-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-dht-3.7.8.tar", last modified: Tue Nov 15 19:01:19 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-dht-4.0.0.tar", last modified: Thu May 11 18:24:41 2023, max compression
```

## Comparing `adafruit-circuitpython-dht-3.7.8.tar` & `adafruit-circuitpython-dht-4.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:01:19.845157 adafruit-circuitpython-dht-3.7.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:01:19.841158 adafruit-circuitpython-dht-3.7.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:01:19.841158 adafruit-circuitpython-dht-3.7.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:01:19.841158 adafruit-circuitpython-dht-3.7.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:01:19.841158 adafruit-circuitpython-dht-3.7.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5625 2022-11-15 19:01:19.845157 adafruit-circuitpython-dht-3.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4844 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:01:19.845157 adafruit-circuitpython-dht-3.7.8/adafruit_circuitpython_dht.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5625 2022-11-15 19:01:19.000000 adafruit-circuitpython-dht-3.7.8/adafruit_circuitpython_dht.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-11-15 19:01:19.000000 adafruit-circuitpython-dht-3.7.8/adafruit_circuitpython_dht.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 19:01:19.000000 adafruit-circuitpython-dht-3.7.8/adafruit_circuitpython_dht.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-15 19:01:19.000000 adafruit-circuitpython-dht-3.7.8/adafruit_circuitpython_dht.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-15 19:01:19.000000 adafruit-circuitpython-dht-3.7.8/adafruit_circuitpython_dht.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11743 2022-11-15 19:01:12.000000 adafruit-circuitpython-dht-3.7.8/adafruit_dht.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:01:19.845157 adafruit-circuitpython-dht-3.7.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:01:19.845157 adafruit-circuitpython-dht-3.7.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5659 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:01:19.845157 adafruit-circuitpython-dht-3.7.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-11-15 19:01:12.000000 adafruit-circuitpython-dht-3.7.8/examples/dht_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3380 2022-11-15 19:01:12.000000 adafruit-circuitpython-dht-3.7.8/examples/dht_time_calibration_advance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-11-15 19:01:12.000000 adafruit-circuitpython-dht-3.7.8/examples/dht_to_led_display.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-11-15 19:01:12.000000 adafruit-circuitpython-dht-3.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-11-15 19:01:04.000000 adafruit-circuitpython-dht-3.7.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 19:01:19.845157 adafruit-circuitpython-dht-3.7.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:24:41.870685 adafruit-circuitpython-dht-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:24:41.862685 adafruit-circuitpython-dht-4.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:24:41.866685 adafruit-circuitpython-dht-4.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:24:41.866685 adafruit-circuitpython-dht-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:24:41.866685 adafruit-circuitpython-dht-4.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-11 18:24:41.870685 adafruit-circuitpython-dht-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:24:41.866685 adafruit-circuitpython-dht-4.0.0/adafruit_circuitpython_dht.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-11 18:24:41.000000 adafruit-circuitpython-dht-4.0.0/adafruit_circuitpython_dht.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-11 18:24:41.000000 adafruit-circuitpython-dht-4.0.0/adafruit_circuitpython_dht.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:24:41.000000 adafruit-circuitpython-dht-4.0.0/adafruit_circuitpython_dht.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 18:24:41.000000 adafruit-circuitpython-dht-4.0.0/adafruit_circuitpython_dht.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 18:24:41.000000 adafruit-circuitpython-dht-4.0.0/adafruit_circuitpython_dht.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11744 2023-05-11 18:24:32.000000 adafruit-circuitpython-dht-4.0.0/adafruit_dht.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:24:41.870685 adafruit-circuitpython-dht-4.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:24:41.870685 adafruit-circuitpython-dht-4.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:24:41.870685 adafruit-circuitpython-dht-4.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-11 18:24:32.000000 adafruit-circuitpython-dht-4.0.0/examples/dht_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-11 18:24:32.000000 adafruit-circuitpython-dht-4.0.0/examples/dht_time_calibration_advance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-11 18:24:32.000000 adafruit-circuitpython-dht-4.0.0/examples/dht_to_led_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 18:24:32.000000 adafruit-circuitpython-dht-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-11 18:24:21.000000 adafruit-circuitpython-dht-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:24:41.870685 adafruit-circuitpython-dht-4.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-dht-3.7.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-dht-4.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/.gitignore` & `adafruit-circuitpython-dht-4.0.0/.gitignore`

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

### Comparing `adafruit-circuitpython-dht-3.7.8/.pre-commit-config.yaml` & `adafruit-circuitpython-dht-4.0.0/.pre-commit-config.yaml`

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
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-dht-3.7.8/.pylintrc` & `adafruit-circuitpython-dht-4.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-dht-4.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/LICENSE` & `adafruit-circuitpython-dht-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-dht-4.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/LICENSES/MIT.txt` & `adafruit-circuitpython-dht-4.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-dht-4.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/PKG-INFO` & `adafruit-circuitpython-dht-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dht
-Version: 3.7.8
+Version: 4.0.0
 Summary: CircuitPython support for DHT11 and DHT22 type temperature/humidity devices
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DHT
 Keywords: adafruit,dht,hardware,sensors,temperature,humidity,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-dht-3.7.8/README.rst` & `adafruit-circuitpython-dht-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/adafruit_circuitpython_dht.egg-info/PKG-INFO` & `adafruit-circuitpython-dht-4.0.0/adafruit_circuitpython_dht.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dht
-Version: 3.7.8
+Version: 4.0.0
 Summary: CircuitPython support for DHT11 and DHT22 type temperature/humidity devices
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DHT
 Keywords: adafruit,dht,hardware,sensors,temperature,humidity,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-dht-3.7.8/adafruit_circuitpython_dht.egg-info/SOURCES.txt` & `adafruit-circuitpython-dht-4.0.0/adafruit_circuitpython_dht.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/adafruit_dht.py` & `adafruit-circuitpython-dht-4.0.0/adafruit_dht.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 try:
     # Used only for typing
     from typing import Union
     from microcontroller import Pin
 except ImportError:
     pass
 
-__version__ = "3.7.8"
+__version__ = "4.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DHT.git"
 
 
 class DHTBase:
     """base support for DHT11 and DHT22 devices
 
     :param bool dht11: True if device is DHT11, otherwise DHT22.
@@ -75,15 +75,15 @@
         self._trig_wait = trig_wait
         self._max_pulses = max_pulses
         self._last_called = 0
         self._humidity = None
         self._temperature = None
         self._use_pulseio = use_pulseio
         if "Linux" not in uname() and not self._use_pulseio:
-            raise Exception("Bitbanging is not supported when using CircuitPython.")
+            raise ValueError("Bitbanging is not supported when using CircuitPython.")
         # We don't use a context because linux-based systems are sluggish
         # and we're better off having a running process
         if self._use_pulseio:
             self.pulse_in = PulseIn(self._pin, maxlen=self._max_pulses, idle_state=True)
             self.pulse_in.pause()
 
     def exit(self) -> None:
```

### Comparing `adafruit-circuitpython-dht-3.7.8/docs/_static/favicon.ico` & `adafruit-circuitpython-dht-4.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/docs/conf.py` & `adafruit-circuitpython-dht-4.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/docs/examples.rst` & `adafruit-circuitpython-dht-4.0.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/docs/index.rst` & `adafruit-circuitpython-dht-4.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/examples/dht_simpletest.py` & `adafruit-circuitpython-dht-4.0.0/examples/dht_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/examples/dht_time_calibration_advance.py` & `adafruit-circuitpython-dht-4.0.0/examples/dht_time_calibration_advance.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/examples/dht_to_led_display.py` & `adafruit-circuitpython-dht-4.0.0/examples/dht_to_led_display.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-3.7.8/pyproject.toml` & `adafruit-circuitpython-dht-4.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-dht"
 description = "CircuitPython support for DHT11 and DHT22 type temperature/humidity devices"
-version = "3.7.8"
+version = "4.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_DHT"}
 keywords = [
     "adafruit",
```

