# Comparing `tmp/colortextpy-0.0.1.tar.gz` & `tmp/colortextpy-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colortextpy-0.0.1.tar", last modified: Sun May  7 09:34:51 2023, max compression
+gzip compressed data, was "colortextpy-0.0.1.1.tar", last modified: Wed May 10 18:54:10 2023, max compression
```

## Comparing `colortextpy-0.0.1.tar` & `colortextpy-0.0.1.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-07 09:34:51.584944 colortextpy-0.0.1/
--rwxrwxrwx   0 ping      (1000) ping      (1000)     1063 2023-05-05 08:00:54.000000 colortextpy-0.0.1/LICENSE
--rwxrwxrwx   0 ping      (1000) ping      (1000)      111 2023-04-27 10:12:58.000000 colortextpy-0.0.1/MANIFEST.in
--rwxrwxrwx   0 ping      (1000) ping      (1000)     1265 2023-05-07 09:34:51.570940 colortextpy-0.0.1/PKG-INFO
--rwxrwxrwx   0 ping      (1000) ping      (1000)      363 2023-05-07 08:43:23.000000 colortextpy-0.0.1/README.md
-drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-07 09:34:50.929507 colortextpy-0.0.1/colortextpy/
--rwxrwxrwx   0 ping      (1000) ping      (1000)       22 2023-05-07 09:05:11.000000 colortextpy-0.0.1/colortextpy/__init__.py
--rwxrwxrwx   0 ping      (1000) ping      (1000)     1629 2023-05-07 09:05:11.000000 colortextpy-0.0.1/colortextpy/_modidx.py
--rwxrwxrwx   0 ping      (1000) ping      (1000)    12160 2023-05-07 09:05:11.000000 colortextpy-0.0.1/colortextpy/color.py
-drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-07 09:34:51.379941 colortextpy-0.0.1/colortextpy.egg-info/
--rwxrwxrwx   0 ping      (1000) ping      (1000)     1265 2023-05-07 09:34:49.000000 colortextpy-0.0.1/colortextpy.egg-info/PKG-INFO
--rwxrwxrwx   0 ping      (1000) ping      (1000)      365 2023-05-07 09:34:49.000000 colortextpy-0.0.1/colortextpy.egg-info/SOURCES.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)        1 2023-05-07 09:34:49.000000 colortextpy-0.0.1/colortextpy.egg-info/dependency_links.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)       44 2023-05-07 09:34:49.000000 colortextpy-0.0.1/colortextpy.egg-info/entry_points.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)        1 2023-05-06 16:09:06.000000 colortextpy-0.0.1/colortextpy.egg-info/not-zip-safe
--rwxrwxrwx   0 ping      (1000) ping      (1000)       27 2023-05-07 09:34:49.000000 colortextpy-0.0.1/colortextpy.egg-info/requires.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)       12 2023-05-07 09:34:49.000000 colortextpy-0.0.1/colortextpy.egg-info/top_level.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)     1085 2023-05-07 09:04:39.000000 colortextpy-0.0.1/settings.ini
--rwxrwxrwx   0 ping      (1000) ping      (1000)       38 2023-05-07 09:34:51.587944 colortextpy-0.0.1/setup.cfg
--rwxrwxrwx   0 ping      (1000) ping      (1000)     2596 2023-04-27 10:12:58.000000 colortextpy-0.0.1/setup.py
+drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-10 18:54:10.328167 colortextpy-0.0.1.1/
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     1063 2023-05-05 08:00:54.000000 colortextpy-0.0.1.1/LICENSE
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      111 2023-04-27 10:12:58.000000 colortextpy-0.0.1.1/MANIFEST.in
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     1267 2023-05-10 18:54:10.325667 colortextpy-0.0.1.1/PKG-INFO
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      363 2023-05-07 08:43:23.000000 colortextpy-0.0.1.1/README.md
+drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-10 18:54:10.189487 colortextpy-0.0.1.1/colortextpy/
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      114 2023-05-10 18:53:41.000000 colortextpy-0.0.1.1/colortextpy/__init__.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     9441 2023-05-10 18:52:42.000000 colortextpy-0.0.1.1/colortextpy/_modidx.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     3310 2023-05-10 18:52:41.000000 colortextpy-0.0.1.1/colortextpy/ansicolor.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)    12367 2023-05-10 18:52:41.000000 colortextpy-0.0.1.1/colortextpy/color.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     8022 2023-05-10 18:52:41.000000 colortextpy-0.0.1.1/colortextpy/colorize.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     1429 2023-05-10 18:52:41.000000 colortextpy-0.0.1.1/colortextpy/printer.py
+drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-10 18:54:10.309167 colortextpy-0.0.1.1/colortextpy.egg-info/
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     1267 2023-05-10 18:54:09.000000 colortextpy-0.0.1.1/colortextpy.egg-info/PKG-INFO
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      437 2023-05-10 18:54:09.000000 colortextpy-0.0.1.1/colortextpy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)        1 2023-05-10 18:54:09.000000 colortextpy-0.0.1.1/colortextpy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)       44 2023-05-10 18:54:09.000000 colortextpy-0.0.1.1/colortextpy.egg-info/entry_points.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)        1 2023-05-06 16:09:06.000000 colortextpy-0.0.1.1/colortextpy.egg-info/not-zip-safe
+-rwxrwxrwx   0 ping      (1000) ping      (1000)       27 2023-05-10 18:54:09.000000 colortextpy-0.0.1.1/colortextpy.egg-info/requires.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)       12 2023-05-10 18:54:09.000000 colortextpy-0.0.1.1/colortextpy.egg-info/top_level.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     1087 2023-05-10 18:54:07.000000 colortextpy-0.0.1.1/settings.ini
+-rwxrwxrwx   0 ping      (1000) ping      (1000)       38 2023-05-10 18:54:10.329167 colortextpy-0.0.1.1/setup.cfg
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     2596 2023-04-27 10:12:58.000000 colortextpy-0.0.1.1/setup.py
```

### Comparing `colortextpy-0.0.1/LICENSE` & `colortextpy-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `colortextpy-0.0.1/PKG-INFO` & `colortextpy-0.0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colortextpy
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Colortextpy is a Python package for adding colors and styles to terminal output, allowing you to create more visually appealing and organized command-line applications.
 Home-page: https://github.com/susuky/colortextpy
 Author: ping
 Author-email: hpisj322@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `colortextpy-0.0.1/colortextpy/color.py` & `colortextpy-0.0.1.1/colortextpy/color.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_color.ipynb.
 
 # %% auto 0
