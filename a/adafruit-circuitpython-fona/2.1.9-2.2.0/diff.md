# Comparing `tmp/adafruit-circuitpython-fona-2.1.9.tar.gz` & `tmp/adafruit-circuitpython-fona-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-fona-2.1.9.tar", last modified: Tue Jun  7 17:25:26 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-fona-2.2.0.tar", last modified: Thu May 11 14:18:31 2023, max compression
```

## Comparing `adafruit-circuitpython-fona-2.1.9.tar` & `adafruit-circuitpython-fona-2.2.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.790668 adafruit-circuitpython-fona-2.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.782668 adafruit-circuitpython-fona-2.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.786668 adafruit-circuitpython-fona-2.1.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.786668 adafruit-circuitpython-fona-2.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.786668 adafruit-circuitpython-fona-2.1.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-06-07 17:25:26.790668 adafruit-circuitpython-fona-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2605 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.786668 adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-06-07 17:25:26.000000 adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-06-07 17:25:26.000000 adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:25:26.000000 adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-07 17:25:26.000000 adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-07 17:25:26.000000 adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.786668 adafruit-circuitpython-fona-2.1.9/adafruit_fona/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/adafruit_fona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33473 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/adafruit_fona/adafruit_fona.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2951 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/adafruit_fona/adafruit_fona_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     8162 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/adafruit_fona/adafruit_fona_socket.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10824 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/adafruit_fona/fona_3g.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.790668 adafruit-circuitpython-fona-2.1.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.790668 adafruit-circuitpython-fona-2.1.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5534 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.790668 adafruit-circuitpython-fona-2.1.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/examples/fona_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2407 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/examples/fona_cheerlights.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/examples/fona_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1267 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/examples/fona_sms.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1229 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/examples/fona_sms_response.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:25:26.790668 adafruit-circuitpython-fona-2.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:18:31.973379 adafruit-circuitpython-fona-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:18:31.965379 adafruit-circuitpython-fona-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:18:31.969379 adafruit-circuitpython-fona-2.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:18:31.969379 adafruit-circuitpython-fona-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:18:31.969379 adafruit-circuitpython-fona-2.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-11 14:18:31.973379 adafruit-circuitpython-fona-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:18:31.969379 adafruit-circuitpython-fona-2.2.0/adafruit_circuitpython_fona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-11 14:18:31.000000 adafruit-circuitpython-fona-2.2.0/adafruit_circuitpython_fona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-11 14:18:31.000000 adafruit-circuitpython-fona-2.2.0/adafruit_circuitpython_fona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:18:31.000000 adafruit-circuitpython-fona-2.2.0/adafruit_circuitpython_fona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 14:18:31.000000 adafruit-circuitpython-fona-2.2.0/adafruit_circuitpython_fona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 14:18:31.000000 adafruit-circuitpython-fona-2.2.0/adafruit_circuitpython_fona.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:18:31.969379 adafruit-circuitpython-fona-2.2.0/adafruit_fona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:18:24.000000 adafruit-circuitpython-fona-2.2.0/adafruit_fona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33787 2023-05-11 14:18:24.000000 adafruit-circuitpython-fona-2.2.0/adafruit_fona/adafruit_fona.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3362 2023-05-11 14:18:24.000000 adafruit-circuitpython-fona-2.2.0/adafruit_fona/adafruit_fona_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-11 14:18:24.000000 adafruit-circuitpython-fona-2.2.0/adafruit_fona/adafruit_fona_socket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10817 2023-05-11 14:18:24.000000 adafruit-circuitpython-fona-2.2.0/adafruit_fona/fona_3g.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:18:31.973379 adafruit-circuitpython-fona-2.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:18:31.973379 adafruit-circuitpython-fona-2.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:18:31.973379 adafruit-circuitpython-fona-2.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-11 14:18:24.000000 adafruit-circuitpython-fona-2.2.0/examples/fona_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2407 2023-05-11 14:18:24.000000 adafruit-circuitpython-fona-2.2.0/examples/fona_cheerlights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-11 14:18:24.000000 adafruit-circuitpython-fona-2.2.0/examples/fona_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1267 2023-05-11 14:18:24.000000 adafruit-circuitpython-fona-2.2.0/examples/fona_sms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1229 2023-05-11 14:18:24.000000 adafruit-circuitpython-fona-2.2.0/examples/fona_sms_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-11 14:18:24.000000 adafruit-circuitpython-fona-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 14:18:16.000000 adafruit-circuitpython-fona-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:18:31.973379 adafruit-circuitpython-fona-2.2.0/setup.cfg
```

### Comparing `adafruit-circuitpython-fona-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-fona-2.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.9/.gitignore` & `adafruit-circuitpython-fona-2.2.0/.gitignore`

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

### Comparing `adafruit-circuitpython-fona-2.1.9/.pre-commit-config.yaml` & `adafruit-circuitpython-fona-2.2.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
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
-          - --disable=consider-using-f-string,duplicate-code
+          - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
       - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
