# Comparing `tmp/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1.tar.gz` & `tmp/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1.tar", last modified: Tue Feb 14 01:41:33 2023, max compression
+gzip compressed data, was "dist/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2.tar", last modified: Wed May 10 11:10:42 2023, max compression
```

## Comparing `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1.tar` & `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 01:41:33.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-14 01:41:32.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-14 01:41:32.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-02-14 01:41:33.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-02-14 01:41:32.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-02-14 01:41:32.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 01:41:33.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-02-14 01:41:32.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-02-14 01:41:33.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-14 01:41:32.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-02-14 01:41:32.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-02-14 01:41:32.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 01:41:33.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_sdk_ak_d9fd09cd1986473d9a4b8dde727aa361/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-14 01:41:32.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_sdk_ak_d9fd09cd1986473d9a4b8dde727aa361/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25786 2023-02-14 01:41:32.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_sdk_ak_d9fd09cd1986473d9a4b8dde727aa361/client.py
--rw-r--r--   0 root         (0) root         (0)    27043 2023-02-14 01:41:32.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_sdk_ak_d9fd09cd1986473d9a4b8dde727aa361/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-14 01:41:33.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-02-14 01:41:32.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:10:42.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-10 11:10:41.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-10 11:10:41.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-10 11:10:42.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-10 11:10:41.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-10 11:10:41.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:10:42.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-10 11:10:42.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-10 11:10:42.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 11:10:42.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-10 11:10:42.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-10 11:10:42.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:10:42.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_sdk_ak_d9fd09cd1986473d9a4b8dde727aa361/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 11:10:41.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_sdk_ak_d9fd09cd1986473d9a4b8dde727aa361/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36512 2023-05-10 11:10:41.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_sdk_ak_d9fd09cd1986473d9a4b8dde727aa361/client.py
+-rw-r--r--   0 root         (0) root         (0)    39082 2023-05-10 11:10:41.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_sdk_ak_d9fd09cd1986473d9a4b8dde727aa361/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-10 11:10:42.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-10 11:10:41.000000 antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/setup.py
```

### Comparing `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/LICENSE` & `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/PKG-INFO` & `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_d9fd09cd1986473d9a4b8dde727aa361
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ant Chain Ak_d9fd09cd1986473d9a4b8dde727aa361 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/README-CN.md` & `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/README.md` & `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/PKG-INFO` & `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-d9fd09cd1986473d9a4b8dde727aa361
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ant Chain Ak_d9fd09cd1986473d9a4b8dde727aa361 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/SOURCES.txt` & `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/antchain_sdk_ak_d9fd09cd1986473d9a4b8dde727aa361/models.py` & `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/antchain_sdk_ak_d9fd09cd1986473d9a4b8dde727aa361/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -215,14 +215,49 @@
         if m.get('some_int') is not None:
             self.some_int = m.get('some_int')
         if m.get('some_list') is not None:
             self.some_list = m.get('some_list')
         return self
 
 
+class FaceImage(TeaModel):
+    def __init__(
+        self,
+        content: str = None,
+        rect: str = None,
+    ):
+        # 123
+        self.content = content
+        # 123
+        self.rect = rect
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
+        if self.content is not None:
+            result['content'] = self.content
+        if self.rect is not None:
+            result['rect'] = self.rect
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        if m.get('rect') is not None:
+            self.rect = m.get('rect')
+        return self
+
+
 class TestStruct(TeaModel):
     def __init__(
         self,
         x: str = None,
         y: DemoClass = None,
         z: List[DemoClass] = None,
     ):
@@ -581,14 +616,373 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class MatchInternationalDemoZolozFacecompareRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_id: str = None,
+        face_1: FaceImage = None,
+        face_2: FaceImage = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 123
+        self.biz_id = biz_id
+        # 123
+        self.face_1 = face_1
+        # 123
+        self.face_2 = face_2
+
+    def validate(self):
+        self.validate_required(self.biz_id, 'biz_id')
+        if self.face_1:
+            self.face_1.validate()
+        if self.face_2:
+            self.face_2.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_id is not None:
+            result['biz_id'] = self.biz_id
+        if self.face_1 is not None:
+            result['face1'] = self.face_1.to_map()
+        if self.face_2 is not None:
+            result['face2'] = self.face_2.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_id') is not None:
+            self.biz_id = m.get('biz_id')
+        if m.get('face1') is not None:
+            temp_model = FaceImage()
+            self.face_1 = temp_model.from_map(m['face1'])
+        if m.get('face2') is not None:
+            temp_model = FaceImage()
+            self.face_2 = temp_model.from_map(m['face2'])
+        return self
+
+
+class MatchInternationalDemoZolozFacecompareResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        transaction_id: str = None,
+        same_person: bool = None,
+        score: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 123
+        self.transaction_id = transaction_id
+        # 123
+        self.same_person = same_person
+        # 100
+        self.score = score
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.transaction_id is not None:
+            result['transaction_id'] = self.transaction_id
+        if self.same_person is not None:
+            result['same_person'] = self.same_person
+        if self.score is not None:
+            result['score'] = self.score
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('transaction_id') is not None:
+            self.transaction_id = m.get('transaction_id')
+        if m.get('same_person') is not None:
+            self.same_person = m.get('same_person')
+        if m.get('score') is not None:
+            self.score = m.get('score')
+        return self
+
+
+class QueryInternationalDemoAaaBbbRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
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
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        return self
+
+
+class QueryInternationalDemoAaaBbbResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class CheckInternationalDemoZolozHealthRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        data: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 1123
+        self.data = data
+
+    def validate(self):
+        self.validate_required(self.data, 'data')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.data is not None:
+            result['data'] = self.data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
+class CheckInternationalDemoZolozHealthResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class GetInternationalDemoAaaBbbRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
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
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        return self
+
+
+class GetInternationalDemoAaaBbbResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
```

### Comparing `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.1/setup.py` & `antchain_ak_d9fd09cd1986473d9a4b8dde727aa361-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_d9fd09cd1986473d9a4b8dde727aa361.
 
-Created on 14/02/2023
+Created on 10/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_d9fd09cd1986473d9a4b8dde727aa361"
 NAME = "antchain_ak_d9fd09cd1986473d9a4b8dde727aa361" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_d9fd09cd1986473d9a4b8dde727aa361 SDK Library for Python"
```

