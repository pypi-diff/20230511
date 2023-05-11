# Comparing `tmp/ssb_sgis-0.1.8.tar.gz` & `tmp/ssb_sgis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.1.8.tar", max compression
+gzip compressed data, was "ssb_sgis-0.1.9.tar", max compression
```

## Comparing `ssb_sgis-0.1.8.tar` & `ssb_sgis-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0     1074 2023-04-16 18:53:28.316596 ssb_sgis-0.1.8/LICENSE
--rw-r--r--   0        0        0     7263 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/README.md
--rw-r--r--   0        0        0     2477 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1651 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/__init__.py
--rw-r--r--   0        0        0     2634 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/dapla.py
--rw-r--r--   0        0        0      666 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8776 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    27637 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5480 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    34770 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/geopandas_tools/line_operations.py
--rw-r--r--   0        0        0    16647 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    14435 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6316 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0     5046 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0     2468 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/helpers.py
--rw-r--r--   0        0        0        0 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0    19154 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/maps/explore.py
--rw-r--r--   0        0        0    20499 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    16711 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/maps/map.py
--rw-r--r--   0        0        0    12747 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    13848 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0        0 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     6119 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2455 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4182 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4416 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    11306 2023-04-16 18:53:43.241504 ssb_sgis-0.1.8/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0    23771 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0     6124 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/networkanalysis/network_norway.py
--rw-r--r--   0        0        0    63500 2023-04-16 18:53:43.241504 ssb_sgis-0.1.8/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12692 2023-04-16 18:53:28.356598 ssb_sgis-0.1.8/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0        0 2023-04-16 18:53:28.356598 ssb_sgis-0.1.8/src/sgis/py.typed
--rw-r--r--   0        0        0     3765 2023-04-16 18:53:28.356598 ssb_sgis-0.1.8/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8627 1970-01-01 00:00:00.000000 ssb_sgis-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-18 12:55:23.109640 ssb_sgis-0.1.9/LICENSE
+-rw-r--r--   0        0        0     7332 2023-04-18 12:55:38.209936 ssb_sgis-0.1.9/README.md
+-rw-r--r--   0        0        0     2477 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1854 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/__init__.py
+-rw-r--r--   0        0        0     2634 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/dapla.py
+-rw-r--r--   0        0        0      666 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0     8776 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    27637 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5480 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    16647 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    14812 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6316 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0     5046 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0     2468 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0    19154 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0    20499 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    16711 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    12875 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    13848 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0        0 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     6199 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2017 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4182 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4487 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    12639 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/closing_network_holes.py
+-rw-r--r--   0        0        0    12096 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/cutting_lines.py
+-rw-r--r--   0        0        0     9247 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0     3438 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/finding_isolated_networks.py
+-rw-r--r--   0        0        0     8242 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0    62946 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12439 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0     6740 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/nodes.py
+-rw-r--r--   0        0        0        0 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/py.typed
+-rw-r--r--   0        0        0     3765 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/read_parquet.py
+-rw-r--r--   0        0        0     8696 1970-01-01 00:00:00.000000 ssb_sgis-0.1.9/PKG-INFO
```

### Comparing `ssb_sgis-0.1.8/LICENSE` & `ssb_sgis-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/README.md` & `ssb_sgis-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 [python version]: https://pypi.org/project/ssb-sgis
 [read the docs]: https://ssb-sgis.readthedocs.io/
 [tests]: https://github.com/statisticsnorway/ssb-sgis/actions?workflow=Tests
 [coverage]: https://sonarcloud.io/component_measures?metric=coverage&id=statisticsnorway_ssb-sgis
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
-sgis builds on the geopandas package and provides functions that make it easier to do advanced GIS in python.
+sgis builds on the geopandas package and provides functions that make it easier to do GIS in python.
 Features include network analysis, functions for exploring multiple GeoDataFrames in a layered interactive map,
 and vector operations like finding k-nearest neighbours, splitting lines by points, snapping and closing holes
 in polygons by size.
 
 ## Network analysis examples
 
 Preparing for network analysis:
@@ -36,34 +36,33 @@
 import sgis as sg
 import pandas as pd
 
 roads = sg.read_parquet_url(
     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet"
 )
 
-nw = (
-    sg.DirectedNetwork(roads)
-    .remove_isolated()
-    .make_directed_network(
-        direction_col="oneway",
-        direction_vals_bft=("B", "FT", "TF"),
-        minute_cols=("drivetime_fw", "drivetime_bw"),
-    )
+connected_roads = sg.get_connected_components(roads).query("connected == 1")
+
+directed_roads = sg.make_directed_network(
+    connected_roads,
+    direction_col="oneway",
+    direction_vals_bft=("B", "FT", "TF"),
+    minute_cols=("drivetime_fw", "drivetime_bw"),
 )
 
-rules = sg.NetworkAnalysisRules(weight="minutes")
+rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
 
-nwa = sg.NetworkAnalysis(network=nw, rules=rules)
+nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules)
 
 nwa
 ```
 
     NetworkAnalysis(
         network=DirectedNetwork(6364 km, percent_bidirectional=87),
-        rules=NetworkAnalysisRules(weight=minutes, search_tolerance=250, search_factor=0, split_lines=False, ...),
+        rules=NetworkAnalysisRules(weight=minutes, directed=True, search_tolerance=250, search_factor=0, split_lines=False, ...),
         log=True, detailed_log=True,
     )
 
 Get number of times each line segment was visited, with optional weighting.
 
 ```python
 origins = points.iloc[:75]
```

### Comparing `ssb_sgis-0.1.8/pyproject.toml` & `ssb_sgis-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.1.8"
+version = "0.1.9"
 description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
```

### Comparing `ssb_sgis-0.1.8/src/sgis/__init__.py` & `ssb_sgis-0.1.9/src/sgis/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,41 +18,50 @@
     to_multipoint,
 )
 from .geopandas_tools.geometry_types import (
     get_geom_type,
     is_single_geom_type,
     to_single_geom_type,
 )
