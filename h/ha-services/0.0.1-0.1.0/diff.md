# Comparing `tmp/ha-services-0.0.1.tar.gz` & `tmp/ha-services-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ha-services-0.0.1.tar", last modified: Sun May  7 20:28:49 2023, max compression
+gzip compressed data, was "ha-services-0.1.0.tar", last modified: Wed May 10 21:49:17 2023, max compression
```

## Comparing `ha-services-0.0.1.tar` & `ha-services-0.1.0.tar`

### file list

```diff
@@ -1,62 +1,82 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 20:28:49.346429 ha-services-0.0.1/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-05-07 13:00:08.000000 ha-services-0.0.1/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-05-07 13:00:08.000000 ha-services-0.0.1/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 20:28:49.342429 ha-services-0.0.1/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 20:28:49.342429 ha-services-0.0.1/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-05-07 13:00:08.000000 ha-services-0.0.1/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-05-07 13:00:08.000000 ha-services-0.0.1/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)     1195 2023-05-07 20:28:49.346429 ha-services-0.0.1/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)      782 2023-05-07 13:00:08.000000 ha-services-0.0.1/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-07 13:00:08.000000 ha-services-0.0.1/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-07 13:00:08.000000 ha-services-0.0.1/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 20:28:49.346429 ha-services-0.0.1/ha_services/
--rw-rw-r--   0 jens      (1000) users      (100)      165 2023-05-07 13:00:08.000000 ha-services-0.0.1/ha_services/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      195 2023-05-07 13:00:08.000000 ha-services-0.0.1/ha_services/__main__.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 20:28:49.346429 ha-services-0.0.1/ha_services/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-07 13:00:08.000000 ha-services-0.0.1/ha_services/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4815 2023-05-07 20:27:47.000000 ha-services-0.0.1/ha_services/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     7880 2023-05-07 20:27:28.000000 ha-services-0.0.1/ha_services/cli/dev.py
--rw-rw-r--   0 jens      (1000) users      (100)       70 2023-05-07 13:00:08.000000 ha-services-0.0.1/ha_services/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)     2541 2023-05-07 20:24:36.000000 ha-services-0.0.1/ha_services/example.py
--rw-rw-r--   0 jens      (1000) users      (100)      240 2023-05-07 17:54:01.000000 ha-services-0.0.1/ha_services/log_setup.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 20:28:49.346429 ha-services-0.0.1/ha_services/mqtt4homeassistant/
--rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 ha-services-0.0.1/ha_services/mqtt4homeassistant/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1898 2023-05-07 13:08:23.000000 ha-services-0.0.1/ha_services/mqtt4homeassistant/converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1061 2023-05-07 14:48:08.000000 ha-services-0.0.1/ha_services/mqtt4homeassistant/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     3723 2023-05-07 20:22:58.000000 ha-services-0.0.1/ha_services/mqtt4homeassistant/mqtt.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 20:28:49.346429 ha-services-0.0.1/ha_services/mqtt4homeassistant/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 ha-services-0.0.1/ha_services/mqtt4homeassistant/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2142 2023-05-07 13:08:23.000000 ha-services-0.0.1/ha_services/mqtt4homeassistant/tests/test_converter.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 20:28:49.346429 ha-services-0.0.1/ha_services/mqtt4homeassistant/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 ha-services-0.0.1/ha_services/mqtt4homeassistant/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 ha-services-0.0.1/ha_services/mqtt4homeassistant/utilities/string_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 20:28:49.346429 ha-services-0.0.1/ha_services/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      262 2023-05-07 14:19:56.000000 ha-services-0.0.1/ha_services/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      217 2023-05-07 13:00:08.000000 ha-services-0.0.1/ha_services/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2579 2023-05-07 20:28:20.000000 ha-services-0.0.1/ha_services/tests/test_project_setup.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 20:28:49.346429 ha-services-0.0.1/ha_services/toml_settings/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-07 15:11:40.000000 ha-services-0.0.1/ha_services/toml_settings/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2378 2023-05-07 19:34:06.000000 ha-services-0.0.1/ha_services/toml_settings/api.py
--rw-rw-r--   0 jens      (1000) users      (100)      233 2023-05-07 16:01:28.000000 ha-services-0.0.1/ha_services/toml_settings/data_class_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      895 2023-05-07 18:10:59.000000 ha-services-0.0.1/ha_services/toml_settings/debug.py
--rw-rw-r--   0 jens      (1000) users      (100)     2287 2023-05-07 18:26:48.000000 ha-services-0.0.1/ha_services/toml_settings/deserialize.py
--rw-rw-r--   0 jens      (1000) users      (100)       56 2023-05-07 17:49:52.000000 ha-services-0.0.1/ha_services/toml_settings/exceptions.py
--rw-rw-r--   0 jens      (1000) users      (100)      829 2023-05-07 17:38:18.000000 ha-services-0.0.1/ha_services/toml_settings/path_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      728 2023-05-07 19:07:25.000000 ha-services-0.0.1/ha_services/toml_settings/sensible_editor.py
--rw-rw-r--   0 jens      (1000) users      (100)     1456 2023-05-07 16:59:18.000000 ha-services-0.0.1/ha_services/toml_settings/serialize.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 20:28:49.346429 ha-services-0.0.1/ha_services/toml_settings/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-07 15:11:40.000000 ha-services-0.0.1/ha_services/toml_settings/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1032 2023-05-07 18:21:43.000000 ha-services-0.0.1/ha_services/toml_settings/tests/fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     4905 2023-05-07 18:29:05.000000 ha-services-0.0.1/ha_services/toml_settings/tests/test_deserialize.py
--rw-rw-r--   0 jens      (1000) users      (100)     2207 2023-05-07 18:29:30.000000 ha-services-0.0.1/ha_services/toml_settings/tests/test_serialize.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 20:28:49.346429 ha-services-0.0.1/ha_services.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)     1195 2023-05-07 20:28:49.000000 ha-services-0.0.1/ha_services.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     1591 2023-05-07 20:28:49.000000 ha-services-0.0.1/ha_services.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-07 20:28:49.000000 ha-services-0.0.1/ha_services.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)      105 2023-05-07 20:28:49.000000 ha-services-0.0.1/ha_services.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      268 2023-05-07 20:28:49.000000 ha-services-0.0.1/ha_services.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)       12 2023-05-07 20:28:49.000000 ha-services-0.0.1/ha_services.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4860 2023-05-07 20:27:28.000000 ha-services-0.0.1/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    53227 2023-05-07 14:32:50.000000 ha-services-0.0.1/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4979 2023-05-07 14:32:31.000000 ha-services-0.0.1/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-07 20:28:49.346429 ha-services-0.0.1/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-05-09 16:39:25.000000 ha-services-0.1.0/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-05-09 16:39:25.000000 ha-services-0.1.0/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-09 16:39:25.000000 ha-services-0.1.0/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-05-09 16:39:25.000000 ha-services-0.1.0/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)     1236 2023-05-10 21:49:17.213478 ha-services-0.1.0/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)      823 2023-05-09 16:39:25.000000 ha-services-0.1.0/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-09 16:39:25.000000 ha-services-0.1.0/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-09 16:39:25.000000 ha-services-0.1.0/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services/
+-rw-rw-r--   0 jens      (1000) users      (100)      165 2023-05-10 21:39:16.000000 ha-services-0.1.0/ha_services/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      195 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7205 2023-05-10 20:16:42.000000 ha-services-0.1.0/ha_services/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7880 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/cli/dev.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services/cli_tools/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.1.0/ha_services/cli_tools/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1649 2023-05-10 07:48:43.000000 ha-services-0.1.0/ha_services/cli_tools/richt_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services/cli_tools/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.1.0/ha_services/cli_tools/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      892 2023-05-10 21:26:41.000000 ha-services-0.1.0/ha_services/cli_tools/test_utils/assertion.py
+-rw-rw-r--   0 jens      (1000) users      (100)      164 2023-05-09 16:59:30.000000 ha-services-0.1.0/ha_services/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2686 2023-05-09 20:53:43.000000 ha-services-0.1.0/ha_services/example.py
+-rw-rw-r--   0 jens      (1000) users      (100)      240 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/log_setup.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services/mqtt4homeassistant/
+-rw-rw-r--   0 jens      (1000) users      (100)       22 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/mqtt4homeassistant/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1898 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/mqtt4homeassistant/converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1061 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/mqtt4homeassistant/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3723 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/mqtt4homeassistant/mqtt.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services/mqtt4homeassistant/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/mqtt4homeassistant/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2142 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/mqtt4homeassistant/tests/test_converter.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services/mqtt4homeassistant/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/mqtt4homeassistant/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      315 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/mqtt4homeassistant/utilities/string_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services/systemd/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.1.0/ha_services/systemd/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4184 2023-05-10 20:41:17.000000 ha-services-0.1.0/ha_services/systemd/api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3302 2023-05-10 07:31:01.000000 ha-services-0.1.0/ha_services/systemd/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)      505 2023-05-10 07:16:49.000000 ha-services-0.1.0/ha_services/systemd/defaults.py
+-rw-rw-r--   0 jens      (1000) users      (100)      331 2023-05-09 19:57:06.000000 ha-services-0.1.0/ha_services/systemd/service_template.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     1794 2023-05-09 19:43:34.000000 ha-services-0.1.0/ha_services/systemd/template.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services/systemd/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.1.0/ha_services/systemd/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3156 2023-05-10 21:37:51.000000 ha-services-0.1.0/ha_services/systemd/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1491 2023-05-10 07:43:13.000000 ha-services-0.1.0/ha_services/systemd/tests/test_data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2471 2023-05-09 19:43:34.000000 ha-services-0.1.0/ha_services/systemd/tests/test_template.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1752 2023-05-10 20:50:36.000000 ha-services-0.1.0/ha_services/systemd/tests/utilities.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      262 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      217 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2579 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/tests/test_project_setup.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services/toml_settings/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/toml_settings/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2769 2023-05-10 19:32:52.000000 ha-services-0.1.0/ha_services/toml_settings/api.py
+-rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-09 20:53:17.000000 ha-services-0.1.0/ha_services/toml_settings/data_class_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)      965 2023-05-09 20:53:17.000000 ha-services-0.1.0/ha_services/toml_settings/debug.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3059 2023-05-09 20:53:17.000000 ha-services-0.1.0/ha_services/toml_settings/deserialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)       56 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/toml_settings/exceptions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      829 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/toml_settings/path_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)      728 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/toml_settings/sensible_editor.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1647 2023-05-09 20:53:17.000000 ha-services-0.1.0/ha_services/toml_settings/serialize.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services/toml_settings/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.1.0/ha_services/toml_settings/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1229 2023-05-09 20:53:54.000000 ha-services-0.1.0/ha_services/toml_settings/tests/fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1158 2023-05-09 20:43:45.000000 ha-services-0.1.0/ha_services/toml_settings/tests/test_demo_settings.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5607 2023-05-09 17:48:29.000000 ha-services-0.1.0/ha_services/toml_settings/tests/test_deserialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2758 2023-05-09 19:41:27.000000 ha-services-0.1.0/ha_services/toml_settings/tests/test_serialize.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-10 21:49:17.213478 ha-services-0.1.0/ha_services.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)     1236 2023-05-10 21:49:17.000000 ha-services-0.1.0/ha_services.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     2212 2023-05-10 21:49:17.000000 ha-services-0.1.0/ha_services.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-10 21:49:17.000000 ha-services-0.1.0/ha_services.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      105 2023-05-10 21:49:17.000000 ha-services-0.1.0/ha_services.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      283 2023-05-10 21:49:17.000000 ha-services-0.1.0/ha_services.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       12 2023-05-10 21:49:17.000000 ha-services-0.1.0/ha_services.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4934 2023-05-09 17:58:58.000000 ha-services-0.1.0/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    53002 2023-05-09 17:59:29.000000 ha-services-0.1.0/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    22054 2023-05-09 17:59:13.000000 ha-services-0.1.0/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-10 21:49:17.213478 ha-services-0.1.0/setup.cfg
```

### Comparing `ha-services-0.0.1/.github/workflows/tests.yml` & `ha-services-0.1.0/.github/workflows/tests.yml`

 * *Files 9% similar despite different names*

```diff
@@ -35,27 +35,27 @@
         python-version: '${{ matrix.python-version }}'
         cache: 'pip' # caching pip dependencies
         cache-dependency-path: '**/requirements.dev.txt'
 
     - name: 'Bootstrap'
       # The first CLI call will create the .venv
       run: |
