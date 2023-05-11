# Comparing `tmp/cognite_power_ops-0.2.1.tar.gz` & `tmp/cognite_power_ops-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.2.1.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.2.2.tar", max compression
```

## Comparing `cognite_power_ops-0.2.1.tar` & `cognite_power_ops-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,48 @@
--rw-r--r--   0        0        0    10758 2023-05-10 11:20:08.335871 cognite_power_ops-0.2.1/LICENSE
--rw-r--r--   0        0        0       76 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/__init__.py
--rw-r--r--   0        0        0    10260 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/bootstrap.py
--rw-r--r--   0        0        0    24685 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/config.py
--rw-r--r--   0        0        0        0 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/__init__.py
--rw-r--r--   0        0        0     2686 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/benchmarking_config.py
--rw-r--r--   0        0        0     2984 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/bid_matrix_generator_config.py
--rw-r--r--   0        0        0    13238 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/cdf_resource_collection.py
--rw-r--r--   0        0        0     2513 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/common.py
--rw-r--r--   0        0        0     1390 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/market_config.py
--rw-r--r--   0        0        0    16603 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/plant.py
--rw-r--r--   0        0        0     5114 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/reserve_scenario.py
--rw-r--r--   0        0        0     1218 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/rkom_bid_combination_config.py
--rw-r--r--   0        0        0      994 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/rkom_market_config.py
--rw-r--r--   0        0        0     2113 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/shop_file_config.py
--rw-r--r--   0        0        0     2815 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/shop_output_definition.py
--rw-r--r--   0        0        0     9189 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/time_series_mapping.py
--rw-r--r--   0        0        0     1144 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/transformation.py
--rw-r--r--   0        0        0     1042 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/logger.py
--rw-r--r--   0        0        0     2070 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/main.py
--rw-r--r--   0        0        0        0 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/__init__.py
--rw-r--r--   0        0        0     1936 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/asset_types.py
--rw-r--r--   0        0        0     1424 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/cdf_auth.py
--rw-r--r--   0        0        0     2724 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/cdf_utils.py
--rw-r--r--   0        0        0      744 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/common.py
--rw-r--r--   0        0        0      324 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/constants.py
--rw-r--r--   0        0        0     3271 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/files.py
--rw-r--r--   0        0        0     4979 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/labels.py
--rw-r--r--   0        0        0     1766 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/mapping/mapping.py
--rw-r--r--   0        0        0     2609 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/mapping/static_mapping.py
--rw-r--r--   0        0        0     3165 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/powerops_asset_hierarchy.py
--rw-r--r--   0        0        0      718 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/powerops_status_events.py
--rw-r--r--   0        0        0     4495 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/relationship_types.py
--rw-r--r--   0        0        0    11602 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/resource_generation.py
--rw-r--r--   0        0        0     1495 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/serializer.py
--rw-r--r--   0        0        0       22 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/version.py
--rw-r--r--   0        0        0     1330 2023-05-10 11:20:08.343871 cognite_power_ops-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 cognite_power_ops-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/LICENSE
+-rw-r--r--   0        0        0       76 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0    10260 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/bootstrap.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/__init__.py
+-rw-r--r--   0        0        0      601 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/config_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/dm/__init__.py
+-rw-r--r--   0        0        0     1891 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/dm/client.py
+-rw-r--r--   0        0        0      895 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/dm/schema.graphql
+-rw-r--r--   0        0        0     2005 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/dm/schema.py
+-rw-r--r--   0        0        0      486 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/mapping_client.py
+-rw-r--r--   0        0        0     1173 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/powerops_client.py
+-rw-r--r--   0        0        0      331 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/transformation_client.py
+-rw-r--r--   0        0        0      803 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/watercourse_client.py
+-rw-r--r--   0        0        0    24691 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/config.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/__init__.py
+-rw-r--r--   0        0        0     2686 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/benchmarking_config.py
+-rw-r--r--   0        0        0     2984 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/bid_matrix_generator_config.py
+-rw-r--r--   0        0        0    13238 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/cdf_resource_collection.py
+-rw-r--r--   0        0        0     2513 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/common.py
+-rw-r--r--   0        0        0     1390 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/market_config.py
+-rw-r--r--   0        0        0    16603 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/plant.py
+-rw-r--r--   0        0        0     5114 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/reserve_scenario.py
+-rw-r--r--   0        0        0     1224 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/rkom_bid_combination_config.py
+-rw-r--r--   0        0        0      994 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/rkom_market_config.py
+-rw-r--r--   0        0        0     2113 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/shop_file_config.py
+-rw-r--r--   0        0        0     2815 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/shop_output_definition.py
+-rw-r--r--   0        0        0     9189 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/time_series_mapping.py
+-rw-r--r--   0        0        0     1144 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/transformation.py
+-rw-r--r--   0        0        0     1042 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/logger.py
+-rw-r--r--   0        0        0     2070 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/main.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0     1936 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/asset_types.py
+-rw-r--r--   0        0        0     1424 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/cdf_auth.py
+-rw-r--r--   0        0        0     2724 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/cdf_utils.py
+-rw-r--r--   0        0        0      744 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/common.py
+-rw-r--r--   0        0        0      324 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/constants.py
+-rw-r--r--   0        0        0     3271 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/files.py
+-rw-r--r--   0        0        0     4979 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/labels.py
+-rw-r--r--   0        0        0     1766 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/mapping/mapping.py
+-rw-r--r--   0        0        0     2609 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/mapping/static_mapping.py
+-rw-r--r--   0        0        0     3165 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/powerops_asset_hierarchy.py
+-rw-r--r--   0        0        0      718 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/powerops_status_events.py
+-rw-r--r--   0        0        0     4495 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/relationship_types.py
+-rw-r--r--   0        0        0    11602 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/resource_generation.py
+-rw-r--r--   0        0        0     1495 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/serializer.py
+-rw-r--r--   0        0        0       22 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/version.py
+-rw-r--r--   0        0        0     1330 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 cognite_power_ops-0.2.2/PKG-INFO
```

### Comparing `cognite_power_ops-0.2.1/LICENSE` & `cognite_power_ops-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/bootstrap.py` & `cognite_power_ops-0.2.2/cognite/powerops/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/config.py` & `cognite_power_ops-0.2.2/cognite/powerops/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,15 @@
     def sorted_volumes(self) -> List[int]:
         return sorted(self.reserve_scenarios.volumes)
 
     @property
     def name(self) -> str:
         return (
             f"{self.watercourse}_"
-            f"{self.reserve_scenarios.auction}_"
+            f"{self.reserve_scenarios.auction.value}_"
             f"{self.reserve_scenarios.product}_"
             f"{self.reserve_scenarios.block}_"
             f"{len(self.price_scenarios)}-prices_"
             f"{self.sorted_volumes[1]}MW-{self.sorted_volumes[-1]}MW"
         )
 
     @property
