# Comparing `tmp/alibabacloud_iot20180120-3.1.0.tar.gz` & `tmp/alibabacloud_iot20180120-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_iot20180120-3.1.0.tar", last modified: Thu Mar  2 12:35:35 2023, max compression
+gzip compressed data, was "dist/alibabacloud_iot20180120-3.1.1.tar", last modified: Mon Mar  6 11:54:50 2023, max compression
```

## Comparing `alibabacloud_iot20180120-3.1.0.tar` & `alibabacloud_iot20180120-3.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/
--rw-r--r--   0 root         (0) root         (0)     1904 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2337 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1350695 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120/client.py
--rw-r--r--   0 root         (0) root         (0)  2512712 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2337 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2619 2023-03-02 12:35:35.000000 alibabacloud_iot20180120-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 11:54:50.000000 alibabacloud_iot20180120-3.1.1/
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-03-06 11:54:50.000000 alibabacloud_iot20180120-3.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 11:54:50.000000 alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1356819 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120/client.py
+-rw-r--r--   0 root         (0) root         (0)  2522174 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 11:54:50.000000 alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-03-06 11:54:50.000000 alibabacloud_iot20180120-3.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-03-06 11:54:49.000000 alibabacloud_iot20180120-3.1.1/setup.py
```

### Comparing `alibabacloud_iot20180120-3.1.0/ChangeLog.md` & `alibabacloud_iot20180120-3.1.1/ChangeLog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-03-02 Version: 3.1.0
+- Add a API QueryDeviceProvisioning to support query provisioning info for device.
+
 2023-02-10 Version: 3.0.16
 - Support broadcast for FengTian.
 
 2023-01-13 Version: 0.3.0
 - Add ClearDeviceDesiredProperty open api.
 
 2023-01-03 Version: 3.0.15
```

### Comparing `alibabacloud_iot20180120-3.1.0/LICENSE` & `alibabacloud_iot20180120-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_iot20180120-3.1.0/PKG-INFO` & `alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_iot20180120
-Version: 3.1.0
+Name: alibabacloud-iot20180120
+Version: 3.1.1
 Summary: Alibaba Cloud IoT Platform (20180120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_iot20180120-3.1.0/README-CN.md` & `alibabacloud_iot20180120-3.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_iot20180120-3.1.0/README.md` & `alibabacloud_iot20180120-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120/client.py` & `alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -14086,14 +14086,92 @@
     async def get_scene_rule_async(
         self,
         request: iot_20180120_models.GetSceneRuleRequest,
     ) -> iot_20180120_models.GetSceneRuleResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_scene_rule_with_options_async(request, runtime)
 
+    def get_share_speech_model_audio_with_options(
+        self,
+        request: iot_20180120_models.GetShareSpeechModelAudioRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> iot_20180120_models.GetShareSpeechModelAudioResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.iot_instance_id):
+            body['IotInstanceId'] = request.iot_instance_id
+        if not UtilClient.is_unset(request.share_task_id):
+            body['ShareTaskId'] = request.share_task_id
+        if not UtilClient.is_unset(request.speech_model_code_list):
+            body['SpeechModelCodeList'] = request.speech_model_code_list
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetShareSpeechModelAudio',
+            version='2018-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            iot_20180120_models.GetShareSpeechModelAudioResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_share_speech_model_audio_with_options_async(
+        self,
+        request: iot_20180120_models.GetShareSpeechModelAudioRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> iot_20180120_models.GetShareSpeechModelAudioResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.iot_instance_id):
+            body['IotInstanceId'] = request.iot_instance_id
+        if not UtilClient.is_unset(request.share_task_id):
+            body['ShareTaskId'] = request.share_task_id
+        if not UtilClient.is_unset(request.speech_model_code_list):
+            body['SpeechModelCodeList'] = request.speech_model_code_list
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetShareSpeechModelAudio',
+            version='2018-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            iot_20180120_models.GetShareSpeechModelAudioResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_share_speech_model_audio(
+        self,
+        request: iot_20180120_models.GetShareSpeechModelAudioRequest,
+    ) -> iot_20180120_models.GetShareSpeechModelAudioResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_share_speech_model_audio_with_options(request, runtime)
+
+    async def get_share_speech_model_audio_async(
+        self,
+        request: iot_20180120_models.GetShareSpeechModelAudioRequest,
+    ) -> iot_20180120_models.GetShareSpeechModelAudioResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_share_speech_model_audio_with_options_async(request, runtime)
+
     def get_share_task_by_device_open_with_options(
         self,
         request: iot_20180120_models.GetShareTaskByDeviceOpenRequest,
         runtime: util_models.RuntimeOptions,
     ) -> iot_20180120_models.GetShareTaskByDeviceOpenResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -25380,14 +25458,84 @@
     async def query_speech_device_async(
         self,
         request: iot_20180120_models.QuerySpeechDeviceRequest,
     ) -> iot_20180120_models.QuerySpeechDeviceResponse:
         runtime = util_models.RuntimeOptions()
         return await self.query_speech_device_with_options_async(request, runtime)
 
