# Comparing `tmp/adafruit-circuitpython-ov5640-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-ov5640-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ov5640-1.1.8.tar", last modified: Mon Aug 22 18:45:14 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ov5640-1.1.9.tar", last modified: Fri Aug 26 02:27:09 2022, max compression
```

## Comparing `adafruit-circuitpython-ov5640-1.1.8.tar` & `adafruit-circuitpython-ov5640-1.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:14.852230 adafruit-circuitpython-ov5640-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:14.848230 adafruit-circuitpython-ov5640-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:14.848230 adafruit-circuitpython-ov5640-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:14.848230 adafruit-circuitpython-ov5640-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:14.848230 adafruit-circuitpython-ov5640-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-08-22 18:45:14.852230 adafruit-circuitpython-ov5640-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:14.848230 adafruit-circuitpython-ov5640-1.1.8/adafruit_circuitpython_ov5640.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-08-22 18:45:14.000000 adafruit-circuitpython-ov5640-1.1.8/adafruit_circuitpython_ov5640.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-22 18:45:14.000000 adafruit-circuitpython-ov5640-1.1.8/adafruit_circuitpython_ov5640.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:45:14.000000 adafruit-circuitpython-ov5640-1.1.8/adafruit_circuitpython_ov5640.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 18:45:14.000000 adafruit-circuitpython-ov5640-1.1.8/adafruit_circuitpython_ov5640.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-22 18:45:14.000000 adafruit-circuitpython-ov5640-1.1.8/adafruit_circuitpython_ov5640.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    41909 2022-08-22 18:45:07.000000 adafruit-circuitpython-ov5640-1.1.8/adafruit_ov5640.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:14.852230 adafruit-circuitpython-ov5640-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:14.852230 adafruit-circuitpython-ov5640-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5861 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:45:14.852230 adafruit-circuitpython-ov5640-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     6247 2022-08-22 18:45:07.000000 adafruit-circuitpython-ov5640-1.1.8/examples/ov5640_directio_kaluga1_3_ili9341.py
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-08-22 18:45:07.000000 adafruit-circuitpython-ov5640-1.1.8/examples/ov5640_jpeg_kaluga1_3.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-08-22 18:45:07.000000 adafruit-circuitpython-ov5640-1.1.8/examples/ov5640_jpeg_kaluga1_3_boot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-08-22 18:45:07.000000 adafruit-circuitpython-ov5640-1.1.8/examples/ov5640_sdcard_kaluga_1_3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-08-22 18:45:07.000000 adafruit-circuitpython-ov5640-1.1.8/examples/ov5640_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     7490 2022-08-22 18:45:07.000000 adafruit-circuitpython-ov5640-1.1.8/examples/ov5640_stopmotion_kaluga1_3.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-08-22 18:45:07.000000 adafruit-circuitpython-ov5640-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-22 18:45:00.000000 adafruit-circuitpython-ov5640-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:45:14.852230 adafruit-circuitpython-ov5640-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.312962 adafruit-circuitpython-ov5640-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.304962 adafruit-circuitpython-ov5640-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.308962 adafruit-circuitpython-ov5640-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.308962 adafruit-circuitpython-ov5640-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.308962 adafruit-circuitpython-ov5640-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-08-26 02:27:09.312962 adafruit-circuitpython-ov5640-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.308962 adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-08-26 02:27:09.000000 adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-26 02:27:09.000000 adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:27:09.000000 adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 02:27:09.000000 adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-26 02:27:09.000000 adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    41909 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/adafruit_ov5640.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.308962 adafruit-circuitpython-ov5640-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.308962 adafruit-circuitpython-ov5640-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     6081 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.312962 adafruit-circuitpython-ov5640-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     6247 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_directio_kaluga1_3_ili9341.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_jpeg_kaluga1_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_jpeg_kaluga1_3_boot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_sdcard_kaluga_1_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7490 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_stopmotion_kaluga1_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:27:09.312962 adafruit-circuitpython-ov5640-1.1.9/setup.cfg
```

### Comparing `adafruit-circuitpython-ov5640-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ov5640-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-ov5640-1.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-ov5640-1.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/.gitignore` & `adafruit-circuitpython-ov5640-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ov5640-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/.pylintrc` & `adafruit-circuitpython-ov5640-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ov5640-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/LICENSE` & `adafruit-circuitpython-ov5640-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ov5640-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ov5640-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ov5640-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/PKG-INFO` & `adafruit-circuitpython-ov5640-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ov5640
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython driver for OV5640 Camera
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_OV5640
 Keywords: adafruit,ov5640,camera,breakout,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ov5640-1.1.8/README.rst` & `adafruit-circuitpython-ov5640-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/adafruit_circuitpython_ov5640.egg-info/PKG-INFO` & `adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ov5640
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython driver for OV5640 Camera
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_OV5640
 Keywords: adafruit,ov5640,camera,breakout,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ov5640-1.1.8/adafruit_circuitpython_ov5640.egg-info/SOURCES.txt` & `adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/adafruit_ov5640.py` & `adafruit-circuitpython-ov5640-1.1.9/adafruit_ov5640.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     from typing import Optional, Sequence, List, Union
     from busio import I2C
     from microcontroller import Pin
     from digitalio import DigitalInOut
 except ImportError:
     pass
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ov5640.git"
 
 from micropython import const
 
 OV5640_COLOR_RGB = 0
 OV5640_COLOR_YUV = 1
 OV5640_COLOR_GRAYSCALE = 2
```

### Comparing `adafruit-circuitpython-ov5640-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ov5640-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/docs/conf.py` & `adafruit-circuitpython-ov5640-1.1.9/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -53,15 +54,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit CircuitPython ov5640 Library"
-copyright = "2021 Jeff Epler"
+creation_year = "2021"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Jeff Epler"
 author = "Jeff Epler"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-ov5640-1.1.8/docs/examples.rst` & `adafruit-circuitpython-ov5640-1.1.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/docs/index.rst` & `adafruit-circuitpython-ov5640-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/examples/ov5640_directio_kaluga1_3_ili9341.py` & `adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_directio_kaluga1_3_ili9341.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/examples/ov5640_jpeg_kaluga1_3.py` & `adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_jpeg_kaluga1_3.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/examples/ov5640_jpeg_kaluga1_3_boot.py` & `adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_jpeg_kaluga1_3_boot.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/examples/ov5640_sdcard_kaluga_1_3.py` & `adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_sdcard_kaluga_1_3.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/examples/ov5640_simpletest.py` & `adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/examples/ov5640_stopmotion_kaluga1_3.py` & `adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_stopmotion_kaluga1_3.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.8/pyproject.toml` & `adafruit-circuitpython-ov5640-1.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ov5640"
 description = "CircuitPython driver for OV5640 Camera"
-version = "1.1.8"
+version = "1.1.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_OV5640"}
 keywords = [
     "adafruit",
```

