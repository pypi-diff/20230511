# Comparing `tmp/cognite_gql_pygen-0.4.4.tar.gz` & `tmp/cognite_gql_pygen-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_gql_pygen-0.4.4.tar", max compression
+gzip compressed data, was "cognite_gql_pygen-0.4.5.tar", max compression
```

## Comparing `cognite_gql_pygen-0.4.4.tar` & `cognite_gql_pygen-0.4.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11349 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/LICENSE
--rw-r--r--   0        0        0     4486 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/README.md
--rw-r--r--   0        0        0     8651 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/README.md
--rw-r--r--   0        0        0        0 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/__init__.py
--rw-r--r--   0        0        0      167 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/cdf/__init__.py
--rw-r--r--   0        0        0    19000 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/cdf/client_dm_v3.py
--rw-r--r--   0        0        0     3909 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/cdf/data_classes_dm_v3.py
--rw-r--r--   0        0        0     2629 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/cdf/get_client.py
--rwxr-xr-x   0        0        0      346 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/config.py
--rw-r--r--   0        0        0      192 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/custom_types/__init__.py
--rw-r--r--   0        0        0      236 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/custom_types/_scalars.py
--rw-r--r--   0        0        0      760 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/custom_types/jsonobject.py
--rw-r--r--   0        0        0     4724 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/custom_types/timestamp.py
--rw-r--r--   0        0        0      196 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/domain_modeling/__init__.py
--rw-r--r--   0        0        0     6324 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/domain_modeling/domain_client.py
--rw-r--r--   0        0        0     3863 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/domain_modeling/domain_model.py
--rw-r--r--   0        0        0    19106 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/domain_modeling/domain_model_api.py
--rw-r--r--   0        0        0     5929 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/domain_modeling/relationship_api.py
--rw-r--r--   0        0        0     7060 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/domain_modeling/schema.py
--rw-r--r--   0        0        0     1423 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/misc.py
--rw-r--r--   0        0        0        0 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/dm_clients/py.typed
--rw-r--r--   0        0        0       76 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/gqlpygen/__init__.py
--rw-r--r--   0        0        0     1904 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/gqlpygen/data_classes.py
--rw-r--r--   0        0        0     1560 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/gqlpygen/generator.py
--rw-r--r--   0        0        0     7728 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/gqlpygen/main.py
--rw-r--r--   0        0        0      596 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/gqlpygen/misc.py
--rw-r--r--   0        0        0     1355 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/gqlpygen/parser.py
--rw-r--r--   0        0        0     1333 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/gqlpygen/templates/client.txt
--rw-r--r--   0        0        0      803 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/gqlpygen/templates/schema.txt
--rw-r--r--   0        0        0       22 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/cognite/gqlpygen/version.py
--rw-r--r--   0        0        0     2047 2023-05-09 14:39:17.810845 cognite_gql_pygen-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     5663 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/LICENSE
+-rw-r--r--   0        0        0     4486 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/README.md
+-rw-r--r--   0        0        0     8651 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/cdf/__init__.py
+-rw-r--r--   0        0        0    19000 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/cdf/client_dm_v3.py
+-rw-r--r--   0        0        0     3909 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/cdf/data_classes_dm_v3.py
+-rw-r--r--   0        0        0     2629 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/cdf/get_client.py
+-rwxr-xr-x   0        0        0      399 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/config.py
+-rw-r--r--   0        0        0      192 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/custom_types/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/custom_types/_scalars.py
+-rw-r--r--   0        0        0      760 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/custom_types/jsonobject.py
+-rw-r--r--   0        0        0     4724 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/custom_types/timestamp.py
+-rw-r--r--   0        0        0      196 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/domain_modeling/__init__.py
+-rw-r--r--   0        0        0     6324 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/domain_modeling/domain_client.py
+-rw-r--r--   0        0        0     4065 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/domain_modeling/domain_model.py
+-rw-r--r--   0        0        0    19106 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/domain_modeling/domain_model_api.py
+-rw-r--r--   0        0        0     5929 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/domain_modeling/relationship_api.py
+-rw-r--r--   0        0        0     7060 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/domain_modeling/schema.py
+-rw-r--r--   0        0        0     1423 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/misc.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/dm_clients/py.typed
+-rw-r--r--   0        0        0       76 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/gqlpygen/__init__.py
+-rw-r--r--   0        0        0     1904 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/gqlpygen/data_classes.py
+-rw-r--r--   0        0        0     1560 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/gqlpygen/generator.py
+-rw-r--r--   0        0        0     7728 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/gqlpygen/main.py
+-rw-r--r--   0        0        0      596 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/gqlpygen/misc.py
+-rw-r--r--   0        0        0     1425 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/gqlpygen/parser.py
+-rw-r--r--   0        0        0     1333 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/gqlpygen/templates/client.txt
+-rw-r--r--   0        0        0      803 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/gqlpygen/templates/schema.txt
+-rw-r--r--   0        0        0       22 2023-05-11 14:07:34.369294 cognite_gql_pygen-0.4.5/cognite/gqlpygen/version.py
+-rw-r--r--   0        0        0     2047 2023-05-11 14:07:34.373294 cognite_gql_pygen-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     5663 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.4.5/PKG-INFO
```

### Comparing `cognite_gql_pygen-0.4.4/LICENSE` & `cognite_gql_pygen-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/README.md` & `cognite_gql_pygen-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/dm_clients/README.md` & `cognite_gql_pygen-0.4.5/cognite/dm_clients/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/dm_clients/cdf/client_dm_v3.py` & `cognite_gql_pygen-0.4.5/cognite/dm_clients/cdf/client_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/dm_clients/cdf/data_classes_dm_v3.py` & `cognite_gql_pygen-0.4.5/cognite/dm_clients/cdf/data_classes_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/dm_clients/cdf/get_client.py` & `cognite_gql_pygen-0.4.5/cognite/dm_clients/cdf/get_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/dm_clients/custom_types/jsonobject.py` & `cognite_gql_pygen-0.4.5/cognite/dm_clients/custom_types/jsonobject.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/dm_clients/custom_types/timestamp.py` & `cognite_gql_pygen-0.4.5/cognite/dm_clients/custom_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/dm_clients/domain_modeling/domain_client.py` & `cognite_gql_pygen-0.4.5/cognite/dm_clients/domain_modeling/domain_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/dm_clients/domain_modeling/domain_model.py` & `cognite_gql_pygen-0.4.5/cognite/dm_clients/domain_modeling/domain_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,20 @@
         if _reference:
             for field_name, field in self.__fields__.items():
                 if field.required and field_name not in kwargs:
                     kwargs[field_name] = field.type_()
         super().__init__(*args, **kwargs)
         self._reference = _reference
 
