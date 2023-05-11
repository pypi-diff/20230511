# Comparing `tmp/pyreason-1.4.0.tar.gz` & `tmp/pyreason-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.4.0.tar", last modified: Thu May 11 06:08:46 2023, max compression
+gzip compressed data, was "pyreason-1.4.1.tar", last modified: Thu May 11 15:52:00 2023, max compression
```

## Comparing `pyreason-1.4.0.tar` & `pyreason-1.4.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.135618 pyreason-1.4.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-05-11 06:08:27.000000 pyreason-1.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-11 06:08:27.000000 pyreason-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-11 06:08:46.135618 pyreason-1.4.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-05-11 06:08:27.000000 pyreason-1.4.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.119618 pyreason-1.4.0/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.123618 pyreason-1.4.0/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.123618 pyreason-1.4.0/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    26093 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.127618 pyreason-1.4.0/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.127618 pyreason-1.4.0/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.127618 pyreason-1.4.0/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4649 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.127618 pyreason-1.4.0/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/facts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.127618 pyreason-1.4.0/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    65031 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.131618 pyreason-1.4.0/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.131618 pyreason-1.4.0/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.131618 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10162 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.131618 pyreason-1.4.0/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1793 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.135618 pyreason-1.4.0/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.135618 pyreason-1.4.0/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3346 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-11 06:08:27.000000 pyreason-1.4.0/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:08:46.123618 pyreason-1.4.0/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-11 06:08:46.000000 pyreason-1.4.0/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-11 06:08:46.000000 pyreason-1.4.0/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 06:08:46.000000 pyreason-1.4.0/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 06:08:46.000000 pyreason-1.4.0/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 06:08:46.000000 pyreason-1.4.0/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 06:08:46.135618 pyreason-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-11 06:08:27.000000 pyreason-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-05-11 15:51:46.000000 pyreason-1.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-11 15:51:46.000000 pyreason-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-11 15:52:00.485568 pyreason-1.4.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-05-11 15:51:46.000000 pyreason-1.4.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27250 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/facts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    65031 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10162 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1793 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-11 15:52:00.000000 pyreason-1.4.1/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-11 15:52:00.000000 pyreason-1.4.1/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:52:00.000000 pyreason-1.4.1/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 15:52:00.000000 pyreason-1.4.1/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 15:52:00.000000 pyreason-1.4.1/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:52:00.485568 pyreason-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-11 15:51:46.000000 pyreason-1.4.1/setup.py
```

### Comparing `pyreason-1.4.0/LICENSE.md` & `pyreason-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/PKG-INFO` & `pyreason-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.4.0
+Version: 1.4.1
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.4.0/README.md` & `pyreason-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/__init__.py` & `pyreason-1.4.1/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.4.1/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.4.1/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.4.1/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/pyreason.py` & `pyreason-1.4.1/pyreason/pyreason.py`

 * *Files 4% similar despite different names*

```diff
@@ -607,20 +607,35 @@
     """
     global __timestamp
 
     output = Output(__timestamp)
     output.save_rule_trace(interpretation, folder)
 
 
-def filter_and_sort(interpretation, labels: List[str], bound: interval.Interval=interval.closed(0,1), sort_by: str='lower', descending: bool=True):
-    """Filters and sorts the interpretation and returns as a list of Pandas dataframes that are easy to access
+def filter_and_sort_nodes(interpretation, labels: List[str], bound: interval.Interval=interval.closed(0,1), sort_by: str='lower', descending: bool=True):
+    """Filters and sorts the node changes in the interpretation and returns as a list of Pandas dataframes that are easy to access
 
     :param interpretation: the output of `pyreason.reason()`, the final interpretation
     :param labels: A list of strings, labels that are in the interpretation that are to be filtered
     :param bound: The bound that will filter any interpretation that is not in it. the default does not filter anything, defaults to interval.closed(0,1)
     :param sort_by: String that is either 'lower' or 'upper', sorts by the lower/upper bound, defaults to 'lower'
     :param descending: A bool that sorts by descending/ascending order, defaults to True
     :return: A list of Pandas dataframes that contain the filtered and sorted interpretations that are easy to access
     """
     filterer = Filter(interpretation.time)
