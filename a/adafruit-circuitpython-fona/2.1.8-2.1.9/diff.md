# Comparing `tmp/adafruit-circuitpython-fona-2.1.8.tar.gz` & `tmp/adafruit-circuitpython-fona-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-fona-2.1.8.tar", last modified: Fri May 20 00:41:17 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-fona-2.1.9.tar", last modified: Tue Jun  7 17:25:26 2022, max compression
```

## Comparing `adafruit-circuitpython-fona-2.1.8.tar` & `adafruit-circuitpython-fona-2.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:41:17.926759 adafruit-circuitpython-fona-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:41:17.918758 adafruit-circuitpython-fona-2.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:41:17.918758 adafruit-circuitpython-fona-2.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:41:17.918758 adafruit-circuitpython-fona-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:41:17.918758 adafruit-circuitpython-fona-2.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-05-20 00:41:17.926759 adafruit-circuitpython-fona-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2605 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:41:17.922759 adafruit-circuitpython-fona-2.1.8/adafruit_circuitpython_fona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-05-20 00:41:17.000000 adafruit-circuitpython-fona-2.1.8/adafruit_circuitpython_fona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-05-20 00:41:17.000000 adafruit-circuitpython-fona-2.1.8/adafruit_circuitpython_fona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 00:41:17.000000 adafruit-circuitpython-fona-2.1.8/adafruit_circuitpython_fona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-20 00:41:17.000000 adafruit-circuitpython-fona-2.1.8/adafruit_circuitpython_fona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-05-20 00:41:17.000000 adafruit-circuitpython-fona-2.1.8/adafruit_circuitpython_fona.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:41:17.922759 adafruit-circuitpython-fona-2.1.8/adafruit_fona/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/adafruit_fona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33473 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/adafruit_fona/adafruit_fona.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2951 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/adafruit_fona/adafruit_fona_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     8162 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/adafruit_fona/adafruit_fona_socket.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10824 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/adafruit_fona/fona_3g.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:41:17.922759 adafruit-circuitpython-fona-2.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:41:17.922759 adafruit-circuitpython-fona-2.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5534 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:41:17.926759 adafruit-circuitpython-fona-2.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/examples/fona_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2407 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/examples/fona_cheerlights.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/examples/fona_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1267 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/examples/fona_sms.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1229 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/examples/fona_sms_response.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-20 00:41:17.926759 adafruit-circuitpython-fona-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-05-20 00:41:04.000000 adafruit-circuitpython-fona-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.790668 adafruit-circuitpython-fona-2.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.782668 adafruit-circuitpython-fona-2.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.786668 adafruit-circuitpython-fona-2.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.786668 adafruit-circuitpython-fona-2.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.786668 adafruit-circuitpython-fona-2.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-06-07 17:25:26.790668 adafruit-circuitpython-fona-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2605 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.786668 adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-06-07 17:25:26.000000 adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-06-07 17:25:26.000000 adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:25:26.000000 adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-07 17:25:26.000000 adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-07 17:25:26.000000 adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.786668 adafruit-circuitpython-fona-2.1.9/adafruit_fona/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/adafruit_fona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33473 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/adafruit_fona/adafruit_fona.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2951 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/adafruit_fona/adafruit_fona_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8162 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/adafruit_fona/adafruit_fona_socket.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10824 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/adafruit_fona/fona_3g.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.790668 adafruit-circuitpython-fona-2.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.790668 adafruit-circuitpython-fona-2.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5534 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:25:26.790668 adafruit-circuitpython-fona-2.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/examples/fona_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2407 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/examples/fona_cheerlights.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/examples/fona_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1267 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/examples/fona_sms.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1229 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/examples/fona_sms_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:25:26.790668 adafruit-circuitpython-fona-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-06-07 17:25:13.000000 adafruit-circuitpython-fona-2.1.9/setup.py
```

### Comparing `adafruit-circuitpython-fona-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-fona-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-fona-2.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-fona-2.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/.gitignore` & `adafruit-circuitpython-fona-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-fona-2.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/.pylintrc` & `adafruit-circuitpython-fona-2.1.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
@@ -248,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-fona-2.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-fona-2.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/LICENSE` & `adafruit-circuitpython-fona-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-fona-2.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-fona-2.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-fona-2.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/PKG-INFO` & `adafruit-circuitpython-fona-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fona
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for the Adafruit FONAA
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_FONA
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython fona fona,cellular
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-fona-2.1.8/README.rst` & `adafruit-circuitpython-fona-2.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/adafruit_circuitpython_fona.egg-info/PKG-INFO` & `adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fona
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for the Adafruit FONAA
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_FONA
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython fona fona,cellular
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-fona-2.1.8/adafruit_circuitpython_fona.egg-info/SOURCES.txt` & `adafruit-circuitpython-fona-2.1.9/adafruit_circuitpython_fona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/adafruit_fona/adafruit_fona.py` & `adafruit-circuitpython-fona-2.1.9/adafruit_fona/adafruit_fona.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/adafruit_fona/adafruit_fona_network.py` & `adafruit-circuitpython-fona-2.1.9/adafruit_fona/adafruit_fona_network.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/adafruit_fona/adafruit_fona_socket.py` & `adafruit-circuitpython-fona-2.1.9/adafruit_fona/adafruit_fona_socket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/adafruit_fona/fona_3g.py` & `adafruit-circuitpython-fona-2.1.9/adafruit_fona/fona_3g.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-fona-2.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/docs/conf.py` & `adafruit-circuitpython-fona-2.1.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-fona-2.1.8/docs/index.rst` & `adafruit-circuitpython-fona-2.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/examples/fona_aio_post.py` & `adafruit-circuitpython-fona-2.1.9/examples/fona_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/examples/fona_cheerlights.py` & `adafruit-circuitpython-fona-2.1.9/examples/fona_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/examples/fona_simpletest.py` & `adafruit-circuitpython-fona-2.1.9/examples/fona_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/examples/fona_sms.py` & `adafruit-circuitpython-fona-2.1.9/examples/fona_sms.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/examples/fona_sms_response.py` & `adafruit-circuitpython-fona-2.1.9/examples/fona_sms_response.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-2.1.8/setup.py` & `adafruit-circuitpython-fona-2.1.9/setup.py`

 * *Files identical despite different names*

