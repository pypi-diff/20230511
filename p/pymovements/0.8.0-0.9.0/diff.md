# Comparing `tmp/pymovements-0.8.0.tar.gz` & `tmp/pymovements-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymovements-0.8.0.tar", last modified: Fri Mar 24 13:15:44 2023, max compression
+gzip compressed data, was "pymovements-0.9.0.tar", last modified: Fri Apr 14 11:40:38 2023, max compression
```

## Comparing `pymovements-0.8.0.tar` & `pymovements-0.9.0.tar`

### file list

```diff
@@ -1,59 +1,63 @@
-drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-03-24 13:15:44.764407 pymovements-0.8.0/
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1075 2023-03-03 12:33:56.000000 pymovements-0.8.0/LICENSE.txt
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5169 2023-03-24 13:15:44.761073 pymovements-0.8.0/PKG-INFO
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     3819 2023-03-16 12:52:36.000000 pymovements-0.8.0/README.md
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     2862 2023-03-24 13:12:01.000000 pymovements-0.8.0/pyproject.toml
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)       38 2023-03-24 13:15:44.764407 pymovements-0.8.0/setup.cfg
-drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-03-24 13:15:44.751073 pymovements-0.8.0/src/
-drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-03-24 13:15:44.754407 pymovements-0.8.0/src/pymovements/
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1629 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/__init__.py
-drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-03-24 13:15:44.754407 pymovements-0.8.0/src/pymovements/datasets/
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     2093 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/datasets/__init__.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)    39144 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/datasets/dataset.py
-drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-03-24 13:15:44.757740 pymovements-0.8.0/src/pymovements/datasets/definitions/
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1395 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/datasets/definitions/__init__.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5532 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/datasets/definitions/gazebase.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5186 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/datasets/definitions/judo1000.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5014 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/datasets/definitions/toy_dataset.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)    14375 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/datasets/public_dataset.py
-drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-03-24 13:15:44.757740 pymovements-0.8.0/src/pymovements/events/
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     2507 2023-03-16 10:17:02.000000 pymovements-0.8.0/src/pymovements/events/__init__.py
-drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-03-24 13:15:44.757740 pymovements-0.8.0/src/pymovements/events/detection/
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1110 2023-03-16 10:17:02.000000 pymovements-0.8.0/src/pymovements/events/detection/__init__.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     8149 2023-03-16 10:17:02.000000 pymovements-0.8.0/src/pymovements/events/detection/engbert.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     7996 2023-03-16 10:17:02.000000 pymovements-0.8.0/src/pymovements/events/detection/idt.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5509 2023-03-16 10:17:02.000000 pymovements-0.8.0/src/pymovements/events/detection/ivt.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     6912 2023-03-10 15:36:43.000000 pymovements-0.8.0/src/pymovements/events/event_processing.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     6115 2023-03-10 15:36:43.000000 pymovements-0.8.0/src/pymovements/events/event_properties.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     7984 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/events/events.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1466 2023-03-10 15:36:43.000000 pymovements-0.8.0/src/pymovements/exceptions.py
-drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-03-24 13:15:44.757740 pymovements-0.8.0/src/pymovements/gaze/
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1951 2023-03-16 10:17:02.000000 pymovements-0.8.0/src/pymovements/gaze/__init__.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5210 2023-03-10 15:36:43.000000 pymovements-0.8.0/src/pymovements/gaze/experiment.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     7629 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/gaze/gaze_dataframe.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     6291 2023-03-10 15:36:43.000000 pymovements-0.8.0/src/pymovements/gaze/screen.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)    15654 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/gaze/transforms.py
-drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-03-24 13:15:44.761073 pymovements-0.8.0/src/pymovements/plotting/
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1748 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/plotting/__init__.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5567 2023-03-16 10:17:02.000000 pymovements-0.8.0/src/pymovements/plotting/heatmap.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     3006 2023-03-16 10:17:02.000000 pymovements-0.8.0/src/pymovements/plotting/main_sequence_plot.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     6901 2023-03-10 15:36:43.000000 pymovements-0.8.0/src/pymovements/plotting/traceplot.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5459 2023-03-10 15:36:43.000000 pymovements-0.8.0/src/pymovements/plotting/tsplot.py
-drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-03-24 13:15:44.761073 pymovements-0.8.0/src/pymovements/synthetic/
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1366 2023-03-16 10:17:02.000000 pymovements-0.8.0/src/pymovements/synthetic/__init__.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5102 2023-03-10 15:36:43.000000 pymovements-0.8.0/src/pymovements/synthetic/step_function.py
-drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-03-24 13:15:44.761073 pymovements-0.8.0/src/pymovements/utils/
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1782 2023-03-16 10:17:02.000000 pymovements-0.8.0/src/pymovements/utils/__init__.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     8932 2023-03-03 12:33:56.000000 pymovements-0.8.0/src/pymovements/utils/archives.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     6081 2023-03-10 15:36:43.000000 pymovements-0.8.0/src/pymovements/utils/checks.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1719 2023-03-16 10:17:02.000000 pymovements-0.8.0/src/pymovements/utils/decorators.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     8832 2023-03-10 15:36:43.000000 pymovements-0.8.0/src/pymovements/utils/downloads.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     3544 2023-03-10 15:36:43.000000 pymovements-0.8.0/src/pymovements/utils/filters.py
--rwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)     7272 2023-03-24 12:59:23.000000 pymovements-0.8.0/src/pymovements/utils/parsing.py
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     4795 2023-03-10 15:36:43.000000 pymovements-0.8.0/src/pymovements/utils/paths.py
-drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-03-24 13:15:44.754407 pymovements-0.8.0/src/pymovements.egg-info/
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5169 2023-03-24 13:15:44.000000 pymovements-0.8.0/src/pymovements.egg-info/PKG-INFO
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1641 2023-03-24 13:15:44.000000 pymovements-0.8.0/src/pymovements.egg-info/SOURCES.txt
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)        1 2023-03-24 13:15:44.000000 pymovements-0.8.0/src/pymovements.egg-info/dependency_links.txt
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)      435 2023-03-24 13:15:44.000000 pymovements-0.8.0/src/pymovements.egg-info/requires.txt
--rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)       12 2023-03-24 13:15:44.000000 pymovements-0.8.0/src/pymovements.egg-info/top_level.txt
+drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-04-14 11:40:38.345830 pymovements-0.9.0/
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1075 2023-03-03 12:33:56.000000 pymovements-0.9.0/LICENSE.txt
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5169 2023-04-14 11:40:38.345830 pymovements-0.9.0/PKG-INFO
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     3819 2023-03-16 12:52:36.000000 pymovements-0.9.0/README.md
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     2861 2023-04-14 11:31:39.000000 pymovements-0.9.0/pyproject.toml
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)       38 2023-04-14 11:40:38.345830 pymovements-0.9.0/setup.cfg
+drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-04-14 11:40:38.335830 pymovements-0.9.0/src/
+drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-04-14 11:40:38.339163 pymovements-0.9.0/src/pymovements/
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1865 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/__init__.py
+drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-04-14 11:40:38.339163 pymovements-0.9.0/src/pymovements/dataset/
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1771 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/dataset/__init__.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)    25227 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/dataset/dataset.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     3379 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/dataset/dataset_definition.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     4872 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/dataset/dataset_download.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)    15117 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/dataset/dataset_files.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     2514 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/dataset/dataset_library.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)    15032 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/dataset/dataset_paths.py
+drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-04-14 11:40:38.339163 pymovements-0.9.0/src/pymovements/datasets/
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1553 2023-03-27 12:29:03.000000 pymovements-0.9.0/src/pymovements/datasets/__init__.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5511 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/datasets/gazebase.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5165 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/datasets/judo1000.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     4995 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/datasets/toy_dataset.py
+drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-04-14 11:40:38.339163 pymovements-0.9.0/src/pymovements/events/
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     2507 2023-03-16 10:17:02.000000 pymovements-0.9.0/src/pymovements/events/__init__.py
+drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-04-14 11:40:38.342497 pymovements-0.9.0/src/pymovements/events/detection/
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1110 2023-03-16 10:17:02.000000 pymovements-0.9.0/src/pymovements/events/detection/__init__.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     8149 2023-03-16 10:17:02.000000 pymovements-0.9.0/src/pymovements/events/detection/engbert.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     8823 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/events/detection/idt.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5509 2023-03-16 10:17:02.000000 pymovements-0.9.0/src/pymovements/events/detection/ivt.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     6912 2023-03-10 15:36:43.000000 pymovements-0.9.0/src/pymovements/events/event_processing.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     6115 2023-03-10 15:36:43.000000 pymovements-0.9.0/src/pymovements/events/event_properties.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     7984 2023-03-24 12:59:23.000000 pymovements-0.9.0/src/pymovements/events/events.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1466 2023-03-10 15:36:43.000000 pymovements-0.9.0/src/pymovements/exceptions.py
+drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-04-14 11:40:38.342497 pymovements-0.9.0/src/pymovements/gaze/
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1951 2023-03-16 10:17:02.000000 pymovements-0.9.0/src/pymovements/gaze/__init__.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5210 2023-03-10 15:36:43.000000 pymovements-0.9.0/src/pymovements/gaze/experiment.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     7629 2023-03-24 12:59:23.000000 pymovements-0.9.0/src/pymovements/gaze/gaze_dataframe.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     6291 2023-03-10 15:36:43.000000 pymovements-0.9.0/src/pymovements/gaze/screen.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)    15654 2023-03-24 12:59:23.000000 pymovements-0.9.0/src/pymovements/gaze/transforms.py
+drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-04-14 11:40:38.345830 pymovements-0.9.0/src/pymovements/plotting/
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1748 2023-03-24 12:59:23.000000 pymovements-0.9.0/src/pymovements/plotting/__init__.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5567 2023-03-16 10:17:02.000000 pymovements-0.9.0/src/pymovements/plotting/heatmap.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     3538 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/plotting/main_sequence_plot.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     6901 2023-03-10 15:36:43.000000 pymovements-0.9.0/src/pymovements/plotting/traceplot.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5459 2023-03-10 15:36:43.000000 pymovements-0.9.0/src/pymovements/plotting/tsplot.py
+drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-04-14 11:40:38.345830 pymovements-0.9.0/src/pymovements/synthetic/
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1366 2023-03-16 10:17:02.000000 pymovements-0.9.0/src/pymovements/synthetic/__init__.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5102 2023-03-10 15:36:43.000000 pymovements-0.9.0/src/pymovements/synthetic/step_function.py
+drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-04-14 11:40:38.345830 pymovements-0.9.0/src/pymovements/utils/
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1782 2023-03-16 10:17:02.000000 pymovements-0.9.0/src/pymovements/utils/__init__.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     8932 2023-03-03 12:33:56.000000 pymovements-0.9.0/src/pymovements/utils/archives.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     6081 2023-03-10 15:36:43.000000 pymovements-0.9.0/src/pymovements/utils/checks.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1719 2023-03-16 10:17:02.000000 pymovements-0.9.0/src/pymovements/utils/decorators.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     8832 2023-03-10 15:36:43.000000 pymovements-0.9.0/src/pymovements/utils/downloads.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     3544 2023-03-10 15:36:43.000000 pymovements-0.9.0/src/pymovements/utils/filters.py
+-rwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)     7272 2023-03-24 12:59:23.000000 pymovements-0.9.0/src/pymovements/utils/parsing.py
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     4866 2023-04-14 11:31:39.000000 pymovements-0.9.0/src/pymovements/utils/paths.py
+drwxr-xr-x   0 krakowczyk  (1001) krakowczyk  (1001)        0 2023-04-14 11:40:38.339163 pymovements-0.9.0/src/pymovements.egg-info/
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     5169 2023-04-14 11:40:38.000000 pymovements-0.9.0/src/pymovements.egg-info/PKG-INFO
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)     1763 2023-04-14 11:40:38.000000 pymovements-0.9.0/src/pymovements.egg-info/SOURCES.txt
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)        1 2023-04-14 11:40:38.000000 pymovements-0.9.0/src/pymovements.egg-info/dependency_links.txt
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)      434 2023-04-14 11:40:38.000000 pymovements-0.9.0/src/pymovements.egg-info/requires.txt
+-rw-r--r--   0 krakowczyk  (1001) krakowczyk  (1001)       12 2023-04-14 11:40:38.000000 pymovements-0.9.0/src/pymovements.egg-info/top_level.txt
```

### Comparing `pymovements-0.8.0/LICENSE.txt` & `pymovements-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/PKG-INFO` & `pymovements-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymovements
-Version: 0.8.0
+Version: 0.9.0
 Summary: A python package for processing eye movement data
 Maintainer-email: Daniel Krakowczyk <daniel.krakowczyk@uni-potsdam.de>
 License: MIT License
 Project-URL: Homepage, https://github.com/aeye-lab/pymovements
 Project-URL: Source Code, https://github.com/aeye-lab/pymovements
 Project-URL: Documentation, https://pymovements.readthedocs.io/en/stable
 Project-URL: Bug Tracker, https://github.com/aeye-lab/pymovements/issues
