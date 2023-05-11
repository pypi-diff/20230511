# Comparing `tmp/tvb-widgets-1.4.1.tar.gz` & `tmp/tvb-widgets-1.4.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-widgets-1.4.1.tar", last modified: Wed May 10 20:02:29 2023, max compression
+gzip compressed data, was "tvb-widgets-1.4.2a1.tar", last modified: Thu May 11 21:19:47 2023, max compression
```

## Comparing `tvb-widgets-1.4.1.tar` & `tvb-widgets-1.4.2a1.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:29.933364 tvb-widgets-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35796 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-10 20:02:29.933364 tvb-widgets-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 20:02:29.933364 tvb-widgets-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:29.929364 tvb-widgets-1.4.1/tvb_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-10 20:02:29.000000 tvb-widgets-1.4.1/tvb_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-10 20:02:29.000000 tvb-widgets-1.4.1/tvb_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:02:29.000000 tvb-widgets-1.4.1/tvb_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-10 20:02:29.000000 tvb-widgets-1.4.1/tvb_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 20:02:29.000000 tvb-widgets-1.4.1/tvb_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:29.929364 tvb-widgets-1.4.1/tvbwidgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:29.929364 tvb-widgets-1.4.1/tvbwidgets/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:29.929364 tvb-widgets-1.4.1/tvbwidgets/core/hpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/hpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/hpc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/hpc/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/ini_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:29.929364 tvb-widgets-1.4.1/tvbwidgets/core/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/logger/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/logger/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:29.929364 tvb-widgets-1.4.1/tvbwidgets/core/pse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/pse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/pse/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/pse/pse_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:29.929364 tvb-widgets-1.4.1/tvbwidgets/core/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/simulator/model_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/core/simulator/tvb_integrators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:29.933364 tvb-widgets-1.4.1/tvbwidgets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/tests/test_drive_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/tests/test_head_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/tests/test_phase_plane_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/tests/test_ts_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/tests/test_tvb_integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/tests/ts_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:29.933364 tvb-widgets-1.4.1/tvbwidgets/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/ui/base_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/ui/drive_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/ui/head_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    36150 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/ui/phase_plane_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/ui/pse_launcher_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/ui/pse_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/ui/storage_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/ui/ts_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/ui/ts_widget_help.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-10 20:02:23.000000 tvb-widgets-1.4.1/tvbwidgets/ui/widget_with_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35796 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.467730 tvb-widgets-1.4.2a1/tvb_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-11 21:19:47.000000 tvb-widgets-1.4.2a1/tvb_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-11 21:19:47.000000 tvb-widgets-1.4.2a1/tvb_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:19:47.000000 tvb-widgets-1.4.2a1/tvb_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-11 21:19:47.000000 tvb-widgets-1.4.2a1/tvb_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 21:19:47.000000 tvb-widgets-1.4.2a1/tvb_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.467730 tvb-widgets-1.4.2a1/tvbwidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/core/hpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/hpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/hpc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/hpc/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/ini_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/core/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/logger/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/logger/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/core/pse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/pse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/pse/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/pse/pse_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/pse/toml_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/core/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/simulator/model_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/core/simulator/tvb_integrators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_drive_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_head_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_phase_plane_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_pse_stage_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_ts_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/test_tvb_integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/tests/ts_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:47.471730 tvb-widgets-1.4.2a1/tvbwidgets/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/base_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/drive_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/head_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36150 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/phase_plane_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/pse_launcher_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/pse_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/storage_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/ts_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/ts_widget_help.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-11 21:19:39.000000 tvb-widgets-1.4.2a1/tvbwidgets/ui/widget_with_browser.py
```

### Comparing `tvb-widgets-1.4.1/LICENSE` & `tvb-widgets-1.4.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/PKG-INFO` & `tvb-widgets-1.4.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-widgets
-Version: 1.4.1
+Version: 1.4.2a1
 Summary: GUI widgets for EBRAINS showcases
 Home-page: https://github.com/the-virtual-brain/tvb-widgets
 Author: TVB Widgets Team (Juelich SDL Neuroscience, INS - Marseille, Codemart)
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb widgets jupyterlab ebrains showcases
 Platform: UNKNOWN
