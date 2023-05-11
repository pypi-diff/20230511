# Comparing `tmp/nl4dv-2.0.0.tar.gz` & `tmp/nl4dv-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nl4dv-2.0.0.tar", last modified: Wed Oct 19 11:34:17 2022, max compression
+gzip compressed data, was "nl4dv-2.1.0.tar", last modified: Thu May 11 00:01:01 2023, max compression
```

## Comparing `nl4dv-2.0.0.tar` & `nl4dv-2.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.129595 nl4dv-2.0.0/
--rw-r--r--   0 curiosity   (501) staff       (20)     1086 2022-09-17 21:53:11.000000 nl4dv-2.0.0/LICENSE
--rw-r--r--   0 curiosity   (501) staff       (20)        0 2022-09-17 21:53:11.000000 nl4dv-2.0.0/MANIFEST.in
--rw-r--r--   0 curiosity   (501) staff       (20)     4144 2022-10-19 11:34:17.127979 nl4dv-2.0.0/PKG-INFO
--rw-r--r--   0 curiosity   (501) staff       (20)     3183 2022-10-19 10:56:23.000000 nl4dv-2.0.0/README.md
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.108385 nl4dv-2.0.0/nl4dv/
--rw-r--r--   0 curiosity   (501) staff       (20)    32542 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/__init__.py
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.113991 nl4dv-2.0.0/nl4dv/attributegenie/
--rw-r--r--   0 curiosity   (501) staff       (20)       30 2022-09-17 21:53:12.000000 nl4dv-2.0.0/nl4dv/attributegenie/__init__.py
--rw-r--r--   0 curiosity   (501) staff       (20)    40524 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/attributegenie/attributegenie.py
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.114943 nl4dv-2.0.0/nl4dv/autogenie/
--rw-r--r--   0 curiosity   (501) staff       (20)       25 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/autogenie/__init__.py
--rw-r--r--   0 curiosity   (501) staff       (20)    10093 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/autogenie/autogenie.py
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.115735 nl4dv-2.0.0/nl4dv/conversationgenie/
--rw-r--r--   0 curiosity   (501) staff       (20)       33 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/conversationgenie/__init__.py
--rw-r--r--   0 curiosity   (501) staff       (20)    43911 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/conversationgenie/conversationgenie.py
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.116593 nl4dv-2.0.0/nl4dv/datagenie/
--rw-r--r--   0 curiosity   (501) staff       (20)       25 2022-09-17 21:53:12.000000 nl4dv-2.0.0/nl4dv/datagenie/__init__.py
--rw-r--r--   0 curiosity   (501) staff       (20)    16867 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/datagenie/datagenie.py
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.118747 nl4dv-2.0.0/nl4dv/querygenie/
--rw-r--r--   0 curiosity   (501) staff       (20)       26 2022-09-17 21:53:12.000000 nl4dv-2.0.0/nl4dv/querygenie/__init__.py
--rw-r--r--   0 curiosity   (501) staff       (20)     2994 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/querygenie/querygenie.py
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.119576 nl4dv-2.0.0/nl4dv/taskgenie/
--rw-r--r--   0 curiosity   (501) staff       (20)       25 2022-09-17 21:53:12.000000 nl4dv-2.0.0/nl4dv/taskgenie/__init__.py
--rw-r--r--   0 curiosity   (501) staff       (20)    37454 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/taskgenie/taskgenie.py
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.120758 nl4dv-2.0.0/nl4dv/tests/
--rw-r--r--   0 curiosity   (501) staff       (20)        0 2022-09-17 21:53:12.000000 nl4dv-2.0.0/nl4dv/tests/__init__.py
--rw-r--r--   0 curiosity   (501) staff       (20)     6571 2022-09-17 21:53:12.000000 nl4dv-2.0.0/nl4dv/tests/test_data_summary.py
--rw-r--r--   0 curiosity   (501) staff       (20)     3039 2022-09-17 21:53:12.000000 nl4dv-2.0.0/nl4dv/tests/test_queries.py
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.121516 nl4dv-2.0.0/nl4dv/updategenie/
--rw-r--r--   0 curiosity   (501) staff       (20)       27 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/updategenie/__init__.py
--rw-r--r--   0 curiosity   (501) staff       (20)     8868 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/updategenie/updategenie.py
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.123000 nl4dv-2.0.0/nl4dv/utils/
--rw-r--r--   0 curiosity   (501) staff       (20)        0 2022-09-17 21:53:12.000000 nl4dv-2.0.0/nl4dv/utils/__init__.py
--rw-r--r--   0 curiosity   (501) staff       (20)    11386 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/utils/constants.py
--rw-r--r--   0 curiosity   (501) staff       (20)      251 2022-09-17 21:53:12.000000 nl4dv-2.0.0/nl4dv/utils/error_codes.py
--rw-r--r--   0 curiosity   (501) staff       (20)     6220 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/utils/helpers.py
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.124805 nl4dv-2.0.0/nl4dv/visgenie/
--rw-r--r--   0 curiosity   (501) staff       (20)       49 2022-09-17 21:53:12.000000 nl4dv-2.0.0/nl4dv/visgenie/__init__.py
--rw-r--r--   0 curiosity   (501) staff       (20)    49256 2022-10-18 01:24:02.000000 nl4dv-2.0.0/nl4dv/visgenie/vis_recos.py
--rw-r--r--   0 curiosity   (501) staff       (20)    23809 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/visgenie/visgenie.py
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.126604 nl4dv-2.0.0/nl4dv/vlgenie/
--rw-r--r--   0 curiosity   (501) staff       (20)       23 2022-09-17 21:53:12.000000 nl4dv-2.0.0/nl4dv/vlgenie/__init__.py
--rw-r--r--   0 curiosity   (501) staff       (20)     8770 2022-10-19 02:44:22.000000 nl4dv-2.0.0/nl4dv/vlgenie/vlgenie.py
-drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2022-10-19 11:34:17.112629 nl4dv-2.0.0/nl4dv.egg-info/
--rw-r--r--   0 curiosity   (501) staff       (20)     4144 2022-10-19 11:34:17.000000 nl4dv-2.0.0/nl4dv.egg-info/PKG-INFO
--rw-r--r--   0 curiosity   (501) staff       (20)      964 2022-10-19 11:34:17.000000 nl4dv-2.0.0/nl4dv.egg-info/SOURCES.txt
--rw-r--r--   0 curiosity   (501) staff       (20)        1 2022-10-19 11:34:17.000000 nl4dv-2.0.0/nl4dv.egg-info/dependency_links.txt
--rw-r--r--   0 curiosity   (501) staff       (20)      141 2022-10-19 11:34:17.000000 nl4dv-2.0.0/nl4dv.egg-info/requires.txt
--rw-r--r--   0 curiosity   (501) staff       (20)        6 2022-10-19 11:34:17.000000 nl4dv-2.0.0/nl4dv.egg-info/top_level.txt
--rw-r--r--   0 curiosity   (501) staff       (20)       38 2022-10-19 11:34:17.129789 nl4dv-2.0.0/setup.cfg
--rw-r--r--   0 curiosity   (501) staff       (20)     1218 2022-10-19 10:57:22.000000 nl4dv-2.0.0/setup.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.740490 nl4dv-2.1.0/
+-rw-r--r--   0 curiosity   (501) staff       (20)     1086 2020-09-30 15:11:37.000000 nl4dv-2.1.0/LICENSE
+-rw-r--r--   0 curiosity   (501) staff       (20)        0 2020-09-16 16:10:40.000000 nl4dv-2.1.0/MANIFEST.in
+-rw-r--r--   0 curiosity   (501) staff       (20)     3705 2023-05-11 00:01:01.739243 nl4dv-2.1.0/PKG-INFO
+-rw-r--r--   0 curiosity   (501) staff       (20)     3233 2023-05-10 23:52:20.000000 nl4dv-2.1.0/README.md
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.687639 nl4dv-2.1.0/nl4dv/
+-rw-r--r--   0 curiosity   (501) staff       (20)    32542 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/__init__.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.699382 nl4dv-2.1.0/nl4dv/attributegenie/
+-rw-r--r--   0 curiosity   (501) staff       (20)       30 2020-09-16 16:10:40.000000 nl4dv-2.1.0/nl4dv/attributegenie/__init__.py
+-rw-r--r--   0 curiosity   (501) staff       (20)    40704 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/attributegenie/attributegenie.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.703156 nl4dv-2.1.0/nl4dv/autogenie/
+-rw-r--r--   0 curiosity   (501) staff       (20)       25 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/autogenie/__init__.py
+-rw-r--r--   0 curiosity   (501) staff       (20)    10093 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/autogenie/autogenie.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.705798 nl4dv-2.1.0/nl4dv/conversationgenie/
+-rw-r--r--   0 curiosity   (501) staff       (20)       33 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/conversationgenie/__init__.py
+-rw-r--r--   0 curiosity   (501) staff       (20)    43911 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/conversationgenie/conversationgenie.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.708505 nl4dv-2.1.0/nl4dv/datagenie/
+-rw-r--r--   0 curiosity   (501) staff       (20)       25 2020-09-16 16:10:40.000000 nl4dv-2.1.0/nl4dv/datagenie/__init__.py
+-rw-r--r--   0 curiosity   (501) staff       (20)    16867 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/datagenie/datagenie.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.713450 nl4dv-2.1.0/nl4dv/querygenie/
+-rw-r--r--   0 curiosity   (501) staff       (20)       26 2020-09-16 16:10:40.000000 nl4dv-2.1.0/nl4dv/querygenie/__init__.py
+-rw-r--r--   0 curiosity   (501) staff       (20)     2994 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/querygenie/querygenie.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.717073 nl4dv-2.1.0/nl4dv/taskgenie/
+-rw-r--r--   0 curiosity   (501) staff       (20)       25 2020-09-16 16:10:40.000000 nl4dv-2.1.0/nl4dv/taskgenie/__init__.py
+-rw-r--r--   0 curiosity   (501) staff       (20)    37454 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/taskgenie/taskgenie.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.720825 nl4dv-2.1.0/nl4dv/tests/
+-rw-r--r--   0 curiosity   (501) staff       (20)        0 2020-09-16 16:10:40.000000 nl4dv-2.1.0/nl4dv/tests/__init__.py
+-rw-r--r--   0 curiosity   (501) staff       (20)     6571 2020-09-16 16:10:40.000000 nl4dv-2.1.0/nl4dv/tests/test_data_summary.py
+-rw-r--r--   0 curiosity   (501) staff       (20)     3039 2020-12-22 17:22:45.000000 nl4dv-2.1.0/nl4dv/tests/test_queries.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.723399 nl4dv-2.1.0/nl4dv/updategenie/
+-rw-r--r--   0 curiosity   (501) staff       (20)       27 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/updategenie/__init__.py
+-rw-r--r--   0 curiosity   (501) staff       (20)     8868 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/updategenie/updategenie.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.728786 nl4dv-2.1.0/nl4dv/utils/
+-rw-r--r--   0 curiosity   (501) staff       (20)        0 2020-09-16 16:10:40.000000 nl4dv-2.1.0/nl4dv/utils/__init__.py
+-rw-r--r--   0 curiosity   (501) staff       (20)    11386 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/utils/constants.py
+-rw-r--r--   0 curiosity   (501) staff       (20)      251 2020-09-16 16:10:40.000000 nl4dv-2.1.0/nl4dv/utils/error_codes.py
+-rw-r--r--   0 curiosity   (501) staff       (20)     6247 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/utils/helpers.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.734424 nl4dv-2.1.0/nl4dv/visgenie/
+-rw-r--r--   0 curiosity   (501) staff       (20)       49 2020-09-16 16:10:40.000000 nl4dv-2.1.0/nl4dv/visgenie/__init__.py
+-rw-r--r--   0 curiosity   (501) staff       (20)    49256 2020-12-23 05:22:55.000000 nl4dv-2.1.0/nl4dv/visgenie/vis_recos.py
+-rw-r--r--   0 curiosity   (501) staff       (20)    23809 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/visgenie/visgenie.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.737913 nl4dv-2.1.0/nl4dv/vlgenie/
+-rw-r--r--   0 curiosity   (501) staff       (20)       23 2020-09-16 16:10:40.000000 nl4dv-2.1.0/nl4dv/vlgenie/__init__.py
+-rw-r--r--   0 curiosity   (501) staff       (20)     8770 2023-05-10 23:52:20.000000 nl4dv-2.1.0/nl4dv/vlgenie/vlgenie.py
+drwxr-xr-x   0 curiosity   (501) staff       (20)        0 2023-05-11 00:01:01.695715 nl4dv-2.1.0/nl4dv.egg-info/
+-rw-r--r--   0 curiosity   (501) staff       (20)     3705 2023-05-11 00:01:01.000000 nl4dv-2.1.0/nl4dv.egg-info/PKG-INFO
+-rw-r--r--   0 curiosity   (501) staff       (20)      964 2023-05-11 00:01:01.000000 nl4dv-2.1.0/nl4dv.egg-info/SOURCES.txt
+-rw-r--r--   0 curiosity   (501) staff       (20)        1 2023-05-11 00:01:01.000000 nl4dv-2.1.0/nl4dv.egg-info/dependency_links.txt
+-rw-r--r--   0 curiosity   (501) staff       (20)      141 2023-05-11 00:01:01.000000 nl4dv-2.1.0/nl4dv.egg-info/requires.txt
+-rw-r--r--   0 curiosity   (501) staff       (20)        6 2023-05-11 00:01:01.000000 nl4dv-2.1.0/nl4dv.egg-info/top_level.txt
+-rw-r--r--   0 curiosity   (501) staff       (20)       38 2023-05-11 00:01:01.741170 nl4dv-2.1.0/setup.cfg
+-rw-r--r--   0 curiosity   (501) staff       (20)     1218 2023-05-10 23:53:55.000000 nl4dv-2.1.0/setup.py
```

### Comparing `nl4dv-2.0.0/LICENSE` & `nl4dv-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/README.md` & `nl4dv-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # NL4DV: **N**atural **L**anguage toolkit **for** **D**ata **V**isualization
 [![DOI:10.1109/TVCG.2020.3030418](https://zenodo.org/badge/DOI/10.1109/TVCG.2020.3030378.svg)](https://doi.org/10.1109/TVCG.2020.3030378)
 [![arxiv badge](https://img.shields.io/badge/arXiv-2008.10723-red)](https://arxiv.org/abs/2008.10723)
 [![arxiv badge](https://img.shields.io/badge/arXiv-2207.00189-%23B31B1B)](https://arxiv.org/abs/2207.00189)
-[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
+[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/nl4dv/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/nl4dv)
 
 
 **NL4DV** takes a **natural language query** about a given **dataset** as input and outputs a **structured JSON object** containing:
 * Data attributes,
 * Analytic tasks, and
 * Visualizations (Vega-Lite specifications)
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 # NL4DV: **N**atural **L**anguage toolkit **for** **D**ata **V**isualization [!
 [DOI:10.1109/TVCG.2020.3030418](https://zenodo.org/badge/DOI/10.1109/
 TVCG.2020.3030378.svg)](https://doi.org/10.1109/TVCG.2020.3030378) [![arxiv
 badge](https://img.shields.io/badge/arXiv-2008.10723-red)](https://arxiv.org/
 abs/2008.10723) [![arxiv badge](https://img.shields.io/badge/arXiv-2207.00189-
 %23B31B1B)](https://arxiv.org/abs/2207.00189) [![PyPI license](https://
-img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/
-ansicolortags/) **NL4DV** takes a **natural language query** about a given
-**dataset** as input and outputs a **structured JSON object** containing: *
-Data attributes, * Analytic tasks, and * Visualizations (Vega-Lite
-specifications) With this output, developers can - Create visualizations in
-Python using natural language, and/or - Add a natural language interface to
-their existing visualization systems. ![NL4DV Overview](https://
-raw.githubusercontent.com/nl4dv/nl4dv/master/overview.gif) ### Setup
+img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/nl4dv/
+) ![PyPI - Downloads](https://img.shields.io/pypi/dm/nl4dv) **NL4DV** takes a
+**natural language query** about a given **dataset** as input and outputs a
+**structured JSON object** containing: * Data attributes, * Analytic tasks, and
+* Visualizations (Vega-Lite specifications) With this output, developers can -
+Create visualizations in Python using natural language, and/or - Add a natural
+language interface to their existing visualization systems. ![NL4DV Overview]
+(https://raw.githubusercontent.com/nl4dv/nl4dv/master/overview.gif) ### Setup
 Instructions, API Documentation, and Examples These can all be found on
 [NL4DV's project website](https://nl4dv.github.io/nl4dv/documentation.html).
 ### Credits NL4DV was created by Arpit_Narechania, Arjun_Srinivasan, Rishab
 Mitra, Alex_Endert, and John_Stasko of the Georgia_Tech_Visualization_Lab. We
 thank the members of the Georgia_Tech_Visualization_Lab for their support and
 constructive feedback.
 ### Citations #### 2020 IEEE TVCG Journal Full Paper (Proceedings of the 2020
```

### Comparing `nl4dv-2.0.0/nl4dv/__init__.py` & `nl4dv-2.1.0/nl4dv/__init__.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv/attributegenie/attributegenie.py` & `nl4dv-2.1.0/nl4dv/attributegenie/attributegenie.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,17 +289,18 @@
 
         value_keyword_mapping = dict()
         keyword_value_mapping = dict()
 
         for attr in data_attributes:
 
             # NL4DV does not look for domain value matches in the Label Attribute. Controversial, but that's how we've designed this.
-            # Update: Since the addition of two Checks below (similarity score and number_of_words matched) for a domain value match, this is NOT required.
-            # if attr == self.nl4dv_instance.label_attribute:
-            #     continue
+            # Update 1: Since the addition of two Checks below (similarity score and number_of_words matched) for a domain value match, this is NOT required.
+            # Update 2: Reverting the uncommented state of this conditional because it was breaking simple query like "What are the average budgets for action and adventure movies?"
+            if attr == self.nl4dv_instance.label_attribute:
+                continue
 
             # Look for domain value matches ONLY for ordinal and nominal variables.
             # For timeseries and quantitative  attribute types, it is difficult to map numbers to attributes AND this is computationally inefficient due to their domain size.
             if self.nl4dv_instance.data_genie_instance.data_attribute_map[attr]["dataType"] in ['Q','T']:
                 continue
 
             # RESET for each Attribute
```

### Comparing `nl4dv-2.0.0/nl4dv/autogenie/autogenie.py` & `nl4dv-2.1.0/nl4dv/autogenie/autogenie.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv/conversationgenie/conversationgenie.py` & `nl4dv-2.1.0/nl4dv/conversationgenie/conversationgenie.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv/datagenie/datagenie.py` & `nl4dv-2.1.0/nl4dv/datagenie/datagenie.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv/querygenie/querygenie.py` & `nl4dv-2.1.0/nl4dv/querygenie/querygenie.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv/taskgenie/taskgenie.py` & `nl4dv-2.1.0/nl4dv/taskgenie/taskgenie.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv/tests/test_data_summary.py` & `nl4dv-2.1.0/nl4dv/tests/test_data_summary.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv/tests/test_queries.py` & `nl4dv-2.1.0/nl4dv/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv/updategenie/updategenie.py` & `nl4dv-2.1.0/nl4dv/updategenie/updategenie.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv/utils/constants.py` & `nl4dv-2.1.0/nl4dv/utils/constants.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv/utils/helpers.py` & `nl4dv-2.1.0/nl4dv/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from nltk.corpus import wordnet as wn
 from itertools import product
 import math
-from collections import Counter, MutableMapping
+from collections import Counter
+from collections.abc import MutableMapping
 from fuzzywuzzy import fuzz
 import Levenshtein
 from datetime import date, datetime
 import copy
 from nl4dv.utils import constants
 import json
```

### Comparing `nl4dv-2.0.0/nl4dv/visgenie/vis_recos.py` & `nl4dv-2.1.0/nl4dv/visgenie/vis_recos.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv/visgenie/visgenie.py` & `nl4dv-2.1.0/nl4dv/visgenie/visgenie.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv/vlgenie/vlgenie.py` & `nl4dv-2.1.0/nl4dv/vlgenie/vlgenie.py`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/nl4dv.egg-info/SOURCES.txt` & `nl4dv-2.1.0/nl4dv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nl4dv-2.0.0/setup.py` & `nl4dv-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # read the contents of the README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nl4dv',
-    version='2.0.0',
+    version='2.1.0',
     author='Arpit Narechania',
     author_email='arpitnarechania@gatech.edu',
     packages=find_packages(),
     include_package_data=True,
     setup_requires=['pytest-runner'],
     test_requires=['pytest', 'pytest-cov'],
     scripts=[],
@@ -24,12 +24,12 @@
     install_requires=[
         "fuzzywuzzy~=0.8.1",
         "nltk~=3.5",
         "pytest~=3.10.1",
         "pytest-cov~=2.6.0",
         "python-Levenshtein~=0.12.0",
         "si-prefix~=1.2.2",
-        "spacy~=2.2",
+        "spacy~=3.0",
         "vega~=3.1",
         "inflect~=5.5.2"
     ]
 )
```

