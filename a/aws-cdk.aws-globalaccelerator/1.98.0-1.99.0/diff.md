# Comparing `tmp/aws-cdk.aws-globalaccelerator-1.98.0.tar.gz` & `tmp/aws-cdk.aws-globalaccelerator-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src518022412/src/packages/@aws-cdk/aws-globalaccelerator/dist/python/aws-cdk.aws-globalaccelerator-1.98.0.tar", last modified: Mon Apr 12 10:09:09 2021, max compression
+gzip compressed data, was "/codebuild/output/src875002972/src/packages/@aws-cdk/aws-globalaccelerator/dist/python/aws-cdk.aws-globalaccelerator-1.99.0.tar", last modified: Tue Apr 13 17:03:18 2021, max compression
```

## Comparing `aws-cdk.aws-globalaccelerator-1.98.0.tar` & `aws-cdk.aws-globalaccelerator-1.99.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/
--rw-r--r--   0 root         (0) root         (0)       23 2021-04-12 10:07:22.000000 aws-cdk.aws-globalaccelerator-1.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8889 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6367 2021-04-12 10:07:22.000000 aws-cdk.aws-globalaccelerator-1.98.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-04-12 10:07:22.000000 aws-cdk.aws-globalaccelerator-1.98.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1905 2021-04-12 10:07:22.000000 aws-cdk.aws-globalaccelerator-1.98.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk/aws_globalaccelerator/
--rw-r--r--   0 root         (0) root         (0)   120869 2021-04-12 10:07:22.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk/aws_globalaccelerator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk/aws_globalaccelerator/_jsii/
--rw-r--r--   0 root         (0) root         (0)      471 2021-04-12 10:07:22.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk/aws_globalaccelerator/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55549 2021-04-12 10:07:20.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk/aws_globalaccelerator/_jsii/aws-globalaccelerator@1.98.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:07:22.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk/aws_globalaccelerator/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk.aws_globalaccelerator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8889 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk.aws_globalaccelerator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      548 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk.aws_globalaccelerator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk.aws_globalaccelerator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      143 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk.aws_globalaccelerator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-04-12 10:09:09.000000 aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk.aws_globalaccelerator.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2021-04-13 17:02:04.000000 aws-cdk.aws-globalaccelerator-1.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-04-13 17:02:05.000000 aws-cdk.aws-globalaccelerator-1.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2021-04-13 17:02:04.000000 aws-cdk.aws-globalaccelerator-1.99.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8889 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6367 2021-04-13 17:02:05.000000 aws-cdk.aws-globalaccelerator-1.99.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-04-13 17:02:05.000000 aws-cdk.aws-globalaccelerator-1.99.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1905 2021-04-13 17:02:05.000000 aws-cdk.aws-globalaccelerator-1.99.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk/aws_globalaccelerator/
+-rw-r--r--   0 root         (0) root         (0)   120869 2021-04-13 17:02:05.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk/aws_globalaccelerator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk/aws_globalaccelerator/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      471 2021-04-13 17:02:05.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk/aws_globalaccelerator/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55550 2021-04-13 17:02:03.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk/aws_globalaccelerator/_jsii/aws-globalaccelerator@1.99.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:02:05.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk/aws_globalaccelerator/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk.aws_globalaccelerator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8889 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk.aws_globalaccelerator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      563 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk.aws_globalaccelerator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk.aws_globalaccelerator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      143 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk.aws_globalaccelerator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2021-04-13 17:03:18.000000 aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk.aws_globalaccelerator.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-globalaccelerator-1.98.0/PKG-INFO` & `aws-cdk.aws-globalaccelerator-1.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-globalaccelerator
-Version: 1.98.0
+Version: 1.99.0
 Summary: The CDK Construct Library for AWS::GlobalAccelerator
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # AWS::GlobalAccelerator Construct Library
```

### Comparing `aws-cdk.aws-globalaccelerator-1.98.0/README.md` & `aws-cdk.aws-globalaccelerator-1.99.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk/aws_globalaccelerator/__init__.py` & `aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk/aws_globalaccelerator/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk.aws_globalaccelerator.egg-info/PKG-INFO` & `aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk.aws_globalaccelerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-globalaccelerator
-Version: 1.98.0
+Version: 1.99.0
 Summary: The CDK Construct Library for AWS::GlobalAccelerator
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # AWS::GlobalAccelerator Construct Library
```

### Comparing `aws-cdk.aws-globalaccelerator-1.98.0/src/aws_cdk.aws_globalaccelerator.egg-info/SOURCES.txt` & `aws-cdk.aws-globalaccelerator-1.99.0/src/aws_cdk.aws_globalaccelerator.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+LICENSE
 MANIFEST.in
+NOTICE
 README.md
 pyproject.toml
 setup.py
 src/aws_cdk.aws_globalaccelerator.egg-info/PKG-INFO
 src/aws_cdk.aws_globalaccelerator.egg-info/SOURCES.txt
 src/aws_cdk.aws_globalaccelerator.egg-info/dependency_links.txt
 src/aws_cdk.aws_globalaccelerator.egg-info/requires.txt
 src/aws_cdk.aws_globalaccelerator.egg-info/top_level.txt
 src/aws_cdk/aws_globalaccelerator/__init__.py
 src/aws_cdk/aws_globalaccelerator/py.typed
 src/aws_cdk/aws_globalaccelerator/_jsii/__init__.py
-src/aws_cdk/aws_globalaccelerator/_jsii/aws-globalaccelerator@1.98.0.jsii.tgz
+src/aws_cdk/aws_globalaccelerator/_jsii/aws-globalaccelerator@1.99.0.jsii.tgz
```

