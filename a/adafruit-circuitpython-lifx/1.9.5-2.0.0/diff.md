# Comparing `tmp/adafruit-circuitpython-lifx-1.9.5.tar.gz` & `tmp/adafruit-circuitpython-lifx-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lifx-1.9.5.tar", last modified: Tue Mar  2 23:59:52 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-lifx-2.0.0.tar", last modified: Thu May 11 18:25:30 2023, max compression
```

## Comparing `adafruit-circuitpython-lifx-1.9.5.tar` & `adafruit-circuitpython-lifx-2.0.0.tar`

### file list

```diff
@@ -1,41 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:59:52.795854 adafruit-circuitpython-lifx-1.9.5/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:59:52.779854 adafruit-circuitpython-lifx-1.9.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:59:52.787854 adafruit-circuitpython-lifx-1.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2329 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)      189 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1020 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    16231 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)      162 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     6147 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1103 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:59:52.791854 adafruit-circuitpython-lifx-1.9.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (116)     4990 2021-03-02 23:59:52.795854 adafruit-circuitpython-lifx-1.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3358 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      108 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:59:52.791854 adafruit-circuitpython-lifx-1.9.5/adafruit_circuitpython_lifx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4990 2021-03-02 23:59:52.000000 adafruit-circuitpython-lifx-1.9.5/adafruit_circuitpython_lifx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      751 2021-03-02 23:59:52.000000 adafruit-circuitpython-lifx-1.9.5/adafruit_circuitpython_lifx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-02 23:59:52.000000 adafruit-circuitpython-lifx-1.9.5/adafruit_circuitpython_lifx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       48 2021-03-02 23:59:52.000000 adafruit-circuitpython-lifx-1.9.5/adafruit_circuitpython_lifx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2021-03-02 23:59:52.000000 adafruit-circuitpython-lifx-1.9.5/adafruit_circuitpython_lifx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     5528 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/adafruit_lifx.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:59:52.795854 adafruit-circuitpython-lifx-1.9.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:59:52.795854 adafruit-circuitpython-lifx-1.9.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (116)      279 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     5133 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      182 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)      899 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:59:52.795854 adafruit-circuitpython-lifx-1.9.5/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     1828 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/examples/lifx_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)      151 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-02 23:59:52.795854 adafruit-circuitpython-lifx-1.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1962 2021-03-02 23:59:41.000000 adafruit-circuitpython-lifx-1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.893089 adafruit-circuitpython-lifx-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.885089 adafruit-circuitpython-lifx-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.889089 adafruit-circuitpython-lifx-2.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.889089 adafruit-circuitpython-lifx-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.889089 adafruit-circuitpython-lifx-2.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-11 18:25:30.893089 adafruit-circuitpython-lifx-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.889089 adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-11 18:25:30.000000 adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-11 18:25:30.000000 adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:25:30.000000 adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-11 18:25:30.000000 adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 18:25:30.000000 adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-11 18:25:23.000000 adafruit-circuitpython-lifx-2.0.0/adafruit_lifx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.893089 adafruit-circuitpython-lifx-2.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.893089 adafruit-circuitpython-lifx-2.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.893089 adafruit-circuitpython-lifx-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-11 18:25:23.000000 adafruit-circuitpython-lifx-2.0.0/examples/lifx_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-11 18:25:23.000000 adafruit-circuitpython-lifx-2.0.0/examples/lifx_simpletest_esp32s2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-11 18:25:23.000000 adafruit-circuitpython-lifx-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:25:30.893089 adafruit-circuitpython-lifx-2.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-lifx-1.9.5/.pre-commit-config.yaml` & `adafruit-circuitpython-lifx-2.0.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,42 @@
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
-    rev: pylint-2.7.1
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
-        exclude: "^(docs/|examples/|setup.py$)"
--   repo: local
-    hooks:
-    -   id: pylint_examples
-        name: pylint (examples code)
+        args:
+          - --disable=consider-using-f-string
+        exclude: "^(docs/|examples/|tests/|setup.py$)"
+      - id: pylint
+        name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
-        entry: /usr/bin/env bash -c
-        args: ['([[ ! -d "examples" ]] || for example in $(find . -path "./examples/*.py"); do pylint --disable=missing-docstring,invalid-name $example; done)']
-        language: system
+        types: [python]
+        files: "^examples/"
+        args:
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
+        name: pylint (test code)
+        description: Run pylint rules on "tests/*.py" files
+        types: [python]
+        files: "^tests/"
+        args:
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-lifx-1.9.5/.pylintrc` & `adafruit-circuitpython-lifx-2.0.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
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
-# jobs=1
-jobs=2
+jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -51,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -222,20 +221,14 @@
 
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
@@ -249,86 +242,58 @@
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
 
@@ -336,17 +301,14 @@
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

