# Comparing `tmp/dynamodump-1.8.0.tar.gz` & `tmp/dynamodump-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamodump-1.8.0.tar", last modified: Thu Feb 23 01:03:06 2023, max compression
+gzip compressed data, was "dynamodump-1.9.0.tar", last modified: Thu May 11 07:09:54 2023, max compression
```

## Comparing `dynamodump-1.8.0.tar` & `dynamodump-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:03:06.326069 dynamodump-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-02-23 01:02:57.000000 dynamodump-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-02-23 01:03:06.326069 dynamodump-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-02-23 01:02:57.000000 dynamodump-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:03:06.326069 dynamodump-1.8.0/dynamodump/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 01:02:57.000000 dynamodump-1.8.0/dynamodump/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54195 2023-02-23 01:02:57.000000 dynamodump-1.8.0/dynamodump/dynamodump.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:03:06.326069 dynamodump-1.8.0/dynamodump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-02-23 01:03:06.000000 dynamodump-1.8.0/dynamodump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-23 01:03:06.000000 dynamodump-1.8.0/dynamodump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 01:03:06.000000 dynamodump-1.8.0/dynamodump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-23 01:03:06.000000 dynamodump-1.8.0/dynamodump.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-23 01:03:06.000000 dynamodump-1.8.0/dynamodump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-23 01:03:06.000000 dynamodump-1.8.0/dynamodump.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-23 01:02:57.000000 dynamodump-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 01:03:06.326069 dynamodump-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-02-23 01:02:57.000000 dynamodump-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 01:03:06.326069 dynamodump-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-02-23 01:02:57.000000 dynamodump-1.8.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:09:54.685798 dynamodump-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-11 07:09:45.000000 dynamodump-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-05-11 07:09:54.685798 dynamodump-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-11 07:09:45.000000 dynamodump-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:09:54.681798 dynamodump-1.9.0/dynamodump/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 07:09:45.000000 dynamodump-1.9.0/dynamodump/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55221 2023-05-11 07:09:45.000000 dynamodump-1.9.0/dynamodump/dynamodump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:09:54.685798 dynamodump-1.9.0/dynamodump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-05-11 07:09:54.000000 dynamodump-1.9.0/dynamodump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-11 07:09:54.000000 dynamodump-1.9.0/dynamodump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 07:09:54.000000 dynamodump-1.9.0/dynamodump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 07:09:54.000000 dynamodump-1.9.0/dynamodump.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 07:09:54.000000 dynamodump-1.9.0/dynamodump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 07:09:54.000000 dynamodump-1.9.0/dynamodump.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 07:09:45.000000 dynamodump-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 07:09:54.685798 dynamodump-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-11 07:09:45.000000 dynamodump-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:09:54.685798 dynamodump-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-11 07:09:45.000000 dynamodump-1.9.0/tests/test.py
```

### Comparing `dynamodump-1.8.0/LICENSE` & `dynamodump-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamodump-1.8.0/PKG-INFO` & `dynamodump-1.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: dynamodump
-Version: 1.8.0
-Summary: Simple backup and restore for Amazon DynamoDB using AWS SDK for Python (boto3)
-Home-page: https://github.com/bchew/dynamodump
-Author: Benny Chew
-Author-email: noreply@bennychew.com
-Project-URL: Releases, https://github.com/bchew/dynamodump/releases
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dynamodump
 
 ![Build Status](https://github.com/bchew/dynamodump/actions/workflows/build.yml/badge.svg)
 ![CodeQL Status](https://github.com/bchew/dynamodump/actions/workflows/codeql-analysis.yml/badge.svg)
 [![Docker Status](https://github.com/bchew/dynamodump/actions/workflows/docker.yml/badge.svg)](https://hub.docker.com/r/bchew/dynamodump)
 ![Linting Status](https://github.com/bchew/dynamodump/actions/workflows/linting.yml/badge.svg)
 ![Test Status](https://github.com/bchew/dynamodump/actions/workflows/test.yml/badge.svg)
@@ -25,15 +11,14 @@
 
 Simple backup and restore script for Amazon DynamoDB using AWS SDK for Python (boto3) to work similarly to mysqldump.
 
 Suitable for DynamoDB usages of smaller data volume which do not warrant the usage of AWS Data Pipeline for backup/restores/empty.
 
 dynamodump supports local DynamoDB instances as well (tested with [DynamoDB Local](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.html)).
 
-
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Script (unattended) usage](#script-unattended-usage)
 - [Docker CLI usage](#docker-cli-usage)
 - [AWS example](#aws-example)
@@ -45,90 +30,60 @@
 ```
 pip install dynamodump
 ```
 
 ## Usage
 
 ```
-usage: dynamodump [-h] [-a {zip,tar}] [-b BUCKET]
-                     [-m {backup,restore,empty}] [-r REGION] [--host HOST]
-                     [--port PORT] [--accessKey ACCESSKEY]
-                     [--secretKey SECRETKEY] [-p PROFILE] [-s SRCTABLE]
-                     [-d DESTTABLE] [--prefixSeparator PREFIXSEPARATOR]
-                     [--noSeparator] [--readCapacity READCAPACITY] [-t TAG]
-                     [--writeCapacity WRITECAPACITY] [--schemaOnly]
-                     [--dataOnly] [--noConfirm] [--skipThroughputUpdate]
-                     [--billingMode BILLING_MODE] [--dumpPath DUMPPATH] [--log LOG]
-                     [-f FILTEROPTION]
+usage: dynamodump.py [-h] [-a {zip,tar}] [-b BUCKET] [-m {backup,restore,empty}] [-r REGION] [--host HOST] [--port PORT] [--accessKey ACCESSKEY] [--secretKey SECRETKEY] [-p PROFILE] [-s SRCTABLE] [-d DESTTABLE]
+                     [--prefixSeparator PREFIXSEPARATOR] [--noSeparator] [--readCapacity READCAPACITY] [-t TAG] [--writeCapacity WRITECAPACITY] [--schemaOnly] [--dataOnly] [--noConfirm] [--skipThroughputUpdate]
+                     [--dumpPath DUMPPATH] [--billingMode {PROVISIONED,PAY_PER_REQUEST}] [--log LOG] [--limit LIMIT] [-f FILTEROPTION]
 
 Simple DynamoDB backup/restore/empty.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -a {zip,tar}, --archive {zip,tar}
-                        Type of compressed archive to create.If unset, don't
-                        create archive
+                        Type of compressed archive to create. If unset, don't create archive
   -b BUCKET, --bucket BUCKET
-                        S3 bucket in which to store or retrieve backups.[must
-                        already exist]
+                        S3 bucket in which to store or retrieve backups. [must already exist]
   -m {backup,restore,empty}, --mode {backup,restore,empty}
                         Operation to perform
   -r REGION, --region REGION
-                        AWS region to use, e.g. 'us-west-1'. Can use
-                        AWS_DEFAULT_REGION for local testing. Use 'local' for
-                        local DynamoDB testing
-  --host HOST           Host of local DynamoDB [required only for local]
+                        AWS region to use, e.g. 'us-west-1'. Can use any region for local testing
+  --host HOST           Host of local DynamoDB. This parameter initialises dynamodump for local DynamoDB testing [required only for local]
   --port PORT           Port of local DynamoDB [required only for local]
   --accessKey ACCESSKEY
                         Access key of local DynamoDB [required only for local]
   --secretKey SECRETKEY
                         Secret key of local DynamoDB [required only for local]
   -p PROFILE, --profile PROFILE
-                        AWS credentials file profile to use. Allows you to use
-                        a profile instead accessKey, secretKey authentication
+                        AWS credentials file profile to use. Allows you to use a profile instead accessKey, secretKey authentication
   -s SRCTABLE, --srcTable SRCTABLE
-                        Source DynamoDB table name to backup or restore from,
-                        use 'tablename*' for wildcard prefix selection or '*'
-                        for all tables. Mutually exclusive with --tag
+                        Source DynamoDB table name to backup or restore from, use 'tablename*' for wildcard prefix selection or '*' for all tables. Mutually exclusive with --tag
   -d DESTTABLE, --destTable DESTTABLE
-                        Destination DynamoDB table name to backup or restore
-                        to, use 'tablename*' for wildcard prefix selection
-                        (defaults to use '-' separator) [optional, defaults to
-                        source]
+                        Destination DynamoDB table name to backup or restore to, use 'tablename*' for wildcard prefix selection (defaults to use '-' separator) [optional, defaults to source]
   --prefixSeparator PREFIXSEPARATOR
-                        Specify a different prefix separator, e.g. '.'
-                        [optional]
-  --noSeparator         Overrides the use of a prefix separator for backup
-                        wildcard searches [optional]
+                        Specify a different prefix separator, e.g. '.' [optional]
+  --noSeparator         Overrides the use of a prefix separator for backup wildcard searches [optional]
   --readCapacity READCAPACITY
-                        Change the temp read capacity of the DynamoDB table to
-                        backup from [optional]
-  -t TAG, --tag TAG     Tag to use for identifying tables to back up. Mutually
-                        exclusive with srcTable. Provided as KEY=VALUE
+                        Change the temp read capacity of the DynamoDB table to backup from [optional]
+  -t TAG, --tag TAG     Tag to use for identifying tables to back up. Mutually exclusive with srcTable. Provided as KEY=VALUE
   --writeCapacity WRITECAPACITY
-                        Change the temp write capacity of the DynamoDB table
-                        to restore to [defaults to 25, optional]
-  --schemaOnly          Backup or restore the schema only. Do not
-                        backup/restore data. Can be used with both backup and
-                        restore modes. Cannot be used with the --dataOnly
-                        [optional]
-  --dataOnly            Restore data only. Do not delete/recreate schema
-                        [optional for restore]
-  --noConfirm           Don't ask for confirmation before deleting existing
-                        schemas.
+                        Change the temp write capacity of the DynamoDB table to restore to [defaults to 25, optional]
+  --schemaOnly          Backup or restore the schema only. Do not backup/restore data. Can be used with both backup and restore modes. Cannot be used with the --dataOnly [optional]
+  --dataOnly            Restore data only. Do not delete/recreate schema [optional for restore]
+  --noConfirm           Don't ask for confirmation before deleting existing schemas.
   --skipThroughputUpdate
-                        Skip updating throughput values across tables
-                        [optional]
-  --billingMode BILLING_MODE
-                        Set billing mode between PROVISIONED|PAY_PER_REQUEST
-                        (defaults to use 'PROVISIONED') [optional]
-  --dumpPath DUMPPATH   Directory to place and search for DynamoDB table
-                        backups (defaults to use 'dump') [optional]
-  --log LOG             Logging level - DEBUG|INFO|WARNING|ERROR|CRITICAL
-                        [optional]
+                        Skip updating throughput values across tables [optional]
+  --dumpPath DUMPPATH   Directory to place and search for DynamoDB table backups (defaults to use 'dump') [optional]
+  --billingMode {PROVISIONED,PAY_PER_REQUEST}
+                        Set billing mode between PROVISIONED|PAY_PER_REQUEST (defaults to use 'PROVISIONED') [optional]
+  --log LOG             Logging level - DEBUG|INFO|WARNING|ERROR|CRITICAL [optional]
+  --limit LIMIT         Limit option for backup, will stop the back up process after number of backed up items reaches the limit [optional]
   -f FILTEROPTION, --filterOption FILTEROPTION
                         Filter option for backup, JSON file of which keys are ['FilterExpression', 'ExpressionAttributeNames', 'ExpressionAttributeValues']
 ```
 
 Backup files are stored in a 'dump' subdirectory, and are restored from there as well by default.
 
 ## Script (unattended) usage
```

### Comparing `dynamodump-1.8.0/README.md` & `dynamodump-1.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: dynamodump
+Version: 1.9.0
+Summary: Simple backup and restore for Amazon DynamoDB using AWS SDK for Python (boto3)
+Home-page: https://github.com/bchew/dynamodump
+Author: Benny Chew
+Author-email: noreply@bennychew.com
+Project-URL: Releases, https://github.com/bchew/dynamodump/releases
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # dynamodump
 
 ![Build Status](https://github.com/bchew/dynamodump/actions/workflows/build.yml/badge.svg)
 ![CodeQL Status](https://github.com/bchew/dynamodump/actions/workflows/codeql-analysis.yml/badge.svg)
 [![Docker Status](https://github.com/bchew/dynamodump/actions/workflows/docker.yml/badge.svg)](https://hub.docker.com/r/bchew/dynamodump)
 ![Linting Status](https://github.com/bchew/dynamodump/actions/workflows/linting.yml/badge.svg)
 ![Test Status](https://github.com/bchew/dynamodump/actions/workflows/test.yml/badge.svg)
@@ -11,15 +25,14 @@
 
 Simple backup and restore script for Amazon DynamoDB using AWS SDK for Python (boto3) to work similarly to mysqldump.
 
 Suitable for DynamoDB usages of smaller data volume which do not warrant the usage of AWS Data Pipeline for backup/restores/empty.
 
 dynamodump supports local DynamoDB instances as well (tested with [DynamoDB Local](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.html)).
 
-
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Script (unattended) usage](#script-unattended-usage)
 - [Docker CLI usage](#docker-cli-usage)
 - [AWS example](#aws-example)
@@ -31,90 +44,60 @@
 ```
 pip install dynamodump
 ```
 
 ## Usage
 
 ```
-usage: dynamodump [-h] [-a {zip,tar}] [-b BUCKET]
-                     [-m {backup,restore,empty}] [-r REGION] [--host HOST]
-                     [--port PORT] [--accessKey ACCESSKEY]
-                     [--secretKey SECRETKEY] [-p PROFILE] [-s SRCTABLE]
-                     [-d DESTTABLE] [--prefixSeparator PREFIXSEPARATOR]
-                     [--noSeparator] [--readCapacity READCAPACITY] [-t TAG]
-                     [--writeCapacity WRITECAPACITY] [--schemaOnly]
-                     [--dataOnly] [--noConfirm] [--skipThroughputUpdate]
-                     [--billingMode BILLING_MODE] [--dumpPath DUMPPATH] [--log LOG]
-                     [-f FILTEROPTION]
+usage: dynamodump.py [-h] [-a {zip,tar}] [-b BUCKET] [-m {backup,restore,empty}] [-r REGION] [--host HOST] [--port PORT] [--accessKey ACCESSKEY] [--secretKey SECRETKEY] [-p PROFILE] [-s SRCTABLE] [-d DESTTABLE]
+                     [--prefixSeparator PREFIXSEPARATOR] [--noSeparator] [--readCapacity READCAPACITY] [-t TAG] [--writeCapacity WRITECAPACITY] [--schemaOnly] [--dataOnly] [--noConfirm] [--skipThroughputUpdate]
+                     [--dumpPath DUMPPATH] [--billingMode {PROVISIONED,PAY_PER_REQUEST}] [--log LOG] [--limit LIMIT] [-f FILTEROPTION]
 
 Simple DynamoDB backup/restore/empty.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -a {zip,tar}, --archive {zip,tar}
-                        Type of compressed archive to create.If unset, don't
-                        create archive
+                        Type of compressed archive to create. If unset, don't create archive
   -b BUCKET, --bucket BUCKET
-                        S3 bucket in which to store or retrieve backups.[must
-                        already exist]
+                        S3 bucket in which to store or retrieve backups. [must already exist]
   -m {backup,restore,empty}, --mode {backup,restore,empty}
                         Operation to perform
   -r REGION, --region REGION
-                        AWS region to use, e.g. 'us-west-1'. Can use
-                        AWS_DEFAULT_REGION for local testing. Use 'local' for
-                        local DynamoDB testing
-  --host HOST           Host of local DynamoDB [required only for local]
+                        AWS region to use, e.g. 'us-west-1'. Can use any region for local testing
+  --host HOST           Host of local DynamoDB. This parameter initialises dynamodump for local DynamoDB testing [required only for local]
   --port PORT           Port of local DynamoDB [required only for local]
   --accessKey ACCESSKEY
                         Access key of local DynamoDB [required only for local]
   --secretKey SECRETKEY
                         Secret key of local DynamoDB [required only for local]
   -p PROFILE, --profile PROFILE
-                        AWS credentials file profile to use. Allows you to use
-                        a profile instead accessKey, secretKey authentication
+                        AWS credentials file profile to use. Allows you to use a profile instead accessKey, secretKey authentication
   -s SRCTABLE, --srcTable SRCTABLE
-                        Source DynamoDB table name to backup or restore from,
-                        use 'tablename*' for wildcard prefix selection or '*'
-                        for all tables. Mutually exclusive with --tag
+                        Source DynamoDB table name to backup or restore from, use 'tablename*' for wildcard prefix selection or '*' for all tables. Mutually exclusive with --tag
   -d DESTTABLE, --destTable DESTTABLE
-                        Destination DynamoDB table name to backup or restore
-                        to, use 'tablename*' for wildcard prefix selection
-                        (defaults to use '-' separator) [optional, defaults to
-                        source]
+                        Destination DynamoDB table name to backup or restore to, use 'tablename*' for wildcard prefix selection (defaults to use '-' separator) [optional, defaults to source]
   --prefixSeparator PREFIXSEPARATOR
-                        Specify a different prefix separator, e.g. '.'
-                        [optional]
-  --noSeparator         Overrides the use of a prefix separator for backup
-                        wildcard searches [optional]
+                        Specify a different prefix separator, e.g. '.' [optional]
+  --noSeparator         Overrides the use of a prefix separator for backup wildcard searches [optional]
   --readCapacity READCAPACITY
-                        Change the temp read capacity of the DynamoDB table to
-                        backup from [optional]
-  -t TAG, --tag TAG     Tag to use for identifying tables to back up. Mutually
-                        exclusive with srcTable. Provided as KEY=VALUE
+                        Change the temp read capacity of the DynamoDB table to backup from [optional]
+  -t TAG, --tag TAG     Tag to use for identifying tables to back up. Mutually exclusive with srcTable. Provided as KEY=VALUE
   --writeCapacity WRITECAPACITY
-                        Change the temp write capacity of the DynamoDB table
-                        to restore to [defaults to 25, optional]
-  --schemaOnly          Backup or restore the schema only. Do not
-                        backup/restore data. Can be used with both backup and
-                        restore modes. Cannot be used with the --dataOnly
-                        [optional]
-  --dataOnly            Restore data only. Do not delete/recreate schema
-                        [optional for restore]
-  --noConfirm           Don't ask for confirmation before deleting existing
-                        schemas.
+                        Change the temp write capacity of the DynamoDB table to restore to [defaults to 25, optional]
+  --schemaOnly          Backup or restore the schema only. Do not backup/restore data. Can be used with both backup and restore modes. Cannot be used with the --dataOnly [optional]
+  --dataOnly            Restore data only. Do not delete/recreate schema [optional for restore]
+  --noConfirm           Don't ask for confirmation before deleting existing schemas.
   --skipThroughputUpdate
-                        Skip updating throughput values across tables
-                        [optional]
-  --billingMode BILLING_MODE
-                        Set billing mode between PROVISIONED|PAY_PER_REQUEST
-                        (defaults to use 'PROVISIONED') [optional]
-  --dumpPath DUMPPATH   Directory to place and search for DynamoDB table
-                        backups (defaults to use 'dump') [optional]
-  --log LOG             Logging level - DEBUG|INFO|WARNING|ERROR|CRITICAL
-                        [optional]
+                        Skip updating throughput values across tables [optional]
+  --dumpPath DUMPPATH   Directory to place and search for DynamoDB table backups (defaults to use 'dump') [optional]
+  --billingMode {PROVISIONED,PAY_PER_REQUEST}
+                        Set billing mode between PROVISIONED|PAY_PER_REQUEST (defaults to use 'PROVISIONED') [optional]
+  --log LOG             Logging level - DEBUG|INFO|WARNING|ERROR|CRITICAL [optional]
+  --limit LIMIT         Limit option for backup, will stop the back up process after number of backed up items reaches the limit [optional]
   -f FILTEROPTION, --filterOption FILTEROPTION
                         Filter option for backup, JSON file of which keys are ['FilterExpression', 'ExpressionAttributeNames', 'ExpressionAttributeValues']
 ```
 
 Backup files are stored in a 'dump' subdirectory, and are restored from there as well by default.
 
 ## Script (unattended) usage
```

### Comparing `dynamodump-1.8.0/dynamodump/dynamodump.py` & `dynamodump-1.9.0/dynamodump/dynamodump.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Suitable for DynamoDB usages of smaller data volume which do not warrant the usage of AWS
     Data Pipeline for backup/restores/empty.
 
     dynamodump supports local DynamoDB instances as well (tested with DynamoDB Local).
 """
 
 import argparse
+import base64
 import boto3
 import datetime
 import errno
 import fnmatch
 import json
 import logging
 import os
@@ -45,17 +46,34 @@
 PAY_PER_REQUEST_BILLING_MODE = "PAY_PER_REQUEST"
 PROVISIONED_BILLING_MODE = "PROVISIONED"
 RESTORE_WRITE_CAPACITY = 25
 RESTORE_READ_CAPACITY = 25
 SCHEMA_FILE = "schema.json"
 THREAD_START_DELAY = 1  # seconds
 
-json.JSONEncoder.default = lambda self, obj: (
-    obj.isoformat() if isinstance(obj, datetime.datetime) else None
-)
+
+def encoder(self, obj):
+    if isinstance(obj, datetime.datetime):
+        return obj.isoformat()
+
+    if isinstance(obj, bytes):
+        return base64.b64encode(obj).decode("utf-8")
+
+    return json.JSONEncoder.encoder(self, obj)
+
+
+json.JSONEncoder.default = encoder
+
+
+def process_item_types(dct):
+    for item in dct["Items"]:
+        for key in item:
+            val = item[key]
+            if "B" in val:
+                item[key]["B"] = base64.b64decode(val["B"].encode("utf-8"))
 
 
 def _get_aws_client(
     service: str,
     profile: str = None,
     region: str = None,
     secret_key: str = None,
@@ -638,15 +656,20 @@
         + table_name
         + " completed. Time taken: "
         + str(datetime.datetime.now().replace(microsecond=0) - start_time)
     )
 
 
 def do_backup(
-    dynamo, read_capacity, table_queue=None, src_table=None, filter_option=None
+    dynamo,
+    read_capacity,
+    table_queue=None,
+    src_table=None,
+    filter_option=None,
+    limit=None,
 ):
     """
     Connect to DynamoDB and perform the backup for src_table or each table in table_queue
     """
 
     if src_table:
         table_name = src_table
@@ -689,14 +712,15 @@
                     )
 
                 # get table data
                 logging.info("Dumping table items for " + table_name)
                 mkdir_p(args.dumpPath + os.sep + table_name + os.sep + DATA_DIR)
 
                 i = 1
+                num_items = 0
                 last_evaluated_key = None
 
                 while True:
                     try:
                         optional_args = {}
                         if last_evaluated_key is not None:
                             optional_args["ExclusiveStartKey"] = last_evaluated_key
@@ -721,19 +745,24 @@
                         + DATA_DIR
                         + os.sep
                         + str(i).zfill(4)
                         + ".json",
                         "w+",
                     )
                     del scanned_table["ResponseMetadata"]
+
                     f.write(json.dumps(scanned_table, indent=JSON_INDENT))
                     f.close()
 
                     i += 1
 
+                    num_items += len(scanned_table["Items"])
+                    if limit and num_items > limit:
+                        break
+
                     try:
                         last_evaluated_key = scanned_table["LastEvaluatedKey"]
                     except KeyError:
                         break
 
                 # revert back to original table read capacity if specified
                 if (
@@ -976,16 +1005,17 @@
                     dump_data_path
                     + os.sep
                     + source_table
                     + os.sep
                     + DATA_DIR
                     + os.sep
                     + data_file
-                )
+                ),
             )
+            process_item_types(item_data)
             items.extend(item_data["Items"])
 
             # batch write data
             put_requests = []
             while len(items) > 0:
                 put_requests.append({"PutRequest": {"Item": items.pop(0)}})
 
@@ -1238,14 +1268,19 @@
         choices=[PROVISIONED_BILLING_MODE, PAY_PER_REQUEST_BILLING_MODE],
         default=str(PROVISIONED_BILLING_MODE),
     )
     parser.add_argument(
         "--log", help="Logging level - DEBUG|INFO|WARNING|ERROR|CRITICAL [optional]"
     )
     parser.add_argument(
+        "--limit",
+        help="Limit option for backup, will stop the back up process after number of backed up items reaches the limit [optional]",
+        type=int,
+    )
+    parser.add_argument(
         "-f",
         "--filterOption",
         help="Filter option for backup, JSON file of which keys are ['FilterExpression', 'ExpressionAttributeNames', 'ExpressionAttributeValues']",
     )
     args = parser.parse_args()
 
     # set log level
@@ -1340,33 +1375,39 @@
         try:
             if args.srcTable.find("*") == -1:
                 do_backup(
                     conn,
                     args.read_capacity,
                     table_queue=None,
                     filter_option=filter_option,
+                    limit=args.limit,
                 )
             else:
                 do_backup(
                     conn,
                     args.read_capacity,
                     matching_backup_tables,
                     filter_option=filter_option,
+                    limit=args.limit,
                 )
         except AttributeError:
             # Didn't specify srcTable if we get here
 
             q = Queue()
             threads = []
 
             for _ in range(MAX_NUMBER_BACKUP_WORKERS):
                 t = threading.Thread(
                     target=do_backup,
                     args=(conn, args.readCapacity),
-                    kwargs={"table_queue": q, "filter_option": filter_option},
+                    kwargs={
+                        "table_queue": q,
+                        "filter_option": filter_option,
+                        "limit": args.limit,
+                    },
                 )
                 t.start()
                 threads.append(t)
                 time.sleep(THREAD_START_DELAY)
 
             for table in matching_backup_tables:
                 q.put(table)
```

### Comparing `dynamodump-1.8.0/dynamodump.egg-info/PKG-INFO` & `dynamodump-1.9.0/dynamodump.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamodump
-Version: 1.8.0
+Version: 1.9.0
 Summary: Simple backup and restore for Amazon DynamoDB using AWS SDK for Python (boto3)
 Home-page: https://github.com/bchew/dynamodump
 Author: Benny Chew
 Author-email: noreply@bennychew.com
 Project-URL: Releases, https://github.com/bchew/dynamodump/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,14 @@
 
 Simple backup and restore script for Amazon DynamoDB using AWS SDK for Python (boto3) to work similarly to mysqldump.
 
 Suitable for DynamoDB usages of smaller data volume which do not warrant the usage of AWS Data Pipeline for backup/restores/empty.
 
 dynamodump supports local DynamoDB instances as well (tested with [DynamoDB Local](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.html)).
 
-
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Script (unattended) usage](#script-unattended-usage)
 - [Docker CLI usage](#docker-cli-usage)
 - [AWS example](#aws-example)
@@ -45,90 +44,60 @@
 ```
 pip install dynamodump
 ```
 
 ## Usage
 
 ```
-usage: dynamodump [-h] [-a {zip,tar}] [-b BUCKET]
-                     [-m {backup,restore,empty}] [-r REGION] [--host HOST]
-                     [--port PORT] [--accessKey ACCESSKEY]
-                     [--secretKey SECRETKEY] [-p PROFILE] [-s SRCTABLE]
-                     [-d DESTTABLE] [--prefixSeparator PREFIXSEPARATOR]
-                     [--noSeparator] [--readCapacity READCAPACITY] [-t TAG]
-                     [--writeCapacity WRITECAPACITY] [--schemaOnly]
-                     [--dataOnly] [--noConfirm] [--skipThroughputUpdate]
-                     [--billingMode BILLING_MODE] [--dumpPath DUMPPATH] [--log LOG]
-                     [-f FILTEROPTION]
+usage: dynamodump.py [-h] [-a {zip,tar}] [-b BUCKET] [-m {backup,restore,empty}] [-r REGION] [--host HOST] [--port PORT] [--accessKey ACCESSKEY] [--secretKey SECRETKEY] [-p PROFILE] [-s SRCTABLE] [-d DESTTABLE]
+                     [--prefixSeparator PREFIXSEPARATOR] [--noSeparator] [--readCapacity READCAPACITY] [-t TAG] [--writeCapacity WRITECAPACITY] [--schemaOnly] [--dataOnly] [--noConfirm] [--skipThroughputUpdate]
+                     [--dumpPath DUMPPATH] [--billingMode {PROVISIONED,PAY_PER_REQUEST}] [--log LOG] [--limit LIMIT] [-f FILTEROPTION]
 
 Simple DynamoDB backup/restore/empty.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -a {zip,tar}, --archive {zip,tar}
-                        Type of compressed archive to create.If unset, don't
-                        create archive
+                        Type of compressed archive to create. If unset, don't create archive
   -b BUCKET, --bucket BUCKET
-                        S3 bucket in which to store or retrieve backups.[must
-                        already exist]
+                        S3 bucket in which to store or retrieve backups. [must already exist]
   -m {backup,restore,empty}, --mode {backup,restore,empty}
                         Operation to perform
   -r REGION, --region REGION
-                        AWS region to use, e.g. 'us-west-1'. Can use
-                        AWS_DEFAULT_REGION for local testing. Use 'local' for
-                        local DynamoDB testing
-  --host HOST           Host of local DynamoDB [required only for local]
+                        AWS region to use, e.g. 'us-west-1'. Can use any region for local testing
+  --host HOST           Host of local DynamoDB. This parameter initialises dynamodump for local DynamoDB testing [required only for local]
   --port PORT           Port of local DynamoDB [required only for local]
   --accessKey ACCESSKEY
                         Access key of local DynamoDB [required only for local]
   --secretKey SECRETKEY
                         Secret key of local DynamoDB [required only for local]
   -p PROFILE, --profile PROFILE
-                        AWS credentials file profile to use. Allows you to use
-                        a profile instead accessKey, secretKey authentication
+                        AWS credentials file profile to use. Allows you to use a profile instead accessKey, secretKey authentication
   -s SRCTABLE, --srcTable SRCTABLE
-                        Source DynamoDB table name to backup or restore from,
-                        use 'tablename*' for wildcard prefix selection or '*'
-                        for all tables. Mutually exclusive with --tag
+                        Source DynamoDB table name to backup or restore from, use 'tablename*' for wildcard prefix selection or '*' for all tables. Mutually exclusive with --tag
   -d DESTTABLE, --destTable DESTTABLE
-                        Destination DynamoDB table name to backup or restore
-                        to, use 'tablename*' for wildcard prefix selection
-                        (defaults to use '-' separator) [optional, defaults to
-                        source]
+                        Destination DynamoDB table name to backup or restore to, use 'tablename*' for wildcard prefix selection (defaults to use '-' separator) [optional, defaults to source]
   --prefixSeparator PREFIXSEPARATOR
-                        Specify a different prefix separator, e.g. '.'
-                        [optional]
-  --noSeparator         Overrides the use of a prefix separator for backup
-                        wildcard searches [optional]
+                        Specify a different prefix separator, e.g. '.' [optional]
+  --noSeparator         Overrides the use of a prefix separator for backup wildcard searches [optional]
   --readCapacity READCAPACITY
-                        Change the temp read capacity of the DynamoDB table to
-                        backup from [optional]
-  -t TAG, --tag TAG     Tag to use for identifying tables to back up. Mutually
-                        exclusive with srcTable. Provided as KEY=VALUE
+                        Change the temp read capacity of the DynamoDB table to backup from [optional]
+  -t TAG, --tag TAG     Tag to use for identifying tables to back up. Mutually exclusive with srcTable. Provided as KEY=VALUE
   --writeCapacity WRITECAPACITY
-                        Change the temp write capacity of the DynamoDB table
-                        to restore to [defaults to 25, optional]
-  --schemaOnly          Backup or restore the schema only. Do not
-                        backup/restore data. Can be used with both backup and
-                        restore modes. Cannot be used with the --dataOnly
-                        [optional]
-  --dataOnly            Restore data only. Do not delete/recreate schema
-                        [optional for restore]
-  --noConfirm           Don't ask for confirmation before deleting existing
-                        schemas.
+                        Change the temp write capacity of the DynamoDB table to restore to [defaults to 25, optional]
+  --schemaOnly          Backup or restore the schema only. Do not backup/restore data. Can be used with both backup and restore modes. Cannot be used with the --dataOnly [optional]
+  --dataOnly            Restore data only. Do not delete/recreate schema [optional for restore]
+  --noConfirm           Don't ask for confirmation before deleting existing schemas.
   --skipThroughputUpdate
-                        Skip updating throughput values across tables
-                        [optional]
-  --billingMode BILLING_MODE
-                        Set billing mode between PROVISIONED|PAY_PER_REQUEST
-                        (defaults to use 'PROVISIONED') [optional]
-  --dumpPath DUMPPATH   Directory to place and search for DynamoDB table
-                        backups (defaults to use 'dump') [optional]
-  --log LOG             Logging level - DEBUG|INFO|WARNING|ERROR|CRITICAL
-                        [optional]
+                        Skip updating throughput values across tables [optional]
+  --dumpPath DUMPPATH   Directory to place and search for DynamoDB table backups (defaults to use 'dump') [optional]
+  --billingMode {PROVISIONED,PAY_PER_REQUEST}
+                        Set billing mode between PROVISIONED|PAY_PER_REQUEST (defaults to use 'PROVISIONED') [optional]
+  --log LOG             Logging level - DEBUG|INFO|WARNING|ERROR|CRITICAL [optional]
+  --limit LIMIT         Limit option for backup, will stop the back up process after number of backed up items reaches the limit [optional]
   -f FILTEROPTION, --filterOption FILTEROPTION
                         Filter option for backup, JSON file of which keys are ['FilterExpression', 'ExpressionAttributeNames', 'ExpressionAttributeValues']
 ```
 
 Backup files are stored in a 'dump' subdirectory, and are restored from there as well by default.
 
 ## Script (unattended) usage
```

### Comparing `dynamodump-1.8.0/setup.py` & `dynamodump-1.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dynamodump",
-    version="1.8.0",
+    version="1.9.0",
     author="Benny Chew",
     author_email="noreply@bennychew.com",
     description="Simple backup and restore for Amazon DynamoDB using AWS SDK for Python (boto3)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bchew/dynamodump",
     project_urls={
@@ -17,12 +17,12 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     packages=["dynamodump"],
     python_requires=">=3.7",
-    install_requires=["boto3==1.26.41", "six==1.16.0"],
+    install_requires=["boto3==1.26.132", "six==1.16.0"],
     entry_points={
         "console_scripts": ["dynamodump=dynamodump.dynamodump:main"],
     },
 )
```

### Comparing `dynamodump-1.8.0/tests/test.py` & `dynamodump-1.9.0/tests/test.py`

 * *Files identical despite different names*