```

### Comparing `pymovements-0.8.0/README.md` & `pymovements-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/pyproject.toml` & `pymovements-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
   "Topic :: Scientific/Engineering",
   "Typing :: Typed"
 ]
 dependencies = [
   "matplotlib>=3.0.0",
   "numpy>=1.10.0",
   "pandas>1.0.0",
-  "polars>=0.16.13",
+  "polars>=0.17.2",
   "pyarrow>=4.0.0",
   "scipy>=1.5.4",
   "tqdm>=4.0.0",
   "typing_extensions>=4.0.0"
 ]
 dynamic = ["version"]
```

### Comparing `pymovements-0.8.0/src/pymovements/__init__.py` & `pymovements-0.9.0/src/pymovements/utils/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,17 +13,29 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""This module provides access to all submodules."""
-from pymovements import datasets  # noqa: F401
-from pymovements import events  # noqa: F401
-from pymovements import gaze  # noqa: F401
-from pymovements import plotting  # noqa: F401
-from pymovements import synthetic  # noqa: F401
-from pymovements import utils  # noqa: F401
-from pymovements.datasets import Dataset  # noqa: F401
-from pymovements.datasets import PublicDataset  # noqa: F401
-from pymovements.datasets import PublicDatasetDefinition  # noqa: F401
+"""This module provides access to all utility functions.
+
+.. rubric:: Modules
+
+.. autosummary::
+   :toctree:
+   :template: module.rst
+
+    pymovements.utils.archives
+    pymovements.utils.checks
+    pymovements.utils.decorators
+    pymovements.utils.downloads
+    pymovements.utils.filters
+    pymovements.utils.parsing
+    pymovements.utils.paths
+"""
+from pymovements.utils import archives  # noqa: F401
+from pymovements.utils import checks  # noqa: F401
+from pymovements.utils import decorators  # noqa: F401
+from pymovements.utils import downloads  # noqa: F401
+from pymovements.utils import parsing  # noqa: F401
+from pymovements.utils import paths  # noqa: F401
```

### Comparing `pymovements-0.8.0/src/pymovements/datasets/__init__.py` & `pymovements-0.9.0/src/pymovements/dataset/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,28 +21,17 @@
 
 .. rubric:: Classes
 
 .. autosummary::
    :toctree:
    :template: class.rst
 
-    pymovements.datasets.Dataset
-    pymovements.datasets.PublicDataset
-    pymovements.datasets.PublicDatasetDefinition
-
-.. rubric:: Public Dataset Definitions
-
-.. autosummary::
-   :toctree:
-   :template: class.rst
-
-    pymovements.datasets.definitions.ToyDataset
-    pymovements.datasets.definitions.GazeBase
-    pymovements.datasets.definitions.JuDo1000
+    pymovements.dataset.Dataset
+    pymovements.dataset.DatasetDefinition
+    pymovements.dataset.DatasetLibrary
+    pymovements.dataset.DatasetPaths
 """