-        ./cli.py version
+        ./dev-cli.py version
 
     - name: 'CLI help'
       run: |
-        ./cli.py --help
+        ./dev-cli.py --help
 
     - name: 'Safety'
       run: |
-        ./cli.py safety
+        ./dev-cli.py safety
 
     - name: 'Run tests with Python v${{ matrix.python-version }}'
       run: |
-        ./cli.py coverage
+        ./dev-cli.py coverage
 
     - name: 'Upload coverage report'
       uses: codecov/codecov-action@v3
       # https://github.com/marketplace/actions/codecov
       with:
         fail_ci_if_error: false
         verbose: true
```

### Comparing `ha-services-0.0.1/PKG-INFO` & `ha-services-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ha-services
-Version: 0.0.1
+Version: 0.1.0
 Summary: Helpers to send periodic information via MQTT to Home Assistant
 Author-email: Jens Diemer <github@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/ha_services
 Project-URL: Source, https://github.com/jedie/ha_services
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
@@ -15,7 +15,9 @@
 [![tests](https://github.com/jedie/ha_services/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/ha_services/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/ha_services/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/ha_services)
 [![ha_services @ PyPi](https://img.shields.io/pypi/v/ha_services?label=ha_services%20%40%20PyPi)](https://pypi.org/project/ha_services/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/ha_services)](https://github.com/jedie/ha_services/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/ha_services)](https://github.com/jedie/ha_services/blob/main/LICENSE)
 
 Helpers to send periodic information via MQTT to Home Assistant
+
+* https://pypi.org/project/ha-services/
```

### Comparing `ha-services-0.0.1/README.md` & `ha-services-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,7 +3,9 @@
 [![tests](https://github.com/jedie/ha_services/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/ha_services/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/ha_services/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/ha_services)
 [![ha_services @ PyPi](https://img.shields.io/pypi/v/ha_services?label=ha_services%20%40%20PyPi)](https://pypi.org/project/ha_services/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/ha_services)](https://github.com/jedie/ha_services/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/ha_services)](https://github.com/jedie/ha_services/blob/main/LICENSE)
 
 Helpers to send periodic information via MQTT to Home Assistant
+
+* https://pypi.org/project/ha-services/
```

### Comparing `ha-services-0.0.1/cli.py` & `ha-services-0.1.0/cli.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.0.1/dev-cli.py` & `ha-services-0.1.0/dev-cli.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.0.1/ha_services/cli/dev.py` & `ha-services-0.1.0/ha_services/cli/dev.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.0.1/ha_services/example.py` & `ha-services-0.1.0/ha_services/example.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import time
 
 from rich import print  # noqa
 
 from ha_services.mqtt4homeassistant.converter import values2mqtt_payload
 from ha_services.mqtt4homeassistant.data_classes import HaValue, HaValues, MqttSettings
 from ha_services.mqtt4homeassistant.mqtt import HaMqttPublisher
+from ha_services.systemd.data_classes import SystemdServiceInfo
 
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class MqttExampleValues:
@@ -30,14 +31,15 @@
     This are just settings for the "ha-services" DEMO.
     Will be used in ha_services example commands.
     See "./cli.py --help" for more information.
     """
 
     mqtt: dataclasses = dataclasses.field(default_factory=MqttSettings)
     app: dataclasses = dataclasses.field(default_factory=MqttExampleValues)
+    systemd: dataclasses = dataclasses.field(default_factory=SystemdServiceInfo)
 
 
 def publish_forever(*, user_settings: DemoSettings, verbose):
     publisher = HaMqttPublisher(
         settings=user_settings.mqtt,
         verbose=verbose,
         config_count=1,  # Send every time the config
```

### Comparing `ha-services-0.0.1/ha_services/mqtt4homeassistant/converter.py` & `ha-services-0.1.0/ha_services/mqtt4homeassistant/converter.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.0.1/ha_services/mqtt4homeassistant/data_classes.py` & `ha-services-0.1.0/ha_services/mqtt4homeassistant/data_classes.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.0.1/ha_services/mqtt4homeassistant/mqtt.py` & `ha-services-0.1.0/ha_services/mqtt4homeassistant/mqtt.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.0.1/ha_services/mqtt4homeassistant/tests/test_converter.py` & `ha-services-0.1.0/ha_services/mqtt4homeassistant/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.0.1/ha_services/tests/test_project_setup.py` & `ha-services-0.1.0/ha_services/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.0.1/ha_services/toml_settings/api.py` & `ha-services-0.1.0/ha_services/toml_settings/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import dataclasses
 import logging
+import sys
 from collections.abc import Iterable
 
 import tomlkit
 from rich import print  # noqa
 from rich.console import Console
 from tomlkit import TOMLDocument
 
@@ -14,26 +15,26 @@
 from ha_services.toml_settings.sensible_editor import open_editor_for
 from ha_services.toml_settings.serialize import dataclass2toml
 
 
 logger = logging.getLogger(__name__)
 
 
-def edit_user_settings(*, user_settings: dataclasses, settings_path: str) -> None:
+def edit_user_settings(*, user_settings, settings_path: str) -> None:
     settings_path = clean_settings_path(settings_path)
     if not settings_path.is_file():
         logger.info('Settings file "%s" not exist -> create default', settings_path)
         document: TOMLDocument = dataclass2toml(instance=user_settings)
         doc_str = tomlkit.dumps(document, sort_keys=False)
         settings_path.write_text(doc_str, encoding='UTF-8')
 
     open_editor_for(settings_path)
 
 
-def get_user_settings(*, user_settings: dataclasses, settings_path: str, debug: bool = False) -> dataclasses:
+def get_user_settings(*, user_settings, settings_path: str, debug: bool = False) -> dataclasses:
     settings_path = clean_settings_path(settings_path)
     if debug:
         print(f'Use user settings file: {settings_path}')
     if not settings_path.is_file():
         raise UserSettingsNotFound(settings_path)
 
     doc_str = settings_path.read_text(encoding='UTF-8')
@@ -46,17 +47,26 @@
         doc_str = tomlkit.dumps(user_settings_doc, sort_keys=False)
         backup(settings_path)
         settings_path.write_text(doc_str, encoding='UTF-8')
 
     return user_settings
 
 
+def get_user_settings_or_exit(*, user_settings, settings_path: str) -> dataclasses:
+    try:
+        user_settings = get_user_settings(user_settings=user_settings, settings_path=settings_path, debug=True)
+    except UserSettingsNotFound as err:
+        print(f'[yellow]No settings created yet[/yellow]: {err} [green](Hint: call "edit-settings" first!)')
+        sys.exit(1)
+    return user_settings
+
+
 def debug_print_user_settings(
-    *, user_settings: dataclasses, settings_path: str, anonymize_keys: Iterable = ('password', 'email')
+    *, user_settings, settings_path: str, anonymize_keys: Iterable = ('password', 'email')
 ) -> None:
     user_settings = get_user_settings(user_settings=user_settings, settings_path=settings_path, debug=True)
 
     print()
     console = Console()
-    console.rule('user settings')
+    console.rule(f'User settings: {settings_path}')
     print_dataclasses(instance=user_settings, anonymize_keys=anonymize_keys)
     console.rule()
```

### Comparing `ha-services-0.0.1/ha_services/toml_settings/debug.py` & `ha-services-0.1.0/ha_services/toml_settings/debug.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,20 +5,25 @@
 
 from bx_py_utils.anonymize import anonymize
 from rich import console, print  # noqa
 
 from ha_services.toml_settings.data_class_utils import iter_dataclass
 
 
-def print_dataclasses(*, instance: dataclasses, anonymize_keys: Iterable):
-    print(f'    [magenta]{instance.__class__.__name__}[/magenta]:')
+def print_dataclasses(*, instance, anonymize_keys: Iterable, indent=0):
+    print(f'{" "*indent}[magenta]{instance.__class__.__name__}[/magenta]:')
+
+    indent += 2
+
     if doc_string := inspect.getdoc(instance):
-        print(textwrap.indent(doc_string, prefix='    # '))
+        print(textwrap.indent(doc_string, prefix=' ' * indent))
+
+    indent += 2
 
     for field_name, field_value in iter_dataclass(instance):
         if dataclasses.is_dataclass(field_value):
             print()
-            print_dataclasses(instance=field_value, anonymize_keys=anonymize_keys)
+            print_dataclasses(instance=field_value, anonymize_keys=anonymize_keys, indent=indent + 4)
         else:
             if field_name in anonymize_keys:
                 field_value = anonymize(field_value)
-            print(f'     * [cyan]{field_name}[/cyan] = {field_value!r}')
+            print(f'{" "*indent}* [cyan]{field_name}[/cyan] = {field_value!r}')
```

### Comparing `ha-services-0.0.1/ha_services/toml_settings/deserialize.py` & `ha-services-0.1.0/ha_services/toml_settings/deserialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import dataclasses
 import logging
+from pathlib import Path
 
 import tomlkit
 from tomlkit import TOMLDocument
 
 from ha_services.toml_settings.data_class_utils import iter_dataclass
 from ha_services.toml_settings.serialize import add_dataclass
 
 
 logger = logging.getLogger(__name__)
 
 
-def toml2dataclass(*, document: TOMLDocument, instance: dataclasses, _changed=False) -> bool:
+def toml2dataclass(*, document: TOMLDocument, instance, _changed=False) -> bool:
     """
     Sync toml and instance in place:
 
      - Transfer all valid values from toml document into the data class instance
      - Add missing or invalid values to the toml document
     """
 
@@ -42,14 +43,31 @@
             # Add missing item, so that the toml file can be updated on disk:
             document[field_name] = field_value
             _changed = True
             continue
 
         if field_value == doc_value:
             logger.debug('Default value %r also used in toml file, ok.', field_value)
+        elif isinstance(field_value, Path):
+            logger.debug('Convert %r value %r to Path instance', field_name, field_value)
+            value = doc_value.unwrap()
+            if not isinstance(value, str):
+                logger.error(
+                    (
+                        'Toml value %s=%r is type %r but must be type str (Will be convert to Path instance)'
+                        ' -> ignored and use default value!'
+                    ),
+                    field_name,
+                    value,
+                    type(value).__name__,
+                )
+                document[field_name] = field_value  # Add default one
+                _changed = True
+            else:
+                setattr(instance, field_name, Path(value))
         elif not isinstance(field_value, type(doc_value.unwrap())):
             logger.error(
                 'Toml value %s=%r is type %r but must be type %r -> ignored and use default value!',
                 field_name,
                 doc_value,
                 type(doc_value.unwrap()).__name__,
                 type(field_value).__name__,
```

### Comparing `ha-services-0.0.1/ha_services/toml_settings/path_utils.py` & `ha-services-0.1.0/ha_services/toml_settings/path_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.0.1/ha_services/toml_settings/sensible_editor.py` & `ha-services-0.1.0/ha_services/toml_settings/sensible_editor.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.0.1/ha_services/toml_settings/serialize.py` & `ha-services-0.1.0/ha_services/toml_settings/serialize.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 import dataclasses
 import inspect
+from pathlib import Path
 
 import tomlkit
 from tomlkit import TOMLDocument
+from tomlkit.items import Item
 
 from ha_services.toml_settings.data_class_utils import iter_dataclass
 
 
 def add_docstring(document: TOMLDocument, instance):
     if doc_string := inspect.getdoc(instance):
         for line in doc_string.strip().splitlines():
             document.add(tomlkit.comment(line))
 
 
-def add_dataclass(document: TOMLDocument, name, instance: dataclasses):
+def add_value(*, field_name, item: Item, value):
+    if isinstance(value, Path):
+        value = str(value)
+
+    item.add(field_name, value)
+
+
+def add_dataclass(document: TOMLDocument, name, instance):
     assert dataclasses.is_dataclass(instance), f'No dataclass: {instance!r}'
 
     document.add(tomlkit.nl())  # Add new line
 
     table = tomlkit.table()
     add_docstring(table, instance)
 
     for field_name, field_value in iter_dataclass(instance):
         if dataclasses.is_dataclass(field_value):
-            raise TypeError(f'Field {field_name} of dataclass {name} is a dataclass! Only two levels are allowed!')
-        table.add(field_name, field_value)
+            add_dataclass(table, field_name, field_value)
+        else:
+            add_value(field_name=field_name, item=table, value=field_value)
 
     document.add(name, table)
 
 
-def dataclass2toml(instance: dataclasses) -> TOMLDocument:
+def dataclass2toml(instance) -> TOMLDocument:
     """
     Serialize a dataclass to a tomlkit document.
     """
     assert dataclasses.is_dataclass(instance), f'No dataclass: {instance!r}'
 
     document = tomlkit.document()
     add_docstring(document, instance)
 
     for field_name, field_value in iter_dataclass(instance):
         if dataclasses.is_dataclass(field_value):
             add_dataclass(document, field_name, field_value)
         else:
-            document.add(field_name, field_value)
+            add_value(field_name=field_name, item=document, value=field_value)
 
     return document
```

### Comparing `ha-services-0.0.1/ha_services/toml_settings/tests/fixtures.py` & `ha-services-0.1.0/ha_services/toml_settings/tests/fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import dataclasses
+from pathlib import Path
 
 
 @dataclasses.dataclass
 class SimpleExample:
     """
     A simple example
     """
@@ -13,14 +14,22 @@
     number: int = 123
 
 
 ###########################################################################################
 
 
 @dataclasses.dataclass
+class PathExample:
+    path: Path = Path('/foo/bar')
+
+
+###########################################################################################
+
+
+@dataclasses.dataclass
 class SubClass1:
     """
     This is SubClass ONE on second level of FirstLevel
     """
 
     number: int = 123
```

### Comparing `ha-services-0.0.1/ha_services/toml_settings/tests/test_deserialize.py` & `ha-services-0.1.0/ha_services/toml_settings/tests/test_deserialize.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import dataclasses
 import inspect
 import logging
+from pathlib import Path
 from unittest import TestCase
 
 import tomlkit
 
 from ha_services.toml_settings.deserialize import toml2dataclass
-from ha_services.toml_settings.tests.fixtures import ComplexExample, SimpleExample
+from ha_services.toml_settings.tests.fixtures import ComplexExample, PathExample, SimpleExample
 
 
 class DeserializeTestCase(TestCase):
     def test_toml2dataclass_simple(self):
         instance = SimpleExample()
         data = dataclasses.asdict(instance)
         self.assertEqual(data, {'one': 'foo', 'two': 'bar', 'three': '', 'number': 123})
@@ -71,14 +72,42 @@
                 'ERROR:ha_services.toml_settings.deserialize:Toml value three=666 is type '
                 "'int' but must be type 'str' -> ignored and use default value!",
                 #
                 'DEBUG:ha_services.toml_settings.deserialize:Default value 123 also used in toml file, ok.',
             ],
         )
 
+    def test_toml2dataclass_path(self):
+        instance = PathExample()
+        data = dataclasses.asdict(instance)
+        self.assertEqual(
+            data,
+            {
+                'path': Path('/foo/bar'),
+            },
+        )
+
+        document = tomlkit.loads(
+            inspect.cleandoc(
+                '''
+                path = "/to/some/other/place/"
+                '''
+            ),
+        )
+
+        toml2dataclass(document=document, instance=instance)
+
+        data = dataclasses.asdict(instance)
+        self.assertEqual(
+            data,
+            {
+                'path': Path('/to/some/other/place'),
+            },
+        )
+
     def test_toml2dataclass_inheritance(self):
         instance = ComplexExample()
         data = dataclasses.asdict(instance)
         self.assertEqual(
             data,
             {
                 'foo': 'bar',
```

### Comparing `ha-services-0.0.1/ha_services/toml_settings/tests/test_serialize.py` & `ha-services-0.1.0/ha_services/toml_settings/tests/test_serialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import inspect
 from unittest import TestCase
 
 import tomlkit
 from tomlkit import TOMLDocument
 
 from ha_services.toml_settings.serialize import dataclass2toml
-from ha_services.toml_settings.tests.fixtures import ComplexExample, SimpleExample
+from ha_services.toml_settings.tests.fixtures import ComplexExample, PathExample, SimpleExample
 
 
 class SerializeTestCase(TestCase):
     def test_dataclass2toml_simple(self):
         document = dataclass2toml(instance=SimpleExample())
         self.assertIsInstance(document, TOMLDocument)
         self.assertEqual(document.unwrap(), {'one': 'foo', 'two': 'bar', 'three': '', 'number': 123})
@@ -25,14 +25,30 @@
                 two = "bar"
                 three = ""
                 number = 123
                 '''
             ),
         )
 
+    def test_dataclass2toml_path(self):
+        document = dataclass2toml(instance=PathExample())
+        self.assertIsInstance(document, TOMLDocument)
+        self.assertEqual(document.unwrap(), {'path': '/foo/bar'})
+
+        doc_str = tomlkit.dumps(document, sort_keys=False).rstrip()
+        self.assertEqual(
+            doc_str,
+            inspect.cleandoc(
+                '''
+                # PathExample(path: pathlib.Path = PosixPath('/foo/bar'))
+                path = "/foo/bar"
+                '''
+            ),
+        )
+
     def test_dataclass2toml_inheritance(self):
         instance = ComplexExample()
         data = dataclasses.asdict(instance)
         self.assertEqual(
             data,
             {
                 'foo': 'bar',
```

### Comparing `ha-services-0.0.1/ha_services.egg-info/PKG-INFO` & `ha-services-0.1.0/ha_services.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ha-services
-Version: 0.0.1
+Version: 0.1.0
 Summary: Helpers to send periodic information via MQTT to Home Assistant
 Author-email: Jens Diemer <github@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/ha_services
 Project-URL: Source, https://github.com/jedie/ha_services
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
@@ -15,7 +15,9 @@
 [![tests](https://github.com/jedie/ha_services/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/ha_services/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/ha_services/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/ha_services)
 [![ha_services @ PyPi](https://img.shields.io/pypi/v/ha_services?label=ha_services%20%40%20PyPi)](https://pypi.org/project/ha_services/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/ha_services)](https://github.com/jedie/ha_services/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/ha_services)](https://github.com/jedie/ha_services/blob/main/LICENSE)
 
 Helpers to send periodic information via MQTT to Home Assistant
+
+* https://pypi.org/project/ha-services/
```

### Comparing `ha-services-0.0.1/ha_services.egg-info/SOURCES.txt` & `ha-services-0.1.0/ha_services.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -18,31 +18,47 @@
 ha_services.egg-info/dependency_links.txt
 ha_services.egg-info/entry_points.txt
 ha_services.egg-info/requires.txt
 ha_services.egg-info/top_level.txt
 ha_services/cli/__init__.py
 ha_services/cli/cli_app.py
 ha_services/cli/dev.py
+ha_services/cli_tools/__init__.py
+ha_services/cli_tools/richt_utils.py
+ha_services/cli_tools/test_utils/__init__.py
+ha_services/cli_tools/test_utils/assertion.py
 ha_services/mqtt4homeassistant/__init__.py
 ha_services/mqtt4homeassistant/converter.py
 ha_services/mqtt4homeassistant/data_classes.py
 ha_services/mqtt4homeassistant/mqtt.py
 ha_services/mqtt4homeassistant/tests/__init__.py
 ha_services/mqtt4homeassistant/tests/test_converter.py
 ha_services/mqtt4homeassistant/utilities/__init__.py
 ha_services/mqtt4homeassistant/utilities/string_utils.py
+ha_services/systemd/__init__.py
+ha_services/systemd/api.py
+ha_services/systemd/data_classes.py
+ha_services/systemd/defaults.py
+ha_services/systemd/service_template.txt
+ha_services/systemd/template.py
+ha_services/systemd/tests/__init__.py
+ha_services/systemd/tests/test_api.py
+ha_services/systemd/tests/test_data_classes.py
+ha_services/systemd/tests/test_template.py
+ha_services/systemd/tests/utilities.py
 ha_services/tests/__init__.py
 ha_services/tests/test_doctests.py
 ha_services/tests/test_project_setup.py
 ha_services/toml_settings/__init__.py
 ha_services/toml_settings/api.py
 ha_services/toml_settings/data_class_utils.py
 ha_services/toml_settings/debug.py
 ha_services/toml_settings/deserialize.py
 ha_services/toml_settings/exceptions.py
 ha_services/toml_settings/path_utils.py
 ha_services/toml_settings/sensible_editor.py
 ha_services/toml_settings/serialize.py
 ha_services/toml_settings/tests/__init__.py
 ha_services/toml_settings/tests/fixtures.py
+ha_services/toml_settings/tests/test_demo_settings.py
 ha_services/toml_settings/tests/test_deserialize.py
 ha_services/toml_settings/tests/test_serialize.py
```

### Comparing `ha-services-0.0.1/pyproject.toml` & `ha-services-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 license = {text = "GPL-3.0-or-later"}
 readme = "README.md"
 authors = [
     {name = 'Jens Diemer', email = 'github@jensdiemer.de'}
 ]
 requires-python = ">=3.9,<4"
 dependencies = [
+    "manageprojects",  # TODO: Move all used parts into seperate project!
     "paho-mqtt",  # https://pypi.org/project/paho-mqtt/
     "tomlkit",  # https://github.com/sdispater/tomlkit
     "msgspec",  # https://github.com/jcrist/msgspec
     "bx_py_utils",  # https://github.com/boxine/bx_py_utils
     "click",  # https://github.com/pallets/click/
     "rich-click",  # https://github.com/ewels/rich-click
     "rich",  # https://github.com/Textualize/rich
```

### Comparing `ha-services-0.0.1/requirements.dev.txt` & `ha-services-0.1.0/requirements.dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -455,15 +455,15 @@
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
     # via markdown-it-py
 more-itertools==9.1.0 \
     --hash=sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d \
     --hash=sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3
     # via jaraco-classes
-msgspec[toml]==0.14.2 \
+msgspec==0.14.2 \
     --hash=sha256:03ddc8c518afbea4fb89afb587d77f11d00909f003966d437f31fb8fffdfac28 \
     --hash=sha256:1c8f7e631fad9d5a33fcfb0f2a27eb86dc0390e91d6b51c95a604b7ccbc264f1 \
     --hash=sha256:1fc99f0929fa91cc53fa35f59be366d67f116c2b7f0f3b29dc60e3179f6fb205 \
     --hash=sha256:2039451b22813af2fd5cbe99eaecfc318d64fcee5af0ce5b3d5cce12427d24cd \
     --hash=sha256:26bcb3a69b348be2757ab19e86038e586920522a99d49d358c12890fbcfb6aa8 \
     --hash=sha256:3288b65ee7c78d08f32003a8b5ca72fff12c6a7400bd35f9d65630c9d58efce2 \
     --hash=sha256:4f13e47803aedbb32c9375317fedbd20af3397dc024d311eebdc635c07f6f908 \
@@ -754,23 +754,18 @@
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   autopep8
     #   black
     #   build
     #   flynt
     #   ha-services (pyproject.toml)
-    #   msgspec
     #   mypy
     #   pyproject-api
     #   pyproject-hooks
     #   tox
-tomli-w==1.0.0 \
-    --hash=sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463 \
-    --hash=sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9
-    # via msgspec
 tomlkit==0.11.8 \
     --hash=sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171 \
     --hash=sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3
     # via
     #   ha-services (pyproject.toml)
     #   manageprojects
 tox==4.5.1 \
```