+    def __repr_args__(self):
+        if self._reference:
+            return [(key, getattr(self, key)) for key in ("externalId", "_reference")]
+        else:
+            return super().__repr_args__()
+
     def as_reference(self) -> Self:
         return type(self)(externalId=self.externalId, _reference=True)
 
     @classmethod
     def ref(cls, externalId: str):  # noqa: N803
         return cls(externalId=externalId, _reference=True)
```

### Comparing `cognite_gql_pygen-0.4.4/cognite/dm_clients/domain_modeling/domain_model_api.py` & `cognite_gql_pygen-0.4.5/cognite/dm_clients/domain_modeling/domain_model_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/dm_clients/domain_modeling/relationship_api.py` & `cognite_gql_pygen-0.4.5/cognite/dm_clients/domain_modeling/relationship_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/dm_clients/domain_modeling/schema.py` & `cognite_gql_pygen-0.4.5/cognite/dm_clients/domain_modeling/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/dm_clients/misc.py` & `cognite_gql_pygen-0.4.5/cognite/dm_clients/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/gqlpygen/data_classes.py` & `cognite_gql_pygen-0.4.5/cognite/gqlpygen/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/gqlpygen/generator.py` & `cognite_gql_pygen-0.4.5/cognite/gqlpygen/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/gqlpygen/main.py` & `cognite_gql_pygen-0.4.5/cognite/gqlpygen/main.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/gqlpygen/misc.py` & `cognite_gql_pygen-0.4.5/cognite/gqlpygen/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/gqlpygen/parser.py` & `cognite_gql_pygen-0.4.5/cognite/gqlpygen/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import graphql
 
 from cognite.dm_clients.misc import to_pascal
 from cognite.gqlpygen.data_classes import DomainModel, DomainModels, Field
 
 GRAPHQL_TO_PYTHON_TYPE_MAP = {
     "String": "str",
+    "Int": "int",
     "Float": "float",
-    "Integer": "int",
     "Boolean": "bool",
 }
 
 
 def parse_graphql(schema_raw: str) -> DomainModels:
     schema = graphql.parse(schema_raw)
 
@@ -24,20 +24,23 @@
 
 
 def _parse_field(field: dict) -> Field:
     field_name = field["name"]["value"]
     is_required = False
     is_list = False
     field_type = field["type"]
-    if field_type["kind"] == "non_null_type":
-        is_required = True
-        field_type = field_type["type"]
-    if field_type["kind"] == "list_type":
-        is_list = True
-        field_type = field_type["type"]
+    while True:
+        if field_type["kind"] == "non_null_type":
+            is_required = True
+            field_type = field_type["type"]
+        elif field_type["kind"] == "list_type":
+            is_list = True
+            field_type = field_type["type"]
+        else:
+            break
     is_named_type = field_type["kind"] == "named_type"
     type_name = field_type["name"]["value"]
 
     return Field(
         name=field_name,
         type=GRAPHQL_TO_PYTHON_TYPE_MAP.get(type_name, type_name),
         is_list=is_list,
```

### Comparing `cognite_gql_pygen-0.4.4/cognite/gqlpygen/templates/client.txt` & `cognite_gql_pygen-0.4.5/cognite/gqlpygen/templates/client.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/cognite/gqlpygen/templates/schema.txt` & `cognite_gql_pygen-0.4.5/cognite/gqlpygen/templates/schema.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.4/pyproject.toml` & `cognite_gql_pygen-0.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-gql-pygen"
-version = "0.4.4"
+version = "0.4.5"
 description = "Cognite graphQL Python generation SDK"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache-2.0"
 
 packages = [{ include="cognite", from="." }]
 exclude = ["cognite/dm_clients/*.toml"]
```

### Comparing `cognite_gql_pygen-0.4.4/PKG-INFO` & `cognite_gql_pygen-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-gql-pygen
-Version: 0.4.4
+Version: 0.4.5
 Summary: Cognite graphQL Python generation SDK
 License: Apache-2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