-from pymovements.datasets import definitions  # noqa:F401
-from pymovements.datasets.dataset import Dataset  # noqa: F401
-from pymovements.datasets.definitions import GazeBase  # noqa: F401
-from pymovements.datasets.definitions import JuDo1000  # noqa: F401
-from pymovements.datasets.definitions import ToyDataset  # noqa: F401
-from pymovements.datasets.public_dataset import PublicDataset  # noqa: F401
-from pymovements.datasets.public_dataset import PublicDatasetDefinition  # noqa: F401
+from pymovements.dataset.dataset import Dataset  # noqa: F401
+from pymovements.dataset.dataset_definition import DatasetDefinition  # noqa: F401
+from pymovements.dataset.dataset_library import DatasetLibrary  # noqa: F401
+from pymovements.dataset.dataset_library import register_dataset  # noqa: F401
+from pymovements.dataset.dataset_paths import DatasetPaths  # noqa: F401
```

### Comparing `pymovements-0.8.0/src/pymovements/datasets/definitions/__init__.py` & `pymovements-0.9.0/src/pymovements/datasets/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,11 +13,22 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""This module holds all dataset definitions."""
-from pymovements.datasets.definitions.gazebase import GazeBase  # noqa: F401
-from pymovements.datasets.definitions.judo1000 import JuDo1000  # noqa: F401
-from pymovements.datasets.definitions.toy_dataset import ToyDataset  # noqa: F401
+"""This module holds all dataset definitions.
+
+.. rubric:: Dataset Definitions
+
+.. autosummary::
+   :toctree:
+   :template: class.rst
+
+    pymovements.datasets.ToyDataset
+    pymovements.datasets.GazeBase
+    pymovements.datasets.JuDo1000
+"""
+from pymovements.datasets.gazebase import GazeBase  # noqa: F401
+from pymovements.datasets.judo1000 import JuDo1000  # noqa: F401
+from pymovements.datasets.toy_dataset import ToyDataset  # noqa: F401
```

### Comparing `pymovements-0.8.0/src/pymovements/datasets/definitions/gazebase.py` & `pymovements-0.9.0/src/pymovements/datasets/gazebase.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 """This module provides an interface to the GazeBase dataset."""
 from __future__ import annotations
 
 from dataclasses import dataclass
 from dataclasses import field
 from typing import Any
 
-from pymovements.datasets.public_dataset import PublicDatasetDefinition
-from pymovements.datasets.public_dataset import register_public_dataset
+from pymovements.dataset.dataset_definition import DatasetDefinition
+from pymovements.dataset.dataset_library import register_dataset
 from pymovements.gaze.experiment import Experiment
 
 
 @dataclass
-@register_public_dataset
-class GazeBase(PublicDatasetDefinition):
+@register_dataset
+class GazeBase(DatasetDefinition):
     """GazeBase dataset :cite:p:`GazeBase`.
 
     This dataset includes monocular (left eye) eye tracking data from 322 participants captured over
     a period of 37 months. Participants attended up to 9 rounds during this time frame, with each
     round consisting of two contiguous sessions.
 
     Eye movements are recorded at a sampling frequency of 1000 Hz using an EyeLink 1000 video-based
