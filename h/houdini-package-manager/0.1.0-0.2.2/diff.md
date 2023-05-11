# Comparing `tmp/houdini_package_manager-0.1.0.tar.gz` & `tmp/houdini_package_manager-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "houdini_package_manager-0.1.0.tar", max compression
+gzip compressed data, was "houdini_package_manager-0.2.2.tar", max compression
```

## Comparing `houdini_package_manager-0.1.0.tar` & `houdini_package_manager-0.2.2.tar`

### file list

```diff
@@ -1,45 +1,69 @@
--rw-r--r--   0        0        0    34523 2023-05-08 08:57:40.345890 houdini_package_manager-0.1.0/LICENSE
--rw-r--r--   0        0        0     1412 2023-05-08 08:57:40.345890 houdini_package_manager-0.1.0/README.md
--rw-r--r--   0        0        0       22 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/__init__.py
--rw-r--r--   0        0        0    60498 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/houdini_package_manager.xd
--rw-r--r--   0        0        0    10421 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/add_packages.svg
--rw-r--r--   0        0        0    10424 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/add_packages_hover.svg
--rw-r--r--   0        0        0      803 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/clear_selection.svg
--rw-r--r--   0        0        0      800 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/clear_selection_hover.svg
--rw-r--r--   0        0        0      427 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/delete.svg
--rw-r--r--   0        0        0      424 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/delete_hover.svg
--rw-r--r--   0        0        0      455 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/file.svg
--rw-r--r--   0        0        0      452 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/file_hover.svg
--rw-r--r--   0        0        0      382 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/folder.svg
--rw-r--r--   0        0        0      379 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/folder_hover.svg
--rw-r--r--   0        0        0     1561 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/hpm.svg
--rw-r--r--   0        0        0      696 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/invert_selection.svg
--rw-r--r--   0        0        0      693 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/invert_selection_hover.svg
--rw-r--r--   0        0        0      323 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/migrate.svg
--rw-r--r--   0        0        0      320 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/migrate_hover.svg
--rw-r--r--   0        0        0     1455 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/refresh.svg
--rw-r--r--   0        0        0     1625 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/refresh_all.svg
--rw-r--r--   0        0        0     1622 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/refresh_all_hover.svg
--rw-r--r--   0        0        0     1452 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/refresh_hover.svg
--rw-r--r--   0        0        0      390 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/remove_all_items.svg
--rw-r--r--   0        0        0      387 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/remove_all_items_hover.svg
--rw-r--r--   0        0        0      484 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/remove_item.svg
--rw-r--r--   0        0        0      502 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/remove_item_hover.svg
--rw-r--r--   0        0        0      224 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/toggle_off.svg
--rw-r--r--   0        0        0      221 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/toggle_off_hover.svg
--rw-r--r--   0        0        0      334 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/toggle_on.svg
--rw-r--r--   0        0        0      331 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/toggle_on_hover.svg
--rw-r--r--   0        0        0      677 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/warning.svg
--rw-r--r--   0        0        0      680 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/warning_hover.svg
--rw-r--r--   0        0        0   332325 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons.ai
--rw-r--r--   0        0        0     1049 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/main.py
--rw-r--r--   0        0        0     1574 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/meta/meta_tools.py
--rw-r--r--   0        0        0      655 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/widgets/actions.py
--rw-r--r--   0        0        0     8216 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/widgets/add_packages_layout.py
--rw-r--r--   0        0        0     3574 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/widgets/custom_widgets.py
--rw-r--r--   0        0        0     3327 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/widgets/main_window.py
--rw-r--r--   0        0        0    20868 2023-05-08 08:57:40.353890 houdini_package_manager-0.1.0/houdini_package_manager/widgets/packages_layout.py
--rw-r--r--   0        0        0    12699 2023-05-08 08:57:40.353890 houdini_package_manager-0.1.0/houdini_package_manager/widgets/packages_table.py
--rw-r--r--   0        0        0    27856 2023-05-08 08:57:40.353890 houdini_package_manager-0.1.0/houdini_package_manager/wrangle/config_control.py
--rw-r--r--   0        0        0     2064 2023-05-08 08:58:21.909908 houdini_package_manager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 houdini_package_manager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-11 06:25:16.980147 houdini_package_manager-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1361 2023-05-11 06:25:16.980147 houdini_package_manager-0.2.2/README.md
+-rw-r--r--   0        0        0       22 2023-05-11 06:25:16.980147 houdini_package_manager-0.2.2/houdini_package_manager/__init__.py
+-rw-r--r--   0        0        0      847 2023-05-11 06:25:16.980147 houdini_package_manager-0.2.2/houdini_package_manager/main.py
+-rw-r--r--   0        0        0     1975 2023-05-11 06:25:16.980147 houdini_package_manager-0.2.2/houdini_package_manager/meta/meta_tools.py
+-rw-r--r--   0        0        0   614544 2023-05-11 06:25:16.988148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Black.ttf
+-rw-r--r--   0        0        0   672480 2023-05-11 06:25:16.992148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf
+-rw-r--r--   0        0        0   657188 2023-05-11 06:25:16.996148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Bold.ttf
+-rw-r--r--   0        0        0   699008 2023-05-11 06:25:17.004148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0        0        0   723544 2023-05-11 06:25:17.008148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Italic.ttf
+-rw-r--r--   0        0        0   644556 2023-05-11 06:25:17.012148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Light.ttf
+-rw-r--r--   0        0        0   658212 2023-05-11 06:25:17.020148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0        0        0   637068 2023-05-11 06:25:17.024148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Medium.ttf
+-rw-r--r--   0        0        0   695588 2023-05-11 06:25:17.028148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf
+-rw-r--r--   0        0        0   657212 2023-05-11 06:25:17.032148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Regular.ttf
+-rw-r--r--   0        0        0      332 2023-05-11 06:25:17.032148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add.svg
+-rw-r--r--   0        0        0      329 2023-05-11 06:25:17.032148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_hover.svg
+-rw-r--r--   0        0        0    10421 2023-05-11 06:25:17.032148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages.svg
+-rw-r--r--   0        0        0    10472 2023-05-11 06:25:17.032148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages_confirm.svg
+-rw-r--r--   0        0        0    10475 2023-05-11 06:25:17.032148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg
+-rw-r--r--   0        0        0    10424 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages_hover.svg
+-rw-r--r--   0        0        0     1991 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/bug.svg
+-rw-r--r--   0        0        0     1988 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/bug_hover.svg
+-rw-r--r--   0        0        0      803 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/clear_selection.svg
+-rw-r--r--   0        0        0      800 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/clear_selection_hover.svg
+-rw-r--r--   0        0        0      427 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/delete.svg
+-rw-r--r--   0        0        0      424 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/delete_hover.svg
+-rw-r--r--   0        0        0      505 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/docs.svg
+-rw-r--r--   0        0        0      502 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/docs_hover.svg
+-rw-r--r--   0        0        0      455 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/file.svg
+-rw-r--r--   0        0        0      452 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/file_hover.svg
+-rw-r--r--   0        0        0      382 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/folder.svg
+-rw-r--r--   0        0        0      379 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/folder_hover.svg
+-rw-r--r--   0        0        0     4286 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm.ico
+-rw-r--r--   0        0        0      566 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm.svg
+-rw-r--r--   0        0        0      598 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm_ICO.svg
+-rw-r--r--   0        0        0      569 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm_hover.svg
+-rw-r--r--   0        0        0      571 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm_icon.svg
+-rw-r--r--   0        0        0      696 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/invert_selection.svg
+-rw-r--r--   0        0        0      693 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/invert_selection_hover.svg
+-rw-r--r--   0        0        0      323 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/migrate.svg
+-rw-r--r--   0        0        0      320 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/migrate_hover.svg
+-rw-r--r--   0        0        0     1455 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh.svg
+-rw-r--r--   0        0        0     1625 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh_all.svg
+-rw-r--r--   0        0        0     1622 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh_all_hover.svg
+-rw-r--r--   0        0        0     1452 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh_hover.svg
+-rw-r--r--   0        0        0      484 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/remove.svg
+-rw-r--r--   0        0        0      390 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/remove_all_items.svg
+-rw-r--r--   0        0        0      387 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/remove_all_items_hover.svg
+-rw-r--r--   0        0        0      502 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/remove_hover.svg
+-rw-r--r--   0        0        0      837 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/repo.svg
+-rw-r--r--   0        0        0      834 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/repo_hover.svg
+-rw-r--r--   0        0        0      224 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/toggle_off.svg
+-rw-r--r--   0        0        0      221 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/toggle_off_hover.svg
+-rw-r--r--   0        0        0      334 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/toggle_on.svg
+-rw-r--r--   0        0        0      331 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/toggle_on_hover.svg
+-rw-r--r--   0        0        0      677 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/warning.svg
+-rw-r--r--   0        0        0      680 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/warning_hover.svg
+-rw-r--r--   0        0        0      868 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/utils.py
+-rw-r--r--   0        0        0      655 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/widgets/actions.py
+-rw-r--r--   0        0        0    22204 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/widgets/add_packages_layout.py
+-rw-r--r--   0        0        0     3574 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/widgets/custom_widgets.py
+-rw-r--r--   0        0        0     6818 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/widgets/main_window.py
+-rw-r--r--   0        0        0    21961 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/widgets/packages_layout.py
+-rw-r--r--   0        0        0    12686 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/widgets/packages_table.py
+-rw-r--r--   0        0        0    28338 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/wrangle/config_control.py
+-rw-r--r--   0        0        0     1079 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/wrangle/package_templates.py
+-rw-r--r--   0        0        0     2064 2023-05-11 06:25:51.996742 houdini_package_manager-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 houdini_package_manager-0.2.2/PKG-INFO
```

### Comparing `houdini_package_manager-0.1.0/LICENSE` & `houdini_package_manager-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/README.md` & `houdini_package_manager-0.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 <p align="center">
   <img width="125" src="https://raw.githubusercontent.com/ariffjeff/houdini-package-manager/main/docs/static/hpm.svg">
 </p style = "margin-bottom: 2rem;">
 
