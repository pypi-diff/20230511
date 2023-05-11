# Comparing `tmp/x4i3-1.2.3.tar.gz` & `tmp/x4i3-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x4i3-1.2.3.tar", last modified: Sun Feb  6 03:17:23 2022, max compression
+gzip compressed data, was "x4i3-1.2.4.tar", last modified: Thu May 11 13:18:10 2023, max compression
```

## Comparing `x4i3-1.2.3.tar` & `x4i3-1.2.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-06 03:17:23.215200 x4i3-1.2.3/
--rw-r--r--   0 vsts      (1001) docker     (121)    17228 2022-02-06 03:17:14.000000 x4i3-1.2.3/LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     4981 2022-02-06 03:17:23.215200 x4i3-1.2.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     3938 2022-02-06 03:17:14.000000 x4i3-1.2.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-02-06 03:17:23.215200 x4i3-1.2.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     3694 2022-02-06 03:17:14.000000 x4i3-1.2.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-06 03:17:23.203199 x4i3-1.2.3/x4i3/
--rw-r--r--   0 vsts      (1001) docker     (121)     9701 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11029 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/abundance.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-06 03:17:23.203199 x4i3-1.2.3/x4i3/data/
--rw-r--r--   0 vsts      (1001) docker     (121)      441 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/data/README.data
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-06 03:17:23.211200 x4i3-1.2.3/x4i3/dicts/
--rw-r--r--   0 vsts      (1001) docker     (121)    77210 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict03.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      728 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict04.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    27384 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict05.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    30853 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict07.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     4741 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict09.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1079 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict18.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1379 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict19.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      753 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict20.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     2829 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict21.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1479 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict22.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      885 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict23.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     3025 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict24.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      961 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict30.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1559 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict33.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     5608 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict34.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      328 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict35.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    62306 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict36.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      411 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/dicts/dict37.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     5098 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/endl_Z.py
--rw-r--r--   0 vsts      (1001) docker     (121)    32966 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_column_parsing.py
--rw-r--r--   0 vsts      (1001) docker     (121)    22084 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6537 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_dicts.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16476 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_entry.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5286 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18992 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_field.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6144 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_grammers.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14363 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_manager.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11545 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_particle.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18079 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_reactions.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4850 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13853 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_section.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4815 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_subentry.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5886 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/exfor_utilities.py
--rw-r--r--   0 vsts      (1001) docker     (121)   151698 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/pyparsing2.py
--rw-r--r--   0 vsts      (1001) docker     (121)   272400 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/pyparsing3.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-06 03:17:23.215200 x4i3-1.2.3/x4i3/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)     7927 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/tests/12898.x4
--rw-r--r--   0 vsts      (1001) docker     (121)     2593 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/tests/E0783.x4
--rw-r--r--   0 vsts      (1001) docker     (121)     1351 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5378 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/tests/test_exfor_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (121)    31961 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/tests/test_exfor_entry.py
--rw-r--r--   0 vsts      (1001) docker     (121)    32185 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/tests/test_exfor_fields.py
--rw-r--r--   0 vsts      (1001) docker     (121)   107577 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/tests/test_exfor_full_integration.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17086 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/tests/test_exfor_manager.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10614 2022-02-06 03:17:14.000000 x4i3-1.2.3/x4i3/tests/test_exfor_reaction.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-06 03:17:23.203199 x4i3-1.2.3/x4i3.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     4981 2022-02-06 03:17:23.000000 x4i3-1.2.3/x4i3.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1264 2022-02-06 03:17:23.000000 x4i3-1.2.3/x4i3.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-02-06 03:17:23.000000 x4i3-1.2.3/x4i3.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       30 2022-02-06 03:17:23.000000 x4i3-1.2.3/x4i3.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        5 2022-02-06 03:17:23.000000 x4i3-1.2.3/x4i3.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 13:18:10.449020 x4i3-1.2.4/
+-rw-r--r--   0 vsts      (1001) docker     (123)    17228 2023-05-11 13:17:33.000000 x4i3-1.2.4/LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     4944 2023-05-11 13:18:10.449020 x4i3-1.2.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3938 2023-05-11 13:17:33.000000 x4i3-1.2.4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-11 13:18:10.449020 x4i3-1.2.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3634 2023-05-11 13:17:33.000000 x4i3-1.2.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 13:18:10.441021 x4i3-1.2.4/x4i3/
+-rw-r--r--   0 vsts      (1001) docker     (123)     9894 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11029 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/abundance.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 13:18:10.445021 x4i3-1.2.4/x4i3/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)      597 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/data/README.data
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 13:18:10.445021 x4i3-1.2.4/x4i3/dicts/
+-rw-r--r--   0 vsts      (1001) docker     (123)    77210 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict03.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      728 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict04.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)    27384 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict05.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)    30853 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict07.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     4741 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict09.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1079 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict18.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1379 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict19.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      753 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict20.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     2829 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict21.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1479 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict22.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      885 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict23.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     3025 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict24.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      961 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict30.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1559 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict33.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     5608 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict34.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      328 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict35.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)    62306 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict36.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      411 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/dicts/dict37.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     5098 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/endl_Z.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    32966 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_column_parsing.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    22084 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6537 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_dicts.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16476 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_entry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5286 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18992 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_field.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6144 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_grammers.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14363 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11545 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_particle.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18079 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_reactions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4850 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13853 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_section.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4815 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_subentry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5886 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/exfor_utilities.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   151698 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/pyparsing2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   272400 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/pyparsing3.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 13:18:10.449020 x4i3-1.2.4/x4i3/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7927 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/tests/12898.x4
+-rw-r--r--   0 vsts      (1001) docker     (123)     2593 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/tests/E0783.x4
+-rw-r--r--   0 vsts      (1001) docker     (123)     1351 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5378 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/tests/test_exfor_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    31961 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/tests/test_exfor_entry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    32185 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/tests/test_exfor_fields.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   107577 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/tests/test_exfor_full_integration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17086 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/tests/test_exfor_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10614 2023-05-11 13:17:33.000000 x4i3-1.2.4/x4i3/tests/test_exfor_reaction.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-11 13:18:10.445021 x4i3-1.2.4/x4i3.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4944 2023-05-11 13:18:10.000000 x4i3-1.2.4/x4i3.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1264 2023-05-11 13:18:10.000000 x4i3-1.2.4/x4i3.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-11 13:18:10.000000 x4i3-1.2.4/x4i3.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       30 2023-05-11 13:18:10.000000 x4i3-1.2.4/x4i3.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-11 13:18:10.000000 x4i3-1.2.4/x4i3.egg-info/top_level.txt
```

### Comparing `x4i3-1.2.3/LICENSE.txt` & `x4i3-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/PKG-INFO` & `x4i3-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: x4i3
-Version: 1.2.3
+Version: 1.2.4
 Summary: A "simple" python interface to the EXFOR library
 Home-page: https://github.com/afedynitch/x4i3/
 Author: David A. Brown (x4i3: Anatoli Fedynitch)
 Author-email: dbrown@bnl.gov
 Maintainer: Anatoli Fedynitch
 Maintainer-email: afedynitch@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -82,9 +80,7 @@
 *David A. Brown (LLNL)* (`x4i`)
 
 *Anatoli Fedynitch* (`x4i3`)
 
 ### Copyright and license
 
 This code is distributed under the [GNU General Public License (GPLv2) (see LICENSE)](LICENSE.txt) without any warranty or guaranty. The full disclaimer and license information is located in the [LICENSE](LICENCE.txt). Very unfortunately, the original code is GPLv2 infecting in a nontransparent way all derived works such as this. Be warned!
