# Comparing `tmp/bassmap-0.0.9.tar.gz` & `tmp/bassmap-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bassmap-0.0.9.tar", last modified: Wed Apr 26 05:09:05 2023, max compression
+gzip compressed data, was "bassmap-0.1.0.tar", last modified: Thu May 11 05:13:03 2023, max compression
```

## Comparing `bassmap-0.0.9.tar` & `bassmap-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:05.322196 bassmap-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-26 05:08:52.000000 bassmap-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 05:08:52.000000 bassmap-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-26 05:09:05.322196 bassmap-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 05:08:52.000000 bassmap-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:05.322196 bassmap-0.0.9/bassmap/
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-26 05:08:52.000000 bassmap-0.0.9/bassmap/Foliumatic.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-26 05:08:52.000000 bassmap-0.0.9/bassmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-04-26 05:08:52.000000 bassmap-0.0.9/bassmap/bassmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:05.322196 bassmap-0.0.9/bassmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-26 05:09:05.000000 bassmap-0.0.9/bassmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 05:09:05.000000 bassmap-0.0.9/bassmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-26 05:09:05.000000 bassmap-0.0.9/bassmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:09:05.000000 bassmap-0.0.9/bassmap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-26 05:09:05.000000 bassmap-0.0.9/bassmap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 05:09:05.000000 bassmap-0.0.9/bassmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-26 05:08:52.000000 bassmap-0.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 05:09:05.322196 bassmap-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-26 05:08:52.000000 bassmap-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:03.267306 bassmap-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-11 05:12:52.000000 bassmap-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 05:12:52.000000 bassmap-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-11 05:13:03.267306 bassmap-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-11 05:12:52.000000 bassmap-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:03.267306 bassmap-0.1.0/bassmap/
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-11 05:12:52.000000 bassmap-0.1.0/bassmap/Foliumatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-11 05:12:52.000000 bassmap-0.1.0/bassmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28693 2023-05-11 05:12:52.000000 bassmap-0.1.0/bassmap/bassmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:13:03.267306 bassmap-0.1.0/bassmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-11 05:13:03.000000 bassmap-0.1.0/bassmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-11 05:13:03.000000 bassmap-0.1.0/bassmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 05:13:03.000000 bassmap-0.1.0/bassmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:13:03.000000 bassmap-0.1.0/bassmap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 05:13:03.000000 bassmap-0.1.0/bassmap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 05:13:03.000000 bassmap-0.1.0/bassmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 05:12:53.000000 bassmap-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-11 05:13:03.267306 bassmap-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-11 05:12:53.000000 bassmap-0.1.0/setup.py
```

### Comparing `bassmap-0.0.9/LICENSE` & `bassmap-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bassmap-0.0.9/bassmap/Foliumatic.py` & `bassmap-0.1.0/bassmap/Foliumatic.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,66 +2,66 @@
 import zipfile
 import io
 import os
 import json
 import folium
 import geopandas as gpd
 
+import folium
+
 class Foliumatic(folium.Map):
     
     def __init__(self):
         self.map = folium.Map()
         
     def __init__(self, lat=0, lon=0, zoom_start=2):
         self.map = folium.Map(location=[lat, lon], zoom_start=zoom_start)
 
-    def add_tile_layer(self, url, name, attribution = "", **kwargs):
-        """Adds a tile layer to the map.
-        
-        Args:
-            url (str): The URL of the tile layer.
-            name (str): The name of the tile layer
-            attribution (str, optional): The attribution of the tile layer. Defaults to **
-            """
-        tile_layer = folium.TileLayer(
-            tiles= url,
-            name = name,
-            attr = attribution,
-            **kwargs
-        )
-        self.add_child(tile_layer)
+    def add_tile_layers(self, tile_layers):
+        for tile_name, tile_url in tile_layers.items():
+            folium.TileLayer(tiles=tile_url, name=tile_name).add_to(self.map)
+
+        folium.LayerControl().add_to(self.map)
+
+        return self.map
 
-    def add_basemap(self, basemap_name, url_template):
+    def add_basemap(self, basemap_name):
         """
-        Adds a basemap to the map using a URL template.
+        Adds a basemap to the map using a predefined URL template for XYZ tile services.
         
         Parameters:
         basemap_name (str): The name of the basemap to add.
-        url_template (str): The URL template to use for the new basemap layer. Must be 
-            a valid XYZ tile service.
         """
+        basemap_urls = {
+            'OpenStreetMap': 'https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png',
+            'Mapbox Satellite': 'https://api.mapbox.com/styles/v1/mapbox/satellite-v9/tiles/{z}/{x}/{y}?access_token=<your-access-token>',
+            'Esri.WorldImagery': 'https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}',
+            'OpenTopoMap': 'https://{s}.tile.opentopomap.org/{z}/{x}/{y}.png',
+            'Esri.NatGeoWorldMap': 'https://server.arcgisonline.com/ArcGIS/rest/services/NatGeo_World_Map/MapServer/tile/{z}/{y}/{x}',
+            'CartoDB.Positron': 'https://{s}.basemaps.cartocdn.com/light_all/{z}/{x}/{y}.png',
+        }
+        
+        url_template = basemap_urls.get(basemap_name)
+        
+        if url_template is None:
+            raise ValueError(f'Unknown basemap name: {basemap_name}')
+        
         new_layer = folium.TileLayer(
             tiles=url_template,
             name=basemap_name,
             attr=' '.join([basemap_name, 'Map data &copy; <a href="https://openstreetmap.org">OpenStreetMap</a> contributors']),
             overlay=True,
             control=True
         )
         self.add_child(new_layer)
 
-    def add_shp(self, data, name='Shapefile', **kwargs):
-        """Adds a Shapefile layer to the map.
-        
-        Args:
-            data (str): the path to the Shapefile.
-        """
-        import geopandas as gpd
+    def add_shp(self, data, **kwargs):
         gdf = gpd.read_file(data)
         geojson = gdf.__geo_interface__
-        self.add_geojson(geojson, name=name, **kwargs)
+        self.add_geojson(geojson, **kwargs)
 
     def add_geojson(self, geojson_data):
         """
         Adds a GeoJSON layer to the map.
         
         Parameters:
         geojson_data (str or dict): The GeoJSON file path, HTTP URL or dictionary to add to the map.
```

### Comparing `bassmap-0.0.9/setup.py` & `bassmap-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='bassmap',
     name='bassmap',
     packages=find_packages(include=['bassmap', 'bassmap.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/bassneel/bassmap',
-    version='0.0.9',
+    version='0.1.0',
     zip_safe=False,
 )
```

