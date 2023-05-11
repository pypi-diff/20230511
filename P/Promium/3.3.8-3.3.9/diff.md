# Comparing `tmp/Promium-3.3.8.tar.gz` & `tmp/Promium-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Promium-3.3.8.tar", last modified: Wed Aug 24 07:28:27 2022, max compression
+gzip compressed data, was "Promium-3.3.9.tar", last modified: Fri Oct 28 20:28:27 2022, max compression
```

## Comparing `Promium-3.3.8.tar` & `Promium-3.3.9.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2022-08-24 07:28:27.000000 Promium-3.3.8/
--rw-r--r--   0 promium   (1000) promium   (1000)     6226 2022-08-24 07:28:27.000000 Promium-3.3.8/PKG-INFO
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2022-08-24 07:28:27.000000 Promium-3.3.8/Promium.egg-info/
--rw-r--r--   0 promium   (1000) promium   (1000)     6226 2022-08-24 07:28:27.000000 Promium-3.3.8/Promium.egg-info/PKG-INFO
--rw-r--r--   0 promium   (1000) promium   (1000)     1388 2022-08-24 07:28:27.000000 Promium-3.3.8/Promium.egg-info/SOURCES.txt
--rw-r--r--   0 promium   (1000) promium   (1000)        1 2022-08-24 07:28:27.000000 Promium-3.3.8/Promium.egg-info/dependency_links.txt
--rw-r--r--   0 promium   (1000) promium   (1000)       37 2022-08-24 07:28:27.000000 Promium-3.3.8/Promium.egg-info/entry_points.txt
--rw-r--r--   0 promium   (1000) promium   (1000)      160 2022-08-24 07:28:27.000000 Promium-3.3.8/Promium.egg-info/requires.txt
--rw-r--r--   0 promium   (1000) promium   (1000)       18 2022-08-24 07:28:27.000000 Promium-3.3.8/Promium.egg-info/top_level.txt
--rw-rw-rw-   0 promium   (1000) promium   (1000)     3982 2022-08-19 12:12:16.000000 Promium-3.3.8/README.rst
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2022-08-24 07:28:27.000000 Promium-3.3.8/doc/
--rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2022-08-19 12:12:16.000000 Promium-3.3.8/doc/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     8763 2022-08-19 12:12:16.000000 Promium-3.3.8/doc/conf.py
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2022-08-24 07:28:27.000000 Promium-3.3.8/promium/
--rw-rw-rw-   0 promium   (1000) promium   (1000)      727 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)    17501 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/assertions.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)    24392 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/base.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     9484 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/browsers.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     9343 2022-08-24 07:25:02.000000 Promium-3.3.8/promium/common.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1995 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/device_config.py
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2022-08-24 07:28:27.000000 Promium-3.3.8/promium/elements/
--rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/elements/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      335 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/elements/checkbox.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      953 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/elements/drop_downs.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      245 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/elements/frame.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1937 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/elements/input_field.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1312 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/elements/link.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      631 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/elements/multiselect_listbox.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1149 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/elements/radio_button.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)       98 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/elements/textarea_field.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      200 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/elements/upload_button.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      545 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/exceptions.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1754 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/expected_conditions.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1738 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/helpers.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     8802 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/logger.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)    17666 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/plugin.py
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2022-08-24 07:28:27.000000 Promium-3.3.8/promium/support/
--rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/support/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     9216 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/support/settings.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     6220 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/test_case.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     8760 2022-08-19 12:12:16.000000 Promium-3.3.8/promium/waits.py
--rw-r--r--   0 promium   (1000) promium   (1000)       38 2022-08-24 07:28:27.000000 Promium-3.3.8/setup.cfg
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1311 2022-08-24 07:25:02.000000 Promium-3.3.8/setup.py
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2022-08-24 07:28:27.000000 Promium-3.3.8/tests/
--rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      165 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/config.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)       43 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/conftest.py
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2022-08-24 07:28:27.000000 Promium-3.3.8/tests/pages/
--rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/pages/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      624 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/pages/catalog_404_page.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     2272 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/pages/catalog_gallery_page.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     2074 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/pages/catalog_main_page.py
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2022-08-24 07:28:27.000000 Promium-3.3.8/tests/settings/
--rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/settings/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     8278 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/settings/test_base.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     2448 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/settings/test_chrome.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      896 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/settings/test_edge.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     4397 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/settings/test_firefox.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1341 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/settings/test_ie.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      431 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/settings/test_opera.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1804 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/test_catalog_404.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1121 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/test_catalog_gallery.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      795 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/test_requests.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)    13115 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/test_soft_asserts.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     7846 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/test_waits.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      667 2022-08-19 12:12:16.000000 Promium-3.3.8/tests/urls.py
+drwxrwxr-x   0 oleh      (1000) oleh      (1000)        0 2022-10-28 20:28:27.032155 Promium-3.3.9/
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     1063 2020-04-25 14:54:05.000000 Promium-3.3.9/LICENSE
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     4749 2022-10-28 20:28:27.032155 Promium-3.3.9/PKG-INFO
+drwxrwxr-x   0 oleh      (1000) oleh      (1000)        0 2022-10-28 20:28:27.028155 Promium-3.3.9/Promium.egg-info/
+-rw-r--r--   0 oleh      (1000) oleh      (1000)     4749 2022-10-28 20:28:27.000000 Promium-3.3.9/Promium.egg-info/PKG-INFO
+-rw-r--r--   0 oleh      (1000) oleh      (1000)     1396 2022-10-28 20:28:27.000000 Promium-3.3.9/Promium.egg-info/SOURCES.txt
+-rw-r--r--   0 oleh      (1000) oleh      (1000)        1 2022-10-28 20:28:27.000000 Promium-3.3.9/Promium.egg-info/dependency_links.txt
+-rw-r--r--   0 oleh      (1000) oleh      (1000)       37 2022-10-28 20:28:27.000000 Promium-3.3.9/Promium.egg-info/entry_points.txt
+-rw-r--r--   0 oleh      (1000) oleh      (1000)      160 2022-10-28 20:28:27.000000 Promium-3.3.9/Promium.egg-info/requires.txt
+-rw-r--r--   0 oleh      (1000) oleh      (1000)       18 2022-10-28 20:28:27.000000 Promium-3.3.9/Promium.egg-info/top_level.txt
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     3982 2020-04-25 14:54:05.000000 Promium-3.3.9/README.rst
+drwxrwxr-x   0 oleh      (1000) oleh      (1000)        0 2022-10-28 20:28:27.028155 Promium-3.3.9/doc/
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)        0 2020-04-25 14:54:05.000000 Promium-3.3.9/doc/__init__.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     8763 2020-04-25 14:54:05.000000 Promium-3.3.9/doc/conf.py
+drwxrwxr-x   0 oleh      (1000) oleh      (1000)        0 2022-10-28 20:28:27.028155 Promium-3.3.9/promium/
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      727 2021-07-27 07:33:22.000000 Promium-3.3.9/promium/__init__.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)    18076 2022-10-28 19:59:13.000000 Promium-3.3.9/promium/assertions.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)    24392 2022-08-04 13:21:22.000000 Promium-3.3.9/promium/base.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     9484 2022-06-28 15:48:30.000000 Promium-3.3.9/promium/browsers.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     9770 2022-10-28 19:59:13.000000 Promium-3.3.9/promium/common.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     1995 2022-01-31 13:50:26.000000 Promium-3.3.9/promium/device_config.py
+drwxrwxr-x   0 oleh      (1000) oleh      (1000)        0 2022-10-28 20:28:27.028155 Promium-3.3.9/promium/elements/
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)        0 2020-04-25 14:54:05.000000 Promium-3.3.9/promium/elements/__init__.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      335 2020-04-25 14:54:05.000000 Promium-3.3.9/promium/elements/checkbox.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      953 2020-04-25 14:54:05.000000 Promium-3.3.9/promium/elements/drop_downs.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      245 2021-07-27 07:33:22.000000 Promium-3.3.9/promium/elements/frame.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     1937 2021-05-11 09:23:09.000000 Promium-3.3.9/promium/elements/input_field.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     1312 2021-11-22 11:37:42.000000 Promium-3.3.9/promium/elements/link.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      631 2020-04-25 14:54:05.000000 Promium-3.3.9/promium/elements/multiselect_listbox.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     1149 2020-04-25 14:54:05.000000 Promium-3.3.9/promium/elements/radio_button.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)       98 2020-04-25 14:54:05.000000 Promium-3.3.9/promium/elements/textarea_field.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      200 2020-04-25 14:54:05.000000 Promium-3.3.9/promium/elements/upload_button.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      545 2020-04-25 14:54:05.000000 Promium-3.3.9/promium/exceptions.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     1754 2020-04-25 14:54:05.000000 Promium-3.3.9/promium/expected_conditions.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     1738 2020-04-25 14:54:05.000000 Promium-3.3.9/promium/helpers.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     8802 2022-09-01 16:30:32.000000 Promium-3.3.9/promium/logger.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)    17666 2022-06-28 20:20:46.000000 Promium-3.3.9/promium/plugin.py
+drwxrwxr-x   0 oleh      (1000) oleh      (1000)        0 2022-10-28 20:28:27.028155 Promium-3.3.9/promium/support/
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)        0 2020-04-25 14:54:05.000000 Promium-3.3.9/promium/support/__init__.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     9216 2021-02-18 11:18:37.000000 Promium-3.3.9/promium/support/settings.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     6220 2022-08-04 12:47:03.000000 Promium-3.3.9/promium/test_case.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     8760 2022-05-26 07:14:11.000000 Promium-3.3.9/promium/waits.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)       38 2022-10-28 20:28:27.032155 Promium-3.3.9/setup.cfg
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     1311 2022-10-28 19:59:13.000000 Promium-3.3.9/setup.py
+drwxrwxr-x   0 oleh      (1000) oleh      (1000)        0 2022-10-28 20:28:27.028155 Promium-3.3.9/tests/
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)        0 2020-04-25 14:54:05.000000 Promium-3.3.9/tests/__init__.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      165 2020-04-25 14:54:05.000000 Promium-3.3.9/tests/config.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)       43 2022-01-14 09:25:42.000000 Promium-3.3.9/tests/conftest.py
+drwxrwxr-x   0 oleh      (1000) oleh      (1000)        0 2022-10-28 20:28:27.032155 Promium-3.3.9/tests/pages/
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)        0 2020-04-25 14:54:05.000000 Promium-3.3.9/tests/pages/__init__.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      624 2022-01-14 09:25:42.000000 Promium-3.3.9/tests/pages/catalog_404_page.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     2272 2020-04-25 14:54:05.000000 Promium-3.3.9/tests/pages/catalog_gallery_page.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     2074 2022-10-18 11:16:44.000000 Promium-3.3.9/tests/pages/catalog_main_page.py
+drwxrwxr-x   0 oleh      (1000) oleh      (1000)        0 2022-10-28 20:28:27.032155 Promium-3.3.9/tests/settings/
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)        0 2020-04-25 14:54:05.000000 Promium-3.3.9/tests/settings/__init__.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     8278 2021-02-18 11:18:37.000000 Promium-3.3.9/tests/settings/test_base.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     2448 2020-04-25 14:54:05.000000 Promium-3.3.9/tests/settings/test_chrome.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      896 2020-04-25 14:54:05.000000 Promium-3.3.9/tests/settings/test_edge.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     4397 2021-02-18 11:18:37.000000 Promium-3.3.9/tests/settings/test_firefox.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     1341 2020-04-25 14:54:05.000000 Promium-3.3.9/tests/settings/test_ie.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      431 2020-04-25 14:54:05.000000 Promium-3.3.9/tests/settings/test_opera.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     1804 2022-01-14 09:25:42.000000 Promium-3.3.9/tests/test_catalog_404.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     1121 2021-02-18 11:18:37.000000 Promium-3.3.9/tests/test_catalog_gallery.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      795 2022-01-14 09:25:42.000000 Promium-3.3.9/tests/test_requests.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)    13115 2020-04-25 14:54:05.000000 Promium-3.3.9/tests/test_soft_asserts.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)     7846 2020-04-25 14:54:05.000000 Promium-3.3.9/tests/test_waits.py
+-rw-rw-r--   0 oleh      (1000) oleh      (1000)      667 2020-04-25 14:54:05.000000 Promium-3.3.9/tests/urls.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Promium-3.3.8/Promium.egg-info/SOURCES.txt` & `Promium-3.3.9/Promium.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.rst
 setup.py
 Promium.egg-info/PKG-INFO
 Promium.egg-info/SOURCES.txt
 Promium.egg-info/dependency_links.txt
 Promium.egg-info/entry_points.txt
 Promium.egg-info/requires.txt
