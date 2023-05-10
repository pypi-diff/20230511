# Comparing `tmp/sphinx_probs_rdf-0.4.1.tar.gz` & `tmp/sphinx_probs_rdf-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_probs_rdf-0.4.1.tar", last modified: Thu May  4 19:57:58 2023, max compression
+gzip compressed data, was "sphinx_probs_rdf-0.4.2.tar", last modified: Wed May 10 23:00:33 2023, max compression
```

## Comparing `sphinx_probs_rdf-0.4.1.tar` & `sphinx_probs_rdf-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-04 19:57:58.970972 sphinx_probs_rdf-0.4.1/
--rw-r--r--   0 rcl38      (502) staff       (20)     1078 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/LICENSE
--rw-r--r--   0 rcl38      (502) staff       (20)       50 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/MANIFEST.in
--rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-05-04 19:57:58.971308 sphinx_probs_rdf-0.4.1/PKG-INFO
--rw-r--r--   0 rcl38      (502) staff       (20)      485 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/README.rst
--rw-r--r--   0 rcl38      (502) staff       (20)      357 2023-05-04 19:57:58.981897 sphinx_probs_rdf-0.4.1/setup.cfg
--rw-r--r--   0 rcl38      (502) staff       (20)     1718 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/setup.py
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-04 19:57:58.879456 sphinx_probs_rdf-0.4.1/src/
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-04 19:57:58.892973 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/
--rw-r--r--   0 rcl38      (502) staff       (20)     5019 2023-05-04 19:48:17.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/__init__.py
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-04 19:57:58.908862 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/_static/
--rw-r--r--   0 rcl38      (502) staff       (20)     2007 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/_static/system-definitions.css
--rw-r--r--   0 rcl38      (502) staff       (20)     1236 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/builder.py
--rw-r--r--   0 rcl38      (502) staff       (20)    30726 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/directives.py
--rw-r--r--   0 rcl38      (502) staff       (20)     1106 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/postprocess.py
--rw-r--r--   0 rcl38      (502) staff       (20)     7867 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/resolve.py
--rw-r--r--   0 rcl38      (502) staff       (20)       27 2023-05-04 19:56:17.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/version.py
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-04 19:57:58.903427 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/
--rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-05-04 19:57:58.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/PKG-INFO
--rw-r--r--   0 rcl38      (502) staff       (20)      805 2023-05-04 19:57:58.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/SOURCES.txt
--rw-r--r--   0 rcl38      (502) staff       (20)        1 2023-05-04 19:57:58.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/dependency_links.txt
--rw-r--r--   0 rcl38      (502) staff       (20)        1 2022-09-21 10:32:32.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/not-zip-safe
--rw-r--r--   0 rcl38      (502) staff       (20)       71 2023-05-04 19:57:58.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/requires.txt
--rw-r--r--   0 rcl38      (502) staff       (20)       17 2023-05-04 19:57:58.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/top_level.txt
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-04 19:57:58.965264 sphinx_probs_rdf-0.4.1/tests/
--rw-r--r--   0 rcl38      (502) staff       (20)     2843 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/tests/test_directive_options.py
--rw-r--r--   0 rcl38      (502) staff       (20)      661 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/tests/test_missing_process.py
--rw-r--r--   0 rcl38      (502) staff       (20)      892 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/tests/test_postprocess.py
--rw-r--r--   0 rcl38      (502) staff       (20)     1360 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/tests/test_probs_rdf_builder_basic.py
--rw-r--r--   0 rcl38      (502) staff       (20)     3989 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.1/tests/test_probs_rdf_builder_myst.py
--rw-r--r--   0 rcl38      (502) staff       (20)     1204 2023-03-08 21:16:17.000000 sphinx_probs_rdf-0.4.1/tests/test_probs_rdf_builder_prefixes.py
--rw-r--r--   0 rcl38      (502) staff       (20)      848 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.1/tests/test_probs_system_directives.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-10 23:00:33.542753 sphinx_probs_rdf-0.4.2/
+-rw-r--r--   0 rcl38      (502) staff       (20)     1078 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/LICENSE
+-rw-r--r--   0 rcl38      (502) staff       (20)       50 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/MANIFEST.in
+-rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-05-10 23:00:33.542877 sphinx_probs_rdf-0.4.2/PKG-INFO
+-rw-r--r--   0 rcl38      (502) staff       (20)      485 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/README.rst
+-rw-r--r--   0 rcl38      (502) staff       (20)      357 2023-05-10 23:00:33.543872 sphinx_probs_rdf-0.4.2/setup.cfg
+-rw-r--r--   0 rcl38      (502) staff       (20)     1718 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/setup.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-10 23:00:33.415589 sphinx_probs_rdf-0.4.2/src/
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-10 23:00:33.484474 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/
+-rw-r--r--   0 rcl38      (502) staff       (20)     5539 2023-05-08 07:12:14.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/__init__.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-10 23:00:33.495337 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/_static/
+-rw-r--r--   0 rcl38      (502) staff       (20)     2007 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/_static/system-definitions.css
+-rw-r--r--   0 rcl38      (502) staff       (20)     1236 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/builder.py
+-rw-r--r--   0 rcl38      (502) staff       (20)    30726 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/directives.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     1106 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/postprocess.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     7867 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/resolve.py
+-rw-r--r--   0 rcl38      (502) staff       (20)       27 2023-05-10 22:59:13.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/version.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-10 23:00:33.490803 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/
+-rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-05-10 23:00:33.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/PKG-INFO
+-rw-r--r--   0 rcl38      (502) staff       (20)      805 2023-05-10 23:00:33.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 rcl38      (502) staff       (20)        1 2023-05-10 23:00:33.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 rcl38      (502) staff       (20)        1 2022-09-21 10:32:32.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/not-zip-safe
+-rw-r--r--   0 rcl38      (502) staff       (20)       71 2023-05-10 23:00:33.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/requires.txt
+-rw-r--r--   0 rcl38      (502) staff       (20)       17 2023-05-10 23:00:33.000000 sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/top_level.txt
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-10 23:00:33.542340 sphinx_probs_rdf-0.4.2/tests/
+-rw-r--r--   0 rcl38      (502) staff       (20)     2843 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/tests/test_directive_options.py
+-rw-r--r--   0 rcl38      (502) staff       (20)      661 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/tests/test_missing_process.py
+-rw-r--r--   0 rcl38      (502) staff       (20)      892 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/tests/test_postprocess.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     1360 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.2/tests/test_probs_rdf_builder_basic.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     3989 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.2/tests/test_probs_rdf_builder_myst.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     1204 2023-03-08 21:16:17.000000 sphinx_probs_rdf-0.4.2/tests/test_probs_rdf_builder_prefixes.py
+-rw-r--r--   0 rcl38      (502) staff       (20)      848 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.2/tests/test_probs_system_directives.py
```

### Comparing `sphinx_probs_rdf-0.4.1/LICENSE` & `sphinx_probs_rdf-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/PKG-INFO` & `sphinx_probs_rdf-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_probs_rdf
-Version: 0.4.1
+Version: 0.4.2
 Summary: sphinx_probs_rdf is a sphinx extension which outputs RDF describing Processes and Objects using the PRObs ontology.
 Home-page: https://github.com/ricklupton/sphinx_probs_rdf
 Download-URL: https://pypi.org/project/sphinx_probs_rdf/
 Author: Rick Lupton
 Author-email: mail@ricklupton.name
 License: BSD
 Platform: any
