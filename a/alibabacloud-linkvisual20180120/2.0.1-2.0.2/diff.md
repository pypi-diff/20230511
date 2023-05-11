# Comparing `tmp/alibabacloud_linkvisual20180120-2.0.1.tar.gz` & `tmp/alibabacloud_linkvisual20180120-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_linkvisual20180120-2.0.1.tar", last modified: Sun Jan 10 14:32:27 2021, max compression
+gzip compressed data, was "dist/alibabacloud_linkvisual20180120-2.0.2.tar", last modified: Tue Mar 30 04:47:18 2021, max compression
```

## Comparing `alibabacloud_linkvisual20180120-2.0.1.tar` & `alibabacloud_linkvisual20180120-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/
--rw-r--r--   0 root         (0) root         (0)       73 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2370 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1043 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/alibabacloud_linkvisual20180120/
--rw-r--r--   0 root         (0) root         (0)       21 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/alibabacloud_linkvisual20180120/__init__.py
--rw-r--r--   0 root         (0) root         (0)   243724 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/alibabacloud_linkvisual20180120/client.py
--rw-r--r--   0 root         (0) root         (0)   671899 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/alibabacloud_linkvisual20180120/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/alibabacloud_linkvisual20180120.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2370 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/alibabacloud_linkvisual20180120.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/alibabacloud_linkvisual20180120.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/alibabacloud_linkvisual20180120.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/alibabacloud_linkvisual20180120.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/alibabacloud_linkvisual20180120.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2597 2021-01-10 14:32:27.000000 alibabacloud_linkvisual20180120-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)      146 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2370 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1043 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/alibabacloud_linkvisual20180120/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/alibabacloud_linkvisual20180120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   390362 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/alibabacloud_linkvisual20180120/client.py
+-rw-r--r--   0 root         (0) root         (0)   695266 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/alibabacloud_linkvisual20180120/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/alibabacloud_linkvisual20180120.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2370 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/alibabacloud_linkvisual20180120.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/alibabacloud_linkvisual20180120.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/alibabacloud_linkvisual20180120.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/alibabacloud_linkvisual20180120.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/alibabacloud_linkvisual20180120.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2645 2021-03-30 04:47:18.000000 alibabacloud_linkvisual20180120-2.0.2/setup.py
```

### Comparing `alibabacloud_linkvisual20180120-2.0.1/LICENSE` & `alibabacloud_linkvisual20180120-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkvisual20180120-2.0.1/PKG-INFO` & `alibabacloud_linkvisual20180120-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_linkvisual20180120
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud LinkVisual (20180120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkvisual20180120-2.0.1/README-CN.md` & `alibabacloud_linkvisual20180120-2.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkvisual20180120-2.0.1/README.md` & `alibabacloud_linkvisual20180120-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkvisual20180120-2.0.1/alibabacloud_linkvisual20180120/models.py` & `alibabacloud_linkvisual20180120-2.0.2/alibabacloud_linkvisual20180120/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,49 +3,41 @@
 from Tea.model import TeaModel
 from typing import Dict, Any, List
 
 
 class AddEventRecordPlanDeviceRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         plan_id: str = None,
         stream_type: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.plan_id = plan_id
         self.stream_type = stream_type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.stream_type is not None:
             result['StreamType'] = self.stream_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         if m.get('StreamType') is not None:
             self.stream_type = m.get('StreamType')
         return self
@@ -64,14 +56,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -104,14 +100,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -124,45 +124,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AddFaceDeviceGroupRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         device_group_name: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.device_group_name = device_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.device_group_name is not None:
             result['DeviceGroupName'] = self.device_group_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('DeviceGroupName') is not None:
             self.device_group_name = m.get('DeviceGroupName')
         return self
 
 
@@ -177,14 +169,18 @@
         self.modified_time = modified_time
         self.device_group_name = device_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.device_group_id is not None:
             result['DeviceGroupId'] = self.device_group_id
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.device_group_name is not None:
             result['DeviceGroupName'] = self.device_group_name
@@ -217,14 +213,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -262,14 +262,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -282,57 +286,49 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AddFaceDeviceToDeviceGroupRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         iot_instance_id: str = None,
         product_key: str = None,
         device_name: str = None,
         device_group_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.iot_instance_id = iot_instance_id
         self.product_key = product_key
         self.device_name = device_name
         self.device_group_id = device_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         if self.product_key is not None:
             result['ProductKey'] = self.product_key
         if self.device_name is not None:
             result['DeviceName'] = self.device_name
         if self.device_group_id is not None:
             result['DeviceGroupId'] = self.device_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         if m.get('ProductKey') is not None:
             self.product_key = m.get('ProductKey')
         if m.get('DeviceName') is not None:
@@ -355,14 +351,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -395,14 +395,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -415,57 +419,49 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AddFaceUserRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         face_pic_url: str = None,
         custom_user_id: str = None,
         name: str = None,
         params: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.face_pic_url = face_pic_url
         self.custom_user_id = custom_user_id
         self.name = name
         self.params = params
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.face_pic_url is not None:
             result['FacePicUrl'] = self.face_pic_url
         if self.custom_user_id is not None:
             result['CustomUserId'] = self.custom_user_id
         if self.name is not None:
             result['Name'] = self.name
         if self.params is not None:
             result['Params'] = self.params
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('FacePicUrl') is not None:
             self.face_pic_url = m.get('FacePicUrl')
         if m.get('CustomUserId') is not None:
             self.custom_user_id = m.get('CustomUserId')
         if m.get('Name') is not None:
@@ -488,14 +484,18 @@
         self.user_id = user_id
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.params is not None:
             result['Params'] = self.params
         if self.custom_user_id is not None:
             result['CustomUserId'] = self.custom_user_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
@@ -532,14 +532,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -577,14 +581,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -597,45 +605,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AddFaceUserGroupRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         user_group_name: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.user_group_name = user_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.user_group_name is not None:
             result['UserGroupName'] = self.user_group_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('UserGroupName') is not None:
             self.user_group_name = m.get('UserGroupName')
         return self
 
 
@@ -650,14 +650,18 @@
         self.user_group_id = user_group_id
         self.user_group_name = user_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.user_group_id is not None:
             result['UserGroupId'] = self.user_group_id
         if self.user_group_name is not None:
             result['UserGroupName'] = self.user_group_name
@@ -690,14 +694,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -735,14 +743,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -755,57 +767,49 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AddFaceUserGroupAndDeviceGroupRelationRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         iot_instance_id: str = None,
         user_group_id: str = None,
         device_group_id: str = None,
         relation: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.iot_instance_id = iot_instance_id
         self.user_group_id = user_group_id
         self.device_group_id = device_group_id
         self.relation = relation
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         if self.user_group_id is not None:
             result['UserGroupId'] = self.user_group_id
         if self.device_group_id is not None:
             result['DeviceGroupId'] = self.device_group_id
         if self.relation is not None:
             result['Relation'] = self.relation
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         if m.get('UserGroupId') is not None:
             self.user_group_id = m.get('UserGroupId')
         if m.get('DeviceGroupId') is not None:
@@ -824,14 +828,18 @@
         self.modified_time = modified_time
         self.control_id = control_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.control_id is not None:
             result['ControlId'] = self.control_id
         return result
 
@@ -860,14 +868,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -905,14 +917,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -925,49 +941,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AddFaceUserPictureRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         user_id: str = None,
         face_pic_url: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.user_id = user_id
         self.face_pic_url = face_pic_url
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
         if self.face_pic_url is not None:
             result['FacePicUrl'] = self.face_pic_url
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('FacePicUrl') is not None:
             self.face_pic_url = m.get('FacePicUrl')
         return self
@@ -988,14 +996,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -1032,14 +1044,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -1052,49 +1068,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AddFaceUserToUserGroupRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         user_id: str = None,
         user_group_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.user_id = user_id
         self.user_group_id = user_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
         if self.user_group_id is not None:
             result['UserGroupId'] = self.user_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('UserGroupId') is not None:
             self.user_group_id = m.get('UserGroupId')
         return self
@@ -1113,14 +1121,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -1153,14 +1165,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -1173,49 +1189,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AddRecordPlanDeviceRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         plan_id: str = None,
         stream_type: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.plan_id = plan_id
         self.stream_type = stream_type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.stream_type is not None:
             result['StreamType'] = self.stream_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         if m.get('StreamType') is not None:
             self.stream_type = m.get('StreamType')
         return self
@@ -1234,14 +1242,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -1274,14 +1286,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -1294,90 +1310,86 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BindAIPlanWithDevicesRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
         iot_id_list: List[str] = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
         self.iot_id_list = iot_id_list
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.iot_id_list is not None:
             result['IotIdList'] = self.iot_id_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         if m.get('IotIdList') is not None:
             self.iot_id_list = m.get('IotIdList')
         return self
 
 
 class BindAIPlanWithDevicesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
         error_message: str = None,
         code: str = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
         self.error_message = error_message
         self.code = code
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class BindAIPlanWithDevicesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -1389,14 +1401,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -1409,47 +1425,45 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BindPictureSearchAppWithDevicesRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         app_instance_id: str = None,
+        iot_instance_id: str = None,
         device_iot_ids: List[str] = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.app_instance_id = app_instance_id
+        self.iot_instance_id = iot_instance_id
         self.device_iot_ids = device_iot_ids
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.app_instance_id is not None:
             result['AppInstanceId'] = self.app_instance_id
+        if self.iot_instance_id is not None:
+            result['IotInstanceId'] = self.iot_instance_id
         if self.device_iot_ids is not None:
             result['DeviceIotIds'] = self.device_iot_ids
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AppInstanceId') is not None:
             self.app_instance_id = m.get('AppInstanceId')
+        if m.get('IotInstanceId') is not None:
+            self.iot_instance_id = m.get('IotInstanceId')
         if m.get('DeviceIotIds') is not None:
             self.device_iot_ids = m.get('DeviceIotIds')
         return self
 
 
 class BindPictureSearchAppWithDevicesResponseBody(TeaModel):
     def __init__(
@@ -1464,14 +1478,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -1504,14 +1522,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -1524,57 +1546,49 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CheckFaceUserDoExistOnDeviceRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         iot_instance_id: str = None,
         user_id: str = None,
         product_key: str = None,
         device_name: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.iot_instance_id = iot_instance_id
         self.user_id = user_id
         self.product_key = product_key
         self.device_name = device_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
         if self.product_key is not None:
             result['ProductKey'] = self.product_key
         if self.device_name is not None:
             result['DeviceName'] = self.device_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('ProductKey') is not None:
@@ -1591,14 +1605,18 @@
     ):
         self.do_exist = do_exist
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.do_exist is not None:
             result['DoExist'] = self.do_exist
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
@@ -1623,14 +1641,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -1668,14 +1690,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -1688,53 +1714,45 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ClearFaceDeviceDBRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         iot_instance_id: str = None,
         product_key: str = None,
         device_name: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.iot_instance_id = iot_instance_id
         self.product_key = product_key
         self.device_name = device_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         if self.product_key is not None:
             result['ProductKey'] = self.product_key
         if self.device_name is not None:
             result['DeviceName'] = self.device_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         if m.get('ProductKey') is not None:
             self.product_key = m.get('ProductKey')
         if m.get('DeviceName') is not None:
@@ -1757,14 +1775,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -1801,14 +1823,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -1821,133 +1847,133 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ConfigAIActionRequestDataTypeConfigList(TeaModel):
     def __init__(
         self,
-        configs: str = None,
         data_type: str = None,
+        configs: str = None,
     ):
-        self.configs = configs
         self.data_type = data_type
+        self.configs = configs
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.configs is not None:
-            result['Configs'] = self.configs
         if self.data_type is not None:
             result['DataType'] = self.data_type
+        if self.configs is not None:
+            result['Configs'] = self.configs
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Configs') is not None:
-            self.configs = m.get('Configs')
         if m.get('DataType') is not None:
             self.data_type = m.get('DataType')
+        if m.get('Configs') is not None:
+            self.configs = m.get('Configs')
         return self
 
 
 class ConfigAIActionRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         action_id: str = None,
-        data_type_config_list: List[ConfigAIActionRequestDataTypeConfigList] = None,
         algo_config: str = None,
+        data_type_config_list: List[ConfigAIActionRequestDataTypeConfigList] = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.action_id = action_id
-        self.data_type_config_list = data_type_config_list
         self.algo_config = algo_config
+        self.data_type_config_list = data_type_config_list
 
     def validate(self):
         if self.data_type_config_list:
             for k in self.data_type_config_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.action_id is not None:
             result['ActionId'] = self.action_id
+        if self.algo_config is not None:
+            result['AlgoConfig'] = self.algo_config
         result['DataTypeConfigList'] = []
         if self.data_type_config_list is not None:
             for k in self.data_type_config_list:
                 result['DataTypeConfigList'].append(k.to_map() if k else None)
-        if self.algo_config is not None:
-            result['AlgoConfig'] = self.algo_config
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('ActionId') is not None:
             self.action_id = m.get('ActionId')
+        if m.get('AlgoConfig') is not None:
+            self.algo_config = m.get('AlgoConfig')
         self.data_type_config_list = []
         if m.get('DataTypeConfigList') is not None:
             for k in m.get('DataTypeConfigList'):
                 temp_model = ConfigAIActionRequestDataTypeConfigList()
                 self.data_type_config_list.append(temp_model.from_map(k))
-        if m.get('AlgoConfig') is not None:
-            self.algo_config = m.get('AlgoConfig')
         return self
 
 
 class ConfigAIActionResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
         error_message: str = None,
         code: str = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
         self.error_message = error_message
         self.code = code
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class ConfigAIActionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -1959,14 +1985,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -1979,57 +2009,49 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateAIAppRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         app_template_id: str = None,
         app_template_version: str = None,
         level: int = None,
         name: str = None,
         description: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.app_template_id = app_template_id
         self.app_template_version = app_template_version
         self.level = level
         self.name = name
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.app_template_id is not None:
             result['AppTemplateId'] = self.app_template_id
         if self.app_template_version is not None:
             result['AppTemplateVersion'] = self.app_template_version
         if self.level is not None:
             result['Level'] = self.level
         if self.name is not None:
             result['Name'] = self.name
         if self.description is not None:
             result['Description'] = self.description
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AppTemplateId') is not None:
             self.app_template_id = m.get('AppTemplateId')
         if m.get('AppTemplateVersion') is not None:
             self.app_template_version = m.get('AppTemplateVersion')
         if m.get('Level') is not None:
             self.level = m.get('Level')
         if m.get('Name') is not None:
@@ -2054,14 +2076,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -2098,14 +2124,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -2118,49 +2148,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateAIPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         app_id: str = None,
         plan_template_id: str = None,
         description: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.app_id = app_id
         self.plan_template_id = plan_template_id
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.app_id is not None:
             result['AppId'] = self.app_id
         if self.plan_template_id is not None:
             result['PlanTemplateId'] = self.plan_template_id
         if self.description is not None:
             result['Description'] = self.description
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AppId') is not None:
             self.app_id = m.get('AppId')
         if m.get('PlanTemplateId') is not None:
             self.plan_template_id = m.get('PlanTemplateId')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         return self
@@ -2181,14 +2203,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -2225,14 +2251,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -2245,45 +2275,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateAlgorithmRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         name: str = None,
         description: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.name = name
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.name is not None:
             result['Name'] = self.name
         if self.description is not None:
             result['Description'] = self.description
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         return self
 
 
@@ -2302,14 +2324,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -2346,14 +2372,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -2366,49 +2396,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateDevicePurifyJobRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         start_time: int = None,
         end_time: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.start_time = start_time
         self.end_time = end_time
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         return self
@@ -2429,14 +2451,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -2473,14 +2499,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -2493,45 +2523,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateDevicePurifyJobByPlanIdRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
         utc: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
         self.utc = utc
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.utc is not None:
             result['Utc'] = self.utc
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         if m.get('Utc') is not None:
             self.utc = m.get('Utc')
         return self
 
 
@@ -2550,14 +2572,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -2594,14 +2620,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -2614,49 +2644,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateDevicePurifyPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         start_time: int = None,
         end_time: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.start_time = start_time
         self.end_time = end_time
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         return self
@@ -2677,14 +2699,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -2721,14 +2747,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -2741,57 +2771,49 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateEventRecordPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         name: str = None,
         event_types: str = None,
         pre_record_duration: int = None,
         record_duration: int = None,
         template_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.name = name
         self.event_types = event_types
         self.pre_record_duration = pre_record_duration
         self.record_duration = record_duration
         self.template_id = template_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.name is not None:
             result['Name'] = self.name
         if self.event_types is not None:
             result['EventTypes'] = self.event_types
         if self.pre_record_duration is not None:
             result['PreRecordDuration'] = self.pre_record_duration
         if self.record_duration is not None:
             result['RecordDuration'] = self.record_duration
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('EventTypes') is not None:
             self.event_types = m.get('EventTypes')
         if m.get('PreRecordDuration') is not None:
             self.pre_record_duration = m.get('PreRecordDuration')
         if m.get('RecordDuration') is not None:
@@ -2816,14 +2838,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -2860,14 +2886,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -2880,43 +2910,39 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateModelRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         algorithm_id: int = None,
         name: str = None,
         model_package_standard: str = None,
         hardware: str = None,
         upload_model_path: str = None,
         need_encrypt: bool = None,
         description: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.algorithm_id = algorithm_id
         self.name = name
         self.model_package_standard = model_package_standard
         self.hardware = hardware
         self.upload_model_path = upload_model_path
         self.need_encrypt = need_encrypt
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.algorithm_id is not None:
             result['AlgorithmId'] = self.algorithm_id
         if self.name is not None:
             result['Name'] = self.name
         if self.model_package_standard is not None:
             result['ModelPackageStandard'] = self.model_package_standard
         if self.hardware is not None:
@@ -2927,18 +2953,14 @@
             result['NeedEncrypt'] = self.need_encrypt
         if self.description is not None:
             result['Description'] = self.description
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AlgorithmId') is not None:
             self.algorithm_id = m.get('AlgorithmId')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('ModelPackageStandard') is not None:
             self.model_package_standard = m.get('ModelPackageStandard')
         if m.get('Hardware') is not None:
@@ -2967,14 +2989,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -3011,14 +3037,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -3031,45 +3061,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreatePictureSearchAppRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         name: str = None,
         desc: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.name = name
         self.desc = desc
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.name is not None:
             result['Name'] = self.name
         if self.desc is not None:
             result['Desc'] = self.desc
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Desc') is not None:
             self.desc = m.get('Desc')
         return self
 
 
@@ -3088,14 +3110,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -3132,14 +3158,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -3149,48 +3179,191 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = CreatePictureSearchAppResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreatePictureSearchJobRequest(TeaModel):
+    def __init__(
+        self,
+        app_instance_id: str = None,
+        search_pic_url: str = None,
+        start_time: int = None,
+        end_time: int = None,
+        threshold: float = None,
+        body_threshold: float = None,
+        picture_search_type: int = None,
+    ):
+        self.app_instance_id = app_instance_id
+        self.search_pic_url = search_pic_url
+        self.start_time = start_time
+        self.end_time = end_time
+        self.threshold = threshold
+        self.body_threshold = body_threshold
+        self.picture_search_type = picture_search_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_instance_id is not None:
+            result['AppInstanceId'] = self.app_instance_id
+        if self.search_pic_url is not None:
+            result['SearchPicUrl'] = self.search_pic_url
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.threshold is not None:
+            result['Threshold'] = self.threshold
+        if self.body_threshold is not None:
+            result['BodyThreshold'] = self.body_threshold
+        if self.picture_search_type is not None:
+            result['PictureSearchType'] = self.picture_search_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AppInstanceId') is not None:
+            self.app_instance_id = m.get('AppInstanceId')
+        if m.get('SearchPicUrl') is not None:
+            self.search_pic_url = m.get('SearchPicUrl')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('Threshold') is not None:
+            self.threshold = m.get('Threshold')
+        if m.get('BodyThreshold') is not None:
+            self.body_threshold = m.get('BodyThreshold')
+        if m.get('PictureSearchType') is not None:
+            self.picture_search_type = m.get('PictureSearchType')
+        return self
+
+
+class CreatePictureSearchJobResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        data: str = None,
+        error_message: str = None,
+        code: str = None,
+        success: bool = None,
+    ):
+        self.request_id = request_id
+        self.data = data
+        self.error_message = error_message
+        self.code = code
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class CreatePictureSearchJobResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: CreatePictureSearchJobResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = CreatePictureSearchJobResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateRecordPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         name: str = None,
         template_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.name = name
         self.template_id = template_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.name is not None:
             result['Name'] = self.name
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         return self
 
 
@@ -3209,14 +3382,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -3253,14 +3430,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -3285,14 +3466,18 @@
         self.begin = begin
         self.end = end
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.day_of_week is not None:
             result['DayOfWeek'] = self.day_of_week
         if self.begin is not None:
             result['Begin'] = self.begin
         if self.end is not None:
             result['End'] = self.end
