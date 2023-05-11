# Comparing `tmp/adafruit-circuitpython-as7341-1.2.8.tar.gz` & `tmp/adafruit-circuitpython-as7341-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-as7341-1.2.8.tar", last modified: Thu Jun  9 18:29:08 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-as7341-1.2.9.tar", last modified: Tue Aug  9 19:44:19 2022, max compression
```

## Comparing `adafruit-circuitpython-as7341-1.2.8.tar` & `adafruit-circuitpython-as7341-1.2.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:08.266030 adafruit-circuitpython-as7341-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:08.262030 adafruit-circuitpython-as7341-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:08.262030 adafruit-circuitpython-as7341-1.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:08.262030 adafruit-circuitpython-as7341-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:08.262030 adafruit-circuitpython-as7341-1.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4638 2022-06-09 18:29:08.266030 adafruit-circuitpython-as7341-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3849 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    28371 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/adafruit_as7341.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:08.262030 adafruit-circuitpython-as7341-1.2.8/adafruit_circuitpython_as7341.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4638 2022-06-09 18:29:08.000000 adafruit-circuitpython-as7341-1.2.8/adafruit_circuitpython_as7341.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-06-09 18:29:08.000000 adafruit-circuitpython-as7341-1.2.8/adafruit_circuitpython_as7341.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:29:08.000000 adafruit-circuitpython-as7341-1.2.8/adafruit_circuitpython_as7341.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-06-09 18:29:08.000000 adafruit-circuitpython-as7341-1.2.8/adafruit_circuitpython_as7341.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-09 18:29:08.000000 adafruit-circuitpython-as7341-1.2.8/adafruit_circuitpython_as7341.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:08.262030 adafruit-circuitpython-as7341-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:08.262030 adafruit-circuitpython-as7341-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5662 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:08.266030 adafruit-circuitpython-as7341-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/examples/as7341_batched_readings.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/examples/as7341_flicker_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/examples/as7341_led_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/examples/as7341_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:29:08.266030 adafruit-circuitpython-as7341-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-06-09 18:28:56.000000 adafruit-circuitpython-as7341-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:44:19.623590 adafruit-circuitpython-as7341-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:44:19.619589 adafruit-circuitpython-as7341-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:44:19.619589 adafruit-circuitpython-as7341-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:44:19.619589 adafruit-circuitpython-as7341-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:44:19.619589 adafruit-circuitpython-as7341-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4644 2022-08-09 19:44:19.623590 adafruit-circuitpython-as7341-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3851 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)    28364 2022-08-09 19:44:11.000000 adafruit-circuitpython-as7341-1.2.9/adafruit_as7341.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:44:19.623590 adafruit-circuitpython-as7341-1.2.9/adafruit_circuitpython_as7341.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4644 2022-08-09 19:44:19.000000 adafruit-circuitpython-as7341-1.2.9/adafruit_circuitpython_as7341.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-08-09 19:44:19.000000 adafruit-circuitpython-as7341-1.2.9/adafruit_circuitpython_as7341.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:44:19.000000 adafruit-circuitpython-as7341-1.2.9/adafruit_circuitpython_as7341.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-08-09 19:44:19.000000 adafruit-circuitpython-as7341-1.2.9/adafruit_circuitpython_as7341.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-09 19:44:19.000000 adafruit-circuitpython-as7341-1.2.9/adafruit_circuitpython_as7341.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:44:19.623590 adafruit-circuitpython-as7341-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:44:19.623590 adafruit-circuitpython-as7341-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5662 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:44:19.623590 adafruit-circuitpython-as7341-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-08-09 19:44:11.000000 adafruit-circuitpython-as7341-1.2.9/examples/as7341_batched_readings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-08-09 19:44:11.000000 adafruit-circuitpython-as7341-1.2.9/examples/as7341_flicker_detection.py
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-08-09 19:44:11.000000 adafruit-circuitpython-as7341-1.2.9/examples/as7341_led_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-08-09 19:44:11.000000 adafruit-circuitpython-as7341-1.2.9/examples/as7341_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-08-09 19:44:11.000000 adafruit-circuitpython-as7341-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2022-08-09 19:44:00.000000 adafruit-circuitpython-as7341-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:44:19.623590 adafruit-circuitpython-as7341-1.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-as7341-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-as7341-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-as7341-1.2.9/.github/workflows/build.yml`

 * *Files 18% similar despite different names*

```diff
@@ -43,17 +43,35 @@
       run: |
         source actions-ci/install.sh
     - name: Pip install Sphinx, pre-commit
       run: |
         pip install --force-reinstall Sphinx sphinx-rtd-theme pre-commit
     - name: Library version
       run: git describe --dirty --always --tags
