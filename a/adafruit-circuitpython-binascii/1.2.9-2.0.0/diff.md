# Comparing `tmp/adafruit-circuitpython-binascii-1.2.9.tar.gz` & `tmp/adafruit-circuitpython-binascii-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-binascii-1.2.9.tar", last modified: Mon Mar 28 14:00:46 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-binascii-2.0.0.tar", last modified: Thu May 11 18:23:47 2023, max compression
```

## Comparing `adafruit-circuitpython-binascii-1.2.9.tar` & `adafruit-circuitpython-binascii-2.0.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 14:00:46.835520 adafruit-circuitpython-binascii-1.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 14:00:46.831520 adafruit-circuitpython-binascii-1.2.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 14:00:46.831520 adafruit-circuitpython-binascii-1.2.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 14:00:46.831520 adafruit-circuitpython-binascii-1.2.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 14:00:46.835520 adafruit-circuitpython-binascii-1.2.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3522 2022-03-28 14:00:46.835520 adafruit-circuitpython-binascii-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5483 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/adafruit_binascii.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 14:00:46.835520 adafruit-circuitpython-binascii-1.2.9/adafruit_circuitpython_binascii.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3522 2022-03-28 14:00:46.000000 adafruit-circuitpython-binascii-1.2.9/adafruit_circuitpython_binascii.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-03-28 14:00:46.000000 adafruit-circuitpython-binascii-1.2.9/adafruit_circuitpython_binascii.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-28 14:00:46.000000 adafruit-circuitpython-binascii-1.2.9/adafruit_circuitpython_binascii.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-28 14:00:46.000000 adafruit-circuitpython-binascii-1.2.9/adafruit_circuitpython_binascii.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-03-28 14:00:46.000000 adafruit-circuitpython-binascii-1.2.9/adafruit_circuitpython_binascii.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 14:00:46.835520 adafruit-circuitpython-binascii-1.2.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 14:00:46.835520 adafruit-circuitpython-binascii-1.2.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5441 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 14:00:46.835520 adafruit-circuitpython-binascii-1.2.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/examples/binascii_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-28 14:00:46.835520 adafruit-circuitpython-binascii-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1889 2022-03-28 14:00:23.000000 adafruit-circuitpython-binascii-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:47.448049 adafruit-circuitpython-binascii-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:47.436048 adafruit-circuitpython-binascii-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:47.444049 adafruit-circuitpython-binascii-2.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:47.444049 adafruit-circuitpython-binascii-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:47.444049 adafruit-circuitpython-binascii-2.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-11 18:23:47.448049 adafruit-circuitpython-binascii-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-11 18:23:37.000000 adafruit-circuitpython-binascii-2.0.0/adafruit_binascii.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:47.448049 adafruit-circuitpython-binascii-2.0.0/adafruit_circuitpython_binascii.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-11 18:23:47.000000 adafruit-circuitpython-binascii-2.0.0/adafruit_circuitpython_binascii.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-11 18:23:47.000000 adafruit-circuitpython-binascii-2.0.0/adafruit_circuitpython_binascii.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:23:47.000000 adafruit-circuitpython-binascii-2.0.0/adafruit_circuitpython_binascii.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-11 18:23:47.000000 adafruit-circuitpython-binascii-2.0.0/adafruit_circuitpython_binascii.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 18:23:47.000000 adafruit-circuitpython-binascii-2.0.0/adafruit_circuitpython_binascii.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:47.448049 adafruit-circuitpython-binascii-2.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:47.448049 adafruit-circuitpython-binascii-2.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:47.448049 adafruit-circuitpython-binascii-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-11 18:23:37.000000 adafruit-circuitpython-binascii-2.0.0/examples/binascii_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-11 18:23:37.000000 adafruit-circuitpython-binascii-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-11 18:23:23.000000 adafruit-circuitpython-binascii-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:23:47.448049 adafruit-circuitpython-binascii-2.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-binascii-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-binascii-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-binascii-1.2.9/.pre-commit-config.yaml` & `adafruit-circuitpython-binascii-2.0.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
-    rev: 20.8b1
+  - repo: https://github.com/python/black
+    rev: 23.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v1.1.2
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.4.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
+    rev: v2.17.4
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
-    -   id: pylint
+      - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
-        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-    -   id: pylint
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
         name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
         types: [python]
         files: "^tests/"
         args:
