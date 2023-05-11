# Comparing `tmp/AdsorptionBreakthroughAnalysis-0.0.1.tar.gz` & `tmp/AdsorptionBreakthroughAnalysis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/Fergus#/Dropbox (Heriot-Watt University Team)/RCCS_Capture_Fergus Mcilwaine/Projects/Daniel_exp_data/Adsorption_Br", last modified: Fri Sep  9 13:44:14 2022, max compression
+gzip compressed data, was "AdsorptionBreakthroughAnalysis-0.0.2.tar", last modified: Thu May 11 12:49:56 2023, max compression
```

## Comparing `AdsorptionBreakthroughAnalysis-0.0.1.tar` & `AdsorptionBreakthroughAnalysis-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,46 @@
-drwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)        0 2022-09-09 13:44:15.824004 AdsorptionBreakthroughAnalysis-0.0.1/
--rwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)     1073 2022-09-08 12:25:17.000000 AdsorptionBreakthroughAnalysis-0.0.1/LICENSE
--rwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)     1881 2022-09-09 13:44:15.819009 AdsorptionBreakthroughAnalysis-0.0.1/PKG-INFO
--rwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)     2443 2022-09-09 13:40:10.000000 AdsorptionBreakthroughAnalysis-0.0.1/README.md
--rwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)      918 2022-09-09 13:42:01.000000 AdsorptionBreakthroughAnalysis-0.0.1/pyproject.toml
--rwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)       38 2022-09-09 13:44:15.826007 AdsorptionBreakthroughAnalysis-0.0.1/setup.cfg
-drwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)        0 2022-09-09 13:44:15.257009 AdsorptionBreakthroughAnalysis-0.0.1/src/
-drwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)        0 2022-09-09 13:44:15.465008 AdsorptionBreakthroughAnalysis-0.0.1/src/AdsorptionBreakthroughAnalysis/
--rwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)        0 2022-09-08 12:27:44.000000 AdsorptionBreakthroughAnalysis-0.0.1/src/AdsorptionBreakthroughAnalysis/__init__.py
--rwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)    38050 2022-09-08 12:44:14.000000 AdsorptionBreakthroughAnalysis-0.0.1/src/AdsorptionBreakthroughAnalysis/breakthrough_analysis.py
-drwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)        0 2022-09-09 13:44:15.771005 AdsorptionBreakthroughAnalysis-0.0.1/src/AdsorptionBreakthroughAnalysis.egg-info/
--rwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)     1881 2022-09-09 13:44:15.000000 AdsorptionBreakthroughAnalysis-0.0.1/src/AdsorptionBreakthroughAnalysis.egg-info/PKG-INFO
--rwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)      428 2022-09-09 13:44:15.000000 AdsorptionBreakthroughAnalysis-0.0.1/src/AdsorptionBreakthroughAnalysis.egg-info/SOURCES.txt
--rwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)        1 2022-09-09 13:44:15.000000 AdsorptionBreakthroughAnalysis-0.0.1/src/AdsorptionBreakthroughAnalysis.egg-info/dependency_links.txt
--rwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)       91 2022-09-09 13:44:15.000000 AdsorptionBreakthroughAnalysis-0.0.1/src/AdsorptionBreakthroughAnalysis.egg-info/requires.txt
--rwxrwxrwx   0 frlmcilwaine  (1000) frlmcilwaine  (1000)       31 2022-09-09 13:44:15.000000 AdsorptionBreakthroughAnalysis-0.0.1/src/AdsorptionBreakthroughAnalysis.egg-info/top_level.txt
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-11 12:49:56.514659 AdsorptionBreakthroughAnalysis-0.0.2/
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     1079 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.2/LICENSE
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      475 2023-04-18 12:58:36.000000 AdsorptionBreakthroughAnalysis-0.0.2/MANIFEST.in
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)    10245 2023-05-11 12:49:56.514659 AdsorptionBreakthroughAnalysis-0.0.2/PKG-INFO
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     8779 2023-04-17 22:20:14.000000 AdsorptionBreakthroughAnalysis-0.0.2/README.md
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-11 12:49:56.494659 AdsorptionBreakthroughAnalysis-0.0.2/docs/
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-11 12:49:56.498659 AdsorptionBreakthroughAnalysis-0.0.2/docs/source/
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      331 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.2/docs/source/cli.rst
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     7505 2023-05-03 17:22:53.000000 AdsorptionBreakthroughAnalysis-0.0.2/docs/source/conf.py
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     1851 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.2/docs/source/index.rst
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      645 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.2/docs/source/installation.rst
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       77 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.2/docs/source/usage.rst
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      377 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.2/pyproject.toml
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)     2780 2023-05-11 12:49:56.514659 AdsorptionBreakthroughAnalysis-0.0.2/setup.cfg
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-11 12:49:56.494659 AdsorptionBreakthroughAnalysis-0.0.2/src/
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-11 12:49:56.498659 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis/
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)      336 2023-05-04 20:07:31.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis/__init__.py
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      347 2023-04-18 13:14:08.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis/__main__.py
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       42 2023-04-17 22:04:29.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis/api.py
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)    53750 2023-05-11 12:26:15.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis/breakthrough_analysis.py
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      979 2023-04-18 13:10:35.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis/cli.py
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)        1 2023-04-17 22:04:29.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis/py.typed
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     1096 2023-05-03 17:22:53.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis/version.py
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-11 12:49:56.502658 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis.egg-info/
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)    10245 2023-05-11 12:49:56.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)     1586 2023-05-11 12:49:56.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)        1 2023-05-11 12:49:56.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       91 2023-05-11 12:49:56.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis.egg-info/entry_points.txt
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)        1 2023-05-11 12:45:00.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis.egg-info/not-zip-safe
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)      182 2023-05-11 12:49:56.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis.egg-info/requires.txt
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       31 2023-05-11 12:49:56.000000 AdsorptionBreakthroughAnalysis-0.0.2/src/AdsorptionBreakthroughAnalysis.egg-info/top_level.txt
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-11 12:49:56.502658 AdsorptionBreakthroughAnalysis-0.0.2/tests/
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       64 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.2/tests/__init__.py
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-11 12:49:56.498659 AdsorptionBreakthroughAnalysis-0.0.2/tests/data/
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-11 12:49:56.506659 AdsorptionBreakthroughAnalysis-0.0.2/tests/data/experimental_data/
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)  8324734 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.2/tests/data/experimental_data/220819-ZIF-8-dry-22%and60%40C20220819134938.txt
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)    35453 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.2/tests/data/experimental_data/220819ZIF8Blank22and60%CO2at40C.csv
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)    81913 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.2/tests/data/experimental_data/220824-ZIF-8-4and22%at40C.csv
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003) 18648765 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.2/tests/data/experimental_data/220824-ZIF-8-4and22%at40C.txt
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-11 12:49:56.514659 AdsorptionBreakthroughAnalysis-0.0.2/tests/data/processed_data/
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)    85579 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.2/tests/data/processed_data/bench_220819-ZIF-8-dry-22%and60%40C20220819134938.txt_220819ZIF8Blank22and60%CO2at40C.csv.csv
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)   113867 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.2/tests/data/processed_data/bench_220824-ZIF-8-4and22%at40C.txt_220824-ZIF-8-4and22%at40C.csv.csv
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      371 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.2/tests/data/processed_data/bench_loading_experiment_22perc_ZIF8.pickle
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      371 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.2/tests/data/processed_data/bench_loading_experiment_22perc_ZIF8_blank.pickle
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     5248 2023-04-18 13:04:06.000000 AdsorptionBreakthroughAnalysis-0.0.2/tests/test_results.py
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      640 2023-04-18 12:35:25.000000 AdsorptionBreakthroughAnalysis-0.0.2/tests/test_version.py
```

### Comparing `AdsorptionBreakthroughAnalysis-0.0.1/LICENSE` & `AdsorptionBreakthroughAnalysis-0.0.2/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-Copyright (c) 2008-present Daniel Maroto-Andresen
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish,
-distribute, sublicense, and/or sell copies of the Software, and to
-permit persons to whom the Software is furnished to do so, subject to
-the following conditions:
+Copyright (c) 2023 Daniel Maroto-Andresen
 
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

