# Comparing `tmp/3scale-api-0.8.0.tar.gz` & `tmp/3scale-api-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3scale-api-0.8.0.tar", last modified: Thu Feb 11 11:33:47 2021, max compression
+gzip compressed data, was "3scale-api-0.9.0.tar", last modified: Tue Mar  2 11:45:54 2021, max compression
```

## Comparing `3scale-api-0.8.0.tar` & `3scale-api-0.9.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxr-x   0 mganisin  (1000) mganisin  (1000)        0 2021-02-11 11:33:47.672348 3scale-api-0.8.0/
-drwxrwxr-x   0 mganisin  (1000) mganisin  (1000)        0 2021-02-11 11:33:47.629348 3scale-api-0.8.0/3scale_api.egg-info/
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     4649 2021-02-11 11:33:47.000000 3scale-api-0.8.0/3scale_api.egg-info/PKG-INFO
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     1707 2021-02-11 11:33:47.000000 3scale-api-0.8.0/3scale_api.egg-info/SOURCES.txt
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)        1 2021-02-11 11:33:47.000000 3scale-api-0.8.0/3scale_api.egg-info/dependency_links.txt
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)       66 2021-02-11 11:33:47.000000 3scale-api-0.8.0/3scale_api.egg-info/requires.txt
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)       21 2021-02-11 11:33:47.000000 3scale-api-0.8.0/3scale_api.egg-info/top_level.txt
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     4649 2021-02-11 11:33:47.670348 3scale-api-0.8.0/PKG-INFO
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     3147 2020-04-01 04:29:14.000000 3scale-api-0.8.0/README.md
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)       38 2021-02-11 11:33:47.672348 3scale-api-0.8.0/setup.cfg
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     1316 2019-09-13 11:26:48.000000 3scale-api-0.8.0/setup.py
-drwxrwxr-x   0 mganisin  (1000) mganisin  (1000)        0 2021-02-11 11:33:47.617348 3scale-api-0.8.0/tests/
-drwxrwxr-x   0 mganisin  (1000) mganisin  (1000)        0 2021-02-11 11:33:47.657348 3scale-api-0.8.0/tests/integration/
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)        0 2019-09-13 11:26:48.000000 3scale-api-0.8.0/tests/integration/__init__.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      945 2019-09-13 11:26:48.000000 3scale-api-0.8.0/tests/integration/asserts.py
-drwxrwxr-x   0 mganisin  (1000) mganisin  (1000)        0 2021-02-11 11:33:47.665348 3scale-api-0.8.0/tests/integration/auth/
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)        0 2020-05-19 07:48:53.000000 3scale-api-0.8.0/tests/integration/auth/__init__.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      268 2020-05-19 07:48:53.000000 3scale-api-0.8.0/tests/integration/auth/test_app_key.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      722 2020-05-19 07:48:53.000000 3scale-api-0.8.0/tests/integration/auth/test_app_key_authorization.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      596 2020-05-19 07:48:53.000000 3scale-api-0.8.0/tests/integration/auth/test_different_app_key_name.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      368 2020-05-19 07:48:53.000000 3scale-api-0.8.0/tests/integration/auth/test_different_user_key_name.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      268 2020-05-19 07:48:53.000000 3scale-api-0.8.0/tests/integration/auth/test_user_key.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)    12246 2021-02-04 13:43:45.000000 3scale-api-0.8.0/tests/integration/conftest.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      735 2020-04-01 04:29:14.000000 3scale-api-0.8.0/tests/integration/test_integration_accounts.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      250 2020-08-27 12:21:19.000000 3scale-api-0.8.0/tests/integration/test_integration_activedocs.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      819 2019-09-13 11:26:48.000000 3scale-api-0.8.0/tests/integration/test_integration_analytics.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      819 2020-05-19 07:48:11.000000 3scale-api-0.8.0/tests/integration/test_integration_api_client.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      830 2019-12-06 17:58:59.000000 3scale-api-0.8.0/tests/integration/test_integration_application.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      828 2019-09-13 11:26:48.000000 3scale-api-0.8.0/tests/integration/test_integration_application_plan.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     2946 2020-04-01 04:29:14.000000 3scale-api-0.8.0/tests/integration/test_integration_backend_mapping_rules.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     4162 2020-04-01 04:29:14.000000 3scale-api-0.8.0/tests/integration/test_integration_backend_metrics.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     1480 2020-04-01 04:29:14.000000 3scale-api-0.8.0/tests/integration/test_integration_backends.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      419 2020-05-19 07:48:53.000000 3scale-api-0.8.0/tests/integration/test_integration_custom_tenant.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      570 2019-09-13 11:26:48.000000 3scale-api-0.8.0/tests/integration/test_integration_limit.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     2634 2019-09-13 11:26:48.000000 3scale-api-0.8.0/tests/integration/test_integration_mapping_rules.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     1545 2019-09-13 11:26:48.000000 3scale-api-0.8.0/tests/integration/test_integration_methods.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     4219 2020-04-01 04:29:14.000000 3scale-api-0.8.0/tests/integration/test_integration_metrics.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      910 2019-09-13 11:26:48.000000 3scale-api-0.8.0/tests/integration/test_integration_policies.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      532 2019-09-13 11:26:48.000000 3scale-api-0.8.0/tests/integration/test_integration_pricing_rules.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     2149 2021-02-04 13:43:45.000000 3scale-api-0.8.0/tests/integration/test_integration_provider_accounts.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     3681 2020-09-11 16:21:31.000000 3scale-api-0.8.0/tests/integration/test_integration_services.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     3267 2020-08-27 12:21:19.000000 3scale-api-0.8.0/tests/integration/test_integration_webhook.py
-drwxrwxr-x   0 mganisin  (1000) mganisin  (1000)        0 2021-02-11 11:33:47.669348 3scale-api-0.8.0/threescale_api/
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)       75 2021-02-11 11:33:11.000000 3scale-api-0.8.0/threescale_api/__init__.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     2139 2020-05-19 07:48:53.000000 3scale-api-0.8.0/threescale_api/auth.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     8753 2021-02-04 13:43:45.000000 3scale-api-0.8.0/threescale_api/client.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)    16649 2020-04-22 16:17:28.000000 3scale-api-0.8.0/threescale_api/defaults.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      553 2020-10-14 19:15:00.000000 3scale-api-0.8.0/threescale_api/errors.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     1697 2020-04-22 16:17:28.000000 3scale-api-0.8.0/threescale_api/log_config.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)    41765 2021-02-11 11:30:27.000000 3scale-api-0.8.0/threescale_api/resources.py
--rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     5843 2020-09-23 13:59:45.000000 3scale-api-0.8.0/threescale_api/utils.py
+drwxrwxr-x   0 mganisin  (1000) mganisin  (1000)        0 2021-03-02 11:45:54.669386 3scale-api-0.9.0/
+drwxrwxr-x   0 mganisin  (1000) mganisin  (1000)        0 2021-03-02 11:45:54.615386 3scale-api-0.9.0/3scale_api.egg-info/
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     4649 2021-03-02 11:45:54.000000 3scale-api-0.9.0/3scale_api.egg-info/PKG-INFO
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     1760 2021-03-02 11:45:54.000000 3scale-api-0.9.0/3scale_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)        1 2021-03-02 11:45:54.000000 3scale-api-0.9.0/3scale_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)       66 2021-03-02 11:45:54.000000 3scale-api-0.9.0/3scale_api.egg-info/requires.txt
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)       21 2021-03-02 11:45:54.000000 3scale-api-0.9.0/3scale_api.egg-info/top_level.txt
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     4649 2021-03-02 11:45:54.667386 3scale-api-0.9.0/PKG-INFO
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     3147 2020-04-01 04:29:14.000000 3scale-api-0.9.0/README.md
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)       38 2021-03-02 11:45:54.669386 3scale-api-0.9.0/setup.cfg
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     1316 2019-09-13 11:26:48.000000 3scale-api-0.9.0/setup.py
+drwxrwxr-x   0 mganisin  (1000) mganisin  (1000)        0 2021-03-02 11:45:54.602386 3scale-api-0.9.0/tests/
+drwxrwxr-x   0 mganisin  (1000) mganisin  (1000)        0 2021-03-02 11:45:54.646386 3scale-api-0.9.0/tests/integration/
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)        0 2019-09-13 11:26:48.000000 3scale-api-0.9.0/tests/integration/__init__.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      945 2019-09-13 11:26:48.000000 3scale-api-0.9.0/tests/integration/asserts.py
+drwxrwxr-x   0 mganisin  (1000) mganisin  (1000)        0 2021-03-02 11:45:54.656386 3scale-api-0.9.0/tests/integration/auth/
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)        0 2020-05-19 07:48:53.000000 3scale-api-0.9.0/tests/integration/auth/__init__.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      268 2020-05-19 07:48:53.000000 3scale-api-0.9.0/tests/integration/auth/test_app_key.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      722 2020-05-19 07:48:53.000000 3scale-api-0.9.0/tests/integration/auth/test_app_key_authorization.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      596 2020-05-19 07:48:53.000000 3scale-api-0.9.0/tests/integration/auth/test_different_app_key_name.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      368 2020-05-19 07:48:53.000000 3scale-api-0.9.0/tests/integration/auth/test_different_user_key_name.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      268 2020-05-19 07:48:53.000000 3scale-api-0.9.0/tests/integration/auth/test_user_key.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)    12572 2021-03-02 11:40:14.000000 3scale-api-0.9.0/tests/integration/conftest.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      735 2020-04-01 04:29:14.000000 3scale-api-0.9.0/tests/integration/test_integration_accounts.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      250 2020-08-27 12:21:19.000000 3scale-api-0.9.0/tests/integration/test_integration_activedocs.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      819 2019-09-13 11:26:48.000000 3scale-api-0.9.0/tests/integration/test_integration_analytics.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      819 2020-05-19 07:48:11.000000 3scale-api-0.9.0/tests/integration/test_integration_api_client.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      830 2019-12-06 17:58:59.000000 3scale-api-0.9.0/tests/integration/test_integration_application.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      828 2019-09-13 11:26:48.000000 3scale-api-0.9.0/tests/integration/test_integration_application_plan.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     2946 2020-04-01 04:29:14.000000 3scale-api-0.9.0/tests/integration/test_integration_backend_mapping_rules.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     4162 2020-04-01 04:29:14.000000 3scale-api-0.9.0/tests/integration/test_integration_backend_metrics.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     1480 2020-04-01 04:29:14.000000 3scale-api-0.9.0/tests/integration/test_integration_backends.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      419 2020-05-19 07:48:53.000000 3scale-api-0.9.0/tests/integration/test_integration_custom_tenant.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      639 2021-03-02 11:40:14.000000 3scale-api-0.9.0/tests/integration/test_integration_default_client.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      570 2019-09-13 11:26:48.000000 3scale-api-0.9.0/tests/integration/test_integration_limit.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     2634 2019-09-13 11:26:48.000000 3scale-api-0.9.0/tests/integration/test_integration_mapping_rules.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     1545 2019-09-13 11:26:48.000000 3scale-api-0.9.0/tests/integration/test_integration_methods.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     4219 2020-04-01 04:29:14.000000 3scale-api-0.9.0/tests/integration/test_integration_metrics.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      910 2019-09-13 11:26:48.000000 3scale-api-0.9.0/tests/integration/test_integration_policies.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      532 2019-09-13 11:26:48.000000 3scale-api-0.9.0/tests/integration/test_integration_pricing_rules.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     2149 2021-02-04 13:43:45.000000 3scale-api-0.9.0/tests/integration/test_integration_provider_accounts.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     3681 2020-09-11 16:21:31.000000 3scale-api-0.9.0/tests/integration/test_integration_services.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     3267 2020-08-27 12:21:19.000000 3scale-api-0.9.0/tests/integration/test_integration_webhook.py
+drwxrwxr-x   0 mganisin  (1000) mganisin  (1000)        0 2021-03-02 11:45:54.666386 3scale-api-0.9.0/threescale_api/
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)       75 2021-03-02 11:45:46.000000 3scale-api-0.9.0/threescale_api/__init__.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     2139 2020-05-19 07:48:53.000000 3scale-api-0.9.0/threescale_api/auth.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     8753 2021-02-04 13:43:45.000000 3scale-api-0.9.0/threescale_api/client.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)    16649 2020-04-22 16:17:28.000000 3scale-api-0.9.0/threescale_api/defaults.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)      553 2020-10-14 19:15:00.000000 3scale-api-0.9.0/threescale_api/errors.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     1697 2020-04-22 16:17:28.000000 3scale-api-0.9.0/threescale_api/log_config.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)    41751 2021-03-02 11:40:14.000000 3scale-api-0.9.0/threescale_api/resources.py
+-rw-rw-r--   0 mganisin  (1000) mganisin  (1000)     5864 2021-03-02 11:40:14.000000 3scale-api-0.9.0/threescale_api/utils.py
```

### Comparing `3scale-api-0.8.0/3scale_api.egg-info/PKG-INFO` & `3scale-api-0.9.0/3scale_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3scale-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: 3scale API python client
 Home-page: https://github.com/pestanko/3scale-api-python
 Author: Peter Stanko
 Author-email: stanko@mail.muni.cz
 Maintainer: Peter Stanko
 License: UNKNOWN
 Description: # 3scale REST API client in Python