@@ -82,15 +82,15 @@
     Examples
     --------
     Initialize your :py:class:`~pymovements.PublicDataset` object with the
     :py:class:`~pymovements.GazeBase` definition:
 
     >>> import pymovements as pm
     >>>
-    >>> dataset = pm.PublicDataset("GazeBase", root='data/')
+    >>> dataset = pm.Dataset("GazeBase", path='data/GazeBase')
 
     Download the dataset resources resources:
 
     >>> dataset.download()# doctest: +SKIP
 
     Load the data into memory:
```

### Comparing `pymovements-0.8.0/src/pymovements/datasets/definitions/judo1000.py` & `pymovements-0.9.0/src/pymovements/datasets/judo1000.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 # SOFTWARE.
 """This module provides an interface to the JuDo1000 dataset."""
 from __future__ import annotations
 
 from dataclasses import dataclass
 from dataclasses import field
 
-from pymovements.datasets.public_dataset import PublicDatasetDefinition
-from pymovements.datasets.public_dataset import register_public_dataset
+from pymovements.dataset.dataset_definition import DatasetDefinition
+from pymovements.dataset.dataset_library import register_dataset
 from pymovements.gaze.experiment import Experiment
 
 
 @dataclass
-@register_public_dataset
-class JuDo1000(PublicDatasetDefinition):
+@register_dataset
+class JuDo1000(DatasetDefinition):
     """JuDo1000 dataset :cite:p:`JuDo1000`.
 
     This dataset includes binocular eye tracking data from 150 participants in four sessions with an
     interval of at least one week between two sessions. Eye movements are recorded at a sampling
     frequency of 1000 Hz using an EyeLink Portable Duo video-based eye tracker and are provided as
     pixel coordinates. Participants are instructed to watch a random jumping dot on a computer
     screen.
@@ -75,15 +75,15 @@
     Examples
     --------
     Initialize your :py:class:`~pymovements.PublicDataset` object with the
     :py:class:`~pymovements.JuDo1000` definition:
 
     >>> import pymovements as pm
     >>>
-    >>> dataset = pm.PublicDataset("JuDo1000", root='data/')
+    >>> dataset = pm.Dataset("JuDo1000", path='data/JuDo1000')
 
     Download the dataset resources resources:
 
     >>> dataset.download()# doctest: +SKIP
 
     Load the data into memory:
```

### Comparing `pymovements-0.8.0/src/pymovements/datasets/definitions/toy_dataset.py` & `pymovements-0.9.0/src/pymovements/datasets/toy_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 # SOFTWARE.
 """This module provides an interface to the pymovements example toy dataset."""
 from __future__ import annotations
 
 from dataclasses import dataclass
 from dataclasses import field
 
-from pymovements.datasets.public_dataset import PublicDatasetDefinition
-from pymovements.datasets.public_dataset import register_public_dataset
+from pymovements.dataset.dataset_definition import DatasetDefinition
+from pymovements.dataset.dataset_library import register_dataset
 from pymovements.gaze.experiment import Experiment
 
 
 @dataclass
-@register_public_dataset
-class ToyDataset(PublicDatasetDefinition):
+@register_dataset
+class ToyDataset(DatasetDefinition):
     """Example toy dataset.
 
     This dataset includes monocular eye tracking data from a single participants in a single
     session. Eye movements are recorded at a sampling frequency of 1000 Hz using an EyeLink Portable
     Duo video-based eye tracker and are provided as pixel coordinates.
 
     The participant is instructed to read 4 texts with 5 screens each.
