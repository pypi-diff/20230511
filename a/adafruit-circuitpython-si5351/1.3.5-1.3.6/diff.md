# Comparing `tmp/adafruit-circuitpython-si5351-1.3.5.tar.gz` & `tmp/adafruit-circuitpython-si5351-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-si5351-1.3.5.tar", last modified: Fri Aug 26 02:30:00 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-si5351-1.3.6.tar", last modified: Thu Oct  6 18:08:38 2022, max compression
```

## Comparing `adafruit-circuitpython-si5351-1.3.5.tar` & `adafruit-circuitpython-si5351-1.3.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:00.993688 adafruit-circuitpython-si5351-1.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:00.981688 adafruit-circuitpython-si5351-1.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:00.985688 adafruit-circuitpython-si5351-1.3.5/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:00.985688 adafruit-circuitpython-si5351-1.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:00.989688 adafruit-circuitpython-si5351-1.3.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3328 2022-08-26 02:30:00.993688 adafruit-circuitpython-si5351-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:00.989688 adafruit-circuitpython-si5351-1.3.5/adafruit_circuitpython_si5351.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3328 2022-08-26 02:30:00.000000 adafruit-circuitpython-si5351-1.3.5/adafruit_circuitpython_si5351.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-08-26 02:30:00.000000 adafruit-circuitpython-si5351-1.3.5/adafruit_circuitpython_si5351.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:30:00.000000 adafruit-circuitpython-si5351-1.3.5/adafruit_circuitpython_si5351.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 02:30:00.000000 adafruit-circuitpython-si5351-1.3.5/adafruit_circuitpython_si5351.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-26 02:30:00.000000 adafruit-circuitpython-si5351-1.3.5/adafruit_circuitpython_si5351.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    21016 2022-08-26 02:29:53.000000 adafruit-circuitpython-si5351-1.3.5/adafruit_si5351.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:00.993688 adafruit-circuitpython-si5351-1.3.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:00.993688 adafruit-circuitpython-si5351-1.3.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5490 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:00.993688 adafruit-circuitpython-si5351-1.3.5/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2022-08-26 02:29:53.000000 adafruit-circuitpython-si5351-1.3.5/examples/si5351_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-08-26 02:29:53.000000 adafruit-circuitpython-si5351-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-26 02:29:46.000000 adafruit-circuitpython-si5351-1.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:30:00.993688 adafruit-circuitpython-si5351-1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:08:38.461094 adafruit-circuitpython-si5351-1.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:08:38.461094 adafruit-circuitpython-si5351-1.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:08:38.461094 adafruit-circuitpython-si5351-1.3.6/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:08:38.461094 adafruit-circuitpython-si5351-1.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:08:38.461094 adafruit-circuitpython-si5351-1.3.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3328 2022-10-06 18:08:38.461094 adafruit-circuitpython-si5351-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:08:38.461094 adafruit-circuitpython-si5351-1.3.6/adafruit_circuitpython_si5351.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3328 2022-10-06 18:08:38.000000 adafruit-circuitpython-si5351-1.3.6/adafruit_circuitpython_si5351.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      919 2022-10-06 18:08:38.000000 adafruit-circuitpython-si5351-1.3.6/adafruit_circuitpython_si5351.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 18:08:38.000000 adafruit-circuitpython-si5351-1.3.6/adafruit_circuitpython_si5351.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-06 18:08:38.000000 adafruit-circuitpython-si5351-1.3.6/adafruit_circuitpython_si5351.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-06 18:08:38.000000 adafruit-circuitpython-si5351-1.3.6/adafruit_circuitpython_si5351.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    21651 2022-10-06 18:08:30.000000 adafruit-circuitpython-si5351-1.3.6/adafruit_si5351.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:08:38.461094 adafruit-circuitpython-si5351-1.3.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:08:38.461094 adafruit-circuitpython-si5351-1.3.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5490 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:08:38.461094 adafruit-circuitpython-si5351-1.3.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     3641 2022-10-06 18:08:30.000000 adafruit-circuitpython-si5351-1.3.6/examples/si5351_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-10-06 18:08:30.000000 adafruit-circuitpython-si5351-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-10-06 18:08:23.000000 adafruit-circuitpython-si5351-1.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-06 18:08:38.461094 adafruit-circuitpython-si5351-1.3.6/setup.cfg
```

### Comparing `adafruit-circuitpython-si5351-1.3.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-si5351-1.3.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/.github/workflows/build.yml` & `adafruit-circuitpython-si5351-1.3.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/.github/workflows/release.yml` & `adafruit-circuitpython-si5351-1.3.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/.gitignore` & `adafruit-circuitpython-si5351-1.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/.pre-commit-config.yaml` & `adafruit-circuitpython-si5351-1.3.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/.pylintrc` & `adafruit-circuitpython-si5351-1.3.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-si5351-1.3.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/LICENSE` & `adafruit-circuitpython-si5351-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-si5351-1.3.6/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/LICENSES/MIT.txt` & `adafruit-circuitpython-si5351-1.3.6/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/LICENSES/Unlicense.txt` & `adafruit-circuitpython-si5351-1.3.6/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/PKG-INFO` & `adafruit-circuitpython-si5351-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-si5351
-Version: 1.3.5
+Version: 1.3.6
 Summary: CircuitPython library for SI5351 clock generator module.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SI5351
 Keywords: adafruit,si5351,clock,generator,module,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-si5351-1.3.5/README.rst` & `adafruit-circuitpython-si5351-1.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/adafruit_circuitpython_si5351.egg-info/PKG-INFO` & `adafruit-circuitpython-si5351-1.3.6/adafruit_circuitpython_si5351.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-si5351
