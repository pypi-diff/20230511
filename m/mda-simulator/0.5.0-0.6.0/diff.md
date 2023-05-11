# Comparing `tmp/mda_simulator-0.5.0.tar.gz` & `tmp/mda_simulator-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mda_simulator-0.5.0.tar", last modified: Tue Jun  7 15:55:59 2022, max compression
+gzip compressed data, was "mda_simulator-0.6.0.tar", last modified: Thu May 11 03:37:11 2023, max compression
```

## Comparing `mda_simulator-0.5.0.tar` & `mda_simulator-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 15:55:59.201079 mda_simulator-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 15:55:59.197079 mda_simulator-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 15:55:59.197079 mda_simulator-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-06-07 15:55:59.201079 mda_simulator-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 15:55:59.201079 mda_simulator-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 15:55:59.201079 mda_simulator-0.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)   443158 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/docs/_static/example-napari.apng
--rw-r--r--   0 runner    (1001) docker     (121)     5377 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 15:55:59.201079 mda_simulator-0.5.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     6075 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/docs/examples/napari-micromanager.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    71651 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/docs/examples/standalone-usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 15:55:59.201079 mda_simulator-0.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     5686 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/examples/config.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/examples/napari-micromanager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 15:55:59.201079 mda_simulator-0.5.0/mda_simulator/
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/mda_simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/mda_simulator/_generators.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-06-07 15:55:58.000000 mda_simulator-0.5.0/mda_simulator/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 15:55:59.201079 mda_simulator-0.5.0/mda_simulator/mmcore/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/mda_simulator/mmcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4927 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/mda_simulator/mmcore/_mmcore.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 15:55:59.201079 mda_simulator-0.5.0/mda_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-06-07 15:55:58.000000 mda_simulator-0.5.0/mda_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-06-07 15:55:59.000000 mda_simulator-0.5.0/mda_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 15:55:58.000000 mda_simulator-0.5.0/mda_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 15:55:57.000000 mda_simulator-0.5.0/mda_simulator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-06-07 15:55:59.000000 mda_simulator-0.5.0/mda_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-07 15:55:59.000000 mda_simulator-0.5.0/mda_simulator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-06-07 15:55:59.201079 mda_simulator-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 15:55:59.201079 mda_simulator-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/tests/test_mda_simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-06-07 15:55:40.000000 mda_simulator-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:37:11.973787 mda_simulator-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:37:11.969787 mda_simulator-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:37:11.969787 mda_simulator-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-11 03:37:11.973787 mda_simulator-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:37:11.969787 mda_simulator-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:37:11.969787 mda_simulator-0.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)   443158 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/docs/_static/example-napari.apng
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:37:11.969787 mda_simulator-0.6.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/docs/examples/napari-micromanager.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    71651 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/docs/examples/standalone-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:37:11.969787 mda_simulator-0.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/examples/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/examples/napari-micromanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:37:11.969787 mda_simulator-0.6.0/mda_simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/mda_simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/mda_simulator/_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 03:37:11.000000 mda_simulator-0.6.0/mda_simulator/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:37:11.973787 mda_simulator-0.6.0/mda_simulator/mmcore/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/mda_simulator/mmcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/mda_simulator/mmcore/_mmcore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:37:11.973787 mda_simulator-0.6.0/mda_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-11 03:37:11.000000 mda_simulator-0.6.0/mda_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-11 03:37:11.000000 mda_simulator-0.6.0/mda_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 03:37:11.000000 mda_simulator-0.6.0/mda_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 03:37:11.000000 mda_simulator-0.6.0/mda_simulator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-11 03:37:11.000000 mda_simulator-0.6.0/mda_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 03:37:11.000000 mda_simulator-0.6.0/mda_simulator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-11 03:37:11.973787 mda_simulator-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:37:11.973787 mda_simulator-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/tests/test_mda_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-11 03:36:52.000000 mda_simulator-0.6.0/tox.ini
```

### Comparing `mda_simulator-0.5.0/.github/workflows/ci.yml` & `mda_simulator-0.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/.github/workflows/publish.yml` & `mda_simulator-0.6.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/.gitignore` & `mda_simulator-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/.pre-commit-config.yaml` & `mda_simulator-0.6.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 ci:
   autoupdate_schedule: 'quarterly'
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.0.1
+    rev: v4.4.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
       - id: mixed-line-ending
       - id: check-merge-conflict
   - repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v1.17.0
