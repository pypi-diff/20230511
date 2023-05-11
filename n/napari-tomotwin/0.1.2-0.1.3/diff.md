# Comparing `tmp/napari-tomotwin-0.1.2.tar.gz` & `tmp/napari-tomotwin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-tomotwin-0.1.2.tar", last modified: Fri Apr 28 11:48:14 2023, max compression
+gzip compressed data, was "napari-tomotwin-0.1.3.tar", last modified: Wed May 10 12:17:43 2023, max compression
```

## Comparing `napari-tomotwin-0.1.2.tar` & `napari-tomotwin-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.370733 napari-tomotwin-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-28 11:48:14.378733 napari-tomotwin-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/src/napari_tomotwin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/src/napari_tomotwin/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/src/napari_tomotwin/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/_tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/load_umap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/make_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/src/napari_tomotwin/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:48:14.374733 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 11:48:14.000000 napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-28 11:47:49.000000 napari-tomotwin-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:43.890031 napari-tomotwin-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:43.886031 napari-tomotwin-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:43.890031 napari-tomotwin-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:43.890031 napari-tomotwin-0.1.3/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-10 12:17:43.890031 napari-tomotwin-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-10 12:17:43.890031 napari-tomotwin-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:43.890031 napari-tomotwin-0.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:43.890031 napari-tomotwin-0.1.3/src/napari_tomotwin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/src/napari_tomotwin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:43.890031 napari-tomotwin-0.1.3/src/napari_tomotwin/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/src/napari_tomotwin/_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:43.890031 napari-tomotwin-0.1.3/src/napari_tomotwin/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/src/napari_tomotwin/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/src/napari_tomotwin/_tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 12:17:43.000000 napari-tomotwin-0.1.3/src/napari_tomotwin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/src/napari_tomotwin/load_umap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/src/napari_tomotwin/make_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/src/napari_tomotwin/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:43.890031 napari-tomotwin-0.1.3/src/napari_tomotwin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-10 12:17:43.000000 napari-tomotwin-0.1.3/src/napari_tomotwin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-10 12:17:43.000000 napari-tomotwin-0.1.3/src/napari_tomotwin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:17:43.000000 napari-tomotwin-0.1.3/src/napari_tomotwin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 12:17:43.000000 napari-tomotwin-0.1.3/src/napari_tomotwin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 12:17:43.000000 napari-tomotwin-0.1.3/src/napari_tomotwin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 12:17:43.000000 napari-tomotwin-0.1.3/src/napari_tomotwin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-10 12:17:19.000000 napari-tomotwin-0.1.3/tox.ini
```

### Comparing `napari-tomotwin-0.1.2/.github/workflows/test_and_deploy.yml` & `napari-tomotwin-0.1.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.2/.gitignore` & `napari-tomotwin-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.2/.napari-hub/config.yml` & `napari-tomotwin-0.1.3/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.2/.pre-commit-config.yaml` & `napari-tomotwin-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.2/LICENSE` & `napari-tomotwin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.2/PKG-INFO` & `napari-tomotwin-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-tomotwin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Several tools for the work with TomoTwin
 Home-page: https://github.com/MPI-Dortmund/napari-tomotwin
 Author: Thorsten Wagner
 Author-email: twa1@posteo.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-tomotwin-0.1.2/README.md` & `napari-tomotwin-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.2/setup.cfg` & `napari-tomotwin-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.2/src/napari_tomotwin/load_umap.py` & `napari-tomotwin-0.1.3/src/napari_tomotwin/load_umap.py`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.2/src/napari_tomotwin/make_targets.py` & `napari-tomotwin-0.1.3/src/napari_tomotwin/make_targets.py`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.2/src/napari_tomotwin/napari.yaml` & `napari-tomotwin-0.1.3/src/napari_tomotwin/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/PKG-INFO` & `napari-tomotwin-0.1.3/src/napari_tomotwin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-tomotwin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Several tools for the work with TomoTwin
 Home-page: https://github.com/MPI-Dortmund/napari-tomotwin
 Author: Thorsten Wagner
 Author-email: twa1@posteo.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-tomotwin-0.1.2/src/napari_tomotwin.egg-info/SOURCES.txt` & `napari-tomotwin-0.1.3/src/napari_tomotwin.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
+changelog.md
 pyproject.toml
 requirements.txt
 setup.cfg
 tox.ini
 .github/workflows/test_and_deploy.yml
 .napari-hub/DESCRIPTION.md
 .napari-hub/config.yml
```

### Comparing `napari-tomotwin-0.1.2/tox.ini` & `napari-tomotwin-0.1.3/tox.ini`

 * *Files identical despite different names*