```

### Comparing `adafruit-circuitpython-fona-2.1.9/.pylintrc` & `adafruit-circuitpython-fona-2.2.0/.pylintrc`

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

### Comparing `adafruit-circuitpython-fona-2.1.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-fona-2.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.9/LICENSE` & `adafruit-circuitpython-fona-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-fona-2.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.9/LICENSES/MIT.txt` & `adafruit-circuitpython-fona-2.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-fona-2.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.9/PKG-INFO` & `adafruit-circuitpython-fona-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fona
-Version: 2.1.9
+Version: 2.2.0
 Summary: CircuitPython library for the Adafruit FONAA
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_FONA
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython fona fona,cellular
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_FONA
+Keywords: adafruit,blinka,circuitpython,micropython,fona,fona,,cellular
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
 
-.. image:: https://readthedocs.org/projects/adafruit-circuitpython-fona/badge/?version=latest
+.. image:: https://readthedocs.org/projects/fona/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/fona/en/latest/
     :alt: Documentation Status
 
 .. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
@@ -67,16 +66,16 @@
     sudo pip3 install adafruit-circuitpython-fona
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-fona
 
 Usage Example
 =============
 
 Please see the examples directory for code usage.
 
@@ -89,9 +88,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_FONA/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-fona-2.1.9/README.rst` & `adafruit-circuitpython-fona-2.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Introduction
 ============
 
-.. image:: https://readthedocs.org/projects/adafruit-circuitpython-fona/badge/?version=latest
+.. image:: https://readthedocs.org/projects/fona/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/fona/en/latest/
     :alt: Documentation Status
 
 .. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
@@ -48,16 +48,16 @@
     sudo pip3 install adafruit-circuitpython-fona
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-fona
 
 Usage Example
 =============
 
 Please see the examples directory for code usage.
```

### Comparing `adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/PKG-INFO` & `adafruit-circuitpython-fona-2.2.0/adafruit_circuitpython_fona.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fona
-Version: 2.1.9
+Version: 2.2.0
 Summary: CircuitPython library for the Adafruit FONAA
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_FONA
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython fona fona,cellular
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_FONA
+Keywords: adafruit,blinka,circuitpython,micropython,fona,fona,,cellular
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
 
-.. image:: https://readthedocs.org/projects/adafruit-circuitpython-fona/badge/?version=latest
+.. image:: https://readthedocs.org/projects/fona/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/fona/en/latest/
     :alt: Documentation Status
 
 .. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
@@ -67,16 +66,16 @@
     sudo pip3 install adafruit-circuitpython-fona
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-fona
 
 Usage Example
 =============
 
 Please see the examples directory for code usage.
 
@@ -89,9 +88,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_FONA/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/SOURCES.txt` & `adafruit-circuitpython-fona-2.2.0/adafruit_circuitpython_fona.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

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
 adafruit_circuitpython_fona.egg-info/PKG-INFO
 adafruit_circuitpython_fona.egg-info/SOURCES.txt
 adafruit_circuitpython_fona.egg-info/dependency_links.txt
 adafruit_circuitpython_fona.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-fona-2.1.9/adafruit_fona/adafruit_fona.py` & `adafruit-circuitpython-fona-2.2.0/adafruit_fona/adafruit_fona.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     try:
         from typing import Literal
     except ImportError:
         from typing_extensions import Literal
 except ImportError:
     pass
 
-__version__ = "0.0.0-auto.0"
+__version__ = "2.2.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FONA.git"
 
 FONA_DEFAULT_TIMEOUT_MS = 500  # TODO: Check this against arduino...
 
 # Commands
 CMD_AT = b"AT"
 # Replies
@@ -52,14 +52,15 @@
 
 # Maximum number of fona800 and fona808 sockets
 FONA_MAX_SOCKETS = const(6)
 
 # FONA Versions
 FONA_800_L = const(0x01)
 FONA_800_H = const(0x6)
