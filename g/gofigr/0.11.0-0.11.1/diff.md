# Comparing `tmp/gofigr-0.11.0.tar.gz` & `tmp/gofigr-0.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gofigr-0.11.0.tar", last modified: Tue May  9 19:07:11 2023, max compression
+gzip compressed data, was "gofigr-0.11.1.tar", last modified: Thu May 11 18:41:37 2023, max compression
```

## Comparing `gofigr-0.11.0.tar` & `gofigr-0.11.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 19:07:11.155597 gofigr-0.11.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-05-09 18:47:57.000000 gofigr-0.11.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-05-09 18:47:57.000000 gofigr-0.11.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-05-09 19:07:11.155597 gofigr-0.11.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6023 2023-05-09 18:47:57.000000 gofigr-0.11.0/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 19:07:11.151597 gofigr-0.11.0/gofigr/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12625 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4991 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/gfconfig.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18303 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/jupyter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42702 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/models.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 19:07:11.155597 gofigr-0.11.0/gofigr/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   584424 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/resources/FreeMono.ttf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3097 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/watermarks.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 19:07:11.155597 gofigr-0.11.0/gofigr.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-05-09 19:07:11.000000 gofigr-0.11.0/gofigr.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-05-09 19:07:11.000000 gofigr-0.11.0/gofigr.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-09 19:07:11.000000 gofigr-0.11.0/gofigr.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-05-09 19:07:11.000000 gofigr-0.11.0/gofigr.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2023-05-09 19:07:11.000000 gofigr-0.11.0/gofigr.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-05-09 19:07:11.000000 gofigr-0.11.0/gofigr.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1546 2023-05-09 18:47:57.000000 gofigr-0.11.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-09 19:07:11.155597 gofigr-0.11.0/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 19:07:11.155597 gofigr-0.11.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40823 2023-05-09 18:47:57.000000 gofigr-0.11.0/tests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1967 2023-05-09 18:47:57.000000 gofigr-0.11.0/tests/test_logs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-05-09 18:47:57.000000 gofigr-0.11.0/tests/test_models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1007 2023-05-09 18:47:57.000000 gofigr-0.11.0/tests/test_watermarks.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 18:41:37.333640 gofigr-0.11.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-05-11 18:22:11.000000 gofigr-0.11.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-05-11 18:22:11.000000 gofigr-0.11.1/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-05-11 18:41:37.333640 gofigr-0.11.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6023 2023-05-11 18:22:11.000000 gofigr-0.11.1/README.rst
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 18:41:37.333640 gofigr-0.11.1/gofigr/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12765 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4991 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/gfconfig.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18524 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/jupyter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42702 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/models.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 18:41:37.333640 gofigr-0.11.1/gofigr/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   584424 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/resources/FreeMono.ttf
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3097 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/watermarks.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 18:41:37.333640 gofigr-0.11.1/gofigr.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-05-11 18:41:37.000000 gofigr-0.11.1/gofigr.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-05-11 18:41:37.000000 gofigr-0.11.1/gofigr.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-11 18:41:37.000000 gofigr-0.11.1/gofigr.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-05-11 18:41:37.000000 gofigr-0.11.1/gofigr.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2023-05-11 18:41:37.000000 gofigr-0.11.1/gofigr.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-05-11 18:41:37.000000 gofigr-0.11.1/gofigr.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1546 2023-05-11 18:22:11.000000 gofigr-0.11.1/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-11 18:41:37.333640 gofigr-0.11.1/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 18:41:37.333640 gofigr-0.11.1/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40823 2023-05-11 18:22:11.000000 gofigr-0.11.1/tests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1967 2023-05-11 18:22:11.000000 gofigr-0.11.1/tests/test_logs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-05-11 18:22:11.000000 gofigr-0.11.1/tests/test_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1007 2023-05-11 18:22:11.000000 gofigr-0.11.1/tests/test_watermarks.py
```

### Comparing `gofigr-0.11.0/LICENSE` & `gofigr-0.11.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.0/PKG-INFO` & `gofigr-0.11.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gofigr
-Version: 0.11.0
+Version: 0.11.1
 Summary: GoFigr client library
 Author-email: Maciej Pacula <maciej@gofigr.io>
 License: Copyright 2022-2023 Flagstaff Solutions, LLC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
         the Software without restriction, including without limitation the rights to
@@ -20,28 +20,28 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://www.gofigr.io
-Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.11.0/
+Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.11.1/
 Keywords: science,visualization,version control,plotting,data,reproducibility
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.11.0)
+GoFigr - Python Client (0.11.1)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.11.0/README.rst` & `gofigr-0.11.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.11.0)
+GoFigr - Python Client (0.11.1)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.11.0/gofigr/__init__.py` & `gofigr-0.11.1/gofigr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,14 +145,19 @@
         self._refresh_token = None
 
         if authenticate:
             self.authenticate()
 
         self._bind_models()
 
+    @property
+    def app_url(self):
+        """Returns the URL to the GoFigr app"""
+        return self.service_url.replace("api", "app")
+
     def _bind_models(self):
         """\
         Create instance-bound model classes, e.g. Workspace, Figure, etc. Each will internally
         store a reference to this GoFigr client -- that way we don't have to pass it around.
 
         :return: None
         """
```

### Comparing `gofigr-0.11.0/gofigr/gfconfig.py` & `gofigr-0.11.1/gofigr/gfconfig.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.0/gofigr/jupyter.py` & `gofigr-0.11.1/gofigr/jupyter.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import PIL
 import ipynbname
 import matplotlib.pyplot as plt
 import six
 from IPython.core.display_functions import display
 