```

### Comparing `Promium-3.3.8/README.rst` & `Promium-3.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/doc/conf.py` & `Promium-3.3.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/__init__.py` & `Promium-3.3.9/promium/__init__.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/assertions.py` & `Promium-3.3.9/promium/assertions.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,29 +52,41 @@
 
 
 class BaseSoftAssertion(object):
 
     # TODO is not cleaned in unit tests need use __init__
     assertion_errors = []
 
-    def soft_assert_true(self, expr, msg=None):
+    @property
+    def add_screenshot(self):
+        if hasattr(self, 'driver'):
+            return f"\nScreenshot: {upload_screenshot(self.driver)}\n"
+        else:
+            return ''
+
+    def soft_assert_true(self, expr, msg=None, with_screen=False):
         """Check that the expression is true."""
         if not expr:
             error = "Is not true." if not msg else msg
-            self.assertion_errors.append(f"{error}\n")
+            screen = self.add_screenshot() if with_screen else ''
+            self.assertion_errors.append(f"{error}{screen}\n")
             return error
 
-    def soft_assert_false(self, expr, msg=None):
+    def soft_assert_false(self, expr, msg=None, with_screen=False):
         """Check that the expression is false."""
         if expr:
             message = "Is not false." if not msg else msg
-            self.assertion_errors.append(f"{message}\n")
+            screen = self.add_screenshot() if with_screen else ''
+            self.assertion_errors.append(f"{message}{screen}\n")
             return message
 
