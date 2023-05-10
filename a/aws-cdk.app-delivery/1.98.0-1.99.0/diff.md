# Comparing `tmp/aws-cdk.app-delivery-1.98.0.tar.gz` & `tmp/aws-cdk.app-delivery-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src518022412/src/packages/@aws-cdk/app-delivery/dist/python/aws-cdk.app-delivery-1.98.0.tar", last modified: Mon Apr 12 10:10:15 2021, max compression
+gzip compressed data, was "/codebuild/output/src875002972/src/packages/@aws-cdk/app-delivery/dist/python/aws-cdk.app-delivery-1.99.0.tar", last modified: Tue Apr 13 17:03:24 2021, max compression
```

## Comparing `aws-cdk.app-delivery-1.98.0.tar` & `aws-cdk.app-delivery-1.99.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/
--rw-r--r--   0 root         (0) root         (0)       23 2021-04-12 10:07:22.000000 aws-cdk.app-delivery-1.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9358 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7089 2021-04-12 10:07:22.000000 aws-cdk.app-delivery-1.98.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-04-12 10:07:22.000000 aws-cdk.app-delivery-1.98.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2115 2021-04-12 10:07:22.000000 aws-cdk.app-delivery-1.98.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk/app_delivery/
--rw-r--r--   0 root         (0) root         (0)    27517 2021-04-12 10:07:22.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk/app_delivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk/app_delivery/_jsii/
--rw-r--r--   0 root         (0) root         (0)      664 2021-04-12 10:07:22.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk/app_delivery/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22730 2021-04-12 10:07:20.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk/app_delivery/_jsii/app-delivery@1.98.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:07:22.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk/app_delivery/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk.app_delivery.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9358 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk.app_delivery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      458 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk.app_delivery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk.app_delivery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      337 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk.app_delivery.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-04-12 10:10:15.000000 aws-cdk.app-delivery-1.98.0/src/aws_cdk.app_delivery.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2021-04-13 17:02:04.000000 aws-cdk.app-delivery-1.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-04-13 17:02:05.000000 aws-cdk.app-delivery-1.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2021-04-13 17:02:04.000000 aws-cdk.app-delivery-1.99.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9358 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7089 2021-04-13 17:02:05.000000 aws-cdk.app-delivery-1.99.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-04-13 17:02:05.000000 aws-cdk.app-delivery-1.99.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2115 2021-04-13 17:02:05.000000 aws-cdk.app-delivery-1.99.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk/app_delivery/
+-rw-r--r--   0 root         (0) root         (0)    27517 2021-04-13 17:02:05.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk/app_delivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk/app_delivery/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      664 2021-04-13 17:02:05.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk/app_delivery/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22730 2021-04-13 17:02:03.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk/app_delivery/_jsii/app-delivery@1.99.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:02:05.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk/app_delivery/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk.app_delivery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9358 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk.app_delivery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      473 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk.app_delivery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk.app_delivery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      337 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk.app_delivery.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2021-04-13 17:03:24.000000 aws-cdk.app-delivery-1.99.0/src/aws_cdk.app_delivery.egg-info/top_level.txt
```

### Comparing `aws-cdk.app-delivery-1.98.0/PKG-INFO` & `aws-cdk.app-delivery-1.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.app-delivery
-Version: 1.98.0
+Version: 1.99.0
 Summary: Continuous Integration / Continuous Delivery for CDK Applications
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # Continuous Integration / Continuous Delivery for CDK Applications
```

### Comparing `aws-cdk.app-delivery-1.98.0/README.md` & `aws-cdk.app-delivery-1.99.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.app-delivery-1.98.0/setup.py` & `aws-cdk.app-delivery-1.99.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.app-delivery",
-    "version": "1.98.0",
+    "version": "1.99.0",
     "description": "Continuous Integration / Continuous Delivery for CDK Applications",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,33 +22,33 @@
     },
     "packages": [
         "aws_cdk.app_delivery",
         "aws_cdk.app_delivery._jsii"
     ],
     "package_data": {
         "aws_cdk.app_delivery._jsii": [
-            "app-delivery@1.98.0.jsii.tgz"
+            "app-delivery@1.99.0.jsii.tgz"
         ],
         "aws_cdk.app_delivery": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk.aws-cloudformation==1.98.0",
-        "aws-cdk.aws-codebuild==1.98.0",
-        "aws-cdk.aws-codepipeline-actions==1.98.0",
-        "aws-cdk.aws-codepipeline==1.98.0",
-        "aws-cdk.aws-events==1.98.0",
-        "aws-cdk.aws-iam==1.98.0",
-        "aws-cdk.cloud-assembly-schema==1.98.0",
-        "aws-cdk.core==1.98.0",
-        "aws-cdk.cx-api==1.98.0",
+        "aws-cdk.aws-cloudformation==1.99.0",
+        "aws-cdk.aws-codebuild==1.99.0",
+        "aws-cdk.aws-codepipeline-actions==1.99.0",
+        "aws-cdk.aws-codepipeline==1.99.0",
+        "aws-cdk.aws-events==1.99.0",
+        "aws-cdk.aws-iam==1.99.0",
+        "aws-cdk.cloud-assembly-schema==1.99.0",
+        "aws-cdk.core==1.99.0",
+        "aws-cdk.cx-api==1.99.0",
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

### Comparing `aws-cdk.app-delivery-1.98.0/src/aws_cdk/app_delivery/__init__.py` & `aws-cdk.app-delivery-1.99.0/src/aws_cdk/app_delivery/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.app-delivery-1.98.0/src/aws_cdk/app_delivery/_jsii/__init__.py` & `aws-cdk.app-delivery-1.99.0/src/aws_cdk/app_delivery/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import aws_cdk.aws_iam._jsii
 import aws_cdk.cloud_assembly_schema._jsii
 import aws_cdk.core._jsii
 import aws_cdk.cx_api._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
-    "@aws-cdk/app-delivery", "1.98.0", __name__[0:-6], "app-delivery@1.98.0.jsii.tgz"
+    "@aws-cdk/app-delivery", "1.99.0", __name__[0:-6], "app-delivery@1.99.0.jsii.tgz"
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-cdk.app-delivery-1.98.0/src/aws_cdk.app_delivery.egg-info/PKG-INFO` & `aws-cdk.app-delivery-1.99.0/src/aws_cdk.app_delivery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.app-delivery
-Version: 1.98.0
+Version: 1.99.0
 Summary: Continuous Integration / Continuous Delivery for CDK Applications
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # Continuous Integration / Continuous Delivery for CDK Applications
```

