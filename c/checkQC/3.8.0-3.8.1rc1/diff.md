# Comparing `tmp/checkQC-3.8.0.tar.gz` & `tmp/checkQC-3.8.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkQC-3.8.0.tar", last modified: Fri May  5 06:05:07 2023, max compression
+gzip compressed data, was "checkQC-3.8.1rc1.tar", last modified: Thu May 11 08:11:49 2023, max compression
```

## Comparing `checkQC-3.8.0.tar` & `checkQC-3.8.1rc1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2023-05-05 06:05:07.512037 checkQC-3.8.0/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)    35141 2022-03-09 14:47:52.000000 checkQC-3.8.0/LICENSE
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      146 2022-03-09 14:47:52.000000 checkQC-3.8.0/MANIFEST.in
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      533 2023-05-05 06:05:07.512037 checkQC-3.8.0/PKG-INFO
--rw-rw-r--   0 matilda   (1000) matilda   (1000)    11335 2023-05-04 09:28:20.000000 checkQC-3.8.0/README.md
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2023-05-05 06:05:07.508037 checkQC-3.8.0/checkQC/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)       23 2023-05-04 11:01:05.000000 checkQC-3.8.0/checkQC/__init__.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     5028 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/app.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     9538 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/config.py
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2023-05-05 06:05:07.508037 checkQC-3.8.0/checkQC/default_config/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)    14396 2023-05-04 09:28:20.000000 checkQC-3.8.0/checkQC/default_config/config.yaml
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      576 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/default_config/logger.yaml
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      836 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/exceptions.py
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2023-05-05 06:05:07.512037 checkQC-3.8.0/checkQC/handlers/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)        0 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/__init__.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1857 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/cluster_pf_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3646 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/error_rate_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     2240 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/q30_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     7911 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/qc_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1545 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/qc_handler_factory.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3248 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/reads_per_sample_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     4146 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/undetermined_percentage_handler.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)    15665 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/handlers/unidentified_index_handler.py
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2023-05-05 06:05:07.512037 checkQC-3.8.0/checkQC/parsers/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)        0 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/parsers/__init__.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3958 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/parsers/demux_summary_parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3532 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/parsers/interop_parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     2245 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/parsers/parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     2098 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/parsers/samplesheet_parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     3189 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/parsers/stats_json_parser.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     4378 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/qc_engine.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     7802 2023-05-04 09:28:20.000000 checkQC-3.8.0/checkQC/run_type_recognizer.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1498 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/run_type_summarizer.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     2937 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/runfolder_reader.py
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     4221 2022-03-09 14:47:52.000000 checkQC-3.8.0/checkQC/web_app.py
-drwxrwxr-x   0 matilda   (1000) matilda   (1000)        0 2023-05-05 06:05:07.508037 checkQC-3.8.0/checkQC.egg-info/
--rw-rw-r--   0 matilda   (1000) matilda   (1000)      533 2023-05-05 06:05:07.000000 checkQC-3.8.0/checkQC.egg-info/PKG-INFO
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1067 2023-05-05 06:05:07.000000 checkQC-3.8.0/checkQC.egg-info/SOURCES.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)        1 2023-05-05 06:05:07.000000 checkQC-3.8.0/checkQC.egg-info/dependency_links.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)       81 2023-05-05 06:05:07.000000 checkQC-3.8.0/checkQC.egg-info/entry_points.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)       65 2023-05-05 06:05:07.000000 checkQC-3.8.0/checkQC.egg-info/requires.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)        8 2023-05-05 06:05:07.000000 checkQC-3.8.0/checkQC.egg-info/top_level.txt
--rw-rw-r--   0 matilda   (1000) matilda   (1000)       79 2023-05-05 06:05:07.512037 checkQC-3.8.0/setup.cfg
--rw-rw-r--   0 matilda   (1000) matilda   (1000)     1180 2022-10-25 10:40:55.000000 checkQC-3.8.0/setup.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2023-05-11 08:11:49.044370 checkQC-3.8.1rc1/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    35141 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/LICENSE
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      146 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/MANIFEST.in
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      540 2023-05-11 08:11:49.044370 checkQC-3.8.1rc1/PKG-INFO
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    11335 2023-05-08 06:26:37.000000 checkQC-3.8.1rc1/README.md
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2023-05-11 08:11:49.040370 checkQC-3.8.1rc1/checkQC/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       27 2023-05-11 07:53:21.000000 checkQC-3.8.1rc1/checkQC/__init__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     5028 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/app.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     9538 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/config.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2023-05-11 08:11:49.040370 checkQC-3.8.1rc1/checkQC/default_config/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    14396 2023-05-08 06:29:26.000000 checkQC-3.8.1rc1/checkQC/default_config/config.yaml
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      576 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/default_config/logger.yaml
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      836 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/exceptions.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2023-05-11 08:11:49.044370 checkQC-3.8.1rc1/checkQC/handlers/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)        0 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/handlers/__init__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1857 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/handlers/cluster_pf_handler.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     3646 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/handlers/error_rate_handler.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2240 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/handlers/q30_handler.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     7911 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/handlers/qc_handler.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1545 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/handlers/qc_handler_factory.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     3248 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/handlers/reads_per_sample_handler.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     4146 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/handlers/undetermined_percentage_handler.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    15676 2023-05-11 07:53:21.000000 checkQC-3.8.1rc1/checkQC/handlers/unidentified_index_handler.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2023-05-11 08:11:49.044370 checkQC-3.8.1rc1/checkQC/parsers/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)        0 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/parsers/__init__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     3958 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/parsers/demux_summary_parser.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     3532 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/parsers/interop_parser.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2245 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/parsers/parser.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2098 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/parsers/samplesheet_parser.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     3189 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/parsers/stats_json_parser.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     4378 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/qc_engine.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     7810 2023-05-08 06:29:26.000000 checkQC-3.8.1rc1/checkQC/run_type_recognizer.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1498 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/run_type_summarizer.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2937 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/runfolder_reader.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     4221 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/checkQC/web_app.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2023-05-11 08:11:49.040370 checkQC-3.8.1rc1/checkQC.egg-info/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      540 2023-05-11 08:11:49.000000 checkQC-3.8.1rc1/checkQC.egg-info/PKG-INFO
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1067 2023-05-11 08:11:49.000000 checkQC-3.8.1rc1/checkQC.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)        1 2023-05-11 08:11:49.000000 checkQC-3.8.1rc1/checkQC.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       81 2023-05-11 08:11:49.000000 checkQC-3.8.1rc1/checkQC.egg-info/entry_points.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       65 2023-05-11 08:11:49.000000 checkQC-3.8.1rc1/checkQC.egg-info/requires.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)        8 2023-05-11 08:11:49.000000 checkQC-3.8.1rc1/checkQC.egg-info/top_level.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       79 2023-05-11 08:11:49.044370 checkQC-3.8.1rc1/setup.cfg
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1180 2022-07-05 12:26:32.000000 checkQC-3.8.1rc1/setup.py
```

### Comparing `checkQC-3.8.0/LICENSE` & `checkQC-3.8.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/PKG-INFO` & `checkQC-3.8.1rc1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: checkQC
-Version: 3.8.0
+Version: 3.8.1rc1
 Summary: A simple program to parse Illumina NGS data and check it for quality criteria.
 Home-page: https://www.github.com/Molmed/checkQC
