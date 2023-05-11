# Comparing `tmp/IQM-Vis-0.2.5.64.tar.gz` & `tmp/IQM-Vis-0.2.5.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IQM-Vis-0.2.5.64.tar", last modified: Wed May 10 16:15:12 2023, max compression
+gzip compressed data, was "IQM-Vis-0.2.5.65.tar", last modified: Thu May 11 14:05:40 2023, max compression
```

## Comparing `IQM-Vis-0.2.5.64.tar` & `IQM-Vis-0.2.5.65.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:15:12.223782 IQM-Vis-0.2.5.64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:15:12.215782 IQM-Vis-0.2.5.64/IQM_Vis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:15:12.219782 IQM-Vis-0.2.5.64/IQM_Vis/UI/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/UI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/UI/custom_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    23805 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/UI/experiment_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/UI/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/UI/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/UI/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/UI/style-dark.css
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/UI/style-light.css
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/UI/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/UI/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23963 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/UI/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:15:12.219782 IQM-Vis-0.2.5.64/IQM_Vis/data_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/data_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/data_handlers/data_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/data_handlers/data_api_abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:15:12.219782 IQM-Vis-0.2.5.64/IQM_Vis/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/examples/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/examples/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/examples/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/examples/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:15:12.219782 IQM-Vis-0.2.5.64/IQM_Vis/examples/images/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/examples/images/HIQM.csv
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/examples/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/examples/images/waves1.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    17780 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/examples/images/waves2.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/examples/images/waves3.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/examples/multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/examples/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:15:12.219782 IQM-Vis-0.2.5.64/IQM_Vis/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    12685 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/metrics/IQMs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:15:12.219782 IQM-Vis-0.2.5.64/IQM_Vis/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/transformations/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/ui_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:15:12.223782 IQM-Vis-0.2.5.64/IQM_Vis/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/utils/gui_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/utils/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/IQM_Vis/utils/save_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:15:12.215782 IQM-Vis-0.2.5.64/IQM_Vis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-10 16:15:12.000000 IQM-Vis-0.2.5.64/IQM_Vis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-10 16:15:12.000000 IQM-Vis-0.2.5.64/IQM_Vis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:15:12.000000 IQM-Vis-0.2.5.64/IQM_Vis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 16:15:12.000000 IQM-Vis-0.2.5.64/IQM_Vis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 16:15:12.000000 IQM-Vis-0.2.5.64/IQM_Vis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-10 16:15:12.223782 IQM-Vis-0.2.5.64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:15:12.223782 IQM-Vis-0.2.5.64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:15:12.223782 IQM-Vis-0.2.5.64/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-10 16:14:54.000000 IQM-Vis-0.2.5.64/tests/test_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:05:40.848369 IQM-Vis-0.2.5.65/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:05:40.840369 IQM-Vis-0.2.5.65/IQM_Vis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:05:40.844370 IQM-Vis-0.2.5.65/IQM_Vis/UI/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/UI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/UI/custom_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24876 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/UI/experiment_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/UI/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/UI/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/UI/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/UI/style-dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/UI/style-light.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/UI/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/UI/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24364 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/UI/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:05:40.844370 IQM-Vis-0.2.5.65/IQM_Vis/data_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/data_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/data_handlers/data_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/data_handlers/data_api_abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:05:40.844370 IQM-Vis-0.2.5.65/IQM_Vis/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/examples/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/examples/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/examples/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/examples/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:05:40.844370 IQM-Vis-0.2.5.65/IQM_Vis/examples/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/examples/images/HIQM.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/examples/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/examples/images/waves1.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    17780 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/examples/images/waves2.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/examples/images/waves3.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/examples/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/examples/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:05:40.844370 IQM-Vis-0.2.5.65/IQM_Vis/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    12685 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/metrics/IQMs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:05:40.844370 IQM-Vis-0.2.5.65/IQM_Vis/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/transformations/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/ui_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:05:40.844370 IQM-Vis-0.2.5.65/IQM_Vis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/utils/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/utils/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/IQM_Vis/utils/save_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:05:40.840369 IQM-Vis-0.2.5.65/IQM_Vis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-11 14:05:40.000000 IQM-Vis-0.2.5.65/IQM_Vis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-11 14:05:40.000000 IQM-Vis-0.2.5.65/IQM_Vis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:05:40.000000 IQM-Vis-0.2.5.65/IQM_Vis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 14:05:40.000000 IQM-Vis-0.2.5.65/IQM_Vis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 14:05:40.000000 IQM-Vis-0.2.5.65/IQM_Vis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-11 14:05:40.844370 IQM-Vis-0.2.5.65/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:05:40.848369 IQM-Vis-0.2.5.65/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:05:40.844370 IQM-Vis-0.2.5.65/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-11 14:05:29.000000 IQM-Vis-0.2.5.65/tests/test_inputs.py
```

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/UI/custom_widgets.py` & `IQM-Vis-0.2.5.65/IQM_Vis/UI/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/UI/experiment_mode.py` & `IQM-Vis-0.2.5.65/IQM_Vis/UI/experiment_mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,42 +14,48 @@
                              QVBoxLayout,
                              QTabWidget,
                              QApplication,
                              QPushButton,
                              QLabel,
                              QMessageBox)
 
-from PyQt6.QtCore import Qt
+from PyQt6.QtCore import Qt, pyqtSignal
 from PyQt6.QtGui import QShortcut, QKeySequence
 
 import IQM_Vis
 from IQM_Vis.UI.custom_widgets import ClickLabel
 from IQM_Vis.UI import utils
 from IQM_Vis.utils import gui_utils, plot_utils, image_utils
 
 
 class make_experiment(QMainWindow):
+    saved_experiment = pyqtSignal(str)
+
     def __init__(self, 
                  checked_transformations, 
                  data_store, 
                  image_display_size,
                  rgb_brightness,
                  display_brightness,
                  default_save_dir=IQM_Vis.utils.save_utils.DEFAULT_SAVE_DIR,
-                 num_trans_values=6):
+                 num_trans_values=6,
+                 image_preprocessing='None',
+                 image_postprocessing='None'):
         super().__init__()
         self.checked_transformations = checked_transformations
         if self.checked_transformations == {}:
             return
         self.data_store = data_store
         self.image_display_size = image_display_size
         self.rgb_brightness = rgb_brightness
         self.display_brightness = display_brightness
         self.default_save_dir = default_save_dir
         self.num_trans_values = num_trans_values
+        self.processing = {'pre': image_preprocessing,
+                           'post': image_postprocessing}
 
         self.clicked_event = threading.Event()
         self.stop_event = threading.Event()
         self.saved = False
         self.quit_experiment = False
         self._init_experiment_window_widgets()
         self.get_all_images()
@@ -359,20 +365,30 @@
         # get a unique directory (same image with diff trans need a new dir)
         i = 1
         unique_dir_found = False
         new_dir = True
         while unique_dir_found == False:
             exp_save_dir = f'{self.default_save_dir}-experiment-{i}'
             if os.path.exists(exp_save_dir):
-                # check if experiment is the same
+                # get transform funcs and params
                 exp_trans_params = IQM_Vis.utils.save_utils.load_obj(
                     os.path.join(exp_save_dir, 'transforms', 'transform_params.pkl'))
                 exp_trans_funcs = IQM_Vis.utils.save_utils.load_obj(
                     os.path.join(exp_save_dir, 'transforms', 'transform_functions.pkl'))
-                if (exp_trans_params == self.original_params_order) and (trans_funcs == exp_trans_funcs):
+                
+                # get image processing saved params
+                processing_file = os.path.join(exp_save_dir, 'transforms', 'processing.json')
+                procesing_same = False
+                if os.path.exists(processing_file):
+                    processing = IQM_Vis.utils.save_utils.load_json_dict(processing_file)
+                    if processing == self.processing:
+                        procesing_same = True
+
+                # check if experiment is the same
+                if (exp_trans_params == self.original_params_order) and (trans_funcs == exp_trans_funcs) and procesing_same:
                     self.default_save_dir = exp_save_dir
                     unique_dir_found = True
                     new_dir = False
                 else:
                     i += 1
             else:
                 self.default_save_dir = exp_save_dir
@@ -391,23 +407,30 @@
             # save the transformations
             IQM_Vis.utils.save_utils.save_obj(
                 os.path.join(self.default_save_dir, 'transforms', 'transform_params.pkl'),
                 self.original_params_order)
             IQM_Vis.utils.save_utils.save_obj(
                 os.path.join(self.default_save_dir, 'transforms', 'transform_functions.pkl'),
                 dict(sorted(trans_funcs.items())))
+            # save the image pre/post processing options
+            IQM_Vis.utils.save_utils.save_json_dict(
+                os.path.join(self.default_save_dir, 'transforms', 'processing.json'),
+                self.processing)
+
         # save the experiment results
         exp_order = []
         for trans in self.experiment_transforms:
             exp_order.append(make_name_for_trans(trans))
+        csv_file = os.path.join(self.default_save_dir, f'{self.data_store.get_reference_image_name()}-results.csv')
         IQM_Vis.utils.save_utils.save_experiment_results(
             self.original_params_order,
             exp_order,
-            os.path.join(self.default_save_dir, f'{self.data_store.get_reference_image_name()}-results.csv'))
+            csv_file)
         self.saved = True
+        self.saved_experiment.emit(csv_file)
 
 
     ''' sorting algorithm resource: https://www.geeksforgeeks.org/quick-sort/'''
     def quick_sort(self):
         self._quick_sort(0, len(self.experiment_transforms)-1)
         if self.quit_experiment != True:
             self.finish_experiment()
```

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/UI/images.py` & `IQM-Vis-0.2.5.65/IQM_Vis/UI/images.py`

 * *Files 11% similar despite different names*

```diff
@@ -140,22 +140,51 @@
             file, _ = QFileDialog.getOpenFileName(
                 self,
                 "Open Human Experiments File for Current Image",
                 start_dir,
                 "CSV Files (*.csv)",)
         except:
             return
