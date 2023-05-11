# Comparing `tmp/terminal_tracker-1.0.0.tar.gz` & `tmp/terminal_tracker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_tracker-1.0.0.tar", last modified: Wed May  3 23:11:14 2023, max compression
+gzip compressed data, was "terminal_tracker-1.0.1.tar", last modified: Thu May 11 15:14:43 2023, max compression
```

## Comparing `terminal_tracker-1.0.0.tar` & `terminal_tracker-1.0.1.tar`

### file list

```diff
@@ -1,57 +1,52 @@
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.358312 terminal_tracker-1.0.0/
--rw-r--r--   0 miloniatal   (501) staff       (20)      401 2023-05-03 23:00:34.000000 terminal_tracker-1.0.0/.bumpversion.cfg
--rw-r--r--   0 miloniatal   (501) staff       (20)       25 2023-03-23 23:29:05.000000 terminal_tracker-1.0.0/.coveragerc
--rw-r--r--   0 miloniatal   (501) staff       (20)     1319 2023-03-23 23:29:05.000000 terminal_tracker-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 miloniatal   (501) staff       (20)     1068 2023-02-15 16:49:03.000000 terminal_tracker-1.0.0/LICENSE
--rw-r--r--   0 miloniatal   (501) staff       (20)      552 2023-04-10 18:45:13.000000 terminal_tracker-1.0.0/MANIFEST.in
--rw-r--r--   0 miloniatal   (501) staff       (20)     2623 2023-04-04 22:56:49.000000 terminal_tracker-1.0.0/Makefile
--rw-r--r--   0 miloniatal   (501) staff       (20)     4955 2023-05-03 23:11:14.358077 terminal_tracker-1.0.0/PKG-INFO
--rw-r--r--   0 miloniatal   (501) staff       (20)     2893 2023-05-03 22:46:36.000000 terminal_tracker-1.0.0/README.md
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.344465 terminal_tracker-1.0.0/docs/
--rw-r--r--   0 miloniatal   (501) staff       (20)      634 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/Makefile
--rw-r--r--   0 miloniatal   (501) staff       (20)     1653 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/conf.py
--rw-r--r--   0 miloniatal   (501) staff       (20)     1818 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/examples.md
--rw-r--r--   0 miloniatal   (501) staff       (20)     2250 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/index.md
--rw-r--r--   0 miloniatal   (501) staff       (20)      765 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/make.bat
--rw-r--r--   0 miloniatal   (501) staff       (20)       85 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/modules.rst
--rw-r--r--   0 miloniatal   (501) staff       (20)     1195 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/terminal_tracker.rst
--rw-r--r--   0 miloniatal   (501) staff       (20)     2277 2023-05-03 23:00:34.000000 terminal_tracker-1.0.0/pyproject.toml
--rw-r--r--   0 miloniatal   (501) staff       (20)       38 2023-05-03 23:11:14.358374 terminal_tracker-1.0.0/setup.cfg
--rw-r--r--   0 miloniatal   (501) staff       (20)       56 2023-05-03 23:00:34.000000 terminal_tracker-1.0.0/setup.py
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.347124 terminal_tracker-1.0.0/terminal_tracker/
--rw-r--r--   0 miloniatal   (501) staff       (20)      231 2023-05-03 22:40:48.000000 terminal_tracker-1.0.0/terminal_tracker/__init__.py
--rw-r--r--   0 miloniatal   (501) staff       (20)       45 2023-03-23 23:29:05.000000 terminal_tracker-1.0.0/terminal_tracker/__main__.py
--rw-r--r--   0 miloniatal   (501) staff       (20)       22 2023-05-03 23:00:34.000000 terminal_tracker-1.0.0/terminal_tracker/_version.py
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.348758 terminal_tracker-1.0.0/terminal_tracker/configs/
--rw-r--r--   0 miloniatal   (501) staff       (20)      466 2023-02-17 18:38:31.000000 terminal_tracker-1.0.0/terminal_tracker/configs/configuring_bash.sh
--rw-r--r--   0 miloniatal   (501) staff       (20)      291 2023-02-18 20:35:46.000000 terminal_tracker-1.0.0/terminal_tracker/configs/configuring_zsh.sh
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.350397 terminal_tracker-1.0.0/terminal_tracker/examples/
--rw-r--r--   0 miloniatal   (501) staff       (20)     4707 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/examples/Frequency.ipynb
--rw-r--r--   0 miloniatal   (501) staff       (20)     2346 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/examples/Searching.ipynb
--rw-r--r--   0 miloniatal   (501) staff       (20)    13832 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/examples/TagTime.ipynb
--rw-r--r--   0 miloniatal   (501) staff       (20)     4657 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/export.py
--rw-r--r--   0 miloniatal   (501) staff       (20)     4502 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/frequency.py
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.356273 terminal_tracker-1.0.0/terminal_tracker/history_files/
--rw-r--r--   0 miloniatal   (501) staff       (20)     1973 2023-02-17 18:38:31.000000 terminal_tracker-1.0.0/terminal_tracker/history_files/bash_history.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)     2322 2023-02-18 20:35:46.000000 terminal_tracker-1.0.0/terminal_tracker/history_files/bash_history_timeframe.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)       97 2023-02-17 18:38:31.000000 terminal_tracker-1.0.0/terminal_tracker/history_files/storing_histfiles.sh
--rw-r--r--   0 miloniatal   (501) staff       (20)    33635 2023-02-18 20:35:46.000000 terminal_tracker-1.0.0/terminal_tracker/history_files/zsh_history.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)    15417 2023-02-18 20:35:46.000000 terminal_tracker-1.0.0/terminal_tracker/history_files/zsh_history_timeframe.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)     4416 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/preprocess.py
--rw-r--r--   0 miloniatal   (501) staff       (20)     1487 2023-05-03 22:40:48.000000 terminal_tracker-1.0.0/terminal_tracker/searching.py
--rw-r--r--   0 miloniatal   (501) staff       (20)     1298 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tag.py
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.357569 terminal_tracker-1.0.0/terminal_tracker/tests/
--rw-r--r--   0 miloniatal   (501) staff       (20)     4976 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tests/test_export.py
--rw-r--r--   0 miloniatal   (501) staff       (20)     4746 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tests/test_frequency.py
--rw-r--r--   0 miloniatal   (501) staff       (20)     3576 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tests/test_preprocess.py
--rw-r--r--   0 miloniatal   (501) staff       (20)     1836 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tests/test_searching.py
--rw-r--r--   0 miloniatal   (501) staff       (20)      520 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tests/test_tag.py
--rw-r--r--   0 miloniatal   (501) staff       (20)     2233 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tests/test_timeanalysis.py
--rw-r--r--   0 miloniatal   (501) staff       (20)      286 2023-03-23 23:29:05.000000 terminal_tracker-1.0.0/terminal_tracker/tests/zsh_test.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)     1177 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/timeanalysis.py
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.348299 terminal_tracker-1.0.0/terminal_tracker.egg-info/
--rw-r--r--   0 miloniatal   (501) staff       (20)     4955 2023-05-03 23:11:14.000000 terminal_tracker-1.0.0/terminal_tracker.egg-info/PKG-INFO
--rw-r--r--   0 miloniatal   (501) staff       (20)     1435 2023-05-03 23:11:14.000000 terminal_tracker-1.0.0/terminal_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)        1 2023-05-03 23:11:14.000000 terminal_tracker-1.0.0/terminal_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)      211 2023-05-03 23:11:14.000000 terminal_tracker-1.0.0/terminal_tracker.egg-info/requires.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)       17 2023-05-03 23:11:14.000000 terminal_tracker-1.0.0/terminal_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-11 15:14:43.365590 terminal_tracker-1.0.1/
+-rw-r--r--   0 miloniatal   (501) staff       (20)      401 2023-05-11 15:09:49.000000 terminal_tracker-1.0.1/.bumpversion.cfg
+-rw-r--r--   0 miloniatal   (501) staff       (20)       25 2023-03-23 23:29:05.000000 terminal_tracker-1.0.1/.coveragerc
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1319 2023-03-23 23:29:05.000000 terminal_tracker-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1068 2023-02-15 16:49:03.000000 terminal_tracker-1.0.1/LICENSE
+-rw-r--r--   0 miloniatal   (501) staff       (20)      552 2023-04-10 18:45:13.000000 terminal_tracker-1.0.1/MANIFEST.in
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2623 2023-04-04 22:56:49.000000 terminal_tracker-1.0.1/Makefile
+-rw-r--r--   0 miloniatal   (501) staff       (20)     5023 2023-05-11 15:14:43.365410 terminal_tracker-1.0.1/PKG-INFO
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2961 2023-05-11 14:52:19.000000 terminal_tracker-1.0.1/README.md
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-11 15:14:43.361154 terminal_tracker-1.0.1/docs/
+-rw-r--r--   0 miloniatal   (501) staff       (20)      634 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/docs/Makefile
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1653 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/docs/conf.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1818 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/docs/examples.md
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2250 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/docs/index.md
+-rw-r--r--   0 miloniatal   (501) staff       (20)      765 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/docs/make.bat
+-rw-r--r--   0 miloniatal   (501) staff       (20)       85 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/docs/modules.rst
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1195 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/docs/terminal_tracker.rst
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2299 2023-05-11 15:09:49.000000 terminal_tracker-1.0.1/pyproject.toml
+-rw-r--r--   0 miloniatal   (501) staff       (20)       38 2023-05-11 15:14:43.365633 terminal_tracker-1.0.1/setup.cfg
+-rw-r--r--   0 miloniatal   (501) staff       (20)       56 2023-05-11 15:09:49.000000 terminal_tracker-1.0.1/setup.py
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-11 15:14:43.362698 terminal_tracker-1.0.1/terminal_tracker/
+-rw-r--r--   0 miloniatal   (501) staff       (20)      231 2023-05-03 22:40:48.000000 terminal_tracker-1.0.1/terminal_tracker/__init__.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)       45 2023-03-23 23:29:05.000000 terminal_tracker-1.0.1/terminal_tracker/__main__.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)       22 2023-05-11 15:09:49.000000 terminal_tracker-1.0.1/terminal_tracker/_version.py
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-11 15:14:43.363847 terminal_tracker-1.0.1/terminal_tracker/examples/
+-rw-r--r--   0 miloniatal   (501) staff       (20)     3017 2023-05-11 15:09:49.000000 terminal_tracker-1.0.1/terminal_tracker/examples/Frequency.ipynb
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2665 2023-05-11 15:09:49.000000 terminal_tracker-1.0.1/terminal_tracker/examples/Searching.ipynb
+-rw-r--r--   0 miloniatal   (501) staff       (20)    13852 2023-05-11 15:09:49.000000 terminal_tracker-1.0.1/terminal_tracker/examples/TagTime.ipynb
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-11 15:14:43.364284 terminal_tracker-1.0.1/terminal_tracker/examples/history_files/
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1973 2023-05-11 14:52:19.000000 terminal_tracker-1.0.1/terminal_tracker/examples/history_files/bash_history.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2322 2023-05-11 14:52:19.000000 terminal_tracker-1.0.1/terminal_tracker/examples/history_files/bash_history_timeframe.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)    33635 2023-05-11 14:52:19.000000 terminal_tracker-1.0.1/terminal_tracker/examples/history_files/zsh_history.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4657 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/terminal_tracker/export.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4502 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/terminal_tracker/frequency.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4416 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/terminal_tracker/preprocess.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1487 2023-05-03 22:40:48.000000 terminal_tracker-1.0.1/terminal_tracker/searching.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1298 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/terminal_tracker/tag.py
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-11 15:14:43.365221 terminal_tracker-1.0.1/terminal_tracker/tests/
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4976 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/terminal_tracker/tests/test_export.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4746 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/terminal_tracker/tests/test_frequency.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     3576 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/terminal_tracker/tests/test_preprocess.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1836 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/terminal_tracker/tests/test_searching.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)      520 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/terminal_tracker/tests/test_tag.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2233 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/terminal_tracker/tests/test_timeanalysis.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)      286 2023-03-23 23:29:05.000000 terminal_tracker-1.0.1/terminal_tracker/tests/zsh_test.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1177 2023-05-03 22:41:16.000000 terminal_tracker-1.0.1/terminal_tracker/timeanalysis.py
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-11 15:14:43.363469 terminal_tracker-1.0.1/terminal_tracker.egg-info/
+-rw-r--r--   0 miloniatal   (501) staff       (20)     5023 2023-05-11 15:14:43.000000 terminal_tracker-1.0.1/terminal_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1264 2023-05-11 15:14:43.000000 terminal_tracker-1.0.1/terminal_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)        1 2023-05-11 15:14:43.000000 terminal_tracker-1.0.1/terminal_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)      226 2023-05-11 15:14:43.000000 terminal_tracker-1.0.1/terminal_tracker.egg-info/requires.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)       17 2023-05-11 15:14:43.000000 terminal_tracker-1.0.1/terminal_tracker.egg-info/top_level.txt
```

### Comparing `terminal_tracker-1.0.0/CONTRIBUTING.md` & `terminal_tracker-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/LICENSE` & `terminal_tracker-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/MANIFEST.in` & `terminal_tracker-1.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/Makefile` & `terminal_tracker-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/PKG-INFO` & `terminal_tracker-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal_tracker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Terminal command tracker
 Author-email: Miloni <miloniatal@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Miloni Atal
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,15 +40,15 @@
 Provides-Extra: develop
 License-File: LICENSE
 
 # terminal-tracker
 
 Maintaining and organizing a history of terminal commands executed for a folder/project from any terminal.
 