```

### Comparing `3scale-api-0.8.0/3scale_api.egg-info/SOURCES.txt` & `3scale-api-0.9.0/3scale_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 tests/integration/test_integration_api_client.py
 tests/integration/test_integration_application.py
 tests/integration/test_integration_application_plan.py
 tests/integration/test_integration_backend_mapping_rules.py
 tests/integration/test_integration_backend_metrics.py
 tests/integration/test_integration_backends.py
 tests/integration/test_integration_custom_tenant.py
+tests/integration/test_integration_default_client.py
 tests/integration/test_integration_limit.py
 tests/integration/test_integration_mapping_rules.py
 tests/integration/test_integration_methods.py
 tests/integration/test_integration_metrics.py
 tests/integration/test_integration_policies.py
 tests/integration/test_integration_pricing_rules.py
 tests/integration/test_integration_provider_accounts.py
```

### Comparing `3scale-api-0.8.0/PKG-INFO` & `3scale-api-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3scale-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: 3scale API python client
 Home-page: https://github.com/pestanko/3scale-api-python
 Author: Peter Stanko
 Author-email: stanko@mail.muni.cz
 Maintainer: Peter Stanko
 License: UNKNOWN
 Description: # 3scale REST API client in Python
```

### Comparing `3scale-api-0.8.0/README.md` & `3scale-api-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/setup.py` & `3scale-api-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/asserts.py` & `3scale-api-0.9.0/tests/integration/asserts.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/auth/test_app_key_authorization.py` & `3scale-api-0.9.0/tests/integration/auth/test_app_key_authorization.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/auth/test_different_app_key_name.py` & `3scale-api-0.9.0/tests/integration/auth/test_different_app_key_name.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/conftest.py` & `3scale-api-0.9.0/tests/integration/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -419,7 +419,21 @@
     yield entity
     cleanup(entity)
 
 
 @pytest.fixture(scope='module')
 def webhook(api):
     return api.webhooks
