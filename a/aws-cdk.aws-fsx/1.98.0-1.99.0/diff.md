# Comparing `tmp/aws-cdk.aws-fsx-1.98.0.tar.gz` & `tmp/aws-cdk.aws-fsx-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src518022412/src/packages/@aws-cdk/aws-fsx/dist/python/aws-cdk.aws-fsx-1.98.0.tar", last modified: Mon Apr 12 10:09:05 2021, max compression
+gzip compressed data, was "/codebuild/output/src875002972/src/packages/@aws-cdk/aws-fsx/dist/python/aws-cdk.aws-fsx-1.99.0.tar", last modified: Tue Apr 13 17:03:15 2021, max compression
```

## Comparing `aws-cdk.aws-fsx-1.98.0.tar` & `aws-cdk.aws-fsx-1.99.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/
--rw-r--r--   0 root         (0) root         (0)       23 2021-04-12 10:07:22.000000 aws-cdk.aws-fsx-1.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8878 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6656 2021-04-12 10:07:22.000000 aws-cdk.aws-fsx-1.98.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-04-12 10:07:22.000000 aws-cdk.aws-fsx-1.98.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1833 2021-04-12 10:07:22.000000 aws-cdk.aws-fsx-1.98.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk/aws_fsx/
--rw-r--r--   0 root         (0) root         (0)    90927 2021-04-12 10:07:22.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk/aws_fsx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk/aws_fsx/_jsii/
--rw-r--r--   0 root         (0) root         (0)      450 2021-04-12 10:07:22.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk/aws_fsx/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51500 2021-04-12 10:07:20.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk/aws_fsx/_jsii/aws-fsx@1.98.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:07:22.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk/aws_fsx/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk.aws_fsx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8878 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk.aws_fsx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      408 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk.aws_fsx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk.aws_fsx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      158 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk.aws_fsx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-04-12 10:09:05.000000 aws-cdk.aws-fsx-1.98.0/src/aws_cdk.aws_fsx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2021-04-13 17:02:04.000000 aws-cdk.aws-fsx-1.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-04-13 17:02:05.000000 aws-cdk.aws-fsx-1.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2021-04-13 17:02:04.000000 aws-cdk.aws-fsx-1.99.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8878 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6656 2021-04-13 17:02:05.000000 aws-cdk.aws-fsx-1.99.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-04-13 17:02:05.000000 aws-cdk.aws-fsx-1.99.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1833 2021-04-13 17:02:05.000000 aws-cdk.aws-fsx-1.99.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk/aws_fsx/
+-rw-r--r--   0 root         (0) root         (0)    90927 2021-04-13 17:02:05.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk/aws_fsx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk/aws_fsx/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      450 2021-04-13 17:02:05.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk/aws_fsx/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51485 2021-04-13 17:02:03.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk/aws_fsx/_jsii/aws-fsx@1.99.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:02:05.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk/aws_fsx/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk.aws_fsx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8878 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk.aws_fsx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      423 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk.aws_fsx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk.aws_fsx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk.aws_fsx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2021-04-13 17:03:15.000000 aws-cdk.aws-fsx-1.99.0/src/aws_cdk.aws_fsx.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-fsx-1.98.0/PKG-INFO` & `aws-cdk.aws-fsx-1.99.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-fsx
-Version: 1.98.0
+Version: 1.99.0
 Summary: The CDK Construct Library for AWS::FSx
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # Amazon FSx Construct Library
```

### Comparing `aws-cdk.aws-fsx-1.98.0/README.md` & `aws-cdk.aws-fsx-1.99.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-fsx-1.98.0/setup.py` & `aws-cdk.aws-fsx-1.99.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-fsx",
-    "version": "1.98.0",
+    "version": "1.99.0",
     "description": "The CDK Construct Library for AWS::FSx",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,28 +22,28 @@
     },
     "packages": [
         "aws_cdk.aws_fsx",
         "aws_cdk.aws_fsx._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_fsx._jsii": [
-            "aws-fsx@1.98.0.jsii.tgz"
+            "aws-fsx@1.99.0.jsii.tgz"
         ],
         "aws_cdk.aws_fsx": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk.aws-ec2==1.98.0",
-        "aws-cdk.aws-iam==1.98.0",
-        "aws-cdk.aws-kms==1.98.0",
-        "aws-cdk.core==1.98.0",
+        "aws-cdk.aws-ec2==1.99.0",
+        "aws-cdk.aws-iam==1.99.0",
+        "aws-cdk.aws-kms==1.99.0",
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

### Comparing `aws-cdk.aws-fsx-1.98.0/src/aws_cdk/aws_fsx/__init__.py` & `aws-cdk.aws-fsx-1.99.0/src/aws_cdk/aws_fsx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1301,15 +1301,15 @@
         '''The configuration for the Amazon FSx for Lustre file system.
 
         :param deployment_type: The type of backing file system deployment used by FSx.
         :param export_path: The path in Amazon S3 where the root of your Amazon FSx file system is exported. The path must use the same Amazon S3 bucket as specified in ImportPath. If you only specify a bucket name, such as s3://import-bucket, you get a 1:1 mapping of file system objects to S3 bucket objects. This mapping means that the input data in S3 is overwritten on export. If you provide a custom prefix in the export path, such as s3://import-bucket/[custom-optional-prefix], Amazon FSx exports the contents of your file system to that export prefix in the Amazon S3 bucket. Default: s3://import-bucket/FSxLustre[creation-timestamp]
         :param imported_file_chunk_size_mib: For files imported from a data repository, this value determines the stripe count and maximum amount of data per file (in MiB) stored on a single physical disk. Allowed values are between 1 and 512,000. Default: 1024
         :param import_path: The path to the Amazon S3 bucket (including the optional prefix) that you're using as the data repository for your Amazon FSx for Lustre file system. Must be of the format "s3://{bucketName}/optional-prefix" and cannot exceed 900 characters. Default: - no bucket is imported
         :param per_unit_storage_throughput: Required for the PERSISTENT_1 deployment type, describes the amount of read and write throughput for each 1 tebibyte of storage, in MB/s/TiB. Valid values are 50, 100, 200. Default: - no default, conditionally required for PERSISTENT_1 deployment type
-        :param weekly_maintenance_start_time: The preferred day and time to perform weekly maintenance. The first digit is the day of the week, starting at 0 for Sunday, then the following are hours and minutes in the UTC time zone, 24 hour clock. For example: '2:20:30' is Tuesdays at 20:30. Default: - no preference
+        :param weekly_maintenance_start_time: The preferred day and time to perform weekly maintenance. The first digit is the day of the week, starting at 1 for Monday, then the following are hours and minutes in the UTC time zone, 24 hour clock. For example: '2:20:30' is Tuesdays at 20:30. Default: - no preference
 
         :see: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-fsx-filesystem-lustreconfiguration.html
         '''
         self._values: typing.Dict[str, typing.Any] = {
             "deployment_type": deployment_type,
         }
         if export_path is not None:
@@ -1380,16 +1380,16 @@
         result = self._values.get("per_unit_storage_throughput")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def weekly_maintenance_start_time(self) -> typing.Optional["LustreMaintenanceTime"]:
         '''The preferred day and time to perform weekly maintenance.
 
-        The first digit is the day of the week, starting at 0
-        for Sunday, then the following are hours and minutes in the UTC time zone, 24 hour clock. For example: '2:20:30'
+        The first digit is the day of the week, starting at 1
+        for Monday, then the following are hours and minutes in the UTC time zone, 24 hour clock. For example: '2:20:30'
         is Tuesdays at 20:30.
 
         :default: - no preference
         '''
         result = self._values.get("weekly_maintenance_start_time")
         return typing.cast(typing.Optional["LustreMaintenanceTime"], result)
 
@@ -1651,28 +1651,28 @@
         )
 
 
 @jsii.enum(jsii_type="@aws-cdk/aws-fsx.Weekday")
 class Weekday(enum.Enum):
     '''Enum for representing all the days of the week.'''
 
-    SUNDAY = "SUNDAY"
-    '''Sunday.'''
     MONDAY = "MONDAY"
     '''Monday.'''
     TUESDAY = "TUESDAY"
     '''Tuesday.'''
     WEDNESDAY = "WEDNESDAY"
     '''Wednesday.'''
     THURSDAY = "THURSDAY"
     '''Thursday.'''
     FRIDAY = "FRIDAY"
     '''Friday.'''
     SATURDAY = "SATURDAY"
     '''Saturday.'''
+    SUNDAY = "SUNDAY"
+    '''Sunday.'''
 
 
 @jsii.implements(IFileSystem)
 class FileSystemBase(
     aws_cdk.core.Resource,
     metaclass=jsii.JSIIAbstractClass,
     jsii_type="@aws-cdk/aws-fsx.FileSystemBase",
```

### Comparing `aws-cdk.aws-fsx-1.98.0/src/aws_cdk.aws_fsx.egg-info/PKG-INFO` & `aws-cdk.aws-fsx-1.99.0/src/aws_cdk.aws_fsx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-fsx
-Version: 1.98.0
+Version: 1.99.0
 Summary: The CDK Construct Library for AWS::FSx
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Description: # Amazon FSx Construct Library
```