+FONA_800_C = const(0x7)
 FONA_808_V1 = const(0x2)
 FONA_808_V2 = const(0x3)
 FONA_3G_A = const(0x4)
 FONA_3G_E = const(0x5)
 
 # FONA preferred SMS storage
 FONA_SMS_STORAGE_SIM = b'"SM"'  # Storage on the SIM
@@ -67,28 +68,28 @@
 
 
 # pylint: disable=too-many-instance-attributes, too-many-public-methods
 class FONA:
     """CircuitPython FONA module interface.
 
     :param ~busio.UART uart: FONA UART connection.
-    :param ~digitalio.DigitalInOut rdt: FONA RST pin.
+    :param ~digitalio.DigitalInOut rst: FONA RST pin.
     :param ~digitalio.DigitalInOut ri: Optional FONA Ring Interrupt (RI) pin.
     :param bool debug: Enable debugging output.
     """
 
     TCP_MODE = const(0)  # TCP socket
     UDP_MODE = const(1)  # UDP socket
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         uart: UART,
         rst: DigitalInOut,
-        ri: Optional[DigitalInOut] = None,
+        ri: Optional[DigitalInOut] = None,  # pylint: disable=invalid-name
         debug: bool = False,
     ) -> None:
         self._buf = b""  # shared buffer
         self._fona_type = 0
         self._debug = debug
 
         self._uart = uart
@@ -143,22 +144,28 @@
             self._fona_type = FONA_808_V2
         elif self._buf.find(b"SIM808 R13") != -1:
             self._fona_type = FONA_808_V1
         elif self._buf.find(b"SIMCOM_SIM5320A") != -1:
             self._fona_type = FONA_3G_A
         elif self._buf.find(b"SIMCOM_SIM5320E") != -1:
             self._fona_type = FONA_3G_E
-
-        if self._fona_type == FONA_800_L:
-            # determine if SIM800H
+        elif self._buf.find(b"SIM800") != -1:
             self._uart_write(b"AT+GMM\r\n")
             self._read_line(multiline=True)
 
             if self._buf.find(b"SIM800H") != -1:
                 self._fona_type = FONA_800_H
+            elif self._buf.find(b"SIM800L") != -1:
+                self._fona_type = FONA_800_L
+            elif self._buf.find(b"SIM800C") != -1:
+                self._fona_type = FONA_800_C
+
+        if self._debug and self._fona_type == 0:
+            print(f"Unsupported module: {self._buf}")
+
         return True
 
     def factory_reset(self) -> bool:
         """Resets modem to factory configuration."""
         self._uart_write(b"ATZ\r\n")
 
         if not self._expect_reply(REPLY_OK):
@@ -362,15 +369,15 @@
         if self._debug:
             print("GPS Fix")
         if self._fona_type == FONA_808_V2:
             # 808 V2 uses GNS commands and doesn't have an explicit 2D/3D fix status.
             # Instead just look for a fix and if found assume it's a 3D fix.
             self._get_reply(b"AT+CGNSINF")
 
-            if not b"+CGNSINF: " in self._buf:
+            if b"+CGNSINF: " not in self._buf:
                 return False
 
             status = int(self._buf[10:11].decode("utf-8"))
             if status == 1:
                 status = 3  # assume 3D fix
             self._read_line()
         else:
```

### Comparing `adafruit-circuitpython-fona-2.1.9/adafruit_fona/adafruit_fona_network.py` & `adafruit-circuitpython-fona-2.2.0/adafruit_fona/adafruit_fona_network.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 try:
     from typing import Optional, Tuple, Type
     from types import TracebackType
     from adafruit_fona.adafruit_fona import FONA
 except ImportError:
     pass
 
-__version__ = "0.0.0-auto.0"
+__version__ = "2.2.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FONA.git"
 
 # Network types
 NET_GSM = 0x01
 NET_CDMA = 0x02
 
 
@@ -37,19 +37,26 @@
 
     def __init__(
         self, fona: FONA, apn: Tuple[str, Optional[str], Optional[str]]
     ) -> None:
         self._iface = fona
         self._apn = apn
         self._network_connected = False
-        self._network_type = NET_CDMA
+        self._network_type = NET_GSM
+        self._has_gps = False
 
