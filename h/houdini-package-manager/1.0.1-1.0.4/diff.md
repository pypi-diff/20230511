# Comparing `tmp/houdini_package_manager-1.0.1.tar.gz` & `tmp/houdini_package_manager-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "houdini_package_manager-1.0.1.tar", max compression
+gzip compressed data, was "houdini_package_manager-1.0.4.tar", max compression
```

## Comparing `houdini_package_manager-1.0.1.tar` & `houdini_package_manager-1.0.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0    34523 2023-05-11 08:11:33.638517 houdini_package_manager-1.0.1/LICENSE
--rw-r--r--   0        0        0     2390 2023-05-11 08:11:33.638517 houdini_package_manager-1.0.1/README.md
--rw-r--r--   0        0        0       22 2023-05-11 08:11:33.642517 houdini_package_manager-1.0.1/houdini_package_manager/__init__.py
--rw-r--r--   0        0        0     1149 2023-05-11 08:11:33.642517 houdini_package_manager-1.0.1/houdini_package_manager/main.py
--rw-r--r--   0        0        0     1975 2023-05-11 08:11:33.642517 houdini_package_manager-1.0.1/houdini_package_manager/meta/meta_tools.py
--rw-r--r--   0        0        0   614544 2023-05-11 08:11:33.646517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Black.ttf
--rw-r--r--   0        0        0   672480 2023-05-11 08:11:33.650517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf
--rw-r--r--   0        0        0   657188 2023-05-11 08:11:33.658517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Bold.ttf
--rw-r--r--   0        0        0   699008 2023-05-11 08:11:33.662517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf
--rw-r--r--   0        0        0   723544 2023-05-11 08:11:33.666517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Italic.ttf
--rw-r--r--   0        0        0   644556 2023-05-11 08:11:33.674517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Light.ttf
--rw-r--r--   0        0        0   658212 2023-05-11 08:11:33.678517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf
--rw-r--r--   0        0        0   637068 2023-05-11 08:11:33.682517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Medium.ttf
--rw-r--r--   0        0        0   695588 2023-05-11 08:11:33.686517 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf
--rw-r--r--   0        0        0   657212 2023-05-11 08:11:33.690518 houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Regular.ttf
--rw-r--r--   0        0        0      332 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add.svg
--rw-r--r--   0        0        0      329 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_hover.svg
--rw-r--r--   0        0        0    10421 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages.svg
--rw-r--r--   0        0        0    10472 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages_confirm.svg
--rw-r--r--   0        0        0    10475 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg
--rw-r--r--   0        0        0    10424 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages_hover.svg
--rw-r--r--   0        0        0     1991 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/bug.svg
--rw-r--r--   0        0        0     1988 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/bug_hover.svg
--rw-r--r--   0        0        0      803 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/clear_selection.svg
--rw-r--r--   0        0        0      800 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/clear_selection_hover.svg
--rw-r--r--   0        0        0      427 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/delete.svg
--rw-r--r--   0        0        0      424 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/delete_hover.svg
--rw-r--r--   0        0        0      505 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/docs.svg
--rw-r--r--   0        0        0      502 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/docs_hover.svg
--rw-r--r--   0        0        0      455 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/file.svg
--rw-r--r--   0        0        0      452 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/file_hover.svg
--rw-r--r--   0        0        0      382 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/folder.svg
--rw-r--r--   0        0        0      379 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/folder_hover.svg
--rw-r--r--   0        0        0     4286 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm.ico
--rw-r--r--   0        0        0      566 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm.svg
--rw-r--r--   0        0        0      598 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm_ICO.svg
--rw-r--r--   0        0        0      569 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm_hover.svg
--rw-r--r--   0        0        0      571 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm_icon.svg
--rw-r--r--   0        0        0      696 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/invert_selection.svg
--rw-r--r--   0        0        0      693 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/invert_selection_hover.svg
--rw-r--r--   0        0        0      323 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/migrate.svg
--rw-r--r--   0        0        0      320 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/migrate_hover.svg
--rw-r--r--   0        0        0     1455 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh.svg
--rw-r--r--   0        0        0     1625 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh_all.svg
--rw-r--r--   0        0        0     1622 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh_all_hover.svg
--rw-r--r--   0        0        0     1452 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh_hover.svg
--rw-r--r--   0        0        0      484 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/remove.svg
--rw-r--r--   0        0        0      390 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/remove_all_items.svg
--rw-r--r--   0        0        0      387 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/remove_all_items_hover.svg
--rw-r--r--   0        0        0      502 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/remove_hover.svg
--rw-r--r--   0        0        0      837 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/repo.svg
--rw-r--r--   0        0        0      834 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/repo_hover.svg
--rw-r--r--   0        0        0      224 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/toggle_off.svg
--rw-r--r--   0        0        0      221 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/toggle_off_hover.svg
--rw-r--r--   0        0        0      334 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/toggle_on.svg
--rw-r--r--   0        0        0      331 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/toggle_on_hover.svg
--rw-r--r--   0        0        0      677 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/warning.svg
--rw-r--r--   0        0        0      680 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/warning_hover.svg
--rw-r--r--   0        0        0     2936 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/update.py
--rw-r--r--   0        0        0      868 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/utils.py
--rw-r--r--   0        0        0      655 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/widgets/actions.py
--rw-r--r--   0        0        0    22204 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/widgets/add_packages_layout.py
--rw-r--r--   0        0        0     3574 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/widgets/custom_widgets.py
--rw-r--r--   0        0        0     6818 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/widgets/main_window.py
--rw-r--r--   0        0        0    21961 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/widgets/packages_layout.py
--rw-r--r--   0        0        0    12686 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/widgets/packages_table.py
--rw-r--r--   0        0        0    28338 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/wrangle/config_control.py
--rw-r--r--   0        0        0     1079 2023-05-11 08:11:33.694517 houdini_package_manager-1.0.1/houdini_package_manager/wrangle/package_templates.py
--rw-r--r--   0        0        0     2105 2023-05-11 08:12:35.123022 houdini_package_manager-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 houdini_package_manager-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-11 17:01:17.261520 houdini_package_manager-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2390 2023-05-11 17:01:17.261520 houdini_package_manager-1.0.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-11 17:01:17.265520 houdini_package_manager-1.0.4/houdini_package_manager/__init__.py
+-rw-r--r--   0        0        0     1149 2023-05-11 17:01:17.265520 houdini_package_manager-1.0.4/houdini_package_manager/main.py
+-rw-r--r--   0        0        0     1975 2023-05-11 17:01:17.265520 houdini_package_manager-1.0.4/houdini_package_manager/meta/meta_tools.py
+-rw-r--r--   0        0        0   614544 2023-05-11 17:01:17.269520 houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-Black.ttf
+-rw-r--r--   0        0        0   672480 2023-05-11 17:01:17.273520 houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf
+-rw-r--r--   0        0        0   657188 2023-05-11 17:01:17.281520 houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-Bold.ttf
+-rw-r--r--   0        0        0   699008 2023-05-11 17:01:17.285520 houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0        0        0   723544 2023-05-11 17:01:17.289520 houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-Italic.ttf
+-rw-r--r--   0        0        0   644556 2023-05-11 17:01:17.297520 houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-Light.ttf
+-rw-r--r--   0        0        0   658212 2023-05-11 17:01:17.301520 houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0        0        0   637068 2023-05-11 17:01:17.305520 houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-Medium.ttf
+-rw-r--r--   0        0        0   695588 2023-05-11 17:01:17.313520 houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf
+-rw-r--r--   0        0        0   657212 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-Regular.ttf
+-rw-r--r--   0        0        0      332 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/add.svg
+-rw-r--r--   0        0        0      329 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/add_hover.svg
+-rw-r--r--   0        0        0    10421 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/add_packages.svg
+-rw-r--r--   0        0        0    10472 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/add_packages_confirm.svg
+-rw-r--r--   0        0        0    10475 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg
+-rw-r--r--   0        0        0    10424 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/add_packages_hover.svg
+-rw-r--r--   0        0        0     1991 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/bug.svg
+-rw-r--r--   0        0        0     1988 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/bug_hover.svg
+-rw-r--r--   0        0        0      803 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/clear_selection.svg
+-rw-r--r--   0        0        0      800 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/clear_selection_hover.svg
+-rw-r--r--   0        0        0      427 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/delete.svg
+-rw-r--r--   0        0        0      424 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/delete_hover.svg
+-rw-r--r--   0        0        0      505 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/docs.svg
+-rw-r--r--   0        0        0      502 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/docs_hover.svg
+-rw-r--r--   0        0        0      455 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/file.svg
+-rw-r--r--   0        0        0      452 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/file_hover.svg
+-rw-r--r--   0        0        0      382 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/folder.svg
+-rw-r--r--   0        0        0      379 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/folder_hover.svg
+-rw-r--r--   0        0        0     4286 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/hpm.ico
+-rw-r--r--   0        0        0      566 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/hpm.svg
+-rw-r--r--   0        0        0      598 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/hpm_ICO.svg
+-rw-r--r--   0        0        0      569 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/hpm_hover.svg
+-rw-r--r--   0        0        0      571 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/hpm_icon.svg
+-rw-r--r--   0        0        0      696 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/invert_selection.svg
+-rw-r--r--   0        0        0      693 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/invert_selection_hover.svg
+-rw-r--r--   0        0        0      323 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/migrate.svg
+-rw-r--r--   0        0        0      320 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/migrate_hover.svg
+-rw-r--r--   0        0        0     1455 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/refresh.svg
+-rw-r--r--   0        0        0     1625 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/refresh_all.svg
+-rw-r--r--   0        0        0     1622 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/refresh_all_hover.svg
+-rw-r--r--   0        0        0     1452 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/refresh_hover.svg
+-rw-r--r--   0        0        0      484 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/remove.svg
+-rw-r--r--   0        0        0      390 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/remove_all_items.svg
+-rw-r--r--   0        0        0      387 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/remove_all_items_hover.svg
+-rw-r--r--   0        0        0      502 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/remove_hover.svg
+-rw-r--r--   0        0        0      837 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/repo.svg
+-rw-r--r--   0        0        0      834 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/repo_hover.svg
+-rw-r--r--   0        0        0      224 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/toggle_off.svg
+-rw-r--r--   0        0        0      221 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/toggle_off_hover.svg
+-rw-r--r--   0        0        0      334 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/toggle_on.svg
+-rw-r--r--   0        0        0      331 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/toggle_on_hover.svg
+-rw-r--r--   0        0        0      677 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/warning.svg
+-rw-r--r--   0        0        0      680 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/warning_hover.svg
+-rw-r--r--   0        0        0     2936 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/update.py
+-rw-r--r--   0        0        0      868 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/utils.py
+-rw-r--r--   0        0        0      655 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/widgets/actions.py
+-rw-r--r--   0        0        0    22228 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/widgets/add_packages_layout.py
+-rw-r--r--   0        0        0     3574 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/widgets/custom_widgets.py
+-rw-r--r--   0        0        0     6818 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/widgets/main_window.py
+-rw-r--r--   0        0        0    21983 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/widgets/packages_layout.py
+-rw-r--r--   0        0        0    12686 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/widgets/packages_table.py
+-rw-r--r--   0        0        0    28576 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/wrangle/config_control.py
+-rw-r--r--   0        0        0     1079 2023-05-11 17:01:17.317520 houdini_package_manager-1.0.4/houdini_package_manager/wrangle/package_templates.py
+-rw-r--r--   0        0        0     2105 2023-05-11 17:01:50.533761 houdini_package_manager-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 houdini_package_manager-1.0.4/PKG-INFO
```

### Comparing `houdini_package_manager-1.0.1/LICENSE` & `houdini_package_manager-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/README.md` & `houdini_package_manager-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/main.py` & `houdini_package_manager-1.0.4/houdini_package_manager/main.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/meta/meta_tools.py` & `houdini_package_manager-1.0.4/houdini_package_manager/meta/meta_tools.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Black.ttf` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Bold.ttf` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Italic.ttf` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Light.ttf` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Medium.ttf` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-Medium.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/fonts/Lato-Regular.ttf` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/add_packages.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages_confirm.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/add_packages_confirm.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/add_packages_hover.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/add_packages_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/bug.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/bug.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/bug_hover.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/bug_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/clear_selection.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/clear_selection.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/clear_selection_hover.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/clear_selection_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm.ico` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/hpm.ico`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/hpm.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm_ICO.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/hpm_ICO.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm_hover.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/hpm_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/hpm_icon.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/hpm_icon.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/invert_selection.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/invert_selection.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/invert_selection_hover.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/invert_selection_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/refresh.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh_all.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/refresh_all.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh_all_hover.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/refresh_all_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/refresh_hover.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/refresh_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/repo.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/repo.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/repo_hover.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/repo_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/warning.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/resources/icons/warning_hover.svg` & `houdini_package_manager-1.0.4/houdini_package_manager/resources/icons/warning_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/update.py` & `houdini_package_manager-1.0.4/houdini_package_manager/update.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/utils.py` & `houdini_package_manager-1.0.4/houdini_package_manager/utils.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/widgets/actions.py` & `houdini_package_manager-1.0.4/houdini_package_manager/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/widgets/add_packages_layout.py` & `houdini_package_manager-1.0.4/houdini_package_manager/widgets/add_packages_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from pathlib import Path
+from typing import List
 
 from PySide6.QtCore import QSize, Qt
 from PySide6.QtWidgets import (
     QAbstractItemView,
     QCheckBox,
     QDialog,
     QFileDialog,
@@ -35,19 +36,19 @@
         parent:
             The parent widget.
 
         table_data (HoudiniManager):
             The data set to populate the QWidgetTable. Data can consist of multiple sets of packages
             for different installed versions of Houdini.
 
-        versions (list[str]):
+        versions (List[str]):
             The list of ordered version numbers that will determine which set of package data is shown in the table.
     """
 
-    def __init__(self, parent, table_data: HoudiniManager, versions: list[str]) -> None:
+    def __init__(self, parent, table_data: HoudiniManager, versions: List[str]) -> None:
         super().__init__(parent)
 
         self.table_data = table_data
         self.versions = versions
         self.tool_widgets = PresetWidgets()
 
         # LIST - HOUDINI VERSIONS
@@ -181,28 +182,28 @@
 
         if existing_paths == 0:
             self.label_file_overwrite.setText("")
             return
 
         self.label_file_overwrite.setText(f"{existing_paths} existing config files will be overwritten.")
 
-    def _selected_versions(self) -> list[str]:
+    def _selected_versions(self) -> List[str]:
         """
         Return a list of the selected houdini version numbers from the version list.
         """
 
         widgets = []
         for i in range(self.layout_v_hou_versions.count()):
             widgets.append(self.layout_v_hou_versions.itemAt(i).widget())
 
         widgets = [widget.property("version") for widget in widgets if widget.isChecked()]
 
         return widgets
 
-    def _create_config_data(self, plugin_paths: list[Path]) -> dict:
+    def _create_config_data(self, plugin_paths: List[Path]) -> dict:
         """
         Create the structured config data from a package template for each plugin path.
         """
 
         new_packages = {}
         for path in plugin_paths:
             new_packages[path.name] = PackageTemplates.standard(path)
```

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/widgets/custom_widgets.py` & `houdini_package_manager-1.0.4/houdini_package_manager/widgets/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/widgets/main_window.py` & `houdini_package_manager-1.0.4/houdini_package_manager/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/widgets/packages_layout.py` & `houdini_package_manager-1.0.4/houdini_package_manager/widgets/packages_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import shutil
 from pathlib import Path
-from typing import Union
+from typing import Dict, List, Union
 
 from PySide6.QtCore import Qt, QUrl
 from PySide6.QtGui import QDesktopServices
 from PySide6.QtWidgets import (
     QCheckBox,
     QComboBox,
     QDialog,
@@ -32,22 +32,22 @@
         parent:
             The parent widget.
 
         table_data (HoudiniManager):
             The data set to populate the QWidgetTable. Data can consist of multiple sets of packages
             for different installed versions of Houdini.
 
-        versions (list[str]):
+        versions (List[str]):
             The list of ordered version numbers that will determine which set of package data is shown in the table.
 
         tabs (QTabWidget):
             The parent QTabWidget. Used for switching tabs based on widget interaction in this QWidget.
     """
 
-    def __init__(self, parent, table_data: HoudiniManager, versions: list[str], tabs: QTabWidget) -> None:
+    def __init__(self, parent, table_data: HoudiniManager, versions: List[str], tabs: QTabWidget) -> None:
         super().__init__(parent)
 
         self.parent_tabs = tabs
         self.table_data = table_data
         self.versions = versions
         self.version_labels = ["Houdini " + version for version in self.versions]
         self._table_version = self.versions[0]
@@ -379,15 +379,15 @@
             f" {len(target_packages_dirs)} other Houdini installs."
         )
 
         # refresh packages table for target houdini versions
         for version in target_versions:
             self.refresh_table(version, status=False)
 
