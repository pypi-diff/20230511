# Comparing `tmp/rat-3.0.0a13.tar.gz` & `tmp/rat-3.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rat-3.0.0a13.tar", last modified: Wed May 10 23:05:05 2023, max compression
+gzip compressed data, was "rat-3.0.0a4.tar", last modified: Tue May  2 17:36:27 2023, max compression
```

## Comparing `rat-3.0.0a13.tar` & `rat-3.0.0a4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:05:05.076889 rat-3.0.0a13/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-10 23:04:56.000000 rat-3.0.0a13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43731 2023-05-10 23:05:05.076889 rat-3.0.0a13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-10 23:04:56.000000 rat-3.0.0a13/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-10 23:04:57.000000 rat-3.0.0a13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 23:05:05.076889 rat-3.0.0a13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 23:04:57.000000 rat-3.0.0a13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:05:05.068889 rat-3.0.0a13/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:05:05.072889 rat-3.0.0a13/src/rat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:05:05.072889 rat-3.0.0a13/src/rat/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/cli/rat_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/cli/rat_init_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/cli/rat_test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:05:05.072889 rat-3.0.0a13/src/rat/core/
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/core/run_altimetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/core/run_metsim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/core/run_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/core/run_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/core/run_sarea.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/core/run_vic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:05:05.072889 rat-3.0.0a13/src/rat/core/sarea/
--rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/core/sarea/TMS.py
--rw-r--r--   0 runner    (1001) docker     (123)    19904 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/core/sarea/sarea_cli_l8.py
--rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/core/sarea/sarea_cli_l9.py
--rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/core/sarea/sarea_cli_s2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/core/sarea/sarea_cli_sar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:05:05.076889 rat-3.0.0a13/src/rat/data_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/data_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/data_processing/altimetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/data_processing/metsim_input_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    28327 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/data_processing/newdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:05:05.076889 rat-3.0.0a13/src/rat/ee_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/ee_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/ee_utils/ee_aec_file_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/ee_utils/ee_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/ee_utils/ee_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40632 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/rat_basin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/run_rat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:05:05.076889 rat-3.0.0a13/src/rat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/utils/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/utils/convert_to_final_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/utils/files_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/utils/metsim_param_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/utils/route_param_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/utils/run_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/utils/science.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-05-10 23:04:56.000000 rat-3.0.0a13/src/rat/utils/vic_param_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:05:05.072889 rat-3.0.0a13/src/rat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43731 2023-05-10 23:05:05.000000 rat-3.0.0a13/src/rat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 23:05:05.000000 rat-3.0.0a13/src/rat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 23:05:05.000000 rat-3.0.0a13/src/rat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-10 23:05:05.000000 rat-3.0.0a13/src/rat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:05:05.076889 rat-3.0.0a13/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 23:04:56.000000 rat-3.0.0a13/tests/test_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.148266 rat-3.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-02 17:36:15.000000 rat-3.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43730 2023-05-02 17:36:27.144266 rat-3.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-02 17:36:15.000000 rat-3.0.0a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-02 17:36:15.000000 rat-3.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:36:27.148266 rat-3.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-02 17:36:15.000000 rat-3.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.132266 rat-3.0.0a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.136266 rat-3.0.0a4/src/rat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.136266 rat-3.0.0a4/src/rat/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/cli/rat_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/cli/rat_init_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/cli/rat_test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.140266 rat-3.0.0a4/src/rat/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_altimetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_metsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_sarea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_vic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.140266 rat-3.0.0a4/src/rat/core/sarea/
+-rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/TMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19904 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/sarea_cli_l8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/sarea_cli_l9.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/sarea_cli_s2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/sarea_cli_sar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.144266 rat-3.0.0a4/src/rat/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/data_processing/altimetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/data_processing/metsim_input_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28327 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/data_processing/newdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.144266 rat-3.0.0a4/src/rat/ee_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/ee_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/ee_utils/ee_aec_file_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/ee_utils/ee_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/ee_utils/ee_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40632 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/rat_basin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/run_rat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.144266 rat-3.0.0a4/src/rat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/convert_to_final_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/metsim_param_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/route_param_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/science.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/vic_param_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.136266 rat-3.0.0a4/src/rat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43730 2023-05-02 17:36:27.000000 rat-3.0.0a4/src/rat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-02 17:36:27.000000 rat-3.0.0a4/src/rat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:36:27.000000 rat-3.0.0a4/src/rat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 17:36:27.000000 rat-3.0.0a4/src/rat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.144266 rat-3.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 17:36:15.000000 rat-3.0.0a4/tests/test_imports.py
```

### Comparing `rat-3.0.0a13/LICENSE` & `rat-3.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/PKG-INFO` & `rat-3.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rat
-Version: 3.0.0a13
+Version: 3.0.0a4
 Summary: Resevoir Monitoring using Satellite Remote Sensing
 Author-email: Pritam Das <pdas47@uw.edu>, Sanchit Minocha <msanchit@uw.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `rat-3.0.0a13/README.md` & `rat-3.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/pyproject.toml` & `rat-3.0.0a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rat"
-version = "3.0.0.alpha.13"
+version = "3.0.0.alpha.4"
 authors = [
   { name="Pritam Das", email="pdas47@uw.edu" },
   { name="Sanchit Minocha", email="msanchit@uw.edu" },
 ]
 description = "Resevoir Monitoring using Satellite Remote Sensing"
 requires-python = ">=3.6"
 readme = "README.md"
```