-    def soft_assert_equals(self, current, expected, msg=None, show_diff=False):
+    def soft_assert_equals(
+            self, current, expected, msg=None, show_diff=False,
+            with_screen=False,
+    ):
         """Just like self.soft_assert_true(current == expected)"""
         message = (
             f"Current and expected has different data types: "
             f"current is {type(current)}, expected is {type(expected)}\n"
             if type(current) != type(expected) else ""
         )
         difference = ""
@@ -92,40 +104,44 @@
         assert_message = (
             f"{base_msg(msg)}\n"
             f"Current - {convert_container(current)}\n"
             f"Expected - {convert_container(expected)}\n"
             f"{difference}"
             f"{message}"
         )
-        return self.soft_assert_true(current == expected, assert_message)
+        return self.soft_assert_true(
+            current == expected, assert_message, with_screen
+        )
 
     def soft_assert_not_equals(self, current, expected, msg=None):
         """Just like self.soft_assert_true(current != expected)"""
         message = (
             f"{base_msg(msg)}"
             f"Current - {convert_container(current)}\n"
             f"Expected - {convert_container(expected)}\n"
         )
         self.soft_assert_false(current == expected, message)
 
-    def soft_assert_in(self, member, container, msg=None):
+    def soft_assert_in(self, member, container, msg=None, with_screen=False):
         """Just like self.soft_assert_true(member IN container)"""
         msg = (
             f"{base_msg(msg)}"
             f"{member} not found in {convert_container(container)}\n"
         )
