# Comparing `tmp/alibabacloud_pts20201020_py2-1.8.6.tar.gz` & `tmp/alibabacloud_pts20201020_py2-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pts20201020_py2-1.8.6.tar", last modified: Tue Dec  7 03:27:16 2021, max compression
+gzip compressed data, was "dist/alibabacloud_pts20201020_py2-1.8.7.tar", last modified: Mon Dec 20 06:04:06 2021, max compression
```

## Comparing `alibabacloud_pts20201020_py2-1.8.6.tar` & `alibabacloud_pts20201020_py2-1.8.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)       25 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2448 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      175 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      588 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1116 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/README.md
--rw-r--r--   0 root         (0) root         (0)     2448 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       28 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020/
--rw-r--r--   0 root         (0) root         (0)    37968 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020/client.py
--rw-r--r--   0 root         (0) root         (0)   277906 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020/models.py
--rw-r--r--   0 root         (0) root         (0)       21 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1033 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2919 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/setup.py
--rw-r--r--   0 root         (0) root         (0)       94 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      271 2021-12-07 03:27:16.000000 alibabacloud_pts20201020_py2-1.8.6/ChangeLog.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-20 06:04:06.000000 alibabacloud_pts20201020_py2-1.8.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-20 06:04:06.000000 alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       25 2021-12-20 06:04:06.000000 alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2448 2021-12-20 06:04:06.000000 alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2021-12-20 06:04:06.000000 alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-20 06:04:06.000000 alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      175 2021-12-20 06:04:06.000000 alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      588 2021-12-20 06:04:05.000000 alibabacloud_pts20201020_py2-1.8.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1116 2021-12-20 06:04:05.000000 alibabacloud_pts20201020_py2-1.8.7/README.md
+-rw-r--r--   0 root         (0) root         (0)     2448 2021-12-20 06:04:06.000000 alibabacloud_pts20201020_py2-1.8.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       28 2021-12-20 06:04:05.000000 alibabacloud_pts20201020_py2-1.8.7/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-20 06:04:06.000000 alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020/
+-rw-r--r--   0 root         (0) root         (0)    36574 2021-12-20 06:04:05.000000 alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020/client.py
+-rw-r--r--   0 root         (0) root         (0)   277775 2021-12-20 06:04:05.000000 alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020/models.py
+-rw-r--r--   0 root         (0) root         (0)       21 2021-12-20 06:04:05.000000 alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2021-12-20 06:04:05.000000 alibabacloud_pts20201020_py2-1.8.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2919 2021-12-20 06:04:05.000000 alibabacloud_pts20201020_py2-1.8.7/setup.py
+-rw-r--r--   0 root         (0) root         (0)       94 2021-12-20 06:04:06.000000 alibabacloud_pts20201020_py2-1.8.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      331 2021-12-20 06:04:05.000000 alibabacloud_pts20201020_py2-1.8.7/ChangeLog.md
```

### Comparing `alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020_py2.egg-info/PKG-INFO` & `alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alibabacloud-pts20201020-py2
-Version: 1.8.6
+Version: 1.8.7
 Summary: Alibaba Cloud Performance Testing (20201020) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pts20201020_py2-1.8.6/LICENSE` & `alibabacloud_pts20201020_py2-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pts20201020_py2-1.8.6/README.md` & `alibabacloud_pts20201020_py2-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pts20201020_py2-1.8.6/PKG-INFO` & `alibabacloud_pts20201020_py2-1.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alibabacloud_pts20201020_py2
-Version: 1.8.6
+Version: 1.8.7
 Summary: Alibaba Cloud Performance Testing (20201020) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020/client.py` & `alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,26 +31,25 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def create_pts_scene_with_options(self, request, runtime):
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
 
@@ -60,26 +59,25 @@
 
     def create_pts_scene_base_line_from_report_with_options(self, request, runtime):
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
 
@@ -88,26 +86,25 @@
         return self.create_pts_scene_base_line_from_report_with_options(request, runtime)
 
     def delete_pts_scene_with_options(self, request, runtime):
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
 
@@ -116,26 +113,25 @@
         return self.delete_pts_scene_with_options(request, runtime)
 
     def delete_pts_scene_base_line_with_options(self, request, runtime):
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
 
@@ -148,26 +144,25 @@
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
 
@@ -184,26 +179,25 @@
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
 
@@ -215,26 +209,25 @@
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
 
@@ -255,26 +248,25 @@
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
 
@@ -283,26 +275,25 @@
         return self.get_jmeter_sampling_logs_with_options(request, runtime)
 
     def get_jmeter_scene_running_data_with_options(self, request, runtime):
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
 
