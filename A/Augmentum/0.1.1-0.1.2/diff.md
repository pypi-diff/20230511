# Comparing `tmp/Augmentum-0.1.1.tar.gz` & `tmp/Augmentum-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Augmentum-0.1.1.tar", last modified: Fri May  5 05:33:39 2023, max compression
+gzip compressed data, was "dist/Augmentum-0.1.2.tar", last modified: Thu May 11 02:30:44 2023, max compression
```

## Comparing `Augmentum-0.1.1.tar` & `Augmentum-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,34 @@
-drwxr-xr-x   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-05 05:33:39.000000 Augmentum-0.1.1/
-drwxr-xr-x   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-05 05:33:39.000000 Augmentum-0.1.1/Augmentum.egg-info/
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)    14864 2023-05-05 05:33:39.000000 Augmentum-0.1.1/Augmentum.egg-info/PKG-INFO
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      326 2023-05-05 05:33:39.000000 Augmentum-0.1.1/Augmentum.egg-info/SOURCES.txt
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)        1 2023-05-05 05:33:39.000000 Augmentum-0.1.1/Augmentum.egg-info/dependency_links.txt
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      204 2023-05-05 05:33:39.000000 Augmentum-0.1.1/Augmentum.egg-info/requires.txt
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)        1 2023-05-05 05:33:39.000000 Augmentum-0.1.1/Augmentum.egg-info/top_level.txt
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     2539 2023-05-05 03:12:19.000000 Augmentum-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)    11357 2023-02-21 21:40:37.000000 Augmentum-0.1.1/LICENSE
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      457 2023-05-04 01:55:12.000000 Augmentum-0.1.1/MANIFEST.in
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      940 2023-05-04 01:55:12.000000 Augmentum-0.1.1/Makefile
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)    14864 2023-05-05 05:33:39.000000 Augmentum-0.1.1/PKG-INFO
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     1504 2023-05-05 03:12:19.000000 Augmentum-0.1.1/README.md
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     1849 2023-05-05 03:12:19.000000 Augmentum-0.1.1/pyproject.toml
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)       38 2023-05-05 05:33:39.000000 Augmentum-0.1.1/setup.cfg
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)       38 2023-05-04 01:55:12.000000 Augmentum-0.1.1/setup.py
-drwxr-xr-x   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-05 05:33:39.000000 Augmentum-0.1.1/source/
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     1895 2023-05-04 01:55:12.000000 Augmentum-0.1.1/source/augment.py
-drwxr-xr-x   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-05 05:33:39.000000 Augmentum-0.1.1/source/tests/
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)       85 2023-05-04 03:57:38.000000 Augmentum-0.1.1/source/tests/__init__.py
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     1638 2023-05-04 03:11:33.000000 Augmentum-0.1.1/source/tests/test_all.py
-drwxr-xr-x   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-05 05:33:39.000000 Augmentum-0.1.1/temp/
--rw-r--r--   0 kerimkurttepeli   (501) staff       (20)       17 2023-05-03 04:36:42.000000 Augmentum-0.1.1/temp/TESTING.md
+drwxr-xr-x   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-11 02:30:44.000000 Augmentum-0.1.2/
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      719 2023-05-11 00:17:56.000000 Augmentum-0.1.2/.readthedocs.yaml
+drwxr-xr-x   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-11 02:30:44.000000 Augmentum-0.1.2/Augmentum/
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     3700 2023-05-11 01:51:53.000000 Augmentum-0.1.2/Augmentum/Augmentum.py
+drwxr-xr-x   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-11 02:30:44.000000 Augmentum-0.1.2/Augmentum/data/
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-11 01:51:53.000000 Augmentum-0.1.2/Augmentum/data/.gitkeep
+drwxr-xr-x   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-11 02:30:44.000000 Augmentum-0.1.2/Augmentum/tests/
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)       85 2023-05-11 00:17:56.000000 Augmentum-0.1.2/Augmentum/tests/__init__.py
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     1491 2023-05-11 01:51:53.000000 Augmentum-0.1.2/Augmentum/tests/test_all.py
+drwxr-xr-x   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-11 02:30:44.000000 Augmentum-0.1.2/Augmentum.egg-info/
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)    15542 2023-05-11 02:30:44.000000 Augmentum-0.1.2/Augmentum.egg-info/PKG-INFO
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      535 2023-05-11 02:30:44.000000 Augmentum-0.1.2/Augmentum.egg-info/SOURCES.txt
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)        1 2023-05-11 02:30:44.000000 Augmentum-0.1.2/Augmentum.egg-info/dependency_links.txt
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      216 2023-05-11 02:30:44.000000 Augmentum-0.1.2/Augmentum.egg-info/requires.txt
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)        1 2023-05-11 02:30:44.000000 Augmentum-0.1.2/Augmentum.egg-info/top_level.txt
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     2539 2023-05-11 00:17:56.000000 Augmentum-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)    11357 2023-05-11 00:17:56.000000 Augmentum-0.1.2/LICENSE
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      597 2023-05-11 01:51:53.000000 Augmentum-0.1.2/MANIFEST.in
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     2758 2023-05-11 00:17:56.000000 Augmentum-0.1.2/Makefile
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)    15542 2023-05-11 02:30:44.000000 Augmentum-0.1.2/PKG-INFO
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     2182 2023-05-11 02:14:04.000000 Augmentum-0.1.2/README.md
+drwxr-xr-x   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-11 02:30:44.000000 Augmentum-0.1.2/docs/
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      638 2023-05-11 00:17:56.000000 Augmentum-0.1.2/docs/Makefile
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      804 2023-05-11 00:17:56.000000 Augmentum-0.1.2/docs/make.bat
+drwxr-xr-x   0 kerimkurttepeli   (501) staff       (20)        0 2023-05-11 02:30:44.000000 Augmentum-0.1.2/docs/source/
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      186 2023-05-11 01:36:14.000000 Augmentum-0.1.2/docs/source/Augmentum.rst
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     1186 2023-05-11 02:23:40.000000 Augmentum-0.1.2/docs/source/conf.py
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     3122 2023-05-11 01:51:53.000000 Augmentum-0.1.2/docs/source/examples.md
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      478 2023-05-11 01:29:44.000000 Augmentum-0.1.2/docs/source/index.rst
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      282 2023-05-11 00:17:56.000000 Augmentum-0.1.2/docs/source/installation.md
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)      138 2023-05-11 01:33:08.000000 Augmentum-0.1.2/docs/source/modules.rst
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)     1874 2023-05-11 02:23:40.000000 Augmentum-0.1.2/pyproject.toml
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)       38 2023-05-11 02:30:44.000000 Augmentum-0.1.2/setup.cfg
+-rw-r--r--   0 kerimkurttepeli   (501) staff       (20)       38 2023-05-11 00:17:56.000000 Augmentum-0.1.2/setup.py
```

### Comparing `Augmentum-0.1.1/Augmentum.egg-info/PKG-INFO` & `Augmentum-0.1.2/Augmentum.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Augmentum
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for doing image augmentation
 Author-email: Kerim Kurttepeli <kk3084@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -213,34 +213,39 @@
 License-File: LICENSE
 
 # Augmentum
 A library for doing image augmentation
 
 [![license badge - Apache 2.0](https://img.shields.io/badge/license-Apache--2.0-brightgreen)](./LICENSE)
 ![image](https://img.shields.io/github/issues/kurttepelikerim/Augmentum)
-[![codecov](https://codecov.io/gh/kurttepelikerim/Augmentum/branch/codecov/graph/badge.svg?token=D4K13TWGTK)](https://codecov.io/gh/kurttepelikerim/Augmentum)
+[![codecov](https://codecov.io/gh/kurttepelikerim/Augmentum/branch/main/graph/badge.svg)](https://codecov.io/gh/kurttepelikerim/Augmentum)
 [![Build Status](https://github.com/kurttepelikerim/Augmentum/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/kurttepelikerim/Augmentum/actions?query=workflow%3A%22Build+Status%22)
+[![PyPI](https://img.shields.io/pypi/v/Augmentum)](https://pypi.org/project/Augmentum/)
+[![Docs](https://img.shields.io/badge/docs-passing-success)](https://kurttepelikerim.github.io/Augmentum/)
 
 ## Overview:
-Augmentum is a library to apply many image augmentations and allow this via a simple interface. This library relies on other libraries and selects the augmentations and their parameters randomly from the sensible presets.
+Image data augmentation is the process of generating new transformed versions of images from the given image dataset to artificially expand the dataset. Augmentum is a library for doing image data augmentation given some images. The main purpose for this library is to apply many data augmentations and allow this via a simple interface without relying on special libraries like opencv, matplotlib, pillow etc.
 
 ### Development and Contributions:
 For development details and contribution instructions, please refer to the [contribution guidelines](https://github.com/kurttepelikerim/Augmentum/blob/main/CONTRIBUTING.md).
 
 ## Installation: 
 First, install Python 3.7 (or later) and numpy, and then install this repo as a Python package. 
 
 ```bash
 $ pip install numpy
 $ pip install Augmentum
 ```
 
 ## Quick Start Example:
-Below is a simple use-case for quick start:
-    
+Users can get more images by passing their pre-existing images using image augmentation techniques.
 ```python
-#given a image in the form of a square matrix (list of lists):
-image_matrix = square_matrix = [[1, 1, 1], [1, 0, 0], [1, 0, 0]]
-
-#returns a list of images:
-new_images = Augmentum.augment_image(image_matrix)
+import Augmentum
+#replace image by the actual grayscale image values
+image =  [[1, 1, 1], [1, 0, 0], [1, 0, 0]]
+#or instead upload a .raw image file under '.../Augmentum/Augmentum/data/'and
+#call process_image() to get a list of lists representations of your grayscale image however
+#you have to specify the number of ROWS and COLS in your image (default value is 512x512)
+image = Augmentum.process_image(ROWS=512, COLS=512)
+new_images = Augmentum.augment_image(image)
 ```
+
```

### Comparing `Augmentum-0.1.1/CONTRIBUTING.md` & `Augmentum-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Augmentum-0.1.1/LICENSE` & `Augmentum-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Augmentum-0.1.1/PKG-INFO` & `Augmentum-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Augmentum
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for doing image augmentation
 Author-email: Kerim Kurttepeli <kk3084@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -213,34 +213,39 @@
 License-File: LICENSE
 
 # Augmentum
 A library for doing image augmentation
 
 [![license badge - Apache 2.0](https://img.shields.io/badge/license-Apache--2.0-brightgreen)](./LICENSE)
 ![image](https://img.shields.io/github/issues/kurttepelikerim/Augmentum)
-[![codecov](https://codecov.io/gh/kurttepelikerim/Augmentum/branch/codecov/graph/badge.svg?token=D4K13TWGTK)](https://codecov.io/gh/kurttepelikerim/Augmentum)
+[![codecov](https://codecov.io/gh/kurttepelikerim/Augmentum/branch/main/graph/badge.svg)](https://codecov.io/gh/kurttepelikerim/Augmentum)
 [![Build Status](https://github.com/kurttepelikerim/Augmentum/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/kurttepelikerim/Augmentum/actions?query=workflow%3A%22Build+Status%22)
+[![PyPI](https://img.shields.io/pypi/v/Augmentum)](https://pypi.org/project/Augmentum/)
+[![Docs](https://img.shields.io/badge/docs-passing-success)](https://kurttepelikerim.github.io/Augmentum/)
 
 ## Overview:
-Augmentum is a library to apply many image augmentations and allow this via a simple interface. This library relies on other libraries and selects the augmentations and their parameters randomly from the sensible presets.
+Image data augmentation is the process of generating new transformed versions of images from the given image dataset to artificially expand the dataset. Augmentum is a library for doing image data augmentation given some images. The main purpose for this library is to apply many data augmentations and allow this via a simple interface without relying on special libraries like opencv, matplotlib, pillow etc.
 
 ### Development and Contributions:
 For development details and contribution instructions, please refer to the [contribution guidelines](https://github.com/kurttepelikerim/Augmentum/blob/main/CONTRIBUTING.md).
 
 ## Installation: 
 First, install Python 3.7 (or later) and numpy, and then install this repo as a Python package. 
 
 ```bash
 $ pip install numpy
 $ pip install Augmentum
 ```
 
 ## Quick Start Example:
-Below is a simple use-case for quick start:
-    
+Users can get more images by passing their pre-existing images using image augmentation techniques.
 ```python
-#given a image in the form of a square matrix (list of lists):
-image_matrix = square_matrix = [[1, 1, 1], [1, 0, 0], [1, 0, 0]]
-
-#returns a list of images:
-new_images = Augmentum.augment_image(image_matrix)
+import Augmentum
+#replace image by the actual grayscale image values
+image =  [[1, 1, 1], [1, 0, 0], [1, 0, 0]]
+#or instead upload a .raw image file under '.../Augmentum/Augmentum/data/'and
+#call process_image() to get a list of lists representations of your grayscale image however
+#you have to specify the number of ROWS and COLS in your image (default value is 512x512)
+image = Augmentum.process_image(ROWS=512, COLS=512)
+new_images = Augmentum.augment_image(image)
 ```
+
```

### Comparing `Augmentum-0.1.1/README.md` & `Augmentum-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 # Augmentum
 A library for doing image augmentation
 
 [![license badge - Apache 2.0](https://img.shields.io/badge/license-Apache--2.0-brightgreen)](./LICENSE)
 ![image](https://img.shields.io/github/issues/kurttepelikerim/Augmentum)
-[![codecov](https://codecov.io/gh/kurttepelikerim/Augmentum/branch/codecov/graph/badge.svg?token=D4K13TWGTK)](https://codecov.io/gh/kurttepelikerim/Augmentum)
+[![codecov](https://codecov.io/gh/kurttepelikerim/Augmentum/branch/main/graph/badge.svg)](https://codecov.io/gh/kurttepelikerim/Augmentum)
 [![Build Status](https://github.com/kurttepelikerim/Augmentum/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/kurttepelikerim/Augmentum/actions?query=workflow%3A%22Build+Status%22)
+[![PyPI](https://img.shields.io/pypi/v/Augmentum)](https://pypi.org/project/Augmentum/)
+[![Docs](https://img.shields.io/badge/docs-passing-success)](https://kurttepelikerim.github.io/Augmentum/)
 
 ## Overview:
-Augmentum is a library to apply many image augmentations and allow this via a simple interface. This library relies on other libraries and selects the augmentations and their parameters randomly from the sensible presets.
+Image data augmentation is the process of generating new transformed versions of images from the given image dataset to artificially expand the dataset. Augmentum is a library for doing image data augmentation given some images. The main purpose for this library is to apply many data augmentations and allow this via a simple interface without relying on special libraries like opencv, matplotlib, pillow etc.
 
 ### Development and Contributions:
 For development details and contribution instructions, please refer to the [contribution guidelines](https://github.com/kurttepelikerim/Augmentum/blob/main/CONTRIBUTING.md).
 
 ## Installation: 
 First, install Python 3.7 (or later) and numpy, and then install this repo as a Python package. 
 
 ```bash
 $ pip install numpy
 $ pip install Augmentum
 ```
 
 ## Quick Start Example:
-Below is a simple use-case for quick start:
-    
+Users can get more images by passing their pre-existing images using image augmentation techniques.
 ```python
-#given a image in the form of a square matrix (list of lists):
-image_matrix = square_matrix = [[1, 1, 1], [1, 0, 0], [1, 0, 0]]
-
-#returns a list of images:
-new_images = Augmentum.augment_image(image_matrix)
+import Augmentum
+#replace image by the actual grayscale image values
+image =  [[1, 1, 1], [1, 0, 0], [1, 0, 0]]
+#or instead upload a .raw image file under '.../Augmentum/Augmentum/data/'and
+#call process_image() to get a list of lists representations of your grayscale image however
+#you have to specify the number of ROWS and COLS in your image (default value is 512x512)
+image = Augmentum.process_image(ROWS=512, COLS=512)
+new_images = Augmentum.augment_image(image)
 ```
+
```

### Comparing `Augmentum-0.1.1/pyproject.toml` & `Augmentum-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "Augmentum"
 authors = [{name = "Kerim Kurttepeli", email = "kk3084@columbia.edu"}]
 description="A library for doing image augmentation"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Programming Language :: Python :: 3.10",
 ]
@@ -38,14 +38,15 @@
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
     "pytest-mock>=3.10.0",
     "twine",
     "wheel",
     "numpy",
     "sphinx",
+    "myst-parser",
     "IPython",
     "config"
 ]
 
 [tool.black]
 color = true
 line-length = 120
@@ -56,15 +57,15 @@
 ignore = [
 ]
 
 [tool.flake8]
 ignore = ['E203', 'W503']
 max-line-length=120
 exclude=[
-    'source/tests/*'
+    'Augmentum/tests/*'
 ]
 per-file-ignores= [
 ]
 
 
 [tool.isort]
 line_length = 120
@@ -88,11 +89,11 @@
 # disallow_subclassing_any = true
 # disallow_incomplete_defs = true
 # disallow_untyped_decorators = true
 # disallow_untyped_calls = true
 
 [tool.pytest.ini_options]
 asyncio_mode = 'strict'
-testpaths = 'source/tests'
+testpaths = 'Augmentum/tests'
 
 [tool.setuptools]
 py-modules = []
```