@@ -73,15 +73,15 @@
     Examples
     --------
     Initialize your :py:class:`~pymovements.PublicDataset` object with the
     :py:class:`~pymovements.ToyDataset` definition:
 
     >>> import pymovements as pm
     >>>
-    >>> dataset = pm.PublicDataset("ToyDataset", root='data/')
+    >>> dataset = pm.Dataset("ToyDataset", path='data/ToyDataset')
 
     Download the dataset resources resources:
 
     >>> dataset.download()# doctest: +SKIP
 
     Load the data into memory:
```

### Comparing `pymovements-0.8.0/src/pymovements/events/__init__.py` & `pymovements-0.9.0/src/pymovements/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/events/detection/__init__.py` & `pymovements-0.9.0/src/pymovements/events/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/events/detection/engbert.py` & `pymovements-0.9.0/src/pymovements/events/detection/engbert.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/events/detection/idt.py` & `pymovements-0.9.0/src/pymovements/events/detection/idt.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,32 +90,46 @@
     Returns
     -------
     pl.DataFrame
         A dataframe with detected fixations as rows.
 
     Raises
     ------
+    TypeError
+        If minimum_duration is not of type ``int`` or timesteps
     ValueError
         If positions is not shaped (N, 2)
         If dispersion_threshold is not greater than 0
         If duration_threshold is not greater than 0
     """
     positions = np.array(positions)
     velocities = np.array(velocities)
     checks.check_shapes_positions_velocities(positions=positions, velocities=velocities)
 
     if timesteps is None:
         timesteps = np.arange(len(velocities), dtype=np.int64)
-    timesteps = np.array(timesteps)
+    timesteps = np.array(timesteps).flatten()
+
+    # Check that timesteps are integers or are floats without a fractional part.
+    timesteps_int = timesteps.astype(int)
+    if np.any((timesteps - timesteps_int) != 0):
+        raise TypeError('timesteps must be of type int')
+    timesteps = timesteps_int
+
     checks.check_is_length_matching(velocities=velocities, timesteps=timesteps)
 
     if dispersion_threshold <= 0:
-        raise ValueError('dispersion threshold must be greater than 0')
+        raise ValueError('dispersion_threshold must be greater than 0')
     if minimum_duration <= 0:
-        raise ValueError('minimum duration must be greater than 0')
+        raise ValueError('minimum_duration must be greater than 0')
+    if not isinstance(minimum_duration, int):
+        raise TypeError(
+            'minimum_duration must be of type int'
+            f' but is of type {type(minimum_duration)}',
+        )
 
     onsets = []
     offsets = []
 
     # Infer minimum duration in number of samples.
     # This implementation is currently very restrictive.
     # It requires that the interval between timesteps is constant.
@@ -123,35 +137,40 @@
     timesteps_diff = np.diff(timesteps)
     if not np.all(timesteps_diff == timesteps_diff[0]):
         raise ValueError('interval between timesteps must be constant')
     if not minimum_duration % timesteps_diff[0] == 0:
         raise ValueError(
             'minimum_duration must be divisible by the constant interval between timesteps',
         )
-    minimum_sample_duration = minimum_duration // timesteps_diff[0]
+    minimum_sample_duration = int(minimum_duration // timesteps_diff[0])
+    if minimum_sample_duration < 2:
+        raise ValueError('minimum_duration must be longer than the equivalent of 2 samples')
 
     # Initialize window over first points to cover the duration threshold
     win_start = 0
     win_end = minimum_sample_duration
 
-    while win_end < len(positions):
+    while win_start < len(timesteps) and win_end <= len(timesteps):
 
         # Initialize window over first points to cover the duration threshold.
         # This automatically extends the window to the specified minimum event duration.
         win_end = max(win_start + minimum_sample_duration, win_end)
+        win_end = min(win_end, len(timesteps))
+        if win_end - win_start < minimum_sample_duration:
+            break
 
         if dispersion(positions[win_start:win_end]) <= dispersion_threshold:
             # Add additional points to the window until dispersion > threshold.
             while dispersion(positions[win_start:win_end]) < dispersion_threshold:
-                win_end += 1
-
                 # break if we reach end of input data
-                if win_end == len(positions):
+                if win_end == len(timesteps):
                     break
 
+                win_end += 1
+
             # check for np.nan values
             if np.sum(np.isnan(positions[win_start:win_end - 1])) > 0:
                 tmp_candidates = [np.arange(win_start, win_end - 1, 1)]
                 tmp_candidates = filter_candidates_remove_nans(
                     candidates=tmp_candidates,
                     values=positions,
                 )
```

### Comparing `pymovements-0.8.0/src/pymovements/events/detection/ivt.py` & `pymovements-0.9.0/src/pymovements/events/detection/ivt.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/events/event_processing.py` & `pymovements-0.9.0/src/pymovements/events/event_processing.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/events/event_properties.py` & `pymovements-0.9.0/src/pymovements/events/event_properties.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/events/events.py` & `pymovements-0.9.0/src/pymovements/events/events.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/exceptions.py` & `pymovements-0.9.0/src/pymovements/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/gaze/__init__.py` & `pymovements-0.9.0/src/pymovements/gaze/__init__.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/gaze/experiment.py` & `pymovements-0.9.0/src/pymovements/gaze/experiment.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/gaze/gaze_dataframe.py` & `pymovements-0.9.0/src/pymovements/gaze/gaze_dataframe.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/gaze/screen.py` & `pymovements-0.9.0/src/pymovements/gaze/screen.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/gaze/transforms.py` & `pymovements-0.9.0/src/pymovements/gaze/transforms.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/plotting/__init__.py` & `pymovements-0.9.0/src/pymovements/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/plotting/heatmap.py` & `pymovements-0.9.0/src/pymovements/plotting/heatmap.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/plotting/main_sequence_plot.py` & `pymovements-0.9.0/src/pymovements/plotting/main_sequence_plot.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,56 +22,69 @@
 """
 from __future__ import annotations
 
 import matplotlib.pyplot as plt
 import polars as pl
 from polars import ColumnNotFoundError
 