-        if not self._iface.version == 0x4 or self._iface.version == 0x5:
-            self._network_type = NET_GSM
+        # These are numbers defined in adafruit_fona FONA versions
+        # For some reason, we can't import them from the adafruit_fona file
+
+        if self._iface.version in (0x4, 0x5):
+            self._network_type = NET_CDMA
+
+        if self._iface.version in (0x2, 0x3, 0x4, 0x5):
             self._iface.gps = True
+            self._has_gps = True
 
     def __enter__(self) -> "CELLULAR":
         return self
 
     def __exit__(
         self,
         exception_type: Optional[Type[type]],
@@ -68,15 +75,22 @@
         """Returns the SIM card's ICCID, as a string."""
         return self._iface.iccid
 
     @property
     def is_attached(self) -> bool:
         """Returns if the modem is attached to the network."""
         if self._network_type == NET_GSM:
-            if self._iface.gps == 3 and self._iface.network_status == 1:
+            if (
+                self._has_gps
+                and self._iface.gps == 3
+                and self._iface.network_status == 1
+            ):
+                return True
+
+            if not self._has_gps and self._iface.network_status == 1:
                 return True
         else:  # Attach CDMA network
             if self._iface.ue_system_info == 1 and self._iface.network_status == 1:
                 return True
         return False
 
     @property
```

### Comparing `adafruit-circuitpython-fona-2.1.9/adafruit_fona/adafruit_fona_socket.py` & `adafruit-circuitpython-fona-2.2.0/adafruit_fona/adafruit_fona_socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 SOCK_DGRAM = const(0x01)  # UDP
 AF_INET = const(3)
 NO_SOCKET_AVAIL = const(255)
 
 # keep track of sockets we allocate
 SOCKETS = []
 
+
 # pylint: disable=too-many-arguments, unused-argument
 def getaddrinfo(host, port: int, family=0, socktype=0, proto=0, flags=0):
     """Translate the host/port argument into a sequence of 5-tuples that
     contain all the necessary arguments for creating a socket connected to that service.
     """
     if not isinstance(port, int):
         raise RuntimeError("Port must be an integer")
@@ -226,15 +227,15 @@
 
     def settimeout(self, value: int) -> None:
         """Sets socket read timeout.
 
         :param int value: Socket read timeout, in seconds.
         """
         if value < 0:
-            raise Exception("Timeout period should be non-negative.")
+            raise ValueError("Timeout period should be non-negative.")
         self._timeout = value
 
     def gettimeout(self) -> int:
         """Return the timeout in seconds (float) associated
         with socket operations, or None if no timeout is set.
         """
         return self._timeout
```

### Comparing `adafruit-circuitpython-fona-2.1.9/adafruit_fona/fona_3g.py` & `adafruit-circuitpython-fona-2.2.0/adafruit_fona/fona_3g.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     try:
         from typing import Literal
     except ImportError:
         from typing_extensions import Literal
 except ImportError:
     pass
 
-__version__ = "0.0.0-auto.0"
+__version__ = "2.2.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FONA.git"
 
 FONA_MAX_SOCKETS = const(10)
 
 
 class FONA3G(FONA):
     """FONA 3G module interface.
```

### Comparing `adafruit-circuitpython-fona-2.1.9/docs/_static/favicon.ico` & `adafruit-circuitpython-fona-2.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.9/docs/conf.py` & `adafruit-circuitpython-fona-2.2.0/docs/conf.py`

 * *Files 5% similar despite different names*

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
@@ -43,15 +44,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit FONA Library"
-copyright = "2020 Brent Rubell, ladyada"
+creation_year = "2020"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Brent Rubell, ladyada"
 author = "Brent Rubell, ladyada"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-fona-2.1.9/docs/index.rst` & `adafruit-circuitpython-fona-2.2.0/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 
     Adafruit FONA808 Breakout <https://www.adafruit.com/product/2542>
     Adafruit FONA808 Shield <https://www.adafruit.com/product/2636>
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_FONA/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_FONA/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-fona-2.1.9/examples/fona_aio_post.py` & `adafruit-circuitpython-fona-2.2.0/examples/fona_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.9/examples/fona_cheerlights.py` & `adafruit-circuitpython-fona-2.2.0/examples/fona_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.9/examples/fona_simpletest.py` & `adafruit-circuitpython-fona-2.2.0/examples/fona_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.9/examples/fona_sms.py` & `adafruit-circuitpython-fona-2.2.0/examples/fona_sms.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.9/examples/fona_sms_response.py` & `adafruit-circuitpython-fona-2.2.0/examples/fona_sms_response.py`

 * *Files identical despite different names*