-
-
```

### Comparing `x4i3-1.2.3/README.md` & `x4i3-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/setup.py` & `x4i3-1.2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,53 +39,49 @@
 # terms and conditions of the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 
 import os
-import setuptools
 from distutils.core import setup
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='x4i3',
-    version='1.2.3',
-    author='David A. Brown (x4i3: Anatoli Fedynitch)',
-    author_email='dbrown@bnl.gov',
-    maintainer='Anatoli Fedynitch',
-    maintainer_email='afedynitch@gmail.com',
-    packages=['x4i3', 'x4i3.tests'],
+    name="x4i3",
+    version="1.2.4",
+    author="David A. Brown (x4i3: Anatoli Fedynitch)",
+    author_email="dbrown@bnl.gov",
+    maintainer="Anatoli Fedynitch",
+    maintainer_email="afedynitch@gmail.com",
+    packages=["x4i3", "x4i3.tests"],
     package_data={
-        'x4i3': [
-            os.path.join('dicts', '*.txt'),
-            os.path.join('data', 'README.data')],
-        'x4i3.tests': [
-            '*.x4',
-            os.path.join('tests','data')]},
-    url='https://github.com/afedynitch/x4i3/',
+        "x4i3": [os.path.join("dicts", "*.txt"), os.path.join("data", "README.data")],
+        "x4i3.tests": ["*.x4", os.path.join("tests", "data")],
+    },
+    url="https://github.com/afedynitch/x4i3/",
     install_requires=[
-        'tqdm',
-        'requests',
+        "tqdm",
+        "requests",
     ],
     extras_require={"tests": ["pytest"]},
     description='A "simple" python interface to the EXFOR library',
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     classifiers=[
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Topic :: Scientific/Engineering :: Physics',
-        'Intended Audience :: Science/Research',
-        'Development Status :: 4 - Beta',
-        'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
-    ]
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Scientific/Engineering :: Physics",
+        "Intended Audience :: Science/Research",
+        "Development Status :: 4 - Beta",
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+    ],
 )
