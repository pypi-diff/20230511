# Comparing `tmp/iam_actions-1.2.20230510.tar.gz` & `tmp/iam_actions-1.2.20230511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230510.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230511.tar", max compression
```

## Comparing `iam_actions-1.2.20230510.tar` & `iam_actions-1.2.20230511.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/README.md
--rw-r--r--   0        0        0      228 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/__init__.py
--rw-r--r--   0        0        0  4248257 2023-05-10 02:27:05.651587 iam_actions-1.2.20230510/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/services.py
--rw-r--r--   0        0        0   546378 2023-05-10 02:27:05.651587 iam_actions-1.2.20230510/iam_actions/policies.json
--rw-r--r--   0        0        0   193758 2023-05-10 02:27:05.651587 iam_actions-1.2.20230510/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   530028 2023-05-10 02:27:05.651587 iam_actions-1.2.20230510/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-10 02:27:06.695580 iam_actions-1.2.20230510/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230510/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230510/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-11 02:25:10.114679 iam_actions-1.2.20230511/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/README.md
+-rw-r--r--   0        0        0      228 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4251216 2023-05-11 02:26:45.768498 iam_actions-1.2.20230511/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   546752 2023-05-11 02:26:45.768498 iam_actions-1.2.20230511/iam_actions/policies.json
+-rw-r--r--   0        0        0   193758 2023-05-11 02:26:45.768498 iam_actions-1.2.20230511/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   530388 2023-05-11 02:26:45.768498 iam_actions-1.2.20230511/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-11 02:26:46.508512 iam_actions-1.2.20230511/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230511/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230511/PKG-INFO
```

### Comparing `iam_actions-1.2.20230510/LICENSE` & `iam_actions-1.2.20230511/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230510/README.md` & `iam_actions-1.2.20230511/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230510/iam_actions/actions.json` & `iam_actions-1.2.20230511/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998487492558333%*

 * *Differences: {"'memorydb'": "{'Connect': OrderedDict([('access_level', 'Undocumented'), ('action', 'Connect'), "*

 * *               "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *               "False), ('resources', [])])}",*

 * * "'quicksight'": "{'DescribeTopicRefresh': OrderedDict([('access_level', 'Undocumented'), "*

 * *                 "('action', 'DescribeTopicRefresh'), ('condition_keys', []), ('description', 'Not "*

 * *                 "Documented by AWS'), ('orphan', False), ('resources', [])]) […]*