-    filtered_df = filterer.filter_and_sort(interpretation, labels, bound, sort_by, descending)
+    filtered_df = filterer.filter_and_sort_nodes(interpretation, labels, bound, sort_by, descending)
+    return filtered_df
+
+
+def filter_and_sort_edges(interpretation, labels: List[str], bound: interval.Interval=interval.closed(0,1), sort_by: str='lower', descending: bool=True):
+    """Filters and sorts the edge changes in the interpretation and returns as a list of Pandas dataframes that are easy to access
+
+    :param interpretation: the output of `pyreason.reason()`, the final interpretation
+    :param labels: A list of strings, labels that are in the interpretation that are to be filtered
+    :param bound: The bound that will filter any interpretation that is not in it. the default does not filter anything, defaults to interval.closed(0,1)
+    :param sort_by: String that is either 'lower' or 'upper', sorts by the lower/upper bound, defaults to 'lower'
+    :param descending: A bool that sorts by descending/ascending order, defaults to True
+    :return: A list of Pandas dataframes that contain the filtered and sorted interpretations that are easy to access
+    """
+    filterer = Filter(interpretation.time)
+    filtered_df = filterer.filter_and_sort_edges(interpretation, labels, bound, sort_by, descending)
     return filtered_df
```

### Comparing `pyreason-1.4.0/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.4.1/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/args.py` & `pyreason-1.4.1/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/components/world.py` & `pyreason-1.4.1/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/diffuse.py` & `pyreason-1.4.1/pyreason/scripts/diffuse.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     # Save the rule trace to a file
     output = Output(timestamp)
     output.save_rule_trace(interpretation, folder='./output')
 
     # This is how you filter the dataframe to show only nodes that have success in a certain interval
     print('Filtering data...')
     filterer = Filter(interpretation.time)
-    filtered_df = filterer.filter_and_sort(interpretation, labels=args.filter_labels, bound=interval.closed(0, 1), sort_by=args.filter_sort_by, descending=args.descending)
+    filtered_df = filterer.filter_and_sort_nodes(interpretation, labels=args.filter_labels, bound=interval.closed(0, 1), sort_by=args.filter_sort_by, descending=args.descending)
 
     # You can index into filtered_df to get a particular timestep
     # This is for each timestep
     for t in range(interpretation.time+1):
         print(f'\n TIMESTEP - {t}')
         print(filtered_df[t])
         print()
```

### Comparing `pyreason-1.4.0/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.4.1/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/facts/fact_node.py` & `pyreason-1.4.1/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.4.1/pyreason/scripts/interpretation/interpretation.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/interval/interval.py` & `pyreason-1.4.1/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/program/program.py` & `pyreason-1.4.1/pyreason/scripts/program/program.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/rules/rule.py` & `pyreason-1.4.1/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/utils/filter.py` & `pyreason-1.4.1/pyreason/scripts/utils/filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,115 @@
 import pandas as pd
 
-import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
-
 
 class Filter:
     def __init__(self, tmax):
-        self.tmax = tmax 
+        self.tmax = tmax
 
-    def filter_by_bound(self, interpretation, label, bound):
+    def filter_and_sort_nodes(self, interpretation, labels, bound, sort_by='lower', descending=True):
         # Make use of rule trace in interpretation object to efficiently filter through data.
+        
         # Initialize nested dict
         df = {}
         nodes = []
+        latest_changes = {}
         for t in range(self.tmax+1):
             df[t] = {}
-            nodes.append({'component':[], label:[]})
+            nodes.append({})
+            latest_changes[t] = {}
 
         # change contains the timestep, fp operation, component, label and interval
+        # Keep only the latest/most recent changes. Since list is sequencial, whatever was earlier will be overwritten
         for change in interpretation.rule_trace_node:
             t, fp, comp, l, bnd = change
+            latest_changes[t][(comp, l)] = bnd
+        
+        # Create a list that needs to be sorted. This contains only the latest changes
+        list_to_be_sorted = []
+        for t, d in latest_changes.items():
+            for (comp, l), bnd in d.items():
+                list_to_be_sorted.append((bnd, t, comp, l))
+
+        # Sort the list
+        reverse = True if descending else False
+        if sort_by == 'lower':
+            list_to_be_sorted.sort(key=lambda x: x[0].lower, reverse=reverse)
+        elif sort_by == 'upper':
+            list_to_be_sorted.sort(key=lambda x: x[0].upper, reverse=reverse)
+
+        # Add sorted elements to df
+        for i in list_to_be_sorted:
+            bnd, t, comp, l = i
             df[t][(comp, l)] = bnd
 
         for t, d in df.items():
             for (comp, l), bnd in d.items():