-__all__ = ['EnumMeta', 'Color']
+__all__ = ['Color', 'rgb2hex']
 
 # %% ../nbs/00_color.ipynb 3
 import enum
 
-__all__ = ['Color']
 
-class EnumMeta(enum.Enum):
+class _EnumMeta(enum.Enum):
     '''
     Add some custom members for `enum.Enum`
     '''
     def __repr__(self):
         return '<%s.%s>' % (self.__class__.__name__, self.name)
     
     def __str__(self):
@@ -24,15 +23,15 @@
     
     @classmethod
     @property
     def available(cls):
         return tuple(cls.__members__.keys())
 
 
-class Color(EnumMeta):
+class Color(_EnumMeta):
     '''
     Use enum.Enum to store color with **hex**, **rgb**, **bgr** format.
     '''
     aliceblue             = (  0, '#f0f8ff', (240, 248, 255), (255, 248, 240))
     antiquewhite          = (  1, '#faebd7', (250, 235, 215), (215, 235, 250))
     aqua                  = (  2, '#00ffff', (0, 255, 255), (255, 255, 0))
     aquamarine            = (  3, '#7fffd4', (127, 255, 212), (212, 255, 127))
@@ -193,7 +192,18 @@
     @property
     def bgr(self):
         return self._bgr
     
     @property
     def __contains__(cls, other):
         return other in cls.available
+
+# %% ../nbs/00_color.ipynb 10
+# def rgb2hex(*rgb) -> str:
+#     return '#{0:x}{1:x}{2:x}'.format(*rgb)
+
+
+def rgb2hex(r: int, g: int, b: int) -> str:
+    '''
+    convert rgb color to hex
+    '''
+    return f'#{r:x}{g:x}{b:x}'
```

### Comparing `colortextpy-0.0.1/colortextpy.egg-info/PKG-INFO` & `colortextpy-0.0.1.1/colortextpy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colortextpy
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Colortextpy is a Python package for adding colors and styles to terminal output, allowing you to create more visually appealing and organized command-line applications.
 Home-page: https://github.com/susuky/colortextpy
 Author: ping
 Author-email: hpisj322@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `colortextpy-0.0.1/settings.ini` & `colortextpy-0.0.1.1/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = colortextpy
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.1.1
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = colortextpy
```

### Comparing `colortextpy-0.0.1/setup.py` & `colortextpy-0.0.1.1/setup.py`

 * *Files identical despite different names*

