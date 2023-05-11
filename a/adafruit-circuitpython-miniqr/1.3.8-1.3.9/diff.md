# Comparing `tmp/adafruit-circuitpython-miniqr-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-miniqr-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-miniqr-1.3.8.tar", last modified: Fri Feb  4 20:17:36 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-miniqr-1.3.9.tar", last modified: Mon Apr  4 17:18:38 2022, max compression
```

## Comparing `adafruit-circuitpython-miniqr-1.3.8.tar` & `adafruit-circuitpython-miniqr-1.3.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:17:36.763078 adafruit-circuitpython-miniqr-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:17:36.759078 adafruit-circuitpython-miniqr-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:17:36.763078 adafruit-circuitpython-miniqr-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:17:36.763078 adafruit-circuitpython-miniqr-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:17:36.763078 adafruit-circuitpython-miniqr-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-02-04 20:17:36.763078 adafruit-circuitpython-miniqr-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2453 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:17:36.763078 adafruit-circuitpython-miniqr-1.3.8/adafruit_circuitpython_miniqr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-02-04 20:17:36.000000 adafruit-circuitpython-miniqr-1.3.8/adafruit_circuitpython_miniqr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-02-04 20:17:36.000000 adafruit-circuitpython-miniqr-1.3.8/adafruit_circuitpython_miniqr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:17:36.000000 adafruit-circuitpython-miniqr-1.3.8/adafruit_circuitpython_miniqr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-04 20:17:36.000000 adafruit-circuitpython-miniqr-1.3.8/adafruit_circuitpython_miniqr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20129 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/adafruit_miniqr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:17:36.763078 adafruit-circuitpython-miniqr-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:17:36.763078 adafruit-circuitpython-miniqr-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5411 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:17:36.763078 adafruit-circuitpython-miniqr-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/examples/miniqr_displaytest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/examples/miniqr_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:17:36.763078 adafruit-circuitpython-miniqr-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-02-04 20:17:26.000000 adafruit-circuitpython-miniqr-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:18:38.870864 adafruit-circuitpython-miniqr-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:18:38.866864 adafruit-circuitpython-miniqr-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:18:38.866864 adafruit-circuitpython-miniqr-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:18:38.866864 adafruit-circuitpython-miniqr-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:18:38.866864 adafruit-circuitpython-miniqr-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3176 2022-04-04 17:18:38.870864 adafruit-circuitpython-miniqr-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:18:38.870864 adafruit-circuitpython-miniqr-1.3.9/adafruit_circuitpython_miniqr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3176 2022-04-04 17:18:38.000000 adafruit-circuitpython-miniqr-1.3.9/adafruit_circuitpython_miniqr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-04-04 17:18:38.000000 adafruit-circuitpython-miniqr-1.3.9/adafruit_circuitpython_miniqr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-04 17:18:38.000000 adafruit-circuitpython-miniqr-1.3.9/adafruit_circuitpython_miniqr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-04 17:18:38.000000 adafruit-circuitpython-miniqr-1.3.9/adafruit_circuitpython_miniqr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    20128 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/adafruit_miniqr.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:18:38.870864 adafruit-circuitpython-miniqr-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:18:38.870864 adafruit-circuitpython-miniqr-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5411 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      893 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:18:38.870864 adafruit-circuitpython-miniqr-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/examples/miniqr_displaytest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/examples/miniqr_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-04 17:18:38.870864 adafruit-circuitpython-miniqr-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-04-04 17:18:28.000000 adafruit-circuitpython-miniqr-1.3.9/setup.py
```

### Comparing `adafruit-circuitpython-miniqr-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-miniqr-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-miniqr-1.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-miniqr-1.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-miniqr-1.3.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
 -   repo: https://github.com/python/black
-    rev: 20.8b1
+    rev: 22.3.0
     hooks:
     - id: black
 -   repo: https://github.com/fsfe/reuse-tool
     rev: v0.12.1
     hooks:
     - id: reuse
 -   repo: https://github.com/pre-commit/pre-commit-hooks
```

### Comparing `adafruit-circuitpython-miniqr-1.3.8/.pylintrc` & `adafruit-circuitpython-miniqr-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-miniqr-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/LICENSE` & `adafruit-circuitpython-miniqr-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-miniqr-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-miniqr-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-miniqr-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/PKG-INFO` & `adafruit-circuitpython-miniqr-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-miniqr
-Version: 1.3.8
+Version: 1.3.9
 Summary: A non-hardware dependant miniature QR generator library. All native Python!
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_miniQR
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit software miniqr qr generator python micropython circuitpython
 Platform: UNKNOWN
@@ -82,20 +82,17 @@
 	print(qr.matrix)
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/miniqr/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_miniQR/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-miniqr-1.3.8/README.rst` & `adafruit-circuitpython-miniqr-1.3.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,15 @@
 	print(qr.matrix)
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/miniqr/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_miniQR/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-miniqr-1.3.8/adafruit_circuitpython_miniqr.egg-info/PKG-INFO` & `adafruit-circuitpython-miniqr-1.3.9/adafruit_circuitpython_miniqr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-miniqr
-Version: 1.3.8
+Version: 1.3.9
 Summary: A non-hardware dependant miniature QR generator library. All native Python!
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_miniQR
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit software miniqr qr generator python micropython circuitpython
 Platform: UNKNOWN
@@ -82,20 +82,17 @@
 	print(qr.matrix)
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/miniqr/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_miniQR/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-miniqr-1.3.8/adafruit_circuitpython_miniqr.egg-info/SOURCES.txt` & `adafruit-circuitpython-miniqr-1.3.9/adafruit_circuitpython_miniqr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/adafruit_miniqr.py` & `adafruit-circuitpython-miniqr-1.3.9/adafruit_miniqr.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
         if mask == 7:
             return ((i * j) % 3 + (i + j) % 2) % 2 == 0
         raise ValueError("Bad mask pattern:" + mask)
         # pylint: enable=multiple-statements, too-many-return-statements
 
     @staticmethod
     def get_error_correct_polynomial(ecc_length):
-        """ Generate a ecc polynomial"""
+        """Generate a ecc polynomial"""
         poly = QRPolynomial([1], 0)
         for i in range(ecc_length):
             poly = poly.multiply(QRPolynomial([1, _gexp(i)], 0))
         return poly
 
 
 class QRPolynomial:
```

### Comparing `adafruit-circuitpython-miniqr-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-miniqr-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/docs/conf.py` & `adafruit-circuitpython-miniqr-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/docs/index.rst` & `adafruit-circuitpython-miniqr-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/examples/miniqr_displaytest.py` & `adafruit-circuitpython-miniqr-1.3.9/examples/miniqr_displaytest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/examples/miniqr_simpletest.py` & `adafruit-circuitpython-miniqr-1.3.9/examples/miniqr_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-1.3.8/setup.py` & `adafruit-circuitpython-miniqr-1.3.9/setup.py`

 * *Files identical despite different names*