-from .geopandas_tools.line_operations import (
-    close_network_holes,
-    close_network_holes_to_deadends,
-    cut_lines,
-    cut_lines_once,
-    get_component_size,
-    get_largest_component,
-    make_edge_coords_cols,
-    make_edge_wkt_cols,
-    make_node_ids,
-    split_lines_by_nearest_point,
-)
 from .geopandas_tools.neighbors import (
     get_all_distances,
     get_k_nearest_neighbors,
     get_neighbor_indices,
 )
 from .geopandas_tools.overlay import clean_shapely_overlay, overlay, overlay_update
 from .geopandas_tools.point_operations import snap_all, snap_within_distance
 from .geopandas_tools.polygon_operations import close_all_holes, close_small_holes
 from .maps.legend import Legend
 from .maps.maps import clipmap, explore, qtm, samplemap
 from .maps.thematicmap import ThematicMap
-from .networkanalysis.directednetwork import DirectedNetwork
+from .networkanalysis.closing_network_holes import (
+    close_network_holes,
+    close_network_holes_to_deadends,
+)
+from .networkanalysis.cutting_lines import (
+    cut_lines,
+    cut_lines_once,
+    split_lines_by_nearest_point,
+)
+from .networkanalysis.directednetwork import (
+    make_directed_network,
+    make_directed_network_norway,
+)
+from .networkanalysis.finding_isolated_networks import (
+    get_component_size,
+    get_connected_components,
+)
 from .networkanalysis.network import Network
 from .networkanalysis.networkanalysis import NetworkAnalysis
 from .networkanalysis.networkanalysisrules import NetworkAnalysisRules
+from .networkanalysis.nodes import (
+    make_edge_coords_cols,
+    make_edge_wkt_cols,
+    make_node_ids,
+)
 from .read_parquet import read_parquet_url
 
 
 try:
     from .dapla import exists, read_geopandas, write_geopandas
 except ImportError:
     pass