+        self._change_human_exp(file)
         
+    def _change_human_exp(self, file):
         # load the csv human scores file and take mean of all experiments
         if os.path.exists(file):
             df = pd.read_csv(file)
             experiment = df.mean().to_dict()
             for i, _ in enumerate(self.data_stores):
                 self.human_experiment_scores[i] = experiment
+            self.human_scores_file = file
+        else:
+            self.update_status_bar(f'No file: {file}')
+            return
         
+        # load the image processing if available
+        processing_file = os.path.join(os.path.dirname(file), 'transforms', 'processing.json')
+        if os.path.exists(processing_file):
+            processing = IQM_Vis.utils.save_utils.load_json_dict(
+                processing_file)
+            updated = False
+            for name, options_var, change_func in zip(['pre', 'post'], 
+                                                      [self.pre_processing_options, self.post_processing_options], 
+                                                      [self.change_pre_processing, self.change_post_processing]):
+                if processing[name] in options_var:
+                    if processing[name] != self.widget_settings[f'image_{name}_processing']['widget'].currentText():
+                        self.widget_settings[f'image_{name}_processing']['widget'].setCurrentText(
+                            processing[name])
+                        change_func()
+                        updated = True
+                else:
+                    self.update_status_bar(
+                        f'Could not load image setting: {processing[name]}')
+            if updated == True:
+                self.update_image_settings()
+        else:
+            self.update_status_bar('Warning: Could not find an image settings file in folder, make sure image pre/post processing settings are correct')
+
         # clear cache and update correlation plot
         self.reset_correlation_data()
         self.display_metric_correlation_plot()
 
     '''
     metric updaters
     '''
