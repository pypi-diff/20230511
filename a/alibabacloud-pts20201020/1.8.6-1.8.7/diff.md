# Comparing `tmp/alibabacloud_pts20201020-1.8.6.tar.gz` & `tmp/alibabacloud_pts20201020-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pts20201020-1.8.6.tar", last modified: Tue Dec  7 03:27:38 2021, max compression
+gzip compressed data, was "dist/alibabacloud_pts20201020-1.8.7.tar", last modified: Mon Dec 20 06:04:03 2021, max compression
```

## Comparing `alibabacloud_pts20201020-1.8.6.tar` & `alibabacloud_pts20201020-1.8.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/
--rw-r--r--   0 root         (0) root         (0)      271 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2344 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020/
--rw-r--r--   0 root         (0) root         (0)       21 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94831 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020/client.py
--rw-r--r--   0 root         (0) root         (0)   275323 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2344 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2626 2021-12-07 03:27:38.000000 alibabacloud_pts20201020-1.8.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-20 06:04:03.000000 alibabacloud_pts20201020-1.8.7/
+-rw-r--r--   0 root         (0) root         (0)      331 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2344 2021-12-20 06:04:03.000000 alibabacloud_pts20201020-1.8.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-20 06:04:03.000000 alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92043 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020/client.py
+-rw-r--r--   0 root         (0) root         (0)   275191 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-20 06:04:03.000000 alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2344 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2021-12-20 06:04:03.000000 alibabacloud_pts20201020-1.8.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2626 2021-12-20 06:04:02.000000 alibabacloud_pts20201020-1.8.7/setup.py
```

### Comparing `alibabacloud_pts20201020-1.8.6/LICENSE` & `alibabacloud_pts20201020-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pts20201020-1.8.6/PKG-INFO` & `alibabacloud_pts20201020-1.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pts20201020
-Version: 1.8.6
+Version: 1.8.7
 Summary: Alibaba Cloud Performance Testing (20201020) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pts20201020-1.8.6/README-CN.md` & `alibabacloud_pts20201020-1.8.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pts20201020-1.8.6/README.md` & `alibabacloud_pts20201020-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020/client.py` & `alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,26 +46,25 @@
         request: pts20201020_models.CreatePtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.CreatePtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['Scene'] = request.scene
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreatePtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.CreatePtsSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -74,26 +73,25 @@
         request: pts20201020_models.CreatePtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.CreatePtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['Scene'] = request.scene
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreatePtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.CreatePtsSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -117,26 +115,25 @@
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.CreatePtsSceneBaseLineFromReportResponse:
         UtilClient.validate_model(request)
         query = {}
         query['ReportId'] = request.report_id
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreatePtsSceneBaseLineFromReport',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.CreatePtsSceneBaseLineFromReportResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -146,26 +143,25 @@
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.CreatePtsSceneBaseLineFromReportResponse:
         UtilClient.validate_model(request)
         query = {}
         query['ReportId'] = request.report_id
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreatePtsSceneBaseLineFromReport',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.CreatePtsSceneBaseLineFromReportResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -188,26 +184,25 @@
         request: pts20201020_models.DeletePtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.DeletePtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeletePtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.DeletePtsSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -216,26 +211,25 @@
         request: pts20201020_models.DeletePtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.DeletePtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeletePtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.DeletePtsSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -258,26 +252,25 @@
         request: pts20201020_models.DeletePtsSceneBaseLineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.DeletePtsSceneBaseLineResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeletePtsSceneBaseLine',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.DeletePtsSceneBaseLineResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -286,26 +279,25 @@
         request: pts20201020_models.DeletePtsSceneBaseLineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.DeletePtsSceneBaseLineResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeletePtsSceneBaseLine',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.DeletePtsSceneBaseLineResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -332,26 +324,25 @@
         request = pts20201020_models.DeletePtsScenesShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.scene_ids):
             request.scene_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.scene_ids, 'SceneIds', 'json')
         query = {}
         query['SceneIds'] = request.scene_ids_shrink
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeletePtsScenes',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.DeletePtsScenesResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -364,26 +355,25 @@
         request = pts20201020_models.DeletePtsScenesShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.scene_ids):
             request.scene_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.scene_ids, 'SceneIds', 'json')
         query = {}
         query['SceneIds'] = request.scene_ids_shrink
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeletePtsScenes',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.DeletePtsScenesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -414,26 +404,25 @@
         query['Keyword'] = request.keyword
         query['Level'] = request.level
         query['PageNumber'] = request.page_number
         query['PageSize'] = request.page_size
         query['ReportId'] = request.report_id
         query['Thread'] = request.thread
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetJMeterLogs',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetJMeterLogsResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -450,26 +439,25 @@
         query['Keyword'] = request.keyword
         query['Level'] = request.level
         query['PageNumber'] = request.page_number
         query['PageSize'] = request.page_size
         query['ReportId'] = request.report_id
         query['Thread'] = request.thread
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetJMeterLogs',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetJMeterLogsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -495,26 +483,25 @@
         UtilClient.validate_model(request)
         query = {}
         query['BeginTime'] = request.begin_time
         query['EndTime'] = request.end_time
         query['ReportId'] = request.report_id
         query['SamplerId'] = request.sampler_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetJMeterSampleMetrics',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetJMeterSampleMetricsResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -526,26 +513,25 @@
         UtilClient.validate_model(request)
         query = {}
         query['BeginTime'] = request.begin_time
         query['EndTime'] = request.end_time
         query['ReportId'] = request.report_id
         query['SamplerId'] = request.sampler_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetJMeterSampleMetrics',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetJMeterSampleMetricsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -580,26 +566,25 @@
         query['PageSize'] = request.page_size
         query['ReportId'] = request.report_id
         query['ResponseCode'] = request.response_code
         query['SamplerId'] = request.sampler_id
         query['Success'] = request.success
         query['Thread'] = request.thread
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetJMeterSamplingLogs',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetJMeterSamplingLogsResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -620,26 +605,25 @@
         query['PageSize'] = request.page_size
         query['ReportId'] = request.report_id
         query['ResponseCode'] = request.response_code
         query['SamplerId'] = request.sampler_id
         query['Success'] = request.success
         query['Thread'] = request.thread
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetJMeterSamplingLogs',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetJMeterSamplingLogsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -662,26 +646,25 @@
         request: pts20201020_models.GetJMeterSceneRunningDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetJMeterSceneRunningDataResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetJMeterSceneRunningData',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetJMeterSceneRunningDataResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -690,26 +673,25 @@
         request: pts20201020_models.GetJMeterSceneRunningDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetJMeterSceneRunningDataResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetJMeterSceneRunningData',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetJMeterSceneRunningDataResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -732,26 +714,25 @@
         request: pts20201020_models.GetOpenJMeterSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetOpenJMeterSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetOpenJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetOpenJMeterSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -760,26 +741,25 @@
         request: pts20201020_models.GetOpenJMeterSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetOpenJMeterSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetOpenJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetOpenJMeterSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -803,26 +783,25 @@
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetPtsReportDetailsResponse:
         UtilClient.validate_model(request)
         query = {}
         query['PlanId'] = request.plan_id
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPtsReportDetails',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetPtsReportDetailsResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -832,26 +811,25 @@
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetPtsReportDetailsResponse:
         UtilClient.validate_model(request)
         query = {}
         query['PlanId'] = request.plan_id
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPtsReportDetails',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetPtsReportDetailsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -876,26 +854,25 @@
     ) -> pts20201020_models.GetPtsReportsBySceneIdResponse:
         UtilClient.validate_model(request)
         query = {}
         query['PageNumber'] = request.page_number
         query['PageSize'] = request.page_size
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPtsReportsBySceneId',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetPtsReportsBySceneIdResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -906,26 +883,25 @@
     ) -> pts20201020_models.GetPtsReportsBySceneIdResponse:
         UtilClient.validate_model(request)
         query = {}
         query['PageNumber'] = request.page_number
         query['PageSize'] = request.page_size
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPtsReportsBySceneId',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetPtsReportsBySceneIdResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -948,26 +924,25 @@
         request: pts20201020_models.GetPtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetPtsSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -976,26 +951,25 @@
         request: pts20201020_models.GetPtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetPtsSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1018,26 +992,25 @@
         request: pts20201020_models.GetPtsSceneBaseLineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetPtsSceneBaseLineResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPtsSceneBaseLine',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetPtsSceneBaseLineResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1046,26 +1019,25 @@
         request: pts20201020_models.GetPtsSceneBaseLineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetPtsSceneBaseLineResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPtsSceneBaseLine',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetPtsSceneBaseLineResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1089,26 +1061,25 @@
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetPtsSceneRunningDataResponse:
         UtilClient.validate_model(request)
         query = {}
         query['PlanId'] = request.plan_id
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPtsSceneRunningData',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetPtsSceneRunningDataResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1118,26 +1089,25 @@
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetPtsSceneRunningDataResponse:
         UtilClient.validate_model(request)
         query = {}
         query['PlanId'] = request.plan_id
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPtsSceneRunningData',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetPtsSceneRunningDataResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1160,26 +1130,25 @@
         request: pts20201020_models.GetPtsSceneRunningStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetPtsSceneRunningStatusResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPtsSceneRunningStatus',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetPtsSceneRunningStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1188,26 +1157,25 @@
         request: pts20201020_models.GetPtsSceneRunningStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.GetPtsSceneRunningStatusResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPtsSceneRunningStatus',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.GetPtsSceneRunningStatusResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1233,26 +1201,25 @@
         UtilClient.validate_model(request)
         query = {}
         query['EnvId'] = request.env_id
         query['EnvName'] = request.env_name
         query['PageNumber'] = request.page_number
         query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListEnvs',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.ListEnvsResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1264,26 +1231,25 @@
         UtilClient.validate_model(request)
         query = {}
         query['EnvId'] = request.env_id
         query['EnvName'] = request.env_name
         query['PageNumber'] = request.page_number
         query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListEnvs',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.ListEnvsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1312,26 +1278,25 @@
         query['EndTime'] = request.end_time
         query['Keyword'] = request.keyword
         query['PageNumber'] = request.page_number
         query['PageSize'] = request.page_size
         query['ReportId'] = request.report_id
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListJMeterReports',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.ListJMeterReportsResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1346,26 +1311,25 @@
         query['EndTime'] = request.end_time
         query['Keyword'] = request.keyword
         query['PageNumber'] = request.page_number
         query['PageSize'] = request.page_size
         query['ReportId'] = request.report_id
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListJMeterReports',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.ListJMeterReportsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1391,26 +1355,25 @@
         UtilClient.validate_model(request)
         query = {}
         query['PageNumber'] = request.page_number
         query['PageSize'] = request.page_size
         query['SceneId'] = request.scene_id
         query['SceneName'] = request.scene_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListOpenJMeterScenes',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.ListOpenJMeterScenesResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1422,26 +1385,25 @@
         UtilClient.validate_model(request)
         query = {}
         query['PageNumber'] = request.page_number
         query['PageSize'] = request.page_size
         query['SceneId'] = request.scene_id
         query['SceneName'] = request.scene_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListOpenJMeterScenes',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.ListOpenJMeterScenesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1466,26 +1428,25 @@
     ) -> pts20201020_models.ListPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['KeyWord'] = request.key_word
         query['PageNumber'] = request.page_number
         query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.ListPtsSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1496,26 +1457,25 @@
     ) -> pts20201020_models.ListPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['KeyWord'] = request.key_word
         query['PageNumber'] = request.page_number
         query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.ListPtsSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1538,26 +1498,25 @@
         request: pts20201020_models.ModifyPtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.ModifyPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['Scene'] = request.scene
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.ModifyPtsSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1566,26 +1525,25 @@
         request: pts20201020_models.ModifyPtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.ModifyPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['Scene'] = request.scene
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.ModifyPtsSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1608,26 +1566,25 @@
         request: pts20201020_models.RemoveEnvRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.RemoveEnvResponse:
         UtilClient.validate_model(request)
         query = {}
         query['EnvId'] = request.env_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RemoveEnv',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.RemoveEnvResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1636,26 +1593,25 @@
         request: pts20201020_models.RemoveEnvRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.RemoveEnvResponse:
         UtilClient.validate_model(request)
         query = {}
         query['EnvId'] = request.env_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RemoveEnv',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.RemoveEnvResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1678,26 +1634,25 @@
         request: pts20201020_models.RemoveOpenJMeterSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.RemoveOpenJMeterSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RemoveOpenJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.RemoveOpenJMeterSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1706,26 +1661,25 @@
         request: pts20201020_models.RemoveOpenJMeterSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.RemoveOpenJMeterSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RemoveOpenJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.RemoveOpenJMeterSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1752,26 +1706,25 @@
         request = pts20201020_models.SaveEnvShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.env):
             request.env_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.env), 'Env', 'json')
         query = {}
         query['Env'] = request.env_shrink
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SaveEnv',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.SaveEnvResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1784,26 +1737,25 @@
         request = pts20201020_models.SaveEnvShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.env):
             request.env_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.env), 'Env', 'json')
         query = {}
         query['Env'] = request.env_shrink
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SaveEnv',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.SaveEnvResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1830,26 +1782,25 @@
         request = pts20201020_models.SaveOpenJMeterSceneShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.open_jmeter_scene):
             request.open_jmeter_scene_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_jmeter_scene), 'OpenJMeterScene', 'json')
         query = {}
         query['OpenJMeterScene'] = request.open_jmeter_scene_shrink
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SaveOpenJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.SaveOpenJMeterSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1862,26 +1813,25 @@
         request = pts20201020_models.SaveOpenJMeterSceneShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.open_jmeter_scene):
             request.open_jmeter_scene_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.open_jmeter_scene), 'OpenJMeterScene', 'json')
         query = {}
         query['OpenJMeterScene'] = request.open_jmeter_scene_shrink
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SaveOpenJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.SaveOpenJMeterSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1904,26 +1854,25 @@
         request: pts20201020_models.StartDebugPtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StartDebugPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StartDebugPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StartDebugPtsSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -1932,26 +1881,25 @@
         request: pts20201020_models.StartDebugPtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StartDebugPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StartDebugPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StartDebugPtsSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -1974,26 +1922,25 @@
         request: pts20201020_models.StartDebuggingJMeterSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StartDebuggingJMeterSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StartDebuggingJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StartDebuggingJMeterSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -2002,26 +1949,25 @@
         request: pts20201020_models.StartDebuggingJMeterSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StartDebuggingJMeterSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StartDebuggingJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StartDebuggingJMeterSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -2044,26 +1990,25 @@
         request: pts20201020_models.StartPtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StartPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StartPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StartPtsSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -2072,26 +2017,25 @@
         request: pts20201020_models.StartPtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StartPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StartPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StartPtsSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -2114,26 +2058,25 @@
         request: pts20201020_models.StartTestingJMeterSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StartTestingJMeterSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StartTestingJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StartTestingJMeterSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -2142,26 +2085,25 @@
         request: pts20201020_models.StartTestingJMeterSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StartTestingJMeterSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StartTestingJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StartTestingJMeterSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -2185,26 +2127,25 @@
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StopDebugPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['PlanId'] = request.plan_id
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StopDebugPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StopDebugPtsSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -2214,26 +2155,25 @@
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StopDebugPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['PlanId'] = request.plan_id
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StopDebugPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StopDebugPtsSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -2256,26 +2196,25 @@
         request: pts20201020_models.StopDebuggingJMeterSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StopDebuggingJMeterSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StopDebuggingJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StopDebuggingJMeterSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -2284,26 +2223,25 @@
         request: pts20201020_models.StopDebuggingJMeterSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StopDebuggingJMeterSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StopDebuggingJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StopDebuggingJMeterSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -2326,26 +2264,25 @@
         request: pts20201020_models.StopPtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StopPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StopPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StopPtsSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -2354,26 +2291,25 @@
         request: pts20201020_models.StopPtsSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StopPtsSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StopPtsScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StopPtsSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -2396,26 +2332,25 @@
         request: pts20201020_models.StopTestingJMeterSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StopTestingJMeterSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StopTestingJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StopTestingJMeterSceneResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -2424,26 +2359,25 @@
         request: pts20201020_models.StopTestingJMeterSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> pts20201020_models.StopTestingJMeterSceneResponse:
         UtilClient.validate_model(request)
         query = {}
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StopTestingJMeterScene',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.StopTestingJMeterSceneResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
@@ -2474,26 +2408,25 @@
         if not UtilClient.is_unset(tmp_req.scene_baseline):
             request.scene_baseline_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.scene_baseline, 'SceneBaseline', 'json')
         query = {}
         query['ApiBaselines'] = request.api_baselines_shrink
         query['SceneBaseline'] = request.scene_baseline_shrink
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='UpdatePtsSceneBaseLine',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.UpdatePtsSceneBaseLineResponse(),
             self.call_api(params, req, runtime)
         )
 