-        return self.soft_assert_true(member in container, msg)
+        return self.soft_assert_true(member in container, msg, with_screen)
 
-    def soft_assert_not_in(self, member, container, msg=None):
+    def soft_assert_not_in(
+            self, member, container, msg=None, with_screen=False
+    ):
         """Just like self.soft_assert_true(member NOT IN container)"""
         msg = (
             f"{base_msg(msg)}"
             f"{member} unexpectedly found in {convert_container(container)}\n"
         )
-        return self.soft_assert_true(member not in container, msg)
+        return self.soft_assert_true(member not in container, msg, with_screen)
 
     def soft_assert_less_equal(self, a, b, msg=None):
         """Just like self.soft_assert_true(a <= b)"""
         error = f"{base_msg(msg)}{a} not less than or equal to {b}\n"
         return self.soft_assert_true(a <= b, error)
 
     def soft_assert_less(self, a, b, msg=None):
@@ -351,76 +367,75 @@
     def driver(self):
         return self.driver
 
     @property
     def url(self):
         return self.driver.current_url
 
-    @property
-    def assertion_screenshot(self):
-        return upload_screenshot(self.driver)
-
     def base_msg(self, default_msg=None, extend_msg=None):
         default = f"Default message: {default_msg}\n" if default_msg else ""
         extend = f"Extend message: {extend_msg}\n" if extend_msg else ""
         return (
             f"{default}{extend}"
             f"URL: {self.url}\n"
-            f"Screenshot: {self.assertion_screenshot}\n"
         )
 
     def soft_assert_page_title(self, expected_title, msg=None):
         default_msg = 'Wrong page title.'
         error = f"{self.base_msg(default_msg=default_msg, extend_msg=msg)}"