```

### Comparing `tvb-widgets-1.4.1/README.md` & `tvb-widgets-1.4.2a1/README.md`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/setup.py` & `tvb-widgets-1.4.2a1/setup.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvb_widgets.egg-info/PKG-INFO` & `tvb-widgets-1.4.2a1/tvb_widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-widgets
-Version: 1.4.1
+Version: 1.4.2a1
 Summary: GUI widgets for EBRAINS showcases
 Home-page: https://github.com/the-virtual-brain/tvb-widgets
 Author: TVB Widgets Team (Juelich SDL Neuroscience, INS - Marseille, Codemart)
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb widgets jupyterlab ebrains showcases
 Platform: UNKNOWN
```

### Comparing `tvb-widgets-1.4.1/tvb_widgets.egg-info/SOURCES.txt` & `tvb-widgets-1.4.2a1/tvb_widgets.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 tvbwidgets/core/hpc/launcher.py
 tvbwidgets/core/logger/__init__.py
 tvbwidgets/core/logger/builder.py
 tvbwidgets/core/logger/logging.conf
 tvbwidgets/core/pse/__init__.py
 tvbwidgets/core/pse/parameters.py
 tvbwidgets/core/pse/pse_data.py
+tvbwidgets/core/pse/toml_storage.py
 tvbwidgets/core/simulator/__init__.py
 tvbwidgets/core/simulator/model_exporters.py
 tvbwidgets/core/simulator/tvb_integrators.py
 tvbwidgets/tests/__init__.py
 tvbwidgets/tests/constants.py
 tvbwidgets/tests/test_base.py
 tvbwidgets/tests/test_drive_widget.py
 tvbwidgets/tests/test_exporters.py
 tvbwidgets/tests/test_head_widget.py
 tvbwidgets/tests/test_phase_plane_export.py
+tvbwidgets/tests/test_pse_stage_in.py
 tvbwidgets/tests/test_ts_widget.py
 tvbwidgets/tests/test_tvb_integrators.py
 tvbwidgets/tests/ts_generator.py
 tvbwidgets/ui/__init__.py
 tvbwidgets/ui/base_widget.py
 tvbwidgets/ui/drive_widget.py
 tvbwidgets/ui/head_widget.py
```

### Comparing `tvb-widgets-1.4.1/tvbwidgets/__init__.py` & `tvb-widgets-1.4.2a1/tvbwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/api.py` & `tvb-widgets-1.4.2a1/tvbwidgets/api.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/core/auth.py` & `tvb-widgets-1.4.2a1/tvbwidgets/core/auth.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/core/exceptions.py` & `tvb-widgets-1.4.2a1/tvbwidgets/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/core/hpc/config.py` & `tvb-widgets-1.4.2a1/tvbwidgets/core/hpc/config.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/core/hpc/launcher.py` & `tvb-widgets-1.4.2a1/tvbwidgets/core/hpc/launcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,47 +3,51 @@
 # "TheVirtualBrain - Widgets" package
 #
 # (c) 2022-2023, TVB Widgets Team
 #
 
 import time
 import pyunicore.client
+from pathlib import Path
 from typing import Callable
 from datetime import datetime
 from urllib.error import HTTPError
 from pyunicore.helpers.jobs import Status, Description
 from pyunicore.credentials import AuthenticationFailedException
 from pkg_resources import get_distribution, DistributionNotFound
 from tvbwidgets.core.auth import get_current_token
 from tvbwidgets.core.hpc.config import HPCConfig
 from tvbwidgets.core.logger.builder import get_logger
 from tvbwidgets.core.pse.parameters import PROGRESS_STATUS
