# Comparing `tmp/cdk-sops-secrets-1.2.91.tar.gz` & `tmp/cdk-sops-secrets-1.2.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-sops-secrets-1.2.91.tar", last modified: Thu May 11 01:10:08 2023, max compression
+gzip compressed data, was "cdk-sops-secrets-1.2.92.tar", last modified: Thu May 11 21:49:25 2023, max compression
```

## Comparing `cdk-sops-secrets-1.2.91.tar` & `cdk-sops-secrets-1.2.92.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:10:08.106614 cdk-sops-secrets-1.2.91/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-11 01:09:56.000000 cdk-sops-secrets-1.2.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 01:09:56.000000 cdk-sops-secrets-1.2.91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-11 01:10:08.106614 cdk-sops-secrets-1.2.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-05-11 01:09:56.000000 cdk-sops-secrets-1.2.91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-11 01:09:56.000000 cdk-sops-secrets-1.2.91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 01:10:08.106614 cdk-sops-secrets-1.2.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-11 01:09:56.000000 cdk-sops-secrets-1.2.91/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:10:08.098614 cdk-sops-secrets-1.2.91/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:10:08.098614 cdk-sops-secrets-1.2.91/src/cdk_sops_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)    76168 2023-05-11 01:09:56.000000 cdk-sops-secrets-1.2.91/src/cdk_sops_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:10:08.102614 cdk-sops-secrets-1.2.91/src/cdk_sops_secrets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-11 01:09:56.000000 cdk-sops-secrets-1.2.91/src/cdk_sops_secrets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  7059427 2023-05-11 01:09:56.000000 cdk-sops-secrets-1.2.91/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.2.91.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 01:09:56.000000 cdk-sops-secrets-1.2.91/src/cdk_sops_secrets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:10:08.102614 cdk-sops-secrets-1.2.91/src/cdk_sops_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-11 01:10:08.000000 cdk-sops-secrets-1.2.91/src/cdk_sops_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-11 01:10:08.000000 cdk-sops-secrets-1.2.91/src/cdk_sops_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 01:10:08.000000 cdk-sops-secrets-1.2.91/src/cdk_sops_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 01:10:08.000000 cdk-sops-secrets-1.2.91/src/cdk_sops_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 01:10:08.000000 cdk-sops-secrets-1.2.91/src/cdk_sops_secrets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:49:25.010129 cdk-sops-secrets-1.2.92/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-11 21:49:13.000000 cdk-sops-secrets-1.2.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 21:49:13.000000 cdk-sops-secrets-1.2.92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-11 21:49:25.006129 cdk-sops-secrets-1.2.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-05-11 21:49:13.000000 cdk-sops-secrets-1.2.92/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-11 21:49:13.000000 cdk-sops-secrets-1.2.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 21:49:25.010129 cdk-sops-secrets-1.2.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-11 21:49:13.000000 cdk-sops-secrets-1.2.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:49:24.998129 cdk-sops-secrets-1.2.92/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:49:25.002129 cdk-sops-secrets-1.2.92/src/cdk_sops_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)    76168 2023-05-11 21:49:13.000000 cdk-sops-secrets-1.2.92/src/cdk_sops_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:49:25.002129 cdk-sops-secrets-1.2.92/src/cdk_sops_secrets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-11 21:49:13.000000 cdk-sops-secrets-1.2.92/src/cdk_sops_secrets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7060084 2023-05-11 21:49:13.000000 cdk-sops-secrets-1.2.92/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.2.92.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:49:13.000000 cdk-sops-secrets-1.2.92/src/cdk_sops_secrets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:49:25.002129 cdk-sops-secrets-1.2.92/src/cdk_sops_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-11 21:49:24.000000 cdk-sops-secrets-1.2.92/src/cdk_sops_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-11 21:49:24.000000 cdk-sops-secrets-1.2.92/src/cdk_sops_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:49:24.000000 cdk-sops-secrets-1.2.92/src/cdk_sops_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 21:49:24.000000 cdk-sops-secrets-1.2.92/src/cdk_sops_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 21:49:24.000000 cdk-sops-secrets-1.2.92/src/cdk_sops_secrets.egg-info/top_level.txt
```

### Comparing `cdk-sops-secrets-1.2.91/LICENSE` & `cdk-sops-secrets-1.2.92/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.2.91/PKG-INFO` & `cdk-sops-secrets-1.2.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.2.91
+Version: 1.2.92
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<dev@markussiebert.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/markussiebert/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-sops-secrets-1.2.91/README.md` & `cdk-sops-secrets-1.2.92/README.md`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.2.91/setup.py` & `cdk-sops-secrets-1.2.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-sops-secrets",
-    "version": "1.2.91",
+    "version": "1.2.92",
     "description": "CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.",
     "license": "Apache-2.0",
     "url": "https://constructs.dev/packages/cdk-sops-secrets",
     "long_description_content_type": "text/markdown",
     "author": "Markus Siebert<dev@markussiebert.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_sops_secrets",
         "cdk_sops_secrets._jsii"
     ],
     "package_data": {
         "cdk_sops_secrets._jsii": [
-            "cdk-sops-secrets@1.2.91.jsii.tgz"
+            "cdk-sops-secrets@1.2.92.jsii.tgz"
         ],
         "cdk_sops_secrets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-sops-secrets-1.2.91/src/cdk_sops_secrets/__init__.py` & `cdk-sops-secrets-1.2.92/src/cdk_sops_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.2.91/src/cdk_sops_secrets.egg-info/PKG-INFO` & `cdk-sops-secrets-1.2.92/src/cdk_sops_secrets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.2.91
+Version: 1.2.92
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<dev@markussiebert.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/markussiebert/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

