# Comparing `tmp/drf-api-tracking-1.8.0.tar.gz` & `tmp/drf-api-tracking-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-api-tracking-1.8.0.tar", last modified: Sun May  2 09:28:06 2021, max compression
+gzip compressed data, was "drf-api-tracking-1.8.2.tar", last modified: Thu May 11 19:07:17 2023, max compression
```

## Comparing `drf-api-tracking-1.8.0.tar` & `drf-api-tracking-1.8.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    12265 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     9092 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/rest_framework_tracking/
--rw-rw-r--   0 travis    (2000) travis    (2000)      916 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/app_settings.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/rest_framework_tracking/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/rest_framework_tracking/templates/admin/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/rest_framework_tracking/templates/admin/rest_framework_tracking/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4784 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1799 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/base_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8334 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/base_mixins.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)      409 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0003_add_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      549 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0009_view_method_max_length_200.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      745 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      698 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0005_auto_20171219_1537.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      986 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0010_auto_20200609_1404.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      521 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0008_auto_20200201_2048.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      438 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0004_add_verbose_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      702 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0006_auto_20180315_1442.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      749 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0002_auto_20170118_1713.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      449 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0011_auto_20201117_2016.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      335 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0007_merge_20180419_1646.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       94 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2934 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/admin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      472 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/mixins.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      188 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/managers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/rest_framework_tracking/management/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/rest_framework_tracking/management/commands/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/rest_framework_tracking/management/commands/clearapilogs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      753 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/drf_api_tracking.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12265 2021-05-02 09:28:05.000000 drf-api-tracking-1.8.0/drf_api_tracking.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-05-02 09:28:05.000000 drf-api-tracking-1.8.0/drf_api_tracking.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2021-05-02 09:28:05.000000 drf-api-tracking-1.8.0/drf_api_tracking.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1515 2021-05-02 09:28:06.000000 drf-api-tracking-1.8.0/drf_api_tracking.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2021-05-02 09:28:05.000000 drf-api-tracking-1.8.0/drf_api_tracking.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3625 2021-05-02 09:27:03.000000 drf-api-tracking-1.8.0/setup.py
+drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.519522 drf-api-tracking-1.8.2/
+-rw-rw-r--   0 ling      (1000) ling      (1000)       61 2020-02-21 11:51:40.000000 drf-api-tracking-1.8.2/MANIFEST.in
+-rw-r--r--   0 ling      (1000) ling      (1000)    12265 2023-05-11 19:07:17.519522 drf-api-tracking-1.8.2/PKG-INFO
+-rw-r--r--   0 ling      (1000) ling      (1000)     9092 2023-05-11 19:05:54.000000 drf-api-tracking-1.8.2/README.md
+drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.516188 drf-api-tracking-1.8.2/drf_api_tracking.egg-info/
+-rw-rw-r--   0 ling      (1000) ling      (1000)    12265 2023-05-11 19:07:17.000000 drf-api-tracking-1.8.2/drf_api_tracking.egg-info/PKG-INFO
+-rw-rw-r--   0 ling      (1000) ling      (1000)     1522 2023-05-11 19:07:17.000000 drf-api-tracking-1.8.2/drf_api_tracking.egg-info/SOURCES.txt
+-rw-rw-r--   0 ling      (1000) ling      (1000)        1 2023-05-11 19:07:17.000000 drf-api-tracking-1.8.2/drf_api_tracking.egg-info/dependency_links.txt
+-rw-rw-r--   0 ling      (1000) ling      (1000)       40 2023-05-11 19:07:17.000000 drf-api-tracking-1.8.2/drf_api_tracking.egg-info/requires.txt
+-rw-rw-r--   0 ling      (1000) ling      (1000)       59 2023-05-11 19:07:17.000000 drf-api-tracking-1.8.2/drf_api_tracking.egg-info/top_level.txt
+-rw-r--r--   0 ling      (1000) ling      (1000)      463 2021-05-03 10:30:46.000000 drf-api-tracking-1.8.2/pyproject.toml
+drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.516188 drf-api-tracking-1.8.2/rest_framework_tracking/
+-rw-r--r--   0 ling      (1000) ling      (1000)      149 2023-05-11 19:06:59.000000 drf-api-tracking-1.8.2/rest_framework_tracking/__init__.py
+-rw-r--r--   0 ling      (1000) ling      (1000)     2982 2023-05-11 19:05:54.000000 drf-api-tracking-1.8.2/rest_framework_tracking/admin.py
+-rw-r--r--   0 ling      (1000) ling      (1000)     1064 2023-05-11 18:58:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/app_settings.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      164 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/apps.py
+-rw-r--r--   0 ling      (1000) ling      (1000)     8359 2023-05-11 19:05:54.000000 drf-api-tracking-1.8.2/rest_framework_tracking/base_mixins.py
+-rw-r--r--   0 ling      (1000) ling      (1000)     1851 2023-05-11 19:05:54.000000 drf-api-tracking-1.8.2/rest_framework_tracking/base_models.py
+drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.516188 drf-api-tracking-1.8.2/rest_framework_tracking/management/
+drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.519522 drf-api-tracking-1.8.2/rest_framework_tracking/management/commands/
+-rw-r--r--   0 ling      (1000) ling      (1000)     1238 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/management/commands/clearapilogs.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      188 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/managers.py
+drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.519522 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/
+-rw-r--r--   0 ling      (1000) ling      (1000)     1886 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0001_initial.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      749 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0002_auto_20170118_1713.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      409 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0003_add_errors.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      438 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0004_add_verbose_name.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      698 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0005_auto_20171219_1537.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      702 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0006_auto_20180315_1442.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      745 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      335 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0007_merge_20180419_1646.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      521 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0008_auto_20200201_2048.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      549 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0009_view_method_max_length_200.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      986 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0010_auto_20200609_1404.py
+-rw-r--r--   0 ling      (1000) ling      (1000)      449 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0011_auto_20201117_2016.py
+-rw-rw-r--   0 ling      (1000) ling      (1000)        0 2020-02-21 11:51:40.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/__init__.py
+-rw-rw-r--   0 ling      (1000) ling      (1000)      472 2020-02-21 11:51:40.000000 drf-api-tracking-1.8.2/rest_framework_tracking/mixins.py
+-rw-rw-r--   0 ling      (1000) ling      (1000)       94 2020-02-21 11:51:40.000000 drf-api-tracking-1.8.2/rest_framework_tracking/models.py
+drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.516188 drf-api-tracking-1.8.2/rest_framework_tracking/templates/
+drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.516188 drf-api-tracking-1.8.2/rest_framework_tracking/templates/admin/
+drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.516188 drf-api-tracking-1.8.2/rest_framework_tracking/templates/admin/rest_framework_tracking/
+drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.519522 drf-api-tracking-1.8.2/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/
+-rw-r--r--   0 ling      (1000) ling      (1000)     4699 2023-05-11 19:05:54.000000 drf-api-tracking-1.8.2/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html
+-rw-rw-r--   0 ling      (1000) ling      (1000)       61 2023-05-11 19:07:17.519522 drf-api-tracking-1.8.2/setup.cfg
+-rw-r--r--   0 ling      (1000) ling      (1000)     3625 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `drf-api-tracking-1.8.0/PKG-INFO` & `drf-api-tracking-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-api-tracking
-Version: 1.8.0
+Version: 1.8.2
 Summary: Utils to log Django Rest Framework requests to the database
 Home-page: https://github.com/lingster/drf-api-tracking
 Author: Anna Schneider
 Author-email: anna@WattTime.org
 License: BSD
 Description: # drf-api-tracking
         
@@ -149,15 +149,15 @@
                 """
                 Save only very slow requests. Requests that took more than a second.
                 """
                 if self.log['response_ms'] > 1000:
                     super(MockCustomLogHandlerView, self).handle_log()
         ```
         