```

### Comparing `x4i3-1.2.3/x4i3/__init__.py` & `x4i3-1.2.4/x4i3/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,26 +44,26 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 
 # General info
 from __future__ import print_function
 import os
 import sys
+import pathlib
 
 MAJOR_VERSION = 1
-MINOR_VERSION = 1
-PATCH = 0
+MINOR_VERSION = 2
+PATCH = 4
 
 __package_name__ = "x4i3 -- The Exfor Interface"
-__version__ = '.'.join(map(str, [MAJOR_VERSION, MINOR_VERSION, PATCH]))
-__author__ = 'David Brown <brown170@llnl.gov>, Anatoli Fedynitch <afedynitch@gmail.com>'
-__url__ = 'https://github.com/afedynitch/x4i3'
-__license__ = 'GPLv2'
-__disclaimer__ = \
-    """LLNL Disclaimer:
+__version__ = ".".join(map(str, [MAJOR_VERSION, MINOR_VERSION, PATCH]))
+__author__ = "David Brown <brown170@llnl.gov>, Anatoli Fedynitch <afedynitch@gmail.com>"
+__url__ = "https://github.com/afedynitch/x4i3"
+__license__ = "GPLv2"
+__disclaimer__ = """LLNL Disclaimer:
   This work was prepared as an account of work sponsored by an agency of the
   United States Government. Neither the United States Government nor the
   University of California nor any of their employees, makes any warranty,
   express or implied, or assumes any liability or responsibility for the
   accuracy, completeness, or usefulness of any information, apparatus, product,
   or process disclosed, or represents that its use would not infringe
   privately-owned rights.  Reference herein to any specific commercial products,