### Comparing `adafruit-circuitpython-lifx-1.9.5/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-lifx-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-1.9.5/LICENSE` & `adafruit-circuitpython-lifx-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-1.9.5/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-lifx-2.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-1.9.5/LICENSES/MIT.txt` & `adafruit-circuitpython-lifx-2.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-1.9.5/LICENSES/Unlicense.txt` & `adafruit-circuitpython-lifx-2.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-1.9.5/README.rst` & `adafruit-circuitpython-lifx-2.0.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-lifx/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/lifx/en/latest/
+    :target: https://docs.circuitpython.org/projects/lifx/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_lifx/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_lifx
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 Control `LIFX devices <https://www.lifx.com>`_ over the internet using CircuitPython.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -47,16 +51,16 @@
     sudo pip3 install adafruit-circuitpython-lifx
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-lifx
 
 Usage Example
 =============
 
 Initialize the LIFX API Client with a WiFiManager object and a
 `LIFX Personal Access token <https://cloud.lifx.com/settings>`_:
@@ -91,18 +95,20 @@
 
 Set the color of a LIFX device to blue and the brightness to 100%:
 
 .. code-block:: python
 
     lifx.set_color(lifx_light, 'on', 'blue', brightness=1.0)
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/lifx/en/latest/>`_.
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
-<https://github.com/adafruit/Adafruit_CircuitPython_lifx/blob/master/CODE_OF_CONDUCT.md>`_
+<https://github.com/adafruit/Adafruit_CircuitPython_lifx/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-lifx-1.9.5/adafruit_lifx.py` & `adafruit-circuitpython-lifx-2.0.0/adafruit_lifx.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,126 +17,152 @@
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 * Adafruit ESP32SPI or ESP_ATcontrol library:
     https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
     https://github.com/adafruit/Adafruit_CircuitPython_ESP_ATcontrol
+
+or:
+
+* Adafruit_requests library:
+   https://github.com/adafruit/Adafruit_CircuitPython_Requests
+
 """
 
-__version__ = "0.0.0-auto.0"
+__version__ = "2.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_lifx.git"
 
 LIFX_URL = "https://api.lifx.com/v1/lights/"
 
+try:
+    from typing import Dict, Any
+    from circuitpython_typing.http import HTTPProtocol
+    from adafruit_requests import Response
+except ImportError:
+    pass
+
 
 class LIFX:
-    """
-    HTTP Interface for interacting with the LIFX API
+    """HTTP Interface for interacting with the LIFX API
+
+    :param wifi_manager: WiFiManager from ESPSPI_WiFiManager/ESPAT_WiFiManager
+        or session from adafruit_requests.Session
+    :param str lifx_token: LIFX API token (https://api.developer.lifx.com/docs/authentication)
     """
 
-    def __init__(self, wifi_manager, lifx_token):
-        """
-        Creates an instance of the LIFX HTTP API client.
-        :param wifi_manager wifi_manager: WiFiManager from ESPSPI_WiFiManager/ESPAT_WiFiManager
-        :param str lifx_token: LIFX API token (https://api.developer.lifx.com/docs/authentication)
-        """
+    def __init__(self, wifi_manager: HTTPProtocol, lifx_token: str) -> None:
         wifi_type = str(type(wifi_manager))
-        if "ESPSPI_WiFiManager" in wifi_type or "ESPAT_WiFiManager" in wifi_type:
+        allowed_wifi_types = ("ESPSPI_WiFiManager", "ESPAT_WiFiManager", "Session")
+        if any(x in wifi_type for x in allowed_wifi_types):
             self._wifi = wifi_manager
         else:
-            raise TypeError("This library requires a WiFiManager object.")
+            raise TypeError("This library requires a WiFiManager or Session object.")
         self._lifx_token = lifx_token
         self._auth_header = {
             "Authorization": "Bearer %s" % self._lifx_token,
         }
 
     @staticmethod
-    def _parse_resp(response):
+    def _parse_resp(response: Response) -> str:
         """Parses and returns the JSON response returned
         from the LIFX HTTP API.
         """
         if response.status_code == 422:
-            raise Exception(
+            raise RuntimeError(
                 "Error: light(s) could not be toggled: " + response["error"]
             )
         try:
             for res in response.json()["results"]:
                 return res["status"]
         except KeyError as err:
             raise KeyError(response.json()["error"]) from err
 
     # HTTP Requests
-    def _post(self, path, data):
+    def _post(self, path: str, data: Dict[str, Any]) -> str:
         """POST data to the LIFX API.
+
         :param str path: Formatted LIFX API URL
-        :param json data: JSON data to POST to the LIFX API.
+        :param dict data: JSON data to POST to the LIFX API.
         """
         response = self._wifi.post(path, json=data, headers=self._auth_header)
         response = self._parse_resp(response)
         return response
 
-    def _put(self, path, data):
+    def _put(self, path: str, data: Dict[str, Any]) -> str:
         """PUT data to the LIFX API.
+
         :param str path: Formatted LIFX API URL
-        :param json data: JSON data to PUT to the LIFX API.
+        :param dict data: JSON data to PUT to the LIFX API.
         """
         response = self._wifi.put(path, json=data, headers=self._auth_header)
         response = self._parse_resp(response)
         return response
 
-    def _get(self, path, data):
+    def _get(self, path: str, data: Dict[str, Any]) -> Dict[str, Any]:
         """GET data from the LIFX API.
+
         :param str path: Formatted LIFX API URL
-        :param json data: JSON data to GET from the LIFX API.
+        :param dict data: JSON data to GET from the LIFX API.
         """
         response = self._wifi.get(path, json=data, headers=self._auth_header)
         return response.json()
 
-    def toggle_light(self, selector, all_lights=False, duration=0):
+    def toggle_light(
+        self, selector: str, all_lights: bool = False, duration: float = 0
+    ) -> str:
         """Toggles current state of LIFX light(s).
-        :param dict selector: Selector to control which lights are requested.
+
+        :param str selector: Selector to control which lights are requested.
         :param bool all: Toggle all lights at once. Defaults to false.
-        :param double duration: Time (in seconds) to spend performing a toggle. Defaults to 0.
+        :param float duration: Time (in seconds) to spend performing a toggle. Defaults to 0.
         """
         if all_lights:
             selector = "all"
         data = {"duration": duration}
         return self._post(LIFX_URL + selector + "/toggle", data)
 
-    def move_effect(self, selector, move_direction, period, power_on):
+    def move_effect(
+        self, selector: str, move_direction: str, period: float, power_on: bool
+    ) -> str:
         """Performs a linear move effect on a light, or lights.
+
+        :param str selector: Selector to control which lights are requested.
         :param str move_direction: Move direction, forward or backward.
-        :param double period: Time in second per effect cycle.
+        :param float period: Time in second per effect cycle.
         :param bool power_on: Turn on a light before performing the move.
         """
         data = {"direction": move_direction, "period": period, "power_on": power_on}
         return self._post(LIFX_URL + selector + "/effects/move", data)
 
-    def effects_off(self, selector, power_off=False):
+    def effects_off(self, selector: str, power_off: bool = False) -> str:
         """Turns off any running effects on the selected device.
-        :param dict selector: Selector to control which lights are requested.
+
+        :param str selector: Selector to control which lights are requested.
         :param bool power_off: If true, the devices will also be turned off.
         """
         data = {"power_off", power_off}
         return self._post(LIFX_URL + selector + "/effects/off", data)
 
-    def set_brightness(self, selector, brightness):
+    def set_brightness(self, selector: str, brightness: float) -> str:
         """Sets the state of the lights within the selector.
-        :param dict selector: Selector to control which lights are requested.
-        :param double brightness: Brightness level of the light, from 0.0 to 1.0.
+
+        :param str selector: Selector to control which lights are requested.
+        :param float brightness: Brightness level of the light, from 0.0 to 1.0.
         """
         data = {"brightness": brightness}
         return self._put(LIFX_URL + selector + "/state", data)
 
-    def set_color(self, selector, **kwargs):
+    def set_color(self, selector: str, **kwargs) -> str:
         """Sets the state of the light's color within the selector.
-        Valid arguments: https://api.developer.lifx.com/docs/set-state
+        Valid keyword arguments: https://api.developer.lifx.com/docs/set-state
+
+        :param str selector: Selector to control which lights are requested.
         """
         return self._put(LIFX_URL + selector + "/state", kwargs)
 
-    def list_lights(self):
+    def list_lights(self) -> Dict[str, Any]:
         """Enumerates all the lights associated with the LIFX Cloud Account"""
         response = self._wifi.get(url=LIFX_URL + "all", headers=self._auth_header)
         resp = response.json()
         response.close()
         return resp
```

### Comparing `adafruit-circuitpython-lifx-1.9.5/docs/_static/favicon.ico` & `adafruit-circuitpython-lifx-2.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-1.9.5/docs/conf.py` & `adafruit-circuitpython-lifx-2.0.0/docs/conf.py`

 * *Files 8% similar despite different names*

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
@@ -19,29 +20,36 @@
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/3.4", None),
-    "CircuitPython": ("https://circuitpython.readthedocs.io/en/latest/", None),
+    "python": ("https://docs.python.org/3", None),
+    "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit LIFX Library"
-copyright = "2019 Brent Rubell"
+creation_year = "2019"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Brent Rubell"
 author = "Brent Rubell"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
@@ -50,15 +58,15 @@
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

### Comparing `adafruit-circuitpython-lifx-1.9.5/docs/index.rst` & `adafruit-circuitpython-lifx-2.0.0/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 .. toctree::
     :caption: Related Products
 
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_lifx/releases/latest>
-    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_lifx/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
+    CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-lifx-1.9.5/examples/lifx_simpletest.py` & `adafruit-circuitpython-lifx-2.0.0/examples/lifx_simpletest.py`

 * *Files identical despite different names*

