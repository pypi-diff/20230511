# Comparing `tmp/xpublish_opendap-0.1.0.tar.gz` & `tmp/xpublish_opendap-0.1.dev36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpublish_opendap-0.1.0.tar", last modified: Thu May 11 20:39:49 2023, max compression
+gzip compressed data, was "xpublish_opendap-0.1.dev36.tar", last modified: Thu May 11 18:24:22 2023, max compression
```

## Comparing `xpublish_opendap-0.1.0.tar` & `xpublish_opendap-0.1.dev36.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:39:49.668071 xpublish_opendap-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:39:49.664071 xpublish_opendap-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:39:49.668071 xpublish_opendap-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-11 20:39:39.000000 xpublish_opendap-0.1.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-11 20:39:39.000000 xpublish_opendap-0.1.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-11 20:39:39.000000 xpublish_opendap-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-11 20:39:39.000000 xpublish_opendap-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-11 20:39:39.000000 xpublish_opendap-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-11 20:39:49.668071 xpublish_opendap-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-11 20:39:39.000000 xpublish_opendap-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-11 20:39:39.000000 xpublish_opendap-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-11 20:39:39.000000 xpublish_opendap-0.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-11 20:39:39.000000 xpublish_opendap-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:39:49.668071 xpublish_opendap-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:39:49.668071 xpublish_opendap-0.1.0/xpublish_opendap/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-11 20:39:39.000000 xpublish_opendap-0.1.0/xpublish_opendap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 20:39:49.000000 xpublish_opendap-0.1.0/xpublish_opendap/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-11 20:39:39.000000 xpublish_opendap-0.1.0/xpublish_opendap/dap_xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-11 20:39:39.000000 xpublish_opendap-0.1.0/xpublish_opendap/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:39:49.668071 xpublish_opendap-0.1.0/xpublish_opendap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-11 20:39:49.000000 xpublish_opendap-0.1.0/xpublish_opendap.egg-info/SOURCES.txt
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 18:24:22.029286 xpublish_opendap-0.1.dev36/
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 18:24:22.020946 xpublish_opendap-0.1.dev36/.github/
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 18:24:22.025732 xpublish_opendap-0.1.dev36/.github/workflows/
+-rw-r--r--   0 akerney    (502) staff       (20)      237 2022-05-14 19:04:37.000000 xpublish_opendap-0.1.dev36/.github/workflows/pre-commit.yml
+-rw-r--r--   0 akerney    (502) staff       (20)     1618 2023-05-11 17:57:29.000000 xpublish_opendap-0.1.dev36/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 akerney    (502) staff       (20)     1175 2023-05-11 17:49:13.000000 xpublish_opendap-0.1.dev36/.github/workflows/tests.yml
+-rw-r--r--   0 akerney    (502) staff       (20)     1214 2023-04-30 14:45:48.000000 xpublish_opendap-0.1.dev36/.pre-commit-config.yaml
+-rw-r--r--   0 akerney    (502) staff       (20)     1472 2022-05-14 18:07:34.000000 xpublish_opendap-0.1.dev36/LICENSE.txt
+-rw-r--r--   0 akerney    (502) staff       (20)      247 2022-05-14 18:09:01.000000 xpublish_opendap-0.1.dev36/MANIFEST.in
+-rw-r--r--   0 akerney    (502) staff       (20)     3847 2023-05-11 18:24:22.028883 xpublish_opendap-0.1.dev36/PKG-INFO
+-rw-r--r--   0 akerney    (502) staff       (20)     1419 2023-05-11 17:49:13.000000 xpublish_opendap-0.1.dev36/README.md
+-rw-r--r--   0 akerney    (502) staff       (20)     1731 2023-05-11 18:23:43.000000 xpublish_opendap-0.1.dev36/pyproject.toml
+-rw-r--r--   0 akerney    (502) staff       (20)      227 2023-05-11 17:49:13.000000 xpublish_opendap-0.1.dev36/requirements-dev.txt
+-rw-r--r--   0 akerney    (502) staff       (20)       46 2023-05-11 17:52:05.000000 xpublish_opendap-0.1.dev36/requirements.txt
+-rw-r--r--   0 akerney    (502) staff       (20)       38 2023-05-11 18:24:22.029443 xpublish_opendap-0.1.dev36/setup.cfg
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 18:24:22.027993 xpublish_opendap-0.1.dev36/xpublish_opendap/
+-rw-r--r--   0 akerney    (502) staff       (20)      236 2023-04-30 14:45:48.000000 xpublish_opendap-0.1.dev36/xpublish_opendap/__init__.py
+-rw-r--r--   0 akerney    (502) staff       (20)      170 2023-05-11 18:24:21.000000 xpublish_opendap-0.1.dev36/xpublish_opendap/_version.py
+-rw-r--r--   0 akerney    (502) staff       (20)     2661 2023-04-30 14:45:48.000000 xpublish_opendap-0.1.dev36/xpublish_opendap/dap_xarray.py
+-rw-r--r--   0 akerney    (502) staff       (20)     2988 2023-04-30 14:45:48.000000 xpublish_opendap-0.1.dev36/xpublish_opendap/plugin.py
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 18:24:22.028412 xpublish_opendap-0.1.dev36/xpublish_opendap.egg-info/
+-rw-r--r--   0 akerney    (502) staff       (20)      325 2023-05-11 18:24:22.000000 xpublish_opendap-0.1.dev36/xpublish_opendap.egg-info/SOURCES.txt
```

### Comparing `xpublish_opendap-0.1.0/.github/workflows/publish-to-pypi.yml` & `xpublish_opendap-0.1.dev36/.github/workflows/publish-to-pypi.yml`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,16 @@
   release:
     types:
       - published
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI and TestPyPI
     runs-on: ubuntu-latest
-    permissions:
-      id-token: write # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
       - uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
 
       # - name: Get tags
@@ -38,22 +34,24 @@
         run: >
           ls dist
           && python -m pip install --upgrade check-manifest
           && check-manifest --verbose
 
       - name: Test wheels
         run: >
-          cd dist
+          cd dist 
           && python -m pip install *.whl
           && python -m pip install --upgrade build twine
           && python -m twine check *
 
-      # Skipping Test PyPI due to issues with setuptools_scm
-      # see https://github.com/xpublish-community/xpublish-opendap/issues/10
-      # - name: Publish distribution 📦 to Test PyPI
-      #   uses: pypa/gh-action-pypi-publish@release/v1
-      #   with:
-      #     repository-url: https://test.pypi.org/legacy/
+          - name: Publish distribution 📦 to Test PyPI
+      uses: pypa/gh-action-pypi-publish@release/v1
+      with:
+        password: ${{ secrets.TEST_PYPI_API_TOKEN }}
+        repository-url: https://test.pypi.org/legacy/
 
       - name: Publish a Python distribution to PyPI
         if: success() && github.event_name == 'release'
         uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          user: __token__
+          password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `xpublish_opendap-0.1.0/.github/workflows/tests.yml` & `xpublish_opendap-0.1.dev36/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `xpublish_opendap-0.1.0/LICENSE.txt` & `xpublish_opendap-0.1.dev36/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xpublish_opendap-0.1.0/PKG-INFO` & `xpublish_opendap-0.1.dev36/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpublish_opendap
-Version: 0.1.0
+Version: 0.1.dev36
 License: Copyright 2017 AUTHOR NAME
         
         
         Redistribution and use in source and binary forms,
         with or without modification,
         are permitted provided that the following conditions are met:
         
@@ -46,34 +46,57 @@
 License-File: LICENSE.txt
 
 ## xpublish_opendap
 
 [![Tests](https://github.com/gulfofmaine/xpublish-opendap/actions/workflows/tests.yml/badge.svg)](https://github.com/gulfofmaine/xpublish-opendap/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/xpublish-community/xpublish-opendap/branch/main/graph/badge.svg?token=0HMS1Q8Z8Y)](https://codecov.io/gh/xpublish-community/xpublish-opendap)
 
-OpenDAP endpoint plugin for Xpublish.
+Quick description
 
-### Installation - Conda not enabled yet
+### Documentation and code
+
+URLs for the docs and code.
+
+### Installation - not really, install from Github instead
 
 For `conda` users you can
 
 ```shell
 conda install --channel conda-forge xpublish_opendap
 ```
 
 or, if you are a `pip` users
 
 ```shell
 pip install xpublish_opendap
 ```
 
-Once it's installed, the plugin will register itself with Xpublish and OpenDAP endpoints will be included for each dataset on the server.
+### Example
+
+```python
+import xarray as xr
+import xpublish
+from xpublish.routers import base_router, zarr_router
+from xpublish_opendap import dap_router
+
+
+ds = xr.open_dataset("dataset.nc")
+
+rest = xpublish.Rest(
+    ds,
+    routers=[
+        (base_router, {"tags": ["info"]}),
+        (dap_router, {"tags": ["opendap"], "prefix": "/dap"}),
+        (zarr_router, {"tags": ["zarr"], "prefix": "/zarr"})
+    ]
+)
+```
 
 ## Get in touch
 
-Report bugs, suggest features or view the source code on [GitHub](https://github.com/xpublish-community/xpublish_opendap/issues).
+Report bugs, suggest features or view the source code on [GitHub](https://github.com/ioos/xpublish_opendap/issues).
 
 ## License and copyright
 
 xpublish_opendap is licensed under BSD 3-Clause "New" or "Revised" License (BSD-3-Clause).
 
-Development occurs on GitHub at <https://github.com/xpublish-community/xpublish_opendap>.
+Development occurs on GitHub at <https://github.com/ioos/xpublish_opendap>.
```