-        self.soft_assert_equals(self.driver.title, expected_title, error)
+        self.soft_assert_equals(
+            self.driver.title, expected_title, error, with_screen=True
+        )
 
     def soft_assert_current_url(self, expected_url, msg=None):
         default_msg = 'Wrong current url.'
         error = f"{self.base_msg(default_msg=default_msg, extend_msg=msg)}"
-        self.soft_assert_equals(self.url, expected_url, error)
+        self.soft_assert_equals(
+            self.url, expected_url, error, with_screen=True
+        )
 
     def soft_assert_current_url_contains(self, url_mask, msg=None):
         default_msg = f"URL {str(self.url)} doesn't contains {str(url_mask)}."
         error = f"{self.base_msg(default_msg=default_msg, extend_msg=msg)}"
-        self.soft_assert_in(url_mask, self.url, error)
+        self.soft_assert_in(url_mask, self.url, error, with_screen=True)
 
     def soft_assert_current_url_not_contains(self, url_mask, msg=None):
         default_msg = f"URL {str(self.url)} contains {str(url_mask)}."
         error = f"{self.base_msg(default_msg=default_msg, extend_msg=msg)}"
-        self.soft_assert_not_in(url_mask, self.url, error)
+        self.soft_assert_not_in(url_mask, self.url, error, with_screen=True)
 
     def soft_assert_element_is_present(self, element, msg=None):
         default_msg = (
             f"Element {element.by}={element.locator} is not present "
             f"on page at current time."
         )
         error = f"{self.base_msg(default_msg=default_msg, extend_msg=msg)}"
-        self.soft_assert_true(element.is_present(), error)
+        self.soft_assert_true(element.is_present(), error, with_screen=True)
 
     def soft_assert_element_is_not_present(self, element, msg=None):
         default_msg = (
             f"Element {element.by}={element.locator} is found on page."
         )
         error = f"{self.base_msg(default_msg=default_msg, extend_msg=msg)}"
-        self.soft_assert_false(element.is_present(), error)
+        self.soft_assert_false(element.is_present(), error, with_screen=True)
 
     def soft_assert_element_is_displayed(self, element, msg=None):
         default_msg = (
             f"Element {element.by}={element.locator} is "
             f"not visible to a user."
         )
         error = f"{self.base_msg(default_msg=default_msg, extend_msg=msg)}"
-        self.soft_assert_true(element.is_displayed(), error)
+        self.soft_assert_true(element.is_displayed(), error, with_screen=True)
 
     def soft_assert_element_is_not_displayed(self, element, msg=None):
         default_msg = (
             f"Element {element.by}={element.locator} is visible to a user."
         )
         error = f"{self.base_msg(default_msg=default_msg, extend_msg=msg)}"