-Version: 1.3.5
+Version: 1.3.6
 Summary: CircuitPython library for SI5351 clock generator module.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SI5351
 Keywords: adafruit,si5351,clock,generator,module,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-si5351-1.3.5/adafruit_circuitpython_si5351.egg-info/SOURCES.txt` & `adafruit-circuitpython-si5351-1.3.6/adafruit_circuitpython_si5351.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/adafruit_si5351.py` & `adafruit-circuitpython-si5351-1.3.6/adafruit_si5351.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,21 @@
 """
 import math
 
 from micropython import const
 
 from adafruit_bus_device import i2c_device
 
+try:
+    import typing  # pylint: disable=unused-import
+    from busio import I2C
+except ImportError:
+    pass
 
-__version__ = "1.3.5"
+__version__ = "1.3.6"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SI5351.git"
 
 
 # Internal constants:
 _SI5351_ADDRESS = const(0x60)  # Assumes ADDR pin = low
 _SI5351_READBIT = const(0x01)
 _SI5351_CRYSTAL_FREQUENCY = 25000000.0  # Fixed 25mhz crystal on board.
@@ -137,26 +142,28 @@
      - address: The I2C address of the device if it differs from the default.
     """
 
     # Internal class to represent a PLL on the SI5351.  There are two instances
     # of this, PLL A and PLL B.  Each can be the source for a clock output
     # (with further division performed per clock output).
     class _PLL:
-        def __init__(self, si5351, base_address, clock_control_enabled):
+        def __init__(
+            self, si5351: "SI5351", base_address: int, clock_control_enabled: bool
+        ) -> None:
             self._si5351 = si5351
             self._base = base_address
             self._frequency = None
             self.clock_control_enabled = clock_control_enabled
 
         @property
-        def frequency(self):
+        def frequency(self) -> int:
             """Get the frequency of the PLL in hertz."""
             return self._frequency
 
-        def _configure_registers(self, p1, p2, p3):
+        def _configure_registers(self, p1: int, p2: int, p3: int) -> None:
             # Update PLL registers.
             # The datasheet is a nightmare of typos and inconsistencies here!
             self._si5351._write_u8(self._base, (p3 & 0x0000FF00) >> 8)
             self._si5351._write_u8(self._base + 1, (p3 & 0x000000FF))
             self._si5351._write_u8(self._base + 2, (p1 & 0x00030000) >> 16)
             self._si5351._write_u8(self._base + 3, (p1 & 0x0000FF00) >> 8)
             self._si5351._write_u8(self._base + 4, (p1 & 0x000000FF))
@@ -164,15 +171,15 @@
                 self._base + 5, ((p3 & 0x000F0000) >> 12) | ((p2 & 0x000F0000) >> 16)
             )
             self._si5351._write_u8(self._base + 6, (p2 & 0x0000FF00) >> 8)
             self._si5351._write_u8(self._base + 7, (p2 & 0x000000FF))
             # Reset both PLLs.
             self._si5351._write_u8(_SI5351_REGISTER_177_PLL_RESET, (1 << 7) | (1 << 5))
 
-        def configure_integer(self, multiplier):
+        def configure_integer(self, multiplier: int) -> None:
             """Configure the PLL with a simple integer multiplier for the most
             accurate (but more limited) PLL frequency generation.
             """
             if multiplier >= 91 or multiplier <= 14:
                 raise Exception("Multiplier must be in range 14 to 91.")
             multiplier = int(multiplier)
             # Compute register values and configure them.
