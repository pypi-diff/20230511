# Comparing `tmp/pysigma_backend_microsoft365defender-0.1.3.tar.gz` & `tmp/pysigma_backend_microsoft365defender-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_microsoft365defender-0.1.3.tar", max compression
+gzip compressed data, was "pysigma_backend_microsoft365defender-0.2.0.tar", max compression
```

## Comparing `pysigma_backend_microsoft365defender-0.1.3.tar` & `pysigma_backend_microsoft365defender-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7653 2023-04-24 17:56:47.544492 pysigma_backend_microsoft365defender-0.1.3/LICENSE
--rw-r--r--   0        0        0      626 2023-04-24 17:56:47.544492 pysigma_backend_microsoft365defender-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      407 2023-04-24 17:56:47.544492 pysigma_backend_microsoft365defender-0.1.3/sigma/backends/microsoft365defender/__init__.py
--rw-r--r--   0        0        0    12539 2023-04-24 17:56:47.544492 pysigma_backend_microsoft365defender-0.1.3/sigma/backends/microsoft365defender/microsoft365defender.py
--rw-r--r--   0        0        0      315 2023-04-24 17:56:47.544492 pysigma_backend_microsoft365defender-0.1.3/sigma/pipelines/microsoft365defender/__init__.py
--rw-r--r--   0        0        0    29236 2023-04-24 17:56:47.544492 pysigma_backend_microsoft365defender-0.1.3/sigma/pipelines/microsoft365defender/microsoft365defender.py
--rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 pysigma_backend_microsoft365defender-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7653 2023-05-11 20:17:46.927628 pysigma_backend_microsoft365defender-0.2.0/LICENSE
+-rw-r--r--   0        0        0      626 2023-05-11 20:17:46.927628 pysigma_backend_microsoft365defender-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      407 2023-05-11 20:17:46.927628 pysigma_backend_microsoft365defender-0.2.0/sigma/backends/microsoft365defender/__init__.py
+-rw-r--r--   0        0        0    13077 2023-05-11 20:17:46.927628 pysigma_backend_microsoft365defender-0.2.0/sigma/backends/microsoft365defender/microsoft365defender.py
+-rw-r--r--   0        0        0      315 2023-05-11 20:17:46.927628 pysigma_backend_microsoft365defender-0.2.0/sigma/pipelines/microsoft365defender/__init__.py
+-rw-r--r--   0        0        0    32472 2023-05-11 20:17:46.927628 pysigma_backend_microsoft365defender-0.2.0/sigma/pipelines/microsoft365defender/microsoft365defender.py
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 pysigma_backend_microsoft365defender-0.2.0/PKG-INFO
```

### Comparing `pysigma_backend_microsoft365defender-0.1.3/LICENSE` & `pysigma_backend_microsoft365defender-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_microsoft365defender-0.1.3/pyproject.toml` & `pysigma_backend_microsoft365defender-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-microsoft365defender"
-version = "0.1.3"
+version = "0.2.0"
 description = "pySigma Microsoft 365 Defender backend"
 authors = ["Stephen Lincoln <stephen.lincoln@attackiq.com>"]
 license = "LGPL-3.0-only"
 repository = "https://github.com/AttackIQ/pySigma-backend-microsoft365defender"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_microsoft365defender-0.1.3/sigma/backends/microsoft365defender/microsoft365defender.py` & `pysigma_backend_microsoft365defender-0.2.0/sigma/backends/microsoft365defender/microsoft365defender.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 from sigma.conversion.base import TextQueryBackend
 from sigma.conversion.deferred import DeferredQueryExpression
 from sigma.conditions import ConditionItem, ConditionAND, ConditionOR, ConditionNOT, ConditionFieldEqualsValueExpression
 from sigma.types import SigmaCompareExpression, SigmaString
 from sigma.pipelines.microsoft365defender import microsoft_365_defender_pipeline
 import sigma
 import re
-from typing import ClassVar, Dict, Tuple, Pattern, Any, Union
+from typing import ClassVar, Dict, Tuple, Pattern, Any, Union, Optional
 
 
 class Microsoft365DefenderBackend(TextQueryBackend):