+from tvb.simulator.simulator import Simulator
+from tvbwidgets.core.pse.toml_storage import TOMLStorage
 
 LOGGER = get_logger(__name__)
 
 
 class HPCLaunch(object):
     pip_libraries = 'tvb-widgets tvb-data'
     EXECUTABLE_KEY = 'Executable'
     PROJECT_KEY = 'Project'
     JOB_TYPE_KEY = 'Job type'
     INTERACTIVE_KEY = 'interactive'
 
-    def __init__(self, hpc_config, param1, param2, param1_values, param2_values, metrics, file_name, update_progress):
-        # type: (HPCConfig, str, str, list, list, list, str, Callable) -> None
+    def __init__(self, simulator, hpc_config, param1, param2, param1_values, param2_values, metrics, file_name,
+                 update_progress):
+        # type: (Simulator, HPCConfig, str, str, list, list, list, str, Callable) -> None
         self.config = hpc_config
         self.param1 = param1
         self.param2 = param2
         self.param1_values = param1_values
         self.param2_values = param2_values
         self.metrics = metrics
         self.file_name = file_name
         self.update_progress = update_progress
-        # TODO WID-208 link here the serialized simulator in the list of inputs
-        self.submit_job("tvbwidgets.core.pse.parameters", [], True)
+        serialized_config = self._serialize_configuration(simulator)
+        self.submit_job("tvbwidgets.core.pse.parameters", serialized_config, True)
 
     @property
     def _activate_command(self):
         return f'source ${self.config.storage_name}/{self.config.env_dir}/{self.config.env_name}/bin/activate'
 
     @property
     def _module_load_command(self):
@@ -55,14 +59,36 @@
                f'&& rm -rf {self.config.env_name} ' \
                f'&& python -mvenv {self.config.env_name}'
 
     @property
     def _install_dependencies_command(self):
         return f'pip install -U pip && pip install {self.pip_libraries}'
 
+    def _serialize_configuration(self, sim):
+        # type: (Simulator) -> Path
+        if self.param1 == "connectivity":
+            param1_values = self.get_connectivity_files(self.param1_values)
+            param2_values = self.param2_values
+        elif self.param2 == "connectivity":
+            param1_values = self.param1_values
+            param2_values = self.get_connectivity_files(self.param2_values)
+        else:
+            param1_values = self.param1_values
+            param2_values = self.param2_values
+
+        return TOMLStorage.write_pse_in_file(sim, self.param1, self.param2, param1_values, param2_values,
+                                             self.metrics, self.config.n_threads, self.file_name)
+
+    def get_connectivity_files(self, values):
+        connectivity_files = []
+        for connectivity in values:
+            connectivity_files.append(f"connectivity_{connectivity.tract_lengths.shape[0]}.zip")
+
+        return connectivity_files
+
     def connect_client(self):
         LOGGER.info(f"Connecting to {self.config.site}...")
         token = get_current_token()
         transport = pyunicore.client.Transport(token)
         registry = pyunicore.client.Registry(transport, pyunicore.client._HBP_REGISTRY_URL)
 
         try:
@@ -138,15 +164,16 @@
         return None
 
     @staticmethod
     def _format_date_for_job(job):
         date = datetime.strptime(job.properties['submissionTime'], '%Y-%m-%dT%H:%M:%S+%f')
         return date.strftime('%m.%d.%Y, %H_%M_%S')
 
-    def submit_job(self, executable, inputs, do_stage_out):
+    def submit_job(self, executable, path_input, do_stage_out):
+        # type (str, Path, bool) -> None
         client = self.connect_client()
         if client is None:
             LOGGER.error(f"Could not connect to {self.config.site}, stopping execution.")
             return
 
         home_storage = self._search_for_home_dir(client)
         if home_storage is None:
@@ -172,23 +199,22 @@
             job_env_prep.poll()
             if job_env_prep.properties['status'] == Status.FAILED:
                 LOGGER.error("Encountered an error during environment setup, stopping execution.")
                 return
             LOGGER.info("Successfully finished the environment setup.")
 
         command = f"{self._module_load_command} && {self._activate_command} && " \
