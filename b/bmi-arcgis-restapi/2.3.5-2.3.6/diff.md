# Comparing `tmp/bmi-arcgis-restapi-2.3.5.tar.gz` & `tmp/bmi-arcgis-restapi-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmi-arcgis-restapi-2.3.5.tar", last modified: Tue Apr  4 20:07:17 2023, max compression
+gzip compressed data, was "bmi-arcgis-restapi-2.3.6.tar", last modified: Thu May 11 21:16:40 2023, max compression
```

## Comparing `bmi-arcgis-restapi-2.3.5.tar` & `bmi-arcgis-restapi-2.3.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.983977 bmi-arcgis-restapi-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    43529 2023-04-04 20:07:17.987977 bmi-arcgis-restapi-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    43756 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.975977 bmi-arcgis-restapi-2.3.5/bmi_arcgis_restapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43529 2023-04-04 20:07:17.000000 bmi-arcgis-restapi-2.3.5/bmi_arcgis_restapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-04 20:07:17.000000 bmi-arcgis-restapi-2.3.5/bmi_arcgis_restapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 20:07:17.000000 bmi-arcgis-restapi-2.3.5/bmi_arcgis_restapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-04 20:07:17.000000 bmi-arcgis-restapi-2.3.5/bmi_arcgis_restapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 20:07:17.000000 bmi-arcgis-restapi-2.3.5/bmi_arcgis_restapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.975977 bmi-arcgis-restapi-2.3.5/restapi/
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/_strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.975977 bmi-arcgis-restapi-2.3.5/restapi/admin/
--rw-r--r--   0 runner    (1001) docker     (123)   127751 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.975977 bmi-arcgis-restapi-2.3.5/restapi/admin/samples/
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/admin/samples/admin_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/admin/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28063 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/arc_restapi.py
--rw-r--r--   0 runner    (1001) docker     (123)   166239 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.975977 bmi-arcgis-restapi-2.3.5/restapi/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)    16306 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.975977 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.975977 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/css/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/css/app.615af0e5.css
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/css/chunk-26ed89da.8fb689c1.css
--rw-r--r--   0 runner    (1001) docker     (123)   219149 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/css/chunk-vendors.64d43e69.css
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.971977 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.979977 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    29808 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/android-chrome-maskable-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/android-chrome-maskable-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/apple-touch-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/apple-touch-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/msapplication-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.979977 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/js/
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/js/app.dbaf9f92.js
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/js/chunk-26ed89da.db4a4cda.js
--rw-r--r--   0 runner    (1001) docker     (123)   347124 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/js/chunk-vendors.20697101.js
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/precache-manifest.b62ded22fc8a9700861c815d7e20acbd.js
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/service-worker.js
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20762 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/open_restapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.979977 bmi-arcgis-restapi-2.3.5/restapi/projections/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/projections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.983977 bmi-arcgis-restapi-2.3.5/restapi/projections/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   964212 2023-04-04 20:07:07.000000 bmi-arcgis-restapi-2.3.5/restapi/projections/bin/gtf.json
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-04 20:07:08.000000 bmi-arcgis-restapi-2.3.5/restapi/projections/bin/linearUnits.json
--rw-r--r--   0 runner    (1001) docker     (123)   188627 2023-04-04 20:07:08.000000 bmi-arcgis-restapi-2.3.5/restapi/projections/bin/projection_names.json
--rw-r--r--   0 runner    (1001) docker     (123)  2060997 2023-04-04 20:07:08.000000 bmi-arcgis-restapi-2.3.5/restapi/projections/bin/projection_strings.json
--rw-r--r--   0 runner    (1001) docker     (123)  2269080 2023-04-04 20:07:08.000000 bmi-arcgis-restapi-2.3.5/restapi/projections/bin/projections.json
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-04 20:07:08.000000 bmi-arcgis-restapi-2.3.5/restapi/rest_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    75045 2023-04-04 20:07:08.000000 bmi-arcgis-restapi-2.3.5/restapi/shapefile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:07:17.983977 bmi-arcgis-restapi-2.3.5/restapi/shp_helper/
--rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-04-04 20:07:08.000000 bmi-arcgis-restapi-2.3.5/restapi/shp_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-04 20:07:17.987977 bmi-arcgis-restapi-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-04 20:07:08.000000 bmi-arcgis-restapi-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.118745 bmi-arcgis-restapi-2.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-05-11 21:16:26.000000 bmi-arcgis-restapi-2.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-11 21:16:26.000000 bmi-arcgis-restapi-2.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    43529 2023-05-11 21:16:40.118745 bmi-arcgis-restapi-2.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43756 2023-05-11 21:16:26.000000 bmi-arcgis-restapi-2.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.106745 bmi-arcgis-restapi-2.3.6/bmi_arcgis_restapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43529 2023-05-11 21:16:40.000000 bmi-arcgis-restapi-2.3.6/bmi_arcgis_restapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-11 21:16:40.000000 bmi-arcgis-restapi-2.3.6/bmi_arcgis_restapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:16:40.000000 bmi-arcgis-restapi-2.3.6/bmi_arcgis_restapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 21:16:40.000000 bmi-arcgis-restapi-2.3.6/bmi_arcgis_restapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 21:16:40.000000 bmi-arcgis-restapi-2.3.6/bmi_arcgis_restapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.110745 bmi-arcgis-restapi-2.3.6/restapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/_strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.110745 bmi-arcgis-restapi-2.3.6/restapi/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)   129567 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.110745 bmi-arcgis-restapi-2.3.6/restapi/admin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/admin/samples/admin_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/admin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28063 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/arc_restapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166239 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.110745 bmi-arcgis-restapi-2.3.6/restapi/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)    16306 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.110745 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.110745 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/css/app.615af0e5.css
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/css/chunk-26ed89da.8fb689c1.css
+-rw-r--r--   0 runner    (1001) docker     (123)   219149 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/css/chunk-vendors.64d43e69.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.106745 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.114745 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29808 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/android-chrome-maskable-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/android-chrome-maskable-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/apple-touch-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/apple-touch-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/msapplication-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.114745 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/js/app.dbaf9f92.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/js/chunk-26ed89da.db4a4cda.js
+-rw-r--r--   0 runner    (1001) docker     (123)   347124 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/js/chunk-vendors.20697101.js
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/precache-manifest.b62ded22fc8a9700861c815d7e20acbd.js
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/service-worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20762 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/open_restapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.114745 bmi-arcgis-restapi-2.3.6/restapi/projections/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/projections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.118745 bmi-arcgis-restapi-2.3.6/restapi/projections/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   964212 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/projections/bin/gtf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/projections/bin/linearUnits.json
+-rw-r--r--   0 runner    (1001) docker     (123)   188627 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/projections/bin/projection_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)  2060997 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/projections/bin/projection_strings.json
+-rw-r--r--   0 runner    (1001) docker     (123)  2269080 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/projections/bin/projections.json
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/rest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75045 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/shapefile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:16:40.118745 bmi-arcgis-restapi-2.3.6/restapi/shp_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/restapi/shp_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 21:16:40.118745 bmi-arcgis-restapi-2.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-11 21:16:27.000000 bmi-arcgis-restapi-2.3.6/setup.py
```

### Comparing `bmi-arcgis-restapi-2.3.5/LICENSE` & `bmi-arcgis-restapi-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/PKG-INFO` & `bmi-arcgis-restapi-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmi-arcgis-restapi
-Version: 2.3.5
+Version: 2.3.6
 Summary: Package for working with ArcGIS REST API
 Home-page: https://github.com/Bolton-and-Menk-GIS/restapi
 Author: Caleb Mackey
 Author-email: calebma@bolton-menk.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `bmi-arcgis-restapi-2.3.5/README.md` & `bmi-arcgis-restapi-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/bmi_arcgis_restapi.egg-info/PKG-INFO` & `bmi-arcgis-restapi-2.3.6/bmi_arcgis_restapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmi-arcgis-restapi
-Version: 2.3.5
+Version: 2.3.6
 Summary: Package for working with ArcGIS REST API
 Home-page: https://github.com/Bolton-and-Menk-GIS/restapi
 Author: Caleb Mackey
 Author-email: calebma@bolton-menk.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `bmi-arcgis-restapi-2.3.5/bmi_arcgis_restapi.egg-info/SOURCES.txt` & `bmi-arcgis-restapi-2.3.6/bmi_arcgis_restapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/__init__.py` & `bmi-arcgis-restapi-2.3.6/restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/_strings.py` & `bmi-arcgis-restapi-2.3.6/restapi/_strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,15 @@
 
 FIELD_KEYS_CREATE = [NAME, ALIAS, TYPE, DOMAIN, LENGTH]
 
 GEOM_CODE = {v:k for k,v in six.iteritems(GEOM_DICT)}
 BASE_PATTERN = 'http*://*/rest/services*'
 PORTAL_BASE_PATTERN = 'http*://*/sharing/rest*'
 PORTAL_SERVICES_PATTERN = 'http*://*/sharing/servers/*/rest/services/*'