-                if l.get_value()==label and bnd in bound:
-                    nodes[t]['component'].append(comp)
-                    nodes[t][label].append(bnd)
+                if l.get_value() in labels and bnd in bound:
+                    if comp not in nodes[t]:
+                        nodes[t][comp] = {lab:[0,1] for lab in labels}
+                    nodes[t][comp][l.get_value()] = [bnd.lower, bnd.upper]
 
         dataframes = []
         for t in range(self.tmax+1):
-            dataframes.append(pd.DataFrame.from_dict(nodes[t]))
+            dataframe = pd.DataFrame.from_dict(nodes[t]).transpose()
+            dataframe = dataframe.reset_index()
+            if not dataframe.empty:
+                dataframe.columns = ['component', *labels]
+            else:
+                dataframe = pd.DataFrame(columns=['component', *labels])
+            dataframes.append(dataframe)
         return dataframes
 
-    def filter_and_sort(self, interpretation, labels, bound, sort_by='lower', descending=True):
+    def filter_and_sort_edges(self, interpretation, labels, bound, sort_by='lower', descending=True):
         # Make use of rule trace in interpretation object to efficiently filter through data.
-        
+
         # Initialize nested dict
         df = {}
-        nodes = []
+        edges = []
         latest_changes = {}
         for t in range(self.tmax+1):
             df[t] = {}
-            nodes.append({})
+            edges.append({})
             latest_changes[t] = {}
 
         # change contains the timestep, fp operation, component, label and interval
-        # Keep only the latest/most recent changes. Since list is sequencial, whatever was earlier will be overwritten
-        for change in interpretation.rule_trace_node:
+        # Keep only the latest/most recent changes. Since list is sequential, whatever was earlier will be overwritten
+        for change in interpretation.rule_trace_edge:
             t, fp, comp, l, bnd = change
             latest_changes[t][(comp, l)] = bnd
-        
+
         # Create a list that needs to be sorted. This contains only the latest changes
         list_to_be_sorted = []
         for t, d in latest_changes.items():
             for (comp, l), bnd in d.items():
                 list_to_be_sorted.append((bnd, t, comp, l))
 
         # Sort the list
         reverse = True if descending else False
-        if sort_by=='lower':
+        if sort_by == 'lower':
             list_to_be_sorted.sort(key=lambda x: x[0].lower, reverse=reverse)
-        elif sort_by=='upper':
+        elif sort_by == 'upper':
             list_to_be_sorted.sort(key=lambda x: x[0].upper, reverse=reverse)
 
         # Add sorted elements to df
         for i in list_to_be_sorted:
             bnd, t, comp, l = i
             df[t][(comp, l)] = bnd
 
         for t, d in df.items():
             for (comp, l), bnd in d.items():
                 if l.get_value() in labels and bnd in bound:
-                    if comp not in nodes[t]:
-                        nodes[t][comp] = {lab:[0,1] for lab in labels}
-                    nodes[t][comp][l.get_value()] = [bnd.lower, bnd.upper]
-
+                    if comp not in edges[t]:
+                        edges[t][comp] = {lab: [0, 1] for lab in labels}
+                    edges[t][comp][l.get_value()] = [bnd.lower, bnd.upper]
 
         dataframes = []
         for t in range(self.tmax+1):
-            dataframe = pd.DataFrame.from_dict(nodes[t]).transpose()
+            dataframe = pd.DataFrame.from_dict(edges[t]).transpose()
             dataframe = dataframe.reset_index()
             if not dataframe.empty:
                 dataframe.columns = ['component', *labels]
             else:
                 dataframe = pd.DataFrame(columns=['component', *labels])
             dataframes.append(dataframe)
         return dataframes
+
```

### Comparing `pyreason-1.4.0/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.4.1/pyreason/scripts/utils/graphml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/utils/output.py` & `pyreason-1.4.1/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/utils/plotter.py` & `pyreason-1.4.1/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/utils/visuals.py` & `pyreason-1.4.1/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.4.1/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/pyreason.egg-info/PKG-INFO` & `pyreason-1.4.1/pyreason.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.4.0
+Version: 1.4.1
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.4.0/pyreason.egg-info/SOURCES.txt` & `pyreason-1.4.1/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.0/setup.py` & `pyreason-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name = 'pyreason',
-    version = '1.4.0',
+    version = '1.4.1',
     author = 'Dyuman Aditya',
     author_email = 'dyuman.aditya@gmail.com',
     description = 'An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/lab-v2/pyreason',
     license = 'BSD 3-clause',
```