```

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/benchmarking_config.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/benchmarking_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/bid_matrix_generator_config.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/bid_matrix_generator_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/cdf_resource_collection.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/cdf_resource_collection.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/common.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/market_config.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/plant.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/reserve_scenario.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/reserve_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/rkom_bid_combination_config.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/rkom_bid_combination_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     @validator("auction", pre=True)
     def to_enum(cls, value):
         return Auction[value] if isinstance(value, str) else value
 
     @property
     def cdf_asset(self) -> Asset:
-        sequence_external_id = f"RKOM_bid_combination_configuration_{self.auction}_{self.name}"
+        sequence_external_id = f"RKOM_bid_combination_configuration_{self.auction.value}_{self.name}"
 
         return Asset(
             name=sequence_external_id.replace("_", " "),
             description="Defining which RKOM bid methods should be combined (into the total bid form)",
             external_id=sequence_external_id,
             metadata={
                 "bid:auction": self.auction.value,
```

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/rkom_market_config.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/rkom_market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/shop_file_config.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/shop_file_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/shop_output_definition.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/shop_output_definition.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/time_series_mapping.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/time_series_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/data_classes/transformation.py` & `cognite_power_ops-0.2.2/cognite/powerops/data_classes/transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/logger.py` & `cognite_power_ops-0.2.2/cognite/powerops/logger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/main.py` & `cognite_power_ops-0.2.2/cognite/powerops/main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/asset_types.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/asset_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/cdf_auth.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/cdf_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/cdf_utils.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/cdf_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/common.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/files.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/labels.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/mapping/mapping.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/mapping/static_mapping.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/mapping/static_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/powerops_asset_hierarchy.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/powerops_asset_hierarchy.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/powerops_status_events.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/powerops_status_events.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/relationship_types.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/relationship_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/resource_generation.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/resource_generation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/cognite/powerops/utils/serializer.py` & `cognite_power_ops-0.2.2/cognite/powerops/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.1/pyproject.toml` & `cognite_power_ops-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-power-ops"
-version = "0.2.1"
+version = "0.2.2"
 description = "SDK for power markets operations on Cognite Data Fusion"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache 2.0"
 packages = [{include = "cognite", from = "."}]
 
 [tool.black]
 line-length = 120
@@ -32,15 +32,15 @@
 numpy = "^1.23.2"
 strawberry-graphql = "^0.156.4"
 docopt = "^0.6.2"
 cachelib = "^0.10.2"
 retry = "^0.9.2"
 loguru = "^0.6.0"
 deepdiff = "^6.3.0"
-cognite-gql-pygen = "0.4.0"
+cognite-gql-pygen = "0.4.4"
 
 [tool.poetry.scripts]
 powerops = "cognite.powerops.main:main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-regressions = "^2.4.2"
```

### Comparing `cognite_power_ops-0.2.1/PKG-INFO` & `cognite_power_ops-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cognite-power-ops
-Version: 0.2.1
+Version: 0.2.2
 Summary: SDK for power markets operations on Cognite Data Fusion
 License: Apache 2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: arrow (>=1.2.2,<2.0.0)
 Requires-Dist: cachelib (>=0.10.2,<0.11.0)
-Requires-Dist: cognite-gql-pygen (==0.4.0)
+Requires-Dist: cognite-gql-pygen (==0.4.4)
 Requires-Dist: cognite-sdk[pandas] (>=5.9.0,<6.0.0)
 Requires-Dist: deepdiff (>=6.3.0,<7.0.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: msal (>=1.16.0,<2.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
```