+    - name: Setup problem matchers
+      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
     - name: Build assets
       run: circuitpython-build-bundles --filename_prefix ${{ steps.repo-name.outputs.repo-name }} --library_location .
+    - name: Archive bundles
+      uses: actions/upload-artifact@v2
+      with:
+        name: bundles
+        path: ${{ github.workspace }}/bundles/
     - name: Build docs
       working-directory: docs
       run: sphinx-build -E -W -b html . _build/html
-    - name: Setup problem matchers
-      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
+    - name: Check For pyproject.toml
+      id: need-pypi
+      run: |
+        echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
+    - name: Build Python package
+      if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
+      run: |
+        pip install --upgrade build twine
+        for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
+            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+        done;
+        python -m build
+        twine check dist/*
```

### Comparing `adafruit-circuitpython-as7341-1.2.8/.gitignore` & `adafruit-circuitpython-as7341-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-as7341-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/.pylintrc` & `adafruit-circuitpython-as7341-1.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-as7341-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/LICENSE` & `adafruit-circuitpython-as7341-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-as7341-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-as7341-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-as7341-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/PKG-INFO` & `adafruit-circuitpython-as7341-1.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-as7341
-Version: 1.2.8
+Version: 1.2.9
 Summary: CircuitPython library for use with the Adafruit AS7341 breakout
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_AS7341
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython as7341 Spectral sensor multi-channel mux calibration
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AS7341
+Keywords: adafruit,blinka,circuitpython,micropython,as7341,Spectral,sensor,multi-channel,mux,calibration
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-as7341/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/as7341/en/latest/
@@ -71,16 +69,16 @@
     sudo pip3 install adafruit-circuitpython-as7341
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-as7341
 
 Usage Example
 =============
 
 .. code-block:: python3
 
@@ -121,9 +119,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_AS7341/blob/master/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-as7341-1.2.8/README.rst` & `adafruit-circuitpython-as7341-1.2.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     sudo pip3 install adafruit-circuitpython-as7341
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-as7341
 
 Usage Example
 =============
 
 .. code-block:: python3
```

### Comparing `adafruit-circuitpython-as7341-1.2.8/adafruit_as7341.py` & `adafruit-circuitpython-as7341-1.2.9/adafruit_as7341.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 
 * Adafruit's Register library:
   https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 """
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_AS7341.git"
 
 from time import sleep, monotonic
 from micropython import const
 from adafruit_bus_device import i2c_device
 
 from adafruit_register.i2c_struct import UnaryStruct, Struct  # , ROUnaryStruct
```

### Comparing `adafruit-circuitpython-as7341-1.2.8/adafruit_circuitpython_as7341.egg-info/PKG-INFO` & `adafruit-circuitpython-as7341-1.2.9/adafruit_circuitpython_as7341.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-as7341
-Version: 1.2.8
+Version: 1.2.9
 Summary: CircuitPython library for use with the Adafruit AS7341 breakout
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_AS7341
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython as7341 Spectral sensor multi-channel mux calibration
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AS7341
+Keywords: adafruit,blinka,circuitpython,micropython,as7341,Spectral,sensor,multi-channel,mux,calibration
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-as7341/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/as7341/en/latest/
@@ -71,16 +69,16 @@
     sudo pip3 install adafruit-circuitpython-as7341
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-as7341
 
 Usage Example
 =============
 
 .. code-block:: python3
 
@@ -121,9 +119,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_AS7341/blob/master/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-as7341-1.2.8/adafruit_circuitpython_as7341.egg-info/SOURCES.txt` & `adafruit-circuitpython-as7341-1.2.9/adafruit_circuitpython_as7341.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_as7341.py
+optional_requirements.txt
 pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
```

### Comparing `adafruit-circuitpython-as7341-1.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-as7341-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/docs/conf.py` & `adafruit-circuitpython-as7341-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/docs/examples.rst` & `adafruit-circuitpython-as7341-1.2.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/docs/index.rst` & `adafruit-circuitpython-as7341-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/examples/as7341_batched_readings.py` & `adafruit-circuitpython-as7341-1.2.9/examples/as7341_batched_readings.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as7341-1.2.8/examples/as7341_simpletest.py` & `adafruit-circuitpython-as7341-1.2.9/examples/as7341_simpletest.py`

 * *Files identical despite different names*