```

### Comparing `ssb_sgis-0.1.8/src/sgis/dapla.py` & `ssb_sgis-0.1.9/src/sgis/dapla.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/exceptions.py` & `ssb_sgis-0.1.9/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.1.9/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.1.9/src/sgis/geopandas_tools/general.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.1.9/src/sgis/geopandas_tools/geometry_types.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.1.9/src/sgis/geopandas_tools/neighbors.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.1.9/src/sgis/geopandas_tools/overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,26 @@
             or a tuple/list with geom_type for df1 and df2 respectfully.
         **kwargs: Additional keyword arguments passed to geopandas.overlay
 
     Returns:
         GeoDataFrame with overlayed geometries and columns from both GeoDataFrames.
 
     """
+    geom_type_left, geom_type_right = _get_geom_type_left_right(geom_type)
+
+    if keep_geom_type and not geom_type_left:
+        geom_type_left = get_geom_type(df1)
+
+    df1 = clean_geoms(df1)
+    if geom_type_left:
+        df1 = to_single_geom_type(df1, geom_type_left)
+    df2 = clean_geoms(df2)
+    if geom_type_right:
+        df2 = to_single_geom_type(df2, geom_type_right)
+
     try:
         overlayed = df1.overlay(df2, how="difference", **kwargs)
     except GEOSException:
         overlayed = clean_shapely_overlay(
             df1,
             df2,
             how="difference",
@@ -218,46 +230,49 @@
 
     geom_type_left, geom_type_right = _get_geom_type_left_right(geom_type)
 
     if keep_geom_type and not geom_type_left:
         geom_type_left = get_geom_type(df1)
 
     df1 = clean_geoms(df1)
+    df2 = clean_geoms(df2)
+
     if geom_type_left:
         df1 = to_single_geom_type(df1, geom_type_left)
-    df2 = clean_geoms(df2)
     if geom_type_right:
         df2 = to_single_geom_type(df2, geom_type_right)
 
     df1 = df1.explode(ignore_index=True)
     df2 = df2.explode(ignore_index=True)
 
     overlayed = _shapely_overlay(df1, df2, how=how).pipe(clean_geoms)
+
     if geom_type_left:
         overlayed = to_single_geom_type(overlayed, geom_type_left)
 
     return overlayed.reset_index(drop=True)
 
 
 def _get_geom_type_left_right(
     geom_type: str | tuple | list | None,
 ) -> tuple[str | None, str | None]:
-    if isinstance(geom_type, (tuple, list)):
+    if isinstance(geom_type, str):
+        return geom_type, geom_type
+    elif geom_type is None:
+        return None, None
+
+    elif hasattr(geom_type, "__iter__"):
         if len(geom_type) == 1:
             return geom_type[0], geom_type[0]
         elif len(geom_type) == 2:
             return geom_type
         else:
             raise ValueError(
                 "'geom_type' should be one or two strings for the left and right gdf"
             )
-    elif isinstance(geom_type, str):
-        return geom_type, geom_type
-    elif geom_type is None:
-        return None, None
     else:
         raise ValueError(
             "'geom_type' should be one or two strings for the left and right gdf"
         )
 
 
 def _shapely_overlay(df1: GeoDataFrame, df2: GeoDataFrame, how: str) -> GeoDataFrame:
```

### Comparing `ssb_sgis-0.1.8/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.1.9/src/sgis/geopandas_tools/point_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-0.1.9/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/helpers.py` & `ssb_sgis-0.1.9/src/sgis/helpers.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/maps/explore.py` & `ssb_sgis-0.1.9/src/sgis/maps/explore.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/maps/legend.py` & `ssb_sgis-0.1.9/src/sgis/maps/legend.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/maps/map.py` & `ssb_sgis-0.1.9/src/sgis/maps/map.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/maps/maps.py` & `ssb_sgis-0.1.9/src/sgis/maps/maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,14 +268,17 @@
             clipped = clipped + (clipped_,)
 
     else:
         for gdf in gdfs[:-1]:
             clipped_ = gdf.clip(gdfs[-1])
             clipped = clipped + (clipped_,)
 
+    if not any(len(gdf) for gdf in clipped):
+        raise ValueError("None of the GeoDataFrames are within the mask extent.")
+
     if explore:
         m = Explore(
             *clipped,
             column=column,
             labels=labels,
             show_in_browser=show_in_browser,
             max_zoom=max_zoom,
```

### Comparing `ssb_sgis-0.1.8/src/sgis/maps/thematicmap.py` & `ssb_sgis-0.1.9/src/sgis/maps/thematicmap.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-0.1.9/src/sgis/networkanalysis/_get_route.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,61 @@
 import warnings
 
-import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
 from igraph import Graph
 from pandas import DataFrame
 
 
+def _get_route_frequencies(
+    graph,
+    roads: GeoDataFrame,
+    weight_df: DataFrame,
+) -> GeoDataFrame:
+    """Function used in the get_route_frequencies method of NetworkAnalysis."""
+    warnings.filterwarnings("ignore", category=RuntimeWarning)
+
+    resultlist: list[DataFrame] = []
+
+    od_pairs = weight_df.index
+
+    for ori_id in od_pairs.get_level_values(0).unique():
+        relevant_pairs = od_pairs[od_pairs.get_level_values(0) == ori_id]
+        destinations = relevant_pairs.get_level_values(1)
+
+        res = graph.get_shortest_paths(
+            weights="weight", v=ori_id, to=destinations, output="epath"
+        )
+
+        for i, des_id in enumerate(destinations):
+            indices = graph.es[res[i]]
+
+            if not indices:
+                continue
+
+            line_ids = DataFrame({"src_tgt_wt": indices["src_tgt_wt"]})
+            line_ids["origin"] = ori_id
+            line_ids["destination"] = des_id
+            line_ids["multiplier"] = weight_df.loc[ori_id, des_id].iloc[0]
+
+            resultlist.append(line_ids)
+
+    summarised: pd.Series = (
+        pd.concat(resultlist, ignore_index=True)
+        .groupby("src_tgt_wt")["multiplier"]
+        .sum()
+    )
+
+    roads["frequency"] = roads["src_tgt_wt"].map(summarised)
+
+    roads_visited = roads.loc[roads.frequency.notna()].drop("src_tgt_wt", axis=1)
+
+    return roads_visited
+
+
 def _get_route(
     graph: Graph,
     weight: str,
     roads: GeoDataFrame,
     od_pairs: pd.MultiIndex,
 ) -> GeoDataFrame:
     """Function used in the get_route method of NetworkAnalysis."""
@@ -88,79 +133,17 @@
     lines = lines.dissolve(
         by=["origin", "destination", "k"], aggfunc="sum", as_index=False
     )
 
     return lines[["origin", "destination", weight, "k", "geometry"]]
 
 
-def _get_route_frequencies(
-    graph,
-    roads: GeoDataFrame,
-    weight_df: DataFrame,
-):
-    """Function used in the get_route_frequencies method of NetworkAnalysis."""
-    warnings.filterwarnings("ignore", category=RuntimeWarning)
-
-    resultlist: list[DataFrame] = []
-
-    od_pairs = weight_df.index
-
-    for ori_id in od_pairs.get_level_values(0).unique():
-        relevant_pairs = od_pairs[od_pairs.get_level_values(0) == ori_id]
-        destinations = relevant_pairs.get_level_values(1)
-
-        res = graph.get_shortest_paths(
-            weights="weight", v=ori_id, to=destinations, output="epath"
-        )
-
-        for i, des_id in enumerate(destinations):
-            indices = graph.es[res[i]]
-
-            if not indices:
-                continue
-
-            line_ids = DataFrame({"src_tgt_wt": indices["src_tgt_wt"]})
-            line_ids["origin"] = ori_id
-            line_ids["destination"] = des_id
-            line_ids["multiplier"] = weight_df.loc[ori_id, des_id].iloc[0]
-
-            resultlist.append(line_ids)
-
-    summarised = (
-        pd.concat(resultlist, ignore_index=True)
-        .groupby("src_tgt_wt")["multiplier"]
-        .sum()
-    )
-
-    roads["frequency"] = roads["src_tgt_wt"].map(summarised)
-
-    roads_visited = roads.loc[roads.frequency.notna()].drop("src_tgt_wt", axis=1)
-
-    return roads_visited
-
-
-def _get_line_geometries(line_ids, roads, weight) -> GeoDataFrame:
-    road_mapper = roads.set_index(["src_tgt_wt"])[[weight, "geometry"]]
-    line_ids = line_ids.join(road_mapper)
-    return GeoDataFrame(line_ids, geometry="geometry", crs=roads.crs)
-
-
-def _create_line_id_df(src_tgt_wt: list, ori_id, des_id) -> DataFrame:
-    line_ids = DataFrame(index=src_tgt_wt)
-
-    # remove edges from ori/des to the roads
-    line_ids = line_ids.loc[~line_ids.index.str.endswith("_0")]
-
-    line_ids["origin"] = ori_id
-    line_ids["destination"] = des_id
-
-    return line_ids
-
-
-def _loop_k_routes(graph: Graph, ori_id, des_id, k, drop_middle_percent) -> DataFrame:
+def _loop_k_routes(
+    graph: Graph, ori_id: str, des_id: str, k: int, drop_middle_percent: int
+) -> DataFrame:
     """Workaround for igraph's get_k_shortest_paths.
 
     igraph's get_k_shorest_paths doesn't seem to work (gives just the same path k
     times), so doing it manually. Run _get_one_route, then remove the edges in the
     middle of the route, given with drop_middle_percent, repeat k times.
     """
     graph = graph.copy()
@@ -194,7 +177,27 @@
         to_be_dropped = edge_tuples[n_edges_to_keep:-n_edges_to_keep]
         graph.delete_edges(to_be_dropped)
 
     if lines:
         return pd.concat(lines)
     else:
         return pd.DataFrame()
+
+
+def _get_line_geometries(
+    line_ids: DataFrame, roads: GeoDataFrame, weight: str
+) -> GeoDataFrame:
+    road_mapper = roads.set_index(["src_tgt_wt"])[[weight, "geometry"]]
+    line_ids = line_ids.join(road_mapper)
+    return GeoDataFrame(line_ids, geometry="geometry", crs=roads.crs)
+
+
+def _create_line_id_df(src_tgt_wt: list, ori_id: str, des_id: str) -> DataFrame:
+    line_ids = DataFrame(index=src_tgt_wt)
+
+    # remove edges from ori/des to the roads
+    line_ids = line_ids.loc[~line_ids.index.str.endswith("_0")]
+
+    line_ids["origin"] = ori_id
+    line_ids["destination"] = des_id
+
+    return line_ids
```

### Comparing `ssb_sgis-0.1.8/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.1.9/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,23 +12,26 @@
     origins: GeoDataFrame,
     destinations: GeoDataFrame,
     weight: str,
     *,
     lines: bool = False,
     rowwise: bool = False,
 ) -> DataFrame | GeoDataFrame:
-    distances: list[list[str]] = graph.distances(
+    assert origins.index.name == "temp_idx"
+    assert destinations.index.name == "temp_idx"
+
+    distances: list[list[float]] = graph.distances(
         weights="weight",
-        source=origins["temp_idx"],
-        target=destinations["temp_idx"],
+        source=origins.index,
+        target=destinations.index,
     )
 
     ori_idx, des_idx, costs = [], [], []
-    for i, f_idx in enumerate(origins["temp_idx"]):
-        for j, t_idx in enumerate(destinations["temp_idx"]):
+    for i, f_idx in enumerate(origins.index):
+        for j, t_idx in enumerate(destinations.index):
             ori_idx.append(f_idx)
             des_idx.append(t_idx)
             costs.append(distances[i][j])
 
     results = (
         pd.DataFrame(data={"origin": ori_idx, "destination": des_idx, weight: costs})
         .replace([np.inf, -np.inf], np.nan)
@@ -36,38 +39,26 @@
     )
 
     # calculating all-to-all distances is much faster than looping rowwise,
     # so filtering to rowwise afterwards instead
     if rowwise:
         rowwise_df = DataFrame(
             {
-                "origin": origins["temp_idx"].reset_index(drop=True),
-                "destination": destinations["temp_idx"].reset_index(drop=True),
+                "origin": origins.index,
+                "destination": destinations.index,
             }
         )
         results = rowwise_df.merge(results, on=["origin", "destination"], how="left")
 
-    wkt_dict_origin = {
-        idx: geom.wkt
-        for idx, geom in zip(origins["temp_idx"], origins.geometry, strict=True)
-    }
-    wkt_dict_destination = {
-        idx: geom.wkt
-        for idx, geom in zip(
-            destinations["temp_idx"], destinations.geometry, strict=True
-        )
-    }
-    results["wkt_ori"] = results["origin"].map(wkt_dict_origin)
-    results["wkt_des"] = results["destination"].map(wkt_dict_destination)
+    results["wkt_ori"] = results["origin"].map(origins.geometry)
+    results["wkt_des"] = results["destination"].map(destinations.geometry)
 
-    results[weight] = np.where(results.wkt_ori == results.wkt_des, 0, results[weight])
+    results.loc[results.wkt_ori == results.wkt_des, weight] = 0
 
     # straight lines between origin and destination
     if lines:
-        origin = gpd.GeoSeries.from_wkt(results["wkt_ori"], crs=25833)
-        destination = gpd.GeoSeries.from_wkt(results["wkt_des"], crs=25833)
-        results["geometry"] = shortest_line(origin, destination)
+        results["geometry"] = shortest_line(results["wkt_ori"], results["wkt_des"])
         results = gpd.GeoDataFrame(results, geometry="geometry", crs=25833)
 
     results = results.drop(["wkt_ori", "wkt_des"], axis=1, errors="ignore")
 
     return results.reset_index(drop=True)
```

### Comparing `ssb_sgis-0.1.8/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.1.9/src/sgis/networkanalysis/_points.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.1.9/src/sgis/networkanalysis/_service_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
 from igraph import Graph
 from shapely import force_2d, reverse
 
-from ..geopandas_tools.line_operations import cut_lines_once, make_edge_wkt_cols
+from .cutting_lines import cut_lines_once
+from .nodes import make_edge_wkt_cols
 
 
 def _service_area(
     graph: Graph,
     origins: GeoDataFrame,
     weight: str,
     breaks: np.ndarray,
     lines: GeoDataFrame,
     nodes: GeoDataFrame,
     directed: bool,
     precice: bool,
 ) -> GeoDataFrame:
     # make sure the nodes are alligned with the vertices in the graph
+    # the weight/distances can then be assigned directly onto the nodes
     node_df = pd.DataFrame(index=np.array(graph.vs["name"]))
     nodes = nodes.set_index("node_id").drop("geometry", axis=1)
     nodes = node_df.join(nodes)
 
     # double edge df with source/target as index
     edge_df = lines.loc[:, ["source", "target", "src_tgt_wt", "geometry"]]
     edge_df = pd.concat(
@@ -35,15 +37,15 @@
     all_distances: list[list[str]] = graph.distances(
         weights="weight", source=origins["temp_idx"], mode="out"
     )
 
     # loop through every origin and every break
     service_areas: list[GeoDataFrame] = []
     for i, idx in enumerate(origins["temp_idx"]):
-        # assign distances to the nodes and give the column to the edges
+        # assign distances to the nodes and join the column to the edges
         nodes[weight] = all_distances[i]
         distance_df = edge_df.join(nodes)
 
         for break_ in breaks:
             nodes_within_break = nodes.loc[nodes[weight] <= break_]
 
             whole_edge_is_within = (edge_df.source.isin(nodes_within_break.index)) & (
```

### Comparing `ssb_sgis-0.1.8/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.1.9/src/sgis/networkanalysis/networkanalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,30 +13,29 @@
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
 from igraph import Graph
 from pandas import DataFrame
 
 from ..geopandas_tools.general import _push_geom_col
-from ..geopandas_tools.line_operations import split_lines_by_nearest_point
 from ._get_route import _get_k_routes, _get_route, _get_route_frequencies
 from ._od_cost_matrix import _od_cost_matrix
 from ._points import Destinations, Origins
 from ._service_area import _service_area
-from .directednetwork import DirectedNetwork
+from .cutting_lines import split_lines_by_nearest_point
 from .network import Network
 from .networkanalysisrules import NetworkAnalysisRules
 
 
 class NetworkAnalysis:
     """Class for doing network analysis.
 