-                  f"python -m  {executable} {self.param1} {self.param2} '{self.param1_values}' " \
-                  f"'{self.param2_values}' '{self.metrics}' {self.file_name} {self.config.n_threads}"
+                  f"python -m {executable} {path_input}"
         LOGGER.info(f"Launching workflow for command: \n {command}")
         job = Description(
             executable=command,
             project=self.config.project,
             resources=self.config.resources
         )
-        job_workflow = client.new_job(job.to_dict(), inputs=inputs)
+        job_workflow = client.new_job(job.to_dict(), inputs=[path_input.as_posix()])
         LOGGER.info(f"Job is running at {self.config.site}: {job_workflow.working_dir.properties['mountPoint']}. "
                     f"Submission time is: {self._format_date_for_job(job_workflow)}.")
         LOGGER.info('Finished remote launch.')
 
         if do_stage_out:
             self.monitor_job(job_workflow)
         else:
```

### Comparing `tvb-widgets-1.4.1/tvbwidgets/core/ini_parser.py` & `tvb-widgets-1.4.2a1/tvbwidgets/core/ini_parser.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/core/logger/builder.py` & `tvb-widgets-1.4.2a1/tvbwidgets/core/logger/builder.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/core/logger/logging.conf` & `tvb-widgets-1.4.2a1/tvbwidgets/core/logger/logging.conf`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/core/pse/parameters.py` & `tvb-widgets-1.4.2a1/tvbwidgets/core/pse/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,31 +9,30 @@
 - Temporary copy from tvb-inversion package
 
 .. moduleauthor: Fousek Jan <jan.fousek@univ-amu.fr>
 .. moduleauthor: Teodora Misan <teodora.misan@codemart.ro>
 """
 
 import os
-import json
 import sys
 import threading
 import numpy as np
 from copy import deepcopy
 from typing import List, Any, Optional, Callable
 from dataclasses import dataclass
 from tvb.analyzers.metric_variance_global import compute_variance_global_metric
 from tvb.analyzers.metric_kuramoto_index import compute_kuramoto_index_metric
 from tvb.analyzers.metric_proxy_metastability import compute_proxy_metastability_metric
 from tvb.analyzers.metric_variance_of_node_variance import compute_variance_of_node_variance_metric
-from tvb.datatypes.connectivity import Connectivity
 from tvb.datatypes.time_series import TimeSeries
 from tvb.simulator.simulator import Simulator
 from joblib import Parallel, delayed
 from tvbwidgets.core.pse.pse_data import PSEData, PSEStorage
 from tvbwidgets.core.logger.builder import get_logger
+from tvbwidgets.core.pse.toml_storage import TOMLStorage
 
 # Here put explicit module name string, for __name__ == __main__
 LOGGER = get_logger("tvbwidgets.core.pse.parameters")
 
 PROGRESS_STATUS = "progress_status.txt"
 
 try:
@@ -80,22 +79,22 @@
             exec(f'obj.{key} = val',
                  {'obj': obj, 'val': val})
         self.pos += 1
         return obj
 
 
 class Metric:
-    "A summary statistic for a simulation."
+    """A summary statistic for a simulation."""
 
     def __call__(self, t, y) -> np.ndarray:  # what about multi metric returning dict of statistics? Also, chaining?
         pass
 
 
 class NodeVariability(Metric):
-    "A simplistic simulation statistic."
+    """A simplistic simulation statistic."""
 
     def __call__(self, t, y):
         return np.std(y[t > (t[-1] / 2), 0, :, 0], axis=0)
 
 
 class GlobalVariance(Metric):
 
@@ -194,18 +193,18 @@
             pse_result.y_value = id_values
         else:
             pse_result.y_value = self.y_values
 
         pse_result.metrics_names = self.metrics
         pse_result.results = metrics_data_np.reshape((len(self.metrics), len(self.x_values), len(self.y_values)))
 
-        f = PSEStorage(self.file_name)
-        f.store(pse_result)
+        pse_file = PSEStorage(self.file_name)
+        pse_file.store(pse_result)
         LOGGER.info(f"{self.file_name} file created")
-        f.close()
+        pse_file.close()
 
 
 @dataclass
 class PostProcess:
     metrics: List[Metric]
     reduction: Reduction
 
@@ -356,58 +355,51 @@
         else:
             resulted_metric = VarianceNodeVariance(sim.monitors[0].period)
         computed_metrics.append(resulted_metric)
 
     return computed_metrics
 
 
-def launch_local_param(simulator, param1, param2, x_values, y_values, metrics, file_name,
+def launch_local_param(sim, param1, param2, x_values, y_values, metrics, file_name,
                        update_progress=None, n_threads=4):
     input_values = []
     for elem1 in x_values:
         for elem2 in y_values:
             if param1 == "conduction_speed" or param1 == "connectivity":
                 el1_value = elem1
             else:
                 el1_value = np.array([elem1])
             if param2 == "conduction_speed" or param2 == "connectivity":
                 el2_value = elem2
             else:
                 el2_value = np.array([elem2])
             input_values.append([el1_value, el2_value])
 
-    sim = simulator.configure()  # deepcopy doesn't work on un-configured simulator o_O
+    sim = sim.configure()  # deepcopy doesn't work on un-configured simulator o_O
     seq = SimSeq(
         template=sim,
         params=[param1, param2],
         values=input_values
     )
     pp = PostProcess(
         metrics=compute_metrics(sim, metrics),
         reduction=SaveDataToDisk(param1, param2, x_values, y_values, metrics, file_name),
     )
     exe = JobLibExec(seq=seq, post=pp, backend=None, checkpoint_dir=None, update_progress=update_progress)
     exe(n_jobs=n_threads)
 
 
 if __name__ == '__main__':
-    param1 = sys.argv[1]
-    param2 = sys.argv[2]
-    param1_values = json.loads(sys.argv[3])
-    param2_values = json.loads(sys.argv[4])
-    n = len(sys.argv[5])
-    metrics = sys.argv[5][1:n - 1].split(', ')
-    file_name = sys.argv[6]
-    n_threads = int(sys.argv[7])
-
-    LOGGER.info(f"We are now starting PSE for '{param1}' x '{param2}' on {n_threads} threads\n"
-                f"Expect the result in '{file_name}' \n"
-                f"{n} Metrics {metrics}")
-
-    # TODO WID-208 deserialize this instance after being passed from the remote launcher
-    sim = Simulator(connectivity=Connectivity.from_file()).configure()
+    in_file = sys.argv[1]
+    name_param1, vals_param1, name_param2, vals_param2, \
+        metrics_list, result_file, n_th, sim_obj = TOMLStorage.read_pse_from_file(in_file)
+
+    LOGGER.info(f"We are now starting PSE for '{name_param1}' x '{name_param2}' on {n_th} threads\n"
+                f"Expect the result in '{result_file}' \n"
+                f"Metrics {metrics_list} \n"
+                f"Simulator {sim_obj}")
 
     with open(PROGRESS_STATUS, "w+") as f:
         f.write("0")
 
-    launch_local_param(sim, param1, param2, param1_values, param2_values, metrics, file_name,
-                       n_threads=n_threads)
+    launch_local_param(sim_obj, name_param1, name_param2, vals_param1, vals_param2, metrics_list, result_file,
+                       n_threads=n_th)
```

