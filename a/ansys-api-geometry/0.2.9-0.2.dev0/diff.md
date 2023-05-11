# Comparing `tmp/ansys-api-geometry-0.2.9.tar.gz` & `tmp/ansys-api-geometry-0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-geometry-0.2.9.tar", last modified: Thu May 11 15:05:14 2023, max compression
+gzip compressed data, was "ansys-api-geometry-0.2.dev0.tar", last modified: Tue May  2 16:12:30 2023, max compression
```

## Comparing `ansys-api-geometry-0.2.9.tar` & `ansys-api-geometry-0.2.dev0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:05:14.191574 ansys-api-geometry-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-11 15:05:14.191574 ansys-api-geometry-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:05:14.183573 ansys-api-geometry-0.2.9/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:05:14.183573 ansys-api-geometry-0.2.9/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:05:14.187573 ansys-api-geometry-0.2.9/ansys/api/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:05:14.191574 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/admin.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/bodies.proto
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/commands.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/components.proto
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/coordinatesystems.proto
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/curves.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/designs.proto
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/edges.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/faces.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/facettools.proto
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/geometryapi.proto
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/geometryapplication.proto
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/materials.proto
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/meshes.proto
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/models.proto
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/namedselections.proto
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/parts.proto
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/preparetools.proto
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/repairtools.proto
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/ansys/api/geometry/v0/streaming.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:05:14.191574 ansys-api-geometry-0.2.9/ansys_api_geometry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-11 15:05:14.000000 ansys-api-geometry-0.2.9/ansys_api_geometry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-11 15:05:14.000000 ansys-api-geometry-0.2.9/ansys_api_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:05:14.000000 ansys-api-geometry-0.2.9/ansys_api_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-11 15:05:14.000000 ansys-api-geometry-0.2.9/ansys_api_geometry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 15:05:14.000000 ansys-api-geometry-0.2.9/ansys_api_geometry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 15:05:14.000000 ansys-api-geometry-0.2.9/ansys_api_geometry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:05:14.191574 ansys-api-geometry-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-11 15:04:54.000000 ansys-api-geometry-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:30.253654 ansys-api-geometry-0.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-02 16:12:30.253654 ansys-api-geometry-0.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:30.245654 ansys-api-geometry-0.2.dev0/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:30.245654 ansys-api-geometry-0.2.dev0/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:30.249654 ansys-api-geometry-0.2.dev0/ansys/api/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:30.253654 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/admin.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/bodies.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/commands.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/components.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/coordinatesystems.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/curves.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/designs.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/edges.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/faces.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/facettools.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/geometryapi.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/geometryapplication.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/materials.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/meshes.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/models.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/namedselections.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/parts.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/preparetools.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/repairtools.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/streaming.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:30.253654 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-02 16:12:30.000000 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-02 16:12:30.000000 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:12:30.000000 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 16:12:30.000000 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 16:12:30.000000 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 16:12:30.000000 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:12:30.253654 ansys-api-geometry-0.2.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/setup.py
```

### Comparing `ansys-api-geometry-0.2.9/LICENSE` & `ansys-api-geometry-0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/PKG-INFO` & `ansys-api-geometry-0.2.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-geometry
-Version: 0.2.9
-Summary: Autogenerated python gRPC interface package for ansys-api-geometry, built on 15:05:14 on 11 May 2023
+Version: 0.2.dev0
+Summary: Autogenerated python gRPC interface package for ansys-api-geometry, built on 16:12:30 on 02 May 2023
 Home-page: https://github.com/ansys/ansys-api-geometry
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-geometry-0.2.9/README.md` & `ansys-api-geometry-0.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/admin.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/admin.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/bodies.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/bodies.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/commands.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/commands.proto`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,14 @@
 message DownloadFileResponse {
   bytes data=1;
 }
 
 message UploadFileRequest {
   bytes data=1;
   string file_name=2;
-  bool open=3;
 }
 
 message UploadFileResponse {
   string file_path=1;
 }
 
 message CreateSphereRequest {
@@ -216,8 +215,8 @@
   double major_radius=3;
   double minor_radius=4;
   Frame frame=5;
 }
 
 message CreateTorusResponse {
   string id=1;
-}
+}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+iso-8859-1
```

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/components.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/components.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/coordinatesystems.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/coordinatesystems.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/curves.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/curves.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/edges.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/edges.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/faces.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/faces.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/facettools.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/facettools.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/geometryapi.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/geometryapi.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/geometryapplication.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/geometryapplication.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/models.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/models.proto`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,14 @@
   string name = 2;
   bool can_suppress = 3;
   bool is_deleted = 4;
   bool is_suppressed = 5;
   Matrix transform_to_master = 6;
   BodyMasterNullable master = 7;
   string master_id = 8;
-  string parent_id = 9;
 }
 
 //
 // A nullable body master.
 message BodyMasterNullable{
   oneof kind 
   {
@@ -143,17 +142,14 @@
 //
 // A component.
 message Component{
   string id = 1;
   string name = 2;
   Part part_occurrence = 3;
   Matrix placement =4;
-  string master_id=5;
-  string parent_id=6;
-  Part part_master=7;
 }
 
 //
 // A part.
 message Part{
   string id = 1;
   string name = 2;
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+iso-8859-1
```

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/namedselections.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/namedselections.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/parts.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/parts.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/preparetools.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/preparetools.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys/api/geometry/v0/repairtools.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/repairtools.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/ansys_api_geometry.egg-info/PKG-INFO` & `ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-geometry
-Version: 0.2.9
-Summary: Autogenerated python gRPC interface package for ansys-api-geometry, built on 15:05:14 on 11 May 2023
+Version: 0.2.dev0
+Summary: Autogenerated python gRPC interface package for ansys-api-geometry, built on 16:12:30 on 02 May 2023
 Home-page: https://github.com/ansys/ansys-api-geometry
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-geometry-0.2.9/ansys_api_geometry.egg-info/SOURCES.txt` & `ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.9/setup.py` & `ansys-api-geometry-0.2.dev0/setup.py`

 * *Files identical despite different names*