@@ -3308,54 +3493,46 @@
             self.end = m.get('End')
         return self
 
 
 class CreateTimeTemplateRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         name: str = None,
         all_day: int = None,
         time_sections: List[CreateTimeTemplateRequestTimeSections] = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.name = name
         self.all_day = all_day
         self.time_sections = time_sections
 
     def validate(self):
         if self.time_sections:
             for k in self.time_sections:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.name is not None:
             result['Name'] = self.name
         if self.all_day is not None:
             result['AllDay'] = self.all_day
         result['TimeSections'] = []
         if self.time_sections is not None:
             for k in self.time_sections:
                 result['TimeSections'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('AllDay') is not None:
             self.all_day = m.get('AllDay')
         self.time_sections = []
         if m.get('TimeSections') is not None:
             for k in m.get('TimeSections'):
@@ -3379,14 +3556,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -3423,14 +3604,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -3443,41 +3628,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteAlgorithmRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         algorithm_id: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.algorithm_id = algorithm_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.algorithm_id is not None:
             result['AlgorithmId'] = self.algorithm_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AlgorithmId') is not None:
             self.algorithm_id = m.get('AlgorithmId')
         return self
 
 
 class DeleteAlgorithmResponseBody(TeaModel):
     def __init__(
@@ -3492,14 +3669,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -3532,14 +3713,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -3552,41 +3737,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteEventRecordPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         return self
 
 
 class DeleteEventRecordPlanResponseBody(TeaModel):
     def __init__(
@@ -3601,14 +3778,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -3641,14 +3822,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -3661,45 +3846,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteEventRecordPlanDeviceRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         stream_type: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.stream_type = stream_type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.stream_type is not None:
             result['StreamType'] = self.stream_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('StreamType') is not None:
             self.stream_type = m.get('StreamType')
         return self
 
 
@@ -3716,14 +3893,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -3756,14 +3937,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -3776,45 +3961,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteFaceDeviceGroupRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         device_group_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.device_group_id = device_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.device_group_id is not None:
             result['DeviceGroupId'] = self.device_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('DeviceGroupId') is not None:
             self.device_group_id = m.get('DeviceGroupId')
         return self
 
 
@@ -3831,14 +4008,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -3871,14 +4052,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -3891,45 +4076,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteFaceUserRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         user_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         return self
 
 
@@ -3946,14 +4123,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -3986,14 +4167,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -4006,45 +4191,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteFaceUserGroupRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         user_group_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.user_group_id = user_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.user_group_id is not None:
             result['UserGroupId'] = self.user_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('UserGroupId') is not None:
             self.user_group_id = m.get('UserGroupId')
         return self
 
 
@@ -4061,14 +4238,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -4101,14 +4282,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -4121,45 +4306,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteFaceUserGroupAndDeviceGroupRelationRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         control_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.control_id = control_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.control_id is not None:
             result['ControlId'] = self.control_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('ControlId') is not None:
             self.control_id = m.get('ControlId')
         return self
 
 
@@ -4176,14 +4353,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -4216,14 +4397,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -4236,49 +4421,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteFaceUserPictureRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         user_id: str = None,
         face_pic_md_5: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.user_id = user_id
         self.face_pic_md_5 = face_pic_md_5
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
         if self.face_pic_md_5 is not None:
             result['FacePicMd5'] = self.face_pic_md_5
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('FacePicMd5') is not None:
             self.face_pic_md_5 = m.get('FacePicMd5')
         return self
@@ -4297,14 +4474,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -4337,14 +4518,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -4357,41 +4542,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteModelRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         model_id: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.model_id = model_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.model_id is not None:
             result['ModelId'] = self.model_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('ModelId') is not None:
             self.model_id = m.get('ModelId')
         return self
 
 
 class DeleteModelResponseBody(TeaModel):
     def __init__(
@@ -4406,14 +4583,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -4446,14 +4627,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -4466,41 +4651,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteRecordPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         return self
 
 
 class DeleteRecordPlanResponseBody(TeaModel):
     def __init__(
@@ -4515,14 +4692,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -4555,14 +4736,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -4575,45 +4760,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteRecordPlanDeviceRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         stream_type: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.stream_type = stream_type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.stream_type is not None:
             result['StreamType'] = self.stream_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('StreamType') is not None:
             self.stream_type = m.get('StreamType')
         return self
 
 
@@ -4630,14 +4807,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -4670,14 +4851,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -4690,41 +4875,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteTimeTemplateRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         template_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.template_id = template_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         return self
 
 
 class DeleteTimeTemplateResponseBody(TeaModel):
     def __init__(
@@ -4739,14 +4916,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -4779,14 +4960,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -4811,14 +4996,18 @@
         self.device_name = device_name
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.product_key is not None:
             result['ProductKey'] = self.product_key
         if self.device_name is not None:
             result['DeviceName'] = self.device_name
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
@@ -4834,50 +5023,42 @@
             self.iot_id = m.get('IotId')
         return self
 
 
 class DeployModelBatchRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         model_id: int = None,
         device_list: List[DeployModelBatchRequestDeviceList] = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.model_id = model_id
         self.device_list = device_list
 
     def validate(self):
         if self.device_list:
             for k in self.device_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.model_id is not None:
             result['ModelId'] = self.model_id
         result['DeviceList'] = []
         if self.device_list is not None:
             for k in self.device_list:
                 result['DeviceList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('ModelId') is not None:
             self.model_id = m.get('ModelId')
         self.device_list = []
         if m.get('DeviceList') is not None:
             for k in m.get('DeviceList'):
                 temp_model = DeployModelBatchRequestDeviceList()
                 self.device_list.append(temp_model.from_map(k))
@@ -4891,14 +5072,18 @@
     ):
         self.deploy_task_result_volist = deploy_task_result_volist
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.deploy_task_result_volist is not None:
             result['DeployTaskResultVOList'] = self.deploy_task_result_volist
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
@@ -4923,14 +5108,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -4968,14 +5157,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -4988,41 +5181,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DetectUserFaceByUrlRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         face_pic_url: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.face_pic_url = face_pic_url
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.face_pic_url is not None:
             result['FacePicUrl'] = self.face_pic_url
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('FacePicUrl') is not None:
             self.face_pic_url = m.get('FacePicUrl')
         return self
 
 
 class DetectUserFaceByUrlResponseBodyDataDataFaceRects(TeaModel):
     def __init__(
@@ -5031,14 +5216,18 @@
     ):
         self.face_rects_data = face_rects_data
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.face_rects_data is not None:
             result['FaceRectsData'] = self.face_rects_data
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
@@ -5054,14 +5243,18 @@
     ):
         self.landmarks_data = landmarks_data
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.landmarks_data is not None:
             result['LandmarksData'] = self.landmarks_data
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
@@ -5069,60 +5262,94 @@
             self.landmarks_data = m.get('LandmarksData')
         return self
 
 
 class DetectUserFaceByUrlResponseBodyDataData(TeaModel):
     def __init__(
         self,
+        blur_score: float = None,
         gender: int = None,
         face_rects: DetectUserFaceByUrlResponseBodyDataDataFaceRects = None,
+        occlusion_score: float = None,
+        good_for_library: bool = None,
+        good_for_recognition: bool = None,
         age: int = None,
         landmarks: DetectUserFaceByUrlResponseBodyDataDataLandmarks = None,
         face_probability: float = None,
+        pose_score: float = None,
     ):
+        self.blur_score = blur_score
         self.gender = gender
         self.face_rects = face_rects
+        self.occlusion_score = occlusion_score
+        self.good_for_library = good_for_library
+        self.good_for_recognition = good_for_recognition
         self.age = age
         self.landmarks = landmarks
         self.face_probability = face_probability
+        self.pose_score = pose_score
 
     def validate(self):
         if self.face_rects:
             self.face_rects.validate()
         if self.landmarks:
             self.landmarks.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
+        if self.blur_score is not None:
+            result['BlurScore'] = self.blur_score
         if self.gender is not None:
             result['Gender'] = self.gender
         if self.face_rects is not None:
             result['FaceRects'] = self.face_rects.to_map()
+        if self.occlusion_score is not None:
+            result['OcclusionScore'] = self.occlusion_score
+        if self.good_for_library is not None:
+            result['GoodForLibrary'] = self.good_for_library
+        if self.good_for_recognition is not None:
+            result['GoodForRecognition'] = self.good_for_recognition
         if self.age is not None:
             result['Age'] = self.age
         if self.landmarks is not None:
             result['Landmarks'] = self.landmarks.to_map()
         if self.face_probability is not None:
             result['FaceProbability'] = self.face_probability
+        if self.pose_score is not None:
+            result['PoseScore'] = self.pose_score
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('BlurScore') is not None:
+            self.blur_score = m.get('BlurScore')
         if m.get('Gender') is not None:
             self.gender = m.get('Gender')
         if m.get('FaceRects') is not None:
             temp_model = DetectUserFaceByUrlResponseBodyDataDataFaceRects()
             self.face_rects = temp_model.from_map(m['FaceRects'])
+        if m.get('OcclusionScore') is not None:
+            self.occlusion_score = m.get('OcclusionScore')
+        if m.get('GoodForLibrary') is not None:
+            self.good_for_library = m.get('GoodForLibrary')
+        if m.get('GoodForRecognition') is not None:
+            self.good_for_recognition = m.get('GoodForRecognition')
         if m.get('Age') is not None:
             self.age = m.get('Age')
         if m.get('Landmarks') is not None:
             temp_model = DetectUserFaceByUrlResponseBodyDataDataLandmarks()
             self.landmarks = temp_model.from_map(m['Landmarks'])
         if m.get('FaceProbability') is not None:
             self.face_probability = m.get('FaceProbability')
+        if m.get('PoseScore') is not None:
+            self.pose_score = m.get('PoseScore')
         return self
 
 
 class DetectUserFaceByUrlResponseBodyData(TeaModel):
     def __init__(
         self,
         data: List[DetectUserFaceByUrlResponseBodyDataData] = None,
@@ -5132,14 +5359,18 @@
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['data'] = []
         if self.data is not None:
             for k in self.data:
                 result['data'].append(k.to_map() if k else None)
         return result
 
@@ -5169,14 +5400,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -5214,14 +5449,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -5234,157 +5473,157 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetAIActionRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         action_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.action_id = action_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.action_id is not None:
             result['ActionId'] = self.action_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('ActionId') is not None:
             self.action_id = m.get('ActionId')
         return self
 
 
 class GetAIActionResponseBodyData(TeaModel):
     def __init__(
         self,
-        action_id: str = None,
-        plan_id: str = None,
+        algo_config: str = None,
         action: str = None,
+        action_id: str = None,
         action_template_id: str = None,
-        action_index: int = None,
         alog: str = None,
-        algo_config: str = None,
+        action_index: int = None,
         action_config: str = None,
+        plan_id: str = None,
     ):
-        self.action_id = action_id
-        self.plan_id = plan_id
+        self.algo_config = algo_config
         self.action = action
+        self.action_id = action_id
         self.action_template_id = action_template_id
-        self.action_index = action_index
         self.alog = alog
-        self.algo_config = algo_config
+        self.action_index = action_index
         self.action_config = action_config
+        self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.action_id is not None:
-            result['ActionId'] = self.action_id
-        if self.plan_id is not None:
-            result['PlanId'] = self.plan_id
+        if self.algo_config is not None:
+            result['AlgoConfig'] = self.algo_config
         if self.action is not None:
             result['Action'] = self.action
+        if self.action_id is not None:
+            result['ActionId'] = self.action_id
         if self.action_template_id is not None:
             result['ActionTemplateId'] = self.action_template_id
-        if self.action_index is not None:
-            result['ActionIndex'] = self.action_index
         if self.alog is not None:
             result['Alog'] = self.alog
-        if self.algo_config is not None:
-            result['AlgoConfig'] = self.algo_config
+        if self.action_index is not None:
+            result['ActionIndex'] = self.action_index
         if self.action_config is not None:
             result['ActionConfig'] = self.action_config
+        if self.plan_id is not None:
+            result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ActionId') is not None:
-            self.action_id = m.get('ActionId')
-        if m.get('PlanId') is not None:
-            self.plan_id = m.get('PlanId')
+        if m.get('AlgoConfig') is not None:
+            self.algo_config = m.get('AlgoConfig')
         if m.get('Action') is not None:
             self.action = m.get('Action')
+        if m.get('ActionId') is not None:
+            self.action_id = m.get('ActionId')
         if m.get('ActionTemplateId') is not None:
             self.action_template_id = m.get('ActionTemplateId')
-        if m.get('ActionIndex') is not None:
-            self.action_index = m.get('ActionIndex')
         if m.get('Alog') is not None:
             self.alog = m.get('Alog')
-        if m.get('AlgoConfig') is not None:
-            self.algo_config = m.get('AlgoConfig')
+        if m.get('ActionIndex') is not None:
+            self.action_index = m.get('ActionIndex')
         if m.get('ActionConfig') is not None:
             self.action_config = m.get('ActionConfig')
+        if m.get('PlanId') is not None:
+            self.plan_id = m.get('PlanId')
         return self
 
 
 class GetAIActionResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
+        data: GetAIActionResponseBodyData = None,
         error_message: str = None,
         code: str = None,
-        data: GetAIActionResponseBodyData = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
+        self.data = data
         self.error_message = error_message
         self.code = code
-        self.data = data
+        self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
+        if m.get('Data') is not None:
+            temp_model = GetAIActionResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = GetAIActionResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class GetAIActionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -5396,14 +5635,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -5416,244 +5659,252 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetAIActionConfigRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         algo: str = None,
         algo_action: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.algo = algo
         self.algo_action = algo_action
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.algo is not None:
             result['Algo'] = self.algo
         if self.algo_action is not None:
             result['AlgoAction'] = self.algo_action
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('Algo') is not None:
             self.algo = m.get('Algo')
         if m.get('AlgoAction') is not None:
             self.algo_action = m.get('AlgoAction')
         return self
 
 
 class GetAIActionConfigResponseBodyDataInParamList(TeaModel):
     def __init__(
         self,
-        data_type: str = None,
         need_config: bool = None,
+        data_type: str = None,
         config_items: List[str] = None,
     ):
-        self.data_type = data_type
         self.need_config = need_config
+        self.data_type = data_type
         self.config_items = config_items
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.data_type is not None:
-            result['DataType'] = self.data_type
         if self.need_config is not None:
             result['NeedConfig'] = self.need_config
+        if self.data_type is not None:
+            result['DataType'] = self.data_type
         if self.config_items is not None:
             result['ConfigItems'] = self.config_items
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('DataType') is not None:
-            self.data_type = m.get('DataType')
         if m.get('NeedConfig') is not None:
             self.need_config = m.get('NeedConfig')
+        if m.get('DataType') is not None:
+            self.data_type = m.get('DataType')
         if m.get('ConfigItems') is not None:
             self.config_items = m.get('ConfigItems')
         return self
 
 
 class GetAIActionConfigResponseBodyDataOutParamList(TeaModel):
     def __init__(
         self,
-        data_type: str = None,
         need_config: bool = None,
+        data_type: str = None,
         config_items: List[str] = None,
     ):
-        self.data_type = data_type
         self.need_config = need_config
+        self.data_type = data_type
         self.config_items = config_items
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.data_type is not None:
-            result['DataType'] = self.data_type
         if self.need_config is not None:
             result['NeedConfig'] = self.need_config
+        if self.data_type is not None:
+            result['DataType'] = self.data_type
         if self.config_items is not None:
             result['ConfigItems'] = self.config_items
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('DataType') is not None:
-            self.data_type = m.get('DataType')
         if m.get('NeedConfig') is not None:
             self.need_config = m.get('NeedConfig')
+        if m.get('DataType') is not None:
+            self.data_type = m.get('DataType')
         if m.get('ConfigItems') is not None:
             self.config_items = m.get('ConfigItems')
         return self
 
 
 class GetAIActionConfigResponseBodyData(TeaModel):
     def __init__(
         self,
+        in_param_list: List[GetAIActionConfigResponseBodyDataInParamList] = None,
         algo_action: str = None,
-        des: str = None,
-        need_device: bool = None,
         sync: str = None,
-        algo_config_items: str = None,
-        in_param_list: List[GetAIActionConfigResponseBodyDataInParamList] = None,
+        need_device: bool = None,
         out_param_list: List[GetAIActionConfigResponseBodyDataOutParamList] = None,
+        algo_config_items: str = None,
+        des: str = None,
     ):
+        self.in_param_list = in_param_list
         self.algo_action = algo_action
-        self.des = des
-        self.need_device = need_device
         self.sync = sync
-        self.algo_config_items = algo_config_items
-        self.in_param_list = in_param_list
+        self.need_device = need_device
         self.out_param_list = out_param_list
+        self.algo_config_items = algo_config_items
+        self.des = des
 
     def validate(self):
         if self.in_param_list:
             for k in self.in_param_list:
                 if k:
                     k.validate()
         if self.out_param_list:
             for k in self.out_param_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.algo_action is not None:
-            result['AlgoAction'] = self.algo_action
-        if self.des is not None:
-            result['Des'] = self.des
-        if self.need_device is not None:
-            result['NeedDevice'] = self.need_device
-        if self.sync is not None:
-            result['Sync'] = self.sync
-        if self.algo_config_items is not None:
-            result['AlgoConfigItems'] = self.algo_config_items
         result['InParamList'] = []
         if self.in_param_list is not None:
             for k in self.in_param_list:
                 result['InParamList'].append(k.to_map() if k else None)
+        if self.algo_action is not None:
+            result['AlgoAction'] = self.algo_action
+        if self.sync is not None:
+            result['Sync'] = self.sync
+        if self.need_device is not None:
+            result['NeedDevice'] = self.need_device
         result['OutParamList'] = []
         if self.out_param_list is not None:
             for k in self.out_param_list:
                 result['OutParamList'].append(k.to_map() if k else None)
+        if self.algo_config_items is not None:
+            result['AlgoConfigItems'] = self.algo_config_items
+        if self.des is not None:
+            result['Des'] = self.des
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('AlgoAction') is not None:
-            self.algo_action = m.get('AlgoAction')
-        if m.get('Des') is not None:
-            self.des = m.get('Des')
-        if m.get('NeedDevice') is not None:
-            self.need_device = m.get('NeedDevice')
-        if m.get('Sync') is not None:
-            self.sync = m.get('Sync')
-        if m.get('AlgoConfigItems') is not None:
-            self.algo_config_items = m.get('AlgoConfigItems')
         self.in_param_list = []
         if m.get('InParamList') is not None:
             for k in m.get('InParamList'):
                 temp_model = GetAIActionConfigResponseBodyDataInParamList()
                 self.in_param_list.append(temp_model.from_map(k))
+        if m.get('AlgoAction') is not None:
+            self.algo_action = m.get('AlgoAction')
+        if m.get('Sync') is not None:
+            self.sync = m.get('Sync')
+        if m.get('NeedDevice') is not None:
+            self.need_device = m.get('NeedDevice')
         self.out_param_list = []
         if m.get('OutParamList') is not None:
             for k in m.get('OutParamList'):
                 temp_model = GetAIActionConfigResponseBodyDataOutParamList()
                 self.out_param_list.append(temp_model.from_map(k))
+        if m.get('AlgoConfigItems') is not None:
+            self.algo_config_items = m.get('AlgoConfigItems')
+        if m.get('Des') is not None:
+            self.des = m.get('Des')
         return self
 
 
 class GetAIActionConfigResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
+        data: GetAIActionConfigResponseBodyData = None,
         error_message: str = None,
         code: str = None,
-        data: GetAIActionConfigResponseBodyData = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
+        self.data = data
         self.error_message = error_message
         self.code = code
-        self.data = data
+        self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
+        if m.get('Data') is not None:
+            temp_model = GetAIActionConfigResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = GetAIActionConfigResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class GetAIActionConfigResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -5665,14 +5916,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -5685,145 +5940,145 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetAIAppRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         app_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.app_id = app_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.app_id is not None:
             result['AppId'] = self.app_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AppId') is not None:
             self.app_id = m.get('AppId')
         return self
 
 
 class GetAIAppResponseBodyData(TeaModel):
     def __init__(
         self,
+        description: str = None,
+        version: str = None,
         app_id: str = None,
         app_template_id: str = None,
-        version: str = None,
-        level: int = None,
         name: str = None,
-        description: str = None,
+        level: int = None,
     ):
+        self.description = description
+        self.version = version
         self.app_id = app_id
         self.app_template_id = app_template_id
-        self.version = version
-        self.level = level
         self.name = name
-        self.description = description
+        self.level = level
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.version is not None:
+            result['Version'] = self.version
         if self.app_id is not None:
             result['AppId'] = self.app_id
         if self.app_template_id is not None:
             result['AppTemplateId'] = self.app_template_id
-        if self.version is not None:
-            result['Version'] = self.version
-        if self.level is not None:
-            result['Level'] = self.level
         if self.name is not None:
             result['Name'] = self.name
-        if self.description is not None:
-            result['Description'] = self.description
+        if self.level is not None:
+            result['Level'] = self.level
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Version') is not None:
+            self.version = m.get('Version')
         if m.get('AppId') is not None:
             self.app_id = m.get('AppId')
         if m.get('AppTemplateId') is not None:
             self.app_template_id = m.get('AppTemplateId')
-        if m.get('Version') is not None:
-            self.version = m.get('Version')
-        if m.get('Level') is not None:
-            self.level = m.get('Level')
         if m.get('Name') is not None:
             self.name = m.get('Name')
-        if m.get('Description') is not None:
-            self.description = m.get('Description')
+        if m.get('Level') is not None:
+            self.level = m.get('Level')
         return self
 
 
 class GetAIAppResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
+        data: GetAIAppResponseBodyData = None,
         error_message: str = None,
         code: str = None,
-        data: GetAIAppResponseBodyData = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
+        self.data = data
         self.error_message = error_message
         self.code = code
-        self.data = data
+        self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
+        if m.get('Data') is not None:
+            temp_model = GetAIAppResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = GetAIAppResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class GetAIAppResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -5835,14 +6090,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -5855,135 +6114,135 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetAIJobRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         job_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.job_id = job_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.job_id is not None:
             result['JobId'] = self.job_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('JobId') is not None:
             self.job_id = m.get('JobId')
         return self
 
 
 class GetAIJobResponseBodyDataDataDTOList(TeaModel):
     def __init__(
         self,
-        data_id: str = None,
-        data_type: str = None,
         data_source: str = None,
+        data_type: str = None,
         algo_data: str = None,
         job_id: str = None,
+        data_id: str = None,
         iot_id: str = None,
     ):
-        self.data_id = data_id
-        self.data_type = data_type
         self.data_source = data_source
+        self.data_type = data_type
         self.algo_data = algo_data
         self.job_id = job_id
+        self.data_id = data_id
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.data_id is not None:
-            result['DataId'] = self.data_id
-        if self.data_type is not None:
-            result['DataType'] = self.data_type
         if self.data_source is not None:
             result['DataSource'] = self.data_source
+        if self.data_type is not None:
+            result['DataType'] = self.data_type
         if self.algo_data is not None:
             result['AlgoData'] = self.algo_data
         if self.job_id is not None:
             result['JobId'] = self.job_id
+        if self.data_id is not None:
+            result['DataId'] = self.data_id
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('DataId') is not None:
-            self.data_id = m.get('DataId')
-        if m.get('DataType') is not None:
-            self.data_type = m.get('DataType')
         if m.get('DataSource') is not None:
             self.data_source = m.get('DataSource')
+        if m.get('DataType') is not None:
+            self.data_type = m.get('DataType')
         if m.get('AlgoData') is not None:
             self.algo_data = m.get('AlgoData')
         if m.get('JobId') is not None:
             self.job_id = m.get('JobId')
+        if m.get('DataId') is not None:
+            self.data_id = m.get('DataId')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         return self
 
 
 class GetAIJobResponseBodyDataActionJobDTO(TeaModel):
     def __init__(
         self,
+        status: int = None,
         job_id: str = None,
         action_id: str = None,
-        status: int = None,
         iot_id: str = None,
     ):
+        self.status = status
         self.job_id = job_id
         self.action_id = action_id
-        self.status = status
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
+        if self.status is not None:
+            result['Status'] = self.status
         if self.job_id is not None:
             result['JobId'] = self.job_id
         if self.action_id is not None:
             result['ActionId'] = self.action_id
-        if self.status is not None:
-            result['Status'] = self.status
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
         if m.get('JobId') is not None:
             self.job_id = m.get('JobId')
         if m.get('ActionId') is not None:
             self.action_id = m.get('ActionId')
-        if m.get('Status') is not None:
-            self.status = m.get('Status')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         return self
 
 
 class GetAIJobResponseBodyData(TeaModel):
     def __init__(
@@ -5999,14 +6258,18 @@
             for k in self.data_dtolist:
                 if k:
                     k.validate()
         if self.action_job_dto:
             self.action_job_dto.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['DataDTOList'] = []
         if self.data_dtolist is not None:
             for k in self.data_dtolist:
                 result['DataDTOList'].append(k.to_map() if k else None)
         if self.action_job_dto is not None:
             result['ActionJobDTO'] = self.action_job_dto.to_map()
@@ -6025,56 +6288,60 @@
         return self
 
 
 class GetAIJobResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
+        data: GetAIJobResponseBodyData = None,
         error_message: str = None,
         code: str = None,
-        data: GetAIJobResponseBodyData = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
+        self.data = data
         self.error_message = error_message
         self.code = code
-        self.data = data
+        self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
+        if m.get('Data') is not None:
+            temp_model = GetAIJobResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = GetAIJobResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class GetAIJobResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -6086,14 +6353,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -6106,151 +6377,151 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetAIPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         return self
 
 
 class GetAIPlanResponseBodyData(TeaModel):
     def __init__(
         self,
-        plan_id: str = None,
-        app_id: str = None,
         plan_template_id: str = None,
         trigger_enum: int = None,
-        interval_timing: int = None,
-        pre_timing: int = None,
         description: str = None,
+        pre_timing: int = None,
+        app_id: str = None,
+        interval_timing: int = None,
+        plan_id: str = None,
     ):
-        self.plan_id = plan_id
-        self.app_id = app_id
         self.plan_template_id = plan_template_id
         self.trigger_enum = trigger_enum
-        self.interval_timing = interval_timing
-        self.pre_timing = pre_timing
         self.description = description
+        self.pre_timing = pre_timing
+        self.app_id = app_id
+        self.interval_timing = interval_timing
+        self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.plan_id is not None:
-            result['PlanId'] = self.plan_id
-        if self.app_id is not None:
-            result['AppId'] = self.app_id
         if self.plan_template_id is not None:
             result['PlanTemplateId'] = self.plan_template_id
         if self.trigger_enum is not None:
             result['TriggerEnum'] = self.trigger_enum
-        if self.interval_timing is not None:
-            result['IntervalTiming'] = self.interval_timing
-        if self.pre_timing is not None:
-            result['PreTiming'] = self.pre_timing
         if self.description is not None:
             result['Description'] = self.description
+        if self.pre_timing is not None:
+            result['PreTiming'] = self.pre_timing
+        if self.app_id is not None:
+            result['AppId'] = self.app_id
+        if self.interval_timing is not None:
+            result['IntervalTiming'] = self.interval_timing
+        if self.plan_id is not None:
+            result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('PlanId') is not None:
-            self.plan_id = m.get('PlanId')
-        if m.get('AppId') is not None:
-            self.app_id = m.get('AppId')
         if m.get('PlanTemplateId') is not None:
             self.plan_template_id = m.get('PlanTemplateId')
         if m.get('TriggerEnum') is not None:
             self.trigger_enum = m.get('TriggerEnum')
-        if m.get('IntervalTiming') is not None:
-            self.interval_timing = m.get('IntervalTiming')
-        if m.get('PreTiming') is not None:
-            self.pre_timing = m.get('PreTiming')
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('PreTiming') is not None:
+            self.pre_timing = m.get('PreTiming')
+        if m.get('AppId') is not None:
+            self.app_id = m.get('AppId')
+        if m.get('IntervalTiming') is not None:
+            self.interval_timing = m.get('IntervalTiming')
+        if m.get('PlanId') is not None:
+            self.plan_id = m.get('PlanId')
         return self
 
 
 class GetAIPlanResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
+        data: GetAIPlanResponseBodyData = None,
         error_message: str = None,
         code: str = None,
-        data: GetAIPlanResponseBodyData = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
+        self.data = data
         self.error_message = error_message
         self.code = code
-        self.data = data
+        self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
+        if m.get('Data') is not None:
+            temp_model = GetAIPlanResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = GetAIPlanResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class GetAIPlanResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -6262,14 +6533,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -6282,41 +6557,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetAlgorithmDetailByIdRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         algorithm_id: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.algorithm_id = algorithm_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.algorithm_id is not None:
             result['AlgorithmId'] = self.algorithm_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AlgorithmId') is not None:
             self.algorithm_id = m.get('AlgorithmId')
         return self
 
 
 class GetAlgorithmDetailByIdResponseBody(TeaModel):
     def __init__(
@@ -6333,14 +6600,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -6377,14 +6648,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -6397,41 +6672,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetAlgorithmDetailByNameRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         name: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.name is not None:
             result['Name'] = self.name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         return self
 
 
 class GetAlgorithmDetailByNameResponseBody(TeaModel):
     def __init__(
@@ -6448,14 +6715,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -6492,14 +6763,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -6512,41 +6787,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetDevicePurifyJobByJobIdRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         job_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.job_id = job_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.job_id is not None:
             result['JobId'] = self.job_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('JobId') is not None:
             self.job_id = m.get('JobId')
         return self
 
 
 class GetDevicePurifyJobByJobIdResponseBodyData(TeaModel):
     def __init__(
@@ -6577,14 +6844,18 @@
         self.iot_id = iot_id
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.status is not None:
             result['Status'] = self.status
         if self.device_name is not None:
             result['DeviceName'] = self.device_name
         if self.user_id is not None:
             result['UserId'] = self.user_id
@@ -6653,14 +6924,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -6698,14 +6973,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -6718,45 +6997,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetModelDetailRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         algorithm_id: int = None,
         version: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.algorithm_id = algorithm_id
         self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.algorithm_id is not None:
             result['AlgorithmId'] = self.algorithm_id
         if self.version is not None:
             result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AlgorithmId') is not None:
             self.algorithm_id = m.get('AlgorithmId')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         return self
 
 
@@ -6775,14 +7046,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -6819,14 +7094,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -6839,41 +7118,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetModelDetailByIdRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         model_id: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.model_id = model_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.model_id is not None:
             result['ModelId'] = self.model_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('ModelId') is not None:
             self.model_id = m.get('ModelId')
         return self
 
 
 class GetModelDetailByIdResponseBody(TeaModel):
     def __init__(
@@ -6890,14 +7161,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -6934,14 +7209,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -6954,49 +7233,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetModelOssPolicyRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         algorithm_id: int = None,
         hardware: str = None,
         model_package_standard: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.algorithm_id = algorithm_id
         self.hardware = hardware
         self.model_package_standard = model_package_standard
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.algorithm_id is not None:
             result['AlgorithmId'] = self.algorithm_id
         if self.hardware is not None:
             result['Hardware'] = self.hardware
         if self.model_package_standard is not None:
             result['ModelPackageStandard'] = self.model_package_standard
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AlgorithmId') is not None:
             self.algorithm_id = m.get('AlgorithmId')
         if m.get('Hardware') is not None:
             self.hardware = m.get('Hardware')
         if m.get('ModelPackageStandard') is not None:
             self.model_package_standard = m.get('ModelPackageStandard')
         return self
@@ -7017,14 +7288,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -7061,14 +7336,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -7081,41 +7360,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetPictureInfoWithVectorIdsRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         vector_id_list: List[str] = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.vector_id_list = vector_id_list
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.vector_id_list is not None:
             result['VectorIdList'] = self.vector_id_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('VectorIdList') is not None:
             self.vector_id_list = m.get('VectorIdList')
         return self
 
 
 class GetPictureInfoWithVectorIdsResponseBodyData(TeaModel):
     def __init__(
@@ -7128,14 +7399,18 @@
         self.gateway_iot_id = gateway_iot_id
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.pic_url is not None:
             result['PicUrl'] = self.pic_url
         if self.gateway_iot_id is not None:
             result['GatewayIotId'] = self.gateway_iot_id
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
@@ -7170,14 +7445,18 @@
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         result['Data'] = []
         if self.data is not None:
             for k in self.data:
                 result['Data'].append(k.to_map() if k else None)
@@ -7219,14 +7498,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -7236,44 +7519,222 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = GetPictureInfoWithVectorIdsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetPictureSearchJobStatusRequest(TeaModel):
+    def __init__(
+        self,
+        app_instance_id: str = None,
+        job_id: str = None,
+    ):
+        self.app_instance_id = app_instance_id
+        self.job_id = job_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_instance_id is not None:
+            result['AppInstanceId'] = self.app_instance_id
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AppInstanceId') is not None:
+            self.app_instance_id = m.get('AppInstanceId')
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        return self
+
+
+class GetPictureSearchJobStatusResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        end_time: int = None,
+        start_time: int = None,
+        job_status: int = None,
+        search_pic_url: str = None,
+        create_time: int = None,
+        job_id: str = None,
+        threshold: float = None,
+    ):
+        self.end_time = end_time
+        self.start_time = start_time
+        self.job_status = job_status
+        self.search_pic_url = search_pic_url
+        self.create_time = create_time
+        self.job_id = job_id
+        self.threshold = threshold
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.job_status is not None:
+            result['JobStatus'] = self.job_status
+        if self.search_pic_url is not None:
+            result['SearchPicUrl'] = self.search_pic_url
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.threshold is not None:
+            result['Threshold'] = self.threshold
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('JobStatus') is not None:
+            self.job_status = m.get('JobStatus')
+        if m.get('SearchPicUrl') is not None:
+            self.search_pic_url = m.get('SearchPicUrl')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('Threshold') is not None:
+            self.threshold = m.get('Threshold')
+        return self
+
+
+class GetPictureSearchJobStatusResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        data: GetPictureSearchJobStatusResponseBodyData = None,
+        error_message: str = None,
+        code: str = None,
+        success: bool = None,
+    ):
+        self.request_id = request_id
+        self.data = data
+        self.error_message = error_message
+        self.code = code
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Data') is not None:
+            temp_model = GetPictureSearchJobStatusResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetPictureSearchJobStatusResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetPictureSearchJobStatusResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetPictureSearchJobStatusResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetPictureWithVectorIdRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         vector_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.vector_id = vector_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.vector_id is not None:
             result['VectorId'] = self.vector_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('VectorId') is not None:
             self.vector_id = m.get('VectorId')
         return self
 
 
 class GetPictureWithVectorIdResponseBody(TeaModel):
     def __init__(
@@ -7290,14 +7751,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -7334,14 +7799,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -7354,49 +7823,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListAlgorithmsByPageRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         name_pattern: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.name_pattern = name_pattern
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.name_pattern is not None:
             result['NamePattern'] = self.name_pattern
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('NamePattern') is not None:
             self.name_pattern = m.get('NamePattern')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         return self
@@ -7417,14 +7878,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -7461,14 +7926,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -7493,14 +7962,18 @@
         self.device_name = device_name
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.product_key is not None:
             result['ProductKey'] = self.product_key
         if self.device_name is not None:
             result['DeviceName'] = self.device_name
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
@@ -7516,50 +7989,42 @@
             self.iot_id = m.get('IotId')
         return self
 
 
 class ListDeployTaskByModelIdAndDevicesRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         model_id: int = None,
         device_list: List[ListDeployTaskByModelIdAndDevicesRequestDeviceList] = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.model_id = model_id
         self.device_list = device_list
 
     def validate(self):
         if self.device_list:
             for k in self.device_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.model_id is not None:
             result['ModelId'] = self.model_id
         result['DeviceList'] = []
         if self.device_list is not None:
             for k in self.device_list:
                 result['DeviceList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('ModelId') is not None:
             self.model_id = m.get('ModelId')
         self.device_list = []
         if m.get('DeviceList') is not None:
             for k in m.get('DeviceList'):
                 temp_model = ListDeployTaskByModelIdAndDevicesRequestDeviceList()
                 self.device_list.append(temp_model.from_map(k))
@@ -7581,14 +8046,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -7625,14 +8094,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -7645,45 +8118,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListDeployTaskByPageRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         return self
 
 
@@ -7702,14 +8167,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -7746,14 +8215,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -7766,43 +8239,39 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListModelsByPageRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         algorithm_id: int = None,
         size_type: str = None,
         model_package_standard: str = None,
         hardware: str = None,
         name_pattern: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.algorithm_id = algorithm_id
         self.size_type = size_type
         self.model_package_standard = model_package_standard
         self.hardware = hardware
         self.name_pattern = name_pattern
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.algorithm_id is not None:
             result['AlgorithmId'] = self.algorithm_id
         if self.size_type is not None:
             result['SizeType'] = self.size_type
         if self.model_package_standard is not None:
             result['ModelPackageStandard'] = self.model_package_standard
         if self.hardware is not None:
@@ -7813,18 +8282,14 @@
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AlgorithmId') is not None:
             self.algorithm_id = m.get('AlgorithmId')
         if m.get('SizeType') is not None:
             self.size_type = m.get('SizeType')
         if m.get('ModelPackageStandard') is not None:
             self.model_package_standard = m.get('ModelPackageStandard')
         if m.get('Hardware') is not None:
@@ -7853,14 +8318,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -7897,14 +8366,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -7917,41 +8390,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListModelVersionsByPageRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         algorithm_name: str = None,
         size_type: str = None,
         model_package_standard: str = None,
         hardware: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.algorithm_name = algorithm_name
         self.size_type = size_type
         self.model_package_standard = model_package_standard
         self.hardware = hardware
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.algorithm_name is not None:
             result['AlgorithmName'] = self.algorithm_name
         if self.size_type is not None:
             result['SizeType'] = self.size_type
         if self.model_package_standard is not None:
             result['ModelPackageStandard'] = self.model_package_standard
         if self.hardware is not None:
@@ -7960,18 +8429,14 @@
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AlgorithmName') is not None:
             self.algorithm_name = m.get('AlgorithmName')
         if m.get('SizeType') is not None:
             self.size_type = m.get('SizeType')
         if m.get('ModelPackageStandard') is not None:
             self.model_package_standard = m.get('ModelPackageStandard')
         if m.get('Hardware') is not None:
@@ -7998,14 +8463,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -8042,14 +8511,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -8062,45 +8535,43 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PictureSearchPictureRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         app_instance_id: str = None,
         page_size: int = None,
         current_page: int = None,
         search_pic_url: str = None,
         start_time: int = None,
         end_time: int = None,
         threshold: float = None,
         contain_pic_url: bool = None,
+        picture_search_type: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.app_instance_id = app_instance_id
         self.page_size = page_size
         self.current_page = current_page
         self.search_pic_url = search_pic_url
         self.start_time = start_time
         self.end_time = end_time
         self.threshold = threshold
         self.contain_pic_url = contain_pic_url
+        self.picture_search_type = picture_search_type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.app_instance_id is not None:
             result['AppInstanceId'] = self.app_instance_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         if self.search_pic_url is not None:
@@ -8109,22 +8580,20 @@
             result['StartTime'] = self.start_time
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.threshold is not None:
             result['Threshold'] = self.threshold
         if self.contain_pic_url is not None:
             result['ContainPicUrl'] = self.contain_pic_url
+        if self.picture_search_type is not None:
+            result['PictureSearchType'] = self.picture_search_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AppInstanceId') is not None:
             self.app_instance_id = m.get('AppInstanceId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('SearchPicUrl') is not None:
@@ -8133,49 +8602,59 @@
             self.start_time = m.get('StartTime')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('Threshold') is not None:
             self.threshold = m.get('Threshold')
         if m.get('ContainPicUrl') is not None:
             self.contain_pic_url = m.get('ContainPicUrl')
+        if m.get('PictureSearchType') is not None:
+            self.picture_search_type = m.get('PictureSearchType')
         return self
 
 
 class PictureSearchPictureResponseBodyDataPageData(TeaModel):
     def __init__(
         self,
         pic_url: str = None,
         event_time: int = None,
         gateway_iot_id: str = None,
         vector_id: str = None,
         threshold: float = None,
+        vector_type: int = None,
         iot_id: str = None,
     ):
         self.pic_url = pic_url
         self.event_time = event_time
         self.gateway_iot_id = gateway_iot_id
         self.vector_id = vector_id
         self.threshold = threshold
+        self.vector_type = vector_type
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.pic_url is not None:
             result['PicUrl'] = self.pic_url
         if self.event_time is not None:
             result['EventTime'] = self.event_time
         if self.gateway_iot_id is not None:
             result['GatewayIotId'] = self.gateway_iot_id
         if self.vector_id is not None:
             result['VectorId'] = self.vector_id
         if self.threshold is not None:
             result['Threshold'] = self.threshold
+        if self.vector_type is not None:
+            result['VectorType'] = self.vector_type
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('PicUrl') is not None:
@@ -8184,14 +8663,16 @@
             self.event_time = m.get('EventTime')
         if m.get('GatewayIotId') is not None:
             self.gateway_iot_id = m.get('GatewayIotId')
         if m.get('VectorId') is not None:
             self.vector_id = m.get('VectorId')
         if m.get('Threshold') is not None:
             self.threshold = m.get('Threshold')
+        if m.get('VectorType') is not None:
+            self.vector_type = m.get('VectorType')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         return self
 
 
 class PictureSearchPictureResponseBodyData(TeaModel):
     def __init__(
@@ -8211,14 +8692,18 @@
     def validate(self):
         if self.page_data:
             for k in self.page_data:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         result['PageData'] = []
         if self.page_data is not None:
             for k in self.page_data:
                 result['PageData'].append(k.to_map() if k else None)
@@ -8264,14 +8749,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -8309,14 +8798,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -8329,163 +8822,163 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryAIActionRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         return self
 
 
 class QueryAIActionResponseBodyData(TeaModel):
     def __init__(
         self,
+        algo_config: str = None,
+        action: str = None,
+        algo: str = None,
         action_id: str = None,
-        plan_id: str = None,
         action_template_id: str = None,
         action_index: int = None,
-        algo: str = None,
-        action: str = None,
-        algo_config: str = None,
         action_config: str = None,
+        plan_id: str = None,
     ):
+        self.algo_config = algo_config
+        self.action = action
+        self.algo = algo
         self.action_id = action_id
-        self.plan_id = plan_id
         self.action_template_id = action_template_id
         self.action_index = action_index
-        self.algo = algo
-        self.action = action
-        self.algo_config = algo_config
         self.action_config = action_config
+        self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
+        if self.algo_config is not None:
+            result['AlgoConfig'] = self.algo_config
+        if self.action is not None:
+            result['Action'] = self.action
+        if self.algo is not None:
+            result['Algo'] = self.algo
         if self.action_id is not None:
             result['ActionId'] = self.action_id
-        if self.plan_id is not None:
-            result['PlanId'] = self.plan_id
         if self.action_template_id is not None:
             result['ActionTemplateId'] = self.action_template_id
         if self.action_index is not None:
             result['ActionIndex'] = self.action_index
-        if self.algo is not None:
-            result['Algo'] = self.algo
-        if self.action is not None:
-            result['Action'] = self.action
-        if self.algo_config is not None:
-            result['AlgoConfig'] = self.algo_config
         if self.action_config is not None:
             result['ActionConfig'] = self.action_config
+        if self.plan_id is not None:
+            result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AlgoConfig') is not None:
+            self.algo_config = m.get('AlgoConfig')
+        if m.get('Action') is not None:
+            self.action = m.get('Action')
+        if m.get('Algo') is not None:
+            self.algo = m.get('Algo')
         if m.get('ActionId') is not None:
             self.action_id = m.get('ActionId')
-        if m.get('PlanId') is not None:
-            self.plan_id = m.get('PlanId')
         if m.get('ActionTemplateId') is not None:
             self.action_template_id = m.get('ActionTemplateId')
         if m.get('ActionIndex') is not None:
             self.action_index = m.get('ActionIndex')
-        if m.get('Algo') is not None:
-            self.algo = m.get('Algo')
-        if m.get('Action') is not None:
-            self.action = m.get('Action')
-        if m.get('AlgoConfig') is not None:
-            self.algo_config = m.get('AlgoConfig')
         if m.get('ActionConfig') is not None:
             self.action_config = m.get('ActionConfig')
+        if m.get('PlanId') is not None:
+            self.plan_id = m.get('PlanId')
         return self
 
 
 class QueryAIActionResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
+        data: List[QueryAIActionResponseBodyData] = None,
         error_message: str = None,
         code: str = None,
-        data: List[QueryAIActionResponseBodyData] = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
+        self.data = data
         self.error_message = error_message
         self.code = code
-        self.data = data
+        self.success = success
 
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        if self.error_message is not None:
-            result['ErrorMessage'] = self.error_message
-        if self.code is not None:
-            result['Code'] = self.code
         result['Data'] = []
         if self.data is not None:
             for k in self.data:
                 result['Data'].append(k.to_map() if k else None)
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        if m.get('ErrorMessage') is not None:
-            self.error_message = m.get('ErrorMessage')
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
         self.data = []
         if m.get('Data') is not None:
             for k in m.get('Data'):
                 temp_model = QueryAIActionResponseBodyData()
                 self.data.append(temp_model.from_map(k))
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class QueryAIActionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -8497,14 +8990,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -8517,206 +9014,210 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryAIAppRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         return self
 
 
 class QueryAIAppResponseBodyDataList(TeaModel):
     def __init__(
         self,
+        description: str = None,
+        version: str = None,
         app_id: str = None,
         app_template_id: str = None,
-        version: str = None,
-        level: int = None,
         name: str = None,
-        description: str = None,
+        level: int = None,
     ):
+        self.description = description
+        self.version = version
         self.app_id = app_id
         self.app_template_id = app_template_id
-        self.version = version
-        self.level = level
         self.name = name
-        self.description = description
+        self.level = level
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.version is not None:
+            result['Version'] = self.version
         if self.app_id is not None:
             result['AppId'] = self.app_id
         if self.app_template_id is not None:
             result['AppTemplateId'] = self.app_template_id
-        if self.version is not None:
-            result['Version'] = self.version
-        if self.level is not None:
-            result['Level'] = self.level
         if self.name is not None:
             result['Name'] = self.name
-        if self.description is not None:
-            result['Description'] = self.description
+        if self.level is not None:
+            result['Level'] = self.level
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Version') is not None:
+            self.version = m.get('Version')
         if m.get('AppId') is not None:
             self.app_id = m.get('AppId')
         if m.get('AppTemplateId') is not None:
             self.app_template_id = m.get('AppTemplateId')
-        if m.get('Version') is not None:
-            self.version = m.get('Version')
-        if m.get('Level') is not None:
-            self.level = m.get('Level')
         if m.get('Name') is not None:
             self.name = m.get('Name')
-        if m.get('Description') is not None:
-            self.description = m.get('Description')
+        if m.get('Level') is not None:
+            self.level = m.get('Level')
         return self
 
 
 class QueryAIAppResponseBodyData(TeaModel):
     def __init__(
         self,
-        total: int = None,
-        page_count: int = None,
         current_page: int = None,
-        page_size: int = None,
         list: List[QueryAIAppResponseBodyDataList] = None,
+        page_size: int = None,
+        total: int = None,
+        page_count: int = None,
     ):
-        self.total = total
-        self.page_count = page_count
         self.current_page = current_page
-        self.page_size = page_size
         self.list = list
+        self.page_size = page_size
+        self.total = total
+        self.page_count = page_count
 
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.total is not None:
-            result['Total'] = self.total
-        if self.page_count is not None:
-            result['PageCount'] = self.page_count
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        if self.page_count is not None:
+            result['PageCount'] = self.page_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Total') is not None:
-            self.total = m.get('Total')
-        if m.get('PageCount') is not None:
-            self.page_count = m.get('PageCount')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
         self.list = []
         if m.get('List') is not None:
             for k in m.get('List'):
                 temp_model = QueryAIAppResponseBodyDataList()
                 self.list.append(temp_model.from_map(k))
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        if m.get('PageCount') is not None:
+            self.page_count = m.get('PageCount')
         return self
 
 
 class QueryAIAppResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
+        data: QueryAIAppResponseBodyData = None,
         error_message: str = None,
         code: str = None,
-        data: QueryAIAppResponseBodyData = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
+        self.data = data
         self.error_message = error_message
         self.code = code
-        self.data = data
+        self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
+        if m.get('Data') is not None:
+            temp_model = QueryAIAppResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = QueryAIAppResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class QueryAIAppResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -8728,14 +9229,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -8748,206 +9253,210 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryAIJobsRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         action_id: str = None,
         iot_id: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.action_id = action_id
         self.iot_id = iot_id
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.action_id is not None:
             result['ActionId'] = self.action_id
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('ActionId') is not None:
             self.action_id = m.get('ActionId')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         return self
 
 
 class QueryAIJobsResponseBodyDataList(TeaModel):
     def __init__(
         self,
+        status: int = None,
         job_id: str = None,
         action_id: str = None,
-        status: int = None,
         iot_id: str = None,
     ):
+        self.status = status
         self.job_id = job_id
         self.action_id = action_id
-        self.status = status
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
+        if self.status is not None:
+            result['Status'] = self.status
         if self.job_id is not None:
             result['JobId'] = self.job_id
         if self.action_id is not None:
             result['ActionId'] = self.action_id
-        if self.status is not None:
-            result['Status'] = self.status
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
         if m.get('JobId') is not None:
             self.job_id = m.get('JobId')
         if m.get('ActionId') is not None:
             self.action_id = m.get('ActionId')
-        if m.get('Status') is not None:
-            self.status = m.get('Status')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         return self
 
 
 class QueryAIJobsResponseBodyData(TeaModel):
     def __init__(
         self,
-        total: int = None,
-        page_count: int = None,
         current_page: int = None,
-        page_size: int = None,
         list: List[QueryAIJobsResponseBodyDataList] = None,
+        page_size: int = None,
+        total: int = None,
+        page_count: int = None,
     ):
-        self.total = total
-        self.page_count = page_count
         self.current_page = current_page
-        self.page_size = page_size
         self.list = list
+        self.page_size = page_size
+        self.total = total
+        self.page_count = page_count
 
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.total is not None:
-            result['Total'] = self.total
-        if self.page_count is not None:
-            result['PageCount'] = self.page_count
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        if self.page_count is not None:
+            result['PageCount'] = self.page_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Total') is not None:
-            self.total = m.get('Total')
-        if m.get('PageCount') is not None:
-            self.page_count = m.get('PageCount')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
         self.list = []
         if m.get('List') is not None:
             for k in m.get('List'):
                 temp_model = QueryAIJobsResponseBodyDataList()
                 self.list.append(temp_model.from_map(k))
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        if m.get('PageCount') is not None:
+            self.page_count = m.get('PageCount')
         return self
 
 
 class QueryAIJobsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
+        data: QueryAIJobsResponseBodyData = None,
         error_message: str = None,
         code: str = None,
-        data: QueryAIJobsResponseBodyData = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
+        self.data = data
         self.error_message = error_message
         self.code = code
-        self.data = data
+        self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
+        if m.get('Data') is not None:
+            temp_model = QueryAIJobsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = QueryAIJobsResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class QueryAIJobsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -8959,14 +9468,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -8979,218 +9492,222 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryAIPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         app_id: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.app_id = app_id
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.app_id is not None:
             result['AppId'] = self.app_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AppId') is not None:
             self.app_id = m.get('AppId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         return self
 
 
 class QueryAIPlanResponseBodyDataList(TeaModel):
     def __init__(
         self,
-        plan_id: str = None,
-        app_id: str = None,
         plan_template_id: str = None,
         trigger_enum: int = None,
-        interval_timing: int = None,
-        pre_timing: int = None,
         description: str = None,
+        pre_timing: int = None,
+        app_id: str = None,
+        interval_timing: int = None,
+        plan_id: str = None,
     ):
-        self.plan_id = plan_id
-        self.app_id = app_id
         self.plan_template_id = plan_template_id
         self.trigger_enum = trigger_enum
-        self.interval_timing = interval_timing
-        self.pre_timing = pre_timing
         self.description = description
+        self.pre_timing = pre_timing
+        self.app_id = app_id
+        self.interval_timing = interval_timing
+        self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.plan_id is not None:
-            result['PlanId'] = self.plan_id
-        if self.app_id is not None:
-            result['AppId'] = self.app_id
         if self.plan_template_id is not None:
             result['PlanTemplateId'] = self.plan_template_id
         if self.trigger_enum is not None:
             result['TriggerEnum'] = self.trigger_enum
-        if self.interval_timing is not None:
-            result['IntervalTiming'] = self.interval_timing
-        if self.pre_timing is not None:
-            result['PreTiming'] = self.pre_timing
         if self.description is not None:
             result['Description'] = self.description
+        if self.pre_timing is not None:
+            result['PreTiming'] = self.pre_timing
+        if self.app_id is not None:
+            result['AppId'] = self.app_id
+        if self.interval_timing is not None:
+            result['IntervalTiming'] = self.interval_timing
+        if self.plan_id is not None:
+            result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('PlanId') is not None:
-            self.plan_id = m.get('PlanId')
-        if m.get('AppId') is not None:
-            self.app_id = m.get('AppId')
         if m.get('PlanTemplateId') is not None:
             self.plan_template_id = m.get('PlanTemplateId')
         if m.get('TriggerEnum') is not None:
             self.trigger_enum = m.get('TriggerEnum')
-        if m.get('IntervalTiming') is not None:
-            self.interval_timing = m.get('IntervalTiming')
-        if m.get('PreTiming') is not None:
-            self.pre_timing = m.get('PreTiming')
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('PreTiming') is not None:
+            self.pre_timing = m.get('PreTiming')
+        if m.get('AppId') is not None:
+            self.app_id = m.get('AppId')
+        if m.get('IntervalTiming') is not None:
+            self.interval_timing = m.get('IntervalTiming')
+        if m.get('PlanId') is not None:
+            self.plan_id = m.get('PlanId')
         return self
 
 
 class QueryAIPlanResponseBodyData(TeaModel):
     def __init__(
         self,
-        total: int = None,
-        page_count: int = None,
         current_page: int = None,
-        page_size: int = None,
         list: List[QueryAIPlanResponseBodyDataList] = None,
+        page_size: int = None,
+        total: int = None,
+        page_count: int = None,
     ):
-        self.total = total
-        self.page_count = page_count
         self.current_page = current_page
-        self.page_size = page_size
         self.list = list
+        self.page_size = page_size
+        self.total = total
+        self.page_count = page_count
 
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.total is not None:
-            result['Total'] = self.total
-        if self.page_count is not None:
-            result['PageCount'] = self.page_count
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        if self.page_count is not None:
+            result['PageCount'] = self.page_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Total') is not None:
-            self.total = m.get('Total')
-        if m.get('PageCount') is not None:
-            self.page_count = m.get('PageCount')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
         self.list = []
         if m.get('List') is not None:
             for k in m.get('List'):
                 temp_model = QueryAIPlanResponseBodyDataList()
                 self.list.append(temp_model.from_map(k))
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        if m.get('PageCount') is not None:
+            self.page_count = m.get('PageCount')
         return self
 
 
 class QueryAIPlanResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
+        data: QueryAIPlanResponseBodyData = None,
         error_message: str = None,
         code: str = None,
-        data: QueryAIPlanResponseBodyData = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
+        self.data = data
         self.error_message = error_message
         self.code = code
-        self.data = data
+        self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
+        if m.get('Data') is not None:
+            temp_model = QueryAIPlanResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = QueryAIPlanResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class QueryAIPlanResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -9202,14 +9719,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -9222,157 +9743,157 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryAIPlanTemplatesRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         app_template_id: str = None,
         app_version: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.app_template_id = app_template_id
         self.app_version = app_version
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.app_template_id is not None:
             result['AppTemplateId'] = self.app_template_id
         if self.app_version is not None:
             result['AppVersion'] = self.app_version
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AppTemplateId') is not None:
             self.app_template_id = m.get('AppTemplateId')
         if m.get('AppVersion') is not None:
             self.app_version = m.get('AppVersion')
         return self
 
 
 class QueryAIPlanTemplatesResponseBodyData(TeaModel):
     def __init__(
         self,
         plan_template_id: str = None,
-        app_template_id: str = None,
-        app_version: str = None,
         trigger_enum: int = None,
         description: str = None,
         interval_timing: int = None,
+        app_version: str = None,
+        app_template_id: str = None,
     ):
         self.plan_template_id = plan_template_id
-        self.app_template_id = app_template_id
-        self.app_version = app_version
         self.trigger_enum = trigger_enum
         self.description = description
         self.interval_timing = interval_timing
+        self.app_version = app_version
+        self.app_template_id = app_template_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.plan_template_id is not None:
             result['PlanTemplateId'] = self.plan_template_id
-        if self.app_template_id is not None:
-            result['AppTemplateId'] = self.app_template_id
-        if self.app_version is not None:
-            result['AppVersion'] = self.app_version
         if self.trigger_enum is not None:
             result['TriggerEnum'] = self.trigger_enum
         if self.description is not None:
             result['Description'] = self.description
         if self.interval_timing is not None:
             result['IntervalTiming'] = self.interval_timing
+        if self.app_version is not None:
+            result['AppVersion'] = self.app_version
+        if self.app_template_id is not None:
+            result['AppTemplateId'] = self.app_template_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('PlanTemplateId') is not None:
             self.plan_template_id = m.get('PlanTemplateId')
-        if m.get('AppTemplateId') is not None:
-            self.app_template_id = m.get('AppTemplateId')
-        if m.get('AppVersion') is not None:
-            self.app_version = m.get('AppVersion')
         if m.get('TriggerEnum') is not None:
             self.trigger_enum = m.get('TriggerEnum')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('IntervalTiming') is not None:
             self.interval_timing = m.get('IntervalTiming')
+        if m.get('AppVersion') is not None:
+            self.app_version = m.get('AppVersion')
+        if m.get('AppTemplateId') is not None:
+            self.app_template_id = m.get('AppTemplateId')
         return self
 
 
 class QueryAIPlanTemplatesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
+        data: List[QueryAIPlanTemplatesResponseBodyData] = None,
         error_message: str = None,
         code: str = None,
-        data: List[QueryAIPlanTemplatesResponseBodyData] = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
+        self.data = data
         self.error_message = error_message
         self.code = code
-        self.data = data
+        self.success = success
 
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        if self.error_message is not None:
-            result['ErrorMessage'] = self.error_message
-        if self.code is not None:
-            result['Code'] = self.code
         result['Data'] = []
         if self.data is not None:
             for k in self.data:
                 result['Data'].append(k.to_map() if k else None)
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        if m.get('ErrorMessage') is not None:
-            self.error_message = m.get('ErrorMessage')
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
         self.data = []
         if m.get('Data') is not None:
             for k in m.get('Data'):
                 temp_model = QueryAIPlanTemplatesResponseBodyData()
                 self.data.append(temp_model.from_map(k))
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class QueryAIPlanTemplatesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -9384,14 +9905,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -9404,43 +9929,39 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryDeviceEventRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         event_type: int = None,
         begin_time: int = None,
         end_time: int = None,
         current_page: int = None,
         page_size: int = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.event_type = event_type
         self.begin_time = begin_time
         self.end_time = end_time
         self.current_page = current_page
         self.page_size = page_size
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.event_type is not None:
             result['EventType'] = self.event_type
         if self.begin_time is not None:
             result['BeginTime'] = self.begin_time
         if self.end_time is not None:
@@ -9451,18 +9972,14 @@
             result['PageSize'] = self.page_size
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('EventType') is not None:
             self.event_type = m.get('EventType')
         if m.get('BeginTime') is not None:
             self.begin_time = m.get('BeginTime')
         if m.get('EndTime') is not None:
@@ -9493,14 +10010,18 @@
         self.event_desc = event_desc
         self.event_data = event_data
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.event_id is not None:
             result['EventId'] = self.event_id
         if self.event_time is not None:
             result['EventTime'] = self.event_time
         if self.event_type is not None:
             result['EventType'] = self.event_type
@@ -9547,14 +10068,18 @@
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
         if self.page_size is not None:
             result['PageSize'] = self.page_size
@@ -9600,14 +10125,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -9645,14 +10174,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -9665,49 +10198,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryDeviceEventPictureRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         event_id: str = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.event_id = event_id
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.event_id is not None:
             result['EventId'] = self.event_id
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('EventId') is not None:
             self.event_id = m.get('EventId')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         return self
@@ -9728,14 +10253,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -9772,14 +10301,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -9792,49 +10325,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryDeviceEventRecordRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         event_id: str = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.event_id = event_id
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.event_id is not None:
             result['EventId'] = self.event_id
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('EventId') is not None:
             self.event_id = m.get('EventId')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         return self
@@ -9853,14 +10378,18 @@
         self.file_name = file_name
         self.vod_url = vod_url
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.begin_time is not None:
             result['BeginTime'] = self.begin_time
         if self.file_name is not None:
             result['FileName'] = self.file_name
@@ -9899,14 +10428,18 @@
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         result['Data'] = []
         if self.data is not None:
             for k in self.data:
                 result['Data'].append(k.to_map() if k else None)
@@ -9948,14 +10481,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -9968,53 +10505,45 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryDeviceFileVodRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         file_name: str = None,
         should_encrypt: bool = None,
         encrypt_type: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.file_name = file_name
         self.should_encrypt = should_encrypt
         self.encrypt_type = encrypt_type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.file_name is not None:
             result['FileName'] = self.file_name
         if self.should_encrypt is not None:
             result['ShouldEncrypt'] = self.should_encrypt
         if self.encrypt_type is not None:
             result['EncryptType'] = self.encrypt_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('FileName') is not None:
             self.file_name = m.get('FileName')
         if m.get('ShouldEncrypt') is not None:
             self.should_encrypt = m.get('ShouldEncrypt')
         if m.get('EncryptType') is not None:
@@ -10029,14 +10558,18 @@
     ):
         self.vod_url = vod_url
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.vod_url is not None:
             result['VodUrl'] = self.vod_url
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
@@ -10063,14 +10596,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.decrypt_key is not None:
             result['DecryptKey'] = self.decrypt_key
         if self.data is not None:
             result['Data'] = self.data.to_map()
@@ -10112,14 +10649,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -10132,53 +10673,45 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryDevicePictureFileRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         capture_id: str = None,
         picture_type: int = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.capture_id = capture_id
         self.picture_type = picture_type
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.capture_id is not None:
             result['CaptureId'] = self.capture_id
         if self.picture_type is not None:
             result['PictureType'] = self.picture_type
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('CaptureId') is not None:
             self.capture_id = m.get('CaptureId')
         if m.get('PictureType') is not None:
             self.picture_type = m.get('PictureType')
         if m.get('IotInstanceId') is not None:
@@ -10201,14 +10734,18 @@
         self.thumb_url = thumb_url
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.pic_url is not None:
             result['PicUrl'] = self.pic_url
         if self.pic_create_time is not None:
             result['PicCreateTime'] = self.pic_create_time
         if self.pic_id is not None:
             result['PicId'] = self.pic_id
@@ -10249,14 +10786,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -10294,14 +10835,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -10314,41 +10859,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryDevicePictureLifeCycleRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         return self
 
 
 class QueryDevicePictureLifeCycleResponseBodyData(TeaModel):
     def __init__(
@@ -10359,14 +10896,18 @@
         self.day = day
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.day is not None:
             result['Day'] = self.day
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         return result
 
@@ -10395,14 +10936,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -10440,14 +10985,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -10460,49 +11009,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryDevicePurifyJobsRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         return self
@@ -10537,14 +11078,18 @@
         self.iot_id = iot_id
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.status is not None:
             result['Status'] = self.status
         if self.device_name is not None:
             result['DeviceName'] = self.device_name
         if self.user_id is not None:
             result['UserId'] = self.user_id
@@ -10615,14 +11160,18 @@
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
@@ -10668,14 +11217,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -10713,14 +11266,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -10733,41 +11290,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryDevicePurifyPlanByPlanIdRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         return self
 
 
 class QueryDevicePurifyPlanByPlanIdResponseBodyData(TeaModel):
     def __init__(
@@ -10790,14 +11339,18 @@
         self.tenant_id = tenant_id
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         if self.product_key is not None:
             result['ProductKey'] = self.product_key
@@ -10850,14 +11403,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -10895,14 +11452,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -10915,49 +11476,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryDevicePurifyPlansRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         return self
@@ -10984,14 +11537,18 @@
         self.tenant_id = tenant_id
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         if self.product_key is not None:
             result['ProductKey'] = self.product_key
@@ -11046,14 +11603,18 @@
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
@@ -11099,14 +11660,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -11144,14 +11709,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -11164,41 +11733,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryDeviceRecordLifeCycleRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         device_list: List[str] = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.device_list = device_list
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.device_list is not None:
             result['DeviceList'] = self.device_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('DeviceList') is not None:
             self.device_list = m.get('DeviceList')
         return self
 
 
 class QueryDeviceRecordLifeCycleResponseBodyData(TeaModel):
     def __init__(
@@ -11209,14 +11770,18 @@
         self.day = day
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.day is not None:
             result['Day'] = self.day
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         return result
 
@@ -11247,14 +11812,18 @@
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         result['Data'] = []
         if self.data is not None:
             for k in self.data:
                 result['Data'].append(k.to_map() if k else None)
@@ -11296,14 +11865,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -11316,93 +11889,95 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryDeviceVodUrlRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
-        iot_id: str = None,
         file_name: str = None,
-        should_encrypt: bool = None,
-        encrypt_type: int = None,
         scheme: str = None,
         seek_time: int = None,
         iot_instance_id: str = None,
+        iot_id: str = None,
+        play_un_limited: bool = None,
+        encrypt_type: int = None,
+        should_encrypt: bool = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
-        self.iot_id = iot_id
         self.file_name = file_name
-        self.should_encrypt = should_encrypt
-        self.encrypt_type = encrypt_type
         self.scheme = scheme
         self.seek_time = seek_time
         self.iot_instance_id = iot_instance_id
+        self.iot_id = iot_id
+        self.play_un_limited = play_un_limited
+        self.encrypt_type = encrypt_type
+        self.should_encrypt = should_encrypt
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
-        if self.iot_id is not None:
-            result['IotId'] = self.iot_id
         if self.file_name is not None:
             result['FileName'] = self.file_name
-        if self.should_encrypt is not None:
-            result['ShouldEncrypt'] = self.should_encrypt
-        if self.encrypt_type is not None:
-            result['EncryptType'] = self.encrypt_type
         if self.scheme is not None:
             result['Scheme'] = self.scheme
         if self.seek_time is not None:
             result['SeekTime'] = self.seek_time
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
+        if self.iot_id is not None:
+            result['IotId'] = self.iot_id
+        if self.play_un_limited is not None:
+            result['PlayUnLimited'] = self.play_un_limited
+        if self.encrypt_type is not None:
+            result['EncryptType'] = self.encrypt_type
+        if self.should_encrypt is not None:
+            result['ShouldEncrypt'] = self.should_encrypt
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
-        if m.get('IotId') is not None:
-            self.iot_id = m.get('IotId')
         if m.get('FileName') is not None:
             self.file_name = m.get('FileName')
-        if m.get('ShouldEncrypt') is not None:
-            self.should_encrypt = m.get('ShouldEncrypt')
-        if m.get('EncryptType') is not None:
-            self.encrypt_type = m.get('EncryptType')
         if m.get('Scheme') is not None:
             self.scheme = m.get('Scheme')
         if m.get('SeekTime') is not None:
             self.seek_time = m.get('SeekTime')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
+        if m.get('IotId') is not None:
+            self.iot_id = m.get('IotId')
+        if m.get('PlayUnLimited') is not None:
+            self.play_un_limited = m.get('PlayUnLimited')
+        if m.get('EncryptType') is not None:
+            self.encrypt_type = m.get('EncryptType')
+        if m.get('ShouldEncrypt') is not None:
+            self.should_encrypt = m.get('ShouldEncrypt')
         return self
 
 
 class QueryDeviceVodUrlResponseBodyData(TeaModel):
     def __init__(
         self,
         vod_url: str = None,
     ):
         self.vod_url = vod_url
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.vod_url is not None:
             result['VodUrl'] = self.vod_url
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
@@ -11429,14 +12004,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.decrypt_key is not None:
             result['DecryptKey'] = self.decrypt_key
         if self.data is not None:
             result['Data'] = self.data.to_map()
@@ -11478,14 +12057,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -11495,44 +12078,234 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = QueryDeviceVodUrlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryDeviceVodUrlByTimeRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: int = None,
+        scheme: str = None,
+        seek_time: int = None,
+        iot_instance_id: str = None,
+        begin_time: int = None,
+        iot_id: str = None,
+        play_un_limited: bool = None,
+        encrypt_type: int = None,
+        should_encrypt: bool = None,
+    ):
+        self.end_time = end_time
+        self.scheme = scheme
+        self.seek_time = seek_time
+        self.iot_instance_id = iot_instance_id
+        self.begin_time = begin_time
+        self.iot_id = iot_id
+        self.play_un_limited = play_un_limited
+        self.encrypt_type = encrypt_type
+        self.should_encrypt = should_encrypt
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.scheme is not None:
+            result['Scheme'] = self.scheme
+        if self.seek_time is not None:
+            result['SeekTime'] = self.seek_time
+        if self.iot_instance_id is not None:
+            result['IotInstanceId'] = self.iot_instance_id
+        if self.begin_time is not None:
+            result['BeginTime'] = self.begin_time
+        if self.iot_id is not None:
+            result['IotId'] = self.iot_id
+        if self.play_un_limited is not None:
+            result['PlayUnLimited'] = self.play_un_limited
+        if self.encrypt_type is not None:
+            result['EncryptType'] = self.encrypt_type
+        if self.should_encrypt is not None:
+            result['ShouldEncrypt'] = self.should_encrypt
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('Scheme') is not None:
+            self.scheme = m.get('Scheme')
+        if m.get('SeekTime') is not None:
+            self.seek_time = m.get('SeekTime')
+        if m.get('IotInstanceId') is not None:
+            self.iot_instance_id = m.get('IotInstanceId')
+        if m.get('BeginTime') is not None:
+            self.begin_time = m.get('BeginTime')
+        if m.get('IotId') is not None:
+            self.iot_id = m.get('IotId')
+        if m.get('PlayUnLimited') is not None:
+            self.play_un_limited = m.get('PlayUnLimited')
+        if m.get('EncryptType') is not None:
+            self.encrypt_type = m.get('EncryptType')
+        if m.get('ShouldEncrypt') is not None:
+            self.should_encrypt = m.get('ShouldEncrypt')
+        return self
+
+
+class QueryDeviceVodUrlByTimeResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        vod_url: str = None,
+    ):
+        self.vod_url = vod_url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.vod_url is not None:
+            result['VodUrl'] = self.vod_url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('VodUrl') is not None:
+            self.vod_url = m.get('VodUrl')
+        return self
+
+
+class QueryDeviceVodUrlByTimeResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        decrypt_key: str = None,
+        data: QueryDeviceVodUrlByTimeResponseBodyData = None,
+        error_message: str = None,
+        code: str = None,
+        success: bool = None,
+    ):
+        self.request_id = request_id
+        self.decrypt_key = decrypt_key
+        self.data = data
+        self.error_message = error_message
+        self.code = code
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.decrypt_key is not None:
+            result['DecryptKey'] = self.decrypt_key
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('DecryptKey') is not None:
+            self.decrypt_key = m.get('DecryptKey')
+        if m.get('Data') is not None:
+            temp_model = QueryDeviceVodUrlByTimeResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class QueryDeviceVodUrlByTimeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: QueryDeviceVodUrlByTimeResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = QueryDeviceVodUrlByTimeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryEventRecordPlanDetailRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         return self
 
 
 class QueryEventRecordPlanDetailResponseBodyDataTemplateInfoTimeSectionList(TeaModel):
     def __init__(
@@ -11545,14 +12318,18 @@
         self.begin = begin
         self.end = end
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.day_of_week is not None:
             result['DayOfWeek'] = self.day_of_week
         if self.begin is not None:
             result['Begin'] = self.begin
         if self.end is not None:
             result['End'] = self.end
@@ -11587,14 +12364,18 @@
     def validate(self):
         if self.time_section_list:
             for k in self.time_section_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['TimeSectionList'] = []
         if self.time_section_list is not None:
             for k in self.time_section_list:
                 result['TimeSectionList'].append(k.to_map() if k else None)
         if self.all_day is not None:
             result['AllDay'] = self.all_day
@@ -11642,14 +12423,18 @@
         self.template_id = template_id
 
     def validate(self):
         if self.template_info:
             self.template_info.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.record_duration is not None:
             result['RecordDuration'] = self.record_duration
         if self.pre_record_duration is not None:
             result['PreRecordDuration'] = self.pre_record_duration
         if self.name is not None:
             result['Name'] = self.name
@@ -11695,14 +12480,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -11740,14 +12529,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -11760,45 +12553,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryEventRecordPlanDeviceByDeviceRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         stream_type: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.stream_type = stream_type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.stream_type is not None:
             result['StreamType'] = self.stream_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('StreamType') is not None:
             self.stream_type = m.get('StreamType')
         return self
 
 
@@ -11813,14 +12598,18 @@
         self.begin = begin
         self.end = end
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.day_of_week is not None:
             result['DayOfWeek'] = self.day_of_week
         if self.begin is not None:
             result['Begin'] = self.begin
         if self.end is not None:
             result['End'] = self.end
@@ -11855,14 +12644,18 @@
     def validate(self):
         if self.time_section_list:
             for k in self.time_section_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['TimeSectionList'] = []
         if self.time_section_list is not None:
             for k in self.time_section_list:
                 result['TimeSectionList'].append(k.to_map() if k else None)
         if self.all_day is not None:
             result['AllDay'] = self.all_day
@@ -11910,14 +12703,18 @@
         self.template_id = template_id
 
     def validate(self):
         if self.template_info:
             self.template_info.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.record_duration is not None:
             result['RecordDuration'] = self.record_duration
         if self.pre_record_duration is not None:
             result['PreRecordDuration'] = self.pre_record_duration
         if self.name is not None:
             result['Name'] = self.name
@@ -11963,14 +12760,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -12008,14 +12809,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -12028,49 +12833,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryEventRecordPlanDeviceByPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
         current_page: int = None,
         page_size: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
         self.current_page = current_page
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         return self
@@ -12085,14 +12882,18 @@
         self.stream_type = stream_type
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.stream_type is not None:
             result['StreamType'] = self.stream_type
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         return result
 
@@ -12123,14 +12924,18 @@
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
         if self.page_size is not None:
             result['PageSize'] = self.page_size
@@ -12176,14 +12981,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -12221,14 +13030,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -12241,45 +13054,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryEventRecordPlansRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         current_page: int = None,
         page_size: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.current_page = current_page
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         return self
 
 
@@ -12300,14 +13105,18 @@
         self.name = name
         self.template_id = template_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.event_type is not None:
             result['EventType'] = self.event_type
         if self.record_duration is not None:
             result['RecordDuration'] = self.record_duration
         if self.pre_record_duration is not None:
             result['PreRecordDuration'] = self.pre_record_duration
@@ -12354,14 +13163,18 @@
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
         if self.page_size is not None:
             result['PageSize'] = self.page_size
@@ -12407,14 +13220,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -12452,14 +13269,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -12472,53 +13293,45 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryFaceAllDeviceGroupRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         iot_instance_id: str = None,
         page_size: int = None,
         page_no: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.iot_instance_id = iot_instance_id
         self.page_size = page_size
         self.page_no = page_no
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.page_no is not None:
             result['PageNo'] = self.page_no
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('PageNo') is not None:
@@ -12537,14 +13350,18 @@
         self.modified_time = modified_time
         self.device_group_name = device_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.device_group_id is not None:
             result['DeviceGroupId'] = self.device_group_id
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.device_group_name is not None:
             result['DeviceGroupName'] = self.device_group_name
@@ -12577,14 +13394,18 @@
     def validate(self):
         if self.device_group_list:
             for k in self.device_group_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['DeviceGroupList'] = []
         if self.device_group_list is not None:
             for k in self.device_group_list:
                 result['DeviceGroupList'].append(k.to_map() if k else None)
         if self.page_no is not None:
             result['PageNo'] = self.page_no
@@ -12626,14 +13447,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -12671,14 +13496,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -12691,49 +13520,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryFaceAllUserGroupRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         page_size: int = None,
         page_no: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.page_size = page_size
         self.page_no = page_no
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.page_no is not None:
             result['PageNo'] = self.page_no
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('PageNo') is not None:
             self.page_no = m.get('PageNo')
         return self
@@ -12750,14 +13571,18 @@
         self.user_group_id = user_group_id
         self.user_group_name = user_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.user_group_id is not None:
             result['UserGroupId'] = self.user_group_id
         if self.user_group_name is not None:
             result['UserGroupName'] = self.user_group_name
@@ -12790,14 +13615,18 @@
     def validate(self):
         if self.user_group_list:
             for k in self.user_group_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.page_no is not None:
             result['PageNo'] = self.page_no
         result['UserGroupList'] = []
         if self.user_group_list is not None:
             for k in self.user_group_list:
                 result['UserGroupList'].append(k.to_map() if k else None)
@@ -12839,14 +13668,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -12884,14 +13717,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -12904,49 +13741,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryFaceAllUserGroupAndDeviceGroupRelationRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         page_size: int = None,
         page_no: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.page_size = page_size
         self.page_no = page_no
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.page_no is not None:
             result['PageNo'] = self.page_no
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('PageNo') is not None:
             self.page_no = m.get('PageNo')
         return self
@@ -12967,14 +13796,18 @@
         self.user_group_id = user_group_id
         self.control_id = control_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.device_group_id is not None:
             result['DeviceGroupId'] = self.device_group_id
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.control_type is not None:
             result['ControlType'] = self.control_type
@@ -13015,14 +13848,18 @@
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
         if self.page_size is not None:
             result['PageSize'] = self.page_size
@@ -13064,14 +13901,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -13109,14 +13950,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -13129,53 +13974,45 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryFaceAllUserIdsByGroupIdRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         user_group_id: str = None,
         page_size: int = None,
         page_no: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.user_group_id = user_group_id
         self.page_size = page_size
         self.page_no = page_no
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.user_group_id is not None:
             result['UserGroupId'] = self.user_group_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.page_no is not None:
             result['PageNo'] = self.page_no
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('UserGroupId') is not None:
             self.user_group_id = m.get('UserGroupId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('PageNo') is not None:
@@ -13196,14 +14033,18 @@
         self.user_id = user_id
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.params is not None:
             result['Params'] = self.params
         if self.custom_user_id is not None:
             result['CustomUserId'] = self.custom_user_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
@@ -13240,14 +14081,18 @@
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
         if self.page_size is not None:
             result['PageSize'] = self.page_size
@@ -13289,14 +14134,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -13334,14 +14183,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -13354,45 +14207,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryFaceCustomUserIdByUserIdRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         user_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         return self
 
 
@@ -13411,14 +14256,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -13455,14 +14304,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -13475,41 +14328,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryFaceDeviceGroupsByDeviceRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         iot_instance_id: str = None,
         product_key: str = None,
         device_name: str = None,
         page_size: int = None,
         page_no: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.iot_instance_id = iot_instance_id
         self.product_key = product_key
         self.device_name = device_name
         self.page_size = page_size
         self.page_no = page_no
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         if self.product_key is not None:
             result['ProductKey'] = self.product_key
         if self.device_name is not None:
@@ -13518,18 +14367,14 @@
             result['PageSize'] = self.page_size
         if self.page_no is not None:
             result['PageNo'] = self.page_no
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         if m.get('ProductKey') is not None:
             self.product_key = m.get('ProductKey')
         if m.get('DeviceName') is not None:
@@ -13552,14 +14397,18 @@
         self.modified_time = modified_time
         self.device_group_name = device_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.device_group_id is not None:
             result['DeviceGroupId'] = self.device_group_id
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.device_group_name is not None:
             result['DeviceGroupName'] = self.device_group_name
@@ -13592,14 +14441,18 @@
     def validate(self):
         if self.device_group_list:
             for k in self.device_group_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['DeviceGroupList'] = []
         if self.device_group_list is not None:
             for k in self.device_group_list:
                 result['DeviceGroupList'].append(k.to_map() if k else None)
         if self.page_no is not None:
             result['PageNo'] = self.page_no
@@ -13641,14 +14494,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -13686,14 +14543,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -13706,45 +14567,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryFaceUserRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         user_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         return self
 
 
@@ -13765,14 +14618,18 @@
         self.error_code = error_code
         self.face_md_5 = face_md_5
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.algorithm_name is not None:
             result['AlgorithmName'] = self.algorithm_name
         if self.algorithm_version is not None:
             result['AlgorithmVersion'] = self.algorithm_version
         if self.algorithm_provider is not None:
             result['AlgorithmProvider'] = self.algorithm_provider
@@ -13815,14 +14672,18 @@
     def validate(self):
         if self.feature_dtolist:
             for k in self.feature_dtolist:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.face_url is not None:
             result['FaceUrl'] = self.face_url
         result['FeatureDTOList'] = []
         if self.feature_dtolist is not None:
             for k in self.feature_dtolist:
                 result['FeatureDTOList'].append(k.to_map() if k else None)
@@ -13862,14 +14723,18 @@
     def validate(self):
         if self.face_pic_list:
             for k in self.face_pic_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.params is not None:
             result['Params'] = self.params
         if self.custom_user_id is not None:
             result['CustomUserId'] = self.custom_user_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
@@ -13915,14 +14780,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -13960,14 +14829,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -13980,53 +14853,45 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryFaceUserGroupRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         user_id: str = None,
         page_size: int = None,
         page_no: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.user_id = user_id
         self.page_size = page_size
         self.page_no = page_no
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.page_no is not None:
             result['PageNo'] = self.page_no
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('PageNo') is not None:
@@ -14045,14 +14910,18 @@
         self.user_group_id = user_group_id
         self.user_group_name = user_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.user_group_id is not None:
             result['UserGroupId'] = self.user_group_id
         if self.user_group_name is not None:
             result['UserGroupName'] = self.user_group_name
@@ -14085,14 +14954,18 @@
     def validate(self):
         if self.user_group_list:
             for k in self.user_group_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.page_no is not None:
             result['PageNo'] = self.page_no
         result['UserGroupList'] = []
         if self.user_group_list is not None:
             for k in self.user_group_list:
                 result['UserGroupList'].append(k.to_map() if k else None)
@@ -14134,14 +15007,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -14179,14 +15056,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -14199,45 +15080,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryFaceUserGroupAndDeviceGroupRelationRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         control_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.control_id = control_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.control_id is not None:
             result['ControlId'] = self.control_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('ControlId') is not None:
             self.control_id = m.get('ControlId')
         return self
 
 
@@ -14256,14 +15129,18 @@
         self.user_group_id = user_group_id
         self.control_id = control_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.device_group_id is not None:
             result['DeviceGroupId'] = self.device_group_id
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.control_type is not None:
             result['ControlType'] = self.control_type
@@ -14304,14 +15181,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -14349,14 +15230,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -14369,45 +15254,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryFaceUserIdByCustomUserIdRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         custom_user_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.custom_user_id = custom_user_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.custom_user_id is not None:
             result['CustomUserId'] = self.custom_user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('CustomUserId') is not None:
             self.custom_user_id = m.get('CustomUserId')
         return self
 
 
@@ -14424,14 +15301,18 @@
         self.user_id = user_id
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.params is not None:
             result['Params'] = self.params
         if self.custom_user_id is not None:
             result['CustomUserId'] = self.custom_user_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
@@ -14468,14 +15349,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -14513,14 +15398,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -14533,151 +15422,151 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryIotIdsByAIPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         return self
 
 
 class QueryIotIdsByAIPlanResponseBodyData(TeaModel):
     def __init__(
         self,
-        total: int = None,
-        page_count: int = None,
         current_page: int = None,
-        page_size: int = None,
         list: List[str] = None,
+        page_size: int = None,
+        total: int = None,
+        page_count: int = None,
     ):
-        self.total = total
-        self.page_count = page_count
         self.current_page = current_page
-        self.page_size = page_size
         self.list = list
+        self.page_size = page_size
+        self.total = total
+        self.page_count = page_count
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.total is not None:
-            result['Total'] = self.total
-        if self.page_count is not None:
-            result['PageCount'] = self.page_count
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
         if self.list is not None:
             result['List'] = self.list
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        if self.page_count is not None:
+            result['PageCount'] = self.page_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Total') is not None:
-            self.total = m.get('Total')
-        if m.get('PageCount') is not None:
-            self.page_count = m.get('PageCount')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
         if m.get('List') is not None:
             self.list = m.get('List')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        if m.get('PageCount') is not None:
+            self.page_count = m.get('PageCount')
         return self
 
 
 class QueryIotIdsByAIPlanResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
+        data: QueryIotIdsByAIPlanResponseBodyData = None,
         error_message: str = None,
         code: str = None,
-        data: QueryIotIdsByAIPlanResponseBodyData = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
+        self.data = data
         self.error_message = error_message
         self.code = code
-        self.data = data
+        self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
+        if m.get('Data') is not None:
+            temp_model = QueryIotIdsByAIPlanResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = QueryIotIdsByAIPlanResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class QueryIotIdsByAIPlanResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -14689,14 +15578,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -14709,73 +15602,83 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryLiveStreamingRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
-        iot_id: str = None,
+        scheme: str = None,
+        iot_instance_id: str = None,
         stream_type: int = None,
+        cache_duration: int = None,
+        iot_id: str = None,
         should_encrypt: bool = None,
+        play_un_limited: bool = None,
         encrypt_type: int = None,
-        scheme: str = None,
-        iot_instance_id: str = None,
+        force_iframe: bool = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
-        self.iot_id = iot_id
+        self.scheme = scheme
+        self.iot_instance_id = iot_instance_id
         self.stream_type = stream_type
+        self.cache_duration = cache_duration
+        self.iot_id = iot_id
         self.should_encrypt = should_encrypt
+        self.play_un_limited = play_un_limited
         self.encrypt_type = encrypt_type
-        self.scheme = scheme
-        self.iot_instance_id = iot_instance_id
+        self.force_iframe = force_iframe
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
-        if self.iot_id is not None:
-            result['IotId'] = self.iot_id
+        if self.scheme is not None:
+            result['Scheme'] = self.scheme
+        if self.iot_instance_id is not None:
+            result['IotInstanceId'] = self.iot_instance_id
         if self.stream_type is not None:
             result['StreamType'] = self.stream_type
+        if self.cache_duration is not None:
+            result['CacheDuration'] = self.cache_duration
+        if self.iot_id is not None:
+            result['IotId'] = self.iot_id
         if self.should_encrypt is not None:
             result['ShouldEncrypt'] = self.should_encrypt
+        if self.play_un_limited is not None:
+            result['PlayUnLimited'] = self.play_un_limited
         if self.encrypt_type is not None:
             result['EncryptType'] = self.encrypt_type
-        if self.scheme is not None:
-            result['Scheme'] = self.scheme
-        if self.iot_instance_id is not None:
-            result['IotInstanceId'] = self.iot_instance_id
+        if self.force_iframe is not None:
+            result['ForceIFrame'] = self.force_iframe
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
-        if m.get('IotId') is not None:
-            self.iot_id = m.get('IotId')
+        if m.get('Scheme') is not None:
+            self.scheme = m.get('Scheme')
+        if m.get('IotInstanceId') is not None:
+            self.iot_instance_id = m.get('IotInstanceId')
         if m.get('StreamType') is not None:
             self.stream_type = m.get('StreamType')
+        if m.get('CacheDuration') is not None:
+            self.cache_duration = m.get('CacheDuration')
+        if m.get('IotId') is not None:
+            self.iot_id = m.get('IotId')
         if m.get('ShouldEncrypt') is not None:
             self.should_encrypt = m.get('ShouldEncrypt')
+        if m.get('PlayUnLimited') is not None:
+            self.play_un_limited = m.get('PlayUnLimited')
         if m.get('EncryptType') is not None:
             self.encrypt_type = m.get('EncryptType')
-        if m.get('Scheme') is not None:
-            self.scheme = m.get('Scheme')
-        if m.get('IotInstanceId') is not None:
-            self.iot_instance_id = m.get('IotInstanceId')
+        if m.get('ForceIFrame') is not None:
+            self.force_iframe = m.get('ForceIFrame')
         return self
 
 
 class QueryLiveStreamingResponseBodyData(TeaModel):
     def __init__(
         self,
         path: str = None,
@@ -14784,14 +15687,18 @@
         self.path = path
         self.decrypt_key = decrypt_key
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.path is not None:
             result['Path'] = self.path
         if self.decrypt_key is not None:
             result['DecryptKey'] = self.decrypt_key
         return result
 
@@ -14820,14 +15727,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -14865,14 +15776,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -14885,49 +15800,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryMonthRecordRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         month: str = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.month = month
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.month is not None:
             result['Month'] = self.month
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('Month') is not None:
             self.month = m.get('Month')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         return self
@@ -14948,14 +15855,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -14992,14 +15903,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -15012,45 +15927,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryPictureFilesRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         begin_time: int = None,
         end_time: int = None,
         current_page: int = None,
         page_size: int = None,
         picture_type: int = None,
         picture_source: int = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.begin_time = begin_time
         self.end_time = end_time
         self.current_page = current_page
         self.page_size = page_size
         self.picture_type = picture_type
         self.picture_source = picture_source
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.begin_time is not None:
             result['BeginTime'] = self.begin_time
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.current_page is not None:
@@ -15063,18 +15974,14 @@
             result['PictureSource'] = self.picture_source
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('BeginTime') is not None:
             self.begin_time = m.get('BeginTime')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('CurrentPage') is not None:
@@ -15105,14 +16012,18 @@
         self.thumb_url = thumb_url
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.pic_url is not None:
             result['PicUrl'] = self.pic_url
         if self.pic_create_time is not None:
             result['PicCreateTime'] = self.pic_create_time
         if self.pic_id is not None:
             result['PicId'] = self.pic_id
@@ -15151,14 +16062,18 @@
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
         if self.page_size is not None:
             result['PageSize'] = self.page_size
@@ -15196,14 +16111,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -15241,14 +16160,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -15261,55 +16184,53 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryPictureSearchAiboxesRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         app_instance_id: str = None,
         page_size: int = None,
         current_page: int = None,
+        iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.app_instance_id = app_instance_id
         self.page_size = page_size
         self.current_page = current_page
+        self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.app_instance_id is not None:
             result['AppInstanceId'] = self.app_instance_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
+        if self.iot_instance_id is not None:
+            result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AppInstanceId') is not None:
             self.app_instance_id = m.get('AppInstanceId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
+        if m.get('IotInstanceId') is not None:
+            self.iot_instance_id = m.get('IotInstanceId')
         return self
 
 
 class QueryPictureSearchAiboxesResponseBodyDataPageData(TeaModel):
     def __init__(
         self,
         nick_name: str = None,
@@ -15318,14 +16239,18 @@
         self.nick_name = nick_name
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.nick_name is not None:
             result['NickName'] = self.nick_name
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         return result
 
@@ -15356,14 +16281,18 @@
     def validate(self):
         if self.page_data:
             for k in self.page_data:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         result['PageData'] = []
         if self.page_data is not None:
             for k in self.page_data:
                 result['PageData'].append(k.to_map() if k else None)
@@ -15409,14 +16338,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -15454,14 +16387,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -15471,43 +16408,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = QueryPictureSearchAiboxesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QueryPictureSearchAppRequest(TeaModel):
-    def __init__(
-        self,
-        api_product: str = None,
-        api_revision: str = None,
-    ):
-        self.api_product = api_product
-        self.api_revision = api_revision
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
-        return self
-
-
 class QueryPictureSearchAppResponseBodyDataData(TeaModel):
     def __init__(
         self,
         app_instance_id: str = None,
         modified_time: int = None,
         version: str = None,
         create_time: int = None,
@@ -15523,14 +16431,18 @@
         self.name = name
         self.level = level
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.app_instance_id is not None:
             result['AppInstanceId'] = self.app_instance_id
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.version is not None:
             result['Version'] = self.version
@@ -15573,14 +16485,18 @@
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['data'] = []
         if self.data is not None:
             for k in self.data:
                 result['data'].append(k.to_map() if k else None)
         return result
 
@@ -15610,14 +16526,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -15655,14 +16575,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -15672,52 +16596,289 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = QueryPictureSearchAppResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryPictureSearchAppsRequest(TeaModel):
+    def __init__(
+        self,
+        page_size: int = None,
+        current_page: int = None,
+    ):
+        self.page_size = page_size
+        self.current_page = current_page
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        return self
+
+
+class QueryPictureSearchAppsResponseBodyDataPageData(TeaModel):
+    def __init__(
+        self,
+        app_instance_id: str = None,
+        modified_time: int = None,
+        description: str = None,
+        version: str = None,
+        create_time: int = None,
+        app_template_id: str = None,
+        name: str = None,
+    ):
+        self.app_instance_id = app_instance_id
+        self.modified_time = modified_time
+        self.description = description
+        self.version = version
+        self.create_time = create_time
+        self.app_template_id = app_template_id
+        self.name = name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_instance_id is not None:
+            result['AppInstanceId'] = self.app_instance_id
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.version is not None:
+            result['Version'] = self.version
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.app_template_id is not None:
+            result['AppTemplateId'] = self.app_template_id
+        if self.name is not None:
+            result['Name'] = self.name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AppInstanceId') is not None:
+            self.app_instance_id = m.get('AppInstanceId')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Version') is not None:
+            self.version = m.get('Version')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('AppTemplateId') is not None:
+            self.app_template_id = m.get('AppTemplateId')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        return self
+
+
+class QueryPictureSearchAppsResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        current_page: int = None,
+        page_data: List[QueryPictureSearchAppsResponseBodyDataPageData] = None,
+        page_size: int = None,
+        total: int = None,
+        page_count: int = None,
+    ):
+        self.current_page = current_page
+        self.page_data = page_data
+        self.page_size = page_size
+        self.total = total
+        self.page_count = page_count
+
+    def validate(self):
+        if self.page_data:
+            for k in self.page_data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        result['PageData'] = []
+        if self.page_data is not None:
+            for k in self.page_data:
+                result['PageData'].append(k.to_map() if k else None)
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        if self.page_count is not None:
+            result['PageCount'] = self.page_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        self.page_data = []
+        if m.get('PageData') is not None:
+            for k in m.get('PageData'):
+                temp_model = QueryPictureSearchAppsResponseBodyDataPageData()
+                self.page_data.append(temp_model.from_map(k))
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        if m.get('PageCount') is not None:
+            self.page_count = m.get('PageCount')
+        return self
+
+
+class QueryPictureSearchAppsResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        data: QueryPictureSearchAppsResponseBodyData = None,
+        error_message: str = None,
+        code: str = None,
+        success: bool = None,
+    ):
+        self.request_id = request_id
+        self.data = data
+        self.error_message = error_message
+        self.code = code
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Data') is not None:
+            temp_model = QueryPictureSearchAppsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class QueryPictureSearchAppsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: QueryPictureSearchAppsResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = QueryPictureSearchAppsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryPictureSearchDevicesRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         app_instance_id: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.app_instance_id = app_instance_id
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.app_instance_id is not None:
             result['AppInstanceId'] = self.app_instance_id
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AppInstanceId') is not None:
             self.app_instance_id = m.get('AppInstanceId')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         return self
@@ -15732,14 +16893,18 @@
         self.nick_name = nick_name
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.nick_name is not None:
             result['NickName'] = self.nick_name
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         return result
 
@@ -15770,14 +16935,18 @@
     def validate(self):
         if self.page_data:
             for k in self.page_data:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         result['PageData'] = []
         if self.page_data is not None:
             for k in self.page_data:
                 result['PageData'].append(k.to_map() if k else None)
@@ -15823,14 +16992,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -15868,14 +17041,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -15885,50 +17062,560 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = QueryPictureSearchDevicesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryPictureSearchJobRequest(TeaModel):
+    def __init__(
+        self,
+        app_instance_id: str = None,
+        job_status: int = None,
+        page_size: int = None,
+        current_page: int = None,
+    ):
+        self.app_instance_id = app_instance_id
+        self.job_status = job_status
+        self.page_size = page_size
+        self.current_page = current_page
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_instance_id is not None:
+            result['AppInstanceId'] = self.app_instance_id
+        if self.job_status is not None:
+            result['JobStatus'] = self.job_status
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AppInstanceId') is not None:
+            self.app_instance_id = m.get('AppInstanceId')
+        if m.get('JobStatus') is not None:
+            self.job_status = m.get('JobStatus')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        return self
+
+
+class QueryPictureSearchJobResponseBodyDataPageData(TeaModel):
+    def __init__(
+        self,
+        end_time: int = None,
+        start_time: int = None,
+        job_status: int = None,
+        search_pic_url: str = None,
+        create_time: int = None,
+        job_id: str = None,
+        threshold: float = None,
+    ):
+        self.end_time = end_time
+        self.start_time = start_time
+        self.job_status = job_status
+        self.search_pic_url = search_pic_url
+        self.create_time = create_time
+        self.job_id = job_id
+        self.threshold = threshold
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.job_status is not None:
+            result['JobStatus'] = self.job_status
+        if self.search_pic_url is not None:
+            result['SearchPicUrl'] = self.search_pic_url
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.threshold is not None:
+            result['Threshold'] = self.threshold
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('JobStatus') is not None:
+            self.job_status = m.get('JobStatus')
+        if m.get('SearchPicUrl') is not None:
+            self.search_pic_url = m.get('SearchPicUrl')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('Threshold') is not None:
+            self.threshold = m.get('Threshold')
+        return self
+
+
+class QueryPictureSearchJobResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        current_page: int = None,
+        page_data: List[QueryPictureSearchJobResponseBodyDataPageData] = None,
+        page_size: int = None,
+        total: int = None,
+        page_count: int = None,
+    ):
+        self.current_page = current_page
+        self.page_data = page_data
+        self.page_size = page_size
+        self.total = total
+        self.page_count = page_count
+
+    def validate(self):
+        if self.page_data:
+            for k in self.page_data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        result['PageData'] = []
+        if self.page_data is not None:
+            for k in self.page_data:
+                result['PageData'].append(k.to_map() if k else None)
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        if self.page_count is not None:
+            result['PageCount'] = self.page_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        self.page_data = []
+        if m.get('PageData') is not None:
+            for k in m.get('PageData'):
+                temp_model = QueryPictureSearchJobResponseBodyDataPageData()
+                self.page_data.append(temp_model.from_map(k))
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        if m.get('PageCount') is not None:
+            self.page_count = m.get('PageCount')
+        return self
+
+
+class QueryPictureSearchJobResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        data: QueryPictureSearchJobResponseBodyData = None,
+        error_message: str = None,
+        code: str = None,
+        success: bool = None,
+    ):
+        self.request_id = request_id
+        self.data = data
+        self.error_message = error_message
+        self.code = code
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Data') is not None:
+            temp_model = QueryPictureSearchJobResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class QueryPictureSearchJobResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: QueryPictureSearchJobResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = QueryPictureSearchJobResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class QueryPictureSearchJobResultRequest(TeaModel):
+    def __init__(
+        self,
+        app_instance_id: str = None,
+        job_id: str = None,
+        page_size: int = None,
+        current_page: int = None,
+    ):
+        self.app_instance_id = app_instance_id
+        self.job_id = job_id
+        self.page_size = page_size
+        self.current_page = current_page
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_instance_id is not None:
+            result['AppInstanceId'] = self.app_instance_id
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AppInstanceId') is not None:
+            self.app_instance_id = m.get('AppInstanceId')
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        return self
+
+
+class QueryPictureSearchJobResultResponseBodyDataPageData(TeaModel):
+    def __init__(
+        self,
+        pic_url: str = None,
+        event_time: int = None,
+        gateway_iot_id: str = None,
+        vector_id: str = None,
+        device_nick_name: str = None,
+        threshold: float = None,
+        iot_id: str = None,
+    ):
+        self.pic_url = pic_url
+        self.event_time = event_time
+        self.gateway_iot_id = gateway_iot_id
+        self.vector_id = vector_id
+        self.device_nick_name = device_nick_name
+        self.threshold = threshold
+        self.iot_id = iot_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.pic_url is not None:
+            result['PicUrl'] = self.pic_url
+        if self.event_time is not None:
+            result['EventTime'] = self.event_time
+        if self.gateway_iot_id is not None:
+            result['GatewayIotId'] = self.gateway_iot_id
+        if self.vector_id is not None:
+            result['VectorId'] = self.vector_id
+        if self.device_nick_name is not None:
+            result['DeviceNickName'] = self.device_nick_name
+        if self.threshold is not None:
+            result['Threshold'] = self.threshold
+        if self.iot_id is not None:
+            result['IotId'] = self.iot_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PicUrl') is not None:
+            self.pic_url = m.get('PicUrl')
+        if m.get('EventTime') is not None:
+            self.event_time = m.get('EventTime')
+        if m.get('GatewayIotId') is not None:
+            self.gateway_iot_id = m.get('GatewayIotId')
+        if m.get('VectorId') is not None:
+            self.vector_id = m.get('VectorId')
+        if m.get('DeviceNickName') is not None:
+            self.device_nick_name = m.get('DeviceNickName')
+        if m.get('Threshold') is not None:
+            self.threshold = m.get('Threshold')
+        if m.get('IotId') is not None:
+            self.iot_id = m.get('IotId')
+        return self
+
+
+class QueryPictureSearchJobResultResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        current_page: int = None,
+        page_data: List[QueryPictureSearchJobResultResponseBodyDataPageData] = None,
+        page_size: int = None,
+        total: int = None,
+        page_count: int = None,
+    ):
+        self.current_page = current_page
+        self.page_data = page_data
+        self.page_size = page_size
+        self.total = total
+        self.page_count = page_count
+
+    def validate(self):
+        if self.page_data:
+            for k in self.page_data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        result['PageData'] = []
+        if self.page_data is not None:
+            for k in self.page_data:
+                result['PageData'].append(k.to_map() if k else None)
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        if self.page_count is not None:
+            result['PageCount'] = self.page_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        self.page_data = []
+        if m.get('PageData') is not None:
+            for k in m.get('PageData'):
+                temp_model = QueryPictureSearchJobResultResponseBodyDataPageData()
+                self.page_data.append(temp_model.from_map(k))
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        if m.get('PageCount') is not None:
+            self.page_count = m.get('PageCount')
+        return self
+
+
+class QueryPictureSearchJobResultResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        data: QueryPictureSearchJobResultResponseBodyData = None,
+        error_message: str = None,
+        code: str = None,
+        success: bool = None,
+    ):
+        self.request_id = request_id
+        self.data = data
+        self.error_message = error_message
+        self.code = code
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Data') is not None:
+            temp_model = QueryPictureSearchJobResultResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class QueryPictureSearchJobResultResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: QueryPictureSearchJobResultResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = QueryPictureSearchJobResultResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryRecordRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         stream_type: int = None,
         begin_time: int = None,
         end_time: int = None,
         record_type: int = None,
         current_page: int = None,
         page_size: int = None,
         need_snapshot: bool = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.stream_type = stream_type
         self.begin_time = begin_time
         self.end_time = end_time
         self.record_type = record_type
         self.current_page = current_page
         self.page_size = page_size
         self.need_snapshot = need_snapshot
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.stream_type is not None:
             result['StreamType'] = self.stream_type
         if self.begin_time is not None:
             result['BeginTime'] = self.begin_time
         if self.end_time is not None:
@@ -15943,18 +17630,14 @@
             result['NeedSnapshot'] = self.need_snapshot
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('StreamType') is not None:
             self.stream_type = m.get('StreamType')
         if m.get('BeginTime') is not None:
             self.begin_time = m.get('BeginTime')
         if m.get('EndTime') is not None:
@@ -15993,14 +17676,18 @@
         self.video_frame_number = video_frame_number
         self.file_size = file_size
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.snapshot_url is not None:
             result['SnapshotUrl'] = self.snapshot_url
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.record_type is not None:
             result['RecordType'] = self.record_type
@@ -16051,14 +17738,18 @@
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
         if self.page_size is not None:
             result['PageSize'] = self.page_size
@@ -16096,14 +17787,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -16141,14 +17836,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -16161,49 +17860,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryRecordByRecordIdRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         record_id: str = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.record_id = record_id
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.record_id is not None:
             result['RecordId'] = self.record_id
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('RecordId') is not None:
             self.record_id = m.get('RecordId')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         return self
@@ -16222,14 +17913,18 @@
         self.file_name = file_name
         self.vod_url = vod_url
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.begin_time is not None:
             result['BeginTime'] = self.begin_time
         if self.file_name is not None:
             result['FileName'] = self.file_name
@@ -16268,14 +17963,18 @@
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         result['Data'] = []
         if self.data is not None:
             for k in self.data:
                 result['Data'].append(k.to_map() if k else None)
@@ -16317,14 +18016,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -16337,41 +18040,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryRecordPlanDetailRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         return self
 
 
 class QueryRecordPlanDetailResponseBodyDataTemplateInfoTimeSectionList(TeaModel):
     def __init__(
@@ -16384,14 +18079,18 @@
         self.begin = begin
         self.end = end
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.day_of_week is not None:
             result['DayOfWeek'] = self.day_of_week
         if self.begin is not None:
             result['Begin'] = self.begin
         if self.end is not None:
             result['End'] = self.end
@@ -16426,14 +18125,18 @@
     def validate(self):
         if self.time_section_list:
             for k in self.time_section_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['TimeSectionList'] = []
         if self.time_section_list is not None:
             for k in self.time_section_list:
                 result['TimeSectionList'].append(k.to_map() if k else None)
         if self.all_day is not None:
             result['AllDay'] = self.all_day
@@ -16477,14 +18180,18 @@
         self.template_id = template_id
 
     def validate(self):
         if self.template_info:
             self.template_info.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.name is not None:
             result['Name'] = self.name
         if self.template_info is not None:
             result['TemplateInfo'] = self.template_info.to_map()
@@ -16522,14 +18229,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -16567,14 +18278,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -16587,45 +18302,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryRecordPlanDeviceByDeviceRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         stream_type: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.stream_type = stream_type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.stream_type is not None:
             result['StreamType'] = self.stream_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('StreamType') is not None:
             self.stream_type = m.get('StreamType')
         return self
 
 
@@ -16640,14 +18347,18 @@
         self.begin = begin
         self.end = end
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.day_of_week is not None:
             result['DayOfWeek'] = self.day_of_week
         if self.begin is not None:
             result['Begin'] = self.begin
         if self.end is not None:
             result['End'] = self.end
@@ -16682,14 +18393,18 @@
     def validate(self):
         if self.time_section_list:
             for k in self.time_section_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['TimeSectionList'] = []
         if self.time_section_list is not None:
             for k in self.time_section_list:
                 result['TimeSectionList'].append(k.to_map() if k else None)
         if self.all_day is not None:
             result['AllDay'] = self.all_day
@@ -16733,14 +18448,18 @@
         self.template_id = template_id
 
     def validate(self):
         if self.template_info:
             self.template_info.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.name is not None:
             result['Name'] = self.name
         if self.template_info is not None:
             result['TemplateInfo'] = self.template_info.to_map()
@@ -16778,14 +18497,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -16823,14 +18546,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -16843,49 +18570,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryRecordPlanDeviceByPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
         current_page: int = None,
         page_size: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
         self.current_page = current_page
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         return self
@@ -16900,14 +18619,18 @@
         self.stream_type = stream_type
         self.iot_id = iot_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.stream_type is not None:
             result['StreamType'] = self.stream_type
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         return result
 
@@ -16938,14 +18661,18 @@
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
         if self.page_size is not None:
             result['PageSize'] = self.page_size
@@ -16991,14 +18718,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -17036,14 +18767,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -17056,45 +18791,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryRecordPlansRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         current_page: int = None,
         page_size: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.current_page = current_page
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         return self
 
 
@@ -17109,14 +18836,18 @@
         self.name = name
         self.template_id = template_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.name is not None:
             result['Name'] = self.name
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
@@ -17151,14 +18882,18 @@
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
         if self.page_size is not None:
             result['PageSize'] = self.page_size
@@ -17204,14 +18939,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -17249,14 +18988,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -17269,49 +19012,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryRecordUrlRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         file_name: str = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.file_name = file_name
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.file_name is not None:
             result['FileName'] = self.file_name
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('FileName') is not None:
             self.file_name = m.get('FileName')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         return self
@@ -17332,14 +19067,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -17376,14 +19115,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -17396,194 +19139,198 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryStandardAIAppTemplatesRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         return self
 
 
 class QueryStandardAIAppTemplatesResponseBodyDataList(TeaModel):
     def __init__(
         self,
-        app_template_id: str = None,
+        description: str = None,
         version: str = None,
+        app_template_id: str = None,
         name: str = None,
-        description: str = None,
     ):
-        self.app_template_id = app_template_id
+        self.description = description
         self.version = version
+        self.app_template_id = app_template_id
         self.name = name
-        self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.app_template_id is not None:
-            result['AppTemplateId'] = self.app_template_id
+        if self.description is not None:
+            result['Description'] = self.description
         if self.version is not None:
             result['Version'] = self.version
+        if self.app_template_id is not None:
+            result['AppTemplateId'] = self.app_template_id
         if self.name is not None:
             result['Name'] = self.name
-        if self.description is not None:
-            result['Description'] = self.description
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('AppTemplateId') is not None:
-            self.app_template_id = m.get('AppTemplateId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
         if m.get('Version') is not None:
             self.version = m.get('Version')
+        if m.get('AppTemplateId') is not None:
+            self.app_template_id = m.get('AppTemplateId')
         if m.get('Name') is not None:
             self.name = m.get('Name')
-        if m.get('Description') is not None:
-            self.description = m.get('Description')
         return self
 
 
 class QueryStandardAIAppTemplatesResponseBodyData(TeaModel):
     def __init__(
         self,
-        total: int = None,
-        page_count: int = None,
         current_page: int = None,
-        page_size: int = None,
         list: List[QueryStandardAIAppTemplatesResponseBodyDataList] = None,
+        page_size: int = None,
+        total: int = None,
+        page_count: int = None,
     ):
-        self.total = total
-        self.page_count = page_count
         self.current_page = current_page
-        self.page_size = page_size
         self.list = list
+        self.page_size = page_size
+        self.total = total
+        self.page_count = page_count
 
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.total is not None:
-            result['Total'] = self.total
-        if self.page_count is not None:
-            result['PageCount'] = self.page_count
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        if self.page_count is not None:
+            result['PageCount'] = self.page_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Total') is not None:
-            self.total = m.get('Total')
-        if m.get('PageCount') is not None:
-            self.page_count = m.get('PageCount')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
         self.list = []
         if m.get('List') is not None:
             for k in m.get('List'):
                 temp_model = QueryStandardAIAppTemplatesResponseBodyDataList()
                 self.list.append(temp_model.from_map(k))
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        if m.get('PageCount') is not None:
+            self.page_count = m.get('PageCount')
         return self
 
 
 class QueryStandardAIAppTemplatesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
+        data: QueryStandardAIAppTemplatesResponseBodyData = None,
         error_message: str = None,
         code: str = None,
-        data: QueryStandardAIAppTemplatesResponseBodyData = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
+        self.data = data
         self.error_message = error_message
         self.code = code
-        self.data = data
+        self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
+        if m.get('Data') is not None:
+            temp_model = QueryStandardAIAppTemplatesResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
-        if m.get('Data') is not None:
-            temp_model = QueryStandardAIAppTemplatesResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class QueryStandardAIAppTemplatesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -17595,14 +19342,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -17615,45 +19366,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryTimeTemplateRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         page_size: int = None,
         current_page: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.page_size = page_size
         self.current_page = current_page
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         return self
 
 
@@ -17668,14 +19411,18 @@
         self.begin = begin
         self.end = end
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.day_of_week is not None:
             result['DayOfWeek'] = self.day_of_week
         if self.begin is not None:
             result['Begin'] = self.begin
         if self.end is not None:
             result['End'] = self.end
@@ -17710,14 +19457,18 @@
     def validate(self):
         if self.time_section_list:
             for k in self.time_section_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['TimeSectionList'] = []
         if self.time_section_list is not None:
             for k in self.time_section_list:
                 result['TimeSectionList'].append(k.to_map() if k else None)
         if self.all_day is not None:
             result['AllDay'] = self.all_day
@@ -17765,14 +19516,18 @@
     def validate(self):
         if self.list:
             for k in self.list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['List'] = []
         if self.list is not None:
             for k in self.list:
                 result['List'].append(k.to_map() if k else None)
         if self.page_size is not None:
             result['PageSize'] = self.page_size
@@ -17818,14 +19573,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -17863,14 +19622,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -17883,41 +19646,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryTimeTemplateDetailRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         template_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.template_id = template_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         return self
 
 
 class QueryTimeTemplateDetailResponseBodyDataTimeSectionList(TeaModel):
     def __init__(
@@ -17930,14 +19685,18 @@
         self.begin = begin
         self.end = end
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.day_of_week is not None:
             result['DayOfWeek'] = self.day_of_week
         if self.begin is not None:
             result['Begin'] = self.begin
         if self.end is not None:
             result['End'] = self.end
@@ -17972,14 +19731,18 @@
     def validate(self):
         if self.time_section_list:
             for k in self.time_section_list:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         result['TimeSectionList'] = []
         if self.time_section_list is not None:
             for k in self.time_section_list:
                 result['TimeSectionList'].append(k.to_map() if k else None)
         if self.all_day is not None:
             result['AllDay'] = self.all_day
@@ -18025,14 +19788,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -18070,14 +19837,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -18090,45 +19861,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryVoiceIntercomRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         return self
 
 
@@ -18141,14 +19904,18 @@
         self.key = key
         self.iv = iv
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.key is not None:
             result['Key'] = self.key
         if self.iv is not None:
             result['Iv'] = self.iv
         return result
 
@@ -18171,14 +19938,18 @@
         self.url = url
 
     def validate(self):
         if self.crypto_key:
             self.crypto_key.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.crypto_key is not None:
             result['CryptoKey'] = self.crypto_key.to_map()
         if self.url is not None:
             result['Url'] = self.url
         return result
 
@@ -18208,14 +19979,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -18253,14 +20028,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -18273,84 +20052,80 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveAIAppRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         app_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.app_id = app_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.app_id is not None:
             result['AppId'] = self.app_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AppId') is not None:
             self.app_id = m.get('AppId')
         return self
 
 
 class RemoveAIAppResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
         error_message: str = None,
         code: str = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
         self.error_message = error_message
         self.code = code
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class RemoveAIAppResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -18362,14 +20137,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -18382,84 +20161,80 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveAIPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         return self
 
 
 class RemoveAIPlanResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
         error_message: str = None,
         code: str = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
         self.error_message = error_message
         self.code = code
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class RemoveAIPlanResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -18471,14 +20246,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -18491,41 +20270,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveDevicePurifyPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         return self
 
 
 class RemoveDevicePurifyPlanResponseBody(TeaModel):
     def __init__(
@@ -18540,14 +20311,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -18580,14 +20355,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -18600,57 +20379,49 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveFaceDeviceFromDeviceGroupRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         iot_instance_id: str = None,
         product_key: str = None,
         device_name: str = None,
         device_group_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.iot_instance_id = iot_instance_id
         self.product_key = product_key
         self.device_name = device_name
         self.device_group_id = device_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         if self.product_key is not None:
             result['ProductKey'] = self.product_key
         if self.device_name is not None:
             result['DeviceName'] = self.device_name
         if self.device_group_id is not None:
             result['DeviceGroupId'] = self.device_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         if m.get('ProductKey') is not None:
             self.product_key = m.get('ProductKey')
         if m.get('DeviceName') is not None:
@@ -18673,14 +20444,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -18713,14 +20488,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -18733,49 +20512,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveFaceUserFromUserGroupRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         user_id: str = None,
         user_group_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.user_id = user_id
         self.user_group_id = user_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
         if self.user_group_id is not None:
             result['UserGroupId'] = self.user_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('UserGroupId') is not None:
             self.user_group_id = m.get('UserGroupId')
         return self
@@ -18794,14 +20565,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -18834,14 +20609,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -18854,45 +20633,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetDevicePictureLifeCycleRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         day: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.day = day
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.day is not None:
             result['Day'] = self.day
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('Day') is not None:
             self.day = m.get('Day')
         return self
 
 
@@ -18909,14 +20680,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -18949,14 +20724,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -18969,45 +20748,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetDeviceRecordLifeCycleRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         day: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.day = day
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.day is not None:
             result['Day'] = self.day
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('Day') is not None:
             self.day = m.get('Day')
         return self
 
 
@@ -19024,14 +20795,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -19064,14 +20839,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -19084,49 +20863,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class StopLiveStreamingRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         stream_type: int = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.stream_type = stream_type
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.stream_type is not None:
             result['StreamType'] = self.stream_type
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('StreamType') is not None:
             self.stream_type = m.get('StreamType')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         return self
@@ -19145,14 +20916,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -19185,14 +20960,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -19205,45 +20984,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class StopTriggeredRecordRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         record_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.record_id = record_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.record_id is not None:
             result['RecordId'] = self.record_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('RecordId') is not None:
             self.record_id = m.get('RecordId')
         return self
 
 
@@ -19260,14 +21031,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -19300,14 +21075,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -19320,45 +21099,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class TriggerCapturePictureRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('IotInstanceId') is not None:
             self.iot_instance_id = m.get('IotInstanceId')
         return self
 
 
@@ -19377,14 +21148,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -19421,14 +21196,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -19441,57 +21220,49 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class TriggerRecordRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         iot_id: str = None,
         stream_type: int = None,
         pre_record_duration: int = None,
         record_duration: int = None,
         iot_instance_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.iot_id = iot_id
         self.stream_type = stream_type
         self.pre_record_duration = pre_record_duration
         self.record_duration = record_duration
         self.iot_instance_id = iot_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.iot_id is not None:
             result['IotId'] = self.iot_id
         if self.stream_type is not None:
             result['StreamType'] = self.stream_type
         if self.pre_record_duration is not None:
             result['PreRecordDuration'] = self.pre_record_duration
         if self.record_duration is not None:
             result['RecordDuration'] = self.record_duration
         if self.iot_instance_id is not None:
             result['IotInstanceId'] = self.iot_instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IotId') is not None:
             self.iot_id = m.get('IotId')
         if m.get('StreamType') is not None:
             self.stream_type = m.get('StreamType')
         if m.get('PreRecordDuration') is not None:
             self.pre_record_duration = m.get('PreRecordDuration')
         if m.get('RecordDuration') is not None:
@@ -19516,14 +21287,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -19560,14 +21335,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -19580,90 +21359,86 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UnbindAIPlanWithDevicesRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
         iot_id_list: List[str] = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
         self.iot_id_list = iot_id_list
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.iot_id_list is not None:
             result['IotIdList'] = self.iot_id_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         if m.get('IotIdList') is not None:
             self.iot_id_list = m.get('IotIdList')
         return self
 
 
 class UnbindAIPlanWithDevicesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
         error_message: str = None,
         code: str = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
         self.error_message = error_message
         self.code = code
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class UnbindAIPlanWithDevicesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -19675,14 +21450,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -19695,47 +21474,45 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UnbindPictureSearchAppWithDevicesRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         app_instance_id: str = None,
+        iot_instance_id: str = None,
         device_iot_ids: List[str] = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.app_instance_id = app_instance_id
+        self.iot_instance_id = iot_instance_id
         self.device_iot_ids = device_iot_ids
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.app_instance_id is not None:
             result['AppInstanceId'] = self.app_instance_id
+        if self.iot_instance_id is not None:
+            result['IotInstanceId'] = self.iot_instance_id
         if self.device_iot_ids is not None:
             result['DeviceIotIds'] = self.device_iot_ids
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AppInstanceId') is not None:
             self.app_instance_id = m.get('AppInstanceId')
+        if m.get('IotInstanceId') is not None:
+            self.iot_instance_id = m.get('IotInstanceId')
         if m.get('DeviceIotIds') is not None:
             self.device_iot_ids = m.get('DeviceIotIds')
         return self
 
 
 class UnbindPictureSearchAppWithDevicesResponseBody(TeaModel):
     def __init__(
@@ -19750,14 +21527,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -19790,14 +21571,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -19810,53 +21595,45 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateAIAppRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         app_id: str = None,
         level: int = None,
         name: str = None,
         description: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.app_id = app_id
         self.level = level
         self.name = name
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.app_id is not None:
             result['AppId'] = self.app_id
         if self.level is not None:
             result['Level'] = self.level
         if self.name is not None:
             result['Name'] = self.name
         if self.description is not None:
             result['Description'] = self.description
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('AppId') is not None:
             self.app_id = m.get('AppId')
         if m.get('Level') is not None:
             self.level = m.get('Level')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Description') is not None:
@@ -19864,48 +21641,52 @@
         return self
 
 
 class UpdateAIAppResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
         error_message: str = None,
         code: str = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
         self.error_message = error_message
         self.code = code
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class UpdateAIAppResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -19917,14 +21698,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -19937,90 +21722,86 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateAIPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
         description: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.description is not None:
             result['Description'] = self.description
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         return self
 
 
 class UpdateAIPlanResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
-        success: bool = None,
         error_message: str = None,
         code: str = None,
+        success: bool = None,
     ):
         self.request_id = request_id
-        self.success = success
         self.error_message = error_message
         self.code = code
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class UpdateAIPlanResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -20032,14 +21813,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -20052,49 +21837,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateDevicePurifyPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
         start_time: int = None,
         end_time: int = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
         self.start_time = start_time
         self.end_time = end_time
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         return self
@@ -20113,14 +21890,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -20153,14 +21934,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -20173,41 +21958,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateEventRecordPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
         name: str = None,
         event_types: str = None,
         pre_record_duration: int = None,
         record_duration: int = None,
         template_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
         self.name = name
         self.event_types = event_types
         self.pre_record_duration = pre_record_duration
         self.record_duration = record_duration
         self.template_id = template_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.name is not None:
             result['Name'] = self.name
         if self.event_types is not None:
             result['EventTypes'] = self.event_types
         if self.pre_record_duration is not None:
@@ -20216,18 +21997,14 @@
             result['RecordDuration'] = self.record_duration
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('EventTypes') is not None:
             self.event_types = m.get('EventTypes')
         if m.get('PreRecordDuration') is not None:
@@ -20252,14 +22029,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -20292,14 +22073,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -20312,41 +22097,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateFaceUserRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         user_id: str = None,
         name: str = None,
         params: str = None,
         face_pic_url: str = None,
         custom_user_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.user_id = user_id
         self.name = name
         self.params = params
         self.face_pic_url = face_pic_url
         self.custom_user_id = custom_user_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.user_id is not None:
             result['UserId'] = self.user_id
         if self.name is not None:
             result['Name'] = self.name
         if self.params is not None:
@@ -20355,18 +22136,14 @@
             result['FacePicUrl'] = self.face_pic_url
         if self.custom_user_id is not None:
             result['CustomUserId'] = self.custom_user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Params') is not None:
@@ -20391,14 +22168,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -20431,14 +22212,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -20451,49 +22236,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateFaceUserGroupAndDeviceGroupRelationRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         isolation_id: str = None,
         control_id: str = None,
         relation: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.isolation_id = isolation_id
         self.control_id = control_id
         self.relation = relation
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.isolation_id is not None:
             result['IsolationId'] = self.isolation_id
         if self.control_id is not None:
             result['ControlId'] = self.control_id
         if self.relation is not None:
             result['Relation'] = self.relation
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('IsolationId') is not None:
             self.isolation_id = m.get('IsolationId')
         if m.get('ControlId') is not None:
             self.control_id = m.get('ControlId')
         if m.get('Relation') is not None:
             self.relation = m.get('Relation')
         return self
@@ -20508,14 +22285,18 @@
         self.modified_time = modified_time
         self.control_id = control_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.control_id is not None:
             result['ControlId'] = self.control_id
         return result
 
@@ -20544,14 +22325,18 @@
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data.to_map()
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -20589,14 +22374,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -20609,53 +22398,45 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateModelRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         model_id: int = None,
         name: str = None,
         hardware: str = None,
         description: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.model_id = model_id
         self.name = name
         self.hardware = hardware
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.model_id is not None:
             result['ModelId'] = self.model_id
         if self.name is not None:
             result['Name'] = self.name
         if self.hardware is not None:
             result['Hardware'] = self.hardware
         if self.description is not None:
             result['Description'] = self.description
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('ModelId') is not None:
             self.model_id = m.get('ModelId')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Hardware') is not None:
             self.hardware = m.get('Hardware')
         if m.get('Description') is not None:
@@ -20678,14 +22459,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.data is not None:
             result['Data'] = self.data
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
@@ -20722,14 +22507,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -20739,52 +22528,165 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = UpdateModelResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdatePictureSearchAppRequest(TeaModel):
+    def __init__(
+        self,
+        app_instance_id: str = None,
+        name: str = None,
+        description: str = None,
+    ):
+        self.app_instance_id = app_instance_id
+        self.name = name
+        self.description = description
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_instance_id is not None:
+            result['AppInstanceId'] = self.app_instance_id
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.description is not None:
+            result['Description'] = self.description
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AppInstanceId') is not None:
+            self.app_instance_id = m.get('AppInstanceId')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        return self
+
+
+class UpdatePictureSearchAppResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        error_message: str = None,
+        code: str = None,
+        success: bool = None,
+    ):
+        self.request_id = request_id
+        self.error_message = error_message
+        self.code = code
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class UpdatePictureSearchAppResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: UpdatePictureSearchAppResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = UpdatePictureSearchAppResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateRecordPlanRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         plan_id: str = None,
         name: str = None,
         template_id: str = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.plan_id = plan_id
         self.name = name
         self.template_id = template_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.plan_id is not None:
             result['PlanId'] = self.plan_id
         if self.name is not None:
             result['Name'] = self.name
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('PlanId') is not None:
             self.plan_id = m.get('PlanId')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         return self
@@ -20803,14 +22705,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -20843,14 +22749,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
@@ -20875,14 +22785,18 @@
         self.begin = begin
         self.end = end
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.day_of_week is not None:
             result['DayOfWeek'] = self.day_of_week
         if self.begin is not None:
             result['Begin'] = self.begin
         if self.end is not None:
             result['End'] = self.end
@@ -20898,58 +22812,50 @@
             self.end = m.get('End')
         return self
 
 
 class UpdateTimeTemplateRequest(TeaModel):
     def __init__(
         self,
-        api_product: str = None,
-        api_revision: str = None,
         template_id: str = None,
         name: str = None,
         all_day: int = None,
         time_sections: List[UpdateTimeTemplateRequestTimeSections] = None,
     ):
-        self.api_product = api_product
-        self.api_revision = api_revision
         self.template_id = template_id
         self.name = name
         self.all_day = all_day
         self.time_sections = time_sections
 
     def validate(self):
         if self.time_sections:
             for k in self.time_sections:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
-        if self.api_product is not None:
-            result['ApiProduct'] = self.api_product
-        if self.api_revision is not None:
-            result['ApiRevision'] = self.api_revision
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         if self.name is not None:
             result['Name'] = self.name
         if self.all_day is not None:
             result['AllDay'] = self.all_day
         result['TimeSections'] = []
         if self.time_sections is not None:
             for k in self.time_sections:
                 result['TimeSections'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApiProduct') is not None:
-            self.api_product = m.get('ApiProduct')
-        if m.get('ApiRevision') is not None:
-            self.api_revision = m.get('ApiRevision')
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('AllDay') is not None:
             self.all_day = m.get('AllDay')
         self.time_sections = []
@@ -20973,14 +22879,18 @@
         self.code = code
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
         if self.code is not None:
             result['Code'] = self.code
@@ -21013,14 +22923,18 @@
     def validate(self):
         self.validate_required(self.headers, 'headers')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
```

### Comparing `alibabacloud_linkvisual20180120-2.0.1/alibabacloud_linkvisual20180120.egg-info/PKG-INFO` & `alibabacloud_linkvisual20180120-2.0.2/alibabacloud_linkvisual20180120.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-linkvisual20180120
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud LinkVisual (20180120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkvisual20180120-2.0.1/setup.py` & `alibabacloud_linkvisual20180120-2.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,29 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_linkvisual20180120.
 
-Created on 10/01/2021
+Created on 30/03/2021
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_linkvisual20180120"
 NAME = "alibabacloud_linkvisual20180120" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud LinkVisual (20180120) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.1, <1.0.0",
-    "alibabacloud_tea_openapi>=0.2.0, <1.0.0",
+    "alibabacloud_tea_util>=0.3.3, <1.0.0",
+    "alibabacloud_tea_openapi>=0.2.4, <1.0.0",
+    "alibabacloud_openapi_util>=0.1.4, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