-Download-URL: https://github.com/Molmed/checkQC/archive/3.8.0.tar.gz
+Download-URL: https://github.com/Molmed/checkQC/archive/3.8.1-rc1.tar.gz
 Author: Johan Dahlberg, SNP&SEQ Technology Platform, Uppsala University
 Author-email: johan.dahlberg@medsci.uu.se
 License: GPLv3
 Keywords: bioinformatics,ngs,quality control
 License-File: LICENSE
 
 A simple program to parse Illumina NGS data and check it for quality criteria.
```

### Comparing `checkQC-3.8.0/README.md` & `checkQC-3.8.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/app.py` & `checkQC-3.8.1rc1/checkQC/app.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/config.py` & `checkQC-3.8.1rc1/checkQC/config.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/default_config/config.yaml` & `checkQC-3.8.1rc1/checkQC/default_config/config.yaml`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/default_config/logger.yaml` & `checkQC-3.8.1rc1/checkQC/default_config/logger.yaml`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/exceptions.py` & `checkQC-3.8.1rc1/checkQC/exceptions.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/handlers/cluster_pf_handler.py` & `checkQC-3.8.1rc1/checkQC/handlers/cluster_pf_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/handlers/error_rate_handler.py` & `checkQC-3.8.1rc1/checkQC/handlers/error_rate_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/handlers/q30_handler.py` & `checkQC-3.8.1rc1/checkQC/handlers/q30_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/handlers/qc_handler.py` & `checkQC-3.8.1rc1/checkQC/handlers/qc_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/handlers/qc_handler_factory.py` & `checkQC-3.8.1rc1/checkQC/handlers/qc_handler_factory.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/handlers/reads_per_sample_handler.py` & `checkQC-3.8.1rc1/checkQC/handlers/reads_per_sample_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/handlers/undetermined_percentage_handler.py` & `checkQC-3.8.1rc1/checkQC/handlers/undetermined_percentage_handler.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/handlers/unidentified_index_handler.py` & `checkQC-3.8.1rc1/checkQC/handlers/unidentified_index_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,32 +6,36 @@
 from checkQC.parsers.stats_json_parser import StatsJsonParser
 from checkQC.parsers.samplesheet_parser import SamplesheetParser
 from checkQC.exceptions import ConfigurationError
 
 
 class UnidentifiedIndexHandler(QCHandler):
     """
-    The UnidentifiedIndexHandler will try to identify if an index is represented at to high a level in unidentified
-    reads, and if that is the case try to pinpoint why that is.
+    The UnidentifiedIndexHandler will try to identify if an index is
+    represented at to high a level in unidentified reads, and if that is the
+    case try to pinpoint why that is.
+
+    It will not output errors, but all information will be displayed as
+    warnings, due to the difficulty of deciding what is an error or not in this
+    context. For most cases the % of unidentified reads will be what is used to
+    issue the error, and then the warnings from this handler can help in
+    identifying the possible underlying cause.
+
+    There are a number of different checks (or rules) in place, which will be
+    checked if and index occurs more then the `significance_threshold`. The
+    samplesheet will be checked to see if the index found matches and of the
+    following rules:
+    - Check if the dual indexes have been swapped
+    - Check if the index has been reversed
+    - Check if the index is the reverse complement
+    - Check if the index is the complementary index
+    - Check if the index is present in another lane
 
-    It will not output errors, but all information will be displayed as warnings, due to the difficulty
-    of deciding what is an error or not in this context. For most cases the % of unidentified reads will be what
-    is used to issue the error, and then the warnings from this handler can help in identifying the
-    possible underlying cause.
-
-    There are a number of different checks (or rules) in place, which will be checked if and index
-    occurs more then the `significance_threshold`. The samplesheet will be checked to see if the index
-    found matches and of the following rules:
-     - Check if the dual indexes have been swapped
-     - Check if the index has been reversed
-     - Check if the index is the reverse complement
-     - Check if the index is the complementary index
-     - Check if the index is present in another lane
-
-    It will ignore any indexes which have N's in them. These are assumed to be read errors.
+    It will ignore any indexes which have N's in them. These are assumed to be
+    read errors.
     """
 
     WHITE_LIST_QC_KEY = 'white_listed_indexes'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.lanes_and_indices = {}
