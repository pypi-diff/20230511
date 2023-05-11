# Comparing `tmp/pythonsdk-0.6.0.tar.gz` & `tmp/pythonsdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsdk-0.6.0.tar", last modified: Mon May  8 09:45:08 2023, max compression
+gzip compressed data, was "pythonsdk-0.7.0.tar", last modified: Thu May 11 20:06:27 2023, max compression
```

## Comparing `pythonsdk-0.6.0.tar` & `pythonsdk-0.7.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.424361 pythonsdk-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.424361 pythonsdk-0.6.0/src/python_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.424361 pythonsdk-0.6.0/src/python_sdk/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/_cli/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/_cli/_fmt.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/_cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/bin/_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config_value_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config_value_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_optional_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_string_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/encoding/_base64url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/log/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_log.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_log_levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_rotating_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_stderr.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/src/python_sdk/sentinel/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/sentinel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/sentinel/_sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/src/python_sdk/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/testing/_prepackaged_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/src/python_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_zipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 09:45:02.000000 pythonsdk-0.6.0/src/python_sdk/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/src/python_sdk/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/versioning/_version_file_based.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/src/pythonsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-08 09:45:08.000000 pythonsdk-0.6.0/src/pythonsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-08 09:45:08.000000 pythonsdk-0.6.0/src/pythonsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:45:08.000000 pythonsdk-0.6.0/src/pythonsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 09:45:08.000000 pythonsdk-0.6.0/src/pythonsdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-08 09:45:08.000000 pythonsdk-0.6.0/src/pythonsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 09:45:08.000000 pythonsdk-0.6.0/src/pythonsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.784914 pythonsdk-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-11 20:06:27.784914 pythonsdk-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:06:27.784914 pythonsdk-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.768914 pythonsdk-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.768914 pythonsdk-0.7.0/src/python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.772914 pythonsdk-0.7.0/src/python_sdk/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/_cli/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/_cli/_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/_cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.772914 pythonsdk-0.7.0/src/python_sdk/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/bin/_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.776914 pythonsdk-0.7.0/src/python_sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/config/_config_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/config/_config_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/config/_config_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/config/_config_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/config/_config_value_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/config/_config_value_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/config/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/config/_optional_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/config/_string_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.776914 pythonsdk-0.7.0/src/python_sdk/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/encoding/_base64url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.776914 pythonsdk-0.7.0/src/python_sdk/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.776914 pythonsdk-0.7.0/src/python_sdk/log/_logging_formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_logging_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_logging_formatter/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_logging_formatter/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.780914 pythonsdk-0.7.0/src/python_sdk/log/_logging_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_logging_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_logging_handler/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_logging_handler/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_logging_handler/_rotating_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_logging_handler/_stderr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/log/_logging_handler/_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.780914 pythonsdk-0.7.0/src/python_sdk/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/secrets/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.780914 pythonsdk-0.7.0/src/python_sdk/secrets/_secrets_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/secrets/_secrets_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/secrets/_secrets_engine/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/secrets/_secrets_engine/_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.780914 pythonsdk-0.7.0/src/python_sdk/sentinel/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/sentinel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/sentinel/_sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.780914 pythonsdk-0.7.0/src/python_sdk/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/testing/_prepackaged_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.784914 pythonsdk-0.7.0/src/python_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/utils/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/utils/_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/utils/_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/utils/_file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/utils/_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/utils/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/utils/_zipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 20:06:21.000000 pythonsdk-0.7.0/src/python_sdk/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.784914 pythonsdk-0.7.0/src/python_sdk/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/src/python_sdk/versioning/_version_file_based.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:06:27.784914 pythonsdk-0.7.0/src/pythonsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-11 20:06:27.000000 pythonsdk-0.7.0/src/pythonsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-11 20:06:27.000000 pythonsdk-0.7.0/src/pythonsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:06:27.000000 pythonsdk-0.7.0/src/pythonsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 20:06:27.000000 pythonsdk-0.7.0/src/pythonsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-11 20:06:27.000000 pythonsdk-0.7.0/src/pythonsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 20:06:27.000000 pythonsdk-0.7.0/src/pythonsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 20:05:52.000000 pythonsdk-0.7.0/version
```

### Comparing `pythonsdk-0.6.0/LICENSE` & `pythonsdk-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/PKG-INFO` & `pythonsdk-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonsdk
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python Software Dev Kit
 Author-email: lijok <lijok@pm.me>
 License: MIT License
         
         Copyright (c) 2023 Lijok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pythonsdk-0.6.0/pyproject.toml` & `pythonsdk-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/_cli/_cli.py` & `pythonsdk-0.7.0/src/python_sdk/_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/_cli/_fmt.py` & `pythonsdk-0.7.0/src/python_sdk/_cli/_fmt.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/bin/_call.py` & `pythonsdk-0.7.0/src/python_sdk/bin/_call.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/config/__init__.py` & `pythonsdk-0.7.0/src/python_sdk/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,9 +18,10 @@
 from python_sdk.config._config_value_validators import ConfigValueValidator as ConfigValueValidator
 from python_sdk.config._config_value_validators import ValidateDirectoryExists as ValidateDirectoryExists
 from python_sdk.config._config_value_validators import ValidateFileExists as ValidateFileExists
 from python_sdk.config._config_value_validators import ValidateFileType as ValidateFileType
 from python_sdk.config._config_value_validators import ValidatePathIsExecutable as ValidatePathIsExecutable
 from python_sdk.config._config_value_validators import ValidatePathIsReadable as ValidatePathIsReadable
 from python_sdk.config._config_value_validators import ValidatePathIsWritable as ValidatePathIsWritable