### Comparing `xpublish_opendap-0.1.0/pyproject.toml` & `xpublish_opendap-0.1.dev36/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -24,28 +24,26 @@
 ]
 
 dynamic = ["version", "dependencies"]
 
 [project.urls]
 "Homepage" = "https://github.com/xpublish-community/xpublish-opendap/"
 
-[project.entry-points."xpublish.plugin"]
-opendap = "xpublish_opendap.plugin:OpenDapPlugin"
-
 [tool.setuptools]
 packages = ["xpublish_opendap"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
 
 [tool.setuptools_scm]
 write_to = "xpublish_opendap/_version.py"
+local_scheme = "no-local-version"
 
-[tool.check-manifest]
-ignore = ["xpublish_opendap/_version.py"]
+[project.entry-points."xpublish.plugin"]
+opendap = "xpublish_opendap.plugin:OpenDapPlugin"
 
 [tool.ruff]
 select = [
     "A",   # flake8-builtins
     "B",   # flake8-bugbear
     "C4",  # flake8-comprehensions
     "D",   # pydocstyle
```

### Comparing `xpublish_opendap-0.1.0/xpublish_opendap/dap_xarray.py` & `xpublish_opendap-0.1.dev36/xpublish_opendap/dap_xarray.py`

 * *Files identical despite different names*

### Comparing `xpublish_opendap-0.1.0/xpublish_opendap/plugin.py` & `xpublish_opendap-0.1.dev36/xpublish_opendap/plugin.py`

 * *Files identical despite different names*

