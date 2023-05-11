# Comparing `tmp/imaxt-multiscale-plugin-0.2.5.tar.gz` & `tmp/imaxt-multiscale-plugin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaxt-multiscale-plugin-0.2.5.tar", last modified: Thu May 11 10:24:24 2023, max compression
+gzip compressed data, was "imaxt-multiscale-plugin-0.3.0.tar", last modified: Thu May 11 10:24:24 2023, max compression
```

## Comparing `imaxt-multiscale-plugin-0.2.5.tar` & `imaxt-multiscale-plugin-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.455643 imaxt-multiscale-plugin-0.2.5/
--rw-rw-rw-   0 root         (0) root         (0)     7653 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3880 2023-05-11 10:24:24.455643 imaxt-multiscale-plugin-0.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2855 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1761 2023-05-11 10:24:24.456643 imaxt-multiscale-plugin-0.2.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.453643 imaxt-multiscale-plugin-0.2.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.454643 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4422 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_reader.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_sample_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.455643 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_tests/test_reader.py
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_tests/test_sample_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_tests/test_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_tests/test_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     1990 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     2449 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/napari.yaml
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.455643 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3880 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      892 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.868656 imaxt-multiscale-plugin-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7653 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-05-11 10:24:24.868656 imaxt-multiscale-plugin-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1748 2023-05-11 10:24:24.868656 imaxt-multiscale-plugin-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.865656 imaxt-multiscale-plugin-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.867656 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_sample_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.868656 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/test_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/test_sample_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/test_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/test_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1990 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/napari.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-05-11 10:24:10.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:24:24.867656 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      926 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-11 10:24:24.000000 imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/top_level.txt
```

### Comparing `imaxt-multiscale-plugin-0.2.5/LICENSE` & `imaxt-multiscale-plugin-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.5/PKG-INFO` & `imaxt-multiscale-plugin-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaxt-multiscale-plugin
-Version: 0.2.5
+Version: 0.3.0
 Summary: A simple plugin to use with napari
 Home-page: https://gitlab.developers.cam.ac.uk/astronomy/camcead/imaxt/imaxt-multiscale-plugin
 Author: Eduardo Gonzalez Solares
 Author-email: E.GonzalezSolares@ast.cam.ac.uk
 License: LGPL-3.0-only
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `imaxt-multiscale-plugin-0.2.5/README.md` & `imaxt-multiscale-plugin-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.5/setup.cfg` & `imaxt-multiscale-plugin-0.3.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.5
+current_version = 0.3.0
 commit = True
 tag = True
 
 [metadata]
 name = imaxt-multiscale-plugin
 version = attr:imaxt_multiscale_plugin.__version__
 description = A simple plugin to use with napari
@@ -30,15 +30,14 @@
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	magicgui
 	qtpy
-	imaxt-image
 	xarray
 	dask
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
```

### Comparing `imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_reader.py` & `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 import zarr
 
 from .utils import get_display_range
 
 
 def get_store_from_path(path):
     if path.startswith("s3://"):
-        from imaxt_image.io.s3 import get_s3_store
+        from .s3 import get_s3_store
 
-        _, alias, instrument, name = Path(path).parts
+        _, alias, *opath = Path(path).parts
+        opath = '/'.join(opath)
         store = None
         for extra in ["mos", "mos.zarr"]:  # v0.9 of pipeline
             with suppress(PermissionError):
-                store = get_s3_store(name, alias, instrument, extra)
+                store = get_s3_store(alias, f"/{opath}/{extra}")
             if store is not None:
                 break
     else:
         path = Path(path)
         if (path / "mos").exists():
             store = path / "mos"
         else:
```

### Comparing `imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_tests/test_reader.py` & `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_tests/test_widget.py` & `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_widget.py` & `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_widget.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/_writer.py` & `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/_writer.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/napari.yaml` & `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/napari.yaml`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin/utils.py` & `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin.egg-info/PKG-INFO` & `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaxt-multiscale-plugin
-Version: 0.2.5
+Version: 0.3.0
 Summary: A simple plugin to use with napari
 Home-page: https://gitlab.developers.cam.ac.uk/astronomy/camcead/imaxt/imaxt-multiscale-plugin
 Author: Eduardo Gonzalez Solares
 Author-email: E.GonzalezSolares@ast.cam.ac.uk
 License: LGPL-3.0-only
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `imaxt-multiscale-plugin-0.2.5/src/imaxt_multiscale_plugin.egg-info/SOURCES.txt` & `imaxt-multiscale-plugin-0.3.0/src/imaxt_multiscale_plugin.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 src/imaxt_multiscale_plugin/__init__.py
 src/imaxt_multiscale_plugin/_reader.py
 src/imaxt_multiscale_plugin/_sample_data.py
 src/imaxt_multiscale_plugin/_widget.py
 src/imaxt_multiscale_plugin/_writer.py
 src/imaxt_multiscale_plugin/napari.yaml
+src/imaxt_multiscale_plugin/s3.py
 src/imaxt_multiscale_plugin/utils.py
 src/imaxt_multiscale_plugin.egg-info/PKG-INFO
 src/imaxt_multiscale_plugin.egg-info/SOURCES.txt
 src/imaxt_multiscale_plugin.egg-info/dependency_links.txt
 src/imaxt_multiscale_plugin.egg-info/entry_points.txt
 src/imaxt_multiscale_plugin.egg-info/requires.txt
 src/imaxt_multiscale_plugin.egg-info/top_level.txt
```