```diff
@@ -95299,14 +95299,22 @@
             ],
             "description": "Grants permissions to apply service updates",
             "orphan": false,
             "resources": [
                 "cluster"
             ]
         },
+        "Connect": {
+            "access_level": "Undocumented",
+            "action": "Connect",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CopySnapshot": {
             "access_level": "Write",
             "action": "CopySnapshot",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
@@ -108474,14 +108482,30 @@
             ],
             "description": "Grants permission to create an alias for a theme version",
             "orphan": false,
             "resources": [
                 "theme"
             ]
         },
+        "CreateTopic": {
+            "access_level": "Undocumented",
+            "action": "CreateTopic",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateTopicRefreshSchedule": {
+            "access_level": "Undocumented",
+            "action": "CreateTopicRefreshSchedule",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateUser": {
             "access_level": "Write",
             "action": "CreateUser",
             "condition_keys": [],
             "description": "Grants permission to provision Amazon QuickSight authors and readers",
             "orphan": false,
             "resources": [
@@ -108704,14 +108728,30 @@
             "condition_keys": [],
             "description": "Grants permission to delete the alias of a theme",
             "orphan": false,
             "resources": [
                 "theme"
             ]
         },
+        "DeleteTopic": {
+            "access_level": "Undocumented",
+            "action": "DeleteTopic",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteTopicRefreshSchedule": {
+            "access_level": "Undocumented",
+            "action": "DeleteTopicRefreshSchedule",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteUser": {
             "access_level": "Write",
             "action": "DeleteUser",
             "condition_keys": [],
             "description": "Grants permission to delete a QuickSight user, given the user name",
             "orphan": false,
             "resources": [
@@ -109048,14 +109088,46 @@
             "condition_keys": [],
             "description": "Grants permission to describe permissions for a theme",
             "orphan": false,
             "resources": [
                 "theme"
             ]
         },
+        "DescribeTopic": {
+            "access_level": "Undocumented",
+            "action": "DescribeTopic",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeTopicPermissions": {
+            "access_level": "Undocumented",
+            "action": "DescribeTopicPermissions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeTopicRefresh": {
+            "access_level": "Undocumented",
+            "action": "DescribeTopicRefresh",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeTopicRefreshSchedule": {
+            "access_level": "Undocumented",
+            "action": "DescribeTopicRefreshSchedule",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeUser": {
             "access_level": "Read",
             "action": "DescribeUser",
             "condition_keys": [],
             "description": "Grants permission to describe a QuickSight user given the user name",
             "orphan": false,
             "resources": [
@@ -109364,14 +109436,30 @@
             "condition_keys": [],
             "description": "Grants permission to list all themes in an account",
             "orphan": false,
             "resources": [
                 "theme"
             ]
         },
+        "ListTopicRefreshSchedules": {
+            "access_level": "Undocumented",
+            "action": "ListTopicRefreshSchedules",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTopics": {
+            "access_level": "Undocumented",
+            "action": "ListTopics",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListUserGroups": {
             "access_level": "List",
             "action": "ListUserGroups",
             "condition_keys": [],
             "description": "Grants permission to list groups that a given user is a member of",
             "orphan": false,
             "resources": [
@@ -109873,14 +109961,38 @@
             "condition_keys": [],
             "description": "Grants permission to update permissions for a theme",
             "orphan": false,
             "resources": [
                 "theme"
             ]
         },
+        "UpdateTopic": {
+            "access_level": "Undocumented",
+            "action": "UpdateTopic",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateTopicPermissions": {
+            "access_level": "Undocumented",
+            "action": "UpdateTopicPermissions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateTopicRefreshSchedule": {
+            "access_level": "Undocumented",
+            "action": "UpdateTopicRefreshSchedule",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateUser": {
             "access_level": "Write",
             "action": "UpdateUser",
             "condition_keys": [],
             "description": "Grants permission to update an Amazon QuickSight user",
             "orphan": false,
             "resources": [
@@ -133027,20 +133139,22 @@
             "resources": [
                 "signing-profile"
             ]
         }
     },
     "simspaceweaver": {
         "CreateSnapshot": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateSnapshot",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create a snapshot",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Simulation"
+            ]
         },
         "DeleteApp": {
             "access_level": "Write",
             "action": "DeleteApp",
             "condition_keys": [],
             "description": "Grants permission to delete an app",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230510/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230511/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230510/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230511/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230510/iam_actions/generate/generate.py` & `iam_actions-1.2.20230511/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230510/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230511/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230510/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230511/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230510/iam_actions/generate/services.py` & `iam_actions-1.2.20230511/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230510/iam_actions/policies.json` & `iam_actions-1.2.20230511/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999855852666855%*

 * *Differences: {"'serviceMap'": "{'AWS Marketplace Seller Reporting': {'ARNFormat': "*

 * *                 "'arn:aws:aws-marketplace::${Account}:${Catalog}/${ResourceType}/${ResourcePath}'}, "*

 * *                 "'Amazon QuickSight': {'Actions': {insert: [(24, 'CreateTopic'), (25, "*

 * *                 "'CreateTopicRefreshSchedule'), (48, 'DeleteTopic'), (49, "*

 * *                 "'DeleteTopicRefreshSchedule'), (83, 'DescribeTopic'), (84, "*

 * *                 "'DescribeTopicPermissions'), (85, 'DescribeTopicRefresh'), (86, "*

 * *          […]*

```diff
@@ -6373,15 +6373,15 @@
                 "DescribeProcurementSystemConfiguration",
                 "PutProcurementSystemConfiguration"
             ],
             "HasResource": false,
             "StringPrefix": "aws-marketplace"
         },
         "AWS Marketplace Seller Reporting": {
-            "ARNFormat": "arn:aws:aws-marketplace::${Account}:${Catalog}/${ResourceType}/${ResourceId}",
+            "ARNFormat": "arn:aws:aws-marketplace::${Account}:${Catalog}/${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:aws-marketplace:.+",
             "Actions": [
                 "GetSellerDashboard"
             ],
             "HasResource": true,
             "StringPrefix": "aws-marketplace"
         },
