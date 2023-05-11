# Comparing `tmp/fairscape_cli-0.1.5.tar.gz` & `tmp/fairscape_cli-0.1.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairscape_cli-0.1.5.tar", max compression
+gzip compressed data, was "fairscape_cli-0.1.5a1.tar", max compression
```

## Comparing `fairscape_cli-0.1.5.tar` & `fairscape_cli-0.1.5a1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.5/LICENSE
--rw-r--r--   0        0        0     4058 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5/fairscape_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5/fairscape_cli/apps/__init__.py
--rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5/fairscape_cli/apps/cache.py
--rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5/fairscape_cli/apps/describe.py
--rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/fairscape.py
--rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/list.py
--rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/models/__init__.py
--rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/models/computation.py
--rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/models/dataset.py
--rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/models/software.py
--rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/objects.py
--rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/rocrate.py
--rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/utils.py
--rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/apps/validator.py
--rw-r--r--   0        0        0      397 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5/fairscape_cli/main.py
--rw-r--r--   0        0        0      221 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/models/__init__.py
--rw-r--r--   0        0        0      291 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5/fairscape_cli/models/computation.py
--rw-r--r--   0        0        0      205 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/models/dataset.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/models/models.py
--rw-r--r--   0        0        0      924 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5/fairscape_cli/models/rocrate.py
--rw-r--r--   0        0        0    12386 2023-05-02 17:00:11.896184 fairscape_cli-0.1.5/fairscape_cli/models/schema.py
--rw-r--r--   0        0        0      128 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5/fairscape_cli/models/software.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/rocrate/__init__.py
--rw-r--r--   0        0        0    14880 2023-05-02 17:50:35.055165 fairscape_cli-0.1.5/fairscape_cli/rocrate/rocrate.py
--rw-r--r--   0        0        0     1326 2023-04-17 19:02:18.839104 fairscape_cli-0.1.5/fairscape_cli/rocrate/utils.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/validate/__init__.py
--rw-r--r--   0        0        0     1365 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5/fairscape_cli/validate/validate_json.py
--rw-r--r--   0        0        0     1534 2023-05-02 17:11:26.855959 fairscape_cli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4903 1970-01-01 00:00:00.000000 fairscape_cli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.5a1/LICENSE
+-rw-r--r--   0        0        0     4058 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a1/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a1/fairscape_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a1/fairscape_cli/apps/__init__.py
+-rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a1/fairscape_cli/apps/cache.py
+-rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a1/fairscape_cli/apps/describe.py
+-rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/fairscape.py
+-rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/list.py
+-rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/models/__init__.py
+-rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/models/computation.py
+-rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/models/dataset.py
+-rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/models/software.py
+-rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/objects.py
+-rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/rocrate.py
+-rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/utils.py
+-rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/validator.py
+-rw-r--r--   0        0        0      397 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5a1/fairscape_cli/main.py
+-rw-r--r--   0        0        0      285 2023-05-11 18:22:39.597260 fairscape_cli-0.1.5a1/fairscape_cli/models/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5a1/fairscape_cli/models/computation.py
+-rw-r--r--   0        0        0      205 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/models/dataset.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/models/models.py
+-rw-r--r--   0        0        0     5033 2023-05-11 18:45:00.117305 fairscape_cli-0.1.5a1/fairscape_cli/models/rocrate.py
+-rw-r--r--   0        0        0    13036 2023-05-10 19:09:33.371675 fairscape_cli-0.1.5a1/fairscape_cli/models/schema.py
+-rw-r--r--   0        0        0      128 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5a1/fairscape_cli/models/software.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/rocrate/__init__.py
+-rw-r--r--   0        0        0    15800 2023-05-11 18:51:57.277320 fairscape_cli-0.1.5a1/fairscape_cli/rocrate/rocrate.py
+-rw-r--r--   0        0        0     1326 2023-04-17 19:02:18.839104 fairscape_cli-0.1.5a1/fairscape_cli/rocrate/utils.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/validate/__init__.py
+-rw-r--r--   0        0        0     1365 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/validate/validate_json.py
+-rw-r--r--   0        0        0     1517 2023-05-11 18:52:55.677321 fairscape_cli-0.1.5a1/pyproject.toml
+-rw-r--r--   0        0        0     4949 1970-01-01 00:00:00.000000 fairscape_cli-0.1.5a1/PKG-INFO
```

### Comparing `fairscape_cli-0.1.5/LICENSE` & `fairscape_cli-0.1.5a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5/README.md` & `fairscape_cli-0.1.5a1/README.md`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5/fairscape_cli/apps/fairscape.py` & `fairscape_cli-0.1.5a1/fairscape_cli/apps/fairscape.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5/fairscape_cli/apps/models/dataset.py` & `fairscape_cli-0.1.5a1/fairscape_cli/apps/models/dataset.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5/fairscape_cli/apps/models/software.py` & `fairscape_cli-0.1.5a1/fairscape_cli/apps/models/software.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5/fairscape_cli/apps/objects.py` & `fairscape_cli-0.1.5a1/fairscape_cli/apps/objects.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5/fairscape_cli/apps/rocrate.py` & `fairscape_cli-0.1.5a1/fairscape_cli/apps/rocrate.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5/fairscape_cli/apps/utils.py` & `fairscape_cli-0.1.5a1/fairscape_cli/apps/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5/fairscape_cli/apps/validator.py` & `fairscape_cli-0.1.5a1/fairscape_cli/apps/validator.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5/fairscape_cli/models/schema.py` & `fairscape_cli-0.1.5a1/fairscape_cli/models/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,14 +153,20 @@
             )
 
         if width != self.ImageSchema.width:
             raise ImageValidationException(
                 message=f"Image Width {width} != {self.ImageSchema.width}"
             )
 
+class FiletypeEnum(str, Enum):
+    """List of supported filetypes with normative naming
+    """
+    csv = "csv"
+    tsv = "tsv"
+    
 
 class DatatypeEnum(str, Enum):
     """
     A Datatype Enum for supported types for validation
 
     These Choices are to be expanded until covering the full spec from [CSV on the Web](https://w3c.github.io/csvw/metadata/#datatypes)
     These datatypes are defined in [XMLSchema](http://www.w3.org/2001/XMLSchema#) as anyAtomicType
@@ -410,24 +416,41 @@
       )
 
       return tabularData
 
 
 class DataValidationException(Exception):
 
-    def __init__(self, message="DataValidationException: Validation Failed"):
+    def __init__(self, error, message="DataValidationException: Validation Failed"):
+        self.error = error
+        self.message = message
+        super().__init__(self.message)
+
+
+class NAValidationException(DataValidationException):
+
+    def __init__(self, error, message="DataValidationException: NA Values in required column"):
+        self.error = error
+        self.message = message
+        super().__init__(self.message)
+
+class DatatypeValidationException(DataValidationException):
+
+    def __init__(self, error, message)
+        self.error = error
         self.message = message
         super().__init__(self.message)
 
 
 class PathNotFoundException(DataValidationException):
 
     def __init__(self, message="PathNotFound", path: pathlib.Path = None):
-        if path is not None:
-            self.message = f"PathNotFound: {str(path)}"
+        self.path = path
+        if self.path is not None:
+            self.message = f"PathNotFound: {str(self.path)}"
         else:
             self.message = message
         super().__init__(self.message)
 
 
 class TabularDataValidation():
     ''' A class for running the execution of data validation as determined by a TabularDataSchema
```