### Comparing `tvb-widgets-1.4.1/tvbwidgets/core/pse/pse_data.py` & `tvb-widgets-1.4.2a1/tvbwidgets/core/pse/pse_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # "TheVirtualBrain - Widgets" package
 #
 # (c) 2022-2023, TVB Widgets Team
 #
 
-from tvb.basic.neotraits.api import NArray, HasTraits, Range, List, Attr
+from tvb.basic.neotraits.api import NArray, HasTraits, Attr
 from tvb.core.neotraits.h5 import H5File, DataSet, Scalar, Json
 
 
 class PSEData(HasTraits):
     x_title = Attr(str)
     y_title = Attr(str)
     x_value = Attr(list)
```

### Comparing `tvb-widgets-1.4.1/tvbwidgets/core/simulator/model_exporters.py` & `tvb-widgets-1.4.2a1/tvbwidgets/core/simulator/model_exporters.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/core/simulator/tvb_integrators.py` & `tvb-widgets-1.4.2a1/tvbwidgets/core/simulator/tvb_integrators.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/tests/test_base.py` & `tvb-widgets-1.4.2a1/tvbwidgets/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/tests/test_drive_widget.py` & `tvb-widgets-1.4.2a1/tvbwidgets/tests/test_drive_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/tests/test_exporters.py` & `tvb-widgets-1.4.2a1/tvbwidgets/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/tests/test_head_widget.py` & `tvb-widgets-1.4.2a1/tvbwidgets/tests/test_head_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/tests/test_phase_plane_export.py` & `tvb-widgets-1.4.2a1/tvbwidgets/tests/test_phase_plane_export.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/tests/test_ts_widget.py` & `tvb-widgets-1.4.2a1/tvbwidgets/tests/test_ts_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/tests/ts_generator.py` & `tvb-widgets-1.4.2a1/tvbwidgets/tests/ts_generator.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/ui/base_widget.py` & `tvb-widgets-1.4.2a1/tvbwidgets/ui/base_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/ui/drive_widget.py` & `tvb-widgets-1.4.2a1/tvbwidgets/ui/drive_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/ui/head_widget.py` & `tvb-widgets-1.4.2a1/tvbwidgets/ui/head_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/ui/phase_plane_widget.py` & `tvb-widgets-1.4.2a1/tvbwidgets/ui/phase_plane_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/ui/pse_launcher_widget.py` & `tvb-widgets-1.4.2a1/tvbwidgets/ui/pse_launcher_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
     def _prepare_launch(self, where="Local"):
         self._update_info_message(f"{where} launch in progress ...")
         x_values = self.compute_params_values(self.param_1.value)
         y_values = self.compute_params_values(self.param_2.value)
         file_name = self.verify_file_name()
         self.progress.min = 0
