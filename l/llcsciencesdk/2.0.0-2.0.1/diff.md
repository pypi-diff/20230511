# Comparing `tmp/llcsciencesdk-2.0.0.tar.gz` & `tmp/llcsciencesdk-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llcsciencesdk-2.0.0.tar", last modified: Wed May 10 13:15:35 2023, max compression
+gzip compressed data, was "llcsciencesdk-2.0.1.tar", last modified: Thu May 11 07:56:30 2023, max compression
```

## Comparing `llcsciencesdk-2.0.0.tar` & `llcsciencesdk-2.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2071 2023-05-10 11:53:51.598334 llcsciencesdk-2.0.0/.gitignore
--rw-r--r--   0        0        0     1080 2021-07-05 15:00:27.981056 llcsciencesdk-2.0.0/LICENSE
--rw-r--r--   0        0        0       83 2023-05-10 11:44:15.775052 llcsciencesdk-2.0.0/llcsciencesdk/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-10 11:44:15.775770 llcsciencesdk-2.0.0/llcsciencesdk/exceptions.py
--rw-r--r--   0        0        0      172 2023-05-10 11:44:15.776288 llcsciencesdk-2.0.0/llcsciencesdk/helpers.py
--rw-r--r--   0        0        0    14233 2023-05-10 11:44:15.776763 llcsciencesdk-2.0.0/llcsciencesdk/llc_api.py
--rw-r--r--   0        0        0     1017 2023-05-10 11:44:15.777187 llcsciencesdk-2.0.0/llcsciencesdk/parameter_mapping.py
--rw-r--r--   0        0        0      719 2022-04-07 10:48:47.109982 llcsciencesdk-2.0.0/llcsciencesdk/sample.py
--rw-r--r--   0        0        0     1440 2023-05-10 11:44:15.777603 llcsciencesdk-2.0.0/llcsciencesdk/tests.py
--rw-r--r--   0        0        0     4905 2023-05-10 11:44:15.778006 llcsciencesdk-2.0.0/llcsciencesdk/urls.py
--rw-r--r--   0        0        0      318 2023-05-10 11:49:19.758651 llcsciencesdk-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1197 2023-05-10 11:44:15.778699 llcsciencesdk-2.0.0/readme.md
--rw-r--r--   0        0        0     1476 1970-01-01 00:00:00.000000 llcsciencesdk-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2071 2023-05-10 11:53:51.598334 llcsciencesdk-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1080 2021-07-05 15:00:27.981056 llcsciencesdk-2.0.1/LICENSE
+-rw-r--r--   0        0        0       83 2023-05-11 07:50:50.096670 llcsciencesdk-2.0.1/llcsciencesdk/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-10 11:44:15.775770 llcsciencesdk-2.0.1/llcsciencesdk/exceptions.py
+-rw-r--r--   0        0        0      172 2023-05-10 11:44:15.776288 llcsciencesdk-2.0.1/llcsciencesdk/helpers.py
+-rw-r--r--   0        0        0    14352 2023-05-11 07:54:33.550767 llcsciencesdk-2.0.1/llcsciencesdk/llc_api.py
+-rw-r--r--   0        0        0     1017 2023-05-10 11:44:15.777187 llcsciencesdk-2.0.1/llcsciencesdk/parameter_mapping.py
+-rw-r--r--   0        0        0      719 2022-04-07 10:48:47.109982 llcsciencesdk-2.0.1/llcsciencesdk/sample.py
+-rw-r--r--   0        0        0     1440 2023-05-10 11:44:15.777603 llcsciencesdk-2.0.1/llcsciencesdk/tests.py
+-rw-r--r--   0        0        0     5002 2023-05-11 07:55:29.842359 llcsciencesdk-2.0.1/llcsciencesdk/urls.py
+-rw-r--r--   0        0        0      318 2023-05-10 13:21:19.253737 llcsciencesdk-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1590 2023-05-10 13:21:08.697984 llcsciencesdk-2.0.1/readme.md
+-rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 llcsciencesdk-2.0.1/PKG-INFO
```

### Comparing `llcsciencesdk-2.0.0/.gitignore` & `llcsciencesdk-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `llcsciencesdk-2.0.0/LICENSE` & `llcsciencesdk-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llcsciencesdk-2.0.0/llcsciencesdk/exceptions.py` & `llcsciencesdk-2.0.1/llcsciencesdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `llcsciencesdk-2.0.0/llcsciencesdk/llc_api.py` & `llcsciencesdk-2.0.1/llcsciencesdk/llc_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,18 @@
         url = self.api_urls.GET_PLANTING_DESIGN_DETAIL
         return self._get_request(url, str(planting_design_id))
 
     def get_planting_design_list(self) -> dict:
         url = self.api_urls.GET_PLANTING_DESIGN_LIST
         return self._get_request(url)
 
