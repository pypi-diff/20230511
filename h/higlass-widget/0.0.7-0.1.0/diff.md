# Comparing `tmp/higlass-widget-0.0.7.tar.gz` & `tmp/higlass_widget-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "higlass-widget-0.0.7.tar", last modified: Mon Feb 14 17:26:09 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `higlass-widget-0.0.7.tar` & `higlass_widget-0.1.0.tar`

### file list

```diff
@@ -1,41 +1,11 @@
-drwxr-xr-x   0 hms-manzt   (501) staff       (20)        0 2022-02-14 17:26:09.303370 higlass-widget-0.0.7/
--rw-r--r--   0 hms-manzt   (501) staff       (20)      205 2022-02-13 02:48:56.000000 higlass-widget-0.0.7/.gitignore
--rw-r--r--   0 hms-manzt   (501) staff       (20)     1074 2022-02-12 20:41:40.000000 higlass-widget-0.0.7/LICENSE
--rw-r--r--   0 hms-manzt   (501) staff       (20)      211 2022-02-13 02:02:36.000000 higlass-widget-0.0.7/MANIFEST.in
--rw-r--r--   0 hms-manzt   (501) staff       (20)     1557 2022-02-14 17:26:09.303501 higlass-widget-0.0.7/PKG-INFO
--rw-r--r--   0 hms-manzt   (501) staff       (20)     1231 2022-02-13 02:18:42.000000 higlass-widget-0.0.7/README.md
--rw-r--r--   0 hms-manzt   (501) staff       (20)       68 2022-02-12 14:53:55.000000 higlass-widget-0.0.7/higlass-widget.json
-drwxr-xr-x   0 hms-manzt   (501) staff       (20)        0 2022-02-14 17:26:09.281395 higlass-widget-0.0.7/higlass_widget/
--rw-r--r--   0 hms-manzt   (501) staff       (20)      573 2022-02-13 17:53:16.000000 higlass-widget-0.0.7/higlass_widget/__init__.py
--rw-r--r--   0 hms-manzt   (501) staff       (20)      231 2022-02-13 17:53:16.000000 higlass-widget-0.0.7/higlass_widget/_version.py
-drwxr-xr-x   0 hms-manzt   (501) staff       (20)        0 2022-02-14 17:26:09.283034 higlass-widget-0.0.7/higlass_widget/labextension/
--rw-r--r--   0 hms-manzt   (501) staff       (20)     1278 2022-02-14 16:31:39.000000 higlass-widget-0.0.7/higlass_widget/labextension/package.json
-drwxr-xr-x   0 hms-manzt   (501) staff       (20)        0 2022-02-14 17:26:09.294302 higlass-widget-0.0.7/higlass_widget/labextension/static/
--rw-r--r--   0 hms-manzt   (501) staff       (20)     1682 2022-02-14 16:31:39.000000 higlass-widget-0.0.7/higlass_widget/labextension/static/345.2446d2ed6029122637de.js
--rw-r--r--   0 hms-manzt   (501) staff       (20)   459162 2022-02-14 16:31:39.000000 higlass-widget-0.0.7/higlass_widget/labextension/static/618.9fc8f4669a3ff7344ddf.js
--rw-r--r--   0 hms-manzt   (501) staff       (20)     3907 2022-02-14 16:31:39.000000 higlass-widget-0.0.7/higlass_widget/labextension/static/618.9fc8f4669a3ff7344ddf.js.LICENSE.txt
--rw-r--r--   0 hms-manzt   (501) staff       (20)     1762 2022-02-14 16:31:39.000000 higlass-widget-0.0.7/higlass_widget/labextension/static/879.a5ae6335efd6d11cd011.js
--rw-r--r--   0 hms-manzt   (501) staff       (20)  5665665 2022-02-14 16:31:39.000000 higlass-widget-0.0.7/higlass_widget/labextension/static/949.0fb376ad87cced53c7dc.js
--rw-r--r--   0 hms-manzt   (501) staff       (20)   215757 2022-02-14 16:31:39.000000 higlass-widget-0.0.7/higlass_widget/labextension/static/949.0fb376ad87cced53c7dc.js.LICENSE.txt
--rw-r--r--   0 hms-manzt   (501) staff       (20)    45826 2022-02-14 16:31:39.000000 higlass-widget-0.0.7/higlass_widget/labextension/static/995.33c7510154ea3a82518c.js
--rw-r--r--   0 hms-manzt   (501) staff       (20)     7438 2022-02-14 16:31:39.000000 higlass-widget-0.0.7/higlass_widget/labextension/static/remoteEntry.19c085e09e0bbe3f5457.js
--rw-r--r--   0 hms-manzt   (501) staff       (20)      118 2022-02-14 16:31:34.000000 higlass-widget-0.0.7/higlass_widget/labextension/static/style.js
--rw-r--r--   0 hms-manzt   (501) staff       (20)    58060 2022-02-14 16:31:39.000000 higlass-widget-0.0.7/higlass_widget/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 hms-manzt   (501) staff       (20)        0 2022-02-14 17:26:09.295327 higlass-widget-0.0.7/higlass_widget/nbextension/
--rw-r--r--   0 hms-manzt   (501) staff       (20)      345 2022-02-12 16:02:27.000000 higlass-widget-0.0.7/higlass_widget/nbextension/extension.js
--rw-r--r--   0 hms-manzt   (501) staff       (20)  6163959 2022-02-14 16:31:33.000000 higlass-widget-0.0.7/higlass_widget/nbextension/index.js
--rw-r--r--   0 hms-manzt   (501) staff       (20)     1233 2022-02-13 17:53:16.000000 higlass-widget-0.0.7/higlass_widget/widget.py
-drwxr-xr-x   0 hms-manzt   (501) staff       (20)        0 2022-02-14 17:26:09.282734 higlass-widget-0.0.7/higlass_widget.egg-info/
--rw-r--r--   0 hms-manzt   (501) staff       (20)     1557 2022-02-14 17:26:09.000000 higlass-widget-0.0.7/higlass_widget.egg-info/PKG-INFO
--rw-r--r--   0 hms-manzt   (501) staff       (20)     1179 2022-02-14 17:26:09.000000 higlass-widget-0.0.7/higlass_widget.egg-info/SOURCES.txt
--rw-r--r--   0 hms-manzt   (501) staff       (20)        1 2022-02-14 17:26:09.000000 higlass-widget-0.0.7/higlass_widget.egg-info/dependency_links.txt
--rw-r--r--   0 hms-manzt   (501) staff       (20)       11 2022-02-14 17:26:09.000000 higlass-widget-0.0.7/higlass_widget.egg-info/requires.txt
--rw-r--r--   0 hms-manzt   (501) staff       (20)       15 2022-02-14 17:26:09.000000 higlass-widget-0.0.7/higlass_widget.egg-info/top_level.txt
--rw-r--r--   0 hms-manzt   (501) staff       (20)   668369 2022-02-14 16:31:01.000000 higlass-widget-0.0.7/package-lock.json
--rw-r--r--   0 hms-manzt   (501) staff       (20)     1162 2022-02-14 16:31:01.000000 higlass-widget-0.0.7/package.json
--rw-r--r--   0 hms-manzt   (501) staff       (20)      116 2022-02-12 19:16:13.000000 higlass-widget-0.0.7/pyproject.toml
--rw-r--r--   0 hms-manzt   (501) staff       (20)      506 2022-02-14 17:26:09.304036 higlass-widget-0.0.7/setup.cfg
--rw-r--r--   0 hms-manzt   (501) staff       (20)     1124 2022-02-13 02:37:31.000000 higlass-widget-0.0.7/setup.py
-drwxr-xr-x   0 hms-manzt   (501) staff       (20)        0 2022-02-14 17:26:09.303123 higlass-widget-0.0.7/src/
--rw-r--r--   0 hms-manzt   (501) staff       (20)      531 2022-02-13 16:12:52.000000 higlass-widget-0.0.7/src/plugin.js
--rw-r--r--   0 hms-manzt   (501) staff       (20)     1830 2022-02-14 06:18:57.000000 higlass-widget-0.0.7/src/widget.js
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/higlass_widget/__init__.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/higlass_widget/widget.js
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/higlass_widget/widget.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/notebooks/Widget.ipynb
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 higlass_widget-0.1.0/PKG-INFO
```