+    def query_speech_license_available_quota_with_options(
+        self,
+        request: iot_20180120_models.QuerySpeechLicenseAvailableQuotaRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> iot_20180120_models.QuerySpeechLicenseAvailableQuotaResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.iot_instance_id):
+            body['IotInstanceId'] = request.iot_instance_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='QuerySpeechLicenseAvailableQuota',
+            version='2018-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            iot_20180120_models.QuerySpeechLicenseAvailableQuotaResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def query_speech_license_available_quota_with_options_async(
+        self,
+        request: iot_20180120_models.QuerySpeechLicenseAvailableQuotaRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> iot_20180120_models.QuerySpeechLicenseAvailableQuotaResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.iot_instance_id):
+            body['IotInstanceId'] = request.iot_instance_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='QuerySpeechLicenseAvailableQuota',
+            version='2018-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            iot_20180120_models.QuerySpeechLicenseAvailableQuotaResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def query_speech_license_available_quota(
+        self,
+        request: iot_20180120_models.QuerySpeechLicenseAvailableQuotaRequest,
+    ) -> iot_20180120_models.QuerySpeechLicenseAvailableQuotaResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.query_speech_license_available_quota_with_options(request, runtime)
+
+    async def query_speech_license_available_quota_async(
+        self,
+        request: iot_20180120_models.QuerySpeechLicenseAvailableQuotaRequest,
+    ) -> iot_20180120_models.QuerySpeechLicenseAvailableQuotaResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.query_speech_license_available_quota_with_options_async(request, runtime)
+
     def query_speech_license_device_list_with_options(
         self,
         request: iot_20180120_models.QuerySpeechLicenseDeviceListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> iot_20180120_models.QuerySpeechLicenseDeviceListResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120/models.py` & `alibabacloud_iot20180120-3.1.1/alibabacloud_iot20180120/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,41 +182,59 @@
             self.share_task_id = m.get('ShareTaskId')
         return self
 
 
 class AddShareTaskDeviceResponseBodyData(TeaModel):
     def __init__(
         self,
+        fail_sum: int = None,
+        failed_result_csv_file: str = None,
         progress: int = None,
         progress_id: str = None,
+        success_sum: int = None,
     ):
+        self.fail_sum = fail_sum
+        self.failed_result_csv_file = failed_result_csv_file
         self.progress = progress
         self.progress_id = progress_id
+        self.success_sum = success_sum
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.fail_sum is not None:
+            result['FailSum'] = self.fail_sum
+        if self.failed_result_csv_file is not None:
+            result['FailedResultCsvFile'] = self.failed_result_csv_file
         if self.progress is not None:
             result['Progress'] = self.progress
         if self.progress_id is not None:
             result['ProgressId'] = self.progress_id
+        if self.success_sum is not None:
+            result['SuccessSum'] = self.success_sum
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('FailSum') is not None:
+            self.fail_sum = m.get('FailSum')
+        if m.get('FailedResultCsvFile') is not None:
+            self.failed_result_csv_file = m.get('FailedResultCsvFile')
         if m.get('Progress') is not None:
             self.progress = m.get('Progress')
         if m.get('ProgressId') is not None:
             self.progress_id = m.get('ProgressId')
+        if m.get('SuccessSum') is not None:
+            self.success_sum = m.get('SuccessSum')
         return self
 
 
 class AddShareTaskDeviceResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
@@ -29141,14 +29159,177 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetSceneRuleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetShareSpeechModelAudioRequest(TeaModel):
+    def __init__(
+        self,
+        iot_instance_id: str = None,
+        share_task_id: str = None,
+        speech_model_code_list: List[str] = None,
+    ):
+        self.iot_instance_id = iot_instance_id
+        self.share_task_id = share_task_id
+        self.speech_model_code_list = speech_model_code_list
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
+        if self.iot_instance_id is not None:
+            result['IotInstanceId'] = self.iot_instance_id
+        if self.share_task_id is not None:
+            result['ShareTaskId'] = self.share_task_id
+        if self.speech_model_code_list is not None:
+            result['SpeechModelCodeList'] = self.speech_model_code_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('IotInstanceId') is not None:
+            self.iot_instance_id = m.get('IotInstanceId')
+        if m.get('ShareTaskId') is not None:
+            self.share_task_id = m.get('ShareTaskId')
+        if m.get('SpeechModelCodeList') is not None:
+            self.speech_model_code_list = m.get('SpeechModelCodeList')
+        return self
+
+
+class GetShareSpeechModelAudioResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        data: List[str] = None,
+    ):
+        self.data = data
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
+        if self.data is not None:
+            result['data'] = self.data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
+class GetShareSpeechModelAudioResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: GetShareSpeechModelAudioResponseBodyData = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.error_message = error_message
+        self.request_id = request_id
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetShareSpeechModelAudioResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetShareSpeechModelAudioResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetShareSpeechModelAudioResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
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
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetShareSpeechModelAudioResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetShareTaskByDeviceOpenRequest(TeaModel):
     def __init__(
         self,
         device_name: str = None,
         iot_id: str = None,
         iot_instance_id: str = None,
         product_key: str = None,
@@ -62393,14 +62574,136 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QuerySpeechDeviceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QuerySpeechLicenseAvailableQuotaRequest(TeaModel):
+    def __init__(
+        self,
+        iot_instance_id: str = None,
+    ):
+        self.iot_instance_id = iot_instance_id
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
+        if self.iot_instance_id is not None:
+            result['IotInstanceId'] = self.iot_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('IotInstanceId') is not None:
+            self.iot_instance_id = m.get('IotInstanceId')
+        return self
+
+
+class QuerySpeechLicenseAvailableQuotaResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: int = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.error_message = error_message
+        self.request_id = request_id
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class QuerySpeechLicenseAvailableQuotaResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QuerySpeechLicenseAvailableQuotaResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
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
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QuerySpeechLicenseAvailableQuotaResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QuerySpeechLicenseDeviceListRequest(TeaModel):
     def __init__(
         self,
         check_group_id: str = None,
         device_name: str = None,
         iot_instance_id: str = None,
         license_status_list: List[str] = None,
```

### Comparing `alibabacloud_iot20180120-3.1.0/alibabacloud_iot20180120.egg-info/PKG-INFO` & `alibabacloud_iot20180120-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-iot20180120
-Version: 3.1.0
+Name: alibabacloud_iot20180120
+Version: 3.1.1
 Summary: Alibaba Cloud IoT Platform (20180120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_iot20180120-3.1.0/setup.py` & `alibabacloud_iot20180120-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_iot20180120.
 
-Created on 02/03/2023
+Created on 06/03/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_iot20180120"
 NAME = "alibabacloud_iot20180120" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud IoT Platform (20180120) SDK Library for Python"
```

