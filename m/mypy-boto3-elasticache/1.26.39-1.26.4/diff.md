# Comparing `tmp/mypy-boto3-elasticache-1.26.39.tar.gz` & `tmp/mypy-boto3-elasticache-1.26.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elasticache-1.26.39.tar", last modified: Wed Dec 28 20:24:49 2022, max compression
+gzip compressed data, was "mypy-boto3-elasticache-1.26.4.tar", last modified: Mon Nov  7 20:50:35 2022, max compression
```

## Comparing `mypy-boto3-elasticache-1.26.39.tar` & `mypy-boto3-elasticache-1.26.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 20:24:49.349914 mypy-boto3-elasticache-1.26.39/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-28 20:24:26.000000 mypy-boto3-elasticache-1.26.39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27270 2022-12-28 20:24:49.349914 mypy-boto3-elasticache-1.26.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25767 2022-12-28 20:24:26.000000 mypy-boto3-elasticache-1.26.39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 20:24:49.349914 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2022-12-28 20:24:26.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2022-12-28 20:24:26.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2022-12-28 20:24:26.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67949 2022-12-28 20:24:27.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    67856 2022-12-28 20:24:26.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13769 2022-12-28 20:24:27.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13767 2022-12-28 20:24:27.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22660 2022-12-28 20:24:27.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22641 2022-12-28 20:24:27.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 20:24:26.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86059 2022-12-28 20:24:29.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85992 2022-12-28 20:24:28.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-28 20:24:26.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2022-12-28 20:24:27.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2022-12-28 20:24:27.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 20:24:49.349914 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27270 2022-12-28 20:24:49.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2022-12-28 20:24:49.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 20:24:49.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 20:24:49.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-28 20:24:49.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-28 20:24:49.000000 mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-28 20:24:49.349914 mypy-boto3-elasticache-1.26.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2022-12-28 20:24:25.000000 mypy-boto3-elasticache-1.26.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:35.236330 mypy-boto3-elasticache-1.26.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    27123 2022-11-07 20:50:35.236330 mypy-boto3-elasticache-1.26.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    25672 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:35.236330 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (121)     5629 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5628 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67591 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67498 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    13089 2022-11-07 20:49:45.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/literals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13087 2022-11-07 20:49:45.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    22660 2022-11-07 20:49:45.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22641 2022-11-07 20:49:45.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    85176 2022-11-07 20:49:47.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    85109 2022-11-07 20:49:46.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-07 20:49:44.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5138 2022-11-07 20:49:45.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5134 2022-11-07 20:49:45.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:35.236330 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    27123 2022-11-07 20:50:35.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-11-07 20:50:35.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:35.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:35.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-07 20:50:35.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-07 20:50:35.000000 mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 20:50:35.236330 mypy-boto3-elasticache-1.26.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-11-07 20:49:43.000000 mypy-boto3-elasticache-1.26.4/setup.py
```

### Comparing `mypy-boto3-elasticache-1.26.39/LICENSE` & `mypy-boto3-elasticache-1.26.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.39/PKG-INFO` & `mypy-boto3-elasticache-1.26.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.26.39
-Summary: Type annotations for boto3.ElastiCache 1.26.39 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.4
+Summary: Type annotations for boto3.ElastiCache 1.26.4 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,15 +18,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticache?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.26.39](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -422,15 +421,14 @@
     DescribeReservedCacheNodesPaginatorName,
     DescribeServiceUpdatesPaginatorName,
     DescribeSnapshotsPaginatorName,
     DescribeUpdateActionsPaginatorName,
     DescribeUserGroupsPaginatorName,
     DescribeUsersPaginatorName,
     DestinationTypeType,
-    InputAuthenticationTypeType,
     IpDiscoveryType,
     LogDeliveryConfigurationStatusType,
     LogFormatType,
     LogTypeType,
     MultiAZStatusType,
     NetworkTypeType,
     NodeUpdateInitiatedByType,
@@ -440,15 +438,14 @@
     ReplicationGroupAvailableWaiterName,
     ReplicationGroupDeletedWaiterName,
     ServiceUpdateSeverityType,
     ServiceUpdateStatusType,
     ServiceUpdateTypeType,
     SlaMetType,
     SourceTypeType,
-    TransitEncryptionModeType,
     UpdateActionStatusType,
     ElastiCacheServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
     RegionName,
@@ -466,15 +463,14 @@
 `mypy_boto3_elasticache.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticache.type_defs import (
     TagTypeDef,
     ResponseMetadataTypeDef,
-    AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     BatchApplyUpdateActionMessageRequestTypeDef,
     BatchStopUpdateActionMessageRequestTypeDef,
     CacheParameterGroupStatusTypeDef,
     CacheSecurityGroupMembershipTypeDef,
@@ -532,14 +528,15 @@
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
+    ModifyUserMessageRequestTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
@@ -553,21 +550,20 @@
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
+    CreateUserMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     AllowedNodeTypeModificationsMessageTypeDef,
     CacheParameterGroupNameMessageTypeDef,
     EmptyResponseMetadataTypeDef,
     TagListMessageTypeDef,
-    CreateUserMessageRequestTypeDef,
-    ModifyUserMessageRequestTypeDef,
     UserResponseMetadataTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
```

### Comparing `mypy-boto3-elasticache-1.26.39/README.md` & `mypy-boto3-elasticache-1.26.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticache?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.26.39](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,15 +390,14 @@
     DescribeReservedCacheNodesPaginatorName,
     DescribeServiceUpdatesPaginatorName,
     DescribeSnapshotsPaginatorName,
     DescribeUpdateActionsPaginatorName,
     DescribeUserGroupsPaginatorName,
     DescribeUsersPaginatorName,
     DestinationTypeType,
-    InputAuthenticationTypeType,
     IpDiscoveryType,
     LogDeliveryConfigurationStatusType,
     LogFormatType,
     LogTypeType,
     MultiAZStatusType,
     NetworkTypeType,
     NodeUpdateInitiatedByType,
@@ -408,15 +407,14 @@
     ReplicationGroupAvailableWaiterName,
     ReplicationGroupDeletedWaiterName,
     ServiceUpdateSeverityType,
     ServiceUpdateStatusType,
     ServiceUpdateTypeType,
     SlaMetType,
     SourceTypeType,
-    TransitEncryptionModeType,
     UpdateActionStatusType,
     ElastiCacheServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
     RegionName,
@@ -434,15 +432,14 @@
 `mypy_boto3_elasticache.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticache.type_defs import (
     TagTypeDef,
     ResponseMetadataTypeDef,
-    AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     BatchApplyUpdateActionMessageRequestTypeDef,
     BatchStopUpdateActionMessageRequestTypeDef,
     CacheParameterGroupStatusTypeDef,
     CacheSecurityGroupMembershipTypeDef,
@@ -500,14 +497,15 @@
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
+    ModifyUserMessageRequestTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
@@ -521,21 +519,20 @@
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
+    CreateUserMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     AllowedNodeTypeModificationsMessageTypeDef,
     CacheParameterGroupNameMessageTypeDef,
     EmptyResponseMetadataTypeDef,
     TagListMessageTypeDef,
-    CreateUserMessageRequestTypeDef,
-    ModifyUserMessageRequestTypeDef,
     UserResponseMetadataTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
```

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/__init__.py` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/__init__.pyi` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/__main__.py` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElastiCache 1.26.39\nVersion:         1.26.39\nBuilder version:"
-        " 7.12.2\nDocs:           "
+        "Type annotations for boto3.ElastiCache 1.26.4\nVersion:         1.26.4\nBuilder version:"
+        " 7.11.10\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.39")
+    print("1.26.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/client.py` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     AuthTokenUpdateStrategyTypeType,
     AZModeType,
     IpDiscoveryType,
     NetworkTypeType,
     OutpostModeType,
     ServiceUpdateStatusType,
     SourceTypeType,
-    TransitEncryptionModeType,
     UpdateActionStatusType,
 )
 from .paginator import (
     DescribeCacheClustersPaginator,
     DescribeCacheEngineVersionsPaginator,
     DescribeCacheParameterGroupsPaginator,
     DescribeCacheParametersPaginator,
@@ -47,15 +46,14 @@
     DescribeSnapshotsPaginator,
     DescribeUpdateActionsPaginator,
     DescribeUserGroupsPaginator,
     DescribeUsersPaginator,
 )
 from .type_defs import (
     AllowedNodeTypeModificationsMessageTypeDef,
-    AuthenticationModeTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheClusterMessageTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheParameterGroupDetailsTypeDef,
     CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CacheSecurityGroupMessageTypeDef,
@@ -453,16 +451,15 @@
         TransitEncryptionEnabled: bool = ...,
         AtRestEncryptionEnabled: bool = ...,
         KmsKeyId: str = ...,
         UserGroupIds: Sequence[str] = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
         DataTieringEnabled: bool = ...,
         NetworkType: NetworkTypeType = ...,
-        IpDiscovery: IpDiscoveryType = ...,
-        TransitEncryptionMode: TransitEncryptionModeType = ...
+        IpDiscovery: IpDiscoveryType = ...
     ) -> CreateReplicationGroupResultTypeDef:
         """
         Creates a Redis (cluster mode disabled) or a Redis (cluster mode enabled)
         replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_replication_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#create_replication_group)
@@ -490,16 +487,15 @@
         *,
         UserId: str,
         UserName: str,
         Engine: str,
         AccessString: str,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...,
-        AuthenticationMode: AuthenticationModeTypeDef = ...
+        Tags: Sequence[TagTypeDef] = ...
     ) -> UserResponseMetadataTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#create_user)
         """