+
+
+@pytest.fixture(scope='module')
+def account_plans_params():
+    suffix = get_suffix()
+    name = f"test-{suffix}"
+    return dict(name=name)
+
+
+@pytest.fixture(scope='module')
+def account_plan(account_plans_params, api):
+    entity = api.account_plans.create(params=account_plans_params)
+    yield entity
+    cleanup(entity)
```

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_accounts.py` & `3scale-api-0.9.0/tests/integration/test_integration_accounts.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_analytics.py` & `3scale-api-0.9.0/tests/integration/test_integration_analytics.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_api_client.py` & `3scale-api-0.9.0/tests/integration/test_integration_api_client.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_application.py` & `3scale-api-0.9.0/tests/integration/test_integration_application.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_application_plan.py` & `3scale-api-0.9.0/tests/integration/test_integration_application_plan.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_backend_mapping_rules.py` & `3scale-api-0.9.0/tests/integration/test_integration_backend_mapping_rules.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_backend_metrics.py` & `3scale-api-0.9.0/tests/integration/test_integration_backend_metrics.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_backends.py` & `3scale-api-0.9.0/tests/integration/test_integration_backends.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_limit.py` & `3scale-api-0.9.0/tests/integration/test_integration_limit.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_mapping_rules.py` & `3scale-api-0.9.0/tests/integration/test_integration_mapping_rules.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_methods.py` & `3scale-api-0.9.0/tests/integration/test_integration_methods.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_metrics.py` & `3scale-api-0.9.0/tests/integration/test_integration_metrics.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_policies.py` & `3scale-api-0.9.0/tests/integration/test_integration_policies.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_pricing_rules.py` & `3scale-api-0.9.0/tests/integration/test_integration_pricing_rules.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_provider_accounts.py` & `3scale-api-0.9.0/tests/integration/test_integration_provider_accounts.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_services.py` & `3scale-api-0.9.0/tests/integration/test_integration_services.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/tests/integration/test_integration_webhook.py` & `3scale-api-0.9.0/tests/integration/test_integration_webhook.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/threescale_api/auth.py` & `3scale-api-0.9.0/threescale_api/auth.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/threescale_api/client.py` & `3scale-api-0.9.0/threescale_api/client.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/threescale_api/defaults.py` & `3scale-api-0.9.0/threescale_api/defaults.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/threescale_api/errors.py` & `3scale-api-0.9.0/threescale_api/errors.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/threescale_api/log_config.py` & `3scale-api-0.9.0/threescale_api/log_config.py`

 * *Files identical despite different names*

