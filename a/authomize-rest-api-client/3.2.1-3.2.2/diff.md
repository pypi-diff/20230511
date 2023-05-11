# Comparing `tmp/authomize-rest-api-client-3.2.1.tar.gz` & `tmp/authomize-rest-api-client-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-3.2.1.tar", last modified: Tue May  9 05:17:30 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-3.2.2.tar", last modified: Wed May 10 16:28:42 2023, max compression
```

## Comparing `authomize-rest-api-client-3.2.1.tar` & `authomize-rest-api-client-3.2.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.110172 authomize-rest-api-client-3.2.1/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-09 05:17:30.110172 authomize-rest-api-client-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2160 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2631 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10105 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    12633 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73614 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24531 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.106172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185721 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.110172 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64932 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-09 05:17:10.000000 authomize-rest-api-client-3.2.1/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 05:17:30.110172 authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-09 05:17:30.000000 authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-09 05:17:30.000000 authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 05:17:30.000000 authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      216 2023-05-09 05:17:30.000000 authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-09 05:17:30.000000 authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-09 05:17:30.110172 authomize-rest-api-client-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1163 2023-05-09 05:17:28.000000 authomize-rest-api-client-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10105 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    12633 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73614 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24509 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185721 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64900 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-10 16:28:22.000000 authomize-rest-api-client-3.2.2/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-10 16:28:42.000000 authomize-rest-api-client-3.2.2/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-10 16:28:42.000000 authomize-rest-api-client-3.2.2/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 16:28:42.000000 authomize-rest-api-client-3.2.2/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      216 2023-05-10 16:28:42.000000 authomize-rest-api-client-3.2.2/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-10 16:28:42.000000 authomize-rest-api-client-3.2.2/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-10 16:28:42.411916 authomize-rest-api-client-3.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-05-10 16:28:26.000000 authomize-rest-api-client-3.2.2/setup.py
```

### Comparing `authomize-rest-api-client-3.2.1/LICENSE.txt` & `authomize-rest-api-client-3.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.1/README.md` & `authomize-rest-api-client-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.1/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-3.2.2/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-3.2.2/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-3.2.2/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-3.2.2/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.1/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-3.2.2/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-3.2.2/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.1/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-3.2.2/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-05-01T07:04:37+00:00
+#   timestamp: 2023-05-10T16:13:43+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
@@ -317,15 +317,15 @@
     A_8_2_3 = 'A.8.2.3'
     A_7_3_1 = 'A.7.3.1'
     A_8_1_4 = 'A.8.1.4'
 
 
 class MeResponse(BaseModel):
     version: Optional[str] = Field(
-        default='3.1.6', description='**version**', title='Version'
+        default='3.2.1', description='**version**', title='Version'
     )
     id: str = Field(..., description='**id**', title='Id')
     tenant: str = Field(..., description='**tenant**', title='Tenant')
 
 
 class NonPaginatedResponseSchemaCommentSchema(BaseModel):
     class Config:
@@ -699,29 +699,29 @@
     campaignId: str = Field(
         ..., description='ID of the Campaign.\n', title='Campaignid'
     )
     reviewerId: str = Field(..., description='Reviewer ID', title='Reviewerid')
     reviewer: Optional[ReviewerSchema] = Field(
         default=None, description='Details of the reviewer.\n', title='Reviewer'
     )