-    """Microsoft 365 Defender KQL Backend"""
-
-    # Automatically apply pipeline
-    backend_processing_pipeline: ClassVar[ProcessingPipeline] = microsoft_365_defender_pipeline()
+    """Microsoft 365 Defender KQL Backend. Automatically applied the microsoft_365_defender_pipeline from
+    sigma.pipelines.microsoft365defender."""
 
     # The backend generates grouping if required
     name: ClassVar[str] = "Microsoft 365 Defender backend"
     formats: Dict[str, str] = {
         "default": "KQL for Microsoft 365 Defender Advanced Hunting queries",
     }
 
@@ -123,23 +121,33 @@
         str] = '_=~{value}'  # Expression for regular expression not bound to a field as format string with placeholder {value}
 
     # Query finalization: appending and concatenating deferred query part
     deferred_start: ClassVar[str] = "\n| "  # String used as separator between main query and deferred parts
     deferred_separator: ClassVar[str] = "\n| "  # String used to join multiple deferred query parts
     deferred_only_query: ClassVar[str] = "*"  # String used as query if final query only contains deferred expression
 
-    # TODO: implement custom methods for query elements not covered by the default backend base.
-    # Documentation: https://sigmahq-pysigma.readthedocs.io/en/latest/Backends.html
-
     # We use =~ for eq_token so everything is case insensitive. But this cannot be used with ints/numbers in queries
     # So we can define a new token to use for SigmaNumeric types and override convert_condition_field_eq_val_num
     # to use it
     num_eq_token: ClassVar[str] = " == "
 
     # Override methods
+    # __init__() to deal with microsoft_365_defender_pipeline params, since it's automatically applied we need to pass
+    # params to __init__()
+    def __init__(self, processing_pipeline: Optional[ProcessingPipeline] = None,
+                 collect_errors: bool = False,
+                 transform_parent_image: bool = True,
+                 **kwargs):
+        super().__init__(processing_pipeline, collect_errors, **kwargs)
+        if self.processing_pipeline:
+            self.processing_pipeline = microsoft_365_defender_pipeline(transform_parent_image) + \
+                                       self.processing_pipeline
+        else:
+            self.processing_pipeline = microsoft_365_defender_pipeline(transform_parent_image)
+
     #  For numeric values, need == instead of =~
     def convert_condition_field_eq_val_num(self, cond: ConditionFieldEqualsValueExpression, state: ConversionState) -> \
             Union[str, DeferredQueryExpression]:
         """Conversion of field = number value expressions"""
         try:
             return self.escape_and_quote_field(cond.field) + self.num_eq_token + str(cond.value)
         except TypeError:  # pragma: no cover
```

### Comparing `pysigma_backend_microsoft365defender-0.1.3/sigma/pipelines/microsoft365defender/microsoft365defender.py` & `pysigma_backend_microsoft365defender-0.2.0/sigma/pipelines/microsoft365defender/microsoft365defender.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from typing import Union, Optional, Iterable
+from collections import defaultdict
 
 from sigma.exceptions import SigmaTransformationError
-from sigma.pipelines.common import logsource_windows_process_creation, \
-    logsource_windows_image_load, logsource_windows_file_event, logsource_windows_file_delete, \
-    logsource_windows_file_change, logsource_windows_file_access, logsource_windows_file_rename, \
-    logsource_windows_registry_set, logsource_windows_registry_add, logsource_windows_registry_delete, \
-    logsource_windows_registry_event, logsource_windows_network_connection
-from sigma.processing.transformations import FieldMappingTransformation, \
-    RuleFailureTransformation, ReplaceStringTransformation, SetStateTransformation, DetectionItemTransformation, \
-    ValueTransformation, DetectionItemFailureTransformation
-from sigma.processing.conditions import IncludeFieldCondition, \
-    RuleProcessingItemAppliedCondition, ExcludeFieldCondition, DetectionItemProcessingItemAppliedCondition
+from sigma.pipelines.common import (logsource_windows_process_creation, logsource_windows_image_load,
+                                    logsource_windows_file_event, logsource_windows_file_delete,
+                                    logsource_windows_file_change, logsource_windows_file_access,
+                                    logsource_windows_file_rename, logsource_windows_registry_set,
+                                    logsource_windows_registry_add, logsource_windows_registry_delete,
+                                    logsource_windows_registry_event, logsource_windows_network_connection)
+from sigma.processing.transformations import (FieldMappingTransformation, RuleFailureTransformation,
+                                              ReplaceStringTransformation, SetStateTransformation,
+                                              DetectionItemTransformation, ValueTransformation,
+                                              DetectionItemFailureTransformation)
+from sigma.processing.conditions import (IncludeFieldCondition, ExcludeFieldCondition,
+                                         DetectionItemProcessingItemAppliedCondition, LogsourceCondition)
 from sigma.conditions import ConditionOR
 from sigma.types import SigmaString, SigmaType
 from sigma.processing.pipeline import ProcessingItem, ProcessingPipeline
 from sigma.rule import SigmaDetectionItem, SigmaDetection