### Comparing `3scale-api-0.8.0/threescale_api/resources.py` & `3scale-api-0.9.0/threescale_api/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,15 +946,15 @@
 
     @property
     def entity_id(self) -> int:
         return self.entity["signup"]["account"]["id"]
 
 
 class Application(DefaultResource):
-    def __init__(self, entity_name='system_name', **kwargs):
+    def __init__(self, entity_name='name', **kwargs):
         super().__init__(entity_name=entity_name, **kwargs)
         self._auth_objects = {
             Service.AUTH_USER_KEY: auth.UserKeyAuth,
             Service.AUTH_APP_ID_KEY: auth.AppIdKeyAuth
         }
         self._api_client_verify = None
         self._client_factory = utils.HttpClient
@@ -1073,15 +1073,15 @@
 
     @property
     def permissions(self) -> 'UserPermissionsClient':
         return UserPermissionsClient(parent=self, instance_klass=UserPermissions)
 
 
 class AccountPlan(DefaultResource):
-    def __init__(self, entity_name='system_name', **kwargs):
+    def __init__(self, entity_name='name', **kwargs):
         super().__init__(entity_name=entity_name, **kwargs)
 
 
 class Limit(DefaultResource):
     @property
     def app_plan(self) -> ApplicationPlan:
         return self.parent
```

### Comparing `3scale-api-0.8.0/threescale_api/utils.py` & `3scale-api-0.9.0/threescale_api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,15 @@
         self._endpoint = endpoint
         if session is None:
             session = requests.Session()
             self.retry_for_session(session)
 
             session.auth = app.authobj
 
-        if verify is not None:
-            session.verify = verify
-
+        self.verify = verify
         self._session = session
 
         logger.debug("[HTTP CLIENT] New instance: %s", self._base_url)
 
     @staticmethod
     def retry_for_session(session: requests.Session, total: int = 8):
         retry = Retry(
@@ -82,14 +80,16 @@
 
     def request(self, method, path,
                 params=None, data=None, headers=None, cookies=None, files=None,
                 auth=None, timeout=None, allow_redirects=True, proxies=None,
                 hooks=None, stream=None, verify=None, cert=None, json=None) -> requests.Response:
         """mimics requests interface"""
         url = urljoin(self._base_url, path)
+        if verify is None:
+            verify = self.verify
 
         req = requests.Request(
             method=method.upper(),
             url=url,
             headers=headers,
             files=files,
             data=data or {},
```