@@ -2510,26 +2443,25 @@
         if not UtilClient.is_unset(tmp_req.scene_baseline):
             request.scene_baseline_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.scene_baseline, 'SceneBaseline', 'json')
         query = {}
         query['ApiBaselines'] = request.api_baselines_shrink
         query['SceneBaseline'] = request.scene_baseline_shrink
         query['SceneId'] = request.scene_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='UpdatePtsSceneBaseLine',
             version='2020-10-20',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             pts20201020_models.UpdatePtsSceneBaseLineResponse(),
             await self.call_api_async(params, req, runtime)
         )
```

### Comparing `alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020/models.py` & `alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1213,42 +1213,48 @@
     def __init__(
         self,
         agent_count: int = None,
         agent_id_list: List[str] = None,
         all_sample_stat: Dict[str, Any] = None,
         concurrency: int = None,
         has_report: bool = None,
+        hold_for: int = None,
         is_debugging: bool = None,
         sample_stat_list: List[Dict[str, Any]] = None,
         scene_id: str = None,
         scene_name: str = None,
         stage_name: str = None,
+        start_time_ts: int = None,
         status: str = None,
         vum: int = None,
     ):
         # 压测引擎数量
         self.agent_count = agent_count
         # 压测引擎列表
         self.agent_id_list = agent_id_list
         # 场景整体的采样状态
         self.all_sample_stat = all_sample_stat
         # 并发量
         self.concurrency = concurrency
         # 是否生成了报告
         self.has_report = has_report
