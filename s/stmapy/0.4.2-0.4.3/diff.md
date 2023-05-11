# Comparing `tmp/stmapy-0.4.2.tar.gz` & `tmp/stmapy-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stmapy-0.4.2.tar", last modified: Thu May 11 01:45:24 2023, max compression
+gzip compressed data, was "stmapy-0.4.3.tar", last modified: Thu May 11 04:25:37 2023, max compression
```

## Comparing `stmapy-0.4.2.tar` & `stmapy-0.4.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 florie    (1000) florie    (1000)        0 2023-05-11 01:45:24.848344 stmapy-0.4.2/
--rwxrwxr-x   0 florie    (1000) florie    (1000)     1068 2023-05-10 22:09:35.000000 stmapy-0.4.2/LICENSE
--rw-rw-r--   0 florie    (1000) florie    (1000)    11514 2023-05-11 01:45:24.848344 stmapy-0.4.2/PKG-INFO
--rwxrwxr-x   0 florie    (1000) florie    (1000)    10854 2023-05-10 22:09:35.000000 stmapy-0.4.2/README.md
--rw-rw-r--   0 florie    (1000) florie    (1000)       38 2023-05-11 01:45:24.848344 stmapy-0.4.2/setup.cfg
--rwxrwxr-x   0 florie    (1000) florie    (1000)     1285 2023-05-11 01:45:03.000000 stmapy-0.4.2/setup.py
-drwxrwxr-x   0 florie    (1000) florie    (1000)        0 2023-05-11 01:45:24.848344 stmapy-0.4.2/stmapy/
--rwxrwxr-x   0 florie    (1000) florie    (1000)      135 2023-05-10 22:09:35.000000 stmapy-0.4.2/stmapy/__init__.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)       22 2023-05-11 01:45:18.000000 stmapy-0.4.2/stmapy/_version.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)    61077 2023-05-10 22:09:35.000000 stmapy-0.4.2/stmapy/citswidget.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)      165 2023-05-10 22:09:35.000000 stmapy-0.4.2/stmapy/config.json
--rwxrwxr-x   0 florie    (1000) florie    (1000)      398 2023-05-10 22:09:35.000000 stmapy-0.4.2/stmapy/main.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)      312 2023-05-10 22:09:35.000000 stmapy-0.4.2/stmapy/matplotlibwidget.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)     3468 2023-05-10 22:09:35.000000 stmapy-0.4.2/stmapy/plotting.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)     9883 2023-05-10 22:09:35.000000 stmapy-0.4.2/stmapy/processing.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)    32334 2023-05-10 22:09:35.000000 stmapy-0.4.2/stmapy/reads.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)     5877 2023-05-10 22:09:35.000000 stmapy-0.4.2/stmapy/shape.py
--rwxrwxr-x   0 florie    (1000) florie    (1000)      814 2023-05-10 22:09:35.000000 stmapy-0.4.2/stmapy/stmapyStyle.mplstyle
--rwxrwxr-x   0 florie    (1000) florie    (1000)    38217 2023-05-10 22:09:35.000000 stmapy-0.4.2/stmapy/ui_citswidget.ui
-drwxrwxr-x   0 florie    (1000) florie    (1000)        0 2023-05-11 01:45:24.848344 stmapy-0.4.2/stmapy.egg-info/
--rw-rw-r--   0 florie    (1000) florie    (1000)    11514 2023-05-11 01:45:24.000000 stmapy-0.4.2/stmapy.egg-info/PKG-INFO
--rw-rw-r--   0 florie    (1000) florie    (1000)      452 2023-05-11 01:45:24.000000 stmapy-0.4.2/stmapy.egg-info/SOURCES.txt
--rw-rw-r--   0 florie    (1000) florie    (1000)        1 2023-05-11 01:45:24.000000 stmapy-0.4.2/stmapy.egg-info/dependency_links.txt
--rw-rw-r--   0 florie    (1000) florie    (1000)       44 2023-05-11 01:45:24.000000 stmapy-0.4.2/stmapy.egg-info/entry_points.txt
--rw-rw-r--   0 florie    (1000) florie    (1000)       40 2023-05-11 01:45:24.000000 stmapy-0.4.2/stmapy.egg-info/requires.txt
--rw-rw-r--   0 florie    (1000) florie    (1000)        7 2023-05-11 01:45:24.000000 stmapy-0.4.2/stmapy.egg-info/top_level.txt
+drwxrwxr-x   0 florie    (1000) florie    (1000)        0 2023-05-11 04:25:37.662757 stmapy-0.4.3/
+-rwxrwxr-x   0 florie    (1000) florie    (1000)     1068 2023-05-10 22:09:35.000000 stmapy-0.4.3/LICENSE
+-rw-rw-r--   0 florie    (1000) florie    (1000)    11514 2023-05-11 04:25:37.662757 stmapy-0.4.3/PKG-INFO
+-rwxrwxr-x   0 florie    (1000) florie    (1000)    10854 2023-05-10 22:09:35.000000 stmapy-0.4.3/README.md
+-rw-rw-r--   0 florie    (1000) florie    (1000)       38 2023-05-11 04:25:37.662757 stmapy-0.4.3/setup.cfg
+-rwxrwxr-x   0 florie    (1000) florie    (1000)     1285 2023-05-11 04:23:23.000000 stmapy-0.4.3/setup.py
+drwxrwxr-x   0 florie    (1000) florie    (1000)        0 2023-05-11 04:25:37.662757 stmapy-0.4.3/stmapy/
+-rwxrwxr-x   0 florie    (1000) florie    (1000)      135 2023-05-10 22:09:35.000000 stmapy-0.4.3/stmapy/__init__.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)       22 2023-05-11 04:23:32.000000 stmapy-0.4.3/stmapy/_version.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)    61082 2023-05-11 04:21:19.000000 stmapy-0.4.3/stmapy/citswidget.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)      165 2023-05-10 22:09:35.000000 stmapy-0.4.3/stmapy/config.json
+-rwxrwxr-x   0 florie    (1000) florie    (1000)      398 2023-05-10 22:09:35.000000 stmapy-0.4.3/stmapy/main.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)      312 2023-05-10 22:09:35.000000 stmapy-0.4.3/stmapy/matplotlibwidget.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)     3468 2023-05-10 22:09:35.000000 stmapy-0.4.3/stmapy/plotting.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)     9883 2023-05-10 22:09:35.000000 stmapy-0.4.3/stmapy/processing.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)    32334 2023-05-10 22:09:35.000000 stmapy-0.4.3/stmapy/reads.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)     5877 2023-05-10 22:09:35.000000 stmapy-0.4.3/stmapy/shape.py
+-rwxrwxr-x   0 florie    (1000) florie    (1000)      814 2023-05-10 22:09:35.000000 stmapy-0.4.3/stmapy/stmapyStyle.mplstyle
+-rwxrwxr-x   0 florie    (1000) florie    (1000)    38217 2023-05-10 22:09:35.000000 stmapy-0.4.3/stmapy/ui_citswidget.ui
+drwxrwxr-x   0 florie    (1000) florie    (1000)        0 2023-05-11 04:25:37.662757 stmapy-0.4.3/stmapy.egg-info/
+-rw-rw-r--   0 florie    (1000) florie    (1000)    11514 2023-05-11 04:25:37.000000 stmapy-0.4.3/stmapy.egg-info/PKG-INFO
+-rw-rw-r--   0 florie    (1000) florie    (1000)      452 2023-05-11 04:25:37.000000 stmapy-0.4.3/stmapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 florie    (1000) florie    (1000)        1 2023-05-11 04:25:37.000000 stmapy-0.4.3/stmapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 florie    (1000) florie    (1000)       44 2023-05-11 04:25:37.000000 stmapy-0.4.3/stmapy.egg-info/entry_points.txt
+-rw-rw-r--   0 florie    (1000) florie    (1000)       40 2023-05-11 04:25:37.000000 stmapy-0.4.3/stmapy.egg-info/requires.txt
+-rw-rw-r--   0 florie    (1000) florie    (1000)        7 2023-05-11 04:25:37.000000 stmapy-0.4.3/stmapy.egg-info/top_level.txt
```

### Comparing `stmapy-0.4.2/LICENSE` & `stmapy-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.2/PKG-INFO` & `stmapy-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stmapy
-Version: 0.4.2
+Version: 0.4.3
 Summary: Scanning tunneling microscopy analysis in Python
 Home-page: https://gitlab.com/lateqs/stmapy
 Author-email: loic.huder@gmail.com, florie.mesple@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `stmapy-0.4.2/README.md` & `stmapy-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.2/setup.py` & `stmapy-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 __version__ = None
 with open("stmapy/_version.py") as o:
     exec(o.read())
 assert __version__ is not None
 
 setuptools.setup(
     name="stmapy",
-    version="0.4.2",
+    version="0.4.3",
     authors="Loïc Huder, Florie Mesple",
     author_email="loic.huder@gmail.com, florie.mesple@gmail.com",
     description="Scanning tunneling microscopy analysis in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/lateqs/stmapy",
     packages=setuptools.find_packages(),
```