-![](https://img.shields.io/github/license/MiloniAtal/terminal-tracker)
+[![](https://img.shields.io/github/license/MiloniAtal/terminal-tracker)](https://github.com/MiloniAtal/terminal-tracker/blob/main/LICENSE)
 ![](https://img.shields.io/github/issues/MiloniAtal/terminal-tracker)
 [![Build Status](https://github.com/MiloniAtal/terminal-tracker/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/MiloniAtal/terminal-tracker/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/MiloniAtal/terminal-tracker/branch/main/graph/badge.svg)](https://codecov.io/gh/MiloniAtal/terminal-tracker)
 [![PyPI](https://img.shields.io/pypi/v/terminal-tracker)](https://pypi.org/project/terminal-tracker/)
 [![Documentation Status](https://readthedocs.org/projects/terminal-tracker/badge/?version=latest)](https://terminal-tracker.readthedocs.io/en/latest/?badge=latest)
     
 ## Overview
```

### Comparing `terminal_tracker-1.0.0/README.md` & `terminal_tracker-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # terminal-tracker
 
 Maintaining and organizing a history of terminal commands executed for a folder/project from any terminal.
 
-![](https://img.shields.io/github/license/MiloniAtal/terminal-tracker)
+[![](https://img.shields.io/github/license/MiloniAtal/terminal-tracker)](https://github.com/MiloniAtal/terminal-tracker/blob/main/LICENSE)
 ![](https://img.shields.io/github/issues/MiloniAtal/terminal-tracker)
 [![Build Status](https://github.com/MiloniAtal/terminal-tracker/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/MiloniAtal/terminal-tracker/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/MiloniAtal/terminal-tracker/branch/main/graph/badge.svg)](https://codecov.io/gh/MiloniAtal/terminal-tracker)
 [![PyPI](https://img.shields.io/pypi/v/terminal-tracker)](https://pypi.org/project/terminal-tracker/)
 [![Documentation Status](https://readthedocs.org/projects/terminal-tracker/badge/?version=latest)](https://terminal-tracker.readthedocs.io/en/latest/?badge=latest)
     
 ## Overview
```

### Comparing `terminal_tracker-1.0.0/docs/Makefile` & `terminal_tracker-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/docs/conf.py` & `terminal_tracker-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/docs/examples.md` & `terminal_tracker-1.0.1/docs/examples.md`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/docs/index.md` & `terminal_tracker-1.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/docs/make.bat` & `terminal_tracker-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/docs/terminal_tracker.rst` & `terminal_tracker-1.0.1/docs/terminal_tracker.rst`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/pyproject.toml` & `terminal_tracker-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "terminal_tracker"
 authors = [{name = "Miloni", email = "miloniatal@gmail.com"}]
 description="Terminal command tracker"
 readme = "README.md"
-version="1.0.0"
+version="1.0.1"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -48,15 +48,16 @@
     "pytest-cov>=2.6.1",
     "twine",
     "wheel",
     "pandas",
     "pytz",
     "sphinx",
     "recommonmark",
-    "sphinxcontrib-napoleon"
+    "sphinxcontrib-napoleon",
+    "black[jupyter]"
 ]
 
 [tool.black]
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
```

### Comparing `terminal_tracker-1.0.0/terminal_tracker/examples/Searching.ipynb` & `terminal_tracker-1.0.1/terminal_tracker/examples/Searching.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9799255952380952%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1, 'outputs': [OrderedDict([('name', 'stdout'), "*

 * *            "('output_type', 'stream'), ('text', ['Collecting terminal-tracker\\n', '  Using "*

 * *            "cached terminal_tracker-1.0.0-py3-none-any.whl (35 kB)\\n', 'Installing collected "*

 * *            "packages: terminal-tracker\\n', 'Successfully installed "*

 * *            "terminal-tracker-1.0.0\\n'])])]}, 1: {'execution_count': 2, 'source': {insert: [(1, "*

 * *            '\'\\n\'), (2, \'sf = SearchFile("history_files/bas […]*

```diff
@@ -1,31 +1,43 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Collecting terminal-tracker\n",
+                        "  Using cached terminal_tracker-1.0.0-py3-none-any.whl (35 kB)\n",
+                        "Installing collected packages: terminal-tracker\n",
+                        "Successfully installed terminal-tracker-1.0.0\n"
+                    ]
+                }
+            ],
             "source": [
                 "!pip install terminal-tracker"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from terminal_tracker import SearchFile\n",
-                "sf = SearchFile(\"../history_files/bash_history.txt\")"
+                "\n",
+                "sf = SearchFile(\"history_files/bash_history.txt\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "docker cp repo:/git/getting-started/ .\n",
@@ -34,20 +46,20 @@
                 }
             ],
             "source": [
                 "# Search for \"name\", get the list of commands\n",
                 "command_list = sf.find(\"git\")\n",
                 "\n",
                 "for c in set(command_list):\n",
-                "    print(c)\n"
+                "    print(c)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "docker cp repo:/git/getting-started/ .\n"
@@ -59,30 +71,30 @@
                 "command = sf.latest(\"git\")\n",
                 "\n",
                 "print(command)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "docker cp repo:/git/getting-started/ .\n",
                         "docker run --name repo alpine/git clone https://github.com/docker/getting-started.git\n"
                     ]
                 }
             ],
             "source": [
                 "# Using the latest iterator\n",
                 "for command in sf.latest_iterator(\"git\"):\n",
-                "   print(command)"
+                "    print(command)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.9.12 ('base')",
             "language": "python",
@@ -94,15 +106,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.16"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "bc18c4434ef79a9e109b03887c72545f896b56f238edb7d9b0f0df76d12bcf46"
             }
         }
```

### Comparing `terminal_tracker-1.0.0/terminal_tracker/examples/TagTime.ipynb` & `terminal_tracker-1.0.1/terminal_tracker/examples/TagTime.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9594128787878788%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1, 'outputs': [OrderedDict([('name', 'stdout'), "*

 * *            "('output_type', 'stream'), ('text', ['Requirement already satisfied: terminal-tracker "*

 * *            'in /Users/miloniatal/opt/anaconda3/envs/tt/lib/python3.9/site-packages '*

 * *            "(1.0.0)\\n'])])]}, 1: {'execution_count': 2, 'outputs': {0: {'execution_count': 2}}, "*

 * *            '\'source\': {insert: [(1, \'\\n\'), (2, \'tg = Tags("history_files/zsh_history.txt", '*

 * *            'timeframe=False, shell="z […]*

```diff
@@ -1,21 +1,29 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Requirement already satisfied: terminal-tracker in /Users/miloniatal/opt/anaconda3/envs/tt/lib/python3.9/site-packages (1.0.0)\n"
+                    ]
+                }
+            ],
             "source": [
                 "!pip install terminal-tracker"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -138,58 +146,59 @@
                             "938   trigram_model.py hw1_data/brown_train.txt hw1_...  NLP  \n",
                             "940   trigram_model.py hw1_data/brown_train.txt hw1_...  NLP  \n",
                             "942   trigram_model.py hw1_data/brown_train.txt hw1_...  NLP  \n",
                             "943   trigram_model.py hw1_data/brown_train.txt hw1_...  NLP  \n",
                             "1103  trigram_model.py hw1_data/brown_train.txt hw1_...  NLP  "
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from terminal_tracker import Tags\n",
-                "tg = Tags(\"../history_files/zsh_history.txt\", timeframe=False, shell=\"zsh\")\n",
+                "\n",
+                "tg = Tags(\"history_files/zsh_history.txt\", timeframe=False, shell=\"zsh\")\n",
                 "\n",
                 "# Search for \"project\", get the dataframe\n",
                 "nlp_df = tg.search_df(\"NLP\")\n",
                 "\n",
-                "nlp_df.head(10)\n"
+                "nlp_df.head(10)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "python trigram_mode.py hw1_data/brown_train.txt hw1_data/brown_test.txt #NLP\n",
-                        "python trigram_model2.py hw1_data/brown_train.txt hw1_data/brown_test.txt #NLP\n",
+                        "python -i trigram_model2.py hw1_data/brown_train.txt hw1_data/brown_test.txt #NLP\n",
                         "python -i trigram_model.py hw1_data/brown_test.txt #NLP\n",
+                        "python -i trigram_model2.py hw1_data/brown_train.txt hw1_data/brown_test.txt #NLP \n",
                         "python trigram_mode2.py hw1_data/brown_train.txt hw1_data/brown_test.txt #NLP\n",
-                        "python -i trigram_model2.py hw1_data/brown_train.txt hw1_data/brown_test.txt #NLP\n",
+                        "python trigram_model2.py hw1_data/brown_train.txt hw1_data/brown_test.txt #NLP\n",
                         "python trigram_model.py hw1_data/brown_train.txt hw1_data/brown_test.txt #NLP\n",
-                        "python -i trigram_model2.py hw1_data/brown_train.txt hw1_data/brown_test.txt #NLP \n"
+                        "python trigram_mode.py hw1_data/brown_train.txt hw1_data/brown_test.txt #NLP\n"
                     ]
                 }
             ],
             "source": [
                 "# Search for \"project\", get the commands\n",
                 "project_command_list = tg.search(\"NLP\")\n",
                 "for command in set(project_command_list):\n",
                 "    print(command)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -334,38 +343,29 @@
                             "5                  \n",
                             "6  ~/.bashrc       \n",
                             "7  ~/.bashrc       \n",
                             "8                  \n",
                             "9  ~/.bashrc       "
                         ]
                     },
-                    "execution_count": 29,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from terminal_tracker import TimeAnalysis\n",
-                "from IPython.utils import io\n",
                 "\n",
-                "with io.capture_output() as captured:\n",
-                "    tg = TimeAnalysis(\"../history_files/bash_history_timeframe.txt\",shell=\"bash\")\n",
+                "tg = TimeAnalysis(\"history_files/bash_history_timeframe.txt\", shell=\"bash\")\n",
                 "\n",
                 "# Search for \"2023-02-18\", get the dataframe\n",
                 "date_df = tg.search_day(\"2023-02-15\")\n",
                 "\n",
                 "date_df.head(10)"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.9.12 ('tt')",
             "language": "python",
             "name": "python3"
```

### Comparing `terminal_tracker-1.0.0/terminal_tracker/export.py` & `terminal_tracker-1.0.1/terminal_tracker/export.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/frequency.py` & `terminal_tracker-1.0.1/terminal_tracker/frequency.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/history_files/bash_history.txt` & `terminal_tracker-1.0.1/terminal_tracker/examples/history_files/bash_history.txt`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/history_files/bash_history_timeframe.txt` & `terminal_tracker-1.0.1/terminal_tracker/examples/history_files/bash_history_timeframe.txt`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/history_files/zsh_history.txt` & `terminal_tracker-1.0.1/terminal_tracker/examples/history_files/zsh_history.txt`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/preprocess.py` & `terminal_tracker-1.0.1/terminal_tracker/preprocess.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/searching.py` & `terminal_tracker-1.0.1/terminal_tracker/searching.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/tag.py` & `terminal_tracker-1.0.1/terminal_tracker/tag.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/tests/test_export.py` & `terminal_tracker-1.0.1/terminal_tracker/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/tests/test_frequency.py` & `terminal_tracker-1.0.1/terminal_tracker/tests/test_frequency.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/tests/test_preprocess.py` & `terminal_tracker-1.0.1/terminal_tracker/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/tests/test_searching.py` & `terminal_tracker-1.0.1/terminal_tracker/tests/test_searching.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/tests/test_tag.py` & `terminal_tracker-1.0.1/terminal_tracker/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/tests/test_timeanalysis.py` & `terminal_tracker-1.0.1/terminal_tracker/tests/test_timeanalysis.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker/timeanalysis.py` & `terminal_tracker-1.0.1/terminal_tracker/timeanalysis.py`

 * *Files identical despite different names*

### Comparing `terminal_tracker-1.0.0/terminal_tracker.egg-info/PKG-INFO` & `terminal_tracker-1.0.1/terminal_tracker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-tracker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Terminal command tracker
 Author-email: Miloni <miloniatal@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Miloni Atal
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,15 +40,15 @@
 Provides-Extra: develop
 License-File: LICENSE
 
 # terminal-tracker
 
 Maintaining and organizing a history of terminal commands executed for a folder/project from any terminal.
 
-![](https://img.shields.io/github/license/MiloniAtal/terminal-tracker)
+[![](https://img.shields.io/github/license/MiloniAtal/terminal-tracker)](https://github.com/MiloniAtal/terminal-tracker/blob/main/LICENSE)
 ![](https://img.shields.io/github/issues/MiloniAtal/terminal-tracker)
 [![Build Status](https://github.com/MiloniAtal/terminal-tracker/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/MiloniAtal/terminal-tracker/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/MiloniAtal/terminal-tracker/branch/main/graph/badge.svg)](https://codecov.io/gh/MiloniAtal/terminal-tracker)
 [![PyPI](https://img.shields.io/pypi/v/terminal-tracker)](https://pypi.org/project/terminal-tracker/)
 [![Documentation Status](https://readthedocs.org/projects/terminal-tracker/badge/?version=latest)](https://terminal-tracker.readthedocs.io/en/latest/?badge=latest)
     
 ## Overview
```

### Comparing `terminal_tracker-1.0.0/terminal_tracker.egg-info/SOURCES.txt` & `terminal_tracker-1.0.1/terminal_tracker.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,24 +24,20 @@
 terminal_tracker/tag.py
 terminal_tracker/timeanalysis.py
 terminal_tracker.egg-info/PKG-INFO
 terminal_tracker.egg-info/SOURCES.txt
 terminal_tracker.egg-info/dependency_links.txt
 terminal_tracker.egg-info/requires.txt
 terminal_tracker.egg-info/top_level.txt
-terminal_tracker/configs/configuring_bash.sh
-terminal_tracker/configs/configuring_zsh.sh
 terminal_tracker/examples/Frequency.ipynb
 terminal_tracker/examples/Searching.ipynb
 terminal_tracker/examples/TagTime.ipynb
-terminal_tracker/history_files/bash_history.txt
-terminal_tracker/history_files/bash_history_timeframe.txt
-terminal_tracker/history_files/storing_histfiles.sh
-terminal_tracker/history_files/zsh_history.txt
-terminal_tracker/history_files/zsh_history_timeframe.txt
+terminal_tracker/examples/history_files/bash_history.txt
+terminal_tracker/examples/history_files/bash_history_timeframe.txt
+terminal_tracker/examples/history_files/zsh_history.txt
 terminal_tracker/tests/test_export.py
 terminal_tracker/tests/test_frequency.py
 terminal_tracker/tests/test_preprocess.py
 terminal_tracker/tests/test_searching.py
 terminal_tracker/tests/test_tag.py
 terminal_tracker/tests/test_timeanalysis.py
 terminal_tracker/tests/zsh_test.txt
```