+        # 压测计划持续时间，单位s
+        self.hold_for = hold_for
         # 是否是调试
         self.is_debugging = is_debugging
         # 每一个采样器的状态
         self.sample_stat_list = sample_stat_list
         # 场景id
         self.scene_id = scene_id
         # 场景名称
         self.scene_name = scene_name
         # 当前所处阶段
         self.stage_name = stage_name
+        # 压测计划开始时间戳，单位ms
+        self.start_time_ts = start_time_ts
         # 状态
         self.status = status
         # 目前消耗的vum
         self.vum = vum
 
     def validate(self):
         pass
@@ -1265,24 +1271,28 @@
             result['AgentIdList'] = self.agent_id_list
         if self.all_sample_stat is not None:
             result['AllSampleStat'] = self.all_sample_stat
         if self.concurrency is not None:
             result['Concurrency'] = self.concurrency
         if self.has_report is not None:
             result['HasReport'] = self.has_report
+        if self.hold_for is not None:
+            result['HoldFor'] = self.hold_for
         if self.is_debugging is not None:
             result['IsDebugging'] = self.is_debugging
         if self.sample_stat_list is not None:
             result['SampleStatList'] = self.sample_stat_list
         if self.scene_id is not None:
             result['SceneId'] = self.scene_id
         if self.scene_name is not None:
             result['SceneName'] = self.scene_name
         if self.stage_name is not None:
             result['StageName'] = self.stage_name