@@ -1087,17 +1083,15 @@
         CacheNodeType: str = ...,
         AuthToken: str = ...,
         AuthTokenUpdateStrategy: AuthTokenUpdateStrategyTypeType = ...,
         UserGroupIdsToAdd: Sequence[str] = ...,
         UserGroupIdsToRemove: Sequence[str] = ...,
         RemoveUserGroups: bool = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
-        IpDiscovery: IpDiscoveryType = ...,
-        TransitEncryptionEnabled: bool = ...,
-        TransitEncryptionMode: TransitEncryptionModeType = ...
+        IpDiscovery: IpDiscoveryType = ...
     ) -> ModifyReplicationGroupResultTypeDef:
         """
         Modifies the settings for a replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_replication_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#modify_replication_group)
         """
@@ -1123,16 +1117,15 @@
     def modify_user(
         self,
         *,
         UserId: str,
         AccessString: str = ...,
         AppendAccessString: str = ...,
         Passwords: Sequence[str] = ...,
-        NoPasswordRequired: bool = ...,
-        AuthenticationMode: AuthenticationModeTypeDef = ...
+        NoPasswordRequired: bool = ...
     ) -> UserResponseMetadataTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#modify_user)
         """
```

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/client.pyi` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     AuthTokenUpdateStrategyTypeType,
     AZModeType,
     IpDiscoveryType,
     NetworkTypeType,
     OutpostModeType,
     ServiceUpdateStatusType,
     SourceTypeType,
-    TransitEncryptionModeType,
     UpdateActionStatusType,
 )
 from .paginator import (
     DescribeCacheClustersPaginator,
     DescribeCacheEngineVersionsPaginator,
     DescribeCacheParameterGroupsPaginator,
     DescribeCacheParametersPaginator,
@@ -47,15 +46,14 @@
     DescribeSnapshotsPaginator,
     DescribeUpdateActionsPaginator,
     DescribeUserGroupsPaginator,
     DescribeUsersPaginator,
 )
 from .type_defs import (
     AllowedNodeTypeModificationsMessageTypeDef,
-    AuthenticationModeTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheClusterMessageTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheParameterGroupDetailsTypeDef,
     CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CacheSecurityGroupMessageTypeDef,
@@ -435,16 +433,15 @@
         TransitEncryptionEnabled: bool = ...,
         AtRestEncryptionEnabled: bool = ...,
         KmsKeyId: str = ...,
         UserGroupIds: Sequence[str] = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
         DataTieringEnabled: bool = ...,
         NetworkType: NetworkTypeType = ...,
-        IpDiscovery: IpDiscoveryType = ...,
-        TransitEncryptionMode: TransitEncryptionModeType = ...
+        IpDiscovery: IpDiscoveryType = ...
     ) -> CreateReplicationGroupResultTypeDef:
         """
         Creates a Redis (cluster mode disabled) or a Redis (cluster mode enabled)
         replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_replication_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#create_replication_group)
@@ -470,16 +467,15 @@
         *,
         UserId: str,
         UserName: str,
         Engine: str,
         AccessString: str,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...,
-        AuthenticationMode: AuthenticationModeTypeDef = ...
+        Tags: Sequence[TagTypeDef] = ...
     ) -> UserResponseMetadataTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#create_user)
         """
@@ -1026,17 +1022,15 @@
         CacheNodeType: str = ...,
         AuthToken: str = ...,
         AuthTokenUpdateStrategy: AuthTokenUpdateStrategyTypeType = ...,
         UserGroupIdsToAdd: Sequence[str] = ...,
         UserGroupIdsToRemove: Sequence[str] = ...,
         RemoveUserGroups: bool = ...,
         LogDeliveryConfigurations: Sequence[LogDeliveryConfigurationRequestTypeDef] = ...,
-        IpDiscovery: IpDiscoveryType = ...,
-        TransitEncryptionEnabled: bool = ...,
-        TransitEncryptionMode: TransitEncryptionModeType = ...
+        IpDiscovery: IpDiscoveryType = ...
     ) -> ModifyReplicationGroupResultTypeDef:
         """
         Modifies the settings for a replication group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_replication_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#modify_replication_group)
         """
@@ -1060,16 +1054,15 @@
     def modify_user(
         self,
         *,
         UserId: str,
         AccessString: str = ...,
         AppendAccessString: str = ...,
         Passwords: Sequence[str] = ...,
-        NoPasswordRequired: bool = ...,
-        AuthenticationMode: AuthenticationModeTypeDef = ...
+        NoPasswordRequired: bool = ...
     ) -> UserResponseMetadataTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#modify_user)
         """
```

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/literals.py` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     "DescribeReservedCacheNodesPaginatorName",
     "DescribeServiceUpdatesPaginatorName",
     "DescribeSnapshotsPaginatorName",
     "DescribeUpdateActionsPaginatorName",
     "DescribeUserGroupsPaginatorName",
     "DescribeUsersPaginatorName",
     "DestinationTypeType",
-    "InputAuthenticationTypeType",
     "IpDiscoveryType",
     "LogDeliveryConfigurationStatusType",
     "LogFormatType",
     "LogTypeType",
     "MultiAZStatusType",
     "NetworkTypeType",
     "NodeUpdateInitiatedByType",
@@ -61,29 +60,28 @@
     "ReplicationGroupAvailableWaiterName",
     "ReplicationGroupDeletedWaiterName",
     "ServiceUpdateSeverityType",
     "ServiceUpdateStatusType",
     "ServiceUpdateTypeType",
     "SlaMetType",
     "SourceTypeType",
-    "TransitEncryptionModeType",
     "UpdateActionStatusType",
     "ElastiCacheServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
 
 AZModeType = Literal["cross-az", "single-az"]
 AuthTokenUpdateStatusType = Literal["ROTATING", "SETTING"]
 AuthTokenUpdateStrategyTypeType = Literal["DELETE", "ROTATE", "SET"]
-AuthenticationTypeType = Literal["iam", "no-password", "password"]
+AuthenticationTypeType = Literal["no-password", "password"]
 AutomaticFailoverStatusType = Literal["disabled", "disabling", "enabled", "enabling"]
 CacheClusterAvailableWaiterName = Literal["cache_cluster_available"]
 CacheClusterDeletedWaiterName = Literal["cache_cluster_deleted"]
 ChangeTypeType = Literal["immediate", "requires-reboot"]
 DataTieringStatusType = Literal["disabled", "enabled"]
 DescribeCacheClustersPaginatorName = Literal["describe_cache_clusters"]
 DescribeCacheEngineVersionsPaginatorName = Literal["describe_cache_engine_versions"]