@@ -184,16 +191,18 @@
             fvco = _SI5351_CRYSTAL_FREQUENCY * multiplier
             # This should actually take the floor to get the true value but
             # there's a limit on how big a value the floor can be and it's
             # easy to hit with high megahertz frequencies:
             #   https://github.com/adafruit/circuitpython/issues/572
             self._frequency = fvco
 
-        def configure_fractional(self, multiplier, numerator, denominator):
-            """Configure the PLL with a fractional multipler specified by
+        def configure_fractional(
+            self, multiplier: int, numerator: int, denominator: int
+        ) -> None:
+            """Configure the PLL with a fractional multiplier specified by
             multiplier and numerator/denominator.  This is less accurate and
             susceptible to jitter but allows a larger range of PLL frequencies.
             """
             if multiplier >= 91 or multiplier <= 14:
                 raise Exception("Multiplier must be in range 14 to 91.")
             if denominator > 0xFFFFF or denominator <= 0:  # Prevent divide by zero.
                 raise Exception(
@@ -222,24 +231,30 @@
             #   https://github.com/adafruit/circuitpython/issues/572
             self._frequency = fvco
 
     # Another internal class to represent each clock output.  There are 3 of
     # these and they can each be independently configured to use a specific
     # PLL source and have their own divider on that PLL.
     class _Clock:
-        def __init__(self, si5351, base_address, control_register, r_register):
+        def __init__(
+            self,
+            si5351: "SI5351",
+            base_address: int,
+            control_register: int,
+            r_register: int,
+        ) -> None:
             self._si5351 = si5351
             self._base = base_address
             self._control = control_register
             self._r = r_register
             self._pll = None
             self._divider = None
 
         @property
-        def frequency(self):
+        def frequency(self) -> float:
             """Get the frequency of this clock output in hertz.  This is
             computed based on the configured PLL, clock divider, and R divider.
             """
             # Make sure a PLL and divider are present, i.e. this clock has
             # been configured, otherwise return nothing.
             if self._pll is None or self._divider is None:
                 return None
@@ -265,53 +280,55 @@
                 return base_frequency / 64
             elif r_divider == R_DIV_128:
                 return base_frequency / 128
             else:
                 raise RuntimeError("Unexpected R divider!")
 
         @property
-        def r_divider(self):
+        def r_divider(self) -> int:
             """Get and set the R divider value, must be one of:
             - R_DIV_1: divider of 1
             - R_DIV_2: divider of 2
             - R_DIV_4: divider of 4
             - R_DIV_8: divider of 8
             - R_DIV_16: divider of 16
             - R_DIV_32: divider of 32
             - R_DIV_64: divider of 64
             - R_DIV_128: divider of 128
             """
             reg_value = self._si5351._read_u8(self._r)
             return (reg_value >> 4) & 0x07
 
         @r_divider.setter
-        def r_divider(self, divider):
+        def r_divider(self, divider: int) -> None:
             if divider > 7 or divider < 0:
                 raise Exception("Divider must in range 0 to 7.")
             reg_value = self._si5351._read_u8(self._r)
             reg_value &= 0x0F
             divider &= 0x07
             divider <<= 4
             reg_value |= divider
             self._si5351._write_u8(self._r, reg_value)
 
-        def _configure_registers(self, p1, p2, p3):
+        def _configure_registers(self, p1: int, p2: int, p3: int) -> None:
             # Update MSx registers.
             self._si5351._write_u8(self._base, (p3 & 0x0000FF00) >> 8)
             self._si5351._write_u8(self._base + 1, (p3 & 0x000000FF))
             self._si5351._write_u8(self._base + 2, (p1 & 0x00030000) >> 16)
             self._si5351._write_u8(self._base + 3, (p1 & 0x0000FF00) >> 8)
             self._si5351._write_u8(self._base + 4, (p1 & 0x000000FF))
             self._si5351._write_u8(
                 self._base + 5, ((p3 & 0x000F0000) >> 12) | ((p2 & 0x000F0000) >> 16)
             )
             self._si5351._write_u8(self._base + 6, (p2 & 0x0000FF00) >> 8)
             self._si5351._write_u8(self._base + 7, (p2 & 0x000000FF))
 
-        def configure_integer(self, pll, divider, inverted=False):
+        def configure_integer(
+            self, pll: "PLL", divider: int, inverted: bool = False
+        ) -> None:
             """Configure the clock output with the specified PLL source
             (should be a PLL instance on the SI5351 class) and specific integer
             divider.  This is the most accurate way to set the clock output
             frequency but supports less of a range of values.
             """
             if divider >= 2049 or divider <= 3:
                 raise Exception("Divider must be in range 3 to 2049.")
@@ -335,18 +352,23 @@
                 control &= 0b11101111  # Make sure to turn it off if not inverted
             self._si5351._write_u8(self._control, control)
             # Store the PLL and divisor value so frequency can be calculated.
             self._pll = pll
             self._divider = divider
 
         def configure_fractional(
-            self, pll, divider, numerator, denominator, inverted=False
-        ):
+            self,
+            pll: "PLL",
+            divider: int,
+            numerator: int,
+            denominator: int,
+            inverted: bool = False,
+        ) -> None:
             """Configure the clock output with the specified PLL source
