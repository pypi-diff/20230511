# Comparing `tmp/aws-cdk.aws-codepipeline-actions-1.98.0.tar.gz` & `tmp/aws-cdk.aws-codepipeline-actions-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src518022412/src/packages/@aws-cdk/aws-codepipeline-actions/dist/python/aws-cdk.aws-codepipeline-actions-1.98", last modified: Mon Apr 12 10:09:19 2021, max compression
+gzip compressed data, was "/codebuild/output/src875002972/src/packages/@aws-cdk/aws-codepipeline-actions/dist/python/aws-cdk.aws-codepipeline-actions-1.99", last modified: Tue Apr 13 17:03:24 2021, max compression
```

## Comparing `aws-cdk.aws-codepipeline-actions-1.98.0.tar` & `aws-cdk.aws-codepipeline-actions-1.99.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/
--rw-r--r--   0 root         (0) root         (0)       23 2021-04-12 10:07:22.000000 aws-cdk.aws-codepipeline-actions-1.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    57767 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    45944 2021-04-12 10:07:22.000000 aws-cdk.aws-codepipeline-actions-1.98.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-04-12 10:07:22.000000 aws-cdk.aws-codepipeline-actions-1.98.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2516 2021-04-12 10:07:22.000000 aws-cdk.aws-codepipeline-actions-1.98.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk/aws_codepipeline_actions/
--rw-r--r--   0 root         (0) root         (0)   424368 2021-04-12 10:07:22.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk/aws_codepipeline_actions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk/aws_codepipeline_actions/_jsii/
--rw-r--r--   0 root         (0) root         (0)      994 2021-04-12 10:07:22.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk/aws_codepipeline_actions/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142018 2021-04-12 10:07:20.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk/aws_codepipeline_actions/_jsii/aws-codepipeline-actions@1.98.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:07:22.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk/aws_codepipeline_actions/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk.aws_codepipeline_actions.egg-info/
--rw-r--r--   0 root         (0) root         (0)    57767 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk.aws_codepipeline_actions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      578 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk.aws_codepipeline_actions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk.aws_codepipeline_actions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      585 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk.aws_codepipeline_actions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-04-12 10:09:19.000000 aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk.aws_codepipeline_actions.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2021-04-13 17:02:04.000000 aws-cdk.aws-codepipeline-actions-1.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-04-13 17:02:05.000000 aws-cdk.aws-codepipeline-actions-1.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1381 2021-04-13 17:02:04.000000 aws-cdk.aws-codepipeline-actions-1.99.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    57767 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    45944 2021-04-13 17:02:05.000000 aws-cdk.aws-codepipeline-actions-1.99.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-04-13 17:02:05.000000 aws-cdk.aws-codepipeline-actions-1.99.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2516 2021-04-13 17:02:05.000000 aws-cdk.aws-codepipeline-actions-1.99.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk/aws_codepipeline_actions/
+-rw-r--r--   0 root         (0) root         (0)   424368 2021-04-13 17:02:05.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk/aws_codepipeline_actions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk/aws_codepipeline_actions/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      994 2021-04-13 17:02:05.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk/aws_codepipeline_actions/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142018 2021-04-13 17:02:03.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk/aws_codepipeline_actions/_jsii/aws-codepipeline-actions@1.99.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:02:05.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk/aws_codepipeline_actions/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk.aws_codepipeline_actions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    57767 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk.aws_codepipeline_actions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      593 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk.aws_codepipeline_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk.aws_codepipeline_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      585 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk.aws_codepipeline_actions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2021-04-13 17:03:24.000000 aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk.aws_codepipeline_actions.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-codepipeline-actions-1.98.0/PKG-INFO` & `aws-cdk.aws-codepipeline-actions-1.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-codepipeline-actions
-Version: 1.98.0
+Version: 1.99.0
 Summary: Concrete Actions for AWS Code Pipeline
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # AWS CodePipeline Actions
```

### Comparing `aws-cdk.aws-codepipeline-actions-1.98.0/README.md` & `aws-cdk.aws-codepipeline-actions-1.99.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-codepipeline-actions-1.98.0/setup.py` & `aws-cdk.aws-codepipeline-actions-1.99.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-codepipeline-actions",
-    "version": "1.98.0",
+    "version": "1.99.0",
     "description": "Concrete Actions for AWS Code Pipeline",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,42 +22,42 @@
     },
     "packages": [
         "aws_cdk.aws_codepipeline_actions",
         "aws_cdk.aws_codepipeline_actions._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_codepipeline_actions._jsii": [
-            "aws-codepipeline-actions@1.98.0.jsii.tgz"
+            "aws-codepipeline-actions@1.99.0.jsii.tgz"
         ],
         "aws_cdk.aws_codepipeline_actions": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk.aws-cloudformation==1.98.0",
-        "aws-cdk.aws-codebuild==1.98.0",
-        "aws-cdk.aws-codecommit==1.98.0",
-        "aws-cdk.aws-codedeploy==1.98.0",
-        "aws-cdk.aws-codepipeline==1.98.0",
-        "aws-cdk.aws-ec2==1.98.0",
-        "aws-cdk.aws-ecr==1.98.0",
-        "aws-cdk.aws-ecs==1.98.0",
-        "aws-cdk.aws-events-targets==1.98.0",
-        "aws-cdk.aws-events==1.98.0",
-        "aws-cdk.aws-iam==1.98.0",
-        "aws-cdk.aws-lambda==1.98.0",
-        "aws-cdk.aws-s3==1.98.0",
-        "aws-cdk.aws-servicecatalog==1.98.0",
-        "aws-cdk.aws-sns-subscriptions==1.98.0",
-        "aws-cdk.aws-sns==1.98.0",
-        "aws-cdk.aws-stepfunctions==1.98.0",
-        "aws-cdk.core==1.98.0",
+        "aws-cdk.aws-cloudformation==1.99.0",
+        "aws-cdk.aws-codebuild==1.99.0",
+        "aws-cdk.aws-codecommit==1.99.0",
+        "aws-cdk.aws-codedeploy==1.99.0",
+        "aws-cdk.aws-codepipeline==1.99.0",
+        "aws-cdk.aws-ec2==1.99.0",
+        "aws-cdk.aws-ecr==1.99.0",
+        "aws-cdk.aws-ecs==1.99.0",
+        "aws-cdk.aws-events-targets==1.99.0",
+        "aws-cdk.aws-events==1.99.0",
+        "aws-cdk.aws-iam==1.99.0",
+        "aws-cdk.aws-lambda==1.99.0",
+        "aws-cdk.aws-s3==1.99.0",
+        "aws-cdk.aws-servicecatalog==1.99.0",
+        "aws-cdk.aws-sns-subscriptions==1.99.0",
+        "aws-cdk.aws-sns==1.99.0",
+        "aws-cdk.aws-stepfunctions==1.99.0",
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

### Comparing `aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk/aws_codepipeline_actions/__init__.py` & `aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk/aws_codepipeline_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk/aws_codepipeline_actions/_jsii/__init__.py` & `aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk/aws_codepipeline_actions/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 import aws_cdk.aws_sns_subscriptions._jsii
 import aws_cdk.aws_stepfunctions._jsii
 import aws_cdk.core._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-cdk/aws-codepipeline-actions",
-    "1.98.0",
+    "1.99.0",
     __name__[0:-6],
-    "aws-codepipeline-actions@1.98.0.jsii.tgz",
+    "aws-codepipeline-actions@1.99.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk.aws_codepipeline_actions.egg-info/PKG-INFO` & `aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk.aws_codepipeline_actions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-codepipeline-actions
-Version: 1.98.0
+Version: 1.99.0
 Summary: Concrete Actions for AWS Code Pipeline
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # AWS CodePipeline Actions
```

### Comparing `aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk.aws_codepipeline_actions.egg-info/SOURCES.txt` & `aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk.aws_codepipeline_actions.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+LICENSE
 MANIFEST.in
+NOTICE
 README.md
 pyproject.toml
 setup.py
 src/aws_cdk.aws_codepipeline_actions.egg-info/PKG-INFO
 src/aws_cdk.aws_codepipeline_actions.egg-info/SOURCES.txt
 src/aws_cdk.aws_codepipeline_actions.egg-info/dependency_links.txt
 src/aws_cdk.aws_codepipeline_actions.egg-info/requires.txt
 src/aws_cdk.aws_codepipeline_actions.egg-info/top_level.txt
 src/aws_cdk/aws_codepipeline_actions/__init__.py
 src/aws_cdk/aws_codepipeline_actions/py.typed
 src/aws_cdk/aws_codepipeline_actions/_jsii/__init__.py
-src/aws_cdk/aws_codepipeline_actions/_jsii/aws-codepipeline-actions@1.98.0.jsii.tgz
+src/aws_cdk/aws_codepipeline_actions/_jsii/aws-codepipeline-actions@1.99.0.jsii.tgz
```

### Comparing `aws-cdk.aws-codepipeline-actions-1.98.0/src/aws_cdk.aws_codepipeline_actions.egg-info/requires.txt` & `aws-cdk.aws-codepipeline-actions-1.99.0/src/aws_cdk.aws_codepipeline_actions.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-aws-cdk.aws-cloudformation==1.98.0
-aws-cdk.aws-codebuild==1.98.0
-aws-cdk.aws-codecommit==1.98.0
-aws-cdk.aws-codedeploy==1.98.0
-aws-cdk.aws-codepipeline==1.98.0
-aws-cdk.aws-ec2==1.98.0
-aws-cdk.aws-ecr==1.98.0
-aws-cdk.aws-ecs==1.98.0
-aws-cdk.aws-events-targets==1.98.0
-aws-cdk.aws-events==1.98.0
-aws-cdk.aws-iam==1.98.0
-aws-cdk.aws-lambda==1.98.0
-aws-cdk.aws-s3==1.98.0
-aws-cdk.aws-servicecatalog==1.98.0
-aws-cdk.aws-sns-subscriptions==1.98.0
-aws-cdk.aws-sns==1.98.0
-aws-cdk.aws-stepfunctions==1.98.0
-aws-cdk.core==1.98.0
+aws-cdk.aws-cloudformation==1.99.0
+aws-cdk.aws-codebuild==1.99.0
+aws-cdk.aws-codecommit==1.99.0
+aws-cdk.aws-codedeploy==1.99.0
+aws-cdk.aws-codepipeline==1.99.0
+aws-cdk.aws-ec2==1.99.0
+aws-cdk.aws-ecr==1.99.0
+aws-cdk.aws-ecs==1.99.0
+aws-cdk.aws-events-targets==1.99.0
+aws-cdk.aws-events==1.99.0
+aws-cdk.aws-iam==1.99.0
+aws-cdk.aws-lambda==1.99.0
+aws-cdk.aws-s3==1.99.0
+aws-cdk.aws-servicecatalog==1.99.0
+aws-cdk.aws-sns-subscriptions==1.99.0
+aws-cdk.aws-sns==1.99.0
+aws-cdk.aws-stepfunctions==1.99.0
+aws-cdk.core==1.99.0
 constructs<4.0.0,>=3.3.69
-jsii<2.0.0,>=1.27.0
+jsii<2.0.0,>=1.28.0
 publication>=0.0.3
```