@@ -101,15 +99,14 @@
 DescribeReservedCacheNodesPaginatorName = Literal["describe_reserved_cache_nodes"]
 DescribeServiceUpdatesPaginatorName = Literal["describe_service_updates"]
 DescribeSnapshotsPaginatorName = Literal["describe_snapshots"]
 DescribeUpdateActionsPaginatorName = Literal["describe_update_actions"]
 DescribeUserGroupsPaginatorName = Literal["describe_user_groups"]
 DescribeUsersPaginatorName = Literal["describe_users"]
 DestinationTypeType = Literal["cloudwatch-logs", "kinesis-firehose"]
-InputAuthenticationTypeType = Literal["iam", "no-password-required", "password"]
 IpDiscoveryType = Literal["ipv4", "ipv6"]
 LogDeliveryConfigurationStatusType = Literal[
     "active", "disabling", "enabling", "error", "modifying"
 ]
 LogFormatType = Literal["json", "text"]
 LogTypeType = Literal["engine-log", "slow-log"]
 MultiAZStatusType = Literal["disabled", "enabled"]
@@ -131,15 +128,14 @@
     "cache-parameter-group",
     "cache-security-group",
     "cache-subnet-group",
     "replication-group",
     "user",
     "user-group",
 ]
-TransitEncryptionModeType = Literal["preferred", "required"]
 UpdateActionStatusType = Literal[
     "complete",
     "in-progress",
     "not-applicable",
     "not-applied",
     "scheduled",
     "scheduling",
@@ -168,15 +164,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -186,29 +181,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -237,15 +230,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -293,15 +285,14 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -317,27 +308,25 @@
     "kafkaconnect",
     "kendra",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -369,32 +358,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -403,15 +388,14 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
-    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -422,44 +406,38 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
-    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
@@ -526,24 +504,21 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
-    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
-    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
-    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/literals.pyi` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     "DescribeReservedCacheNodesPaginatorName",
     "DescribeServiceUpdatesPaginatorName",
     "DescribeSnapshotsPaginatorName",
     "DescribeUpdateActionsPaginatorName",
     "DescribeUserGroupsPaginatorName",
     "DescribeUsersPaginatorName",
     "DestinationTypeType",
-    "InputAuthenticationTypeType",
     "IpDiscoveryType",
     "LogDeliveryConfigurationStatusType",
     "LogFormatType",
     "LogTypeType",
     "MultiAZStatusType",
     "NetworkTypeType",
     "NodeUpdateInitiatedByType",
@@ -60,28 +59,27 @@
     "ReplicationGroupAvailableWaiterName",
     "ReplicationGroupDeletedWaiterName",
     "ServiceUpdateSeverityType",
     "ServiceUpdateStatusType",
     "ServiceUpdateTypeType",
     "SlaMetType",
     "SourceTypeType",
-    "TransitEncryptionModeType",
     "UpdateActionStatusType",
     "ElastiCacheServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
 AZModeType = Literal["cross-az", "single-az"]
 AuthTokenUpdateStatusType = Literal["ROTATING", "SETTING"]
 AuthTokenUpdateStrategyTypeType = Literal["DELETE", "ROTATE", "SET"]
-AuthenticationTypeType = Literal["iam", "no-password", "password"]
+AuthenticationTypeType = Literal["no-password", "password"]
 AutomaticFailoverStatusType = Literal["disabled", "disabling", "enabled", "enabling"]
 CacheClusterAvailableWaiterName = Literal["cache_cluster_available"]
 CacheClusterDeletedWaiterName = Literal["cache_cluster_deleted"]
 ChangeTypeType = Literal["immediate", "requires-reboot"]
 DataTieringStatusType = Literal["disabled", "enabled"]
 DescribeCacheClustersPaginatorName = Literal["describe_cache_clusters"]
 DescribeCacheEngineVersionsPaginatorName = Literal["describe_cache_engine_versions"]
@@ -99,15 +97,14 @@
 DescribeReservedCacheNodesPaginatorName = Literal["describe_reserved_cache_nodes"]
 DescribeServiceUpdatesPaginatorName = Literal["describe_service_updates"]
 DescribeSnapshotsPaginatorName = Literal["describe_snapshots"]
 DescribeUpdateActionsPaginatorName = Literal["describe_update_actions"]
 DescribeUserGroupsPaginatorName = Literal["describe_user_groups"]
 DescribeUsersPaginatorName = Literal["describe_users"]
 DestinationTypeType = Literal["cloudwatch-logs", "kinesis-firehose"]
-InputAuthenticationTypeType = Literal["iam", "no-password-required", "password"]
 IpDiscoveryType = Literal["ipv4", "ipv6"]
 LogDeliveryConfigurationStatusType = Literal[
     "active", "disabling", "enabling", "error", "modifying"
 ]
 LogFormatType = Literal["json", "text"]
 LogTypeType = Literal["engine-log", "slow-log"]
 MultiAZStatusType = Literal["disabled", "enabled"]
@@ -129,15 +126,14 @@
     "cache-parameter-group",
     "cache-security-group",
     "cache-subnet-group",
     "replication-group",
     "user",
     "user-group",
 ]
-TransitEncryptionModeType = Literal["preferred", "required"]
 UpdateActionStatusType = Literal[
     "complete",
     "in-progress",
     "not-applicable",
     "not-applied",
     "scheduled",
     "scheduling",
@@ -166,15 +162,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -184,29 +179,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -235,15 +228,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -291,15 +283,14 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -315,27 +306,25 @@
     "kafkaconnect",
     "kendra",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -367,32 +356,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -401,15 +386,14 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
-    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -420,44 +404,38 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
-    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
@@ -524,24 +502,21 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
-    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
-    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
-    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/paginator.py` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/paginator.pyi` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/type_defs.py` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -20,47 +20,43 @@
     AuthTokenUpdateStatusType,
     AuthTokenUpdateStrategyTypeType,
     AutomaticFailoverStatusType,
     AZModeType,
     ChangeTypeType,
     DataTieringStatusType,
     DestinationTypeType,
-    InputAuthenticationTypeType,
     IpDiscoveryType,
     LogDeliveryConfigurationStatusType,
     LogFormatType,
     LogTypeType,
     MultiAZStatusType,
     NetworkTypeType,
     NodeUpdateInitiatedByType,
     NodeUpdateStatusType,
     OutpostModeType,
     PendingAutomaticFailoverStatusType,
     ServiceUpdateSeverityType,
     ServiceUpdateStatusType,
     SlaMetType,
     SourceTypeType,
-    TransitEncryptionModeType,
     UpdateActionStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "ResponseMetadataTypeDef",
-    "AuthenticationModeTypeDef",
     "AuthenticationTypeDef",
     "AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchApplyUpdateActionMessageRequestTypeDef",
     "BatchStopUpdateActionMessageRequestTypeDef",
     "CacheParameterGroupStatusTypeDef",
     "CacheSecurityGroupMembershipTypeDef",
@@ -118,14 +114,15 @@
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
+    "ModifyUserMessageRequestTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
@@ -139,21 +136,20 @@
     "AddTagsToResourceMessageRequestTypeDef",
     "CopySnapshotMessageRequestTypeDef",
     "CreateCacheParameterGroupMessageRequestTypeDef",
     "CreateCacheSecurityGroupMessageRequestTypeDef",
     "CreateCacheSubnetGroupMessageRequestTypeDef",
     "CreateSnapshotMessageRequestTypeDef",
     "CreateUserGroupMessageRequestTypeDef",
+    "CreateUserMessageRequestTypeDef",
     "PurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
     "AllowedNodeTypeModificationsMessageTypeDef",
     "CacheParameterGroupNameMessageTypeDef",
     "EmptyResponseMetadataTypeDef",
     "TagListMessageTypeDef",
-    "CreateUserMessageRequestTypeDef",
-    "ModifyUserMessageRequestTypeDef",
     "UserResponseMetadataTypeDef",
     "UserTypeDef",
     "CacheNodeTypeDef",
     "NodeGroupMemberTypeDef",
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
@@ -280,23 +276,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-AuthenticationModeTypeDef = TypedDict(
-    "AuthenticationModeTypeDef",
-    {
-        "Type": InputAuthenticationTypeType,
-        "Passwords": Sequence[str],
-    },
-    total=False,
-)
-
 AuthenticationTypeDef = TypedDict(
     "AuthenticationTypeDef",
     {
         "Type": AuthenticationTypeType,
         "PasswordCount": int,
     },
     total=False,
@@ -330,22 +317,20 @@
     {
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
     },
     total=False,
 )
 
-
 class BatchApplyUpdateActionMessageRequestTypeDef(
     _RequiredBatchApplyUpdateActionMessageRequestTypeDef,
     _OptionalBatchApplyUpdateActionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchStopUpdateActionMessageRequestTypeDef = TypedDict(
     "_RequiredBatchStopUpdateActionMessageRequestTypeDef",
     {
         "ServiceUpdateName": str,
     },
 )
 _OptionalBatchStopUpdateActionMessageRequestTypeDef = TypedDict(
@@ -353,22 +338,20 @@
     {
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
     },
     total=False,
 )
 
-
 class BatchStopUpdateActionMessageRequestTypeDef(
     _RequiredBatchStopUpdateActionMessageRequestTypeDef,
     _OptionalBatchStopUpdateActionMessageRequestTypeDef,
 ):
     pass
 
-
 CacheParameterGroupStatusTypeDef = TypedDict(
     "CacheParameterGroupStatusTypeDef",
     {
         "CacheParameterGroupName": str,
         "ParameterApplyStatus": str,
         "CacheNodeIdsToReboot": List[str],
     },
@@ -503,21 +486,19 @@
     "_OptionalCompleteMigrationMessageRequestTypeDef",
     {
         "Force": bool,
     },
     total=False,
 )
 
-
 class CompleteMigrationMessageRequestTypeDef(
     _RequiredCompleteMigrationMessageRequestTypeDef, _OptionalCompleteMigrationMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredConfigureShardTypeDef = TypedDict(
     "_RequiredConfigureShardTypeDef",
     {
         "NodeGroupId": str,
         "NewReplicaCount": int,
     },
 )
@@ -526,19 +507,17 @@
     {
         "PreferredAvailabilityZones": Sequence[str],
         "PreferredOutpostArns": Sequence[str],
     },
     total=False,
 )
 
-
 class ConfigureShardTypeDef(_RequiredConfigureShardTypeDef, _OptionalConfigureShardTypeDef):
     pass
 
-
 _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupIdSuffix": str,
         "PrimaryReplicationGroupId": str,
     },
 )