-    def find_file_conflicts(self) -> dict[list[Path]]:
+    def find_file_conflicts(self) -> Dict[str, List[Path]]:
         """
         Search for file conflicts in other Houdini packages directories by comparing
         all the Package configs in the current houdini version with all the other houdini version Package configs.
         This is useful for if config files from one houdini version need to be moved to another.
 
         Returns a dict of all other houdini versions where each value is a list of package Paths.
         """
@@ -411,15 +411,15 @@
             file_conflicts[version] = []
             for pkg_path in current_package_paths:
                 if pkg_path.name in paths:
                     file_conflicts[version].append(pkg_path)
 
         return file_conflicts
 
-    def current_packages(self) -> list[Package]:
+    def current_packages(self) -> List[Package]:
         """
         Return a list of the Package objects assosciated with the currently loaded table.
         """
 
         current_table = self.stacked_widget.currentWidget()
         if not hasattr(current_table, "packages"):
             return []
@@ -431,22 +431,22 @@
         Return the houdini version number of the current displayed package table.
         """
 
         label = self.combo_version.currentText()
         label = label.split(" ")[-1]
         return label
 
-    def get_packages(self, versions: Union[str, list[str]] = None) -> dict[Package]:
+    def get_packages(self, versions: Union[str, List[str]] = None) -> Dict[str, Package]:
         """
         Return a dict of the package data for the all the tables.
         The key is the Houdini version number.
         The value is the Package object.
 
         Arguments:
-            versions (Union(str, list[str])):
+            versions (Union(str, List[str])):
                 The Houdini versions to get packages from.
                 If no version is provided, the packages for all Houdini versions will be returned.
         """
 
         all_versions = self.table_data.hou_installs
         if not versions:
             return all_versions
@@ -529,15 +529,15 @@
 
         self.label_file_overwrites.setText(f"{self.checked_file_conflicts} files will be overwritten.")
 
     def get_checkbox_data(self):
         # Return a list of tuples containing the checkbox labels and whether they are checked
         return [checkbox.isChecked() for checkbox in self.checkboxes]
 
-    def enabled_checkboxes(self) -> list[str]:
+    def enabled_checkboxes(self) -> List[str]:
         """
         Return a list of the enabled checkbox labels.
         """
 
         selected_checkboxes = []
         for checkbox in self.checkboxes:
             if checkbox.isChecked():
```

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/widgets/packages_table.py` & `houdini_package_manager-1.0.4/houdini_package_manager/widgets/packages_table.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/wrangle/config_control.py` & `houdini_package_manager-1.0.4/houdini_package_manager/wrangle/config_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import json
 import os
 import platform
 import re
 import subprocess
 from itertools import takewhile
 from pathlib import Path
-from typing import Union
+from typing import Dict, List, Union
 
 
 class HoudiniManager:
     """
     A class for managing data related to multiple installed versions of Houdini.
 
     Attributes:
         install_directories (Dict[str, Path]):
             The directories containing the install locations of different Houdini versions.
             The keys are the version numbers. The values are the directories.
 