@@ -15690,14 +15690,15 @@
             "StringPrefix": "mechanicalturk"
         },
         "Amazon MemoryDB": {
             "ARNFormat": "arn:aws:memorydb:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:memorydb:.+:.+:.+",
             "Actions": [
                 "BatchUpdateCluster",
+                "Connect",
                 "CopySnapshot",
                 "CreateAcl",
                 "CreateCluster",
                 "CreateParameterGroup",
                 "CreateSnapshot",
                 "CreateSubnetGroup",
                 "CreateUser",
@@ -16600,14 +16601,16 @@
                 "CreateNamespace",
                 "CreateReader",
                 "CreateRefreshSchedule",
                 "CreateTemplate",
                 "CreateTemplateAlias",
                 "CreateTheme",
                 "CreateThemeAlias",
+                "CreateTopic",
+                "CreateTopicRefreshSchedule",
                 "CreateUser",
                 "CreateVPCConnection",
                 "DeleteAccountCustomization",
                 "DeleteAccountSubscription",
                 "DeleteAnalysis",
                 "DeleteCustomPermissions",
                 "DeleteDashboard",
@@ -16622,14 +16625,16 @@
                 "DeleteIAMPolicyAssignment",
                 "DeleteNamespace",
                 "DeleteRefreshSchedule",
                 "DeleteTemplate",
                 "DeleteTemplateAlias",
                 "DeleteTheme",
                 "DeleteThemeAlias",
+                "DeleteTopic",
+                "DeleteTopicRefreshSchedule",
                 "DeleteUser",
                 "DeleteUserByPrincipalId",
                 "DeleteVPCConnection",
                 "DescribeAccountCustomization",
                 "DescribeAccountSettings",
                 "DescribeAccountSubscription",
                 "DescribeAnalysis",
@@ -16655,14 +16660,18 @@
                 "DescribeRefreshSchedule",
                 "DescribeTemplate",
                 "DescribeTemplateAlias",
                 "DescribeTemplatePermissions",
                 "DescribeTheme",
                 "DescribeThemeAlias",
                 "DescribeThemePermissions",
+                "DescribeTopic",
+                "DescribeTopicPermissions",
+                "DescribeTopicRefresh",
+                "DescribeTopicRefreshSchedule",
                 "DescribeUser",
                 "DescribeVPCConnection",
                 "GenerateEmbedUrlForAnonymousUser",
                 "GenerateEmbedUrlForRegisteredUser",
                 "GetAnonymousUserEmbedUrl",
                 "GetAuthCode",
                 "GetDashboardEmbedUrl",
@@ -16686,14 +16695,16 @@
                 "ListTagsForResource",
                 "ListTemplateAliases",
                 "ListTemplateVersions",
                 "ListTemplates",
                 "ListThemeAliases",
                 "ListThemeVersions",
                 "ListThemes",
+                "ListTopicRefreshSchedules",
+                "ListTopics",
                 "ListUserGroups",
                 "ListUsers",
                 "ListVPCConnections",
                 "PassDataSet",
                 "PassDataSource",
                 "PutDataSetRefreshProperties",
                 "RegisterUser",
@@ -16734,14 +16745,17 @@
                 "UpdateResourcePermissions",
                 "UpdateTemplate",
                 "UpdateTemplateAlias",
                 "UpdateTemplatePermissions",
                 "UpdateTheme",
                 "UpdateThemeAlias",
                 "UpdateThemePermissions",
+                "UpdateTopic",
+                "UpdateTopicPermissions",
+                "UpdateTopicRefreshSchedule",
                 "UpdateUser",
                 "UpdateVPCConnection"
             ],
             "HasResource": true,
             "StringPrefix": "quicksight",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
```

### Comparing `iam_actions-1.2.20230510/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230511/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230510/iam_actions/services.json` & `iam_actions-1.2.20230511/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999910927089023%*

 * *Differences: {"'aws-marketplace'": "{'ARNFormats': {insert: [(1, "*

 * *                      "'arn:aws:aws-marketplace::${Account}:${Catalog}/${ResourceType}/${ResourcePath}')], "*

 * *                      'delete: [1]}}',*

 * * "'memorydb'": "{'Actions': {insert: [(1, 'Connect')]}}",*

 * * "'quicksight'": "{'Actions': {insert: [(24, 'CreateTopic'), (25, 'CreateTopicRefreshSchedule'), "*

 * *                 "(48, 'DeleteTopic'), (49, 'DeleteTopicRefreshSchedule'), (83, 'DescribeTopic'), "*

 * *                 "(84, 'DescribeTopicPermissions'), ( […]*

```diff
@@ -1577,15 +1577,15 @@
         "ServiceNames": [
             "AWS Auto Scaling"
         ]
     },
     "aws-marketplace": {
         "ARNFormats": [
             "arn:aws:aws-marketplace:${Region}:${Account}:${Catalog}/${ResourceType}/${ResourceId}",
-            "arn:aws:aws-marketplace::${Account}:${Catalog}/${ResourceType}/${ResourceId}"
+            "arn:aws:aws-marketplace::${Account}:${Catalog}/${ResourceType}/${ResourcePath}"
         ],
         "ARNRegexes": [
             "^arn:aws:aws-marketplace:.+"
         ],
         "Actions": [
             "AcceptAgreementApprovalRequest",
             "AcceptAgreementRequest",
@@ -13370,14 +13370,15 @@
             "arn:aws:memorydb:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:memorydb:.+:.+:.+"
         ],
         "Actions": [
             "BatchUpdateCluster",
+            "Connect",
             "CopySnapshot",
             "CreateAcl",
             "CreateCluster",
             "CreateParameterGroup",
             "CreateSnapshot",
             "CreateSubnetGroup",
             "CreateUser",
@@ -15279,14 +15280,16 @@
             "CreateNamespace",
             "CreateReader",
             "CreateRefreshSchedule",
             "CreateTemplate",
             "CreateTemplateAlias",
             "CreateTheme",
             "CreateThemeAlias",
+            "CreateTopic",
+            "CreateTopicRefreshSchedule",
             "CreateUser",
             "CreateVPCConnection",
             "DeleteAccountCustomization",
             "DeleteAccountSubscription",
             "DeleteAnalysis",
             "DeleteCustomPermissions",
             "DeleteDashboard",
@@ -15301,14 +15304,16 @@
             "DeleteIAMPolicyAssignment",
             "DeleteNamespace",
             "DeleteRefreshSchedule",
             "DeleteTemplate",
             "DeleteTemplateAlias",
             "DeleteTheme",
             "DeleteThemeAlias",
+            "DeleteTopic",
+            "DeleteTopicRefreshSchedule",
             "DeleteUser",
             "DeleteUserByPrincipalId",
             "DeleteVPCConnection",
             "DescribeAccountCustomization",
             "DescribeAccountSettings",
             "DescribeAccountSubscription",
             "DescribeAnalysis",
@@ -15334,14 +15339,18 @@
             "DescribeRefreshSchedule",
             "DescribeTemplate",
             "DescribeTemplateAlias",
             "DescribeTemplatePermissions",
             "DescribeTheme",
             "DescribeThemeAlias",
             "DescribeThemePermissions",
+            "DescribeTopic",
+            "DescribeTopicPermissions",
+            "DescribeTopicRefresh",
+            "DescribeTopicRefreshSchedule",
             "DescribeUser",
             "DescribeVPCConnection",
             "GenerateEmbedUrlForAnonymousUser",
             "GenerateEmbedUrlForRegisteredUser",
             "GetAnonymousUserEmbedUrl",
             "GetAuthCode",
             "GetDashboardEmbedUrl",
@@ -15365,14 +15374,16 @@
             "ListTagsForResource",
             "ListTemplateAliases",
             "ListTemplateVersions",
             "ListTemplates",
             "ListThemeAliases",
             "ListThemeVersions",
             "ListThemes",
+            "ListTopicRefreshSchedules",
+            "ListTopics",
             "ListUserGroups",
             "ListUsers",
             "ListVPCConnections",
             "PassDataSet",
             "PassDataSource",
             "PutDataSetRefreshProperties",
             "RegisterUser",
@@ -15413,14 +15424,17 @@
             "UpdateResourcePermissions",
             "UpdateTemplate",
             "UpdateTemplateAlias",
             "UpdateTemplatePermissions",
             "UpdateTheme",
             "UpdateThemeAlias",
             "UpdateThemePermissions",
+            "UpdateTopic",
+            "UpdateTopicPermissions",
+            "UpdateTopicRefreshSchedule",
             "UpdateUser",
             "UpdateVPCConnection"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys",
```

### Comparing `iam_actions-1.2.20230510/pyproject.toml` & `iam_actions-1.2.20230511/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230510"
+version = "1.2.20230511"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230510/setup.py` & `iam_actions-1.2.20230511/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230510',
+    'version': '1.2.20230511',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230510/PKG-INFO` & `iam_actions-1.2.20230511/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230510
+Version: 1.2.20230511
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

