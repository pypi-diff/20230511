# Comparing `tmp/aws-cdk.aws-elasticsearch-1.98.0.tar.gz` & `tmp/aws-cdk.aws-elasticsearch-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src518022412/src/packages/@aws-cdk/aws-elasticsearch/dist/python/aws-cdk.aws-elasticsearch-1.98.0.tar", last modified: Mon Apr 12 10:09:10 2021, max compression
+gzip compressed data, was "/codebuild/output/src875002972/src/packages/@aws-cdk/aws-elasticsearch/dist/python/aws-cdk.aws-elasticsearch-1.99.0.tar", last modified: Tue Apr 13 17:03:19 2021, max compression
```

## Comparing `aws-cdk.aws-elasticsearch-1.98.0.tar` & `aws-cdk.aws-elasticsearch-1.99.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/
--rw-r--r--   0 root         (0) root         (0)       23 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticsearch-1.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13585 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10207 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticsearch-1.98.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticsearch-1.98.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2160 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticsearch-1.98.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk/aws_elasticsearch/
--rw-r--r--   0 root         (0) root         (0)   292824 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk/aws_elasticsearch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk/aws_elasticsearch/_jsii/
--rw-r--r--   0 root         (0) root         (0)      704 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk/aws_elasticsearch/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89002 2021-04-12 10:07:20.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk/aws_elasticsearch/_jsii/aws-elasticsearch@1.98.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:07:22.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk/aws_elasticsearch/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk.aws_elasticsearch.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13585 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk.aws_elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk.aws_elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk.aws_elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      349 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk.aws_elasticsearch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-04-12 10:09:10.000000 aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk.aws_elasticsearch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2021-04-13 17:02:04.000000 aws-cdk.aws-elasticsearch-1.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticsearch-1.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2021-04-13 17:02:04.000000 aws-cdk.aws-elasticsearch-1.99.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13585 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10207 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticsearch-1.99.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticsearch-1.99.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2160 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticsearch-1.99.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk/aws_elasticsearch/
+-rw-r--r--   0 root         (0) root         (0)   292824 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk/aws_elasticsearch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk/aws_elasticsearch/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      704 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk/aws_elasticsearch/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89001 2021-04-13 17:02:03.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk/aws_elasticsearch/_jsii/aws-elasticsearch@1.99.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:02:05.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk/aws_elasticsearch/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk.aws_elasticsearch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13585 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk.aws_elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      523 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk.aws_elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk.aws_elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      349 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk.aws_elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2021-04-13 17:03:19.000000 aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk.aws_elasticsearch.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-elasticsearch-1.98.0/PKG-INFO` & `aws-cdk.aws-elasticsearch-1.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-elasticsearch
-Version: 1.98.0
+Version: 1.99.0
 Summary: The CDK Construct Library for AWS::Elasticsearch
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # Amazon Elasticsearch Service Construct Library
```

### Comparing `aws-cdk.aws-elasticsearch-1.98.0/README.md` & `aws-cdk.aws-elasticsearch-1.99.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-elasticsearch-1.98.0/setup.py` & `aws-cdk.aws-elasticsearch-1.99.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-elasticsearch",
-    "version": "1.98.0",
+    "version": "1.99.0",
     "description": "The CDK Construct Library for AWS::Elasticsearch",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,34 +22,34 @@
     },
     "packages": [
         "aws_cdk.aws_elasticsearch",
         "aws_cdk.aws_elasticsearch._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_elasticsearch._jsii": [
-            "aws-elasticsearch@1.98.0.jsii.tgz"
+            "aws-elasticsearch@1.99.0.jsii.tgz"
         ],
         "aws_cdk.aws_elasticsearch": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk.aws-certificatemanager==1.98.0",
-        "aws-cdk.aws-cloudwatch==1.98.0",
-        "aws-cdk.aws-ec2==1.98.0",
-        "aws-cdk.aws-iam==1.98.0",
-        "aws-cdk.aws-kms==1.98.0",
-        "aws-cdk.aws-logs==1.98.0",
-        "aws-cdk.aws-route53==1.98.0",
-        "aws-cdk.aws-secretsmanager==1.98.0",
-        "aws-cdk.core==1.98.0",
-        "aws-cdk.custom-resources==1.98.0",
+        "aws-cdk.aws-certificatemanager==1.99.0",
+        "aws-cdk.aws-cloudwatch==1.99.0",
+        "aws-cdk.aws-ec2==1.99.0",
+        "aws-cdk.aws-iam==1.99.0",
+        "aws-cdk.aws-kms==1.99.0",
+        "aws-cdk.aws-logs==1.99.0",
+        "aws-cdk.aws-route53==1.99.0",
+        "aws-cdk.aws-secretsmanager==1.99.0",
+        "aws-cdk.core==1.99.0",
+        "aws-cdk.custom-resources==1.99.0",
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

### Comparing `aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk/aws_elasticsearch/__init__.py` & `aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk/aws_elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk/aws_elasticsearch/_jsii/__init__.py` & `aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk/aws_elasticsearch/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import aws_cdk.aws_secretsmanager._jsii
 import aws_cdk.core._jsii
 import aws_cdk.custom_resources._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-cdk/aws-elasticsearch",
-    "1.98.0",
+    "1.99.0",
     __name__[0:-6],
-    "aws-elasticsearch@1.98.0.jsii.tgz",
+    "aws-elasticsearch@1.99.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-cdk.aws-elasticsearch-1.98.0/src/aws_cdk.aws_elasticsearch.egg-info/PKG-INFO` & `aws-cdk.aws-elasticsearch-1.99.0/src/aws_cdk.aws_elasticsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-elasticsearch
-Version: 1.98.0
+Version: 1.99.0
 Summary: The CDK Construct Library for AWS::Elasticsearch
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # Amazon Elasticsearch Service Construct Library
```