-        hou_installs (Dict[HoudiniInstall]):
+        hou_installs (Dict[str, HoudiniInstall]):
             A dictionary of all the installed versions of Houdini and their data.
     """
 
     def __init__(self, only_hou_installs=True) -> None:
         self.install_directories = self._get_houdini_paths()
         if only_hou_installs:
             self.install_directories = self.only_houdini_locations()
 
         self.hou_installs = {}
 
-    def get_houdini_data(self, versions: Union[str, list[str]] = None) -> None:
+    def get_houdini_data(self, versions: Union[str, List[str]] = None) -> None:
         """
         Get the package data and relevant meta data for each installed version of Houdini.
         If an install has no package data then the config will simply be empty.
 
         Arguments:
-            version (Union[str, list[str]]):
+            version (Union[str, List[str]]):
                 Get all data for only the given Houdini version(s). If the data already exists
                 for a version then it is replaced by a new set of data.
         """
 
         if isinstance(versions, str):
             versions = [versions]
 
@@ -216,25 +216,25 @@
                 data[name] = pkg.table_model
         else:
             data = []
             for _name, pkg in self.packages.configs.items():
                 data.append(list(pkg.table_model.values()))
         return data
 
-    def get_package_warnings(self) -> list[str]:
+    def get_package_warnings(self) -> List[str]:
         """
         Get the warnings for each package.
         """
 
         data = {}
         for name, pkg in self.packages.configs.items():
             data[name] = pkg.warnings
         return data
 
-    def get_labels(self) -> list[str]:
+    def get_labels(self) -> List[str]:
         for _, pkg in self.packages.configs.items():
             return list(pkg.table_model.keys())
 
 
 class HouVersion:
     """
     Version components of a Houdini version.
