# Comparing `tmp/aws-cdk.pipelines-1.98.0.tar.gz` & `tmp/aws-cdk.pipelines-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src518022412/src/packages/@aws-cdk/pipelines/dist/python/aws-cdk.pipelines-1.98.0.tar", last modified: Mon Apr 12 10:09:20 2021, max compression
+gzip compressed data, was "/codebuild/output/src875002972/src/packages/@aws-cdk/pipelines/dist/python/aws-cdk.pipelines-1.99.0.tar", last modified: Tue Apr 13 17:03:24 2021, max compression
```

## Comparing `aws-cdk.pipelines-1.98.0.tar` & `aws-cdk.pipelines-1.99.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/
--rw-r--r--   0 root         (0) root         (0)       23 2021-04-12 10:07:22.000000 aws-cdk.pipelines-1.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    38889 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    31757 2021-04-12 10:07:22.000000 aws-cdk.pipelines-1.98.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-04-12 10:07:22.000000 aws-cdk.pipelines-1.98.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2097 2021-04-12 10:07:22.000000 aws-cdk.pipelines-1.98.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk/pipelines/
--rw-r--r--   0 root         (0) root         (0)   232789 2021-04-12 10:07:22.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk/pipelines/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk/pipelines/_jsii/
--rw-r--r--   0 root         (0) root         (0)      682 2021-04-12 10:07:22.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk/pipelines/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   123489 2021-04-12 10:07:20.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk/pipelines/_jsii/pipelines@1.98.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:07:22.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk/pipelines/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk.pipelines.egg-info/
--rw-r--r--   0 root         (0) root         (0)    38889 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk.pipelines.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk.pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk.pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      356 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk.pipelines.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-04-12 10:09:20.000000 aws-cdk.pipelines-1.98.0/src/aws_cdk.pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2021-04-13 17:02:04.000000 aws-cdk.pipelines-1.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-04-13 17:02:05.000000 aws-cdk.pipelines-1.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2021-04-13 17:02:04.000000 aws-cdk.pipelines-1.99.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    38889 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    31757 2021-04-13 17:02:05.000000 aws-cdk.pipelines-1.99.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-04-13 17:02:05.000000 aws-cdk.pipelines-1.99.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2097 2021-04-13 17:02:05.000000 aws-cdk.pipelines-1.99.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk/pipelines/
+-rw-r--r--   0 root         (0) root         (0)   232789 2021-04-13 17:02:05.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk/pipelines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk/pipelines/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      682 2021-04-13 17:02:05.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk/pipelines/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   123488 2021-04-13 17:02:03.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk/pipelines/_jsii/pipelines@1.99.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:02:05.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk/pipelines/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk.pipelines.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    38889 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk.pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk.pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk.pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      356 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk.pipelines.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2021-04-13 17:03:24.000000 aws-cdk.pipelines-1.99.0/src/aws_cdk.pipelines.egg-info/top_level.txt
```

### Comparing `aws-cdk.pipelines-1.98.0/PKG-INFO` & `aws-cdk.pipelines-1.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.pipelines
-Version: 1.98.0
+Version: 1.99.0
 Summary: Continuous Delivery of CDK applications
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # CDK Pipelines
```

### Comparing `aws-cdk.pipelines-1.98.0/README.md` & `aws-cdk.pipelines-1.99.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.pipelines-1.98.0/setup.py` & `aws-cdk.pipelines-1.99.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.pipelines",
-    "version": "1.98.0",
+    "version": "1.99.0",
     "description": "Continuous Delivery of CDK applications",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,34 +22,34 @@
     },
     "packages": [
         "aws_cdk.pipelines",
         "aws_cdk.pipelines._jsii"
     ],
     "package_data": {
         "aws_cdk.pipelines._jsii": [
-            "pipelines@1.98.0.jsii.tgz"
+            "pipelines@1.99.0.jsii.tgz"
         ],
         "aws_cdk.pipelines": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk.aws-codebuild==1.98.0",
-        "aws-cdk.aws-codepipeline-actions==1.98.0",
-        "aws-cdk.aws-codepipeline==1.98.0",
-        "aws-cdk.aws-ec2==1.98.0",
-        "aws-cdk.aws-events==1.98.0",
-        "aws-cdk.aws-iam==1.98.0",
-        "aws-cdk.aws-s3-assets==1.98.0",
-        "aws-cdk.cloud-assembly-schema==1.98.0",
-        "aws-cdk.core==1.98.0",
-        "aws-cdk.cx-api==1.98.0",
+        "aws-cdk.aws-codebuild==1.99.0",
+        "aws-cdk.aws-codepipeline-actions==1.99.0",
+        "aws-cdk.aws-codepipeline==1.99.0",
+        "aws-cdk.aws-ec2==1.99.0",
+        "aws-cdk.aws-events==1.99.0",
+        "aws-cdk.aws-iam==1.99.0",
+        "aws-cdk.aws-s3-assets==1.99.0",
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

### Comparing `aws-cdk.pipelines-1.98.0/src/aws_cdk/pipelines/__init__.py` & `aws-cdk.pipelines-1.99.0/src/aws_cdk/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.pipelines-1.98.0/src/aws_cdk/pipelines/_jsii/__init__.py` & `aws-cdk.pipelines-1.99.0/src/aws_cdk/pipelines/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import aws_cdk.aws_s3_assets._jsii
 import aws_cdk.cloud_assembly_schema._jsii
 import aws_cdk.core._jsii
 import aws_cdk.cx_api._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
-    "@aws-cdk/pipelines", "1.98.0", __name__[0:-6], "pipelines@1.98.0.jsii.tgz"
+    "@aws-cdk/pipelines", "1.99.0", __name__[0:-6], "pipelines@1.99.0.jsii.tgz"
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-cdk.pipelines-1.98.0/src/aws_cdk.pipelines.egg-info/PKG-INFO` & `aws-cdk.pipelines-1.99.0/src/aws_cdk.pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.pipelines
-Version: 1.98.0
+Version: 1.99.0
 Summary: Continuous Delivery of CDK applications
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # CDK Pipelines
```