-        - --disable=missing-docstring,consider-using-f-string,duplicate-code
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-binascii-1.2.9/.pylintrc` & `adafruit-circuitpython-binascii-2.0.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# SPDX-FileCopyrightText: 2020 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
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
@@ -248,86 +242,58 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
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

### Comparing `adafruit-circuitpython-binascii-1.2.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-binascii-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-binascii-1.2.9/LICENSE` & `adafruit-circuitpython-binascii-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-binascii-1.2.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-binascii-2.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-binascii-1.2.9/LICENSES/MIT.txt` & `adafruit-circuitpython-binascii-2.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-binascii-1.2.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-binascii-2.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-binascii-1.2.9/PKG-INFO` & `adafruit-circuitpython-binascii-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-binascii
-Version: 1.2.9
+Version: 2.0.0
 Summary: Helpers for conversions between binary and ASCII
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_binascii
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython binascii binary,ascii,conversion
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_binascii
+Keywords: adafruit,blinka,circuitpython,micropython,binascii,binary,,ascii,,conversion
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
 
-.. image:: https://readthedocs.org/projects/adafruit-circuitpython-binascii/badge/?version=latest
+.. image:: https://readthedocs.org/projects/binascii/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/binascii/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_binascii/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_binascii/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 The binascii module contains a number of methods to convert between binary and various ASCII-encoded binary representations.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -60,16 +63,16 @@
     sudo pip3 install adafruit-circuitpython-binascii
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-binascii
 
 Usage Example
 =============
 
 Hex <-> Binary Conversions
 
@@ -96,9 +99,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_binascii/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-binascii-1.2.9/README.rst` & `adafruit-circuitpython-binascii-2.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Introduction
 ============
 
-.. image:: https://readthedocs.org/projects/adafruit-circuitpython-binascii/badge/?version=latest
+.. image:: https://readthedocs.org/projects/binascii/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/binascii/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_binascii/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_binascii/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 The binascii module contains a number of methods to convert between binary and various ASCII-encoded binary representations.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -41,16 +45,16 @@
     sudo pip3 install adafruit-circuitpython-binascii
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-binascii
 
 Usage Example
 =============
 
 Hex <-> Binary Conversions
```

### Comparing `adafruit-circuitpython-binascii-1.2.9/adafruit_binascii.py` & `adafruit-circuitpython-binascii-2.0.0/adafruit_binascii.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 try:
+    from typing import Union
+    from circuitpython_typing import ReadableBuffer
     from binascii import hexlify, unhexlify
 except ImportError:
     pass
 
