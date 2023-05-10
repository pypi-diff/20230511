# Comparing `tmp/aws-cdk.cdk-assets-schema-1.98.0.tar.gz` & `tmp/aws-cdk.cdk-assets-schema-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src518022412/src/packages/@aws-cdk/cdk-assets-schema/dist/python/aws-cdk.cdk-assets-schema-1.98.0.tar", last modified: Mon Apr 12 10:09:50 2021, max compression
+gzip compressed data, was "/codebuild/output/src875002972/src/packages/@aws-cdk/cdk-assets-schema/dist/python/aws-cdk.cdk-assets-schema-1.99.0.tar", last modified: Tue Apr 13 17:03:50 2021, max compression
```

## Comparing `aws-cdk.cdk-assets-schema-1.98.0.tar` & `aws-cdk.cdk-assets-schema-1.99.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/
--rw-r--r--   0 root         (0) root         (0)       23 2021-04-12 10:07:21.000000 aws-cdk.cdk-assets-schema-1.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1005 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       52 2021-04-12 10:07:21.000000 aws-cdk.cdk-assets-schema-1.98.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-04-12 10:07:21.000000 aws-cdk.cdk-assets-schema-1.98.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1601 2021-04-12 10:07:21.000000 aws-cdk.cdk-assets-schema-1.98.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/src/aws_cdk/cdk_assets_schema/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/src/aws_cdk/cdk_assets_schema/_jsii/
--rw-r--r--   0 root         (0) root         (0)      345 2021-04-12 10:07:21.000000 aws-cdk.cdk-assets-schema-1.98.0/src/aws_cdk/cdk_assets_schema/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6165 2021-04-12 10:07:20.000000 aws-cdk.cdk-assets-schema-1.98.0/src/aws_cdk/cdk_assets_schema/_jsii/cdk-assets-schema@1.98.0.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/src/aws_cdk.cdk_assets_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1005 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/src/aws_cdk.cdk_assets_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      427 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/src/aws_cdk.cdk_assets_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/src/aws_cdk.cdk_assets_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/src/aws_cdk.cdk_assets_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-04-12 10:09:50.000000 aws-cdk.cdk-assets-schema-1.98.0/src/aws_cdk.cdk_assets_schema.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:50.000000 aws-cdk.cdk-assets-schema-1.99.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2021-04-13 17:02:04.000000 aws-cdk.cdk-assets-schema-1.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-04-13 17:02:04.000000 aws-cdk.cdk-assets-schema-1.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2021-04-13 17:02:04.000000 aws-cdk.cdk-assets-schema-1.99.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1005 2021-04-13 17:03:50.000000 aws-cdk.cdk-assets-schema-1.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       52 2021-04-13 17:02:04.000000 aws-cdk.cdk-assets-schema-1.99.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-04-13 17:02:04.000000 aws-cdk.cdk-assets-schema-1.99.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-04-13 17:03:50.000000 aws-cdk.cdk-assets-schema-1.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1601 2021-04-13 17:02:04.000000 aws-cdk.cdk-assets-schema-1.99.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:50.000000 aws-cdk.cdk-assets-schema-1.99.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:50.000000 aws-cdk.cdk-assets-schema-1.99.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:50.000000 aws-cdk.cdk-assets-schema-1.99.0/src/aws_cdk/cdk_assets_schema/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:50.000000 aws-cdk.cdk-assets-schema-1.99.0/src/aws_cdk/cdk_assets_schema/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      345 2021-04-13 17:02:04.000000 aws-cdk.cdk-assets-schema-1.99.0/src/aws_cdk/cdk_assets_schema/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6164 2021-04-13 17:02:03.000000 aws-cdk.cdk-assets-schema-1.99.0/src/aws_cdk/cdk_assets_schema/_jsii/cdk-assets-schema@1.99.0.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:50.000000 aws-cdk.cdk-assets-schema-1.99.0/src/aws_cdk.cdk_assets_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1005 2021-04-13 17:03:49.000000 aws-cdk.cdk-assets-schema-1.99.0/src/aws_cdk.cdk_assets_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      442 2021-04-13 17:03:50.000000 aws-cdk.cdk-assets-schema-1.99.0/src/aws_cdk.cdk_assets_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:03:49.000000 aws-cdk.cdk-assets-schema-1.99.0/src/aws_cdk.cdk_assets_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2021-04-13 17:03:49.000000 aws-cdk.cdk-assets-schema-1.99.0/src/aws_cdk.cdk_assets_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2021-04-13 17:03:49.000000 aws-cdk.cdk-assets-schema-1.99.0/src/aws_cdk.cdk_assets_schema.egg-info/top_level.txt
```

### Comparing `aws-cdk.cdk-assets-schema-1.98.0/PKG-INFO` & `aws-cdk.cdk-assets-schema-1.99.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cdk-assets-schema
-Version: 1.98.0
+Version: 1.99.0
 Summary: Schema definition for the Asset Manifest
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: aws-cdk.cdk-assets-schema
         =========================
```

### Comparing `aws-cdk.cdk-assets-schema-1.98.0/setup.py` & `aws-cdk.cdk-assets-schema-1.99.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.cdk-assets-schema",
-    "version": "1.98.0",
+    "version": "1.99.0",
     "description": "Schema definition for the Asset Manifest",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -21,20 +21,20 @@
         "": "src"
     },
     "packages": [
         "aws_cdk.cdk_assets_schema._jsii"
     ],
     "package_data": {
         "aws_cdk.cdk_assets_schema._jsii": [
-            "cdk-assets-schema@1.98.0.jsii.tgz"
+            "cdk-assets-schema@1.99.0.jsii.tgz"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "jsii>=1.27.0, <2.0.0",
+        "jsii>=1.28.0, <2.0.0",
         "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `aws-cdk.cdk-assets-schema-1.98.0/src/aws_cdk.cdk_assets_schema.egg-info/PKG-INFO` & `aws-cdk.cdk-assets-schema-1.99.0/src/aws_cdk.cdk_assets_schema.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cdk-assets-schema
-Version: 1.98.0
+Version: 1.99.0
 Summary: Schema definition for the Asset Manifest
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: aws-cdk.cdk-assets-schema
         =========================
```