@@ -71,44 +71,60 @@
   not necessarily constitute or imply its endorsement, recommendation, or
   favoring by the United States Government or the University of California. The
   views and opinions of authors expressed herein do not necessarily state or
   reflect those of the United States Government or the University of California,
   and shall not be used for advertising or product endorsement purposes."""
 
 # Common filenames
-indexFileName = 'index.tbl'
-errorFileName = 'error-entries.pickle'
-coupledFileName = 'coupled-entries.pickle'
-monitoredFileName = 'monitored-entries.pickle'
-reactionCountFileName = 'reaction-count.pickle'
-dbPath = 'db'
+indexFileName = "index.tbl"
+errorFileName = "error-entries.pickle"
+coupledFileName = "coupled-entries.pickle"
+monitoredFileName = "monitored-entries.pickle"
+reactionCountFileName = "reaction-count.pickle"
+dbPath = "db"
 
 # URL to the compressed database files on github
-url='https://github.com/afedynitch/x4i3/releases/download/last_before_pep8_formatting/x4i3_X4-2021-03-08.tar.gz'
+url = "https://github.com/afedynitch/x4i3/releases/download/last_before_pep8_formatting/x4i3_X4-2023-04-29.tar.gz"
 # url='https://github.com/afedynitch/x4i3/releases/download/last_before_pep8_formatting/x4i3_EXFOR-2016-04-01.tar.gz'
 
-# Paths for standard usage
-if 'X43I_DATAPATH' in os.environ:
-    DATAPATH = os.environ['X43I_DATAPATH']
+if "X43I_DATAPATH" in os.environ:
+    DATAPATH = pathlib.Path(os.environ["X43I_DATAPATH"])
+    if not DATAPATH.exists():
+        raise FileNotFoundError(
+            f"X43I_DATAPATH={DATAPATH} does not exist. Please point this variable"
+            + " to the x4i3_EXFOR-20XX-XX-XX directory created by unpacking"
+            + " masterfiles with x4i3_tools."
+        )
+    tags = list(DATAPATH.glob("X4-20*"))
+    if len(tags) == 0:
+        raise FileNotFoundError(
+            f"No tag file in the format 'X4-20XX-XX-XX' found in {DATAPATH}"
+        )
+    else:
+        dbTagFile = DATAPATH / tags[0]
 else:
-    DATAPATH = os.path.abspath(os.path.join(__path__[0], 'data'))
+    # Follow default path
+    DATAPATH = pathlib.Path(__path__[0], "data").absolute()
+    dbTagFile = DATAPATH / pathlib.Path(url).stem[:-4]
 
-fullIndexFileName = os.path.join(DATAPATH, indexFileName)
-fullErrorFileName = os.path.join(DATAPATH, errorFileName)
-fullCoupledFileName = os.path.join(DATAPATH, coupledFileName)
-fullMonitoredFileName = os.path.join(DATAPATH, monitoredFileName)
-fullReactionCountFileName = os.path.join(DATAPATH, reactionCountFileName)
-fullDBPath = os.path.join(DATAPATH, dbPath)
-dbTagFile = os.path.join(DATAPATH, 
-    os.path.splitext(os.path.splitext(os.path.split(url)[1])[0])[0][5:])
+
+fullIndexFileName = DATAPATH / indexFileName
+fullErrorFileName = DATAPATH / errorFileName
+fullCoupledFileName = DATAPATH / coupledFileName
+fullMonitoredFileName = DATAPATH / monitoredFileName
+fullReactionCountFileName = DATAPATH / reactionCountFileName
+fullDBPath = DATAPATH / dbPath
+
+print(f"Using database version {dbTagFile.stem} located in: {DATAPATH}")
 
 # Paths for unit testing only
-TESTDATAPATH = os.path.abspath(os.path.join(__path__[0], 'tests', 'data'))  # Mock db for testing
-testDBPath = os.path.join(TESTDATAPATH, dbPath)
-testIndexFileName = os.path.join(TESTDATAPATH, indexFileName)
+# Mock db for testing
+TESTDATAPATH = pathlib.Path(__path__[0], "tests", "data").absolute()
+testDBPath = TESTDATAPATH / "db"
+testIndexFileName = TESTDATAPATH / indexFileName
 
 
 def _download_and_unpack_file(url):
     """Downloads the database files created with setup-exfor-db.py as
     a tarball and unpacks them to the correct folder."""
 
     from tqdm import tqdm
@@ -117,90 +133,115 @@
     import math
     import tarfile
     import tempfile
     import shutil
 
     # cleanup
     for f in [
-        fullIndexFileName, fullErrorFileName,
-        fullCoupledFileName, fullMonitoredFileName,
-        fullReactionCountFileName, fullDBPath, dbTagFile
+        fullIndexFileName,
+        fullErrorFileName,
+        fullCoupledFileName,
+        fullMonitoredFileName,
+        fullReactionCountFileName,
+        fullDBPath,
+        dbTagFile,
     ]:
         try:
             shutil.rmtree(f)
         except NotADirectoryError:
             os.remove(f)
         except FileNotFoundError:
             pass
     # Tag files:
-    tag_files = [
-        f for tag in ['X4-*', 'EXFOR-*'] for f in glob(os.path.join(DATAPATH, tag))
-        ]
-    for tagfile in tag_files:
+    
+    for tagfile in DATAPATH.glob("X4-*"):
         try:
             os.remove(tagfile)
         except FileNotFoundError:
             pass
-        
 
     # Streaming, so we can iterate over the response.
     r = requests.get(url, stream=True)
     tarname = os.path.basename(url)
 
     # Total size in bytes.
-    total_size = int(r.headers.get('content-length', 0))
+    total_size = int(r.headers.get("content-length", 0))
     block_size = 1024 * 1024
     wrote = 0
     tempfile = tempfile.TemporaryFile()
-    
-    print('Downloading data file', tarname)
-    for data in tqdm(r.iter_content(block_size), total=math.ceil(total_size // block_size),
-                    unit='MB', unit_scale=True):
+
+    print("Downloading data file", tarname)
+    for data in tqdm(
+        r.iter_content(block_size),
+        total=math.ceil(total_size // block_size),
+        unit="MB",
+        unit_scale=True,
+    ):
         wrote = wrote + len(data)
         tempfile.write(data)
     if total_size != 0 and wrote != total_size:
         raise Exception("ERROR, something went wrong")
     tempfile.flush()
     tempfile.seek(0)
-    print('Decompressing archive', tarname)
-    wrote = 0
-    with tarfile.open(fileobj=tempfile, mode='r') as _tar:
+    print("Decompressing archive", tarname)
+    with tarfile.open(fileobj=tempfile, mode="r") as _tar:
         total = len(_tar.getmembers())
         for member in tqdm(_tar.getmembers(), total=total):
-            wrote = wrote + len(data)
             _tar.extract(member, DATAPATH)
     tempfile.close()
 
-    with open(dbTagFile,'wb') as f:
-        print('Installed database version', dbTagFile)
+    with open(dbTagFile, "wb") as f:
+        print("Installed database version", dbTagFile.stem)
         pass
 
+
 def check_if_exists(path, return_bool=False):
     if return_bool:
         if not os.path.exists(path):
             return False
         else:
-            return True    
+            return True
     if not os.path.exists(path):
-        raise IOError('File/Directory', path, 'not found. Check installation.')
+        raise IOError("File/Directory", path, "not found. Check installation.")
+
 
 # Don't download an unpack the files if the module is just tested
 if "pytest" not in sys.modules:
     # Check if all files can be located and redownload the archive
-    if not all([check_if_exists(p, return_bool=True) for p in [
-        DATAPATH, fullIndexFileName, fullErrorFileName,
-        fullCoupledFileName, fullMonitoredFileName,
-        fullReactionCountFileName, fullDBPath, dbTagFile]]):
+    if not all(
+        [
+            check_if_exists(p, return_bool=True)
+            for p in [
+                DATAPATH,
+                fullIndexFileName,
+                fullErrorFileName,
+                fullCoupledFileName,
+                fullMonitoredFileName,
+                fullReactionCountFileName,
+                fullDBPath,
+                dbTagFile,
+            ]
+        ]
+    ):
         _download_and_unpack_file(url)
 
     # Check if all files can be located and raise exception if still not there
-    _ = [check_if_exists(p) for p in [
-        DATAPATH, fullIndexFileName, fullErrorFileName,
-        fullCoupledFileName, fullMonitoredFileName,
-        fullReactionCountFileName, fullDBPath, dbTagFile]]
+    _ = [
+        check_if_exists(p)
+        for p in [
+            DATAPATH,
+            fullIndexFileName,
+            fullErrorFileName,
+            fullCoupledFileName,
+            fullMonitoredFileName,
+            fullReactionCountFileName,
+            fullDBPath,
+            dbTagFile,
+        ]
+    ]
 
 # Applications that query multiple entries subsequently using an in-memory
 # dictionary that contains all .x4 files from the db folder can improve performance
 
 
 class DataBaseCache(dict):
     """Reads all .x4 files from db folder and strres them
