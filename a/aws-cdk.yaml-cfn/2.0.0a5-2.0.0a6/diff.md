# Comparing `tmp/aws-cdk.yaml-cfn-2.0.0a5.tar.gz` & `tmp/aws-cdk.yaml-cfn-2.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src216857142/src/packages/@aws-cdk/yaml-cfn/dist/python/aws-cdk.yaml-cfn-2.0.0a5.tar", last modified: Mon Feb 22 12:05:05 2021, max compression
+gzip compressed data, was "/codebuild/output/src222689986/src/packages/@aws-cdk/yaml-cfn/dist/python/aws-cdk.yaml-cfn-2.0.0a6.tar", last modified: Wed Mar  3 14:59:53 2021, max compression
```

## Comparing `aws-cdk.yaml-cfn-2.0.0a5.tar` & `aws-cdk.yaml-cfn-2.0.0a6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/
--rw-r--r--   0 root         (0) root         (0)       23 2021-02-22 12:05:01.000000 aws-cdk.yaml-cfn-2.0.0a5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2023 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      927 2021-02-22 12:05:01.000000 aws-cdk.yaml-cfn-2.0.0a5/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-02-22 12:05:01.000000 aws-cdk.yaml-cfn-2.0.0a5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1581 2021-02-22 12:05:01.000000 aws-cdk.yaml-cfn-2.0.0a5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/src/aws_cdk/yaml_cfn/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/src/aws_cdk/yaml_cfn/_jsii/
--rw-r--r--   0 root         (0) root         (0)      341 2021-02-22 12:05:01.000000 aws-cdk.yaml-cfn-2.0.0a5/src/aws_cdk/yaml_cfn/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104883 2021-02-22 12:05:01.000000 aws-cdk.yaml-cfn-2.0.0a5/src/aws_cdk/yaml_cfn/_jsii/yaml-cfn@2.0.0-alpha.5.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/src/aws_cdk.yaml_cfn.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2023 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/src/aws_cdk.yaml_cfn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      362 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/src/aws_cdk.yaml_cfn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/src/aws_cdk.yaml_cfn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/src/aws_cdk.yaml_cfn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-02-22 12:05:05.000000 aws-cdk.yaml-cfn-2.0.0a5/src/aws_cdk.yaml_cfn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/
+-rw-r--r--   0 root         (0) root         (0)       23 2021-03-03 14:59:49.000000 aws-cdk.yaml-cfn-2.0.0a6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2023 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      927 2021-03-03 14:59:49.000000 aws-cdk.yaml-cfn-2.0.0a6/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-03-03 14:59:49.000000 aws-cdk.yaml-cfn-2.0.0a6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1581 2021-03-03 14:59:49.000000 aws-cdk.yaml-cfn-2.0.0a6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/src/aws_cdk/yaml_cfn/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/src/aws_cdk/yaml_cfn/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      341 2021-03-03 14:59:49.000000 aws-cdk.yaml-cfn-2.0.0a6/src/aws_cdk/yaml_cfn/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104884 2021-03-03 14:59:49.000000 aws-cdk.yaml-cfn-2.0.0a6/src/aws_cdk/yaml_cfn/_jsii/yaml-cfn@2.0.0-alpha.6.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/src/aws_cdk.yaml_cfn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2023 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/src/aws_cdk.yaml_cfn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      362 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/src/aws_cdk.yaml_cfn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/src/aws_cdk.yaml_cfn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/src/aws_cdk.yaml_cfn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2021-03-03 14:59:53.000000 aws-cdk.yaml-cfn-2.0.0a6/src/aws_cdk.yaml_cfn.egg-info/top_level.txt
```

### Comparing `aws-cdk.yaml-cfn-2.0.0a5/PKG-INFO` & `aws-cdk.yaml-cfn-2.0.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.yaml-cfn
-Version: 2.0.0a5
+Version: 2.0.0a6
 Summary: Utilities for handling CloudFormation-flavored YAML
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # CloudFormation YAML utilities
```

### Comparing `aws-cdk.yaml-cfn-2.0.0a5/README.md` & `aws-cdk.yaml-cfn-2.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.yaml-cfn-2.0.0a5/setup.py` & `aws-cdk.yaml-cfn-2.0.0a6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.yaml-cfn",
-    "version": "2.0.0.a5",
+    "version": "2.0.0.a6",
     "description": "Utilities for handling CloudFormation-flavored YAML",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -21,15 +21,15 @@
         "": "src"
     },
     "packages": [
         "aws_cdk.yaml_cfn._jsii"
     ],
     "package_data": {
         "aws_cdk.yaml_cfn._jsii": [
-            "yaml-cfn@2.0.0-alpha.5.jsii.tgz"
+            "yaml-cfn@2.0.0-alpha.6.jsii.tgz"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
         "jsii>=1.21.0, <2.0.0",
         "publication>=0.0.3"
     ],
```

### Comparing `aws-cdk.yaml-cfn-2.0.0a5/src/aws_cdk.yaml_cfn.egg-info/PKG-INFO` & `aws-cdk.yaml-cfn-2.0.0a6/src/aws_cdk.yaml_cfn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.yaml-cfn
-Version: 2.0.0a5
+Version: 2.0.0a6
 Summary: Utilities for handling CloudFormation-flavored YAML
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # CloudFormation YAML utilities
```

