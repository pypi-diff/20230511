# Comparing `tmp/pyreason-1.3.0.tar.gz` & `tmp/pyreason-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.3.0.tar", last modified: Fri Apr 14 12:16:43 2023, max compression
+gzip compressed data, was "pyreason-1.4.0.tar", last modified: Thu May 11 06:08:46 2023, max compression
```

## Comparing `pyreason-1.3.0.tar` & `pyreason-1.4.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.054364 pyreason-1.3.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-04-14 12:16:29.000000 pyreason-1.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 12:16:29.000000 pyreason-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-14 12:16:43.054364 pyreason-1.3.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-04-14 12:16:29.000000 pyreason-1.3.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.046363 pyreason-1.3.0/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    21896 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4649 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/facts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    65031 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10162 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.054364 pyreason-1.3.0/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1793 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.054364 pyreason-1.3.0/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.054364 pyreason-1.3.0/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3346 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-14 12:16:43.000000 pyreason-1.3.0/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-14 12:16:43.000000 pyreason-1.3.0/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:16:43.000000 pyreason-1.3.0/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 12:16:43.000000 pyreason-1.3.0/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 12:16:43.000000 pyreason-1.3.0/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:16:43.054364 pyreason-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-14 12:16:29.000000 pyreason-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.135618 pyreason-1.4.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-05-11 06:08:27.000000 pyreason-1.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-11 06:08:27.000000 pyreason-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-11 06:08:46.135618 pyreason-1.4.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-05-11 06:08:27.000000 pyreason-1.4.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.119618 pyreason-1.4.0/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.123618 pyreason-1.4.0/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.123618 pyreason-1.4.0/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26093 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.127618 pyreason-1.4.0/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.127618 pyreason-1.4.0/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.127618 pyreason-1.4.0/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4649 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.127618 pyreason-1.4.0/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/facts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.127618 pyreason-1.4.0/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    65031 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.131618 pyreason-1.4.0/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.131618 pyreason-1.4.0/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.131618 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10162 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.131618 pyreason-1.4.0/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1793 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.135618 pyreason-1.4.0/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.135618 pyreason-1.4.0/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3346 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.123618 pyreason-1.4.0/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-11 06:08:46.000000 pyreason-1.4.0/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-11 06:08:46.000000 pyreason-1.4.0/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 06:08:46.000000 pyreason-1.4.0/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 06:08:46.000000 pyreason-1.4.0/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 06:08:46.000000 pyreason-1.4.0/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 06:08:46.135618 pyreason-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-11 06:08:27.000000 pyreason-1.4.0/setup.py
```

### Comparing `pyreason-1.3.0/LICENSE.md` & `pyreason-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/PKG-INFO` & `pyreason-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.3.0
+Version: 1.4.0
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.3.0/README.md` & `pyreason-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/__init__.py` & `pyreason-1.4.0/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.4.0/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.4.0/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.4.0/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/pyreason.py` & `pyreason-1.4.0/pyreason/pyreason.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This is the file that will be imported when "import pyreason" is called. All content will be run automatically
 import numba
 import time
 import sys
 import warnings
+import numpy as np
 import memory_profiler as mp
 from typing import List, Type
 
 from pyreason.scripts.utils.output import Output
 from pyreason.scripts.utils.filter import Filter
 from pyreason.scripts.program.program import Program
-from pyreason.scripts.interpretation.interpretation import Interpretation
 from pyreason.scripts.utils.graphml_parser import GraphmlParser
 import pyreason.scripts.utils.yaml_parser as yaml_parser
 import pyreason.scripts.numba_wrapper.numba_types.label_type as label
+import pyreason.scripts.numba_wrapper.numba_types.rule_type as rule
 import pyreason.scripts.numba_wrapper.numba_types.fact_node_type as fact_node
 import pyreason.scripts.numba_wrapper.numba_types.fact_edge_type as fact_edge
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
 
 
-
 # USER VARIABLES
 class _Settings:
     def __init__(self):
         self.__verbose = True
         self.__output_to_file = False
         self.__output_file_name = 'pyreason_output'
         self.__graph_attribute_parsing = True