### Comparing `higlass-widget-0.0.7/LICENSE` & `higlass_widget-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `higlass-widget-0.0.7/PKG-INFO` & `higlass_widget-0.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,43 @@
-Metadata-Version: 2.1
-Name: higlass-widget
-Version: 0.0.7
-Summary: A Jupyter Widget for HiGlass
-Home-page: https://github.com/higlass/higlass-widget
-Author: Trevor Manz
-Author-email: trevor.j.manz@gmail.com
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # higlass-widget
 
 [![PyPI](https://img.shields.io/pypi/v/higlass-widget.svg?color=green)](https://pypi.org/project/higlass-widget)
 [![License](https://img.shields.io/pypi/l/gosling.svg?color=green)](https://github.com/higlass/higlass-widget/raw/main/LICENSE)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/higlass/higlass-widget/blob/main/notebooks/Widget.ipynb)
 
-
 ```
 pip install higlass-widget
 ```
 
 ### Development
 
-```bash
-pip install -e .
-```
-
-If you are using the classic Jupyter Notebook you need to install the nbextension:
+This project uses [`hatch`](https://github.com/pypa/hatch), which installs and sync
+all dependencies from `pyproject.toml` automatically.
 
-```bash
-jupyter nbextension install --py --symlink --sys-prefix higlass_widget
-jupyter nbextension enable --py --sys-prefix higlass_widget
+```sh
+hatch shell
 ```
 
-Note for developers:
+Alternatively, you can create and manage your own virtual environments and install
+an editable version of `higlass-widget`:
 
-- the `-e` pip option allows one to modify the Python code in-place. Restart the kernel in order to see the changes.
-- the `--symlink` argument on Linux or OS X allows one to modify the JavaScript code in-place. This feature is not available with Windows.
+```sh
+pip install -e ".[dev]"
+```
 
-For developing with JupyterLab:
+Finally, you can now run the notebooks with:
 
-```
-jupyter labextension develop --overwrite higlass_widget
+```sh
+jupyterlab
 ```
 
+`higlass_widget.HiGlassWidget` is built with [`anywidget`](https://github.com/manzt/anywidget).
+You can edit the contents of `higlass_widget/widget.js` and changes will be reflected automatically
+in your active Jupyter notebook.
 
 ### Release
 
 ```
 npm version [major|minor|patch]
 git tag -a vX.X.X -m "vX.X.X"
 git push --follow-tags
 ```
-
-
```