+        if self.start_time_ts is not None:
+            result['StartTimeTS'] = self.start_time_ts
         if self.status is not None:
             result['Status'] = self.status
         if self.vum is not None:
             result['Vum'] = self.vum
         return result
 
     def from_map(self, m: dict = None):
@@ -1293,24 +1303,28 @@
             self.agent_id_list = m.get('AgentIdList')
         if m.get('AllSampleStat') is not None:
             self.all_sample_stat = m.get('AllSampleStat')
         if m.get('Concurrency') is not None:
             self.concurrency = m.get('Concurrency')
         if m.get('HasReport') is not None:
             self.has_report = m.get('HasReport')
+        if m.get('HoldFor') is not None:
+            self.hold_for = m.get('HoldFor')
         if m.get('IsDebugging') is not None:
             self.is_debugging = m.get('IsDebugging')
         if m.get('SampleStatList') is not None:
             self.sample_stat_list = m.get('SampleStatList')
         if m.get('SceneId') is not None:
             self.scene_id = m.get('SceneId')
         if m.get('SceneName') is not None:
             self.scene_name = m.get('SceneName')
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
+        if m.get('StartTimeTS') is not None:
+            self.start_time_ts = m.get('StartTimeTS')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('Vum') is not None:
             self.vum = m.get('Vum')
         return self
 
 
