# Comparing `tmp/adafruit-circuitpython-mcp9600-1.3.5.tar.gz` & `tmp/adafruit-circuitpython-mcp9600-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mcp9600-1.3.5.tar", last modified: Fri Aug 26 02:26:03 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-mcp9600-1.3.6.tar", last modified: Thu Sep 22 18:18:19 2022, max compression
```

## Comparing `adafruit-circuitpython-mcp9600-1.3.5.tar` & `adafruit-circuitpython-mcp9600-1.3.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:03.621872 adafruit-circuitpython-mcp9600-1.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:03.613872 adafruit-circuitpython-mcp9600-1.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:03.613872 adafruit-circuitpython-mcp9600-1.3.5/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:03.613872 adafruit-circuitpython-mcp9600-1.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:03.617872 adafruit-circuitpython-mcp9600-1.3.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4857 2022-08-26 02:26:03.621872 adafruit-circuitpython-mcp9600-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:03.617872 adafruit-circuitpython-mcp9600-1.3.5/adafruit_circuitpython_mcp9600.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4857 2022-08-26 02:26:03.000000 adafruit-circuitpython-mcp9600-1.3.5/adafruit_circuitpython_mcp9600.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-08-26 02:26:03.000000 adafruit-circuitpython-mcp9600-1.3.5/adafruit_circuitpython_mcp9600.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:26:03.000000 adafruit-circuitpython-mcp9600-1.3.5/adafruit_circuitpython_mcp9600.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-26 02:26:03.000000 adafruit-circuitpython-mcp9600-1.3.5/adafruit_circuitpython_mcp9600.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-26 02:26:03.000000 adafruit-circuitpython-mcp9600-1.3.5/adafruit_circuitpython_mcp9600.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14516 2022-08-26 02:25:55.000000 adafruit-circuitpython-mcp9600-1.3.5/adafruit_mcp9600.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:03.617872 adafruit-circuitpython-mcp9600-1.3.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:03.621872 adafruit-circuitpython-mcp9600-1.3.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5647 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:03.621872 adafruit-circuitpython-mcp9600-1.3.5/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-08-26 02:25:55.000000 adafruit-circuitpython-mcp9600-1.3.5/examples/mcp9600_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-08-26 02:25:55.000000 adafruit-circuitpython-mcp9600-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-26 02:25:47.000000 adafruit-circuitpython-mcp9600-1.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:26:03.621872 adafruit-circuitpython-mcp9600-1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:18:19.751364 adafruit-circuitpython-mcp9600-1.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:18:19.743364 adafruit-circuitpython-mcp9600-1.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:18:19.747364 adafruit-circuitpython-mcp9600-1.3.6/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:18:19.747364 adafruit-circuitpython-mcp9600-1.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:18:19.747364 adafruit-circuitpython-mcp9600-1.3.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4857 2022-09-22 18:18:19.747364 adafruit-circuitpython-mcp9600-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:18:19.747364 adafruit-circuitpython-mcp9600-1.3.6/adafruit_circuitpython_mcp9600.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4857 2022-09-22 18:18:19.000000 adafruit-circuitpython-mcp9600-1.3.6/adafruit_circuitpython_mcp9600.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2022-09-22 18:18:19.000000 adafruit-circuitpython-mcp9600-1.3.6/adafruit_circuitpython_mcp9600.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 18:18:19.000000 adafruit-circuitpython-mcp9600-1.3.6/adafruit_circuitpython_mcp9600.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-09-22 18:18:19.000000 adafruit-circuitpython-mcp9600-1.3.6/adafruit_circuitpython_mcp9600.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-22 18:18:19.000000 adafruit-circuitpython-mcp9600-1.3.6/adafruit_circuitpython_mcp9600.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    14618 2022-09-22 18:18:09.000000 adafruit-circuitpython-mcp9600-1.3.6/adafruit_mcp9600.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:18:19.747364 adafruit-circuitpython-mcp9600-1.3.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:18:19.747364 adafruit-circuitpython-mcp9600-1.3.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5647 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:18:19.747364 adafruit-circuitpython-mcp9600-1.3.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-22 18:18:09.000000 adafruit-circuitpython-mcp9600-1.3.6/examples/mcp9600_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-09-22 18:18:09.000000 adafruit-circuitpython-mcp9600-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-09-22 18:18:00.000000 adafruit-circuitpython-mcp9600-1.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-22 18:18:19.751364 adafruit-circuitpython-mcp9600-1.3.6/setup.cfg
```

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mcp9600-1.3.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/.github/workflows/build.yml` & `adafruit-circuitpython-mcp9600-1.3.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/.github/workflows/release.yml` & `adafruit-circuitpython-mcp9600-1.3.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/.gitignore` & `adafruit-circuitpython-mcp9600-1.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/.pre-commit-config.yaml` & `adafruit-circuitpython-mcp9600-1.3.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/.pylintrc` & `adafruit-circuitpython-mcp9600-1.3.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mcp9600-1.3.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/LICENSE` & `adafruit-circuitpython-mcp9600-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mcp9600-1.3.6/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/LICENSES/MIT.txt` & `adafruit-circuitpython-mcp9600-1.3.6/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mcp9600-1.3.6/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/PKG-INFO` & `adafruit-circuitpython-mcp9600-1.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp9600
-Version: 1.3.5
+Version: 1.3.6
 Summary: CircuitPython library for the Adafruit MCP9600 breakout
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP9600
 Keywords: adafruit,blinka,circuitpython,micropython,mcp9600,temp,temperature,i2c,thermocouple
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/README.rst` & `adafruit-circuitpython-mcp9600-1.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/adafruit_circuitpython_mcp9600.egg-info/PKG-INFO` & `adafruit-circuitpython-mcp9600-1.3.6/adafruit_circuitpython_mcp9600.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp9600
-Version: 1.3.5
+Version: 1.3.6
 Summary: CircuitPython library for the Adafruit MCP9600 breakout
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP9600
 Keywords: adafruit,blinka,circuitpython,micropython,mcp9600,temp,temperature,i2c,thermocouple
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/adafruit_circuitpython_mcp9600.egg-info/SOURCES.txt` & `adafruit-circuitpython-mcp9600-1.3.6/adafruit_circuitpython_mcp9600.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/adafruit_mcp9600.py` & `adafruit-circuitpython-mcp9600-1.3.6/adafruit_mcp9600.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 try:
     # Used only for typing
     import typing  # pylint: disable=unused-import
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.3.5"
+__version__ = "1.3.6"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP9600.git"
 
 _DEFAULT_ADDRESS = const(0x67)
 
 _REGISTER_HOT_JUNCTION = const(0x00)
 _REGISTER_DELTA_TEMP = const(0x01)
 _REGISTER_COLD_JUNCTION = const(0x02)
@@ -359,15 +359,18 @@
         value = unpack(">xH", data)[0] * 0.0625
         if data[1] & 0x80:
             value -= 4096
         return value
 
     @property
     def delta_temperature(self) -> float:
-        """Delta temperature in Celsius"""
+        """
+        Delta between hot junction (thermocouple probe) and
+        cold junction (ambient/room) temperatures in Celsius
+        """
         data = self._read_register(_REGISTER_DELTA_TEMP, 2)
         value = unpack(">xH", data)[0] * 0.0625
         if data[1] & 0x80:
             value -= 4096
         return value
 
     def _read_register(self, reg: int, count: int = 1) -> bytearray:
```

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/docs/_static/favicon.ico` & `adafruit-circuitpython-mcp9600-1.3.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/docs/conf.py` & `adafruit-circuitpython-mcp9600-1.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/docs/index.rst` & `adafruit-circuitpython-mcp9600-1.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp9600-1.3.5/pyproject.toml` & `adafruit-circuitpython-mcp9600-1.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-mcp9600"
 description = "CircuitPython library for the Adafruit MCP9600 breakout"
-version = "1.3.5"
+version = "1.3.6"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MCP9600"}
 keywords = [
     "adafruit",
```