@@ -311,26 +302,25 @@
         return self.get_jmeter_scene_running_data_with_options(request, runtime)
 
     def get_open_jmeter_scene_with_options(self, request, runtime):
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
 
@@ -340,26 +330,25 @@
 
     def get_pts_report_details_with_options(self, request, runtime):
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
 
@@ -370,26 +359,25 @@
     def get_pts_reports_by_scene_id_with_options(self, request, runtime):
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
 
@@ -398,26 +386,25 @@
         return self.get_pts_reports_by_scene_id_with_options(request, runtime)
 
     def get_pts_scene_with_options(self, request, runtime):
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
 
@@ -426,26 +413,25 @@
         return self.get_pts_scene_with_options(request, runtime)
 
     def get_pts_scene_base_line_with_options(self, request, runtime):
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
 
@@ -455,26 +441,25 @@
 
     def get_pts_scene_running_data_with_options(self, request, runtime):
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
 
@@ -483,26 +468,25 @@
         return self.get_pts_scene_running_data_with_options(request, runtime)
 
     def get_pts_scene_running_status_with_options(self, request, runtime):
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
 
@@ -514,26 +498,25 @@
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
 
@@ -548,26 +531,25 @@
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
 
@@ -579,26 +561,25 @@
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
 
@@ -609,26 +590,25 @@
     def list_pts_scene_with_options(self, request, runtime):
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
 
@@ -637,26 +617,25 @@
         return self.list_pts_scene_with_options(request, runtime)
 
     def modify_pts_scene_with_options(self, request, runtime):
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
 
@@ -665,26 +644,25 @@
         return self.modify_pts_scene_with_options(request, runtime)
 
     def remove_env_with_options(self, request, runtime):
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
 
@@ -693,26 +671,25 @@
         return self.remove_env_with_options(request, runtime)
 
     def remove_open_jmeter_scene_with_options(self, request, runtime):
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
 
@@ -725,26 +702,25 @@
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
 
@@ -757,26 +733,25 @@
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
 
@@ -785,26 +760,25 @@
         return self.save_open_jmeter_scene_with_options(request, runtime)
 
     def start_debug_pts_scene_with_options(self, request, runtime):
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
 
@@ -813,26 +787,25 @@
         return self.start_debug_pts_scene_with_options(request, runtime)
 
     def start_debugging_jmeter_scene_with_options(self, request, runtime):
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
 
@@ -841,26 +814,25 @@
         return self.start_debugging_jmeter_scene_with_options(request, runtime)
 
     def start_pts_scene_with_options(self, request, runtime):
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
 
@@ -869,26 +841,25 @@
         return self.start_pts_scene_with_options(request, runtime)
 
     def start_testing_jmeter_scene_with_options(self, request, runtime):
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
 
@@ -898,26 +869,25 @@
 
     def stop_debug_pts_scene_with_options(self, request, runtime):
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
 
@@ -926,26 +896,25 @@
         return self.stop_debug_pts_scene_with_options(request, runtime)
 
     def stop_debugging_jmeter_scene_with_options(self, request, runtime):
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
 
@@ -954,26 +923,25 @@
         return self.stop_debugging_jmeter_scene_with_options(request, runtime)
 
     def stop_pts_scene_with_options(self, request, runtime):
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
 
@@ -982,26 +950,25 @@
         return self.stop_pts_scene_with_options(request, runtime)
 
     def stop_testing_jmeter_scene_with_options(self, request, runtime):
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
 
@@ -1018,26 +985,25 @@
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
```

### Comparing `alibabacloud_pts20201020_py2-1.8.6/alibabacloud_pts20201020/models.py` & `alibabacloud_pts20201020_py2-1.8.7/alibabacloud_pts20201020/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1060,36 +1060,40 @@
         if m.get('SceneId') is not None:
             self.scene_id = m.get('SceneId')
         return self
 
 
 class GetJMeterSceneRunningDataResponseBodyRunningData(TeaModel):
     def __init__(self, agent_count=None, agent_id_list=None, all_sample_stat=None, concurrency=None,
-                 has_report=None, is_debugging=None, sample_stat_list=None, scene_id=None, scene_name=None, stage_name=None,
-                 status=None, vum=None):
+                 has_report=None, hold_for=None, is_debugging=None, sample_stat_list=None, scene_id=None, scene_name=None,
+                 stage_name=None, start_time_ts=None, status=None, vum=None):
         # 压测引擎数量
         self.agent_count = agent_count  # type: int
         # 压测引擎列表
         self.agent_id_list = agent_id_list  # type: list[str]
         # 场景整体的采样状态
         self.all_sample_stat = all_sample_stat  # type: dict[str, any]
         # 并发量
         self.concurrency = concurrency  # type: int
         # 是否生成了报告
         self.has_report = has_report  # type: bool