-        If your endpoint accepts large file uploads, drf-api-tracking's default behavior to decode the request body may cause a `RequestDataTooBig` exception. This behavior can be disabled globally by setting `DRF_TRACKING_DECODE_REQUEST_BODY = FALSE` in your `settings.py`file.
+        If your endpoint accepts large file uploads, drf-api-tracking's default behavior to decode the request body may cause a `RequestDataTooBig` exception. This behavior can be disabled globally by setting `DRF_TRACKING_DECODE_REQUEST_BODY = False` in your `settings.py`file.
         
         You can also customize this behavior for individual views by setting the `decode_request_body` attribute:
         
         ``` python
         class LoggingView(LoggingMixin, generics.GenericAPIView):
             decode_request_body = False
         ```
```

### Comparing `drf-api-tracking-1.8.0/README.md` & `drf-api-tracking-1.8.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         """
         Save only very slow requests. Requests that took more than a second.
         """
         if self.log['response_ms'] > 1000:
             super(MockCustomLogHandlerView, self).handle_log()
 ```
 
-If your endpoint accepts large file uploads, drf-api-tracking's default behavior to decode the request body may cause a `RequestDataTooBig` exception. This behavior can be disabled globally by setting `DRF_TRACKING_DECODE_REQUEST_BODY = FALSE` in your `settings.py`file.
+If your endpoint accepts large file uploads, drf-api-tracking's default behavior to decode the request body may cause a `RequestDataTooBig` exception. This behavior can be disabled globally by setting `DRF_TRACKING_DECODE_REQUEST_BODY = False` in your `settings.py`file.
 
 You can also customize this behavior for individual views by setting the `decode_request_body` attribute:
 
 ``` python
 class LoggingView(LoggingMixin, generics.GenericAPIView):
     decode_request_body = False
 ```
```

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/app_settings.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/app_settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,9 +23,14 @@
         return self._setting("DECODE_REQUEST_BODY", True)
 
     @property
     def PATH_LENGTH(self):
         """Maximum length of request path to log"""
         return self._setting("PATH_LENGTH", 200)
 