-            (should be a PLL instance on the SI5351 class) and specifiec
+            (should be a PLL instance on the SI5351 class) and specific
             fractional divider with numerator/denominator.  Again this is less
             accurate but has a wider range of output frequencies.
             """
             # pylint: disable=too-many-arguments
             if divider >= 2049 or divider <= 3:
                 raise Exception("Divider must be in range 3 to 2049.")
             if denominator > 0xFFFFF or denominator <= 0:  # Prevent divide by zero.
@@ -382,15 +404,15 @@
             self._pll = pll
             self._divider = divider + (numerator / denominator)
 
     # Class-level buffer to reduce allocations and heap fragmentation.
     # This is not thread-safe or re-entrant by design!
     _BUFFER = bytearray(2)
 
-    def __init__(self, i2c, *, address=_SI5351_ADDRESS):
+    def __init__(self, i2c: I2C, *, address: int = _SI5351_ADDRESS) -> None:
         self._device = i2c_device.I2CDevice(i2c, address)
         # Setup the SI5351.
         # Disable all outputs setting CLKx_DIS high.
         self._write_u8(_SI5351_REGISTER_3_OUTPUT_ENABLE_CONTROL, 0xFF)
         # Power down all output drivers
         self._write_u8(_SI5351_REGISTER_16_CLK0_CONTROL, 0x80)
         self._write_u8(_SI5351_REGISTER_17_CLK1_CONTROL, 0x80)
@@ -419,46 +441,46 @@
         self.clock_2 = self._Clock(
             self,
             _SI5351_REGISTER_58_MULTISYNTH2_PARAMETERS_1,
             _SI5351_REGISTER_18_CLK2_CONTROL,
             _SI5351_REGISTER_60_MULTISYNTH2_PARAMETERS_3,
         )
 
-    def _read_u8(self, address):
+    def _read_u8(self, address: int) -> int:
         # Read an 8-bit unsigned value from the specified 8-bit address.
         with self._device as i2c:
             self._BUFFER[0] = address & 0xFF
             i2c.write(self._BUFFER, end=1)
             i2c.readinto(self._BUFFER, end=1)
         return self._BUFFER[0]
 
-    def _write_u8(self, address, val):
+    def _write_u8(self, address: int, val: int) -> None:
         # Write an 8-bit unsigned value to the specified 8-bit address.
         with self._device as i2c:
             self._BUFFER[0] = address & 0xFF
             self._BUFFER[1] = val & 0xFF
             i2c.write(self._BUFFER, end=2)
 
     @property
-    def outputs_enabled(self):
+    def outputs_enabled(self) -> bool:
         """Get and set the enabled state of all clock outputs as a boolean.
         If true then all clock outputs are enabled, and if false then they are
         all disabled.
         """
         return self._read_u8(_SI5351_REGISTER_3_OUTPUT_ENABLE_CONTROL) == 0xFF
 
     @outputs_enabled.setter
-    def outputs_enabled(self, val):
+    def outputs_enabled(self, val: bool) -> None:
         if not val:
             self._write_u8(_SI5351_REGISTER_3_OUTPUT_ENABLE_CONTROL, 0xFF)
         else:
             self._write_u8(_SI5351_REGISTER_3_OUTPUT_ENABLE_CONTROL, 0x00)
         self.reset_plls()
 
-    def reset_plls(self):
+    def reset_plls(self) -> None:
         """Reset both PLLs. This is required when the phase between clocks
         needs to be non-random.
 
         See e.g.
 
             https://groups.io/g/BITX20/topic/si5351a_facts_and_myths/5430607
         """
```

### Comparing `adafruit-circuitpython-si5351-1.3.5/docs/_static/favicon.ico` & `adafruit-circuitpython-si5351-1.3.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/docs/conf.py` & `adafruit-circuitpython-si5351-1.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/docs/index.rst` & `adafruit-circuitpython-si5351-1.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/examples/si5351_simpletest.py` & `adafruit-circuitpython-si5351-1.3.6/examples/si5351_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.3.5/pyproject.toml` & `adafruit-circuitpython-si5351-1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-si5351"
 description = "CircuitPython library for SI5351 clock generator module."
-version = "1.3.5"
+version = "1.3.6"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SI5351"}
 keywords = [
     "adafruit",
```