@@ -264,15 +264,15 @@
     """
     Package JSON configurations and the associated plugin data the configs point to.
 
     Arguments:
         packages_directory (str):
             The directory containing the JSON packages that Houdini references to find plugins.
 
-        env_vars (dict[str]):
+        env_vars (Dict[str, str]):
             The environment variables needed to help resolve variables found in package configuration
             files. They are aggregated by hconfig
 
         get_data (bool):
             Whether or not to automatically get the package data and its respective plugin data upon
             creation of the Packages object.
             Default is True.
@@ -280,15 +280,15 @@
     Attributes:
         hconfig_plugin_paths (list):
             The paths from HOUDINI_PATH which is from hconfig. These are all
             the plugins paths from all the packages that hconfig found for a single installed
             version of Houdini.
     """
 
-    def __init__(self, packages_directory: Path = None, env_vars: dict[str] = None, get_data=True) -> None:
+    def __init__(self, packages_directory: Path = None, env_vars: Dict[str, str] = None, get_data=True) -> None:
         if packages_directory and not isinstance(packages_directory, Path):
             raise TypeError("directory must be a pathlib.Path object.")
 
         if not env_vars:
             env_vars = {}
         if not isinstance(env_vars, dict):
             raise TypeError("env_vars must be a dict.")
@@ -320,14 +320,18 @@
         """
 
         if not self.packages_directory:
             raise AttributeError(
                 "directory is not set to any path. Make sure env_vars contains data as well if needed."
             )
 
+        if not self.packages_directory.exists():
+            self.packages_directory.mkdir(parents=True)
+            print(f"Created missing packages folder: {self.packages_directory}")
+
         # add the package directory as a needed environment variable
         # which isn't automatically added by hconfig for some reason.
         HOUDINI_PACKAGE_PATH = "HOUDINI_PACKAGE_PATH"
         if HOUDINI_PACKAGE_PATH not in self.env_vars:
             self.env_vars.update({HOUDINI_PACKAGE_PATH: str(self.packages_directory) or ""})
 
         self.hconfig_plugin_paths = self.extract_plugin_paths_from_HOUDINI_PATH(self.env_vars["HOUDINI_PATH"])
@@ -335,15 +339,15 @@
         files = next(os.walk(self.packages_directory))
         files = [name for name in files[2] if ".json" in name]  # only .json files
         for file in files:
             self.configs[Path(file).stem] = Package(
                 Path(self.packages_directory, file), self.hconfig_plugin_paths, self.env_vars
             )
 
-    def extract_plugin_paths_from_HOUDINI_PATH(self, houdini_path: str) -> list[Path]:
+    def extract_plugin_paths_from_HOUDINI_PATH(self, houdini_path: str) -> List[Path]:
         """
         Extract all the paths from the value of the HOUDINI_PATH environment variable.
         The paths are the directories that Houdini will search for the plugin data (HDAs/OTLs).
 
         Returns a list of pathlib.Path paths that exist.
         """
 
@@ -351,30 +355,32 @@
         plugin_paths = [Path(path) for path in plugin_paths]
         plugin_paths = [path for path in plugin_paths if path.exists()]
 
         return plugin_paths
 
 
 class Package:
-    def __init__(self, config_path: Path, hconfig_plugin_paths: list[Path] = None, env_vars: dict[str] = None) -> None:
+    def __init__(
+        self, config_path: Path, hconfig_plugin_paths: List[Path] = None, env_vars: Dict[str, str] = None
+    ) -> None:
         """
         A single JSON package file and its configuration and related data.
 
         If hconfig_plugin_paths is not given, manually determine which plugins the package are pointing to since
         we cannot use all_plugin_paths as a helping guide which was extracted from hconfig.
 
         Arguments:
             config_path (pathlib.Path):
                 The file path of the package .json file.
 