```

### Comparing `checkQC-3.8.0/checkQC/parsers/demux_summary_parser.py` & `checkQC-3.8.1rc1/checkQC/parsers/demux_summary_parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/parsers/interop_parser.py` & `checkQC-3.8.1rc1/checkQC/parsers/interop_parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/parsers/parser.py` & `checkQC-3.8.1rc1/checkQC/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/parsers/samplesheet_parser.py` & `checkQC-3.8.1rc1/checkQC/parsers/samplesheet_parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/parsers/stats_json_parser.py` & `checkQC-3.8.1rc1/checkQC/parsers/stats_json_parser.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/qc_engine.py` & `checkQC-3.8.1rc1/checkQC/qc_engine.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/run_type_recognizer.py` & `checkQC-3.8.1rc1/checkQC/run_type_recognizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             "ST": HiSeqX,
             "A": NovaSeq,
             "FS": ISeq,
             "LH": NovaSeqXPlus,
         }
 
         for instrument_code, instrument_class in machine_type_mappings.items():
-            if instrument_name.startswith(instrument_code):
+            if instrument_name.upper().startswith(instrument_code):
                 return instrument_class()
 
         raise InstrumentTypeUnknown("Did not recognize instrument type of: {}".format(instrument_name))
 
     def instrument_and_reagent_version(self):
         """
         Get the instrument and reagent version associated with this runfolder.
```

### Comparing `checkQC-3.8.0/checkQC/run_type_summarizer.py` & `checkQC-3.8.1rc1/checkQC/run_type_summarizer.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/runfolder_reader.py` & `checkQC-3.8.1rc1/checkQC/runfolder_reader.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC/web_app.py` & `checkQC-3.8.1rc1/checkQC/web_app.py`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/checkQC.egg-info/PKG-INFO` & `checkQC-3.8.1rc1/checkQC.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: checkQC
-Version: 3.8.0
+Version: 3.8.1rc1
 Summary: A simple program to parse Illumina NGS data and check it for quality criteria.
 Home-page: https://www.github.com/Molmed/checkQC
-Download-URL: https://github.com/Molmed/checkQC/archive/3.8.0.tar.gz
+Download-URL: https://github.com/Molmed/checkQC/archive/3.8.1-rc1.tar.gz
 Author: Johan Dahlberg, SNP&SEQ Technology Platform, Uppsala University
 Author-email: johan.dahlberg@medsci.uu.se
 License: GPLv3
 Keywords: bioinformatics,ngs,quality control
 License-File: LICENSE
 
 A simple program to parse Illumina NGS data and check it for quality criteria.
```

### Comparing `checkQC-3.8.0/checkQC.egg-info/SOURCES.txt` & `checkQC-3.8.1rc1/checkQC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `checkQC-3.8.0/setup.py` & `checkQC-3.8.1rc1/setup.py`

 * *Files identical despite different names*