@@ -282,14 +311,16 @@
                     # cache it
                     self.correlation_data[i][metric] = scores
                 plot = plot_utils.get_correlation_plot(self.human_experiment_scores[i],
                                                 self.correlation_data[i],
                                                 self.widget_row[i]['metrics']['correlation']['data'],
                                                 metric,
                                                 self.view_correlation_instance)
+                if hasattr(self, 'human_scores_file'):
+                    plot.ax.axes.set_title(self.human_scores_file, fontsize=6)
                 plot.show()
             else:
                 self.widget_row[i]['metrics']['correlation']['data'].axes.clear()
                 self.widget_row[i]['metrics']['correlation']['data'].axes.text(
                     0.5, 0.5, 'Go to: File->Load Human Scores', horizontalalignment='center', verticalalignment='center')
                 self.widget_row[i]['metrics']['correlation']['data'].draw()
```

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/UI/layout.py` & `IQM-Vis-0.2.5.65/IQM_Vis/UI/layout.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/UI/main.py` & `IQM-Vis-0.2.5.65/IQM_Vis/UI/main.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/UI/threads.py` & `IQM-Vis-0.2.5.65/IQM_Vis/UI/threads.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/UI/widgets.py` & `IQM-Vis-0.2.5.65/IQM_Vis/UI/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 '''
 # Author: Matt Clifford <matt.clifford@bristol.ac.uk>
 from functools import partial
 
 import numpy as np
 from PyQt6.QtWidgets import QPushButton, QLabel, QSlider, QCheckBox, QComboBox, QLineEdit
 from PyQt6.QtGui import QIntValidator
-from PyQt6.QtCore import Qt
+from PyQt6.QtCore import Qt, pyqtSlot
 
 import IQM_Vis
 from IQM_Vis.UI.custom_widgets import ClickLabel
 from IQM_Vis.utils import gui_utils, plot_utils, image_utils
 
 # sub class used by IQM_Vis.main.make_app to initialise widgets and general UI functions for widgets
 class widgets():
@@ -406,17 +406,25 @@
 
     def update_status_bar(self, v):
         self.status_bar.showMessage(v)
 
     def launch_experiment(self):
         if self.checked_transformations != {}:
             self.experiment = IQM_Vis.UI.make_experiment(self.checked_transformations,
-                                                        self.data_stores[0],
-                                                        self.image_display_size,
-                                                        self.rgb_brightness,
-                                                        self.display_brightness,
-                                                        self.default_save_dir,
-                                                        self.num_steps_range)
+                                                         self.data_stores[0],
+                                                         self.image_display_size,
+                                                         self.rgb_brightness,
+                                                         self.display_brightness,
+                                                         self.default_save_dir,
+                                                         self.num_steps_range,
+                                                         self.pre_processing_option,
+                                                         self.post_processing_option)
+            self.experiment.saved_experiment.connect(
+                self.change_human_scores_after_exp)
             self.experiment.show()
             self.experiment.showFullScreen()
         else:
             self.status_bar.showMessage('Cannot make experiment without transforms', 5000)
+
+    @pyqtSlot(str)
+    def change_human_scores_after_exp(self, path):
+        self._change_human_exp(path)
```

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/data_handlers/data_api.py` & `IQM-Vis-0.2.5.65/IQM_Vis/data_handlers/data_api.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/data_handlers/data_api_abstract.py` & `IQM-Vis-0.2.5.65/IQM_Vis/data_handlers/data_api_abstract.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/examples/all.py` & `IQM-Vis-0.2.5.65/IQM_Vis/examples/all.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/examples/dataset.py` & `IQM-Vis-0.2.5.65/IQM_Vis/examples/dataset.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/examples/dists.py` & `IQM-Vis-0.2.5.65/IQM_Vis/examples/dists.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/examples/experiment.py` & `IQM-Vis-0.2.5.65/IQM_Vis/examples/experiment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import numpy as np
 import IQM_Vis
 
 
 def run():
     # metrics functions must return a single value