```

### Comparing `sphinx_probs_rdf-0.4.1/setup.py` & `sphinx_probs_rdf-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/__init__.py` & `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,35 @@
     EndSubObjectsDirective,
     TTL,
     ObjectEquivalentTo,
 )
 from .resolve import ProbsTransform
 
 
+# Old version
 NB_RENDER_PRIORITY = {
     "probs_rdf": (
         "application/vnd.jupyter.widget-view+json",
         "application/javascript",
         "text/html",
         "image/svg+xml",
         "image/png",
         "image/jpeg",
         "text/markdown",
         "text/latex",
         "text/plain",
     )
 }
 
+NB_RENDER_PRIORITY_NEW = [
+    (k, v, (1 + i) * 10)
+    for k, items in NB_RENDER_PRIORITY.items()
+    for i, v in enumerate(items)
+]
+
 
 
 def copy_custom_files(app, exc):
     if app.builder.format == 'html' and not exc:
         staticdir = path.join(app.builder.outdir, '_static')
         here = path.dirname(__file__)
         copy_asset_file(path.join(here, '_static/system-definitions.css'), staticdir)
@@ -114,18 +121,26 @@
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     app.add_builder(ProbsSystemRDFBuilder)
     # Add config for jupyter-book / myst_nb.
     # See https://jupyterbook.org/advanced/advanced.html#enabling-a-custom-builder
     # -using-jupyter-book