### Comparing `rat-3.0.0a13/src/rat/cli/rat_cli.py` & `rat-3.0.0a4/src/rat/cli/rat_cli.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/cli/rat_init_config.py` & `rat-3.0.0a4/src/rat/cli/rat_init_config.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/cli/rat_test_config.py` & `rat-3.0.0a4/src/rat/cli/rat_test_config.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/core/run_altimetry.py` & `rat-3.0.0a4/src/rat/core/run_altimetry.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/core/run_metsim.py` & `rat-3.0.0a4/src/rat/core/run_metsim.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/core/run_postprocessing.py` & `rat-3.0.0a4/src/rat/core/run_postprocessing.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/core/run_routing.py` & `rat-3.0.0a4/src/rat/core/run_routing.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/core/run_sarea.py` & `rat-3.0.0a4/src/rat/core/run_sarea.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/core/run_vic.py` & `rat-3.0.0a4/src/rat/core/run_vic.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/core/sarea/TMS.py` & `rat-3.0.0a4/src/rat/core/sarea/TMS.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/core/sarea/sarea_cli_l8.py` & `rat-3.0.0a4/src/rat/core/sarea/sarea_cli_l8.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/core/sarea/sarea_cli_l9.py` & `rat-3.0.0a4/src/rat/core/sarea/sarea_cli_l9.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/core/sarea/sarea_cli_s2.py` & `rat-3.0.0a4/src/rat/core/sarea/sarea_cli_s2.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/core/sarea/sarea_cli_sar.py` & `rat-3.0.0a4/src/rat/core/sarea/sarea_cli_sar.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/data_processing/altimetry.py` & `rat-3.0.0a4/src/rat/data_processing/altimetry.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/data_processing/metsim_input_processing.py` & `rat-3.0.0a4/src/rat/data_processing/metsim_input_processing.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/data_processing/newdata.py` & `rat-3.0.0a4/src/rat/data_processing/newdata.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/ee_utils/ee_aec_file_creator.py` & `rat-3.0.0a4/src/rat/ee_utils/ee_aec_file_creator.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/ee_utils/ee_utils.py` & `rat-3.0.0a4/src/rat/ee_utils/ee_utils.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/rat_basin.py` & `rat-3.0.0a4/src/rat/rat_basin.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/run_rat.py` & `rat-3.0.0a4/src/rat/run_rat.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/utils/clean.py` & `rat-3.0.0a4/src/rat/utils/clean.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/utils/convert_to_final_outputs.py` & `rat-3.0.0a4/src/rat/utils/convert_to_final_outputs.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/utils/files_creator.py` & `rat-3.0.0a4/src/rat/utils/files_creator.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/utils/logging.py` & `rat-3.0.0a4/src/rat/utils/logging.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/utils/metsim_param_reader.py` & `rat-3.0.0a4/src/rat/utils/metsim_param_reader.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/utils/route_param_reader.py` & `rat-3.0.0a4/src/rat/utils/route_param_reader.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/utils/run_command.py` & `rat-3.0.0a4/src/rat/utils/run_command.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/utils/science.py` & `rat-3.0.0a4/src/rat/utils/science.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/utils/utils.py` & `rat-3.0.0a4/src/rat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat/utils/vic_param_reader.py` & `rat-3.0.0a4/src/rat/utils/vic_param_reader.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a13/src/rat.egg-info/PKG-INFO` & `rat-3.0.0a4/src/rat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rat
-Version: 3.0.0a13
+Version: 3.0.0a4
 Summary: Resevoir Monitoring using Satellite Remote Sensing
 Author-email: Pritam Das <pdas47@uw.edu>, Sanchit Minocha <msanchit@uw.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `rat-3.0.0a13/src/rat.egg-info/SOURCES.txt` & `rat-3.0.0a4/src/rat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