-    The class takes a (Directed)Network and rules for the analyses
-    (NetworkAnalysisRules), and holds methods for doing network analysis
-    based on GeoDataFrames of origin and destination points.
+    The class takes a GeoDataFrame of line geometries and rules for the analyses,
+    and holds methods for doing network analysis based on GeoDataFrames of origin
+    and destination points.
 
     The 'od_cost_matrix' method is the fastest, and returns a DataFrame with only
     indices and travel costs between each origin-destination pair.
 
     The 'get_route' method does the same, but also returns the line geometry of the
     routes. 'get_k_routes' can be used to find multiple routes between each OD pair.
 
@@ -44,98 +43,83 @@
     can be reached within one or more breaks.
 
     The 'get_route_frequencies' method is a bit different. It returns the individual
     line segments that were visited with an added column for how many times the
     segments were used.
 
     Args:
-        network: either the base Network class or a subclass, chiefly the
-            DirectedNetwork class. The network can be customized beforehand, or
-            accessed through the 'network' attribute of this class.
-        rules: NetworkAnalysisRules class instance.
+        network: A GeoDataFrame of line geometries.
+        rules: The rules for the analysis, either as an instance of
+            NetworkAnalysisRules or a dictionary with the parameters
+            as keys.
         log: If True (default), a DataFrame with information about each
             analysis run will be stored in the 'log' attribute.