+    rev: v2.2.0
     hooks:
       - id: setup-cfg-fmt
   - repo: https://github.com/PyCQA/flake8
-    rev: 3.9.2
+    rev: 6.0.0
     hooks:
       - id: flake8
-        additional_dependencies: [flake8-typing-imports==1.7.0]
   - repo: https://github.com/myint/autoflake
-    rev: v1.4
+    rev: v2.1.1
     hooks:
       - id: autoflake
         args: ["--in-place", "--remove-all-unused-imports", "--ignore-init-module-imports", "--remove-unused-variables"]
   - repo: https://github.com/PyCQA/isort
-    rev: 5.8.0
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.19.0
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
-  - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.812
-    hooks:
-      - id: mypy
+  # - repo: https://github.com/pre-commit/mirrors-mypy
+  #   rev: v1.2.0
+  #   hooks:
+  #     - id: mypy
```

### Comparing `mda_simulator-0.5.0/LICENSE` & `mda_simulator-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/PKG-INFO` & `mda_simulator-0.6.0/mda_simulator.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
-Name: mda_simulator
-Version: 0.5.0
+Name: mda-simulator
+Version: 0.6.0
 Summary: mda simulator
 Home-page: https://github.com/ianhi/mda-simulator
 Author: Ian Hunt-Isaak, John Russell
 Author-email: ianhuntisaak@gmail.com
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/ianhi/mda-simulator
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `mda_simulator-0.5.0/README.md` & `mda_simulator-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/docs/Makefile` & `mda_simulator-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/docs/_static/example-napari.apng` & `mda_simulator-0.6.0/docs/_static/example-napari.apng`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/docs/conf.py` & `mda_simulator-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/docs/contributing.md` & `mda_simulator-0.6.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/docs/examples/napari-micromanager.ipynb` & `mda_simulator-0.6.0/docs/examples/napari-micromanager.ipynb`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/docs/examples/standalone-usage.ipynb` & `mda_simulator-0.6.0/docs/examples/standalone-usage.ipynb`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/docs/index.md` & `mda_simulator-0.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/docs/make.bat` & `mda_simulator-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/examples/basic.py` & `mda_simulator-0.6.0/examples/basic.py`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/examples/config.cfg` & `mda_simulator-0.6.0/examples/config.cfg`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/examples/napari-micromanager.py` & `mda_simulator-0.6.0/examples/napari-micromanager.py`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/mda_simulator/_generators.py` & `mda_simulator-0.6.0/mda_simulator/_generators.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,37 +18,48 @@
         N: int,
         img_shape: tuple[int, int] = (512, 512),
         extent=10,
         radius_loc=25,
         radius_scale=5,
         step_scale: tuple[float, float] = (2.5, 2.5),
         XY_stage_drift: tuple[int, int] = (0, 0),
+        snr=1,
     ):
         self._rng = np.random.default_rng()
         self._N = N
         self._ids = np.arange(N)
         self._radii = self._rng.normal(radius_loc, radius_scale, N)
         self._colors = self._rng.random((N, 3))
         self._shape = np.array(img_shape)
         X = self._rng.uniform(-self._shape[0] * extent, self._shape[0] * extent, (N, 1))
         Y = self._rng.uniform(-self._shape[1] * extent, self._shape[1] * extent, (N, 1))
         self._pos = np.hstack((X, Y))
         self._step_scale = np.asarray(step_scale)
         self._stage_drift = np.array(XY_stage_drift)
+        self._snr = snr
         # A is per channel
         self._A: dict[int, np.ndarray] = defaultdict(
             lambda: np.abs(self._rng.normal(1024, 256))
         )
         # sigma dict is per cell/per channel
         self._sigma: dict[int, np.ndarray] = defaultdict(
             lambda: 1
             + np.abs(self._rng.normal(radius_loc / 10, radius_scale / 10, size=self._N))
         )
 
     @property
+    def snr(self) -> float:
+        return self._snr
+
+    @snr.setter
+    def snr(self, val: float):
+        # TODO: add validation
+        self._snr = val
+
+    @property
     def img_shape(self) -> np.ndarray:
         return self._shape
 
     def snap_img(self, xy: tuple[float, float], c: int = 0, z: float = 0, exposure=1):
         return self._snap_img(tuple(xy), c, z, exposure)
 
     @lru_cache(256)
@@ -67,26 +78,28 @@
         inter = radii**2 - z**2
         inter[inter < 0] = 0
         radii = np.sqrt(inter)
         sigmas = self._sigma[c][idx]
         A = self._A[c]
         ids = self._ids[idx]
 
-        out = np.zeros(self._shape, dtype=np.uint16)
+        out = np.zeros(self._shape, dtype=np.int16)
 
         for pos, r, id_, sigma in zip(coords, radii, ids, sigmas):
-
             pixels = disk(pos, r, shape=self._shape)
             if c > 0:
                 dists = np.sqrt((pixels[0] - pos[0]) ** 2 + (pixels[1] - pos[1]) ** 2)
                 intensity = exposure * A * np.exp(-dists / (2 * sigma**2))
             else:
-                intensity = id_
+                intensity = A
             out[pixels] = intensity
-        return out
+        # todo: make this poisson
+        out = out + self._rng.normal(0, A / self._snr, size=self._shape)
+        out[out < 0] = 0
+        return out.astype(np.uint16).T
 
     def image2rgb(self, img):
         """
         Convert a grayscale image from this generator to RGB for easy viewing
         Parameters
         ----------
         img : (M, M) of int
```

