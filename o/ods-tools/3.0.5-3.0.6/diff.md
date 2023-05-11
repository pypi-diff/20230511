# Comparing `tmp/ods_tools-3.0.5.tar.gz` & `tmp/ods_tools-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ods_tools-3.0.5.tar", last modified: Thu Apr  6 10:45:21 2023, max compression
+gzip compressed data, was "ods_tools-3.0.6.tar", last modified: Thu May 11 14:33:33 2023, max compression
```

## Comparing `ods_tools-3.0.5.tar` & `ods_tools-3.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:45:21.084897 ods_tools-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-04-06 10:45:21.084897 ods_tools-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-06 10:45:05.000000 ods_tools-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:45:21.084897 ods_tools-3.0.5/ods_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-06 10:45:05.000000 ods_tools-3.0.5/ods_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-06 10:45:05.000000 ods_tools-3.0.5/ods_tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:45:21.084897 ods_tools-3.0.5/ods_tools/oed/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-06 10:45:05.000000 ods_tools-3.0.5/ods_tools/oed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-04-06 10:45:05.000000 ods_tools-3.0.5/ods_tools/oed/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-04-06 10:45:05.000000 ods_tools-3.0.5/ods_tools/oed/exposure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-06 10:45:05.000000 ods_tools-3.0.5/ods_tools/oed/forex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-06 10:45:05.000000 ods_tools-3.0.5/ods_tools/oed/oed_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-04-06 10:45:05.000000 ods_tools-3.0.5/ods_tools/oed/setting_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20875 2023-04-06 10:45:05.000000 ods_tools-3.0.5/ods_tools/oed/source.py
--rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-04-06 10:45:05.000000 ods_tools-3.0.5/ods_tools/oed/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:45:21.084897 ods_tools-3.0.5/ods_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-04-06 10:45:21.000000 ods_tools-3.0.5/ods_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-06 10:45:21.000000 ods_tools-3.0.5/ods_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 10:45:21.000000 ods_tools-3.0.5/ods_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-06 10:45:21.000000 ods_tools-3.0.5/ods_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-06 10:45:21.000000 ods_tools-3.0.5/ods_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 10:45:21.000000 ods_tools-3.0.5/ods_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 10:45:21.084897 ods_tools-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-06 10:45:05.000000 ods_tools-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:33:33.864809 ods_tools-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-11 14:33:33.864809 ods_tools-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-11 14:33:13.000000 ods_tools-3.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:33:33.860809 ods_tools-3.0.6/ods_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:33:33.864809 ods_tools-3.0.6/ods_tools/oed/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/forex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/oed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/setting_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20875 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-05-11 14:33:13.000000 ods_tools-3.0.6/ods_tools/oed/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:33:33.864809 ods_tools-3.0.6/ods_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-11 14:33:33.000000 ods_tools-3.0.6/ods_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-11 14:33:33.000000 ods_tools-3.0.6/ods_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:33:33.000000 ods_tools-3.0.6/ods_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 14:33:33.000000 ods_tools-3.0.6/ods_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 14:33:33.000000 ods_tools-3.0.6/ods_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 14:33:33.000000 ods_tools-3.0.6/ods_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:33:33.864809 ods_tools-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-11 14:33:13.000000 ods_tools-3.0.6/setup.py
```

### Comparing `ods_tools-3.0.5/PKG-INFO` & `ods_tools-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ods_tools
-Version: 3.0.5
+Version: 3.0.6
 Summary: Tools to manage ODS files
 Home-page: https://github.com/OasisLMF/OpenDataStandards
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ods_tools-3.0.5/README.md` & `ods_tools-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.5/ods_tools/main.py` & `ods_tools-3.0.6/ods_tools/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,16 @@
     'convert',
     'check'
 ]
 
 import argparse
 import logging
 
-from .oed import OedExposure, OdsException
-
-logger = logging.getLogger(__name__)
+from ods_tools.oed import OedExposure, OdsException
+from ods_tools import logger
 
 
 def get_oed_exposure(config_json=None, oed_dir=None, **kwargs):
     if config_json:
         return OedExposure.from_config(config_json, **kwargs)
     elif oed_dir:
         return OedExposure.from_dir(oed_dir, **kwargs)