-__version__ = "0.0.0-auto.0"
+__version__ = "2.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_binascii.git"
 
 # fmt: off
 TABLE_A2B_B64 = (
     -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1,
     -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1,
     -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, 62, -1, -1, -1, 63,
@@ -59,39 +61,40 @@
 
     # pylint: disable=unnecessary-pass
     pass
 
 
 if not "unhexlify" in globals():
     # pylint: disable=function-redefined
-    def unhexlify(hexstr: str) -> bytes:
+    def unhexlify(hexstr: Union[str, ReadableBuffer]) -> bytes:
         """Return the binary data represented by hexstr.
-        :param str hexstr: Hexadecimal string.
 
+        :param str|ReadableBuffer hexstr: Hexadecimal string.
         """
+
         if len(hexstr) % 2 != 0:
             raise Error("Odd-length string")
 
         return bytes([int(hexstr[i : i + 2], 16) for i in range(0, len(hexstr), 2)])
 
 
 if not "hexlify" in globals():
     # pylint: disable=function-redefined
-    def hexlify(data: bytes) -> bytes:
+    def hexlify(data: ReadableBuffer) -> bytes:
         """Return the hexadecimal representation of the
         binary data. Every byte of data is converted into
         the corresponding 2-digit hex representation.
         The returned bytes object is therefore twice
         as long as the length of data.
 
         :param bytes data: Binary data, as bytes.
-
         """
         if not data:
             raise TypeError("Data provided is zero-length")
+
         data = "".join("%02x" % i for i in data)
         return bytes(data, "utf-8")
 
 
 B2A_HEX = hexlify
 A2B_HEX = unhexlify
 
@@ -102,20 +105,20 @@
     return chr(n)
 
 
 TABLE_A2B_B64 = "".join(map(_transform, TABLE_A2B_B64))
 assert len(TABLE_A2B_B64) == 256
 
 
-def a2b_base64(b64_data: bytes) -> bytes:
+def a2b_base64(b64_data: ReadableBuffer) -> bytes:
     """Convert a block of base64 data back to binary and return the binary data.
 
     :param bytes b64_data: Base64 data.
-
     """
+
     res = []
     quad_pos = 0
     leftchar = 0
     leftbits = 0
     last_char_was_a_pad = False
 
     for char in b64_data:
@@ -139,25 +142,25 @@
                 leftbits -= 8
                 res.append((leftchar >> leftbits).to_bytes(1, "big"))
                 leftchar &= (1 << leftbits) - 1
             #
             last_char_was_a_pad = False
     else:
         if leftbits != 0:
-            raise Exception("Incorrect padding")
+            raise ValueError("Incorrect padding")
 
     return b"".join(res)
 
 
-def b2a_base64(bin_data: bytes) -> bytes:
+def b2a_base64(bin_data: ReadableBuffer) -> bytes:
     """Convert binary data to a line of ASCII characters in base64 coding.
 
-    :param bytes bin_data: Binary data string, as bytes
-
+    :param ReadableBuffer bin_data: Binary data string, as bytes
     """
+
     newlength = (len(bin_data) + 2) // 3
     newlength = newlength * 4 + 1
     res = []
 
     leftchar = 0
     leftbits = 0
     for char in bin_data:
```

### Comparing `adafruit-circuitpython-binascii-1.2.9/adafruit_circuitpython_binascii.egg-info/PKG-INFO` & `adafruit-circuitpython-binascii-2.0.0/adafruit_circuitpython_binascii.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-binascii
-Version: 1.2.9
+Version: 2.0.0
 Summary: Helpers for conversions between binary and ASCII
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_binascii
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython binascii binary,ascii,conversion
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_binascii
+Keywords: adafruit,blinka,circuitpython,micropython,binascii,binary,,ascii,,conversion
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
 
-.. image:: https://readthedocs.org/projects/adafruit-circuitpython-binascii/badge/?version=latest
+.. image:: https://readthedocs.org/projects/binascii/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/binascii/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_binascii/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_binascii/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 The binascii module contains a number of methods to convert between binary and various ASCII-encoded binary representations.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -60,16 +63,16 @@
     sudo pip3 install adafruit-circuitpython-binascii
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-binascii
 
 Usage Example
 =============
 
 Hex <-> Binary Conversions
 
@@ -96,9 +99,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_binascii/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-binascii-1.2.9/adafruit_circuitpython_binascii.egg-info/SOURCES.txt` & `adafruit-circuitpython-binascii-2.0.0/adafruit_circuitpython_binascii.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_binascii.py
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
 adafruit_circuitpython_binascii.egg-info/PKG-INFO
 adafruit_circuitpython_binascii.egg-info/SOURCES.txt
 adafruit_circuitpython_binascii.egg-info/dependency_links.txt
 adafruit_circuitpython_binascii.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-binascii-1.2.9/docs/_static/favicon.ico` & `adafruit-circuitpython-binascii-2.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-binascii-1.2.9/docs/conf.py` & `adafruit-circuitpython-binascii-2.0.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2020 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -39,15 +40,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit binascii Library"
-copyright = "2019 Brent Rubell "
+creation_year = "2019"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Brent Rubell "
 author = "Brent Rubell "
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
@@ -56,15 +64,15 @@
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

### Comparing `adafruit-circuitpython-binascii-1.2.9/docs/index.rst` & `adafruit-circuitpython-binascii-2.0.0/docs/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 .. toctree::
     :caption: Related Products
 
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_binascii/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_binascii/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-binascii-1.2.9/examples/binascii_simpletest.py` & `adafruit-circuitpython-binascii-2.0.0/examples/binascii_simpletest.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 print("Original Binary Data: ", data)
 
 # Get the hexadecimal representation of the binary data
 hex_data = hexlify(data)
 print("Hex Data: ", hex_data)
 # Verify data
 assert (
-    hex_data == b"43697263756974507974686f6e20697320417765736f6d6521",
+    hex_data == b"43697263756974507974686f6e20697320417765736f6d6521"
 ), "hexlified data does not match expected data."
 # Get the binary data represented by hex_data
 bin_data = unhexlify(hex_data)
 print("Binary Data: ", bin_data)
 # Verify data
 assert bin_data == data, "unhexlified binary data does not match original binary data."
```