+    # Map Layers
+    def get_map_layers(self) -> dict:
+        return self._get_request(self.api_urls.GET_MAP_LAYERS)
+
     # Calibrate
 
     def get_calibrate_input(self, calibrate_scenario_id: int) -> dict:
         return self._get_request(
             self.api_urls.GET_CALIBRATE_INPUT, str(calibrate_scenario_id)
         )
```

### Comparing `llcsciencesdk-2.0.0/llcsciencesdk/parameter_mapping.py` & `llcsciencesdk-2.0.1/llcsciencesdk/parameter_mapping.py`

 * *Files identical despite different names*

### Comparing `llcsciencesdk-2.0.0/llcsciencesdk/sample.py` & `llcsciencesdk-2.0.1/llcsciencesdk/sample.py`

 * *Files identical despite different names*

### Comparing `llcsciencesdk-2.0.0/llcsciencesdk/tests.py` & `llcsciencesdk-2.0.1/llcsciencesdk/tests.py`

 * *Files identical despite different names*

### Comparing `llcsciencesdk-2.0.0/llcsciencesdk/urls.py` & `llcsciencesdk-2.0.1/llcsciencesdk/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     GET_PLANTING_DESIGN_DETAIL: str = field(
         init=False, default="/plantingdesign/api/detail/"
     )
     GET_PLANTING_DESIGN_LIST: str = field(
         init=False, default="/plantingdesign/api/list"
     )
 
+    # May Layers
+    GET_MAP_LAYERS: str = field(init=False, default="/rs_dashboard/maplayers")
+
     # Calibrate
     GET_CALIBRATE_INPUT: str = field(
         init=False, default="/sciencemodel/calibrateinput/"
     )
     UPDATE_CALIBRATE_SCENARIO_PARAMETERS: str = field(
         init=False,
         default="/sciencemodel/fasttrackinput/calibrate_scenario_update_parameters",
```

### Comparing `llcsciencesdk-2.0.0/PKG-INFO` & `llcsciencesdk-2.0.1/readme.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: llcsciencesdk
-Version: 2.0.0
-Summary: A mini SDK for interacting with the LLC Science Admin
-Author: Ariel Delgado
-Author-email: a.delgado@landlifecompany.com
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
-
 # LLC Science SDK
 
 > A simple way to fetch scientific data from the Science Admin.
 > Please visit {BASE_URL}/api/schema/swagger-ui/#/ for more information on the API.
 
 ## Installation
 
@@ -54,12 +45,35 @@
 llc_api.login("username", "password")
 model_input = llc_api.get_ft_input(1)
 planting_design_list = llc_api.get_planting_design_list()
 planting_design_detail = llc_api.get_planting_design(10)
 ```
 
 
-```
 
 ## Supported endpoints
 
 See the swagger docs for a complete list. {BASE_URL}/api/schema/swagger-ui/#/
+
+## For Developers
+
+### Updating package
+
+1. Make sure you have supported version of flit installed (see project.toml).
+
+```
+    python3 -m pip install flit
+```
+
+2. Set env variables for PiPy login:
+
+```
+    export FLIT_USERNAME=username
+    export FLIT_PASSWORD=password
+```
+3. Update the version of the API in the __init__.py file.
+4. Run command to publish to PiPy:
+
+```
+    flit publish
+```
+
```

