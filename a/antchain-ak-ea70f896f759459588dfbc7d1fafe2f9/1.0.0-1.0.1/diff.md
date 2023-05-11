# Comparing `tmp/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0.tar.gz` & `tmp/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0.tar", last modified: Wed May 10 09:22:44 2023, max compression
+gzip compressed data, was "dist/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1.tar", last modified: Wed May 10 09:49:35 2023, max compression
```

## Comparing `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0.tar` & `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 09:22:44.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-10 09:22:44.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 09:22:44.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 09:22:44.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_sdk_ak_ea70f896f759459588dfbc7d1fafe2f9/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_sdk_ak_ea70f896f759459588dfbc7d1fafe2f9/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15112 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_sdk_ak_ea70f896f759459588dfbc7d1fafe2f9/client.py
--rw-r--r--   0 root         (0) root         (0)     8406 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_sdk_ak_ea70f896f759459588dfbc7d1fafe2f9/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-10 09:22:44.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-10 09:22:43.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 09:49:35.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-10 09:49:35.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 09:49:35.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 09:49:35.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_sdk_ak_ea70f896f759459588dfbc7d1fafe2f9/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_sdk_ak_ea70f896f759459588dfbc7d1fafe2f9/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22608 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_sdk_ak_ea70f896f759459588dfbc7d1fafe2f9/client.py
+-rw-r--r--   0 root         (0) root         (0)    15220 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_sdk_ak_ea70f896f759459588dfbc7d1fafe2f9/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-10 09:49:35.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-10 09:49:34.000000 antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/setup.py
```

### Comparing `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/LICENSE` & `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/PKG-INFO` & `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_ak_ea70f896f759459588dfbc7d1fafe2f9
-Version: 1.0.0
+Name: antchain-ak-ea70f896f759459588dfbc7d1fafe2f9
+Version: 1.0.1
 Summary: Ant Chain Ak_ea70f896f759459588dfbc7d1fafe2f9 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/README-CN.md` & `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/README.md` & `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/PKG-INFO` & `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-ak-ea70f896f759459588dfbc7d1fafe2f9
-Version: 1.0.0
+Name: antchain_ak_ea70f896f759459588dfbc7d1fafe2f9
+Version: 1.0.1
 Summary: Ant Chain Ak_ea70f896f759459588dfbc7d1fafe2f9 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/SOURCES.txt` & `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_ak_ea70f896f759459588dfbc7d1fafe2f9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/antchain_sdk_ak_ea70f896f759459588dfbc7d1fafe2f9/models.py` & `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/antchain_sdk_ak_ea70f896f759459588dfbc7d1fafe2f9/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -225,7 +225,235 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
+class BindDemoAsdAsdAsdRequest(TeaModel):
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
+class BindDemoAsdAsdAsdResponse(TeaModel):
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
+class QueryDemoAaaBbbCccRequest(TeaModel):
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
+class QueryDemoAaaBbbCccResponse(TeaModel):
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
+class QueryDemoAbcAbcAbcRequest(TeaModel):
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
+class QueryDemoAbcAbcAbcResponse(TeaModel):
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
```

### Comparing `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.0/setup.py` & `antchain_ak_ea70f896f759459588dfbc7d1fafe2f9-1.0.1/setup.py`

 * *Files identical despite different names*