@@ -208,45 +249,40 @@
 
     def __init__(self):
         self.__initialized = False
 
     def __load_cache(self):
         for sd in os.listdir(fullDBPath):
             for x4f in os.listdir(os.path.join(fullDBPath, sd)):
-                k = sd + '/' + x4f
-                dict.__setitem__(self, k, open(os.path.join(
-                    fullDBPath, sd, x4f), 'rb').readlines())
+                k = sd + "/" + x4f
+                dict.__setitem__(
+                    self, k, open(os.path.join(fullDBPath, sd, x4f), "rb").readlines()
+                )
         self.__initialized = True
 
     def __getitem__(self, key):
         if not self.__initialized:
             self.__load_cache()
         return dict.__getitem__(self, key)
 
 
 # Does lazy initialization, only loads x4 files into memory on access
 database_dict = DataBaseCache()
 
-# The stuff below is not well placed here, bad practice, and will be removed soon.
-# from x4i3 import exfor_manager, exfor_entry
-
-# __databaseManager = exfor_manager.X4DBManagerDefault()
-
-# def query(**kw): return __databaseManager.query(**kw)
-
-
-# def raw_retrieve(**kw): return __databaseManager.retrieve(**kw)
-
-
-# def retrieve(**kw):
-#     rr = {}
-#     r = __databaseManager.retrieve(**kw)
-#     for k, v in r.items():
-#         rr[k] = exfor_entry.X4Entry(v)
-#     return rr
-
-
 __all__ = [
-    '__init__', 'exfor_dataset', 'exfor_exceptions', 'exfor_manager', 'exfor_reference',
-    'exfor_utilities', 'endl_Z', 'exfor_dicts', 'exfor_field', 'exfor_particle', 'exfor_section',
-    'exfor_column_parsing', 'exfor_entry', 'exfor_grammers', 'exfor_reactions', 'exfor_subentry'
+    "__init__",
+    "exfor_dataset",
+    "exfor_exceptions",
+    "exfor_manager",
+    "exfor_reference",
+    "exfor_utilities",
+    "endl_Z",
+    "exfor_dicts",
+    "exfor_field",
+    "exfor_particle",
+    "exfor_section",
+    "exfor_column_parsing",
+    "exfor_entry",
+    "exfor_grammers",
+    "exfor_reactions",
+    "exfor_subentry",
 ]