@@ -546,22 +525,20 @@
     "_OptionalCreateGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupDescription": str,
     },
     total=False,
 )
 
-
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 NodeGroupConfigurationTypeDef = TypedDict(
     "NodeGroupConfigurationTypeDef",
     {
         "NodeGroupId": str,
         "Slots": str,
         "ReplicaCount": int,
         "PrimaryAvailabilityZone": str,
@@ -594,44 +571,40 @@
     {
         "GlobalNodeGroupsToRemove": Sequence[str],
         "GlobalNodeGroupsToRetain": Sequence[str],
     },
     total=False,
 )
 
-
 class DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredDecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalDecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalDeleteCacheClusterMessageRequestTypeDef = TypedDict(
     "_OptionalDeleteCacheClusterMessageRequestTypeDef",
     {
         "FinalSnapshotIdentifier": str,
     },
     total=False,
 )
 
-
 class DeleteCacheClusterMessageRequestTypeDef(
     _RequiredDeleteCacheClusterMessageRequestTypeDef,
     _OptionalDeleteCacheClusterMessageRequestTypeDef,
 ):
     pass
 
-
 DeleteCacheParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
     },
 )
 
@@ -668,22 +641,20 @@
     {
         "RetainPrimaryCluster": bool,
         "FinalSnapshotIdentifier": str,
     },
     total=False,
 )
 
-
 class DeleteReplicationGroupMessageRequestTypeDef(
     _RequiredDeleteReplicationGroupMessageRequestTypeDef,
     _OptionalDeleteReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 DeleteSnapshotMessageRequestTypeDef = TypedDict(
     "DeleteSnapshotMessageRequestTypeDef",
     {
         "SnapshotName": str,
     },
 )
 
@@ -767,22 +738,20 @@
         "Source": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeCacheParametersMessageRequestTypeDef(
     _RequiredDescribeCacheParametersMessageRequestTypeDef,
     _OptionalDescribeCacheParametersMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeCacheSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -810,22 +779,20 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -1041,22 +1008,20 @@
     {
         "CacheSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyCacheSubnetGroupMessageRequestTypeDef(
     _RequiredModifyCacheSubnetGroupMessageRequestTypeDef,
     _OptionalModifyCacheSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "ApplyImmediately": bool,
     },
 )
@@ -1068,22 +1033,20 @@
         "CacheParameterGroupName": str,
         "GlobalReplicationGroupDescription": str,
         "AutomaticFailoverEnabled": bool,
     },
     total=False,
 )
 
-
 class ModifyGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredModifyGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalModifyGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 ReshardingConfigurationTypeDef = TypedDict(
     "ReshardingConfigurationTypeDef",
     {
         "NodeGroupId": str,
         "PreferredAvailabilityZones": Sequence[str],
     },
     total=False,
@@ -1100,20 +1063,40 @@
     {
         "UserIdsToAdd": Sequence[str],
         "UserIdsToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
+_RequiredModifyUserMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyUserMessageRequestTypeDef",
+    {
+        "UserId": str,
+    },
+)
+_OptionalModifyUserMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyUserMessageRequestTypeDef",
+    {
+        "AccessString": str,
+        "AppendAccessString": str,
+        "Passwords": Sequence[str],
+        "NoPasswordRequired": bool,
+    },
+    total=False,
+)
+
+class ModifyUserMessageRequestTypeDef(
+    _RequiredModifyUserMessageRequestTypeDef, _OptionalModifyUserMessageRequestTypeDef
+):
+    pass
 
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
@@ -1274,21 +1257,19 @@
         "TargetBucket": str,
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopySnapshotMessageRequestTypeDef(
     _RequiredCopySnapshotMessageRequestTypeDef, _OptionalCopySnapshotMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateCacheParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheParameterGroupMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
         "CacheParameterGroupFamily": str,
         "Description": str,
     },
@@ -1297,22 +1278,20 @@
     "_OptionalCreateCacheParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCacheParameterGroupMessageRequestTypeDef(
     _RequiredCreateCacheParameterGroupMessageRequestTypeDef,
     _OptionalCreateCacheParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateCacheSecurityGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheSecurityGroupMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "Description": str,
     },
 )