-            hconfig_plugin_paths (list[str]):
+            hconfig_plugin_paths (List[str]):
                 The list of paths extracted from the HOUDINI_PATH environment variable produced by hconfig.
                 These paths are associated with all packages for an installed version of Houdini.
 
-            env_vars (dict[str]):
+            env_vars (Dict[str, str]):
                 The environment variables that apply to all the packages for an
                 installed Houdini version.
         """
 
         if not isinstance(config_path, Path):
             raise TypeError("package_path must be a pathlib.Path object.")
 
@@ -583,39 +589,39 @@
             for i, item in enumerate(data):
                 path = [*prefix, i]
                 flat.extend(self._flatten_package(item, path))
         else:  # str, int, bool
             flat.append([*prefix, data])
         return flat
 
-    def _standard_paths(self, data: list[list]) -> list[list]:
+    def _standard_paths(self, data: List[list]) -> List[list]:
         """
         Replace invalid double backslashes in paths with valid forward slashes.
         This ensures future regex operations do not encounter errors parsing escape characters.
         """
 
         for i, value in enumerate(data):
             value = value[-1]
             if isinstance(value, str) and ("/" in value or "\\" in value):
                 value = value.replace("\\", "/")
                 data[i][-1] = value
         return data
 
-    def _split_indexes(self, nums: list[int], split_num: int) -> list[list[int]]:
+    def _split_indexes(self, nums: List[int], split_num: int) -> List[List[int]]:
         index = len(nums)
         for i, num in enumerate(nums):
             if num > split_num:
                 index = i
                 break
 
         start = nums[:index]
         end = nums[index:]
         return [start, end]
 
-    def _replace_var_calls(self, data: list[list], var_calls: list, potential_var_names: list) -> list[list]:
+    def _replace_var_calls(self, data: List[list], var_calls: list, potential_var_names: list) -> List[list]:
         """
         Continuously replace variable calls with their respective values until no variable calls remain.
         Only replaces var calls if the variable exists to replace it with.
         Catches circular referencing variable calls.
         """
 
         # get all var inits
@@ -658,15 +664,15 @@
                     )
                     if call and call in potential_var_names
                 ]
                 self._replace_var_calls(data, new_var_calls, potential_var_names)
 
         return data
 
-    def _resolve_vars(self, config: list[list]) -> None:
+    def _resolve_vars(self, config: List[list]) -> None:
         """
         Replace every variable call in a package config with the variable's value.
 
         Custom package data structure rules:
             The last list element is a value.
             The second last list element is a value's key.
             When variable call found, work backwards from the call to find the most recent