+    @property
+    def LOOKUP_FIELD(self):
+        """Field to identify user in User model"""
+        return self._setting("LOOKUP_FIELD", 'email')
+
 
 app_settings = AppSettings("DRF_TRACKING_")
```

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html` & `drf-api-tracking-1.8.2/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,14 @@
                                 day: 'MMM D',
                             },
                         },
                     }, ],
                     yAxes: [{
                         ticks: {
                             beginAtZero: true,
-                            stepSize: 1,
-                            suggestedMax: 5,
                         },
                     }, ],
                 },
             },
         });
 
         function onDateChange(newStart, newEnd) {
@@ -118,8 +116,8 @@
 </div>
 <!-- Render the chart -->
 <div style="width: 80%;">
     <canvas style="margin-bottom: 30px; width: 60%; height: 50%;" id="chart"></canvas>
 </div>
 <!-- Render the rest of the ChangeList view -->
 {{ block.super }}
-{% endblock %}
+{% endblock %}
```

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/base_models.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/base_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,20 +37,21 @@
         null=True,
         blank=True,
         db_index=True,
     )
     remote_addr = models.GenericIPAddressField()
     host = models.URLField()
     method = models.CharField(max_length=10)
+    user_agent = models.CharField(max_length=255, blank=True)
     query_params = models.TextField(null=True, blank=True)
     data = models.TextField(null=True, blank=True)
     response = models.TextField(null=True, blank=True)
     errors = models.TextField(null=True, blank=True)
     status_code = models.PositiveIntegerField(null=True, blank=True, db_index=True)
     objects = PrefetchUserManager()
 
     class Meta:
         abstract = True
         verbose_name = "API Request Log"
 
     def __str__(self):