-    metric = {} #IQM_Vis.metrics.get_all_metrics()
+    metric = {'MSE': IQM_Vis.IQMs.MSE()}
 
     # metrics images return a numpy image
     metric_images = {}
 
     # make dataset list of images
     file_path = os.path.dirname(os.path.abspath(__file__))
     dataset = [os.path.join(file_path, 'images', 'waves1.jpeg'),
```

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/examples/images/waves1.jpeg` & `IQM-Vis-0.2.5.65/IQM_Vis/examples/images/waves1.jpeg`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/examples/images/waves2.jpeg` & `IQM-Vis-0.2.5.65/IQM_Vis/examples/images/waves2.jpeg`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/examples/images/waves3.jpeg` & `IQM-Vis-0.2.5.65/IQM_Vis/examples/images/waves3.jpeg`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/examples/multiple.py` & `IQM-Vis-0.2.5.65/IQM_Vis/examples/multiple.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/examples/simple.py` & `IQM-Vis-0.2.5.65/IQM_Vis/examples/simple.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/metrics/IQMs.py` & `IQM-Vis-0.2.5.65/IQM_Vis/metrics/IQMs.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/metrics/__init__.py` & `IQM-Vis-0.2.5.65/IQM_Vis/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/transformations/__init__.py` & `IQM-Vis-0.2.5.65/IQM_Vis/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/transformations/transforms.py` & `IQM-Vis-0.2.5.65/IQM_Vis/transformations/transforms.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/ui_wrapper.py` & `IQM-Vis-0.2.5.65/IQM_Vis/ui_wrapper.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/utils/gui_utils.py` & `IQM-Vis-0.2.5.65/IQM_Vis/utils/gui_utils.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/utils/image_utils.py` & `IQM-Vis-0.2.5.65/IQM_Vis/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/utils/plot_utils.py` & `IQM-Vis-0.2.5.65/IQM_Vis/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis/utils/save_utils.py` & `IQM-Vis-0.2.5.65/IQM_Vis/utils/save_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 '''
 utils for saving experiments, images and figures
 '''
 # Author: Matt Clifford <matt.clifford@bristol.ac.uk>
 import os
+import json
 import pickle
 import pandas as pd
 
 DEFAULT_SAVE_DIR = os.path.join(os.path.expanduser("~"), 'IQM-Vis-experiments')
 
 def save_obj(pickle_path, trans):
     ''' save transforms as pickle file '''
@@ -36,7 +37,15 @@
     df = df[trans_names]
 
     # save results
     if os.path.exists(file):
         df_saved = pd.read_csv(file)
         df = pd.concat([df_saved, df])
     df.to_csv(file, index=False)
+
+def save_json_dict(path, dict_):
+    with open(path, 'w') as fp:
+        json.dump(dict_, fp)
+
+def load_json_dict(path):
+    with open(path, 'r') as fp:
+        return json.load(fp)
```

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis.egg-info/PKG-INFO` & `IQM-Vis-0.2.5.65/IQM_Vis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IQM-Vis
-Version: 0.2.5.64
+Version: 0.2.5.65
 Summary: Extendable user interface for the assessment of transformations on image metrics.
 Author: Matt Clifford
 Author-email: matt.clifford@bristol.ac.uk
 Description-Content-Type: text/markdown
 
 | | |
 |-|-|
```

### Comparing `IQM-Vis-0.2.5.64/IQM_Vis.egg-info/SOURCES.txt` & `IQM-Vis-0.2.5.65/IQM_Vis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/PKG-INFO` & `IQM-Vis-0.2.5.65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IQM-Vis
-Version: 0.2.5.64
+Version: 0.2.5.65
 Summary: Extendable user interface for the assessment of transformations on image metrics.
 Author: Matt Clifford
 Author-email: matt.clifford@bristol.ac.uk
 Description-Content-Type: text/markdown
 
 | | |
 |-|-|
```

### Comparing `IQM-Vis-0.2.5.64/README.md` & `IQM-Vis-0.2.5.65/README.md`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/setup.py` & `IQM-Vis-0.2.5.65/setup.py`

 * *Files identical despite different names*

### Comparing `IQM-Vis-0.2.5.64/tests/test_inputs.py` & `IQM-Vis-0.2.5.65/tests/test_inputs.py`

 * *Files identical despite different names*