+from pymovements.events import EventDataFrame
+
 
 def main_sequence_plot(
-        data: pl.DataFrame,
+        event_df: EventDataFrame,
         figsize: tuple[int, int] = (15, 5),
         title: str | None = None,
         savepath: str | None = None,
         show: bool = True,
 ) -> None:
     """
     Plots the saccade main sequence.
 
     Parameters
     ----------
-    data:
-        Data frame. It must contain columns "peak_velocity" and "amplitude".
+    event_df:
+        Event dataframe. It must contain columns "peak_velocity" and "amplitude".
     figsize: tuple
         Figure size.
     title: str, optional
         Figure title.
     savepath: str, optional
         If given, figure will be saved to this path.
     show: bool
         If True, figure will be shown.
 
     Raises
     ------
     KeyError
         If the input dataframe has no 'amplitude' and/or 'peak_velocity' column.
         Those are needed to create the plot.
+    ValueError
+        If the event dataframe does not contain any saccades.
     """
+    event_col_name = 'name'
+    saccades = event_df.frame.filter(pl.col(event_col_name) == 'saccade')
+
+    if saccades.is_empty():
+        raise ValueError(
+            'There are no saccades in the event dataframe. '
+            'Please make sure you ran a saccade detection algorithm. '
+            f'The event name should be stored in a colum called "{event_col_name}".',
+        )
 
     try:
-        peak_velocities = data['peak_velocity'].to_list()
+        peak_velocities = saccades['peak_velocity'].to_list()
     except ColumnNotFoundError as exc:
         raise KeyError(
             'The input dataframe you provided does not contain '
             'the saccade peak velocities which are needed to create '
             'the main sequence plot. ',
         ) from exc
 
     try:
-        amplitudes = data['amplitude'].to_list()
+        amplitudes = saccades['amplitude'].to_list()
     except ColumnNotFoundError as exc:
         raise KeyError(
             'The input dataframe you provided does not contain '
             'the saccade amplitudes which are needed to create '
             'the main sequence plot. ',
         ) from exc
```

### Comparing `pymovements-0.8.0/src/pymovements/plotting/traceplot.py` & `pymovements-0.9.0/src/pymovements/plotting/traceplot.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/plotting/tsplot.py` & `pymovements-0.9.0/src/pymovements/plotting/tsplot.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/synthetic/__init__.py` & `pymovements-0.9.0/src/pymovements/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/synthetic/step_function.py` & `pymovements-0.9.0/src/pymovements/synthetic/step_function.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/utils/archives.py` & `pymovements-0.9.0/src/pymovements/utils/archives.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/utils/checks.py` & `pymovements-0.9.0/src/pymovements/utils/checks.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/utils/decorators.py` & `pymovements-0.9.0/src/pymovements/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/utils/downloads.py` & `pymovements-0.9.0/src/pymovements/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/utils/filters.py` & `pymovements-0.9.0/src/pymovements/utils/filters.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/utils/parsing.py` & `pymovements-0.9.0/src/pymovements/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `pymovements-0.8.0/src/pymovements/utils/paths.py` & `pymovements-0.9.0/src/pymovements/utils/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,20 @@
 
     Raises
     ------
     ValueError
         If ``path`` does not point to a directory.
     """
     path = Path(path)
+
+    if not path.exists():
+        raise ValueError(f'path does not exist (path = {path})')
+
     if not path.is_dir():
-        raise ValueError(f'path must point to a directory, but points to a file (path = {path})')
+        raise ValueError(f'path must point to a directory (path = {path})')
 
     if relative and relative_anchor is None:
         relative_anchor = path
 
     match_dicts: list[dict[str, str]] = []
     for childpath in path.iterdir():
         if childpath.is_dir():
```