@@ -278,14 +278,15 @@
         :raises TypeError: If not bool raise error
         """
         if not isinstance(value, bool):
             raise TypeError('value has to be a bool')
         else:
             self.__static_graph_facts = value
 
+
 # VARIABLES
 __graph = None
 __rules = None
 __node_facts = None
 __edge_facts = None
 __ipl = None
 __node_labels = None
@@ -330,39 +331,145 @@
     """Load labels from YAML file path into program
 
     :param path: Path for the YAML labels file
     """
     global __node_labels, __edge_labels, __specific_node_labels, __specific_edge_labels
     __node_labels, __edge_labels, __specific_node_labels, __specific_edge_labels = yaml_parser.parse_labels(path)
 
+
 def load_facts(path: str) -> None:
     """Load facts from YAML file path into program
 
     :param path: Path for the YAML facts file
     """
     global __node_facts, __edge_facts, settings
     __node_facts, __edge_facts = yaml_parser.parse_facts(path, settings.reverse_digraph)
 
+
 def load_rules(path: str) -> None:
     """Load rules from YAML file path into program
 
     :param path: Path for the YAML rules file
     """
     global __rules
-    __rules = yaml_parser.parse_rules(path)
+
+    if __rules is None:
+        __rules = yaml_parser.parse_rules(path)
+    else:
+        __rules.extend(yaml_parser.parse_rules(path))
+
 
 def load_inconsistent_predicate_list(path: str) -> None:
     """Load IPL from YAML file path into program
 
     :param path: Path for the YAML IPL file
     """
     global __ipl
     __ipl = yaml_parser.parse_ipl(path)
 
 
+def add_rules_from_text(rule_text: str, name: str) -> None:
+    """Add a rule to pyreason from text format. This format is not as modular as the YAML format.
+    1. It is not possible to specify target criteria
+    2. It is not possible to specify delta_t. delta_t=0 by default.
+    3. It is not possible to specify thresholds. Threshold is greater than or equal to 1 by default
+    4. It is not possible to add edges between subsets of nodes
+    5. It is not possible to have an annotation function. We set to [1,1] by default
+    6. It is not possible to have weights for different clauses. Weights are 1 by default with bias 0
+
+    Example:
+    `'pred1(x,y) <- pred2(a, b), pred3(b, c)'`
+
+    :param rule_text: The rule in text format
+    :param name: The name of the rule. This will appear in the rule trace
+    """
+    global __rules
+
+    # First remove all spaces from line
+    r = rule_text.replace(' ', '')
+
+    # Separate into head and body
+    head, body = r.split('<-')
+
+    # Separate clauses in body
+    body = body[:-1].replace(')', '))') + ')'
+    body = body.split('),')
+
+    # Find the target predicate
+    idx = head.find('(')
+    target = head[:idx]
+    target = label.Label(target)
+
+    # Variable(s) in the head of the rule
+    head_variables = head[idx + 1:-1].split(',')
+
+    # Target criteria is empty for this text format to pyreason rule
+    target_criteria = numba.typed.List.empty_list(numba.types.Tuple((label.label_type, interval.interval_type)))
+
+    # Get the variables in the body
+    body_predicates = []
+    body_variables = []
+    for clause in body:
+        idx = clause.find('(')
+        body_predicates.append(clause[:idx])
+        body_variables.append(clause[idx+1:-1].split(','))
+
+    # Replace the variables in the body with source/target if they match the variables in the head
+    head_var_map = {0: 'source', 1: 'target'}
+    for i in range(len(body_variables)):
+        for j in range(len(body_variables[i])):
+            # Loop through the head variables and see if there's a match
+            for k in range(len(head_variables)):
+                if body_variables[i][j] == head_variables[k]:
+                    body_variables[i][j] = head_var_map[k] if len(head_variables) == 2 else 'target'
+
+    # Start setting up neigh_criteria
+    # neigh_criteria = [c1, c2, c3, c4]
+    # thresholds = [t1, t2, t3, t4]
+
+    # Array of thresholds to keep track of for each neighbor criterion. Form [(comparison, (number/percent, total/available), thresh)]
+    thresholds = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.UniTuple(numba.types.string, 2), numba.types.float64)))
+
+    # Array to store clauses for nodes: node/edge, [subset]/[subset1, subset2], label, interval
+    neigh_criteria = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.UniTuple(numba.types.string, 2), label.label_type, interval.interval_type)))
+
+    # Loop though clauses
+    for predicate, variables in zip(body_predicates, body_variables):
+        # Neigh criteria
+        clause_type = 'node' if len(variables) == 1 else 'edge'
+        subset = (variables[0], variables[0]) if clause_type == 'node' else (variables[0], variables[1])
+        l = label.Label(predicate)
+        bnd = interval.closed(1, 1)
+        neigh_criteria.append((clause_type, subset, l, bnd))
+
+        # Threshold
+        quantifier = 'greater_equal'
+        quantifier_type = ('number', 'total')
+        thresh = 1
+        thresholds.append((quantifier, quantifier_type, thresh))
+
+    # Cannot add edges
+    edges = ('', '', label.Label(''))
+
+    # Bound to set atom if rule fires
+    bnd = interval.closed(1, 1)
+    ann_fn = ''
+    ann_label = label.Label('')
+
+    weights = np.ones(len(body_predicates), dtype=np.float64)
+    weights = np.append(weights, 0)
+
+    r = rule.Rule(name, target, target_criteria, numba.types.int8(0), neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges)
+
+    # Add to collection of rules
+    if __rules is None:
+        __rules = numba.typed.List.empty_list(rule.rule_type)
+    __rules.append(r)
+
+
 def reason(timesteps: int=-1, convergence_threshold: int=-1, convergence_bound_threshold: float=-1, again: bool=False, node_facts: List[Type[fact_node.Fact]]=None, edge_facts: List[Type[fact_edge.Fact]]=None, include_graph_facts: bool=True):
     """Function to start the main reasoning process. Graph and rules must already be loaded.
 
     :param timesteps: Max number of timesteps to run. -1 specifies run till convergence, defaults to -1
     :param convergence_threshold: Maximim number of interpretations that have changed between timesteps or fixed point operations until considered convergent. Program will end at convergence. -1 => no changes, perfect convergence, defaults to -1
     :param convergence_bound_threshold: Maximum change in any interpretation (bounds) between timesteps or fixed point operations until considered convergent, defaults to -1
     :param again: Whether to reason again on an existing interpretation, defaults to False