### Comparing `fairscape_cli-0.1.5/fairscape_cli/rocrate/utils.py` & `fairscape_cli-0.1.5a1/fairscape_cli/rocrate/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5/fairscape_cli/validate/validate_json.py` & `fairscape_cli-0.1.5a1/fairscape_cli/validate/validate_json.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5/pyproject.toml` & `fairscape_cli-0.1.5a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,25 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3"]
 keywords = ["fairscape", "reproducibility", "fair", "b2ai"]
 dependencies = [
         "pydantic",
         "fairscape-models",
-        "typer[all]",
-        "pydantic",
         "pyld"
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/fairscape/fairscape-cli"
 
 
 [tool.poetry]
 name = "fairscape-cli"
-version = "0.1.5"
+version = "0.1.5a1"
 description = "A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API"
 authors = ["mlev71 <max.adam.levinson@gmail.com>"]
 license = "LICENSE"
 readme = "README.md"
 packages = [{include = "fairscape_cli"}]
 
 
@@ -41,14 +39,15 @@
 python = "^3.8"
 pydantic = "^1.10.7"
 pyld = "^2.0.3"
 click = "^8.1.3"
 fairscape-models = "^0.1.2"
 imageio = "^2.27.0"
 pandas = "^2.0.0"
+prettytable = "^3.7.0"
 
 
 [tool.poetry.scripts]
 fairscape-cli = "fairscape_cli.main:cli"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `fairscape_cli-0.1.5/PKG-INFO` & `fairscape_cli-0.1.5a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairscape-cli
-Version: 0.1.5
+Version: 0.1.5a1
 Summary: A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API
 License: LICENSE
 Author: mlev71
 Author-email: max.adam.levinson@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: fairscape-models (>=0.1.2,<0.2.0)
 Requires-Dist: imageio (>=2.27.0,<3.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: prettytable (>=3.7.0,<4.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyld (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # fairscape-cli
 Data Validation and Packaging utility for sending evidence graphs to FAIRSCAPE
```