### Comparing `mda_simulator-0.5.0/mda_simulator/mmcore/_mmcore.py` & `mda_simulator-0.6.0/mda_simulator/mmcore/_mmcore.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,19 @@
             The number of real world seconds to wait to update the simulation time
             step.
         core : CMMCorePlus
             If not provided then the current instance will be used
         """
         self._core = core if core else CMMCorePlus.instance()
         self._channel_tracker = ChannelTracker(core=core)
-        self._lock = self._core.lock
+        try:
+            self._lock = self._core._lock
+        except AttributeError:
+            self._lock = self._core.lock
+
         self._image = None
         self._img_gen: ImageGenerator = img_gen if img_gen else ImageGenerator(10000)
         self._core.snapImage = self._snapImage
         self._core.getImage = self._getImage
         self._core.getLastImage = self._getLastImage
 
         self._timing = timing
@@ -129,15 +133,14 @@
         """
         self._timer.stop()
 
     def _bump_time(self):
         self._img_gen.increment_time()
 
     def _snapImage(self) -> None:
-
         with synchronized(self._lock):
             # self.core
             xy = self._core.getXYPosition()
 
             c = self._channel_tracker.current_channel_idx
             z = self._core.getPosition()
             exp = self._core.getExposure()
```

### Comparing `mda_simulator-0.5.0/mda_simulator.egg-info/PKG-INFO` & `mda_simulator-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
-Name: mda-simulator
-Version: 0.5.0
+Name: mda_simulator
+Version: 0.6.0
 Summary: mda simulator
 Home-page: https://github.com/ianhi/mda-simulator
 Author: Ian Hunt-Isaak, John Russell
 Author-email: ianhuntisaak@gmail.com
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/ianhi/mda-simulator
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `mda_simulator-0.5.0/mda_simulator.egg-info/SOURCES.txt` & `mda_simulator-0.6.0/mda_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/pyproject.toml` & `mda_simulator-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mda_simulator-0.5.0/setup.cfg` & `mda_simulator-0.6.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 license_file = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: Implementation :: CPython
 project_urls = 
 	Source Code =https://github.com/ianhi/mda-simulator
 
 [options]
 packages = find:
 install_requires =
```

### Comparing `mda_simulator-0.5.0/tox.ini` & `mda_simulator-0.6.0/tox.ini`

 * *Files identical despite different names*

