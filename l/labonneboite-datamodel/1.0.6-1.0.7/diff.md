# Comparing `tmp/labonneboite_datamodel-1.0.6.tar.gz` & `tmp/labonneboite_datamodel-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labonneboite_datamodel-1.0.6.tar", max compression
+gzip compressed data, was "labonneboite_datamodel-1.0.7.tar", max compression
```

## Comparing `labonneboite_datamodel-1.0.6.tar` & `labonneboite_datamodel-1.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      224 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/__init__.py
--rw-r--r--   0        0        0      697 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/crud.py
--rw-r--r--   0        0        0     2022 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/job.py
--rw-r--r--   0        0        0     7672 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/office.py
--rw-r--r--   0        0        0        0 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/__init__.py
--rw-r--r--   0        0        0     3589 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/data/test.csv
--rw-r--r--   0        0        0      997 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/test_job.py
--rw-r--r--   0        0        0     5612 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/test_office.py
--rw-r--r--   0        0        0     1205 2023-04-24 11:56:38.875328 labonneboite_datamodel-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 labonneboite_datamodel-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      224 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.7/labonneboite_datamodel/__init__.py
+-rw-r--r--   0        0        0      697 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.7/labonneboite_datamodel/crud.py
+-rw-r--r--   0        0        0     2022 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.7/labonneboite_datamodel/job.py
+-rw-r--r--   0        0        0     7718 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.7/labonneboite_datamodel/office.py
+-rw-r--r--   0        0        0        0 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.7/labonneboite_datamodel/tests/__init__.py
+-rw-r--r--   0        0        0     3589 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.7/labonneboite_datamodel/tests/data/test.csv
+-rw-r--r--   0        0        0      997 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.7/labonneboite_datamodel/tests/test_job.py
+-rw-r--r--   0        0        0     5612 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.7/labonneboite_datamodel/tests/test_office.py
+-rw-r--r--   0        0        0     1205 2023-05-10 08:45:10.370481 labonneboite_datamodel-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 labonneboite_datamodel-1.0.7/PKG-INFO
```

### Comparing `labonneboite_datamodel-1.0.6/labonneboite_datamodel/crud.py` & `labonneboite_datamodel-1.0.7/labonneboite_datamodel/crud.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.0.6/labonneboite_datamodel/job.py` & `labonneboite_datamodel-1.0.7/labonneboite_datamodel/job.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.0.6/labonneboite_datamodel/office.py` & `labonneboite_datamodel-1.0.7/labonneboite_datamodel/office.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,17 +279,19 @@
     This is only for gps information
 
     Attributes:
         department_number: Department number (75, 47, etc.) where the company is.
         department: Department name where the company is.
         city:
         region:
+        region_number:
         latitude:
         longitude:
     """
 
     department_number: int
     department: str
     city: str
     region: str
+    region_number: int
     latitude: float
     longitude: float
```

### Comparing `labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/data/test.csv` & `labonneboite_datamodel-1.0.7/labonneboite_datamodel/tests/data/test.csv`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/test_job.py` & `labonneboite_datamodel-1.0.7/labonneboite_datamodel/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/test_office.py` & `labonneboite_datamodel-1.0.7/labonneboite_datamodel/tests/test_office.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.0.6/pyproject.toml` & `labonneboite_datamodel-1.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labonneboite-datamodel"
-version = "1.0.6"
+version = "1.0.7"
 description = "Datamodel for labonneboite"
 authors = ["Sylvain Touret"]
 license = "MIT"
 packages = [{include = "labonneboite_datamodel"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