+from python_sdk.config._config_value_validators import ValidateRegexMatch as ValidateRegexMatch
 from python_sdk.config._flags import disable_on_access_config_reloading as disable_on_access_config_reloading
 from python_sdk.config._flags import enable_on_access_config_reloading as enable_on_access_config_reloading
```

### Comparing `pythonsdk-0.6.0/src/python_sdk/config/_config.py` & `pythonsdk-0.7.0/src/python_sdk/config/_config.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/config/_config_option.py` & `pythonsdk-0.7.0/src/python_sdk/config/_config_option.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/config/_config_sources.py` & `pythonsdk-0.7.0/src/python_sdk/config/_config_sources.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/config/_config_value_types.py` & `pythonsdk-0.7.0/src/python_sdk/config/_config_value_types.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/config/_config_value_validators.py` & `pythonsdk-0.7.0/src/python_sdk/config/_config_value_validators.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import pathlib
+import re
 import typing
 
 if typing.TYPE_CHECKING:
     from python_sdk.config import _config_option
 
 
 class ConfigValueValidationError(Exception):
@@ -126,14 +127,16 @@
             raise ConfigValueValidationError(f"{config_value} is not executable")
 
 
 class ValidateFileType:
     name: str = "Validate File Type"
     description: str = "Validates that the file at a given path is of set file type."
 
+    file_type: str
+
     def __init__(self, file_type: str) -> None:
         self.file_type = file_type if file_type[0] == "." else f".{file_type}"
 
     def __call__(
         self,
         config_option_name: str,
         config_option: "_config_option.ConfigOption",
@@ -141,7 +144,35 @@
     ) -> None:
         """
         Raises:
             ConfigValueValidationError: Path is not of correct file type.
         """
         if "".join(config_value.suffixes) != self.file_type:
             raise ConfigValueValidationError(f"{config_value} is not {self.file_type}")
+
+
+class ValidateRegexMatch:
+    name: str = "Validate Regex Match"
+    description: str = """
+    Validates that the passed value(s) match a regex pattern.
+    This can be used with strings and lists of strings.
+    """
+
+    pattern: re.Pattern
+
+    def __init__(self, pattern: str) -> None:
+        self.pattern = re.compile(pattern=pattern)
+
+    def __call__(
+        self,
+        config_option_name: str,
+        config_option: "_config_option.ConfigOption",
+        config_value: str | list[str],
+    ) -> None:
+        """
+        Raises:
+            ConfigValueValidationError: Value does not match regex pattern.
+        """
+        values_to_validate = config_value if isinstance(config_value, list) else [config_value]
+        for value in values_to_validate:
+            if not self.pattern.match(value):
+                raise ConfigValueValidationError(f"Value does not match regex pattern {self.pattern.pattern}")
```

### Comparing `pythonsdk-0.6.0/src/python_sdk/config/_flags.py` & `pythonsdk-0.7.0/src/python_sdk/config/_flags.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/config/_string_decoder.py` & `pythonsdk-0.7.0/src/python_sdk/config/_string_decoder.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/encoding/_base64url.py` & `pythonsdk-0.7.0/src/python_sdk/encoding/_base64url.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/log/__init__.py` & `pythonsdk-0.7.0/src/python_sdk/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/log/_base.py` & `pythonsdk-0.7.0/src/python_sdk/log/_base.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/log/_config.py` & `pythonsdk-0.7.0/src/python_sdk/log/_config.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/log/_context.py` & `pythonsdk-0.7.0/src/python_sdk/log/_context.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/log/_log.py` & `pythonsdk-0.7.0/src/python_sdk/log/_log.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/log/_logger.py` & `pythonsdk-0.7.0/src/python_sdk/log/_logger.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_factory.py` & `pythonsdk-0.7.0/src/python_sdk/log/_logging_formatter/_factory.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_protocol.py` & `pythonsdk-0.7.0/src/python_sdk/log/_logging_formatter/_protocol.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py` & `pythonsdk-0.7.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py` & `pythonsdk-0.7.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_factory.py` & `pythonsdk-0.7.0/src/python_sdk/log/_logging_handler/_factory.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_rotating_file.py` & `pythonsdk-0.7.0/src/python_sdk/log/_logging_handler/_rotating_file.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/secrets/__init__.py` & `pythonsdk-0.7.0/src/python_sdk/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/secrets/_config.py` & `pythonsdk-0.7.0/src/python_sdk/secrets/_config.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py` & `pythonsdk-0.7.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py` & `pythonsdk-0.7.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py` & `pythonsdk-0.7.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_factory.py` & `pythonsdk-0.7.0/src/python_sdk/secrets/_secrets_engine/_factory.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_protocol.py` & `pythonsdk-0.7.0/src/python_sdk/secrets/_secrets_engine/_protocol.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/sentinel/_sentinel.py` & `pythonsdk-0.7.0/src/python_sdk/sentinel/_sentinel.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/testing/_prepackaged_tests.py` & `pythonsdk-0.7.0/src/python_sdk/testing/_prepackaged_tests.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/utils/__init__.py` & `pythonsdk-0.7.0/src/python_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/utils/_file_watcher.py` & `pythonsdk-0.7.0/src/python_sdk/utils/_file_watcher.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/utils/_zipfile.py` & `pythonsdk-0.7.0/src/python_sdk/utils/_zipfile.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/python_sdk/versioning/_version_file_based.py` & `pythonsdk-0.7.0/src/python_sdk/versioning/_version_file_based.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.6.0/src/pythonsdk.egg-info/PKG-INFO` & `pythonsdk-0.7.0/src/pythonsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonsdk
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python Software Dev Kit
 Author-email: lijok <lijok@pm.me>
 License: MIT License
         
         Copyright (c) 2023 Lijok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pythonsdk-0.6.0/src/pythonsdk.egg-info/SOURCES.txt` & `pythonsdk-0.7.0/src/pythonsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