-        self.progress.max = len(x_values) * len(y_values) + 1   # no of simulations + 1 for preparation step
+        self.progress.max = len(x_values) * len(y_values) + 1  # no of simulations + 1 for preparation step
         self.update_progress(0)
         return file_name, x_values, y_values
 
     def handle_launch_buttons(self):
         self.launch_local_button = widgets.Button(
             description='Local launch',
             disabled=False,
@@ -104,15 +104,15 @@
             disabled=self.hpc_config is None,
             button_style='success',
         )
 
         def hpc_launch(_change):
             if self.launch_hpc_button.button_style == "success":
                 file_name, x_values, y_values = self._prepare_launch("HPC")
-                HPCLaunch(self.hpc_config, self.param_1.value, self.param_2.value, x_values, y_values,
+                HPCLaunch(self.simulator, self.hpc_config, self.param_1.value, self.param_2.value, x_values, y_values,
                           list(self.metrics_sm.value), file_name, self.update_progress)
                 self._update_info_message("PSE completed! ")
 
         def local_launch(_change):
             self.logger.info("Local launch in progress")
             if self.launch_local_button.button_style == "success":
                 file_name, x_values, y_values = self._prepare_launch("Local")
```

### Comparing `tvb-widgets-1.4.1/tvbwidgets/ui/pse_widget.py` & `tvb-widgets-1.4.2a1/tvbwidgets/ui/pse_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/ui/storage_widget.py` & `tvb-widgets-1.4.2a1/tvbwidgets/ui/storage_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/ui/ts_widget.py` & `tvb-widgets-1.4.2a1/tvbwidgets/ui/ts_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/ui/ts_widget_help.ini` & `tvb-widgets-1.4.2a1/tvbwidgets/ui/ts_widget_help.ini`

 * *Files identical despite different names*

### Comparing `tvb-widgets-1.4.1/tvbwidgets/ui/widget_with_browser.py` & `tvb-widgets-1.4.2a1/tvbwidgets/ui/widget_with_browser.py`

 * *Files identical despite different names*