-        detailed_log: If True (default), the log DataFrame will include columns for
-            all arguments held by the NetworkAnalysisRules class and the analysis
-            method used. Will also include standard deviation, 25th, 50th and 75th
-            percentile of the weight column in the results.
+        detailed_log: If True, the log DataFrame will include columns for
+            all arguments passed to the analysis method, plus standard deviation and
+            percentiles (25th, 50th, 75th) of the weight column in the results.
+            Defaults to False.
 
     Attributes:
-        network: The Network instance.
-        rules: The NetworkAnalysisRules instance.
+        network: A Network instance that holds the lines and nodes (points) of the
+            GeoDataFrame of line geometries.
+        rules: NetworkAnalysisRules instance.
         log: A DataFrame with information about each analysis run.
 
-    See also
-    --------
-    DirectedNetwork : For customising and optimising line data before directed network
-        analysis.
-
-    Network : For customising and optimising line data before undirected network
-        analysis.
-
     Examples
     --------
     Read example data.
 
     >>> import sgis as sg
     >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
 
-    Creating a NetworkAnalysis class instance.
+    Preparing the lines for directed network analysis.
+
+    >>> connected_roads = sg.get_connected_components(roads).query("connected == 1")
 
-    >>> nw = (
-    ...     sg.DirectedNetwork(roads)
-    ...     .remove_isolated()
-    ...     .make_directed_network(
-    ...         direction_col="oneway",
-    ...         direction_vals_bft=("B", "FT", "TF"),
-    ...         minute_cols=("drivetime_fw", "drivetime_bw"),
-    ...     )
+    >>> directed_roads = sg.make_directed_network(
+    ...     connected_roads,
+    ...     direction_col="oneway",
+    ...     direction_vals_bft=("B", "FT", "TF"),
+    ...     minute_cols=("drivetime_fw", "drivetime_bw"),
     ... )
+
     >>> rules = sg.NetworkAnalysisRules(weight="minutes")
-    >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
+    >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
     >>> nwa
     NetworkAnalysis(
         network=DirectedNetwork(6364 km, percent_bidirectional=87),
-        rules=NetworkAnalysisRules(weight=minutes, search_tolerance=250, search_factor=0, split_lines=False, ...),
+        rules=NetworkAnalysisRules(weight=minutes, directed=True, search_tolerance=250, search_factor=0, split_lines=False, ...),
         log=True, detailed_log=True,
     )
 
-    Now it's ready for network analysis.
+    Now we're ready for network analysis.
 
     """
 
     def __init__(
         self,
-        network: Network | DirectedNetwork,
-        rules: NetworkAnalysisRules,
+        network: GeoDataFrame,
+        rules: NetworkAnalysisRules | dict,
         log: bool = True,
-        detailed_log: bool = True,
+        detailed_log: bool = False,
     ):
-        self.network = network
-        self.rules = rules
-        self._log = log
-        self.detailed_log = detailed_log
-
         if not isinstance(rules, NetworkAnalysisRules):
-            raise TypeError(
-                f"'rules' should be of type NetworkAnalysisRules. Got {type(rules)}"
-            )
+            rules = NetworkAnalysisRules(**rules)
 
         if not isinstance(network, Network):
-            raise TypeError(
-                "'network' should of type DirectedNetwork or Network. "
-                f"Got {type(network)}"
-            )
+            network = Network(network)
 
-        self.network.gdf = self.rules._validate_weight(self.network.gdf)
+        self.network = network
+        self.rules = rules.copy()
+        self._log = log
+        self.detailed_log = detailed_log
 
         self._check_if_holes_are_nan()
 
-        if isinstance(self.network, DirectedNetwork):
-            self.network._warn_if_undirected()
+        self.network.gdf = self.rules._validate_weight(self.network.gdf)
 
         self._update_wkts()
         self.rules._update_rules()
 
         if log:
             self.log = DataFrame()
 
@@ -143,21 +127,16 @@
 
     def _check_if_holes_are_nan(self):
         HOLES_ARE_NAN = (
             "Network holes have been filled by straigt lines, but the rows have "
             f"NaN values in the {self.rules.weight!r} column. Either remove NaNs "
             "or fill these values with a numeric value (e.g. 0)."
         )
-        if hasattr(self.network, "_hole_col") and all(
-            self.network.gdf[self.rules.weight].isna()
-        ):
-            raise ValueError(HOLES_ARE_NAN)
-
         if hasattr(self.network.gdf, "hole") and all(
-            self.network.gdf[self.rules.weight].isna()
+            self.network.gdf[self.network.gdf["hole"] == 1, self.rules.weight].isna()
         ):
             raise ValueError(HOLES_ARE_NAN)
 
     def od_cost_matrix(
         self,
         origins: GeoDataFrame,
         destinations: GeoDataFrame,
@@ -188,17 +167,17 @@
 
         Examples
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
-        >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
-        >>> rules = sg.NetworkAnalysisRules(weight="minutes")
-        >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
+        >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+        >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
+        >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
 
         Create some origin and destination points.
 
         >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
         >>> origins = points.loc[:99, ["geometry"]]
         >>> origins
                                   geometry
@@ -366,18 +345,20 @@
 
         """
         if self._log:
             time_ = perf_counter()
 
         self._prepare_network_analysis(origins, destinations, rowwise)
 
+        ori = self.origins.gdf.set_index("temp_idx")
+        des = self.destinations.gdf.set_index("temp_idx")
         results = _od_cost_matrix(
             graph=self.graph,
-            origins=self.origins.gdf,
-            destinations=self.destinations.gdf,
+            origins=ori,
+            destinations=des,
             weight=self.rules.weight,
             lines=lines,
             rowwise=rowwise,
         )
 
         results["origin"] = results["origin"].map(self.origins.idx_dict)
         results["destination"] = results["destination"].map(self.destinations.idx_dict)
@@ -447,17 +428,17 @@
         Examples
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> import pandas as pd
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
-        >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
-        >>> rules = sg.NetworkAnalysisRules(weight="minutes")
-        >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
+        >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+        >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
+        >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
 
         Get some points.
 
         >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
         >>> origins = points.iloc[:25]
         >>> destinations = points.iloc[25:50]
 
@@ -639,17 +620,17 @@
 
         Examples
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
-        >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
-        >>> rules = sg.NetworkAnalysisRules(weight="minutes")
-        >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
+        >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+        >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
+        >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
 
         Get routes from 1 to 1000 points.
 
         >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 
         >>> routes = nwa.get_route(points.iloc[[0]], points)
         >>> routes
@@ -750,17 +731,17 @@
 
         Examples
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> roads = sg.read_parquet_url('https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet')
-        >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
-        >>> rules = sg.NetworkAnalysisRules(weight='minutes')
-        >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
+        >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+        >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
+        >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
 
         Getting 10 fastest routes from one point to another point.
 
         >>> points = sg.read_parquet_url('https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet')
         >>> point1 = points.iloc[[0]]
         >>> point2 = points.iloc[[1]]
 
@@ -888,17 +869,17 @@
 
         Examples
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
-        >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
-        >>> rules = sg.NetworkAnalysisRules(weight="minutes")
-        >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
+        >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+        >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
+        >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
 
         10 minute service area for three origin points.
 
         >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
         >>> service_areas = nwa.service_area(
         ...         points.loc[:2],
         ...         breaks=10,
@@ -936,15 +917,15 @@
         results = _service_area(
             graph=self.graph,
             origins=self.origins.gdf,
             breaks=breaks,
             weight=self.rules.weight,
             lines=self.network.gdf,
             nodes=self.network.nodes,
-            directed=self.network._as_directed,
+            directed=self.rules.directed,
             precice=False,
         )
 
         if not all(results.geometry.isna()):
             results = results.drop_duplicates(["src_tgt_wt", "origin"])
 
             if dissolve:
@@ -1016,17 +997,17 @@
 
         Examples
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
-        >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
-        >>> rules = sg.NetworkAnalysisRules(weight="minutes")
-        >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
+        >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+        >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
+        >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
 
         10 minute service area for one origin point.
 
         >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 
         >>> sa = nwa.precice_service_area(
         ...         points.iloc[[0]],
@@ -1063,15 +1044,15 @@
         results = _service_area(
             graph=self.graph,
             origins=self.origins.gdf,
             breaks=breaks,
             weight=self.rules.weight,
             lines=self.network.gdf,
             nodes=self.network.nodes,
-            directed=self.network._as_directed,
+            directed=self.rules.directed,
             precice=True,
         )
 
         if not all(results.geometry.isna()):
             results = results.drop_duplicates(["src_tgt_wt", "origin"])
 
             if dissolve:
@@ -1197,33 +1178,26 @@
 
         Args:
             method: the name of the network analysis method used
             minutes_elapsed: time use of the method
 
         Returns:
             A one-row DataFrame with log info columns
-
-        Note:
-            The 'isolated_removed' column does not account for
-            preperation done before initialising the (Directed)Network class.
         """
         data = {
             "endtime": pd.to_datetime(datetime.now()).floor("S").to_pydatetime(),
             "minutes_elapsed": minutes_elapsed,
             "method": method,
             "origins_count": np.nan,
             "destinations_count": np.nan,
             "percent_missing": np.nan,
             "cost_mean": np.nan,
         }
-        if self.detailed_log:
-            data = data | {
-                "isolated_removed": self.network._isolated_removed,
-                "percent_bidirectional": self.network.percent_bidirectional,
-            }
+        if self.rules.directed:
+            data["percent_bidirectional"] = self.network.percent_bidirectional
 
         df = DataFrame(data, index=[0])
 
         if not self.detailed_log:
             return df
 
         for key, value in self.rules.__dict__.items():
@@ -1306,15 +1280,15 @@
 
             edges, weights, ids = self._get_edges_and_weights()
 
             self.graph = self._make_graph(
                 edges=edges,
                 weights=weights,
                 edge_ids=ids,
-                directed=self.network._as_directed,
+                directed=self.rules.directed,
             )
 
             self._add_missing_vertices()
 
             self._graph_updated_count += 1
 
         self._update_wkts()
@@ -1381,15 +1355,15 @@
 
         self.network.gdf["meters_"] = self.network.gdf.length
 
         # create an id from before the split, used to revert the split later
         self.network.gdf["temp_idx__"] = range(len(self.network.gdf))
 
         lines = split_lines_by_nearest_point(
-            lines=self.network.gdf,
+            gdf=self.network.gdf,
             points=points,
             max_distance=self.rules.search_tolerance,
         )
 
         # save the unsplit lines for later
         splitted = lines.loc[lines["splitted"] == 1, "temp_idx__"]
         self.network._not_splitted = self.network.gdf.loc[
@@ -1535,14 +1509,15 @@
         )
 
     def __repr__(self) -> str:
         """The print representation."""
         # drop the 'weight_to_nodes_' parameters in the repr of rules to avoid clutter
         rules = (
             f"{self.rules.__class__.__name__}(weight={self.rules.weight}, "
+            f"directed={self.rules.directed}, "
             f"search_tolerance={self.rules.search_tolerance}, "
             f"search_factor={self.rules.search_factor}, "
             f"split_lines={self.rules.split_lines}, "
         )
 
         # add one 'weight_to_nodes_' parameter if used,
         # else inform that there are more parameters with '...'
@@ -1561,13 +1536,17 @@
             "\n)"
         )
 
     def __getitem__(self, item):
         """To be able to write self['origins'] as well as self.origins."""
         return getattr(self, item)
 
-    def copy(self):
-        """Returns a shallow copy of the class instance."""
-        return copy(self)
+    def copy(self, deep=True):
+        """Returns a (deep) copy of the class instance.
 
-    def deepcopy(self):
-        return deepcopy(self)
+        Args:
+            deep: Whether to return a deep or shallow copy. Defaults to True.
+        """
+        if deep:
+            return deepcopy(self)
+        else:
+            return copy(self)
```

### Comparing `ssb_sgis-0.1.8/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.1.9/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """The NetworkAnalysisRules class sets the rules for the network analysis.
 
 The class is to be used as the 'rules' parameter in the NetworkAnalysis
 class.
 """
 import warnings
+from copy import copy, deepcopy
 from dataclasses import dataclass
 
 from geopandas import GeoDataFrame
 
 from ..helpers import unit_is_meters
 
 
@@ -17,14 +18,15 @@
 
     To be used as the 'rules' parameter in the NetworkAnalysis class.
 
     Args:
         weight: Either a column in the GeoDataFrame of the Network or
             'meters'/'metres'. A 'minutes' column can be created with the
             'make_directed_network' method of the DirectedNetwork class.
+        directed: Whether the lines will be considered traversable in both directions.
         search_tolerance: distance to search for nodes in the network. Origins and
             destinations further away from the network than the search_tolerance will
             not find any paths. Defaults to 250.
         search_factor: number of meters and percent to add to the closest distance to a
             node when connecting origins and destinations to the network. Defaults to
             0, meaning only the closest node is used. If search_factor is 10 and the
             closest node is 1 meter away, paths will be created from the point and all
@@ -42,38 +44,28 @@
             that connect them. Defaults to None, meaning 0 weight is added for the
             edges.
         nodedist_multiplier: When using "meters" as weight, this sets the weight for
             the edges between origins/destinations and the network nodes that connect
             them. Defaults to None, meaning 0 weight is added for these edges. If set
             to 1, the weight will be equal to the straigt line distance.
 
-    Note:
-        Whether the network analysis will be directed or undirected is not stored here,
-        although it can be considered a 'rule'. Whether to do directed network
-        analysis, depends on the network. So if the graph is made directed or not, is
-        decided by which network class you use, DirectedNetwork to make a directed
-        graph and the base Network class to make an undirected graph.
-
     Examples
     --------
     Read testdata.
 
     >>> import sgis as sg
     >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
     >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 
-    Let's start by setting the default rules. 'weight' is the only parameter with no
-    default.
+    Let's start by setting the default rules. 'weight' and 'directed' has noe default
+    values.
 
-    >>> nw = (sg.DirectedNetwork(roads)
-    ...       .remove_isolated()
-    ...       .make_directed_network_norway()
-    ... )
-    >>> rules = sg.NetworkAnalysisRules(weight="minutes")
-    >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules)
+    >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
+    >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
+    >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
     >>> nwa
     NetworkAnalysis(
         network=DirectedNetwork(6364 km, percent_bidirectional=87),
         rules=NetworkAnalysisRules(weight=minutes, search_tolerance=250, search_factor=0, split_lines=False, ...),
         log=True, detailed_log=True,
     )
 
@@ -157,51 +149,55 @@
     If the weight is 'meters', setting nodedist_multiplier=1 will make the distance
     to nodes count as its straight line distance.
 
     >>> rules = NetworkAnalysisRules(
     ...     weight="meters",
     ...     search_tolerance=5000,
     ... )
-    >>> nwa = NetworkAnalysis(network=nw, rules=rules)
+    >>> nwa = NetworkAnalysis(network=directed_roads, rules=rules)
     >>> od = nwa.od_cost_matrix(points, points)
     >>> nwa.rules.nodedist_multiplier = 1
     >>> od = nwa.od_cost_matrix(points, points)
 
     >>> nwa.log[['nodedist_multiplier', 'cost_mean']]
       nodedist_multiplier     cost_mean
     0                None  10228.400228
     1                   1  10277.926186
     """
 
+    directed: bool
     weight: str
     search_tolerance: int = 250
     search_factor: int = 0
     split_lines: bool = False
     nodedist_multiplier: int | float | None = None
     nodedist_kmh: int | float | None = None
 
     def _update_rules(self):
         """Stores the rules as separate attributes.
 
         Used for checking whether the rules have changed and the graph have to be
         remade.
         """
+        self._directed = self.directed
         self._weight = self.weight
         self._search_tolerance = self.search_tolerance
         self._search_factor = self.search_factor
         self._split_lines = self.split_lines
         self._nodedist_multiplier = self.nodedist_multiplier
         self._nodedist_kmh = self.nodedist_kmh
 
     def _rules_have_changed(self):
         """Checks if any of the rules have changed since the graph was last created.
 
         If no rules have changed, time can be saved by not remaking the graph
         (the network and the points have to be unchanged as well).
         """
+        if self.directed != self._directed:
+            return True
         if self.weight != self._weight:
             return True
         if self.search_factor != self._search_factor:
             return True
         if self.search_tolerance != self._search_tolerance:
             return True
         if self.split_lines != self._split_lines:
@@ -228,20 +224,20 @@
                 )
             self.weight = "minutes"
             gdf["minutes"] = gdf[self.weight]
             return gdf
 
         elif self.weight in gdf.columns:
             gdf[self.weight] = gdf[self.weight].astype(float)
-            gdf = self._check_for_nans(gdf, self.weight)
-            gdf = self._check_for_negative_values(gdf, self.weight)
+            self._check_for_nans(gdf, self.weight)
+            self._check_for_negative_values(gdf, self.weight)
             gdf = self._try_to_float(gdf, self.weight)
             return gdf
 
-        # at this point, the weight is wrong. Now to determine the error/warning
+        # at this point, the weight is wrong. Now to determine the error
         # message
 
         if "meter" in self.weight or "metre" in self.weight:
             raise ValueError(
                 "the crs of the roads have to have units in 'meters' when the "
                 "weight is 'meters'."
             )
@@ -262,41 +258,38 @@
     def _check_for_nans(df, col):
         """Remove NaNs and give warning if there are any."""
         if all(df[col].isna()):
             raise ValueError(f"All values in the {col!r} column are NaN.")
 
         nans = sum(df[col].isna())
         if nans:
-            warnings.warn(
-                f"Warning: {nans} rows have missing values in the {col!r} column. "
-                "Removing these rows.",
-                stacklevel=2,
+            raise ValueError(
+                f"{nans} rows have missing values in the {col!r} column. "
+                "Fill these rows with 0 or another number.",
             )
-            df = df.loc[df[col].notna()]
-
-        return df
 
     @staticmethod
     def _check_for_negative_values(df, col):
         """Remove negative values and give warning if there are any."""
         negative = sum(df[col] < 0)
         if negative:
-            warnings.warn(
-                f"Warning: {negative} rows have a 'col' less than 0. Removing these "
-                "rows.",
-                stacklevel=2,
+            raise ValueError(
+                f": {negative} rows have {col!r} less than 0. Removing these " "rows.",
             )
-            df = df.loc[df[col] >= 0]
-
-        return df
 
     @staticmethod
     def _try_to_float(df, col):
         """Try to convert weight column to float, raise ValueError if it fails."""
         try:
             df[col] = df[col].astype(float)
         except ValueError as e:
             raise ValueError(
                 f"The {col!r} column must be numeric. Got characters that couldn't be "
                 "interpreted as numbers."
             ) from e
         return df
+
+    def copy(self):
+        return copy(self)
+
+    def deepcopy(self):
+        return deepcopy(self)
```

### Comparing `ssb_sgis-0.1.8/src/sgis/read_parquet.py` & `ssb_sgis-0.1.9/src/sgis/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.8/PKG-INFO` & `ssb_sgis-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.1.8
+Version: 0.1.9
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -53,15 +53,15 @@
 [python version]: https://pypi.org/project/ssb-sgis
 [read the docs]: https://ssb-sgis.readthedocs.io/
 [tests]: https://github.com/statisticsnorway/ssb-sgis/actions?workflow=Tests
 [coverage]: https://sonarcloud.io/component_measures?metric=coverage&id=statisticsnorway_ssb-sgis
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
-sgis builds on the geopandas package and provides functions that make it easier to do advanced GIS in python.
+sgis builds on the geopandas package and provides functions that make it easier to do GIS in python.
 Features include network analysis, functions for exploring multiple GeoDataFrames in a layered interactive map,
 and vector operations like finding k-nearest neighbours, splitting lines by points, snapping and closing holes
 in polygons by size.
 
 ## Network analysis examples
 
 Preparing for network analysis:
@@ -70,34 +70,33 @@
 import sgis as sg
 import pandas as pd
 
 roads = sg.read_parquet_url(
     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet"
 )
 
-nw = (
-    sg.DirectedNetwork(roads)
-    .remove_isolated()
-    .make_directed_network(
-        direction_col="oneway",
-        direction_vals_bft=("B", "FT", "TF"),
-        minute_cols=("drivetime_fw", "drivetime_bw"),
-    )
+connected_roads = sg.get_connected_components(roads).query("connected == 1")
+
+directed_roads = sg.make_directed_network(
+    connected_roads,
+    direction_col="oneway",
+    direction_vals_bft=("B", "FT", "TF"),
+    minute_cols=("drivetime_fw", "drivetime_bw"),
 )
 
-rules = sg.NetworkAnalysisRules(weight="minutes")
+rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
 
-nwa = sg.NetworkAnalysis(network=nw, rules=rules)
+nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules)
 
 nwa
 ```
 
     NetworkAnalysis(
         network=DirectedNetwork(6364 km, percent_bidirectional=87),
-        rules=NetworkAnalysisRules(weight=minutes, search_tolerance=250, search_factor=0, split_lines=False, ...),
+        rules=NetworkAnalysisRules(weight=minutes, directed=True, search_tolerance=250, search_factor=0, split_lines=False, ...),
         log=True, detailed_log=True,
     )
 
 Get number of times each line segment was visited, with optional weighting.
 
 ```python
 origins = points.iloc[:75]
```