+        # 压测计划持续时间，单位s
+        self.hold_for = hold_for  # type: int
         # 是否是调试
         self.is_debugging = is_debugging  # type: bool
         # 每一个采样器的状态
         self.sample_stat_list = sample_stat_list  # type: list[dict[str, any]]
         # 场景id
         self.scene_id = scene_id  # type: str
         # 场景名称
         self.scene_name = scene_name  # type: str
         # 当前所处阶段
         self.stage_name = stage_name  # type: str
+        # 压测计划开始时间戳，单位ms
+        self.start_time_ts = start_time_ts  # type: long
         # 状态
         self.status = status  # type: str
         # 目前消耗的vum
         self.vum = vum  # type: long
 
     def validate(self):
         pass
@@ -1106,24 +1110,28 @@
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
 
     def from_map(self, m=None):
@@ -1134,24 +1142,28 @@
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
 
 
@@ -5838,23 +5850,21 @@
             self.name = m.get('Name')
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class SaveEnvRequestEnv(TeaModel):
-    def __init__(self, env_id=None, env_name=None, files=None, jmeter_plugin_label=None, properties=None):
+    def __init__(self, env_id=None, env_name=None, files=None, properties=None):
         # 环境id，不填表示新建环境，填了表示修改该环境
         self.env_id = env_id  # type: str
         # 环境名称
         self.env_name = env_name  # type: str
         # 环境依赖的文件
         self.files = files  # type: list[SaveEnvRequestEnvFiles]
-        # jmeter插件的环境标签
-        self.jmeter_plugin_label = jmeter_plugin_label  # type: str
         # jmeter属性
         self.properties = properties  # type: list[SaveEnvRequestEnvProperties]
 
     def validate(self):
         if self.files:
             for k in self.files:
                 if k:
@@ -5874,16 +5884,14 @@
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
 
     def from_map(self, m=None):
@@ -5893,16 +5901,14 @@
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
 
@@ -6166,16 +6172,16 @@
             self.value = m.get('Value')
         return self
 
 
 class SaveOpenJMeterSceneRequestOpenJMeterScene(TeaModel):
     def __init__(self, agent_count=None, concurrency=None, constant_throughput_timer_type=None,
                  dns_cache_config=None, duration=None, environment_id=None, file_list=None, is_vpc_test=None, jmeter_properties=None,
-                 jmeter_plugin_label=None, ramp_up=None, region_id=None, scene_id=None, scene_name=None, security_group_id=None,
-                 steps=None, sync_timer_type=None, test_file=None, v_switch_id=None, vpc_id=None):
+                 ramp_up=None, region_id=None, scene_id=None, scene_name=None, security_group_id=None, steps=None,
+                 sync_timer_type=None, test_file=None, v_switch_id=None, vpc_id=None):
         # 施压引擎数量
         self.agent_count = agent_count  # type: int
         # 最大并发
         self.concurrency = concurrency  # type: int
         # constantThroughputTimerType
         self.constant_throughput_timer_type = constant_throughput_timer_type  # type: str
         # DNS配置
@@ -6186,16 +6192,14 @@
         self.environment_id = environment_id  # type: str
         # 文件列表
         self.file_list = file_list  # type: list[SaveOpenJMeterSceneRequestOpenJMeterSceneFileList]
         # 是否为VPC测试，默认为false表示公网测试，此值为true时VPC相关配置才生效
         self.is_vpc_test = is_vpc_test  # type: bool
         # Jmeter属性
         self.jmeter_properties = jmeter_properties  # type: list[SaveOpenJMeterSceneRequestOpenJMeterSceneJMeterProperties]
-        # jmeter插件的环境标签
-        self.jmeter_plugin_label = jmeter_plugin_label  # type: str
         # 预热时间
         self.ramp_up = ramp_up  # type: int
         # region的id，VPC压测时配置
         self.region_id = region_id  # type: str
         # 场景ID
         self.scene_id = scene_id  # type: str
         # 场景名
@@ -6249,16 +6253,14 @@
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
@@ -6300,16 +6302,14 @@
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

### Comparing `alibabacloud_pts20201020_py2-1.8.6/README-CN.md` & `alibabacloud_pts20201020_py2-1.8.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pts20201020_py2-1.8.6/setup.py` & `alibabacloud_pts20201020_py2-1.8.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pts20201020_py2.
 
-Created on 07/12/2021
+Created on 20/12/2021
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pts20201020"
 NAME = "alibabacloud_pts20201020_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Performance Testing (20201020) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.5, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.0, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