@@ -429,15 +536,14 @@
         __edge_facts = numba.typed.List.empty_list(fact_edge.fact_type)
 
     if __ipl is None:
         if settings.verbose:
             warnings.warn('Inconsistent Predicate List yaml file has not been loaded. Use `load_ipl`. Loading IPL is optional\n')
         __ipl = numba.typed.List.empty_list(numba.types.Tuple((label.label_type, label.label_type)))
 
-    
     # If graph attribute parsing, add results to existing specific labels and facts
     for label_name, nodes in __specific_graph_node_labels.items():
         if label_name in __specific_node_labels:
             __specific_node_labels[label_name].extend(nodes)
         else:
             __specific_node_labels[label_name] = nodes
```

### Comparing `pyreason-1.3.0/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.4.0/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/args.py` & `pyreason-1.4.0/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/components/world.py` & `pyreason-1.4.0/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/diffuse.py` & `pyreason-1.4.0/pyreason/scripts/diffuse.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,25 +67,25 @@
     facts_node += non_fluent_facts_node
     facts_edge += non_fluent_facts_edge
 
     # Inconsistent predicate list
     ipl = yaml_parser.parse_ipl(args.ipl_yaml_path)
 
     # Program comes here
-    program = Program(graph, tmax, facts_node, facts_edge, rules, ipl, args.reverse_digraph, args.atom_trace, args.save_graph_attributes_to_trace, args.canonical, args.inconsistency_check)
+    program = Program(graph, facts_node, facts_edge, rules, ipl, args.reverse_digraph, args.atom_trace, args.save_graph_attributes_to_trace, args.canonical, args.inconsistency_check)
     program.available_labels_node = node_labels
     program.available_labels_edge = edge_labels
     program.specific_node_labels = specific_node_labels
     program.specific_edge_labels = specific_edge_labels
 
     # Reasoning process
     print('Graph loaded successfully, rules, labels, facts and ipl parsed successfully')
     print('Starting diffusion')
     start = time.time()
-    interpretation = program.reason(args.convergence_threshold, args.convergence_bound_threshold)
+    interpretation = program.reason(tmax, args.convergence_threshold, args.convergence_bound_threshold)
     end = time.time()
     print('Time to complete diffusion:', end-start)
     print('Finished diffusion')
 
     # Save the rule trace to a file
     output = Output(timestamp)
     output.save_rule_trace(interpretation, folder='./output')
```

### Comparing `pyreason-1.3.0/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.4.0/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/facts/fact_node.py` & `pyreason-1.4.0/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.4.0/pyreason/scripts/interpretation/interpretation.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/interval/interval.py` & `pyreason-1.4.0/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/program/program.py` & `pyreason-1.4.0/pyreason/scripts/program/program.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/rules/rule.py` & `pyreason-1.4.0/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/utils/filter.py` & `pyreason-1.4.0/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.4.0/pyreason/scripts/utils/graphml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/utils/output.py` & `pyreason-1.4.0/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/utils/plotter.py` & `pyreason-1.4.0/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/utils/visuals.py` & `pyreason-1.4.0/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.4.0/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/pyreason.egg-info/PKG-INFO` & `pyreason-1.4.0/pyreason.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.3.0
+Version: 1.4.0
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.3.0/pyreason.egg-info/SOURCES.txt` & `pyreason-1.4.0/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.3.0/setup.py` & `pyreason-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name = 'pyreason',
-    version = '1.3.0',
+    version = '1.4.0',
     author = 'Dyuman Aditya',
     author_email = 'dyuman.aditya@gmail.com',
     description = 'An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/lab-v2/pyreason',
     license = 'BSD 3-clause',
```

