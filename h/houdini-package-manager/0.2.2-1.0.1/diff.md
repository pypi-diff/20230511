# Comparing `tmp/houdini_package_manager-0.2.2.tar.gz` & `tmp/houdini_package_manager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "houdini_package_manager-0.2.2.tar", max compression
+gzip compressed data, was "houdini_package_manager-1.0.1.tar", max compression
```

## Comparing `houdini_package_manager-0.2.2.tar` & `houdini_package_manager-1.0.1.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0    34523 2023-05-11 06:25:16.980147 houdini_package_manager-0.2.2/LICENSE
--rw-r--r--   0        0        0     1361 2023-05-11 06:25:16.980147 houdini_package_manager-0.2.2/README.md
--rw-r--r--   0        0        0       22 2023-05-11 06:25:16.980147 houdini_package_manager-0.2.2/houdini_package_manager/__init__.py
--rw-r--r--   0        0        0      847 2023-05-11 06:25:16.980147 houdini_package_manager-0.2.2/houdini_package_manager/main.py
--rw-r--r--   0        0        0     1975 2023-05-11 06:25:16.980147 houdini_package_manager-0.2.2/houdini_package_manager/meta/meta_tools.py
--rw-r--r--   0        0        0   614544 2023-05-11 06:25:16.988148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Black.ttf
--rw-r--r--   0        0        0   672480 2023-05-11 06:25:16.992148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf
--rw-r--r--   0        0        0   657188 2023-05-11 06:25:16.996148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Bold.ttf
--rw-r--r--   0        0        0   699008 2023-05-11 06:25:17.004148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf
--rw-r--r--   0        0        0   723544 2023-05-11 06:25:17.008148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Italic.ttf
--rw-r--r--   0        0        0   644556 2023-05-11 06:25:17.012148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Light.ttf
--rw-r--r--   0        0        0   658212 2023-05-11 06:25:17.020148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf
--rw-r--r--   0        0        0   637068 2023-05-11 06:25:17.024148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Medium.ttf
--rw-r--r--   0        0        0   695588 2023-05-11 06:25:17.028148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf
--rw-r--r--   0        0        0   657212 2023-05-11 06:25:17.032148 houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Regular.ttf
--rw-r--r--   0        0        0      332 2023-05-11 06:25:17.032148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add.svg
--rw-r--r--   0        0        0      329 2023-05-11 06:25:17.032148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_hover.svg
--rw-r--r--   0        0        0    10421 2023-05-11 06:25:17.032148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages.svg
--rw-r--r--   0        0        0    10472 2023-05-11 06:25:17.032148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages_confirm.svg
--rw-r--r--   0        0        0    10475 2023-05-11 06:25:17.032148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg
--rw-r--r--   0        0        0    10424 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages_hover.svg
--rw-r--r--   0        0        0     1991 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/bug.svg
--rw-r--r--   0        0        0     1988 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/bug_hover.svg
--rw-r--r--   0        0        0      803 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/clear_selection.svg
--rw-r--r--   0        0        0      800 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/clear_selection_hover.svg
--rw-r--r--   0        0        0      427 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/delete.svg
--rw-r--r--   0        0        0      424 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/delete_hover.svg
--rw-r--r--   0        0        0      505 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/docs.svg
--rw-r--r--   0        0        0      502 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/docs_hover.svg
--rw-r--r--   0        0        0      455 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/file.svg
--rw-r--r--   0        0        0      452 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/file_hover.svg
--rw-r--r--   0        0        0      382 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/folder.svg
--rw-r--r--   0        0        0      379 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/folder_hover.svg
--rw-r--r--   0        0        0     4286 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm.ico
--rw-r--r--   0        0        0      566 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm.svg
--rw-r--r--   0        0        0      598 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm_ICO.svg
--rw-r--r--   0        0        0      569 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm_hover.svg
--rw-r--r--   0        0        0      571 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm_icon.svg
--rw-r--r--   0        0        0      696 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/invert_selection.svg
--rw-r--r--   0        0        0      693 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/invert_selection_hover.svg
--rw-r--r--   0        0        0      323 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/migrate.svg
--rw-r--r--   0        0        0      320 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/migrate_hover.svg
--rw-r--r--   0        0        0     1455 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh.svg
--rw-r--r--   0        0        0     1625 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh_all.svg
--rw-r--r--   0        0        0     1622 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh_all_hover.svg
--rw-r--r--   0        0        0     1452 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh_hover.svg
--rw-r--r--   0        0        0      484 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/remove.svg
--rw-r--r--   0        0        0      390 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/remove_all_items.svg
--rw-r--r--   0        0        0      387 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/remove_all_items_hover.svg
--rw-r--r--   0        0        0      502 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/remove_hover.svg
--rw-r--r--   0        0        0      837 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/repo.svg
--rw-r--r--   0        0        0      834 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/repo_hover.svg
--rw-r--r--   0        0        0      224 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/toggle_off.svg
--rw-r--r--   0        0        0      221 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/toggle_off_hover.svg
--rw-r--r--   0        0        0      334 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/toggle_on.svg
--rw-r--r--   0        0        0      331 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/toggle_on_hover.svg
--rw-r--r--   0        0        0      677 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/warning.svg
--rw-r--r--   0        0        0      680 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/warning_hover.svg
--rw-r--r--   0        0        0      868 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/utils.py
--rw-r--r--   0        0        0      655 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/widgets/actions.py
--rw-r--r--   0        0        0    22204 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/widgets/add_packages_layout.py
--rw-r--r--   0        0        0     3574 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/widgets/custom_widgets.py
--rw-r--r--   0        0        0     6818 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/widgets/main_window.py
--rw-r--r--   0        0        0    21961 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/widgets/packages_layout.py
--rw-r--r--   0        0        0    12686 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/widgets/packages_table.py
--rw-r--r--   0        0        0    28338 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/wrangle/config_control.py
--rw-r--r--   0        0        0     1079 2023-05-11 06:25:17.036148 houdini_package_manager-0.2.2/houdini_package_manager/wrangle/package_templates.py
--rw-r--r--   0        0        0     2064 2023-05-11 06:25:51.996742 houdini_package_manager-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 houdini_package_manager-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-11 08:11:33.638517 houdini_package_manager-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2390 2023-05-11 08:11:33.638517 houdini_package_manager-1.0.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-11 08:11:33.642517 houdini_package_manager-1.0.1/houdini_package_manager/__init__.py
+-rw-r--r--   0        0        0     1149 2023-05-11 08:11:33.642517 houdini_package_manager-1.0.1/houdini_package_manager/main.py
+-rw-r--r--   0        0        0     1975 2023-05-11 08:11:33.642517 houdini_package_manager-1.0.1/houdini_package_manager/meta/meta_tools.py
+-rw-r--r--   0        0        0   614544 2023-05-11 08:11:33.646517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Black.ttf
+-rw-r--r--   0        0        0   672480 2023-05-11 08:11:33.650517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf
+-rw-r--r--   0        0        0   657188 2023-05-11 08:11:33.658517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Bold.ttf
+-rw-r--r--   0        0        0   699008 2023-05-11 08:11:33.662517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0        0        0   723544 2023-05-11 08:11:33.666517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Italic.ttf
+-rw-r--r--   0        0        0   644556 2023-05-11 08:11:33.674517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Light.ttf
+-rw-r--r--   0        0        0   658212 2023-05-11 08:11:33.678517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0        0        0   637068 2023-05-11 08:11:33.682517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Medium.ttf
+-rw-r--r--   0        0        0   695588 2023-05-11 08:11:33.686517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf
+-rw-r--r--   0        0        0   657212 2023-05-11 08:11:33.690518 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Regular.ttf
+-rw-r--r--   0        0        0      332 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add.svg
+-rw-r--r--   0        0        0      329 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_hover.svg
+-rw-r--r--   0        0        0    10421 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages.svg
+-rw-r--r--   0        0        0    10472 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages_confirm.svg
+-rw-r--r--   0        0        0    10475 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg
+-rw-r--r--   0        0        0    10424 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages_hover.svg
+-rw-r--r--   0        0        0     1991 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/bug.svg
+-rw-r--r--   0        0        0     1988 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/bug_hover.svg
+-rw-r--r--   0        0        0      803 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/clear_selection.svg
+-rw-r--r--   0        0        0      800 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/clear_selection_hover.svg
+-rw-r--r--   0        0        0      427 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/delete.svg
+-rw-r--r--   0        0        0      424 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/delete_hover.svg
+-rw-r--r--   0        0        0      505 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/docs.svg
+-rw-r--r--   0        0        0      502 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/docs_hover.svg
+-rw-r--r--   0        0        0      455 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/file.svg
+-rw-r--r--   0        0        0      452 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/file_hover.svg
+-rw-r--r--   0        0        0      382 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/folder.svg
+-rw-r--r--   0        0        0      379 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/folder_hover.svg
+-rw-r--r--   0        0        0     4286 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm.ico
+-rw-r--r--   0        0        0      566 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm.svg
+-rw-r--r--   0        0        0      598 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm_ICO.svg
+-rw-r--r--   0        0        0      569 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm_hover.svg
+-rw-r--r--   0        0        0      571 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm_icon.svg
+-rw-r--r--   0        0        0      696 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/invert_selection.svg
+-rw-r--r--   0        0        0      693 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/invert_selection_hover.svg
+-rw-r--r--   0        0        0      323 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/migrate.svg
+-rw-r--r--   0        0        0      320 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/migrate_hover.svg
+-rw-r--r--   0        0        0     1455 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh.svg
+-rw-r--r--   0        0        0     1625 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh_all.svg
+-rw-r--r--   0        0        0     1622 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh_all_hover.svg
+-rw-r--r--   0        0        0     1452 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh_hover.svg
+-rw-r--r--   0        0        0      484 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/remove.svg
+-rw-r--r--   0        0        0      390 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/remove_all_items.svg
+-rw-r--r--   0        0        0      387 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/remove_all_items_hover.svg
+-rw-r--r--   0        0        0      502 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/remove_hover.svg
+-rw-r--r--   0        0        0      837 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/repo.svg
+-rw-r--r--   0        0        0      834 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/repo_hover.svg
+-rw-r--r--   0        0        0      224 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/toggle_off.svg
+-rw-r--r--   0        0        0      221 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/toggle_off_hover.svg
+-rw-r--r--   0        0        0      334 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/toggle_on.svg
+-rw-r--r--   0        0        0      331 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/toggle_on_hover.svg
+-rw-r--r--   0        0        0      677 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/warning.svg
+-rw-r--r--   0        0        0      680 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/warning_hover.svg
+-rw-r--r--   0        0        0     2936 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/update.py
+-rw-r--r--   0        0        0      868 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/utils.py
+-rw-r--r--   0        0        0      655 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/widgets/actions.py
+-rw-r--r--   0        0        0    22204 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/widgets/add_packages_layout.py
+-rw-r--r--   0        0        0     3574 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/widgets/custom_widgets.py
+-rw-r--r--   0        0        0     6818 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/widgets/main_window.py
+-rw-r--r--   0        0        0    21961 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/widgets/packages_layout.py
+-rw-r--r--   0        0        0    12686 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/widgets/packages_table.py
+-rw-r--r--   0        0        0    28338 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/wrangle/config_control.py
+-rw-r--r--   0        0        0     1079 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/wrangle/package_templates.py
+-rw-r--r--   0        0        0     2105 2023-05-11 08:12:35.123022 houdini_package_manager-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 houdini_package_manager-1.0.1/PKG-INFO
```

### Comparing `houdini_package_manager-0.2.2/LICENSE` & `houdini_package_manager-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/main.py` & `houdini_package_manager-1.0.1/houdini_package_manager/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # for processing cli args
 import sys
 