@@ -711,15 +717,15 @@
             if not var_calls or self.warnings:
                 break
 
             config = self._replace_var_calls(config, var_calls, potential_var_names)
 
         return config
 
-    def _find_plugin_paths(self, paths: list[list]) -> list[str]:
+    def _find_plugin_paths(self, paths: List[list]) -> List[str]:
         """
         Find all the plugin paths in the package.
         Returns a list of all the valid paths.
         """
 
         def split_paths(string: str) -> list:
             """
```

### Comparing `houdini_package_manager-1.0.1/houdini_package_manager/wrangle/package_templates.py` & `houdini_package_manager-1.0.4/houdini_package_manager/wrangle/package_templates.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.1/pyproject.toml` & `houdini_package_manager-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "houdini_package_manager"
-version = "1.0.1"
+version = "1.0.4"
 description = "GUI package manager for Houdini"
 authors = ["Ariff Jeff <fariffjeff@icloud.com>"]
 repository = "https://github.com/ariffjeff/houdini-package-manager"
 documentation = "https://ariffjeff.github.io/houdini-package-manager/"
 readme = "README.md"
 packages = [
   {include = "houdini_package_manager"}
```

### Comparing `houdini_package_manager-1.0.1/PKG-INFO` & `houdini_package_manager-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: houdini-package-manager
-Version: 1.0.1
+Version: 1.0.4
 Summary: GUI package manager for Houdini
 Home-page: https://github.com/ariffjeff/houdini-package-manager
 Author: Ariff Jeff
 Author-email: fariffjeff@icloud.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