@@ -6619,25 +6633,22 @@
 
 class SaveEnvRequestEnv(TeaModel):
     def __init__(
         self,
         env_id: str = None,
         env_name: str = None,
         files: List[SaveEnvRequestEnvFiles] = None,
-        jmeter_plugin_label: str = None,
         properties: List[SaveEnvRequestEnvProperties] = None,
     ):
         # 环境id，不填表示新建环境，填了表示修改该环境
         self.env_id = env_id
         # 环境名称
         self.env_name = env_name
         # 环境依赖的文件
         self.files = files
-        # jmeter插件的环境标签
-        self.jmeter_plugin_label = jmeter_plugin_label
         # jmeter属性
         self.properties = properties
 
     def validate(self):
         if self.files:
             for k in self.files:
                 if k:
@@ -6657,16 +6668,14 @@
             result['EnvId'] = self.env_id
         if self.env_name is not None:
             result['EnvName'] = self.env_name
         result['Files'] = []
         if self.files is not None:
             for k in self.files:
                 result['Files'].append(k.to_map() if k else None)
-        if self.jmeter_plugin_label is not None:
-            result['JmeterPluginLabel'] = self.jmeter_plugin_label
         result['Properties'] = []
         if self.properties is not None:
             for k in self.properties:
                 result['Properties'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
@@ -6676,16 +6685,14 @@
         if m.get('EnvName') is not None:
             self.env_name = m.get('EnvName')
         self.files = []
         if m.get('Files') is not None:
             for k in m.get('Files'):
                 temp_model = SaveEnvRequestEnvFiles()
                 self.files.append(temp_model.from_map(k))
-        if m.get('JmeterPluginLabel') is not None:
-            self.jmeter_plugin_label = m.get('JmeterPluginLabel')
         self.properties = []
         if m.get('Properties') is not None:
             for k in m.get('Properties'):
                 temp_model = SaveEnvRequestEnvProperties()
                 self.properties.append(temp_model.from_map(k))
         return self
 
@@ -6993,15 +7000,14 @@
         constant_throughput_timer_type: str = None,
         dns_cache_config: SaveOpenJMeterSceneRequestOpenJMeterSceneDnsCacheConfig = None,
         duration: int = None,
         environment_id: str = None,
         file_list: List[SaveOpenJMeterSceneRequestOpenJMeterSceneFileList] = None,
         is_vpc_test: bool = None,
         jmeter_properties: List[SaveOpenJMeterSceneRequestOpenJMeterSceneJMeterProperties] = None,
-        jmeter_plugin_label: str = None,
         ramp_up: int = None,
         region_id: str = None,
         scene_id: str = None,
         scene_name: str = None,
         security_group_id: str = None,
         steps: int = None,
         sync_timer_type: str = None,
@@ -7023,16 +7029,14 @@
         self.environment_id = environment_id
         # 文件列表
         self.file_list = file_list
         # 是否为VPC测试，默认为false表示公网测试，此值为true时VPC相关配置才生效
         self.is_vpc_test = is_vpc_test
         # Jmeter属性
         self.jmeter_properties = jmeter_properties
-        # jmeter插件的环境标签
-        self.jmeter_plugin_label = jmeter_plugin_label
         # 预热时间
         self.ramp_up = ramp_up
         # region的id，VPC压测时配置
         self.region_id = region_id
         # 场景ID
         self.scene_id = scene_id
         # 场景名
@@ -7086,16 +7090,14 @@
                 result['FileList'].append(k.to_map() if k else None)
         if self.is_vpc_test is not None:
             result['IsVpcTest'] = self.is_vpc_test
         result['JMeterProperties'] = []
         if self.jmeter_properties is not None:
             for k in self.jmeter_properties:
                 result['JMeterProperties'].append(k.to_map() if k else None)
-        if self.jmeter_plugin_label is not None:
-            result['JmeterPluginLabel'] = self.jmeter_plugin_label
         if self.ramp_up is not None:
             result['RampUp'] = self.ramp_up
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.scene_id is not None:
             result['SceneId'] = self.scene_id
         if self.scene_name is not None:
@@ -7137,16 +7139,14 @@
         if m.get('IsVpcTest') is not None:
             self.is_vpc_test = m.get('IsVpcTest')
         self.jmeter_properties = []
         if m.get('JMeterProperties') is not None:
             for k in m.get('JMeterProperties'):
                 temp_model = SaveOpenJMeterSceneRequestOpenJMeterSceneJMeterProperties()
                 self.jmeter_properties.append(temp_model.from_map(k))
-        if m.get('JmeterPluginLabel') is not None:
-            self.jmeter_plugin_label = m.get('JmeterPluginLabel')
         if m.get('RampUp') is not None:
             self.ramp_up = m.get('RampUp')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('SceneId') is not None:
             self.scene_id = m.get('SceneId')
         if m.get('SceneName') is not None:
```

### Comparing `alibabacloud_pts20201020-1.8.6/alibabacloud_pts20201020.egg-info/PKG-INFO` & `alibabacloud_pts20201020-1.8.7/alibabacloud_pts20201020.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pts20201020
-Version: 1.8.6
+Version: 1.8.7
 Summary: Alibaba Cloud Performance Testing (20201020) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pts20201020-1.8.6/setup.py` & `alibabacloud_pts20201020-1.8.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pts20201020.
 
-Created on 07/12/2021
+Created on 20/12/2021
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pts20201020"
 NAME = "alibabacloud_pts20201020" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Performance Testing (20201020) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.5, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.0, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.5, <1.0.0",
+    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