@@ -1320,22 +1299,20 @@
     "_OptionalCreateCacheSecurityGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCacheSecurityGroupMessageRequestTypeDef(
     _RequiredCreateCacheSecurityGroupMessageRequestTypeDef,
     _OptionalCreateCacheSecurityGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateCacheSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheSubnetGroupMessageRequestTypeDef",
     {
         "CacheSubnetGroupName": str,
         "CacheSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -1344,22 +1321,20 @@
     "_OptionalCreateCacheSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCacheSubnetGroupMessageRequestTypeDef(
     _RequiredCreateCacheSubnetGroupMessageRequestTypeDef,
     _OptionalCreateCacheSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotMessageRequestTypeDef",
     {
         "SnapshotName": str,
     },
 )
 _OptionalCreateSnapshotMessageRequestTypeDef = TypedDict(
@@ -1369,21 +1344,19 @@
         "CacheClusterId": str,
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSnapshotMessageRequestTypeDef(
     _RequiredCreateSnapshotMessageRequestTypeDef, _OptionalCreateSnapshotMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateUserGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateUserGroupMessageRequestTypeDef",
     {
         "UserGroupId": str,
         "Engine": str,
     },
 )
@@ -1392,20 +1365,42 @@
     {
         "UserIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateUserGroupMessageRequestTypeDef(
     _RequiredCreateUserGroupMessageRequestTypeDef, _OptionalCreateUserGroupMessageRequestTypeDef
 ):
     pass
 
+_RequiredCreateUserMessageRequestTypeDef = TypedDict(
+    "_RequiredCreateUserMessageRequestTypeDef",
+    {
+        "UserId": str,
+        "UserName": str,
+        "Engine": str,
+        "AccessString": str,
+    },
+)
+_OptionalCreateUserMessageRequestTypeDef = TypedDict(
+    "_OptionalCreateUserMessageRequestTypeDef",
+    {
+        "Passwords": Sequence[str],
+        "NoPasswordRequired": bool,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateUserMessageRequestTypeDef(
+    _RequiredCreateUserMessageRequestTypeDef, _OptionalCreateUserMessageRequestTypeDef
+):
+    pass
 
 _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
     {
         "ReservedCacheNodesOfferingId": str,
     },
 )
@@ -1415,22 +1410,20 @@
         "ReservedCacheNodeId": str,
         "CacheNodeCount": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PurchaseReservedCacheNodesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
 ):
     pass
 
-
 AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
     "AllowedNodeTypeModificationsMessageTypeDef",
     {
         "ScaleUpModifications": List[str],
         "ScaleDownModifications": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1455,66 +1448,14 @@
     "TagListMessageTypeDef",
     {
         "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateUserMessageRequestTypeDef = TypedDict(
-    "_RequiredCreateUserMessageRequestTypeDef",
-    {
-        "UserId": str,
-        "UserName": str,
-        "Engine": str,
-        "AccessString": str,
-    },
-)
-_OptionalCreateUserMessageRequestTypeDef = TypedDict(
-    "_OptionalCreateUserMessageRequestTypeDef",
-    {
-        "Passwords": Sequence[str],
-        "NoPasswordRequired": bool,
-        "Tags": Sequence[TagTypeDef],
-        "AuthenticationMode": AuthenticationModeTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateUserMessageRequestTypeDef(
-    _RequiredCreateUserMessageRequestTypeDef, _OptionalCreateUserMessageRequestTypeDef
-):
-    pass
-
-
-_RequiredModifyUserMessageRequestTypeDef = TypedDict(
-    "_RequiredModifyUserMessageRequestTypeDef",
-    {
-        "UserId": str,
-    },
-)
-_OptionalModifyUserMessageRequestTypeDef = TypedDict(
-    "_OptionalModifyUserMessageRequestTypeDef",
-    {
-        "AccessString": str,
-        "AppendAccessString": str,
-        "Passwords": Sequence[str],
-        "NoPasswordRequired": bool,
-        "AuthenticationMode": AuthenticationModeTypeDef,
-    },
-    total=False,
-)
-
-
-class ModifyUserMessageRequestTypeDef(
-    _RequiredModifyUserMessageRequestTypeDef, _OptionalModifyUserMessageRequestTypeDef
-):
-    pass
-
-
 UserResponseMetadataTypeDef = TypedDict(
     "UserResponseMetadataTypeDef",
     {
         "UserId": str,
         "UserName": str,
         "Status": str,
         "Engine": str,
@@ -1638,22 +1579,20 @@
         "NewReplicaCount": int,
         "ReplicaConfiguration": Sequence[ConfigureShardTypeDef],
         "ReplicasToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class DecreaseReplicaCountMessageRequestTypeDef(
     _RequiredDecreaseReplicaCountMessageRequestTypeDef,
     _OptionalDecreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredIncreaseReplicaCountMessageRequestTypeDef = TypedDict(
     "_RequiredIncreaseReplicaCountMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "ApplyImmediately": bool,
     },
 )
@@ -1662,22 +1601,20 @@
     {
         "NewReplicaCount": int,
         "ReplicaConfiguration": Sequence[ConfigureShardTypeDef],
     },
     total=False,
 )
 
-
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
-
 NodeSnapshotTypeDef = TypedDict(
     "NodeSnapshotTypeDef",
     {
         "CacheClusterId": str,
         "NodeGroupId": str,
         "CacheNodeId": str,
         "NodeGroupConfiguration": NodeGroupConfigurationTypeDef,
@@ -1787,22 +1724,20 @@
     {
         "Source": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
     _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
 ):
     pass
 
-
 DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
     "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
     {
         "CacheSecurityGroupName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1827,22 +1762,20 @@
     "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
 ):
     pass
 
-
 DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -2043,22 +1976,20 @@
     {
         "ResetAllParameters": bool,
         "ParameterNameValues": Sequence[ParameterNameValueTypeDef],
     },
     total=False,
 )
 
-
 class ResetCacheParameterGroupMessageRequestTypeDef(
     _RequiredResetCacheParameterGroupMessageRequestTypeDef,
     _OptionalResetCacheParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyReplicationGroupShardConfigurationMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "NodeGroupCount": int,
         "ApplyImmediately": bool,
     },
@@ -2069,22 +2000,20 @@
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
         "NodeGroupsToRemove": Sequence[str],
         "NodeGroupsToRetain": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyReplicationGroupShardConfigurationMessageRequestTypeDef(
     _RequiredModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     _OptionalModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
 ):
     pass
 
-
 RegionalConfigurationTypeDef = TypedDict(
     "RegionalConfigurationTypeDef",
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
@@ -2433,22 +2362,20 @@
     "_OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     {
         "RegionalConfigurations": Sequence[RegionalConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2596,22 +2523,20 @@
         "TransitEncryptionEnabled": bool,
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
     },
     total=False,
 )
 
-
 class CreateCacheClusterMessageRequestTypeDef(
     _RequiredCreateCacheClusterMessageRequestTypeDef,
     _OptionalCreateCacheClusterMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "ReplicationGroupDescription": str,
     },
 )
@@ -2648,27 +2573,24 @@
         "AtRestEncryptionEnabled": bool,
         "KmsKeyId": str,
         "UserGroupIds": Sequence[str],
         "LogDeliveryConfigurations": Sequence[LogDeliveryConfigurationRequestTypeDef],
         "DataTieringEnabled": bool,
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
-        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
-
 class CreateReplicationGroupMessageRequestTypeDef(
     _RequiredCreateReplicationGroupMessageRequestTypeDef,
     _OptionalCreateReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalModifyCacheClusterMessageRequestTypeDef = TypedDict(
@@ -2694,22 +2616,20 @@
         "AuthTokenUpdateStrategy": AuthTokenUpdateStrategyTypeType,
         "LogDeliveryConfigurations": Sequence[LogDeliveryConfigurationRequestTypeDef],
         "IpDiscovery": IpDiscoveryType,
     },
     total=False,
 )
 
-
 class ModifyCacheClusterMessageRequestTypeDef(
     _RequiredModifyCacheClusterMessageRequestTypeDef,
     _OptionalModifyCacheClusterMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationGroupMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
     },
 )
 _OptionalModifyReplicationGroupMessageRequestTypeDef = TypedDict(
@@ -2736,54 +2656,46 @@
         "AuthToken": str,
         "AuthTokenUpdateStrategy": AuthTokenUpdateStrategyTypeType,
         "UserGroupIdsToAdd": Sequence[str],
         "UserGroupIdsToRemove": Sequence[str],
         "RemoveUserGroups": bool,
         "LogDeliveryConfigurations": Sequence[LogDeliveryConfigurationRequestTypeDef],
         "IpDiscovery": IpDiscoveryType,
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
-
 class ModifyReplicationGroupMessageRequestTypeDef(
     _RequiredModifyReplicationGroupMessageRequestTypeDef,
     _OptionalModifyReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-
 PendingModifiedValuesTypeDef = TypedDict(
     "PendingModifiedValuesTypeDef",
     {
         "NumCacheNodes": int,
         "CacheNodeIdsToRemove": List[str],
         "EngineVersion": str,
         "CacheNodeType": str,
         "AuthTokenStatus": AuthTokenUpdateStatusType,
         "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
 ReplicationGroupPendingModifiedValuesTypeDef = TypedDict(
     "ReplicationGroupPendingModifiedValuesTypeDef",
     {
         "PrimaryClusterId": str,
         "AutomaticFailoverStatus": PendingAutomaticFailoverStatusType,
         "Resharding": ReshardingStatusTypeDef,
         "AuthTokenStatus": AuthTokenUpdateStatusType,
         "UserGroups": UserGroupsUpdateStatusTypeDef,
         "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
@@ -2849,15 +2761,14 @@
         "TransitEncryptionEnabled": bool,
         "AtRestEncryptionEnabled": bool,
         "ARN": str,
         "ReplicationGroupLogDeliveryEnabled": bool,
         "LogDeliveryConfigurations": List[LogDeliveryConfigurationTypeDef],
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
-        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
 ReplicationGroupTypeDef = TypedDict(
     "ReplicationGroupTypeDef",
     {
@@ -2886,15 +2797,14 @@
         "UserGroupIds": List[str],
         "LogDeliveryConfigurations": List[LogDeliveryConfigurationTypeDef],
         "ReplicationGroupCreateTime": datetime,
         "DataTiering": DataTieringStatusType,
         "AutoMinorVersionUpgrade": bool,
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
-        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
 CacheClusterMessageTypeDef = TypedDict(
     "CacheClusterMessageTypeDef",
     {
```

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/type_defs.pyi` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,46 +20,44 @@
     AuthTokenUpdateStatusType,
     AuthTokenUpdateStrategyTypeType,
     AutomaticFailoverStatusType,
     AZModeType,
     ChangeTypeType,
     DataTieringStatusType,
     DestinationTypeType,
-    InputAuthenticationTypeType,
     IpDiscoveryType,
     LogDeliveryConfigurationStatusType,
     LogFormatType,
     LogTypeType,
     MultiAZStatusType,
     NetworkTypeType,
     NodeUpdateInitiatedByType,
     NodeUpdateStatusType,
     OutpostModeType,
     PendingAutomaticFailoverStatusType,
     ServiceUpdateSeverityType,
     ServiceUpdateStatusType,
     SlaMetType,
     SourceTypeType,
-    TransitEncryptionModeType,
     UpdateActionStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
     "ResponseMetadataTypeDef",
-    "AuthenticationModeTypeDef",
     "AuthenticationTypeDef",
     "AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchApplyUpdateActionMessageRequestTypeDef",
     "BatchStopUpdateActionMessageRequestTypeDef",
     "CacheParameterGroupStatusTypeDef",
     "CacheSecurityGroupMembershipTypeDef",
@@ -117,14 +115,15 @@
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
+    "ModifyUserMessageRequestTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
@@ -138,21 +137,20 @@
     "AddTagsToResourceMessageRequestTypeDef",
     "CopySnapshotMessageRequestTypeDef",
     "CreateCacheParameterGroupMessageRequestTypeDef",
     "CreateCacheSecurityGroupMessageRequestTypeDef",
     "CreateCacheSubnetGroupMessageRequestTypeDef",
     "CreateSnapshotMessageRequestTypeDef",
     "CreateUserGroupMessageRequestTypeDef",
+    "CreateUserMessageRequestTypeDef",
     "PurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
     "AllowedNodeTypeModificationsMessageTypeDef",
     "CacheParameterGroupNameMessageTypeDef",
     "EmptyResponseMetadataTypeDef",
     "TagListMessageTypeDef",
-    "CreateUserMessageRequestTypeDef",
-    "ModifyUserMessageRequestTypeDef",
     "UserResponseMetadataTypeDef",
     "UserTypeDef",
     "CacheNodeTypeDef",
     "NodeGroupMemberTypeDef",
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
@@ -279,23 +277,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-AuthenticationModeTypeDef = TypedDict(
-    "AuthenticationModeTypeDef",
-    {
-        "Type": InputAuthenticationTypeType,
-        "Passwords": Sequence[str],
-    },
-    total=False,
-)
-
 AuthenticationTypeDef = TypedDict(
     "AuthenticationTypeDef",
     {
         "Type": AuthenticationTypeType,
         "PasswordCount": int,
     },
     total=False,
@@ -329,20 +318,22 @@
     {
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
     },
     total=False,
 )
 
+
 class BatchApplyUpdateActionMessageRequestTypeDef(
     _RequiredBatchApplyUpdateActionMessageRequestTypeDef,
     _OptionalBatchApplyUpdateActionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchStopUpdateActionMessageRequestTypeDef = TypedDict(
     "_RequiredBatchStopUpdateActionMessageRequestTypeDef",
     {
         "ServiceUpdateName": str,
     },
 )
 _OptionalBatchStopUpdateActionMessageRequestTypeDef = TypedDict(
@@ -350,20 +341,22 @@
     {
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
     },
     total=False,
 )
 
+
 class BatchStopUpdateActionMessageRequestTypeDef(
     _RequiredBatchStopUpdateActionMessageRequestTypeDef,
     _OptionalBatchStopUpdateActionMessageRequestTypeDef,
 ):
     pass
 
+
 CacheParameterGroupStatusTypeDef = TypedDict(
     "CacheParameterGroupStatusTypeDef",
     {
         "CacheParameterGroupName": str,
         "ParameterApplyStatus": str,
         "CacheNodeIdsToReboot": List[str],
     },
@@ -498,19 +491,21 @@
     "_OptionalCompleteMigrationMessageRequestTypeDef",
     {
         "Force": bool,
     },
     total=False,
 )
 
+
 class CompleteMigrationMessageRequestTypeDef(
     _RequiredCompleteMigrationMessageRequestTypeDef, _OptionalCompleteMigrationMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredConfigureShardTypeDef = TypedDict(
     "_RequiredConfigureShardTypeDef",
     {
         "NodeGroupId": str,
         "NewReplicaCount": int,
     },
 )
@@ -519,17 +514,19 @@
     {
         "PreferredAvailabilityZones": Sequence[str],
         "PreferredOutpostArns": Sequence[str],
     },
     total=False,
 )
 
+
 class ConfigureShardTypeDef(_RequiredConfigureShardTypeDef, _OptionalConfigureShardTypeDef):
     pass
 
+
 _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupIdSuffix": str,
         "PrimaryReplicationGroupId": str,
     },
 )
@@ -537,20 +534,22 @@
     "_OptionalCreateGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupDescription": str,
     },
     total=False,
 )
 
+
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 NodeGroupConfigurationTypeDef = TypedDict(
     "NodeGroupConfigurationTypeDef",
     {
         "NodeGroupId": str,
         "Slots": str,
         "ReplicaCount": int,
         "PrimaryAvailabilityZone": str,
@@ -583,40 +582,44 @@
     {
         "GlobalNodeGroupsToRemove": Sequence[str],
         "GlobalNodeGroupsToRetain": Sequence[str],
     },
     total=False,
 )
 
+
 class DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredDecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalDecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalDeleteCacheClusterMessageRequestTypeDef = TypedDict(
     "_OptionalDeleteCacheClusterMessageRequestTypeDef",
     {
         "FinalSnapshotIdentifier": str,
     },
     total=False,
 )
 
+
 class DeleteCacheClusterMessageRequestTypeDef(
     _RequiredDeleteCacheClusterMessageRequestTypeDef,
     _OptionalDeleteCacheClusterMessageRequestTypeDef,
 ):
     pass
 
+
 DeleteCacheParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
     },
 )
 
@@ -653,20 +656,22 @@
     {
         "RetainPrimaryCluster": bool,
         "FinalSnapshotIdentifier": str,
     },
     total=False,
 )
 
+
 class DeleteReplicationGroupMessageRequestTypeDef(
     _RequiredDeleteReplicationGroupMessageRequestTypeDef,
     _OptionalDeleteReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 DeleteSnapshotMessageRequestTypeDef = TypedDict(
     "DeleteSnapshotMessageRequestTypeDef",
     {
         "SnapshotName": str,
     },
 )
 
@@ -750,20 +755,22 @@
         "Source": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeCacheParametersMessageRequestTypeDef(
     _RequiredDescribeCacheParametersMessageRequestTypeDef,
     _OptionalDescribeCacheParametersMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeCacheSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -791,20 +798,22 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -1020,20 +1029,22 @@
     {
         "CacheSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyCacheSubnetGroupMessageRequestTypeDef(
     _RequiredModifyCacheSubnetGroupMessageRequestTypeDef,
     _OptionalModifyCacheSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "ApplyImmediately": bool,
     },
 )
@@ -1045,20 +1056,22 @@
         "CacheParameterGroupName": str,
         "GlobalReplicationGroupDescription": str,
         "AutomaticFailoverEnabled": bool,
     },
     total=False,
 )
 
+
 class ModifyGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredModifyGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalModifyGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 ReshardingConfigurationTypeDef = TypedDict(
     "ReshardingConfigurationTypeDef",
     {
         "NodeGroupId": str,
         "PreferredAvailabilityZones": Sequence[str],
     },
     total=False,
@@ -1075,19 +1088,45 @@
     {
         "UserIdsToAdd": Sequence[str],
         "UserIdsToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
+
+_RequiredModifyUserMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyUserMessageRequestTypeDef",
+    {
+        "UserId": str,
+    },
+)
+_OptionalModifyUserMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyUserMessageRequestTypeDef",
+    {
+        "AccessString": str,
+        "AppendAccessString": str,
+        "Passwords": Sequence[str],
+        "NoPasswordRequired": bool,
+    },
+    total=False,
+)
+
+
+class ModifyUserMessageRequestTypeDef(
+    _RequiredModifyUserMessageRequestTypeDef, _OptionalModifyUserMessageRequestTypeDef
+):
+    pass
+
+
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1247,19 +1286,21 @@
         "TargetBucket": str,
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopySnapshotMessageRequestTypeDef(
     _RequiredCopySnapshotMessageRequestTypeDef, _OptionalCopySnapshotMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateCacheParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheParameterGroupMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
         "CacheParameterGroupFamily": str,
         "Description": str,
     },
@@ -1268,20 +1309,22 @@
     "_OptionalCreateCacheParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCacheParameterGroupMessageRequestTypeDef(
     _RequiredCreateCacheParameterGroupMessageRequestTypeDef,
     _OptionalCreateCacheParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateCacheSecurityGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheSecurityGroupMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "Description": str,
     },
 )
@@ -1289,20 +1332,22 @@
     "_OptionalCreateCacheSecurityGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCacheSecurityGroupMessageRequestTypeDef(
     _RequiredCreateCacheSecurityGroupMessageRequestTypeDef,
     _OptionalCreateCacheSecurityGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateCacheSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheSubnetGroupMessageRequestTypeDef",
     {
         "CacheSubnetGroupName": str,
         "CacheSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -1311,20 +1356,22 @@
     "_OptionalCreateCacheSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCacheSubnetGroupMessageRequestTypeDef(
     _RequiredCreateCacheSubnetGroupMessageRequestTypeDef,
     _OptionalCreateCacheSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotMessageRequestTypeDef",
     {
         "SnapshotName": str,
     },
 )
 _OptionalCreateSnapshotMessageRequestTypeDef = TypedDict(
@@ -1334,19 +1381,21 @@
         "CacheClusterId": str,
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSnapshotMessageRequestTypeDef(
     _RequiredCreateSnapshotMessageRequestTypeDef, _OptionalCreateSnapshotMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateUserGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateUserGroupMessageRequestTypeDef",
     {
         "UserGroupId": str,
         "Engine": str,
     },
 )
@@ -1355,19 +1404,47 @@
     {
         "UserIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateUserGroupMessageRequestTypeDef(
     _RequiredCreateUserGroupMessageRequestTypeDef, _OptionalCreateUserGroupMessageRequestTypeDef
 ):
     pass
 
+
+_RequiredCreateUserMessageRequestTypeDef = TypedDict(
+    "_RequiredCreateUserMessageRequestTypeDef",
+    {
+        "UserId": str,
+        "UserName": str,
+        "Engine": str,
+        "AccessString": str,
+    },
+)
+_OptionalCreateUserMessageRequestTypeDef = TypedDict(
+    "_OptionalCreateUserMessageRequestTypeDef",
+    {
+        "Passwords": Sequence[str],
+        "NoPasswordRequired": bool,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateUserMessageRequestTypeDef(
+    _RequiredCreateUserMessageRequestTypeDef, _OptionalCreateUserMessageRequestTypeDef
+):
+    pass
+
+
 _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
     {
         "ReservedCacheNodesOfferingId": str,
     },
 )
 _OptionalPurchaseReservedCacheNodesOfferingMessageRequestTypeDef = TypedDict(
@@ -1376,20 +1453,22 @@
         "ReservedCacheNodeId": str,
         "CacheNodeCount": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PurchaseReservedCacheNodesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
 ):
     pass
 
+
 AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
     "AllowedNodeTypeModificationsMessageTypeDef",
     {
         "ScaleUpModifications": List[str],
         "ScaleDownModifications": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1414,62 +1493,14 @@
     "TagListMessageTypeDef",
     {
         "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateUserMessageRequestTypeDef = TypedDict(
-    "_RequiredCreateUserMessageRequestTypeDef",
-    {
-        "UserId": str,
-        "UserName": str,
-        "Engine": str,
-        "AccessString": str,
-    },
-)
-_OptionalCreateUserMessageRequestTypeDef = TypedDict(
-    "_OptionalCreateUserMessageRequestTypeDef",
-    {
-        "Passwords": Sequence[str],
-        "NoPasswordRequired": bool,
-        "Tags": Sequence[TagTypeDef],
-        "AuthenticationMode": AuthenticationModeTypeDef,
-    },
-    total=False,
-)
-
-class CreateUserMessageRequestTypeDef(
-    _RequiredCreateUserMessageRequestTypeDef, _OptionalCreateUserMessageRequestTypeDef
-):
-    pass
-
-_RequiredModifyUserMessageRequestTypeDef = TypedDict(
-    "_RequiredModifyUserMessageRequestTypeDef",
-    {
-        "UserId": str,
-    },
-)
-_OptionalModifyUserMessageRequestTypeDef = TypedDict(
-    "_OptionalModifyUserMessageRequestTypeDef",
-    {
-        "AccessString": str,
-        "AppendAccessString": str,
-        "Passwords": Sequence[str],
-        "NoPasswordRequired": bool,
-        "AuthenticationMode": AuthenticationModeTypeDef,
-    },
-    total=False,
-)
-
-class ModifyUserMessageRequestTypeDef(
-    _RequiredModifyUserMessageRequestTypeDef, _OptionalModifyUserMessageRequestTypeDef
-):
-    pass
-
 UserResponseMetadataTypeDef = TypedDict(
     "UserResponseMetadataTypeDef",
     {
         "UserId": str,
         "UserName": str,
         "Status": str,
         "Engine": str,
@@ -1593,20 +1624,22 @@
         "NewReplicaCount": int,
         "ReplicaConfiguration": Sequence[ConfigureShardTypeDef],
         "ReplicasToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class DecreaseReplicaCountMessageRequestTypeDef(
     _RequiredDecreaseReplicaCountMessageRequestTypeDef,
     _OptionalDecreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredIncreaseReplicaCountMessageRequestTypeDef = TypedDict(
     "_RequiredIncreaseReplicaCountMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "ApplyImmediately": bool,
     },
 )
@@ -1615,20 +1648,22 @@
     {
         "NewReplicaCount": int,
         "ReplicaConfiguration": Sequence[ConfigureShardTypeDef],
     },
     total=False,
 )
 
+
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
+
 NodeSnapshotTypeDef = TypedDict(
     "NodeSnapshotTypeDef",
     {
         "CacheClusterId": str,
         "NodeGroupId": str,
         "CacheNodeId": str,
         "NodeGroupConfiguration": NodeGroupConfigurationTypeDef,
@@ -1738,20 +1773,22 @@
     {
         "Source": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
     _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
 ):
     pass
 
+
 DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
     "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
     {
         "CacheSecurityGroupName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1776,20 +1813,22 @@
     "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
 ):
     pass
 
+
 DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -1990,20 +2029,22 @@
     {
         "ResetAllParameters": bool,
         "ParameterNameValues": Sequence[ParameterNameValueTypeDef],
     },
     total=False,
 )
 
+
 class ResetCacheParameterGroupMessageRequestTypeDef(
     _RequiredResetCacheParameterGroupMessageRequestTypeDef,
     _OptionalResetCacheParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyReplicationGroupShardConfigurationMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "NodeGroupCount": int,
         "ApplyImmediately": bool,
     },
@@ -2014,20 +2055,22 @@
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
         "NodeGroupsToRemove": Sequence[str],
         "NodeGroupsToRetain": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyReplicationGroupShardConfigurationMessageRequestTypeDef(
     _RequiredModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     _OptionalModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
 ):
     pass
 
+
 RegionalConfigurationTypeDef = TypedDict(
     "RegionalConfigurationTypeDef",
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
@@ -2376,20 +2419,22 @@
     "_OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     {
         "RegionalConfigurations": Sequence[RegionalConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2537,20 +2582,22 @@
         "TransitEncryptionEnabled": bool,
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
     },
     total=False,
 )
 
+
 class CreateCacheClusterMessageRequestTypeDef(
     _RequiredCreateCacheClusterMessageRequestTypeDef,
     _OptionalCreateCacheClusterMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "ReplicationGroupDescription": str,
     },
 )
@@ -2587,25 +2634,26 @@
         "AtRestEncryptionEnabled": bool,
         "KmsKeyId": str,
         "UserGroupIds": Sequence[str],
         "LogDeliveryConfigurations": Sequence[LogDeliveryConfigurationRequestTypeDef],
         "DataTieringEnabled": bool,
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
-        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
+
 class CreateReplicationGroupMessageRequestTypeDef(
     _RequiredCreateReplicationGroupMessageRequestTypeDef,
     _OptionalCreateReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalModifyCacheClusterMessageRequestTypeDef = TypedDict(
@@ -2631,20 +2679,22 @@
         "AuthTokenUpdateStrategy": AuthTokenUpdateStrategyTypeType,
         "LogDeliveryConfigurations": Sequence[LogDeliveryConfigurationRequestTypeDef],
         "IpDiscovery": IpDiscoveryType,
     },
     total=False,
 )
 
+
 class ModifyCacheClusterMessageRequestTypeDef(
     _RequiredModifyCacheClusterMessageRequestTypeDef,
     _OptionalModifyCacheClusterMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationGroupMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
     },
 )
 _OptionalModifyReplicationGroupMessageRequestTypeDef = TypedDict(
@@ -2671,52 +2721,48 @@
         "AuthToken": str,
         "AuthTokenUpdateStrategy": AuthTokenUpdateStrategyTypeType,
         "UserGroupIdsToAdd": Sequence[str],
         "UserGroupIdsToRemove": Sequence[str],
         "RemoveUserGroups": bool,
         "LogDeliveryConfigurations": Sequence[LogDeliveryConfigurationRequestTypeDef],
         "IpDiscovery": IpDiscoveryType,
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
+
 class ModifyReplicationGroupMessageRequestTypeDef(
     _RequiredModifyReplicationGroupMessageRequestTypeDef,
     _OptionalModifyReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+
 PendingModifiedValuesTypeDef = TypedDict(
     "PendingModifiedValuesTypeDef",
     {
         "NumCacheNodes": int,
         "CacheNodeIdsToRemove": List[str],
         "EngineVersion": str,
         "CacheNodeType": str,
         "AuthTokenStatus": AuthTokenUpdateStatusType,
         "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
 ReplicationGroupPendingModifiedValuesTypeDef = TypedDict(
     "ReplicationGroupPendingModifiedValuesTypeDef",
     {
         "PrimaryClusterId": str,
         "AutomaticFailoverStatus": PendingAutomaticFailoverStatusType,
         "Resharding": ReshardingStatusTypeDef,
         "AuthTokenStatus": AuthTokenUpdateStatusType,
         "UserGroups": UserGroupsUpdateStatusTypeDef,
         "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
@@ -2782,15 +2828,14 @@
         "TransitEncryptionEnabled": bool,
         "AtRestEncryptionEnabled": bool,
         "ARN": str,
         "ReplicationGroupLogDeliveryEnabled": bool,
         "LogDeliveryConfigurations": List[LogDeliveryConfigurationTypeDef],
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
-        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
 ReplicationGroupTypeDef = TypedDict(
     "ReplicationGroupTypeDef",
     {
@@ -2819,15 +2864,14 @@
         "UserGroupIds": List[str],
         "LogDeliveryConfigurations": List[LogDeliveryConfigurationTypeDef],
         "ReplicationGroupCreateTime": datetime,
         "DataTiering": DataTieringStatusType,
         "AutoMinorVersionUpgrade": bool,
         "NetworkType": NetworkTypeType,
         "IpDiscovery": IpDiscoveryType,
-        "TransitEncryptionMode": TransitEncryptionModeType,
     },
     total=False,
 )
 
 CacheClusterMessageTypeDef = TypedDict(
     "CacheClusterMessageTypeDef",
     {
```

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/waiter.py` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache/waiter.pyi` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache.egg-info/PKG-INFO` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.26.39
-Summary: Type annotations for boto3.ElastiCache 1.26.39 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.4
+Summary: Type annotations for boto3.ElastiCache 1.26.4 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,15 +18,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticache?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.26.39](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -422,15 +421,14 @@
     DescribeReservedCacheNodesPaginatorName,
     DescribeServiceUpdatesPaginatorName,
     DescribeSnapshotsPaginatorName,
     DescribeUpdateActionsPaginatorName,
     DescribeUserGroupsPaginatorName,
     DescribeUsersPaginatorName,
     DestinationTypeType,
-    InputAuthenticationTypeType,
     IpDiscoveryType,
     LogDeliveryConfigurationStatusType,
     LogFormatType,
     LogTypeType,
     MultiAZStatusType,
     NetworkTypeType,
     NodeUpdateInitiatedByType,
@@ -440,15 +438,14 @@
     ReplicationGroupAvailableWaiterName,
     ReplicationGroupDeletedWaiterName,
     ServiceUpdateSeverityType,
     ServiceUpdateStatusType,
     ServiceUpdateTypeType,
     SlaMetType,
     SourceTypeType,
-    TransitEncryptionModeType,
     UpdateActionStatusType,
     ElastiCacheServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
     RegionName,
@@ -466,15 +463,14 @@
 `mypy_boto3_elasticache.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticache.type_defs import (
     TagTypeDef,
     ResponseMetadataTypeDef,
-    AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     BatchApplyUpdateActionMessageRequestTypeDef,
     BatchStopUpdateActionMessageRequestTypeDef,
     CacheParameterGroupStatusTypeDef,
     CacheSecurityGroupMembershipTypeDef,
@@ -532,14 +528,15 @@
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
+    ModifyUserMessageRequestTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
@@ -553,21 +550,20 @@
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
+    CreateUserMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     AllowedNodeTypeModificationsMessageTypeDef,
     CacheParameterGroupNameMessageTypeDef,
     EmptyResponseMetadataTypeDef,
     TagListMessageTypeDef,
-    CreateUserMessageRequestTypeDef,
-    ModifyUserMessageRequestTypeDef,
     UserResponseMetadataTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
```

### Comparing `mypy-boto3-elasticache-1.26.39/mypy_boto3_elasticache.egg-info/SOURCES.txt` & `mypy-boto3-elasticache-1.26.4/mypy_boto3_elasticache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.26.39/setup.py` & `mypy-boto3-elasticache-1.26.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,46 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-elasticache",
-    version="1.26.39",
+    version="1.26.4",
     packages=["mypy_boto3_elasticache"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElastiCache 1.26.39 service generated with mypy-boto3-builder"
-        " 7.12.2"
+        "Type annotations for boto3.ElastiCache 1.26.4 service generated with mypy-boto3-builder"
+        " 7.11.10"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 elasticache type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_elasticache": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_elasticache": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