```

### Comparing `ods_tools-3.0.5/ods_tools/oed/__init__.py` & `ods_tools-3.0.6/ods_tools/oed/__init__.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.5/ods_tools/oed/common.py` & `ods_tools-3.0.6/ods_tools/oed/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     'ReinsScope': ['ReinsNumber', 'PortNumber', 'AccNumber', 'LocNumber']
 }
 
 VALIDATOR_ON_ERROR_ACTION = {'raise', 'log', 'ignore', 'return'}
 DEFAULT_VALIDATION_CONFIG = [
     {'name': 'source_coherence', 'on_error': 'raise'},
     {'name': 'required_fields', 'on_error': 'raise'},
-    {'name': 'unknown_column', 'on_error': 'log'},
+    {'name': 'unknown_column', 'on_error': 'raise'},
     {'name': 'valid_values', 'on_error': 'raise'},
     {'name': 'perils', 'on_error': 'raise'},
     {'name': 'occupancy_code', 'on_error': 'raise'},
     {'name': 'construction_code', 'on_error': 'raise'},
     {'name': 'country_and_area_code', 'on_error': 'raise'},
 ]
```

### Comparing `ods_tools-3.0.5/ods_tools/oed/exposure.py` & `ods_tools-3.0.6/ods_tools/oed/exposure.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.5/ods_tools/oed/forex.py` & `ods_tools-3.0.6/ods_tools/oed/forex.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.5/ods_tools/oed/oed_schema.py` & `ods_tools-3.0.6/ods_tools/oed/oed_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,38 +73,50 @@
                 for area in areas:
                     country_area.add((country, area))
             schema["country_area"] = country_area
 
             return cls(schema, oed_json)
 
     @staticmethod
+    def to_universal_field_name(column: str):
+        """
+        transform column name into string that can be matched directly with the schema field name
+        Args:
+            column (str): name of the column
+        :return:
+            str
+        """
+        return column.strip().lower()
+
+    @staticmethod
     def column_to_field(columns: list, oed_fields: dict, use_generic_flexi=True):
         """
         map column to OED field
 
         Args:
             columns (list): name of the columns in OED file
             oed_fields (dict): all the field in ods_schema
             use_generic_flexi (bool): if true flexi column return the oed_schema name
                                       if false flexi column are just lower cased
         Return:
             dict mapping between exact OED column name and field name in oed_schema
         """
         # support for name different from standard OED column name
-        aliases = {field_info.get('alias').lower(): field_name for field_name, field_info in oed_fields.items() if field_info.get('alias')}
+        aliases = {OedSchema.to_universal_field_name(field_info.get('alias')): field_name for field_name,
+                   field_info in oed_fields.items() if field_info.get('alias')}
         result = {}
         for column in columns:
-            if column.lower() in oed_fields:
-                result[column] = oed_fields[column.lower()]
-            elif column.lower() in aliases:
-                result[column] = oed_fields[aliases[column.lower()]]
+            if OedSchema.to_universal_field_name(column) in oed_fields:
+                result[column] = oed_fields[OedSchema.to_universal_field_name(column)]
+            elif OedSchema.to_universal_field_name(column) in aliases:
+                result[column] = oed_fields[aliases[OedSchema.to_universal_field_name(column)]]
             else:
                 for field_suffix in ['xx', 'zzz']:
-                    for i in range(1, len(column)):
-                        field_name = column.lower()[:-i] + field_suffix
+                    for i in range(1, len(OedSchema.to_universal_field_name(column))):
+                        field_name = OedSchema.to_universal_field_name(column)[:-i] + field_suffix
                         if field_name in oed_fields:
                             if use_generic_flexi:
                                 result[column] = oed_fields[field_name]
                             break
                     else:
                         continue
                     break
```

### Comparing `ods_tools-3.0.5/ods_tools/oed/setting_schema.py` & `ods_tools-3.0.6/ods_tools/oed/setting_schema.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.5/ods_tools/oed/source.py` & `ods_tools-3.0.6/ods_tools/oed/source.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.0.5/ods_tools/oed/validator.py` & `ods_tools-3.0.6/ods_tools/oed/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         log_msg = invalid_data_group.get('log', [])
         return_msg = invalid_data_group.get('return', [])
 
         def invalid_data_to_str(_data):
             return f"in {_data['name']} {_data['source']}\n {_data['msg']}"
 
         for invalid_data in log_msg:
-            logger.info(invalid_data_to_str(invalid_data))
+            logger.warning(invalid_data_to_str(invalid_data))
         if raise_msg:
             raise OdsException('\n'.join(invalid_data_to_str(invalid_data) for invalid_data in raise_msg))
         return return_msg
 
     def check_source_coherence(self):
         """"""
         invalid_data = []
```

### Comparing `ods_tools-3.0.5/ods_tools.egg-info/PKG-INFO` & `ods_tools-3.0.6/ods_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ods-tools
-Version: 3.0.5
+Version: 3.0.6
 Summary: Tools to manage ODS files
 Home-page: https://github.com/OasisLMF/OpenDataStandards
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ods_tools-3.0.5/setup.py` & `ods_tools-3.0.6/setup.py`

 * *Files identical despite different names*