----
-
-# houdini-package-manager
+# Houdini Package Manager
 
 [![Release](https://img.shields.io/github/v/release/ariffjeff/houdini-package-manager)](https://img.shields.io/github/v/release/ariffjeff/houdini-package-manager)
 [![Build status](https://img.shields.io/github/actions/workflow/status/ariffjeff/houdini-package-manager/main.yml?branch=main)](https://github.com/ariffjeff/houdini-package-manager/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/ariffjeff/houdini-package-manager/branch/main/graph/badge.svg)](https://codecov.io/gh/ariffjeff/houdini-package-manager)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/ariffjeff/houdini-package-manager)](https://img.shields.io/github/commit-activity/m/ariffjeff/houdini-package-manager)
 [![License](https://img.shields.io/github/license/ariffjeff/houdini-package-manager)](https://img.shields.io/github/license/ariffjeff/houdini-package-manager)
 
-GUI package manager for Houdini
+A comprehensive GUI package manager for Houdini. Manage all your plugins and create new packages with ease.
 
 - **Github repository**: <https://github.com/ariffjeff/houdini-package-manager/>
-- **Documentation** <https://ariffjeff.github.io/houdini-package-manager/>
-
-## Usage
-
-
-
----
-
-Repository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).
+- **PyPI repository**: <https://pypi.org/project/houdini-package-manager/>
```

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/design/icons/add_packages.svg` & `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/design/icons/add_packages_hover.svg` & `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/design/icons/clear_selection.svg` & `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/clear_selection.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/design/icons/clear_selection_hover.svg` & `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/clear_selection_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/design/icons/invert_selection.svg` & `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/invert_selection.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/design/icons/invert_selection_hover.svg` & `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/invert_selection_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/design/icons/refresh.svg` & `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/design/icons/refresh_all.svg` & `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh_all.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/design/icons/refresh_all_hover.svg` & `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh_all_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/design/icons/refresh_hover.svg` & `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/design/icons/warning.svg` & `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/design/icons/warning_hover.svg` & `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/warning_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/main.py` & `houdini_package_manager-0.2.2/houdini_package_manager/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # for processing cli args
 import sys
 
-from PySide6.QtGui import QIcon
 from PySide6.QtWidgets import QApplication
 
 from houdini_package_manager.widgets.main_window import MainWindow
 
 
 def main(start: bool = True, headless: bool = False) -> QApplication:
     """Start the Houdini package manager app
@@ -16,22 +15,17 @@
         start (bool): Start the app. Default is True.
             If False, the app won't start but the QApplication object will still be created.
         headless (bool): The app window will not show when the app starts if True. Default is False.
 
     Returns:
         QApplication: PySide6.QtWidgets object
     """
-    app = QApplication(sys.argv)
 
-    TITLE = "Houdini Package Manager"
+    app = QApplication(sys.argv)
     window = MainWindow(app)
-    window.setWindowTitle(TITLE)
-
-    logo = QIcon("./houdini_package_manager/design/icons/hpm.svg")
-    window.setWindowIcon(logo)
 
     if not headless:
         window.show()
 
     if start:
         app.exec()
```

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/meta/meta_tools.py` & `houdini_package_manager-0.2.2/houdini_package_manager/meta/meta_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,48 @@
+from enum import Enum
+
 from PySide6.QtWidgets import QApplication, QMainWindow, QStatusBar
 
 
+class TextColor(Enum):
+    """
+    Text colors determined by CSS style text color.
+    """
+
+    DEFAULT = "color: white;"
+    ERROR = "color: red;"
+    SUCCESS = "color: green;"
+    WARNING = "color: yellow;"
+
+
 class StatusBar:
     """
     The status bar of the application.
     This is a wrapper around QStatusBar.
     """
 
     @classmethod
-    def message(cls, message: str) -> None:
+    def message(cls, message: str, text_color: TextColor = None) -> None:
         """
         Print a message to the main window's status bar.
 
-        Arguments (str):
-            The string to print to the status bar.
+        Arguments:
+            message (str):
+                The string to print to the status bar.
+
+            text_color (TextColor):
+                The text color enum that sets the color the status bar message text.
+                Default is white.
         """
 
+        if not text_color:
+            text_color = TextColor.DEFAULT
+
         status_bar = cls.status_bar()
-        status_bar.setStyleSheet(
-            """
-            font-family: Lato;
-            font-weight: 100;
-            font-size: 12px;
-            """
-        )
+        status_bar.setStyleSheet(text_color.value)
         status_bar.showMessage(message)
 
     @staticmethod
     def status_bar(raise_on_error=True) -> QStatusBar:
         """
         Return the status bar object.
         Raises an error or returns False if the status bar cannot be found depending on what
```

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/widgets/actions.py` & `houdini_package_manager-0.2.2/houdini_package_manager/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/widgets/custom_widgets.py` & `houdini_package_manager-0.2.2/houdini_package_manager/widgets/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/widgets/packages_layout.py` & `houdini_package_manager-0.2.2/houdini_package_manager/widgets/packages_layout.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,21 @@
     QCheckBox,
     QComboBox,
     QDialog,
     QDialogButtonBox,
     QHBoxLayout,
     QLabel,
     QStackedWidget,
+    QTabWidget,
     QVBoxLayout,
     QWidget,
 )
 
-from houdini_package_manager.meta.meta_tools import StatusBar
+from houdini_package_manager.meta.meta_tools import StatusBar, TextColor
+from houdini_package_manager.utils import epath
 from houdini_package_manager.widgets.custom_widgets import SvgPushButton
 from houdini_package_manager.widgets.packages_table import PackageTableModel
 from houdini_package_manager.wrangle.config_control import HoudiniManager, Package
 
 
 class PackagesWidget(QWidget):
     """
@@ -32,35 +34,41 @@
 
         table_data (HoudiniManager):
             The data set to populate the QWidgetTable. Data can consist of multiple sets of packages
             for different installed versions of Houdini.
 
         versions (list[str]):
             The list of ordered version numbers that will determine which set of package data is shown in the table.
+
+        tabs (QTabWidget):
+            The parent QTabWidget. Used for switching tabs based on widget interaction in this QWidget.
     """
 
-    def __init__(self, parent, table_data: HoudiniManager, versions: list[str]) -> None:
+    def __init__(self, parent, table_data: HoudiniManager, versions: list[str], tabs: QTabWidget) -> None:
         super().__init__(parent)
 
+        self.parent_tabs = tabs
         self.table_data = table_data
         self.versions = versions
         self.version_labels = ["Houdini " + version for version in self.versions]
         self._table_version = self.versions[0]
 
         # LABEL - HOUDINI VERSION DROPDOWN
         label_version_dropdown = QLabel("HOUDINI VERSIONS")
+        label_version_dropdown.setStyleSheet("QLabel { color: #ff6600 }")
 
         # BUTTON - ADD PACKAGE
         button_add_package = SvgPushButton(
             self,
             120,
             36,
-            "./houdini_package_manager/design/icons/add_packages.svg",
-            "./houdini_package_manager/design/icons/add_packages_hover.svg",
+            epath("resources/icons/add_packages.svg"),
+            epath("resources/icons/add_packages_hover.svg"),
         )
+        button_add_package.clicked.connect(self.add_packages)
 
         # DROPDOWN - HOUDINI VERSION
         self.combo_version = QComboBox()
         self.combo_version.addItems(self.version_labels)
         self.combo_version.activated.connect(self.switch_package_table)
         self.combo_version.setMinimumHeight(29)
         self.combo_version.setMinimumWidth(155)
@@ -80,53 +88,53 @@
         )
 
         # BUTTON - HOUDINI VERSION FOLDER
         self.button_version = SvgPushButton(
             self,
             38,
             24,
-            "./houdini_package_manager/design/icons/folder.svg",
-            "./houdini_package_manager/design/icons/folder_hover.svg",
+            epath("resources/icons/folder.svg"),
+            epath("resources/icons/folder_hover.svg"),
         )
         path = self.current_packages_directory()
         self.button_version.set_hover_status_message(f"Open: {path}")
         self.button_version.setToolTip("Open packages folder")
         self.button_version.setProperty("path", path)
         self.button_version.clicked.connect(self.open_path)
 
         # BUTTONS - PACKAGE OPTIONS
         # copy all the packages in the current table to another houdini version
         self.button_copy = SvgPushButton(
             self,
             28,
             28,
-            "./houdini_package_manager/design/icons/migrate.svg",
-            "./houdini_package_manager/design/icons/migrate_hover.svg",
+            epath("resources/icons/migrate.svg"),
+            epath("resources/icons/migrate_hover.svg"),
         )
         self.button_copy.set_hover_status_message("Copy selected packages to other installed Houdini versions.")
         self.button_copy.setToolTip("Copy selected packages to other installed Houdini versions")
         self.button_copy.clicked.connect(self.migrate_packages)
 
         self.button_refresh = SvgPushButton(
             self,
             28,
             28,
-            "./houdini_package_manager/design/icons/refresh.svg",
-            "./houdini_package_manager/design/icons/refresh_hover.svg",
+            epath("resources/icons/refresh.svg"),
+            epath("resources/icons/refresh_hover.svg"),
         )
         self.button_refresh.set_hover_status_message(f"Refresh Houdini {self.table_version} packages.")
         self.button_refresh.setToolTip("Refresh packages for current table")
         self.button_refresh.clicked.connect(self.refresh_table)
 
         self.button_refresh_all = SvgPushButton(
             self,
             28,
             28,
-            "./houdini_package_manager/design/icons/refresh_all.svg",
-            "./houdini_package_manager/design/icons/refresh_all_hover.svg",
+            epath("resources/icons/refresh_all.svg"),
+            epath("resources/icons/refresh_all_hover.svg"),
         )
         self.button_refresh_all.set_hover_status_message("Refresh all packages for all installed versions of Houdini.")
         self.button_refresh_all.setToolTip("Refresh all packages for all installed versions of Houdini")
         self.button_refresh_all.clicked.connect(self.refresh_all_tables)
 
         # TABLE - PACKAGE DATA
         current_hou_version = self.table_data.hou_installs[self.versions[0]]
@@ -170,14 +178,30 @@
         layout_table_options.setAlignment(layout_package_buttons, Qt.AlignRight)
 
     @property
     def table_version(self):
         self._table_version = self.combo_version.currentText().split(" ")[-1]
         return self._table_version
 
+    def add_packages(self) -> None:
+        """
+        Switch to the tab for creating packages from local plugins.
+        Choosing the tab index to switch to is determined by a tab's
+        matching "id" property.
+        """
+
+        target_id = "local_plugin_adder"
+        tab_widget_id = []
+        for i in range(self.parent_tabs.count()):
+            tab_widget_id.append(self.parent_tabs.widget(i).property("id"))
+
+        target_index = tab_widget_id.index(target_id)
+
+        self.parent_tabs.setCurrentIndex(target_index)
+
     def open_path(self) -> None:
         """
         Get the path that is associated with a button and open it.
         """
 
         button = self.sender()
         path = button.property("path")
@@ -307,26 +331,38 @@
 
     def migrate_packages(self) -> None:
         """
         Make copies of all the packages in the currently displayed table and put them
         in the target packages directory of the target installed versions of Houdini.
         """
 
+        if len(self.versions) <= 1:
+            StatusBar.message("No other Houdini versions to copy packages to.", TextColor.ERROR)
+            return
+
         checkbox_version_options = list(self.versions)
         checkbox_version_options.remove(self.table_version)
         checkbox_version_options = [f"Houdini {version}" for version in checkbox_version_options]
 
         # identify any potential file overwrite conflicts for different houdini versions
         current_package_paths = [package.config_path for package in self.current_packages()]
         if not current_package_paths:
             StatusBar.message(f"No packages in Houdini {self.current_table_version()} to copy.")
             return
 
         file_conflicts = self.find_file_conflicts()
         dialog = CheckboxDialog(checkbox_version_options, len(current_package_paths), file_conflicts)
+        dialog.setStyleSheet(
+            """
+            * {
+                background-color: #303030;
+                color: white;
+            }
+        """
+        )
         result = dialog.exec()
         if result == 0:
             return
 
         target_versions = dialog.enabled_checkboxes()
         target_versions = [version.split(" ")[-1] for version in target_versions]
         target_packages_dirs = [
```

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/widgets/packages_table.py` & `houdini_package_manager-0.2.2/houdini_package_manager/widgets/packages_table.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     QSizePolicy,
     QStyledItemDelegate,
     QTableWidget,
     QWidget,
 )
 
 from houdini_package_manager.meta.meta_tools import StatusBar
+from houdini_package_manager.utils import epath
 from houdini_package_manager.widgets.custom_widgets import SvgPushButton
 from houdini_package_manager.wrangle.config_control import HoudiniInstall, Package
 
 
 class PackageTableModel(QTableWidget):
     """
     The table widget that displays Houdini package configuration data and various buttons/options to navigate and manipulate them.
@@ -56,15 +57,15 @@
         self.verticalHeader().setVisible(False)
 
         self.setRowCount(len(self.table_data))
         self.setColumnCount(len(self.labels))
 
         self.setHorizontalHeaderLabels(self.labels)
         self.resizeColumnsToContents()  # before manual width adjustments
-        self.setColumnWidth(self.labels.index("Name"), 180)
+        self.setColumnWidth(self.labels.index("Package"), 180)
         self.setColumnWidth(self.labels.index("Plugins"), 200)
         # self.setColumnWidth(0, 26)  # doesnt seem to work with small numbers
 
         style = """
             ::section {
                 background-color: #3d3d3d;
                 border: none;
@@ -203,16 +204,16 @@
         # A label replaces the dropdown if there is no plugin data.
 
         # if the package config has problems
         button_warning = SvgPushButton(
             parent,
             32,
             29,
-            "./houdini_package_manager/design/icons/warning.svg",
-            "./houdini_package_manager/design/icons/warning_hover.svg",
+            epath("resources/icons/warning.svg"),
+            epath("resources/icons/warning_hover.svg"),
         )
 
         pkg_name = parent._current_package(row).name
         if pkg_name[-5:] != ".json":
             pkg_name += ".json"
         button_warning.set_hover_status_message(f"Can't process package, error(s) in config: {pkg_name}")
         button_warning.setToolTip(warnings)
@@ -291,16 +292,16 @@
     @staticmethod
     def button_config(parent: PackageTableModel, value) -> SvgPushButton:
         # Config: push button that opens its file path when clicked
         config_button = SvgPushButton(
             parent,
             23,
             29,
-            "./houdini_package_manager/design/icons/file.svg",
-            "./houdini_package_manager/design/icons/file_hover.svg",
+            epath("resources/icons/file.svg"),
+            epath("resources/icons/file_hover.svg"),
         )
         config_button.setToolTip(str(value))
         config_button.setProperty("path", value)
         config_button.clicked.connect(parent.open_path)
         config_button.set_hover_status_message(f"Open: {value}")
         return config_button
```

### Comparing `houdini_package_manager-0.1.0/houdini_package_manager/wrangle/config_control.py` & `houdini_package_manager-0.2.2/houdini_package_manager/wrangle/config_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import os
 import platform
 import re
 import subprocess
-import winreg
 from itertools import takewhile
 from pathlib import Path
 from typing import Union
 
 
 class HoudiniManager:
     """
@@ -85,14 +84,16 @@
 
     def _win_registry_values(self, key_path: str) -> dict:
         """
         Get the values of a Windows registry key.
         Paths are converted to pathlib.Path objects.
         """
 
+        import winreg
+
         try:
             # Open the registry key
             key = winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, key_path)
 
             # Iterate over all values in the key
             values = {}
             i = 0
@@ -164,15 +165,22 @@
         self.HFS = install_dir
         self.HB = Path(self.HFS, "bin")
         self.version = HouVersion(str(self.HFS))
 
         # get metadata from hconfig
         self.env_vars = self.run_hconfig()
 
-        self.packages = PackageCollection(Path(self.env_vars["HOUDINI_USER_PREF_DIR"], "packages"), self.env_vars)
+        PREF_DIR_KEY = "HOUDINI_USER_PREF_DIR"
+
+        # if hconfig.exe failed to produce the "HOUDINI_USER_PREF_DIR" env var or any env var data
+        # because maybe the houdini install is corrupted somehow, then no package data can be retrieved.
+        if PREF_DIR_KEY not in self.env_vars:
+            self.packages = None
+        else:
+            self.packages = PackageCollection(Path(self.env_vars[PREF_DIR_KEY], "packages"), self.env_vars)
 
     def run_hconfig(self) -> list:
         """
         Execute Houdini's hconfig to generate the environment variables associated with an installed version of Houdini.
 
         Returns a list of the environment variables.
         """
@@ -448,18 +456,20 @@
         return [path[-1] for path in self.config]
 
     @property
     def table_model(self):
         # the order here is how the columns are ordered in the GUI
         return {
             "Enable": self.enable,
-            "Name": self.name,
-            "Version": self.version,
-            "Author": self.author,
-            "Date Installed": self.date_installed,
+            "Package": self.name,
+            # commented out because these values are really only able
+            # to be gotten from a package index service
+            # "Version": self.version,
+            # "Author": self.author,
+            # "Date Installed": self.date_installed,
             "Config": self.config_path,
             "Plugins": self.plugin_paths,
         }
 
     def is_enabled(self) -> bool:
         """
         Returns True or False based on whether or not the package is
```

### Comparing `houdini_package_manager-0.1.0/pyproject.toml` & `houdini_package_manager-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "houdini_package_manager"
-version = "0.1.0"
+version = "0.2.2"
 description = "GUI package manager for Houdini"
 authors = ["Ariff Jeff <fariffjeff@icloud.com>"]
 repository = "https://github.com/ariffjeff/houdini-package-manager"
 documentation = "https://ariffjeff.github.io/houdini-package-manager/"
 readme = "README.md"
 packages = [
   {include = "houdini_package_manager"}
```

### Comparing `houdini_package_manager-0.1.0/PKG-INFO` & `houdini_package_manager-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: houdini-package-manager
-Version: 0.1.0
+Version: 0.2.2
 Summary: GUI package manager for Houdini
 Home-page: https://github.com/ariffjeff/houdini-package-manager
 Author: Ariff Jeff
 Author-email: fariffjeff@icloud.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -16,29 +16,20 @@
 Project-URL: Repository, https://github.com/ariffjeff/houdini-package-manager
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img width="125" src="https://raw.githubusercontent.com/ariffjeff/houdini-package-manager/main/docs/static/hpm.svg">
 </p style = "margin-bottom: 2rem;">
 
----
-
-# houdini-package-manager
+# Houdini Package Manager
 
 [![Release](https://img.shields.io/github/v/release/ariffjeff/houdini-package-manager)](https://img.shields.io/github/v/release/ariffjeff/houdini-package-manager)
 [![Build status](https://img.shields.io/github/actions/workflow/status/ariffjeff/houdini-package-manager/main.yml?branch=main)](https://github.com/ariffjeff/houdini-package-manager/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/ariffjeff/houdini-package-manager/branch/main/graph/badge.svg)](https://codecov.io/gh/ariffjeff/houdini-package-manager)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/ariffjeff/houdini-package-manager)](https://img.shields.io/github/commit-activity/m/ariffjeff/houdini-package-manager)
 [![License](https://img.shields.io/github/license/ariffjeff/houdini-package-manager)](https://img.shields.io/github/license/ariffjeff/houdini-package-manager)
 
-GUI package manager for Houdini
+A comprehensive GUI package manager for Houdini. Manage all your plugins and create new packages with ease.
 
 - **Github repository**: <https://github.com/ariffjeff/houdini-package-manager/>
-- **Documentation** <https://ariffjeff.github.io/houdini-package-manager/>
-
-## Usage
-
-
-
----
+- **PyPI repository**: <https://pypi.org/project/houdini-package-manager/>
 
-Repository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).
```

