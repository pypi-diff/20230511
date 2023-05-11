# Comparing `tmp/adafruit-circuitpython-bitbangio-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-bitbangio-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bitbangio-1.3.8.tar", last modified: Fri Aug 26 02:32:53 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-bitbangio-1.3.9.tar", last modified: Wed Sep 21 05:11:30 2022, max compression
```

## Comparing `adafruit-circuitpython-bitbangio-1.3.8.tar` & `adafruit-circuitpython-bitbangio-1.3.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:53.005966 adafruit-circuitpython-bitbangio-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:52.997965 adafruit-circuitpython-bitbangio-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:53.001966 adafruit-circuitpython-bitbangio-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:53.001966 adafruit-circuitpython-bitbangio-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:53.001966 adafruit-circuitpython-bitbangio-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4303 2022-08-26 02:32:53.005966 adafruit-circuitpython-bitbangio-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    18000 2022-08-26 02:32:44.000000 adafruit-circuitpython-bitbangio-1.3.8/adafruit_bitbangio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:53.001966 adafruit-circuitpython-bitbangio-1.3.8/adafruit_circuitpython_bitbangio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4303 2022-08-26 02:32:52.000000 adafruit-circuitpython-bitbangio-1.3.8/adafruit_circuitpython_bitbangio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-08-26 02:32:52.000000 adafruit-circuitpython-bitbangio-1.3.8/adafruit_circuitpython_bitbangio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:32:52.000000 adafruit-circuitpython-bitbangio-1.3.8/adafruit_circuitpython_bitbangio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-26 02:32:52.000000 adafruit-circuitpython-bitbangio-1.3.8/adafruit_circuitpython_bitbangio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-26 02:32:52.000000 adafruit-circuitpython-bitbangio-1.3.8/adafruit_circuitpython_bitbangio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:53.005966 adafruit-circuitpython-bitbangio-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:53.005966 adafruit-circuitpython-bitbangio-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5659 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:53.005966 adafruit-circuitpython-bitbangio-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-08-26 02:32:44.000000 adafruit-circuitpython-bitbangio-1.3.8/examples/bitbangio_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-08-26 02:32:44.000000 adafruit-circuitpython-bitbangio-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-08-26 02:32:36.000000 adafruit-circuitpython-bitbangio-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:32:53.005966 adafruit-circuitpython-bitbangio-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 05:11:30.949441 adafruit-circuitpython-bitbangio-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 05:11:30.941440 adafruit-circuitpython-bitbangio-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 05:11:30.945440 adafruit-circuitpython-bitbangio-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 05:11:30.945440 adafruit-circuitpython-bitbangio-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 05:11:30.945440 adafruit-circuitpython-bitbangio-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4303 2022-09-21 05:11:30.949441 adafruit-circuitpython-bitbangio-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3490 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)    18178 2022-09-21 05:11:21.000000 adafruit-circuitpython-bitbangio-1.3.9/adafruit_bitbangio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 05:11:30.945440 adafruit-circuitpython-bitbangio-1.3.9/adafruit_circuitpython_bitbangio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4303 2022-09-21 05:11:30.000000 adafruit-circuitpython-bitbangio-1.3.9/adafruit_circuitpython_bitbangio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      940 2022-09-21 05:11:30.000000 adafruit-circuitpython-bitbangio-1.3.9/adafruit_circuitpython_bitbangio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 05:11:30.000000 adafruit-circuitpython-bitbangio-1.3.9/adafruit_circuitpython_bitbangio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-09-21 05:11:30.000000 adafruit-circuitpython-bitbangio-1.3.9/adafruit_circuitpython_bitbangio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-21 05:11:30.000000 adafruit-circuitpython-bitbangio-1.3.9/adafruit_circuitpython_bitbangio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 05:11:30.945440 adafruit-circuitpython-bitbangio-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 05:11:30.949441 adafruit-circuitpython-bitbangio-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5659 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      891 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 05:11:30.949441 adafruit-circuitpython-bitbangio-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      733 2022-09-21 05:11:21.000000 adafruit-circuitpython-bitbangio-1.3.9/examples/bitbangio_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-09-21 05:11:21.000000 adafruit-circuitpython-bitbangio-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-21 05:11:08.000000 adafruit-circuitpython-bitbangio-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 05:11:30.949441 adafruit-circuitpython-bitbangio-1.3.9/setup.cfg
```

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bitbangio-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-bitbangio-1.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-bitbangio-1.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/.gitignore` & `adafruit-circuitpython-bitbangio-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-bitbangio-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/.pylintrc` & `adafruit-circuitpython-bitbangio-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bitbangio-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/LICENSE` & `adafruit-circuitpython-bitbangio-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bitbangio-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-bitbangio-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bitbangio-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/PKG-INFO` & `adafruit-circuitpython-bitbangio-1.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bitbangio
-Version: 1.3.8
+Version: 1.3.9
 Summary: A library for adding bitbang I2C and SPI to CircuitPython without the built-in bitbangio module
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BitbangIO
 Keywords: adafruit,blinka,circuitpython,micropython,bitbangio,bitbang,spi,i2c,software
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/README.rst` & `adafruit-circuitpython-bitbangio-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/adafruit_bitbangio.py` & `adafruit-circuitpython-bitbangio-1.3.9/adafruit_bitbangio.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,27 @@
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 try:
-    from typing import Optional, List
+    from typing import List, Optional, Type
     from typing_extensions import Literal
+    from types import TracebackType
     from circuitpython_typing import WriteableBuffer, ReadableBuffer
     from microcontroller import Pin
 except ImportError:
     pass
 
 # imports
 from time import monotonic
 from digitalio import DigitalInOut
 
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BitbangIO.git"
 
 MSBFIRST = 0
 LSBFIRST = 1
 
 
 class _BitBangIO:
@@ -63,18 +64,23 @@
             raise ValueError("Not locked")
 
     def _check_lock(self) -> Literal[True]:
         if not self._locked:
             raise RuntimeError("First call try_lock()")
         return True
 
-    def __enter__(self):
+    def __enter__(self) -> "_BitBangIO":
         return self
 
-    def __exit__(self, exc_type, exc_value, traceback) -> None:
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_value: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> None:
         self.deinit()
 
     # pylint: disable=no-self-use
     def deinit(self) -> None:
         """Free any hardware used by the object."""
         return
```

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/adafruit_circuitpython_bitbangio.egg-info/PKG-INFO` & `adafruit-circuitpython-bitbangio-1.3.9/adafruit_circuitpython_bitbangio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bitbangio
-Version: 1.3.8
+Version: 1.3.9
 Summary: A library for adding bitbang I2C and SPI to CircuitPython without the built-in bitbangio module
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BitbangIO
 Keywords: adafruit,blinka,circuitpython,micropython,bitbangio,bitbang,spi,i2c,software
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/adafruit_circuitpython_bitbangio.egg-info/SOURCES.txt` & `adafruit-circuitpython-bitbangio-1.3.9/adafruit_circuitpython_bitbangio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-bitbangio-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/docs/conf.py` & `adafruit-circuitpython-bitbangio-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/docs/index.rst` & `adafruit-circuitpython-bitbangio-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/examples/bitbangio_simpletest.py` & `adafruit-circuitpython-bitbangio-1.3.9/examples/bitbangio_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitbangio-1.3.8/pyproject.toml` & `adafruit-circuitpython-bitbangio-1.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bitbangio"
 description = "A library for adding bitbang I2C and SPI to CircuitPython without the built-in bitbangio module"
-version = "1.3.8"
+version = "1.3.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BitbangIO"}
 keywords = [
     "adafruit",
```