-from collections import defaultdict
 
 
 # CUSTOM TRANSFORMATIONS
 ## Custom DetectionItemTransformation to split domain and user, if applicable
 class SplitDomainUserTransformation(DetectionItemTransformation):
     """Custom DetectionItemTransformation transformation to split a User field into separate domain and user fields,
     if applicable.  This is to handle the case where the Sysmon `User` field may contain a domain AND username, and
@@ -116,14 +118,29 @@
     def apply_value(self, field: str, val: SigmaType) -> Optional[Union[SigmaType, Iterable[SigmaType]]]:
         mapped_vals = self.value_mappings.get(val.to_plain(), val.to_plain())
         if isinstance(mapped_vals, list):
             return [SigmaString(v) for v in mapped_vals]
         return SigmaString(mapped_vals)
 
 
+# Extract parent process name from ParentImage after applying ParentImage field mapping
+class ParentImageValueTransformation(ValueTransformation):
+    """Custom ValueTransformation transformation.  Unfortunately, none of the table schemas have
+    InitiatingProcessParentFolderPath like they do InitiatingProcessFolderPath. Due to this, we cannot directly map the
+    Sysmon `ParentImage` field to a table field. However, InitiatingProcessParentFileName is an available field in
+    nearly all tables, so we will extract the process name and use that instead.
+
+    Use this transformation BEFORE mapping ParentImage to InitiatingProcessFileName
+    """
+
+    def apply_value(self, field: str, val: SigmaType) -> Optional[Union[SigmaType, Iterable[SigmaType]]]:
+        parent_process_name = str(val.to_plain().split("\\")[-1].split("/")[-1])
+        return SigmaString(parent_process_name)
+
+
 class InvalidFieldTransformation(DetectionItemFailureTransformation):
     """
     Overrides the apply_detection_item() method from DetectionItemFailureTransformation to also include the field name
     in the error message
     """
 
     def apply_detection_item(self, detection_item: SigmaDetectionItem) -> None:
@@ -331,14 +348,17 @@
                             'InitiatingProcessFolderPath', 'InitiatingProcessParentFileName',
                             'InitiatingProcessParentId', 'InitiatingProcessParentCreationTime',
                             'InitiatingProcessAccountDomain', 'InitiatingProcessAccountName',
                             'InitiatingProcessAccountSid', 'InitiatingProcessAccountUpn',
                             'InitiatingProcessAccountObjectId', 'InitiatingProcessIntegrityLevel',
                             'InitiatingProcessTokenElevation', 'ReportId', 'AppGuardContainerId', 'AdditionalFields']}
 
+# Mapping from ParentImage to InitiatingProcessParentFileName. Must be used alongside of ParentImageValueTransformation
+parent_image_field_mapping = {'ParentImage': 'InitiatingProcessParentFileName'}
+
 # OTHER MAPPINGS
 ## useful for creating ProcessingItems() with list comprehension
 
 ## Query Table names -> rule categories
 table_to_category_mappings = {
     'DeviceProcessEvents': ['process_creation'],
     'DeviceImageLoadEvents': ['image_load'],
@@ -403,14 +423,15 @@
         DetectionItemProcessingItemAppliedCondition(f"microsoft_365_defender_fieldmappings_{table_name}")
         for table_name in table_to_category_mappings.keys()
     ],
     detection_item_condition_linking=any,
     detection_item_condition_negation=True,
 )
 ]
+
 ## Field Value Replacements ProcessingItems
 replacement_proc_items = [
     # Sysmon uses abbreviations in RegistryKey values, replace with full key names as the DeviceRegistryEvents schema
     # expects them to be
     # Note: Ensure this comes AFTER field mapping renames, as we're specifying DeviceRegistryEvent fields
     #
     # Do this one first, or else the HKLM only one will replace HKLM and mess up the regex
@@ -452,14 +473,42 @@
     ProcessingItem(
         identifier="microsoft_365_defender_hashes_field_values",
         transformation=HashesValuesTransformation(),
         field_name_conditions=[IncludeFieldCondition(['Hashes'])]
     ),
 ]
 
+# ParentImage -> InitiatingProcessParentFileName
+parent_image_proc_items = [
+    # First apply fieldmapping from ParentImage to InitiatingProcessParentFileName for non process-creation rules
+    ProcessingItem(
+        identifier="microsoft_365_defender_parent_image_fieldmapping",
+        transformation=FieldMappingTransformation(parent_image_field_mapping),
+        rule_conditions=[
+            # Exclude process_creation events, there's direct field mapping in this schema table
+            LogsourceCondition(category='process_creation')
+        ],
+        rule_condition_negation=True
+    ),
+    # Second, extract the parent process name from the full path
+    ProcessingItem(
+        identifier="microsoft_365_defender_parent_image_name_value",
+        transformation=ParentImageValueTransformation(),
+        field_name_conditions=[
+            IncludeFieldCondition(["InitiatingProcessParentFileName"]),
+        ],
+        rule_conditions=[
+            # Exclude process_creation events, there's direct field mapping in this schema table
+            LogsourceCondition(category='process_creation')
+        ],
+        rule_condition_negation=True
+    )
+
+]
+
 ## Exceptions/Errors ProcessingItems
 rule_error_proc_items = [
     # Category Not Supported
     ProcessingItem(
         identifier="microsoft_365_defender_unsupported_rule_category",
         rule_condition_linking=any,
         transformation=RuleFailureTransformation(
@@ -487,25 +536,40 @@
         ],
         rule_condition_linking=any,
     )
     for table_name, table_fields in valid_fields_per_table.items()
 ]
 
 
-def microsoft_365_defender_pipeline() -> ProcessingPipeline:
+def microsoft_365_defender_pipeline(transform_parent_image: Optional[bool] = True) -> ProcessingPipeline:
     """Pipeline for transformations for SigmaRules to use in the Microsoft 365 Defender Backend
     Field mappings based on documentation found here:
     https://learn.microsoft.com/en-us/microsoft-365/security/defender/advanced-hunting-query-language?view=o365-worldwide