-        return "{} {}".format(self.method, self.path)
+        return f"{self.method} {self.path}"
```

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/base_mixins.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/base_mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,21 @@
         assert isinstance(
             self.CLEANED_SUBSTITUTE, str
         ), "CLEANED_SUBSTITUTE must be a string."
         super(BaseLoggingMixin, self).__init__(*args, **kwargs)
 
     def initial(self, request, *args, **kwargs):
         self.log = {"requested_at": now()}
-        if not getattr(self, "decode_request_body", app_settings.DECODE_REQUEST_BODY):
-            self.log["data"] = ""
-        else:
-            self.log["data"] = self._clean_data(request.body)
+        self.log["data"] = (
+            self._clean_data(request.body)
+            if getattr(
+                self, "decode_request_body", app_settings.DECODE_REQUEST_BODY
+            )
+            else ""
+        )
 
         super(BaseLoggingMixin, self).initial(request, *args, **kwargs)
 
         try:
             # Accessing request.data *for the first time* parses the request body, which may raise
             # ParseError and UnsupportedMediaType exceptions. It's important not to swallow these,
             # as (depending on implementation details) they may only get raised this once, and
@@ -69,27 +72,28 @@
             if response.streaming:
                 rendered_content = None
             elif hasattr(response, "rendered_content"):
                 rendered_content = response.rendered_content
             else:
                 rendered_content = response.getvalue()
 
+            user = self._get_user(request)
+
             self.log.update(
                 {
                     "remote_addr": self._get_ip_address(request),
                     "view": self._get_view_name(request),
                     "view_method": self._get_view_method(request),
                     "path": self._get_path(request),
                     "host": request.get_host(),
+                    "user_agent": request.META.get("HTTP_USER_AGENT", ""),
                     "method": request.method,
                     "query_params": self._clean_data(request.query_params.dict()),
-                    "user": self._get_user(request),
-                    "username_persistent": self._get_user(request).get_username()
-                    if self._get_user(request)
-                    else "Anonymous",
+                    "user": user,
+                    "username_persistent": user.get_username() if user else "Anonymous",
                     "response_ms": self._get_response_ms(),
                     "response": self._clean_data(rendered_content),
                     "status_code": response.status_code,
                 }
             )
             if self._clean_data(request.query_params.dict()) == {}:
                 self.log.update({"query_params": self.log["data"]})
@@ -115,15 +119,15 @@
 
     def _get_ip_address(self, request):
         """Get the remote ip address the request was generated from."""
         ipaddr = request.META.get("HTTP_X_FORWARDED_FOR", None)
         if ipaddr:
             ipaddr = ipaddr.split(",")[0]
         else:
-            ipaddr = request.META.get("REMOTE_ADDR", "")
+            ipaddr = request.META.get("REMOTE_ADDR", "").split(",")[0]
 
         # Account for IPv4 and IPv6 addresses, each possibly with port appended. Possibilities are:
         # <ipv4 address>
         # <ipv6 address>
         # <ipv4 address>:port
         # [<ipv6 address>]:port
         # Note that ipv6 addresses are colon separated hex numbers
@@ -138,17 +142,16 @@
         return ipaddr
 
     def _get_view_name(self, request):
         """Get view name."""
         method = request.method.lower()
         try:
             attributes = getattr(self, method)
-            return (
-                type(attributes.__self__).__module__ + "." + type(attributes.__self__).__name__
-            )
+            return f"{type(attributes.__self__).__module__}.{type(attributes.__self__).__name__}"
+
 
         except AttributeError:
             return None
 
     def _get_view_method(self, request):
         """Get view method."""
         if hasattr(self, "action"):
```

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0009_view_method_max_length_200.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0009_view_method_max_length_200.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0005_auto_20171219_1537.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0005_auto_20171219_1537.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0001_initial.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0010_auto_20200609_1404.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0010_auto_20200609_1404.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0008_auto_20200201_2048.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0008_auto_20200201_2048.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0006_auto_20180315_1442.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0006_auto_20180315_1442.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/migrations/0002_auto_20170118_1713.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0002_auto_20170118_1713.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/admin.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         "host",
         "query_params",
     )
     ordering = ("-requested_at",)
     list_filter = ("view_method", "status_code")
     search_fields = (
         "path",
-        "user__email",
+        f"user__{app_settings.LOOKUP_FIELD}",
     )
     raw_id_fields = ("user",)
 
     if app_settings.ADMIN_LOG_READONLY:
         readonly_fields = (
             "user",
             "username_persistent",
@@ -45,14 +45,15 @@
             "host",
             "method",
             "query_params",
             "data",
             "response",
             "errors",
             "status_code",
+            "user_agent"
         )
 
     def changelist_view(self, request, extra_context=None):
         # Aggregate api logs per day
         chart_data = (
             APIRequestLog.objects.annotate(date=TruncDay("requested_at"))
             .values("date")
```

### Comparing `drf-api-tracking-1.8.0/rest_framework_tracking/management/commands/clearapilogs.py` & `drf-api-tracking-1.8.2/rest_framework_tracking/management/commands/clearapilogs.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.0/drf_api_tracking.egg-info/PKG-INFO` & `drf-api-tracking-1.8.2/drf_api_tracking.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-api-tracking
-Version: 1.8.0
+Version: 1.8.2
 Summary: Utils to log Django Rest Framework requests to the database
 Home-page: https://github.com/lingster/drf-api-tracking
 Author: Anna Schneider
 Author-email: anna@WattTime.org
 License: BSD
 Description: # drf-api-tracking
         
@@ -149,15 +149,15 @@
                 """
                 Save only very slow requests. Requests that took more than a second.
                 """
                 if self.log['response_ms'] > 1000:
                     super(MockCustomLogHandlerView, self).handle_log()
         ```
         
-        If your endpoint accepts large file uploads, drf-api-tracking's default behavior to decode the request body may cause a `RequestDataTooBig` exception. This behavior can be disabled globally by setting `DRF_TRACKING_DECODE_REQUEST_BODY = FALSE` in your `settings.py`file.
+        If your endpoint accepts large file uploads, drf-api-tracking's default behavior to decode the request body may cause a `RequestDataTooBig` exception. This behavior can be disabled globally by setting `DRF_TRACKING_DECODE_REQUEST_BODY = False` in your `settings.py`file.
         
         You can also customize this behavior for individual views by setting the `decode_request_body` attribute:
         
         ``` python
         class LoggingView(LoggingMixin, generics.GenericAPIView):
             decode_request_body = False
         ```
```

### Comparing `drf-api-tracking-1.8.0/drf_api_tracking.egg-info/SOURCES.txt` & `drf-api-tracking-1.8.2/drf_api_tracking.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 drf_api_tracking.egg-info/PKG-INFO
 drf_api_tracking.egg-info/SOURCES.txt
 drf_api_tracking.egg-info/dependency_links.txt
 drf_api_tracking.egg-info/requires.txt
 drf_api_tracking.egg-info/top_level.txt
```

### Comparing `drf-api-tracking-1.8.0/setup.py` & `drf-api-tracking-1.8.2/setup.py`

 * *Files identical despite different names*