+from PySide6.QtCore import QTimer
 from PySide6.QtWidgets import QApplication
 
+from houdini_package_manager.update import Updater
 from houdini_package_manager.widgets.main_window import MainWindow
 
 
 def main(start: bool = True, headless: bool = False) -> QApplication:
     """Start the Houdini package manager app
 
     Create and open the Houdini package manager window
@@ -19,18 +21,30 @@
     Returns:
         QApplication: PySide6.QtWidgets object
     """
 
     app = QApplication(sys.argv)
     window = MainWindow(app)
 
+    # delay updater dialog until main window shows
+    QTimer.singleShot(0, show_updater)
+
     if not headless:
         window.show()
 
     if start:
         app.exec()
 
     return app
 
 
+def show_updater():
+    """
+    Show the version update dialog.
+    """
+
+    updater = Updater()
+    updater.check_update()
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/meta/meta_tools.py` & `houdini_package_manager-1.0.1/houdini_package_manager/meta/meta_tools.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Black.ttf` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Bold.ttf` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Italic.ttf` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Light.ttf` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Medium.ttf` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Medium.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/fonts/Lato-Regular.ttf` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages_confirm.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages_confirm.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/add_packages_hover.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/bug.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/bug.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/bug_hover.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/bug_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/clear_selection.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/clear_selection.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/clear_selection_hover.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/clear_selection_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm.ico` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm.ico`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm_ICO.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm_ICO.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm_hover.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/hpm_icon.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm_icon.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/invert_selection.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/invert_selection.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/invert_selection_hover.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/invert_selection_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh_all.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh_all.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh_all_hover.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh_all_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/refresh_hover.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/repo.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/repo.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/repo_hover.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/repo_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/warning.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/resources/icons/warning_hover.svg` & `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/warning_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/utils.py` & `houdini_package_manager-1.0.1/houdini_package_manager/utils.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/widgets/actions.py` & `houdini_package_manager-1.0.1/houdini_package_manager/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/widgets/add_packages_layout.py` & `houdini_package_manager-1.0.1/houdini_package_manager/widgets/add_packages_layout.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/widgets/custom_widgets.py` & `houdini_package_manager-1.0.1/houdini_package_manager/widgets/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/widgets/main_window.py` & `houdini_package_manager-1.0.1/houdini_package_manager/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/widgets/packages_layout.py` & `houdini_package_manager-1.0.1/houdini_package_manager/widgets/packages_layout.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/widgets/packages_table.py` & `houdini_package_manager-1.0.1/houdini_package_manager/widgets/packages_table.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/wrangle/config_control.py` & `houdini_package_manager-1.0.1/houdini_package_manager/wrangle/config_control.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/houdini_package_manager/wrangle/package_templates.py` & `houdini_package_manager-1.0.1/houdini_package_manager/wrangle/package_templates.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-0.2.2/pyproject.toml` & `houdini_package_manager-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "houdini_package_manager"
-version = "0.2.2"
+version = "1.0.1"
 description = "GUI package manager for Houdini"
 authors = ["Ariff Jeff <fariffjeff@icloud.com>"]
 repository = "https://github.com/ariffjeff/houdini-package-manager"
 documentation = "https://ariffjeff.github.io/houdini-package-manager/"
 readme = "README.md"
 packages = [
   {include = "houdini_package_manager"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 pyside6 = "^6.4.2"
+packaging = "^23.1"
+requests = "^2.30.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.6.4"
 mypy = "^0.981"
 pre-commit = "^2.20.0"
```