-    accessById: str = Field(
+    actorId: str = Field(
         ...,
-        description='Access by ID (Account or Grouping ID) that their access was reviewed. \n',
-        title='Accessbyid',
+        description='Actor ID (Account or Grouping ID) that their access was reviewed. \n',
+        title='Actorid',
     )
-    accessByType: AccessByType = Field(
+    actorType: AccessByType = Field(
         ...,
         description='Type of entity that was reviewed, can be Account or Grouping.\n',
     )
-    accessToId: str = Field(
+    targetId: str = Field(
         ...,
-        description='Access to ID (Asset or Grouping ID) that the access to was reviewed, for example a database the access to was reviewed.  \n',
-        title='Accesstoid',
+        description='Target ID (Asset or Grouping ID) that the access to was reviewed, for example a database the access to was reviewed.  \n',
+        title='Targetid',
     )
-    accessToType: AccessToType = Field(
+    targetType: AccessToType = Field(
         ..., description='Assets or grouping that the access to was reviewed.  \n'
     )
     privilegeId: Optional[str] = Field(
         default=None,
         description='ID of the privileges that was reviewed. \n',
         title='Privilegeid',
     )
```

### Comparing `authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-3.2.2/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.1/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-3.2.2/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874705551609848%*

 * *Differences: {"'components'": "{'schemas': {'CampaignsPermissionSchema': {'required': {insert: [(3, 'actorId'), "*

 * *                 "(4, 'actorType'), (5, 'targetId'), (6, 'targetType')], delete: [6, 5, 4, 3]}, "*

 * *                 "'properties': {'actorId': OrderedDict([('title', 'Actorid'), ('type', 'string'), "*

 * *                 "('description', 'Actor ID (Account or Grouping ID) that their access was "*

 * *                 "reviewed. \\n')]), 'actorType': OrderedDict([('allOf', [OrderedDict([('$ref', "*

 * *                 "'#/ […]*

```diff
@@ -269,40 +269,27 @@
                     }
                 },
                 "title": "CampaignStatusFilter",
                 "type": "object"
             },
             "CampaignsPermissionSchema": {
                 "properties": {
-                    "accessById": {
-                        "description": "Access by ID (Account or Grouping ID) that their access was reviewed. \n",
-                        "title": "Accessbyid",
+                    "actorId": {
+                        "description": "Actor ID (Account or Grouping ID) that their access was reviewed. \n",
+                        "title": "Actorid",
                         "type": "string"
                     },
-                    "accessByType": {
+                    "actorType": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/AccessByType"
                             }
                         ],
                         "description": "Type of entity that was reviewed, can be Account or Grouping.\n"
                     },
-                    "accessToId": {
-                        "description": "Access to ID (Asset or Grouping ID) that the access to was reviewed, for example a database the access to was reviewed.  \n",
-                        "title": "Accesstoid",
-                        "type": "string"
-                    },
-                    "accessToType": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/AccessToType"
-                            }
-                        ],
-                        "description": "Assets or grouping that the access to was reviewed.  \n"
-                    },
                     "campaignId": {
                         "description": "ID of the Campaign.\n",
                         "title": "Campaignid",
                         "type": "string"
                     },
                     "decision": {
                         "allOf": [
@@ -336,24 +323,37 @@
                         "description": "Details of the reviewer.\n",
                         "title": "Reviewer"
                     },
                     "reviewerId": {
                         "description": "Reviewer ID",
                         "title": "Reviewerid",
                         "type": "string"
+                    },
+                    "targetId": {
+                        "description": "Target ID (Asset or Grouping ID) that the access to was reviewed, for example a database the access to was reviewed.  \n",
+                        "title": "Targetid",
+                        "type": "string"
+                    },
+                    "targetType": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/AccessToType"
+                            }
+                        ],
+                        "description": "Assets or grouping that the access to was reviewed.  \n"
                     }
                 },
                 "required": [
                     "id",
                     "campaignId",
                     "reviewerId",
-                    "accessById",
-                    "accessByType",
-                    "accessToId",
-                    "accessToType"
+                    "actorId",
+                    "actorType",
+                    "targetId",
+                    "targetType"
                 ],
                 "title": "CampaignsPermissionSchema",
                 "type": "object"
             },
             "Ccm301": {
                 "properties": {
                     "id": {
@@ -1005,15 +1005,15 @@
                     },
                     "tenant": {
                         "description": "**tenant**",
                         "title": "Tenant",
                         "type": "string"
                     },
                     "version": {
-                        "default": "3.1.6",
+                        "default": "3.2.1",
                         "description": "**version**",
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
@@ -1734,15 +1734,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "3.1.6",
+        "version": "3.2.1",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
```

### Comparing `authomize-rest-api-client-3.2.1/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-3.2.2/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.1/setup.py` & `authomize-rest-api-client-3.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='3.2.1',
+        version='3.2.2',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