-    if "nb_render_priority" in app.config:
+    #
+    # Older version -- kept for compatibility with myst-nb<0.14 for now
+    if (
+        "nb_render_priority" in app.config
+        and app.config["nb_render_priority"] != "--unset--"
+    ):
         app.config["nb_render_priority"]["probs_rdf"] = NB_RENDER_PRIORITY["probs_rdf"]
+    elif "nb_mime_priority_overrides" in app.config:
+        app.config["nb_mime_priority_overrides"] = NB_RENDER_PRIORITY_NEW
     else:
         app.add_config_value("nb_render_priority", NB_RENDER_PRIORITY, "probs_rdf")
+        app.add_config_value("nb_mime_priority_overrides", NB_RENDER_PRIORITY_NEW, "env")
 
     app.add_domain(SystemDomain)
 
     app.add_directive("start-sub-processes", StartSubProcessesDirective)
     app.add_directive("start-sub-objects", StartSubObjectsDirective)
     app.add_directive("end-sub-processes", EndSubProcessesDirective)
     app.add_directive("end-sub-objects", EndSubObjectsDirective)
```

### Comparing `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/_static/system-definitions.css` & `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/_static/system-definitions.css`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/builder.py` & `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/builder.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/directives.py` & `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/directives.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/postprocess.py` & `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/postprocess.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/resolve.py` & `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf/resolve.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/PKG-INFO` & `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-probs-rdf
-Version: 0.4.1
+Version: 0.4.2
 Summary: sphinx_probs_rdf is a sphinx extension which outputs RDF describing Processes and Objects using the PRObs ontology.
 Home-page: https://github.com/ricklupton/sphinx_probs_rdf
 Download-URL: https://pypi.org/project/sphinx_probs_rdf/
 Author: Rick Lupton
 Author-email: mail@ricklupton.name
 License: BSD
 Platform: any
```

### Comparing `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/SOURCES.txt` & `sphinx_probs_rdf-0.4.2/src/sphinx_probs_rdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/tests/test_directive_options.py` & `sphinx_probs_rdf-0.4.2/tests/test_directive_options.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/tests/test_missing_process.py` & `sphinx_probs_rdf-0.4.2/tests/test_missing_process.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/tests/test_postprocess.py` & `sphinx_probs_rdf-0.4.2/tests/test_postprocess.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/tests/test_probs_rdf_builder_basic.py` & `sphinx_probs_rdf-0.4.2/tests/test_probs_rdf_builder_basic.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/tests/test_probs_rdf_builder_myst.py` & `sphinx_probs_rdf-0.4.2/tests/test_probs_rdf_builder_myst.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/tests/test_probs_rdf_builder_prefixes.py` & `sphinx_probs_rdf-0.4.2/tests/test_probs_rdf_builder_prefixes.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.1/tests/test_probs_system_directives.py` & `sphinx_probs_rdf-0.4.2/tests/test_probs_system_directives.py`

 * *Files identical despite different names*

