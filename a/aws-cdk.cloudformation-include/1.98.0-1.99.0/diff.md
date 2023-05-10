# Comparing `tmp/aws-cdk.cloudformation-include-1.98.0.tar.gz` & `tmp/aws-cdk.cloudformation-include-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src518022412/src/packages/@aws-cdk/cloudformation-include/dist/python/aws-cdk.cloudformation-include-1.98.0.t", last modified: Mon Apr 12 10:10:14 2021, max compression
+gzip compressed data, was "/codebuild/output/src875002972/src/packages/@aws-cdk/cloudformation-include/dist/python/aws-cdk.cloudformation-include-1.99.0.t", last modified: Tue Apr 13 17:04:07 2021, max compression
```

## Comparing `aws-cdk.cloudformation-include-1.98.0.tar` & `aws-cdk.cloudformation-include-1.99.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/
--rw-r--r--   0 root         (0) root         (0)       23 2021-04-12 10:07:22.000000 aws-cdk.cloudformation-include-1.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15269 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11466 2021-04-12 10:07:22.000000 aws-cdk.cloudformation-include-1.98.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-04-12 10:07:22.000000 aws-cdk.cloudformation-include-1.98.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     7881 2021-04-12 10:07:22.000000 aws-cdk.cloudformation-include-1.98.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk/cloudformation_include/
--rw-r--r--   0 root         (0) root         (0)    30810 2021-04-12 10:07:22.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk/cloudformation_include/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk/cloudformation_include/_jsii/
--rw-r--r--   0 root         (0) root         (0)     5547 2021-04-12 10:07:22.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk/cloudformation_include/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   153777 2021-04-12 10:07:20.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk/cloudformation_include/_jsii/cloudformation-include@1.98.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:07:22.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk/cloudformation_include/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk.cloudformation_include.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15269 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk.cloudformation_include.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      558 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk.cloudformation_include.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk.cloudformation_include.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     4497 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk.cloudformation_include.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-04-12 10:10:14.000000 aws-cdk.cloudformation-include-1.98.0/src/aws_cdk.cloudformation_include.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2021-04-13 17:02:04.000000 aws-cdk.cloudformation-include-1.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-04-13 17:02:05.000000 aws-cdk.cloudformation-include-1.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1069 2021-04-13 17:02:04.000000 aws-cdk.cloudformation-include-1.99.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15269 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11466 2021-04-13 17:02:05.000000 aws-cdk.cloudformation-include-1.99.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-04-13 17:02:05.000000 aws-cdk.cloudformation-include-1.99.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     7881 2021-04-13 17:02:05.000000 aws-cdk.cloudformation-include-1.99.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk/cloudformation_include/
+-rw-r--r--   0 root         (0) root         (0)    30810 2021-04-13 17:02:05.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk/cloudformation_include/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk/cloudformation_include/_jsii/
+-rw-r--r--   0 root         (0) root         (0)     5547 2021-04-13 17:02:05.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk/cloudformation_include/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   153774 2021-04-13 17:02:03.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk/cloudformation_include/_jsii/cloudformation-include@1.99.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:02:05.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk/cloudformation_include/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk.cloudformation_include.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15269 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk.cloudformation_include.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      573 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk.cloudformation_include.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk.cloudformation_include.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     4497 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk.cloudformation_include.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2021-04-13 17:04:07.000000 aws-cdk.cloudformation-include-1.99.0/src/aws_cdk.cloudformation_include.egg-info/top_level.txt
```

### Comparing `aws-cdk.cloudformation-include-1.98.0/PKG-INFO` & `aws-cdk.cloudformation-include-1.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cloudformation-include
-Version: 1.98.0
+Version: 1.99.0
 Summary: A package that facilitates working with existing CloudFormation templates in the CDK
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # Include CloudFormation templates in the CDK
```

### Comparing `aws-cdk.cloudformation-include-1.98.0/README.md` & `aws-cdk.cloudformation-include-1.99.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.cloudformation-include-1.98.0/setup.py` & `aws-cdk.cloudformation-include-1.99.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.cloudformation-include",
-    "version": "1.98.0",
+    "version": "1.99.0",
     "description": "A package that facilitates working with existing CloudFormation templates in the CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,171 +22,171 @@
     },
     "packages": [
         "aws_cdk.cloudformation_include",
         "aws_cdk.cloudformation_include._jsii"
     ],
     "package_data": {
         "aws_cdk.cloudformation_include._jsii": [
-            "cloudformation-include@1.98.0.jsii.tgz"
+            "cloudformation-include@1.99.0.jsii.tgz"
         ],
         "aws_cdk.cloudformation_include": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk.alexa-ask==1.98.0",
-        "aws-cdk.aws-accessanalyzer==1.98.0",
-        "aws-cdk.aws-acmpca==1.98.0",
-        "aws-cdk.aws-amazonmq==1.98.0",
-        "aws-cdk.aws-amplify==1.98.0",
-        "aws-cdk.aws-apigateway==1.98.0",
-        "aws-cdk.aws-apigatewayv2==1.98.0",
-        "aws-cdk.aws-appconfig==1.98.0",
-        "aws-cdk.aws-appflow==1.98.0",
-        "aws-cdk.aws-applicationautoscaling==1.98.0",
-        "aws-cdk.aws-applicationinsights==1.98.0",
-        "aws-cdk.aws-appmesh==1.98.0",
-        "aws-cdk.aws-appstream==1.98.0",
-        "aws-cdk.aws-appsync==1.98.0",
-        "aws-cdk.aws-athena==1.98.0",
-        "aws-cdk.aws-auditmanager==1.98.0",
-        "aws-cdk.aws-autoscaling==1.98.0",
-        "aws-cdk.aws-autoscalingplans==1.98.0",
-        "aws-cdk.aws-backup==1.98.0",
-        "aws-cdk.aws-batch==1.98.0",
-        "aws-cdk.aws-budgets==1.98.0",
-        "aws-cdk.aws-cassandra==1.98.0",
-        "aws-cdk.aws-ce==1.98.0",
-        "aws-cdk.aws-certificatemanager==1.98.0",
-        "aws-cdk.aws-chatbot==1.98.0",
-        "aws-cdk.aws-cloud9==1.98.0",
-        "aws-cdk.aws-cloudfront==1.98.0",
-        "aws-cdk.aws-cloudtrail==1.98.0",
-        "aws-cdk.aws-cloudwatch==1.98.0",
-        "aws-cdk.aws-codeartifact==1.98.0",
-        "aws-cdk.aws-codebuild==1.98.0",
-        "aws-cdk.aws-codecommit==1.98.0",
-        "aws-cdk.aws-codedeploy==1.98.0",
-        "aws-cdk.aws-codeguruprofiler==1.98.0",
-        "aws-cdk.aws-codegurureviewer==1.98.0",
-        "aws-cdk.aws-codepipeline==1.98.0",
-        "aws-cdk.aws-codestar==1.98.0",
-        "aws-cdk.aws-codestarconnections==1.98.0",
-        "aws-cdk.aws-codestarnotifications==1.98.0",
-        "aws-cdk.aws-cognito==1.98.0",
-        "aws-cdk.aws-config==1.98.0",
-        "aws-cdk.aws-databrew==1.98.0",
-        "aws-cdk.aws-datapipeline==1.98.0",
-        "aws-cdk.aws-datasync==1.98.0",
-        "aws-cdk.aws-dax==1.98.0",
-        "aws-cdk.aws-detective==1.98.0",
-        "aws-cdk.aws-devopsguru==1.98.0",
-        "aws-cdk.aws-directoryservice==1.98.0",
-        "aws-cdk.aws-dlm==1.98.0",
-        "aws-cdk.aws-dms==1.98.0",
-        "aws-cdk.aws-docdb==1.98.0",
-        "aws-cdk.aws-dynamodb==1.98.0",
-        "aws-cdk.aws-ec2==1.98.0",
-        "aws-cdk.aws-ecr==1.98.0",
-        "aws-cdk.aws-ecs==1.98.0",
-        "aws-cdk.aws-efs==1.98.0",
-        "aws-cdk.aws-eks==1.98.0",
-        "aws-cdk.aws-elasticache==1.98.0",
-        "aws-cdk.aws-elasticbeanstalk==1.98.0",
-        "aws-cdk.aws-elasticloadbalancing==1.98.0",
-        "aws-cdk.aws-elasticloadbalancingv2==1.98.0",
-        "aws-cdk.aws-elasticsearch==1.98.0",
-        "aws-cdk.aws-emr==1.98.0",
-        "aws-cdk.aws-emrcontainers==1.98.0",
-        "aws-cdk.aws-events==1.98.0",
-        "aws-cdk.aws-eventschemas==1.98.0",
-        "aws-cdk.aws-fis==1.98.0",
-        "aws-cdk.aws-fms==1.98.0",
-        "aws-cdk.aws-fsx==1.98.0",
-        "aws-cdk.aws-gamelift==1.98.0",
-        "aws-cdk.aws-globalaccelerator==1.98.0",
-        "aws-cdk.aws-glue==1.98.0",
-        "aws-cdk.aws-greengrass==1.98.0",
-        "aws-cdk.aws-greengrassv2==1.98.0",
-        "aws-cdk.aws-guardduty==1.98.0",
-        "aws-cdk.aws-iam==1.98.0",
-        "aws-cdk.aws-imagebuilder==1.98.0",
-        "aws-cdk.aws-inspector==1.98.0",
-        "aws-cdk.aws-iot1click==1.98.0",
-        "aws-cdk.aws-iot==1.98.0",
-        "aws-cdk.aws-iotanalytics==1.98.0",
-        "aws-cdk.aws-iotevents==1.98.0",
-        "aws-cdk.aws-iotsitewise==1.98.0",
-        "aws-cdk.aws-iotthingsgraph==1.98.0",
-        "aws-cdk.aws-iotwireless==1.98.0",
-        "aws-cdk.aws-ivs==1.98.0",
-        "aws-cdk.aws-kendra==1.98.0",
-        "aws-cdk.aws-kinesis==1.98.0",
-        "aws-cdk.aws-kinesisanalytics==1.98.0",
-        "aws-cdk.aws-kinesisfirehose==1.98.0",
-        "aws-cdk.aws-kms==1.98.0",
-        "aws-cdk.aws-lakeformation==1.98.0",
-        "aws-cdk.aws-lambda==1.98.0",
-        "aws-cdk.aws-licensemanager==1.98.0",
-        "aws-cdk.aws-logs==1.98.0",
-        "aws-cdk.aws-lookoutvision==1.98.0",
-        "aws-cdk.aws-macie==1.98.0",
-        "aws-cdk.aws-managedblockchain==1.98.0",
-        "aws-cdk.aws-mediaconnect==1.98.0",
-        "aws-cdk.aws-mediaconvert==1.98.0",
-        "aws-cdk.aws-medialive==1.98.0",
-        "aws-cdk.aws-mediapackage==1.98.0",
-        "aws-cdk.aws-mediastore==1.98.0",
-        "aws-cdk.aws-msk==1.98.0",
-        "aws-cdk.aws-mwaa==1.98.0",
-        "aws-cdk.aws-neptune==1.98.0",
-        "aws-cdk.aws-networkfirewall==1.98.0",
-        "aws-cdk.aws-networkmanager==1.98.0",
-        "aws-cdk.aws-opsworks==1.98.0",
-        "aws-cdk.aws-opsworkscm==1.98.0",
-        "aws-cdk.aws-pinpoint==1.98.0",
-        "aws-cdk.aws-pinpointemail==1.98.0",
-        "aws-cdk.aws-qldb==1.98.0",
-        "aws-cdk.aws-quicksight==1.98.0",
-        "aws-cdk.aws-ram==1.98.0",
-        "aws-cdk.aws-rds==1.98.0",
-        "aws-cdk.aws-redshift==1.98.0",
-        "aws-cdk.aws-resourcegroups==1.98.0",
-        "aws-cdk.aws-robomaker==1.98.0",
-        "aws-cdk.aws-route53==1.98.0",
-        "aws-cdk.aws-route53resolver==1.98.0",
-        "aws-cdk.aws-s3==1.98.0",
-        "aws-cdk.aws-s3objectlambda==1.98.0",
-        "aws-cdk.aws-s3outposts==1.98.0",
-        "aws-cdk.aws-sagemaker==1.98.0",
-        "aws-cdk.aws-sam==1.98.0",
-        "aws-cdk.aws-sdb==1.98.0",
-        "aws-cdk.aws-secretsmanager==1.98.0",
-        "aws-cdk.aws-securityhub==1.98.0",
-        "aws-cdk.aws-servicecatalog==1.98.0",
-        "aws-cdk.aws-servicecatalogappregistry==1.98.0",
-        "aws-cdk.aws-servicediscovery==1.98.0",
-        "aws-cdk.aws-ses==1.98.0",
-        "aws-cdk.aws-signer==1.98.0",
-        "aws-cdk.aws-sns==1.98.0",
-        "aws-cdk.aws-sqs==1.98.0",
-        "aws-cdk.aws-ssm==1.98.0",
-        "aws-cdk.aws-sso==1.98.0",
-        "aws-cdk.aws-stepfunctions==1.98.0",
-        "aws-cdk.aws-synthetics==1.98.0",
-        "aws-cdk.aws-timestream==1.98.0",
-        "aws-cdk.aws-transfer==1.98.0",
-        "aws-cdk.aws-waf==1.98.0",
-        "aws-cdk.aws-wafregional==1.98.0",
-        "aws-cdk.aws-wafv2==1.98.0",
-        "aws-cdk.aws-workspaces==1.98.0",
-        "aws-cdk.core==1.98.0",
+        "aws-cdk.alexa-ask==1.99.0",
+        "aws-cdk.aws-accessanalyzer==1.99.0",
+        "aws-cdk.aws-acmpca==1.99.0",
+        "aws-cdk.aws-amazonmq==1.99.0",
+        "aws-cdk.aws-amplify==1.99.0",
+        "aws-cdk.aws-apigateway==1.99.0",
+        "aws-cdk.aws-apigatewayv2==1.99.0",
+        "aws-cdk.aws-appconfig==1.99.0",
+        "aws-cdk.aws-appflow==1.99.0",
+        "aws-cdk.aws-applicationautoscaling==1.99.0",
+        "aws-cdk.aws-applicationinsights==1.99.0",
+        "aws-cdk.aws-appmesh==1.99.0",
+        "aws-cdk.aws-appstream==1.99.0",
+        "aws-cdk.aws-appsync==1.99.0",
+        "aws-cdk.aws-athena==1.99.0",
+        "aws-cdk.aws-auditmanager==1.99.0",
+        "aws-cdk.aws-autoscaling==1.99.0",
+        "aws-cdk.aws-autoscalingplans==1.99.0",
+        "aws-cdk.aws-backup==1.99.0",
+        "aws-cdk.aws-batch==1.99.0",
+        "aws-cdk.aws-budgets==1.99.0",
+        "aws-cdk.aws-cassandra==1.99.0",
+        "aws-cdk.aws-ce==1.99.0",
+        "aws-cdk.aws-certificatemanager==1.99.0",
+        "aws-cdk.aws-chatbot==1.99.0",
+        "aws-cdk.aws-cloud9==1.99.0",
+        "aws-cdk.aws-cloudfront==1.99.0",
+        "aws-cdk.aws-cloudtrail==1.99.0",
+        "aws-cdk.aws-cloudwatch==1.99.0",
+        "aws-cdk.aws-codeartifact==1.99.0",
+        "aws-cdk.aws-codebuild==1.99.0",
+        "aws-cdk.aws-codecommit==1.99.0",
+        "aws-cdk.aws-codedeploy==1.99.0",
+        "aws-cdk.aws-codeguruprofiler==1.99.0",
+        "aws-cdk.aws-codegurureviewer==1.99.0",
+        "aws-cdk.aws-codepipeline==1.99.0",
+        "aws-cdk.aws-codestar==1.99.0",
+        "aws-cdk.aws-codestarconnections==1.99.0",
+        "aws-cdk.aws-codestarnotifications==1.99.0",
+        "aws-cdk.aws-cognito==1.99.0",
+        "aws-cdk.aws-config==1.99.0",
+        "aws-cdk.aws-databrew==1.99.0",
+        "aws-cdk.aws-datapipeline==1.99.0",
+        "aws-cdk.aws-datasync==1.99.0",
+        "aws-cdk.aws-dax==1.99.0",
+        "aws-cdk.aws-detective==1.99.0",
+        "aws-cdk.aws-devopsguru==1.99.0",
+        "aws-cdk.aws-directoryservice==1.99.0",
+        "aws-cdk.aws-dlm==1.99.0",
+        "aws-cdk.aws-dms==1.99.0",
+        "aws-cdk.aws-docdb==1.99.0",
+        "aws-cdk.aws-dynamodb==1.99.0",
+        "aws-cdk.aws-ec2==1.99.0",
+        "aws-cdk.aws-ecr==1.99.0",
+        "aws-cdk.aws-ecs==1.99.0",
+        "aws-cdk.aws-efs==1.99.0",
+        "aws-cdk.aws-eks==1.99.0",
+        "aws-cdk.aws-elasticache==1.99.0",
+        "aws-cdk.aws-elasticbeanstalk==1.99.0",
+        "aws-cdk.aws-elasticloadbalancing==1.99.0",
+        "aws-cdk.aws-elasticloadbalancingv2==1.99.0",
+        "aws-cdk.aws-elasticsearch==1.99.0",
+        "aws-cdk.aws-emr==1.99.0",
+        "aws-cdk.aws-emrcontainers==1.99.0",
+        "aws-cdk.aws-events==1.99.0",
+        "aws-cdk.aws-eventschemas==1.99.0",
+        "aws-cdk.aws-fis==1.99.0",
+        "aws-cdk.aws-fms==1.99.0",
+        "aws-cdk.aws-fsx==1.99.0",
+        "aws-cdk.aws-gamelift==1.99.0",
+        "aws-cdk.aws-globalaccelerator==1.99.0",
+        "aws-cdk.aws-glue==1.99.0",
+        "aws-cdk.aws-greengrass==1.99.0",
+        "aws-cdk.aws-greengrassv2==1.99.0",
+        "aws-cdk.aws-guardduty==1.99.0",
+        "aws-cdk.aws-iam==1.99.0",
+        "aws-cdk.aws-imagebuilder==1.99.0",
+        "aws-cdk.aws-inspector==1.99.0",
+        "aws-cdk.aws-iot1click==1.99.0",
+        "aws-cdk.aws-iot==1.99.0",
+        "aws-cdk.aws-iotanalytics==1.99.0",
+        "aws-cdk.aws-iotevents==1.99.0",
+        "aws-cdk.aws-iotsitewise==1.99.0",
+        "aws-cdk.aws-iotthingsgraph==1.99.0",
+        "aws-cdk.aws-iotwireless==1.99.0",
+        "aws-cdk.aws-ivs==1.99.0",
+        "aws-cdk.aws-kendra==1.99.0",
+        "aws-cdk.aws-kinesis==1.99.0",
+        "aws-cdk.aws-kinesisanalytics==1.99.0",
+        "aws-cdk.aws-kinesisfirehose==1.99.0",
+        "aws-cdk.aws-kms==1.99.0",
+        "aws-cdk.aws-lakeformation==1.99.0",
+        "aws-cdk.aws-lambda==1.99.0",
+        "aws-cdk.aws-licensemanager==1.99.0",
+        "aws-cdk.aws-logs==1.99.0",
+        "aws-cdk.aws-lookoutvision==1.99.0",
+        "aws-cdk.aws-macie==1.99.0",
+        "aws-cdk.aws-managedblockchain==1.99.0",
+        "aws-cdk.aws-mediaconnect==1.99.0",
+        "aws-cdk.aws-mediaconvert==1.99.0",
+        "aws-cdk.aws-medialive==1.99.0",
+        "aws-cdk.aws-mediapackage==1.99.0",
+        "aws-cdk.aws-mediastore==1.99.0",
+        "aws-cdk.aws-msk==1.99.0",
+        "aws-cdk.aws-mwaa==1.99.0",
+        "aws-cdk.aws-neptune==1.99.0",
+        "aws-cdk.aws-networkfirewall==1.99.0",
+        "aws-cdk.aws-networkmanager==1.99.0",
+        "aws-cdk.aws-opsworks==1.99.0",
+        "aws-cdk.aws-opsworkscm==1.99.0",
+        "aws-cdk.aws-pinpoint==1.99.0",
+        "aws-cdk.aws-pinpointemail==1.99.0",
+        "aws-cdk.aws-qldb==1.99.0",
+        "aws-cdk.aws-quicksight==1.99.0",
+        "aws-cdk.aws-ram==1.99.0",
+        "aws-cdk.aws-rds==1.99.0",
+        "aws-cdk.aws-redshift==1.99.0",
+        "aws-cdk.aws-resourcegroups==1.99.0",
+        "aws-cdk.aws-robomaker==1.99.0",
+        "aws-cdk.aws-route53==1.99.0",
+        "aws-cdk.aws-route53resolver==1.99.0",
+        "aws-cdk.aws-s3==1.99.0",
+        "aws-cdk.aws-s3objectlambda==1.99.0",
+        "aws-cdk.aws-s3outposts==1.99.0",
+        "aws-cdk.aws-sagemaker==1.99.0",
+        "aws-cdk.aws-sam==1.99.0",
+        "aws-cdk.aws-sdb==1.99.0",
+        "aws-cdk.aws-secretsmanager==1.99.0",
+        "aws-cdk.aws-securityhub==1.99.0",
+        "aws-cdk.aws-servicecatalog==1.99.0",
+        "aws-cdk.aws-servicecatalogappregistry==1.99.0",
+        "aws-cdk.aws-servicediscovery==1.99.0",
+        "aws-cdk.aws-ses==1.99.0",
+        "aws-cdk.aws-signer==1.99.0",
+        "aws-cdk.aws-sns==1.99.0",
+        "aws-cdk.aws-sqs==1.99.0",
+        "aws-cdk.aws-ssm==1.99.0",
+        "aws-cdk.aws-sso==1.99.0",
+        "aws-cdk.aws-stepfunctions==1.99.0",
+        "aws-cdk.aws-synthetics==1.99.0",
+        "aws-cdk.aws-timestream==1.99.0",
+        "aws-cdk.aws-transfer==1.99.0",
+        "aws-cdk.aws-waf==1.99.0",
+        "aws-cdk.aws-wafregional==1.99.0",
+        "aws-cdk.aws-wafv2==1.99.0",
+        "aws-cdk.aws-workspaces==1.99.0",
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

### Comparing `aws-cdk.cloudformation-include-1.98.0/src/aws_cdk/cloudformation_include/__init__.py` & `aws-cdk.cloudformation-include-1.99.0/src/aws_cdk/cloudformation_include/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.cloudformation-include-1.98.0/src/aws_cdk/cloudformation_include/_jsii/__init__.py` & `aws-cdk.cloudformation-include-1.99.0/src/aws_cdk/cloudformation_include/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,17 +155,17 @@
 import aws_cdk.aws_wafv2._jsii
 import aws_cdk.aws_workspaces._jsii
 import aws_cdk.core._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-cdk/cloudformation-include",
-    "1.98.0",
+    "1.99.0",
     __name__[0:-6],
-    "cloudformation-include@1.98.0.jsii.tgz",
+    "cloudformation-include@1.99.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-cdk.cloudformation-include-1.98.0/src/aws_cdk.cloudformation_include.egg-info/PKG-INFO` & `aws-cdk.cloudformation-include-1.99.0/src/aws_cdk.cloudformation_include.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cloudformation-include
-Version: 1.98.0
+Version: 1.99.0
 Summary: A package that facilitates working with existing CloudFormation templates in the CDK
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # Include CloudFormation templates in the CDK
```

### Comparing `aws-cdk.cloudformation-include-1.98.0/src/aws_cdk.cloudformation_include.egg-info/SOURCES.txt` & `aws-cdk.cloudformation-include-1.99.0/src/aws_cdk.cloudformation_include.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+LICENSE
 MANIFEST.in
+NOTICE
 README.md
 pyproject.toml
 setup.py
 src/aws_cdk.cloudformation_include.egg-info/PKG-INFO
 src/aws_cdk.cloudformation_include.egg-info/SOURCES.txt
 src/aws_cdk.cloudformation_include.egg-info/dependency_links.txt
 src/aws_cdk.cloudformation_include.egg-info/requires.txt
 src/aws_cdk.cloudformation_include.egg-info/top_level.txt
 src/aws_cdk/cloudformation_include/__init__.py
 src/aws_cdk/cloudformation_include/py.typed
 src/aws_cdk/cloudformation_include/_jsii/__init__.py
-src/aws_cdk/cloudformation_include/_jsii/cloudformation-include@1.98.0.jsii.tgz
+src/aws_cdk/cloudformation_include/_jsii/cloudformation-include@1.99.0.jsii.tgz
```

### Comparing `aws-cdk.cloudformation-include-1.98.0/src/aws_cdk.cloudformation_include.egg-info/requires.txt` & `aws-cdk.cloudformation-include-1.99.0/src/aws_cdk.cloudformation_include.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-aws-cdk.alexa-ask==1.98.0
-aws-cdk.aws-accessanalyzer==1.98.0
-aws-cdk.aws-acmpca==1.98.0
-aws-cdk.aws-amazonmq==1.98.0
-aws-cdk.aws-amplify==1.98.0
-aws-cdk.aws-apigateway==1.98.0
-aws-cdk.aws-apigatewayv2==1.98.0
-aws-cdk.aws-appconfig==1.98.0
-aws-cdk.aws-appflow==1.98.0
-aws-cdk.aws-applicationautoscaling==1.98.0
-aws-cdk.aws-applicationinsights==1.98.0
-aws-cdk.aws-appmesh==1.98.0
-aws-cdk.aws-appstream==1.98.0
-aws-cdk.aws-appsync==1.98.0
-aws-cdk.aws-athena==1.98.0
-aws-cdk.aws-auditmanager==1.98.0
-aws-cdk.aws-autoscaling==1.98.0
-aws-cdk.aws-autoscalingplans==1.98.0
-aws-cdk.aws-backup==1.98.0
-aws-cdk.aws-batch==1.98.0
-aws-cdk.aws-budgets==1.98.0
-aws-cdk.aws-cassandra==1.98.0
-aws-cdk.aws-ce==1.98.0
-aws-cdk.aws-certificatemanager==1.98.0
-aws-cdk.aws-chatbot==1.98.0
-aws-cdk.aws-cloud9==1.98.0
-aws-cdk.aws-cloudfront==1.98.0
-aws-cdk.aws-cloudtrail==1.98.0
-aws-cdk.aws-cloudwatch==1.98.0
-aws-cdk.aws-codeartifact==1.98.0
-aws-cdk.aws-codebuild==1.98.0
-aws-cdk.aws-codecommit==1.98.0
-aws-cdk.aws-codedeploy==1.98.0
-aws-cdk.aws-codeguruprofiler==1.98.0
-aws-cdk.aws-codegurureviewer==1.98.0
-aws-cdk.aws-codepipeline==1.98.0
-aws-cdk.aws-codestar==1.98.0
-aws-cdk.aws-codestarconnections==1.98.0
-aws-cdk.aws-codestarnotifications==1.98.0
-aws-cdk.aws-cognito==1.98.0
-aws-cdk.aws-config==1.98.0
-aws-cdk.aws-databrew==1.98.0
-aws-cdk.aws-datapipeline==1.98.0
-aws-cdk.aws-datasync==1.98.0
-aws-cdk.aws-dax==1.98.0
-aws-cdk.aws-detective==1.98.0
-aws-cdk.aws-devopsguru==1.98.0
-aws-cdk.aws-directoryservice==1.98.0
-aws-cdk.aws-dlm==1.98.0
-aws-cdk.aws-dms==1.98.0
-aws-cdk.aws-docdb==1.98.0
-aws-cdk.aws-dynamodb==1.98.0
-aws-cdk.aws-ec2==1.98.0
-aws-cdk.aws-ecr==1.98.0
-aws-cdk.aws-ecs==1.98.0
-aws-cdk.aws-efs==1.98.0
-aws-cdk.aws-eks==1.98.0
-aws-cdk.aws-elasticache==1.98.0
-aws-cdk.aws-elasticbeanstalk==1.98.0
-aws-cdk.aws-elasticloadbalancing==1.98.0
-aws-cdk.aws-elasticloadbalancingv2==1.98.0
-aws-cdk.aws-elasticsearch==1.98.0
-aws-cdk.aws-emr==1.98.0
-aws-cdk.aws-emrcontainers==1.98.0
-aws-cdk.aws-events==1.98.0
-aws-cdk.aws-eventschemas==1.98.0
-aws-cdk.aws-fis==1.98.0
-aws-cdk.aws-fms==1.98.0
-aws-cdk.aws-fsx==1.98.0
-aws-cdk.aws-gamelift==1.98.0
-aws-cdk.aws-globalaccelerator==1.98.0
-aws-cdk.aws-glue==1.98.0
-aws-cdk.aws-greengrass==1.98.0
-aws-cdk.aws-greengrassv2==1.98.0
-aws-cdk.aws-guardduty==1.98.0
-aws-cdk.aws-iam==1.98.0
-aws-cdk.aws-imagebuilder==1.98.0
-aws-cdk.aws-inspector==1.98.0
-aws-cdk.aws-iot1click==1.98.0
-aws-cdk.aws-iot==1.98.0
-aws-cdk.aws-iotanalytics==1.98.0
-aws-cdk.aws-iotevents==1.98.0
-aws-cdk.aws-iotsitewise==1.98.0
-aws-cdk.aws-iotthingsgraph==1.98.0
-aws-cdk.aws-iotwireless==1.98.0
-aws-cdk.aws-ivs==1.98.0
-aws-cdk.aws-kendra==1.98.0
-aws-cdk.aws-kinesis==1.98.0
-aws-cdk.aws-kinesisanalytics==1.98.0
-aws-cdk.aws-kinesisfirehose==1.98.0
-aws-cdk.aws-kms==1.98.0
-aws-cdk.aws-lakeformation==1.98.0
-aws-cdk.aws-lambda==1.98.0
-aws-cdk.aws-licensemanager==1.98.0
-aws-cdk.aws-logs==1.98.0
-aws-cdk.aws-lookoutvision==1.98.0
-aws-cdk.aws-macie==1.98.0
-aws-cdk.aws-managedblockchain==1.98.0
-aws-cdk.aws-mediaconnect==1.98.0
-aws-cdk.aws-mediaconvert==1.98.0
-aws-cdk.aws-medialive==1.98.0
-aws-cdk.aws-mediapackage==1.98.0
-aws-cdk.aws-mediastore==1.98.0
-aws-cdk.aws-msk==1.98.0
-aws-cdk.aws-mwaa==1.98.0
-aws-cdk.aws-neptune==1.98.0
-aws-cdk.aws-networkfirewall==1.98.0
-aws-cdk.aws-networkmanager==1.98.0
-aws-cdk.aws-opsworks==1.98.0
-aws-cdk.aws-opsworkscm==1.98.0
-aws-cdk.aws-pinpoint==1.98.0
-aws-cdk.aws-pinpointemail==1.98.0
-aws-cdk.aws-qldb==1.98.0
-aws-cdk.aws-quicksight==1.98.0
-aws-cdk.aws-ram==1.98.0
-aws-cdk.aws-rds==1.98.0
-aws-cdk.aws-redshift==1.98.0
-aws-cdk.aws-resourcegroups==1.98.0
-aws-cdk.aws-robomaker==1.98.0
-aws-cdk.aws-route53==1.98.0
-aws-cdk.aws-route53resolver==1.98.0
-aws-cdk.aws-s3==1.98.0
-aws-cdk.aws-s3objectlambda==1.98.0
-aws-cdk.aws-s3outposts==1.98.0
-aws-cdk.aws-sagemaker==1.98.0
-aws-cdk.aws-sam==1.98.0
-aws-cdk.aws-sdb==1.98.0
-aws-cdk.aws-secretsmanager==1.98.0
-aws-cdk.aws-securityhub==1.98.0
-aws-cdk.aws-servicecatalog==1.98.0
-aws-cdk.aws-servicecatalogappregistry==1.98.0
-aws-cdk.aws-servicediscovery==1.98.0
-aws-cdk.aws-ses==1.98.0
-aws-cdk.aws-signer==1.98.0
-aws-cdk.aws-sns==1.98.0
-aws-cdk.aws-sqs==1.98.0
-aws-cdk.aws-ssm==1.98.0
-aws-cdk.aws-sso==1.98.0
-aws-cdk.aws-stepfunctions==1.98.0
-aws-cdk.aws-synthetics==1.98.0
-aws-cdk.aws-timestream==1.98.0
-aws-cdk.aws-transfer==1.98.0
-aws-cdk.aws-waf==1.98.0
-aws-cdk.aws-wafregional==1.98.0
-aws-cdk.aws-wafv2==1.98.0
-aws-cdk.aws-workspaces==1.98.0
-aws-cdk.core==1.98.0
+aws-cdk.alexa-ask==1.99.0
+aws-cdk.aws-accessanalyzer==1.99.0
+aws-cdk.aws-acmpca==1.99.0
+aws-cdk.aws-amazonmq==1.99.0
+aws-cdk.aws-amplify==1.99.0
+aws-cdk.aws-apigateway==1.99.0
+aws-cdk.aws-apigatewayv2==1.99.0
+aws-cdk.aws-appconfig==1.99.0
+aws-cdk.aws-appflow==1.99.0
+aws-cdk.aws-applicationautoscaling==1.99.0
+aws-cdk.aws-applicationinsights==1.99.0
+aws-cdk.aws-appmesh==1.99.0
+aws-cdk.aws-appstream==1.99.0
+aws-cdk.aws-appsync==1.99.0
+aws-cdk.aws-athena==1.99.0
+aws-cdk.aws-auditmanager==1.99.0
+aws-cdk.aws-autoscaling==1.99.0
+aws-cdk.aws-autoscalingplans==1.99.0
+aws-cdk.aws-backup==1.99.0
+aws-cdk.aws-batch==1.99.0
+aws-cdk.aws-budgets==1.99.0
+aws-cdk.aws-cassandra==1.99.0
+aws-cdk.aws-ce==1.99.0
+aws-cdk.aws-certificatemanager==1.99.0
+aws-cdk.aws-chatbot==1.99.0
+aws-cdk.aws-cloud9==1.99.0
+aws-cdk.aws-cloudfront==1.99.0
+aws-cdk.aws-cloudtrail==1.99.0
+aws-cdk.aws-cloudwatch==1.99.0
+aws-cdk.aws-codeartifact==1.99.0
+aws-cdk.aws-codebuild==1.99.0
+aws-cdk.aws-codecommit==1.99.0
+aws-cdk.aws-codedeploy==1.99.0
+aws-cdk.aws-codeguruprofiler==1.99.0
+aws-cdk.aws-codegurureviewer==1.99.0
+aws-cdk.aws-codepipeline==1.99.0
+aws-cdk.aws-codestar==1.99.0
+aws-cdk.aws-codestarconnections==1.99.0
+aws-cdk.aws-codestarnotifications==1.99.0
+aws-cdk.aws-cognito==1.99.0
+aws-cdk.aws-config==1.99.0
+aws-cdk.aws-databrew==1.99.0
+aws-cdk.aws-datapipeline==1.99.0
+aws-cdk.aws-datasync==1.99.0
+aws-cdk.aws-dax==1.99.0
+aws-cdk.aws-detective==1.99.0
+aws-cdk.aws-devopsguru==1.99.0
+aws-cdk.aws-directoryservice==1.99.0
+aws-cdk.aws-dlm==1.99.0
+aws-cdk.aws-dms==1.99.0
+aws-cdk.aws-docdb==1.99.0
+aws-cdk.aws-dynamodb==1.99.0
+aws-cdk.aws-ec2==1.99.0
+aws-cdk.aws-ecr==1.99.0
+aws-cdk.aws-ecs==1.99.0
+aws-cdk.aws-efs==1.99.0
+aws-cdk.aws-eks==1.99.0
+aws-cdk.aws-elasticache==1.99.0
+aws-cdk.aws-elasticbeanstalk==1.99.0
+aws-cdk.aws-elasticloadbalancing==1.99.0
+aws-cdk.aws-elasticloadbalancingv2==1.99.0
+aws-cdk.aws-elasticsearch==1.99.0
+aws-cdk.aws-emr==1.99.0
+aws-cdk.aws-emrcontainers==1.99.0
+aws-cdk.aws-events==1.99.0
+aws-cdk.aws-eventschemas==1.99.0
+aws-cdk.aws-fis==1.99.0
+aws-cdk.aws-fms==1.99.0
+aws-cdk.aws-fsx==1.99.0
+aws-cdk.aws-gamelift==1.99.0
+aws-cdk.aws-globalaccelerator==1.99.0
+aws-cdk.aws-glue==1.99.0
+aws-cdk.aws-greengrass==1.99.0
+aws-cdk.aws-greengrassv2==1.99.0
+aws-cdk.aws-guardduty==1.99.0
+aws-cdk.aws-iam==1.99.0
+aws-cdk.aws-imagebuilder==1.99.0
+aws-cdk.aws-inspector==1.99.0
+aws-cdk.aws-iot1click==1.99.0
+aws-cdk.aws-iot==1.99.0
+aws-cdk.aws-iotanalytics==1.99.0
+aws-cdk.aws-iotevents==1.99.0
+aws-cdk.aws-iotsitewise==1.99.0
+aws-cdk.aws-iotthingsgraph==1.99.0
+aws-cdk.aws-iotwireless==1.99.0
+aws-cdk.aws-ivs==1.99.0
+aws-cdk.aws-kendra==1.99.0
+aws-cdk.aws-kinesis==1.99.0
+aws-cdk.aws-kinesisanalytics==1.99.0
+aws-cdk.aws-kinesisfirehose==1.99.0
+aws-cdk.aws-kms==1.99.0
+aws-cdk.aws-lakeformation==1.99.0
+aws-cdk.aws-lambda==1.99.0
+aws-cdk.aws-licensemanager==1.99.0
+aws-cdk.aws-logs==1.99.0
+aws-cdk.aws-lookoutvision==1.99.0
+aws-cdk.aws-macie==1.99.0
+aws-cdk.aws-managedblockchain==1.99.0
+aws-cdk.aws-mediaconnect==1.99.0
+aws-cdk.aws-mediaconvert==1.99.0
+aws-cdk.aws-medialive==1.99.0
+aws-cdk.aws-mediapackage==1.99.0
+aws-cdk.aws-mediastore==1.99.0
+aws-cdk.aws-msk==1.99.0
+aws-cdk.aws-mwaa==1.99.0
+aws-cdk.aws-neptune==1.99.0
+aws-cdk.aws-networkfirewall==1.99.0
+aws-cdk.aws-networkmanager==1.99.0
+aws-cdk.aws-opsworks==1.99.0
+aws-cdk.aws-opsworkscm==1.99.0
+aws-cdk.aws-pinpoint==1.99.0
+aws-cdk.aws-pinpointemail==1.99.0
+aws-cdk.aws-qldb==1.99.0
+aws-cdk.aws-quicksight==1.99.0
+aws-cdk.aws-ram==1.99.0
+aws-cdk.aws-rds==1.99.0
+aws-cdk.aws-redshift==1.99.0
+aws-cdk.aws-resourcegroups==1.99.0
+aws-cdk.aws-robomaker==1.99.0
+aws-cdk.aws-route53==1.99.0
+aws-cdk.aws-route53resolver==1.99.0
+aws-cdk.aws-s3==1.99.0
+aws-cdk.aws-s3objectlambda==1.99.0
+aws-cdk.aws-s3outposts==1.99.0
+aws-cdk.aws-sagemaker==1.99.0
+aws-cdk.aws-sam==1.99.0
+aws-cdk.aws-sdb==1.99.0
+aws-cdk.aws-secretsmanager==1.99.0
+aws-cdk.aws-securityhub==1.99.0
+aws-cdk.aws-servicecatalog==1.99.0
+aws-cdk.aws-servicecatalogappregistry==1.99.0
+aws-cdk.aws-servicediscovery==1.99.0
+aws-cdk.aws-ses==1.99.0
+aws-cdk.aws-signer==1.99.0
+aws-cdk.aws-sns==1.99.0
+aws-cdk.aws-sqs==1.99.0
+aws-cdk.aws-ssm==1.99.0
+aws-cdk.aws-sso==1.99.0
+aws-cdk.aws-stepfunctions==1.99.0
+aws-cdk.aws-synthetics==1.99.0
+aws-cdk.aws-timestream==1.99.0
+aws-cdk.aws-transfer==1.99.0
+aws-cdk.aws-waf==1.99.0
+aws-cdk.aws-wafregional==1.99.0
+aws-cdk.aws-wafv2==1.99.0
+aws-cdk.aws-workspaces==1.99.0
+aws-cdk.core==1.99.0
 constructs<4.0.0,>=3.3.69
-jsii<2.0.0,>=1.27.0
+jsii<2.0.0,>=1.28.0
 publication>=0.0.3
```

