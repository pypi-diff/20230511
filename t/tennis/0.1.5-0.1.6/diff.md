# Comparing `tmp/tennis-0.1.5.tar.gz` & `tmp/tennis-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tennis-0.1.5.tar", last modified: Thu May 11 03:49:47 2023, max compression
+gzip compressed data, was "tennis-0.1.6.tar", last modified: Thu May 11 03:53:15 2023, max compression
```

## Comparing `tennis-0.1.5.tar` & `tennis-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 03:49:47.274431 tennis-0.1.5/
--rw-rw-rw-   0        0        0     1083 2023-05-09 03:08:15.000000 tennis-0.1.5/LICENSE
--rw-rw-rw-   0        0        0    16120 2023-05-11 03:49:47.274431 tennis-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    15633 2023-05-11 03:44:22.000000 tennis-0.1.5/README.md
--rw-rw-rw-   0        0        0      516 2023-05-11 03:49:17.000000 tennis-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 03:49:47.276430 tennis-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      330 2023-05-11 03:49:14.000000 tennis-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 03:49:47.262426 tennis-0.1.5/tennis/
--rw-rw-rw-   0        0        0        0 2023-05-06 20:11:19.000000 tennis-0.1.5/tennis/__init__.py
--rw-rw-rw-   0        0        0    30931 2023-05-11 01:21:55.000000 tennis-0.1.5/tennis/match.py
--rw-rw-rw-   0        0        0    17036 2023-05-10 21:30:40.000000 tennis-0.1.5/tennis/tiebreak.py
-drwxrwxrwx   0        0        0        0 2023-05-11 03:49:47.274431 tennis-0.1.5/tennis.egg-info/
--rw-rw-rw-   0        0        0    16120 2023-05-11 03:49:47.000000 tennis-0.1.5/tennis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-05-11 03:49:47.000000 tennis-0.1.5/tennis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 03:49:47.000000 tennis-0.1.5/tennis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-11 03:49:47.000000 tennis-0.1.5/tennis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 03:53:15.639835 tennis-0.1.6/
+-rw-rw-rw-   0        0        0     1083 2023-05-09 03:08:15.000000 tennis-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0    16127 2023-05-11 03:53:15.638837 tennis-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    15640 2023-05-11 03:52:36.000000 tennis-0.1.6/README.md
+-rw-rw-rw-   0        0        0      516 2023-05-11 03:53:02.000000 tennis-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 03:53:15.639835 tennis-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      330 2023-05-11 03:52:59.000000 tennis-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 03:53:15.620370 tennis-0.1.6/tennis/
+-rw-rw-rw-   0        0        0        0 2023-05-06 20:11:19.000000 tennis-0.1.6/tennis/__init__.py
+-rw-rw-rw-   0        0        0    30931 2023-05-11 01:21:55.000000 tennis-0.1.6/tennis/match.py
+-rw-rw-rw-   0        0        0    17036 2023-05-10 21:30:40.000000 tennis-0.1.6/tennis/tiebreak.py
+drwxrwxrwx   0        0        0        0 2023-05-11 03:53:15.636847 tennis-0.1.6/tennis.egg-info/
+-rw-rw-rw-   0        0        0    16127 2023-05-11 03:53:15.000000 tennis-0.1.6/tennis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-05-11 03:53:15.000000 tennis-0.1.6/tennis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 03:53:15.000000 tennis-0.1.6/tennis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 03:53:15.000000 tennis-0.1.6/tennis.egg-info/top_level.txt
```

### Comparing `tennis-0.1.5/LICENSE` & `tennis-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tennis-0.1.5/PKG-INFO` & `tennis-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tennis
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library for tracking tennis matches and scoring
 Home-page: https://github.com/bear102/tennis
 Author: bear102
 License: MIT
 Project-URL: Homepage, https://github.com/bear102/tennis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tennis Library
 [![PyPI](https://img.shields.io/pypi/v/tennis)](https://pypi.org/project/tennis/)
-[![GitHub](https://img.shields.io/badge/GitHub-bear102-%2312100E.svg?style=flat&logo=github)](https://github.com/bear102)
+[![GitHub](https://img.shields.io/badge/GitHub-bear102-%2312100E.svg?style=flat&logo=github)](https://github.com/bear102/tennis)
 ![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 The Tennis library is a Python package that provides functionalities for simulating tennis matches and tiebreakers. It offers easy-to-use methods to simulate and track scores, tiebreakers, and various statistics. The tennis library is perfect for tracking real time data input.
 
 <br>
```

### Comparing `tennis-0.1.5/README.md` & `tennis-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Tennis Library
 [![PyPI](https://img.shields.io/pypi/v/tennis)](https://pypi.org/project/tennis/)
-[![GitHub](https://img.shields.io/badge/GitHub-bear102-%2312100E.svg?style=flat&logo=github)](https://github.com/bear102)
+[![GitHub](https://img.shields.io/badge/GitHub-bear102-%2312100E.svg?style=flat&logo=github)](https://github.com/bear102/tennis)
 ![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 The Tennis library is a Python package that provides functionalities for simulating tennis matches and tiebreakers. It offers easy-to-use methods to simulate and track scores, tiebreakers, and various statistics. The tennis library is perfect for tracking real time data input.
 
 <br>
```

### Comparing `tennis-0.1.5/pyproject.toml` & `tennis-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tennis"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="bear102" },
 ]
 description = "A library for tracking tennis matches and scoring"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tennis-0.1.5/tennis/match.py` & `tennis-0.1.6/tennis/match.py`

 * *Files identical despite different names*

### Comparing `tennis-0.1.5/tennis/tiebreak.py` & `tennis-0.1.6/tennis/tiebreak.py`

 * *Files identical despite different names*

### Comparing `tennis-0.1.5/tennis.egg-info/PKG-INFO` & `tennis-0.1.6/tennis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tennis
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library for tracking tennis matches and scoring
 Home-page: https://github.com/bear102/tennis
 Author: bear102
 License: MIT
 Project-URL: Homepage, https://github.com/bear102/tennis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tennis Library
 [![PyPI](https://img.shields.io/pypi/v/tennis)](https://pypi.org/project/tennis/)
-[![GitHub](https://img.shields.io/badge/GitHub-bear102-%2312100E.svg?style=flat&logo=github)](https://github.com/bear102)
+[![GitHub](https://img.shields.io/badge/GitHub-bear102-%2312100E.svg?style=flat&logo=github)](https://github.com/bear102/tennis)
 ![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 The Tennis library is a Python package that provides functionalities for simulating tennis matches and tiebreakers. It offers easy-to-use methods to simulate and track scores, tiebreakers, and various statistics. The tennis library is perfect for tracking real time data input.
 
 <br>
```