-        self.soft_assert_false(element.is_displayed(), error)
+        self.soft_assert_false(element.is_displayed(), error, with_screen=True)
 
     def soft_assert_element_displayed_in_viewport(self, element, msg=None):
         """This method checks that element is viewable in viewport"""
         element_in_viewport = self.driver.execute_script(
             """
             function elementInViewport(el) {
                 var top = el.offsetTop;
```

### Comparing `Promium-3.3.8/promium/base.py` & `Promium-3.3.9/promium/base.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/browsers.py` & `Promium-3.3.9/promium/browsers.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/common.py` & `Promium-3.3.9/promium/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,16 +131,35 @@
     screenshots_folder = "/tmp"
     if not os.path.exists(screenshots_folder):
         os.makedirs(screenshots_folder)
     screenshot_path = os.path.join(screenshots_folder, screenshot_name)
     return screenshot_path, screenshot_name
 
 
+def if_server_have_problem():
+    try:
+        r = requests.get(
+            url=f"https://{SCREENSHOT_SERVER_HOST}",
+            verify=False,
+            timeout=(5, 5),
+        )
+        print(r.status_code)
+        r.raise_for_status()
+        return False
+    except Exception as e:
+        print(e)
+        return str(e)
+
+
 def _upload_to_server(screenshot_path, screenshot_name):
 
+    status_server = if_server_have_problem()
+    if status_server:
+        return status_server
+
     def read_in_chunks(img, block_size=1024, chunks=-1):
         """
         Lazy function (generator) to read a file piece by piece.
         Default chunk size: 1k.
         """
         while chunks:
             data = img.read(block_size)
@@ -150,15 +169,15 @@
             chunks -= 1
 
     screenshot_url = f"https://{SCREENSHOT_SERVER_HOST}/{screenshot_name}"
     r = requests.put(
         url=screenshot_url,
         auth=(SCREENSHOT_SERVER_LOGIN, SCREENSHOT_SERVER_PASSWORD),
         data=read_in_chunks(open(screenshot_path, 'rb')),
-        verify=False
+        verify=False,
     )
     os.remove(screenshot_path)
     if not r.ok:
         return (
             f"Screenshot not uploaded to server. "
             f"Status code: {r.status_code}, reason: {r.reason}"
         )
```

### Comparing `Promium-3.3.8/promium/device_config.py` & `Promium-3.3.9/promium/device_config.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/elements/drop_downs.py` & `Promium-3.3.9/promium/elements/drop_downs.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/elements/input_field.py` & `Promium-3.3.9/promium/elements/input_field.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/elements/link.py` & `Promium-3.3.9/promium/elements/link.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/elements/multiselect_listbox.py` & `Promium-3.3.9/promium/elements/multiselect_listbox.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/elements/radio_button.py` & `Promium-3.3.9/promium/elements/radio_button.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/exceptions.py` & `Promium-3.3.9/promium/exceptions.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/expected_conditions.py` & `Promium-3.3.9/promium/expected_conditions.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/helpers.py` & `Promium-3.3.9/promium/helpers.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/logger.py` & `Promium-3.3.9/promium/logger.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/plugin.py` & `Promium-3.3.9/promium/plugin.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/support/settings.py` & `Promium-3.3.9/promium/support/settings.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/test_case.py` & `Promium-3.3.9/promium/test_case.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/promium/waits.py` & `Promium-3.3.9/promium/waits.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/setup.py` & `Promium-3.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     'pytest-instafail>=0.3.0',
     'deepdiff>=5.7.0',
 ]
 
 
 setup(
     name='Promium',
-    version='3.3.8',
+    version='3.3.9',
     install_requires=REQUIREMENTS,
     author='Denis Korytkin, Nataliia Guieva,'
            ' Roman Zaporozhets, Vladimir Kritov',
     project_urls={
         'Home page': 'https://none',
         'Documentation': 'https://none',
     },
```

### Comparing `Promium-3.3.8/tests/pages/catalog_404_page.py` & `Promium-3.3.9/tests/pages/catalog_404_page.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/pages/catalog_gallery_page.py` & `Promium-3.3.9/tests/pages/catalog_gallery_page.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/pages/catalog_main_page.py` & `Promium-3.3.9/tests/pages/catalog_main_page.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/settings/test_base.py` & `Promium-3.3.9/tests/settings/test_base.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/settings/test_chrome.py` & `Promium-3.3.9/tests/settings/test_chrome.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/settings/test_edge.py` & `Promium-3.3.9/tests/settings/test_edge.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/settings/test_firefox.py` & `Promium-3.3.9/tests/settings/test_firefox.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/settings/test_ie.py` & `Promium-3.3.9/tests/settings/test_ie.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/test_catalog_404.py` & `Promium-3.3.9/tests/test_catalog_404.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/test_catalog_gallery.py` & `Promium-3.3.9/tests/test_catalog_gallery.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/test_requests.py` & `Promium-3.3.9/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/test_soft_asserts.py` & `Promium-3.3.9/tests/test_soft_asserts.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/test_waits.py` & `Promium-3.3.9/tests/test_waits.py`

 * *Files identical despite different names*

### Comparing `Promium-3.3.8/tests/urls.py` & `Promium-3.3.9/tests/urls.py`

 * *Files identical despite different names*

