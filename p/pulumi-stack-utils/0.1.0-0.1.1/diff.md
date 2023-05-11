# Comparing `tmp/pulumi-stack-utils-0.1.0.tar.gz` & `tmp/pulumi-stack-utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi-stack-utils-0.1.0.tar", last modified: Thu May 11 16:55:34 2023, max compression
+gzip compressed data, was "pulumi-stack-utils-0.1.1.tar", last modified: Thu May 11 18:07:52 2023, max compression
```

## Comparing `pulumi-stack-utils-0.1.0.tar` & `pulumi-stack-utils-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:55:34.584724 pulumi-stack-utils-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-11 16:55:10.000000 pulumi-stack-utils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-11 16:55:34.584724 pulumi-stack-utils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-11 16:55:10.000000 pulumi-stack-utils-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:55:34.584724 pulumi-stack-utils-0.1.0/pulumi_stack_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 16:55:10.000000 pulumi-stack-utils-0.1.0/pulumi_stack_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:55:34.584724 pulumi-stack-utils-0.1.0/pulumi_stack_utils/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:55:10.000000 pulumi-stack-utils-0.1.0/pulumi_stack_utils/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-11 16:55:10.000000 pulumi-stack-utils-0.1.0/pulumi_stack_utils/aws/autotag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-11 16:55:10.000000 pulumi-stack-utils-0.1.0/pulumi_stack_utils/stack_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:55:34.584724 pulumi-stack-utils-0.1.0/pulumi_stack_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-11 16:55:34.000000 pulumi-stack-utils-0.1.0/pulumi_stack_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-11 16:55:34.000000 pulumi-stack-utils-0.1.0/pulumi_stack_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:55:34.000000 pulumi-stack-utils-0.1.0/pulumi_stack_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 16:55:34.000000 pulumi-stack-utils-0.1.0/pulumi_stack_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 16:55:34.000000 pulumi-stack-utils-0.1.0/pulumi_stack_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-11 16:55:10.000000 pulumi-stack-utils-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:55:34.584724 pulumi-stack-utils-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:55:34.584724 pulumi-stack-utils-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-11 16:55:10.000000 pulumi-stack-utils-0.1.0/test/test_stack_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:07:52.888652 pulumi-stack-utils-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-11 18:07:35.000000 pulumi-stack-utils-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-11 18:07:52.888652 pulumi-stack-utils-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-11 18:07:35.000000 pulumi-stack-utils-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:07:52.888652 pulumi-stack-utils-0.1.1/pulumi_stack_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 18:07:35.000000 pulumi-stack-utils-0.1.1/pulumi_stack_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:07:52.888652 pulumi-stack-utils-0.1.1/pulumi_stack_utils/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:07:35.000000 pulumi-stack-utils-0.1.1/pulumi_stack_utils/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-11 18:07:35.000000 pulumi-stack-utils-0.1.1/pulumi_stack_utils/aws/autotag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-11 18:07:35.000000 pulumi-stack-utils-0.1.1/pulumi_stack_utils/stack_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:07:52.888652 pulumi-stack-utils-0.1.1/pulumi_stack_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-11 18:07:52.000000 pulumi-stack-utils-0.1.1/pulumi_stack_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-11 18:07:52.000000 pulumi-stack-utils-0.1.1/pulumi_stack_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:07:52.000000 pulumi-stack-utils-0.1.1/pulumi_stack_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 18:07:52.000000 pulumi-stack-utils-0.1.1/pulumi_stack_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 18:07:52.000000 pulumi-stack-utils-0.1.1/pulumi_stack_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-11 18:07:35.000000 pulumi-stack-utils-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:07:52.888652 pulumi-stack-utils-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:07:52.888652 pulumi-stack-utils-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-11 18:07:35.000000 pulumi-stack-utils-0.1.1/test/test_stack_reference.py
```

### Comparing `pulumi-stack-utils-0.1.0/LICENSE` & `pulumi-stack-utils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pulumi-stack-utils-0.1.0/pulumi_stack_utils/aws/autotag.py` & `pulumi-stack-utils-0.1.1/pulumi_stack_utils/aws/autotag.py`

 * *Files identical despite different names*

### Comparing `pulumi-stack-utils-0.1.0/pulumi_stack_utils/stack_reference.py` & `pulumi-stack-utils-0.1.1/pulumi_stack_utils/stack_reference.py`

 * *Files identical despite different names*

### Comparing `pulumi-stack-utils-0.1.0/pyproject.toml` & `pulumi-stack-utils-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "pulumi-stack-utils"
 description = "Utilities for working with Pulumi stacks"
 readme = "README.md"
 license = { text = "BSD-2-Clause" }
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name="James Arnold", email="james@rs21.io" }
 ]
 dependencies = [
     "boto3",
     "pulumi",
     "pyyaml",
```

### Comparing `pulumi-stack-utils-0.1.0/test/test_stack_reference.py` & `pulumi-stack-utils-0.1.1/test/test_stack_reference.py`

 * *Files identical despite different names*