### Comparing `pymovements-0.8.0/src/pymovements.egg-info/PKG-INFO` & `pymovements-0.9.0/src/pymovements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymovements
-Version: 0.8.0
+Version: 0.9.0
 Summary: A python package for processing eye movement data
 Maintainer-email: Daniel Krakowczyk <daniel.krakowczyk@uni-potsdam.de>
 License: MIT License
 Project-URL: Homepage, https://github.com/aeye-lab/pymovements
 Project-URL: Source Code, https://github.com/aeye-lab/pymovements
 Project-URL: Documentation, https://pymovements.readthedocs.io/en/stable
 Project-URL: Bug Tracker, https://github.com/aeye-lab/pymovements/issues
```

### Comparing `pymovements-0.8.0/src/pymovements.egg-info/SOURCES.txt` & `pymovements-0.9.0/src/pymovements.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 src/pymovements/__init__.py
 src/pymovements/exceptions.py
 src/pymovements.egg-info/PKG-INFO
 src/pymovements.egg-info/SOURCES.txt
 src/pymovements.egg-info/dependency_links.txt
 src/pymovements.egg-info/requires.txt
 src/pymovements.egg-info/top_level.txt
+src/pymovements/dataset/__init__.py
+src/pymovements/dataset/dataset.py
+src/pymovements/dataset/dataset_definition.py
+src/pymovements/dataset/dataset_download.py
+src/pymovements/dataset/dataset_files.py
+src/pymovements/dataset/dataset_library.py
+src/pymovements/dataset/dataset_paths.py
 src/pymovements/datasets/__init__.py
-src/pymovements/datasets/dataset.py
-src/pymovements/datasets/public_dataset.py
-src/pymovements/datasets/definitions/__init__.py
-src/pymovements/datasets/definitions/gazebase.py
-src/pymovements/datasets/definitions/judo1000.py
-src/pymovements/datasets/definitions/toy_dataset.py
+src/pymovements/datasets/gazebase.py
+src/pymovements/datasets/judo1000.py
+src/pymovements/datasets/toy_dataset.py
 src/pymovements/events/__init__.py
 src/pymovements/events/event_processing.py
 src/pymovements/events/event_properties.py
 src/pymovements/events/events.py
 src/pymovements/events/detection/__init__.py
 src/pymovements/events/detection/engbert.py
 src/pymovements/events/detection/idt.py
```