-from gofigr import GoFigr, CodeLanguage, API_URL, APP_URL
+from gofigr import GoFigr, CodeLanguage, API_URL
 from gofigr.watermarks import DefaultWatermark
 
 
 class _GoFigrExtension:
     """\
     Implements the main Jupyter extension functionality. You will not want to instantiate this class directly.
     Instead, please refer to the _GF_EXTENSION singleton.
@@ -263,15 +263,15 @@
     return bio.read()
 
 
 class Publisher:
     """\
     Publishes revisions to the GoFigr server.
     """
-    def __init__(self, gf, watermark=None, annotators=DEFAULT_ANNOTATORS, image_formats=("png", "eps"),
+    def __init__(self, gf, watermark=None, annotators=DEFAULT_ANNOTATORS, image_formats=("png", "eps", "svg"),
                  default_metadata=None, clear=True):
         """
 
         :param gf: GoFigr instance
         :param watermark: watermark generator, e.g. QRWatermark()
         :param annotators: revision annotators
         :param image_formats: image formats to save by default
@@ -352,30 +352,33 @@
 
         # Create a bare revision first to get the API ID
         rev = gf.Revision(figure=target, metadata=combined_meta)
         target.revisions.create(rev)
 
         image_data = []
         for fmt in self.image_formats:
-            img = PIL.Image.open(io.BytesIO(figure_to_bytes(fig, fmt)))
-            img.load()
-
-            watermarked_img = self.watermark.apply(img, rev)
+            if fmt.lower() == "png":
+                img = PIL.Image.open(io.BytesIO(figure_to_bytes(fig, fmt)))
+                img.load()
+                watermarked_img = self.watermark.apply(img, rev)
+            else:
+                watermarked_img = None
 
             # First, save the image without the watermark
             image_data.append(gf.ImageData(name="figure", format=fmt, data=figure_to_bytes(fig, fmt),
                                            is_watermarked=False))
 
-            # Now, save the watermarked version
-            bio = io.BytesIO()
-            watermarked_img.save(bio, format=fmt)
-            image_data.append(gf.ImageData(name="figure", format=fmt, data=bio.getvalue(),
-                                           is_watermarked=True))
+            # Now, save the watermarked version (if available)
+            if watermarked_img is not None:
+                bio = io.BytesIO()
+                watermarked_img.save(bio, format=fmt)
+                image_data.append(gf.ImageData(name="figure", format=fmt, data=bio.getvalue(),
+                                               is_watermarked=True))
 
-            if fmt == 'png':
+            if fmt.lower() == 'png' and watermarked_img is not None:
                 display(watermarked_img)
 
         rev.image_data = image_data
 
         if dataframes is not None:
             table_data = []
             for name, frame in dataframes.items():
@@ -390,15 +393,15 @@
         rev.save(silent=True)
 
         fig._gf_is_published = True
 
         if self.clear:
             plt.close(fig)
 
-        print(f"{APP_URL}/r/{rev.api_id}")
+        print(f"{gf.app_url}/r/{rev.api_id}")
 
         return rev if return_revision else None
 
 
 def from_config_or_env(env_prefix, config_path):
     """\
     Decorator that binds function arguments in order of priority (most important first):
```

### Comparing `gofigr-0.11.0/gofigr/models.py` & `gofigr-0.11.1/gofigr/models.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.0/gofigr/resources/FreeMono.ttf` & `gofigr-0.11.1/gofigr/resources/FreeMono.ttf`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.0/gofigr/watermarks.py` & `gofigr-0.11.1/gofigr/watermarks.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.0/gofigr.egg-info/PKG-INFO` & `gofigr-0.11.1/gofigr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gofigr
-Version: 0.11.0
+Version: 0.11.1
 Summary: GoFigr client library
 Author-email: Maciej Pacula <maciej@gofigr.io>
 License: Copyright 2022-2023 Flagstaff Solutions, LLC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
         the Software without restriction, including without limitation the rights to
@@ -20,28 +20,28 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://www.gofigr.io
-Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.11.0/
+Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.11.1/
 Keywords: science,visualization,version control,plotting,data,reproducibility
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.11.0)
+GoFigr - Python Client (0.11.1)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.11.0/pyproject.toml` & `gofigr-0.11.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gofigr"
-version = "0.11.0"
+version = "0.11.1"
 description = "GoFigr client library"
 readme = "README.rst"
 authors = [{ name = "Maciej Pacula", email = "maciej@gofigr.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -24,21 +24,21 @@
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "bumpver", "build", "twine", "pylint", "flake8", "sphinx", "sphinx_rtd_theme", "sphinxcontrib-jquery"]
 
 [project.urls]
 Homepage = "https://www.gofigr.io"
-Documentation = "https://gofigr.io/docs/gofigr-python/0.11.0/"
+Documentation = "https://gofigr.io/docs/gofigr-python/0.11.1/"
 
 [project.scripts]
 gfconfig = "gofigr.gfconfig:main"
 
 [tool.bumpver]
-current_version = "0.11.0"
+current_version = "0.11.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gofigr-0.11.0/tests/test_client.py` & `gofigr-0.11.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.0/tests/test_logs.py` & `gofigr-0.11.1/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.0/tests/test_models.py` & `gofigr-0.11.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.0/tests/test_watermarks.py` & `gofigr-0.11.1/tests/test_watermarks.py`

 * *Files identical despite different names*