```

### Comparing `x4i3-1.2.3/x4i3/abundance.py` & `x4i3-1.2.4/x4i3/abundance.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict03.txt` & `x4i3-1.2.4/x4i3/dicts/dict03.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict04.txt` & `x4i3-1.2.4/x4i3/dicts/dict04.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict05.txt` & `x4i3-1.2.4/x4i3/dicts/dict05.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict07.txt` & `x4i3-1.2.4/x4i3/dicts/dict07.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict09.txt` & `x4i3-1.2.4/x4i3/dicts/dict09.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict18.txt` & `x4i3-1.2.4/x4i3/dicts/dict18.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict19.txt` & `x4i3-1.2.4/x4i3/dicts/dict19.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict20.txt` & `x4i3-1.2.4/x4i3/dicts/dict20.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict21.txt` & `x4i3-1.2.4/x4i3/dicts/dict21.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict22.txt` & `x4i3-1.2.4/x4i3/dicts/dict22.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict23.txt` & `x4i3-1.2.4/x4i3/dicts/dict23.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict24.txt` & `x4i3-1.2.4/x4i3/dicts/dict24.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict30.txt` & `x4i3-1.2.4/x4i3/dicts/dict30.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict33.txt` & `x4i3-1.2.4/x4i3/dicts/dict33.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict34.txt` & `x4i3-1.2.4/x4i3/dicts/dict34.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/dicts/dict36.txt` & `x4i3-1.2.4/x4i3/dicts/dict36.txt`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/endl_Z.py` & `x4i3-1.2.4/x4i3/endl_Z.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_column_parsing.py` & `x4i3-1.2.4/x4i3/exfor_column_parsing.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_dataset.py` & `x4i3-1.2.4/x4i3/exfor_dataset.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_dicts.py` & `x4i3-1.2.4/x4i3/exfor_dicts.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_entry.py` & `x4i3-1.2.4/x4i3/exfor_entry.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_exceptions.py` & `x4i3-1.2.4/x4i3/exfor_exceptions.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_field.py` & `x4i3-1.2.4/x4i3/exfor_field.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_grammers.py` & `x4i3-1.2.4/x4i3/exfor_grammers.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_manager.py` & `x4i3-1.2.4/x4i3/exfor_manager.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_particle.py` & `x4i3-1.2.4/x4i3/exfor_particle.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_reactions.py` & `x4i3-1.2.4/x4i3/exfor_reactions.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_reference.py` & `x4i3-1.2.4/x4i3/exfor_reference.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_section.py` & `x4i3-1.2.4/x4i3/exfor_section.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_subentry.py` & `x4i3-1.2.4/x4i3/exfor_subentry.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/exfor_utilities.py` & `x4i3-1.2.4/x4i3/exfor_utilities.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/pyparsing2.py` & `x4i3-1.2.4/x4i3/pyparsing2.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/pyparsing3.py` & `x4i3-1.2.4/x4i3/pyparsing3.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/tests/12898.x4` & `x4i3-1.2.4/x4i3/tests/12898.x4`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/tests/E0783.x4` & `x4i3-1.2.4/x4i3/tests/E0783.x4`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/tests/__init__.py` & `x4i3-1.2.4/x4i3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/tests/test_exfor_dataset.py` & `x4i3-1.2.4/x4i3/tests/test_exfor_dataset.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/tests/test_exfor_entry.py` & `x4i3-1.2.4/x4i3/tests/test_exfor_entry.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/tests/test_exfor_fields.py` & `x4i3-1.2.4/x4i3/tests/test_exfor_fields.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/tests/test_exfor_full_integration.py` & `x4i3-1.2.4/x4i3/tests/test_exfor_full_integration.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/tests/test_exfor_manager.py` & `x4i3-1.2.4/x4i3/tests/test_exfor_manager.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3/tests/test_exfor_reaction.py` & `x4i3-1.2.4/x4i3/tests/test_exfor_reaction.py`

 * *Files identical despite different names*

### Comparing `x4i3-1.2.3/x4i3.egg-info/PKG-INFO` & `x4i3-1.2.4/x4i3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: x4i3
-Version: 1.2.3
+Version: 1.2.4
 Summary: A "simple" python interface to the EXFOR library
 Home-page: https://github.com/afedynitch/x4i3/
 Author: David A. Brown (x4i3: Anatoli Fedynitch)
 Author-email: dbrown@bnl.gov
 Maintainer: Anatoli Fedynitch
 Maintainer-email: afedynitch@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -82,9 +80,7 @@
 *David A. Brown (LLNL)* (`x4i`)
 
 *Anatoli Fedynitch* (`x4i3`)
 
 ### Copyright and license
 
 This code is distributed under the [GNU General Public License (GPLv2) (see LICENSE)](LICENSE.txt) without any warranty or guaranty. The full disclaimer and license information is located in the [LICENSE](LICENCE.txt). Very unfortunately, the original code is GPLv2 infecting in a nontransparent way all derived works such as this. Be warned!
-
-
```

### Comparing `x4i3-1.2.3/x4i3.egg-info/SOURCES.txt` & `x4i3-1.2.4/x4i3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