### Comparing `stmapy-0.4.2/stmapy/citswidget.py` & `stmapy-0.4.3/stmapy/citswidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     lineTopoPlot, 
     imageTopoPlot
 )
 from PIL import Image, ImageFile
 from scipy.signal import find_peaks
 
 #Set style
-matplotlib.pyplot.style.use(os.path.join(os.path.dirname(__file__),'stmapy.mplstyle')) 
+matplotlib.pyplot.style.use(os.path.join(os.path.dirname(__file__),'stmapyStyle.mplstyle')) 
 
 # Set explictly the backend to Qt for consistency with pyqt.
 matplotlib.use("qt5agg")
 
 # noinspection PyPep8Naming
 class CitsWidget(QtWidgets.QMainWindow):
     # %% Building methods
```

### Comparing `stmapy-0.4.2/stmapy/plotting.py` & `stmapy-0.4.3/stmapy/plotting.py`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.2/stmapy/processing.py` & `stmapy-0.4.3/stmapy/processing.py`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.2/stmapy/reads.py` & `stmapy-0.4.3/stmapy/reads.py`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.2/stmapy/shape.py` & `stmapy-0.4.3/stmapy/shape.py`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.2/stmapy/stmapyStyle.mplstyle` & `stmapy-0.4.3/stmapy/stmapyStyle.mplstyle`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.2/stmapy/ui_citswidget.ui` & `stmapy-0.4.3/stmapy/ui_citswidget.ui`

 * *Files identical despite different names*

### Comparing `stmapy-0.4.2/stmapy.egg-info/PKG-INFO` & `stmapy-0.4.3/stmapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stmapy
-Version: 0.4.2
+Version: 0.4.3
 Summary: Scanning tunneling microscopy analysis in Python
 Home-page: https://gitlab.com/lateqs/stmapy
 Author-email: loic.huder@gmail.com, florie.mesple@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

