# Comparing `tmp/aws-cdk.aws-dms-1.98.0.tar.gz` & `tmp/aws-cdk.aws-dms-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src518022412/src/packages/@aws-cdk/aws-dms/dist/python/aws-cdk.aws-dms-1.98.0.tar", last modified: Mon Apr 12 10:08:49 2021, max compression
+gzip compressed data, was "/codebuild/output/src875002972/src/packages/@aws-cdk/aws-dms/dist/python/aws-cdk.aws-dms-1.99.0.tar", last modified: Tue Apr 13 17:03:06 2021, max compression
```

## Comparing `aws-cdk.aws-dms-1.98.0.tar` & `aws-cdk.aws-dms-1.99.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/
--rw-r--r--   0 root         (0) root         (0)       23 2021-04-12 10:07:21.000000 aws-cdk.aws-dms-1.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1533 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2021-04-12 10:07:21.000000 aws-cdk.aws-dms-1.98.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-04-12 10:07:21.000000 aws-cdk.aws-dms-1.98.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1715 2021-04-12 10:07:21.000000 aws-cdk.aws-dms-1.98.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk/aws_dms/
--rw-r--r--   0 root         (0) root         (0)   195517 2021-04-12 10:07:21.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk/aws_dms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk/aws_dms/_jsii/
--rw-r--r--   0 root         (0) root         (0)      363 2021-04-12 10:07:21.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk/aws_dms/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68295 2021-04-12 10:07:20.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk/aws_dms/_jsii/aws-dms@1.98.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:07:21.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk/aws_dms/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk.aws_dms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1533 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk.aws_dms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      408 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk.aws_dms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk.aws_dms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk.aws_dms.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-04-12 10:08:49.000000 aws-cdk.aws-dms-1.98.0/src/aws_cdk.aws_dms.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:06.000000 aws-cdk.aws-dms-1.99.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2021-04-13 17:02:04.000000 aws-cdk.aws-dms-1.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-04-13 17:02:04.000000 aws-cdk.aws-dms-1.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2021-04-13 17:02:04.000000 aws-cdk.aws-dms-1.99.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1533 2021-04-13 17:03:06.000000 aws-cdk.aws-dms-1.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2021-04-13 17:02:04.000000 aws-cdk.aws-dms-1.99.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-04-13 17:02:04.000000 aws-cdk.aws-dms-1.99.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-04-13 17:03:06.000000 aws-cdk.aws-dms-1.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1715 2021-04-13 17:02:04.000000 aws-cdk.aws-dms-1.99.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:06.000000 aws-cdk.aws-dms-1.99.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:06.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:06.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk/aws_dms/
+-rw-r--r--   0 root         (0) root         (0)   195517 2021-04-13 17:02:04.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk/aws_dms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:06.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk/aws_dms/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      363 2021-04-13 17:02:04.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk/aws_dms/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68295 2021-04-13 17:02:03.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk/aws_dms/_jsii/aws-dms@1.99.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:02:04.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk/aws_dms/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:06.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk.aws_dms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1533 2021-04-13 17:03:05.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk.aws_dms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      423 2021-04-13 17:03:05.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk.aws_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:03:05.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk.aws_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2021-04-13 17:03:05.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk.aws_dms.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2021-04-13 17:03:05.000000 aws-cdk.aws-dms-1.99.0/src/aws_cdk.aws_dms.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-dms-1.98.0/PKG-INFO` & `aws-cdk.aws-dms-1.99.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-dms
-Version: 1.98.0
+Version: 1.99.0
 Summary: The CDK Construct Library for AWS::DMS
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # AWS Database Migration Service Construct Library
```

### Comparing `aws-cdk.aws-dms-1.98.0/setup.py` & `aws-cdk.aws-dms-1.99.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-dms",
-    "version": "1.98.0",
+    "version": "1.99.0",
     "description": "The CDK Construct Library for AWS::DMS",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "aws_cdk.aws_dms",
         "aws_cdk.aws_dms._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_dms._jsii": [
-            "aws-dms@1.98.0.jsii.tgz"
+            "aws-dms@1.99.0.jsii.tgz"
         ],
         "aws_cdk.aws_dms": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk.core==1.98.0",
+        "aws-cdk.core==1.99.0",
         "constructs>=3.3.69, <4.0.0",
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

### Comparing `aws-cdk.aws-dms-1.98.0/src/aws_cdk/aws_dms/__init__.py` & `aws-cdk.aws-dms-1.99.0/src/aws_cdk/aws_dms/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-dms-1.98.0/src/aws_cdk.aws_dms.egg-info/PKG-INFO` & `aws-cdk.aws-dms-1.99.0/src/aws_cdk.aws_dms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-dms
-Version: 1.98.0
+Version: 1.99.0
 Summary: The CDK Construct Library for AWS::DMS
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # AWS Database Migration Service Construct Library
```