+
+    :param transform_parent_image: If True, the ParentImage field will be mapped to InitiatingProcessParentFileName, and
+    the parent process name in the ParentImage will be extracted and used. This is because the Microsoft 365 Defender
+    table schema does not contain a InitiatingProcessParentFolderPath field like it does for InitiatingProcessFolderPath.
+    i.e. ParentImage: C:\\Windows\\System32\\whoami.exe -> InitiatingProcessParentFileName: whoami.exe.
+    Defaults to True
+    :type transform_parent_image: Optional[bool]
+
     :return: ProcessingPipeline for Microsoft 365 Defender Backend
     :rtype: ProcessingPipeline
     """
+
+    pipeline_items = [
+        *query_table_proc_items,
+        *fieldmappings_proc_items,
+        *generic_field_mappings_proc_item,
+        *replacement_proc_items,
+        *rule_error_proc_items,
+        *field_error_proc_items,
+    ]
+
+    if transform_parent_image:
+        pipeline_items[4:4] = parent_image_proc_items
+
     return ProcessingPipeline(
         name="Generic Log Sources to Windows 365 Defender Transformation",
         priority=10,
-        items=[*query_table_proc_items,
-               *fieldmappings_proc_items,
-               *generic_field_mappings_proc_item,
-               *replacement_proc_items,
-               *rule_error_proc_items,
-               *field_error_proc_items,
-               ]
+        items=pipeline_items,
     )
```

### Comparing `pysigma_backend_microsoft365defender-0.1.3/PKG-INFO` & `pysigma_backend_microsoft365defender-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-microsoft365defender
-Version: 0.1.3
+Version: 0.2.0
 Summary: pySigma Microsoft 365 Defender backend
 Home-page: https://github.com/AttackIQ/pySigma-backend-microsoft365defender
 License: LGPL-3.0-only
 Author: Stephen Lincoln
 Author-email: stephen.lincoln@attackiq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

