# Comparing `tmp/clip_bbox-0.3.0.tar.gz` & `tmp/clip_bbox-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clip_bbox-0.3.0.tar", last modified: Wed May  3 15:13:05 2023, max compression
+gzip compressed data, was "clip_bbox-0.3.1.tar", last modified: Thu May 11 02:04:43 2023, max compression
```

## Comparing `clip_bbox-0.3.0.tar` & `clip_bbox-0.3.1.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.323311 clip_bbox-0.3.0/
--rw-rw----   0 gsu      (20682) gsu      (24121)      528 2023-05-03 15:06:29.000000 clip_bbox-0.3.0/.bumpversion.cfg
--rw-rw----   0 gsu      (20682) gsu      (24121)      123 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/.coveragerc
--rw-rw----   0 gsu      (20682) gsu      (24121)     1804 2023-04-05 02:04:28.000000 clip_bbox-0.3.0/CONTRIBUTING.md
--rw-rw----   0 gsu      (20682) gsu      (24121)    11357 2023-04-05 01:37:03.000000 clip_bbox-0.3.0/LICENSE
--rw-rw----   0 gsu      (20682) gsu      (24121)      681 2023-05-03 14:55:34.000000 clip_bbox-0.3.0/MANIFEST.in
--rw-rw----   0 gsu      (20682) gsu      (24121)     2402 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/Makefile
--rw-rw----   0 gsu      (20682) gsu      (24121)    16565 2023-05-03 15:13:05.323311 clip_bbox-0.3.0/PKG-INFO
--rw-rw----   0 gsu      (20682) gsu      (24121)     2738 2023-05-02 21:26:04.000000 clip_bbox-0.3.0/README.md
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.295311 clip_bbox-0.3.0/clip_bbox/
--rw-rw----   0 gsu      (20682) gsu      (24121)       47 2023-05-03 15:06:29.000000 clip_bbox-0.3.0/clip_bbox/__init__.py
--rw-rw----   0 gsu      (20682) gsu      (24121)      638 2023-05-02 21:26:04.000000 clip_bbox-0.3.0/clip_bbox/__main__.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     6884 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/bbox_utils.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     9375 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/clip.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     2600 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/clip_model_setup.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     3526 2023-05-02 21:26:04.000000 clip_bbox-0.3.0/clip_bbox/clipbbox.py
--rw-rw----   0 gsu      (20682) gsu      (24121)    18878 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/model.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     1239 2023-04-05 03:35:06.000000 clip_bbox-0.3.0/clip_bbox/newpad.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     2601 2023-05-03 14:55:34.000000 clip_bbox-0.3.0/clip_bbox/preprocess.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     4740 2023-04-05 03:35:06.000000 clip_bbox-0.3.0/clip_bbox/simple_tokenizer.py
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.299311 clip_bbox-0.3.0/clip_bbox/tests/
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.315311 clip_bbox-0.3.0/clip_bbox/tests/assets/
--rw-rw----   0 gsu      (20682) gsu      (24121)     3784 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/tests/assets/heat.npz
--rw-rw----   0 gsu      (20682) gsu      (24121) 11059328 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/tests/assets/rocket.npy
--rw-rw----   0 gsu      (20682) gsu      (24121)   302557 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/tests/assets/rocket.png
--rw-rw----   0 gsu      (20682) gsu      (24121)   342530 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/clip_bbox/tests/assets/test_all-gt_output.png
--rw-rw----   0 gsu      (20682) gsu      (24121)     3740 2023-05-02 21:26:04.000000 clip_bbox-0.3.0/clip_bbox/tests/test_all.py
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.299311 clip_bbox-0.3.0/clip_bbox.egg-info/
--rw-rw----   0 gsu      (20682) gsu      (24121)    16565 2023-05-03 15:13:05.000000 clip_bbox-0.3.0/clip_bbox.egg-info/PKG-INFO
--rw-rw----   0 gsu      (20682) gsu      (24121)      930 2023-05-03 15:13:05.000000 clip_bbox-0.3.0/clip_bbox.egg-info/SOURCES.txt
--rw-rw----   0 gsu      (20682) gsu      (24121)        1 2023-05-03 15:13:05.000000 clip_bbox-0.3.0/clip_bbox.egg-info/dependency_links.txt
--rw-rw----   0 gsu      (20682) gsu      (24121)      278 2023-05-03 15:13:05.000000 clip_bbox-0.3.0/clip_bbox.egg-info/requires.txt
--rw-rw----   0 gsu      (20682) gsu      (24121)       10 2023-05-03 15:13:05.000000 clip_bbox-0.3.0/clip_bbox.egg-info/top_level.txt
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.319311 clip_bbox-0.3.0/docs/
--rw-rw----   0 gsu      (20682) gsu      (24121)      638 2023-04-05 02:04:28.000000 clip_bbox-0.3.0/docs/Makefile
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.319311 clip_bbox-0.3.0/docs/images/
--rw-rw----   0 gsu      (20682) gsu      (24121)   833138 2023-05-03 14:55:34.000000 clip_bbox-0.3.0/docs/images/command_line_usage.gif
--rw-rw----   0 gsu      (20682) gsu      (24121)   330320 2023-04-05 02:04:28.000000 clip_bbox-0.3.0/docs/images/example_output.png
--rw-rw----   0 gsu      (20682) gsu      (24121)   341790 2023-05-03 14:55:34.000000 clip_bbox-0.3.0/docs/images/rocket_result.png
--rw-rw----   0 gsu      (20682) gsu      (24121)      804 2023-04-05 02:04:28.000000 clip_bbox-0.3.0/docs/make.bat
--rw-rw----   0 gsu      (20682) gsu      (24121)      122 2023-05-03 15:06:29.000000 clip_bbox-0.3.0/docs/requirements.txt
-drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-03 15:13:05.323311 clip_bbox-0.3.0/docs/source/
--rw-rw----   0 gsu      (20682) gsu      (24121)      728 2023-04-09 16:57:10.000000 clip_bbox-0.3.0/docs/source/clip_bbox.rst
--rw-rw----   0 gsu      (20682) gsu      (24121)     1478 2023-05-03 15:06:29.000000 clip_bbox-0.3.0/docs/source/conf.py
--rw-rw----   0 gsu      (20682) gsu      (24121)     1678 2023-05-03 14:55:34.000000 clip_bbox-0.3.0/docs/source/index.md
--rw-rw----   0 gsu      (20682) gsu      (24121)       66 2023-04-05 03:41:23.000000 clip_bbox-0.3.0/docs/source/modules.rst
--rw-rw----   0 gsu      (20682) gsu      (24121)     2509 2023-05-03 15:06:29.000000 clip_bbox-0.3.0/pyproject.toml
--rw-rw----   0 gsu      (20682) gsu      (24121)      150 2023-05-02 20:35:04.000000 clip_bbox-0.3.0/requirements.txt
--rw-rw----   0 gsu      (20682) gsu      (24121)       38 2023-05-03 15:13:05.323311 clip_bbox-0.3.0/setup.cfg
--rw-rw----   0 gsu      (20682) gsu      (24121)       39 2023-04-05 01:37:03.000000 clip_bbox-0.3.0/setup.py
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-11 02:04:43.513312 clip_bbox-0.3.1/
+-rw-rw----   0 gsu      (20682) gsu      (24121)      528 2023-05-11 02:00:40.000000 clip_bbox-0.3.1/.bumpversion.cfg
+-rw-rw----   0 gsu      (20682) gsu      (24121)      123 2023-05-02 20:35:04.000000 clip_bbox-0.3.1/.coveragerc
+-rw-rw----   0 gsu      (20682) gsu      (24121)     1896 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/CONTRIBUTING.md
+-rw-rw----   0 gsu      (20682) gsu      (24121)    11338 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/LICENSE
+-rw-rw----   0 gsu      (20682) gsu      (24121)      681 2023-05-03 14:55:34.000000 clip_bbox-0.3.1/MANIFEST.in
+-rw-rw----   0 gsu      (20682) gsu      (24121)     2402 2023-05-02 20:35:04.000000 clip_bbox-0.3.1/Makefile
+-rw-rw----   0 gsu      (20682) gsu      (24121)    16694 2023-05-11 02:04:43.513312 clip_bbox-0.3.1/PKG-INFO
+-rw-rw----   0 gsu      (20682) gsu      (24121)     2886 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/README.md
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-11 02:04:43.485312 clip_bbox-0.3.1/clip_bbox/
+-rw-rw----   0 gsu      (20682) gsu      (24121)       47 2023-05-11 02:00:40.000000 clip_bbox-0.3.1/clip_bbox/__init__.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)      638 2023-05-02 21:26:04.000000 clip_bbox-0.3.1/clip_bbox/__main__.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     5568 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/clip_bbox/bbox_utils.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     9350 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/clip_bbox/clip.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     2860 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/clip_bbox/clip_model_setup.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     4001 2023-05-11 01:49:23.000000 clip_bbox-0.3.1/clip_bbox/clipbbox.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)    18878 2023-05-10 02:56:29.000000 clip_bbox-0.3.1/clip_bbox/model.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     1239 2023-04-05 03:35:06.000000 clip_bbox-0.3.1/clip_bbox/newpad.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     3168 2023-05-11 01:50:00.000000 clip_bbox-0.3.1/clip_bbox/preprocess.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     4740 2023-04-05 03:35:06.000000 clip_bbox-0.3.1/clip_bbox/simple_tokenizer.py
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-11 02:04:43.485312 clip_bbox-0.3.1/clip_bbox/tests/
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-11 02:04:43.509312 clip_bbox-0.3.1/clip_bbox/tests/assets/
+-rw-rw----   0 gsu      (20682) gsu      (24121)   142314 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/clip_bbox/tests/assets/camera.png
+-rw-rw----   0 gsu      (20682) gsu      (24121)     3784 2023-05-02 20:35:04.000000 clip_bbox-0.3.1/clip_bbox/tests/assets/heat.npz
+-rw-rw----   0 gsu      (20682) gsu      (24121) 11059328 2023-05-02 20:35:04.000000 clip_bbox-0.3.1/clip_bbox/tests/assets/rocket.npy
+-rw-rw----   0 gsu      (20682) gsu      (24121)   302557 2023-05-02 20:35:04.000000 clip_bbox-0.3.1/clip_bbox/tests/assets/rocket.png
+-rw-rw----   0 gsu      (20682) gsu      (24121)   530702 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/clip_bbox/tests/assets/test_all-gt_camera.png
+-rw-rw----   0 gsu      (20682) gsu      (24121)   393398 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/clip_bbox/tests/assets/test_all-gt_rocket.png
+-rw-rw----   0 gsu      (20682) gsu      (24121)   341790 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/clip_bbox/tests/assets/test_img_heat_bbox_disp-gt_output.png
+-rw-rw----   0 gsu      (20682) gsu      (24121)     4175 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/clip_bbox/tests/test_all.py
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-11 02:04:43.485312 clip_bbox-0.3.1/clip_bbox.egg-info/
+-rw-rw----   0 gsu      (20682) gsu      (24121)    16694 2023-05-11 02:04:43.000000 clip_bbox-0.3.1/clip_bbox.egg-info/PKG-INFO
+-rw-rw----   0 gsu      (20682) gsu      (24121)     1071 2023-05-11 02:04:43.000000 clip_bbox-0.3.1/clip_bbox.egg-info/SOURCES.txt
+-rw-rw----   0 gsu      (20682) gsu      (24121)        1 2023-05-11 02:04:43.000000 clip_bbox-0.3.1/clip_bbox.egg-info/dependency_links.txt
+-rw-rw----   0 gsu      (20682) gsu      (24121)      278 2023-05-11 02:04:43.000000 clip_bbox-0.3.1/clip_bbox.egg-info/requires.txt
+-rw-rw----   0 gsu      (20682) gsu      (24121)       10 2023-05-11 02:04:43.000000 clip_bbox-0.3.1/clip_bbox.egg-info/top_level.txt
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-11 02:04:43.509312 clip_bbox-0.3.1/docs/
+-rw-rw----   0 gsu      (20682) gsu      (24121)      638 2023-04-05 02:04:28.000000 clip_bbox-0.3.1/docs/Makefile
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-11 02:04:43.513312 clip_bbox-0.3.1/docs/images/
+-rw-rw----   0 gsu      (20682) gsu      (24121)   833138 2023-05-03 14:55:34.000000 clip_bbox-0.3.1/docs/images/command_line_usage.gif
+-rw-rw----   0 gsu      (20682) gsu      (24121)   530702 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/docs/images/example_output.png
+-rw-rw----   0 gsu      (20682) gsu      (24121)   341790 2023-05-03 14:55:34.000000 clip_bbox-0.3.1/docs/images/rocket_result.png
+-rw-rw----   0 gsu      (20682) gsu      (24121)      804 2023-04-05 02:04:28.000000 clip_bbox-0.3.1/docs/make.bat
+-rw-rw----   0 gsu      (20682) gsu      (24121)      139 2023-05-11 02:00:40.000000 clip_bbox-0.3.1/docs/requirements.txt
+drwxrwx---   0 gsu      (20682) gsu      (24121)        0 2023-05-11 02:04:43.513312 clip_bbox-0.3.1/docs/source/
+-rw-rw----   0 gsu      (20682) gsu      (24121)      728 2023-04-09 16:57:10.000000 clip_bbox-0.3.1/docs/source/clip_bbox.rst
+-rw-rw----   0 gsu      (20682) gsu      (24121)     1478 2023-05-11 02:00:40.000000 clip_bbox-0.3.1/docs/source/conf.py
+-rw-rw----   0 gsu      (20682) gsu      (24121)     2195 2023-05-11 01:27:17.000000 clip_bbox-0.3.1/docs/source/index.md
+-rw-rw----   0 gsu      (20682) gsu      (24121)       66 2023-04-05 03:41:23.000000 clip_bbox-0.3.1/docs/source/modules.rst
+-rw-rw----   0 gsu      (20682) gsu      (24121)     2509 2023-05-11 02:00:40.000000 clip_bbox-0.3.1/pyproject.toml
+-rw-rw----   0 gsu      (20682) gsu      (24121)      150 2023-05-02 20:35:04.000000 clip_bbox-0.3.1/requirements.txt
+-rw-rw----   0 gsu      (20682) gsu      (24121)       38 2023-05-11 02:04:43.513312 clip_bbox-0.3.1/setup.cfg
+-rw-rw----   0 gsu      (20682) gsu      (24121)       39 2023-04-05 01:37:03.000000 clip_bbox-0.3.1/setup.py
```

### Comparing `clip_bbox-0.3.0/.bumpversion.cfg` & `clip_bbox-0.3.1/.bumpversion.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.0
+current_version = 0.3.1
 commit = True
 tag = True
 
 [bumpversion:file:clip_bbox/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `clip_bbox-0.3.0/CONTRIBUTING.md` & `clip_bbox-0.3.1/CONTRIBUTING.md`

 * *Files 14% similar despite different names*

```diff
@@ -18,30 +18,32 @@
     $ make develop
 
 ## Makefile
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
+- `make check`: check library assets for packaging
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
-- `make annotate`: run type checking using `mypy`
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 - `make dist`: package library for distribution
+- `make clean`: clean the repository
+- `make docs`: clean and build the documentation website
 
 ## Before Opening a Pull Request
 
 If you add any features, please add tests for them in `tests/`.
 
 Be sure to check code quality by confirming that the following commands run successfully:
 
     $ make clean
     $ make lint
-    $ make annotate
     $ make coverage
-    $ make test
+    $ make check
+    $ make docs
 
 ## Submitting Changes
 Once you are done making changes on your own fork of `clip_bbox`, make a pull request to this repository to submit your changes. 
 
 Be sure to describe your changes in the description of your pull request.
```

### Comparing `clip_bbox-0.3.0/LICENSE` & `clip_bbox-0.3.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 Grace Su
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `clip_bbox-0.3.0/MANIFEST.in` & `clip_bbox-0.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/Makefile` & `clip_bbox-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/PKG-INFO` & `clip_bbox-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clip_bbox
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python library for detecting image objects with natural language text labels
 Author-email: Grace Su <grace.duansu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -187,15 +187,15 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright [yyyy] [name of copyright owner]
+           Copyright 2023 Grace Su
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
@@ -226,22 +226,22 @@
 `CLIP_BBox` is a Python library for detecting image objects with natural language text labels. 
 
 [![Build Status](https://github.com/graceduansu/clip_bbox/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/graceduansu/clip_bbox/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/graceduansu/clip_bbox/branch/main/graph/badge.svg)](https://codecov.io/gh/graceduansu/clip_bbox)
 [![GitHub](https://img.shields.io/github/license/graceduansu/clip_bbox)](./LICENSE)
 ![GitHub issues](https://img.shields.io/github/issues/graceduansu/clip_bbox)
 [![PyPI](https://img.shields.io/pypi/v/clip-bbox)](https://pypi.org/project/clip-bbox/)
-[![Documentation Status](https://readthedocs.org/projects/clip-bbox/badge/?version=latest)](https://clip-bbox.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/clip-bbox/badge/?version=latest)](https://clip-bbox.readthedocs.io)
 
 
-## Overview
+## Overview / About
 
 [CLIP](https://github.com/openai/CLIP) is a neural network, pretrained on image-text pairs, that can predict the most relevant text snippet for a given image. 
 
-Given an image and a natural language text label, `CLIP_BBox` will obtain the image's spatial embedding and text label's embedding from CLIP, compute the similarity heatmap between the embeddings, then draw a bounding box around the image region with the highest image-text correspondence. 
+Given an image and a natural language text label, `CLIP_BBox` will obtain the image's spatial embedding and text label's embedding from CLIP, compute the similarity heatmap between the embeddings, then draw bounding boxes around the image regions with the highest image-text correspondences. 
 
 ## Note
 The files for building the CLIP model (`clip.py`, `model.py`, `newpad.py`, `simple_tokenizer.py`) are third-party code from the [CLIP repo](https://github.com/openai/CLIP). They are not included in test coverage.
 
 ### Features
 
 The library provides functions for the following operations:
@@ -280,7 +280,12 @@
 To draw bounding boxes on an image based on its caption, do the following:
 
 ```python
 from clip_bbox import run_clip_bbox
 
 run_clip_bbox("path/to/img.png", "caption of your image", "path/to/output_path.png")
 ```
+
+### Example Output
+Here is an example output image for the caption `"a camera on a tripod"`:
+
+![example output](./clip_bbox/tests/assets/test_all-gt_camera.png)
```

### Comparing `clip_bbox-0.3.0/README.md` & `clip_bbox-0.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 `CLIP_BBox` is a Python library for detecting image objects with natural language text labels. 
 
 [![Build Status](https://github.com/graceduansu/clip_bbox/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/graceduansu/clip_bbox/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/graceduansu/clip_bbox/branch/main/graph/badge.svg)](https://codecov.io/gh/graceduansu/clip_bbox)
 [![GitHub](https://img.shields.io/github/license/graceduansu/clip_bbox)](./LICENSE)
 ![GitHub issues](https://img.shields.io/github/issues/graceduansu/clip_bbox)
 [![PyPI](https://img.shields.io/pypi/v/clip-bbox)](https://pypi.org/project/clip-bbox/)
-[![Documentation Status](https://readthedocs.org/projects/clip-bbox/badge/?version=latest)](https://clip-bbox.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/clip-bbox/badge/?version=latest)](https://clip-bbox.readthedocs.io)
 
 
-## Overview
+## Overview / About
 
 [CLIP](https://github.com/openai/CLIP) is a neural network, pretrained on image-text pairs, that can predict the most relevant text snippet for a given image. 
 
-Given an image and a natural language text label, `CLIP_BBox` will obtain the image's spatial embedding and text label's embedding from CLIP, compute the similarity heatmap between the embeddings, then draw a bounding box around the image region with the highest image-text correspondence. 
+Given an image and a natural language text label, `CLIP_BBox` will obtain the image's spatial embedding and text label's embedding from CLIP, compute the similarity heatmap between the embeddings, then draw bounding boxes around the image regions with the highest image-text correspondences. 
 
 ## Note
 The files for building the CLIP model (`clip.py`, `model.py`, `newpad.py`, `simple_tokenizer.py`) are third-party code from the [CLIP repo](https://github.com/openai/CLIP). They are not included in test coverage.
 
 ### Features
 
 The library provides functions for the following operations:
@@ -58,7 +58,12 @@
 To draw bounding boxes on an image based on its caption, do the following:
 
 ```python
 from clip_bbox import run_clip_bbox
 
 run_clip_bbox("path/to/img.png", "caption of your image", "path/to/output_path.png")
 ```
+
+### Example Output
+Here is an example output image for the caption `"a camera on a tripod"`:
+
+![example output](./clip_bbox/tests/assets/test_all-gt_camera.png)
```

### Comparing `clip_bbox-0.3.0/clip_bbox/__main__.py` & `clip_bbox-0.3.1/clip_bbox/__main__.py`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/clip_bbox/clip.py` & `clip_bbox-0.3.1/clip_bbox/clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,17 +123,14 @@
 
 
 def available_models() -> List[str]:
     """Returns the names of available CLIP models"""
     return list(_MODELS.keys())
 
 
-# TODO: type checking?
-
-
 def load(
     name: str,
     device: Union[str, torch.device] = "cuda" if torch.cuda.is_available() else "cpu",
     jit: bool = False,
     download_root: str = None,
 ):
     """Load a CLIP model
```

### Comparing `clip_bbox-0.3.0/clip_bbox/clip_model_setup.py` & `clip_bbox-0.3.1/clip_bbox/clip_model_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,19 +31,23 @@
 
 
 def get_clip_model(device, model_name="RN50", input_res=(720, 1280)):
     """Downloads pre-trained CLIP model and adjusts model to accept
     desired input resolution.
 
     Args:
-        model_name (str): Description of arg1
-        input_res (tuple[int]): Input resolution represented as (height, width)
+        device (Torch.device): Device Torch should use to run CLIP. For example, the device can be
+            `torch.device("cpu")` or `torch.device("cuda")`
+        model_name (str): The name of the desired CLIP model to download. The options are "RN50", "RN101", "RN50x4", or
+            "ViT-B/32".
+
+        input_res (tuple[int]): Input resolution represented as (height, width).
 
     Returns:
-        Modified Torch model accepting the desired input resolution
+        Modified Torch model accepting the desired input resolution.
 
     """
     print("Torch version:", torch.__version__)
 
     input_resolution = input_res
 
     if not os.path.exists("model.pt"):
```

### Comparing `clip_bbox-0.3.0/clip_bbox/clipbbox.py` & `clip_bbox-0.3.1/clip_bbox/clipbbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 #!/usr/bin/env python3
 
 import torch
 
 from . import clip_model_setup
 from . import bbox_utils
 from . import preprocess
+from math import sqrt, ceil
+
+
+def get_square_int_factors(n):
+    """Finds the 2 largest integer factors that multiply together to produce n.
+
+    Args:
+        n (int): The target integer.
+
+    Returns:
+        tuple: A tuple containing:
+            - val (int): An integer factor of n.
+            - val2 (int): Another integer factor of n.
+
+    """
+    val = ceil(sqrt(n))
+    while True:
+        if not n % val:
+            val2 = n // val
+            break
+        val -= 1
+
+    return val, val2
 
 
 def run_clip_bbox(img_path, caption, out_path):
     """Draws bounding boxes on an input image.
 
     Args:
-        img_path (str): path to input image
-        caption (str): caption of input image
-        out_path (str): path to output image displaying bounding boxes
+        img_path (str): path to input image.
+        caption (str): caption of input image.
+        out_path (str): path to output image displaying bounding boxes.
 
     Returns:
-        None
+        None.
 
     """
     device = torch.device("cpu")
 
     print('torch device:', device)
 
-    input_resolution = (720, 1280)
-    images, image_input = preprocess.preprocess_imgs([img_path], device, input_resolution=input_resolution)
+    # input_resolution = (720, 1280)
+    images, image_input = preprocess.preprocess_imgs([img_path], device)
 
-    # TODO: make img_fts_to_heatmap accept all resolutions
-    # input_resolution = images[0].size()[1:]
+    input_resolution = images[0].size()[1:]
 
     model_modded = clip_model_setup.get_clip_model(device, input_res=input_resolution)
     text_input = preprocess.preprocess_texts([caption], model_modded.context_length, device)
 
     with torch.no_grad():
         image_features = model_modded.encode_image(image_input).float()
         text_features = model_modded.encode_text(text_input).float()
@@ -45,49 +67,46 @@
     heatmap_list = img_fts_to_heatmap(img_fts, text_features)
     pred_bboxes = []
     for h in range(len(heatmap_list)):
         heat = heatmap_list[h]
         # np.savez("heat.npz", heat)
         bboxes = bbox_utils.heat2bbox(heat, input_resolution)
         pred_bboxes.append([torch.tensor(b["bbox_normalized"]).unsqueeze(0) for b in bboxes])
-        bbox_utils.img_heat_bbox_disp(
-            images[h].permute(1, 2, 0).cpu(),
-            heat,
-            out_path,
-            bboxes=bboxes,
-            order="xyxy",
-        )
+        bbox_utils.img_heat_bbox_disp(images[h].permute(1, 2, 0).cpu(), heat, out_path, bboxes=bboxes)
+
+    print("CLIP_BBox run complete!")
 
 
 def img_fts_to_heatmap(img_fts, txt_fts):
     """Computes the similarity heatmap between a pair of
     image and text embeddings from CLIP.
 
     Args:
-        img_fts (numpy array): Image embedding from CLIP
-        txt_fts (numpy array): Text embedding from CLIP
+        img_fts (numpy array): Image embedding from CLIP.
+        txt_fts (numpy array): Text embedding from CLIP.
 
     Returns:
-        numpy array: Similarity heatmap between
-        the image and text embeddings
+        numpy array: Similarity heatmap between the image and text embeddings.
 
     """
 
     # dot product with normalization
     img_norm = img_fts / img_fts.norm(dim=-1, keepdim=True)
     txt_norm = txt_fts / txt_fts.norm(dim=-1, keepdim=True)
 
     batch_size = len(txt_norm)
     # print(batch_size)
 
     # img_norm = F.interpolate(img_norm.permute(2,1,0), size=int(input_resolution[0]*input_resolution[1]/64),
     #      mode='nearest').permute(2,1,0)
     # resize = torch.flatten(img_norm).size()[0] / batch_size / img_fts.size()[0]
     # resize = int(math.sqrt(resize))
-    img_reshape = torch.reshape(img_norm, (22, 40, batch_size, img_fts.size()[2]))
+    dim1, dim2 = get_square_int_factors(img_fts.size(0))
+    print(f"image feature dimensions: {dim1} x {dim2}")
+    img_reshape = torch.reshape(img_norm, (dim1, dim2, batch_size, img_fts.size()[2]))
     # img_reshape = torch.reshape(img_norm, (7, 7, batch_size, 1024))
     # img_reshape = torch.reshape(img_norm, (resize, resize, batch_size, img_fts.size()[0]))
     # print(img_reshape.shape)
     # print(txt_norm.shape)
 
     img_reshape = img_reshape.cpu()
```

### Comparing `clip_bbox-0.3.0/clip_bbox/model.py` & `clip_bbox-0.3.1/clip_bbox/model.py`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/clip_bbox/newpad.py` & `clip_bbox-0.3.1/clip_bbox/newpad.py`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/clip_bbox/preprocess.py` & `clip_bbox-0.3.1/clip_bbox/preprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,30 @@
 from .simple_tokenizer import SimpleTokenizer
 
 
 def preprocess_imgs(img_path_list, device, input_resolution=None):
     """Preprocess list of images for CLIP.
 
     Args:
-        img_path_list (List[str]): List of image paths to preprocess
-        input_resolution (tuple[int]): Input resolution represented as (height, width)
+        img_path_list (List[str]): List of image paths to preprocess.
+        device (Torch.device): Device Torch should use to run CLIP. For example, the device can be
+            `torch.device("cpu")` or `torch.device("cuda")`
+
+        input_resolution (tuple[int]): Input resolution represented as (height, width). If not
+            specified, the default value will be the first input image's original dimensions.
 
     Returns:
-        List[Torch tensor]: List of images
-        Torch tensor: Array of images preprocessed as a Torch tensor
+        tuple: A tuple containing:
+            - images (List[Torch tensor]): List of images.
+            - image input (Torch tensor): Array of images preprocessed for input to CLIP.
 
     """
     if not input_resolution:
         input_resolution = Image.open(img_path_list[0]).size
+        input_resolution = (input_resolution[1], input_resolution[0])
 
     preprocess = Compose(
         [
             Resize(input_resolution, interpolation=Image.BICUBIC),
             ToTensor(),
         ]
     )
@@ -49,19 +55,21 @@
     return images, image_input
 
 
 def preprocess_texts(caption_list, context_length, device):
     """Preprocess list of texts for CLIP.
 
     Args:
-        caption_list (List[str]): List of captions
-        context_length (int): CLIP model parameter
+        caption_list (List[str]): List of captions.
+        context_length (int): CLIP model parameter.
+        device (Torch.device): Device Torch should use to run CLIP. For example, the device can be
+            `torch.device("cpu")` or `torch.device("cuda")`
 
     Returns:
-        Torch tensor: Array of preprocessed texts
+        Torch tensor: Array of preprocessed texts.
 
     """
     tokenizer = SimpleTokenizer()
     text_tokens = [tokenizer.encode("This is " + desc) for desc in caption_list]
 
     text_input = torch.zeros(len(text_tokens), context_length, dtype=torch.long)
     sot_token = tokenizer.encoder["<|startoftext|>"]
```

### Comparing `clip_bbox-0.3.0/clip_bbox/simple_tokenizer.py` & `clip_bbox-0.3.1/clip_bbox/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/clip_bbox/tests/assets/heat.npz` & `clip_bbox-0.3.1/clip_bbox/tests/assets/heat.npz`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/clip_bbox/tests/assets/rocket.npy` & `clip_bbox-0.3.1/clip_bbox/tests/assets/rocket.npy`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/clip_bbox/tests/assets/rocket.png` & `clip_bbox-0.3.1/clip_bbox/tests/assets/rocket.png`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/clip_bbox/tests/test_all.py` & `clip_bbox-0.3.1/clip_bbox/tests/test_all.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 
 
 def imgs_are_same(img1_path, img2_path):
     img1 = Image.open(img1_path).convert('RGB')
     img2 = Image.open(img2_path).convert('RGB')
 
     equal_size = img1.height == img2.height and img1.width == img2.width
-    equal_content = len(set(ImageChops.difference(img1, img2).getbbox())) < 5
+    diff = ImageChops.difference(img1, img2).getbbox()
+
+    if diff:
+        equal_content = len(set(diff)) < 5
+    else:
+        equal_content = True
 
     return equal_size and equal_content
 
 
 # Ground truth outputs:
 heat = np.load("clip_bbox/tests/assets/heat.npz")['arr_0']
 gt_bboxes = [
@@ -52,19 +57,19 @@
         assert isclose(gt_score, score, rel_tol=1e-6)
         assert gt_bboxes[i]['bbox'] == bboxes[i]['bbox']
         assert np.allclose(gt_bboxes[i]['bbox_normalized'], bboxes[i]['bbox_normalized'], atol=1e-6)
 
 
 def test_img_heat_bbox_disp():
     image = np.load("clip_bbox/tests/assets/rocket.npy")
-    fig = bu.img_heat_bbox_disp(
-        image, heat, "clip_bbox/tests/test_img_heat_bbox_disp.png", bboxes=gt_bboxes, order="xyxy"
-    )
+    fig = bu.img_heat_bbox_disp(image, heat, "clip_bbox/tests/test_img_heat_bbox_disp.png", bboxes=gt_bboxes)
     assert isinstance(fig, Figure)
-    assert imgs_are_same("clip_bbox/tests/assets/test_all-gt_output.png", "clip_bbox/tests/test_img_heat_bbox_disp.png")
+    assert imgs_are_same(
+        "clip_bbox/tests/assets/test_img_heat_bbox_disp-gt_output.png", "clip_bbox/tests/test_img_heat_bbox_disp.png"
+    )
     os.remove("clip_bbox/tests/test_img_heat_bbox_disp.png")
 
 
 # preprocess
 def test_preprocess_imgs():
     device = torch.device("cpu")
     images, input = p.preprocess_imgs(["clip_bbox/tests/assets/rocket.png"], device, input_resolution=input_resolution)
@@ -92,18 +97,26 @@
 
 
 # INTEGRATION TESTS
 
 
 def test_run_clip_bbox():
     cb.run_clip_bbox(
-        "clip_bbox/tests/assets/rocket.png", "a rocket standing on a launchpad", "clip_bbox/tests/test_all.png"
+        "clip_bbox/tests/assets/rocket.png", "a rocket standing on a launchpad", "clip_bbox/tests/test_all-rocket.png"
     )
-    assert imgs_are_same("clip_bbox/tests/assets/test_all-gt_output.png", "clip_bbox/tests/test_all.png")
-    os.remove("clip_bbox/tests/test_all.png")
+    assert imgs_are_same("clip_bbox/tests/assets/test_all-gt_rocket.png", "clip_bbox/tests/test_all-rocket.png")
+    os.remove("clip_bbox/tests/test_all-rocket.png")
+
+    cb.run_clip_bbox("clip_bbox/tests/assets/camera.png", "a camera on a tripod", "clip_bbox/tests/test_all-camera.png")
+    assert imgs_are_same("clip_bbox/tests/assets/test_all-gt_camera.png", "clip_bbox/tests/test_all-camera.png")
+    os.remove("clip_bbox/tests/test_all-camera.png")
 
 
 def test_main():
-    cli_args = ["clip_bbox/tests/assets/rocket.png", "a rocket standing on a launchpad", "clip_bbox/tests/test_all.png"]
+    cli_args = [
+        "clip_bbox/tests/assets/rocket.png",
+        "a rocket standing on a launchpad",
+        "clip_bbox/tests/test_all-rocket.png",
+    ]
     main(cli_args)
-    assert imgs_are_same("clip_bbox/tests/assets/test_all-gt_output.png", "clip_bbox/tests/test_all.png")
-    os.remove("clip_bbox/tests/test_all.png")
+    assert imgs_are_same("clip_bbox/tests/assets/test_all-gt_rocket.png", "clip_bbox/tests/test_all-rocket.png")
+    os.remove("clip_bbox/tests/test_all-rocket.png")
```

### Comparing `clip_bbox-0.3.0/clip_bbox.egg-info/PKG-INFO` & `clip_bbox-0.3.1/clip_bbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clip-bbox
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python library for detecting image objects with natural language text labels
 Author-email: Grace Su <grace.duansu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -187,15 +187,15 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright [yyyy] [name of copyright owner]
+           Copyright 2023 Grace Su
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
@@ -226,22 +226,22 @@
 `CLIP_BBox` is a Python library for detecting image objects with natural language text labels. 
 
 [![Build Status](https://github.com/graceduansu/clip_bbox/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/graceduansu/clip_bbox/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/graceduansu/clip_bbox/branch/main/graph/badge.svg)](https://codecov.io/gh/graceduansu/clip_bbox)
 [![GitHub](https://img.shields.io/github/license/graceduansu/clip_bbox)](./LICENSE)
 ![GitHub issues](https://img.shields.io/github/issues/graceduansu/clip_bbox)
 [![PyPI](https://img.shields.io/pypi/v/clip-bbox)](https://pypi.org/project/clip-bbox/)
-[![Documentation Status](https://readthedocs.org/projects/clip-bbox/badge/?version=latest)](https://clip-bbox.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/clip-bbox/badge/?version=latest)](https://clip-bbox.readthedocs.io)
 
 
-## Overview
+## Overview / About
 
 [CLIP](https://github.com/openai/CLIP) is a neural network, pretrained on image-text pairs, that can predict the most relevant text snippet for a given image. 
 
-Given an image and a natural language text label, `CLIP_BBox` will obtain the image's spatial embedding and text label's embedding from CLIP, compute the similarity heatmap between the embeddings, then draw a bounding box around the image region with the highest image-text correspondence. 
+Given an image and a natural language text label, `CLIP_BBox` will obtain the image's spatial embedding and text label's embedding from CLIP, compute the similarity heatmap between the embeddings, then draw bounding boxes around the image regions with the highest image-text correspondences. 
 
 ## Note
 The files for building the CLIP model (`clip.py`, `model.py`, `newpad.py`, `simple_tokenizer.py`) are third-party code from the [CLIP repo](https://github.com/openai/CLIP). They are not included in test coverage.
 
 ### Features
 
 The library provides functions for the following operations:
@@ -280,7 +280,12 @@
 To draw bounding boxes on an image based on its caption, do the following:
 
 ```python
 from clip_bbox import run_clip_bbox
 
 run_clip_bbox("path/to/img.png", "caption of your image", "path/to/output_path.png")
 ```
+
+### Example Output
+Here is an example output image for the caption `"a camera on a tripod"`:
+
+![example output](./clip_bbox/tests/assets/test_all-gt_camera.png)
```

### Comparing `clip_bbox-0.3.0/clip_bbox.egg-info/SOURCES.txt` & `clip_bbox-0.3.1/clip_bbox.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,18 +20,21 @@
 clip_bbox/simple_tokenizer.py
 clip_bbox.egg-info/PKG-INFO
 clip_bbox.egg-info/SOURCES.txt
 clip_bbox.egg-info/dependency_links.txt
 clip_bbox.egg-info/requires.txt
 clip_bbox.egg-info/top_level.txt
 clip_bbox/tests/test_all.py
+clip_bbox/tests/assets/camera.png
 clip_bbox/tests/assets/heat.npz
 clip_bbox/tests/assets/rocket.npy
 clip_bbox/tests/assets/rocket.png
-clip_bbox/tests/assets/test_all-gt_output.png
+clip_bbox/tests/assets/test_all-gt_camera.png
+clip_bbox/tests/assets/test_all-gt_rocket.png
+clip_bbox/tests/assets/test_img_heat_bbox_disp-gt_output.png
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/images/command_line_usage.gif
 docs/images/example_output.png
 docs/images/rocket_result.png
 docs/source/clip_bbox.rst
```

### Comparing `clip_bbox-0.3.0/docs/Makefile` & `clip_bbox-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/docs/images/command_line_usage.gif` & `clip_bbox-0.3.1/docs/images/command_line_usage.gif`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/docs/images/rocket_result.png` & `clip_bbox-0.3.1/clip_bbox/tests/assets/test_img_heat_bbox_disp-gt_output.png`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/docs/make.bat` & `clip_bbox-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/docs/source/clip_bbox.rst` & `clip_bbox-0.3.1/docs/source/clip_bbox.rst`

 * *Files identical despite different names*

### Comparing `clip_bbox-0.3.0/docs/source/conf.py` & `clip_bbox-0.3.1/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'clip_bbox'
 copyright = '2023, Grace Su'
 author = 'Grace Su'
-release = "0.3.0"
+release = "0.3.1"
 
 master_doc = 'index'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['recommonmark', 'sphinx.ext.autodoc', 'sphinx.ext.githubpages', 'sphinx.ext.napoleon']
```

### Comparing `clip_bbox-0.3.0/docs/source/index.md` & `clip_bbox-0.3.1/docs/source/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Welcome to clip_bbox's documentation!
 
+## Overview / About
+
+[CLIP](https://github.com/openai/CLIP) is a neural network, pretrained on image-text pairs, that can predict the most relevant text snippet for a given image. 
+
+Given an image and a natural language text label, `CLIP_BBox` will obtain the image's spatial embedding and text label's embedding from CLIP, compute the similarity heatmap between the embeddings, then draw bounding boxes around the image regions with the highest image-text correspondences. 
+
 ## Installation
 
 Use pip to install clip_bbox as a Python package:
 
     $ pip install clip-bbox
 
 ### Use As a Command Line Script
@@ -37,15 +43,15 @@
 from clip_bbox import run_clip_bbox
 
 run_clip_bbox("path/to/img.png", "caption of your image", "path/to/output_path.png")
 ```
 
 Using the `run_clip_bbox()` will result in an output image displaying the original image, the similarity heatmap between then spatial and text embeddings from CLIP, and the image with bounding boxes & heatmap drawn on top of it. 
 
-Here is an example output image:
+Here is an example output image for the caption `"a camera on a tripod"`:
 ```eval_rst
 .. image:: ../images/example_output.png
 ```
 
 #### Usage Example
 
 ```python
```

### Comparing `clip_bbox-0.3.0/pyproject.toml` & `clip_bbox-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "clip_bbox"
 authors = [{name = "Grace Su", email = "grace.duansu@gmail.com"}]
 description="Python library for detecting image objects with natural language text labels"
 readme = "README.md"
-version = "0.3.0"
+version = "0.3.1"
 requires-python = ">=3.7"
 
 dependencies = [
     "torch==1.7.1", 
     "torchvision", 
     "ftfy", 
     "regex",
```