-VERSION = '2.3.5'
+VERSION = '2.3.6'
 PACKAGE_NAME = 'restapi'
 USER_AGENT = '{}/{} (Python)'.format(PACKAGE_NAME, VERSION)
 GET = 'GET'
 POST = 'POST'
 
 PROTOCOL = ''
```

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/admin/__init__.py` & `bmi-arcgis-restapi-2.3.6/restapi/admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Use with caution!
 from __future__ import print_function
 import sys
 import os
 import fnmatch
 import datetime
 import json
+import time
 from collections import namedtuple
 from ..exceptions import RequestError
 from ..rest_utils import Token, mil_to_date, date_to_mil, IdentityManager, JsonGetter, \
     generate_token, ID_MANAGER, do_request, SpatialReferenceMixin, parse_url, get_portal_base, requestClient, \
     get_request_method, get_request_client, TokenExpired
 from ..decorator import decorator
 import munch
@@ -21,14 +22,15 @@
 from six.moves import reload_module
 from six.moves import urllib
 
 # Globals
 BASE_PATTERN = '*:*/arcgis/*admin*'
 AGOL_ADMIN_BASE_PATTERN = 'http*://*/rest/admin/services*'
 VERBOSE = True
+ASYNC_TIMEOUT = 300
 
 # VERBOSE is set to true by default, this will echo the status of all operations
 #  i.e. reporting an administrative change was successful.  To turn this off, simply
 #  change VERBOSE to False.  This can be done like this:
 #    VERBOSE = False #because you get this with importing the admin module
 #  or:
 #    restapi.admin.VERBOSE = False
@@ -3229,83 +3231,117 @@
         Returns:
             The edited input JSON.
         """
         if EDITING_INFO in in_json:
             in_json[EDITING_INFO][LAST_EDIT_DATE] = ''
         return in_json
 
+    def waitForAsync(self, jobUrl):
+        """helper to wait for an async operation to complete.
+
+        Args:
+            jobUrl (str): the job status URL returned by the async request
+
+        Raises:
+            RequestError: error response from job status endpoint
+            RequestError: Async operation took too long
+
+        """
+        count = 0
+        response = self.request(jobUrl)
+        while response.status != 'Completed':
+            response = self.request(jobUrl)
+            if response.status == 'Failed':
+                raise RequestError({'error': response})
+            if count >= ASYNC_TIMEOUT:
+                raise RequestError({'error': 'Async operation took too long'})
+            count += 1
+            time.sleep(1)
+        return response
+
+
     @passthrough
-    def addToDefinition(self, addToDefinition, runAsync=FALSE):
+    def addToDefinition(self, addToDefinition, runAsync=FALSE, wait=True):
         """Adds a definition property in a feature layer.
 
         Args:
             addToDefinition: The service update to the layer definition property
                 for a feature service layer.
             runAsync: Optional boolean to run this process asynchronously.
                 Default is FALSE.
+            wait: Optional boolean, honored only when runAsync=true. Determines whether to initiate the
+                async process and wait for it to finish, or return immediately.
         """
 
         self.clearLastEditedDate(addToDefinition)
         url = '/'.join([self.url, ADD_TO_DEFINITION])
 
         params = {
             F: JSON,
             ADD_TO_DEFINITION: addToDefinition,
-            # ASYNC: runAsync
+            ASYNC: runAsync
         }
 
         result = self.request(url, params, method='post')
+        if runAsync and wait:
+            result = self.waitForAsync(result.statusURL)
         self.refresh()
         self.reload()
         return result
 
     @passthrough
-    def deleteFromDefinition(self, deleteFromDefinition, runAsync=FALSE):
+    def deleteFromDefinition(self, deleteFromDefinition, runAsync=FALSE, wait=True):
         """Deletes a definition property in a feature layer.
 
         Args:
             deleteFromDefinition: The service update to the layer definition property
                 for a feature service layer.
             runAsync: Optional boolean to run this process asynchronously.
                 Defaults to FALSE.
+            wait: Optional boolean, honored only when runAsync=true. Determines whether to initiate the
+                async process and wait for it to finish, or return immediately.
         """
 
         self.clearLastEditedDate(deleteFromDefinition)
         url = '/'.join([self.url, DELETE_FROM_DEFINITION])
         params = {
             F: JSON,
             DELETE_FROM_DEFINITION: deleteFromDefinition,
-            # ASYNC: runAsync
+            ASYNC: runAsync
         }
-
         result = self.request(url, params, method='post')
+        if runAsync and wait:
+            result = self.waitForAsync(result.statusURL)
         self.refresh()
         self.reload()
         return result
 
     @passthrough
-    def updateDefinition(self, updateDefinition, runAsync=FALSE):
+    def updateDefinition(self, updateDefinition, runAsync=FALSE, wait=True):
         """Updates a definition property in a feature layer.
 
         Args:
             updateDefinition: The service update to the layer definition property
                 for a feature service layer.
             runAsync: Optional boolean to run this process asynchronously.
                 Default is FALSE.
+
         """
 
         self.clearLastEditedDate(updateDefinition)
         url = '/'.join([self.url, UPDATE_DEFINITION])
         params = {
             F: JSON,
             UPDATE_DEFINITION: updateDefinition,
-            # ASYNC: runAsync
+            ASYNC: runAsync
         }
 
         result = self.request(url, params, method='post')
+        if runAsync and wait:
+            result = self.waitForAsync(result.statusURL)
         self.refresh()
         self.reload()
         return result
 
     @passthrough
     def enableEditorTracking(self):
         capabilities = self.get(CAPABILITIES, '')
@@ -3468,34 +3504,40 @@
             alias: Optional field name for alias.
             **kwargs: Optional additional field keys to set.
         """
 
         self.addToDefinition({FIELDS: [self.createNewFieldDefinition(name, field_type, alias or name, **kwargs)]})
 
     @passthrough
-    def truncate(self, attachmentOnly=TRUE, runAsync=FALSE):
+    def truncate(self, attachmentOnly=TRUE, runAsync=FALSE, wait=True):
         """Truncates the feature layer by removing all features.
 
         Args:
             attachmentOnly -- Optional boolean to delete all attachments only.
                 Defaults to TRUE.
             runAsync: Optional boolean to run this process asynchronously.
                 Defaults to FALSE.
+            wait: Optional boolean, honored only when runAsync=true. Determines whether to initiate the
+                async process and wait for it to finish, or return immediately.
         """
 
         if not self.json.get(SUPPORTS_TRUNCATE, False):
             raise NotImplementedError('This resource does not support the Truncate method')
 
         url = '/'.join([self.url, TRUNCATE])
         params = {
             ATTACHMENT_ONLY: attachmentOnly,
             ASYNC: runAsync
         }
 
-        return self.request(url, params, method=POST)
+        result = self.request(url, params, method=POST)
+        if runAsync and wait:
+            return self.waitForAsync(result.statusURL)
+        return result
+
 
     def __repr__(self):
         return '<{}: "{}">'.format(self.__class__.__name__, self.name)
 
 class AGOLMapService(AdminRESTEndpoint):
     # TODO
     pass
```

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/admin/samples/admin_samples.py` & `bmi-arcgis-restapi-2.3.6/restapi/admin/samples/admin_samples.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/admin/utils.py` & `bmi-arcgis-restapi-2.3.6/restapi/admin/utils.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/arc_restapi.py` & `bmi-arcgis-restapi-2.3.6/restapi/arc_restapi.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/common_types.py` & `bmi-arcgis-restapi-2.3.6/restapi/common_types.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/conversion.py` & `bmi-arcgis-restapi-2.3.6/restapi/conversion.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/decorator/__init__.py` & `bmi-arcgis-restapi-2.3.6/restapi/decorator/__init__.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/enums.py` & `bmi-arcgis-restapi-2.3.6/restapi/enums.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/exceptions.py` & `bmi-arcgis-restapi-2.3.6/restapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/css/chunk-26ed89da.8fb689c1.css` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/css/chunk-26ed89da.8fb689c1.css`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/css/chunk-vendors.64d43e69.css` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/css/chunk-vendors.64d43e69.css`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/favicon.ico` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/favicon.ico`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/android-chrome-192x192.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/android-chrome-512x512.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/android-chrome-maskable-192x192.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/android-chrome-maskable-192x192.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/android-chrome-maskable-512x512.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/android-chrome-maskable-512x512.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/apple-touch-icon-120x120.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/apple-touch-icon-152x152.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/apple-touch-icon-180x180.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/apple-touch-icon-60x60.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/apple-touch-icon-76x76.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/apple-touch-icon.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/favicon-16x16.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/favicon-32x32.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/msapplication-icon-144x144.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/msapplication-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/img/icons/mstile-150x150.png` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/img/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/index.html` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/index.html`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/js/app.dbaf9f92.js` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/js/app.dbaf9f92.js`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/js/chunk-26ed89da.db4a4cda.js` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/js/chunk-26ed89da.db4a4cda.js`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/js/chunk-vendors.20697101.js` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/js/chunk-vendors.20697101.js`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/manifest.json` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/manifest.json`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/precache-manifest.b62ded22fc8a9700861c815d7e20acbd.js` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/precache-manifest.b62ded22fc8a9700861c815d7e20acbd.js`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/geometry-helper/service-worker.js` & `bmi-arcgis-restapi-2.3.6/restapi/geometry-helper/service-worker.js`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/globals.py` & `bmi-arcgis-restapi-2.3.6/restapi/globals.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/open_restapi.py` & `bmi-arcgis-restapi-2.3.6/restapi/open_restapi.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/projections/__init__.py` & `bmi-arcgis-restapi-2.3.6/restapi/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/projections/bin/gtf.json` & `bmi-arcgis-restapi-2.3.6/restapi/projections/bin/gtf.json`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/projections/bin/linearUnits.json` & `bmi-arcgis-restapi-2.3.6/restapi/projections/bin/linearUnits.json`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/projections/bin/projection_names.json` & `bmi-arcgis-restapi-2.3.6/restapi/projections/bin/projection_names.json`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/projections/bin/projection_strings.json` & `bmi-arcgis-restapi-2.3.6/restapi/projections/bin/projection_strings.json`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/projections/bin/projections.json` & `bmi-arcgis-restapi-2.3.6/restapi/projections/bin/projections.json`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/rest_utils.py` & `bmi-arcgis-restapi-2.3.6/restapi/rest_utils.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/shapefile.py` & `bmi-arcgis-restapi-2.3.6/restapi/shapefile.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/restapi/shp_helper/__init__.py` & `bmi-arcgis-restapi-2.3.6/restapi/shp_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `bmi-arcgis-restapi-2.3.5/setup.py` & `bmi-arcgis-restapi-2.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 name = 'bmi-arcgis-restapi'
 
 setup(name=name,
-      version='2.3.5',
+      version='2.3.6',
       description='Package for working with ArcGIS REST API',
       author='Caleb Mackey',
       author_email='calebma@bolton-menk.com',
       url='https://github.com/Bolton-and-Menk-GIS/restapi',
       license='GPL',
       packages=find_packages(),
       include_package_data=True,
```

